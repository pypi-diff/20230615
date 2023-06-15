# Comparing `tmp/wireguard_tools-0.4.2.tar.gz` & `tmp/wireguard_tools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireguard_tools-0.4.2.tar", max compression
+gzip compressed data, was "wireguard_tools-0.4.3.tar", max compression
```

## Comparing `wireguard_tools-0.4.2.tar` & `wireguard_tools-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1083 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSE
-drwxr-xr-x   0        0        0        0 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSES/
--rw-r--r--   0        0        0      643 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSES/0BSD.txt
--rw-r--r--   0        0        0     1593 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSES/CC-PDDC.txt
--rw-r--r--   0        0        0     1078 2022-12-13 17:55:51.419036 wireguard_tools-0.4.2/LICENSES/MIT.txt
--rw-r--r--   0        0        0     6461 2023-02-10 16:50:15.058517 wireguard_tools-0.4.2/README.md
--rw-r--r--   0        0        0     2151 2023-05-24 16:10:48.981131 wireguard_tools-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      362 2023-05-24 16:10:48.981131 wireguard_tools-0.4.2/src/wireguard_tools/__init__.py
--rw-r--r--   0        0        0      188 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/src/wireguard_tools/__main__.py
--rw-r--r--   0        0        0     7924 2022-12-16 20:19:27.612313 wireguard_tools-0.4.2/src/wireguard_tools/cli.py
--rw-r--r--   0        0        0     5689 2022-12-19 15:20:49.914859 wireguard_tools-0.4.2/src/wireguard_tools/curve25519.py
--rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/src/wireguard_tools/py.typed
--rw-r--r--   0        0        0      335 2023-03-15 16:34:00.717711 wireguard_tools-0.4.2/src/wireguard_tools/tunnel.conf
--rw-r--r--   0        0        0    10566 2023-03-15 18:09:02.843944 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_config.py
--rw-r--r--   0        0        0     1250 2022-12-16 19:21:20.697346 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_device.py
--rw-r--r--   0        0        0     2571 2022-12-19 15:53:22.370441 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_key.py
--rw-r--r--   0        0        0     4456 2023-05-24 16:10:17.684255 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_netlink.py
--rw-r--r--   0        0        0     5964 2022-12-19 15:53:36.746821 wireguard_tools-0.4.2/src/wireguard_tools/wireguard_uapi.py
--rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/__init__.py
--rw-r--r--   0        0        0      215 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0     8965 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/test_curve25519.py
--rw-r--r--   0        0        0     1460 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/test_wireguard_config.py
--rw-r--r--   0        0        0      661 2022-12-13 17:55:51.423036 wireguard_tools-0.4.2/tests/test_wireguard_key.py
--rw-r--r--   0        0        0     7570 1970-01-01 00:00:00.000000 wireguard_tools-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSE
+drwxr-xr-x   0        0        0        0 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSES/
+-rw-r--r--   0        0        0      643 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSES/0BSD.txt
+-rw-r--r--   0        0        0     1593 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSES/CC-PDDC.txt
+-rw-r--r--   0        0        0     1078 2022-12-13 17:55:51.419036 wireguard_tools-0.4.3/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     6461 2023-02-10 16:50:15.058517 wireguard_tools-0.4.3/README.md
+-rw-r--r--   0        0        0     2151 2023-06-15 19:21:39.004341 wireguard_tools-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-06-15 19:21:39.004341 wireguard_tools-0.4.3/src/wireguard_tools/__init__.py
+-rw-r--r--   0        0        0      188 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/src/wireguard_tools/__main__.py
+-rw-r--r--   0        0        0     7924 2022-12-16 20:19:27.612313 wireguard_tools-0.4.3/src/wireguard_tools/cli.py
+-rw-r--r--   0        0        0     5689 2022-12-19 15:20:49.914859 wireguard_tools-0.4.3/src/wireguard_tools/curve25519.py
+-rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/src/wireguard_tools/py.typed
+-rw-r--r--   0        0        0      335 2023-03-15 16:34:00.717711 wireguard_tools-0.4.3/src/wireguard_tools/tunnel.conf
+-rw-r--r--   0        0        0    11336 2023-06-15 19:18:53.774947 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_config.py
+-rw-r--r--   0        0        0     1250 2022-12-16 19:21:20.697346 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_device.py
+-rw-r--r--   0        0        0     2571 2022-12-19 15:53:22.370441 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_key.py
+-rw-r--r--   0        0        0     4456 2023-05-24 16:10:17.684255 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_netlink.py
+-rw-r--r--   0        0        0     5964 2022-12-19 15:53:36.746821 wireguard_tools-0.4.3/src/wireguard_tools/wireguard_uapi.py
+-rw-r--r--   0        0        0        0 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/__init__.py
+-rw-r--r--   0        0        0      215 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/conftest.py
+-rw-r--r--   0        0        0     8965 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/test_curve25519.py
+-rw-r--r--   0        0        0     1460 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/test_wireguard_config.py
+-rw-r--r--   0        0        0      661 2022-12-13 17:55:51.423036 wireguard_tools-0.4.3/tests/test_wireguard_key.py
+-rw-r--r--   0        0        0     7570 1970-01-01 00:00:00.000000 wireguard_tools-0.4.3/PKG-INFO
```

### Comparing `wireguard_tools-0.4.2/LICENSE` & `wireguard_tools-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/LICENSES/0BSD.txt` & `wireguard_tools-0.4.3/LICENSES/0BSD.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/LICENSES/CC-PDDC.txt` & `wireguard_tools-0.4.3/LICENSES/CC-PDDC.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/LICENSES/MIT.txt` & `wireguard_tools-0.4.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/README.md` & `wireguard_tools-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/pyproject.toml` & `wireguard_tools-0.4.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2022-2023 Carnegie Mellon University
 # SPDX-License-Identifier: 0BSD
 
 [tool.poetry]
 name = "wireguard-tools"
