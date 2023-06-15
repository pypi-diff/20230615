# Comparing `tmp/me_setups-1.8.4.tar.gz` & `tmp/me_setups-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_setups-1.8.4.tar", last modified: Wed Jun 14 18:10:34 2023, max compression
+gzip compressed data, was "me_setups-1.8.5.tar", last modified: Thu Jun 15 09:32:27 2023, max compression
```

## Comparing `me_setups-1.8.4.tar` & `me_setups-1.8.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 18:10:34.239925 me_setups-1.8.4/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-14 18:10:34.239934 me_setups-1.8.4/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.4/README.md
--rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-14 18:10:34.241923 me_setups-1.8.4/setup.cfg
--rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.4/setup.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 18:10:34.207632 me_setups-1.8.4/src/
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 18:10:34.221827 me_setups-1.8.4/src/me_setups/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.4/src/me_setups/__init__.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 18:10:34.228936 me_setups-1.8.4/src/me_setups/boards/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.4/src/me_setups/boards/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.4/src/me_setups/boards/default_boards.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    11657 2023-06-04 13:52:01.000000 me_setups-1.8.4/src/me_setups/boards/gas52.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.4/src/me_setups/boards/types.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 18:10:34.243554 me_setups-1.8.4/src/me_setups/components/
--rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.4/src/me_setups/components/__init__.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     8688 2023-06-14 18:10:00.000000 me_setups-1.8.4/src/me_setups/components/comp.py
--rw-r--r--   0 idof     (12090585) develop   (1000)    12933 2023-06-04 13:52:01.000000 me_setups-1.8.4/src/me_setups/components/eqs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.4/src/me_setups/components/mcs.py
--rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.4/src/me_setups/components/mcu.py
--rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-06-06 17:26:44.000000 me_setups-1.8.4/src/me_setups/utils.py
-drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-14 18:10:34.223922 me_setups-1.8.4/src/me_setups.egg-info/
--rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-14 18:10:34.000000 me_setups-1.8.4/src/me_setups.egg-info/PKG-INFO
--rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-14 18:10:34.000000 me_setups-1.8.4/src/me_setups.egg-info/SOURCES.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-14 18:10:34.000000 me_setups-1.8.4/src/me_setups.egg-info/dependency_links.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-14 18:10:34.000000 me_setups-1.8.4/src/me_setups.egg-info/requires.txt
--rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-14 18:10:34.000000 me_setups-1.8.4/src/me_setups.egg-info/top_level.txt
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.425586 me_setups-1.8.5/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-15 09:32:27.425643 me_setups-1.8.5/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)       19 2023-01-29 18:05:41.000000 me_setups-1.8.5/README.md
+-rw-r--r--   0 idof     (12090585) develop   (1000)     1242 2023-06-15 09:32:27.428591 me_setups-1.8.5/setup.cfg
+-rw-r--r--   0 idof     (12090585) develop   (1000)       74 2023-01-29 18:02:02.000000 me_setups-1.8.5/setup.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.372950 me_setups-1.8.5/src/
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.387617 me_setups-1.8.5/src/me_setups/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-29 21:40:13.000000 me_setups-1.8.5/src/me_setups/__init__.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.410119 me_setups-1.8.5/src/me_setups/boards/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-02-15 14:02:28.000000 me_setups-1.8.5/src/me_setups/boards/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      920 2023-03-12 12:03:35.000000 me_setups-1.8.5/src/me_setups/boards/default_boards.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    11657 2023-06-04 13:52:01.000000 me_setups-1.8.5/src/me_setups/boards/gas52.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      119 2023-02-16 19:57:32.000000 me_setups-1.8.5/src/me_setups/boards/types.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.420883 me_setups-1.8.5/src/me_setups/components/
+-rw-r--r--   0 idof     (12090585) develop   (1000)        0 2023-01-30 07:57:12.000000 me_setups-1.8.5/src/me_setups/components/__init__.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     8532 2023-06-15 09:29:46.000000 me_setups-1.8.5/src/me_setups/components/comp.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)    12933 2023-06-04 13:52:01.000000 me_setups-1.8.5/src/me_setups/components/eqs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      198 2023-05-18 10:10:02.000000 me_setups-1.8.5/src/me_setups/components/mcs.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)     4187 2023-05-18 10:10:02.000000 me_setups-1.8.5/src/me_setups/components/mcu.py
+-rw-r--r--   0 idof     (12090585) develop   (1000)      488 2023-06-06 17:26:44.000000 me_setups-1.8.5/src/me_setups/utils.py
+drwxr-xr-x   0 idof     (12090585) develop   (1000)        0 2023-06-15 09:32:27.398644 me_setups-1.8.5/src/me_setups.egg-info/
+-rw-r--r--   0 idof     (12090585) develop   (1000)      586 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/PKG-INFO
+-rw-r--r--   0 idof     (12090585) develop   (1000)      559 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)        1 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       66 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/requires.txt
+-rw-r--r--   0 idof     (12090585) develop   (1000)       10 2023-06-15 09:32:27.000000 me_setups-1.8.5/src/me_setups.egg-info/top_level.txt
```

### Comparing `me_setups-1.8.4/PKG-INFO` & `me_setups-1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_setups
-Version: 1.8.4
+Version: 1.8.5
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.4/setup.cfg` & `me_setups-1.8.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = me_setups
-version = 1.8.4
+version = 1.8.5
 description = Abstraction for Mobileye setups.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://gitlab.mobileye.com/idof/me-setups
 author = Ido Frenkel
 author_email = ido.frenkel@mobileye.com
 classifiers =
