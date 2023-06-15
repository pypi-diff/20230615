# Comparing `tmp/radtrun-0.1.1.tar.gz` & `tmp/radtrun-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radtrun-0.1.1.tar", last modified: Thu Jun 15 14:50:23 2023, max compression
+gzip compressed data, was "radtrun-0.1.3.tar", last modified: Thu Jun 15 15:27:52 2023, max compression
```

## Comparing `radtrun-0.1.1.tar` & `radtrun-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      144 2023-06-15 14:44:17.450860 radtrun-0.1.1/README.md
--rw-r--r--   0        0        0      433 2023-06-15 14:50:21.404326 radtrun-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      149 2023-06-15 14:50:23.004332 radtrun-0.1.1/radtrun/__init__.py
--rw-r--r--   0        0        0       63 2023-06-14 18:44:41.625589 radtrun-0.1.1/radtrun/__main__.py
--rw-r--r--   0        0        0        0 2023-06-14 18:10:26.872470 radtrun-0.1.1/radtrun/listeners/__init__.py
--rw-r--r--   0        0        0     2165 2023-06-15 10:33:28.277851 radtrun-0.1.1/radtrun/listeners/dcgmi_listener.py
--rw-r--r--   0        0        0     1155 2023-06-14 18:48:25.738606 radtrun-0.1.1/radtrun/listeners/ps_listener.py
--rw-r--r--   0        0        0     1559 2023-06-14 18:48:28.674620 radtrun-0.1.1/radtrun/listeners/smi_listener.py
--rw-r--r--   0        0        0     2705 2023-06-14 18:48:32.002635 radtrun-0.1.1/radtrun/listeners/top_listener.py
--rw-r--r--   0        0        0     3156 2023-06-14 18:47:21.690315 radtrun-0.1.1/radtrun/mldgpu.py
--rw-r--r--   0        0        0     4871 2023-06-15 14:42:51.694439 radtrun-0.1.1/radtrun/radtrun.py
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 radtrun-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      144 2023-06-15 15:25:53.269964 radtrun-0.1.3/README.md
+-rw-r--r--   0        0        0      433 2023-06-15 15:25:53.269964 radtrun-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-06-15 15:25:53.269964 radtrun-0.1.3/radtrun/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-15 15:25:53.269964 radtrun-0.1.3/radtrun/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-15 15:25:53.269964 radtrun-0.1.3/radtrun/listeners/__init__.py
+-rw-r--r--   0        0        0     2165 2023-06-15 15:25:53.269964 radtrun-0.1.3/radtrun/listeners/dcgmi_listener.py
+-rw-r--r--   0        0        0     1155 2023-06-15 15:25:53.269964 radtrun-0.1.3/radtrun/listeners/ps_listener.py
+-rw-r--r--   0        0        0     1559 2023-06-15 15:25:53.269964 radtrun-0.1.3/radtrun/listeners/smi_listener.py
+-rw-r--r--   0        0        0     2705 2023-06-15 15:25:53.269964 radtrun-0.1.3/radtrun/listeners/top_listener.py
+-rw-r--r--   0        0        0     3156 2023-06-15 15:25:53.269964 radtrun-0.1.3/radtrun/mldgpu.py
+-rw-r--r--   0        0        0     4871 2023-06-15 15:25:53.269964 radtrun-0.1.3/radtrun/radtrun.py
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 radtrun-0.1.3/PKG-INFO
```

### Comparing `radtrun-0.1.1/radtrun/listeners/dcgmi_listener.py` & `radtrun-0.1.3/radtrun/listeners/dcgmi_listener.py`

 * *Files identical despite different names*

### Comparing `radtrun-0.1.1/radtrun/listeners/ps_listener.py` & `radtrun-0.1.3/radtrun/listeners/ps_listener.py`

 * *Files identical despite different names*

### Comparing `radtrun-0.1.1/radtrun/listeners/smi_listener.py` & `radtrun-0.1.3/radtrun/listeners/smi_listener.py`

 * *Files identical despite different names*

### Comparing `radtrun-0.1.1/radtrun/listeners/top_listener.py` & `radtrun-0.1.3/radtrun/listeners/top_listener.py`

 * *Files identical despite different names*

### Comparing `radtrun-0.1.1/radtrun/mldgpu.py` & `radtrun-0.1.3/radtrun/mldgpu.py`

 * *Files identical despite different names*

### Comparing `radtrun-0.1.1/radtrun/radtrun.py` & `radtrun-0.1.3/radtrun/radtrun.py`

 * *Files identical despite different names*

### Comparing `radtrun-0.1.1/PKG-INFO` & `radtrun-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radtrun
-Version: 0.1.1
+Version: 0.1.3
 Summary: Runner for Resource-Aware Data systems Tracker (radT) for automatically tracking and training machine learning software
 Author-email: Ties Robroek <titr@itu.dk>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/Resource-Aware-Data-systems-RAD/radt
 
 # radtrun
```

