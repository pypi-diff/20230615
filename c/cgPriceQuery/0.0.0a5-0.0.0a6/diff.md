# Comparing `tmp/cgPriceQuery-0.0.0a5.tar.gz` & `tmp/cgPriceQuery-0.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgPriceQuery-0.0.0a5.tar", last modified: Tue Oct 11 14:02:56 2022, max compression
+gzip compressed data, was "cgPriceQuery-0.0.0a6.tar", last modified: Thu Jun 15 16:48:35 2023, max compression
```

## Comparing `cgPriceQuery-0.0.0a5.tar` & `cgPriceQuery-0.0.0a6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gerg       (502) staff       (20)        0 2022-10-11 14:02:56.875450 cgPriceQuery-0.0.0a5/
--rw-r--r--   0 gerg       (502) staff       (20)       23 2022-01-08 14:48:48.000000 cgPriceQuery-0.0.0a5/MANIFEST.in
--rw-r--r--   0 gerg       (502) staff       (20)     1214 2022-10-11 14:02:56.875498 cgPriceQuery-0.0.0a5/PKG-INFO
--rw-r--r--   0 gerg       (502) staff       (20)      671 2022-01-08 17:06:08.000000 cgPriceQuery-0.0.0a5/README.md
-drwxr-xr-x   0 gerg       (502) staff       (20)        0 2022-10-11 14:02:56.874509 cgPriceQuery-0.0.0a5/cgPriceQuery/
--rw-r--r--   0 gerg       (502) staff       (20)        0 2022-01-07 19:45:57.000000 cgPriceQuery-0.0.0a5/cgPriceQuery/__init__.py
--rw-r--r--   0 gerg       (502) staff       (20)     6178 2022-03-04 16:44:16.000000 cgPriceQuery-0.0.0a5/cgPriceQuery/blockTimestamps.py
--rw-r--r--   0 gerg       (502) staff       (20)     3404 2022-03-21 12:53:37.000000 cgPriceQuery-0.0.0a5/cgPriceQuery/cgPriceQuery.py
--rw-r--r--   0 gerg       (502) staff       (20)     9148 2022-10-11 14:01:35.000000 cgPriceQuery-0.0.0a5/cgPriceQuery/historicalPriceQuery.py
-drwxr-xr-x   0 gerg       (502) staff       (20)        0 2022-10-11 14:02:56.875332 cgPriceQuery-0.0.0a5/cgPriceQuery.egg-info/
--rw-r--r--   0 gerg       (502) staff       (20)     1214 2022-10-11 14:02:56.000000 cgPriceQuery-0.0.0a5/cgPriceQuery.egg-info/PKG-INFO
--rw-r--r--   0 gerg       (502) staff       (20)      348 2022-10-11 14:02:56.000000 cgPriceQuery-0.0.0a5/cgPriceQuery.egg-info/SOURCES.txt
--rw-r--r--   0 gerg       (502) staff       (20)        1 2022-10-11 14:02:56.000000 cgPriceQuery-0.0.0a5/cgPriceQuery.egg-info/dependency_links.txt
--rw-r--r--   0 gerg       (502) staff       (20)       82 2022-10-11 14:02:56.000000 cgPriceQuery-0.0.0a5/cgPriceQuery.egg-info/requires.txt
--rw-r--r--   0 gerg       (502) staff       (20)       13 2022-10-11 14:02:56.000000 cgPriceQuery-0.0.0a5/cgPriceQuery.egg-info/top_level.txt
--rw-r--r--   0 gerg       (502) staff       (20)      103 2021-10-07 19:16:42.000000 cgPriceQuery-0.0.0a5/pyproject.toml
--rw-r--r--   0 gerg       (502) staff       (20)      754 2022-10-11 14:02:56.875727 cgPriceQuery-0.0.0a5/setup.cfg
+drwxr-xr-x   0 gerg       (502) staff       (20)        0 2023-06-15 16:48:35.059440 cgPriceQuery-0.0.0a6/
+-rw-r--r--   0 gerg       (502) staff       (20)       23 2022-01-08 14:48:48.000000 cgPriceQuery-0.0.0a6/MANIFEST.in
+-rw-r--r--   0 gerg       (502) staff       (20)     1214 2023-06-15 16:48:35.059496 cgPriceQuery-0.0.0a6/PKG-INFO
+-rw-r--r--   0 gerg       (502) staff       (20)      671 2022-01-08 17:06:08.000000 cgPriceQuery-0.0.0a6/README.md
+drwxr-xr-x   0 gerg       (502) staff       (20)        0 2023-06-15 16:48:35.058699 cgPriceQuery-0.0.0a6/cgPriceQuery/
+-rw-r--r--   0 gerg       (502) staff       (20)        0 2022-01-07 19:45:57.000000 cgPriceQuery-0.0.0a6/cgPriceQuery/__init__.py
+-rw-r--r--   0 gerg       (502) staff       (20)     6178 2022-03-04 16:44:16.000000 cgPriceQuery-0.0.0a6/cgPriceQuery/blockTimestamps.py
+-rw-r--r--   0 gerg       (502) staff       (20)     3432 2023-06-15 16:47:36.000000 cgPriceQuery-0.0.0a6/cgPriceQuery/cgPriceQuery.py
+-rw-r--r--   0 gerg       (502) staff       (20)     9148 2022-10-11 14:01:35.000000 cgPriceQuery-0.0.0a6/cgPriceQuery/historicalPriceQuery.py
+drwxr-xr-x   0 gerg       (502) staff       (20)        0 2023-06-15 16:48:35.059338 cgPriceQuery-0.0.0a6/cgPriceQuery.egg-info/
+-rw-r--r--   0 gerg       (502) staff       (20)     1214 2023-06-15 16:48:35.000000 cgPriceQuery-0.0.0a6/cgPriceQuery.egg-info/PKG-INFO
+-rw-r--r--   0 gerg       (502) staff       (20)      348 2023-06-15 16:48:35.000000 cgPriceQuery-0.0.0a6/cgPriceQuery.egg-info/SOURCES.txt
+-rw-r--r--   0 gerg       (502) staff       (20)        1 2023-06-15 16:48:35.000000 cgPriceQuery-0.0.0a6/cgPriceQuery.egg-info/dependency_links.txt
+-rw-r--r--   0 gerg       (502) staff       (20)       82 2023-06-15 16:48:35.000000 cgPriceQuery-0.0.0a6/cgPriceQuery.egg-info/requires.txt
+-rw-r--r--   0 gerg       (502) staff       (20)       13 2023-06-15 16:48:35.000000 cgPriceQuery-0.0.0a6/cgPriceQuery.egg-info/top_level.txt
+-rw-r--r--   0 gerg       (502) staff       (20)      103 2021-10-07 19:16:42.000000 cgPriceQuery-0.0.0a6/pyproject.toml
+-rw-r--r--   0 gerg       (502) staff       (20)      754 2023-06-15 16:48:35.059759 cgPriceQuery-0.0.0a6/setup.cfg
```

### Comparing `cgPriceQuery-0.0.0a5/PKG-INFO` & `cgPriceQuery-0.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgPriceQuery
-Version: 0.0.0a5
+Version: 0.0.0a6
 Summary: Historical and current CoinGecko price queries
 Home-page: https://github.com/gerrrg/cgPriceQuery
 Author: gerrrg
 Author-email: gerrrrrrrg@gmail.com
 Project-URL: Bug Tracker, https://github.com/gerrrg/cgPriceQuery/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cgPriceQuery-0.0.0a5/README.md` & `cgPriceQuery-0.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `cgPriceQuery-0.0.0a5/cgPriceQuery/blockTimestamps.py` & `cgPriceQuery-0.0.0a6/cgPriceQuery/blockTimestamps.py`

 * *Files identical despite different names*

