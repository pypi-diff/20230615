# Comparing `tmp/cgPriceQuery-0.0.0a8.tar.gz` & `tmp/cgPriceQuery-0.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgPriceQuery-0.0.0a8.tar", last modified: Thu Jun 15 17:03:02 2023, max compression
+gzip compressed data, was "cgPriceQuery-0.0.0a9.tar", last modified: Thu Jun 15 17:05:08 2023, max compression
```

## Comparing `cgPriceQuery-0.0.0a8.tar` & `cgPriceQuery-0.0.0a9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gerg       (502) staff       (20)        0 2023-06-15 17:03:02.413813 cgPriceQuery-0.0.0a8/
--rw-r--r--   0 gerg       (502) staff       (20)       23 2022-01-08 14:48:48.000000 cgPriceQuery-0.0.0a8/MANIFEST.in
--rw-r--r--   0 gerg       (502) staff       (20)     1214 2023-06-15 17:03:02.413861 cgPriceQuery-0.0.0a8/PKG-INFO
--rw-r--r--   0 gerg       (502) staff       (20)      671 2022-01-08 17:06:08.000000 cgPriceQuery-0.0.0a8/README.md
-drwxr-xr-x   0 gerg       (502) staff       (20)        0 2023-06-15 17:03:02.413153 cgPriceQuery-0.0.0a8/cgPriceQuery/
--rw-r--r--   0 gerg       (502) staff       (20)        0 2022-01-07 19:45:57.000000 cgPriceQuery-0.0.0a8/cgPriceQuery/__init__.py
--rw-r--r--   0 gerg       (502) staff       (20)     6336 2023-06-15 17:02:06.000000 cgPriceQuery-0.0.0a8/cgPriceQuery/blockTimestamps.py
--rw-r--r--   0 gerg       (502) staff       (20)     3432 2023-06-15 16:47:36.000000 cgPriceQuery-0.0.0a8/cgPriceQuery/cgPriceQuery.py
--rw-r--r--   0 gerg       (502) staff       (20)     9273 2023-06-15 16:55:29.000000 cgPriceQuery-0.0.0a8/cgPriceQuery/historicalPriceQuery.py
-drwxr-xr-x   0 gerg       (502) staff       (20)        0 2023-06-15 17:03:02.413723 cgPriceQuery-0.0.0a8/cgPriceQuery.egg-info/
--rw-r--r--   0 gerg       (502) staff       (20)     1214 2023-06-15 17:03:02.000000 cgPriceQuery-0.0.0a8/cgPriceQuery.egg-info/PKG-INFO
--rw-r--r--   0 gerg       (502) staff       (20)      348 2023-06-15 17:03:02.000000 cgPriceQuery-0.0.0a8/cgPriceQuery.egg-info/SOURCES.txt
--rw-r--r--   0 gerg       (502) staff       (20)        1 2023-06-15 17:03:02.000000 cgPriceQuery-0.0.0a8/cgPriceQuery.egg-info/dependency_links.txt
--rw-r--r--   0 gerg       (502) staff       (20)       82 2023-06-15 17:03:02.000000 cgPriceQuery-0.0.0a8/cgPriceQuery.egg-info/requires.txt
--rw-r--r--   0 gerg       (502) staff       (20)       13 2023-06-15 17:03:02.000000 cgPriceQuery-0.0.0a8/cgPriceQuery.egg-info/top_level.txt
--rw-r--r--   0 gerg       (502) staff       (20)      103 2021-10-07 19:16:42.000000 cgPriceQuery-0.0.0a8/pyproject.toml
--rw-r--r--   0 gerg       (502) staff       (20)      754 2023-06-15 17:03:02.414105 cgPriceQuery-0.0.0a8/setup.cfg
+drwxr-xr-x   0 gerg       (502) staff       (20)        0 2023-06-15 17:05:08.655607 cgPriceQuery-0.0.0a9/
+-rw-r--r--   0 gerg       (502) staff       (20)       23 2022-01-08 14:48:48.000000 cgPriceQuery-0.0.0a9/MANIFEST.in
+-rw-r--r--   0 gerg       (502) staff       (20)     1214 2023-06-15 17:05:08.655655 cgPriceQuery-0.0.0a9/PKG-INFO
+-rw-r--r--   0 gerg       (502) staff       (20)      671 2022-01-08 17:06:08.000000 cgPriceQuery-0.0.0a9/README.md
+drwxr-xr-x   0 gerg       (502) staff       (20)        0 2023-06-15 17:05:08.654946 cgPriceQuery-0.0.0a9/cgPriceQuery/
+-rw-r--r--   0 gerg       (502) staff       (20)        0 2022-01-07 19:45:57.000000 cgPriceQuery-0.0.0a9/cgPriceQuery/__init__.py
+-rw-r--r--   0 gerg       (502) staff       (20)     6336 2023-06-15 17:02:06.000000 cgPriceQuery-0.0.0a9/cgPriceQuery/blockTimestamps.py
+-rw-r--r--   0 gerg       (502) staff       (20)     3444 2023-06-15 17:04:29.000000 cgPriceQuery-0.0.0a9/cgPriceQuery/cgPriceQuery.py
+-rw-r--r--   0 gerg       (502) staff       (20)     9273 2023-06-15 16:55:29.000000 cgPriceQuery-0.0.0a9/cgPriceQuery/historicalPriceQuery.py
+drwxr-xr-x   0 gerg       (502) staff       (20)        0 2023-06-15 17:05:08.655514 cgPriceQuery-0.0.0a9/cgPriceQuery.egg-info/
+-rw-r--r--   0 gerg       (502) staff       (20)     1214 2023-06-15 17:05:08.000000 cgPriceQuery-0.0.0a9/cgPriceQuery.egg-info/PKG-INFO
+-rw-r--r--   0 gerg       (502) staff       (20)      348 2023-06-15 17:05:08.000000 cgPriceQuery-0.0.0a9/cgPriceQuery.egg-info/SOURCES.txt
+-rw-r--r--   0 gerg       (502) staff       (20)        1 2023-06-15 17:05:08.000000 cgPriceQuery-0.0.0a9/cgPriceQuery.egg-info/dependency_links.txt
+-rw-r--r--   0 gerg       (502) staff       (20)       82 2023-06-15 17:05:08.000000 cgPriceQuery-0.0.0a9/cgPriceQuery.egg-info/requires.txt
+-rw-r--r--   0 gerg       (502) staff       (20)       13 2023-06-15 17:05:08.000000 cgPriceQuery-0.0.0a9/cgPriceQuery.egg-info/top_level.txt
+-rw-r--r--   0 gerg       (502) staff       (20)      103 2021-10-07 19:16:42.000000 cgPriceQuery-0.0.0a9/pyproject.toml
+-rw-r--r--   0 gerg       (502) staff       (20)      754 2023-06-15 17:05:08.655885 cgPriceQuery-0.0.0a9/setup.cfg
```

### Comparing `cgPriceQuery-0.0.0a8/PKG-INFO` & `cgPriceQuery-0.0.0a9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgPriceQuery
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: Historical and current CoinGecko price queries
 Home-page: https://github.com/gerrrg/cgPriceQuery
 Author: gerrrg
 Author-email: gerrrrrrrg@gmail.com
 Project-URL: Bug Tracker, https://github.com/gerrrg/cgPriceQuery/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cgPriceQuery-0.0.0a8/README.md` & `cgPriceQuery-0.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `cgPriceQuery-0.0.0a8/cgPriceQuery/blockTimestamps.py` & `cgPriceQuery-0.0.0a9/cgPriceQuery/blockTimestamps.py`

 * *Files identical despite different names*

