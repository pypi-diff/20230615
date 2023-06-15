# Comparing `tmp/bluesky-darkframes-0.5.0.tar.gz` & `tmp/bluesky-darkframes-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluesky-darkframes-0.5.0.tar", last modified: Fri Oct  8 19:27:10 2021, max compression
+gzip compressed data, was "bluesky-darkframes-0.6.0.tar", last modified: Thu Jun 15 15:37:16 2023, max compression
```

## Comparing `bluesky-darkframes-0.5.0.tar` & `bluesky-darkframes-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-08 19:27:10.211244 bluesky-darkframes-0.5.0/
--rw-r--r--   0 joshualynch   (503) staff       (20)      173 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/AUTHORS.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)     3144 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)     1557 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/LICENSE
--rw-r--r--   0 joshualynch   (503) staff       (20)      371 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/MANIFEST.in
--rw-r--r--   0 joshualynch   (503) staff       (20)     1033 2021-10-08 19:27:10.211357 bluesky-darkframes-0.5.0/PKG-INFO
--rw-r--r--   0 joshualynch   (503) staff       (20)      545 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/README.rst
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-08 19:27:10.212068 bluesky-darkframes-0.5.0/bluesky_darkframes/
--rw-r--r--   0 joshualynch   (503) staff       (20)    21374 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/bluesky_darkframes/__init__.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      497 2021-10-08 19:27:10.212139 bluesky-darkframes-0.5.0/bluesky_darkframes/_version.py
--rw-r--r--   0 joshualynch   (503) staff       (20)     4447 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/bluesky_darkframes/sim.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-08 19:27:10.207958 bluesky-darkframes-0.5.0/bluesky_darkframes/tests/
--rw-r--r--   0 joshualynch   (503) staff       (20)        0 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/bluesky_darkframes/tests/__init__.py
--rw-r--r--   0 joshualynch   (503) staff       (20)       46 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/bluesky_darkframes/tests/conftest.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    11145 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/bluesky_darkframes/tests/tests.py
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-08 19:27:10.207023 bluesky-darkframes-0.5.0/bluesky_darkframes.egg-info/
--rw-r--r--   0 joshualynch   (503) staff       (20)     1033 2021-10-08 19:27:09.000000 bluesky-darkframes-0.5.0/bluesky_darkframes.egg-info/PKG-INFO
--rw-r--r--   0 joshualynch   (503) staff       (20)      738 2021-10-08 19:27:09.000000 bluesky-darkframes-0.5.0/bluesky_darkframes.egg-info/SOURCES.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)        1 2021-10-08 19:27:09.000000 bluesky-darkframes-0.5.0/bluesky_darkframes.egg-info/dependency_links.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)       20 2021-10-08 19:27:09.000000 bluesky-darkframes-0.5.0/bluesky_darkframes.egg-info/entry_points.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)       45 2021-10-08 19:27:09.000000 bluesky-darkframes-0.5.0/bluesky_darkframes.egg-info/requires.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)       19 2021-10-08 19:27:09.000000 bluesky-darkframes-0.5.0/bluesky_darkframes.egg-info/top_level.txt
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-08 19:27:10.208715 bluesky-darkframes-0.5.0/docs/
--rw-r--r--   0 joshualynch   (503) staff       (20)      673 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/docs/Makefile
--rw-r--r--   0 joshualynch   (503) staff       (20)      797 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/docs/make.bat
-drwxr-xr-x   0 joshualynch   (503) staff       (20)        0 2021-10-08 19:27:10.210906 bluesky-darkframes-0.5.0/docs/source/
--rw-r--r--   0 joshualynch   (503) staff       (20)     6467 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/docs/source/conf.py
--rw-r--r--   0 joshualynch   (503) staff       (20)      392 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/docs/source/index.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)      100 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/docs/source/installation.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)      402 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/docs/source/reference.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)     4080 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/docs/source/release-history.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)     9641 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/docs/source/usage.rst
--rw-r--r--   0 joshualynch   (503) staff       (20)       46 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/requirements.txt
--rw-r--r--   0 joshualynch   (503) staff       (20)      200 2021-10-08 19:27:10.211796 bluesky-darkframes-0.5.0/setup.cfg
--rw-r--r--   0 joshualynch   (503) staff       (20)     2185 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/setup.py
--rw-r--r--   0 joshualynch   (503) staff       (20)    68611 2021-10-08 16:36:21.000000 bluesky-darkframes-0.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:16.429405 bluesky-darkframes-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-15 15:37:16.429405 bluesky-darkframes-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:16.433405 bluesky-darkframes-0.6.0/bluesky_darkframes/
+-rw-r--r--   0 runner    (1001) docker     (123)    21672 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/bluesky_darkframes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 15:37:16.433405 bluesky-darkframes-0.6.0/bluesky_darkframes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/bluesky_darkframes/sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:16.429405 bluesky-darkframes-0.6.0/bluesky_darkframes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/bluesky_darkframes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/bluesky_darkframes/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/bluesky_darkframes/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:16.429405 bluesky-darkframes-0.6.0/bluesky_darkframes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-15 15:37:16.000000 bluesky-darkframes-0.6.0/bluesky_darkframes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 15:37:16.000000 bluesky-darkframes-0.6.0/bluesky_darkframes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:37:16.000000 bluesky-darkframes-0.6.0/bluesky_darkframes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 15:37:16.000000 bluesky-darkframes-0.6.0/bluesky_darkframes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 15:37:16.000000 bluesky-darkframes-0.6.0/bluesky_darkframes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:16.429405 bluesky-darkframes-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:37:16.429405 bluesky-darkframes-0.6.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-15 15:37:16.429405 bluesky-darkframes-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68503 2023-06-15 15:37:13.000000 bluesky-darkframes-0.6.0/versioneer.py
```

### Comparing `bluesky-darkframes-0.5.0/CONTRIBUTING.rst` & `bluesky-darkframes-0.6.0/CONTRIBUTING.rst`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,7 @@
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put
    your new functionality into a function with a docstring, and add the
    feature to the list in README.rst.
 3. The pull request should work for Python 2.7, 3.3, 3.4, 3.5 and for PyPy. Check
    https://travis-ci.org/bluesky/bluesky-darkframes/pull_requests
    and make sure that the tests pass for all supported Python versions.
-
```

### Comparing `bluesky-darkframes-0.5.0/LICENSE` & `bluesky-darkframes-0.6.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
+BSD 3-Clause License
+
 Copyright (c) 2019, Brookhaven National Lab
