# Comparing `tmp/yacman-0.9.0.tar.gz` & `tmp/yacman-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yacman-0.9.0.tar", last modified: Thu Mar  2 15:55:54 2023, max compression
+gzip compressed data, was "yacman-0.9.1.tar", last modified: Thu Jun 15 18:59:43 2023, max compression
```

## Comparing `yacman-0.9.0.tar` & `yacman-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:55:54.974053 yacman-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-02 15:55:43.000000 yacman-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-02 15:55:43.000000 yacman-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-02 15:55:54.974053 yacman-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-02 15:55:43.000000 yacman-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:55:54.974053 yacman-0.9.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-02 15:55:43.000000 yacman-0.9.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 15:55:43.000000 yacman-0.9.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-02 15:55:43.000000 yacman-0.9.0/requirements/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-02 15:55:43.000000 yacman-0.9.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 15:55:54.974053 yacman-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-03-02 15:55:43.000000 yacman-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:55:54.974053 yacman-0.9.0/yacman/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-02 15:55:43.000000 yacman-0.9.0/yacman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-02 15:55:43.000000 yacman-0.9.0/yacman/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-03-02 15:55:43.000000 yacman-0.9.0/yacman/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-03-02 15:55:43.000000 yacman-0.9.0/yacman/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-02 15:55:43.000000 yacman-0.9.0/yacman/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20153 2023-03-02 15:55:43.000000 yacman-0.9.0/yacman/yacman.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21616 2023-03-02 15:55:43.000000 yacman-0.9.0/yacman/yacman1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 15:55:54.974053 yacman-0.9.0/yacman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-02 15:55:54.000000 yacman-0.9.0/yacman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-02 15:55:54.000000 yacman-0.9.0/yacman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 15:55:54.000000 yacman-0.9.0/yacman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-02 15:55:54.000000 yacman-0.9.0/yacman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-02 15:55:54.000000 yacman-0.9.0/yacman.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:43.605808 yacman-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-15 18:59:34.000000 yacman-0.9.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 18:59:34.000000 yacman-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-15 18:59:43.605808 yacman-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-15 18:59:34.000000 yacman-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:43.601808 yacman-0.9.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 18:59:34.000000 yacman-0.9.1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:34.000000 yacman-0.9.1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-15 18:59:34.000000 yacman-0.9.1/requirements/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 18:59:34.000000 yacman-0.9.1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 18:59:43.605808 yacman-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-15 18:59:34.000000 yacman-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:43.605808 yacman-0.9.1/yacman/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 18:59:34.000000 yacman-0.9.1/yacman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 18:59:34.000000 yacman-0.9.1/yacman/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-06-15 18:59:34.000000 yacman-0.9.1/yacman/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-15 18:59:34.000000 yacman-0.9.1/yacman/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 18:59:34.000000 yacman-0.9.1/yacman/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20153 2023-06-15 18:59:34.000000 yacman-0.9.1/yacman/yacman.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22736 2023-06-15 18:59:34.000000 yacman-0.9.1/yacman/yacman1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 18:59:43.605808 yacman-0.9.1/yacman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-15 18:59:43.000000 yacman-0.9.1/yacman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-15 18:59:43.000000 yacman-0.9.1/yacman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 18:59:43.000000 yacman-0.9.1/yacman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 18:59:43.000000 yacman-0.9.1/yacman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 18:59:43.000000 yacman-0.9.1/yacman.egg-info/top_level.txt
```

### Comparing `yacman-0.9.0/LICENSE.txt` & `yacman-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yacman-0.9.0/PKG-INFO` & `yacman-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yacman
-Version: 0.9.0
+Version: 0.9.1
 Summary: A standardized configuration object for reference genome assemblies
 Home-page: https://github.com/databio/yacman
 Author: Nathan Sheffield, Michal Stolarczyk
 Author-email: nathan@code.databio.org
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `yacman-0.9.0/README.md` & `yacman-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `yacman-0.9.0/setup.py` & `yacman-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `yacman-0.9.0/yacman/alias.py` & `yacman-0.9.1/yacman/alias.py`

 * *Files identical despite different names*

### Comparing `yacman-0.9.0/yacman/const.py` & `yacman-0.9.1/yacman/const.py`

 * *Files identical despite different names*

### Comparing `yacman-0.9.0/yacman/yacman.py` & `yacman-0.9.1/yacman/yacman.py`

 * *Files identical despite different names*

### Comparing `yacman-0.9.0/yacman/yacman1.py` & `yacman-0.9.1/yacman/yacman1.py`

 * *Files 2% similar despite different names*

```diff
@@ -417,16 +417,46 @@
         return len(self.data)
 
     def __delitem__(self, key):
         value = self[key]
         del self.data[key]
         self.pop(value, None)
 
+    def priority_get(
+        self,
+        arg_name: str,
+        env_var: str = None,
+        default: str = None,
+        override: str = None,
+        strict: bool = False,
+    ):
+        """
+        Helper function to select a value from a config, or, if missing, then go to an env var.
 
-from ubiquerg import expandpath
+        :param str arg_name: Argument to retrieve
+        :param bool strict: Should missing args raise an error? False=warning
+        :param env_var: Env var to retrieve from should it be missing from the cfg
+        """
+        if override:
+            return override
+        if self.data.get(arg_name) is not None:
+            return self.data[arg_name]
+        if env_var is not None:
+            arg = os.getenv(env_var, None)
+            if arg is not None:
+                _LOGGER.debug(f"Value '{arg}' sourced from '{env_var}' env var")
+                return expandpath(arg)
+        if default is not None:
+            return default
+        if strict:
+            message = (
+                "Value for required argument '{arg_name}' could not be determined."
+            )
+            _LOGGER.warning(message)
+            raise Exception(message)
 
 
 # A big issue here is: if you route the __getitem__ through this,
 # then it returns a copy of the data, rather than the data itself.
 # That's the point, so we don't adjust it. But then you can't use multi-level
 # item setting, like ycm["x"]["y"] = value, because ycm['x'] returns a different
 # dict, and so you're updating that copy of it.
```

### Comparing `yacman-0.9.0/yacman.egg-info/PKG-INFO` & `yacman-0.9.1/yacman.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yacman
-Version: 0.9.0
+Version: 0.9.1
 Summary: A standardized configuration object for reference genome assemblies
 Home-page: https://github.com/databio/yacman
 Author: Nathan Sheffield, Michal Stolarczyk
 Author-email: nathan@code.databio.org
 License: BSD2
 Keywords: bioinformatics,sequencing,ngs
 Classifier: Development Status :: 4 - Beta
```

