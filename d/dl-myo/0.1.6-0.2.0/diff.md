# Comparing `tmp/dl_myo-0.1.6.tar.gz` & `tmp/dl_myo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_myo-0.1.6.tar", max compression
+gzip compressed data, was "dl_myo-0.2.0.tar", max compression
```

## Comparing `dl_myo-0.1.6.tar` & `dl_myo-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    35131 2023-06-13 18:39:07.020525 dl_myo-0.1.6/LICENSE
--rw-r--r--   0        0        0     2514 2023-06-13 18:39:07.020525 dl_myo-0.1.6/README.md
--rw-r--r--   0        0        0      455 2023-06-13 18:39:07.020525 dl_myo-0.1.6/myo/__init__.py
--rw-r--r--   0        0        0     3226 2023-06-13 18:39:07.020525 dl_myo-0.1.6/myo/commands.py
--rw-r--r--   0        0        0     6562 2023-06-13 18:39:07.020525 dl_myo-0.1.6/myo/device.py
--rw-r--r--   0        0        0     6485 2023-06-13 18:39:07.024525 dl_myo-0.1.6/myo/handle.py
--rw-r--r--   0        0        0     9457 2023-06-13 18:39:07.024525 dl_myo-0.1.6/myo/types.py
--rw-r--r--   0        0        0     3140 2023-06-13 18:39:28.676804 dl_myo-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 dl_myo-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35131 2023-06-14 22:05:38.798261 dl_myo-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2514 2023-06-14 22:05:38.798261 dl_myo-0.2.0/README.md
+-rw-r--r--   0        0        0     7012 2023-06-14 22:05:38.802261 dl_myo-0.2.0/myo/__init__.py
+-rw-r--r--   0        0        0     3226 2023-06-14 22:05:38.802261 dl_myo-0.2.0/myo/commands.py
+-rw-r--r--   0        0        0     5783 2023-06-14 22:05:38.802261 dl_myo-0.2.0/myo/handle.py
+-rw-r--r--   0        0        0     9499 2023-06-14 22:05:38.802261 dl_myo-0.2.0/myo/types.py
+-rw-r--r--   0        0        0     3194 2023-06-14 22:05:57.490298 dl_myo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 dl_myo-0.2.0/PKG-INFO
```

### Comparing `dl_myo-0.1.6/LICENSE` & `dl_myo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.6/README.md` & `dl_myo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.6/myo/commands.py` & `dl_myo-0.2.0/myo/commands.py`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.6/myo/device.py` & `dl_myo-0.2.0/myo/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,197 +1,224 @@
 # -*- coding: utf-8 -*-
+"""
+    Top-level package for dl-myo
+~~~~~~~~~~~~~~~~~~~~
+   >>> import myo
+"""
+
 from __future__ import annotations
 
+__author__ = """Iori Mizutani"""
+__email__ = "iori.mizutani@gmail.com"
+
+from pkgutil import extend_path
+
+__path__ = extend_path(__path__, __name__)
+
 import binascii
 import json
 import logging
 
 from bleak import BleakClient, BleakScanner
 from bleak.backends.characteristic import BleakGATTCharacteristic
 from bleak.backends.device import BLEDevice
 from bleak.backends.scanner import AdvertisementData
 
+
 from .commands import (
     Command,
     SetMode,
     Vibrate,
     DeepSleep,
     LED,
     Vibrate2,
     SetSleepMode,
     Unlock,
     UserAction,
 )
 from .handle import Handle, UUID
 from .types import FirmwareInfo, FirmwareVersion
 
-# from .quaternion import Quaternion
-
 logger = logging.getLogger(__name__)
 
 
-class Device:
-    __slots__ = ("__device", "__name")
+class Myo:
+    __slots__ = ("_client", "_device")
 
     def __init__(self):
         pass
 
     @property
-    def device(self) -> BLEDevice:
-        return self.__device
+    def client(self) -> BleakClient:
+        return self._client
 
     @property
-    def name(self) -> str:
-        return self.__name
+    def device(self) -> BLEDevice:
+        return self._device
 
     @classmethod
-    async def with_mac(cls, mac: str) -> Device:
+    async def with_mac(cls, mac: str) -> Myo:
         def match_myo_mac(device: BLEDevice, _: AdvertisementData):
             if mac.lower() == device.address.lower():
                 return True
             return False
 
         self = cls()
         try:
             # scan the device
-            self.__device = await BleakScanner.find_device_by_filter(match_myo_mac, cb=dict(use_bdaddr=True))
+            self._device = await BleakScanner.find_device_by_filter(match_myo_mac, cb=dict(use_bdaddr=True))
             if self.device is None:
                 logger.error(f"could not find device with address {mac}")
-                return self
+                return None
         except Exception as e:
             logger.error("the mac address may be invalid", e)
-            return self
-
-        # get the device name
-        self.__name = str(self.device.name)
+            return None
 
+        await self.connect()
         return self
 
     @classmethod
-    async def with_uuid(cls) -> Device:
+    async def with_uuid(cls) -> Myo:
         def match_myo_uuid(_: BLEDevice, adv: AdvertisementData):
             if str(UUID.MYO_SERVICE).lower() in adv.service_uuids:
                 return True
             return False
 
         self = cls()
         # scan the device
-        self.__device = await BleakScanner.find_device_by_filter(match_myo_uuid, cb=dict(use_bdaddr=True))
+        self._device = await BleakScanner.find_device_by_filter(match_myo_uuid, cb=dict(use_bdaddr=True))
         if self.device is None:
             logger.error(f"could not find device with service UUID {UUID.MYO_SERVICE}")
-            return self
-
-        # get the device name
-        self.__name = str(self.device.name)
+            return None
 
+        await self.connect()
         return self
 
-    async def battery_level(self, client: BleakClient):
+    async def battery_level(self):
         """
         Battery Level Characteristic
         """
-        val = await client.read_gatt_char(Handle.BATTERY_LEVEL)
+        val = await self.client.read_gatt_char(Handle.BATTERY_LEVEL.value)
         return ord(val)
 
-    async def command(self, client: BleakClient, cmd: Command):
+    async def command(self, cmd: Command):
         """
         Command Characteristic
         """
-        await client.write_gatt_char(Handle.COMMAND.value, cmd.data, True)
+        await self.client.write_gatt_char(Handle.COMMAND.value, cmd.data, True)
+
+    async def connect(self):
+        self._client = BleakClient(self.device)
+        if self.client is None:
+            logger.error("connection failed")
+            return None
+
+        # connect to the device
+        await self.client.connect()
+        logger.info(f"connected to {self.device.name}")
 
     async def deep_sleep(self, client: BleakClient):
         """
         Deep Sleep Command
         """
         await self.command(client, DeepSleep())
 
-    async def get_services(self, client: BleakClient, indent=2) -> str:
+    async def disconnect(self):
+        if self.client is None:
+            logger.error("connection is already closed")
+
+        # disconnect from the device
+        await self.client.disconnect()
+        self._client = None
+        logger.info(f"disconnected from {self.device.name}")
+
+    async def get_services(self, indent=2) -> str:
         """fetch available services as dict"""
         sd = {}
-        for service in client.services:  # BleakGATTServiceCollection
+        for service in self.client.services:  # BleakGATTServiceCollection
             try:
                 service_name = Handle(service.handle).name
             except Exception as e:
                 logger.debug("unknown handle: {}", e)
                 continue
 
             chars = {}
             for char in service.characteristics:  # List[BleakGATTCharacteristic]
-                cd = await gatt_char_to_dict(client, char)
+                cd = await gatt_char_to_dict(self.client, char)
                 if cd:
                     chars[hex(char.handle)] = cd
 
             # end char
             sd[hex(service.handle)] = {
                 "name": service_name,
                 "uuid": service.uuid,
                 "chars": chars,
             }
         # end service
         return json.dumps({"services": sd}, indent=indent)
 
-    async def led(self, client: BleakClient, *args):
+    async def led(self, *args):
         """
         LED Command
             - set leds color
 
         *args: [logoR, logoG, logoB], [lineR, lineG, lineB]
         """
 
         if not isinstance(args, tuple) or len(args) != 2:
             raise Exception(f"Unknown payload for LEDs: {args}")
 
         for lst in args:
             if any(not isinstance(v, int) for v in lst):
                 raise Exception(f"Values must be int 0-255: {lst}")
 
-        await self.command(client, LED(args[0], args[1]))
+        await self.command(LED(args[0], args[1]))
 
-    async def set_mode(self, client: BleakClient, emg_mode, imu_mode, classifier_mode):
+    async def set_mode(self, emg_mode, imu_mode, classifier_mode):
         """
         Set Mode Command
             - configures EMG, IMU, and Classifier modes
         """
-        await self.command(client, SetMode(emg_mode, imu_mode, classifier_mode))
+        await self.command(SetMode(emg_mode, imu_mode, classifier_mode))
 
-    async def set_sleep_mode(self, client: BleakClient, sleep_mode):
+    async def set_sleep_mode(self, sleep_mode):
         """
         Set Sleep Mode Command
         """
-        await self.command(client, SetSleepMode(sleep_mode))
+        await self.command(SetSleepMode(sleep_mode))
 
-    async def unlock(self, client: BleakClient, unlock_type):
+    async def unlock(self, unlock_type):
         """
         Unlock Command
         """
-        await self.command(client, Unlock(unlock_type))
+        await self.command(Unlock(unlock_type))
 
-    async def user_action(self, client: BleakClient, user_action_type):
+    async def user_action(self, user_action_type):
         """
         User Action Command
         """
-        await self.command(client, UserAction(user_action_type))
+        await self.command(UserAction(user_action_type))
 
-    async def vibrate(self, client: BleakClient, vibration_type):
+    async def vibrate(self, vibration_type):
         """
         Vibrate Command
         """
-        await self.command(client, Vibrate(vibration_type))
+        await self.command(Vibrate(vibration_type))
 
-    async def vibrate2(self, client: BleakClient, duration, strength):
+    async def vibrate2(self, duration, strength):
         """
         Vibrate2 Command
         """
-        await self.command(client, Vibrate2(duration, strength))
+        await self.command(Vibrate2(duration, strength))
 
-    async def write(self, client, handle, value):
+    async def write(self, handle, value):
         """
         Write characteristic
         """
-        await client.write_gatt_char(handle, value, True)
+        await self.client.write_gatt_char(handle, value, True)
 
 
 async def gatt_char_to_dict(client: BleakClient, char: BleakGATTCharacteristic):
     try:
         char_name = Handle(char.handle).name
     except Exception as e:
         logger.debug("unknown handle: {}", e)
```

