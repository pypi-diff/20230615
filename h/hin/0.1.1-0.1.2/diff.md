# Comparing `tmp/hin-0.1.1.tar.gz` & `tmp/hin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hin-0.1.1.tar", max compression
+gzip compressed data, was "hin-0.1.2.tar", max compression
```

## Comparing `hin-0.1.1.tar` & `hin-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2023-06-14 10:28:55.233256 hin-0.1.1/LICENSE
--rw-r--r--   0        0        0     2960 2023-06-14 10:28:55.233401 hin-0.1.1/README.rst
--rw-r--r--   0        0        0      123 2023-06-14 10:28:55.233905 hin-0.1.1/hin/__init__.py
--rw-r--r--   0        0        0      146 2023-06-14 10:28:59.380763 hin-0.1.1/hin/__main__.py
--rw-r--r--   0        0        0     3398 2023-06-14 10:28:59.380882 hin-0.1.1/hin/_actions.py
--rw-r--r--   0        0        0     3535 2023-06-14 10:28:59.380994 hin-0.1.1/hin/_add.py
--rw-r--r--   0        0        0      763 2023-06-14 10:28:59.381085 hin-0.1.1/hin/_clone.py
--rw-r--r--   0        0        0     1321 2023-06-14 10:28:59.381194 hin-0.1.1/hin/_commit.py
--rw-r--r--   0        0        0     2077 2023-06-14 10:28:59.381312 hin-0.1.1/hin/_config.py
--rw-r--r--   0        0        0     7741 2023-06-14 10:28:59.381438 hin-0.1.1/hin/_decorators.py
--rw-r--r--   0        0        0     5675 2023-06-14 10:29:01.034086 hin-0.1.1/hin/_file.py
--rw-r--r--   0        0        0     1647 2023-06-14 10:28:59.381643 hin-0.1.1/hin/_gitignore.py
--rw-r--r--   0        0        0     1913 2023-06-14 10:28:59.381747 hin-0.1.1/hin/_link.py
--rw-r--r--   0        0        0      673 2023-06-14 10:28:59.381849 hin-0.1.1/hin/_list.py
--rw-r--r--   0        0        0     5357 2023-06-14 10:28:59.381968 hin-0.1.1/hin/_main.py
--rw-r--r--   0        0        0     1129 2023-06-14 10:28:59.382090 hin-0.1.1/hin/_push.py
--rw-r--r--   0        0        0     1164 2023-06-14 10:28:59.382178 hin-0.1.1/hin/_remove.py
--rw-r--r--   0        0        0     2496 2023-06-14 10:29:01.034230 hin-0.1.1/hin/_status.py
--rw-r--r--   0        0        0     1265 2023-06-14 10:28:59.382378 hin-0.1.1/hin/_undo.py
--rw-r--r--   0        0        0      204 2023-06-14 10:29:01.215534 hin-0.1.1/hin/_version.py
--rw-r--r--   0        0        0        0 2023-06-14 10:28:55.235217 hin-0.1.1/hin/py.typed
--rw-r--r--   0        0        0     2231 2023-06-14 10:29:01.216119 hin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-15 12:16:18.426286 hin-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2960 2023-06-15 12:16:18.426451 hin-0.1.2/README.rst
+-rw-r--r--   0        0        0      123 2023-06-15 12:16:18.426964 hin-0.1.2/hin/__init__.py
+-rw-r--r--   0        0        0      146 2023-06-15 12:16:20.893899 hin-0.1.2/hin/__main__.py
+-rw-r--r--   0        0        0     3398 2023-06-15 12:16:20.894017 hin-0.1.2/hin/_actions.py
+-rw-r--r--   0        0        0     3535 2023-06-15 12:16:20.894117 hin-0.1.2/hin/_add.py
+-rw-r--r--   0        0        0      763 2023-06-15 12:16:20.894216 hin-0.1.2/hin/_clone.py
+-rw-r--r--   0        0        0     1321 2023-06-15 12:16:20.894321 hin-0.1.2/hin/_commit.py
+-rw-r--r--   0        0        0     2077 2023-06-15 12:16:20.894431 hin-0.1.2/hin/_config.py
+-rw-r--r--   0        0        0     7741 2023-06-15 12:16:20.894546 hin-0.1.2/hin/_decorators.py
+-rw-r--r--   0        0        0     5683 2023-06-15 12:16:23.085121 hin-0.1.2/hin/_file.py
+-rw-r--r--   0        0        0     1647 2023-06-15 12:16:20.894763 hin-0.1.2/hin/_gitignore.py
+-rw-r--r--   0        0        0     1913 2023-06-15 12:16:20.894860 hin-0.1.2/hin/_link.py
+-rw-r--r--   0        0        0      673 2023-06-15 12:16:20.894986 hin-0.1.2/hin/_list.py
+-rw-r--r--   0        0        0     5357 2023-06-15 12:16:20.895098 hin-0.1.2/hin/_main.py
+-rw-r--r--   0        0        0     1129 2023-06-15 12:16:20.895184 hin-0.1.2/hin/_push.py
+-rw-r--r--   0        0        0     1160 2023-06-15 12:17:07.056506 hin-0.1.2/hin/_remove.py
+-rw-r--r--   0        0        0     2496 2023-06-15 12:16:22.528694 hin-0.1.2/hin/_status.py
+-rw-r--r--   0        0        0     1265 2023-06-15 12:16:20.895461 hin-0.1.2/hin/_undo.py
+-rw-r--r--   0        0        0      204 2023-06-15 12:21:52.625933 hin-0.1.2/hin/_version.py
+-rw-r--r--   0        0        0        0 2023-06-15 12:16:18.428640 hin-0.1.2/hin/py.typed
+-rw-r--r--   0        0        0     2231 2023-06-15 12:21:52.626463 hin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 hin-0.1.2/PKG-INFO
```

### Comparing `hin-0.1.1/LICENSE` & `hin-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/README.rst` & `hin-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_actions.py` & `hin-0.1.2/hin/_actions.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_add.py` & `hin-0.1.2/hin/_add.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_clone.py` & `hin-0.1.2/hin/_clone.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_commit.py` & `hin-0.1.2/hin/_commit.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_config.py` & `hin-0.1.2/hin/_config.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_decorators.py` & `hin-0.1.2/hin/_decorators.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_file.py` & `hin-0.1.2/hin/_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         """Full path to the file."""
         return self.root / self.relpath
 
 
 class _Symlink(_File):
     def __init__(self, value: str | _Path) -> None:
         super().__init__(value)
