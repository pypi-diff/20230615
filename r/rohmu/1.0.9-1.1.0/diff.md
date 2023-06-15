# Comparing `tmp/rohmu-1.0.9.tar.gz` & `tmp/rohmu-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/rohmu/rohmu/dist/.tmp-8attazkl/rohmu-1.0.9.tar", last modified: Wed Dec  7 13:21:45 2022, max compression
+gzip compressed data, was "rohmu-1.1.0.tar", last modified: Thu Jun 15 10:17:15 2023, max compression
```

## Comparing `rohmu-1.0.9.tar` & `rohmu-1.1.0.tar`

### file list

```diff
@@ -1,60 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:21:45.000000 rohmu-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2022-12-07 13:21:33.000000 rohmu-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2022-12-07 13:21:45.000000 rohmu-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2022-12-07 13:21:33.000000 rohmu-1.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      282 2022-12-07 13:21:33.000000 rohmu-1.0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu/
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/atomic_opener.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/compressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu/delta/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/delta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/delta/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/delta/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14763 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/filewrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/inotify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/notifier/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/notifier/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/notifier/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/notifier/null.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu/object_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/object_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/object_storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/object_storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25486 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/object_storage/google.py
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/object_storage/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    19762 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/object_storage/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/object_storage/sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/object_storage/swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/rohmufile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/snappyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2022-12-07 13:21:33.000000 rohmu-1.0.9/rohmu/zstdfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2022-12-07 13:21:45.000000 rohmu-1.0.9/rohmu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2022-12-07 13:21:45.000000 rohmu-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      219 2022-12-07 13:21:33.000000 rohmu-1.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-07 13:21:45.000000 rohmu-1.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_atomic_opener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_encryptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_object_storage_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_object_storage_google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_object_storage_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_object_storage_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_object_storage_sftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_object_storage_swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_rohmu_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_rohmufile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2022-12-07 13:21:33.000000 rohmu-1.0.9/test/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.029233 rohmu-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-06-15 10:16:58.000000 rohmu-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-15 10:17:15.029233 rohmu-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-15 10:16:58.000000 rohmu-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-15 10:16:58.000000 rohmu-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/atomic_opener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/common/statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/delta/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/delta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/delta/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/delta/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17454 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/filewrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/inotify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/notifier/null.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu/object_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35772 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/object_storage/swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/rohmufile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/snappyfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/transfer_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-15 10:16:58.000000 rohmu-1.1.0/rohmu/zstdfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.025233 rohmu-1.1.0/rohmu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:17:15.000000 rohmu-1.1.0/rohmu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-15 10:17:15.029233 rohmu-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-15 10:16:58.000000 rohmu-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:17:15.029233 rohmu-1.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_atomic_opener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_from_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_inotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_sftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_object_storage_swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_rohmu_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_rohmufile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_transfer_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-15 10:16:58.000000 rohmu-1.1.0/test/test_util.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rohmu-1.0.9/LICENSE` & `rohmu-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rohmu-1.0.9/PKG-INFO` & `rohmu-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: rohmu
-Version: 1.0.9
+Version: 1.1.0
 Summary: "Rohmu is a python library providing an interface to various cloud storage providers."
 Home-page: https://github.com/aiven/rohmu/
 License: Apache 2.0
 Platform: POSIX
 Platform: MacOS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
@@ -39,15 +38,15 @@
 -  Supported compression algorithms: Snappy,
    `zstd <https://github.com/facebook/zstd>`__ and
    `lzma <https://docs.python.org/3/library/lzma.html>`__.
 
 Requirements
 ============
 
-Rohmu requires Python >= 3.7. For Python libary dependencies, have a
+Rohmu requires Python >= 3.8. For Python library dependencies, have a
 look at
 `requirements.txt <https://github.com/aiven/rohmu/blob/main/requirements.txt>`__.
 
 Usage example
 =============
 
 *Add usage example here*
```

### Comparing `rohmu-1.0.9/README.rst` & `rohmu-1.1.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 -  Supported compression algorithms: Snappy,
    `zstd <https://github.com/facebook/zstd>`__ and
    `lzma <https://docs.python.org/3/library/lzma.html>`__.
 
 Requirements
 ============
 
-Rohmu requires Python >= 3.7. For Python libary dependencies, have a
+Rohmu requires Python >= 3.8. For Python library dependencies, have a
 look at
 `requirements.txt <https://github.com/aiven/rohmu/blob/main/requirements.txt>`__.
 
 Usage example
 =============
 
 *Add usage example here*
```

### Comparing `rohmu-1.0.9/rohmu/atomic_opener.py` & `rohmu-1.1.0/rohmu/atomic_opener.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,23 @@
 from contextlib import contextmanager
 from pathlib import Path
-from typing import BinaryIO, Callable, cast, ContextManager, Generator, Optional, overload, TextIO, TYPE_CHECKING, Union
+from typing import BinaryIO, Callable, cast, ContextManager, Generator, Optional, overload, TextIO, Union
+from typing_extensions import TypeAlias
 
-# workaround < Python3.8 missing Literal.
-# if we just use the try/except block, mypy will complain
-# about the fact that Write* variables are being redefined.
-# so we need to pour in an additional branch.
-if TYPE_CHECKING:
+try:
     from typing import Literal
-
-    Write = Literal["w"]
-    WriteBinary = Literal["wb"]
-    WriteTest = Literal["somethingrandomw"]
-else:
-    try:
-        from typing import Literal
-
-        Write = Literal["w"]
-        WriteBinary = Literal["wb"]
-        WriteTest = Literal["somethingrandomw"]
-    except ImportError:
-        from typing import Any
-
-        Write = Any
-        WriteBinary = Any
-        WriteTest = Any
-
+except ImportError:
+    from typing_extensions import Literal  # type: ignore [assignment]
 
 import errno
 import os
 
+Write: TypeAlias = Literal["w"]
+WriteBinary: TypeAlias = Literal["wb"]
+
 
 def _fd_close_quietly(fd: int) -> None:
     try:
         os.close(fd)
     except OSError as e:
         if e.errno == errno.EBADF:
             # closed already
@@ -59,27 +43,14 @@
     encoding: Optional[str] = None,
     _fd_spy: Callable[[int], None] = lambda unused: None,
     _after_link_hook: Callable[[], None] = lambda: None,
 ) -> ContextManager[TextIO]:
     ...
 
 
-if TYPE_CHECKING:
-    # necessary for testing or tests will fail type checking
-    @overload
-    def atomic_opener(
-        final_path: Path,
-        mode: WriteTest,
-        encoding: Optional[str] = None,
-        _fd_spy: Callable[[int], None] = lambda unused: None,
-        _after_link_hook: Callable[[], None] = lambda: None,
-    ) -> ContextManager[TextIO]:
-        ...
-
-
 def atomic_opener(
     final_path: Path,
     mode: str,
     encoding: Optional[str] = None,
     _fd_spy: Callable[[int], None] = lambda unused: None,
     _after_link_hook: Callable[[], None] = lambda: None,
 ) -> ContextManager[Union[TextIO, BinaryIO]]:
```

### Comparing `rohmu-1.0.9/rohmu/compat.py` & `rohmu-1.1.0/rohmu/compat.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.0.9/rohmu/compressor.py` & `rohmu-1.1.0/rohmu/compressor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """
 rohmu - compressor interface
 
 Copyright (c) 2016 Ohmu Ltd
 See LICENSE for details
 """
-
 from .errors import InvalidConfigurationError
 from .filewrap import Sink, Stream
 from .snappyfile import SnappyFile
+from .typing import BinaryData, Compressor, Decompressor, FileLike, HasRead, HasWrite
 from .zstdfile import open as zstd_open
+from typing import cast, IO
 
 import lzma
 
 try:
     import snappy
 except ImportError:
     snappy = None  # type: ignore
 
 try:
     import zstandard as zstd
 except ImportError:
     zstd = None  # type: ignore
 
 
-def CompressionFile(dst_fp, algorithm, level=0, threads=0):
+def CompressionFile(dst_fp: FileLike, algorithm: str, level: int = 0, threads: int = 0) -> FileLike:
     """This looks like a class to users, but is actually a function that instantiates a class based on algorithm."""
     if algorithm == "lzma":
-        return lzma.open(dst_fp, "w", preset=level)
+        return lzma.open(cast(IO[bytes], dst_fp), "w", preset=level)
 
     if algorithm == "snappy":
         return SnappyFile(dst_fp, "wb")
 
     if algorithm == "zstd":
         return zstd_open(dst_fp, "wb", level=level, threads=threads)
 
@@ -39,63 +40,65 @@
 
     return dst_fp
 
 
 class CompressionStream(Stream):
     """Non-seekable stream of data that adds compression on top of given source stream"""
 
-    def __init__(self, src_fp, algorithm, level=0):
+    def __init__(self, src_fp: HasRead, algorithm: str, level: int = 0) -> None:
         super().__init__(src_fp, minimum_read_size=32 * 1024)
+        self._compressor: Compressor
         if algorithm == "lzma":
             self._compressor = lzma.LZMACompressor(lzma.FORMAT_XZ, -1, level, None)
         elif algorithm == "snappy":
             self._compressor = snappy.StreamCompressor()
         elif algorithm == "zstd":
             self._compressor = zstd.ZstdCompressor(level=level).compressobj()
         else:
             raise InvalidConfigurationError("invalid compression algorithm: {!r}".format(algorithm))
 
-    def _process_chunk(self, data):
+    def _process_chunk(self, data: bytes) -> bytes:
         return self._compressor.compress(data)
 
-    def _finalize(self):
+    def _finalize(self) -> bytes:
         return self._compressor.flush()
 
 
-def DecompressionFile(src_fp, algorithm):
+def DecompressionFile(src_fp: FileLike, algorithm: str) -> FileLike:
     """This looks like a class to users, but is actually a function that instantiates a class based on algorithm."""
     if algorithm == "lzma":
-        return lzma.open(src_fp, "r")
+        return lzma.open(cast(IO[bytes], src_fp), "r")
 
     if algorithm == "snappy":
         return SnappyFile(src_fp, "rb")
 
     if algorithm == "zstd":
         return zstd_open(src_fp, "rb")
 
     if algorithm:
         raise InvalidConfigurationError("invalid compression algorithm: {!r}".format(algorithm))
 
     return src_fp
 
 
 class DecompressSink(Sink):
-    def __init__(self, next_sink, compression_algorithm):
+    def __init__(self, next_sink: HasWrite, compression_algorithm: str):
         super().__init__(next_sink)
         self.decompressor = self._create_decompressor(compression_algorithm)
 
-    def _create_decompressor(self, alg):
+    def _create_decompressor(self, alg: str) -> Decompressor:
         if alg == "snappy":
             return snappy.StreamDecompressor()
         elif alg == "lzma":
             return lzma.LZMADecompressor()
         elif alg == "zstd":
             return zstd.ZstdDecompressor().decompressobj()
         raise InvalidConfigurationError("invalid compression algorithm: {!r}".format(alg))
 
-    def write(self, data):
+    def write(self, data: BinaryData) -> int:
+        data = bytes(data) if not isinstance(data, bytes) else data
         written = len(data)
         if not data:
             return written
         data = self.decompressor.decompress(data)
         self._write_to_next_sink(data)
         return written
```

### Comparing `rohmu-1.0.9/rohmu/dates.py` & `rohmu-1.1.0/rohmu/dates.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,30 +5,26 @@
 See LICENSE for details
 """
 import datetime
 import dateutil.parser
 import dateutil.tz
 
 
-def parse_timestamp(ts, *, with_tz=True, assume_local=False):
+def parse_timestamp(ts: str, *, with_tz: bool = True, assume_local: bool = False) -> datetime.datetime:
     """Parse a given timestamp and return a datetime object with or without tzinfo.
 
     If `with_tz` is False and we can't parse a timezone from the timestamp the datetime object is returned
     as-is and we assume the timezone is whatever was requested.  If `with_tz` is False and we can parse a
     timezone, the timestamp is converted to either local or UTC time based on `assume_local` after which tzinfo
     is stripped and the timestamp is returned.
 
     When `with_tz` is True and there's a timezone in the timestamp we return it as-is.  If `with_tz` is True
     but we can't parse a timezone we add either local or UTC timezone to the datetime based on `assume_local`.
     """
-    parse_result = dateutil.parser.parse(ts)
-
-    # pylint thinks dateutil.parser.parse always returns a tuple even though we didn't request it.
-    # So this check is pointless but convinces pylint that we really have a datetime object now.
-    dt = parse_result[0] if isinstance(parse_result, tuple) else parse_result  # pylint: disable=unsubscriptable-object
+    dt = dateutil.parser.parse(ts)
 
     if with_tz is False:
         if not dt.tzinfo:
             return dt
 
         tz = dateutil.tz.tzlocal() if assume_local else datetime.timezone.utc
         return dt.astimezone(tz).replace(tzinfo=None)
@@ -36,9 +32,9 @@
     if dt.tzinfo:
         return dt
 
     tz = dateutil.tz.tzlocal() if assume_local else datetime.timezone.utc
     return dt.replace(tzinfo=tz)
 
 
-def now():
+def now() -> datetime.datetime:
     return datetime.datetime.now(datetime.timezone.utc)
```

### Comparing `rohmu-1.0.9/rohmu/delta/common.py` & `rohmu-1.1.0/rohmu/delta/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # Copyright (c) 2021 Aiven, Helsinki, Finland. https://aiven.io/
+
+from __future__ import annotations
+
 from dataclasses import dataclass
 from datetime import datetime
 from multiprocessing.dummy import Pool
 from pathlib import Path
 from pydantic import BaseModel, Field
 from rohmu.dates import now
-from typing import List, Optional
+from rohmu.typing import AnyPath, HasRead
+from types import TracebackType
+from typing import Any, Callable, Iterable, List, Optional, Sequence, Type, TypeVar
 
 import functools
 import hashlib
 import json as _json
 import logging
 import math
 import os
@@ -19,25 +24,25 @@
 
 # Hexdigest is 32 bytes, so something orders of magnitude more at least
 EMBEDDED_FILE_SIZE = 150
 
 logger = logging.getLogger(__name__)
 
 
-def hash_hexdigest_readable(f, *, read_buffer=1_000_000):
+def hash_hexdigest_readable(f: HasRead, *, read_buffer: int = 1_000_000) -> str:
     h = _hash()
     while True:
         data = f.read(read_buffer)
         if not data:
             break
         h.update(data)
     return h.hexdigest()
 
 
-def increase_worth_reporting(value, new_value=None, *, total=None):
+def increase_worth_reporting(value: int, new_value: Optional[int] = None, *, total: Optional[int] = None) -> bool:
     """Make reporting sparser and sparser as values grow larger
     - report every 1.1**N or so
     - if we know total, report every percent
     """
     if new_value is None:
         new_value = value
         value = new_value - 1
@@ -72,47 +77,47 @@
 
         # Validate also assignments
         # validate_assignment = True
         # TBD: Figure out why this doesn't work in some unit tests;
         # possibly the tests themselves are broken
         validate_assignment = True
 
-    def jsondict(self, **kw):
+    def jsondict(self, **kw: Any) -> dict[str, Any]:
         # By default,
         #
         # .json() returns json string.
         # .dict() returns Python dict, but it has things that are not
         # json serializable.
         #
         # We provide json seralizable dict (super inefficiently) here.
         #
         # This is mostly used for test code so that should be fine
         return _json.loads(self.json(**kw))
 
 
 class SizeLimitedFile:
-    def __init__(self, *, path, file_size):
+    def __init__(self, *, path: AnyPath, file_size: int) -> None:
         self._f = open(path, "rb")
         self._file_size = file_size
         self.tell = self._f.tell
 
-    def __enter__(self):
+    def __enter__(self) -> SizeLimitedFile:
         return self
 
-    def __exit__(self, t, v, tb):
+    def __exit__(self, t: Optional[Type[BaseException]], v: Optional[BaseException], tb: Optional[TracebackType]) -> None:
         self._f.close()
 
-    def read(self, n=None):
+    def read(self, n: Optional[int] = None) -> bytes:
         can_read = max(0, self._file_size - self._f.tell())
         if n is None:
             n = can_read
         n = min(can_read, n)
         return self._f.read(n)
 
-    def seek(self, ofs, whence=0):
+    def seek(self, ofs: int, whence: int = 0) -> int:
         if whence == os.SEEK_END:
             ofs += self._file_size
             whence = os.SEEK_SET
         return self._f.seek(ofs, whence)
 
 
 class SnapshotHash(DeltaModel):
@@ -123,49 +128,49 @@
     same hexdigest is available from multiple nodes.
 
     """
 
     hexdigest: str
     size: int
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if isinstance(other, SnapshotHash):
             return self.hexdigest == other.hexdigest
         return False
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         # hexdigests should be unique, regardless of size
         return hash(self.hexdigest)
 
 
 @functools.total_ordering
 class SnapshotFile(DeltaModel):
     relative_path: Path = Field(..., allow_mutation=False)
     file_size: int
     stored_file_size: int
     mtime_ns: int
     hexdigest: str = ""
-    content_b64: Optional[str]
+    content_b64: Optional[str] = None
     # Indicator if a file should be part of a chunk/bundle - useful for the files which are small to be treated as
     # separate delta hash files, but not small enough to be embedded into a manifest file, so better to group them
     # together when e.g. uploading to the object storage
     should_be_bundled: bool = False
     missing_ok: bool = True
 
-    def __lt__(self, o):
+    def __lt__(self, o: SnapshotFile) -> bool:
         # In our use case, paths uniquely identify files we care about
         return self.relative_path < o.relative_path
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(self.relative_path)
 
-    def equals_excluding_mtime(self, o):
+    def equals_excluding_mtime(self, o: SnapshotFile) -> bool:
         return self.copy(update={"mtime_ns": 0}) == o.copy(update={"mtime_ns": 0})
 
-    def open_for_reading(self, root_path):
+    def open_for_reading(self, root_path: Path) -> SizeLimitedFile:
         return SizeLimitedFile(path=root_path / self.relative_path, file_size=self.file_size)
 
 
 class SnapshotState(DeltaModel):
     root_globs: List[str]
     files: List[SnapshotFile]
     empty_dirs: List[Path]
@@ -207,88 +212,94 @@
     """JSON-encodable progress meter of sorts"""
 
     handled: int = 0
     failed: int = 0
     total: int = 0
     final: bool = False
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         finished = ", finished" if self.final else ""
         return f"{self.handled}/{self.total} handled, {self.failed} failures{finished}"
 
-    def start(self, n):
+    def start(self, n: int) -> None:
         "Optional 'first' step, just for logic handling state (e.g. no progress object reuse desired)"
         assert not self.total
         logger.debug("start")
         self.add_total(n)
 
-    def add_total(self, n):
+    def add_total(self, n: int) -> None:
         if not n:
             return
         old_total = self.total
         self.total += n
         if increase_worth_reporting(old_total, self.total):
             logger.debug("add_total %r -> %r", n, self)
         assert not self.final
 
-    def add_fail(self, n=1, *, info="add_fail"):
+    def add_fail(self, n: int = 1, *, info: str = "add_fail") -> None:
         assert n > 0
         old_failed = self.failed
         self.failed += n
         if increase_worth_reporting(old_failed, self.failed):
             logger.debug("%s %r -> %r", info, n, self)
         assert not self.final
 
-    def add_success(self, n=1, *, info="add_success"):
+    def add_success(self, n: int = 1, *, info: str = "add_success") -> None:
         assert n > 0
         old_handled = self.handled
         self.handled += n
         assert self.handled <= self.total
         if increase_worth_reporting(old_handled, self.handled, total=self.total):
             logger.debug("%s %r -> %r", info, n, self)
         assert not self.final
 
-    def download_success(self, size):
+    def download_success(self, size: int) -> None:
         self.add_success(size, info="download_success")
 
-    def upload_success(self, hexdigest):
+    def upload_success(self, hexdigest: str) -> None:
         self.add_success(info=f"upload_success {hexdigest}")
 
-    def upload_missing(self, hexdigest):
+    def upload_missing(self, hexdigest: str) -> None:
         self.add_fail(info=f"upload_missing {hexdigest}")
 
-    def upload_failure(self, hexdigest):
+    def upload_failure(self, hexdigest: str) -> None:
         self.add_fail(info=f"upload_failure {hexdigest}")
 
-    def done(self):
+    def done(self) -> None:
         assert self.total is not None and self.handled <= self.total
         assert not self.final
         self.final = True
         logger.debug("done %r", self)
 
     @property
-    def finished_successfully(self):
+    def finished_successfully(self) -> bool:
         return self.final and not self.failed and self.handled == self.total
 
     @property
-    def finished_failed(self):
+    def finished_failed(self) -> bool:
         return self.final and not self.finished_successfully
 
     @classmethod
-    def merge(cls, progresses):
+    def merge(cls, progresses: Sequence[Progress]) -> Progress:
         p = cls()
         for progress in progresses:
             p.handled += progress.handled
             p.failed += progress.failed
             p.total += progress.total
         p.final = all(progress.final for progress in progresses)
         return p
 
 
-def parallel_map_to(*, fun, iterable, result_callback, n=None) -> bool:
+Item = TypeVar("Item")
+Result = TypeVar("Result")
+
+
+def parallel_map_to(
+    *, fun: Callable[[Item], Result], iterable: Iterable[Item], result_callback: Callable[..., bool], n: Optional[int] = None
+) -> bool:
     iterable_as_list = list(iterable)
     with Pool(n) as p:
         for map_in, map_out in zip(iterable_as_list, p.imap(fun, iterable_as_list)):
             if not result_callback(map_in=map_in, map_out=map_out):
                 return False
     return True
```

### Comparing `rohmu-1.0.9/rohmu/delta/snapshot.py` & `rohmu-1.1.0/rohmu/delta/snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 # Copyright (c) 2021 Aiven, Helsinki, Finland. https://aiven.io/
+
+from __future__ import annotations
+
 from pathlib import Path
 from rohmu.delta.common import (
     BackupPath,
     EMBEDDED_FILE_SIZE,
     hash_hexdigest_readable,
     increase_worth_reporting,
     parallel_map_to,
     Progress,
     SnapshotFile,
     SnapshotHash,
     SnapshotState,
 )
-from typing import Callable, Dict, Generator, Iterable, List, Optional, Sequence, Set, Tuple, Union
+from rohmu.typing import StrOrPathLike
+from typing import Any, Callable, Generator, Iterable, List, Optional, Sequence, Set, Tuple, Union
 
 import base64
 import logging
 import os
 import threading
 
 logger = logging.getLogger(__name__)
 
 
 class Snapshotter:
     """Snapshotter keeps track of files on disk, and their hashes.
 
     The hash on disk MAY change, which may require subsequent
-    incremential snapshot and-or ignoring the files which have changed.
+    incremental snapshot and-or ignoring the files which have changed.
 
     The output to outside is just root object's hash, as well as list
     of other hashes which correspond to files referred to within the
     file list contained in root object.
 
     Note that any call to public API MUST be made with
     snapshotter.lock held. This is because Snapshotter is process-wide
@@ -41,28 +45,28 @@
     built-in to Snapshotter, but having it there enables asserting its
     state during public API calls.
     """
 
     def __init__(
         self,
         *,
-        src,
-        dst,
-        globs,
+        src: StrOrPathLike,
+        dst: StrOrPathLike,
+        globs: list[str],
         src_iterate_func: Optional[Callable[[], Iterable[Union[BackupPath, str, Path]]]] = None,
         parallel: int = 1,
         min_delta_file_size: int = 0,
-    ):
+    ) -> None:
         assert globs
         self.src = Path(src)
         self.dst = Path(dst)
         self.globs = globs
         self.src_iterate_func = src_iterate_func
-        self.relative_path_to_snapshotfile: Dict[Path, SnapshotFile] = {}
-        self.hexdigest_to_snapshotfiles: Dict[str, List[SnapshotFile]] = {}
+        self.relative_path_to_snapshotfile: dict[Path, SnapshotFile] = {}
+        self.hexdigest_to_snapshotfiles: dict[str, List[SnapshotFile]] = {}
         self.parallel = parallel
         self.lock = threading.Lock()
         self.empty_dirs: List[Path] = []
         self.min_delta_file_size = min_delta_file_size
 
     def _list_files(self, basepath: Path) -> List[Path]:
         result_files = set()
@@ -271,26 +275,27 @@
         # ones were already removed)
         dst_dirs, dst_files = self._list_dirs_and_files(self.dst)
         self.empty_dirs = src_dirs
         snapshotfiles = list(self._gen_snapshot_hashes(dst_files, reuse_old_snapshotfiles, required_paths=required_paths))
 
         progress.add_total(len(snapshotfiles))
 
-        def _cb(snapshotfile: SnapshotFile):
+        def _cb(snapshotfile: SnapshotFile) -> SnapshotFile:
             # src may or may not be present; dst is present as it is in snapshot
             with snapshotfile.open_for_reading(self.dst) as f:
                 if snapshotfile.file_size <= EMBEDDED_FILE_SIZE:
                     snapshotfile.content_b64 = base64.b64encode(f.read()).decode()
                 elif snapshotfile.file_size < self.min_delta_file_size:
                     snapshotfile.should_be_bundled = True
                 else:
                     snapshotfile.hexdigest = hash_hexdigest_readable(f)
             return snapshotfile
 
-        def _result_cb(*, map_in, map_out):
+        def _result_cb(*, map_in: Any, map_out: SnapshotFile) -> bool:
             self._add_snapshotfile(map_out)
+            assert progress is not None
             progress.add_success()
             return True
 
         changes += len(snapshotfiles)
         parallel_map_to(iterable=snapshotfiles, fun=_cb, result_callback=_result_cb, n=self.parallel)
         return changes
```

### Comparing `rohmu-1.0.9/rohmu/encryptor.py` & `rohmu-1.1.0/rohmu/encryptor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,155 +1,187 @@
 """
 rohmu - content encryption
 
 Copyright (c) 2016 Ohmu Ltd
 See LICENSE for details
 """
-
 from . import IO_BLOCK_SIZE
+from .errors import UninitializedError
 from .filewrap import FileWrap, Sink, Stream