-Laboratory. All rights reserved.
+All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
 
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-* Neither the name of the Brookhaven Science Associates, Brookhaven National
-  Laboratory nor the names of its contributors may be used to endorse or promote
-  products derived from this software without specific prior written permission.
+3. Neither the name of the copyright holder nor the names of its contributors
+   may be used to endorse or promote products derived from this software
+   without specific prior written permission.
 
 THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `bluesky-darkframes-0.5.0/PKG-INFO` & `bluesky-darkframes-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: bluesky-darkframes
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools for acquiring and subtracting darkframes
 Home-page: https://github.com/bluesky/bluesky-darkframes
 Author: Brookhaven National Lab
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-===============================
+==================
 Bluesky Darkframes
-===============================
+==================
+
+.. image:: https://github.com/bluesky/bluesky-darkframes/actions/workflows/testing.yml/badge.svg
+   :target: https://github.com/bluesky/bluesky-darkframes/actions/workflows/testing.yml
 
-.. image:: https://img.shields.io/travis/bluesky/bluesky-darkframes.svg
-        :target: https://travis-ci.org/bluesky/bluesky-darkframes
 
 .. image:: https://img.shields.io/pypi/v/bluesky-darkframes.svg
         :target: https://pypi.python.org/pypi/bluesky-darkframes
 
 
 Tools for acquiring and subtracting darkframes
 
 * Free software: 3-clause BSD license
 * Documentation: (COMING SOON!) https://bluesky.github.io/bluesky-darkframes.
 
 Features
 --------
 
 * TODO
-
-
```

### Comparing `bluesky-darkframes-0.5.0/bluesky_darkframes/__init__.py` & `bluesky-darkframes-0.6.0/bluesky_darkframes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,38 +3,40 @@
 import functools
 import inspect
 import logging
 import time
 import uuid
 import warnings
 
-import event_model
-from frozendict import frozendict
-import bluesky.preprocessors
 import bluesky.plan_stubs as bps
+import bluesky.preprocessors
+import event_model
+import numpy as np
 from bluesky.utils import short_uid
-import numpy
+from frozendict import frozendict
 from ophyd import Device
 
 from ._version import get_versions
-__version__ = get_versions()['version']
+
+__version__ = get_versions()["version"]
 del get_versions
 
 
-logger = logging.getLogger('bluesky.darkframes')
+logger = logging.getLogger("bluesky.darkframes")
 
 
 class SnapshotDevice(Device):
     """
     A mock Device that stashes a snapshot of another Device for later reading
 
     Parameters
     ----------
     device: Device
     """
+
     def __init__(self, device):
         super().__init__(name=device.name, parent=device.parent)
 
         self._describe = device.describe()
         self._describe_configuration = device.describe_configuration()
         self._read = device.read()
         self._read_configuration = device.read_configuration()
@@ -90,43 +92,43 @@
 
         - Make shallow copies of Resource and Datum docs with new unique identifiers.
         - Update the return value of read() with the new datum_ids.
         """
         resources = {}  # map old uid to new uid
         new_asset_docs_cache = []
         for name, doc in self._asset_docs_cache:
-            if name == 'resource':
+            if name == "resource":
                 new_uid = str(uuid.uuid4())
-                resources[doc['uid']] = new_uid
+                resources[doc["uid"]] = new_uid
                 new_doc = doc.copy()
-                new_doc['uid'] = new_uid
+                new_doc["uid"] = new_uid
                 new_asset_docs_cache.append((name, new_doc))
-            elif name == 'datum':
+            elif name == "datum":
                 new_doc = doc.copy()
-                old_resource_uid = doc['resource']
+                old_resource_uid = doc["resource"]
                 new_resource_uid = resources[old_resource_uid]
-                new_doc['resource'] = new_resource_uid
+                new_doc["resource"] = new_resource_uid
                 # Some existing code in other libraries looks for the
                 # {resource_uid}/{integer} pattern in Event documents and uses that
                 # to take a fast path. The changes to Datum proposed in
                 # https://github.com/bluesky/event-model/issues/156
                 # would make this less fragile.
-                old_datum_id = doc['datum_id']
+                old_datum_id = doc["datum_id"]
                 if old_datum_id.startswith(f"{old_resource_uid}/"):
-                    _, suffix = old_datum_id.split('/', 1)
+                    _, suffix = old_datum_id.split("/", 1)
                     new_datum_id = f"{new_resource_uid}/{suffix}"
                 else:
                     new_datum_id = str(uuid.uuid4())
-                new_doc['datum_id'] = new_datum_id
+                new_doc["datum_id"] = new_datum_id
                 new_asset_docs_cache.append((name, new_doc))
                 # Update the return value of read() to replace the old datum_id
                 # with the new one.
                 for k, v in list(self._read.items()):
-                    if v['value'] == old_datum_id:
-                        self._read[k]['value'] = new_datum_id
+                    if v["value"] == old_datum_id:
+                        self._read[k]["value"] = new_datum_id
             else:
                 raise BlueskyDarkframesValueError(f"Unexpected name {name}")
         self._asset_docs_cache = new_asset_docs_cache
 
 
 class _SnapshotShell:
     # This enables us to hot-swap Snapshot instances in the middle of a Run.
@@ -137,19 +139,38 @@
 
     def set_snaphsot(self, snapshot):
         self.__snapshot = snapshot
 
     def get_snapshot(self):
         return self.__snapshot
 
+    def describe(self):
+        return self.__snapshot.describe()
+
+    def describe_configuration(self):
+        return self.__snapshot.describe_configuration()
+
+    def read(self):
+        return self.__snapshot.read()
+
+    def read_configuration(self):
+        return self.__snapshot.read_configuration()
+
+    def trigger(self):
+        return self.__snapshot.trigger()
+
+    @property
+    def name(self):
+        return self.__snapshot.name
+
     def __getattr__(self, key):
         return getattr(self.__snapshot, key)
 
 
-GROUP_PREFIX = 'bluesky-darkframes-trigger'
+GROUP_PREFIX = "bluesky-darkframes-trigger"
 
 
 class DarkFramePreprocessor:
     """
     A plan preprocessor that ensures each Run records a dark frame.
 
     Specifically this adds a new Event stream, named 'dark' by default. It
