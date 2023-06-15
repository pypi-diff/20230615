# Comparing `tmp/heatshrinkpy-0.11.0.tar.gz` & `tmp/heatshrinkpy-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatshrinkpy-0.11.0.tar", max compression
+gzip compressed data, was "heatshrinkpy-0.11.1.tar", max compression
```

## Comparing `heatshrinkpy-0.11.0.tar` & `heatshrinkpy-0.11.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      898 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/LICENSE
--rw-r--r--   0        0        0      702 2023-06-07 16:19:00.444244 heatshrinkpy-0.11.0/README.rst
--rw-r--r--   0        0        0     3088 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/__init__.py
--rw-r--r--   0        0        0       36 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/__main__.py
--rw-r--r--   0        0        0     2693 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/core/__init__.py
--rw-r--r--   0        0        0      813 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/core/common.py
--rw-r--r--   0        0        0      146 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/core/consts.py
--rw-r--r--   0        0        0     7404 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/core/decoder.py
--rw-r--r--   0        0        0     9892 2023-06-07 16:19:19.162264 heatshrinkpy-0.11.0/heatshrinkpy/core/encoder.py
--rw-r--r--   0        0        0    12855 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/streams.py
--rw-r--r--   0        0        0      258 2023-06-07 16:19:00.439243 heatshrinkpy-0.11.0/heatshrinkpy/version.py
--rw-r--r--   0        0        0      730 2023-06-07 16:19:00.443243 heatshrinkpy-0.11.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/__init__.py
--rw-r--r--   0        0        0     2510 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/constants.py
--rw-r--r--   0        0        0     3281 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/files/foo-8-5.hs
--rw-r--r--   0        0        0     2727 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/files/foo.hs
--rw-r--r--   0        0        0     3970 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/files/foo.txt
--rw-r--r--   0        0        0     2167 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/test_command_line.py
--rw-r--r--   0        0        0     6032 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/test_core.py
--rw-r--r--   0        0        0    11667 2023-06-07 16:19:00.438243 heatshrinkpy-0.11.0/tests/test_streams.py
--rw-r--r--   0        0        0      795 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/utils.py
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 heatshrinkpy-0.11.0/PKG-INFO
+-rw-r--r--   0        0        0      898 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.1/LICENSE
+-rw-r--r--   0        0        0      702 2023-06-07 16:19:00.444244 heatshrinkpy-0.11.1/README.rst
+-rw-r--r--   0        0        0     3088 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.1/heatshrinkpy/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.1/heatshrinkpy/__main__.py
+-rw-r--r--   0        0        0     2693 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.1/heatshrinkpy/core/__init__.py
+-rw-r--r--   0        0        0      813 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.1/heatshrinkpy/core/common.py
+-rw-r--r--   0        0        0      146 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.1/heatshrinkpy/core/consts.py
+-rw-r--r--   0        0        0     7404 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.1/heatshrinkpy/core/decoder.py
+-rw-r--r--   0        0        0     9908 2023-06-15 08:27:39.114400 heatshrinkpy-0.11.1/heatshrinkpy/core/encoder.py
+-rw-r--r--   0        0        0    12855 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.1/heatshrinkpy/streams.py
+-rw-r--r--   0        0        0      258 2023-06-07 16:19:00.439243 heatshrinkpy-0.11.1/heatshrinkpy/version.py
+-rw-r--r--   0        0        0      730 2023-06-15 08:31:23.154394 heatshrinkpy-0.11.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.1/tests/__init__.py
+-rw-r--r--   0        0        0     2510 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.1/tests/constants.py
+-rw-r--r--   0        0        0     3281 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.1/tests/files/foo-8-5.hs
+-rw-r--r--   0        0        0     2727 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.1/tests/files/foo.hs
+-rw-r--r--   0        0        0     3970 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.1/tests/files/foo.txt
+-rw-r--r--   0        0        0     2167 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.1/tests/test_command_line.py
+-rw-r--r--   0        0        0     6348 2023-06-15 08:27:41.608284 heatshrinkpy-0.11.1/tests/test_core.py
+-rw-r--r--   0        0        0    11667 2023-06-07 16:19:00.438243 heatshrinkpy-0.11.1/tests/test_streams.py
+-rw-r--r--   0        0        0      795 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.1/tests/utils.py
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 heatshrinkpy-0.11.1/PKG-INFO
```

### Comparing `heatshrinkpy-0.11.0/LICENSE` & `heatshrinkpy-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/README.rst` & `heatshrinkpy-0.11.1/README.rst`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/heatshrinkpy/__init__.py` & `heatshrinkpy-0.11.1/heatshrinkpy/__init__.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/heatshrinkpy/core/__init__.py` & `heatshrinkpy-0.11.1/heatshrinkpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/heatshrinkpy/core/common.py` & `heatshrinkpy-0.11.1/heatshrinkpy/core/common.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/heatshrinkpy/core/decoder.py` & `heatshrinkpy-0.11.1/heatshrinkpy/core/decoder.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/heatshrinkpy/core/encoder.py` & `heatshrinkpy-0.11.1/heatshrinkpy/core/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         while pos - start >= 0:
             ml = 0
             if self._buffer[pos + match_maxlen] != self._buffer[end + match_maxlen]:
                 pos = self._search_index[pos]
                 continue
 
             for ml in range(1, maxlen + 1):
-                if self._buffer[pos + ml] != self._buffer[end + ml]:
+                if ml == maxlen or self._buffer[pos + ml] != self._buffer[end + ml]:
                     break
 
             if ml > match_maxlen:
                 match_maxlen = ml
                 match_index = pos
                 if ml == maxlen:
                     break
```