### Comparing `dl_myo-0.1.6/myo/handle.py` & `dl_myo-0.2.0/myo/handle.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,42 @@
 # -*- coding: utf-8 -*-
 """
 # myo/handle.py
 #
 # reflection from myo-bluetooth/myohw.h
 # the names are slightly different in dl-myo
-Services = {
-    # core service
-    0x0001: "ControlService",
-    0x0101: "MyoInfoCharacteristic",
-    0x0201: "FirmwareVersionCharacteristic ",
-    0x0401: "CommandCharacteristic",
-    # imu service
-    0x0002: "ImuDataService",
-    0x0402: "ImuDataCharacteristic",
-    0x0502: "MotionEventCharacteristic",
-    0x0003: "ClassifierService",
-    0x0103: "ClassifierEventCharacteristic",
-    # emg service
-    0x0005: "EmgDataService",
-    0x0105: "EmgData0Characteristic",
-    0x0205: "EmgData1Characteristic",
-    0x0305: "EmgData2Characteristic",
-    0x0405: "EmgData3Characteristic",
-    # standard bluetooh device service
-    0x180F: "BatteryService",
-    0x2A19: "BatteryLevelCharacteristic",
-    0x2A00: "DeviceName",
-}
+#
 """
 import aenum
 
 
 # fmt: off
 class Handle(aenum.Enum):
