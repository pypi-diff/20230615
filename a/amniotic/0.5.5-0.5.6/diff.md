# Comparing `tmp/amniotic-0.5.5.tar.gz` & `tmp/amniotic-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amniotic-0.5.5.tar", last modified: Thu Jan  5 12:39:16 2023, max compression
+gzip compressed data, was "amniotic-0.5.6.tar", last modified: Thu Jun 15 14:34:41 2023, max compression
```

## Comparing `amniotic-0.5.5.tar` & `amniotic-0.5.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 12:39:16.879565 amniotic-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-01-05 12:39:16.875565 amniotic-0.5.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 12:39:16.875565 amniotic-0.5.5/amniotic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20096 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 12:39:16.875565 amniotic-0.5.5/amniotic/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/mqtt/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/mqtt/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/mqtt/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/mqtt/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/mqtt/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-01-05 12:39:12.000000 amniotic-0.5.5/amniotic/version
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-05 12:39:08.000000 amniotic-0.5.5/amniotic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 12:39:16.875565 amniotic-0.5.5/amniotic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-01-05 12:39:16.000000 amniotic-0.5.5/amniotic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-05 12:39:16.000000 amniotic-0.5.5/amniotic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 12:39:16.000000 amniotic-0.5.5/amniotic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-01-05 12:39:16.000000 amniotic-0.5.5/amniotic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-05 12:39:16.000000 amniotic-0.5.5/amniotic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-05 12:39:16.000000 amniotic-0.5.5/amniotic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 12:39:16.879565 amniotic-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-05 12:39:08.000000 amniotic-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:41.897549 amniotic-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-15 14:34:41.897549 amniotic-0.5.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:41.893549 amniotic-0.5.6/amniotic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:41.897549 amniotic-0.5.6/amniotic/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 14:34:38.000000 amniotic-0.5.6/amniotic/version
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:41.893549 amniotic-0.5.6/amniotic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:34:41.897549 amniotic-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-15 14:34:32.000000 amniotic-0.5.6/setup.py
```

### Comparing `amniotic-0.5.5/PKG-INFO` & `amniotic-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amniotic
-Version: 0.5.5
+Version: 0.5.6
 Summary: A multi-output ambient sound mixer for Home Assistant
 Home-page: https://link.frontmatter.ai/amniotic
 Author: Frontmatter
 License: Copyright © 2022 Frontmatter. All rights reserved.
 Keywords: ambient sound audio white noise masking sleep
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `amniotic-0.5.5/amniotic/audio.py` & `amniotic-0.5.6/amniotic/audio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from itertools import cycle
+
 import getpass
 import logging
 import vlc
 from cachetools.func import ttl_cache
 from copy import deepcopy
 from datetime import datetime
-from itertools import cycle
 from numbers import Number
 from pathlib import Path
 from random import choice
 from typing import Union, Optional, Dict
 
 VLC_VERBOSITY = 0
 DEVICES_POLL_PERIOD_SECONDS = 10
@@ -91,15 +92,15 @@
     value = round(value)
     value = min(value, 100)
     value = max(value, 0)
     return value
 
 
 class Amniotic:
-    VOLUME_DEFAULT = 50
+    VOLUME_DEFAULT = 10
     THEME_NAME_DEFAULT = 'Default Theme'
 
     def __init__(self, path: Union[Path, str], device_names: Optional[dict[str, str]] = None, presets: Dict = None):
         """
 
         Read audio directories and instantiate Theme objects
```

### Comparing `amniotic-0.5.5/amniotic/config.py` & `amniotic-0.5.6/amniotic/config.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.5/amniotic/mqtt/control.py` & `amniotic-0.5.6/amniotic/mqtt/control.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.5/amniotic/mqtt/device.py` & `amniotic-0.5.6/amniotic/mqtt/device.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.5/amniotic/mqtt/loop.py` & `amniotic-0.5.6/amniotic/mqtt/loop.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.5/amniotic/mqtt/sensor.py` & `amniotic-0.5.6/amniotic/mqtt/sensor.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.5/amniotic/mqtt/tools.py` & `amniotic-0.5.6/amniotic/mqtt/tools.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.5/amniotic.egg-info/PKG-INFO` & `amniotic-0.5.6/amniotic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amniotic
-Version: 0.5.5
+Version: 0.5.6
 Summary: A multi-output ambient sound mixer for Home Assistant
 Home-page: https://link.frontmatter.ai/amniotic
 Author: Frontmatter
 License: Copyright © 2022 Frontmatter. All rights reserved.
 Keywords: ambient sound audio white noise masking sleep
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `amniotic-0.5.5/setup.py` & `amniotic-0.5.6/setup.py`

 * *Files identical despite different names*

