# Comparing `tmp/motion_python-0.1.63.tar.gz` & `tmp/motion_python-0.1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.63.tar", max compression
+gzip compressed data, was "motion_python-0.1.64.tar", max compression
```

## Comparing `motion_python-0.1.63.tar` & `motion_python-0.1.64.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-10 23:50:33.240118 motion_python-0.1.63/README.md
--rw-r--r--   0        0        0      276 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/cli.py
--rw-r--r--   0        0        0    23922 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/component.py
--rw-r--r--   0        0        0    17501 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/execute.py
--rw-r--r--   0        0        0     5815 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/fit_task.py
--rw-r--r--   0        0        0    12849 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/route.py
--rw-r--r--   0        0        0     8853 2023-06-10 23:50:33.240118 motion_python-0.1.63/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-10 23:50:53.664479 motion_python-0.1.63/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.63/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-14 22:35:09.463752 motion_python-0.1.64/README.md
+-rw-r--r--   0        0        0      276 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/cli.py
+-rw-r--r--   0        0        0    23922 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/component.py
+-rw-r--r--   0        0        0    17508 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/execute.py
+-rw-r--r--   0        0        0    12849 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/route.py
+-rw-r--r--   0        0        0     5815 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/server/fit_task.py
+-rw-r--r--   0        0        0     8853 2023-06-14 22:35:09.463752 motion_python-0.1.64/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-14 22:35:37.176000 motion_python-0.1.64/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.64/PKG-INFO
```

### Comparing `motion_python-0.1.63/README.md` & `motion_python-0.1.64/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.63/motion/cli.py` & `motion_python-0.1.64/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.63/motion/component.py` & `motion_python-0.1.64/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.63/motion/execute.py` & `motion_python-0.1.64/motion/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from uuid import uuid4
 
 import cloudpickle
 import psutil
 import redis
 from redis.lock import Lock
 
-from motion.fit_task import FitTask
 from motion.route import Route
+from motion.server.fit_task import FitTask
 from motion.utils import (
     CustomDict,
     FitEvent,
     FitEventGroup,
     RedisParams,
     hash_object,
     loadState,
```

### Comparing `motion_python-0.1.63/motion/fit_task.py` & `motion_python-0.1.64/motion/server/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.63/motion/instance.py` & `motion_python-0.1.64/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.63/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.64/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.63/motion/route.py` & `motion_python-0.1.64/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.63/motion/utils.py` & `motion_python-0.1.64/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.63/pyproject.toml` & `motion_python-0.1.64/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.63"
+version = "0.1.64"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.63/PKG-INFO` & `motion_python-0.1.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.63
+Version: 0.1.64
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