### Comparing `heatshrinkpy-0.11.0/heatshrinkpy/streams.py` & `heatshrinkpy-0.11.1/heatshrinkpy/streams.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/pyproject.toml` & `heatshrinkpy-0.11.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heatshrinkpy"
-version = "0.11.0"
+version = "0.11.1"
 description = "Pure Python heatshrink library, based on heatshrink2 library"
 # Poetry includes only the first author in the dist
 # as python metadata supports only a single author
 authors = [
     "Marcin Jaworski <marcin@jaworski.me>",
     "Antonis Kalou <antonis@johan-sports.com>",
     "Erik Moqvist <erik.moqvist@gmail.com>",
```

### Comparing `heatshrinkpy-0.11.0/tests/constants.py` & `heatshrinkpy-0.11.1/tests/constants.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/tests/files/foo-8-5.hs` & `heatshrinkpy-0.11.1/tests/files/foo-8-5.hs`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/tests/files/foo.hs` & `heatshrinkpy-0.11.1/tests/files/foo.hs`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/tests/files/foo.txt` & `heatshrinkpy-0.11.1/tests/files/foo.txt`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/tests/test_command_line.py` & `heatshrinkpy-0.11.1/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/tests/test_core.py` & `heatshrinkpy-0.11.1/tests/test_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,7 +156,13 @@
     def test_with_large_strings(self):
         test_sizes = [1000, 10000, 100000]
 
         for size in test_sizes:
             contents = random_string(size).encode('ascii')
             decompressed = heatshrink.decompress(heatshrink.compress(contents))
             self.assertEqual(decompressed, contents)
+
+    def test_with_all_zeros_longer_than_windows_size(self):
+        contents = b"\x00" * 8004
+        compressed = heatshrink.compress(contents, window_sz2=12, lookahead_sz2=4)
+        decompressed = heatshrink.decompress(compressed, window_sz2=12, lookahead_sz2=4)
+        self.assertEqual(contents, decompressed)
```

### Comparing `heatshrinkpy-0.11.0/tests/test_streams.py` & `heatshrinkpy-0.11.1/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/tests/utils.py` & `heatshrinkpy-0.11.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.11.0/PKG-INFO` & `heatshrinkpy-0.11.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatshrinkpy
-Version: 0.11.0
+Version: 0.11.1
 Summary: Pure Python heatshrink library, based on heatshrink2 library
 License: ISC
 Author: Marcin Jaworski
 Author-email: marcin@jaworski.me
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