-        self._str = str(_Path(_os.path.expandvars(value)).absolute())
+        self._str = str(_Path.home() / _Path(_os.path.expandvars(value)))
 
     def __repr__(self) -> str:
         return f"${self.env}/{self.relpath}"
 
     @property
     def env(self) -> str:
         """Environment variable to save link under."""
@@ -78,15 +78,15 @@
     :param value: Actual file or directory for this matrix.
     """
 
     def __init__(self, key: str | _Path, value: str | _Path) -> None:
         self._key = (
             _UserDataSymlink(key)
             if _e["USER_DATA_DIR"]
-            in str(_Path(_os.path.expandvars(key)).absolute())
+            in str(_Path.home() / _Path(_os.path.expandvars(key)))
             else _Symlink(key)
         )
         self._value: _File = _Dotfile(value)
 
     @property
     def key(self) -> _Symlink:
         """The symlink pointing to this matrix."""
```

### Comparing `hin-0.1.1/hin/_gitignore.py` & `hin-0.1.2/hin/_gitignore.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_link.py` & `hin-0.1.2/hin/_link.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_list.py` & `hin-0.1.2/hin/_list.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_main.py` & `hin-0.1.2/hin/_main.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_push.py` & `hin-0.1.2/hin/_push.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_remove.py` & `hin-0.1.2/hin/_remove.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 @_decorators.console
 @_decorators.config
 @_decorators.repository
 def remove(config: _Config, out: _Console, file: str) -> str:
     """Remove FILE from version control.
 
-    All links that point to the file, and any any links to those links,
+    All links that point to the file, and any links to those links,
     will be removed.
 
     If the dotfile is not a link to another dotfile then the checked in
     file or directory will be moved back to its original location in its
     place.
 
     Changes will be committed.
```

### Comparing `hin-0.1.1/hin/_status.py` & `hin-0.1.2/hin/_status.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/hin/_undo.py` & `hin-0.1.2/hin/_undo.py`

 * *Files identical despite different names*

### Comparing `hin-0.1.1/pyproject.toml` & `hin-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -64,30 +64,30 @@
 license = "MIT"
 maintainers = [
   "jshwi <stephen@jshwisolutions.com>"
 ]
 name = "hin"
 readme = "README.rst"
 repository = "https://github.com/jshwi/hin"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 appdirs = "^1.4.4"
 click = "^8.1.3"
 click-help-colors = "^0.9.1"
 configobj = "^5.0.8"
 gitpython = "^3.1.31"
 python = "^3.8"
 rich = "^13.3.5"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
 deptry = "^0.11.0"
 freezegun = "^1.2.2"
-pre-commit = "^3.1.1"
+pre-commit = "^3.3.3"
 pyaud = "^6.2.1"
 pylint = "2.17.4"
 pytest = "^7.2.0"
 pytest-randomly = "^3.12.0"
 pytest-sugar = "^0.9.6"
 pytest-xdist = "^3.3.1"
 restview = "^3.0.0"
```

### Comparing `hin-0.1.1/PKG-INFO` & `hin-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hin
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dotfile manager
 Home-page: https://pypi.org/project/hin/
 License: MIT
 Keywords: config,dot,dotfile,file,hin
 Author: jshwi
 Author-email: stephen@jshwisolutions.com
 Maintainer: jshwi
```