@@ -172,34 +193,35 @@
         prompt us to take a new one. Typical examples would be exposure time or
         gain, anything that changes the expected dark frame.
     limit: integer or None, optional
         Number of dark frames to cache. If None, do not limit.
     stream_name: string, optional
         Event stream name for dark frames. Default is 'dark'.
     """
-    def __init__(self, *, dark_plan, detector, max_age,
-                 locked_signals=None, limit=None, stream_name='dark'):
+
+    def __init__(self, *, dark_plan, detector, max_age, locked_signals=None, limit=None, stream_name="dark"):
         self._dark_plan = dark_plan
         if not inspect.signature(dark_plan).parameters:
             warnings.warn(
                 f"The dark_plan {dark_plan} is now expected to accept the "
                 f"detector as an argument. A dark_plan that accepts no "
                 f"arguments is still supported, but it may not be supported "
-                f"in future releases.")
+                f"in future releases."
+            )
             self._partialed_dark_plan = dark_plan
         else:
             self._partialed_dark_plan = functools.partial(dark_plan, detector)
         self._detector = detector
         self.max_age = max_age
         # The signals have to have unique names for this to work.
         names = [signal.name for signal in locked_signals or ()]
         if len(names) != len(set(names)):
             raise BlueskyDarkframesValueError(
-                f"The signals in locked_signals need to have unique names. "
-                f"The names given were: {names}")
+                f"The signals in locked_signals need to have unique names. The names given were: {names}"
+            )
         self._locked_signals = tuple(locked_signals or ())
         self._limit = limit
         self.stream_name = stream_name
         # Map state to (creation_time, snapshot).
         self._cache = collections.OrderedDict()
         self._current_snapshot = _SnapshotShell()
         self._force_read_before_next_event = True
@@ -280,15 +302,16 @@
         self._evict_old_entries()
         key = frozendict(state)
         try:
             creation_time, snapshot = self._cache[key]
         except KeyError as err:
             raise NoMatchingSnapshot(
                 f"No Snapshot matches the state {state}. Perhaps there *was* "
-                f"match but it has aged out of the cache.") from err
+                f"match but it has aged out of the cache."
+            ) from err
         else:
             self._cache.move_to_end(key, last=False)
             return snapshot
 
     def clear(self):
         """
         Clear all cached darkframes.
@@ -300,90 +323,90 @@
         Preprocessor: Takes in a plan and creates a modified plan.
 
         This inserts messages to add extra readings to the plan. First, it
         decides whether it needs to trigger the detector to get a fresh reading
         or whether it can use a cached reading.
         """
 
+        self._latch = False
+
         if self._disabled:
             logger.info("%r is disabled, will act as a no-op", self)
             return (yield from plan)
 
         def insert_dark_frame(force_read, msg=None):
             # Acquire a fresh Snapshot if we need one, or retrieve a cached one.
             state = {}
             for signal in self.locked_signals:
                 reading = yield from bluesky.plan_stubs.read(signal)
                 # Restructure
                 # {'data_key': {'value': <value>, 'timestamp': <timestamp>}, ...}
                 # into (('data_key', <value>) ...).
-                values_only = tuple((k, v['value']) for k, v in reading.items())
+                values_only = tuple((k, v["value"]) for k, v in reading.items())
                 state[signal.name] = values_only
             try:
                 snapshot = self.get_snapshot(state)
             except NoMatchingSnapshot:
                 # If we are here, we either haven't taken a reading when the
                 # locked_signals were in this state, or the last such reading
                 # we took has aged out of the cache. We have to trigger the
                 # hardware and get a fresh snapshot.
-                logger.info("Taking a new %r reading for state=%r",
-                            self.stream_name, state)
+                logger.info("Taking a new %r reading for state=%r", self.stream_name, state)
                 snapshot = yield from self._partialed_dark_plan()
                 self.add_snapshot(snapshot, state)
             # If the Snapshot is the same as the one we most recently inserted,
             # then we don't need to create a new Event. The previous Event
             # still holds.
             snapshot_changed = snapshot is not self._current_snapshot.get_snapshot()
             if snapshot_changed or force_read:
-                logger.info("Creating a %r Event for state=%r",
-                            self.stream_name, state)
+                logger.info("Creating a %r Event for state=%r", self.stream_name, state)
                 self._current_snapshot.set_snaphsot(snapshot)
                 # Read the Snapshot. This does not actually trigger hardware,
                 # but it goes through all the bluesky steps to generate new
                 # Event.
                 # The reason we handle self._current_snapshot here instead of
                 # snapshot itself is the bluesky RunEngine notices if you give
                 # it a different object than you had given it earlier. Thus,
                 # bluesky will always see the "Device" self._current_snapshot
                 # here, and it will be satisfied.
                 yield from bps.stage(self._current_snapshot)
                 yield from trigger_and_read(
-                    [self._current_snapshot],
-                    name=self.stream_name,
-                    group=short_uid(GROUP_PREFIX))
+                    [self._current_snapshot], name=self.stream_name, group=short_uid(GROUP_PREFIX)
+                )
                 yield from bps.unstage(self._current_snapshot)
             self._latch = False
             if msg is not None:
                 return (yield msg)
 
         def maybe_insert_dark_frame(msg):
             # * Is this a 'trigger' message?
             # * Does it refer to the detector that this preprocessor cares about?
             # * Is it *not* from another DarkFramePreprocessor. (There can be
             # multiple nested DarkFramePreprocessors watching the same detector
             # by applying different dark_plans / recording Events in different
             # streams.)
-            if (msg.command == 'trigger'
-                    and msg.obj is self.detector
-                    and not msg.kwargs['group'].startswith(GROUP_PREFIX)
-                    and not self._latch):
+            if (
+                msg.command == "trigger"
+                and msg.obj is self.detector
+                and not msg.kwargs["group"].startswith(GROUP_PREFIX)
+                and not self._latch
+            ):
                 force_read = self._force_read_before_next_event
                 self._force_read_before_next_event = False
                 self._latch = True  # prevents infinite recursion
                 return insert_dark_frame(force_read=force_read, msg=msg), None
-            elif msg.command == 'open_run':
+            elif msg.command == "open_run":
                 # Make sure we get a new Event because we have just started a
                 # new Run.
                 self._force_read_before_next_event = True
                 return None, None
             else:
                 return None, None
 
-        return (yield from bluesky.preprocessors.plan_mutator(
-            plan, maybe_insert_dark_frame))
+        return (yield from bluesky.preprocessors.plan_mutator(plan, maybe_insert_dark_frame))
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {len(self.cache)} snapshots cached>"
 
     def disable(self):
         """
         Make this preprocessor a no-op.
