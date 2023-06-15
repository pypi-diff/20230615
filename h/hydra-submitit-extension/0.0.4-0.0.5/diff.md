# Comparing `tmp/hydra_submitit_extension-0.0.4.tar.gz` & `tmp/hydra_submitit_extension-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra_submitit_extension-0.0.4.tar", last modified: Mon Jun 12 21:03:35 2023, max compression
+gzip compressed data, was "hydra_submitit_extension-0.0.5.tar", last modified: Thu Jun 15 21:05:22 2023, max compression
```

## Comparing `hydra_submitit_extension-0.0.4.tar` & `hydra_submitit_extension-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.420018 hydra_submitit_extension-0.0.4/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      607 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/.coveragerc
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      566 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/.gitignore
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      530 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/.readthedocs.yml
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       83 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/AUTHORS.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      115 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/CHANGELOG.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13698 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/CONTRIBUTING.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1079 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/LICENSE.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3479 2023-06-12 21:03:35.420018 hydra_submitit_extension-0.0.4/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3015 2023-06-12 19:09:50.000000 hydra_submitit_extension-0.0.4/README.md
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.416018 hydra_submitit_extension-0.0.4/docs/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1154 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/Makefile
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.416018 hydra_submitit_extension-0.0.4/docs/_static/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       18 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/_static/.gitignore
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       71 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/authors.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       73 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/changelog.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10109 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/conf.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       76 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/contributing.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      969 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/index.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       66 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/license.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       70 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/readme.md
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      254 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/docs/requirements.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      346 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/pyproject.toml
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1245 2023-06-12 21:03:35.424018 hydra_submitit_extension-0.0.4/setup.cfg
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      721 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/setup.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.412018 hydra_submitit_extension-0.0.4/src/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.412018 hydra_submitit_extension-0.0.4/src/hydra_plugins/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.420018 hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      577 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      968 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/config.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6931 2023-06-12 20:55:21.000000 hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/submitit_launcher.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.420018 hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/utils/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      612 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/utils/slurm_info.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.420018 hydra_submitit_extension-0.0.4/src/hydra_submitit_extension.egg-info/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3479 2023-06-12 21:03:35.000000 hydra_submitit_extension-0.0.4/src/hydra_submitit_extension.egg-info/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      982 2023-06-12 21:03:35.000000 hydra_submitit_extension-0.0.4/src/hydra_submitit_extension.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-06-12 21:03:35.000000 hydra_submitit_extension-0.0.4/src/hydra_submitit_extension.egg-info/dependency_links.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-06-12 13:13:11.000000 hydra_submitit_extension-0.0.4/src/hydra_submitit_extension.egg-info/not-zip-safe
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      120 2023-06-12 21:03:35.000000 hydra_submitit_extension-0.0.4/src/hydra_submitit_extension.egg-info/requires.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       14 2023-06-12 21:03:35.000000 hydra_submitit_extension-0.0.4/src/hydra_submitit_extension.egg-info/top_level.txt
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.420018 hydra_submitit_extension-0.0.4/tests/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.420018 hydra_submitit_extension-0.0.4/tests/conf/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      288 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.4/tests/conf/config.yaml
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-12 21:03:35.420018 hydra_submitit_extension-0.0.4/tests/conf/slurm/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      653 2023-06-12 12:38:44.000000 hydra_submitit_extension-0.0.4/tests/conf/slurm/cpu.yaml
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      292 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/tests/conftest.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      601 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/tests/test_skeleton.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      492 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.4/tests/test_submtit_launcher.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2851 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.4/tox.ini
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      607 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/.coveragerc
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      566 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/.gitignore
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      530 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/.readthedocs.yml
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       83 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/AUTHORS.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      115 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/CHANGELOG.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    13698 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/CONTRIBUTING.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1079 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/LICENSE.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3479 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3015 2023-06-12 19:09:50.000000 hydra_submitit_extension-0.0.5/README.md
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/docs/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1154 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/Makefile
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/docs/_static/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       18 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/_static/.gitignore
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       71 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/authors.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       73 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/changelog.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)    10109 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/conf.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       76 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/contributing.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      969 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/index.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       66 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/license.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       70 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/readme.md
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      254 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/docs/requirements.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      346 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/pyproject.toml
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     1245 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/setup.cfg
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      721 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/setup.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.480230 hydra_submitit_extension-0.0.5/src/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.480230 hydra_submitit_extension-0.0.5/src/hydra_plugins/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      577 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/__init__.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      880 2023-06-13 22:12:42.000000 hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/config.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     4729 2023-06-15 21:03:24.000000 hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/submitit_launcher.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/utils/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      612 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/utils/slurm_info.py
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/src/hydra_submitit_extension.egg-info/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     3479 2023-06-15 21:05:22.000000 hydra_submitit_extension-0.0.5/src/hydra_submitit_extension.egg-info/PKG-INFO
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      982 2023-06-15 21:05:22.000000 hydra_submitit_extension-0.0.5/src/hydra_submitit_extension.egg-info/SOURCES.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-06-15 21:05:22.000000 hydra_submitit_extension-0.0.5/src/hydra_submitit_extension.egg-info/dependency_links.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2023-06-12 13:13:11.000000 hydra_submitit_extension-0.0.5/src/hydra_submitit_extension.egg-info/not-zip-safe
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      120 2023-06-15 21:05:22.000000 hydra_submitit_extension-0.0.5/src/hydra_submitit_extension.egg-info/requires.txt
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)       14 2023-06-15 21:05:22.000000 hydra_submitit_extension-0.0.5/src/hydra_submitit_extension.egg-info/top_level.txt
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/tests/
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/tests/conf/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      288 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.5/tests/conf/config.yaml
+drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2023-06-15 21:05:22.484230 hydra_submitit_extension-0.0.5/tests/conf/slurm/
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      653 2023-06-12 12:38:44.000000 hydra_submitit_extension-0.0.5/tests/conf/slurm/cpu.yaml
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      292 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/tests/conftest.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      601 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/tests/test_skeleton.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)      492 2023-06-11 14:39:09.000000 hydra_submitit_extension-0.0.5/tests/test_submtit_launcher.py
+-rw-rw-r--   0 stefan    (1000) stefan    (1000)     2851 2023-06-07 14:29:09.000000 hydra_submitit_extension-0.0.5/tox.ini
```

### Comparing `hydra_submitit_extension-0.0.4/.coveragerc` & `hydra_submitit_extension-0.0.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/.gitignore` & `hydra_submitit_extension-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/.readthedocs.yml` & `hydra_submitit_extension-0.0.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/CONTRIBUTING.md` & `hydra_submitit_extension-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/LICENSE.txt` & `hydra_submitit_extension-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/PKG-INFO` & `hydra_submitit_extension-0.0.5/src/hydra_submitit_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hydra_submitit_extension
-Version: 0.0.4
+Name: hydra-submitit-extension
+Version: 0.0.5
 Summary: A more flexible hydra submitit launcher
 Home-page: https://github.com/caplett/hydra_submitit_extension
 Author: Stefan Geyer
 Author-email: git@caplett.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hydra_submitit_extension-0.0.4/README.md` & `hydra_submitit_extension-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/docs/Makefile` & `hydra_submitit_extension-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/docs/conf.py` & `hydra_submitit_extension-0.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/docs/index.md` & `hydra_submitit_extension-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/setup.cfg` & `hydra_submitit_extension-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/setup.py` & `hydra_submitit_extension-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/__init__.py` & `hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/config.py` & `hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional
