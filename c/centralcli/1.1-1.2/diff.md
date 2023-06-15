# Comparing `tmp/centralcli-1.1.tar.gz` & `tmp/centralcli-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centralcli-1.1.tar", max compression
+gzip compressed data, was "centralcli-1.2.tar", max compression
```

## Comparing `centralcli-1.1.tar` & `centralcli-1.2.tar`

### file list

```diff
@@ -1,48 +1,47 @@
--rw-r--r--   0        0        0    11929 2022-07-11 23:06:32.918521 centralcli-1.1/README.md
--rw-r--r--   0        0        0     4279 2022-06-22 02:13:00.537341 centralcli-1.1/centralcli/__init__.py
--rw-r--r--   0        0        0     1266 2022-09-23 14:08:18.905345 centralcli-1.1/centralcli/boilerplate/README.md
--rw-r--r--   0        0        0  1080145 2023-06-10 14:09:43.613064 centralcli-1.1/centralcli/boilerplate/allcalls.py
--rw-r--r--   0        0        0   168637 2022-09-23 14:10:56.815345 centralcli-1.1/centralcli/boilerplate/configuration.py
--rw-r--r--   0        0        0    23734 2022-09-23 14:12:10.005345 centralcli-1.1/centralcli/boilerplate/firmware.py
--rw-r--r--   0        0        0    37375 2022-09-23 14:14:48.045345 centralcli-1.1/centralcli/boilerplate/guest.py
--rw-r--r--   0        0        0    55587 2022-09-23 14:18:58.145345 centralcli-1.1/centralcli/boilerplate/wlan.py
--rw-r--r--   0        0        0    12139 2022-06-03 00:05:56.000000 centralcli-1.1/centralcli/caas.py
--rw-r--r--   0        0        0    78021 2023-02-21 21:25:42.842490 centralcli-1.1/centralcli/cache.py
--rw-r--r--   0        0        0   196449 2023-06-09 00:21:27.422666 centralcli-1.1/centralcli/central.py
--rw-r--r--   0        0        0    35466 2023-06-09 00:06:32.643001 centralcli-1.1/centralcli/cleaner.py
--rw-r--r--   0        0        0    41954 2022-10-03 05:26:22.821699 centralcli-1.1/centralcli/cli.py
--rw-r--r--   0        0        0    29703 2023-06-07 16:20:54.400957 centralcli-1.1/centralcli/cliadd.py
--rw-r--r--   0        0        0     4729 2022-07-14 03:34:30.218521 centralcli-1.1/centralcli/cliassign.py
--rw-r--r--   0        0        0    50683 2023-05-04 03:15:53.898642 centralcli-1.1/centralcli/clibatch.py
--rw-r--r--   0        0        0    16403 2022-06-18 06:04:41.177341 centralcli-1.1/centralcli/clicaas.py
--rw-r--r--   0        0        0     2995 2022-01-02 22:57:26.000000 centralcli-1.1/centralcli/cliclone.py
--rw-r--r--   0        0        0    21576 2022-12-28 02:39:54.056256 centralcli-1.1/centralcli/clicommon.py
--rw-r--r--   0        0        0    21359 2023-01-31 22:11:43.015287 centralcli-1.1/centralcli/clidel.py
--rw-r--r--   0        0        0     3251 2022-06-17 04:56:34.221894 centralcli-1.1/centralcli/clirefresh.py
--rw-r--r--   0        0        0   117310 2023-06-09 00:35:29.061168 centralcli-1.1/centralcli/clishow.py
--rw-r--r--   0        0        0     3943 2022-04-14 02:45:35.000000 centralcli-1.1/centralcli/clishowbranch.py
--rw-r--r--   0        0        0     7645 2022-09-23 00:12:29.685345 centralcli-1.1/centralcli/clishowfirmware.py
--rw-r--r--   0        0        0    12980 2023-05-04 02:10:12.446341 centralcli-1.1/centralcli/clishowospf.py
--rw-r--r--   0        0        0    17267 2022-06-17 03:33:33.981894 centralcli-1.1/centralcli/clishowwids.py
--rw-r--r--   0        0        0     8262 2022-07-14 01:24:31.928521 centralcli-1.1/centralcli/clitest.py
--rw-r--r--   0        0        0     6379 2022-09-15 06:49:16.849375 centralcli-1.1/centralcli/clitshoot.py
--rw-r--r--   0        0        0     5245 2022-07-14 00:35:03.158521 centralcli-1.1/centralcli/cliunassign.py
--rw-r--r--   0        0        0    22034 2022-12-08 05:48:17.878629 centralcli-1.1/centralcli/cliupdate.py
--rw-r--r--   0        0        0     8971 2023-01-18 01:56:38.384183 centralcli-1.1/centralcli/cliupgrade.py
--rw-r--r--   0        0        0    18707 2023-01-31 22:28:11.185804 centralcli-1.1/centralcli/config.py
--rw-r--r--   0        0        0    37152 2023-05-04 02:09:38.206295 centralcli-1.1/centralcli/constants.py
--rw-r--r--   0        0        0      160 2022-12-14 19:38:57.975685 centralcli-1.1/centralcli/exceptions.py
--rw-r--r--   0        0        0     6501 2022-02-23 03:21:04.000000 centralcli-1.1/centralcli/logger.py
--rw-r--r--   0        0        0      242 2022-09-07 14:50:09.838574 centralcli-1.1/centralcli/models.py
--rw-r--r--   0        0        0    15620 2022-12-28 04:26:44.221670 centralcli-1.1/centralcli/render.py
--rw-r--r--   0        0        0    36501 2023-06-10 14:17:38.298215 centralcli-1.1/centralcli/response.py
--rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-1.1/centralcli/setup.py
--rw-r--r--   0        0        0     1150 2022-02-10 22:18:16.000000 centralcli-1.1/centralcli/static/favicon.ico
--rw-r--r--   0        0        0     9157 2023-05-04 02:27:25.277696 centralcli-1.1/centralcli/strings.py
--rw-r--r--   0        0        0    31046 2022-10-06 02:15:00.061699 centralcli-1.1/centralcli/utils.py
--rw-r--r--   0        0        0     5407 2022-04-29 01:09:46.000000 centralcli-1.1/centralcli/vscodeargs.py
--rw-r--r--   0        0        0    15567 2022-12-28 03:21:15.553278 centralcli-1.1/centralcli/wh_proxy.py
--rw-r--r--   0        0        0      393 2022-01-14 00:45:59.000000 centralcli-1.1/centralcli/wh_proxy_service.py
--rw-r--r--   0        0        0     1982 2023-06-10 14:34:12.497780 centralcli-1.1/pyproject.toml
--rw-r--r--   0        0        0    13588 2023-06-10 14:35:26.204030 centralcli-1.1/setup.py
--rw-r--r--   0        0        0    13871 2023-06-10 14:35:26.205282 centralcli-1.1/PKG-INFO
+-rw-r--r--   0        0        0    11929 2022-07-11 23:06:32.918521 centralcli-1.2/README.md
+-rw-r--r--   0        0        0     4279 2022-06-22 02:13:00.537341 centralcli-1.2/centralcli/__init__.py
+-rw-r--r--   0        0        0     1266 2022-09-23 14:08:18.905345 centralcli-1.2/centralcli/boilerplate/README.md
+-rw-r--r--   0        0        0  1080145 2023-06-10 14:09:43.613064 centralcli-1.2/centralcli/boilerplate/allcalls.py
+-rw-r--r--   0        0        0   168637 2022-09-23 14:10:56.815345 centralcli-1.2/centralcli/boilerplate/configuration.py
+-rw-r--r--   0        0        0    23734 2022-09-23 14:12:10.005345 centralcli-1.2/centralcli/boilerplate/firmware.py
+-rw-r--r--   0        0        0    37375 2022-09-23 14:14:48.045345 centralcli-1.2/centralcli/boilerplate/guest.py
+-rw-r--r--   0        0        0    55587 2022-09-23 14:18:58.145345 centralcli-1.2/centralcli/boilerplate/wlan.py
+-rw-r--r--   0        0        0    12139 2022-06-03 00:05:56.000000 centralcli-1.2/centralcli/caas.py
+-rw-r--r--   0        0        0    78021 2023-02-21 21:25:42.842490 centralcli-1.2/centralcli/cache.py
+-rw-r--r--   0        0        0   196449 2023-06-09 00:21:27.422666 centralcli-1.2/centralcli/central.py
+-rw-r--r--   0        0        0    38326 2023-06-14 23:58:53.222184 centralcli-1.2/centralcli/cleaner.py
+-rw-r--r--   0        0        0    41954 2022-10-03 05:26:22.821699 centralcli-1.2/centralcli/cli.py
+-rw-r--r--   0        0        0    29703 2023-06-07 16:20:54.400957 centralcli-1.2/centralcli/cliadd.py
+-rw-r--r--   0        0        0     4729 2022-07-14 03:34:30.218521 centralcli-1.2/centralcli/cliassign.py
+-rw-r--r--   0        0        0    50683 2023-05-04 03:15:53.898642 centralcli-1.2/centralcli/clibatch.py
+-rw-r--r--   0        0        0    16403 2022-06-18 06:04:41.177341 centralcli-1.2/centralcli/clicaas.py
+-rw-r--r--   0        0        0     2995 2022-01-02 22:57:26.000000 centralcli-1.2/centralcli/cliclone.py
+-rw-r--r--   0        0        0    21576 2022-12-28 02:39:54.056256 centralcli-1.2/centralcli/clicommon.py
+-rw-r--r--   0        0        0    21359 2023-01-31 22:11:43.015287 centralcli-1.2/centralcli/clidel.py
+-rw-r--r--   0        0        0     3251 2022-06-17 04:56:34.221894 centralcli-1.2/centralcli/clirefresh.py
+-rw-r--r--   0        0        0   117482 2023-06-15 00:01:37.531566 centralcli-1.2/centralcli/clishow.py
+-rw-r--r--   0        0        0     3943 2022-04-14 02:45:35.000000 centralcli-1.2/centralcli/clishowbranch.py
+-rw-r--r--   0        0        0     7645 2022-09-23 00:12:29.685345 centralcli-1.2/centralcli/clishowfirmware.py
+-rw-r--r--   0        0        0    12980 2023-05-04 02:10:12.446341 centralcli-1.2/centralcli/clishowospf.py
+-rw-r--r--   0        0        0    17267 2022-06-17 03:33:33.981894 centralcli-1.2/centralcli/clishowwids.py
+-rw-r--r--   0        0        0     8262 2022-07-14 01:24:31.928521 centralcli-1.2/centralcli/clitest.py
+-rw-r--r--   0        0        0     6379 2022-09-15 06:49:16.849375 centralcli-1.2/centralcli/clitshoot.py
+-rw-r--r--   0        0        0     5245 2022-07-14 00:35:03.158521 centralcli-1.2/centralcli/cliunassign.py
+-rw-r--r--   0        0        0    22034 2022-12-08 05:48:17.878629 centralcli-1.2/centralcli/cliupdate.py
+-rw-r--r--   0        0        0     8971 2023-01-18 01:56:38.384183 centralcli-1.2/centralcli/cliupgrade.py
+-rw-r--r--   0        0        0    18707 2023-01-31 22:28:11.185804 centralcli-1.2/centralcli/config.py
+-rw-r--r--   0        0        0    37152 2023-05-04 02:09:38.206295 centralcli-1.2/centralcli/constants.py
+-rw-r--r--   0        0        0      160 2022-12-14 19:38:57.975685 centralcli-1.2/centralcli/exceptions.py
+-rw-r--r--   0        0        0     6501 2022-02-23 03:21:04.000000 centralcli-1.2/centralcli/logger.py
+-rw-r--r--   0        0        0      242 2022-09-07 14:50:09.838574 centralcli-1.2/centralcli/models.py
+-rw-r--r--   0        0        0    15620 2022-12-28 04:26:44.221670 centralcli-1.2/centralcli/render.py
+-rw-r--r--   0        0        0    36501 2023-06-10 14:17:38.298215 centralcli-1.2/centralcli/response.py
+-rw-r--r--   0        0        0       96 2021-10-13 20:41:19.000000 centralcli-1.2/centralcli/setup.py
+-rw-r--r--   0        0        0     1150 2022-02-10 22:18:16.000000 centralcli-1.2/centralcli/static/favicon.ico
+-rw-r--r--   0        0        0     9157 2023-05-04 02:27:25.277696 centralcli-1.2/centralcli/strings.py
+-rw-r--r--   0        0        0    31046 2022-10-06 02:15:00.061699 centralcli-1.2/centralcli/utils.py
+-rw-r--r--   0        0        0     5407 2022-04-29 01:09:46.000000 centralcli-1.2/centralcli/vscodeargs.py
+-rw-r--r--   0        0        0    15567 2022-12-28 03:21:15.553278 centralcli-1.2/centralcli/wh_proxy.py
+-rw-r--r--   0        0        0      393 2022-01-14 00:45:59.000000 centralcli-1.2/centralcli/wh_proxy_service.py
+-rw-r--r--   0        0        0     1995 2023-06-15 00:08:57.950478 centralcli-1.2/pyproject.toml
+-rw-r--r--   0        0        0    13880 1970-01-01 00:00:00.000000 centralcli-1.2/PKG-INFO
```

### Comparing `centralcli-1.1/README.md` & `centralcli-1.2/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/__init__.py` & `centralcli-1.2/centralcli/__init__.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/boilerplate/README.md` & `centralcli-1.2/centralcli/boilerplate/README.md`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/boilerplate/allcalls.py` & `centralcli-1.2/centralcli/boilerplate/allcalls.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/boilerplate/configuration.py` & `centralcli-1.2/centralcli/boilerplate/configuration.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/boilerplate/firmware.py` & `centralcli-1.2/centralcli/boilerplate/firmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/boilerplate/guest.py` & `centralcli-1.2/centralcli/boilerplate/guest.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/boilerplate/wlan.py` & `centralcli-1.2/centralcli/boilerplate/wlan.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/caas.py` & `centralcli-1.2/centralcli/caas.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/cache.py` & `centralcli-1.2/centralcli/cache.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/central.py` & `centralcli-1.2/centralcli/central.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/cleaner.py` & `centralcli-1.2/centralcli/cleaner.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
 Collection of functions used to clean output from Aruba Central API into a consistent structure.
 """
+from __future__ import annotations
 import functools
 import ipaddress
 import logging
 import sys
 from pathlib import Path
 from typing import Any, Dict, List, Union
 
@@ -203,14 +204,16 @@
     "dr_address": "DR IP",
     "bdr_address": "BDR IP",
     "dr_id": "DR rtr id",
     "bdr_id": "BDR rtr id",
     "auth_type": "auth",
     "neighbor_count": "nbrs",
     "area_id": "area",
+    "intf_state_down_reason": "Down Reason",
+    "is_uplink": "Uplink",
 }
 
 
 def strip_outer_keys(data: dict) -> Union[list, dict]:
     """strip unnecessary wrapping key from API response payload
 
     Args:
@@ -293,14 +296,41 @@
         if key in ["sites", "labels"]:
             value = _extract_names_from_id_name_dict(value)
         elif key in ["events_details"]:
             value = _extract_event_details(value)
 
     return short_key(key), _unlist(value)
 
+def simple_kv_formatter(data: List) -> List:
+    """Default simple formatter
+
+    runs all key/values through _short_key, _short_value
+
+    Args:
+        data (List): Data typically a list of dicts
+
+    Returns:
+        List: Formatted data
+    """
+    if not isinstance(data, list):
+        log.warning(f"cleaner.simple_kv_formatter expected a list but rcvd {type(data)}")
+        return data
+
+    data = [
+        dict(
+            short_value(
+                k,
+                v,
+            )
+            for k, v in d.items()
+        )
+        for d in data
+    ]
+
+    return data
 
 def _get_group_names(data: List[List[str],]) -> list:
     """Convert list of single item lists to a list of strs
 
     Also removes "unprovisioned" group as it has no value for our
     purposes, and moves default group to beginning of list.
 
@@ -459,28 +489,49 @@
         data = [d for d in data if d["connected device"].lower() in _filter.lower()]
     # data = [_client_concat_associated_dev(d, verbose=verbose, cache=cache, **kwargs) for d in data]
     data = strip_no_value(data)
 
     return data
 
 
-def strip_no_value(data: List[dict]) -> List[dict]:
-    """strip out any columns that have no value in any row"""
+def strip_no_value(data: List[dict] | Dict[dict]) -> List[dict] | Dict[dict]:
+    """strip out any columns that have no value in any row
+
+    Accepts either List of dicts, or a Dict where the value for each key is a dict
+    """
     no_val_strings = ["Unknown", "NA", "None", "--", ""]
-    no_val: List[List[int]] = [
-        [
-            idx
-            for idx, v in enumerate(id.values())
-            if (not isinstance(v, bool) and not v) or (isinstance(v, str) and v and v in no_val_strings)
+    if isinstance(data, list):
+        no_val: List[List[int]] = [
+            [
+                idx
+                for idx, v in enumerate(id.values())
+                if (not isinstance(v, bool) and not v) or (isinstance(v, str) and v and v in no_val_strings)
+            ]
+            for id in data
         ]
-        for id in data
-    ]
-    if no_val:
-        common_idx: set = set.intersection(*map(set, no_val))
-        data = [{k: v for idx, (k, v) in enumerate(id.items()) if idx not in common_idx} for id in data]
+        if no_val:
+            common_idx: set = set.intersection(*map(set, no_val))
+            data = [{k: v for idx, (k, v) in enumerate(id.items()) if idx not in common_idx} for id in data]
+
+    elif isinstance(data, dict) and all(isinstance(d, dict) for d in data.values()):
+        no_val: List[List[int]] = [
+            [
+                idx
+                for idx, v in enumerate(data[id].values())
+                if (not isinstance(v, bool) and not v) or (isinstance(v, str) and v and v in no_val_strings)
+            ]
+            for id in data
+        ]
+        if no_val:
+            common_idx: set = set.intersection(*map(set, no_val))
+            data = {id: {k: v for idx, (k, v) in enumerate(data[id].items()) if idx not in common_idx} for id in data}
+    else:
+        log.error(
+            f"cleaner.strip_no_value recieved unexpected type {type(data)}. Expects List[dict], or Dict[dict]. Data was returned as is."
+        )
 
     return data
 
 
 def sort_result_keys(data: List[dict], order: List[str] = None) -> List[dict]:
     data = utils.listify(data)
     all_keys = list(set([ik for k in data for ik in k.keys()]))
@@ -1145,8 +1196,50 @@
         dict(
             short_value(
                 k if k != "address" else "ip/mask", v if k != "address" else str(ipaddress.ip_network(f"{inner['address']}/{inner['mask']}", strict=False))
             ) for k, v in inner.items() if k != "mask"
         ) for inner in data
     ]
 
-    return data
+    return data
+
+def show_interfaces(data: Union[List[dict], dict],) -> Union[List[dict], dict]:
+    data = utils.listify(data)
+
+    # TODO verbose and non-verbose
+    # TODO verify oper_state and status are always the same and only show one of them
+    key_order = [
+        "macaddr",
+        "type",
+        "phy_type",
+        "port",
+        "oper_state",
+        "admin_state",
+        "status",
+        "intf_state_down_reason",
+        "speed",
+        "duplex_mode",
+        "vlan",
+        "allowed_vlan",
+        "vlan_mode",
+        "mode",
+        "has_poe",
+        "poe_state",
+        "power_consumption",
+        "is_uplink",
+        "trusted",
+        "tx_usage",
+        "rx_usage",
+        "mux",
+        "vsx_enabled",
+    ]
+    strip_keys = ["port_number", "alignment",]
+
+    # Append any additional keys to the end
+    key_order = [*key_order, *data[-1].keys()]
+
+    # send all key/value pairs through formatters and convert List[Dict] to Dict where port_number is key
+    data = {
+        d["port_number"] if not all(d.isdigit() for d in d["port_number"]) else int(d["port_number"]): dict(short_value(k, d.get(k),) for k in key_order if k not in strip_keys) for d in data
+    }
+
+    return strip_no_value(data)
```