+from .typing import BinaryData, FileLike, HasRead, HasWrite
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import padding
-from cryptography.hazmat.primitives.ciphers import algorithms, Cipher, modes
+from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
+from cryptography.hazmat.primitives.ciphers import algorithms, Cipher, CipherContext, modes
 from cryptography.hazmat.primitives.hashes import SHA1, SHA256
 from cryptography.hazmat.primitives.hmac import HMAC
+from typing import Optional, Union
 
-import cryptography
-import cryptography.hazmat.backends.openssl.backend
 import io
 import logging
 import os
 import struct
 
-if cryptography.__version__ < "1.6":  # type: ignore
-    # workaround for deadlock https://github.com/pyca/cryptography/issues/2911
-    cryptography.hazmat.backends.openssl.backend.activate_builtin_random()
-
 FILEMAGIC = b"pghoa1"
 AES_BLOCK_SIZE = 16
 
 
 class EncryptorError(Exception):
     """EncryptorError"""
 
 
 class Encryptor:
-    def __init__(self, rsa_public_key_pem):
+    def __init__(self, rsa_public_key_pem: Union[str, bytes]):
         if not isinstance(rsa_public_key_pem, bytes):
             rsa_public_key_pem = rsa_public_key_pem.encode("ascii")
-        self.rsa_public_key = serialization.load_pem_public_key(rsa_public_key_pem, backend=default_backend())
-        self.cipher = None
-        self.authenticator = None
+        public_key = serialization.load_pem_public_key(rsa_public_key_pem, backend=default_backend())
+        assert isinstance(public_key, RSAPublicKey)
+        self.rsa_public_key = public_key
+        self._cipher: Optional[CipherContext] = None
+        self._authenticator: Optional[HMAC] = None
+
+    @property
+    def cipher(self) -> CipherContext:
+        if self._cipher is None:
+            raise UninitializedError("cipher not initialized")
+        return self._cipher
+
+    @property
+    def authenticator(self) -> HMAC:
+        if self._authenticator is None:
+            raise UninitializedError("authenticator not initialized")
+        return self._authenticator
 
-    def update(self, data):
+    def update(self, data: bytes) -> bytes:
         ret = b""
-        if self.cipher is None:
+        if self._cipher is None:
             key = os.urandom(16)
             nonce = os.urandom(16)
             auth_key = os.urandom(32)
-            self.cipher = Cipher(algorithms.AES(key), modes.CTR(nonce), backend=default_backend()).encryptor()
-            self.authenticator = HMAC(auth_key, SHA256(), backend=default_backend())
+            self._cipher = Cipher(algorithms.AES(key), modes.CTR(nonce), backend=default_backend()).encryptor()
+            self._authenticator = HMAC(auth_key, SHA256(), backend=default_backend())
             pad = padding.OAEP(mgf=padding.MGF1(algorithm=SHA1()), algorithm=SHA1(), label=None)
             cipherkey = self.rsa_public_key.encrypt(key + nonce + auth_key, pad)
             ret = FILEMAGIC + struct.pack(">H", len(cipherkey)) + cipherkey
         cur = self.cipher.update(data)
         self.authenticator.update(cur)
         if ret:
             return ret + cur
         else:
             return cur
 
-    def finalize(self):
-        if self.cipher is None:
+    def finalize(self) -> bytes:
+        if self._cipher is None:
             return b""  # empty plaintext input yields empty encrypted output
 
         ret = self.cipher.finalize()
         self.authenticator.update(ret)
         ret += self.authenticator.finalize()
-        self.cipher = None
-        self.authenticator = None
+        self._cipher = None
+        self._authenticator = None
         return ret
 
 
 class EncryptorFile(FileWrap):
-    def __init__(self, next_fp, rsa_public_key_pem):
+    def __init__(self, next_fp: FileLike, rsa_public_key_pem: Union[str, bytes]) -> None:
         super().__init__(next_fp)
         self.key = rsa_public_key_pem
-        self.encryptor = Encryptor(self.key)
+        self._encryptor: Optional[Encryptor] = Encryptor(self.key)
         self.offset = 0
         self.state = "OPEN"
 
-    def flush(self):
+    @property
+    def encryptor(self) -> Encryptor:
+        if self._encryptor is None:
+            raise UninitializedError("encryptor was not initialized")
+        return self._encryptor
+
+    def flush(self) -> None:
         self._check_not_closed()
         self.next_fp.flush()
 
-    def close(self):
+    def close(self) -> None:
         if self.state == "CLOSED":
             return
         final = self.encryptor.finalize()
-        self.encryptor = None
         self.next_fp.write(final)
         super().close()
+        self._encryptor = None
 
-    def writable(self):
+    def writable(self) -> bool:
         """True if this stream supports writing"""
         self._check_not_closed()
         return True
 
-    def write(self, data):
+    def write(self, data: BinaryData) -> int:
         """Encrypt and write the given bytes"""
         self._check_not_closed()
         if not data:
             return 0
-        enc_data = self.encryptor.update(data)
+        data_as_bytes = bytes(data)
+        enc_data = self.encryptor.update(data_as_bytes)
         self.next_fp.write(enc_data)
-        self.offset += len(data)
-        return len(data)
+        self.offset += len(data_as_bytes)
+        return len(data_as_bytes)
 
 
 class EncryptorStream(Stream):
     """Non-seekable stream of data that adds encryption on top of given source stream"""
 
-    def __init__(self, src_fp, rsa_public_key_pem):
+    def __init__(self, src_fp: HasRead, rsa_public_key_pem: Union[str, bytes]) -> None:
         super().__init__(src_fp)
         self._encryptor = Encryptor(rsa_public_key_pem)
 
-    def _process_chunk(self, data):
+    def _process_chunk(self, data: bytes) -> bytes:
         return self._encryptor.update(data)
 
-    def _finalize(self):
+    def _finalize(self) -> bytes:
         return self._encryptor.finalize()
 
 
 class Decryptor:
-    def __init__(self, rsa_private_key_pem):
+    def __init__(self, rsa_private_key_pem: Union[str, bytes]) -> None:
         if not isinstance(rsa_private_key_pem, bytes):
             rsa_private_key_pem = rsa_private_key_pem.encode("ascii")
         self.rsa_private_key = serialization.load_pem_private_key(
             data=rsa_private_key_pem, password=None, backend=default_backend()
         )
-        self.cipher = None
-        self.authenticator = None
+        self._cipher: Optional[CipherContext] = None
+        self._authenticator: Optional[HMAC] = None
         self._cipher_key_len = None
         self._header_size = None
         self._footer_size = 32
 
-    def expected_header_bytes(self):
+    @property
+    def authenticator(self) -> HMAC:
+        if self._authenticator is None:
+            raise UninitializedError("authenticator not initialized")
+        return self._authenticator
+
+    @property
+    def cipher(self) -> CipherContext:
+        if self._cipher is None:
+            raise UninitializedError("cipher not initialized")
+        return self._cipher
+
+    def expected_header_bytes(self) -> int:
         if self._header_size is not None:
             return 0
         return self._cipher_key_len or 8
 
-    def header_size(self):
+    def header_size(self) -> int:
+        if self._header_size is None:
+            raise UninitializedError("header_size not initialized")
         return self._header_size
 
-    def footer_size(self):
+    def footer_size(self) -> int:
         return self._footer_size
 
-    def process_header(self, data):
+    def process_header(self, data: bytes) -> None:
         if self._cipher_key_len is None:
             if data[0:6] != FILEMAGIC:
                 raise EncryptorError("Invalid magic bytes")
             self._cipher_key_len = struct.unpack(">H", data[6:8])[0]
         else:
             pad = padding.OAEP(mgf=padding.MGF1(algorithm=SHA1()), algorithm=SHA1(), label=None)
             try:
@@ -159,125 +191,144 @@
             if len(plainkey) != 64:
                 raise EncryptorError("Integrity check failed")
             key = plainkey[0:16]
             nonce = plainkey[16:32]
             auth_key = plainkey[32:64]
             self._header_size = 8 + len(data)
 
-            self.cipher = Cipher(algorithms.AES(key), modes.CTR(nonce), backend=default_backend()).decryptor()
-            self.authenticator = HMAC(auth_key, SHA256(), backend=default_backend())
+            self._cipher = Cipher(algorithms.AES(key), modes.CTR(nonce), backend=default_backend()).decryptor()
+            self._authenticator = HMAC(auth_key, SHA256(), backend=default_backend())
 
-    def process_data(self, data):
+    def process_data(self, data: bytes) -> bytes:
         if not data:
             return b""
         self.authenticator.update(data)
         return self.cipher.update(data)
 
-    def finalize(self, footer):
+    def finalize(self, footer: bytes) -> bytes:
         if footer != self.authenticator.finalize():
             raise EncryptorError("Integrity check failed")
         result = self.cipher.finalize()
-        self.cipher = None
-        self.authenticator = None
+        self._cipher = None
+        self._authenticator = None
         return result
 
 
 class DecryptorFile(FileWrap):
-    def __init__(self, next_fp, rsa_private_key_pem):
+    def __init__(self, next_fp: FileLike, rsa_private_key_pem: Union[bytes, str]):
         super().__init__(next_fp)
         self._key = rsa_private_key_pem
         self.log = logging.getLogger(self.__class__.__name__)
-        self._decryptor = None
-        self._crypted_size = None
-        self._boundary_block = None
-        self._plaintext_size = None
+        self._maybe_decryptor: Optional[Decryptor] = None
+        self._maybe_crypted_size: Optional[int] = None
+        self._maybe_plaintext_size: Optional[int] = None
+        self._maybe_boundary_block: Optional[bytes] = None
         # Our actual plain-text read offset. seek may change self.offset to something
         # else temporarily but we keep _decrypt_offset intact until we actually do a
         # read in case the caller just called seek in order to then immediately seek back
-        self._decrypt_offset = None
-        self.offset = None
+        self._decrypt_offset = 0
+        self.offset = 0
         self._reset()
 
-    def _reset(self):
-        self._decryptor = Decryptor(self._key)
-        self._crypted_size = self._file_size(self.next_fp)
-        self._boundary_block = None
-        self._plaintext_size = None
+    @property
+    def _decryptor(self) -> Decryptor:
+        if self._maybe_decryptor is None:
+            raise UninitializedError("decryptor not initialized")
+        return self._maybe_decryptor
+
+    @property
+    def _crypted_size(self) -> int:
+        if self._maybe_crypted_size is None:
+            raise UninitializedError("crypted_size not initialized")
+        return self._maybe_crypted_size
+
+    @property
+    def _plaintext_size(self) -> int:
+        if self._maybe_plaintext_size is None:
+            raise UninitializedError("plaintext_size not initialized")
+        return self._maybe_plaintext_size
+
+    def _reset(self) -> None:
+        self._maybe_decryptor = Decryptor(self._key)
+        self._maybe_crypted_size = self._file_size(self.next_fp)
+        self._maybe_boundary_block = None
+        self._maybe_plaintext_size = None
         self._decrypt_offset = 0
         # Plaintext offset
         self.offset = 0
         self.state = "OPEN"
 
     @classmethod
-    def _file_size(cls, file):
+    def _file_size(cls, file: FileLike) -> int:
         current_offset = file.seek(0, os.SEEK_SET)
         file_end_offset = file.seek(0, os.SEEK_END)
         file.seek(current_offset, os.SEEK_SET)
         return file_end_offset
 
-    def _initialize_decryptor(self):
-        if self._plaintext_size is not None:
+    def _initialize_decryptor(self) -> None:
+        if self._maybe_plaintext_size is not None:
             return
         while True:
             required_bytes = self._decryptor.expected_header_bytes()
             if not required_bytes:
                 break
             self._decryptor.process_header(self._read_raw_exactly(required_bytes))
-        self._plaintext_size = self._crypted_size - self._decryptor.header_size() - self._decryptor.footer_size()
+        self._maybe_plaintext_size = self._crypted_size - self._decryptor.header_size() - self._decryptor.footer_size()
 
-    def _read_raw_exactly(self, required_bytes):
+    def _read_raw_exactly(self, required_bytes: int) -> bytes:
         data = self.next_fp.read(required_bytes)
         while data and len(data) < required_bytes:
             next_chunk = self.next_fp.read(required_bytes - len(data))
             if not next_chunk:
                 break
             data += next_chunk
         if not data or len(data) != required_bytes:
             raise EncryptorError("Failed to read {} bytes of header or footer data".format(required_bytes))
         return data
 
-    def _move_decrypt_offset_to_plaintext_offset(self):
+    def _move_decrypt_offset_to_plaintext_offset(self) -> None:
         if self._decrypt_offset == self.offset:
             return
         seek_to = self.offset
         if self._decrypt_offset > self.offset:
             self.log.warning("Negative seek from %d to %d, must re-initialize decryptor", self._decrypt_offset, self.offset)
             self._reset()
             self._initialize_decryptor()
         discard_bytes = seek_to - self._decrypt_offset
         self.offset = self._decrypt_offset
         while discard_bytes > 0:
             data = self._read_block(discard_bytes)
             discard_bytes -= len(data)
 
-    def _read_all(self):
+    def _read_all(self) -> bytes:
         full_data = bytearray()
         while True:
             data = self._read_block(IO_BLOCK_SIZE)
             if not data:
                 return bytes(full_data)
             full_data.extend(data)
 
-    def _read_block(self, size):
+    def _read_block(self, size: int) -> bytes:
         if self._crypted_size == 0:
             return b""
 
         self._initialize_decryptor()
 
         if self.offset == self._plaintext_size:
             return b""
 
         self._move_decrypt_offset_to_plaintext_offset()
 
         # If we have an existing boundary block, fulfil the read entirely from that
-        if self._boundary_block:
-            size = min(size, len(self._boundary_block) - self.offset % AES_BLOCK_SIZE)
-            data = self._boundary_block[self.offset % AES_BLOCK_SIZE : self.offset % AES_BLOCK_SIZE + size]
-            if self.offset % AES_BLOCK_SIZE + size == len(self._boundary_block):
-                self._boundary_block = None
+        if self._maybe_boundary_block:
+            boundary_block: bytes = self._maybe_boundary_block
+            size = min(size, len(boundary_block) - self.offset % AES_BLOCK_SIZE)
+            data = boundary_block[self.offset % AES_BLOCK_SIZE : self.offset % AES_BLOCK_SIZE + size]
+            if self.offset % AES_BLOCK_SIZE + size == len(boundary_block):
+                self._maybe_boundary_block = None
             data_len = len(data)
             self.offset += data_len
             self._decrypt_offset += data_len
             return data
 
         # Only serve multiples of AES_BLOCK_SIZE whenever possible to keep things simpler
         read_size = size
@@ -293,41 +344,41 @@
         if self.offset + read_size == self._plaintext_size:
             footer = self._read_raw_exactly(self._decryptor.footer_size())
             last_part = self._decryptor.finalize(footer)
             if last_part:
                 decrypted += last_part
 
         if size < AES_BLOCK_SIZE:
-            self._boundary_block = decrypted
+            self._maybe_boundary_block = decrypted
             return self._read_block(size)
         decrypted_len = len(decrypted)
         self.offset += decrypted_len
         self._decrypt_offset += decrypted_len
         return decrypted
 
-    def close(self):
+    def close(self) -> None:
         super().close()
-        self._decryptor = None
+        self._maybe_decryptor = None
 
-    def read(self, size=-1):
+    def read(self, size: Optional[int] = -1) -> bytes:
         """Read up to size decrypted bytes"""
         self._check_not_closed()
         if self.state == "EOF" or size == 0:
             return b""
-        elif size < 0:
+        elif size is None or size < 0:
             return self._read_all()
         else:
             return self._read_block(size)
 
-    def readable(self):
+    def readable(self) -> bool:
         """True if this stream supports reading"""
         self._check_not_closed()
         return self.state in ["OPEN", "EOF"]
 
-    def seek(self, offset, whence=0):
+    def seek(self, offset: int, whence: int = 0) -> int:
         self._check_not_closed()
         self._initialize_decryptor()
         if whence == os.SEEK_SET:
             if offset != self.offset:
                 if offset > self._plaintext_size:
                     raise io.UnsupportedOperation("DecryptorFile does not support seeking beyond EOF")
                 if offset < 0:
@@ -342,58 +393,59 @@
             if offset != 0:
                 raise io.UnsupportedOperation("can't do nonzero end-relative seeks")
             self.offset = self._plaintext_size
             return self.offset
         else:
             raise ValueError("Invalid whence value")
 
-    def seekable(self):
+    def seekable(self) -> bool:
         """True if this stream supports random access"""
         self._check_not_closed()
         return True
 
 
 class DecryptSink(Sink):
-    def __init__(self, next_sink, file_size, encryption_key_data):
+    def __init__(self, next_sink: HasWrite, file_size: int, encryption_key_data: Union[str, bytes]) -> None:
         super().__init__(next_sink)
         if file_size <= 0:
             raise ValueError("Invalid file_size: " + str(file_size))
         self.data_bytes_received = 0
         self.data_size = file_size
         self.decryptor = Decryptor(encryption_key_data)
         self.file_size = file_size
         self.footer = b""
         self.header = b""
 
-    def _extract_encryption_footer_bytes(self, data):
+    def _extract_encryption_footer_bytes(self, data: bytes) -> bytes:
         expected_data_bytes = self.data_size - self.data_bytes_received
         if len(data) > expected_data_bytes:
             self.footer += data[expected_data_bytes:]
             data = data[:expected_data_bytes]
         return data
 
-    def _process_encryption_header(self, data):
+    def _process_encryption_header(self, data: bytes) -> bytes:
         if not data or not self.decryptor.expected_header_bytes():
             return data
         if self.header:
             data = self.header + data
-            self.header = None
+            self.header = b""
         offset = 0
         while self.decryptor.expected_header_bytes() > 0:
             header_bytes = self.decryptor.expected_header_bytes()
             if header_bytes + offset > len(data):
                 self.header = data[offset:]
                 return b""
             self.decryptor.process_header(data[offset : offset + header_bytes])
             offset += header_bytes
         data = data[offset:]
         self.data_size = self.file_size - self.decryptor.header_size() - self.decryptor.footer_size()
         return data
 
-    def write(self, data):
+    def write(self, data: BinaryData) -> int:
+        data = bytes(data) if not isinstance(data, bytes) else data
         written = len(data)
         data = self._process_encryption_header(data)
         if not data:
             return written
         data = self._extract_encryption_footer_bytes(data)
         self.data_bytes_received += len(data)
         if data:
```

### Comparing `rohmu-1.0.9/rohmu/errors.py` & `rohmu-1.1.0/rohmu/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,7 +28,19 @@
 
 class MissingLibraryError(Exception):
     """Missing dependency library"""
 
 
 class MaybeRecoverableError(Error):
     """An error that may be recoverable"""
+
+
+class UninitializedError(Error):
+    """Error trying to access an uninitialized resource"""
+
+
+class InvalidByteRangeError(Error):
+    """Error specifying a content-range in a request"""
+
+
+class InvalidTransferError(Error):
+    """You tried to access a transfer object that you already returned to the pool"""
```

### Comparing `rohmu-1.0.9/rohmu/filewrap.py` & `rohmu-1.1.0/rohmu/filewrap.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,89 +1,98 @@
 """
 rohmu - file transformation wrapper
 
 Copyright (c) 2016 Ohmu Ltd
 See LICENSE for details
 """
+from .errors import UninitializedError
+from .typing import BinaryData, FileLike, HasRead, HasWrite
+from typing import Callable, Optional
 
 import io
 import time
 
 
 class FileWrap(io.BufferedIOBase):
     # pylint: disable=unused-argument
 
-    def __init__(self, next_fp):
+    def __init__(self, next_fp: FileLike) -> None:
         super().__init__()
-        self.next_fp = next_fp
+        self._next_fp: Optional[FileLike] = next_fp
         self.offset = 0
         self.state = "OPEN"
 
-    def _check_not_closed(self):
+    @property
+    def next_fp(self) -> FileLike:
+        if self._next_fp is None:
+            raise UninitializedError("next_fp not initialized")
+        return self._next_fp
+
+    def _check_not_closed(self) -> None:
         if self.state == "CLOSED":
             raise ValueError("I/O operation on closed file")
 
-    def close(self):
-        """Close stream"""
+    def close(self) -> None:
+        """Close stream."""
         if self.state == "CLOSED":
             return
         self.flush()
         # We close the stack of rohmu file wrappers, but leave the underlying real io object open to allow the
         # caller to do something useful with it if they like, for example reading the output out of a BytesIO
         # object or linking a temporary file to another name, etc.
         if isinstance(self.next_fp, FileWrap):
             self.next_fp.close()
-        self.next_fp = None
+        self._next_fp = None
         self.state = "CLOSED"
 
     @property
-    def closed(self):
+    def closed(self) -> bool:
         """True if this stream is closed"""
         return self.state == "CLOSED"
 
-    def fileno(self):
+    def fileno(self) -> int:
         self._check_not_closed()
         return self.next_fp.fileno()
 
-    def flush(self):
+    def flush(self) -> None:
         self._check_not_closed()
 
-    def tell(self):
+    def tell(self) -> int:
         self._check_not_closed()
         return self.offset
 
-    def readable(self):
+    def readable(self) -> bool:
         """True if this stream supports reading"""
         self._check_not_closed()
         return False
 
-    def read(self, size=-1):
+    def read(self, size: Optional[int] = -1) -> bytes:
         """Read up to size decrypted bytes"""
         self._check_not_closed()
         raise io.UnsupportedOperation("Read not supported")
 
-    def seekable(self):
+    def seekable(self) -> bool:
         """True if this stream supports random access"""
         self._check_not_closed()
         return False
 
-    def seek(self, offset, whence=0):
+    def seek(self, offset: int, whence: int = 0) -> int:
         self._check_not_closed()
         raise io.UnsupportedOperation("Seek not supported")
 
-    def truncate(self):
+    def truncate(self, size: Optional[int] = None) -> int:
         self._check_not_closed()
         raise io.UnsupportedOperation("Truncate not supported")
 
-    def writable(self):
+    def writable(self) -> bool:
         """True if this stream supports writing"""
         self._check_not_closed()
         return False
 
-    def write(self, data):
+    def write(self, data: BinaryData) -> int:
         """Encrypt and write the given bytes"""
         self._check_not_closed()
         raise io.UnsupportedOperation("Write not supported")
 
 
 class Sink:
     """Sink performs transformation for received input data and passes it forward to
@@ -91,68 +100,69 @@
     turn calls `write` for the next sink.
 
     Unlike the FileWrap interface, which is useful for performing transformation when
     data is being pulled from a source, the Sink interface can be used when data is
     pushed through a pipeline of transformations. This provides better performance as
     any temporary files or buffers can be omitted."""
 
-    def __init__(self, next_sink):
+    def __init__(self, next_sink: HasWrite) -> None:
         self.next_sink = next_sink
 
-    def _data_written(self, bytes_written, pending_bytes):
+    def _data_written(self, bytes_written: int, pending_bytes: int) -> None:
         pass
 
-    def _write_to_next_sink(self, data):
+    def _write_to_next_sink(self, data: BinaryData) -> None:
         data = memoryview(data)
         offset = 0
         while offset < len(data):
             start_offset = offset
             offset += self.next_sink.write(data[offset:])
             self._data_written(offset - start_offset, len(data) - offset)
 
-    def write(self, data):
+    def write(self, data: BinaryData) -> int:
         """Performs some transformation for given data and writes the transformed
         data to next sink."""
+        data = memoryview(data)
         self._write_to_next_sink(data)
         return len(data)
 
 
 class ThrottleSink(Sink):
     """Provides simple throttling sink that can be used if the target sink is
     non-blocking device that can return short if all data cannot be immediately
     written. In such cases writing again immediately after a small write would
     result in unnecessary busy-looping."""
 
-    def __init__(self, next_sink, wait_time, sleep_fn=time.sleep):
+    def __init__(self, next_sink: HasWrite, wait_time: float, sleep_fn: Callable[[float], None] = time.sleep) -> None:
         super().__init__(next_sink)
         self.sleep_fn = sleep_fn
         self.wait_time = wait_time
 
-    def _data_written(self, bytes_written, pending_bytes):
+    def _data_written(self, bytes_written: int, pending_bytes: int) -> None:
         if pending_bytes > 0 and bytes_written < 10 * 1024:
             self.sleep_fn(self.wait_time)
 
 
 class Stream:
     """Non-seekable stream of data that performs some kind of processing for given source stream"""
 
-    def __init__(self, src_fp, *, minimum_read_size=8 * 1024):
+    def __init__(self, src_fp: HasRead, *, minimum_read_size: int = 8 * 1024) -> None:
         self._eof = False
         self._remainder = b""
         self._src = src_fp
         self.minimum_read_size = minimum_read_size
         self._offset = 0
 
-    def _process_chunk(self, data):
+    def _process_chunk(self, data: bytes) -> bytes:
         raise NotImplementedError
 
-    def _finalize(self):
+    def _finalize(self) -> bytes:
         raise NotImplementedError
 
-    def read(self, size=-1):
+    def read(self, size: int = -1) -> bytes:
         bytes_available = len(self._remainder)
         chunks = [self._remainder] if self._remainder else []
         while not self._eof and (size < 0 or bytes_available < size):
             bytes_to_read = -1 if size < 0 else size - bytes_available
             # Always read at least self.minimum_read_size bytes even if fewer bytes are requested to avoid
             # looping with very small buffers when stream processor needs non-trivial amount of input to
             # make progress
@@ -184,9 +194,9 @@
                 data += chunks[-1][:bytes_missing]
                 self._remainder = chunks[-1][bytes_missing:]
             else:
                 self._remainder = chunks[-1]
         self._offset += len(data)
         return data
 
-    def tell(self):
+    def tell(self) -> int:
         return self._offset
```

### Comparing `rohmu-1.0.9/rohmu/inotify.py` & `rohmu-1.1.0/rohmu/inotify.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """
 rohmu - inotify wrapper
 
 Copyright (c) 2016 Ohmu Ltd
 See LICENSE for details
 """
+
+from __future__ import annotations
+
 from contextlib import suppress
 from ctypes import c_char_p, c_int, c_uint32