### Comparing `cgPriceQuery-0.0.0a5/cgPriceQuery/cgPriceQuery.py` & `cgPriceQuery-0.0.0a6/cgPriceQuery/cgPriceQuery.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 class priceQuery():
 	networks = [
 		"ethereum",
 		"mainnet",
 		"polygon",
 		"arbitrum",
 		"fantom",
+		"xdai",
+		"polygon-zkevm"
 		];
 
 	def __init__(self, timeBufferSeconds=46800, verbose=False):
 		self.verbose = verbose;
 		self.timeBufferSeconds = timeBufferSeconds; #default=13h
 
 	def queryPriceAtTime(self, network, token, time):
```

### Comparing `cgPriceQuery-0.0.0a5/cgPriceQuery/historicalPriceQuery.py` & `cgPriceQuery-0.0.0a6/cgPriceQuery/historicalPriceQuery.py`

 * *Files identical despite different names*

### Comparing `cgPriceQuery-0.0.0a5/cgPriceQuery.egg-info/PKG-INFO` & `cgPriceQuery-0.0.0a6/cgPriceQuery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgPriceQuery
-Version: 0.0.0a5
+Version: 0.0.0a6
 Summary: Historical and current CoinGecko price queries
 Home-page: https://github.com/gerrrg/cgPriceQuery
 Author: gerrrg
 Author-email: gerrrrrrrg@gmail.com
 Project-URL: Bug Tracker, https://github.com/gerrrg/cgPriceQuery/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cgPriceQuery-0.0.0a5/setup.cfg` & `cgPriceQuery-0.0.0a6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cgPriceQuery
-version = 0.0.0a5
+version = 0.0.0a6
 author = gerrrg
 author_email = gerrrrrrrg@gmail.com
 description = Historical and current CoinGecko price queries
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gerrrg/cgPriceQuery
 project_urls =
```

