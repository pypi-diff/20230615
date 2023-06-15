# Comparing `tmp/morel-1.2.1.tar.gz` & `tmp/morel-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morel-1.2.1.tar", last modified: Thu Jun 15 20:49:04 2023, max compression
+gzip compressed data, was "morel-1.2.2.tar", last modified: Thu Jun 15 21:07:54 2023, max compression
```

## Comparing `morel-1.2.1.tar` & `morel-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 20:49:04.140593 morel-1.2.1/
--rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.2.1/LICENSE
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-15 20:49:04.139593 morel-1.2.1/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.2.1/README.md
--rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-15 20:48:27.000000 morel-1.2.1/pyproject.toml
--rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-15 20:49:04.140593 morel-1.2.1/setup.cfg
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 20:49:04.137593 morel-1.2.1/src/
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 20:49:04.138593 morel-1.2.1/src/morel/
--rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.2.1/src/morel/__init__.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.2.1/src/morel/app.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.2.1/src/morel/exploit_template.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.2.1/src/morel/exploits.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.2.1/src/morel/logger.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-05-24 09:29:29.000000 morel-1.2.1/src/morel/singleton.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)     2750 2023-06-15 20:36:09.000000 morel-1.2.1/src/morel/target.py
--rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.2.1/src/morel/target_template.py
-drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 20:49:04.139593 morel-1.2.1/src/morel.egg-info/
--rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/PKG-INFO
--rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/SOURCES.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/dependency_links.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/entry_points.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/requires.txt
--rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-15 20:49:04.000000 morel-1.2.1/src/morel.egg-info/top_level.txt
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 21:07:54.767378 morel-1.2.2/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)    35148 2023-06-11 10:50:26.000000 morel-1.2.2/LICENSE
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-15 21:07:54.766378 morel-1.2.2/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      101 2023-06-11 11:30:40.000000 morel-1.2.2/README.md
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      794 2023-06-15 21:07:01.000000 morel-1.2.2/pyproject.toml
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       38 2023-06-15 21:07:54.767378 morel-1.2.2/setup.cfg
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 21:07:54.765378 morel-1.2.2/src/
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 21:07:54.766378 morel-1.2.2/src/morel/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       76 2023-06-13 07:59:42.000000 morel-1.2.2/src/morel/__init__.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     3725 2023-06-13 10:51:58.000000 morel-1.2.2/src/morel/app.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      693 2023-06-13 08:50:20.000000 morel-1.2.2/src/morel/exploit_template.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1057 2023-06-15 13:11:55.000000 morel-1.2.2/src/morel/exploits.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      406 2023-06-11 14:53:08.000000 morel-1.2.2/src/morel/logger.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     1525 2023-05-24 09:29:29.000000 morel-1.2.2/src/morel/singleton.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)     2822 2023-06-15 20:58:17.000000 morel-1.2.2/src/morel/target.py
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      304 2023-06-13 08:11:32.000000 morel-1.2.2/src/morel/target_template.py
+drwxr-xr-x   0 basilef   (1000) basilef   (1000)        0 2023-06-15 21:07:54.766378 morel-1.2.2/src/morel.egg-info/
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      695 2023-06-15 21:07:54.000000 morel-1.2.2/src/morel.egg-info/PKG-INFO
+-rw-r--r--   0 basilef   (1000) basilef   (1000)      415 2023-06-15 21:07:54.000000 morel-1.2.2/src/morel.egg-info/SOURCES.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        1 2023-06-15 21:07:54.000000 morel-1.2.2/src/morel.egg-info/dependency_links.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       36 2023-06-15 21:07:54.000000 morel-1.2.2/src/morel.egg-info/entry_points.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)       13 2023-06-15 21:07:54.000000 morel-1.2.2/src/morel.egg-info/requires.txt
+-rw-r--r--   0 basilef   (1000) basilef   (1000)        6 2023-06-15 21:07:54.000000 morel-1.2.2/src/morel.egg-info/top_level.txt
```

### Comparing `morel-1.2.1/LICENSE` & `morel-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `morel-1.2.1/PKG-INFO` & `morel-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.2.1
+Version: 1.2.2
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `morel-1.2.1/pyproject.toml` & `morel-1.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "morel"
-version = "1.2.1"
+version = "1.2.2"
 authors = [
   { name="Francesco Basile", email="basile1fr@gmail.com" },
 ]
 description = "morel helps you write and test your A/D exploits, built with Milkman compatibility in mind"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `morel-1.2.1/src/morel/app.py` & `morel-1.2.2/src/morel/app.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.1/src/morel/exploit_template.py` & `morel-1.2.2/src/morel/exploit_template.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.1/src/morel/exploits.py` & `morel-1.2.2/src/morel/exploits.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.1/src/morel/singleton.py` & `morel-1.2.2/src/morel/singleton.py`

 * *Files identical despite different names*

### Comparing `morel-1.2.1/src/morel/target.py` & `morel-1.2.2/src/morel/target.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 
 class Targets(_restrictedDict, metaclass=SingletonMeta):
     def __init__(self):
         self._lock = Lock()
         self.p = Path(".")
         self.update()
 
+    def __getitem__(self, key):
+        super().__getitem__(self, key)
+
     def setBaseDir(self, dir):
         self.p = Path(dir)
 
     def add_targets(self, targets):
         with self._lock:
             self.append(targets)
```

### Comparing `morel-1.2.1/src/morel.egg-info/PKG-INFO` & `morel-1.2.2/src/morel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morel
-Version: 1.2.1
+Version: 1.2.2
 Summary: morel helps you write and test your A/D exploits, built with Milkman compatibility in mind
 Author-email: Francesco Basile <basile1fr@gmail.com>
 Project-URL: Homepage, https://github.com/parmigggiana/morel
 Project-URL: Bug Tracker, https://github.com/parmigggiana/morel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