+from queue import Queue
+from rohmu.typing import AnyPath
 from threading import Thread
+from typing import Iterable, Iterator, Optional
 
 import ctypes
 import logging
 import os
 import select
 import struct
 
@@ -38,50 +44,61 @@
     "IN_DELETE_SELF": 0x00000400,
     "IN_IGNORED": 0x8000,
 }
 
 IN_NONBLOCK = 0x00004000
 
 
-def parse_inotify_buffer(event_buffer):
+def parse_inotify_buffer(event_buffer: bytes) -> Iterator[tuple[int, int, int, bytes]]:
+    """Yield parsed inotify events from a raw bytes sequence.
+
+    The `event_buffer` must be a byte sequence consisting of 0 or more sequences of the kind:
+
+        +------------------+------+--------+-------------+------+
+        | Watch descriptor | Mask | Cookie | Name length | Name |
+        +------------------+------+--------+-------------+------+
+
+    This function yields successive tuples (Watch descriptor, Mask, Cookie, Name) parsed from the provided bytes.
+
+    """
     i = 0
     while i + s_size <= len(event_buffer):
         wd, mask, cookie, length = struct.unpack_from("iIII", event_buffer, i)
         name = event_buffer[i + s_size : i + s_size + length].rstrip(b"\0")
         i += s_size + length
         yield wd, mask, cookie, name
 
 
 class InotifyWatcher(Thread):
-    def __init__(self, compression_queue):
+    def __init__(self, compression_queue: Queue[dict[str, str]]) -> None:
         super().__init__()
         # use the newer form for future-proofness
         self.log = logging.getLogger("PGHoardInotify")
         self.libc = ctypes.CDLL("libc.so.6", use_errno=True)
         self.fd = self.libc.inotify_init()
-        self.watch_to_path = {}
-        self.cookies = {}
+        self.watch_to_path: dict[int, str] = {}
+        self.cookies: dict[int, str] = {}
         self.running = True
         self.compression_queue = compression_queue
         self.timeout = 1.0
         self.log.debug("InotifyWatcher initialized")
 
-    def add_watch(self, path, events=None):
+    def add_watch(self, path: str, events: Optional[Iterable[str]] = None) -> None:
         mask = 0
         events = events or event_types.keys()
         for key in events:
             mask |= event_types[key]
         watch = self.libc.inotify_add_watch(self.fd, c_char_p(path.encode("utf8")), c_uint32(mask))
         if watch < 0:
             errno = ctypes.get_errno()
             raise OSError(errno, os.strerror(errno))
         self.watch_to_path[watch] = path
         self.log.debug("Added watch for path: %r", path)
 
-    def read_events(self):
+    def read_events(self) -> None:
         event_buffer = None
         while self.running:
             with suppress(InterruptedError):
                 rlist, _, _ = select.select([self.fd], [], [], self.timeout)
                 if rlist:
                     for fd in rlist:
                         event_buffer = os.read(fd, INOTIFY_EVENT_BUFFER_SIZE)
@@ -89,26 +106,26 @@
         if not event_buffer:
             return
         for wd, mask, cookie, name in parse_inotify_buffer(event_buffer):
             if wd == -1:
                 continue
             self.create_event(wd, mask, cookie, name)
 
-    def log_event(self, ev_type, full_path):
+    def log_event(self, ev_type: str, full_path: AnyPath) -> None:
         if self.log.getEffectiveLevel() > logging.DEBUG:
             return
 
         try:
             st = os.stat(full_path)
         except:  # pylint: disable=bare-except
             st = None
 
         self.log.debug("event: %s %s, %r", full_path, ev_type, st)
 
-    def create_event(self, wd, mask, cookie, name):
+    def create_event(self, wd: int, mask: int, cookie: int, name: bytes) -> None:
         if mask & event_types["IN_IGNORED"]:
             # explicit removal of watch or dir, ignore
             return
 
         decoded_name = name.decode("utf8")
         watched_path = self.watch_to_path[wd]
         full_path = os.path.join(self.watch_to_path[wd], decoded_name)
@@ -144,13 +161,13 @@
                         "src_path": src_path,
                         "watched_path": watched_path,
                     }
                 )
             else:
                 self.compression_queue.put({"type": "CREATE", "full_path": full_path, "watched_path": watched_path})
 
-    def run(self):
+    def run(self) -> None:
         self.log.debug("Starting InotifyWatcher")
         while self.running:
             self.read_events()
         self.log.debug("Quitting InotifyWatcher")
         os.close(self.fd)
```

### Comparing `rohmu-1.0.9/rohmu/notifier/http.py` & `rohmu-1.1.0/rohmu/notifier/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/"""
+from __future__ import annotations
+
 from .interface import Notifier
 from dataclasses import dataclass
 from datetime import datetime, timezone
 from enum import Enum, unique
 from logging import getLogger
 from queue import Empty, Queue
 from requests.exceptions import RequestException
@@ -48,15 +50,15 @@
 class HTTPNotifyJob:
     url: str
     json: str
 
 
 def background_http_request(
     session: requests.Session,
-    queue: "Queue[HTTPNotifyJob]",
+    queue: Queue[HTTPNotifyJob],
     stop_event: threading.Event,
     stop_event_check_timeout: float,
 ) -> None:
     with session:
         while not stop_event.is_set():
             try:
                 notification = queue.get(timeout=stop_event_check_timeout)
@@ -81,15 +83,15 @@
                 # For non-transient errors the thread must kept running to consume from the queue,
                 # because there is no mechanism to stop producing to it. Hopefully the failure is
                 # fast enough that the queue won't grow faster than this threads consumes from it.
                 queue.task_done()
 
 
 def initialize_background_thread(
-    queue: Queue,
+    queue: Queue[HTTPNotifyJob],
     stop_event: threading.Event,
     stop_event_check_timeout: float = _CHECK_STOP_EVENT_TIMEOUT,
     session: Optional[requests.Session] = None,
 ) -> threading.Thread:
     thread_session = session or _get_requests_session()
     thread_args = (thread_session, queue, stop_event, stop_event_check_timeout)
     thread = threading.Thread(
@@ -108,15 +110,15 @@
     def __init__(
         self,
         url: str,
         stop_event_check_timeout: float = _CHECK_STOP_EVENT_TIMEOUT,
         session: Optional[requests.Session] = None,
     ) -> None:
         self._url = url
-        self._queue: "Queue[HTTPNotifyJob]" = Queue()
+        self._queue: Queue[HTTPNotifyJob] = Queue()
         self._stop_event = threading.Event()
         self._thread = initialize_background_thread(
             self._queue,
             self._stop_event,
             stop_event_check_timeout,
             session=session,
         )
@@ -126,15 +128,15 @@
         # because it has a strong reference to itself.
         self.close()
 
     def close(self) -> None:
         self._stop_event.set()
         self._thread.join(_THREAD_JOIN_TIMEOUT)
 
-    def object_created(self, key: str, size: Optional[int], metadata: Optional[dict]) -> None:
+    def object_created(self, key: str, size: Optional[int], metadata: Optional[dict[str, str]]) -> None:
         self._queue.put(
             HTTPNotifyJob(
                 self._url,
                 json.dumps(
                     {
                         "op": Operation.UPLOAD.value,
                         "key": key,
```

### Comparing `rohmu-1.0.9/rohmu/notifier/interface.py` & `rohmu-1.1.0/rohmu/notifier/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/"""
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from typing import Optional
 
 
 class Notifier(ABC):
     """This interface allows external code to be notified about object changes."""
 
     @abstractmethod
