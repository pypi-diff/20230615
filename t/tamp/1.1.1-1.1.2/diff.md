# Comparing `tmp/tamp-1.1.1.tar.gz` & `tmp/tamp-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamp-1.1.1.tar", max compression
+gzip compressed data, was "tamp-1.1.2.tar", max compression
```

## Comparing `tamp-1.1.1.tar` & `tamp-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-06-09 19:43:29.360603 tamp-1.1.1/LICENSE
--rw-r--r--   0        0        0    17462 2023-06-09 19:43:29.360603 tamp-1.1.1/README.rst
--rw-r--r--   0        0        0     2226 2023-06-09 19:43:29.364603 tamp-1.1.1/build.py
--rw-r--r--   0        0        0     5577 2023-06-09 19:43:54.016758 tamp-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2806 2023-06-09 19:43:54.020758 tamp-1.1.1/tamp/__init__.py
--rw-r--r--   0        0        0     1619 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/__init__.pyi
--rw-r--r--   0        0        0       57 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/__main__.py
--rw-r--r--   0        0        0       65 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_common.pxd
--rw-r--r--   0        0        0      343 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_common.pyx
--rw-r--r--   0        0        0     4498 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_compressor.pyx
--rw-r--r--   0        0        0     3994 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_decompressor.pyx
--rw-r--r--   0        0        0      834 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_src/tamp/common.c
--rw-r--r--   0        0        0     1515 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_src/tamp/common.h
--rw-r--r--   0        0        0    11579 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_src/tamp/compressor.c
--rw-r--r--   0        0        0     5468 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_src/tamp/compressor.h
--rw-r--r--   0        0        0     8294 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_src/tamp/decompressor.c
--rw-r--r--   0        0        0     2524 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/_c_src/tamp/decompressor.h
--rw-r--r--   0        0        0        0 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/cli/__init__.py
--rw-r--r--   0        0        0     2715 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/cli/main.py
--rw-r--r--   0        0        0     8656 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/compressor.py
--rw-r--r--   0        0        0     7257 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/compressor_viper.py
--rw-r--r--   0        0        0     2802 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/ctamp.pxd
--rw-r--r--   0        0        0     7626 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/decompressor.py
--rw-r--r--   0        0        0     9543 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/decompressor_viper.py
--rw-r--r--   0        0        0        0 2023-06-09 19:43:29.368603 tamp-1.1.1/tamp/py.typed
--rw-r--r--   0        0        0    18074 1970-01-01 00:00:00.000000 tamp-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-15 21:03:04.536048 tamp-1.1.2/LICENSE
+-rw-r--r--   0        0        0    17339 2023-06-15 21:03:04.536048 tamp-1.1.2/README.rst
+-rw-r--r--   0        0        0     2851 2023-06-15 21:03:04.540048 tamp-1.1.2/build.py
+-rw-r--r--   0        0        0     5577 2023-06-15 21:03:33.391772 tamp-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2806 2023-06-15 21:03:33.395772 tamp-1.1.2/tamp/__init__.py
+-rw-r--r--   0        0        0     1619 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/__init__.pyi
+-rw-r--r--   0        0        0       57 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/__main__.py
+-rw-r--r--   0        0        0       65 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_common.pxd
+-rw-r--r--   0        0        0      343 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_common.pyx
+-rw-r--r--   0        0        0     4498 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_compressor.pyx
+-rw-r--r--   0        0        0     4168 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_decompressor.pyx
+-rw-r--r--   0        0        0      834 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/common.c
+-rw-r--r--   0        0        0     1791 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/common.h
+-rw-r--r--   0        0        0    11680 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/compressor.c
+-rw-r--r--   0        0        0     5468 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/compressor.h
+-rw-r--r--   0        0        0     8976 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/decompressor.c
+-rw-r--r--   0        0        0     2524 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/_c_src/tamp/decompressor.h
+-rw-r--r--   0        0        0        0 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/cli/__init__.py
+-rw-r--r--   0        0        0     2715 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/cli/main.py
+-rw-r--r--   0        0        0     8656 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/compressor.py
+-rw-r--r--   0        0        0     7257 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/compressor_viper.py
+-rw-r--r--   0        0        0     2802 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/ctamp.pxd
+-rw-r--r--   0        0        0     7882 2023-06-15 21:03:04.544048 tamp-1.1.2/tamp/decompressor.py
+-rw-r--r--   0        0        0     9681 2023-06-15 21:03:04.548048 tamp-1.1.2/tamp/decompressor_viper.py
+-rw-r--r--   0        0        0        0 2023-06-15 21:03:04.548048 tamp-1.1.2/tamp/py.typed
+-rw-r--r--   0        0        0    17951 1970-01-01 00:00:00.000000 tamp-1.1.2/PKG-INFO
```

### Comparing `tamp-1.1.1/LICENSE` & `tamp-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/README.rst` & `tamp-1.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -279,21 +279,22 @@
 Both tamp and heatshrink have a few dozen bytes of overhead in addition to the primary window buffer, but are implementation-specific and ignored for clarity here.
 
 Runtime
 ^^^^^^^
 As a rough benchmark, here is the performance (in seconds) of these different compression algorithms on the 100MB enwik8 dataset.
 These tests were performed on an M1 Macbook Air.
 