+from typing import Optional
 
 from hydra.core.config_store import ConfigStore
 
 from hydra_plugins.hydra_submitit_launcher.config import SlurmQueueConf
 
 @dataclass
 class ExtendedSlurmQueueConf(SlurmQueueConf):
```

### Comparing `hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/submitit_launcher.py` & `hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/submitit_launcher.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,28 @@
-# Copyright (c) Facebook, Inc. and its affiliates. All Rights Reserved
 import logging
 import os
 import time
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Set, Optional, Sequence
+from typing import Any, List, Set, Sequence
 
 from hydra.core.singleton import Singleton
-from hydra.core.utils import JobReturn, filter_overrides, run_job, setup_globals, JobStatus
-from hydra.types import HydraContext, TaskFunction
-from omegaconf import DictConfig, OmegaConf, open_dict
+from hydra.core.utils import JobReturn, filter_overrides, JobStatus
+from omegaconf import OmegaConf
 
 from hydra_plugins.hydra_submitit_launcher.submitit_launcher import SlurmLauncher
 from submitit.core.core import Job
 from hydra_plugins.hydra_submitit_extension.config import ExtendedSlurmQueueConf
 from hydra_plugins.hydra_submitit_extension.utils.slurm_info import QueueInfo
 
 log = logging.getLogger(__name__)
 
 class ExtendedSlurmLauncher(SlurmLauncher):
     ACTIVE_JOB_STATES = ["RUNNING","PENDING","UNKNOWN"]
 