### Comparing `centralcli-1.1/centralcli/cli.py` & `centralcli-1.2/centralcli/cli.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/cliadd.py` & `centralcli-1.2/centralcli/cliadd.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/cliassign.py` & `centralcli-1.2/centralcli/cliassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clibatch.py` & `centralcli-1.2/centralcli/clibatch.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clicaas.py` & `centralcli-1.2/centralcli/clicaas.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/cliclone.py` & `centralcli-1.2/centralcli/cliclone.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clicommon.py` & `centralcli-1.2/centralcli/clicommon.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clidel.py` & `centralcli-1.2/centralcli/clidel.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clirefresh.py` & `centralcli-1.2/centralcli/clirefresh.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clishow.py` & `centralcli-1.2/centralcli/clishow.py`

 * *Files 0% similar despite different names*

```diff
@@ -551,16 +551,18 @@
 
     dev = cli.cache.get_dev_identifier(device,)
     if dev.generic_type == "gw":
         resp = cli.central.request(cli.central.get_gateway_ports, dev.serial)
     else:
         resp = cli.central.request(cli.central.get_switch_ports, dev.serial, slot=slot, cx=dev.type == "CX")
 
-    tablefmt = cli.get_format(do_json=do_json, do_yaml=do_yaml, do_csv=do_csv, do_table=do_table, default="json")
-    cli.display_results(resp, tablefmt=tablefmt, pager=pager, outfile=outfile, sort_by=sort_by, reverse=reverse)
+    tablefmt = cli.get_format(do_json=do_json, do_yaml=do_yaml, do_csv=do_csv, do_table=do_table, default="yaml")
+
+    # TODO cleaner returns a Dict[dict] assuming "vsx enabled" is the same bool for all ports put it in caption and remove from each item
+    cli.display_results(resp, tablefmt=tablefmt, pager=pager, outfile=outfile, sort_by=sort_by, reverse=reverse, cleaner=cleaner.show_interfaces)
 
 
 @app.command(help="Show (switch) poe details for an interface")
 def poe(
     device: str = typer.Argument(..., metavar=iden_meta.dev, hidden=False, autocompletion=cli.cache.dev_switch_completion),
     port: str = typer.Argument(None,),
     _port: str = typer.Option(None, "--port"),
```