-+---------------+-------------------------+----------+------+-------------------------+----------------------------+
-| Action        | tamp (Python Reference) | tamp (C) | zlib | heatshrink (with index) | heatshrink (without index) |
-+===============+=========================+==========+======+=========================+============================+
-| Compression   | 109.5                   | 17.44    | 4.84 | 6.22                    | 41.729                     |
-+---------------+-------------------------+----------+------+-------------------------+----------------------------+
-| Decompression | 54.0                    | 0.09     | 0.08 | 0.82                    | 0.82                       |
-+---------------+-------------------------+----------+------+-------------------------+----------------------------+
++---------------+--------------------+-------+------+--------------+-----------------+
+| Action        | tamp               | tamp  | zlib | heatshrink   | heatshrink      |
+|               | (Python Reference) | (C)   |      | (with index) | (without index) |
++===============+====================+=======+======+==============+=================+
+| Compression   | 109.5              | 16.45 | 4.84 | 6.22         | 41.729          |
++---------------+--------------------+-------+------+--------------+-----------------+
+| Decompression | 54.0               | 0.98  | 0.08 | 0.82         | 0.82            |
++---------------+--------------------+-------+------+--------------+-----------------+
 
 Heatshrink v0.4.1 was used in these benchmarks.
 When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, tripling the memory requirement.
 Tamp could use a similar indexing to increase compression speed, but has chosen not to to focus on the primary goal of a low-memory compressor.
 
 Binary Size
 ^^^^^^^^^^^
@@ -302,15 +303,15 @@
 Numbers reported in bytes.
 
 +--------------------+------------+--------------+---------------------------+
 | Library            | Compressor | Decompressor | Compressor + Decompressor |
 +====================+============+==============+===========================+
 | Tamp (micropython) | 4779       | 4717         | 8262                      |
 +--------------------+------------+--------------+---------------------------+
-| Tamp (C)           | 2956       | 2204         | 5036                      |
+| Tamp (C)           | 2996       | 2192         | 5064                      |
 +--------------------+------------+--------------+---------------------------+
 | Heatshrink         | 2956       | 3876         | 6832                      |
 +--------------------+------------+--------------+---------------------------+
 | uzlib              | 2355       | 3963         | 6318                      |
 +--------------------+------------+--------------+---------------------------+
 
 Heatshrink doesn't include a high level API; in an apples-to-apples comparison the Tamp library would be even smaller.
```

### Comparing `tamp-1.1.1/build.py` & `tamp-1.1.2/build.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 import os
 import shutil
 from pathlib import Path
 
 allowed_to_fail = os.environ.get("CIBUILDWHEEL", "0") != "1"
 
+profile = os.environ.get("TAMP_PROFILE", "0") == "1"
+
 
 def build_cython_extensions():
