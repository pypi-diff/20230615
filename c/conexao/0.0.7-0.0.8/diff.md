# Comparing `tmp/conexao-0.0.7.tar.gz` & `tmp/conexao-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conexao-0.0.7.tar", last modified: Thu Jan 19 12:15:22 2023, max compression
+gzip compressed data, was "conexao-0.0.8.tar", last modified: Thu Jun 15 14:42:35 2023, max compression
```

## Comparing `conexao-0.0.7.tar` & `conexao-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-01-19 12:15:22.597307 conexao-0.0.7/
--rw-r--r--   0 andres    (1000) andres    (1000)    35057 2022-10-04 11:42:55.000000 conexao-0.0.7/LICENSE
--rw-r--r--   0 andres    (1000) andres    (1000)     1949 2023-01-19 12:15:22.597307 conexao-0.0.7/PKG-INFO
--rw-r--r--   0 andres    (1000) andres    (1000)     1589 2022-10-31 18:00:04.000000 conexao-0.0.7/README.md
--rw-r--r--   0 andres    (1000) andres    (1000)      384 2023-01-19 12:14:19.000000 conexao-0.0.7/pyproject.toml
--rw-r--r--   0 andres    (1000) andres    (1000)       38 2023-01-19 12:15:22.597307 conexao-0.0.7/setup.cfg
-drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-01-19 12:15:22.590640 conexao-0.0.7/src/
-drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-01-19 12:15:22.593974 conexao-0.0.7/src/conexao/
--rw-r--r--   0 andres    (1000) andres    (1000)        0 2022-10-04 10:46:11.000000 conexao-0.0.7/src/conexao/__init__.py
--rw-r--r--   0 andres    (1000) andres    (1000)      834 2022-10-04 11:21:55.000000 conexao-0.0.7/src/conexao/cli.py
--rw-r--r--   0 andres    (1000) andres    (1000)      160 2022-09-28 09:59:07.000000 conexao-0.0.7/src/conexao/config.py
--rw-r--r--   0 andres    (1000) andres    (1000)      237 2022-09-27 14:01:41.000000 conexao-0.0.7/src/conexao/docker.py
-drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-01-19 12:15:22.597307 conexao-0.0.7/src/conexao/mongodb/
--rw-r--r--   0 andres    (1000) andres    (1000)       34 2022-10-05 12:07:37.000000 conexao-0.0.7/src/conexao/mongodb/__init__.py
-drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-01-19 12:15:22.597307 conexao-0.0.7/src/conexao/mongodb/auto/
--rw-r--r--   0 andres    (1000) andres    (1000)      753 2022-10-05 12:59:57.000000 conexao-0.0.7/src/conexao/mongodb/auto/__init__.py
--rw-r--r--   0 andres    (1000) andres    (1000)      487 2022-10-03 13:10:25.000000 conexao-0.0.7/src/conexao/mongodb/client.py
--rw-r--r--   0 andres    (1000) andres    (1000)     1615 2023-01-19 11:48:58.000000 conexao-0.0.7/src/conexao/ssh.py
-drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-01-19 12:15:22.593974 conexao-0.0.7/src/conexao.egg-info/
--rw-r--r--   0 andres    (1000) andres    (1000)     1949 2023-01-19 12:15:22.000000 conexao-0.0.7/src/conexao.egg-info/PKG-INFO
--rw-r--r--   0 andres    (1000) andres    (1000)      415 2023-01-19 12:15:22.000000 conexao-0.0.7/src/conexao.egg-info/SOURCES.txt
--rw-r--r--   0 andres    (1000) andres    (1000)        1 2023-01-19 12:15:22.000000 conexao-0.0.7/src/conexao.egg-info/dependency_links.txt
--rw-r--r--   0 andres    (1000) andres    (1000)       44 2023-01-19 12:15:22.000000 conexao-0.0.7/src/conexao.egg-info/entry_points.txt
--rw-r--r--   0 andres    (1000) andres    (1000)        8 2023-01-19 12:15:22.000000 conexao-0.0.7/src/conexao.egg-info/top_level.txt
+drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-06-15 14:42:35.508882 conexao-0.0.8/
+-rw-r--r--   0 andres    (1000) andres    (1000)    35057 2022-10-04 11:42:55.000000 conexao-0.0.8/LICENSE
+-rw-r--r--   0 andres    (1000) andres    (1000)     1949 2023-06-15 14:42:35.508882 conexao-0.0.8/PKG-INFO
+-rw-r--r--   0 andres    (1000) andres    (1000)     1589 2022-10-31 18:00:04.000000 conexao-0.0.8/README.md
+-rw-r--r--   0 andres    (1000) andres    (1000)      384 2023-06-15 14:41:39.000000 conexao-0.0.8/pyproject.toml
+-rw-r--r--   0 andres    (1000) andres    (1000)       38 2023-06-15 14:42:35.508882 conexao-0.0.8/setup.cfg
+drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-06-15 14:42:35.508882 conexao-0.0.8/src/
+drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-06-15 14:42:35.508882 conexao-0.0.8/src/conexao/
+-rw-r--r--   0 andres    (1000) andres    (1000)        0 2022-10-04 10:46:11.000000 conexao-0.0.8/src/conexao/__init__.py
+-rw-r--r--   0 andres    (1000) andres    (1000)      834 2022-10-04 11:21:55.000000 conexao-0.0.8/src/conexao/cli.py
+-rw-r--r--   0 andres    (1000) andres    (1000)      160 2022-09-28 09:59:07.000000 conexao-0.0.8/src/conexao/config.py
+-rw-r--r--   0 andres    (1000) andres    (1000)      237 2022-09-27 14:01:41.000000 conexao-0.0.8/src/conexao/docker.py
+drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-06-15 14:42:35.508882 conexao-0.0.8/src/conexao/mongodb/
+-rw-r--r--   0 andres    (1000) andres    (1000)       34 2022-10-05 12:07:37.000000 conexao-0.0.8/src/conexao/mongodb/__init__.py
+drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-06-15 14:42:35.508882 conexao-0.0.8/src/conexao/mongodb/auto/
+-rw-r--r--   0 andres    (1000) andres    (1000)      753 2022-10-05 12:59:57.000000 conexao-0.0.8/src/conexao/mongodb/auto/__init__.py
+-rw-r--r--   0 andres    (1000) andres    (1000)      562 2023-06-15 07:11:11.000000 conexao-0.0.8/src/conexao/mongodb/client.py
+-rw-r--r--   0 andres    (1000) andres    (1000)     1615 2023-01-19 11:48:58.000000 conexao-0.0.8/src/conexao/ssh.py
+drwxr-xr-x   0 andres    (1000) andres    (1000)        0 2023-06-15 14:42:35.508882 conexao-0.0.8/src/conexao.egg-info/
+-rw-r--r--   0 andres    (1000) andres    (1000)     1949 2023-06-15 14:42:35.000000 conexao-0.0.8/src/conexao.egg-info/PKG-INFO
+-rw-r--r--   0 andres    (1000) andres    (1000)      415 2023-06-15 14:42:35.000000 conexao-0.0.8/src/conexao.egg-info/SOURCES.txt
+-rw-r--r--   0 andres    (1000) andres    (1000)        1 2023-06-15 14:42:35.000000 conexao-0.0.8/src/conexao.egg-info/dependency_links.txt
+-rw-r--r--   0 andres    (1000) andres    (1000)       44 2023-06-15 14:42:35.000000 conexao-0.0.8/src/conexao.egg-info/entry_points.txt
+-rw-r--r--   0 andres    (1000) andres    (1000)        8 2023-06-15 14:42:35.000000 conexao-0.0.8/src/conexao.egg-info/top_level.txt
```

### Comparing `conexao-0.0.7/LICENSE` & `conexao-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `conexao-0.0.7/PKG-INFO` & `conexao-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conexao
-Version: 0.0.7
+Version: 0.0.8
 Summary: A connection helper.
 Project-URL: Homepage, https://gitlab.com/evagio/conexao
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `conexao-0.0.7/README.md` & `conexao-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `conexao-0.0.7/src/conexao/cli.py` & `conexao-0.0.8/src/conexao/cli.py`

 * *Files identical despite different names*

### Comparing `conexao-0.0.7/src/conexao/mongodb/auto/__init__.py` & `conexao-0.0.8/src/conexao/mongodb/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `conexao-0.0.7/src/conexao/ssh.py` & `conexao-0.0.8/src/conexao/ssh.py`

 * *Files identical despite different names*

### Comparing `conexao-0.0.7/src/conexao.egg-info/PKG-INFO` & `conexao-0.0.8/src/conexao.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conexao
-Version: 0.0.7
+Version: 0.0.8
 Summary: A connection helper.
 Project-URL: Homepage, https://gitlab.com/evagio/conexao
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