@@ -448,77 +471,74 @@
          Pedestal to add to the data to make sure subtracted result does not
          fall below 0.
 
          This is actually pre subtracted from the dark frame for efficiency.
 
          Defaults to 100.
     """
-    def __init__(self,
-                 field,
-                 light_stream_name='primary',
-                 dark_stream_name='dark',
-                 pedestal=100):
+
+    def __init__(self, field, light_stream_name="primary", dark_stream_name="dark", pedestal=100):
         self.field = field
         self.light_stream_name = light_stream_name
         self.dark_stream_name = dark_stream_name
         self.light_descriptor = None
         self.dark_descriptor = None
         self.dark_frame = None
         self.pedestal = pedestal
 
     def descriptor(self, doc):
-        if doc['name'] == self.light_stream_name:
-            self.light_descriptor = doc['uid']
+        if doc["name"] == self.light_stream_name:
+            self.light_descriptor = doc["uid"]
             # add flag that we did the background subtraction
             doc = copy.deepcopy(dict(doc))
-            doc['data_keys'][f'{self.field}_is_background_subtracted'] = {
-                'source': 'DarkSubtraction',
-                'dtype': 'number',
-                'shape': [],
-                'precsion': 0,
-                'object_name': f'{self.field}_DarkSubtraction'}
-            doc['configuration'][f'{self.field}_DarkSubtraction'] = {
-                'data': {'pedestal': self.pedestal},
-                'timestamps': {'pedestal': time.time()},
-                'data_keys': {
-                    'pedestal': {
-                        'source': 'DarkSubtraction',
-                        'dtype': 'number',
-                        'shape': [],
-                        'precsion': 0,
+            doc["data_keys"][f"{self.field}_is_background_subtracted"] = {
+                "source": "DarkSubtraction",
+                "dtype": "number",
+                "shape": [],
+                "precsion": 0,
+                "object_name": f"{self.field}_DarkSubtraction",
+            }
+            doc["configuration"][f"{self.field}_DarkSubtraction"] = {
+                "data": {"pedestal": self.pedestal},
+                "timestamps": {"pedestal": time.time()},
+                "data_keys": {
+                    "pedestal": {
+                        "source": "DarkSubtraction",
+                        "dtype": "number",
+                        "shape": [],
+                        "precsion": 0,
                     }
-                }
+                },
             }
-            doc['object_keys'][f'{self.field}_DarkSubtraction'] = [
-                f'{self.field}_is_background_subtracted']
+            doc["object_keys"][f"{self.field}_DarkSubtraction"] = [f"{self.field}_is_background_subtracted"]
 
-        elif doc['name'] == self.dark_stream_name:
-            self.dark_descriptor = doc['uid']
+        elif doc["name"] == self.dark_stream_name:
+            self.dark_descriptor = doc["uid"]
         return doc
 
     def event_page(self, doc):
-        if doc['descriptor'] == self.dark_descriptor:
-            self.dark_frame, = doc['data'][self.field]
+        if doc["descriptor"] == self.dark_descriptor:
+            (self.dark_frame,) = np.asarray(doc["data"][self.field])
             self.dark_frame -= self.pedestal
-            numpy.clip(self.dark_frame, a_min=0, a_max=None, out=self.dark_frame)
-        elif doc['descriptor'] == self.light_descriptor:
+            np.clip(self.dark_frame, a_min=0, a_max=None, out=self.dark_frame)
+        elif doc["descriptor"] == self.light_descriptor:
             if self.dark_frame is None:
                 raise NoDarkFrame(
-                    "DarkSubtraction has not received a 'dark' Event yet, so "
-                    "it has nothing to subtract.")
+                    "DarkSubtraction has not received a 'dark' Event yet, so it has nothing to subtract."
+                )
             doc = copy.deepcopy(dict(doc))
-            light = numpy.asarray(doc['data'][self.field])
+            light = np.asarray(doc["data"][self.field])
             subtracted = self.subtract(light, self.dark_frame)
-            doc['data'][self.field] = subtracted
-            doc['data'][f'{self.field}_is_background_subtracted'] = [True]
-            doc['timestamps'][f'{self.field}_is_background_subtracted'] = [time.time()]
+            doc["data"][self.field] = subtracted
+            doc["data"][f"{self.field}_is_background_subtracted"] = [True]
+            doc["timestamps"][f"{self.field}_is_background_subtracted"] = [time.time()]
         return doc
 
     def subtract(self, light, dark):
-        return numpy.clip(light - dark, a_min=0, a_max=None).astype(light.dtype)
+        return np.clip(light - dark, a_min=0, a_max=None).astype(light.dtype)
 
 
 class BlueskyDarkframesException(Exception):
     ...
 
 
 class BlueskyDarkframesValueError(ValueError, BlueskyDarkframesException):
@@ -532,15 +552,15 @@
 class NoMatchingSnapshot(KeyError, BlueskyDarkframesException):
     ...
 
 
 # Vendored from bluesky.plan_stubs, added `group` parameter
 
 
-def trigger_and_read(devices, name='primary', group=None):
+def trigger_and_read(devices, name="primary", group=None):
     """
     Trigger and read a list of detectors and bundle readings into one Event.
 
     Parameters
     ----------
     devices : iterable
         devices to trigger (if they have a trigger method) and then read
@@ -560,27 +580,28 @@
         yield from bps.null()
     devices = bps.separate_devices(devices)  # remove redundant entries
     rewindable = bps.all_safe_rewind(devices)  # if devices can be re-triggered
 
     def inner_trigger_and_read():
         nonlocal group
         if group is None:
-            group = short_uid('trigger')
+            group = short_uid("trigger")
         no_wait = True
         for obj in devices:
-            if hasattr(obj, 'trigger'):
+            if hasattr(obj, "trigger"):
                 no_wait = False
                 yield from bps.trigger(obj, group=group)
         # Skip 'wait' if none of the devices implemented a trigger method.
         if not no_wait:
             yield from bps.wait(group=group)
         yield from bps.create(name)
         ret = {}  # collect and return readings to give plan access to them
         for obj in devices:
-            reading = (yield from bps.read(obj))
+            reading = yield from bps.read(obj)
             if reading is not None:
                 ret.update(reading)
         yield from bps.save()
         return ret
+
     from bluesky.preprocessors import rewindable_wrapper
-    return (yield from rewindable_wrapper(inner_trigger_and_read(),
-                                          rewindable))
+
+    return (yield from rewindable_wrapper(inner_trigger_and_read(), rewindable))
```

### Comparing `bluesky-darkframes-0.5.0/bluesky_darkframes/tests/tests.py` & `bluesky-darkframes-0.6.0/bluesky_darkframes/tests/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,88 +1,92 @@
-import time
 import os
+import time
 
 import bluesky.plan_stubs as bps
-import bluesky_darkframes
-import bluesky_darkframes.sim
+import pytest
 from bluesky.plans import count
 from event_model import RunRouter
 from ophyd.sim import NumpySeqHandler
-import pytest
 from suitcase.tiff_series import Serializer
 
+import bluesky_darkframes
+import bluesky_darkframes.sim
 
 # This is some simulated hardware for demo purposes.
-det = bluesky_darkframes.sim.DiffractionDetector(name='det')
+det = bluesky_darkframes.sim.DiffractionDetector(name="det")
 det.exposure_time.put(0.01)
-shutter = bluesky_darkframes.sim.Shutter(name='shutter', value='open')
+shutter = bluesky_darkframes.sim.Shutter(name="shutter", value="open")
 
 
 def dark_plan(detector):
     yield from bps.unstage(detector)
-    yield from bps.mv(shutter, 'closed')
+    yield from bps.mv(shutter, "closed")
     yield from bps.stage(detector)
-    yield from bps.trigger(detector, group='bluesky-darkframes-trigger')
-    yield from bps.wait('darkframe-trigger')
+    yield from bps.trigger(detector, group="bluesky-darkframes-trigger")
+    yield from bps.wait("darkframe-trigger")
     snapshot = bluesky_darkframes.SnapshotDevice(detector)
     yield from bps.unstage(detector)
-    yield from bps.mv(shutter, 'open')
+    yield from bps.mv(shutter, "open")
     yield from bps.stage(detector)
     return snapshot
 
 
 def test_one_dark_event_emitted(RE):
     dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-        dark_plan=dark_plan, detector=det, max_age=3)