+    import Cython.Compiler.Options
     from Cython.Build import build_ext, cythonize
+    from Cython.Compiler.Options import get_directive_defaults
     from setuptools import Extension
     from setuptools.dist import Distribution
 
+    Cython.Compiler.Options.annotate = True
+
+    define_macros = []
+
+    if profile:
+        print("Setting profiling configuration.")
+        directive_defaults = get_directive_defaults()
+        directive_defaults["linetrace"] = True
+        directive_defaults["binding"] = True
+
+        define_macros.append(("CYTHON_TRACE", "1"))
+
     if os.name == "nt":  # Windows
         extra_compile_args = [
             "/O2",
         ]
     else:  # UNIX-based systems
         extra_compile_args = [
             "-O3",
@@ -30,43 +46,46 @@
                 "tamp/_c_src/tamp/common.c",
                 "tamp/_c_src/tamp/compressor.c",
                 "tamp/_c_compressor.pyx",
             ],
             include_dirs=include_dirs,
             extra_compile_args=extra_compile_args,
             language="c",
+            define_macros=define_macros,
         ),
         Extension(
             "tamp._c_decompressor",
             [
                 "tamp/_c_src/tamp/common.c",
                 "tamp/_c_src/tamp/decompressor.c",
                 "tamp/_c_decompressor.pyx",
             ],
             include_dirs=include_dirs,
             extra_compile_args=extra_compile_args,
             language="c",
+            define_macros=define_macros,
         ),
         Extension(
             "tamp._c_common",
             [
                 "tamp/_c_common.pyx",
             ],
             include_dirs=include_dirs,
             extra_compile_args=extra_compile_args,
             language="c",
+            define_macros=define_macros,
         ),
     ]
 
     include_dirs = set()
     for extension in extensions:
         include_dirs.update(extension.include_dirs)
     include_dirs = list(include_dirs)
 
-    ext_modules = cythonize(extensions, include_path=include_dirs, language_level=3)
+    ext_modules = cythonize(extensions, include_path=include_dirs, language_level=3, annotate=True)
     dist = Distribution({"ext_modules": ext_modules})
     cmd = build_ext(dist)
     cmd.ensure_finalized()
     cmd.run()
 
     for output in cmd.get_outputs():
         output = Path(output)
```

### Comparing `tamp-1.1.1/pyproject.toml` & `tamp-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "semver"
 
 [tool.poetry]
 name = "tamp"
-version = "1.1.1"  # Do not change, let poetry-dynamic-versioning handle it.
+version = "1.1.2"  # Do not change, let poetry-dynamic-versioning handle it.
 homepage = "https://github.com/BrianPugh/tamp"
 repository = "https://github.com/BrianPugh/tamp"
 license = "Apache-2.0"
 description = ""
 authors = ["Brian Pugh"]
 readme = "README.rst"
 packages = [{include = "tamp"}]
```

### Comparing `tamp-1.1.1/tamp/__init__.py` & `tamp-1.1.2/tamp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Don't manually change, let poetry-dynamic-versioning-plugin handle it.
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 
 class ExcessBitsError(Exception):
     """Provided data has more bits than expected ``literal`` bits."""
 
 
 def bit_size(value):