### Comparing `centralcli-1.1/centralcli/clishowbranch.py` & `centralcli-1.2/centralcli/clishowbranch.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clishowfirmware.py` & `centralcli-1.2/centralcli/clishowfirmware.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clishowospf.py` & `centralcli-1.2/centralcli/clishowospf.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clishowwids.py` & `centralcli-1.2/centralcli/clishowwids.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clitest.py` & `centralcli-1.2/centralcli/clitest.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/clitshoot.py` & `centralcli-1.2/centralcli/clitshoot.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/cliunassign.py` & `centralcli-1.2/centralcli/cliunassign.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/cliupdate.py` & `centralcli-1.2/centralcli/cliupdate.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/cliupgrade.py` & `centralcli-1.2/centralcli/cliupgrade.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/config.py` & `centralcli-1.2/centralcli/config.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/constants.py` & `centralcli-1.2/centralcli/constants.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/logger.py` & `centralcli-1.2/centralcli/logger.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/render.py` & `centralcli-1.2/centralcli/render.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/response.py` & `centralcli-1.2/centralcli/response.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/static/favicon.ico` & `centralcli-1.2/centralcli/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/strings.py` & `centralcli-1.2/centralcli/strings.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/utils.py` & `centralcli-1.2/centralcli/utils.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/vscodeargs.py` & `centralcli-1.2/centralcli/vscodeargs.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/centralcli/wh_proxy.py` & `centralcli-1.2/centralcli/wh_proxy.py`

 * *Files identical despite different names*

