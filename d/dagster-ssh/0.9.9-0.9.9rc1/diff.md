# Comparing `tmp/dagster-ssh-0.9.9.tar.gz` & `tmp/dagster-ssh-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-ssh-0.9.9.tar", last modified: Thu Sep 17 21:28:53 2020, max compression
+gzip compressed data, was "dist/dagster-ssh-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:28 2020, max compression
```

## Comparing `dagster-ssh-0.9.9.tar` & `dagster-ssh-0.9.9rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      577 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/dagster_ssh/
--rw-r--r--   0 bobchen    (501) staff       (20)      246 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/dagster_ssh/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     9297 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/dagster_ssh/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/dagster_ssh/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/dagster_ssh.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      577 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/dagster_ssh.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      428 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/dagster_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/dagster_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/dagster_ssh.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/dagster_ssh.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/dagster_ssh.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/dagster_ssh_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/dagster_ssh_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8086 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/dagster_ssh_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/dagster_ssh_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:28:53.000000 dagster-ssh-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1043 2020-09-17 21:24:45.000000 dagster-ssh-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      119 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh/
+-rw-r--r--   0 bobchen    (501) staff       (20)      246 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     9297 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      428 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       30 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/dagster_ssh_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     8086 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh_tests/test_resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       89 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/dagster_ssh_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:28.000000 dagster-ssh-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1043 2020-09-17 21:04:59.000000 dagster-ssh-0.9.9rc1/setup.py
```

### Comparing `dagster-ssh-0.9.9/LICENSE` & `dagster-ssh-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-ssh-0.9.9/PKG-INFO` & `dagster-ssh-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-ssh
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for ssh Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-ssh
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-ssh-0.9.9/dagster_ssh/resources.py` & `dagster-ssh-0.9.9rc1/dagster_ssh/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-ssh-0.9.9/dagster_ssh.egg-info/PKG-INFO` & `dagster-ssh-0.9.9rc1/dagster_ssh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-ssh
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: Package for ssh Dagster framework components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-ssh
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-ssh-0.9.9/dagster_ssh_tests/test_resources.py` & `dagster-ssh-0.9.9rc1/dagster_ssh_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-ssh-0.9.9/setup.py` & `dagster-ssh-0.9.9rc1/setup.py`

 * *Files identical despite different names*

