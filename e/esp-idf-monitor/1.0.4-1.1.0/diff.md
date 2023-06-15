# Comparing `tmp/esp-idf-monitor-1.0.4.tar.gz` & `tmp/esp-idf-monitor-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-60e4z_0t/esp-idf-monitor-1.0.4.tar", last modified: Fri Apr 21 13:10:59 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-cmnzt9cx/esp-idf-monitor-1.1.0.tar", last modified: Thu Jun 15 14:48:47 2023, max compression
```

## Comparing `esp-idf-monitor-1.0.4.tar` & `esp-idf-monitor-1.1.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/ansi_color_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/chip_specific_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/console_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/console_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/coredump.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/gdbhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/line_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/output_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/pc_address_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/serial_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/base/web_socket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/gdb_panic_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17243 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/esp_idf_monitor/idf_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:10:59.000000 esp-idf-monitor-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-21 13:10:34.000000 esp-idf-monitor-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/ansi_color_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/chip_specific_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/console_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/console_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/coredump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/gdbhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/line_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/output_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/pc_address_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/rom_elf_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/serial_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/web_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/gdb_panic_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17723 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/idf_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/setup.py
```

### Comparing `esp-idf-monitor-1.0.4/LICENSE` & `esp-idf-monitor-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/PKG-INFO` & `esp-idf-monitor-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.0.4
+Version: 1.1.0
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.0.4/README.md` & `esp-idf-monitor-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/ansi_color_converter.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/ansi_color_converter.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/argument_parser.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/argument_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,14 +62,21 @@
     parser.add_argument(
         'elf_file', help='ELF file of application',
         type=lambda f: open(f, 'rb') if os.path.exists(f) else f'{f}',
         nargs='?'
     )
 
     parser.add_argument(
+        '--rom-elf-file',
+        help='ELF file of target ROM for address decoding. '
+        'If not specified, autodetection is attempted based on the IDF_PATH and ESP_ROM_ELF_DIR env vars.',
+        type=lambda f: open(f, 'rb') if os.path.exists(f) else f'{f}',
+    )
+
+    parser.add_argument(
         '--print_filter',
         help='Filtering string',
         default=DEFAULT_PRINT_FILTER)
 
     parser.add_argument(
         '--decode-coredumps',
         choices=[COREDUMP_DECODE_INFO, COREDUMP_DECODE_DISABLE],
```

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/chip_specific_config.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/chip_specific_config.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/console_parser.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/console_parser.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/console_reader.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/console_reader.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/constants.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/constants.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/coredump.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/coredump.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/gdbhelper.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/gdbhelper.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/line_matcher.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/line_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/logger.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 from .constants import ADDRESS_RE
 from .output_helpers import lookup_pc_address, red_print, yellow_print
 from .pc_address_matcher import PcAddressMatcher
 
 
 class Logger:
     def __init__(self, elf_file, console, timestamps, timestamp_format, pc_address_buffer, enable_address_decoding,
-                 toolchain_prefix):
-        # type: (str, miniterm.Console, bool, str, bytes, bool, str) -> None
+                 toolchain_prefix, rom_elf_file=None):
+        # type: (str, miniterm.Console, bool, str, bytes, bool, str, Optional[str]) -> None
         self.log_file = None  # type: Optional[BinaryIO]
         self._output_enabled = True  # type: bool
         self.elf_file = elf_file
+        self.rom_elf_file = rom_elf_file
         self.console = console
         self.timestamps = timestamps
         self.timestamp_format = timestamp_format
         self._pc_address_buffer = pc_address_buffer
         self.enable_address_decoding = enable_address_decoding
         self.toolchain_prefix = toolchain_prefix
-        self.pc_address_matcher = PcAddressMatcher(self.elf_file) if enable_address_decoding else None
+        if enable_address_decoding:
+            self.pc_address_matcher = PcAddressMatcher(self.elf_file)
+            if rom_elf_file is not None:
+                self.rom_pc_address_matcher = PcAddressMatcher(self.rom_elf_file)  # type: ignore
 
     @property
     def pc_address_buffer(self):  # type: () -> bytes
         return self._pc_address_buffer
 
     @pc_address_buffer.setter
     def pc_address_buffer(self, value):  # type: (bytes) -> None
@@ -117,11 +121,20 @@
     def handle_possible_pc_address_in_line(self, line):  # type: (bytes) -> None
         line = self._pc_address_buffer + line
         self._pc_address_buffer = b''
         if not self.enable_address_decoding:
             return
         for m in re.finditer(ADDRESS_RE, line.decode(errors='ignore')):
             num = m.group()
-            if self.pc_address_matcher.is_executable_address(int(num, 16)):  # type: ignore
+            address_int = int(num, 16)
+            translation = None
+
+            # Try looking for the address in the app ELF file
+            if self.pc_address_matcher.is_executable_address(address_int):
                 translation = lookup_pc_address(num, self.toolchain_prefix, self.elf_file)
-                if translation:
-                    self.print(translation, console_printer=yellow_print)
+            # Not found in app ELF file, check ROM ELF file (if it is available)
+            if translation is None and self.rom_elf_file is not None and self.rom_pc_address_matcher.is_executable_address(address_int):
+                translation = lookup_pc_address(num, self.toolchain_prefix, self.rom_elf_file, is_rom=True)
+
+            # Translation found either in the app or ROM ELF file
+            if translation is not None:
+                self.print(translation, console_printer=yellow_print)
```

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/output_helpers.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/output_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,18 @@
     color_print(message, ANSI_YELLOW, newline)
 
 
 def red_print(message, newline='\n'):  # type: (str, Optional[str]) -> None
     color_print(message, ANSI_RED, newline)
 
 
-def lookup_pc_address(pc_addr, toolchain_prefix, elf_file):  # type: (str, str, str) -> Optional[str]
+def lookup_pc_address(pc_addr, toolchain_prefix, elf_file, is_rom=False):  # type: (str, str, str, bool) -> Optional[str]
     cmd = ['%saddr2line' % toolchain_prefix, '-pfiaC', '-e', elf_file, pc_addr]
 
     try:
         translation = subprocess.check_output(cmd, cwd='.')
         if b'?? ??:0' not in translation:
-            return translation.decode()
+            decoded = translation.decode()
+            return decoded if not is_rom else decoded.replace('at ??:?', 'in ROM')
     except OSError as e:
         red_print('%s: %s' % (' '.join(cmd), e))
     return None
```

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/pc_address_matcher.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/pc_address_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/serial_handler.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/serial_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,17 +253,17 @@
                 data = data[(pos + 1):]
 
         sp = self.splitdata(data)
         for line in sp:
             if self._serial_check_exit and line.strip() == console_parser.exit_key.encode('latin-1'):
                 raise SerialStopException()
 
-            self.logger.print(line)
-            self.compare_elf_sha256(line.decode(errors='ignore'))
-            self._force_line_print = False
+            if self._force_line_print or line_matcher.match(line.decode(errors='ignore')):
+                self.logger.print(line)
+                self._force_line_print = False
 
         if self._last_line_part.startswith(CONSOLE_STATUS_QUERY):
             self.logger.print(CONSOLE_STATUS_QUERY)
             self._last_line_part = self._last_line_part[len(CONSOLE_STATUS_QUERY):]
 
         force_print_or_matched = any((
             self._force_line_print,
```

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/serial_reader.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/serial_reader.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/stoppable_thread.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/base/web_socket_client.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/base/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/gdb_panic_server.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/gdb_panic_server.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor/idf_monitor.py` & `esp-idf-monitor-1.1.0/esp_idf_monitor/idf_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
                                             TAG_SERIAL_FLUSH)
 from esp_idf_monitor.base.coredump import COREDUMP_DECODE_INFO, CoreDump
 from esp_idf_monitor.base.exceptions import SerialStopException
 from esp_idf_monitor.base.gdbhelper import GDBHelper
 from esp_idf_monitor.base.line_matcher import LineMatcher
 from esp_idf_monitor.base.logger import Logger
 from esp_idf_monitor.base.output_helpers import normal_print, yellow_print