+        dark_plan=dark_plan, detector=det, max_age=3
+    )
     RE.preprocessors.append(dark_frame_preprocessor)
 
     def verify_one_dark_frame(name, doc):
-        if name == 'stop':
-            assert doc['num_events']['dark'] == 1
+        if name == "stop":
+            assert doc["num_events"]["dark"] == 1
 
     RE(count([det]), verify_one_dark_frame)
     RE(count([det], 3), verify_one_dark_frame)
 
 
 def test_disable(RE):
     dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-        dark_plan=dark_plan, detector=det, max_age=3)
+        dark_plan=dark_plan, detector=det, max_age=3
+    )
     RE.preprocessors.append(dark_frame_preprocessor)
     dark_frame_preprocessor.disable()
 
     def verify_no_dark_stream(name, doc):
-        if name == 'stop':
-            assert 'dark' not in doc['num_events']
+        if name == "stop":
+            assert "dark" not in doc["num_events"]
 
     RE(count([det]), verify_no_dark_stream)
 
 
 def test_mid_scan_dark_frames(RE):
     dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-        dark_plan=dark_plan, detector=det, max_age=0)
+        dark_plan=dark_plan, detector=det, max_age=0
+    )
     RE.preprocessors.append(dark_frame_preprocessor)
 
     def verify_three_dark_frames(name, doc):
-        if name == 'stop':
-            assert doc['num_events']['dark'] == 3
+        if name == "stop":
+            assert doc["num_events"]["dark"] == 3
 
     RE(count([det], 3), verify_three_dark_frames)
 
 
 def test_max_age(RE):
     """
     Test the a dark frame is reused until it expires, and then re-taken.
     """
     dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-        dark_plan=dark_plan, detector=det, max_age=1)
+        dark_plan=dark_plan, detector=det, max_age=1
+    )
     RE.preprocessors.append(dark_frame_preprocessor)
     # The first executation adds something to the cache.
     RE(count([det]))
     assert len(dark_frame_preprocessor.cache) == 1
-    state, = dark_frame_preprocessor.cache
+    (state,) = dark_frame_preprocessor.cache
     # A second execution reuses the cache entry, adds nothing.
     RE(count([det]))
     assert len(dark_frame_preprocessor.cache) == 1
     dark_frame_preprocessor.get_snapshot(state)
     # Wait for it to age out.
     time.sleep(1.01)
     with pytest.raises(bluesky_darkframes.NoMatchingSnapshot):
@@ -92,16 +96,16 @@
 def test_locked_signals(RE):
     """
     Test that if a 'locked signal' is changed, a new dark frame is taken, but
     if the locked signal goes back to the original value, the original dark
     frame is reused.
     """
     dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-        dark_plan=dark_plan, detector=det, max_age=100,
-        locked_signals=[det.exposure_time])
+        dark_plan=dark_plan, detector=det, max_age=100, locked_signals=[det.exposure_time]
+    )
     RE.preprocessors.append(dark_frame_preprocessor)
     RE(count([det]))
     assert len(dark_frame_preprocessor.cache) == 1
     RE(bps.mv(det.exposure_time, 0.02))
     # This should take a new dark frame.
     RE(count([det]))
     assert len(dark_frame_preprocessor.cache) == 2
@@ -118,16 +122,16 @@
     only require actually *triggering* to get a new snapshot twice.
 
     That is, if we change the state of the locked_signals like A -> B -> A, we
     only need one snapshot for A and one snapshot for B, but there will be two
     Events containing the reading from A.
     """
     dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-        dark_plan=dark_plan, detector=det, max_age=100,
-        locked_signals=[det.exposure_time])
+        dark_plan=dark_plan, detector=det, max_age=100, locked_signals=[det.exposure_time]
+    )
     RE.preprocessors.append(dark_frame_preprocessor)
 
     def plan():
         yield from bps.open_run()
         yield from bps.stage(det)
         yield from bps.mv(det.exposure_time, 0.01)
         yield from bps.trigger_and_read([det])  # should prompt new dark Event
@@ -139,50 +143,49 @@
         yield from bps.trigger_and_read([det])  # should prompt new dark Event
         yield from bps.trigger_and_read([det])
         yield from bps.trigger_and_read([det])
         yield from bps.unstage(det)
         yield from bps.close_run()
 
     def verify_event_count(name, doc):
-        if name == 'stop':
-            assert doc['num_events']['dark'] == 3
-            assert doc['num_events']['primary'] == 7
+        if name == "stop":
+            assert doc["num_events"]["dark"] == 3
+            assert doc["num_events"]["primary"] == 7
 
     RE(plan(), verify_event_count)
 
     assert len(dark_frame_preprocessor.cache) == 2
 
 
 def test_limit(RE):
     """
     Test that if a 'locked signal' is changed, a new dark frame is taken, but
     if the locked signal goes back to the original value, the original dark
     frame is reused.
     """
     dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-        dark_plan=dark_plan, detector=det, max_age=100,
-        locked_signals=[det.exposure_time],
-        limit=1)
+        dark_plan=dark_plan, detector=det, max_age=100, locked_signals=[det.exposure_time], limit=1
+    )
     RE.preprocessors.append(dark_frame_preprocessor)
     RE(count([det]))
     assert len(dark_frame_preprocessor.cache) == 1
-    state, = dark_frame_preprocessor.cache
+    (state,) = dark_frame_preprocessor.cache
     previous_state = state
     RE(bps.mv(det.exposure_time, 0.02))
     # This should take a new dark frame and evict the last one.
     RE(count([det]))
     assert len(dark_frame_preprocessor.cache) == 1
-    state, = dark_frame_preprocessor.cache
+    (state,) = dark_frame_preprocessor.cache
     assert state != previous_state
     previous_state = state
     # This should take a new dark frame and evict the last one.
     RE(bps.mv(det.exposure_time, 0.01))
     RE(count([det]))
     assert len(dark_frame_preprocessor.cache) == 1
-    state, = dark_frame_preprocessor.cache
+    (state,) = dark_frame_preprocessor.cache
     assert state != previous_state
     previous_state = state
 
 
 def test_non_colliding_uids(RE):
     """
     Tests that when the same Snapshot is used multiple times it issues distinct
@@ -191,110 +194,116 @@
 
     class LocalException(Exception):
         ...
 
     cache = set()
 
     def check_uniqueness(name, doc):
-        if name == 'datum':
-            key = (name, doc['datum_id'])
+        if name == "datum":
+            key = (name, doc["datum_id"])
         else:
-            key = (name, doc['uid'])
+            key = (name, doc["uid"])
         if key in cache:
             raise LocalException(f"Collision {key}")
         cache.add(key)
 
     RE.subscribe(check_uniqueness)
 
     dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-        dark_plan=dark_plan, detector=det, max_age=100)
