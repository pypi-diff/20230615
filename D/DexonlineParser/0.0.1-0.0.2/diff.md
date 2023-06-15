# Comparing `tmp/dexonlineparser-0.0.1.tar.gz` & `tmp/dexonlineparser-0.0.2.tar.gz`

## Comparing `dexonlineparser-0.0.1.tar` & `dexonlineparser-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dexonlineparser-0.0.1/src/DexonlineParser/__init__.py
--rwxr-xr-x   0        0        0    15583 2020-02-02 00:00:00.000000 dexonlineparser-0.0.1/src/DexonlineParser/parser.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dexonlineparser-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dexonlineparser-0.0.1/README.md
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 dexonlineparser-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 dexonlineparser-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 dexonlineparser-0.0.2/src/DexonlineParser/__init__.py
+-rwxr-xr-x   0        0        0    15583 2020-02-02 00:00:00.000000 dexonlineparser-0.0.2/src/DexonlineParser/parser.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dexonlineparser-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dexonlineparser-0.0.2/README.md
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 dexonlineparser-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 dexonlineparser-0.0.2/PKG-INFO
```

### Comparing `dexonlineparser-0.0.1/src/DexonlineParser/parser.py` & `dexonlineparser-0.0.2/src/DexonlineParser/parser.py`

 * *Files identical despite different names*

### Comparing `dexonlineparser-0.0.1/LICENSE` & `dexonlineparser-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dexonlineparser-0.0.1/pyproject.toml` & `dexonlineparser-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DexonlineParser"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Eric Floyd", email="erixefb@gmail.com" },
 ]
 description = "Dexonline Parser package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