-    def object_created(self, key: str, size: Optional[int], metadata: Optional[dict]) -> None:
+    def object_created(self, key: str, size: Optional[int], metadata: Optional[dict[str, str]]) -> None:
         """Called when an object is created."""
 
     @abstractmethod
     def object_deleted(self, key: str) -> None:
         """Called when an object is deleted.
 
         Note: This may be called with each individual object as a side-effect
@@ -24,13 +26,13 @@
         """May be called when a tree is deleted.
 
         Note: Not every driver supports this operation, for those objects will
         be listed and deleted individually, in that case `object_deleted` is
         called instead.
         """
 
-    def object_copied(self, key: str, size: Optional[int], metadata: Optional[dict]) -> None:
+    def object_copied(self, key: str, size: Optional[int], metadata: Optional[dict[str, str]]) -> None:
         """Called when an object is copied."""
         self.object_created(key=key, size=size, metadata=metadata)
 
     def close(self) -> None:
         """Method used to clean resources of the notifier, if any."""
```

### Comparing `rohmu-1.0.9/rohmu/object_storage/google.py` & `rohmu-1.1.0/rohmu/object_storage/google.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,52 @@
 """
 rohmu - google cloud object store interface
 
 Copyright (c) 2016 Ohmu Ltd
 Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/
 See LICENSE for details
 """
-# pylint: disable=import-error, no-name-in-module
 
+from __future__ import annotations
+
+from ..common.models import ProxyInfo, StorageModel, StorageOperation
+from ..common.statsd import StatsClient, StatsdConfig
 from ..dates import parse_timestamp
-from ..errors import FileNotFoundFromStorageError, InvalidConfigurationError
+from ..errors import FileNotFoundFromStorageError, InvalidByteRangeError, InvalidConfigurationError
 from ..notifier.interface import Notifier
-from .base import BaseTransfer, get_total_memory, IterKeyItem, KEY_TYPE_OBJECT, KEY_TYPE_PREFIX
+from ..typing import AnyPath, Metadata
+from ..util import get_total_size_from_content_range
+from .base import (
+    BaseTransfer,
+    get_total_memory,
+    IncrementalProgressCallbackType,
+    IterKeyItem,
+    KEY_TYPE_OBJECT,
+    KEY_TYPE_PREFIX,
+    ProgressProportionCallbackType,
+)
 from contextlib import contextmanager
-from googleapiclient.discovery import build
+from googleapiclient.discovery import build, Resource
 from googleapiclient.errors import HttpError
-from googleapiclient.http import build_http, MediaFileUpload, MediaIoBaseDownload, MediaIoBaseUpload, MediaUpload
+from googleapiclient.http import (
+    build_http,
+    HttpRequest,
+    MediaDownloadProgress,
+    MediaIoBaseDownload,
+    MediaUpload,
+    MediaUploadProgress,
+)
 from http.client import IncompleteRead
-from io import BytesIO, FileIO
 from oauth2client import GOOGLE_TOKEN_URI
 from oauth2client.client import GoogleCredentials
-from typing import Optional
+from typing import Any, BinaryIO, Callable, Dict, Iterable, Iterator, Optional, TextIO, Tuple, TypeVar, Union
+from typing_extensions import Protocol
 
 import codecs
+import dataclasses
 import errno
 
 # NOTE: this import is not needed per-se, but it's imported here first to point the
 # user to the most important possible missing dependency
 import googleapiclient  # noqa pylint: disable=unused-import
 import httplib2
 import json
@@ -39,15 +60,17 @@
 try:
     from oauth2client.service_account import ServiceAccountCredentials
 
     ServiceAccountCredentials_from_dict = ServiceAccountCredentials.from_json_keyfile_dict
 except ImportError:
     from oauth2client.service_account import _ServiceAccountCredentials
 
-    def ServiceAccountCredentials_from_dict(credentials, scopes=None):
+    def ServiceAccountCredentials_from_dict(
+        credentials: dict[str, Any], scopes: Optional[list[str]] = None
+    ) -> GoogleCredentials:
         if scopes is None:
             scopes = []
         return _ServiceAccountCredentials(
             service_account_id=credentials["client_id"],
             service_account_email=credentials["client_email"],
             private_key_id=credentials["private_key_id"],
             private_key_pkcs8_text=credentials["private_key"],
@@ -59,19 +82,21 @@
 logging.getLogger("googleapiclient.discovery_cache").setLevel(logging.ERROR)
 logging.getLogger("googleapiclient").setLevel(logging.WARNING)
 logging.getLogger("oauth2client").setLevel(logging.WARNING)
 
 # googleapiclient download performs some 3-4 times better with 50 MB chunk size than 5 MB chunk size;
 # but decrypting/decompressing big chunks needs a lot of memory so use smaller chunks on systems with less
 # than 2 GB RAM
-DOWNLOAD_CHUNK_SIZE = 1024 * 1024 * 5 if get_total_memory() < 2048 else 1024 * 1024 * 50
+DOWNLOAD_CHUNK_SIZE = 1024 * 1024 * 5 if (get_total_memory() or 0) < 2048 else 1024 * 1024 * 50
 UPLOAD_CHUNK_SIZE = 1024 * 1024 * 5
 
 
-def get_credentials(credential_file=None, credentials=None):
+def get_credentials(
+    credential_file: Optional[TextIO] = None, credentials: Optional[dict[str, Any]] = None
+) -> GoogleCredentials:
     if credential_file:
         return GoogleCredentials.from_stream(credential_file)
 
     if credentials and credentials["type"] == "service_account":
         return ServiceAccountCredentials_from_dict(
             credentials,
             scopes=["https://www.googleapis.com/auth/cloud-platform"],
@@ -87,52 +112,111 @@
             token_uri=GOOGLE_TOKEN_URI,
             user_agent="pghoard",
         )
 
     return GoogleCredentials.get_application_default()
 
 
-def base64_to_hex(b64val):
+def base64_to_hex(b64val: Union[str, bytes]) -> str:
     if isinstance(b64val, str):
         b64val = b64val.encode("ascii")
     rawval = codecs.decode(b64val, "base64")
     hexval = codecs.encode(rawval, "hex")
     return hexval.decode("ascii")
 
 
-class GoogleTransfer(BaseTransfer):
+@dataclasses.dataclass
+class Reporter:
+    """Used for storing default and also reporting them accordingly
+
+    the whole point of this class is to handle different cases
+    - when file size is too small, reporting *_CHUNK_SIZE is wrong as 1000's of
+      small files over a long period (may be a month) is a lot of error
+    - Same is the case of _retry_on_reset
+    - This error extrapolates when replication is being used
+
+    size should ideally be min(real_size, *_CHUNK_SIZE). real_size is avaiable
+    when download or upload (from string or file), but when using FD, size is
+    not known so assuming something too big for small files is almost wrong and
+    in case it is bigger than CHUNKED then status reporting (from the
+    googleclient lib) should help get the correct sizes
+
+    """
+
+    operation: StorageOperation
+    size: Optional[int] = None
+    progress_prev: int = 0
+
+    def report(self, stats: StatsClient) -> None:
+        # reports the default.
+        # for sized operation, reporting after the operation is fine as _retry_on_reset will
+        # have reported the something already
+        # and if the operation eventually succeeds then report_status() or this will take care
+        # of it.
+        SIZED_OPERATIONS = {
+            StorageOperation.store_file: UPLOAD_CHUNK_SIZE,
+            StorageOperation.get_file: DOWNLOAD_CHUNK_SIZE,
+        }
+
+        if self.operation in SIZED_OPERATIONS:
+            size = self.size if self.size is not None else SIZED_OPERATIONS[self.operation]
+            stats.operation(operation=self.operation, size=size)
+        else:
+            stats.operation(operation=self.operation)
+
+    def report_status(self, stats: StatsClient, status: Union[MediaUploadProgress, MediaDownloadProgress]) -> None:
+        stats.operation(operation=self.operation, size=status.resumable_progress - self.progress_prev)
+        self.progress_prev = status.resumable_progress
+
+
+class Config(StorageModel):
+    project_id: str
+    bucket_name: str
+    credential_file: Optional[str] = None
+    credentials: Optional[Dict[str, Any]] = None
+    proxy_info: Optional[ProxyInfo] = None
+    prefix: Optional[str] = None
+
+
+ResType = TypeVar("ResType")
+
+
+class GoogleTransfer(BaseTransfer[Config]):
+    config_model = Config
+
     def __init__(
         self,
-        project_id,
-        bucket_name,
-        credential_file=None,
-        credentials=None,
-        prefix=None,
-        proxy_info=None,
+        project_id: str,
+        bucket_name: str,
+        credential_file: Optional[TextIO] = None,
+        credentials: Optional[dict[str, Any]] = None,
+        prefix: Optional[str] = None,
+        proxy_info: Optional[dict[str, Union[str, int]]] = None,
         notifier: Optional[Notifier] = None,
+        statsd_info: Optional[StatsdConfig] = None,
     ) -> None:
-        super().__init__(prefix=prefix, notifier=notifier)
+        super().__init__(prefix=prefix, notifier=notifier, statsd_info=statsd_info)
         self.project_id = project_id
         self.proxy_info = proxy_info
         self.google_creds = get_credentials(credential_file=credential_file, credentials=credentials)
-        self.gs = self._init_google_client()
+        self.gs: Optional[Resource] = self._init_google_client()
         self.gs_object_client = None
         self.bucket_name = self.get_or_create_bucket(bucket_name)
         self.log.debug("GoogleTransfer initialized")
 
-    def _init_google_client(self):
+    def _init_google_client(self) -> Resource:
         start_time = time.monotonic()
         delay = 2
         while True:
             http = build_http()
             if self.proxy_info:
                 if self.proxy_info.get("type") == "socks5":
-                    proxy_type = httplib2.socks.PROXY_TYPE_SOCKS5
+                    proxy_type = httplib2.socks.PROXY_TYPE_SOCKS5  # type: ignore [attr-defined]
                 else:
-                    proxy_type = httplib2.socks.PROXY_TYPE_HTTP
+                    proxy_type = httplib2.socks.PROXY_TYPE_HTTP  # type: ignore [attr-defined]
 
                 http.proxy_info = httplib2.ProxyInfo(
                     proxy_type,
                     self.proxy_info["host"],
                     self.proxy_info["port"],
                     proxy_user=self.proxy_info.get("user"),
                     proxy_pass=self.proxy_info.get("pass"),
@@ -149,38 +233,37 @@
                     raise
 
             # retry on DNS issues
             time.sleep(delay)
             delay = delay * 2
 
     @contextmanager
-    def _object_client(self, *, not_found=None):
+    def _object_client(self, *, not_found: Optional[str] = None) -> Iterator[Any]:
         """(Re-)initialize object client if required, handle 404 errors gracefully and reset the client on
         server errors.  Server errors have been shown to be caused by invalid state in the client and do not
         seem to be resolved without resetting."""
         if self.gs_object_client is None:
             if self.gs is None:
                 self.gs = self._init_google_client()
             # https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.objects.html
-            self.gs_object_client = self.gs.objects()  # pylint: disable=no-member
-
+            self.gs_object_client = self.gs.objects()  # type: ignore [attr-defined] # pylint: disable=no-member
         try:
             yield self.gs_object_client
         except HttpError as ex:
             if ex.resp["status"] == "404" and not_found is not None:
                 raise FileNotFoundFromStorageError(not_found)
             if ex.resp["status"] >= "500" and ex.resp["status"] <= "599":
                 self.log.error("Received server error %r, resetting Google API client", ex.resp["status"])
                 self.gs = None
                 self.gs_object_client = None
             raise
 
-    def _retry_on_reset(self, request, action):
+    def _retry_on_reset(self, request: HttpRequest, action: Callable[[], ResType], retry_reporter: Reporter) -> ResType:
         retries = 60
-        retry_wait = 2
+        retry_wait = 2.0
         while True:
             try:
                 return action()
             except (IncompleteRead, HttpError, ssl.SSLEOFError, socket.timeout, OSError, socket.gaierror) as ex:
                 # Note that socket.timeout and ssl.SSLEOFError inherit from OSError
                 # and the order of handling the errors here needs to be correct
                 if not retries:
@@ -198,71 +281,91 @@
                     raise
                 # getaddrinfo sometimes fails with "Name or service not known"
                 elif isinstance(ex, socket.gaierror) and ex.errno != socket.EAI_NONAME:
                     raise
 
                 self.log.warning("%s failed: %s (%s), retrying in %.2fs", action, ex.__class__.__name__, ex, retry_wait)
 
+            retry_reporter.report(self.stats)
+
             # we want to reset the http connection state in case of error
             if request and hasattr(request, "http"):
                 request.http.connections.clear()  # reset connection cache
 
             retries -= 1
             time.sleep(retry_wait)
 
-    def copy_file(self, *, source_key, destination_key, metadata=None, **_kwargs):
+    def copy_file(
+        self, *, source_key: str, destination_key: str, metadata: Optional[Metadata] = None, **_kwargs: Any
+    ) -> None:
         source_object = self.format_key_for_backend(source_key)
         destination_object = self.format_key_for_backend(destination_key)
         body = {}
         if metadata is not None:
             body["metadata"] = metadata
 
+        reporter = Reporter(StorageOperation.copy_file)
         with self._object_client(not_found=source_key) as clob:
             # https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.objects.html#copy
             request = clob.copy(
                 body=body,
                 destinationBucket=self.bucket_name,
                 destinationObject=destination_object,
                 sourceBucket=self.bucket_name,
                 sourceObject=source_object,
             )
-            result = self._retry_on_reset(request, request.execute)
+            result = self._retry_on_reset(request, request.execute, retry_reporter=reporter)
             if result.get("size", None) is not None:
-                self.notifier.object_copied(key=destination_key, size=int(result["size"]), metadata=metadata)
+                size = int(result["size"])
+                reporter.size = size
+                self.notifier.object_copied(key=destination_key, size=size, metadata=metadata)
+            reporter.report(self.stats)
 
-    def get_metadata_for_key(self, key):
+    def get_metadata_for_key(self, key: str) -> Metadata:
         path = self.format_key_for_backend(key)
         with self._object_client(not_found=path) as clob:
-            return self._metadata_for_key(clob, path)
+            return self._metadata_for_key(clob, path)[0]
 
-    def _metadata_for_key(self, clob, key):
+    def _metadata_for_key(self, clob: Any, key: str) -> tuple[dict[str, Any], int]:
         # https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.objects.html#get
         req = clob.get(bucket=self.bucket_name, object=key)
-        obj = self._retry_on_reset(req, req.execute)
-        return obj.get("metadata", {})
 
-    def _unpaginate(self, domain, initial_op, *, on_properties):
+        reporter = Reporter(StorageOperation.get_metadata_for_key)
+        obj = self._retry_on_reset(req, req.execute, retry_reporter=reporter)
+        reporter.report(self.stats)
+        return obj.get("metadata", {}), int(obj["size"])
+
+    def _unpaginate(
+        self, domain: Any, initial_op: Callable[[Any], Optional[HttpRequest]], *, on_properties: Iterable[str]
+    ) -> Iterator[tuple[str, Any]]:
         """Iterate thru the request pages until all items have been processed"""
         request = initial_op(domain)
         while request is not None:
-            result = self._retry_on_reset(request, request.execute)
+            reporter = Reporter(StorageOperation.iter_key)
+            result = self._retry_on_reset(request, request.execute, retry_reporter=reporter)
+            reporter.report(self.stats)
             for on_property in on_properties:
                 items = result.get(on_property)
                 if items is not None:
                     yield on_property, items
             request = domain.list_next(request, result)
 
     def iter_key(
-        self, key, *, with_metadata=True, deep=False, include_key=False  # pylint: disable=unused-argument, unused-variable
-    ):
+        self,
+        key: str,
+        *,
+        with_metadata: bool = True,  # pylint: disable=unused-argument
+        deep: bool = False,
+        include_key: bool = False,  # pylint: disable=unused-argument, unused-variable
+    ) -> Iterator[IterKeyItem]:
         path = self.format_key_for_backend(key, trailing_slash=not include_key)
         self.log.debug("Listing path %r", path)
         with self._object_client() as clob:
 
-            def initial_op(domain):
+            def initial_op(domain: Any) -> HttpRequest:
                 if deep:
                     kwargs = {}
                 else:
                     kwargs = {"delimiter": "/"}
                 # https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.objects.html#list
                 return domain.list(bucket=self.bucket_name, prefix=path, **kwargs)
 
@@ -285,182 +388,229 @@
                         )
                 elif property_name == "prefixes":
                     for prefix in items:
                         yield IterKeyItem(type=KEY_TYPE_PREFIX, value=self.format_key_from_backend(prefix).rstrip("/"))
                 else:
                     raise NotImplementedError(property_name)
 
-    def delete_key(self, key):
+    def delete_key(self, key: str) -> None:
         path = self.format_key_for_backend(key)
         self.log.debug("Deleting key: %r", path)
         with self._object_client(not_found=path) as clob:
             # https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.objects.html#delete
             req = clob.delete(bucket=self.bucket_name, object=path)
-            self._retry_on_reset(req, req.execute)
+            reporter = Reporter(StorageOperation.delete_key)
+            self._retry_on_reset(req, req.execute, retry_reporter=reporter)
+            reporter.report(self.stats)
             self.notifier.object_deleted(key)
 
-    def get_contents_to_file(self, key, filepath_to_store_to, *, progress_callback=None):
-        fileobj = FileIO(filepath_to_store_to, mode="wb")
-        done = False
-        metadata = {}
-        try:
-            metadata = self.get_contents_to_fileobj(key, fileobj, progress_callback=progress_callback)
-            done = True
-        finally:
-            fileobj.close()
-            if not done:
-                os.unlink(filepath_to_store_to)
-        return metadata
-
-    def get_contents_to_fileobj(self, key, fileobj_to_store_to, *, progress_callback=None):
+    def get_contents_to_fileobj(
+        self,
+        key: str,
+        fileobj_to_store_to: BinaryIO,
+        *,
+        byte_range: Optional[Tuple[int, int]] = None,
+        progress_callback: ProgressProportionCallbackType = None,
+    ) -> Metadata:
         path = self.format_key_for_backend(key)
         self.log.debug("Starting to fetch the contents of: %r to %r", path, fileobj_to_store_to)
         next_prog_report = 0.0
         last_log_output = 0.0
+        self._validate_byte_range(byte_range)
         with self._object_client(not_found=path) as clob:
+            metadata, obj_size = self._metadata_for_key(clob, path)
+            if byte_range is None:
+                size_to_download = obj_size
+            else:
+                size_to_download = min(obj_size - byte_range[0], byte_range[1] - byte_range[0] + 1)
+            reporter = Reporter(
+                StorageOperation.get_file,
+                size=min(size_to_download, DOWNLOAD_CHUNK_SIZE),
+            )
             # https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.objects.html#get_media
-            req = clob.get_media(bucket=self.bucket_name, object=path)
-            download = MediaIoBaseDownload(fileobj_to_store_to, req, chunksize=DOWNLOAD_CHUNK_SIZE)
+            req: HttpRequest = clob.get_media(bucket=self.bucket_name, object=path)
+            download: MediaDownloadProtocol
+            if byte_range is None:
+                download = MediaIoBaseDownload(fileobj_to_store_to, req, chunksize=DOWNLOAD_CHUNK_SIZE)
+            else:
+                download = MediaIoBaseDownloadWithByteRange(
+                    fileobj_to_store_to, req, chunksize=DOWNLOAD_CHUNK_SIZE, byte_range=byte_range
+                )
+
             done = False
             while not done:
-                status, done = self._retry_on_reset(getattr(download, "_request", None), download.next_chunk)
+                status, done = self._retry_on_reset(req, download.next_chunk, retry_reporter=reporter)
                 if status:
+                    reporter.report_status(self.stats, status)
                     progress_pct = status.progress() * 100
                     now = time.monotonic()
                     if (now - last_log_output) >= 5.0:
                         self.log.debug("Download of %r: %d%%", path, progress_pct)
                         last_log_output = now
 
                     if progress_callback and progress_pct > next_prog_report:
                         progress_callback(progress_pct, 100)
                         next_prog_report = progress_pct + 0.1
-            return self._metadata_for_key(clob, path)
-
-    def get_contents_to_string(self, key):
-        path = self.format_key_for_backend(key)
-        self.log.debug("Starting to fetch the contents of: %r", path)
-        with self._object_client(not_found=path) as clob:
-            # https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.objects.html#get_media
-            req = clob.get_media(bucket=self.bucket_name, object=path)
-            data = self._retry_on_reset(req, req.execute)
-            return data, self._metadata_for_key(clob, path)
+                elif done:
+                    reporter.report_status(self.stats, MediaDownloadProgress(size_to_download, size_to_download))
+                else:
+                    reporter.report(self.stats)
+            if progress_callback:
+                progress_callback(100, 100)
+            return metadata
 
-    def get_file_size(self, key):
+    def get_file_size(self, key: str) -> int:
         path = self.format_key_for_backend(key)
+        reporter = Reporter(StorageOperation.get_file_size)
         with self._object_client(not_found=path) as clob:
             # https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.objects.html#get
             req = clob.get(bucket=self.bucket_name, object=path)
-            obj = self._retry_on_reset(req, req.execute)
+            obj = self._retry_on_reset(req, req.execute, retry_reporter=reporter)
+            reporter.report(self.stats)
             return int(obj["size"])
 
-    def _upload(self, upload, key, metadata, extra_props, cache_control, upload_progress_fn=None):
+    def _upload(
+        self,
+        upload: MediaUpload,
+        key: str,
+        metadata: Metadata,
+        extra_props: Optional[dict[str, Any]],
+        cache_control: Optional[str],
+        reporter: Reporter,
+        upload_progress_fn: IncrementalProgressCallbackType = None,
+    ) -> dict[str, str]:
         path = self.format_key_for_backend(key)
         self.log.debug("Starting to upload %r", path)
-        body = {"metadata": metadata}
+        body: dict[str, Any] = {"metadata": metadata}
         if extra_props:
             body.update(extra_props)
         if cache_control is not None:
             body["cacheControl"] = cache_control
 
         last_log_output = 0.0
         with self._object_client() as clob:
             # https://googleapis.github.io/google-api-python-client/docs/dyn/storage_v1.objects.html#insert
             req = clob.insert(bucket=self.bucket_name, name=path, media_body=upload, body=body)
             response = None
             while response is None:
-                status, response = self._retry_on_reset(req, req.next_chunk)
+                status, response = self._retry_on_reset(req, req.next_chunk, retry_reporter=reporter)
                 if status:
+                    reporter.report_status(self.stats, status)
                     now = time.monotonic()
                     if (now - last_log_output) >= 5.0:
                         self.log.debug(
                             "Upload of %r to %r: %d%%, %s bytes",
                             upload,
                             path,
                             status.progress() * 100,
                             status.resumable_progress,
                         )
                         last_log_output = now
 
                     if upload_progress_fn:
                         upload_progress_fn(status.resumable_progress)
+                elif response is not None:
+                    reporter.report_status(self.stats, MediaUploadProgress(int(response["size"]), int(response["size"])))
+                else:
+                    reporter.report(self.stats)
         return response
 
     # pylint: disable=arguments-differ
-    def store_file_from_memory(self, key, memstring, metadata=None, extra_props=None, cache_control=None, mimetype=None):
-        data = BytesIO(memstring)
-        upload = MediaIoBaseUpload(data, mimetype or "application/octet-stream", chunksize=UPLOAD_CHUNK_SIZE, resumable=True)
-        sanitized_metadata = self.sanitize_metadata(metadata)
-        result = self._upload(upload, key, sanitized_metadata, extra_props, cache_control=cache_control)
-        self.notifier.object_created(key=key, size=int(result.get("size", len(memstring))), metadata=sanitized_metadata)
-        return result
-
-    # pylint: disable=arguments-differ
     def store_file_from_disk(
         self,
-        key,
-        filepath,
-        metadata=None,  # pylint: disable=arguments-differ, unused-variable
+        key: str,
+        filepath: AnyPath,
+        metadata: Optional[Metadata] = None,
         *,
-        multipart=None,
-        extra_props=None,  # pylint: disable=arguments-differ, unused-variable
-        cache_control=None,
-        mimetype=None
-    ):
-        mimetype = mimetype or "application/octet-stream"
-        upload = MediaFileUpload(filepath, mimetype, chunksize=UPLOAD_CHUNK_SIZE, resumable=True)
-        sanitized_metadata = self.sanitize_metadata(metadata)
-        result = self._upload(upload, key, sanitized_metadata, extra_props, cache_control=cache_control)
-        size = result.get("size", os.path.getsize(filepath))
-        self.notifier.object_created(key=key, size=int(size), metadata=sanitized_metadata)
-        return result
+        cache_control: Optional[str] = None,
+        mimetype: Optional[str] = None,
+        multipart: Optional[bool] = None,
+        progress_fn: ProgressProportionCallbackType = None,
+        extra_props: Optional[dict[str, Any]] = None,  # pylint: disable=arguments-differ
+    ) -> None:  # pylint: disable=unused-argument
+        # TODO: extra_props seems to be used only to set cacheControl in pghoard tests.
+        #
+        # When that is gone (.. long enough ..), we could get rid of
+        # this whole function and use the superclass default which
+        # falls back to store_file_object.
+        size = os.path.getsize(filepath)
+        with open(filepath, "rb") as fd:
+            metadata = metadata or {}
+            metadata.setdefault("Content-Length", size)
+            self.store_file_object(
+                key,
+                fd,
+                cache_control=cache_control,
+                metadata=metadata,
+                mimetype=mimetype,
+                multipart=multipart,
+                upload_progress_fn=self._incremental_to_proportional_progress(cb=progress_fn, size=size),
+                extra_props=extra_props,
+            )
 
-    def store_file_object(self, key, fd, *, cache_control=None, metadata=None, mimetype=None, upload_progress_fn=None):
+    def store_file_object(
+        self,
+        key: str,
+        fd: BinaryIO,
+        metadata: Optional[Metadata] = None,
+        *,
+        cache_control: Optional[str] = None,
+        mimetype: Optional[str] = None,
+        multipart: Optional[bool] = None,  # pylint: disable=unused-argument
+        upload_progress_fn: IncrementalProgressCallbackType = None,
+        extra_props: Optional[dict[str, Any]] = None,  # pylint: disable=arguments-differ
+    ) -> None:
         mimetype = mimetype or "application/octet-stream"
         sanitized_metadata = self.sanitize_metadata(metadata)
+        reporter = Reporter(StorageOperation.store_file)
         result = self._upload(
             MediaStreamUpload(fd, chunk_size=UPLOAD_CHUNK_SIZE, mime_type=mimetype, name=key),
             key,
             sanitized_metadata,
-            None,
+            extra_props,
             cache_control=cache_control,
             upload_progress_fn=upload_progress_fn,
+            reporter=reporter,
         )
         self.notifier.object_created(key=key, size=int(result["size"]), metadata=sanitized_metadata)
-        return result
 
-    def get_or_create_bucket(self, bucket_name):
+    def get_or_create_bucket(self, bucket_name: str) -> str:
         """Look up the bucket if it already exists and try to create the
         bucket in case it doesn't.  Note that we can't just always try to
         unconditionally create the bucket as Google imposes a strict rate
         limit on bucket creation operations, even if it doesn't result in a
         new bucket.
 
         Quietly handle the case where the bucket already exists to avoid
         race conditions.  Note that we'll get a 400 Bad Request response for
         invalid bucket names ("Invalid bucket name") as well as for invalid
         project ("Invalid argument"), try to handle both gracefully."""
         start_time = time.time()
-        gs_buckets = self.gs.buckets()  # pylint: disable=no-member
+        gs_buckets = self.gs.buckets()  # type: ignore [union-attr] # pylint: disable=no-member
         try:
             request = gs_buckets.get(bucket=bucket_name)
-            self._retry_on_reset(request, request.execute)
+            reporter = Reporter(StorageOperation.head_request)
+            self._retry_on_reset(request, request.execute, retry_reporter=reporter)
+            reporter.report(self.stats)
             self.log.debug("Bucket: %r already exists, took: %.3fs", bucket_name, time.time() - start_time)
         except HttpError as ex:
             if ex.resp["status"] == "404":
                 pass  # we need to create it
             elif ex.resp["status"] == "403":
                 raise InvalidConfigurationError("Bucket {0!r} exists but isn't accessible".format(bucket_name))
             else:
                 raise
         else:
             return bucket_name
 
         try:
             req = gs_buckets.insert(project=self.project_id, body={"name": bucket_name})
-            self._retry_on_reset(req, req.execute)
+            reporter = Reporter(StorageOperation.create_bucket)
+            self._retry_on_reset(req, req.execute, retry_reporter=reporter)
+            reporter.report(self.stats)
             self.log.debug("Created bucket: %r successfully, took: %.3fs", bucket_name, time.time() - start_time)
         except HttpError as ex:
             error = json.loads(ex.content.decode("utf-8"))["error"]
             if error["message"].startswith("You already own this bucket"):
                 self.log.debug("Bucket: %r already exists, took: %.3fs", bucket_name, time.time() - start_time)
             elif error["message"] == "Invalid argument.":
                 raise InvalidConfigurationError("Invalid project id {0!r}".format(self.project_id))
@@ -471,54 +621,54 @@
 
         return bucket_name
 
 
 class MediaStreamUpload(MediaUpload):
     """Support streaming arbitrary amount of data from non-seekable object supporting read method."""
 
-    def __init__(self, fd, *, chunk_size, mime_type, name):
+    def __init__(self, fd: BinaryIO, *, chunk_size: int, mime_type: str, name: str) -> None:
         self._data = b""
         self._next_chunk = b""
         self._chunk_size = chunk_size
         self._fd = fd
         self._mime_type = mime_type
         self._name = name
-        self._position = None
+        self._position: Optional[int] = None
 
-    def chunksize(self):
+    def chunksize(self) -> int:  # type: ignore [override]
         return self._chunk_size
 
-    def mimetype(self):
+    def mimetype(self) -> str:
         return self._mime_type
 
-    def size(self):
+    def size(self) -> Optional[int]:  # type: ignore [override]
         self.peek()
         if len(self._next_chunk) < self.peeksize:
             # The total file size should be returned if we have hit the final chunk.
             return (self._position or 0) + len(self._data) + len(self._next_chunk)
         return None
 
-    def resumable(self):
+    def resumable(self) -> bool:
         return True
 
     @property
-    def peeksize(self):
+    def peeksize(self) -> int:
         # Using 1 extra byte to avoid perfectly aligned file
         return self._chunk_size + 1
 
-    def peek(self):
+    def peek(self) -> None:
         """try to top up some data into _next_chunk"""
         if len(self._next_chunk) < self.peeksize:
             # top-up the _next_chunk
             self._next_chunk = self._read_bytes(self.peeksize - len(self._next_chunk), initial_data=self._next_chunk)
 
     # second parameter is length but baseclass incorrectly names it end
-    def getbytes(self, begin, length):  # pylint: disable=arguments-differ
+    def getbytes(self, begin: int, length: int) -> bytes:  # type: ignore [override] # pylint: disable=arguments-differ
         if begin < (self._position or 0):
-            msg = "Requested position {} for {!r} preceeds already fulfilled position {}".format(
+            msg = "Requested position {} for {!r} precedes already fulfilled position {}".format(
                 begin, self._name, self._position
             )
             raise IndexError(msg)
         elif begin > (self._position or 0) + len(self._data):
             msg = "Requested position {} for {!r} has gap from previous position {} and {} byte chunk".format(
                 begin, self._name, self._position, len(self._data)
             )
@@ -542,21 +692,21 @@
                 self._next_chunk = b""
                 self._data = self._read_bytes(length - len(retain_chunk), initial_data=retain_chunk)
 
         self.peek()
         self._position = begin
         return self._data
 
-    def has_stream(self):
+    def has_stream(self) -> bool:
         return False
 
-    def stream(self):
+    def stream(self) -> BinaryIO:  # type: ignore [override]
         raise NotImplementedError
 
-    def _read_bytes(self, length, *, initial_data=None):
+    def _read_bytes(self, length: int, *, initial_data: Optional[bytes] = None) -> bytes:
         bytes_remaining = length
         read_results = []
         if initial_data:
             read_results.append(initial_data)
         while bytes_remaining > 0:
             data = self._fd.read(bytes_remaining)
             if data:
@@ -567,7 +717,103 @@
 
         if not read_results:
             return b""
         elif len(read_results) == 1:
             return read_results[0]
         else:
             return b"".join(read_results)
+
+
+class MediaDownloadProtocol(Protocol):
+    def next_chunk(self) -> tuple[MediaDownloadProgress, bool]:
+        ...
+
+
+class MediaIoBaseDownloadWithByteRange:
+    """This class is mostly a copy of the googleapiclient's MediaIOBaseDownload class,
+    but with the addition of the support for fetching a specific byte_range.
+
+    """
+
+    def __init__(
+        self,
+        fd: BinaryIO,
+        request: HttpRequest,
+        chunksize: int = DOWNLOAD_CHUNK_SIZE,
+        *,
+        byte_range: tuple[int, int],
+    ) -> None:
+        """Constructor.
+
+        Args:
+          fd: io.Base or file object, The stream in which to write the downloaded
+            bytes.
+          request: googleapiclient.http.HttpRequest, the media request to perform in
+            chunks.
+          chunksize: int, File will be downloaded in chunks of this many bytes.
+          byte_range: tuple[int, int], The byterange to fetch
+        """
+        self._fd = fd
+        self._http = request.http
+        self._uri = request.uri
+        self._chunksize = chunksize
+        self._start_position, self._end_position = byte_range
+        self._num_bytes_downloaded = 0
+        self._range_size = self._end_position - self._start_position + 1
+        if self._range_size < 0:
+            raise InvalidByteRangeError(f"Invalid byte_range: {byte_range}. Start must be < end.")
+        self._done = False
+
+        self._headers = {}
+        for k, v in request.headers.items():
+            # allow users to supply custom headers by setting them on the request
+            # but strip out the ones that are set by default on requests generated by
+            # API methods like Drive's files().get(fileId=...)
+            if k.lower() not in ("accept", "accept-encoding", "user-agent"):
+                self._headers[k] = v
+
+    def next_chunk(self) -> tuple[MediaDownloadProgress, bool]:
+        """Get the next chunk of the download.
+
+        Returns:
+          (status, done): The value of done will be True when the media has been fully
+             downloaded or the total size of the media is unknown.
+
+        Raises:
+          googleapiclient.errors.HttpError if the response was not a 2xx (or a 416 is received and the file is empty)
+          httplib2.HttpLib2Error if a transport error has occurred.
+        """
+        headers = self._headers.copy()
+        chunk_start = self._num_bytes_downloaded + self._start_position
+        chunk_end = chunk_start + self._chunksize - 1
+        if self._end_position < chunk_end:
+            chunk_end = self._end_position
+        headers["range"] = f"bytes={chunk_start}-{chunk_end}"
+        resp, content = self._http.request(self._uri, "GET", headers=headers)
+
+        total_size: Optional[int] = None
+        if resp.status in (200, 206):
+            if "content-location" in resp and resp["content-location"] != self._uri:
+                self._uri = resp["content-location"]
+            self._num_bytes_downloaded += len(content)
+            self._fd.write(content)
+
+            if "content-range" in resp:
+                total_size = get_total_size_from_content_range(resp["content-range"])
+            elif "content-length" in resp:
+                # By RFC 9110 if we end up here this is a 200 OK response and this is the total size of the object
+                total_size = int(resp["content-length"])
+
+            size_to_download = (
+                self._range_size if total_size is None else min(self._range_size, total_size - self._start_position)
+            )
+            if self._num_bytes_downloaded == size_to_download:
+                self._done = True
+            return MediaDownloadProgress(self._num_bytes_downloaded, size_to_download), self._done
+        elif resp.status == 416:
+            # 416 is Range Not Satisfiable
+            # This typically occurs with a zero byte file
+            total_size = get_total_size_from_content_range(resp["content-range"])
+            if total_size == 0:
+                self._done = True
+                return MediaDownloadProgress(self._num_bytes_downloaded, total_size), self._done
+        raise HttpError(resp, content, uri=self._uri)
```

### Comparing `rohmu-1.0.9/rohmu/object_storage/local.py` & `rohmu-1.1.0/rohmu/object_storage/local.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,148 @@
 """
 rohmu - local filesystem interface
 
 Copyright (c) 2016 Ohmu Ltd
 Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/
 See LICENSE for details
 """
-from ..errors import FileNotFoundFromStorageError, LocalFileIsRemoteFileError
+from ..common.models import StorageModel
+from ..common.statsd import StatsdConfig
+from ..errors import FileNotFoundFromStorageError
 from ..notifier.interface import Notifier
-from .base import BaseTransfer, IterKeyItem, KEY_TYPE_OBJECT, KEY_TYPE_PREFIX
-from io import BytesIO
-from typing import Optional
+from ..typing import Metadata
+from .base import (
+    BaseTransfer,
+    IncrementalProgressCallbackType,
+    IterKeyItem,
+    KEY_TYPE_OBJECT,
+    KEY_TYPE_PREFIX,
+    ProgressProportionCallbackType,
+)
+from pathlib import Path
+from typing import Any, BinaryIO, Iterator, Optional, TextIO, Tuple, Union
 
 import contextlib
 import datetime
+import hashlib
 import json
 import os
 import shutil
 import tempfile
 
 CHUNK_SIZE = 1024 * 1024
+INTERNAL_METADATA_KEY_HASH = "_hash"
+INTERNAL_METADATA_KEYS = {INTERNAL_METADATA_KEY_HASH}
 
 
-class LocalTransfer(BaseTransfer):
+class Config(StorageModel):
+    directory: str
+    prefix: Optional[str] = None
+
+
+class LocalTransfer(BaseTransfer[Config]):
+    config_model = Config
+
+    is_thread_safe = True
+
     def __init__(
         self,
-        directory,
-        prefix=None,
+        directory: Union[str, Path],
+        prefix: Optional[str] = None,
         notifier: Optional[Notifier] = None,
+        statsd_info: Optional[StatsdConfig] = None,
     ) -> None:
         prefix = os.path.join(directory, (prefix or "").strip("/"))
-        super().__init__(prefix=prefix, notifier=notifier)
+        super().__init__(prefix=prefix, notifier=notifier, statsd_info=statsd_info)
         self.log.debug("LocalTransfer initialized")
 
-    def copy_file(self, *, source_key, destination_key, metadata=None, **_kwargs):
+    def copy_file(
+        self, *, source_key: str, destination_key: str, metadata: Optional[Metadata] = None, **_kwargs: Any
+    ) -> None:
         source_path = self.format_key_for_backend(source_key.strip("/"))
         destination_path = self.format_key_for_backend(destination_key.strip("/"))
         if not os.path.isfile(source_path):
             raise FileNotFoundFromStorageError(source_key)
         os.makedirs(os.path.dirname(destination_path), exist_ok=True)
         shutil.copy(source_path, destination_path)
         if metadata is None:
             shutil.copy(source_path + ".metadata", destination_path + ".metadata")
         else:
-            self._save_metadata(destination_path, metadata)
+            new_metadata = self._filter_internal_metadata(self._get_metadata_for_key(source_key))
+            new_metadata.update(metadata)
+            self._save_metadata(destination_path, new_metadata)
         self.notifier.object_copied(key=destination_key, size=os.path.getsize(destination_path), metadata=metadata)
 
-    def get_metadata_for_key(self, key):
+    def _get_metadata_for_key(self, key: str) -> Metadata:
         source_path = self.format_key_for_backend(key.strip("/"))
         if not os.path.exists(source_path):
             raise FileNotFoundFromStorageError(key)
         metadata_path = source_path + ".metadata"
         try:
             with open(metadata_path, "r") as fp:
                 return json.load(fp)
         except FileNotFoundError:
             raise FileNotFoundFromStorageError(key)
 
-    def delete_key(self, key):
+    def _filter_internal_metadata(self, metadata: Metadata) -> Metadata:
+        return {key: value for key, value in metadata.items() if key in INTERNAL_METADATA_KEYS}
+
+    def _filter_metadata(self, metadata: Metadata) -> Metadata:
+        return {key: value for key, value in metadata.items() if key not in INTERNAL_METADATA_KEYS}
+
+    def get_metadata_for_key(self, key: str) -> Metadata:
+        return self._filter_metadata(self._get_metadata_for_key(key))
+
+    def delete_key(self, key: str) -> None:
         self.log.debug("Deleting key: %r", key)
         target_path = self.format_key_for_backend(key.strip("/"))
         if not os.path.exists(target_path):
             raise FileNotFoundFromStorageError(key)
         os.unlink(target_path)
         metadata_tmp_path = target_path + ".metadata_tmp"
         with contextlib.suppress(FileNotFoundError):
             os.unlink(metadata_tmp_path)
         metadata_path = target_path + ".metadata"
         with contextlib.suppress(FileNotFoundError):
             os.unlink(metadata_path)
         self.notifier.object_deleted(key=key)
 
-    def delete_tree(self, key):
+    def delete_tree(self, key: str) -> None:
         self.log.debug("Deleting tree: %r", key)
         target_path = self.format_key_for_backend(key.strip("/"))
         if not os.path.isdir(target_path):
             raise FileNotFoundFromStorageError(key)
         shutil.rmtree(target_path)
         self.notifier.tree_deleted(key=key)
 
     @staticmethod
-    def _skip_file_name(file_name):
+    def _skip_file_name(file_name: str) -> bool:
         return file_name.startswith(".") or file_name.endswith(".metadata") or ".metadata_tmp" in file_name
 
-    @staticmethod
-    def _yield_object(key, full_path, with_metadata):
-        metadata_file = full_path + ".metadata"
-        if not os.path.exists(metadata_file):
+    def _yield_object(self, key: str, full_path: str, with_metadata: bool) -> Iterator[IterKeyItem]:
+        try:
+            metadata = self._get_metadata_for_key(key)
+        except FileNotFoundFromStorageError:
             return
-        if with_metadata:
-            with open(metadata_file, "r") as fp:
-                metadata = json.load(fp)
-        else:
-            metadata = None
         st = os.stat(full_path)
         last_modified = datetime.datetime.fromtimestamp(st.st_mtime, tz=datetime.timezone.utc)
         yield IterKeyItem(
             type=KEY_TYPE_OBJECT,
             value={
                 "name": key,
                 "size": st.st_size,
                 "last_modified": last_modified,
-                "metadata": metadata,
+                "md5": metadata[INTERNAL_METADATA_KEY_HASH],
+                "metadata": self._filter_metadata(metadata) if with_metadata else None,
             },
         )
 
-    def iter_key(self, key, *, with_metadata=True, deep=False, include_key=False):
+    def iter_key(
+        self, key: str, *, with_metadata: bool = True, deep: bool = False, include_key: bool = False
+    ) -> Iterator[IterKeyItem]:
         target_path = self.format_key_for_backend(key.strip("/"))
         try:
             input_files = os.listdir(target_path)
         except FileNotFoundError:
             return
         except NotADirectoryError:
             if include_key:
@@ -125,122 +159,97 @@
             if os.path.isdir(full_path):
                 file_key = os.path.join(key.strip("/"), file_name)
                 if deep:
                     yield from self.iter_key(file_key, with_metadata=with_metadata, deep=True)
                 else:
                     yield IterKeyItem(type=KEY_TYPE_PREFIX, value=file_key)
             else:
-                # Don't return files if metadata file is not present; files are written in two phases and
-                # should be considered available only after also metadata has been written
-                if not os.path.exists(full_path + ".metadata"):
-                    continue
                 yield from self._yield_object(
                     key=os.path.join(key.strip("/"), file_name),
                     full_path=full_path,
                     with_metadata=with_metadata,
                 )
 
-    def get_contents_to_file(self, key, filepath_to_store_to, *, progress_callback=None):
-        source_path = self.format_key_for_backend(key.strip("/"))
-        try:
-            src_stat = os.stat(source_path)
-        except FileNotFoundError:
-            raise FileNotFoundFromStorageError(key)
-        with contextlib.suppress(FileNotFoundError):
-            dst_stat = os.stat(filepath_to_store_to)
-            if dst_stat.st_dev == src_stat.st_dev and dst_stat.st_ino == src_stat.st_ino:
-                raise LocalFileIsRemoteFileError(source_path)
-        with open(filepath_to_store_to, "wb") as fileobj_to_store_to:
-            return self.get_contents_to_fileobj(key, fileobj_to_store_to, progress_callback=progress_callback)
-
-    def get_contents_to_fileobj(self, key, fileobj_to_store_to, *, progress_callback=None):
+    def get_contents_to_fileobj(
+        self,
+        key: str,
+        fileobj_to_store_to: BinaryIO,
+        *,
+        byte_range: Optional[Tuple[int, int]] = None,
+        progress_callback: ProgressProportionCallbackType = None,
+    ) -> Metadata:
+        self._validate_byte_range(byte_range)
         source_path = self.format_key_for_backend(key.strip("/"))
         if not os.path.exists(source_path):
             raise FileNotFoundFromStorageError(key)
 
         input_size = os.stat(source_path).st_size
         bytes_written = 0
         with open(source_path, "rb") as fp:
-            while True:
-                buf = fp.read(CHUNK_SIZE)
+            if byte_range:
+                fp.seek(byte_range[0])
+                input_size = byte_range[1] - byte_range[0] + 1
+            while bytes_written <= input_size:
+                left = min(input_size - bytes_written, CHUNK_SIZE)
+                buf = fp.read(left)
                 if not buf:
                     break
                 fileobj_to_store_to.write(buf)
                 bytes_written += len(buf)
                 if progress_callback:
                     progress_callback(bytes_written, input_size)
 
         return self.get_metadata_for_key(key)
 
-    def get_contents_to_string(self, key):
-        bio = BytesIO()
-        metadata = self.get_contents_to_fileobj(key, bio)
-        return bio.getvalue(), metadata
-
-    def get_file_size(self, key):
+    def get_file_size(self, key: str) -> int:
         source_path = self.format_key_for_backend(key.strip("/"))
         if not os.path.exists(source_path):
             raise FileNotFoundFromStorageError(key)
         return os.stat(source_path).st_size
 
-    def _save_metadata(self, target_path, metadata):
+    def _save_metadata(self, target_path: str, metadata: Optional[Metadata]) -> None:
         metadata_path = target_path + ".metadata"
         with atomic_create_file(metadata_path) as fp:
             json.dump(self.sanitize_metadata(metadata), fp)
 
-    def store_file_from_memory(self, key, memstring, metadata=None, cache_control=None, mimetype=None):
-        target_path = self.format_key_for_backend(key.strip("/"))
-        os.makedirs(os.path.dirname(target_path), exist_ok=True)
-        with open(target_path, "wb") as fp:
-            fp.write(memstring)
-        self._save_metadata(target_path, metadata)
-        self.notifier.object_created(key=key, size=os.path.getsize(target_path), metadata=self.sanitize_metadata(metadata))
-
-    def store_file_from_disk(self, key, filepath, metadata=None, multipart=None, cache_control=None, mimetype=None):
-        target_path = self.format_key_for_backend(key.strip("/"))
-        src_stat = os.stat(filepath)
-        with contextlib.suppress(FileNotFoundError):
-            dst_stat = os.stat(target_path)
-            if dst_stat.st_dev == src_stat.st_dev and dst_stat.st_ino == src_stat.st_ino:
-                self._save_metadata(target_path, metadata)
-                raise LocalFileIsRemoteFileError(target_path)
-        os.makedirs(os.path.dirname(target_path), exist_ok=True)
-        shutil.copyfile(filepath, target_path)
-        self._save_metadata(target_path, metadata)
-        self.notifier.object_created(key=key, size=os.path.getsize(target_path), metadata=self.sanitize_metadata(metadata))
-
     def store_file_object(
         self,
-        key,
-        fd,
+        key: str,
+        fd: BinaryIO,
+        metadata: Optional[Metadata] = None,
         *,
-        cache_control=None,  # pylint: disable=unused-argument
-        metadata=None,
-        mimetype=None,
-        upload_progress_fn=None
-    ):  # pylint: disable=unused-argument
+        cache_control: Optional[str] = None,  # pylint: disable=unused-argument
+        mimetype: Optional[str] = None,  # pylint: disable=unused-argument
+        multipart: Optional[bool] = None,  # pylint: disable=unused-argument
+        upload_progress_fn: IncrementalProgressCallbackType = None,
+    ) -> None:
         target_path = self.format_key_for_backend(key.strip("/"))
         os.makedirs(os.path.dirname(target_path), exist_ok=True)
         bytes_written = 0
+        m = hashlib.sha256()
         with open(target_path, "wb") as output_fp:
             while True:
                 data = fd.read(1024 * 1024)
                 if not data:
                     break
+                m.update(data)
                 output_fp.write(data)
                 bytes_written += len(data)
                 if upload_progress_fn:
                     upload_progress_fn(bytes_written)
-
+        metadata = metadata.copy() if metadata is not None else {}
+        metadata[INTERNAL_METADATA_KEY_HASH] = m.hexdigest()
         self._save_metadata(target_path, metadata)
-        self.notifier.object_created(key=key, size=os.path.getsize(target_path), metadata=self.sanitize_metadata(metadata))
+        self.notifier.object_created(
+            key=key, size=os.path.getsize(target_path), metadata=self.sanitize_metadata(self._filter_metadata(metadata))
+        )
 
 
 @contextlib.contextmanager
-def atomic_create_file(file_path):
+def atomic_create_file(file_path: str) -> Iterator[TextIO]:
     """Open a temporary file for writing, rename to final name when done"""
     fd, tmp_file_path = tempfile.mkstemp(
         prefix=os.path.basename(file_path), dir=os.path.dirname(file_path), suffix=".metadata_tmp"
     )
     try:
         with os.fdopen(fd, "w") as out_file:
             yield out_file
```

### Comparing `rohmu-1.0.9/rohmu/object_storage/s3.py` & `rohmu-1.1.0/rohmu/object_storage/s3.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,83 @@
 """
 rohmu - aws s3 object store interface
 
 Copyright (c) 2016 Ohmu Ltd
 Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/
 See LICENSE for details
 """
+
+from __future__ import annotations
+
+from ..common.models import ProxyInfo, StorageModel, StorageOperation
+from ..common.statsd import StatsdConfig
 from ..errors import FileNotFoundFromStorageError, InvalidConfigurationError, StorageError
 from ..notifier.interface import Notifier
-from .base import BaseTransfer, get_total_memory, IterKeyItem, KEY_TYPE_OBJECT, KEY_TYPE_PREFIX
-from typing import Dict, Optional
+from ..typing import Metadata
+from .base import (
+    BaseTransfer,
+    get_total_memory,
+    IncrementalProgressCallbackType,
+    IterKeyItem,
+    KEY_TYPE_OBJECT,
+    KEY_TYPE_PREFIX,
+    ProgressProportionCallbackType,
+)
+from botocore.response import StreamingBody
+from rohmu.util import batched
+from typing import Any, BinaryIO, cast, Collection, Iterator, Optional, Tuple, TYPE_CHECKING, Union
 
 import botocore.client
 import botocore.config
 import botocore.exceptions
 import botocore.session
 import math
-import os
 import time
 
+if TYPE_CHECKING:
+    from mypy_boto3_s3 import S3Client
+
 
-def calculate_chunk_size():
+# botocore typing stubs are incomplete. We either have to write all the stubs we need
+# or work around the problem a bit by importing the typing library only for type checking purposes.
+def create_s3_client(
+    *,
+    session: botocore.session.Session,
+    config: botocore.config.Config,
+    aws_access_key_id: Optional[str],
+    aws_secret_access_key: Optional[str],
+    aws_session_token: Optional[str],
+    region_name: str,
+    verify: Optional[bool | str] = None,
+    endpoint_url: Optional[str] = None,
+) -> S3Client:
+    s3_client = session.create_client(
+        "s3",
+        config=config,
+        aws_access_key_id=aws_access_key_id,
+        aws_secret_access_key=aws_secret_access_key,
+        aws_session_token=aws_session_token,
+        region_name=region_name,
+        verify=verify,
+        endpoint_url=endpoint_url,
+    )
+
+    if TYPE_CHECKING:
+        return cast(S3Client, s3_client)
+    else:
+        return s3_client
+
+
+def calculate_chunk_size() -> int:
     total_mem_mib = get_total_memory() or 0
     # At least 5 MiB, at most 524 MiB. Max block size used for hosts with ~210+ GB of memory
     return max(min(int(total_mem_mib / 400), 524), 5) * 1024 * 1024
 
 
-def get_proxy_url(proxy_info):
+def get_proxy_url(proxy_info: dict[str, Union[str, int]]) -> str:
     username = proxy_info.get("user")
     password = proxy_info.get("pass")
     if username and password:
         auth = f"{username}:{password}@"
     else:
         auth = ""
     host = proxy_info["host"]
@@ -46,51 +94,72 @@
 # files. Minimum chunk size is 5 MiB, which means max ~50 GB files can be uploaded. In order to get
 # to that 5 TiB increase the block size based on host memory; we don't want to use the max for all
 # hosts to avoid allocating too large portion of all available memory.
 MULTIPART_CHUNK_SIZE = calculate_chunk_size()
 READ_BLOCK_SIZE = 1024 * 1024 * 1
 
 
-class S3Transfer(BaseTransfer):
+class Config(StorageModel):
+    region: str
+    bucket_name: str
+    aws_access_key_id: Optional[str] = None
+    aws_secret_access_key: Optional[str] = None
+    prefix: Optional[str] = None
+    host: Optional[str] = None
+    port: Optional[str] = None
+    is_secure: bool = False
+    is_verify_tls: bool = False
+    segment_size: int = MULTIPART_CHUNK_SIZE
+    encrypted: bool = False
+    proxy_info: Optional[ProxyInfo] = None
+    connect_timeout: Optional[str] = None
+    read_timeout: Optional[str] = None
+    aws_session_token: Optional[str] = None
+
+
+class S3Transfer(BaseTransfer[Config]):
+    config_model = Config
+
     def __init__(
         self,
-        region,
-        bucket_name,
-        aws_access_key_id=None,
-        aws_secret_access_key=None,
-        prefix=None,
-        host=None,
-        port=None,
-        is_secure=False,
-        is_verify_tls=False,
-        segment_size=MULTIPART_CHUNK_SIZE,
-        encrypted=False,
-        proxy_info=None,
-        connect_timeout=None,
-        read_timeout=None,
+        region: str,
+        bucket_name: str,
+        aws_access_key_id: Optional[str] = None,
+        aws_secret_access_key: Optional[str] = None,
+        prefix: Optional[str] = None,
+        host: Optional[str] = None,
+        port: Optional[int] = None,
+        is_secure: bool = False,
+        is_verify_tls: bool = False,
+        segment_size: int = MULTIPART_CHUNK_SIZE,
+        encrypted: bool = False,
+        proxy_info: Optional[dict[str, Union[str, int]]] = None,
+        connect_timeout: Optional[float] = None,
+        read_timeout: Optional[float] = None,
         notifier: Optional[Notifier] = None,
         aws_session_token: Optional[str] = None,
+        statsd_info: Optional[StatsdConfig] = None,
     ) -> None:
-        super().__init__(prefix=prefix, notifier=notifier)
-        botocore_session = botocore.session.get_session()
+        super().__init__(prefix=prefix, notifier=notifier, statsd_info=statsd_info)
+        session = botocore.session.get_session()
         self.bucket_name = bucket_name
         self.location = ""
         self.region = region
-        timeouts = {}
+        timeouts: dict[str, Any] = {}
         if connect_timeout:
             timeouts["connect_timeout"] = connect_timeout
         if read_timeout:
             timeouts["read_timeout"] = read_timeout
         if not host or not port:
-            custom_config = {**timeouts}
+            custom_config: dict[str, Any] = {**timeouts}
             if proxy_info:
                 proxy_url = get_proxy_url(proxy_info)
                 custom_config["proxies"] = {"https": proxy_url}
-            self.s3_client = botocore_session.create_client(
-                "s3",
+            self.s3_client = create_s3_client(
+                session=session,
                 config=botocore.config.Config(**custom_config),
                 aws_access_key_id=aws_access_key_id,
                 aws_secret_access_key=aws_secret_access_key,
                 aws_session_token=aws_session_token,
                 region_name=region,
             )
             if self.region and self.region != "us-east-1":
@@ -99,25 +168,25 @@
             scheme = "https" if is_secure else "http"
             custom_url = "{scheme}://{host}:{port}".format(scheme=scheme, host=host, port=port)
             if self.region:
                 signature_version = "s3v4"
                 self.location = self.region
             else:
                 signature_version = "s3"
-            proxies: Optional[Dict[str, str]] = None
+            proxies: Optional[dict[str, str]] = None
             if proxy_info:
                 proxies = {"https": get_proxy_url(proxy_info)}
             boto_config = botocore.client.Config(
                 s3={"addressing_style": "path"},
                 signature_version=signature_version,
                 proxies=proxies,
                 **timeouts,
             )
-            self.s3_client = botocore_session.create_client(
-                "s3",
+            self.s3_client = create_s3_client(
+                session=session,
                 aws_access_key_id=aws_access_key_id,
                 aws_secret_access_key=aws_secret_access_key,
                 aws_session_token=aws_session_token,
                 config=boto_config,
                 endpoint_url=custom_url,
                 region_name=region,
                 verify=is_verify_tls,
@@ -125,17 +194,20 @@
 
         self.check_or_create_bucket()
 
         self.multipart_chunk_size = segment_size
         self.encrypted = encrypted
         self.log.debug("S3Transfer initialized")
 
-    def copy_file(self, *, source_key, destination_key, metadata=None, **_kwargs):
+    def copy_file(
+        self, *, source_key: str, destination_key: str, metadata: Optional[Metadata] = None, **_kwargs: Any
+    ) -> None:
         source_path = self.bucket_name + "/" + self.format_key_for_backend(source_key, remove_slash_prefix=True)
         destination_path = self.format_key_for_backend(destination_key, remove_slash_prefix=True)
+        self.stats.operation(StorageOperation.copy_file)
         try:
             self.s3_client.copy_object(
                 Bucket=self.bucket_name,
                 CopySource=source_path,
                 Key=destination_path,
                 Metadata=metadata or {},
                 MetadataDirective="COPY" if metadata is None else "REPLACE",
@@ -144,67 +216,75 @@
         except botocore.exceptions.ClientError as ex:
             status_code = ex.response.get("ResponseMetadata", {}).get("HTTPStatusCode")
             if status_code == 404:
                 raise FileNotFoundFromStorageError(source_key)
             else:
                 raise StorageError("Copying {!r} to {!r} failed: {!r}".format(source_key, destination_key, ex)) from ex
 
-    def get_metadata_for_key(self, key):
+    def get_metadata_for_key(self, key: str) -> Metadata:
         path = self.format_key_for_backend(key, remove_slash_prefix=True)
         return self._metadata_for_key(path)
 
-    def _metadata_for_key(self, key):
+    def _metadata_for_key(self, key: str) -> Metadata:
+        self.stats.operation(StorageOperation.metadata_for_key)
         try:
             response = self.s3_client.head_object(Bucket=self.bucket_name, Key=key)
         except botocore.exceptions.ClientError as ex:
             status_code = ex.response.get("ResponseMetadata", {}).get("HTTPStatusCode")
             if status_code == 404:
                 raise FileNotFoundFromStorageError(key)
             else:
                 raise StorageError("Metadata lookup failed for {}".format(key)) from ex
 
         return response["Metadata"]
 
-    def delete_key(self, key):
+    def delete_key(self, key: str) -> None:
         path = self.format_key_for_backend(key, remove_slash_prefix=True)
         self.log.debug("Deleting key: %r", path)
         self._metadata_for_key(path)  # check that key exists
+        self.stats.operation(StorageOperation.delete_key)
         self.s3_client.delete_object(Bucket=self.bucket_name, Key=path)
         self.notifier.object_deleted(key=key)
 
-    def delete_tree(self, key):
-        path = self.format_key_for_backend(key, remove_slash_prefix=True, trailing_slash=True)
-        self.log.debug("Deleting tree: %r", path)
-        objects_to_delete = self.s3_client.list_objects(Bucket=self.bucket_name, Prefix=path)
-        delete_keys = [{"Key": key} for key in [obj["Key"] for obj in objects_to_delete.get("Contents", [])]]
-        if delete_keys:
-            self.s3_client.delete_objects(Bucket=self.bucket_name, Delete={"Objects": delete_keys})
+    def delete_keys(self, keys: Collection[str]) -> None:
+        self.stats.operation(StorageOperation.delete_key, count=len(keys))
+        for batch in batched(keys, 1000):  # Cannot delete more than 1000 objects at a time
+            self.s3_client.delete_objects(
+                Bucket=self.bucket_name,
+                Delete={"Objects": [{"Key": self.format_key_for_backend(key, remove_slash_prefix=True)} for key in batch]},
+            )
             # Note: `tree_deleted` is not used here because the operation on S3 is not atomic, i.e.
             # it is possible for a new object to be created after `list_objects` above
-            for obj in delete_keys:
-                self.notifier.object_deleted(key=obj["Key"])
+            for key in batch:
+                self.notifier.object_deleted(key=key)
 
-    def iter_key(self, key, *, with_metadata=True, deep=False, include_key=False):
+    def iter_key(
+        self, key: str, *, with_metadata: bool = True, deep: bool = False, include_key: bool = False
+    ) -> Iterator[IterKeyItem]:
         path = self.format_key_for_backend(key, remove_slash_prefix=True, trailing_slash=not include_key)
         self.log.debug("Listing path %r", path)
         continuation_token = None
         while True:
-            args = {
+            args: dict[str, Any] = {
                 "Bucket": self.bucket_name,
                 "Prefix": path,
             }
             if not deep:
                 args["Delimiter"] = "/"
             if continuation_token:
                 args["ContinuationToken"] = continuation_token
+            self.stats.operation(StorageOperation.iter_key)
             response = self.s3_client.list_objects_v2(**args)
 
             for item in response.get("Contents", []):
                 if with_metadata:
-                    metadata = {k.lower(): v for k, v in self._metadata_for_key(item["Key"]).items()}
+                    try:
+                        metadata = {k.lower(): v for k, v in self._metadata_for_key(item["Key"]).items()}
+                    except FileNotFoundFromStorageError:
+                        continue
                 else:
                     metadata = None
                 name = self.format_key_from_backend(item["Key"])
                 yield IterKeyItem(
                     type=KEY_TYPE_OBJECT,
                     value={
                         "last_modified": item["LastModified"],
@@ -222,158 +302,140 @@
                 )
 
             if "NextContinuationToken" in response:
                 continuation_token = response["NextContinuationToken"]
             else:
                 break
 
-    def _get_object_stream(self, key):
+    def _get_object_stream(self, key: str, byte_range: Optional[tuple[int, int]]) -> tuple[StreamingBody, int, Metadata]:
         path = self.format_key_for_backend(key, remove_slash_prefix=True)
+        kwargs: dict[str, Any] = {}
+        if byte_range:
+            kwargs["Range"] = f"bytes {byte_range[0]}-{byte_range[1]}"
         try:
-            response = self.s3_client.get_object(
-                Bucket=self.bucket_name,
-                Key=path,
-            )
+            # Actual usage is accounted for in
+            # _read_object_to_fileobj, although that omits the initial
+            # get_object call if it fails.
+            response = self.s3_client.get_object(Bucket=self.bucket_name, Key=path, **kwargs)
         except botocore.exceptions.ClientError as ex:
             status_code = ex.response.get("ResponseMetadata", {}).get("HTTPStatusCode")
             if status_code == 404:
                 raise FileNotFoundFromStorageError(path)
             else:
                 raise StorageError("Fetching the remote object {} failed".format(path)) from ex
         return response["Body"], response["ContentLength"], response["Metadata"]
 
-    def _read_object_to_fileobj(self, fileobj, streaming_body, body_length, cb=None):
+    def _read_object_to_fileobj(
+        self, fileobj: BinaryIO, streaming_body: StreamingBody, body_length: int, cb: ProgressProportionCallbackType = None
+    ) -> None:
         data_read = 0
         while data_read < body_length:
             read_amount = body_length - data_read
             if read_amount > READ_BLOCK_SIZE:
                 read_amount = READ_BLOCK_SIZE
             data = streaming_body.read(amt=read_amount)
             fileobj.write(data)
             data_read += len(data)
             if cb:
                 cb(data_read, body_length)
+            self.stats.operation(operation=StorageOperation.get_file, size=len(data))
         if cb:
             cb(data_read, body_length)
 
-    def get_contents_to_file(self, key, filepath_to_store_to, *, progress_callback=None):
-        with open(filepath_to_store_to, "wb") as fh:
-            stream, length, metadata = self._get_object_stream(key)
-            self._read_object_to_fileobj(fh, stream, length, cb=progress_callback)
-        return metadata
-
-    def get_contents_to_fileobj(self, key, fileobj_to_store_to, *, progress_callback=None):
-        stream, length, metadata = self._get_object_stream(key)
+    def get_contents_to_fileobj(
+        self,
+        key: str,
+        fileobj_to_store_to: BinaryIO,
+        *,
+        byte_range: Optional[Tuple[int, int]] = None,
+        progress_callback: ProgressProportionCallbackType = None,
+    ) -> Metadata:
+        self._validate_byte_range(byte_range)
+        stream, length, metadata = self._get_object_stream(key, byte_range)
         self._read_object_to_fileobj(fileobj_to_store_to, stream, length, cb=progress_callback)
         return metadata
 
-    def get_contents_to_string(self, key):
-        stream, _, metadata = self._get_object_stream(key)
-        data = stream.read()
-        return data, metadata
-
-    def get_file_size(self, key):
+    def get_file_size(self, key: str) -> int:
         path = self.format_key_for_backend(key, remove_slash_prefix=True)
+        self.stats.operation(StorageOperation.get_file_size)
         try:
             response = self.s3_client.head_object(Bucket=self.bucket_name, Key=path)
             return int(response["ContentLength"])
         except botocore.exceptions.ClientError as ex:
             if ex.response.get("ResponseMetadata", {}).get("HTTPStatusCode") == 404:
                 raise FileNotFoundFromStorageError(path)
             else:
                 raise StorageError("File size lookup failed for {}".format(path)) from ex
 
-    def store_file_from_memory(self, key, memstring, metadata=None, cache_control=None, mimetype=None):
-        path = self.format_key_for_backend(key, remove_slash_prefix=True)
-        data = bytes(memstring)  # make sure Body is of type bytes as memoryview's not allowed, only bytes/bytearrays
-        args = {
-            "Bucket": self.bucket_name,
-            "Body": data,
-            "Key": path,
-        }
-        sanitized_metadata = metadata
-        if metadata:
-            sanitized_metadata = args["Metadata"] = self.sanitize_metadata(metadata)
-        if self.encrypted:
-            args["ServerSideEncryption"] = "AES256"
-        if cache_control is not None:
-            args["CacheControl"] = cache_control
-        if mimetype is not None:
-            args["ContentType"] = mimetype
-        self.s3_client.put_object(**args)
-        self.notifier.object_created(key=key, size=len(data), metadata=sanitized_metadata)
-
-    def store_file_from_disk(self, key, filepath, metadata=None, multipart=None, cache_control=None, mimetype=None):
-        size = os.path.getsize(filepath)
-        if not multipart or size <= self.multipart_chunk_size:
-            with open(filepath, "rb") as fh:
-                data = fh.read()
-                self.store_file_from_memory(key, data, metadata, cache_control=cache_control)
-            return
-
-        with open(filepath, "rb") as fp:
-            self.multipart_upload_file_object(
-                cache_control=cache_control, fp=fp, key=key, metadata=metadata, mimetype=mimetype, size=size
-            )
-            sanitized_metadata = self.sanitize_metadata(metadata)
-            self.notifier.object_created(key=key, size=size, metadata=sanitized_metadata)
-
-    def multipart_upload_file_object(self, *, cache_control, fp, key, metadata, mimetype, progress_fn=None, size=None):
+    def multipart_upload_file_object(
+        self,
+        *,
+        cache_control: Optional[str],
+        fp: BinaryIO,
+        key: str,
+        metadata: Optional[Metadata],
+        mimetype: Optional[str],
+        progress_fn: ProgressProportionCallbackType = None,
+        size: Optional[int] = None,
+    ) -> None:
         path = self.format_key_for_backend(key, remove_slash_prefix=True)
         start_of_multipart_upload = time.monotonic()
         bytes_sent = 0
 
-        chunks = "Unknown"
+        chunks: int = 1
         if size is not None:
             chunks = math.ceil(size / self.multipart_chunk_size)
         self.log.debug("Starting to upload multipart file: %r, size: %s, chunks: %s", path, size, chunks)
 
         parts = []
         part_number = 1
 
-        args = {
+        args: dict[str, Any] = {
             "Bucket": self.bucket_name,
             "Key": path,
         }
         sanitized_metadata = metadata
         if metadata:
             sanitized_metadata = args["Metadata"] = self.sanitize_metadata(metadata)
         if self.encrypted:
             args["ServerSideEncryption"] = "AES256"
         if cache_control is not None:
             args["CacheControl"] = cache_control
         if mimetype is not None:
             args["ContentType"] = mimetype
+        self.stats.operation(StorageOperation.create_multipart_upload)
         try:
-            response = self.s3_client.create_multipart_upload(**args)
+            cmu_response = self.s3_client.create_multipart_upload(**args)
         except botocore.exceptions.ClientError as ex:
             raise StorageError("Failed to initiate multipart upload for {}".format(path)) from ex
 
-        mp_id = response["UploadId"]
+        mp_id = cmu_response["UploadId"]
 
         while True:
             data = self._read_bytes(fp, self.multipart_chunk_size)
             if not data:
                 break
 
             attempts = 10
             start_of_part_upload = time.monotonic()
             while True:
                 attempts -= 1
+                self.stats.operation(StorageOperation.store_file, size=len(data))
                 try:
-                    response = self.s3_client.upload_part(
+                    cup_response = self.s3_client.upload_part(
                         Body=data,
                         Bucket=self.bucket_name,
                         Key=path,
                         PartNumber=part_number,
                         UploadId=mp_id,
                     )
                 except botocore.exceptions.ClientError as ex:
                     self.log.exception("Uploading part %d for %s failed, attempts left: %d", part_number, path, attempts)
                     if attempts <= 0:
+                        self.stats.operation(StorageOperation.multipart_aborted)
                         try:
                             self.s3_client.abort_multipart_upload(
                                 Bucket=self.bucket_name,
                                 Key=path,
                                 UploadId=mp_id,
                             )
                         finally:
@@ -387,33 +449,36 @@
                         part_number,
                         chunks,
                         len(data),
                         time.monotonic() - start_of_part_upload,
                     )
                     parts.append(
                         {
-                            "ETag": response["ETag"],
+                            "ETag": cup_response["ETag"],
                             "PartNumber": part_number,
                         }
                     )
                     part_number += 1
                     bytes_sent += len(data)
                     if progress_fn:
-                        progress_fn(bytes_sent)
+                        # TODO: change this to incremental progress. Size parameter is currently unused.
+                        progress_fn(bytes_sent, size)  # type: ignore [arg-type]
                     break
 
+        self.stats.operation(StorageOperation.multipart_complete)
         try:
             self.s3_client.complete_multipart_upload(
                 Bucket=self.bucket_name,
                 Key=path,
-                MultipartUpload={"Parts": parts},
+                MultipartUpload={"Parts": parts},  # type: ignore
                 UploadId=mp_id,
             )
         except botocore.exceptions.ClientError as ex:
             try:
+                self.stats.operation(StorageOperation.multipart_aborted)
                 self.s3_client.abort_multipart_upload(
                     Bucket=self.bucket_name,
                     Key=path,
                     UploadId=mp_id,
                 )
             finally:
                 raise StorageError("Failed to complete multipart upload for {}".format(path)) from ex
@@ -422,26 +487,77 @@
         self.log.info(
             "Multipart upload of %r complete, size: %r, took: %.2fs",
             path,
             size,
             time.monotonic() - start_of_multipart_upload,
         )
 
-    def store_file_object(self, key, fd, *, cache_control=None, metadata=None, mimetype=None, upload_progress_fn=None):
+    def store_file_from_memory(
+        self,
+        key: str,
+        memstring: bytes,
+        metadata: Optional[Metadata] = None,
+        *,
+        cache_control: Optional[str] = None,
+        mimetype: Optional[str] = None,
+        multipart: Optional[bool] = None,  # pylint: disable=unused-argument
+        progress_fn: ProgressProportionCallbackType = None,  # pylint: disable=unused-argument
+    ) -> None:
+        path = self.format_key_for_backend(key, remove_slash_prefix=True)
+        data = bytes(memstring)  # make sure Body is of type bytes as memoryview's not allowed, only bytes/bytearrays
+        args: dict[str, Any] = {
+            "Bucket": self.bucket_name,
+            "Body": data,
+            "Key": path,
+        }
+        sanitized_metadata = metadata
+        if metadata:
+            sanitized_metadata = args["Metadata"] = self.sanitize_metadata(metadata)
+        if self.encrypted:
+            args["ServerSideEncryption"] = "AES256"
+        if cache_control is not None:
+            args["CacheControl"] = cache_control
+        if mimetype is not None:
+            args["ContentType"] = mimetype
+        self.stats.operation(StorageOperation.store_file, size=len(data))
+        self.s3_client.put_object(**args)
+        self.notifier.object_created(key=key, size=len(data), metadata=sanitized_metadata)
+
+    def store_file_object(
+        self,
+        key: str,
+        fd: BinaryIO,
+        metadata: Optional[Metadata] = None,
+        *,
+        cache_control: Optional[str] = None,
+        mimetype: Optional[str] = None,
+        multipart: Optional[bool] = None,
+        upload_progress_fn: IncrementalProgressCallbackType = None,
+    ) -> None:  # pylint: disable=unused-argument
+        if not self._should_multipart(
+            chunk_size=self.multipart_chunk_size, default=True, metadata=metadata, multipart=multipart
+        ):
+            data = fd.read()
+            self.store_file_from_memory(key, data, metadata, cache_control=cache_control, mimetype=mimetype)
+            if upload_progress_fn:
+                upload_progress_fn(len(data))
+            return
+
         self.multipart_upload_file_object(
             cache_control=cache_control,
             fp=fd,
             key=key,
             metadata=metadata,
             mimetype=mimetype,
-            progress_fn=upload_progress_fn,
+            progress_fn=self._proportional_to_incremental_progress(upload_progress_fn),
         )
 
-    def check_or_create_bucket(self):
+    def check_or_create_bucket(self) -> None:
         create_bucket = False
+        self.stats.operation(StorageOperation.head_request)
         try:
             self.s3_client.head_bucket(Bucket=self.bucket_name)
         except botocore.exceptions.ClientError as ex:
             status_code = ex.response.get("ResponseMetadata", {}).get("HTTPStatusCode")
             if status_code == 301:
                 raise InvalidConfigurationError("Wrong region for bucket {}, check configuration".format(self.bucket_name))
             elif status_code == 403:
@@ -449,26 +565,27 @@
             elif status_code == 404:
                 create_bucket = True
             else:
                 raise
 
         if create_bucket:
             self.log.debug("Creating bucket: %r in location: %r", self.bucket_name, self.region)
-            args = {
+            args: dict[str, Any] = {
                 "Bucket": self.bucket_name,
             }
             if self.location:
                 args["CreateBucketConfiguration"] = {
                     "LocationConstraint": self.location,
                 }
 
+            self.stats.operation(StorageOperation.create_bucket)
             self.s3_client.create_bucket(**args)
 
     @classmethod
-    def _read_bytes(cls, stream, length):
+    def _read_bytes(cls, stream: BinaryIO, length: int) -> Optional[bytes]:
         bytes_remaining = length
         read_results = []
         while bytes_remaining > 0:
             data = stream.read(bytes_remaining)
             if data:
                 read_results.append(data)
                 bytes_remaining -= len(data)
```

### Comparing `rohmu-1.0.9/rohmu/object_storage/sftp.py` & `rohmu-1.1.0/rohmu/object_storage/sftp.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,41 +2,63 @@
 rohmu - sftp object store interface
 
 Copyright (c) 2016 Ohmu Ltd
 Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/
 See LICENSE for details
 """
 