-    DEVICE_INFORMATION = 12 # 0x0c
+    DEVICE_INFORMATION = 12  # 0x0c
     MANUFACTURER_NAME_STRING = 13  # 0x0d
-    BATTERY_SERVICE = 15    # 0x0f
-    BATTERY_LEVEL = 16      # 0x10
-    CONTROL_SERVICE = 19    # 0x13
-    FIRMWARE_INFO = 20      # 0x14
-    FIRMWARE_VERSION = 22   # 0x16
-    COMMAND = 24            # 0x18
-    IMU_SERVICE = 26        # 0x1a
-    IMU_DATA = 27           # 0x1b
-    MOTION_EVENT = 30       # 0x1e
-    CLASSIFIER_SERVICE = 33 # 0x21
-    CLASSIFIER_EVENT = 34   # 0x22
-    FV_SERVICE = 37         # 0x25: EMG Filtered Value Service
-    FV_DATA = 38            # 0x26: EMG Filtered Value Data
-    EMG_SERVICE = 41        # 0x29
-    EMG0_DATA = 42          # 0x2a
-    EMG1_DATA = 45          # 0x2d
-    EMG2_DATA = 48          # 0x30
-    EMG3_DATA = 51          # 0x33
-    UNKNOWN_SERVICE = 54    # 0x36
-    UNKNOWN_CHAR = 55       # 0x37
+    BATTERY_SERVICE = 15     # 0x0f
+    BATTERY_LEVEL = 16       # 0x10
+    CONTROL_SERVICE = 19     # 0x13
+    FIRMWARE_INFO = 20       # 0x14
+    FIRMWARE_VERSION = 22    # 0x16
+    COMMAND = 24             # 0x18
+    IMU_SERVICE = 26         # 0x1a
+    IMU_DATA = 27            # 0x1b
+    MOTION_EVENT = 30        # 0x1e
+    CLASSIFIER_SERVICE = 33  # 0x21
+    CLASSIFIER_EVENT = 34    # 0x22
+    FV_SERVICE = 37          # 0x25: EMG Filtered Value Service
+    FV_DATA = 38             # 0x26: EMG Filtered Value Data
+    EMG_SERVICE = 41         # 0x29
+    EMG0_DATA = 42           # 0x2a
+    EMG1_DATA = 45           # 0x2d
+    EMG2_DATA = 48           # 0x30
+    EMG3_DATA = 51           # 0x33
+    UNKNOWN_SERVICE = 54     # 0x36
+    UNKNOWN_CHAR = 55        # 0x37
 # fmt: on
 
 
 class UUID:
     MYO_SERVICE = "d5060001-a904-deb9-4748-2c7f4a124842"
 
     # [Service] (Handle: 12): Device Information
