# Comparing `tmp/plover-stenograph-2.0.4.tar.gz` & `tmp/plover-stenograph-2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-stenograph-2.0.4.tar", last modified: Mon Nov 14 18:20:44 2022, max compression
+gzip compressed data, was "plover-stenograph-2.0.dev1.tar", last modified: Wed Jul 28 06:54:17 2021, max compression
```

## Comparing `plover-stenograph-2.0.4.tar` & `plover-stenograph-2.0.dev1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:20:44.096161 plover-stenograph-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-11-14 18:20:44.096161 plover-stenograph-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:20:44.096161 plover-stenograph-2.0.4/plover_stenograph/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/plover_stenograph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4387 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/plover_stenograph/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/plover_stenograph/usb.py
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/plover_stenograph/wifi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:20:44.096161 plover-stenograph-2.0.4/plover_stenograph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-11-14 18:20:44.000000 plover-stenograph-2.0.4/plover_stenograph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-11-14 18:20:44.000000 plover-stenograph-2.0.4/plover_stenograph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 18:20:44.000000 plover-stenograph-2.0.4/plover_stenograph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-14 18:20:44.000000 plover-stenograph-2.0.4/plover_stenograph.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-14 18:20:44.000000 plover-stenograph-2.0.4/plover_stenograph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-14 18:20:44.000000 plover-stenograph-2.0.4/plover_stenograph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 18:20:44.000000 plover-stenograph-2.0.4/plover_stenograph.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-11-14 18:20:44.096161 plover-stenograph-2.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       63 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 18:20:44.096161 plover-stenograph-2.0.4/stenograph/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/stenograph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/stenograph/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     5005 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/stenograph/packet.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/stenograph/stroke.py
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/stenograph/transport.py
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/stenograph/transport_libusb.py
--rw-r--r--   0 runner    (1001) docker     (121)     3542 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/stenograph/transport_wifi.py
--rw-r--r--   0 runner    (1001) docker     (121)     9511 2022-11-14 18:20:41.000000 plover-stenograph-2.0.4/stenograph/transport_windows.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 06:54:17.216223 plover-stenograph-2.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2021-07-28 06:54:17.216223 plover-stenograph-2.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 06:54:17.212222 plover-stenograph-2.0.dev1/plover_stenograph/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/plover_stenograph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3745 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/plover_stenograph/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/plover_stenograph/usb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/plover_stenograph/wifi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 06:54:17.212222 plover-stenograph-2.0.dev1/plover_stenograph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2021-07-28 06:54:17.000000 plover-stenograph-2.0.dev1/plover_stenograph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2021-07-28 06:54:17.000000 plover-stenograph-2.0.dev1/plover_stenograph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-28 06:54:17.000000 plover-stenograph-2.0.dev1/plover_stenograph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-07-28 06:54:17.000000 plover-stenograph-2.0.dev1/plover_stenograph.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-07-28 06:54:17.000000 plover-stenograph-2.0.dev1/plover_stenograph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-07-28 06:54:17.000000 plover-stenograph-2.0.dev1/plover_stenograph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-28 06:54:17.000000 plover-stenograph-2.0.dev1/plover_stenograph.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2021-07-28 06:54:17.216223 plover-stenograph-2.0.dev1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)       63 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-28 06:54:17.216223 plover-stenograph-2.0.dev1/stenograph/
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/stenograph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      802 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/stenograph/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4910 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/stenograph/packet.py
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/stenograph/stroke.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/stenograph/transport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2857 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/stenograph/transport_libusb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3467 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/stenograph/transport_wifi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9541 2021-07-28 06:54:16.000000 plover-stenograph-2.0.dev1/stenograph/transport_windows.py
```

### Comparing `plover-stenograph-2.0.4/PKG-INFO` & `plover-stenograph-2.0.dev1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: plover-stenograph
-Version: 2.0.4
+Version: 2.0.dev1
 Summary: Plover plugin for Stenograph machines