+        dark_plan=dark_plan, detector=det, max_age=100
+    )
     RE.preprocessors.append(dark_frame_preprocessor)
 
     RE(count([det]), check_uniqueness)
     RE(count([det]), check_uniqueness)
     RE(count([det]), check_uniqueness)
 
 
-@pytest.mark.parametrize('pedestal', [None, 0, 100])
+@pytest.mark.parametrize("pedestal", [None, 0, 100])
 def test_streaming_export(RE, tmp_path, pedestal):
     """
     Test that DarkSubtractor generates files when subscribed to RE.
     """
+
     def factory(name, doc):
         # The problem this is solving is to store documents from this run long
         # enough to cross-reference them (e.g. light frames and dark frames),
         # and then tearing it down when we're done with this run.
         kwargs = {}
         if pedestal is not None:
-            kwargs['pedestal'] = pedestal
-        subtractor = bluesky_darkframes.DarkSubtraction('det_image', **kwargs)
+            kwargs["pedestal"] = pedestal
+        subtractor = bluesky_darkframes.DarkSubtraction("det_image", **kwargs)
         serializer = Serializer(tmp_path)
 
         # And by returning this function below, we are routing all other
         # documents *for this run* through here.
         def subtract_and_serialize(name, doc):
             name, doc = subtractor(name, doc)
             serializer(name, doc)
 
         return [subtract_and_serialize], []
 
-    rr = RunRouter([factory], {'NPY_SEQ': NumpySeqHandler})
+    rr = RunRouter([factory], {"NPY_SEQ": NumpySeqHandler})
     RE.subscribe(rr)
 
     dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-        dark_plan=dark_plan, detector=det, max_age=100)
+        dark_plan=dark_plan, detector=det, max_age=100
+    )
     RE.preprocessors.append(dark_frame_preprocessor)
 
-    RE(count([det]))
+    (uid,) = RE(count([det]))
     exported_files = os.listdir(tmp_path)
+    for filename in exported_files:
+        assert filename.startswith(uid)
 
     assert len(exported_files) == 2
 
 
 def test_no_dark_frames(RE, tmp_path):
     """
     Test that a readable error is raised if no 'dark' frame is received.
     """
+
     def factory(name, doc):
         # The problem this is solving is to store documents from this run long
         # enough to cross-reference them (e.g. light frames and dark frames),
         # and then tearing it down when we're done with this run.
-        subtractor = bluesky_darkframes.DarkSubtraction('det_image')
+        subtractor = bluesky_darkframes.DarkSubtraction("det_image")
         serializer = Serializer(tmp_path)
 
         # And by returning this function below, we are routing all other
         # documents *for this run* through here.
         def subtract_and_serialize(name, doc):
             name, doc = subtractor(name, doc)
             serializer(name, doc)
 
         return [subtract_and_serialize], []
 
-    rr = RunRouter([factory], {'NPY_SEQ': NumpySeqHandler})
+    rr = RunRouter([factory], {"NPY_SEQ": NumpySeqHandler})
     RE.subscribe(rr)
 
     # We intentionally 'forget' to set up a dark_frame_preprocessor for this
     # test.
 
     with pytest.raises(bluesky_darkframes.NoDarkFrame):
         RE(count([det]))
 
 
 def test_nested_preprocessors(RE):
     N = 3
     for i in range(N):
         dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-            dark_plan=dark_plan, detector=det, max_age=0,
-            stream_name=f'dark_{i}')
+            dark_plan=dark_plan, detector=det, max_age=0, stream_name=f"dark_{i}"
+        )
         RE.preprocessors.append(dark_frame_preprocessor)
 
     def verify_event_count(name, doc):
-        if name == 'stop':
+        if name == "stop":
             for i in range(N):
-                assert doc['num_events'][f'dark_{i}'] == 3
+                assert doc["num_events"][f"dark_{i}"] == 3
 
     RE(count([det], 3), verify_event_count)
 
 
 def test_old_dark_plan_signature(RE):
     """
     In bluesky-darkfarmes < 0.4.0, we expected dark_plan to take no args.
@@ -304,16 +313,17 @@
     """
 
     def old_dark_plan():
         return (yield from dark_plan(det))
 
     with pytest.warns(UserWarning, match="dark_plan"):
         dark_frame_preprocessor = bluesky_darkframes.DarkFramePreprocessor(
-            dark_plan=old_dark_plan, detector=det, max_age=3)
+            dark_plan=old_dark_plan, detector=det, max_age=3
+        )
     RE.preprocessors.append(dark_frame_preprocessor)
 
     def verify_one_dark_frame(name, doc):
-        if name == 'stop':
-            assert doc['num_events']['dark'] == 1
+        if name == "stop":
+            assert doc["num_events"]["dark"] == 1
 
     RE(count([det]), verify_one_dark_frame)
     RE(count([det], 3), verify_one_dark_frame)
```

### Comparing `bluesky-darkframes-0.5.0/bluesky_darkframes.egg-info/PKG-INFO` & `bluesky-darkframes-0.6.0/bluesky_darkframes.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: bluesky-darkframes
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools for acquiring and subtracting darkframes
 Home-page: https://github.com/bluesky/bluesky-darkframes
 Author: Brookhaven National Lab
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
 
-===============================
+==================
 Bluesky Darkframes
-===============================
+==================
+
+.. image:: https://github.com/bluesky/bluesky-darkframes/actions/workflows/testing.yml/badge.svg
+   :target: https://github.com/bluesky/bluesky-darkframes/actions/workflows/testing.yml
 
-.. image:: https://img.shields.io/travis/bluesky/bluesky-darkframes.svg
-        :target: https://travis-ci.org/bluesky/bluesky-darkframes
 
 .. image:: https://img.shields.io/pypi/v/bluesky-darkframes.svg
         :target: https://pypi.python.org/pypi/bluesky-darkframes
 
 
 Tools for acquiring and subtracting darkframes
 
 * Free software: 3-clause BSD license
 * Documentation: (COMING SOON!) https://bluesky.github.io/bluesky-darkframes.
 
 Features
 --------
 
 * TODO