```

### Comparing `tamp-1.1.1/tamp/__init__.pyi` & `tamp-1.1.2/tamp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/tamp/_c_compressor.pyx` & `tamp-1.1.2/tamp/_c_compressor.pyx`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/tamp/_c_decompressor.pyx` & `tamp-1.1.2/tamp/_c_decompressor.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         bytearray _window_buffer
         unsigned char *_window_buffer_ptr
         object input_buffer
         unsigned char *input_buffer_ptr
         size_t input_size
         size_t input_consumed
         object f
+        cdef bint _close_f_on_close
 
     def __cinit__(self):
         self._c_decompressor = <ctamp.TampDecompressor*>PyMem_Malloc(sizeof(ctamp.TampDecompressor))
         if self._c_decompressor is NULL:
             raise MemoryError
 
     def __dealloc__(self):
@@ -33,14 +34,17 @@
     def __init__(self, f, *, dictionary=None):
         cdef:
             ctamp.TampConf conf
             size_t input_consumed_size;
 
         if not hasattr(f, "read"):  # It's probably a path-like object.
             f = open(str(f), "rb")
+            self._close_f_on_close = True
+        else:
+            self._close_f_on_close = False
 
         self.f = f
 
         self.input_buffer = bytearray(CHUNK_SIZE)
         self.input_buffer_ptr = self.input_buffer
         self.input_size = 0
         self.input_consumed = 0
@@ -103,15 +107,16 @@
 
             # Check signals for things like KeyboardInterrupt
             PyErr_CheckSignals()
 
         return bytearray().join(output_list)
 
     def close(self):
-        self.f.close()
+        if self._close_f_on_close:
+            self.f.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tamp-1.1.1/tamp/_c_src/tamp/common.c` & `tamp-1.1.2/tamp/_c_src/tamp/common.c`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/tamp/_c_src/tamp/common.h` & `tamp-1.1.2/tamp/_c_src/tamp/common.h`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 extern "C" {
 #endif
 
 #include <stdlib.h>
 #include <stdbool.h>
 #include <stdint.h>
 
+/* Compiler branch optimizations */
+#if defined(__clang__) || (defined(__GNUC__) && (__GNUC__ > 2))
+#define TAMP_LIKELY(c) (__builtin_expect(!!(c), 1))
+#define TAMP_UNLIKELY(c) (__builtin_expect(!!(c), 0))
+#else
+#define TAMP_LIKELY(c) (c)
+#define TAMP_UNLIKELY(c) (c)
+#endif
+
 enum {
     /* Normal/Recoverable status >= 0 */
     TAMP_OK = 0,
     TAMP_OUTPUT_FULL = 1,  // Wasn't able to complete action due to full output buffer.
     TAMP_INPUT_EXHAUSTED = 2, // Wasn't able to complete action due to exhausted input buffer.
 
     /* Error codes < 0 */
```

### Comparing `tamp-1.1.1/tamp/_c_src/tamp/compressor.c` & `tamp-1.1.2/tamp/_c_src/tamp/compressor.c`

 * *Files 3% similar despite different names*

```diff
@@ -68,42 +68,42 @@
 static inline void find_best_match(
         TampCompressor *compressor,
         uint16_t *match_index,
         uint8_t *match_size
         ){
     *match_size = 0;
 
-    if(compressor->input_size < compressor->min_pattern_size)
+    if(TAMP_UNLIKELY(compressor->input_size < compressor->min_pattern_size))
         return;
 
     const uint16_t first_second = (read_input(0) << 8) | read_input(1);
     const uint16_t window_size_minus_1 = WINDOW_SIZE - 1;
     const uint8_t max_pattern_size = MIN(compressor->input_size, MAX_PATTERN_SIZE);
     uint16_t meow = compressor->window[0];
     unsigned char c;
 
     for(uint16_t window_index=0; window_index < window_size_minus_1; window_index++){
         meow <<= 8;
         meow |= compressor->window[window_index + 1];
-        if(meow != first_second)
+        if(TAMP_LIKELY(meow != first_second))
             continue;
 
         for(uint8_t input_offset=2; ; input_offset++){
-            if(input_offset > *match_size){
+            if(TAMP_UNLIKELY(input_offset > *match_size)){
                 *match_size = input_offset;
                 *match_index = window_index;
-                if(*match_size == max_pattern_size)
+                if(TAMP_UNLIKELY(*match_size == max_pattern_size))
                     return;
             }
 
-            if(window_index + input_offset > window_size_minus_1)
+            if(TAMP_UNLIKELY(window_index + input_offset > window_size_minus_1))
                 return;
 
             c = read_input(input_offset);
-            if(compressor->window[window_index + input_offset] != c)
+            if(TAMP_LIKELY(compressor->window[window_index + input_offset] != c))
                 break;
         }
     }
 }
 
 tamp_res tamp_compressor_init(TampCompressor *compressor, const TampConf *conf, unsigned char *window){
     const TampConf conf_default = {.window=10, .literal=8, .use_custom_dictionary=false};
@@ -198,15 +198,15 @@
         size_t input_size,
         size_t *consumed_size
         ){
     if(consumed_size)
         *consumed_size = 0;
 
     for(size_t i=0; i < input_size; i++){
-        if(compressor->input_size == sizeof(compressor->input))
+        if(TAMP_UNLIKELY(compressor->input_size == sizeof(compressor->input)))
             break;
         compressor->input[input_add(compressor->input_size)] = input[i];
         compressor->input_size += 1;
         if(consumed_size)
             (*consumed_size)++;
     }
 }
```