-from ..errors import FileNotFoundFromStorageError, InvalidConfigurationError, StorageError
+from ..common.models import StorageModel
+from ..common.statsd import StatsdConfig
+from ..errors import FileNotFoundFromStorageError, InvalidConfigurationError
 from ..notifier.interface import Notifier
-from .base import BaseTransfer, IterKeyItem, KEY_TYPE_OBJECT, KEY_TYPE_PREFIX
-from io import BytesIO, StringIO
+from ..typing import Metadata
+from .base import (
+    BaseTransfer,
+    IncrementalProgressCallbackType,
+    IterKeyItem,
+    KEY_TYPE_OBJECT,
+    KEY_TYPE_PREFIX,
+    ProgressProportionCallbackType,
+)
+from io import BytesIO
 from stat import S_ISDIR
-from typing import cast, Optional
+from typing import Any, BinaryIO, cast, Iterator, Optional, Tuple
 
 import datetime
 import json
 import logging
 import os
 import paramiko
 import warnings
 
 
-class SFTPTransfer(BaseTransfer):
+class Config(StorageModel):
+    server: str
+    port: int
+    username: str
+    password: Optional[str] = None
+    private_key: Optional[str] = None
+    prefix: Optional[str] = None
+
+
+class SFTPTransfer(BaseTransfer[Config]):
+    config_model = Config
+
     def __init__(
         self,
-        server,
-        port,
-        username,
-        password=None,
-        private_key=None,
-        prefix=None,
+        server: str,
+        port: int,
+        username: str,
+        password: Optional[str] = None,
+        private_key: Optional[str] = None,
+        prefix: Optional[str] = None,
         notifier: Optional[Notifier] = None,
+        statsd_info: Optional[StatsdConfig] = None,
     ) -> None:
-        super().__init__(prefix=prefix, notifier=notifier)
+        super().__init__(prefix=prefix, notifier=notifier, statsd_info=statsd_info)
         self.server = server
         self.port = port
         self.username = username
         self.password = password
         self.private_key = private_key
 
         if not password and not private_key:
@@ -45,64 +67,68 @@
         logging.getLogger("paramiko").setLevel(logging.WARNING)
 
         # https://github.com/paramiko/paramiko/issues/1386#issuecomment-470847772
         warnings.filterwarnings(action="ignore", module=".*paramiko.*")
 
         transport = paramiko.Transport((self.server, self.port))
 
-        if private_key:
+        if self.private_key:
             pkey = paramiko.RSAKey.from_private_key_file(self.private_key)
             transport.connect(username=self.username, pkey=pkey)
         else:  # password must be defined due to previous check above
             transport.connect(username=self.username, password=self.password)
 
         self.client = cast(paramiko.SFTPClient, paramiko.SFTPClient.from_transport(transport))
 
         self.log.debug("SFTPTransfer initialized")
 
-    def get_contents_to_file(self, key, filepath_to_store_to, *, progress_callback=None):
-        with open(filepath_to_store_to, "wb") as fh:
-            return self.get_contents_to_fileobj(key, fh, progress_callback=progress_callback)
-
-    def get_contents_to_fileobj(self, key, fileobj_to_store_to, *, progress_callback=None):
+    def get_contents_to_fileobj(
+        self,
+        key: str,
+        fileobj_to_store_to: BinaryIO,
+        *,
+        byte_range: Optional[Tuple[int, int]] = None,
+        progress_callback: ProgressProportionCallbackType = None,
+    ) -> Metadata:
+        if byte_range:
+            raise NotImplementedError("byte range fetching not supported")
         self._get_contents_to_fileobj(key, fileobj_to_store_to, progress_callback)
         return self.get_metadata_for_key(key)
 
-    def _get_contents_to_fileobj(self, key, fileobj_to_store_to, progress_callback=None):
+    def _get_contents_to_fileobj(
+        self, key: str, fileobj_to_store_to: BinaryIO, progress_callback: ProgressProportionCallbackType = None
+    ) -> None:
         target_path = self.format_key_for_backend(key.strip("/"))
         self.log.debug("Get file content: %r", target_path)
 
         try:
             # the paramiko progress callback has the same interface as pghoard for downloads
-            return self.client.getfo(remotepath=target_path, fl=fileobj_to_store_to, callback=progress_callback)
+            self.client.getfo(remotepath=target_path, fl=fileobj_to_store_to, callback=progress_callback)
         except FileNotFoundError as ex:
             raise FileNotFoundFromStorageError(key) from ex
 
-    def get_contents_to_string(self, key):
-        bio = BytesIO()
-        metadata = self.get_contents_to_fileobj(key, bio)
-        return bio.getvalue(), metadata
-
-    def get_file_size(self, key):
+    def get_file_size(self, key: str) -> int:
         target_path = self.format_key_for_backend(key.strip("/"))
         try:
-            return self.client.stat(target_path).st_size
+            return self.client.stat(target_path).st_size  # type: ignore
         except FileNotFoundError as ex:
             raise FileNotFoundFromStorageError(key) from ex
 
-    def get_metadata_for_key(self, key):
+    def get_metadata_for_key(self, key: str) -> Metadata:
         bio = BytesIO()
         self._get_contents_to_fileobj(key + ".metadata", bio)
         return json.loads(bio.getvalue().decode())
 
     @staticmethod
-    def _skip_file_name(file_name):
+    def _skip_file_name(file_name: str) -> bool:
         return file_name.startswith(".") or file_name.endswith(".metadata") or ".metadata_tmp" in file_name
 
-    def iter_key(self, key, *, with_metadata=True, deep=False, include_key=False):
+    def iter_key(
+        self, key: str, *, with_metadata: bool = True, deep: bool = False, include_key: bool = False
+    ) -> Iterator[IterKeyItem]:
         target_path = self.format_key_for_backend(key.strip("/"))
         self.log.debug("Listing path: %r", target_path)
 
         try:
             attrs = self.client.listdir_attr(target_path)
         except FileNotFoundError:  # if not a directory will throw exception
             if include_key:
@@ -114,15 +140,17 @@
                     attr = self.client.stat(target_path)
 
                     if with_metadata:
                         metadata = self.get_metadata_for_key(key)
                     else:
                         metadata = None
 
-                    last_modified = datetime.datetime.fromtimestamp(attr.st_mtime, tz=datetime.timezone.utc)
+                    last_modified = datetime.datetime.fromtimestamp(
+                        attr.st_mtime, tz=datetime.timezone.utc  # type: ignore [arg-type]
+                    )
                     yield IterKeyItem(
                         type=KEY_TYPE_OBJECT,
                         value={
                             "name": key,
                             "size": attr.st_size,
                             "last_modified": last_modified,
                             "metadata": metadata,
@@ -137,104 +165,113 @@
         files = set(attr.filename for attr in attrs)
 
         for attr in attrs:
             if self._skip_file_name(attr.filename):
                 continue
 
             file_key = os.path.join(key.strip("/"), attr.filename)
-            if S_ISDIR(attr.st_mode):
+            if S_ISDIR(attr.st_mode):  # type: ignore [arg-type]
                 if deep:
                     yield from self.iter_key(file_key, with_metadata=with_metadata, deep=True)
                 else:
                     yield IterKeyItem(type=KEY_TYPE_PREFIX, value=file_key)
             else:
                 # Don't return files if metadata file is not present; files are written in two phases and
                 # should be considered available only after also metadata has been written
                 if attr.filename + ".metadata" in files:
                     if with_metadata:
                         metadata = self.get_metadata_for_key(file_key)
                     else:
                         metadata = None
 
-                    last_modified = datetime.datetime.fromtimestamp(attr.st_mtime, tz=datetime.timezone.utc)
+                    last_modified = datetime.datetime.fromtimestamp(
+                        attr.st_mtime, tz=datetime.timezone.utc  # type: ignore [arg-type]
+                    )
                     yield IterKeyItem(
                         type=KEY_TYPE_OBJECT,
                         value={
                             "name": file_key,
                             "size": attr.st_size,
                             "last_modified": last_modified,
                             "metadata": metadata,
                         },
                     )
 
     # can't support remote copy, only remote rename
-    def copy_file(self, *, source_key, destination_key, metadata=None, **_kwargs):
+    def copy_file(
+        self, *, source_key: str, destination_key: str, metadata: Optional[Metadata] = None, **_kwargs: Any
+    ) -> None:
         raise NotImplementedError
 
-    def delete_key(self, key):
+    def delete_key(self, key: str) -> None:
         target_path = self.format_key_for_backend(key.strip("/"))
         self.log.info("Removing path: %r", target_path)
 
         try:
             self.client.remove(target_path + ".metadata")
             self.client.remove(target_path)
             self.notifier.object_deleted(key=key)
         except FileNotFoundError as ex:
             raise FileNotFoundFromStorageError(key) from ex
 
-    # pylint: disable=unused-argument
-    def store_file_from_memory(self, key, memstring, metadata=None, cache_control=None, mimetype=None):
-        data = bytes(memstring)
-        bio = BytesIO(data)
-        try:
-            self._put_object(key=key, fd=bio, metadata=metadata)
-            self.notifier.object_created(key=key, size=len(data), metadata=self.sanitize_metadata(metadata))
-        except OSError as ex:
-            raise StorageError(key) from ex
-
-    def store_file_from_disk(self, key, filepath, metadata=None, multipart=None, cache_control=None, mimetype=None):
-        with open(filepath, "rb") as fh:
-            self._put_object(key=key, fd=fh, metadata=metadata)
-            self.notifier.object_created(
-                key=key, size=os.fstat(fh.fileno()).st_size, metadata=self.sanitize_metadata(metadata)
-            )
-
-    def store_file_object(self, key, fd, *, cache_control=None, metadata=None, mimetype=None, upload_progress_fn=None):
-        bytes_written = self._put_object(key, fd, metadata=metadata, upload_progress_fn=upload_progress_fn)
+    def store_file_object(
+        self,
+        key: str,
+        fd: BinaryIO,
+        metadata: Optional[Metadata] = None,
+        *,
+        cache_control: Optional[str] = None,  # pylint: disable=unused-argument
+        mimetype: Optional[str] = None,  # pylint: disable=unused-argument
+        multipart: Optional[bool] = None,  # pylint: disable=unused-argument
+        upload_progress_fn: IncrementalProgressCallbackType = None,
+    ) -> None:
+        bytes_written = self._put_object(
+            key, fd, metadata=metadata, upload_progress_fn=self._proportional_to_incremental_progress(upload_progress_fn)
+        )
         self.notifier.object_created(key=key, size=bytes_written, metadata=self.sanitize_metadata(metadata))
+        if upload_progress_fn:
+            upload_progress_fn(bytes_written)
 
-    def _put_object(self, key, fd, *, metadata=None, upload_progress_fn=None) -> int:
+    def _put_object(
+        self,
+        key: str,
+        fd: BinaryIO,
+        *,
+        metadata: Optional[Metadata] = None,
+        upload_progress_fn: ProgressProportionCallbackType = None,
+    ) -> int:
         target_path = self.format_key_for_backend(key.strip("/"))
-        total_bytes_written = [0]
+        total_bytes_written = 0
 
         self.log.debug("Store path: %r", target_path)
 
-        def wrapper_upload_progress_fn(bytes_written, total_bytes):  # pylint: disable=unused-argument
-            total_bytes_written[0] = bytes_written
+        def wrapper_upload_progress_fn(bytes_written: int, total_bytes: int) -> None:
+            nonlocal total_bytes_written
+            total_bytes_written = bytes_written
             if upload_progress_fn:
-                upload_progress_fn(bytes_written)
+                upload_progress_fn(bytes_written, total_bytes)
 
         self._mkdir_p(os.path.dirname(target_path))
         self.client.putfo(fl=fd, remotepath=target_path, callback=wrapper_upload_progress_fn)
 
         # metadata is saved last, because we ignore data files until the metadata file exists
         # see iter_key above
         self._save_metadata(target_path, metadata)
-        return total_bytes_written[0]
+        return total_bytes_written
 
-    def _save_metadata(self, target_path, metadata):
+    def _save_metadata(self, target_path: str, metadata: Optional[Metadata]) -> None:
         metadata_path = target_path + ".metadata"
         self.log.debug("Save metadata: %r", metadata_path)
 
         sanitised = self.sanitize_metadata(metadata)
-        bio = StringIO(json.dumps(sanitised))
+        bio = BytesIO(json.dumps(sanitised).encode())
         self.client.putfo(fl=bio, remotepath=metadata_path)
 
     # https://stackoverflow.com/questions/14819681/upload-files-using-sftp-in-python-but-create-directories-if-path-doesnt-exist
-    def _mkdir_p(self, remote):
+    def _mkdir_p(self, remote: str) -> None:
         dirs_ = []
         dir_ = remote
         while len(dir_) > 1:
             dirs_.append(dir_)
             dir_, _ = os.path.split(dir_)
 
         if len(dir_) == 1 and not dir_.startswith("/"):
```

### Comparing `rohmu-1.0.9/rohmu/object_storage/swift.py` & `rohmu-1.1.0/rohmu/object_storage/swift.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 """
 rohmu - openstack swift object store interface
 
 Copyright (c) 2016 Ohmu Ltd
 Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/
 See LICENSE for details
 """
+
+from __future__ import annotations
+
+from ..common.models import StorageModel
+from ..common.statsd import StatsdConfig
 from ..dates import parse_timestamp
 from ..errors import FileNotFoundFromStorageError
 from ..notifier.interface import Notifier
-from .base import BaseTransfer, IterKeyItem, KEY_TYPE_OBJECT, KEY_TYPE_PREFIX
+from ..typing import Metadata
+from .base import (
+    BaseTransfer,
+    IncrementalProgressCallbackType,
+    IterKeyItem,
+    KEY_TYPE_OBJECT,
+    KEY_TYPE_PREFIX,
+    ProgressProportionCallbackType,
+)
 from contextlib import suppress
 from swiftclient import client, exceptions  # pylint: disable=import-error
-from typing import Optional
+from typing import Any, BinaryIO, Iterator, Optional, Tuple
 
 import logging
 import os
 import time
 
 CHUNK_SIZE = 1024 * 1024 * 5  # 5 Mi
 SEGMENT_SIZE = 1024 * 1024 * 1024 * 3  # 3 Gi
 
 
 # Swift client logs excessively at INFO level, outputting things like a curl
 # command line to recreate the request that failed with a simple 404 error.
 # At WARNING level curl commands are not logged, but we get a full ugly
 # traceback for all failures, including 404s.  Monkey-patch them away.
-def swift_exception_logger(err):
+def swift_exception_logger(err: BaseException) -> Any:
     if not isinstance(err, exceptions.ClientException):
         return orig_swift_exception_logger(err)
     if getattr(err, "http_status", None) is None:
         return orig_swift_exception_logger(err)
     if err.http_status == 404 and err.msg.startswith("Object GET failed"):
         client.logger.debug("GET %r FAILED: %r", err.http_path, err.http_status)
     else:
@@ -38,41 +51,65 @@
 
 
 orig_swift_exception_logger = client.logger.exception
 client.logger.exception = swift_exception_logger
 logging.getLogger("swiftclient").setLevel(logging.WARNING)
 
 
-class SwiftTransfer(BaseTransfer):
+class Config(StorageModel):
+    user: str
+    key: str
+    container_name: str
+    auth_url: str
+    auth_version: str = "2.0"
+    tenant_name: Optional[str] = None
+    segment_size: int = SEGMENT_SIZE
+    region_name: Optional[str] = None
+    user_id: Optional[str] = None
+    user_domain_id: Optional[str] = None
+    user_domain_name: Optional[str] = None
+    tenant_id: Optional[str] = None
+    project_id: Optional[str] = None
+    project_name: Optional[str] = None
+    project_domain_id: Optional[str] = None
+    project_domain_name: Optional[str] = None
+    service_type: Optional[str] = None
+    endpoint_type: Optional[str] = None
+
+
+class SwiftTransfer(BaseTransfer[Config]):
+    config_model = Config
+
     def __init__(
         self,
         *,
-        user,
-        key,
-        container_name,
-        auth_url,
-        auth_version="2.0",
-        tenant_name=None,
-        prefix=None,
-        segment_size=SEGMENT_SIZE,
-        region_name=None,
-        user_id=None,
-        user_domain_id=None,
-        user_domain_name=None,
-        tenant_id=None,
-        project_id=None,
-        project_name=None,
-        project_domain_id=None,
-        project_domain_name=None,
-        service_type=None,
-        endpoint_type=None,
+        user: str,
+        key: str,
+        container_name: str,
+        auth_url: str,
+        auth_version: str = "2.0",
+        tenant_name: Optional[str] = None,
+        prefix: Optional[str] = None,
+        segment_size: int = SEGMENT_SIZE,
+        region_name: Optional[str] = None,
+        user_id: Optional[str] = None,
+        user_domain_id: Optional[str] = None,
+        user_domain_name: Optional[str] = None,
+        tenant_id: Optional[str] = None,
+        project_id: Optional[str] = None,
+        project_name: Optional[str] = None,
+        project_domain_id: Optional[str] = None,
+        project_domain_name: Optional[str] = None,
+        service_type: Optional[str] = None,
+        endpoint_type: Optional[str] = None,
         notifier: Optional[Notifier] = None,
+        statsd_info: Optional[StatsdConfig] = None,
     ) -> None:
         prefix = prefix.lstrip("/") if prefix else ""
-        super().__init__(prefix=prefix, notifier=notifier)
+        super().__init__(prefix=prefix, notifier=notifier, statsd_info=statsd_info)
         self.container_name = container_name
 
         if auth_version == "3.0":
             os_options = {
                 "region_name": region_name,
                 "user_id": user_id,
                 "user_domain_id": user_domain_id,
@@ -95,26 +132,26 @@
             user=user, key=key, authurl=auth_url, tenant_name=tenant_name, auth_version=auth_version, os_options=os_options
         )
         self.container = self.get_or_create_container(self.container_name)
         self.segment_size = segment_size
         self.log.debug("SwiftTransfer initialized")
 
     @staticmethod
-    def _headers_to_metadata(headers):
+    def _headers_to_metadata(headers: dict[str, str]) -> Metadata:
         return {name[len("x-object-meta-") :]: value for name, value in headers.items() if name.startswith("x-object-meta-")}
 
     @staticmethod
-    def _metadata_to_headers(metadata):
+    def _metadata_to_headers(metadata: Metadata) -> dict[str, str]:
         return {"x-object-meta-{}".format(name): str(value) for name, value in metadata.items()}
 
-    def get_metadata_for_key(self, key):
+    def get_metadata_for_key(self, key: str) -> Metadata:
         path = self.format_key_for_backend(key)
         return self._metadata_for_key(path)
 
-    def _metadata_for_key(self, key, *, resolve_manifest=False):
+    def _metadata_for_key(self, key: str, *, resolve_manifest: bool = False) -> Metadata:
         try:
             headers = self.conn.head_object(self.container_name, key)
         except exceptions.ClientException as ex:
             if ex.http_status == 404:
                 raise FileNotFoundFromStorageError(key)
             raise
 
@@ -125,15 +162,17 @@
             seg_container, seg_prefix = manifest.split("/", 1)
             _, segments = self.conn.get_container(seg_container, prefix=seg_prefix, delimiter="/")
             segments_size = sum(item["bytes"] for item in segments if "bytes" in item)
             metadata["_segments_size"] = segments_size
 
         return metadata
 
-    def iter_key(self, key, *, with_metadata=True, deep=False, include_key=False):
+    def iter_key(
+        self, key: str, *, with_metadata: bool = True, deep: bool = False, include_key: bool = False
+    ) -> Iterator[IterKeyItem]:
         path = self.format_key_for_backend(key, remove_slash_prefix=True, trailing_slash=not include_key)
         self.log.debug("Listing path %r", path)
         if not deep:
             kwargs = {"delimiter": "/"}
         else:
             kwargs = {}
         _, results = self.conn.get_container(self.container_name, prefix=path, full_listing=True, **kwargs)
@@ -159,58 +198,58 @@
                         "size": item["bytes"] + segments_size,
                         "last_modified": last_modified,
                         "metadata": metadata,
                         "hash": item["hash"],
                     },
                 )
 
-    def _delete_object_plain(self, key):
+    def _delete_object_plain(self, key: str) -> None:
         try:
             return self.conn.delete_object(self.container_name, key)
         except exceptions.ClientException as ex:
             if ex.http_status == 404:
                 raise FileNotFoundFromStorageError(key)
             raise
 