```

### Comparing `dl_myo-0.1.6/myo/types.py` & `dl_myo-0.2.0/myo/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # -*- coding: utf-8 -*-type
+"""
 # myo/types.py
-# based on myo-bluetooth/myohw.h
+#
+# type reflection from myo-bluetooth/myohw.h
+#
+"""
 import json
 import struct
 
 import aenum
 
 
 class Constant(aenum.NamedConstant):
@@ -127,21 +131,21 @@
         return {"fv": self.fv, "mask": self.mask}
 
 
 # -> myohw_emg_mode_t
 # cf. https://github.com/dzhu/myo-raw/issues/17#issuecomment-913140042
 # fmt: off
 class EMGMode(aenum.Enum):
-    NONE = 0x00      # Do not send EMG data.
-    SEND_FILT = 0x01 # Send bandpass-filtered && rectified EMG data.
-                     #  - This is a hidden mode in myohw.h.
-                     #  - See FVData for the interpolated type
-    SEND_EMG = 0x02  # Send filtered && unrectified EMG data.
-    SEND_RAW = 0x03  # Send unfiltered and unrectified EMG data.
-                     #  - The values are scaled between [-128,127]
+    NONE = 0x00       # Do not send EMG data.
+    SEND_FILT = 0x01  # Send bandpass-filtered && rectified EMG data.
+    # noqa            #  - This is a hidden mode in myohw.h.
+    # noqa            #  - See FVData for the interpolated type
+    SEND_EMG = 0x02   # Send filtered && unrectified EMG data.
+    SEND_RAW = 0x03   # Send unfiltered and unrectified EMG data.
+    # noqa                  #  - The values are scaled between [-128,127]
 # fmt: on
 
 
 # -> myohw_fw_info_t
 class FirmwareInfo:
     def __init__(self, data):
         u = struct.unpack("<6BH12B", data)  # 20 bytes
@@ -231,19 +235,19 @@
             "gyroscope": self.gyroscope,
         }
 
 
 # -> myohw_imu_mode_t
 # fmt: off
 class IMUMode(aenum.Enum):
-    NONE = 0x00        # Do not send IMU data or events.
-    SEND_DATA = 0x01   # Send IMU data streams (accel, gyro, and orientation).
-    SEND_EVENTS = 0x02 # Send motion events detected by the IMU (e.g. taps).
-    SEND_ALL = 0x03    # Send both IMU data streams and motion events.
-    SEND_RAW = 0x04    # Send raw IMU data streams.
+    NONE = 0x00         # Do not send IMU data or events.
+    SEND_DATA = 0x01    # Send IMU data streams (accel, gyro, and orientation).
+    SEND_EVENTS = 0x02  # Send motion events detected by the IMU (e.g. taps).
+    SEND_ALL = 0x03     # Send both IMU data streams and motion events.
+    SEND_RAW = 0x04     # Send raw IMU data streams.
 # fmt: on
 
 
 # -> myohw_motion_event_t
 class MotionEvent:
     def __init__(self, data):
         t, _, _ = struct.unpack("<3b", data)
```

### Comparing `dl_myo-0.1.6/pyproject.toml` & `dl_myo-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "Environment :: Console",
     "Framework :: AsyncIO",
     "Framework :: Hatch",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Human Machine Interfaces",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
@@ -66,15 +67,14 @@
 # Same as Black.
 line-length = 120
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 # Assume Python 3.10.
 target-version = "py311"
 
-
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
@@ -90,31 +90,32 @@
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.poetry]
 name = "dl-myo"
-version = "0.1.6"
+version = "0.2.0"
 description = "A replacement middleware to MyoConnect for Myo Armband"
 authors = ["Iori Mizutani <iori.mizutani@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "myo"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 aenum = "^3.1.12"
 bleak = "^0.20.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
-format = "{base}"
+vcs = "git"
+style = "semver"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `dl_myo-0.1.6/PKG-INFO` & `dl_myo-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: dl-myo
-Version: 0.1.6
+Version: 0.2.0
 Summary: A replacement middleware to MyoConnect for Myo Armband
 License: GPLv3
 Author: Iori Mizutani
 Author-email: iori.mizutani@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aenum (>=3.1.12,<4.0.0)
 Requires-Dist: bleak (>=0.20.2,<0.21.0)
 Description-Content-Type: text/markdown
 
 # dl-myo (Dongle-less Myo)
```

