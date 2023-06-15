# Comparing `tmp/predeployed-generator-1.2.0a1.tar.gz` & `tmp/predeployed-generator-1.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predeployed-generator-1.2.0a1.tar", last modified: Thu Jun 15 13:19:41 2023, max compression
+gzip compressed data, was "predeployed-generator-1.2.0b0.tar", last modified: Tue Jun 13 12:45:02 2023, max compression
```

## Comparing `predeployed-generator-1.2.0a1.tar` & `predeployed-generator-1.2.0b0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:19:41.980733 predeployed-generator-1.2.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 13:19:41.980733 predeployed-generator-1.2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-15 13:19:41.980733 predeployed-generator-1.2.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:19:41.976734 predeployed-generator-1.2.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:19:41.976734 predeployed-generator-1.2.0a1/src/predeployed_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/contract_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:19:41.976734 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/access_control_enumerable_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:19:41.980733 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/.keep
--rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-06-15 13:19:34.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/ProxyAdmin.json
--rw-r--r--   0 runner    (1001) docker     (123)   518781 2023-06-15 13:19:34.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/ProxyAdmin.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-06-15 13:19:35.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/TransparentUpgradeableProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)   518798 2023-06-15 13:19:35.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/TransparentUpgradeableProxy.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/openzeppelin_contract_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/proxy_admin_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/transparent_upgradeable_proxy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/src/predeployed_generator/upgradeable_contract_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:19:41.976734 predeployed-generator-1.2.0a1/src/predeployed_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 13:19:41.000000 predeployed-generator-1.2.0a1/src/predeployed_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-15 13:19:41.000000 predeployed-generator-1.2.0a1/src/predeployed_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:19:41.000000 predeployed-generator-1.2.0a1/src/predeployed_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 13:19:41.000000 predeployed-generator-1.2.0a1/src/predeployed_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 13:19:41.000000 predeployed-generator-1.2.0a1/src/predeployed_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:19:41.980733 predeployed-generator-1.2.0a1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/test/test_access_control_enumerable_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/test/test_artifacts_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/test/test_contract_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/test/test_proxy_admin_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/test/test_transparent_upgradeable_proxy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-15 13:18:04.000000 predeployed-generator-1.2.0a1/test/test_upgradeable_contract_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 13:18:14.000000 predeployed-generator-1.2.0a1/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:45:02.102496 predeployed-generator-1.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-13 12:45:02.102496 predeployed-generator-1.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-13 12:45:02.102496 predeployed-generator-1.2.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:45:02.098495 predeployed-generator-1.2.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:45:02.098495 predeployed-generator-1.2.0b0/src/predeployed_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/contract_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:45:02.102496 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/access_control_enumerable_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:45:02.102496 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-06-13 12:44:54.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/ProxyAdmin.json
+-rw-r--r--   0 runner    (1001) docker     (123)   518781 2023-06-13 12:44:54.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/ProxyAdmin.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-06-13 12:44:54.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/TransparentUpgradeableProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)   518798 2023-06-13 12:44:54.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/TransparentUpgradeableProxy.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/openzeppelin_contract_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/proxy_admin_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/transparent_upgradeable_proxy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/src/predeployed_generator/upgradeable_contract_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:45:02.102496 predeployed-generator-1.2.0b0/src/predeployed_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-13 12:45:02.000000 predeployed-generator-1.2.0b0/src/predeployed_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-13 12:45:02.000000 predeployed-generator-1.2.0b0/src/predeployed_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:45:02.000000 predeployed-generator-1.2.0b0/src/predeployed_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 12:45:02.000000 predeployed-generator-1.2.0b0/src/predeployed_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 12:45:02.000000 predeployed-generator-1.2.0b0/src/predeployed_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:45:02.102496 predeployed-generator-1.2.0b0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/test/test_access_control_enumerable_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/test/test_artifacts_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/test/test_contract_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/test/test_proxy_admin_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/test/test_transparent_upgradeable_proxy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-13 12:43:20.000000 predeployed-generator-1.2.0b0/test/test_upgradeable_contract_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 12:43:32.000000 predeployed-generator-1.2.0b0/version.txt
```

### Comparing `predeployed-generator-1.2.0a1/LICENSE` & `predeployed-generator-1.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/PKG-INFO` & `predeployed-generator-1.2.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predeployed-generator
-Version: 1.2.0a1
+Version: 1.2.0b0
 Summary: A tool for generating memory layout of smart contracts written in solidity
 Home-page: https://github.com/skalenetwork/predeployed-generator
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `predeployed-generator-1.2.0a1/setup.cfg` & `predeployed-generator-1.2.0b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/contract_generator.py` & `predeployed-generator-1.2.0b0/src/predeployed_generator/contract_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/access_control_enumerable_generator.py` & `predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/access_control_enumerable_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/ProxyAdmin.json` & `predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/ProxyAdmin.json`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/ProxyAdmin.meta.json` & `predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/ProxyAdmin.meta.json`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/TransparentUpgradeableProxy.json` & `predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/TransparentUpgradeableProxy.json`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/artifacts/TransparentUpgradeableProxy.meta.json` & `predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/artifacts/TransparentUpgradeableProxy.meta.json`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/openzeppelin_contract_generator.py` & `predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/openzeppelin_contract_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/proxy_admin_generator.py` & `predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/proxy_admin_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/openzeppelin/transparent_upgradeable_proxy_generator.py` & `predeployed-generator-1.2.0b0/src/predeployed_generator/openzeppelin/transparent_upgradeable_proxy_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/tools.py` & `predeployed-generator-1.2.0b0/src/predeployed_generator/tools.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator/upgradeable_contract_generator.py` & `predeployed-generator-1.2.0b0/src/predeployed_generator/upgradeable_contract_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator.egg-info/PKG-INFO` & `predeployed-generator-1.2.0b0/src/predeployed_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: predeployed-generator
-Version: 1.2.0a1
+Version: 1.2.0b0
 Summary: A tool for generating memory layout of smart contracts written in solidity
 Home-page: https://github.com/skalenetwork/predeployed-generator
 Author: Dmytro Stebaiev
 Author-email: dmytro@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `predeployed-generator-1.2.0a1/src/predeployed_generator.egg-info/SOURCES.txt` & `predeployed-generator-1.2.0b0/src/predeployed_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/test/test_access_control_enumerable_generator.py` & `predeployed-generator-1.2.0b0/test/test_access_control_enumerable_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/test/test_artifacts_handler.py` & `predeployed-generator-1.2.0b0/test/test_artifacts_handler.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/test/test_contract_generator.py` & `predeployed-generator-1.2.0b0/test/test_contract_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/test/test_proxy_admin_generator.py` & `predeployed-generator-1.2.0b0/test/test_proxy_admin_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/test/test_transparent_upgradeable_proxy_generator.py` & `predeployed-generator-1.2.0b0/test/test_transparent_upgradeable_proxy_generator.py`

 * *Files identical despite different names*

### Comparing `predeployed-generator-1.2.0a1/test/test_upgradeable_contract_generator.py` & `predeployed-generator-1.2.0b0/test/test_upgradeable_contract_generator.py`

 * *Files identical despite different names*