-Home-page: https://github.com/sammdot/plover-stenograph
+Home-page: UNKNOWN
+License: UNKNOWN
+Description: # Plover Stenograph
+        
+        A Plover plugin for using newer Stenograph machines (Stentura Protégé and
+        Fusion, Élan Mira and Cybra, Diamanté, Wave, Luminex) connected to the computer
+        over USB or Wi-Fi.
+        
+        This is a work-in-progress rewrite of the
+        [plover-stenograph-usb](https://github.com/morinted/plover_stenograph_usb) and
+        [plover-stenograph-wifi](https://github.com/stanographer/plover_stenograph_wifi)
+        plugins to reuse code and add more protocol functionality.
+        
 Keywords: plover plover_plugin
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
-
-# Plover Stenograph
-
-A Plover plugin for using newer Stenograph machines (Stentura Protégé and
-Fusion, Élan Mira and Cybra, Diamanté, Wave, Luminex) connected to the computer
-over USB or Wi-Fi.
-
-This is a work-in-progress rewrite of the
-[plover-stenograph-usb](https://github.com/morinted/plover_stenograph_usb) and
-[plover-stenograph-wifi](https://github.com/stanographer/plover_stenograph_wifi)
-plugins to reuse code and add more protocol functionality.
```

### Comparing `plover-stenograph-2.0.4/plover_stenograph/base.py` & `plover-stenograph-2.0.dev1/plover_stenograph/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from plover import log
 from plover.machine.base import ThreadedStenotypeBase
 
 from stenograph import *
-from time import sleep
-
 
 class StenographMachine(ThreadedStenotypeBase):
 
     KEYS_LAYOUT = """
         #  #  #  #  #  #  #  #  #  #
         S- T- P- H- * -F -P -L -T -D
         S- K- W- R- * -R -B -G -S -Z
@@ -32,31 +30,29 @@
             self._transport.connect()
         except ConnectionError as e:
             log.error("Stenograph writer is not connected: %s" % e)
             self._error()
         except IOError as e:
             log.error("Lost connection to Stenograph writer: %s" % e)
             self._error()
-        except Exception as e:
-            log.error("Error connecting to Stenograph writer: %s" % e)
-            self._error()
         else:
             self._ready()
             self.start()
 
     def _reconnect(self):
         self._error()
         while not self.finished.wait(0.25):
             try:
                 self._initializing()
                 self._transport.connect()
             except Exception as e:
                 log.debug("Stenograph writer exception: %s" % e)
                 self._error()
             else:
+                self._ready()
                 break
 
     def _send_receive(self, request):
         """Send a StenoPacket and return the response or raise exceptions."""
         log.debug("Requesting from Stenograph writer: %s", request)
         response = self._transport.send_receive(request)
         log.debug("Response from Stenograph writer: %s", response)
@@ -71,55 +67,43 @@
                 self.offset = 0  # File offset to read from
 
             def reset(self):
                 self.__init__()
 
         state = ReadState()
 
-        # Tracks whether the machine *just* disconnected, or has been disconnected
-        # for a while, to prevent showing the warning more times than needed.
-        disconnected = False
-
         while not self.finished.isSet():
             try:
                 if not state.realtime_file_open:
                     # Open realtime file
                     self._send_receive(StenoPacket.make_open_request())
                     state.realtime_file_open = True
                 response = self._send_receive(
                     StenoPacket.make_read_request(file_offset=state.offset)
                 )
             except ConnectionError as e:
-                if not disconnected:
-                    log.warning("Stenograph writer disconnected, attempting to reconnect")
-                    disconnected = True
+                log.warning("Stenograph writer disconnected, reconnecting...")
                 log.debug("Stenograph writer exception: %s", e)
                 # User could start a new file while disconnected.
                 state.reset()
                 self._reconnect()
             except NoRealtimeFileException:
                 # User hasn"t started writing, just keep opening the realtime file
                 state.reset()
             except FinishedReadingClosedFileException:
                 # File closed! Open the realtime file.
                 state.reset()
             else:
-                if disconnected:
-                    log.warning("Stenograph writer reconnected")
-                    self._ready()
-                    disconnected = False
                 if response.data_length:
                     state.offset += response.data_length
                 elif not state.realtime:
                     state.realtime = True
                 if response.data_length and state.realtime:
                     for stroke in response.strokes():
                         self._on_stroke(stroke.keys)
-                if state.realtime:
-                    sleep(0.10)
 
         self._transport.disconnect()
 
     def stop_capture(self):
         super().stop_capture()
         self._transport = None
         self._stopped()
```

### Comparing `plover-stenograph-2.0.4/plover_stenograph.egg-info/PKG-INFO` & `plover-stenograph-2.0.dev1/plover_stenograph.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: plover-stenograph
-Version: 2.0.4
+Version: 2.0.dev1
 Summary: Plover plugin for Stenograph machines
-Home-page: https://github.com/sammdot/plover-stenograph
+Home-page: UNKNOWN
+License: UNKNOWN
+Description: # Plover Stenograph
+        
+        A Plover plugin for using newer Stenograph machines (Stentura Protégé and
+        Fusion, Élan Mira and Cybra, Diamanté, Wave, Luminex) connected to the computer
+        over USB or Wi-Fi.
+        
+        This is a work-in-progress rewrite of the
+        [plover-stenograph-usb](https://github.com/morinted/plover_stenograph_usb) and
+        [plover-stenograph-wifi](https://github.com/stanographer/plover_stenograph_wifi)
+        plugins to reuse code and add more protocol functionality.
+        
 Keywords: plover plover_plugin
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
-
-# Plover Stenograph
-
-A Plover plugin for using newer Stenograph machines (Stentura Protégé and
-Fusion, Élan Mira and Cybra, Diamanté, Wave, Luminex) connected to the computer
-over USB or Wi-Fi.
-
-This is a work-in-progress rewrite of the
-[plover-stenograph-usb](https://github.com/morinted/plover_stenograph_usb) and
-[plover-stenograph-wifi](https://github.com/stanographer/plover_stenograph_wifi)
-plugins to reuse code and add more protocol functionality.
```

### Comparing `plover-stenograph-2.0.4/plover_stenograph.egg-info/SOURCES.txt` & `plover-stenograph-2.0.dev1/plover_stenograph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.0.4/setup.cfg` & `plover-stenograph-2.0.dev1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 [metadata]
 name = plover-stenograph
-version = 2.0.4
+version = 2.0-dev1
 description = Plover plugin for Stenograph machines
 long_description = file:README.md
 long_description_content_type = text/markdown
-home_page = https://github.com/sammdot/plover-stenograph
 keywords = plover plover_plugin
 classifiers = 
 	Programming Language :: Python :: 3.9
 
 [options]
 zip_safe = True
 setup_requires = 
 	setuptools>=30.3.0
 install_requires = 
 	plover>=4.0.0.dev10
-	more_itertools>=6.0.0
-	pyusb>=1.0.0  ; platform_system != "Windows"
-	pyusb_libusb1_backend  ; platform_system != "Windows"
+	more_itertools
+	pyusb>=1.0.0  ; platform_system!="Windows"
 packages = 
 	stenograph
 	plover_stenograph
 
 [options.entry_points]
 plover.machine = 
 	Stenograph USB = plover_stenograph:StenographUsb
```

### Comparing `plover-stenograph-2.0.4/stenograph/exception.py` & `plover-stenograph-2.0.dev1/stenograph/exception.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 class ConnectionError(Exception):
     """We could not connect to the writer."""
     pass
 
+
+class TransportError(Exception):
+    """We could not read from or write to the writer"""
+    pass
+
+
 class ProtocolViolationException(Exception):
     """The writer did something unexpected"""
     pass
 
 
 class UnableToPerformRequestException(Exception):
     """The writer cannot perform the action requested"""
```

### Comparing `plover-stenograph-2.0.4/stenograph/packet.py` & `plover-stenograph-2.0.dev1/stenograph/packet.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,23 +132,19 @@
             p2=byte_count,
         )
 
     @property
     def is_error(self):
         return self.packet_type == PacketType.ERROR
 
-    @property
-    def is_ok(self):
-        return self.packet_type == PacketType.OK
-
     def strokes(self):
         """Get list of strokes represented in this packet's data"""
 
         # Expecting 8-byte chords (4 bytes of steno, 4 of timestamp.)
         assert self.data_length % 8 == 0
         # Steno should only be present on ACTION_READ packets
         assert self.packet_type == PacketType.READ_FILE
 
         return [
             Stroke.unpack(stroke_data)
-            for stroke_data in grouper(self.data, 8, fillvalue=0)
+            for stroke_data in grouper(8, self.data, 0)
         ]
```

### Comparing `plover-stenograph-2.0.4/stenograph/stroke.py` & `plover-stenograph-2.0.dev1/stenograph/stroke.py`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.0.4/stenograph/transport.py` & `plover-stenograph-2.0.dev1/stenograph/transport.py`

 * *Files identical despite different names*

### Comparing `plover-stenograph-2.0.4/stenograph/transport_libusb.py` & `plover-stenograph-2.0.dev1/stenograph/transport_libusb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from usb import core, util
-from pyusb_libusb1_backend import get_pyusb_backend
 
 from stenograph.transport import MachineTransport
 from stenograph.packet import MAX_READ, StenoPacket
 from stenograph.exception import ProtocolViolationException, ConnectionError
 
 
 VENDOR_ID = 0x112b
@@ -13,24 +12,23 @@
 
     def __init__(self):
         super().__init__()
         self._usb_device = None
         self._endpoint_in = None
         self._endpoint_out = None
         self._connected = False
-        self._backend = get_pyusb_backend()
 
     def connect(self):
         """Attempt to and return connection"""
         # Disconnect device if it's already connected.
         if self._connected:
             self.disconnect()
 
         # Find the device by the vendor ID.
-        usb_device = core.find(backend=self._backend, idVendor=VENDOR_ID)
+        usb_device = core.find(idVendor=VENDOR_ID)
         if not usb_device:  # Device not found
             raise ConnectionError("USB device not connected")
 
         # Copy the default configuration.
         usb_device.set_configuration()
         config = usb_device.get_active_configuration()
         interface = config[(0, 0)]
```

### Comparing `plover-stenograph-2.0.4/stenograph/transport_wifi.py` & `plover-stenograph-2.0.dev1/stenograph/transport_wifi.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,12 +86,11 @@
             response = self._sock.recv(MAX_READ + StenoPacket.HEADER_SIZE)
         except Exception as e:
             raise ConnectionError(e)
         else:
             if response and len(response) >= StenoPacket.HEADER_SIZE:
                 writer_packet = StenoPacket.unpack(response)
                 if (writer_packet.sequence_number == request.sequence_number and
-                    (writer_packet.packet_type == request.packet_type or
-                        writer_packet.is_error or writer_packet.is_ok)):
+                    writer_packet.packet_type == request.packet_type):
                     return self.handle_response(writer_packet)
                 raise ProtocolViolationException()
             raise ConnectionError("No response from writer")
```

### Comparing `plover-stenograph-2.0.4/stenograph/transport_windows.py` & `plover-stenograph-2.0.dev1/stenograph/transport_windows.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ctypes import windll, wintypes
 import ctypes
 import uuid
 
 from stenograph.transport import MachineTransport
 from stenograph.packet import MAX_READ, StenoPacket
-from stenograph.exception import ProtocolViolationException, ConnectionError, ConnectionError
+from stenograph.exception import ProtocolViolationException, ConnectionError, TransportError
 
 GUID = wintypes.BYTE * 16
 HDEVINFO = wintypes.HANDLE
 
 LPOVERLAPPED = wintypes.LPVOID
 LPSECURITY_ATTRIBUTES = wintypes.LPVOID
 PSP_DEVINFO_DATA = wintypes.LPVOID
@@ -142,109 +142,110 @@
         dev_interface_data.cbSize = ctypes.sizeof(SP_DEVICE_INTERFACE_DATA)
 
         if not SetupDiEnumDeviceInterfaces(
             device_info, None, ctypes.byref(guid),
             0, ctypes.byref(dev_interface_data)
         ):
             if ctypes.GetLastError() != ERROR_NO_MORE_ITEMS:
-                raise ConnectionError('SetupDiEnumDeviceInterfaces: %s' % ctypes.WinError())
+                raise ConnectionError('SetupDiEnumDeviceInterfaces: %s', ctypes.WinError())
             return INVALID_HANDLE_VALUE
 
         request_length = wintypes.DWORD(0)
         status = SetupDiGetDeviceInterfaceDetail(
             device_info,
             ctypes.byref(dev_interface_data),
             # Call with (None, 0) to see how big a buffer is needed.
             None, 0,
             ctypes.pointer(request_length),
             None,
         )
         if status or ctypes.GetLastError() != ERROR_INSUFFICIENT_BUFFER:
-            raise ConnectionError('last error not insufficient buffer: %s' % ctypes.WinError())
+            raise ConnectionError('last error not insufficient buffer: %s', ctypes.WinError())
 
         dev_detail_data_buffer = ctypes.create_string_buffer(request_length.value)
         dev_detail_data_ptr = ctypes.cast(dev_detail_data_buffer, PSP_DEVICE_INTERFACE_DETAIL_DATA_A)
         dev_detail_data_ptr[0].cbSize = ctypes.sizeof(SP_DEVICE_INTERFACE_DETAIL_DATA_A)
 
         # Now put the actual detail data into the buffer
         if not SetupDiGetDeviceInterfaceDetail(
             device_info,
             ctypes.byref(dev_interface_data),
             dev_detail_data_ptr,
             ctypes.sizeof(dev_detail_data_buffer),
             None,
             None,
         ):
-            raise ConnectionError('SetupDiGetDeviceInterfaceDetail: %s' % ctypes.WinError())
+            raise ConnectionError('SetupDiGetDeviceInterfaceDetail: %s', ctypes.WinError())
 
         device_path = dev_detail_data_ptr[0].DevicePath
 
+        raise ConnectionError('okay, creating file, device path: %s', device_path)
+
         handle = CreateFile(device_path,
                             GENERIC_READ | GENERIC_WRITE,
                             FILE_SHARE_READ | FILE_SHARE_WRITE,
                             None,
                             CREATE_ALWAYS | CREATE_NEW,
                             FILE_ATTRIBUTE_NORMAL,
                             None)
         if handle == INVALID_HANDLE_VALUE:
-            raise ConnectionError('CreateFile: %s' % ctypes.WinError())
+            raise ConnectionError('CreateFile: %s', ctypes.WinError())
         return handle
 
     @staticmethod
     def _open_device_by_class_interface_and_instance(class_guid):
         device_info = SetupDiGetClassDevs(ctypes.byref(class_guid), None, None,
                                           DIGCF_DEVICEINTERFACE | DIGCF_PRESENT)
         if device_info == INVALID_HANDLE_VALUE:
-            raise ConnectionError('SetupDiGetClassDevs: %s' % ctypes.WinError())
-        usb_device = WindowsUsbTransport._open_device_instance(device_info, class_guid)
+            raise ConnectionError('SetupDiGetClassDevs: %s', ctypes.WinError())
+        usb_device = StenographMachine._open_device_instance(device_info, class_guid)
         if not SetupDiDestroyDeviceInfoList(device_info):
-            raise ConnectionError('SetupDiDestroyDeviceInfoList: %s' % ctypes.WinError())
+            raise ConnectionError('SetupDiDestroyDeviceInfoList: %s', ctypes.WinError())
         return usb_device
 
     def _usb_write_packet(self, request):
         bytes_written = wintypes.DWORD(0)
         request_packet = request.pack()
         if not WriteFile(self._usb_device,
                          request_packet,
                          StenoPacket.HEADER_SIZE + request.data_length,
                          ctypes.byref(bytes_written),
                          None):
-            raise ConnectionError('WriteFile: %s' % ctypes.WinError())
+            raise TransportError('WriteFile: %s', ctypes.WinError())
         return bytes_written.value
 
     def _usb_read_packet(self):
         bytes_read = wintypes.DWORD(0)
         if not ReadFile(self._usb_device,
                         self._read_buffer,
                         MAX_READ + StenoPacket.HEADER_SIZE,
                         ctypes.byref(bytes_read),
                         None):
-            raise ConnectionError('ReadFile: %s' % ctypes.WinError())
+            raise TransportError('ReadFile: %s', ctypes.WinError())
         if bytes_read.value < StenoPacket.HEADER_SIZE:
-            raise ConnectionError('ReadFile: short read, %u < %u',
+            raise TransportError('ReadFile: short read, %u < %u',
                       bytes_read.value, StenoPacket.HEADER_SIZE)
         writer_packet = StenoPacket.unpack(self._read_buffer)
         return writer_packet
 
     def disconnect(self):
         self._usb_device = INVALID_HANDLE_VALUE
         if not CloseHandle(self._usb_device):
-            raise ConnectionError('CloseHandle: %s' % ctypes.WinError())
+            raise ConnectionError('CloseHandle: %s', ctypes.WinError())
 
     def connect(self):
         # If already connected, disconnect first.
         if self._usb_device != INVALID_HANDLE_VALUE:
             self.disconnect()
         self._usb_device = self._open_device_by_class_interface_and_instance(USB_WRITER_GUID)
         return self._usb_device != INVALID_HANDLE_VALUE
 
     def send_receive(self, request):
-        if self._usb_device == INVALID_HANDLE_VALUE:
-            raise ConnectionError("USB device is not open")
+        assert self._usb_device != INVALID_HANDLE_VALUE, 'device not open'
         written = self._usb_write_packet(request)
         if written < StenoPacket.HEADER_SIZE:
-            raise ConnectionError("Could not write to USB device")
+            raise TransportError("Could not write to USB device")
         writer_packet = self._usb_read_packet()
         if (writer_packet.sequence_number == request.sequence_number and
             writer_packet.packet_type == request.packet_type):
             return self.handle_response(writer_packet)
         raise ProtocolViolationException()
```