-
-
```

### Comparing `bluesky-darkframes-0.5.0/docs/Makefile` & `bluesky-darkframes-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bluesky-darkframes-0.5.0/docs/source/conf.py` & `bluesky-darkframes-0.6.0/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,175 +28,190 @@
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'sphinx.ext.autodoc',
-    'sphinx.ext.autosummary',
-    'sphinx.ext.githubpages',
-    'sphinx.ext.intersphinx',
-    'sphinx.ext.mathjax',
-    'sphinx.ext.viewcode',
-    'jupyter_sphinx',
-    'matplotlib.sphinxext.plot_directive',
-    'numpydoc',
-    'sphinx_copybutton',
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.githubpages",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.viewcode",
+    "IPython.sphinxext.ipython_directive",
+    "IPython.sphinxext.ipython_console_highlighting",
+    "jupyter_sphinx",
+    "matplotlib.sphinxext.plot_directive",
+    "numpydoc",
+    "sphinx_copybutton",
 ]
 
 # Configuration options for plot_directive. See:
 # https://github.com/matplotlib/matplotlib/blob/f3ed922d935751e08494e5fb5311d3050a3b637b/lib/matplotlib/sphinxext/plot_directive.py#L81
 plot_html_show_source_link = False
 plot_html_show_formats = False
 
 # Generate the API documentation when building
 autosummary_generate = True
 numpydoc_show_class_members = False
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'Bluesky Darkframes'
-copyright = '2019, Brookhaven National Lab'
-author = 'Brookhaven National Lab'
+project = "Bluesky Darkframes"
+copyright = "2019, Brookhaven National Lab"
+author = "Brookhaven National Lab"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 import bluesky_darkframes
+
 # The short X.Y version.
 version = bluesky_darkframes.__version__
 # The full version, including alpha/beta/rc tags.
 release = bluesky_darkframes.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = "sphinx_rtd_theme"
 import sphinx_rtd_theme
+
 html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # Custom sidebar templates, must be a dictionary that maps document names
 # to template names.
 #
 # This is required for the alabaster theme
 # refs: http://alabaster.readthedocs.io/en/latest/installation.html#sidebars
 html_sidebars = {
-    '**': [
-        'relations.html',  # needs 'show_related': True theme option to display
-        'searchbox.html',
+    "**": [
+        "relations.html",  # needs 'show_related': True theme option to display
+        "searchbox.html",
     ]
 }
 
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'bluesky-darkframes'
+htmlhelp_basename = "bluesky-darkframes"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
-    #
     # 'papersize': 'letterpaper',
-
-    # The font size ('10pt', '11pt' or '12pt').
     #
+    # The font size ('10pt', '11pt' or '12pt').
     # 'pointsize': '10pt',
-
-    # Additional stuff for the LaTeX preamble.
     #
+    # Additional stuff for the LaTeX preamble.
     # 'preamble': '',
-
-    # Latex figure (float) alignment
     #
+    # Latex figure (float) alignment
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'bluesky-darkframes.tex', 'Bluesky Darkframes Documentation',
-     'Contributors', 'manual'),
+    (
+        master_doc,
+        "bluesky-darkframes.tex",
+        "Bluesky Darkframes Documentation",
+        "Contributors",
+        "manual",
+    ),
 ]
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    (master_doc, 'bluesky-darkframes', 'Bluesky Darkframes Documentation',
-     [author], 1)
+    (
+        master_doc,
+        "bluesky-darkframes",
+        "Bluesky Darkframes Documentation",
+        [author],
+        1,
+    )
 ]
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'bluesky-darkframes', 'Bluesky Darkframes Documentation',
-     author, 'bluesky-darkframes', 'Tools for acquiring and subtracting darkframes',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "bluesky-darkframes",
+        "Bluesky Darkframes Documentation",
+        author,
+        "bluesky-darkframes",
+        "Tools for acquiring and subtracting darkframes",
+        "Miscellaneous",
+    ),
 ]
 
 