+from esp_idf_monitor.base.rom_elf_getter import get_rom_elf_path
 from esp_idf_monitor.base.serial_handler import (SerialHandler,
                                                  SerialHandlerNoElf, run_make)
 from esp_idf_monitor.base.serial_reader import (LinuxReader, Reader,
                                                 SerialReader)
 from esp_idf_monitor.base.web_socket_client import WebSocketClient
 
 key_description = miniterm.key_description
@@ -90,28 +91,29 @@
         decode_coredumps=COREDUMP_DECODE_INFO,  # type: str
         decode_panic=PANIC_DECODE_DISABLE,  # type: str
         target='esp32',  # type: str
         websocket_client=None,  # type: Optional[WebSocketClient]
         enable_address_decoding=True,  # type: bool
         timestamps=False,  # type: bool
         timestamp_format='',  # type: str
-        force_color=False  # type: bool
+        force_color=False,  # type: bool
+        rom_elf_file=None,  # type: Optional[str]
     ):
         self.event_queue = queue.Queue()  # type: queue.Queue
         self.cmd_queue = queue.Queue()  # type: queue.Queue
         self.console = miniterm.Console()
         # if the variable is set ANSI will be printed even if we do not print to terminal
         sys.stderr = get_ansi_converter(sys.stderr, force_color=force_color)  # type: ignore
         self.console.output = get_ansi_converter(self.console.output, force_color=force_color)
         self.console.byte_output = get_ansi_converter(self.console.byte_output, force_color=force_color)
 
         self.elf_file = elf_file or ''
         self.elf_exists = os.path.exists(self.elf_file)
         self.logger = Logger(self.elf_file, self.console, timestamps, timestamp_format, b'', enable_address_decoding,
-                             toolchain_prefix)
+                             toolchain_prefix, rom_elf_file=rom_elf_file)
 
         self.coredump = CoreDump(decode_coredumps, self.event_queue, self.logger, websocket_client,
                                  self.elf_file) if self.elf_exists else None
 
         # allow for possibility the "make" arg is a list of arguments (for idf.py)
         self.make = make if os.path.exists(make) else shlex.split(make)  # type: Any[Union[str, List[str]], str]
         self.target = target