-    def _delete_object_segments(self, key, manifest):
+    def _delete_object_segments(self, key: str, manifest: str) -> None:
         self._delete_object_plain(key)
         seg_container, seg_prefix = manifest.split("/", 1)
         _, segments = self.conn.get_container(seg_container, prefix=seg_prefix, delimiter="/")
         for item in segments:
             if "name" in item:
                 with suppress(FileNotFoundFromStorageError):
                     self._delete_object_plain(item["name"])
 
-    def delete_key(self, key):
+    def delete_key(self, key: str) -> None:
         path = self.format_key_for_backend(key)
         self.log.debug("Deleting key: %r", path)
         try:
             headers = self.conn.head_object(self.container_name, path)
         except exceptions.ClientException as ex:
             if ex.http_status == 404:
                 raise FileNotFoundFromStorageError(path)
             raise
         if "x-object-manifest" in headers:
             self._delete_object_segments(path, headers["x-object-manifest"])
         else:
             self._delete_object_plain(path)
         self.notifier.object_deleted(key=key)
 
-    def get_contents_to_file(self, key, filepath_to_store_to, *, progress_callback=None):
-        temp_filepath = "{}~".format(filepath_to_store_to)
-        try:
-            with open(temp_filepath, "wb") as fp:
-                metadata = self.get_contents_to_fileobj(key, fp, progress_callback=progress_callback)
-                os.rename(temp_filepath, filepath_to_store_to)
-        finally:
-            with suppress(FileNotFoundError):
-                os.unlink(temp_filepath)
-        return metadata
-
-    def get_contents_to_fileobj(self, key, fileobj_to_store_to, *, progress_callback=None):
+    def get_contents_to_fileobj(
+        self,
+        key: str,
+        fileobj_to_store_to: BinaryIO,
+        *,
+        byte_range: Optional[Tuple[int, int]] = None,
+        progress_callback: ProgressProportionCallbackType = None,
+    ) -> Metadata:
+        if byte_range:
+            # TODO if someday relevant. swift API itself implements it,
+            # c.f. https://docs.openstack.org/api-ref/object-store/
+            raise NotImplementedError("byte range fetching not supported")
         path = self.format_key_for_backend(key)
         try:
             headers, data_gen = self.conn.get_object(self.container_name, path, resp_chunk_size=CHUNK_SIZE)
         except exceptions.ClientException as ex:
             if ex.http_status == 404:
                 raise FileNotFoundFromStorageError(path)
             raise
@@ -225,58 +264,20 @@
                     progress_callback(1, 2)
                 else:
                     current_pos += len(chunk)
                     progress_callback(current_pos, content_len)
 
         return self._headers_to_metadata(headers)
 
-    def get_contents_to_string(self, key):
-        path = self.format_key_for_backend(key)
-        self.log.debug("Starting to fetch the contents of: %r", path)
-        try:
-            headers, data = self.conn.get_object(self.container_name, path)
-        except exceptions.ClientException as ex:
-            if ex.http_status == 404:
-                raise FileNotFoundFromStorageError(path)
-            raise
-
-        metadata = self._headers_to_metadata(headers)
-        return data, metadata
-
-    def get_file_size(self, key):
+    def get_file_size(self, key: str) -> int:
         # Not implemented due to lack of environment where to test this. This method is not required by
         # PGHoard itself, this is only called by external apps that utilize PGHoard's object storage abstraction.
         raise NotImplementedError
 
-    def store_file_from_memory(self, key, memstring, metadata=None, cache_control=None, mimetype=None):
-        if cache_control is not None:
-            raise NotImplementedError("SwiftTransfer: cache_control support not implemented")
-
-        path = self.format_key_for_backend(key)
-        sanitized_metadata = self.sanitize_metadata(metadata)
-        metadata_to_send = self._metadata_to_headers(sanitized_metadata)
-        data = bytes(memstring)
-        self.conn.put_object(self.container_name, path, contents=data, content_type=mimetype, headers=metadata_to_send)
-        self.notifier.object_created(key=key, size=len(data), metadata=sanitized_metadata)
-
-    def store_file_from_disk(self, key, filepath, metadata=None, multipart=None, cache_control=None, mimetype=None):
-        obsz = os.path.getsize(filepath)
-        with open(filepath, "rb") as fp:
-            self._store_file_contents(
-                key,
-                fp,
-                metadata=metadata,
-                multipart=multipart,
-                cache_control=cache_control,
-                mimetype=mimetype,
-                content_length=obsz,
-            )
-        self.notifier.object_created(key=key, size=obsz, metadata=self.sanitize_metadata(metadata))
-
-    def get_or_create_container(self, container_name):
+    def get_or_create_container(self, container_name: str) -> str:
         start_time = time.monotonic()
         try:
             self.conn.get_container(container_name, headers={}, limit=1)  # Limit 1 here to not traverse the entire folder
         except exceptions.ClientException as ex:
             if ex.http_status == 404:
                 self.conn.put_container(container_name, headers={})
                 self.log.debug(
@@ -284,58 +285,71 @@
                     container_name,
                     time.monotonic() - start_time,
                 )
                 return container_name
             raise
         return container_name
 
-    def copy_file(self, *, source_key, destination_key, metadata=None, **_kwargs):
+    def copy_file(
+        self, *, source_key: str, destination_key: str, metadata: Optional[Metadata] = None, **_kwargs: Any
+    ) -> None:
         source_key = self.format_key_for_backend(source_key)
         destination_key = "/".join((self.container_name, self.format_key_for_backend(destination_key)))
         sanitized_metadata = self.sanitize_metadata(metadata)
-        headers = self._metadata_to_headers(sanitized_metadata)
+        headers: Metadata = self._metadata_to_headers(sanitized_metadata)
         if metadata:
             headers["X-Fresh-Metadata"] = True
         self.conn.copy_object(self.container_name, source_key, destination=destination_key, headers=headers)
         self.notifier.object_copied(key=destination_key, size=None, metadata=sanitized_metadata)
 
-    def store_file_object(self, key, fd, *, cache_control=None, metadata=None, mimetype=None, upload_progress_fn=None):
+    def store_file_object(
+        self,
+        key: str,
+        fd: BinaryIO,
+        metadata: Optional[Metadata] = None,
+        *,
+        cache_control: Optional[str] = None,
+        mimetype: Optional[str] = None,
+        multipart: Optional[bool] = None,
+        upload_progress_fn: IncrementalProgressCallbackType = None,
+    ) -> None:  # pylint: disable=unused-argument
         metadata = metadata or {}
         content_length = metadata.get("Content-Length")
-
+        multipart = self._should_multipart(
+            chunk_size=self.segment_size, default=True, metadata=metadata, multipart=multipart
+        )
         self._store_file_contents(
             key,
             fd,
             cache_control=cache_control,
             metadata=metadata,
             mimetype=mimetype,
             upload_progress_fn=upload_progress_fn,
-            multipart=True,
+            multipart=multipart,
             content_length=content_length,
         )
         self.notifier.object_created(key=key, size=content_length, metadata=self.sanitize_metadata(metadata))
 
     def _store_file_contents(
         self,
-        key,
-        fp,
-        cache_control=None,
-        metadata=None,
-        mimetype=None,
-        upload_progress_fn=None,
-        multipart=None,
-        content_length=None,
-    ):
+        key: str,
+        fp: BinaryIO,
+        cache_control: Optional[str] = None,
+        metadata: Optional[Metadata] = None,
+        mimetype: Optional[str] = None,
+        upload_progress_fn: IncrementalProgressCallbackType = None,
+        multipart: Optional[bool] = None,
+        content_length: Optional[int] = None,
+    ) -> None:
         if cache_control is not None:
             raise NotImplementedError("SwiftTransfer: cache_control support not implemented")
 
         if multipart:
             # Start by trying to delete the file - if it's a potential multipart file we need to manually
-            # delete it, otherwise old segments won't be cleaned up by anything.  Note that we only issue
-            # deletes with the store_file_from_disk functions, store_file_from_memory is used to upload smaller
+            # delete it, otherwise old segments won't be cleaned up by anything.
             # chunks.
             with suppress(FileNotFoundFromStorageError):
                 self.delete_key(key)
         path = self.format_key_for_backend(key)
         headers = self._metadata_to_headers(self.sanitize_metadata(metadata))
         # Fall back to the "one segment" if possible
         if (not multipart) or (not content_length) or content_length <= self.segment_size:
```

### Comparing `rohmu-1.0.9/rohmu/snappyfile.py` & `rohmu-1.1.0/rohmu/snappyfile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 rohmu - file-like interface for snappy
 
 Copyright (c) 2016 Ohmu Ltd
 See LICENSE for details
 """
-
 from . import IO_BLOCK_SIZE
 from .filewrap import FileWrap
+from .typing import BinaryData, FileLike
+from typing import Optional
 
 import io
 
 try:
     import snappy
 except ImportError:
     snappy = None  # type: ignore
 
 
 class SnappyFile(FileWrap):
-    def __init__(self, next_fp, mode):
+    def __init__(self, next_fp: FileLike, mode: str) -> None:
         if snappy is None:
             raise io.UnsupportedOperation("Snappy is not available")
 
         if mode == "rb":
             self.decr = snappy.StreamDecompressor()
             self.encr = None
         elif mode == "wb":
@@ -29,37 +30,38 @@
             self.encr = snappy.StreamCompressor()
         else:
             raise io.UnsupportedOperation("unsupported mode for SnappyFile")
 
         super().__init__(next_fp)
         self.decr_done = False
 
-    def close(self):
+    def close(self) -> None:
         if self.closed:
             return
         if self.encr:
             data = self.encr.flush() or b""
             if data:
                 self.next_fp.write(data)
             self.next_fp.flush()
         super().close()
 
-    def write(self, data):
+    def write(self, data: BinaryData) -> int:
         self._check_not_closed()
         if self.encr is None:
             raise io.UnsupportedOperation("file not open for writing")
-        compressed_data = self.encr.compress(data)
+        data_as_bytes = bytes(data)
+        compressed_data = self.encr.compress(data_as_bytes)
         self.next_fp.write(compressed_data)
-        self.offset += len(data)
-        return len(data)
+        self.offset += len(data_as_bytes)
+        return len(data_as_bytes)
 
-    def writable(self):
+    def writable(self) -> bool:
         return self.encr is not None
 
-    def read(self, size=-1):  # pylint: disable=unused-argument
+    def read(self, size: Optional[int] = -1) -> bytes:  # pylint: disable=unused-argument
         # NOTE: size arg is ignored, random size output is returned
         self._check_not_closed()
         if self.decr is None:
             raise io.UnsupportedOperation("file not open for reading")
         while not self.decr_done:
             compressed = self.next_fp.read(IO_BLOCK_SIZE)
             if not compressed:
@@ -70,9 +72,9 @@
 
             if output:
                 self.offset += len(output)
                 return output
 
         return b""
 
-    def readable(self):
+    def readable(self) -> bool:
         return self.decr is not None
```

### Comparing `rohmu-1.0.9/rohmu/zstdfile.py` & `rohmu-1.1.0/rohmu/zstdfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 """
 rohmu - file-like interface for zstd
 
 Copyright (c) 2016 Ohmu Ltd
 See LICENSE for details
 """
-
 from . import IO_BLOCK_SIZE
 from .filewrap import FileWrap
+from .typing import BinaryData, FileLike
+from typing import Optional
 
 import io
 
 try:
     import zstandard as zstd
 except ImportError:
     zstd = None  # type: ignore
 
 
 class _ZstdFileWriter(FileWrap):
-    def __init__(self, next_fp, level, threads=0):
+    def __init__(self, next_fp: FileLike, level: int, threads: int = 0) -> None:
         self._zstd = zstd.ZstdCompressor(level=level, threads=threads).compressobj()
         super().__init__(next_fp)
 
-    def close(self):
+    def close(self) -> None:
         if self.closed:
             return
         data = self._zstd.flush() or b""
         if data:
             self.next_fp.write(data)
         self.next_fp.flush()
         super().close()
 
-    def write(self, data):
+    def write(self, data: BinaryData) -> int:
         self._check_not_closed()
-        compressed_data = self._zstd.compress(data)
+        data_as_bytes = bytes(data)
+        compressed_data = self._zstd.compress(data_as_bytes)
         self.next_fp.write(compressed_data)
-        self.offset += len(data)
-        return len(data)
+        self.offset += len(data_as_bytes)
+        return len(data_as_bytes)
 
-    def writable(self):
+    def writable(self) -> bool:
         return True
 
 
 class _ZtsdFileReader(FileWrap):
-    def __init__(self, next_fp):
+    def __init__(self, next_fp: FileLike) -> None:
         self._zstd = zstd.ZstdDecompressor().decompressobj()
         super().__init__(next_fp)
         self._done = False
 
-    def close(self):
+    def close(self) -> None:
         if self.closed:
             return
         super().close()
 
-    def read(self, size=-1):  # pylint: disable=unused-argument
+    def read(self, size: Optional[int] = -1) -> bytes:  # pylint: disable=unused-argument
         # NOTE: size arg is ignored, random size output is returned
         self._check_not_closed()
         while not self._done:
             compressed = self.next_fp.read(IO_BLOCK_SIZE)
             if not compressed:
                 self._done = True
                 output = self._zstd.flush() or b""
@@ -65,19 +67,19 @@
 
             if output:
                 self.offset += len(output)
                 return output
 
         return b""
 
-    def readable(self):
+    def readable(self) -> bool:
         return True
 
 
-def open(fp, mode, level=0, threads=0):  # pylint: disable=redefined-builtin
+def open(fp: FileLike, mode: str, level: int = 0, threads: int = 0) -> FileWrap:  # pylint: disable=redefined-builtin
     if zstd is None:
         raise io.UnsupportedOperation("zstd is not available")
 
     if mode == "wb":
         return _ZstdFileWriter(fp, level, threads)
 
     if mode == "rb":
```

### Comparing `rohmu-1.0.9/rohmu.egg-info/PKG-INFO` & `rohmu-1.1.0/rohmu.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: rohmu
-Version: 1.0.9
+Version: 1.1.0
 Summary: "Rohmu is a python library providing an interface to various cloud storage providers."
 Home-page: https://github.com/aiven/rohmu/
 License: Apache 2.0
 Platform: POSIX
 Platform: MacOS
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Database :: Database Engines/Servers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
@@ -39,15 +38,15 @@
 -  Supported compression algorithms: Snappy,
    `zstd <https://github.com/facebook/zstd>`__ and
    `lzma <https://docs.python.org/3/library/lzma.html>`__.
 
 Requirements
 ============
 
-Rohmu requires Python >= 3.7. For Python libary dependencies, have a
+Rohmu requires Python >= 3.8. For Python library dependencies, have a
 look at
 `requirements.txt <https://github.com/aiven/rohmu/blob/main/requirements.txt>`__.
 
 Usage example
 =============
 
 *Add usage example here*
```

### Comparing `rohmu-1.0.9/rohmu.egg-info/SOURCES.txt` & `rohmu-1.1.0/rohmu.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -10,17 +10,22 @@
 ./rohmu/dates.py
 ./rohmu/encryptor.py
 ./rohmu/errors.py
 ./rohmu/filewrap.py
 ./rohmu/inotify.py
 ./rohmu/rohmufile.py
 ./rohmu/snappyfile.py
+./rohmu/transfer_pool.py
+./rohmu/typing.py
 ./rohmu/util.py
 ./rohmu/version.py
 ./rohmu/zstdfile.py
+./rohmu/common/__init__.py
+./rohmu/common/models.py
+./rohmu/common/statsd.py
 ./rohmu/delta/__init__.py
 ./rohmu/delta/common.py
 ./rohmu/delta/snapshot.py
 ./rohmu/notifier/__init__.py
 ./rohmu/notifier/http.py
 ./rohmu/notifier/interface.py
 ./rohmu/notifier/logger.py
@@ -35,18 +40,24 @@
 ./rohmu/object_storage/swift.py
 rohmu.egg-info/PKG-INFO
 rohmu.egg-info/SOURCES.txt
 rohmu.egg-info/dependency_links.txt
 rohmu.egg-info/requires.txt
 rohmu.egg-info/top_level.txt
 test/test_atomic_opener.py
+test/test_compressor.py
 test/test_dates.py
 test/test_encryptor.py
+test/test_from_model.py
+test/test_inotify.py
 test/test_object_storage_azure.py
 test/test_object_storage_google.py
 test/test_object_storage_local.py
 test/test_object_storage_s3.py
 test/test_object_storage_sftp.py
 test/test_object_storage_swift.py
 test/test_rohmu_dates.py
 test/test_rohmufile.py
-test/test_storage.py
+test/test_statsd.py
+test/test_storage.py
+test/test_transfer_pool.py
+test/test_util.py
```

### Comparing `rohmu-1.0.9/setup.cfg` & `rohmu-1.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 license = Apache 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Database :: Database Engines/Servers
 	Topic :: Software Development :: Libraries :: Python Modules
 url = https://github.com/aiven/rohmu/
 platforms = 
@@ -34,14 +33,15 @@
 	oauth2client
 	paramiko
 	pydantic
 	python-dateutil
 	python-snappy
 	requests
 	zstandard
+	typing_extensions >= 3.10, < 5
 
 [options.packages.find]
 where = .
 include = rohmu*
 
 [egg_info]
 tag_build =
```

### Comparing `rohmu-1.0.9/test/test_atomic_opener.py` & `rohmu-1.1.0/test/test_atomic_opener.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,49 @@
+from __future__ import annotations
+
 from pathlib import Path
 from rohmu.atomic_opener import atomic_opener
+from typing import cast, TextIO
 
 import errno
 import os
 import pytest
 import time
 
 
-def _verify_file_not_created_and_dir_not_polluted(output_file: Path):
+def _verify_file_not_created_and_dir_not_polluted(output_file: Path) -> None:
     assert os.listdir(output_file.parent) == []
     assert not output_file.exists()
 
 
-def test_error_thrown_if_final_path_parent_doesnt_exist(tmp_path: Path):
+def test_error_thrown_if_final_path_parent_doesnt_exist(tmp_path: Path) -> None:
     with pytest.raises(IOError):
         with atomic_opener(tmp_path / "nonexistingdir" / "final_path", mode="w"):
             pass
 
 
-def test_error_mode_doesnt_contain_write(tmp_path: Path):
+def test_error_mode_doesnt_contain_write(tmp_path: Path) -> None:
     with pytest.raises(ValueError):
-        with atomic_opener(tmp_path, mode="r"):  # type: ignore
+        with atomic_opener(tmp_path, mode="r"):  # type: ignore [call-overload]
             pass
 
 
-def test_file_is_atomically_created_only_after_function_execution_is_over(tmp_path: Path):
+def test_file_is_atomically_created_only_after_function_execution_is_over(tmp_path: Path) -> None:
     data_block = "x" * 100_000_000
     # manually tested with block_count of 1000 but it seems overkill to do it every time and it can hog
     # the testing infra quite a bit.
     # block_count = 1000
     block_count = 1
     size = len(data_block)
 
     output_file = tmp_path / "something"
     try:
         _verify_file_not_created_and_dir_not_polluted(output_file)
-        with atomic_opener(output_file, mode="w") as f:
+        # FIXME: when dropping python3.7 support we should not need cast here
+        with cast(TextIO, atomic_opener(output_file, mode="w")) as f:
             inode_inside = os.stat(f.fileno()).st_ino
             _verify_file_not_created_and_dir_not_polluted(output_file)
             for unused_counter in range(block_count):
                 f.write(data_block)
                 f.flush()
                 _verify_file_not_created_and_dir_not_polluted(output_file)
             timestamp_before_exiting = time.monotonic()
@@ -55,67 +59,67 @@
         # the file can be big, we want to delete it ASAP
         try:
             output_file.unlink()
         except FileNotFoundError:
             pass
 
 
-def test_file_is_never_created_if_function_breaks(tmp_path: Path):
+def test_file_is_never_created_if_function_breaks(tmp_path: Path) -> None:
     output_file = tmp_path / "something"
 
     try:
         _verify_file_not_created_and_dir_not_polluted(output_file)
-        with atomic_opener(output_file, mode="w") as f:
+        with cast(TextIO, atomic_opener(output_file, mode="w")) as f:
             _verify_file_not_created_and_dir_not_polluted(output_file)
             f.write("aaaaaaaaaa")
             f.flush()
             _verify_file_not_created_and_dir_not_polluted(output_file)
             time.sleep(1.0)
             _verify_file_not_created_and_dir_not_polluted(output_file)
             raise ValueError("crash")
         pytest.fail("codepath should never be taken")
     except ValueError:
         _verify_file_not_created_and_dir_not_polluted(output_file)
 
 
-def test_file_is_fully_written_if_visible(tmp_path: Path):
+def test_file_is_fully_written_if_visible(tmp_path: Path) -> None:
     output_file = tmp_path / "something"
 
-    def linkhook():
+    def linkhook() -> None:
         assert output_file.exists()
         assert output_file.read_text() == "aaaaaaaaaa"
 
     try:
         _verify_file_not_created_and_dir_not_polluted(output_file)
-        with atomic_opener(output_file, mode="w", _after_link_hook=linkhook) as f:
+        with cast(TextIO, atomic_opener(output_file, mode="w", _after_link_hook=linkhook)) as f:
             _verify_file_not_created_and_dir_not_polluted(output_file)
             f.write("aaaaaaaaaa")
             _verify_file_not_created_and_dir_not_polluted(output_file)
             time.sleep(1.0)
             _verify_file_not_created_and_dir_not_polluted(output_file)
 
     except ValueError:
         _verify_file_not_created_and_dir_not_polluted(output_file)
 
 
-def test_open_for_writing_text_opens_proper_encoding_file(tmp_path: Path):
+def test_open_for_writing_text_opens_proper_encoding_file(tmp_path: Path) -> None:
     final_path = tmp_path / "file"
-    with atomic_opener(final_path, encoding="iso-8859-1", mode="w") as f:
+    with cast(TextIO, atomic_opener(final_path, encoding="iso-8859-1", mode="w")) as f:
         f.write("à")
     assert final_path.read_bytes() == b"\xe0"
 
 
-def test_open_for_writing_bytes_properly_writes_bytes(tmp_path: Path):
+def test_open_for_writing_bytes_properly_writes_bytes(tmp_path: Path) -> None:
     final_path = tmp_path / "file"
     with atomic_opener(final_path, mode="wb") as f:
         f.write(b"\xe0")
     assert final_path.read_text("iso-8859-1") == "à"
 
 
-def test_no_fd_leak_if_fdopen_fails_because_of_wrong_encoding(tmp_path: Path):
+def test_no_fd_leak_if_fdopen_fails_because_of_wrong_encoding(tmp_path: Path) -> None:
     final_path = tmp_path / "file"
     opened_fd: list[int] = []
     try:
         with atomic_opener(final_path, mode="w", encoding="unknownencoding", _fd_spy=opened_fd.append):
             pass
         pytest.fail("should fail, encoding is wrong")
     except LookupError:
@@ -124,19 +128,21 @@
             pytest.fail("should fail, file descriptor must be invalid")
         except OSError as e:
             if e.errno != errno.EBADF:
                 raise
             # descriptor is invalid, all ok
 
 
-def test_no_fd_leak_if_fdopen_fails_because_of_unknown_mode(tmp_path: Path):
+def test_no_fd_leak_if_fdopen_fails_because_of_unknown_mode(tmp_path: Path) -> None:
     final_path = tmp_path / "file"
     opened_fd: list[int] = []
     try:
-        with atomic_opener(final_path, mode="somethingrandomw", encoding="ascii", _fd_spy=opened_fd.append):
+        with atomic_opener(
+            final_path, mode="somethingrandomw", encoding="ascii", _fd_spy=opened_fd.append
+        ):  # type: ignore [call-overload]
             pass
         pytest.fail("should fail, mode is wrong")
     except ValueError:
         try:
             os.fstat(opened_fd[0])
             pytest.fail("should fail, file descriptor must be invalid")
         except OSError as e:
```

### Comparing `rohmu-1.0.9/test/test_dates.py` & `rohmu-1.1.0/test/test_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rohmu.dates import parse_timestamp
 
 import datetime
 import dateutil.tz
 import re
 
 
-def test_parse_timestamp():
+def test_parse_timestamp() -> None:
     local_aware = datetime.datetime.now(dateutil.tz.tzlocal())
 
     # split local_aware such as "2021-02-08T09:58:27.988218-05:00" into date, time, tzoffset components
     str_date, str_localtime_aware = local_aware.isoformat().split("T", 1)
     str_localtime_naive = re.split("[+-]", str_localtime_aware, maxsplit=1)[0]
     str_local_aware_named = "{}T{} {}".format(str_date, str_localtime_naive, local_aware.tzname())
```

### Comparing `rohmu-1.0.9/test/test_encryptor.py` & `rohmu-1.1.0/test/test_encryptor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Copyright (c) 2015 Ohmu Ltd
 See LICENSE for details
 """
 from .base import CONSTANT_TEST_RSA_PRIVATE_KEY, CONSTANT_TEST_RSA_PUBLIC_KEY
+from py.path import LocalPath  # type: ignore [import] # pylint: disable=import-error
 from rohmu import IO_BLOCK_SIZE
 from rohmu.encryptor import Decryptor, DecryptorFile, Encryptor, EncryptorFile, EncryptorStream
+from typing import cast, IO
 
 import io
 import json
 import os
 import pytest
 import random
 import tarfile
 
 
-def test_encryptor_decryptor():
+def test_encryptor_decryptor() -> None:
     plaintext = b"test"
     for op in (None, "json"):
         if op == "json":
             public_key = json.loads(json.dumps(CONSTANT_TEST_RSA_PUBLIC_KEY))
             private_key = json.loads(json.dumps(CONSTANT_TEST_RSA_PRIVATE_KEY))
         else:
             public_key = CONSTANT_TEST_RSA_PUBLIC_KEY
@@ -35,15 +37,15 @@
             offset += len(chunk)
         decrypted_size = len(encrypted) - decryptor.header_size() - decryptor.footer_size()
         decrypted = decryptor.process_data(encrypted[decryptor.header_size() : decryptor.header_size() + decrypted_size])
         decrypted += decryptor.finalize(encrypted[-decryptor.footer_size() :])
         assert plaintext == decrypted
 
 