### Comparing `cgPriceQuery-0.0.0a8/cgPriceQuery/cgPriceQuery.py` & `cgPriceQuery-0.0.0a9/cgPriceQuery/cgPriceQuery.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 	networks = [
 		"ethereum",
 		"mainnet",
 		"polygon",
 		"arbitrum",
 		"fantom",
 		"xdai",
+		"gnosis",
 		"polygon-zkevm"
 		];
 
 	def __init__(self, timeBufferSeconds=46800, verbose=False):
 		self.verbose = verbose;
 		self.timeBufferSeconds = timeBufferSeconds; #default=13h
```

### Comparing `cgPriceQuery-0.0.0a8/cgPriceQuery/historicalPriceQuery.py` & `cgPriceQuery-0.0.0a9/cgPriceQuery/historicalPriceQuery.py`

 * *Files identical despite different names*

### Comparing `cgPriceQuery-0.0.0a8/cgPriceQuery.egg-info/PKG-INFO` & `cgPriceQuery-0.0.0a9/cgPriceQuery.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgPriceQuery
-Version: 0.0.0a8
+Version: 0.0.0a9
 Summary: Historical and current CoinGecko price queries
 Home-page: https://github.com/gerrrg/cgPriceQuery
 Author: gerrrg
 Author-email: gerrrrrrrg@gmail.com
 Project-URL: Bug Tracker, https://github.com/gerrrg/cgPriceQuery/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