### Comparing `tamp-1.1.1/tamp/_c_src/tamp/compressor.h` & `tamp-1.1.2/tamp/_c_src/tamp/compressor.h`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/tamp/_c_src/tamp/decompressor.c` & `tamp-1.1.2/tamp/_c_src/tamp/decompressor.c`

 * *Files 16% similar despite different names*

```diff
@@ -15,17 +15,15 @@
  *
  * @return Tamp Status Code.
  *     TAMP_INVALID_SYMBOL if no valid symbol decoded. Buffer is NOT restored.
  */
 static int8_t huffman_decode(uint32_t *bit_buffer, uint8_t *bit_buffer_pos){
     uint8_t code = 0;
 
-    while(true){
-        if(*bit_buffer_pos == 0)
-            return -1;
+    while(TAMP_LIKELY(*bit_buffer_pos != 0)){
         code = (code << 1) | (*bit_buffer >> 31);
         *bit_buffer <<= 1;
         *bit_buffer_pos -= 1;
         switch(code){
             case 0:   return 0;
             case 3:   return 1;
             case 8:   return 2;
@@ -39,14 +37,15 @@
             case 148: return 10;
             case 149: return 11;
             case 170: return 12;
             case 39:  return 13;
             case 171: return FLUSH;
         }
     }
+    return -1;
 }
 
 tamp_res tamp_decompressor_read_header(TampConf *conf, const unsigned char *input, size_t input_size, size_t *input_consumed_size) {
     if(input_consumed_size)
         (*input_consumed_size) = 0;
     if(input_size == 0)
         return TAMP_INPUT_EXHAUSTED;
@@ -60,32 +59,47 @@
     conf->window = ((input[0] >> 5) & 0x7) + 8;
     conf->literal = ((input[0] >> 3) & 0x3) + 5;
     conf->use_custom_dictionary = ((input[0] >> 2) & 0x1);
 
     return TAMP_OK;
 }
 
+/**
+ * Populate the rest of the decompressor structure after the following fields have been populated:
+ *   * conf
+ *   * window
+ */
+static tamp_res tamp_decompressor_populate_from_conf(TampDecompressor *decompressor){
+    const TampConf *conf = &(decompressor->conf);
+    if(conf->window < 8 || conf->window > 15)
+        return TAMP_INVALID_CONF;
+    if(conf->literal < 5 || conf->literal > 8)
+        return TAMP_INVALID_CONF;
+    if(!conf->use_custom_dictionary)
+        tamp_initialize_dictionary(decompressor->window, (1 << conf->window));
+
+    decompressor->min_pattern_size = tamp_compute_min_pattern_size(
+            conf->window, conf->literal
+    );
+    decompressor->configured = true;
+
+    return TAMP_OK;
+}
+
 tamp_res tamp_decompressor_init(TampDecompressor *decompressor, const TampConf *conf, unsigned char *window){
+    tamp_res res = TAMP_OK;
     for(uint8_t i=0; i < sizeof(TampDecompressor); i++)  // Zero-out the struct
         ((unsigned char *)decompressor)[i] = 0;
     decompressor->window = window;
     if(conf){
-        if(conf->window < 8 || conf->window > 15)
-            return TAMP_INVALID_CONF;
-        if(conf->literal < 5 || conf->literal > 8)
-            return TAMP_INVALID_CONF;
-        if(!conf->use_custom_dictionary)
-            tamp_initialize_dictionary(window, (1 << conf->window));
-
-        decompressor->min_pattern_size = tamp_compute_min_pattern_size(conf->window, conf->literal);
         decompressor->conf = *conf;
-        decompressor->configured = true;
+        res = tamp_decompressor_populate_from_conf(decompressor);
     }
 
-    return TAMP_OK;
+    return res;
 }
 
 tamp_res tamp_decompressor_decompress(
         TampDecompressor *decompressor,
         unsigned char *output,
         size_t output_size,
         size_t *output_written_size,
@@ -112,33 +126,38 @@
         //Read in header
         size_t header_consumed_size;
         res = tamp_decompressor_read_header(&decompressor->conf, input, input_end - input, &header_consumed_size);
         if(res != TAMP_OK)
             return res;
         input += header_consumed_size;
         (*input_consumed_size) += header_consumed_size;
+
+        res = tamp_decompressor_populate_from_conf(decompressor);
+        if(res != TAMP_OK)
+            return res;
     }
     while(input != input_end || decompressor->bit_buffer_pos){
         // Populate the bit buffer
         while(input != input_end && decompressor->bit_buffer_pos <= 24){
             decompressor->bit_buffer_pos += 8;
             decompressor->bit_buffer |=  *input << (32 - decompressor->bit_buffer_pos);
             input++;
             (*input_consumed_size)++;
         }
 
-        if(decompressor->bit_buffer_pos == 0)
+        if(TAMP_UNLIKELY(decompressor->bit_buffer_pos == 0))
             return TAMP_INPUT_EXHAUSTED;
 
-        if(output == output_end)
+        if(TAMP_UNLIKELY(output == output_end))
             return TAMP_OUTPUT_FULL;
 
-        if(decompressor->bit_buffer >> 31){
+        // Hint that patterns are more likely than literals
+        if(TAMP_UNLIKELY(decompressor->bit_buffer >> 31)){
             // is literal
-            if(decompressor->bit_buffer_pos < (1 + decompressor->conf.literal))
+            if(TAMP_UNLIKELY(decompressor->bit_buffer_pos < (1 + decompressor->conf.literal)))
                 return TAMP_INPUT_EXHAUSTED;
             decompressor->bit_buffer <<= 1;  // shift out the is_literal flag
 
             // Copy literal to output
             *output = decompressor->bit_buffer >> (32 - decompressor->conf.literal);
             decompressor->bit_buffer <<= decompressor->conf.literal;
             decompressor->bit_buffer_pos -= (1 + decompressor->conf.literal);
@@ -159,39 +178,39 @@
             int8_t match_size;
             int8_t match_size_skip;
 
             // shift out the is_literal flag
             bit_buffer <<= 1;
             bit_buffer_pos--;
 
-            if((match_size = huffman_decode(&bit_buffer, &bit_buffer_pos)) < 0){
+            if((TAMP_UNLIKELY(match_size = huffman_decode(&bit_buffer, &bit_buffer_pos)) < 0)){
                 // Insufficient input
                 return TAMP_INPUT_EXHAUSTED;
             }
-            if(match_size == FLUSH){
+            if(TAMP_UNLIKELY(match_size == FLUSH)){
                 // flush bit_buffer to the nearest byte and skip the remainder of decoding
                 decompressor->bit_buffer = bit_buffer << (bit_buffer_pos & 7);
                 decompressor->bit_buffer_pos = bit_buffer_pos & ~7;  // Round bit_buffer_pos down to nearest multiple of 8.
                 continue;
             }
-            if(bit_buffer_pos < decompressor->conf.window){
+            if(TAMP_UNLIKELY(bit_buffer_pos < decompressor->conf.window)){
                 // There are not enough bits to decode window offset
                 return TAMP_INPUT_EXHAUSTED;
             }
             match_size += decompressor->min_pattern_size;
             window_offset = bit_buffer >> (32 - decompressor->conf.window);
 
             // Apply skip_bytes
             match_size_skip = match_size - decompressor->skip_bytes;
             window_offset_skip = window_offset + decompressor->skip_bytes;
 
             // Check if we are output-buffer-limited, and if so to set skip_bytes
             // Otherwise, update the decompressor buffers
             size_t remaining = output_end - output;
-            if((uint8_t)match_size_skip > remaining){
+            if(TAMP_UNLIKELY((uint8_t)match_size_skip > remaining)){
                 decompressor->skip_bytes += remaining;
                 match_size_skip = remaining;
             }
             else {
                 decompressor->skip_bytes = 0;
                 decompressor->bit_buffer = bit_buffer << decompressor->conf.window;
                 decompressor->bit_buffer_pos = bit_buffer_pos - decompressor->conf.window;
@@ -199,15 +218,15 @@
 
             // Copy pattern to output
             for(uint8_t i=0; i < match_size_skip; i++){
                 *output++ = decompressor->window[window_offset_skip + i];
             }
             (*output_written_size) += match_size_skip;
 
-            if(decompressor->skip_bytes == 0){
+            if(TAMP_LIKELY(decompressor->skip_bytes == 0)){
                 // Perform window update;
                 // copy to a temporary buffer in case src precedes dst, and is overlapping.
                 uint8_t tmp_buf[16];
                 for(uint8_t i=0; i < match_size; i++){
                     tmp_buf[i] = decompressor->window[window_offset + i];
                 }
                 for(uint8_t i=0; i < match_size; i++){
```

