# Comparing `tmp/pepver-1.1.0.tar.gz` & `tmp/pepver-1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepver-1.1.0.tar", max compression
+gzip compressed data, was "pepver-1.1.post1.tar", max compression
```

## Comparing `pepver-1.1.0.tar` & `pepver-1.1.post1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2023-06-02 11:53:00.615630 pepver-1.1.0/LICENSE
--rw-r--r--   0        0        0    12824 2023-06-02 11:53:00.615630 pepver-1.1.0/pepver/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 11:53:00.615630 pepver-1.1.0/pepver/py.typed
--rw-r--r--   0        0        0      955 2023-06-02 11:53:00.615630 pepver-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1983 2023-06-02 11:53:00.615630 pepver-1.1.0/readme.md
--rw-r--r--   0        0        0     2776 1970-01-01 00:00:00.000000 pepver-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-15 12:40:02.789450 pepver-1.1.post1/LICENSE
+-rw-r--r--   0        0        0    12849 2023-06-15 12:40:02.789450 pepver-1.1.post1/pepver/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 12:40:02.789450 pepver-1.1.post1/pepver/py.typed
+-rw-r--r--   0        0        0      959 2023-06-15 12:40:02.789450 pepver-1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     1983 2023-06-15 12:40:02.789450 pepver-1.1.post1/readme.md
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 pepver-1.1.post1/PKG-INFO
```

### Comparing `pepver-1.1.0/LICENSE` & `pepver-1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `pepver-1.1.0/pepver/__init__.py` & `pepver-1.1.post1/pepver/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,28 +174,27 @@
             release = *self.release[:idx], self.release[idx] + change
         return type(self)(epoch=self.epoch, release=release)
 
     def truncate_release(self, keep: int = 0) -> "Version":
         """
         Remove trailing zeroes from the release part of the version.
 
-        str(Version.parse("1.0.0.0").truncate()) == "1"
-        str(Version.parse("1.0.0.0").truncate(3)) == "1.0.0"
-        str(Version.parse("1.0.0.1").truncate(3)) == "1.0.0.1"
+        str(Version.parse("1.0.0.0").truncate_release()) == "1"
+        str(Version.parse("1.0.0.0").truncate_release(3)) == "1.0.0"
+        str(Version.parse("1.0.0.1").truncate_release(3)) == "1.0.0.1"
         """
         if keep < 0:
             raise ValueError("kept number of digits must be non-negative")
         if keep == 0:
             keep = 1
 
         version = deepcopy(self)
         version.release = _truncate(version.release, keep)
         return version
 
-
     @property
     def major(self) -> int:
         """Major (first) segment of the release part."""
         return self.release[0]
 
     @major.setter
     def major(self, value: int) -> None:
@@ -374,11 +373,11 @@
     return left < right
 
 
 def _truncate(value: Tuple[int, ...], keep: int) -> Tuple[int, ...]:
     if len(value) <= keep:
         return value
     last_non_zero = keep
-    for i, val in enumerate(value[keep:], start=keep+1):
+    for i, val in enumerate(value[keep:], start=keep + 1):
         if val:
             last_non_zero = i
     return tuple(value[:last_non_zero])
```

### Comparing `pepver-1.1.0/pyproject.toml` & `pepver-1.1.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pepver"
-version = "1.1.0"
+version = "1.1.post1"
 description = "PEP-440 version parsing, interpretation and manipulation"
 authors = ["technomunk <thegriffones@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/technomunk/pepver"
 repository = "https://github.com/technomunk/pepver"
 keywords = ["version", "package"]
```

### Comparing `pepver-1.1.0/readme.md` & `pepver-1.1.post1/readme.md`

 * *Files identical despite different names*

### Comparing `pepver-1.1.0/PKG-INFO` & `pepver-1.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepver
-Version: 1.1.0
+Version: 1.1.post1
 Summary: PEP-440 version parsing, interpretation and manipulation
 Home-page: https://github.com/technomunk/pepver
 License: MIT
 Keywords: version,package
 Author: technomunk
 Author-email: thegriffones@gmail.com
 Requires-Python: >=3.8,<4.0
```

