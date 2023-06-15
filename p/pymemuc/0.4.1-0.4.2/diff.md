# Comparing `tmp/pymemuc-0.4.1.tar.gz` & `tmp/pymemuc-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.4.1.tar", max compression
+gzip compressed data, was "pymemuc-0.4.2.tar", max compression
```

## Comparing `pymemuc-0.4.1.tar` & `pymemuc-0.4.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-06-14 01:21:02.159552 pymemuc-0.4.1/LICENSE
--rw-r--r--   0        0        0     1586 2023-06-14 01:21:02.159552 pymemuc-0.4.1/README.md
--rw-r--r--   0        0        0      386 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/__init__.py
--rw-r--r--   0        0        0    23116 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_constants.py
--rw-r--r--   0        0        0     5146 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_control.py
--rw-r--r--   0        0        0     1214 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_decorators.py
--rw-r--r--   0        0        0    15149 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_manage.py
--rw-r--r--   0        0        0     4624 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/exceptions.py
--rw-r--r--   0        0        0     3014 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-06-14 01:21:02.159552 pymemuc-0.4.1/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1665 2023-06-14 01:21:21.368139 pymemuc-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-06-15 00:06:44.775289 pymemuc-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1586 2023-06-15 00:06:44.775289 pymemuc-0.4.2/README.md
+-rw-r--r--   0        0        0      386 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/__init__.py
+-rw-r--r--   0        0        0    23371 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_constants.py
+-rw-r--r--   0        0        0     5146 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_control.py
+-rw-r--r--   0        0        0     1214 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    15149 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_manage.py
+-rw-r--r--   0        0        0     4624 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     3014 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-06-15 00:06:44.779289 pymemuc-0.4.2/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-06-15 00:07:06.403401 pymemuc-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.4.2/PKG-INFO
```

### Comparing `pymemuc-0.4.1/LICENSE` & `pymemuc-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.1/README.md` & `pymemuc-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.1/pymemuc/_command.py` & `pymemuc-0.4.2/pymemuc/_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module contains functions for commanding running virtual machines with memuc.exe.
 Functions for interacting with running VMs are defined here."""
 from typing import TYPE_CHECKING, Literal, Tuple, Union
 
+from ._decorators import _retryable
 from .exceptions import PyMemucError, PyMemucIndexError, PyMemucTimeoutExpired
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
 
 
 def sort_out_all_vm(self: "PyMemuc") -> bool:
@@ -99,36 +100,44 @@
         raise PyMemucIndexError("Please specify either a vm index or a vm name")
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to uninstall APK: {output}")
     return True
 
 
+@_retryable
 def start_app_vm(
     self: "PyMemuc",
     package_name,
     vm_index: Union[int, None] = None,
     vm_name: Union[str, None] = None,
+    timeout: Union[int, None] = None,
 ) -> Literal[True]:
     """Start an app on a VM, must specify either a vm index or a vm name
 
     :param package_name: Package name of the APK
     :type package_name: str
     :param vm_index: VM index. Defaults to None.
     :type vm_index: int, optional
     :param vm_name: VM name. Defaults to None.
     :type vm_name: str, optional
+    :param timeout: Timeout in seconds. Defaults to None.
+    :type timeout: int, optional
     :raises PyMemucIndexError: an error if neither a vm index or a vm name is specified
     :return: True if the vm app start was successful
     :rtype: Literal[True]
     """
     if vm_index is not None:
-        status, output = self.memuc_run(["-i", str(vm_index), "startapp", package_name])
+        status, output = self.memuc_run(
+            ["-i", str(vm_index), "startapp", package_name], timeout=timeout
+        )
     elif vm_name is not None:
-        status, output = self.memuc_run(["-n", vm_name, "startapp", package_name])
+        status, output = self.memuc_run(
+            ["-n", vm_name, "startapp", package_name], timeout=timeout
+        )
     else:
         raise PyMemucIndexError("Please specify either a vm index or a vm name")
     success = status == 0 and output is not None and "SUCCESS" in output
     if not success:
         raise PyMemucError(f"Failed to start app: {output}")
     return True
```

### Comparing `pymemuc-0.4.1/pymemuc/_control.py` & `pymemuc-0.4.2/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.1/pymemuc/_decorators.py` & `pymemuc-0.4.2/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.1/pymemuc/_manage.py` & `pymemuc-0.4.2/pymemuc/_manage.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.1/pymemuc/_memuc.py` & `pymemuc-0.4.2/pymemuc/_memuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.1/pymemuc/exceptions.py` & `pymemuc-0.4.2/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.1/pymemuc/pymemuc.py` & `pymemuc-0.4.2/pymemuc/pymemuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.4.1/pyproject.toml` & `pymemuc-0.4.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.4.1"
+version = "v0.4.2"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.4.1/PKG-INFO` & `pymemuc-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```