### Comparing `centralcli-1.1/pyproject.toml` & `centralcli-1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "centralcli"
-version = "1.1"
+version = "1.2"
 description = "A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central."
 license = "MIT"
 authors = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 maintainers = ["Wade Wells (Pack3tL0ss) <wade@consolepi.org>"]
 readme = "README.md"
 repository = "https://github.com/Pack3tL0ss/central-api-cli"
 documentation = "https://central-api-cli.readthedocs.org"
@@ -24,48 +24,48 @@
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.scripts]
 cencli = "centralcli.cli:app"
 
 [tool.poetry.dependencies]
-python = "^3.8"
-tabulate = "^0.8.*"
-halo = "^0.0.*"
-typer = "^0.4"
-pylibyaml = "^0.1.0"
-PyYAML = "^6"
-tinydb = "^4"
-shellingham = "^1"
-pendulum = "^2"
-pycentral = "^0.0.3"
-aiohttp = "^3"
-asyncio = "^3"
+python = ">=3.8"
+tabulate = ">=0.8"
+halo = "*"
+typer = ">=0.4"
+pylibyaml = ">=0.1.0"
+PyYAML = ">=6"
+tinydb = ">=4"
+shellingham = ">=1"
+pendulum = ">=2"
+pycentral = ">=0.0.3"
+aiohttp = ">=3"
+asyncio = ">=3"
 rich = ">=10"