-version = "0.4.2"
+version = "0.4.3"
 description = "Pure python reimplementation of wireguard-tools"
 authors = [
     "Carnegie Mellon University <satya+group@cs.cmu.edu>",
     "Jan Harkes <jaharkes@cs.cmu.edu>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `wireguard_tools-0.4.2/src/wireguard_tools/cli.py` & `wireguard_tools-0.4.3/src/wireguard_tools/cli.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/src/wireguard_tools/curve25519.py` & `wireguard_tools-0.4.3/src/wireguard_tools/curve25519.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_config.py` & `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,14 +147,19 @@
     )
     dns_servers: list[IPv4Address | IPv6Address] = field(
         converter=_list_of_ipaddress, factory=list
     )
     search_domains: list[str] = field(factory=list)
     mtu: int | None = field(converter=optional(int), default=None)
 
+    preup: list[str] = field(factory=list)
+    postup: list[str] = field(factory=list)
+    predown: list[str] = field(factory=list)
+    postdown: list[str] = field(factory=list)
+
     # wireguard-android specific extensions
     included_applications: list[str] = field(factory=list)
     excluded_applications: list[str] = field(factory=list)
 
     @classmethod
     def from_dict(cls, config_dict: dict[str, Any]) -> WireguardConfig:
         config_dict = config_dict.copy()
@@ -189,15 +194,15 @@
             return value
 
         return asdict(self, filter=_filter, value_serializer=_serializer)
 
     @classmethod
     def from_wgconfig(cls, configfile: TextIO) -> WireguardConfig:
         text = configfile.read()
-        _pre, *parts = re.split(r"\[(Interface|Peer)\]\n", text, re.I)
+        _pre, *parts = re.split(r"\[(Interface|Peer)\]\n", text, flags=re.I)
         sections = [section.lower() for section in parts[0::2]]
         if sections.count("interface") > 1:
             raise ValueError("More than one [Interface] section in config file")
 
         config = cls()
         for section, content in zip(sections, parts[1::2]):
             key_value = [
@@ -227,14 +232,22 @@
                     self._add_dns_entry(item)
             elif key == "mtu":
                 self.mtu = int(value)
             elif key == "includedapplications":
                 self.included_applications.extend(item for item in value.split(", "))
             elif key == "excludedapplications":
                 self.excluded_applications.extend(item for item in value.split(", "))
+            elif key == "preup":
+                self.preup.append(value)
+            elif key == "postup":
+                self.postup.append(value)
+            elif key == "predown":
+                self.predown.append(value)
+            elif key == "postdown":
+                self.postdown.append(value)
 
     def _add_dns_entry(self, item: str) -> None:
         try:
             self.dns_servers.append(ip_address(item))
         except ValueError:
             self.search_domains.append(item)
 
@@ -255,14 +268,19 @@
         if wgquick_format:
             if self.mtu is not None:
                 conf.append(f"MTU = {self.mtu}")
             conf.extend([f"Address = {addr}" for addr in self.addresses])
             conf.extend([f"DNS = {addr}" for addr in self.dns_servers])
             conf.extend([f"DNS = {domain}" for domain in self.search_domains])
 
+            conf.extend([f"PreUp = {cmd}" for cmd in self.preup])
+            conf.extend([f"PostUp = {cmd}" for cmd in self.postup])
+            conf.extend([f"PreDown = {cmd}" for cmd in self.predown])
+            conf.extend([f"PostDown = {cmd}" for cmd in self.postdown])
+
             # wireguard-android specific extensions
             if self.included_applications:
                 apps = ", ".join(self.included_applications)
                 conf.append(f"IncludedApplications = {apps}")
             if self.excluded_applications:
                 apps = ", ".join(self.excluded_applications)
                 conf.append(f"ExcludedApplications = {apps}")
```

### Comparing `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_device.py` & `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_device.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_key.py` & `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_key.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_netlink.py` & `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_netlink.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/src/wireguard_tools/wireguard_uapi.py` & `wireguard_tools-0.4.3/src/wireguard_tools/wireguard_uapi.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/tests/test_curve25519.py` & `wireguard_tools-0.4.3/tests/test_curve25519.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/tests/test_wireguard_config.py` & `wireguard_tools-0.4.3/tests/test_wireguard_config.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/tests/test_wireguard_key.py` & `wireguard_tools-0.4.3/tests/test_wireguard_key.py`

 * *Files identical despite different names*

### Comparing `wireguard_tools-0.4.2/PKG-INFO` & `wireguard_tools-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wireguard-tools
-Version: 0.4.2
+Version: 0.4.3
 Summary: Pure python reimplementation of wireguard-tools
 Home-page: https://github.com/cmusatyalab/wireguard-tools
 License: MIT
 Author: Carnegie Mellon University
 Author-email: satya+group@cs.cmu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

