# Comparing `tmp/crelm-0.0.33a1.tar.gz` & `tmp/crelm-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crelm-0.0.33a1.tar", max compression
+gzip compressed data, was "crelm-0.0.35.tar", max compression
```

## Comparing `crelm-0.0.33a1.tar` & `crelm-0.0.35.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1108 2023-05-03 17:25:38.782803 crelm-0.0.33a1/LICENSE
--rw-r--r--   0        0        0      600 2023-05-03 17:25:38.782803 crelm-0.0.33a1/README.md
--rw-r--r--   0        0        0      187 2023-05-03 17:25:38.782803 crelm-0.0.33a1/crelm/__init__.py
--rw-r--r--   0        0        0     3071 2023-05-03 17:25:38.782803 crelm-0.0.33a1/crelm/factory.py
--rw-r--r--   0        0        0      388 2023-05-13 18:12:40.800567 crelm-0.0.33a1/crelm/libcrelm.py
--rw-r--r--   0        0        0   107326 2023-05-03 17:25:38.784803 crelm-0.0.33a1/crelm/makeheaders.c
--rw-r--r--   0        0        0     1987 2023-05-03 17:25:38.784803 crelm-0.0.33a1/crelm/makeheaders_crelm.c
--rw-r--r--   0        0        0    14462 2023-05-13 14:41:12.722203 crelm-0.0.33a1/crelm/tube.py
--rw-r--r--   0        0        0      778 2023-05-13 18:05:17.136000 crelm-0.0.33a1/pyproject.toml
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 crelm-0.0.33a1/PKG-INFO
+-rw-r--r--   0        0        0     1108 2023-05-03 17:25:38.782803 crelm-0.0.35/LICENSE
+-rw-r--r--   0        0        0      600 2023-05-03 17:25:38.782803 crelm-0.0.35/README.md
+-rw-r--r--   0        0        0      187 2023-05-03 17:25:38.782803 crelm-0.0.35/crelm/__init__.py
+-rw-r--r--   0        0        0     3071 2023-05-14 14:20:50.777933 crelm-0.0.35/crelm/factory.py
+-rw-r--r--   0        0        0      388 2023-05-13 18:12:40.800567 crelm-0.0.35/crelm/libcrelm.py
+-rw-r--r--   0        0        0   107326 2023-05-03 17:25:38.784803 crelm-0.0.35/crelm/makeheaders.c
+-rw-r--r--   0        0        0     1987 2023-05-03 17:25:38.784803 crelm-0.0.35/crelm/makeheaders_crelm.c
+-rw-r--r--   0        0        0    15200 2023-06-15 19:32:10.157880 crelm-0.0.35/crelm/tube.py
+-rw-r--r--   0        0        0      776 2023-06-15 19:37:49.788553 crelm-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 crelm-0.0.35/PKG-INFO
```

### Comparing `crelm-0.0.33a1/LICENSE` & `crelm-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `crelm-0.0.33a1/README.md` & `crelm-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `crelm-0.0.33a1/crelm/factory.py` & `crelm-0.0.35/crelm/factory.py`

 * *Files identical despite different names*

### Comparing `crelm-0.0.33a1/crelm/makeheaders.c` & `crelm-0.0.35/crelm/makeheaders.c`

 * *Files identical despite different names*

### Comparing `crelm-0.0.33a1/crelm/makeheaders_crelm.c` & `crelm-0.0.35/crelm/makeheaders_crelm.c`

 * *Files identical despite different names*

### Comparing `crelm-0.0.33a1/crelm/tube.py` & `crelm-0.0.35/crelm/tube.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         self._name = name
 
         self._source_folder = '.'
         self._target_folder = None
         self._imports = []
         self._header_filenames = []
         self._source_filenames = []
+        self._include_dirs = []
         self._source_text = ''
         self._header_text = ''
         self._macros = []
         self._externs = []
         self._compiler_args = []
         self._lib_path = None
         self._temp_folderbame = path_join(gettempdir(), 'crelm')
@@ -118,21 +119,23 @@
             [line.strip() for line in lines if not line.startswith('#')]).strip()
 
     def _preprocess_headers(self) -> str:
 
         headers = '\n'.join(
             [f'#include "{x}"' for x in self._header_filenames])
 