### Comparing `tamp-1.1.1/tamp/_c_src/tamp/decompressor.h` & `tamp-1.1.2/tamp/_c_src/tamp/decompressor.h`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/tamp/cli/main.py` & `tamp-1.1.2/tamp/cli/main.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/tamp/compressor.py` & `tamp-1.1.2/tamp/compressor.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/tamp/compressor_viper.py` & `tamp-1.1.2/tamp/compressor_viper.py`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/tamp/ctamp.pxd` & `tamp-1.1.2/tamp/ctamp.pxd`

 * *Files identical despite different names*

### Comparing `tamp-1.1.1/tamp/decompressor.py` & `tamp-1.1.2/tamp/decompressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     0b10101011: _FLUSH,
 }
 
 
 class BitReader:
     """Reads bits from a stream."""
 
-    def __init__(self, f):
+    def __init__(self, f, close_f_on_close=False):
+        self.close_f_on_close = close_f_on_close
         self.f = f
         self.clear()
 
     def read_huffman(self):
         proposed_code = 0
         lookup = huffman_lookup
         read = self.read
@@ -69,14 +70,16 @@
         self.bit_pos = 0
 
         self.backup_buffer = None
         self.backup_bit_pos = None
 
     def close(self):
         self.f.close()
+        if self.close_f_on_close:
+            self.f.close()
 
     def __len__(self):
         return self.bit_pos
 
     def __enter__(self):
         # Context manager to restore all read bits in a session if any read fails.
 
