# Comparing `tmp/stellanow_cli-0.0.1.tar.gz` & `tmp/stellanow_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellanow_cli-0.0.1.tar", last modified: Thu Jun 15 15:35:44 2023, max compression
+gzip compressed data, was "stellanow_cli-0.0.2.tar", last modified: Thu Jun 15 21:08:47 2023, max compression
```

## Comparing `stellanow_cli-0.0.1.tar` & `stellanow_cli-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 15:35:44.600986 stellanow_cli-0.0.1/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       83 2023-06-15 15:35:44.599146 stellanow_cli-0.0.1/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1761 2023-06-15 14:56:57.000000 stellanow_cli-0.0.1/README.md
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-15 15:35:44.601058 stellanow_cli-0.0.1/setup.cfg
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      420 2023-06-10 20:20:54.000000 stellanow_cli-0.0.1/setup.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 15:35:44.324656 stellanow_cli-0.0.1/stellanow_cli/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        0 2023-06-04 15:58:17.000000 stellanow_cli-0.0.1/stellanow_cli/__init__.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 15:35:44.453184 stellanow_cli-0.0.1/stellanow_cli/api/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       98 2023-06-10 09:11:51.000000 stellanow_cli-0.0.1/stellanow_cli/api/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     6159 2023-06-15 09:04:10.000000 stellanow_cli-0.0.1/stellanow_cli/api/stellanow_api.py
--rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1002 2023-06-05 21:47:35.000000 stellanow_cli-0.0.1/stellanow_cli/cli.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 15:35:44.483265 stellanow_cli-0.0.1/stellanow_cli/code_generators/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       79 2023-06-10 16:45:11.000000 stellanow_cli-0.0.1/stellanow_cli/code_generators/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1135 2023-06-10 20:04:26.000000 stellanow_cli-0.0.1/stellanow_cli/code_generators/code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     2861 2023-06-15 09:34:56.000000 stellanow_cli-0.0.1/stellanow_cli/code_generators/csharp_code_generator.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     3532 2023-06-15 00:09:35.000000 stellanow_cli-0.0.1/stellanow_cli/command_config.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 15:35:44.555812 stellanow_cli-0.0.1/stellanow_cli/config/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      185 2023-06-14 23:23:00.000000 stellanow_cli-0.0.1/stellanow_cli/config/__init__.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      521 2023-06-14 23:51:50.000000 stellanow_cli-0.0.1/stellanow_cli/config/config.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      155 2023-06-14 22:55:16.000000 stellanow_cli-0.0.1/stellanow_cli/config/dev.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      151 2023-06-14 22:54:59.000000 stellanow_cli-0.0.1/stellanow_cli/config/int.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      555 2023-06-08 21:03:54.000000 stellanow_cli-0.0.1/stellanow_cli/logger.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      362 2023-06-15 09:34:56.000000 stellanow_cli-0.0.1/stellanow_cli/utils.py
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      473 2023-06-04 23:32:41.000000 stellanow_cli-0.0.1/stellanow_cli/validate.py
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 15:35:44.431335 stellanow_cli-0.0.1/stellanow_cli.egg-info/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       83 2023-06-15 15:35:43.000000 stellanow_cli-0.0.1/stellanow_cli.egg-info/PKG-INFO
--rw-r--r--   0 tom-kandziora   (501) staff       (20)      756 2023-06-15 15:35:44.000000 stellanow_cli-0.0.1/stellanow_cli.egg-info/SOURCES.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-15 15:35:43.000000 stellanow_cli-0.0.1/stellanow_cli.egg-info/dependency_links.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-15 15:35:43.000000 stellanow_cli-0.0.1/stellanow_cli.egg-info/entry_points.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-15 15:35:43.000000 stellanow_cli-0.0.1/stellanow_cli.egg-info/requires.txt
--rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-15 15:35:43.000000 stellanow_cli-0.0.1/stellanow_cli.egg-info/top_level.txt
-drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 15:35:44.596476 stellanow_cli-0.0.1/tests/
--rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.1/tests/test_command_configure.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.175656 stellanow_cli-0.0.2/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7787 2023-06-15 21:08:47.174300 stellanow_cli-0.0.2/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1761 2023-06-15 20:48:36.000000 stellanow_cli-0.0.2/README.md
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       38 2023-06-15 21:08:47.175822 stellanow_cli-0.0.2/setup.cfg
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      935 2023-06-15 21:02:18.000000 stellanow_cli-0.0.2/setup.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:46.927672 stellanow_cli-0.0.2/stellanow_cli/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      322 2023-06-15 20:52:42.000000 stellanow_cli-0.0.2/stellanow_cli/__init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       22 2023-06-15 21:00:57.000000 stellanow_cli-0.0.2/stellanow_cli/_version.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.036609 stellanow_cli-0.0.2/stellanow_cli/api/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      422 2023-06-15 20:54:39.000000 stellanow_cli-0.0.2/stellanow_cli/api/__init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     6483 2023-06-15 20:54:33.000000 stellanow_cli-0.0.2/stellanow_cli/api/stellanow_api.py
+-rwxr-xr-x   0 tom-kandziora   (501) staff       (20)     1354 2023-06-15 21:06:20.000000 stellanow_cli-0.0.2/stellanow_cli/cli.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.109286 stellanow_cli-0.0.2/stellanow_cli/code_generators/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      403 2023-06-15 20:54:24.000000 stellanow_cli-0.0.2/stellanow_cli/code_generators/__init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1459 2023-06-15 20:54:18.000000 stellanow_cli-0.0.2/stellanow_cli/code_generators/code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3185 2023-06-15 20:54:11.000000 stellanow_cli-0.0.2/stellanow_cli/code_generators/csharp_code_generator.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     3856 2023-06-15 20:52:20.000000 stellanow_cli-0.0.2/stellanow_cli/command_config.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.161181 stellanow_cli-0.0.2/stellanow_cli/config/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      509 2023-06-15 20:53:06.000000 stellanow_cli-0.0.2/stellanow_cli/config/__init__.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      845 2023-06-15 20:53:01.000000 stellanow_cli-0.0.2/stellanow_cli/config/config.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      479 2023-06-15 20:52:56.000000 stellanow_cli-0.0.2/stellanow_cli/config/dev.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      475 2023-06-15 20:52:51.000000 stellanow_cli-0.0.2/stellanow_cli/config/int.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      879 2023-06-15 20:52:13.000000 stellanow_cli-0.0.2/stellanow_cli/logger.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      686 2023-06-15 20:51:44.000000 stellanow_cli-0.0.2/stellanow_cli/utils.py
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      797 2023-06-15 20:51:30.000000 stellanow_cli-0.0.2/stellanow_cli/validate.py
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.007513 stellanow_cli-0.0.2/stellanow_cli.egg-info/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     7787 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/PKG-INFO
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)      782 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)        1 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       52 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/entry_points.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       46 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/requires.txt
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)       14 2023-06-15 21:08:46.000000 stellanow_cli-0.0.2/stellanow_cli.egg-info/top_level.txt
+drwxr-xr-x   0 tom-kandziora   (501) staff       (20)        0 2023-06-15 21:08:47.170423 stellanow_cli-0.0.2/tests/
+-rw-r--r--   0 tom-kandziora   (501) staff       (20)     1762 2023-06-05 08:22:00.000000 stellanow_cli-0.0.2/tests/test_command_configure.py
```

### Comparing `stellanow_cli-0.0.1/README.md` & `stellanow_cli-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stellanow_cli-0.0.1/stellanow_cli/api/stellanow_api.py` & `stellanow_cli-0.0.2/stellanow_cli/api/stellanow_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+Copyright (C) 2022-2023 Stella Technologies (UK) Limited.
+
+This software is the proprietary information of Stella Technologies (UK) Limited.
+Use, reproduction, or redistribution of this software is strictly prohibited without
+the express written permission of Stella Technologies (UK) Limited.
+All rights reserved.
+"""
+
 import json
 import requests
 
 from dataclasses import dataclass
 from sys import maxsize
 from typing import Generator, List
```

### Comparing `stellanow_cli-0.0.1/stellanow_cli/code_generators/csharp_code_generator.py` & `stellanow_cli-0.0.2/stellanow_cli/code_generators/csharp_code_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+Copyright (C) 2022-2023 Stella Technologies (UK) Limited.
+
+This software is the proprietary information of Stella Technologies (UK) Limited.
+Use, reproduction, or redistribution of this software is strictly prohibited without
+the express written permission of Stella Technologies (UK) Limited.
+All rights reserved.
+"""
+
 import difflib
 import json
 import re
 
 from dataclasses import asdict
 from datetime import datetime
 from typing import Iterator