-
-
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    'event_model': ('https://blueskyproject.io/event-model', None),
-    'python': ('https://docs.python.org/3/', None),
-    'numpy': ('https://docs.scipy.org/doc/numpy/', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
-    'pandas': ('https://pandas.pydata.org/pandas-docs/stable', None),
-    'matplotlib': ('https://matplotlib.org', None),
+    "event_model": ("https://blueskyproject.io/event-model/main/", None),
+    "suitcase.tiff_series": ("https://blueskyproject.io/suitcase", None),
+    "python": ("https://docs.python.org/3/", None),
+    "numpy": ("https://numpy.org/doc/stable/", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/reference/", None),
+    "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
+    "matplotlib": ("https://matplotlib.org/stable", None),
 }
```

### Comparing `bluesky-darkframes-0.5.0/docs/source/release-history.rst` & `bluesky-darkframes-0.6.0/docs/source/release-history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 ===============
 Release History
 ===============
 
+v0.6.0 (2023-06-15)
+-------------------
+
+Fixed
++++++
+* clean up on ``RE.abort()`` properly
+* support for read-only arrays from databroker
+* fix versioneer compatibility with Python 3.11
+
+Changed
+++++++++
+* rerender the project's structure with new cookiecutter.
+* improve tests
+
+
 v0.5.0 (2021-10-08)
-------------------
+-------------------
 
 Fixed
 +++++
 * support detectors not defining method ``collect_asset_docs``
 * resolve jupyter_sphinx deprecation warning
 
 Changed
```

### Comparing `bluesky-darkframes-0.5.0/docs/source/usage.rst` & `bluesky-darkframes-0.6.0/docs/source/usage.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,20 @@
        yield from bps.close_run()
        yield from bps.unstage(detector)
 
 This direct solution is best one for some circumstances. However, if you find
 yourself looking at the prospect of rewriting a large number of plans just to
 add this dark frame logic, it may be simpler to use a bluesky *preprocessor*. A
 preprocessor can augment or modify the steps in a plan. The
-:class:`DarkFramePreprocessor` watches for a given detector to be triggered and
-inserts steps in the plan to acquire and/or record a dark frame when needed.
-Depending on how you configure it, it can reuse a given dark frame multiple
-times. Thus, it will not necessarily *acquire* a dark frame for every Run, but
-it will ensure that at least one 'dark' Event is *recorded* in every Run.
+:class:`~bluesky_darkframes.DarkFramePreprocessor` watches for a given detector
+to be triggered and inserts steps in the plan to acquire and/or record a dark
+frame when needed.  Depending on how you configure it, it can reuse a given dark
+frame multiple times. Thus, it will not necessarily *acquire* a dark frame for
+every Run, but it will ensure that at least one 'dark' Event is *recorded* in
+every Run.
 
 The preprocessor can be applied to specific plans, using Python's decorator
 syntax
 
 .. code:: python
 
    from bluesky.preprocessors import make_decorator
@@ -87,15 +88,15 @@
 #. What are the rules for when to take a fresh dark frame and when to reuse one
    that has already been taken?
 #. If you would like to compute subtracted frames on the fly, where should the
    results go?
 
 To address (1) define a bluesky plan that closes the shutter, takes an
 acquistion, and reopens the shutter. The last two lines in this example use a
-special mechanism, :class:`bluesky_darkframes.SnapshotDevice`, to stash the
+special mechanism, :class:`~bluesky_darkframes.SnapshotDevice`, to stash the
 acquisition where it can potentially be reused. (Later on we'll set the rules
 for whether/how dark frames can be reused.)
 
 .. jupyter-execute::
 
    import bluesky.plan_stubs as bps
    import bluesky_darkframes
@@ -231,15 +232,15 @@
 original if desired.
 
 .. jupyter-execute::
 
    !ls exported_files
 
 To customize the file name and other output options, see
-:class:`suitcase.tiff_series.Serializer`.
+:class:`~suitcase.tiff_series.Serializer`.
 
 Export data during acquisition (streaming)
 ------------------------------------------
 
 Here we use a :class:`event_model.RunRouter`.
 
 .. jupyter-execute::
```

### Comparing `bluesky-darkframes-0.5.0/setup.py` & `bluesky-darkframes-0.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,72 @@
-from os import path
-from setuptools import setup, find_packages
 import sys
-import versioneer
+from os import path
 
+from setuptools import find_packages, setup
+
+import versioneer
 
 # NOTE: This file must remain Python 2 compatible for the foreseeable future,
 # to ensure that we error out properly for people with outdated setuptools
 # and/or pip.
-min_version = (3, 6)
+min_version = (
+    3,
+    8,
+)
 if sys.version_info < min_version:
     error = """
 bluesky-darkframes does not support Python {0}.{1}.
 Python {2}.{3} and above is required. Check your Python version like so:
 
 python3 --version
 
 This may be due to an out-of-date pip. Make sure you have pip >= 9.0.1.
 Upgrade pip like so:
 
 pip install --upgrade pip
-""".format(*(sys.version_info[:2] + min_version))
+""".format(
+        *(sys.version_info[:2] + min_version)
+    )
     sys.exit(error)
 
 here = path.abspath(path.dirname(__file__))
 
-with open(path.join(here, 'README.rst'), encoding='utf-8') as readme_file:
+with open(path.join(here, "README.rst"), encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
-with open(path.join(here, 'requirements.txt')) as requirements_file:
+with open(path.join(here, "requirements.txt")) as requirements_file:
     # Parse requirements.txt, ignoring any commented-out lines.
-    requirements = [line for line in requirements_file.read().splitlines()
-                    if not line.startswith('#')]
+    requirements = [line for line in requirements_file.read().splitlines() if not line.startswith("#")]
 
 
 setup(
-    name='bluesky-darkframes',
+    name="bluesky-darkframes",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description="Tools for acquiring and subtracting darkframes",
     long_description=readme,
     author="Brookhaven National Lab",
-    author_email='dallan@bnl.gov',
-    url='https://github.com/bluesky/bluesky-darkframes',
-    python_requires='>={}'.format('.'.join(str(n) for n in min_version)),
-    packages=find_packages(exclude=['docs', 'tests']),
+    author_email="dallan@bnl.gov",
+    url="https://github.com/bluesky/bluesky-darkframes",
+    python_requires=">={}".format(".".join(str(n) for n in min_version)),
+    packages=find_packages(exclude=["docs", "tests"]),
     entry_points={
-        'console_scripts': [
+        "console_scripts": [
             # 'command = some.module:some_function',
         ],
     },
     include_package_data=True,
     package_data={
-        'bluesky_darkframes': [
+        "bluesky_darkframes": [
             # When adding files here, remember to update MANIFEST.in as well,
             # or else they will not be included in the distribution on PyPI!
             # 'path/to/data_file',
         ]
     },
     install_requires=requirements,
     license="BSD (3-clause)",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
+        "Development Status :: 2 - Pre-Alpha",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
     ],
 )
```

### Comparing `bluesky-darkframes-0.5.0/versioneer.py` & `bluesky-darkframes-0.6.0/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -273,14 +272,15 @@
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
 from __future__ import print_function
+
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
 import os
@@ -304,54 +304,55 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         me = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(me)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(me), versioneer_py))
+            print("Warning: build in %s is using versioneer.py from %s" % (os.path.dirname(me), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+    parser = configparser.ConfigParser()
+    parser.read(setup_cfg)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
+
     cfg = VersioneerConfig()
     cfg.VCS = VCS
     cfg.style = get(parser, "style") or ""
     cfg.versionfile_source = get(parser, "versionfile_source")
     cfg.versionfile_build = get(parser, "versionfile_build")
     cfg.tag_prefix = get(parser, "tag_prefix")
     if cfg.tag_prefix in ("''", '""'):
@@ -368,36 +369,40 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY = {}
 HANDLERS = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Decorator to mark a method as the handler for a particular VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     p = None
     for c in commands:
         try:
             dispcmd = str([c] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            p = subprocess.Popen([c] + args, cwd=cwd, env=env,
-                                 stdout=subprocess.PIPE,
-                                 stderr=(subprocess.PIPE if hide_stderr
-                                         else None))
+            p = subprocess.Popen(
+                [c] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+            )
             break
         except EnvironmentError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -414,15 +419,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
-LONG_VERSION_PY['git'] = '''
+LONG_VERSION_PY[
+    "git"
+] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -989,71 +996,86 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG):] for r in refs if r.startswith(TAG)])
+    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r'\d', r)])
+        tags = set([r for r in refs if re.search(r"\d", r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, run_command=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
 
-    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                          hide_stderr=True)
+    out, rc = run_command(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = run_command(GITS, ["describe", "--tags", "--dirty",
-                                          "--always", "--long",
-                                          "--match", "%s*" % tag_prefix],
-                                   cwd=root)
+    describe_out, rc = run_command(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            "%s*" % tag_prefix,
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = run_command(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
@@ -1068,54 +1090,53 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"],
-                                    cwd=root)
+        count_out, rc = run_command(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
         pieces["distance"] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"],
-                       cwd=root)[0].strip()
+    date = run_command(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
@@ -1163,24 +1184,27 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for i in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         else:
             rootdirs.append(root)
             root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print("Tried directories %s but none started with prefix %s" % (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.18) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1201,29 +1225,26 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S)
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1247,16 +1268,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
@@ -1362,19 +1382,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-pre":
@@ -1386,17 +1408,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1411,16 +1437,15 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert cfg.versionfile_source is not None, "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1466,17 +1491,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1517,14 +1546,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1549,22 +1579,23 @@
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1577,25 +1608,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.distutils_buildexe import py2exe as _py2exe  # py3
         except ImportError:
             from py2exe.build_exe import py2exe as _py2exe  # py2
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1606,21 +1641,25 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if "setuptools" in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
@@ -1639,16 +1678,16 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(target_versionfile, self._versioneer_generated_versions)
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -1695,36 +1734,41 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (EnvironmentError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (
+        EnvironmentError,
+        configparser.NoSectionError,
+        configparser.NoOptionError,
+    ) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except EnvironmentError:
             old = ""
         if INIT_PY_SNIPPET not in old:
@@ -1758,16 +1802,15 @@
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
         with open(manifest_in, "a") as f:
             f.write("include versioneer.py\n")
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
-        print(" appending versionfile_source ('%s') to MANIFEST.in" %
-              cfg.versionfile_source)
+        print(" appending versionfile_source ('%s') to MANIFEST.in" % cfg.versionfile_source)
         with open(manifest_in, "a") as f:
             f.write("include %s\n" % cfg.versionfile_source)
     else:
         print(" versionfile_source already in MANIFEST.in")
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
```

