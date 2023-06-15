# Comparing `tmp/pyechorobotics-0.0.8.tar.gz` & `tmp/pyechorobotics-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyechorobotics-0.0.8.tar", last modified: Sat Jun  3 13:05:32 2023, max compression
+gzip compressed data, was "pyechorobotics-0.0.9.tar", last modified: Sat Jun  3 20:03:48 2023, max compression
```

## Comparing `pyechorobotics-0.0.8.tar` & `pyechorobotics-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:05:32.702789 pyechorobotics-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-03 13:05:32.702789 pyechorobotics-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-03 13:05:32.702789 pyechorobotics-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:05:32.698789 pyechorobotics-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:05:32.698789 pyechorobotics-0.0.8/src/echoroboticsapi/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/src/echoroboticsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/src/echoroboticsapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/src/echoroboticsapi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-03 13:05:17.000000 pyechorobotics-0.0.8/src/echoroboticsapi/smart_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 13:05:32.698789 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-03 13:05:32.000000 pyechorobotics-0.0.8/src/pyechorobotics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:03:48.665539 pyechorobotics-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-03 20:03:37.000000 pyechorobotics-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-03 20:03:48.665539 pyechorobotics-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-03 20:03:37.000000 pyechorobotics-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-03 20:03:37.000000 pyechorobotics-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-03 20:03:48.665539 pyechorobotics-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-03 20:03:37.000000 pyechorobotics-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:03:48.661539 pyechorobotics-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:03:48.665539 pyechorobotics-0.0.9/src/echoroboticsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-03 20:03:37.000000 pyechorobotics-0.0.9/src/echoroboticsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-03 20:03:37.000000 pyechorobotics-0.0.9/src/echoroboticsapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-03 20:03:37.000000 pyechorobotics-0.0.9/src/echoroboticsapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-03 20:03:37.000000 pyechorobotics-0.0.9/src/echoroboticsapi/smart_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:03:48.665539 pyechorobotics-0.0.9/src/pyechorobotics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-03 20:03:48.000000 pyechorobotics-0.0.9/src/pyechorobotics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-03 20:03:48.000000 pyechorobotics-0.0.9/src/pyechorobotics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:03:48.000000 pyechorobotics-0.0.9/src/pyechorobotics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 20:03:48.000000 pyechorobotics-0.0.9/src/pyechorobotics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-03 20:03:48.000000 pyechorobotics-0.0.9/src/pyechorobotics.egg-info/top_level.txt
```

### Comparing `pyechorobotics-0.0.8/LICENSE.md` & `pyechorobotics-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.8/PKG-INFO` & `pyechorobotics-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyechorobotics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Access API for echorobotics robot lawn mowers
 Author-email: functionpointer <suspendfunction@gmail.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.10
```

### Comparing `pyechorobotics-0.0.8/README.md` & `pyechorobotics-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.8/pyproject.toml` & `pyechorobotics-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyechorobotics"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
     "aiohttp",
     "yarl",
     "pydantic",
     "python-dateutil"
 ]
 readme = "README.md"
```

### Comparing `pyechorobotics-0.0.8/src/echoroboticsapi/api.py` & `pyechorobotics-0.0.9/src/echoroboticsapi/api.py`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.8/src/echoroboticsapi/models.py` & `pyechorobotics-0.0.9/src/echoroboticsapi/models.py`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.8/src/echoroboticsapi/smart_mode.py` & `pyechorobotics-0.0.9/src/echoroboticsapi/smart_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     async def notify_mode_set(self, newmode: Mode) -> None:
         self._last_known_mode = newmode
         self._mode_known_since = time.time()
 
     async def notify_laststatuses_received(self, receivedstatus: Status) -> None:
         ismowing: bool = receivedstatus in ["LeaveStation", "Work"]
 
-        happend_a_while_ago: bool = time.time() < self._mode_known_since + 60
+        happend_a_while_ago: bool = time.time() > self._mode_known_since + 60
         if ismowing and self._last_known_mode != "work" and happend_a_while_ago:
             self.logger.info(
                 "laststatuses: status is %s, inferring modechange from %s to %s",
                 receivedstatus,
                 self._last_known_mode,
                 "work",
             )
```

### Comparing `pyechorobotics-0.0.8/src/pyechorobotics.egg-info/PKG-INFO` & `pyechorobotics-0.0.9/src/pyechorobotics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyechorobotics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Access API for echorobotics robot lawn mowers
 Author-email: functionpointer <suspendfunction@gmail.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.10
```