+        include_dirs = ' '.join([f'-I {x}' for x in self._include_dirs])
+                                
         amalgamated_header_filename = self._make_gen_filename(
             'amalgamated_headers.h')
 
         with open(amalgamated_header_filename, 'wt') as f:
             f.write(headers)
 
-        command = f'gcc -w -E {self.compile_defines} {amalgamated_header_filename}'
+        command = f'gcc -w -E {self.compile_defines} {include_dirs} {amalgamated_header_filename}'
         if self._verbose:
             print(f'_preprocess_headers: {command}')
 
         output, status = pexpect_run(command, withexitstatus=True)
         if status != 0:
             if self._verbose:
                 print(output.decode())
@@ -227,34 +230,35 @@
         args = self._build_compiler_args()
 
         if self._verbose:
             print(f'module: {self._module_name}')
             print(f'cdef: {self._cdef}')
             print(f'headers: {headers}')
             print(f'sources: {source_filenames}')
+            print(f'include dirs: {self._include_dirs}')
             print(f'externs: {self._externs}')
             print(f'args: {args}')
             print(f'verbose: {self._verbose}')
             print(f'gen folder: {self._gen_foldername}')
 
         ffibuilder = FFI()
 
         try:
             ffibuilder.cdef(self._cdef)
-        except:
+        except BaseException as arg:
             print(self._cdef)
-            print(f'{self._name}: invalid cdef')
+            print(f'{self._name}: invalid cdef ({arg})')
             return False
 
         ffibuilder.set_source(self._module_name,
                               headers,
                               sources=source_filenames,
                               extra_compile_args=args,
                               libraries=[],
-                              include_dirs=[],
+                              include_dirs=self._include_dirs,
                               library_dirs=[],
                               )
 
         try:
             self._lib_path = ffibuilder.compile(
                 tmpdir=self._gen_foldername,
                 verbose=self._verbose)
@@ -275,15 +279,15 @@
         self._compiler_args.append(f'-Wno-{warning}')
         return self
 
     def save_compiler_temps(self) -> TSelf:
         self._compiler_args.append('-save-temps=obj')
         return self
 
-    def set_gen_folder(self, path: str) -> TSelf:
+    def set_gen_folder(self, path: str) -> TSelf: # todo foss: something about this
         # self._gen_foldername = path
         return self
 
     def set_source_folder(self, folder: str) -> TSelf:
         self._source_folder = folder
         return self
 
@@ -331,14 +335,24 @@
             self.add_source_and_header_file(filename)
         return self
 
     def add_source_text(self, text: str) -> TSelf:
         self._source_text += '\n' + text
         return self
 
+    def add_include_dir_relative(self, dir: str) -> TSelf:
+        fullpath = self._make_source_fullpath(dir)
+        self._include_dirs.append(fullpath)
+        return self
+
+    def add_include_dir(self, dir: str) -> TSelf:
+        path = realpath(dir)
+        self._include_dirs.append(path)
+        return self
+
     def add_macro(self, macro: str) -> TSelf:
         self._macros.append(macro)
         return self
 
     def add_macros(self, macros: List[str]) -> TSelf:
         for macro in macros:
             self._macros.append(macro)
@@ -422,18 +436,21 @@
             except BaseException as arg:
                 print(f'{self._name}: build failed ({arg})')
                 return None
 
         from sys import path
         path.append(self._gen_foldername)
 
+        if self._verbose:
+            print(f'loading module {self._module_name} from {self._gen_foldername}...')
+
         try:
             module = import_module(self._module_name)
-        except Exception as error:
-            print(f'{self._name}: Unable to load module {error}')
+        except BaseException as arg:
+            print(f'{self._name}: Unable to load module ({arg})')
             return None
 
         reload(module)
         self._lib = module.lib
         self._ffi = module.ffi
 
         paste = Tube.Paste(self)
```

### Comparing `crelm-0.0.33a1/pyproject.toml` & `crelm-0.0.35/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crelm"
-version = "0.0.33a1"
+version = "0.0.35"
 description = "Utility that automates turning simple C classes into Python objects"
 authors = [
   "WideOpenTech <foss@wideopentech.co.uk>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `crelm-0.0.33a1/PKG-INFO` & `crelm-0.0.35/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crelm
-Version: 0.0.33a1
+Version: 0.0.35
 Summary: Utility that automates turning simple C classes into Python objects
 Home-page: https://github.com/wideopensource/crelm
 Author: WideOpenTech
 Author-email: foss@wideopentech.co.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

