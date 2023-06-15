# Comparing `tmp/jobmanager-0.4.0.tar.gz` & `tmp/jobmanager-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobmanager-0.4.0.tar", max compression
+gzip compressed data, was "jobmanager-0.4.1.tar", max compression
```

## Comparing `jobmanager-0.4.0.tar` & `jobmanager-0.4.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2016-09-27 20:39:36.170516 jobmanager-0.4.0/LICENSE
--rw-r--r--   0        0        0     1359 2023-06-15 21:46:17.941745 jobmanager-0.4.0/README.md
--rw-r--r--   0        0        0      851 2016-09-29 18:55:19.118543 jobmanager-0.4.0/jobmanager/__init__.py
--rw-r--r--   0        0        0     6633 2023-06-15 21:32:12.814108 jobmanager-0.4.0/jobmanager/clients.py
--rw-r--r--   0        0        0    99780 2023-06-15 21:34:26.912639 jobmanager-0.4.0/jobmanager/jobmanager.py
--rw-r--r--   0        0        0    10228 2023-06-15 21:36:19.606765 jobmanager-0.4.0/jobmanager/ode_wrapper.py
--rw-r--r--   0        0        0     2049 2023-06-15 21:34:26.916639 jobmanager-0.4.0/jobmanager/servers.py
--rw-r--r--   0        0        0     3357 2021-11-01 21:25:44.466676 jobmanager-0.4.0/jobmanager/signalDelay.py
--rw-r--r--   0        0        0      928 2023-06-15 21:44:57.464301 jobmanager-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 jobmanager-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2016-09-27 20:39:36.170516 jobmanager-0.4.1/LICENSE
+-rw-r--r--   0        0        0      702 2023-06-15 21:52:01.363989 jobmanager-0.4.1/README.md
+-rw-r--r--   0        0        0      851 2016-09-29 18:55:19.118543 jobmanager-0.4.1/jobmanager/__init__.py
+-rw-r--r--   0        0        0     6633 2023-06-15 21:32:12.814108 jobmanager-0.4.1/jobmanager/clients.py
+-rw-r--r--   0        0        0    99780 2023-06-15 21:34:26.912639 jobmanager-0.4.1/jobmanager/jobmanager.py
+-rw-r--r--   0        0        0    10228 2023-06-15 21:36:19.606765 jobmanager-0.4.1/jobmanager/ode_wrapper.py
+-rw-r--r--   0        0        0     2049 2023-06-15 21:34:26.916639 jobmanager-0.4.1/jobmanager/servers.py
+-rw-r--r--   0        0        0     3357 2021-11-01 21:25:44.466676 jobmanager-0.4.1/jobmanager/signalDelay.py
+-rw-r--r--   0        0        0      928 2023-06-15 21:52:49.604874 jobmanager-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1798 1970-01-01 00:00:00.000000 jobmanager-0.4.1/PKG-INFO
```

### Comparing `jobmanager-0.4.0/LICENSE` & `jobmanager-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.0/jobmanager/__init__.py` & `jobmanager-0.4.1/jobmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.0/jobmanager/clients.py` & `jobmanager-0.4.1/jobmanager/clients.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.0/jobmanager/jobmanager.py` & `jobmanager-0.4.1/jobmanager/jobmanager.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.0/jobmanager/ode_wrapper.py` & `jobmanager-0.4.1/jobmanager/ode_wrapper.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.0/jobmanager/servers.py` & `jobmanager-0.4.1/jobmanager/servers.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.0/jobmanager/signalDelay.py` & `jobmanager-0.4.1/jobmanager/signalDelay.py`

 * *Files identical despite different names*

### Comparing `jobmanager-0.4.0/pyproject.toml` & `jobmanager-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobmanager"
-version = "0.4.0"
+version = "0.4.1"
 description = "a facility for distributed computing"
 authors = ["Richard Hartmann", "Paul Müller"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cimatosa/jobmanager"
 repository = "https://github.com/cimatosa/jobmanager"
 keywords =[
```