@@ -315,14 +317,20 @@
 
     if isinstance(args.elf_file, io.BufferedReader):
         elf_file = args.elf_file.name
         args.elf_file.close()  # don't need this as a file
     else:
         elf_file = args.elf_file
 
+    if isinstance(args.rom_elf_file, io.BufferedReader):
+        rom_elf_file = args.rom_elf_file.name
+        args.rom_elf_file.close()  # don't need this as a file
+    else:
+        rom_elf_file = args.rom_elf_file if args.rom_elf_file is not None else get_rom_elf_path(args.target, args.revision)
+
     # remove the parallel jobserver arguments from MAKEFLAGS, as any
     # parent make is only running 1 job (monitor), so we can re-spawn
     # all of the child makes we need (the -j argument remains part of
     # MAKEFLAGS)
     try:
         makeflags = os.environ[MAKEFLAGS_ENVIRON]
         makeflags = re.sub(r'--jobserver[^ =]*=[0-9,]+ ?', '', makeflags)
@@ -364,15 +372,16 @@
                       args.decode_coredumps,
                       args.decode_panic,
                       args.target,
                       ws,
                       not args.disable_address_decoding,
                       args.timestamps,
                       args.timestamp_format,
-                      args.force_color)
+                      args.force_color,
+                      rom_elf_file)
 
         yellow_print('--- Quit: {} | Menu: {} | Help: {} followed by {} ---'.format(
             key_description(monitor.console_parser.exit_key),
             key_description(monitor.console_parser.menu_key),
             key_description(monitor.console_parser.menu_key),
             key_description(CTRL_H)))
         if args.print_filter != DEFAULT_PRINT_FILTER:
```

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/PKG-INFO` & `esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.0.4
+Version: 1.1.0
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.0.4/esp_idf_monitor.egg-info/SOURCES.txt` & `esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 esp_idf_monitor/base/coredump.py
 esp_idf_monitor/base/exceptions.py
 esp_idf_monitor/base/gdbhelper.py
 esp_idf_monitor/base/line_matcher.py
 esp_idf_monitor/base/logger.py
 esp_idf_monitor/base/output_helpers.py
 esp_idf_monitor/base/pc_address_matcher.py
+esp_idf_monitor/base/rom_elf_getter.py
 esp_idf_monitor/base/serial_handler.py
 esp_idf_monitor/base/serial_reader.py
 esp_idf_monitor/base/stoppable_thread.py
 esp_idf_monitor/base/web_socket_client.py
```

### Comparing `esp-idf-monitor-1.0.4/setup.py` & `esp-idf-monitor-1.1.0/setup.py`

 * *Files identical despite different names*