```

### Comparing `stellanow_cli-0.0.1/stellanow_cli/command_config.py` & `stellanow_cli-0.0.2/stellanow_cli/command_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+Copyright (C) 2022-2023 Stella Technologies (UK) Limited.
+
+This software is the proprietary information of Stella Technologies (UK) Limited.
+Use, reproduction, or redistribution of this software is strictly prohibited without
+the express written permission of Stella Technologies (UK) Limited.
+All rights reserved.
+"""
+
 import click
 import functools
 import os
 
 from .api import StellaAPI
 from .logger import setup_logger, logger
 from .utils import snake_to_camel
```

### Comparing `stellanow_cli-0.0.1/stellanow_cli/config/config.py` & `stellanow_cli-0.0.2/stellanow_cli/config/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+"""
+Copyright (C) 2022-2023 Stella Technologies (UK) Limited.
+
+This software is the proprietary information of Stella Technologies (UK) Limited.
+Use, reproduction, or redistribution of this software is strictly prohibited without
+the express written permission of Stella Technologies (UK) Limited.
+All rights reserved.
+"""
+
 from dataclasses import dataclass
 
 
 @dataclass
 class Config:
     base_url: str = ""
```

### Comparing `stellanow_cli-0.0.1/stellanow_cli.egg-info/SOURCES.txt` & `stellanow_cli-0.0.2/stellanow_cli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 stellanow_cli/__init__.py
+stellanow_cli/_version.py
 stellanow_cli/cli.py
 stellanow_cli/command_config.py
 stellanow_cli/logger.py
 stellanow_cli/utils.py
 stellanow_cli/validate.py
 stellanow_cli.egg-info/PKG-INFO
 stellanow_cli.egg-info/SOURCES.txt
```

### Comparing `stellanow_cli-0.0.1/tests/test_command_configure.py` & `stellanow_cli-0.0.2/tests/test_command_configure.py`

 * *Files identical despite different names*