-def test_encryptor_stream():
+def test_encryptor_stream() -> None:
     plaintext = os.urandom(2 * 1024 * 1024)
     encrypted_stream = EncryptorStream(io.BytesIO(plaintext), CONSTANT_TEST_RSA_PUBLIC_KEY)
     result_data = io.BytesIO()
     while True:
         bytes_requested = random.randrange(1, 12345)
         data = encrypted_stream.read(bytes_requested)
         if not data:
@@ -64,15 +66,15 @@
     result_data = io.BytesIO()
     result_data.write(encrypted_stream.read())
     result_data.seek(0)
     decrypted = DecryptorFile(result_data, CONSTANT_TEST_RSA_PRIVATE_KEY).read()
     assert plaintext == decrypted
 
 
-def test_decryptorfile(tmpdir):
+def test_decryptorfile(tmpdir: LocalPath) -> None:
     # create a plaintext blob bigger than IO_BLOCK_SIZE
     plaintext1 = b"rvdmfki6iudmx8bb25tx1sozex3f4u0nm7uba4eibscgda0ckledcydz089qw1p1wer"
     repeat = int(1.5 * IO_BLOCK_SIZE / len(plaintext1))
     plaintext = repeat * plaintext1
     encryptor = Encryptor(CONSTANT_TEST_RSA_PUBLIC_KEY)
     ciphertext = encryptor.update(plaintext) + encryptor.finalize()
     plain_fp = open(tmpdir.join("plain").strpath, mode="w+b")
@@ -138,15 +140,15 @@
     # close the file (this can be safely called multiple times), other ops should fail after that
     fp.close()
     fp.close()
     with pytest.raises(ValueError):
         fp.truncate()
 
 
-def test_decryptorfile_for_tarfile(tmpdir):
+def test_decryptorfile_for_tarfile(tmpdir: LocalPath) -> None:
     testdata = b"file contents"
     data_tmp_name = tmpdir.join("plain.data").strpath
     with open(data_tmp_name, mode="wb") as data_tmp:
         data_tmp.write(testdata)
 
     tar_data = io.BytesIO()
     with tarfile.open(name="foo", fileobj=tar_data, mode="w") as tar:
@@ -157,32 +159,33 @@
     ciphertext = encryptor.update(plaintext) + encryptor.finalize()
     enc_tar_name = tmpdir.join("enc.tar.data").strpath
     with open(enc_tar_name, "w+b") as enc_tar:
         enc_tar.write(ciphertext)
         enc_tar.seek(0)
 
         dfile = DecryptorFile(enc_tar, CONSTANT_TEST_RSA_PRIVATE_KEY)
-        with tarfile.open(fileobj=dfile, mode="r") as tar:
+        with tarfile.open(fileobj=cast(IO[bytes], dfile), mode="r") as tar:
             info = tar.getmember("archived_content")
             assert info.isfile() is True
             assert info.size == len(testdata)
             content_file = tar.extractfile("archived_content")
-            content = content_file.read()  # pylint: disable=no-member
-            content_file.close()  # pylint: disable=no-member
+            assert content_file is not None
+            content = content_file.read()
+            content_file.close()
             assert testdata == content
 
             decout = tmpdir.join("dec_out_dir").strpath
             os.makedirs(decout)
             tar.extract("archived_content", decout)
             extracted_path = os.path.join(decout, "archived_content")
             with open(extracted_path, "rb") as ext_fp:
                 assert testdata == ext_fp.read()
 
 
-def test_encryptorfile(tmpdir):
+def test_encryptorfile(tmpdir: LocalPath) -> None:
     # create a plaintext blob bigger than IO_BLOCK_SIZE
     plaintext1 = b"rvdmfki6iudmx8bb25tx1sozex3f4u0nm7uba4eibscgda0ckledcydz089qw1p1"
     repeat = int(1.5 * IO_BLOCK_SIZE / len(plaintext1))
     plaintext = repeat * plaintext1
 
     fn = tmpdir.join("data").strpath
     with open(fn, "w+b") as plain_fp:
@@ -214,41 +217,42 @@
             dec_fp.write(b"x")
         dec_fp.flush()
 
         result = dec_fp.read()
         assert plaintext == result
 
 
-def test_encryptorfile_for_tarfile(tmpdir):
+def test_encryptorfile_for_tarfile(tmpdir: LocalPath) -> None:
     testdata = b"file contents"
     data_tmp_name = tmpdir.join("plain.data").strpath
     with open(data_tmp_name, mode="wb") as data_tmp:
         data_tmp.write(testdata)
 
     enc_tar_name = tmpdir.join("enc.tar.data").strpath
     with open(enc_tar_name, "w+b") as plain_fp:
         enc_fp = EncryptorFile(plain_fp, CONSTANT_TEST_RSA_PUBLIC_KEY)
-        with tarfile.open(name="foo", fileobj=enc_fp, mode="w") as tar:
+        with tarfile.open(name="foo", fileobj=cast(IO[bytes], enc_fp), mode="w") as tar:
             tar.add(data_tmp_name, arcname="archived_content")
         enc_fp.close()
 
         plain_fp.seek(0)
 
         dfile = DecryptorFile(plain_fp, CONSTANT_TEST_RSA_PRIVATE_KEY)
-        with tarfile.open(fileobj=dfile, mode="r") as tar:
+        with tarfile.open(fileobj=cast(IO[bytes], dfile), mode="r") as tar:
             info = tar.getmember("archived_content")
             assert info.isfile() is True
             assert info.size == len(testdata)
             content_file = tar.extractfile("archived_content")
-            content = content_file.read()  # pylint: disable=no-member
-            content_file.close()  # pylint: disable=no-member
+            assert content_file is not None
+            content = content_file.read()
+            content_file.close()
             assert testdata == content
 
 
-def test_empty_file():
+def test_empty_file() -> None:
     bio = io.BytesIO()
     ef = EncryptorFile(bio, CONSTANT_TEST_RSA_PUBLIC_KEY)
     ef.write(b"")
     ef.close()
     assert bio.tell() == 0
 
     df = DecryptorFile(bio, CONSTANT_TEST_RSA_PRIVATE_KEY)
```

### Comparing `rohmu-1.0.9/test/test_object_storage_azure.py` & `rohmu-1.1.0/test/test_object_storage_azure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/"""
 from datetime import datetime
 from io import BytesIO
+from rohmu.errors import InvalidByteRangeError
 from tempfile import NamedTemporaryFile
 from types import ModuleType
-from typing import Tuple
+from typing import Any, Tuple
 from unittest.mock import MagicMock, patch
 
 import pytest
 import sys
 
 
 @pytest.fixture(scope="module", name="mock_azure_module")
@@ -23,20 +24,20 @@
     with patch.dict(sys.modules, module_patches):
         import rohmu.object_storage.azure
 
     return rohmu.object_storage.azure, get_blob_client_mock
 
 
 @pytest.fixture(name="azure_module")
-def fixture_azure_module(mock_azure_module) -> ModuleType:
+def fixture_azure_module(mock_azure_module: Tuple[ModuleType, MagicMock]) -> ModuleType:
     return mock_azure_module[0]
 
 
 @pytest.fixture(name="get_blob_client")
-def fixture_get_blob_client(mock_azure_module) -> MagicMock:
+def fixture_get_blob_client(mock_azure_module: Tuple[ModuleType, MagicMock]) -> MagicMock:
     return mock_azure_module[1]
 
 
 def test_store_file_from_disk(azure_module: ModuleType, get_blob_client: MagicMock) -> None:
     notifier = MagicMock()
     transfer = azure_module.AzureTransfer(
         bucket_name="test_bucket",
@@ -68,21 +69,37 @@
         account_key="test_key2",
         notifier=notifier,
     )
     test_data = b"test-data"
     metadata = {"Content-Length": len(test_data), "some-date": datetime(2022, 11, 15, 18, 30, 58, 486644)}
     file_object = BytesIO(test_data)
 
-    def upload_side_effect(*args, **kwargs):  # pylint: disable=unused-argument
+    def upload_side_effect(*args: Any, **kwargs: Any) -> None:  # pylint: disable=unused-argument
         if kwargs.get("raw_response_hook"):
             kwargs["raw_response_hook"](MagicMock(context={"upload_stream_current": len(test_data)}))
 
     # Size reporting relies on the progress callback from azure client
     upload_blob = MagicMock(wraps=upload_side_effect)
     get_blob_client.return_value = MagicMock(upload_blob=upload_blob)
 
     transfer.store_file_object(key="test_key2", fd=file_object, metadata=metadata)
 
     upload_blob.assert_called_once()
     notifier.object_created.assert_called_once_with(
         key="test_key2", size=len(test_data), metadata={"Content_Length": "9", "some_date": "2022-11-15 18:30:58.486644"}
     )
+
+
+def test_get_contents_to_fileobj_raises_error_on_invalid_byte_range(azure_module: ModuleType) -> None:
+    notifier = MagicMock()
+    transfer = azure_module.AzureTransfer(
+        bucket_name="test_bucket",
+        account_name="test_account",
+        account_key="test_key2",
+        notifier=notifier,
+    )
+    with pytest.raises(InvalidByteRangeError):
+        transfer.get_contents_to_fileobj(
+            key="testkey",
+            fileobj_to_store_to=BytesIO(),
+            byte_range=(100, 10),
+        )
```

### Comparing `rohmu-1.0.9/test/test_object_storage_local.py` & `rohmu-1.1.0/test/test_object_storage_local.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/"""
 from io import BytesIO
+from rohmu.errors import InvalidByteRangeError
 from rohmu.object_storage.local import LocalTransfer
 from tempfile import NamedTemporaryFile, TemporaryDirectory
 from unittest.mock import MagicMock
 
 import os
+import pytest
 
 
 def test_store_file_from_disk() -> None:
     with TemporaryDirectory() as destdir:
         notifier = MagicMock()
         transfer = LocalTransfer(
             directory=destdir,
@@ -17,15 +19,17 @@
         test_data = b"test-data"
         with NamedTemporaryFile() as tmpfile:
             tmpfile.write(test_data)
             tmpfile.flush()
             transfer.store_file_from_disk(key="test_key1", filepath=tmpfile.name)
 
         assert open(os.path.join(destdir, "test_key1"), "rb").read() == test_data
-        notifier.object_created.assert_called_once_with(key="test_key1", size=len(test_data), metadata={})
+        notifier.object_created.assert_called_once_with(
+            key="test_key1", size=len(test_data), metadata={"Content-Length": "9"}
+        )
 
 
 def test_store_file_object() -> None:
     with TemporaryDirectory() as destdir:
         notifier = MagicMock()
         transfer = LocalTransfer(
             directory=destdir,
@@ -34,7 +38,31 @@
         test_data = b"test-data-2"
         file_object = BytesIO(test_data)
 
         transfer.store_file_object(key="test_key2", fd=file_object)
 
         assert open(os.path.join(destdir, "test_key2"), "rb").read() == test_data
         notifier.object_created.assert_called_once_with(key="test_key2", size=len(test_data), metadata={})
+
+        data, _ = transfer.get_contents_to_string("test_key2")
+        assert data == test_data
+
+        data, _ = transfer.get_contents_to_string("test_key2", byte_range=(1, 123456))
+        assert data == test_data[1:]
+
+        data, _ = transfer.get_contents_to_string("test_key2", byte_range=(0, len(test_data) - 2))
+        assert data == test_data[:-1]
+
+
+def test_get_contents_to_fileobj_raises_error_on_invalid_byte_range() -> None:
+    with TemporaryDirectory() as destdir:
+        notifier = MagicMock()
+        transfer = LocalTransfer(
+            directory=destdir,
+            notifier=notifier,
+        )
+        with pytest.raises(InvalidByteRangeError):
+            transfer.get_contents_to_fileobj(
+                key="testkey",
+                fileobj_to_store_to=BytesIO(),
+                byte_range=(100, 10),
+            )
```

### Comparing `rohmu-1.0.9/test/test_object_storage_sftp.py` & `rohmu-1.1.0/test/test_object_storage_sftp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 """Copyright (c) 2022 Aiven, Helsinki, Finland. https://aiven.io/"""
 from datetime import datetime
 from io import BytesIO
 from rohmu.object_storage.sftp import SFTPTransfer
 from tempfile import NamedTemporaryFile
+from typing import Any
 from unittest.mock import MagicMock, patch
 
 
 def test_store_file_from_disk() -> None:
     notifier = MagicMock()
     with patch("paramiko.Transport") as _, patch("paramiko.SFTPClient") as sftp_client:
+
+        def _putfo() -> int:
+            return 42
+
         client = MagicMock()
+
+        # Size reporting relies on the progress callback from paramiko
+        def upload_side_effect(*args: Any, **kwargs: Any) -> None:  # pylint: disable=unused-argument
+            if kwargs.get("callback"):
+                kwargs["callback"](len(test_data), len(test_data))
+
+        client.putfo = MagicMock(wraps=upload_side_effect)
+
         sftp_client.from_transport.return_value = client
         transfer = SFTPTransfer(
             server="sftp.example.com",
             port=2222,
             username="testuser",
             password="testpass",
             notifier=notifier,
@@ -43,15 +56,15 @@
             password="testpass",
             notifier=notifier,
         )
         test_data = b"test-data"
         file_object = BytesIO(test_data)
 
         # Size reporting relies on the progress callback from paramiko
-        def upload_side_effect(*args, **kwargs):  # pylint: disable=unused-argument
+        def upload_side_effect(*args: Any, **kwargs: Any) -> None:  # pylint: disable=unused-argument
             if kwargs.get("callback"):
                 kwargs["callback"](len(test_data), len(test_data))
 
         client.putfo = MagicMock(wraps=upload_side_effect)
 
         metadata = {"Content-Length": len(test_data), "some-date": datetime(2022, 11, 15, 18, 30, 58, 486644)}
         transfer.store_file_object(key="test_key2", fd=file_object, metadata=metadata)
```

### Comparing `rohmu-1.0.9/test/test_object_storage_swift.py` & `rohmu-1.1.0/test/test_object_storage_swift.py`

 * *Files identical despite different names*

### Comparing `rohmu-1.0.9/test/test_rohmu_dates.py` & `rohmu-1.1.0/test/test_rohmu_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from rohmu.dates import parse_timestamp
 
 import datetime
 import dateutil.tz
 import re
 
 
-def test_parse_timestamp():
+def test_parse_timestamp() -> None:
     local_aware = datetime.datetime.now(dateutil.tz.tzlocal())
 
     # split local_aware such as "2021-02-08T09:58:27.988218-05:00" into date, time, tzoffset components
     str_date, str_localtime_aware = local_aware.isoformat().split("T", 1)
     str_localtime_naive = re.split("[+-]", str_localtime_aware, maxsplit=1)[0]
     str_local_aware_named = "{}T{} {}".format(str_date, str_localtime_naive, local_aware.tzname())
```

### Comparing `rohmu-1.0.9/test/test_rohmufile.py` & `rohmu-1.1.0/test/test_rohmufile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 # Copyright (c) 2021 Aiven, Helsinki, Finland. https://aiven.io/
 
 from io import BytesIO
 from rohmu import rohmufile
 from rohmu.errors import InvalidConfigurationError
 from tempfile import NamedTemporaryFile
+from typing import Any
 
 import pytest
 
 
-def test_fileobj_name(tmpdir):
+def test_fileobj_name(tmpdir: Any) -> None:
     with NamedTemporaryFile(dir=tmpdir, suffix="foo") as raw_output_obj:
-        result = rohmufile._fileobj_name(raw_output_obj)  # pylint: disable=protected-access
+        result = rohmufile._fileobj_name(raw_output_obj)  # type: ignore # pylint: disable=protected-access
         assert result.startswith("open file ")
         assert "foo" in result
 
 
-def test_get_encryption_key_data_no_metadata():
+def test_get_encryption_key_data_no_metadata() -> None:
     assert rohmufile._get_encryption_key_data(None, None) is None  # pylint: disable=protected-access
     assert rohmufile._get_encryption_key_data({}, None) is None  # pylint: disable=protected-access
 
 
-def test_get_encryption_key_data_invalid_configuration():
+def test_get_encryption_key_data_invalid_configuration() -> None:
     metadata = {"encryption-key-id": "foo"}
     with pytest.raises(InvalidConfigurationError, match="File is encrypted with key 'foo' but key not found"):
         rohmufile._get_encryption_key_data(metadata, lambda key_id: None)  # pylint: disable=protected-access
 
 
-def test_get_encryption_key_data():
-    def _getkey(key_id):
+def test_get_encryption_key_data() -> None:
+    def _getkey(key_id: str) -> str:
         assert key_id == "foo"
         return "bar"
 
     metadata = {"encryption-key-id": "foo"}
     key_data = rohmufile._get_encryption_key_data(metadata, _getkey)  # pylint: disable=protected-access
     assert key_data == "bar"
 
 
-def test_file_reader_no_metadata():
+def test_file_reader_no_metadata() -> None:
     fileobj = BytesIO(b"foo")
     assert rohmufile.file_reader(fileobj=fileobj) == fileobj
 
 
-def test_file_reader_no_key():
+def test_file_reader_no_key() -> None:
     fileobj = BytesIO(b"foo")
     metadata = {"encryption-key-id": "foo"}
     with pytest.raises(InvalidConfigurationError, match="File is encrypted with key 'foo' but key not found"):
         rohmufile.file_reader(fileobj=fileobj, metadata=metadata)
 
 
-def test_file_reader_no_encryption_compression():
+def test_file_reader_no_encryption_compression() -> None:
     fileobj = BytesIO(b"foo")
     metadata = {"a": "b"}
     assert rohmufile.file_reader(fileobj=fileobj, metadata=metadata) == fileobj
```

### Comparing `rohmu-1.0.9/test/test_storage.py` & `rohmu-1.1.0/test/test_storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,146 @@
 from datetime import datetime
 from io import BytesIO
 from pathlib import Path
 from rohmu import errors
+from rohmu.object_storage.local import LocalTransfer
+from typing import Any
 
 import pytest
 
+DUMMY_CONTENT = b"dummy"
+DUMMY_METADATA = {"Content-Length": str(len(DUMMY_CONTENT))}
 
-@pytest.mark.parametrize("transfer", ["local_transfer"])
-def test_nonexistent(transfer, request):
-    transfer = request.getfixturevalue(transfer)
+
+@pytest.mark.parametrize("transfer_type", ["local_transfer"])
+def test_nonexistent(transfer_type: str, request: Any) -> None:
+    transfer = request.getfixturevalue(transfer_type)
     with pytest.raises(errors.FileNotFoundFromStorageError):
         transfer.get_metadata_for_key("NONEXISTENT")
     with pytest.raises(errors.FileNotFoundFromStorageError):
         transfer.delete_key("NONEXISTENT")
     with pytest.raises(errors.FileNotFoundFromStorageError):
         transfer.get_contents_to_file("NONEXISTENT", "nonexistent/a")
     with pytest.raises(errors.FileNotFoundFromStorageError):
         transfer.get_contents_to_fileobj("NONEXISTENT", BytesIO())
     with pytest.raises(errors.FileNotFoundFromStorageError):
         transfer.get_contents_to_string("NONEXISTENT")
     assert transfer.list_path("") == []
     assert transfer.list_path("NONEXISTENT") == []
 
 
-@pytest.mark.parametrize("transfer", ["local_transfer"])
-def test_basic_upload(transfer, tmp_path, request):
+@pytest.mark.parametrize("transfer_type", ["local_transfer"])
+def test_basic_upload(transfer_type: str, tmp_path: Path, request: Any) -> None:
     scratch = tmp_path / "scratch"
     scratch.mkdir()
-    transfer = request.getfixturevalue(transfer)
-    transfer.store_file_from_memory("x1", b"dummy", {"k": "v"})
-    assert transfer.get_contents_to_string("x1") == (b"dummy", {"k": "v"})
+    transfer = request.getfixturevalue(transfer_type)
+    sent_metadata = {"k": "v"}
+    metadata = DUMMY_METADATA.copy()
+    metadata.update(sent_metadata)
+    transfer.store_file_from_memory("x1", DUMMY_CONTENT, sent_metadata)
+
+    assert transfer.get_contents_to_string("x1") == (DUMMY_CONTENT, metadata)
     # Same thing, but with a key looking like a directory
-    transfer.store_file_from_memory("NONEXISTENT-DIR/x1", b"dummy", None)
-    assert transfer.get_contents_to_string("NONEXISTENT-DIR/x1") == (b"dummy", {})
+    transfer.store_file_from_memory("NONEXISTENT-DIR/x1", DUMMY_CONTENT, None)
+    assert transfer.get_contents_to_string("NONEXISTENT-DIR/x1") == (DUMMY_CONTENT, DUMMY_METADATA)
 
     # Same thing, but from disk now
     dummy_file = scratch / "a"
     with open(dummy_file, "wb") as fp:
-        fp.write(b"dummy")
+        fp.write(DUMMY_CONTENT)
     transfer.store_file_from_disk("test1/x1", dummy_file, None)
     out = BytesIO()
 
-    assert transfer.get_contents_to_fileobj("test1/x1", out) == {}
-    assert out.getvalue() == b"dummy"
+    assert transfer.get_contents_to_fileobj("test1/x1", out) == DUMMY_METADATA
+    assert out.getvalue() == DUMMY_CONTENT
 
 
-@pytest.mark.parametrize("transfer", ["local_transfer"])
-def test_copy(transfer, request):
-    transfer = request.getfixturevalue(transfer)
-    transfer.store_file_from_memory("dummy", b"dummy", {"k": "v"})
+@pytest.mark.parametrize("transfer_type", ["local_transfer"])
+def test_copy(transfer_type: str, request: Any) -> None:
+    transfer = request.getfixturevalue(transfer_type)
+    sent_metadata = {"k": "v"}
+    metadata = DUMMY_METADATA.copy()
+    metadata.update(sent_metadata)
+    transfer.store_file_from_memory("dummy", DUMMY_CONTENT, sent_metadata)
     transfer.copy_file(source_key="dummy", destination_key="dummy_copy")
-    assert transfer.get_contents_to_string("dummy_copy") == (b"dummy", {"k": "v"})
+    assert transfer.get_contents_to_string("dummy_copy") == (DUMMY_CONTENT, metadata)
+
     # Same thing, but with different metadata
     transfer.copy_file(source_key="dummy", destination_key="dummy_copy_metadata", metadata={"new_k": "new_v"})
-    assert transfer.get_contents_to_string("dummy_copy_metadata") == (b"dummy", {"new_k": "new_v"})
+    assert transfer.get_contents_to_string("dummy_copy_metadata") == (DUMMY_CONTENT, {"new_k": "new_v"})
 
 
-@pytest.mark.parametrize("transfer", ["local_transfer"])
-def test_list(transfer, request):
-    transfer = request.getfixturevalue(transfer)
+@pytest.mark.parametrize("transfer_type", ["local_transfer"])
+def test_list(transfer_type: str, request: Any) -> None:
+    transfer = request.getfixturevalue(transfer_type)
     assert transfer.list_path("") == []
 
     # Test with a single file at root
-    transfer.store_file_from_memory("dummy", b"dummy", metadata={"k": "v"})
+    sent_metadata = {"k": "v"}
+    metadata = DUMMY_METADATA.copy()
+    metadata.update(sent_metadata)
+    transfer.store_file_from_memory("dummy", DUMMY_CONTENT, metadata=sent_metadata)
     file_list = transfer.list_path("")
     assert len(file_list) == 1
     assert file_list[0]["name"] == "dummy"
-    assert file_list[0]["metadata"] == {"k": "v"}
+    assert file_list[0]["metadata"] == metadata
     assert file_list[0]["size"] == len("dummy")
     assert isinstance(file_list[0]["last_modified"], datetime)
 
     # Test with a "subdirectory"
-    transfer.store_file_from_memory("dummydir/dummy", b"dummy", metadata={"k": "v"})
+    transfer.store_file_from_memory("dummydir/dummy", DUMMY_CONTENT, metadata=sent_metadata)
     assert len(transfer.list_path("")) == 1
     assert set(transfer.iter_prefixes("")) == {"dummydir"}
     assert len(transfer.list_path("dummydir")) == 1
 
     files = transfer.list_path("", deep=True)
     assert len(files) == 2
     assert set(f["name"] for f in files) == {"dummy", "dummydir/dummy"}
 
 
-def test_hidden_local_files(local_transfer):
+def test_hidden_local_files(local_transfer: LocalTransfer) -> None:
     """
     Local storage specific test.
     """
     storage_dir = Path(local_transfer.prefix)
     # Since we've never used the local storage, need to create the directory
     storage_dir.mkdir()
     # When creating the file manually, we need to create some metadata too.
     with open(Path(local_transfer.prefix) / ".null", "w"):
         pass
     with open(Path(local_transfer.prefix) / ".null.metadata", "w") as f:
-        f.write('{"k": "v"}')
+        f.write('{"k": "v", "_hash": ""}')
     assert local_transfer.list_path("") == []
 
     # Make sure the previous test actually worked, by manually creating a file
     # that must appear.
     with open(Path(local_transfer.prefix) / "somefile", "w"):
         pass
     with open(Path(local_transfer.prefix) / "somefile.metadata", "w") as f:
-        f.write('{"k": "v"}')
+        f.write('{"k": "v", "_hash": ""}')
 
     files = local_transfer.list_path("")
     assert len(files) == 1
     assert files[0]["name"] == "somefile"
+
+
+@pytest.mark.parametrize("transfer", ["local_transfer"])
+def test_delete(transfer: LocalTransfer, request: Any) -> None:
+    transfer = request.getfixturevalue(transfer)
+
+    def setup() -> None:
+        assert transfer.list_path("") == []
+        transfer.store_file_from_memory("shallow", b"1")
+        transfer.store_file_from_memory("something/quite/deep", b"2")
+        assert len(transfer.list_path("", deep=True)) == 2
+
+    setup()
+    transfer.delete_tree("")
+
+    setup()
+    transfer.delete_keys(["shallow", "something/quite/deep"])
+
+    setup()
+    transfer.delete_key("shallow")
+    transfer.delete_key("something/quite/deep")
+
+    assert transfer.list_path("") == []
```