@@ -130,16 +133,19 @@
         f: Union[file, str]
             File-like object to read compressed bytes from.
         dictionary: bytearray
             Use dictionary inplace as window buffer.
         """
         if not hasattr(f, "read"):  # It's probably a path-like object.
             f = open(str(f), "rb")
+            close_f_on_close = True
+        else:
+            close_f_on_close = False
 
-        self._bit_reader = BitReader(f)
+        self._bit_reader = BitReader(f, close_f_on_close=close_f_on_close)
 
         # Read Header
         self.window_bits = self._bit_reader.read(3) + 8
         self.literal_bits = self._bit_reader.read(2) + 5
         uses_custom_dictionary = self._bit_reader.read(1)
         reserved = self._bit_reader.read(1)
         more_header_bytes = self._bit_reader.read(1)
```

### Comparing `tamp-1.1.1/tamp/decompressor_viper.py` & `tamp-1.1.2/tamp/decompressor_viper.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from . import compute_min_pattern_size, initialize_dictionary
 
 
 class Decompressor:
     def __init__(self, f, *, dictionary=None):
         if not hasattr(f, "read"):  # It's probably a path-like object.
             f = open(str(f), "rb")
+            self._close_f_on_close = True
+        else:
+            self._close_f_on_close = False
 
         self.f = f
         self.f_buf = 0
         self.f_pos = 0
 
         # Read Header
         header = self.f.read(1)[0]
@@ -232,15 +235,16 @@
             decompressed_bytes = self._decompress_into(out)
             if decompressed_bytes != size:
                 out = out[:decompressed_bytes]
 
         return out
 
     def close(self):
-        self.f.close()
+        if self._close_f_on_close:
+            self.f.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tamp-1.1.1/PKG-INFO` & `tamp-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tamp
-Version: 1.1.1
+Version: 1.1.2
 Summary: 
 Home-page: https://github.com/BrianPugh/tamp
 License: Apache-2.0
 Author: Brian Pugh
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -297,21 +297,22 @@
 Both tamp and heatshrink have a few dozen bytes of overhead in addition to the primary window buffer, but are implementation-specific and ignored for clarity here.
 
 Runtime
 ^^^^^^^
 As a rough benchmark, here is the performance (in seconds) of these different compression algorithms on the 100MB enwik8 dataset.
 These tests were performed on an M1 Macbook Air.
 
-+---------------+-------------------------+----------+------+-------------------------+----------------------------+
-| Action        | tamp (Python Reference) | tamp (C) | zlib | heatshrink (with index) | heatshrink (without index) |
-+===============+=========================+==========+======+=========================+============================+
-| Compression   | 109.5                   | 17.44    | 4.84 | 6.22                    | 41.729                     |
-+---------------+-------------------------+----------+------+-------------------------+----------------------------+
-| Decompression | 54.0                    | 0.09     | 0.08 | 0.82                    | 0.82                       |
-+---------------+-------------------------+----------+------+-------------------------+----------------------------+
++---------------+--------------------+-------+------+--------------+-----------------+
+| Action        | tamp               | tamp  | zlib | heatshrink   | heatshrink      |
+|               | (Python Reference) | (C)   |      | (with index) | (without index) |
++===============+====================+=======+======+==============+=================+
+| Compression   | 109.5              | 16.45 | 4.84 | 6.22         | 41.729          |
++---------------+--------------------+-------+------+--------------+-----------------+
+| Decompression | 54.0               | 0.98  | 0.08 | 0.82         | 0.82            |
++---------------+--------------------+-------+------+--------------+-----------------+
 
 Heatshrink v0.4.1 was used in these benchmarks.
 When heathshrink uses an index, an additional ``(1 << (windowBits + 1))`` bytes of memory are used, tripling the memory requirement.
 Tamp could use a similar indexing to increase compression speed, but has chosen not to to focus on the primary goal of a low-memory compressor.
 
 Binary Size
 ^^^^^^^^^^^
@@ -320,15 +321,15 @@
 Numbers reported in bytes.
 
 +--------------------+------------+--------------+---------------------------+
 | Library            | Compressor | Decompressor | Compressor + Decompressor |
 +====================+============+==============+===========================+
 | Tamp (micropython) | 4779       | 4717         | 8262                      |
 +--------------------+------------+--------------+---------------------------+
-| Tamp (C)           | 2956       | 2204         | 5036                      |
+| Tamp (C)           | 2996       | 2192         | 5064                      |
 +--------------------+------------+--------------+---------------------------+
 | Heatshrink         | 2956       | 3876         | 6832                      |
 +--------------------+------------+--------------+---------------------------+
 | uzlib              | 2355       | 3963         | 6318                      |
 +--------------------+------------+--------------+---------------------------+
 
 Heatshrink doesn't include a high level API; in an apples-to-apples comparison the Tamp library would be even smaller.
```

