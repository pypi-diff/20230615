# Comparing `tmp/eons-2.6.0.tar.gz` & `tmp/eons-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.6.0.tar", last modified: Wed Jun 14 01:27:57 2023, max compression
+gzip compressed data, was "eons-2.6.1.tar", last modified: Thu Jun 15 02:51:36 2023, max compression
```

## Comparing `eons-2.6.0.tar` & `eons-2.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.259849 eons-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-14 01:27:57.259849 eons-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-14 01:27:37.000000 eons-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.251849 eons-2.6.0/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.251849 eons-2.6.0/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 01:27:47.000000 eons-2.6.0/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    89323 2023-06-14 01:27:47.000000 eons-2.6.0/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.255849 eons-2.6.0/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:27:47.000000 eons-2.6.0/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.259849 eons-2.6.0/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:27:47.000000 eons-2.6.0/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 01:27:27.000000 eons-2.6.0/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:27:57.255849 eons-2.6.0/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-14 01:27:57.000000 eons-2.6.0/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-14 01:27:47.000000 eons-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-14 01:27:57.259849 eons-2.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.823963 eons-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-15 02:51:36.823963 eons-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-15 02:51:21.000000 eons-2.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.819963 eons-2.6.1/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.819963 eons-2.6.1/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 02:51:28.000000 eons-2.6.1/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89390 2023-06-15 02:51:28.000000 eons-2.6.1/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.819963 eons-2.6.1/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:51:28.000000 eons-2.6.1/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.823963 eons-2.6.1/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:51:28.000000 eons-2.6.1/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-15 02:51:13.000000 eons-2.6.1/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:51:36.819963 eons-2.6.1/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 02:51:36.000000 eons-2.6.1/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 02:51:28.000000 eons-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 02:51:36.823963 eons-2.6.1/setup.cfg
```

### Comparing `eons-2.6.0/PKG-INFO` & `eons-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.0
+Version: 2.6.1
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.0/README.md` & `eons-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.6.0/pkg/eons/eons.py` & `eons-2.6.1/pkg/eons/eons.py`

 * *Files 0% similar despite different names*

```diff
@@ -811,17 +811,18 @@
 
 		#NOTE: In order for *this to be called multiple times, required and optional kwargs must always be fetched and not use stale data from *this.
 
 		if (this.requiredKWArgs):
 			for rkw in this.requiredKWArgs:
 				if (rkw in argMap.keys()):
 					continue
-
-				fetched = this.FetchWithout(['this'], rkw)
-				if (fetched is not None):
+				
+				logging.debug(f"Fetching required value {rkw}...")
+				fetched, found = this.FetchWithout(['this'], rkw, start = False)
+				if (found):
 					this.Set(rkw, fetched)
 					continue
 
 				# Nope. Failed.
 				logging.error(f"{rkw} required but not found.")
 				raise MissingArgumentError(f"Key-word argument {rkw} could not be Fetched.")
```

### Comparing `eons-2.6.0/pkg/eons/method/External.py` & `eons-2.6.1/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.0/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.6.1/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.0/pkg/eons/resolve/resolve_import_module.py` & `eons-2.6.1/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.6.1/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.0/pkg/eons.egg-info/PKG-INFO` & `eons-2.6.1/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.0
+Version: 2.6.1
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.0/pkg/eons.egg-info/SOURCES.txt` & `eons-2.6.1/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.6.0/setup.cfg` & `eons-2.6.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.6.0
+version = 2.6.1
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,18 +18,18 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	tqdm
 	jsonpickle
-	pyyaml
 	requests
+	tqdm
+	pyyaml
 	eot
 	requests_futures
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
```

