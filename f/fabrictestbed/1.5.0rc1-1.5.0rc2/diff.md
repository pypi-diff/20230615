# Comparing `tmp/fabrictestbed-1.5.0rc1.tar.gz` & `tmp/fabrictestbed-1.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.5.0rc1.tar", last modified: Thu May 11 18:11:42 2023, max compression
+gzip compressed data, was "fabrictestbed-1.5.0rc2.tar", last modified: Fri May 12 13:47:33 2023, max compression
```

## Comparing `fabrictestbed-1.5.0rc1.tar` & `fabrictestbed-1.5.0rc2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1806 2023-05-11 17:40:59.099816 fabrictestbed-1.5.0rc1/.gitignore
--rw-r--r--   0        0        0     1071 2023-05-11 17:40:59.100151 fabrictestbed-1.5.0rc1/LICENSE
--rw-r--r--   0        0        0       24 2023-05-11 17:40:59.100302 fabrictestbed-1.5.0rc1/MANIFEST.in
--rw-r--r--   0        0        0     5603 2023-05-11 17:40:59.100450 fabrictestbed-1.5.0rc1/README.md
--rw-r--r--   0        0        0       25 2023-05-11 18:11:24.842592 fabrictestbed-1.5.0rc1/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:40:59.100987 fabrictestbed-1.5.0rc1/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    18169 2023-05-11 17:40:59.101162 fabrictestbed-1.5.0rc1/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.101319 fabrictestbed-1.5.0rc1/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0     1914 2023-05-11 17:40:59.101479 fabrictestbed-1.5.0rc1/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2023-05-11 17:40:59.101641 fabrictestbed-1.5.0rc1/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    17886 2023-05-11 17:40:59.101856 fabrictestbed-1.5.0rc1/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2023-05-11 17:40:59.101985 fabrictestbed-1.5.0rc1/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.102200 fabrictestbed-1.5.0rc1/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0      909 2023-05-11 18:03:35.194348 fabrictestbed-1.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 17:40:59.102597 fabrictestbed-1.5.0rc1/test/__init__.py
--rw-r--r--   0        0        0     2210 2023-05-11 17:40:59.102713 fabrictestbed-1.5.0rc1/test/test_cli.py
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 fabrictestbed-1.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-05-11 17:40:59.099816 fabrictestbed-1.5.0rc2/.gitignore
+-rw-r--r--   0        0        0     1071 2023-05-11 17:40:59.100151 fabrictestbed-1.5.0rc2/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-11 17:40:59.100302 fabrictestbed-1.5.0rc2/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-05-11 17:40:59.100450 fabrictestbed-1.5.0rc2/README.md
+-rw-r--r--   0        0        0       25 2023-05-12 13:47:31.855483 fabrictestbed-1.5.0rc2/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:59.100987 fabrictestbed-1.5.0rc2/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    18169 2023-05-11 17:40:59.101162 fabrictestbed-1.5.0rc2/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.101319 fabrictestbed-1.5.0rc2/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-05-11 17:40:59.101479 fabrictestbed-1.5.0rc2/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-05-11 17:40:59.101641 fabrictestbed-1.5.0rc2/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    17886 2023-05-11 17:40:59.101856 fabrictestbed-1.5.0rc2/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:59.101985 fabrictestbed-1.5.0rc2/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.102200 fabrictestbed-1.5.0rc2/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0      909 2023-05-12 13:47:25.949580 fabrictestbed-1.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:59.102597 fabrictestbed-1.5.0rc2/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-05-11 17:40:59.102713 fabrictestbed-1.5.0rc2/test/test_cli.py
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 fabrictestbed-1.5.0rc2/PKG-INFO
```

### Comparing `fabrictestbed-1.5.0rc1/.gitignore` & `fabrictestbed-1.5.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc1/LICENSE` & `fabrictestbed-1.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc1/README.md` & `fabrictestbed-1.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc1/fabrictestbed/cli/cli.py` & `fabrictestbed-1.5.0rc2/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc1/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.5.0rc2/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc1/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.5.0rc2/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc1/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.5.0rc2/fabrictestbed/slice_manager/slice_manager.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc1/fabrictestbed/util/constants.py` & `fabrictestbed-1.5.0rc2/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc1/pyproject.toml` & `fabrictestbed-1.5.0rc2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "click",
     "fabric-credmgr-client==1.5.0rc1",
-    "fabric-orchestrator-client==1.5.0rc1",
+    "fabric-orchestrator-client==1.5.0rc2",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
 [project.urls]
 Home = "https://fabric-testbed.net/"
```

### Comparing `fabrictestbed-1.5.0rc1/test/test_cli.py` & `fabrictestbed-1.5.0rc2/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc1/PKG-INFO` & `fabrictestbed-1.5.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.5.0rc1
+Version: 1.5.0rc2
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: click
 Requires-Dist: fabric-credmgr-client==1.5.0rc1
-Requires-Dist: fabric-orchestrator-client==1.5.0rc1
+Requires-Dist: fabric-orchestrator-client==1.5.0rc2
 Requires-Dist: paramiko
 Project-URL: Home, https://fabric-testbed.net/
 Project-URL: Sources, https://github.com/fabric-testbed/fabric-cli
 
 [![PyPI](https://img.shields.io/pypi/v/fabrictestbed?style=plastic)](https://pypi.org/project/fabrictestbed/)
```