```

### Comparing `me_setups-1.8.4/src/me_setups/boards/default_boards.py` & `me_setups-1.8.5/src/me_setups/boards/default_boards.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.4/src/me_setups/boards/gas52.py` & `me_setups-1.8.5/src/me_setups/boards/gas52.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.4/src/me_setups/components/comp.py` & `me_setups-1.8.5/src/me_setups/components/comp.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,32 +84,29 @@
         """
         super().__init__(*args, **kwargs)
         self.daemon = True
         self.serial = serial
         self.alive = threading.Event()
 
     def stop(self) -> None:
-        """\
-            Stop sniffing
-        """
+        """Stop sniffing"""
         self.alive.clear()
 
     def run(self) -> None:
         self.alive.set()
         while self.alive.is_set() and self.serial.is_open:
             try:
                 self.serial.read(self.serial.in_waiting or 1)
             except SerialException:  # pragma: no cover
                 break
             except OSError:  # pragma: no cover
                 self.serial.close()
                 self.serial.open()
                 self.serial.read(self.serial.in_waiting or 1)
-        if self.alive.is_set():  # pragma: no cover
-            self.alive.clear()
+        self.alive.clear()
 
 
 class SerialSniffer(Serial):
     timeout: float
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """\
@@ -151,32 +148,30 @@
 
     def start_sniffing(self) -> ReaderThread:
         """start the sniffing thread
 
         Returns:
             ReaderThread: The sniffing thread
         """
-        if not self.sniff_thread.is_alive():  # pragma: no cover
+        if not self.sniff_thread.is_alive():
             self.sniff_thread = ReaderThread(self)
         self.sniff_thread.start()
         return self.sniff_thread
 
     def stop_sniffing(self) -> None:
-        """\
-            Stops the Sniffing thread
-        """
-        if self.sniff_thread.alive.is_set():  # pragma: no cover
-            self.sniff_thread.stop()
+        """Stops the Sniffing thread"""
+        self.sniff_thread.stop()
 
         self.sniff_thread.join(10)
         if self.sniff_thread.is_alive():
             raise RuntimeError("stop sniffing fail!")  # pragma: no cover
 
         if self.protocol.log_file is not None:
             self.protocol.log_file.close()
+            self.protocol.log_file = None
 
     def config_sniffer(
         self,
         *,
         clean_line: bool = True,
         add_timestamp: bool = True,
     ) -> None:  # pragma: no cover
@@ -244,18 +239,18 @@
     ) -> None:
         """config log file for the sniffer.
 
         Args:
             log_file (pathlib.Path | str): path for the log file.
             mode (Literal['w', 'a'], optional): like open(). Defaults to 'a'.
         """
-        if self.serial.sniff_thread.alive.is_set():  # pragma: no cover
+        if self.serial.sniff_thread.alive.is_set():
             self.serial.stop_sniffing()
-            assert self.serial.protocol.log_file
-            self.serial.protocol.log_file.close()
+            if self.serial.protocol.log_file is not None:
+                self.serial.protocol.log_file.close()
 
         self.logger.debug(f"configuring log file for serial - {str(log_file)!r}")
         log_file = pathlib.Path(log_file)
         log_file.parent.mkdir(parents=True, exist_ok=True)
         self.serial.protocol.log_file = log_file.open(mode, buffering=1)
 
     def wait_for_msg(self, msg: bytes, timeout: float) -> bytes:
```

### Comparing `me_setups-1.8.4/src/me_setups/components/eqs.py` & `me_setups-1.8.5/src/me_setups/components/eqs.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.4/src/me_setups/components/mcu.py` & `me_setups-1.8.5/src/me_setups/components/mcu.py`

 * *Files identical despite different names*

### Comparing `me_setups-1.8.4/src/me_setups.egg-info/PKG-INFO` & `me_setups-1.8.5/src/me_setups.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me-setups
-Version: 1.8.4
+Version: 1.8.5
 Summary: Abstraction for Mobileye setups.
 Home-page: http://gitlab.mobileye.com/idof/me-setups
 Author: Ido Frenkel
 Author-email: ido.frenkel@mobileye.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `me_setups-1.8.4/src/me_setups.egg-info/SOURCES.txt` & `me_setups-1.8.5/src/me_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

