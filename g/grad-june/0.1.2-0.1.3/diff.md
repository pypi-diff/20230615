# Comparing `tmp/grad_june-0.1.2.tar.gz` & `tmp/grad_june-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grad_june-0.1.2.tar", last modified: Thu Jun 15 13:44:47 2023, max compression
+gzip compressed data, was "grad_june-0.1.3.tar", last modified: Thu Jun 15 13:52:44 2023, max compression
```

## Comparing `grad_june-0.1.2.tar` & `grad_june-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:44:47.486155 grad_june-0.1.2/
--rw-r--r--   0 arnull     (504) staff       (20)     1077 2022-06-16 10:39:12.000000 grad_june-0.1.2/LICENSE
--rw-r--r--   0 arnull     (504) staff       (20)     1283 2023-06-15 13:44:47.486225 grad_june-0.1.2/PKG-INFO
--rw-r--r--   0 arnull     (504) staff       (20)      972 2023-01-20 11:11:57.000000 grad_june-0.1.2/README.md
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:44:47.483002 grad_june-0.1.2/grad_june/
--rw-r--r--   0 arnull     (504) staff       (20)      368 2023-06-15 10:47:46.000000 grad_june-0.1.2/grad_june/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)      755 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/cuda_utils.py
--rw-r--r--   0 arnull     (504) staff       (20)     5931 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/default_parameters.py
--rw-r--r--   0 arnull     (504) staff       (20)     2601 2023-06-15 10:48:16.000000 grad_june-0.1.2/grad_june/infection.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:44:47.484051 grad_june-0.1.2/grad_june/infection_networks/
--rw-r--r--   0 arnull     (504) staff       (20)      315 2023-03-20 16:13:20.000000 grad_june-0.1.2/grad_june/infection_networks/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)     5657 2023-06-15 10:48:16.000000 grad_june-0.1.2/grad_june/infection_networks/base.py
--rw-r--r--   0 arnull     (504) staff       (20)     4166 2023-06-15 10:48:16.000000 grad_june-0.1.2/grad_june/infection_networks/leisure_network.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:44:47.485240 grad_june-0.1.2/grad_june/june_world_loader/
--rw-r--r--   0 arnull     (504) staff       (20)       85 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/june_world_loader/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)     1398 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/june_world_loader/agent_data_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      184 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/june_world_loader/care_home_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      178 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/june_world_loader/company_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)     1462 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/june_world_loader/graph_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      184 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/june_world_loader/household_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)     4032 2023-03-20 13:17:17.000000 grad_june-0.1.2/grad_june/june_world_loader/leisure_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)     1624 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/june_world_loader/network_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      175 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/june_world_loader/school_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)      188 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/june_world_loader/university_loader.py
--rw-r--r--   0 arnull     (504) staff       (20)     5414 2023-06-15 10:48:16.000000 grad_june-0.1.2/grad_june/model.py
--rw-r--r--   0 arnull     (504) staff       (20)      201 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/paths.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:44:47.485838 grad_june-0.1.2/grad_june/policies/
--rw-r--r--   0 arnull     (504) staff       (20)      258 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/policies/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)      757 2023-04-18 17:56:26.000000 grad_june-0.1.2/grad_june/policies/close_venue_policies.py
--rw-r--r--   0 arnull     (504) staff       (20)     1027 2023-06-15 10:47:46.000000 grad_june-0.1.2/grad_june/policies/interaction_policies.py
--rw-r--r--   0 arnull     (504) staff       (20)     4073 2023-03-20 11:51:45.000000 grad_june-0.1.2/grad_june/policies/policies.py
--rw-r--r--   0 arnull     (504) staff       (20)     1097 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/policies/quarantine_policies.py
--rw-r--r--   0 arnull     (504) staff       (20)     9423 2023-06-15 10:48:16.000000 grad_june-0.1.2/grad_june/runner.py
--rw-r--r--   0 arnull     (504) staff       (20)     9981 2023-06-15 10:48:16.000000 grad_june-0.1.2/grad_june/symptoms.py
--rw-r--r--   0 arnull     (504) staff       (20)     4579 2023-01-20 11:11:57.000000 grad_june-0.1.2/grad_june/timer.py
--rw-r--r--   0 arnull     (504) staff       (20)     1877 2023-06-15 10:48:16.000000 grad_june-0.1.2/grad_june/transmission.py
--rw-r--r--   0 arnull     (504) staff       (20)     4572 2023-06-15 10:48:16.000000 grad_june-0.1.2/grad_june/utils.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:44:47.483678 grad_june-0.1.2/grad_june.egg-info/
--rw-r--r--   0 arnull     (504) staff       (20)     1283 2023-06-15 13:44:47.000000 grad_june-0.1.2/grad_june.egg-info/PKG-INFO
--rw-r--r--   0 arnull     (504) staff       (20)     1256 2023-06-15 13:44:47.000000 grad_june-0.1.2/grad_june.egg-info/SOURCES.txt
--rw-r--r--   0 arnull     (504) staff       (20)        1 2023-06-15 13:44:47.000000 grad_june-0.1.2/grad_june.egg-info/dependency_links.txt
--rw-r--r--   0 arnull     (504) staff       (20)       94 2023-06-15 13:44:47.000000 grad_june-0.1.2/grad_june.egg-info/requires.txt
--rw-r--r--   0 arnull     (504) staff       (20)       15 2023-06-15 13:44:47.000000 grad_june-0.1.2/grad_june.egg-info/top_level.txt
--rw-r--r--   0 arnull     (504) staff       (20)      126 2023-06-15 13:44:47.486575 grad_june-0.1.2/setup.cfg
--rw-r--r--   0 arnull     (504) staff       (20)      976 2023-06-15 13:43:32.000000 grad_june-0.1.2/setup.py
-drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:44:47.486050 grad_june-0.1.2/test/
--rw-r--r--   0 arnull     (504) staff       (20)        0 2022-06-16 10:39:12.000000 grad_june-0.1.2/test/__init__.py
--rw-r--r--   0 arnull     (504) staff       (20)     3869 2023-06-15 10:48:16.000000 grad_june-0.1.2/test/conftest.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:52:44.129534 grad_june-0.1.3/
+-rw-r--r--   0 arnull     (504) staff       (20)     1077 2022-06-16 10:39:12.000000 grad_june-0.1.3/LICENSE
+-rw-r--r--   0 arnull     (504) staff       (20)     1059 2023-06-15 13:52:44.129603 grad_june-0.1.3/PKG-INFO
+-rw-r--r--   0 arnull     (504) staff       (20)      748 2023-06-15 13:45:30.000000 grad_june-0.1.3/README.md
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:52:44.126608 grad_june-0.1.3/grad_june/
+-rw-r--r--   0 arnull     (504) staff       (20)      368 2023-06-15 10:47:46.000000 grad_june-0.1.3/grad_june/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)      755 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/cuda_utils.py
+-rw-r--r--   0 arnull     (504) staff       (20)     5931 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/default_parameters.py
+-rw-r--r--   0 arnull     (504) staff       (20)     2601 2023-06-15 10:48:16.000000 grad_june-0.1.3/grad_june/infection.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:52:44.127509 grad_june-0.1.3/grad_june/infection_networks/
+-rw-r--r--   0 arnull     (504) staff       (20)      315 2023-03-20 16:13:20.000000 grad_june-0.1.3/grad_june/infection_networks/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)     5657 2023-06-15 10:48:16.000000 grad_june-0.1.3/grad_june/infection_networks/base.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4166 2023-06-15 10:48:16.000000 grad_june-0.1.3/grad_june/infection_networks/leisure_network.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:52:44.128649 grad_june-0.1.3/grad_june/june_world_loader/
+-rw-r--r--   0 arnull     (504) staff       (20)       85 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/june_world_loader/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1398 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/june_world_loader/agent_data_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      184 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/june_world_loader/care_home_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      178 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/june_world_loader/company_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1462 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/june_world_loader/graph_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      184 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/june_world_loader/household_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4032 2023-03-20 13:17:17.000000 grad_june-0.1.3/grad_june/june_world_loader/leisure_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1624 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/june_world_loader/network_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      175 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/june_world_loader/school_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)      188 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/june_world_loader/university_loader.py
+-rw-r--r--   0 arnull     (504) staff       (20)     5414 2023-06-15 10:48:16.000000 grad_june-0.1.3/grad_june/model.py
+-rw-r--r--   0 arnull     (504) staff       (20)      194 2023-06-15 13:49:23.000000 grad_june-0.1.3/grad_june/paths.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:52:44.129222 grad_june-0.1.3/grad_june/policies/
+-rw-r--r--   0 arnull     (504) staff       (20)      258 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/policies/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)      757 2023-04-18 17:56:26.000000 grad_june-0.1.3/grad_june/policies/close_venue_policies.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1027 2023-06-15 10:47:46.000000 grad_june-0.1.3/grad_june/policies/interaction_policies.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4073 2023-03-20 11:51:45.000000 grad_june-0.1.3/grad_june/policies/policies.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1097 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/policies/quarantine_policies.py
+-rw-r--r--   0 arnull     (504) staff       (20)     9423 2023-06-15 10:48:16.000000 grad_june-0.1.3/grad_june/runner.py
+-rw-r--r--   0 arnull     (504) staff       (20)     9981 2023-06-15 10:48:16.000000 grad_june-0.1.3/grad_june/symptoms.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4579 2023-01-20 11:11:57.000000 grad_june-0.1.3/grad_june/timer.py
+-rw-r--r--   0 arnull     (504) staff       (20)     1877 2023-06-15 10:48:16.000000 grad_june-0.1.3/grad_june/transmission.py
+-rw-r--r--   0 arnull     (504) staff       (20)     4572 2023-06-15 10:48:16.000000 grad_june-0.1.3/grad_june/utils.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:52:44.127169 grad_june-0.1.3/grad_june.egg-info/
+-rw-r--r--   0 arnull     (504) staff       (20)     1059 2023-06-15 13:52:44.000000 grad_june-0.1.3/grad_june.egg-info/PKG-INFO
+-rw-r--r--   0 arnull     (504) staff       (20)     1256 2023-06-15 13:52:44.000000 grad_june-0.1.3/grad_june.egg-info/SOURCES.txt
+-rw-r--r--   0 arnull     (504) staff       (20)        1 2023-06-15 13:52:44.000000 grad_june-0.1.3/grad_june.egg-info/dependency_links.txt
+-rw-r--r--   0 arnull     (504) staff       (20)       94 2023-06-15 13:52:44.000000 grad_june-0.1.3/grad_june.egg-info/requires.txt
+-rw-r--r--   0 arnull     (504) staff       (20)       15 2023-06-15 13:52:44.000000 grad_june-0.1.3/grad_june.egg-info/top_level.txt
+-rw-r--r--   0 arnull     (504) staff       (20)      126 2023-06-15 13:52:44.129837 grad_june-0.1.3/setup.cfg
+-rw-r--r--   0 arnull     (504) staff       (20)      891 2023-06-15 13:52:27.000000 grad_june-0.1.3/setup.py
+drwxr-xr-x   0 arnull     (504) staff       (20)        0 2023-06-15 13:52:44.129428 grad_june-0.1.3/test/
+-rw-r--r--   0 arnull     (504) staff       (20)        0 2022-06-16 10:39:12.000000 grad_june-0.1.3/test/__init__.py
+-rw-r--r--   0 arnull     (504) staff       (20)     3869 2023-06-15 10:48:16.000000 grad_june-0.1.3/test/conftest.py
```

### Comparing `grad_june-0.1.2/LICENSE` & `grad_june-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/PKG-INFO` & `grad_june-0.1.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grad_june
-Version: 0.1.2
+Version: 0.1.3
 Summary: Differentiable implementation of the JUNE model.
 Home-page: https://github.com/arnauqb/GradABM-JUNE
 Author: Arnau Quera-Bofarull
 Author-email: arnauq@protonmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,29 +14,16 @@
 [![Build and test package](https://github.com/arnauqb/GradABM-JUNE/actions/workflows/ci.yml/badge.svg)](https://github.com/arnauqb/GradABM-JUNE/actions/workflows/ci.yml)
 
 # GradABM-JUNE
 Implementation of the JUNE model using the GradABM framework.
 
 # Setup 
 
-Install requirements
+The easiest way is to install the package from the PyPI package repository
 
-```bash
-pip install -r requirements.txt
-```
-
-and install PyTorch geometric, manually for now:
-
-```bash
-pip install torch-scatter torch-sparse torch-cluster torch-geometric -f https://data.pyg.org/whl/torch-1.13.0+cpu.html
-```
-
-Then install the GradABM-JUNE package
-
-```bash
-pip install -e .
 ```
+pip install 
 
 
 # Usage
 
 See the [docs](https://arnauqb.github.io/GradABM-JUNE/).
```

### Comparing `grad_june-0.1.2/grad_june/cuda_utils.py` & `grad_june-0.1.3/grad_june/cuda_utils.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/default_parameters.py` & `grad_june-0.1.3/grad_june/default_parameters.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/infection.py` & `grad_june-0.1.3/grad_june/infection.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/infection_networks/base.py` & `grad_june-0.1.3/grad_june/infection_networks/base.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/infection_networks/leisure_network.py` & `grad_june-0.1.3/grad_june/infection_networks/leisure_network.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/june_world_loader/agent_data_loader.py` & `grad_june-0.1.3/grad_june/june_world_loader/agent_data_loader.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/june_world_loader/graph_loader.py` & `grad_june-0.1.3/grad_june/june_world_loader/graph_loader.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/june_world_loader/leisure_loader.py` & `grad_june-0.1.3/grad_june/june_world_loader/leisure_loader.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/june_world_loader/network_loader.py` & `grad_june-0.1.3/grad_june/june_world_loader/network_loader.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/model.py` & `grad_june-0.1.3/grad_june/model.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/policies/close_venue_policies.py` & `grad_june-0.1.3/grad_june/policies/close_venue_policies.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/policies/interaction_policies.py` & `grad_june-0.1.3/grad_june/policies/interaction_policies.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/policies/policies.py` & `grad_june-0.1.3/grad_june/policies/policies.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/policies/quarantine_policies.py` & `grad_june-0.1.3/grad_june/policies/quarantine_policies.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/runner.py` & `grad_june-0.1.3/grad_june/runner.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/symptoms.py` & `grad_june-0.1.3/grad_june/symptoms.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/timer.py` & `grad_june-0.1.3/grad_june/timer.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/transmission.py` & `grad_june-0.1.3/grad_june/transmission.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june/utils.py` & `grad_june-0.1.3/grad_june/utils.py`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/grad_june.egg-info/PKG-INFO` & `grad_june-0.1.3/grad_june.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grad-june
-Version: 0.1.2
+Version: 0.1.3
 Summary: Differentiable implementation of the JUNE model.
 Home-page: https://github.com/arnauqb/GradABM-JUNE
 Author: Arnau Quera-Bofarull
 Author-email: arnauq@protonmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,29 +14,16 @@
 [![Build and test package](https://github.com/arnauqb/GradABM-JUNE/actions/workflows/ci.yml/badge.svg)](https://github.com/arnauqb/GradABM-JUNE/actions/workflows/ci.yml)
 
 # GradABM-JUNE
 Implementation of the JUNE model using the GradABM framework.
 
 # Setup 
 
-Install requirements
+The easiest way is to install the package from the PyPI package repository
 
-```bash
-pip install -r requirements.txt
-```
-
-and install PyTorch geometric, manually for now:
-
-```bash
-pip install torch-scatter torch-sparse torch-cluster torch-geometric -f https://data.pyg.org/whl/torch-1.13.0+cpu.html
-```
-
-Then install the GradABM-JUNE package
-
-```bash
-pip install -e .
 ```
+pip install 
 
 
 # Usage
 
 See the [docs](https://arnauqb.github.io/GradABM-JUNE/).
```

### Comparing `grad_june-0.1.2/grad_june.egg-info/SOURCES.txt` & `grad_june-0.1.3/grad_june.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grad_june-0.1.2/setup.py` & `grad_june-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 # -*- coding: utf-8 -*-
-from setuptools import setup, find_packages, Extension
-from setuptools.command.install import install
-import subprocess
-import os
+from setuptools import setup, find_packages
 from os.path import abspath, dirname, join
 
 this_dir = abspath(dirname(__file__))
+
 with open(join(this_dir, "LICENSE")) as f:
     license = f.read()
 
 with open(join(this_dir, "README.md"), encoding="utf-8") as file:
     long_description = file.read()
 
 with open(join(this_dir, "requirements.txt")) as f:
     requirements = f.read().split("\n")
 
 
 setup(
     name="grad_june",
-    version="0.1.2",
+    version="0.1.3",
     description="Differentiable implementation of the JUNE model.",
     url="https://github.com/arnauqb/GradABM-JUNE",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Arnau Quera-Bofarull",
     author_email="arnauq@protonmail.com",
     license="MIT License",
```

### Comparing `grad_june-0.1.2/test/conftest.py` & `grad_june-0.1.3/test/conftest.py`

 * *Files identical despite different names*