-tablib = "^3"
+tablib = ">=3"
 jinja2 = "*"
-pydantic = "^1.9.0"
-click = "^7.1.2"
+pydantic = ">=1.9.0"
+click = ">=7.1.2"
 ipaddress = "*"
 
 # Optional dependencies see tool.poetry.extras
 fastapi = {version = "*", optional = true}
 uvicorn = {version = "*", optional = true}
 psutil = {version = "*", optional = true}
-cchardet = {version = "^2.1.*", markers = "platform_system != 'Windows'", optional=true}
-aiodns = {version = "^1.1", optional = true}
+cchardet = {version = ">=2.1", markers = "platform_system != 'Windows'", optional=true}
+aiodns = {version = ">=1.1", optional = true}
 Brotli = {version = "*", optional = true}
 
 [tool.poetry.dev-dependencies]
-pyflakes = "^2"
-pycodestyle = "^2"
-flake8 = "^4"
-pytest = "^6"
-black = "^21.0"
-click = "^7.1.2"
+pyflakes = ">=2"
+pycodestyle = ">=2"
+flake8 = ">=4"
+pytest = ">=6"
+black = ">=21.0"
+click = ">=7.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 filterwarnings = [
```

### Comparing `centralcli-1.1/setup.py` & `centralcli-1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,184 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: centralcli
+Version: 1.2
+Summary: A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central.
+Home-page: https://github.com/Pack3tL0ss/central-api-cli
+License: MIT
+Keywords: cli,Aruba,Aruba Networks,Aruba Central,HPE,API,RESTFUL,REST
+Author: Wade Wells (Pack3tL0ss)
+Author-email: wade@consolepi.org
+Maintainer: Wade Wells (Pack3tL0ss)
+Maintainer-email: wade@consolepi.org
+Requires-Python: >=3.8
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: hook-proxy
+Provides-Extra: speedups
+Requires-Dist: Brotli ; extra == "speedups"
+Requires-Dist: PyYAML (>=6)
+Requires-Dist: aiodns (>=1.1) ; extra == "speedups"
+Requires-Dist: aiohttp (>=3)
+Requires-Dist: asyncio (>=3)
+Requires-Dist: cchardet (>=2.1) ; (platform_system != "Windows") and (extra == "speedups")
+Requires-Dist: click (>=7.1.2)
+Requires-Dist: fastapi ; extra == "hook-proxy"
+Requires-Dist: halo
+Requires-Dist: ipaddress
+Requires-Dist: jinja2
+Requires-Dist: pendulum (>=2)
+Requires-Dist: psutil ; extra == "hook-proxy"
+Requires-Dist: pycentral (>=0.0.3)
+Requires-Dist: pydantic (>=1.9.0)
+Requires-Dist: pylibyaml (>=0.1.0)
+Requires-Dist: rich (>=10)
+Requires-Dist: shellingham (>=1)
+Requires-Dist: tablib (>=3)
+Requires-Dist: tabulate (>=0.8)
+Requires-Dist: tinydb (>=4)
+Requires-Dist: typer (>=0.4)
+Requires-Dist: uvicorn ; extra == "hook-proxy"
+Project-URL: Documentation, https://central-api-cli.readthedocs.org
+Project-URL: Repository, https://github.com/Pack3tL0ss/central-api-cli
+Description-Content-Type: text/markdown
+
+# Aruba Central API CLI
+
+[![Latest Version](https://img.shields.io/pypi/v/centralcli.svg)](https://pypi.org/project/centralcli)
+[![Documentation Status](https://readthedocs.org/projects/central-api-cli/badge/?version=latest)](https://central-api-cli.readthedocs.io/en/latest/?badge=latest)
+
+A CLI app for interacting with Aruba Central Cloud Management Platform. With cross-platform shell support. Auto Completion, easy device/site/group/template identification (fuzzy match), support for batch import, and a lot more.
+
+  > As commands are built out the CLI hierarchy may evolve.  Refer to the [documentation](https://central-api-cli.readthedocs.org) or help text for CLI structure/syntax.
+
+![centralcli Animated Demo](https://raw.githubusercontent.com/Pack3tL0ss/central-api-cli/master/docs/img/cencli-demo.gif)
+
+## Features
+
+- Cross Platform Support
+- Auto/TAB Completion
+- Specify device, site, etc. by fuzzy match of multiple fields (i.e. name, mac, serial#, ip address)
+- Multiple output formats
+- Output to file
+- Numerous import formats (csv, yaml, json, xls, etc.)
+- Multiple account support (easily switch between different central accounts `--account myotheraccount`)
+- Batch Operation based on data from input file.  i.e. Add sites in batch based on data from a csv.
+- Automatic Token refresh.  With prompt to paste in a new token if it becomes invalid.
+  > If using Tokens, dedicate the token to the CLI alone, using it in swagger or on another system, will eventually lead to a refresh that invalidates the tokens on the other systems using it.
+- You can also use username/Password Auth. which will facilitate automatic retrieval of new Tokens even if they do become invalid.
+
+## Installation
+
+Requires python 3.7+ and pip
+
+`pip3 install centralcli`
+
+> You can also install in a virtual environment (venv), but you'll lose auto-completion, unless you activate the venv.
+
+### Upgrading the CLI
+
+`pip3 install -U centralcli`
+
+### if you don't have python
+
+- You can get it for any platform @ [https://www.python.org](https://www.python.org)
+- On Windows 10 it's also available in the Windows store.
+
+## Configuration
+
+Refer to [config.yaml.example](https://github.com/Pack3tL0ss/central-api-cli/blob/master/config/config.yaml.example) to guide in the creation of config.yaml and place in the config directory.
+
+CentralCli will look in \<Users home dir\>/.config/centralcli, and \<Users home dir\>\\.centralcli.
+i.e. on Windows `c:\Users\wade\.centralcli` or on Linux `/home/wade/.config/centralcli`
+
+Once `config.yaml` is populated per [config.yaml.example](config/config.yaml.example), run some test commands to validate the config.
+
+For Example `cencli show all`
+
+```bash
+wade@wellswa6:~ $ cencli show all
+                                                                                       All Devices
+ ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
+  name                  type   model                            ip                mac                 serial       group          site             labels        version       status
+ ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
+  6100F-48-LAB          cx     6100 48G CL4 4SFP+ Swch          10.0.40.11        --redacted--   --redacted--    WadeLab8x                                     10.08.1010       Down
+                               (JL675A)
+  SDBranch1:7008        gw     A7008                            192.168.240.101   --redacted--   --redacted--    Branch1        Antigua          Branch View   10.3.0.0_82528   Up
+  br1-2930F-sw          sw     Aruba2930F-8G-PoE+-2SFP+         10.101.5.4        --redacted--   --redacted--    Branch1        Antigua          Branch View   16.11.0002       Up
+                               Switch(JL258A)
+  br1-315.0c88-ap       ap     315                              10.101.6.200      --redacted--   --redacted--    Branch1        Antigua          Branch View   10.3.0.0_82528   Up
+  MB1-505h              ap     505H                             10.10.1.101       --redacted--   --redacted--    MicroBranch1   Champions Hill                 10.3.0.0_82528   Up
+  6200F-Bot             cx     6200F 48G CL4 4SFP+740W Swch     10.0.40.16        --redacted--   --redacted--    WadeLab8x      Pommore                        10.08.1010       Down
+                               (JL728A)
+  6200F-Top             cx     6200F 48G CL4 4SFP+740W Swch     10.0.40.6         --redacted--   --redacted--    WadeLab8x      Pommore                        10.08.1010       Down
+                               (JL728A)
+  APGW1                 gw     A9004-LTE                        10.0.35.10        --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82528   Up
+  APGW2                 gw     A9004                            10.0.35.20        --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82528   Up
+  VPNC1                 gw     A7005                            172.30.0.242      --redacted--   --redacted--    VPNC           WadeLab          Branch View   10.3.0.0_82528   Up
+  VPNC2                 gw     A7005                            172.30.0.243      --redacted--   --redacted--    VPNC           WadeLab          Branch View   10.3.0.0_82528   Up
+  av-555.11b8-ap        ap     555                              10.0.31.155       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down
+  barn-303p.2c30-ap     ap     303P                             10.1.30.151       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82528   Up
+  barn-4100i            cx     4100i 12G CL4/6 POE 2SFP+ DIN    10.1.30.152       --redacted--   --redacted--    WadeLab        WadeLab                        10.08.1010       Up
+                               Sw (JL817A)
+  barn-518.2816-ap      ap     518                              10.1.30.101       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82528   Up
+  bsmt-515.51s9-ap      ap     515                              10.0.30.233       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down
+  craft-2930F           sw     Aruba2930F-8G-PoE+-2SFP+         10.0.30.5         --redacted--   --redacted--    WadeLab        WadeLab                        16.11.0002       Up
+                               Switch(JL258A)
+  garage-345.5136-ap    ap     345                              10.0.31.148       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down
+  ktcn-505H.206c-ap     ap     505H                             10.0.30.212       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down
+  lwrptio-575.0824-ap   ap     575                              10.0.30.219       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down
+  zrm-535.70be-ap       ap     535                              10.0.31.101       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down
+ ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────
+  Show all displays fields common to all device types. To see all columns for a given device type use show <DEVICE TYPE>
+  API Rate Limit: 925 of 1000 remaining.
+
+```
+
+Use `cencli ?` to become familiar with the command options.
+
+### Auto Completion
+
+The CLI supports auto-completion.  To configure auto-completion run `cencli --install-completion`.  This will auto-detect the type of shell you are running in, and install the necessary completion into your profile.  You'll need to exit the shell and start a new session for it to take effect.
+
+## Usage Notes
+
+### Caching & Friendly identifiers
+
+- Caching: The CLI caches information on all devices, sites, groups, and templates in Central.  It's a minimal amount per device, and is done to allow human friendly identifiers.  The API typically accepts serial #, site id, etc.  This function allows you to specify a device by name, IP, mac (any format), and serial.
+
+The lookup sequence for a device:
+
+  1. Exact Match of any of the identifier fields (name, ip, mac, serial)
+  2. case insensitive match
+  3. case insensitive match disregarding all hyphens and underscores (in case you type 6200f_bot and the device name is 6200F-Bot)
+  4. Case insensitive Fuzzy match with implied wild-card, otherwise match any devices that start with the identifier provided. `cencli show switches 6200F` will result in a match of `6200F-Bot`.
+
+> If there is no match found, a cache update is triggered, and the match rules are re-tried.
+
+- Caching works in a similar manner for groups, templates, and sites.  Sites can match on name and nearly any address field.  So if you only had one site in San Antonio you could specify that site with `show sites 'San Antonio'`  \<-- Note the use of quotes because there is a space in the name.
+
+- **Multiple Matches**:  It's possible to specify an identifier that returns multiple matches (if drops all the way down to the Fuzzy match/implied trailing wild-card).  If that occurs you are prompted to select the intended device from a list of the matches.
+
+### Output Formats
+
+There are a number of output formats available.  Most commands default to what is likely the easiest to view given the number of fields.  Otherwise longer outputs are typically displayed vertically by default.  If the output can reasonably fit, it's displayed in tabular format horizontally.
+
+You can specify the output format with command line flags `--json`, `--yaml`, `--csv`, `--table`  rich is tabular format with folding (multi line within the same row) and truncating.
+
+> Most outputs will evolve to support an output with the most commonly desired fields by default and expanded vertical output via the `-v` option (not implemented yet.).  Currently the output is tabular horizontally if the amount of data is likely to fit most displays, and vertical otherwise.
+
+### File Output
 
-packages = \
-['centralcli', 'centralcli.boilerplate']
+Just use `--out \<filename\>` (or \<path\\filename\>), and specify the desired format.
 
-package_data = \
-{'': ['*'], 'centralcli': ['static/*']}
+## CLI Tree
 
-install_requires = \
-['PyYAML>=6,<7',
- 'aiohttp>=3,<4',
- 'asyncio>=3,<4',
- 'click>=7.1.2,<8.0.0',
- 'halo',
- 'ipaddress',
- 'jinja2',
- 'pendulum>=2,<3',
- 'pycentral>=0.0.3,<0.0.4',
- 'pydantic>=1.9.0,<2.0.0',
- 'pylibyaml>=0.1.0,<0.2.0',
- 'rich>=10',
- 'shellingham>=1,<2',
- 'tablib>=3,<4',
- 'tabulate',
- 'tinydb>=4,<5',
- 'typer>=0.4,<0.5']
-
-extras_require = \
-{'hook-proxy': ['fastapi', 'uvicorn', 'psutil'],
- 'speedups': ['aiodns>=1.1,<2.0', 'Brotli'],
- 'speedups:platform_system != "Windows"': ['cchardet']}
-
-entry_points = \
-{'console_scripts': ['cencli = centralcli.cli:app']}
-
-setup_kwargs = {
-    'name': 'centralcli',
-    'version': '1.1',
-    'description': 'A CLI for interacting with Aruba Central (Cloud Management Platform).  Facilitates bulk imports, exports, reporting.  A handy tool if you have devices managed by Aruba Central.',
-    'long_description': "# Aruba Central API CLI\n\n[![Latest Version](https://img.shields.io/pypi/v/centralcli.svg)](https://pypi.org/project/centralcli)\n[![Documentation Status](https://readthedocs.org/projects/central-api-cli/badge/?version=latest)](https://central-api-cli.readthedocs.io/en/latest/?badge=latest)\n\nA CLI app for interacting with Aruba Central Cloud Management Platform. With cross-platform shell support. Auto Completion, easy device/site/group/template identification (fuzzy match), support for batch import, and a lot more.\n\n  > As commands are built out the CLI hierarchy may evolve.  Refer to the [documentation](https://central-api-cli.readthedocs.org) or help text for CLI structure/syntax.\n\n![centralcli Animated Demo](https://raw.githubusercontent.com/Pack3tL0ss/central-api-cli/master/docs/img/cencli-demo.gif)\n\n## Features\n\n- Cross Platform Support\n- Auto/TAB Completion\n- Specify device, site, etc. by fuzzy match of multiple fields (i.e. name, mac, serial#, ip address)\n- Multiple output formats\n- Output to file\n- Numerous import formats (csv, yaml, json, xls, etc.)\n- Multiple account support (easily switch between different central accounts `--account myotheraccount`)\n- Batch Operation based on data from input file.  i.e. Add sites in batch based on data from a csv.\n- Automatic Token refresh.  With prompt to paste in a new token if it becomes invalid.\n  > If using Tokens, dedicate the token to the CLI alone, using it in swagger or on another system, will eventually lead to a refresh that invalidates the tokens on the other systems using it.\n- You can also use username/Password Auth. which will facilitate automatic retrieval of new Tokens even if they do become invalid.\n\n## Installation\n\nRequires python 3.7+ and pip\n\n`pip3 install centralcli`\n\n> You can also install in a virtual environment (venv), but you'll lose auto-completion, unless you activate the venv.\n\n### Upgrading the CLI\n\n`pip3 install -U centralcli`\n\n### if you don't have python\n\n- You can get it for any platform @ [https://www.python.org](https://www.python.org)\n- On Windows 10 it's also available in the Windows store.\n\n## Configuration\n\nRefer to [config.yaml.example](https://github.com/Pack3tL0ss/central-api-cli/blob/master/config/config.yaml.example) to guide in the creation of config.yaml and place in the config directory.\n\nCentralCli will look in \\<Users home dir\\>/.config/centralcli, and \\<Users home dir\\>\\\\.centralcli.\ni.e. on Windows `c:\\Users\\wade\\.centralcli` or on Linux `/home/wade/.config/centralcli`\n\nOnce `config.yaml` is populated per [config.yaml.example](config/config.yaml.example), run some test commands to validate the config.\n\nFor Example `cencli show all`\n\n```bash\nwade@wellswa6:~ $ cencli show all\n                                                                                       All Devices\n ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────\n  name                  type   model                            ip                mac                 serial       group          site             labels        version       status\n ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────\n  6100F-48-LAB          cx     6100 48G CL4 4SFP+ Swch          10.0.40.11        --redacted--   --redacted--    WadeLab8x                                     10.08.1010       Down\n                               (JL675A)\n  SDBranch1:7008        gw     A7008                            192.168.240.101   --redacted--   --redacted--    Branch1        Antigua          Branch View   10.3.0.0_82528   Up\n  br1-2930F-sw          sw     Aruba2930F-8G-PoE+-2SFP+         10.101.5.4        --redacted--   --redacted--    Branch1        Antigua          Branch View   16.11.0002       Up\n                               Switch(JL258A)\n  br1-315.0c88-ap       ap     315                              10.101.6.200      --redacted--   --redacted--    Branch1        Antigua          Branch View   10.3.0.0_82528   Up\n  MB1-505h              ap     505H                             10.10.1.101       --redacted--   --redacted--    MicroBranch1   Champions Hill                 10.3.0.0_82528   Up\n  6200F-Bot             cx     6200F 48G CL4 4SFP+740W Swch     10.0.40.16        --redacted--   --redacted--    WadeLab8x      Pommore                        10.08.1010       Down\n                               (JL728A)\n  6200F-Top             cx     6200F 48G CL4 4SFP+740W Swch     10.0.40.6         --redacted--   --redacted--    WadeLab8x      Pommore                        10.08.1010       Down\n                               (JL728A)\n  APGW1                 gw     A9004-LTE                        10.0.35.10        --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82528   Up\n  APGW2                 gw     A9004                            10.0.35.20        --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82528   Up\n  VPNC1                 gw     A7005                            172.30.0.242      --redacted--   --redacted--    VPNC           WadeLab          Branch View   10.3.0.0_82528   Up\n  VPNC2                 gw     A7005                            172.30.0.243      --redacted--   --redacted--    VPNC           WadeLab          Branch View   10.3.0.0_82528   Up\n  av-555.11b8-ap        ap     555                              10.0.31.155       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down\n  barn-303p.2c30-ap     ap     303P                             10.1.30.151       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82528   Up\n  barn-4100i            cx     4100i 12G CL4/6 POE 2SFP+ DIN    10.1.30.152       --redacted--   --redacted--    WadeLab        WadeLab                        10.08.1010       Up\n                               Sw (JL817A)\n  barn-518.2816-ap      ap     518                              10.1.30.101       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82528   Up\n  bsmt-515.51s9-ap      ap     515                              10.0.30.233       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down\n  craft-2930F           sw     Aruba2930F-8G-PoE+-2SFP+         10.0.30.5         --redacted--   --redacted--    WadeLab        WadeLab                        16.11.0002       Up\n                               Switch(JL258A)\n  garage-345.5136-ap    ap     345                              10.0.31.148       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down\n  ktcn-505H.206c-ap     ap     505H                             10.0.30.212       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down\n  lwrptio-575.0824-ap   ap     575                              10.0.30.219       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down\n  zrm-535.70be-ap       ap     535                              10.0.31.101       --redacted--   --redacted--    WLNET          WadeLab                        10.3.0.0_82463   Down\n ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────\n  Show all displays fields common to all device types. To see all columns for a given device type use show <DEVICE TYPE>\n  API Rate Limit: 925 of 1000 remaining.\n\n```\n\nUse `cencli ?` to become familiar with the command options.\n\n### Auto Completion\n\nThe CLI supports auto-completion.  To configure auto-completion run `cencli --install-completion`.  This will auto-detect the type of shell you are running in, and install the necessary completion into your profile.  You'll need to exit the shell and start a new session for it to take effect.\n\n## Usage Notes\n\n### Caching & Friendly identifiers\n\n- Caching: The CLI caches information on all devices, sites, groups, and templates in Central.  It's a minimal amount per device, and is done to allow human friendly identifiers.  The API typically accepts serial #, site id, etc.  This function allows you to specify a device by name, IP, mac (any format), and serial.\n\nThe lookup sequence for a device:\n\n  1. Exact Match of any of the identifier fields (name, ip, mac, serial)\n  2. case insensitive match\n  3. case insensitive match disregarding all hyphens and underscores (in case you type 6200f_bot and the device name is 6200F-Bot)\n  4. Case insensitive Fuzzy match with implied wild-card, otherwise match any devices that start with the identifier provided. `cencli show switches 6200F` will result in a match of `6200F-Bot`.\n\n> If there is no match found, a cache update is triggered, and the match rules are re-tried.\n\n- Caching works in a similar manner for groups, templates, and sites.  Sites can match on name and nearly any address field.  So if you only had one site in San Antonio you could specify that site with `show sites 'San Antonio'`  \\<-- Note the use of quotes because there is a space in the name.\n\n- **Multiple Matches**:  It's possible to specify an identifier that returns multiple matches (if drops all the way down to the Fuzzy match/implied trailing wild-card).  If that occurs you are prompted to select the intended device from a list of the matches.\n\n### Output Formats\n\nThere are a number of output formats available.  Most commands default to what is likely the easiest to view given the number of fields.  Otherwise longer outputs are typically displayed vertically by default.  If the output can reasonably fit, it's displayed in tabular format horizontally.\n\nYou can specify the output format with command line flags `--json`, `--yaml`, `--csv`, `--table`  rich is tabular format with folding (multi line within the same row) and truncating.\n\n> Most outputs will evolve to support an output with the most commonly desired fields by default and expanded vertical output via the `-v` option (not implemented yet.).  Currently the output is tabular horizontally if the amount of data is likely to fit most displays, and vertical otherwise.\n\n### File Output\n\nJust use `--out \\<filename\\>` (or \\<path\\\\filename\\>), and specify the desired format.\n\n## CLI Tree\n\nUse `?` or `--help` from the cli, which you can do at any level.  `ccenli ?`, `cencli bounce --help` etc.\n\nYou can also see the entire supported tree via the [CLI Reference Guide](https://central-api-cli.readthedocs.io/en/latest/cli.html).\n*NOTE: The Reference Guide documents a few commands that are hidden in the CLI*\n",
-    'author': 'Wade Wells (Pack3tL0ss)',
-    'author_email': 'wade@consolepi.org',
-    'maintainer': 'Wade Wells (Pack3tL0ss)',
-    'maintainer_email': 'wade@consolepi.org',
-    'url': 'https://github.com/Pack3tL0ss/central-api-cli',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+Use `?` or `--help` from the cli, which you can do at any level.  `ccenli ?`, `cencli bounce --help` etc.
 
+You can also see the entire supported tree via the [CLI Reference Guide](https://central-api-cli.readthedocs.io/en/latest/cli.html).
+*NOTE: The Reference Guide documents a few commands that are hidden in the CLI*
 
-setup(**setup_kwargs)
```