-    def __init__(self, **params: Any) -> None:
-        self.params = {}
-        for k, v in params.items():
-            if OmegaConf.is_config(v):
-                v = OmegaConf.to_container(v, resolve=True)
-            self.params[k] = v
-
-        self.config: Optional[DictConfig] = None
-        self.task_function: Optional[TaskFunction] = None
-        self.sweep_configs: Optional[TaskFunction] = None
-        self.hydra_context: Optional[HydraContext] = None
-
-    def setup(
-        self,
-        *,
-        hydra_context: HydraContext,
-        task_function: TaskFunction,
-        config: DictConfig,
-    ) -> None:
-        self.config = config
-        self.hydra_context = hydra_context
-        self.task_function = task_function
-
-    def __call__(
-        self,
-        sweep_overrides: List[str],
-        job_dir_key: str,
-        job_num: int,
-        job_id: str,
-        singleton_state: Dict[type, Singleton],
-    ) -> JobReturn:
-        # lazy import to ensure plugin discovery remains fast
-        import submitit
-
-        assert self.hydra_context is not None
-        assert self.config is not None
-        assert self.task_function is not None
-
-        Singleton.set_state(singleton_state)
-        setup_globals()
-        sweep_config = self.hydra_context.config_loader.load_sweep_config(
-            self.config, sweep_overrides
-        )
-
-        with open_dict(sweep_config.hydra.job) as job:
-            # Populate new job variables
-            job.id = submitit.JobEnvironment().job_id  # type: ignore
-            sweep_config.hydra.job.num = job_num
-
-        return run_job(
-            hydra_context=self.hydra_context,
-            task_function=self.task_function,
-            config=sweep_config,
-            job_dir_key=job_dir_key,
-            job_subdir_key="hydra.sweep.subdir",
-        )
-
-    def checkpoint(self, *args: Any, **kwargs: Any) -> Any:
-        """Resubmit the current callable at its current state with the same initial arguments."""
-        # lazy import to ensure plugin discovery remains fast
-        import submitit
-
-        return submitit.helpers.DelayedSubmission(self, *args, **kwargs)
-
     def launch(
         self, job_overrides: Sequence[Sequence[str]], initial_job_idx: int
     ) -> Sequence[JobReturn]:
         # lazy import to ensure plugin discovery remains fast
         import submitit
 
         assert self.config is not None
@@ -169,14 +103,18 @@
                 if len(job_params)!=0:
                     queue_info = QueueInfo()
                     if queue_info.getTotalJobs() < params["max_jobs_in_total"]:
                         if queue_info.getJobsInPartition(params["partition"]) < params["max_jobs_in_partition"]:
                             jp = job_params.pop(0)
                             all_jobs.append(executor.submit(self, *jp))
                             log.info(f"\t#{jp[2]} : Scheduled")
+                        else:
+                            break
+                    else:
+                        break
                     # Dont overrun the scheduler
                     time.sleep(1)
                 else:
                     break
 
             for i in set(all_jobs) - finished_jobs: 
                 if i.state not in self.ACTIVE_JOB_STATES:
```

### Comparing `hydra_submitit_extension-0.0.4/src/hydra_plugins/hydra_submitit_extension/utils/slurm_info.py` & `hydra_submitit_extension-0.0.5/src/hydra_plugins/hydra_submitit_extension/utils/slurm_info.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/src/hydra_submitit_extension.egg-info/PKG-INFO` & `hydra_submitit_extension-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hydra-submitit-extension
-Version: 0.0.4
+Name: hydra_submitit_extension
+Version: 0.0.5
 Summary: A more flexible hydra submitit launcher
 Home-page: https://github.com/caplett/hydra_submitit_extension
 Author: Stefan Geyer
 Author-email: git@caplett.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `hydra_submitit_extension-0.0.4/src/hydra_submitit_extension.egg-info/SOURCES.txt` & `hydra_submitit_extension-0.0.5/src/hydra_submitit_extension.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/tests/conf/slurm/cpu.yaml` & `hydra_submitit_extension-0.0.5/tests/conf/slurm/cpu.yaml`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/tests/test_skeleton.py` & `hydra_submitit_extension-0.0.5/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `hydra_submitit_extension-0.0.4/tox.ini` & `hydra_submitit_extension-0.0.5/tox.ini`

 * *Files identical despite different names*

