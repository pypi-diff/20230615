# Comparing `tmp/port-for-0.6.3.tar.gz` & `tmp/port-for-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port-for-0.6.3.tar", last modified: Thu Dec 15 16:49:19 2022, max compression
+gzip compressed data, was "port-for-0.7.0.tar", last modified: Thu Jun 15 08:13:13 2023, max compression
```

## Comparing `port-for-0.6.3.tar` & `port-for-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 16:49:19.309113 port-for-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2022-12-15 16:49:06.000000 port-for-0.6.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2022-12-15 16:49:06.000000 port-for-0.6.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2022-12-15 16:49:06.000000 port-for-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2022-12-15 16:49:19.309113 port-for-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2022-12-15 16:49:06.000000 port-for-0.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 16:49:19.309113 port-for-0.6.3/port_for/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/_download_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)    13189 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/docopt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2022-12-15 16:49:06.000000 port-for-0.6.3/port_for/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 16:49:19.309113 port-for-0.6.3/port_for.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2022-12-15 16:49:19.000000 port-for-0.6.3/port_for.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2022-12-15 16:49:19.000000 port-for-0.6.3/port_for.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 16:49:19.000000 port-for-0.6.3/port_for.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-15 16:49:19.000000 port-for-0.6.3/port_for.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-15 16:49:19.000000 port-for-0.6.3/port_for.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 16:49:19.000000 port-for-0.6.3/port_for.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2022-12-15 16:49:06.000000 port-for-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-15 16:49:19.309113 port-for-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:13.653290 port-for-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-15 08:13:04.000000 port-for-0.7.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-15 08:13:04.000000 port-for-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 08:13:04.000000 port-for-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-15 08:13:13.653290 port-for-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 08:13:04.000000 port-for-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:13.653290 port-for-0.7.0/port_for/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/_download_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/docopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 08:13:04.000000 port-for-0.7.0/port_for/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:13.653290 port-for-0.7.0/port_for.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:13:13.000000 port-for-0.7.0/port_for.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-15 08:13:04.000000 port-for-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 08:13:13.657290 port-for-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:13:13.653290 port-for-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-15 08:13:04.000000 port-for-0.7.0/tests/test_cases.py
```

### Comparing `port-for-0.6.3/CHANGES.rst` & `port-for-0.7.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 CHANGELOG
 =========
 
 .. towncrier release notes start
 
+0.7.0 (2023-06-15)
+==================
+
+Features
+--------
+
+- get_port will now allow passing additional exclude_ports parameter - these ports will not be chosen. (`#143 <https://https://github.com/kmike/port-for/issues/143>`_)
+
+
 0.6.3 (2022-12-15)
 ==================
 
 Features
 --------
 
 - Add python 3.11 to the list of supported python versions. (`#111 <https://https://github.com/kmike/port-for/issues/111>`_)
```

### Comparing `port-for-0.6.3/LICENSE.txt` & `port-for-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `port-for-0.6.3/PKG-INFO` & `port-for-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-for
-Version: 0.6.3
+Version: 0.7.0
 Summary: Utility that helps with local TCP ports management. It can find an unused TCP localhost port and remember the association.
 Author-email: Mikhail Korobov <kmike84@gmail.com>
 Maintainer-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License: Copyright (c) 2012 Mikhail Korobov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,15 +22,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Source, https://github.com/kmike/port-for/
 Project-URL: Bug Tracker, https://github.com/kmike/port-for/issues
-Project-URL: Changelog, https://github.com/kmike/port-for/blob/v0.6.3/CHANGES.rst
+Project-URL: Changelog, https://github.com/kmike/port-for/blob/v0.7.0/CHANGES.rst
 Keywords: port,posix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `port-for-0.6.3/README.rst` & `port-for-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `port-for-0.6.3/port_for/__init__.py` & `port-for-0.7.0/port_for/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """port_for package."""
-__version__ = "0.6.3"
+__version__ = "0.7.0"
 
 from ._ranges import UNASSIGNED_RANGES
 from .api import (
     available_good_ports,
     available_ports,
     is_available,
     good_port_ranges,
```

### Comparing `port-for-0.6.3/port_for/_download_ranges.py` & `port-for-0.7.0/port_for/_download_ranges.py`

 * *Files identical despite different names*

### Comparing `port-for-0.6.3/port_for/_ranges.py` & `port-for-0.7.0/port_for/_ranges.py`

 * *Files identical despite different names*

### Comparing `port-for-0.6.3/port_for/api.py` & `port-for-0.7.0/port_for/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,34 +143,36 @@
         Set[int],
         List[str],
         List[int],
         List[Tuple[int, int]],
         List[Set[int]],
         List[Union[Set[int], Tuple[int, int]]],
         List[Union[str, int, Tuple[int, int], Set[int]]],
-    ]
+    ],
+    exclude_ports: Optional[Iterable[int]] = None,
 ) -> Optional[int]:
     """
     Retuns a random available port. If there's only one port passed
     (e.g. 5000 or '5000') function does not check if port is available.
     If there's -1 passed as an argument, function returns None.
 
-    :param str|int|tuple|set|list ports:
+    :param ports:
         exact port (e.g. '8000', 8000)
         randomly selected port (None) - any random available port
         [(2000,3000)] or (2000,3000) - random available port from a given range
         [{4002,4003}] or {4002,4003} - random of 4002 or 4003 ports
         [(2000,3000), {4002,4003}] -random of given range and set
+    :param exclude_ports: A set of known ports that can not be selected.
     :returns: a random free port
     :raises: ValueError
     """
     if ports == -1:
         return None
     elif not ports:
-        return select_random(None)
+        return select_random(None, exclude_ports)
 
     try:
         return int(ports)  # type: ignore[arg-type]
     except TypeError:
         pass
 
     ports_set: Set[int] = set()
@@ -196,8 +198,8 @@
             'You should provide a ports range "[(4000,5000)]"'
             'or "(4000,5000)" or a comma-separated ports set'
             '"[{4000,5000,6000}]" or list of ints "[400,5000,6000,8000]"'
             'or all of them "[(20000, 30000), {48889, 50121}, 4000, 4004]"'
             % (ports,)
         )
 
-    return select_random(ports_set)
+    return select_random(ports_set, exclude_ports)
```

### Comparing `port-for-0.6.3/port_for/cmd.py` & `port-for-0.7.0/port_for/cmd.py`

 * *Files identical despite different names*

### Comparing `port-for-0.6.3/port_for/docopt.py` & `port-for-0.7.0/port_for/docopt.py`

 * *Files identical despite different names*

### Comparing `port-for-0.6.3/port_for/ephemeral.py` & `port-for-0.7.0/port_for/ephemeral.py`

 * *Files identical despite different names*

### Comparing `port-for-0.6.3/port_for/store.py` & `port-for-0.7.0/port_for/store.py`

 * *Files identical despite different names*

### Comparing `port-for-0.6.3/port_for/utils.py` & `port-for-0.7.0/port_for/utils.py`

 * *Files identical despite different names*

### Comparing `port-for-0.6.3/port_for.egg-info/PKG-INFO` & `port-for-0.7.0/port_for.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-for
-Version: 0.6.3
+Version: 0.7.0
 Summary: Utility that helps with local TCP ports management. It can find an unused TCP localhost port and remember the association.
 Author-email: Mikhail Korobov <kmike84@gmail.com>
 Maintainer-email: Grzegorz Śliwiński <fizyk+pypi@fizyk.dev>
 License: Copyright (c) 2012 Mikhail Korobov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -22,15 +22,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
         THE SOFTWARE.
         
 Project-URL: Source, https://github.com/kmike/port-for/
 Project-URL: Bug Tracker, https://github.com/kmike/port-for/issues
-Project-URL: Changelog, https://github.com/kmike/port-for/blob/v0.6.3/CHANGES.rst
+Project-URL: Changelog, https://github.com/kmike/port-for/blob/v0.7.0/CHANGES.rst
 Keywords: port,posix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `port-for-0.6.3/pyproject.toml` & `port-for-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "port-for"
-version = "0.6.3"
+version = "0.7.0"
 description = "Utility that helps with local TCP ports management. It can find an unused TCP localhost port and remember the association."
 readme = "README.rst"
 keywords = ["port", "posix"]
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Mikhail Korobov", email = "kmike84@gmail.com"}
 ]
@@ -29,15 +29,15 @@
     "Topic :: Internet :: WWW/HTTP :: Site Management",
 ]
 requires-python = ">= 3.7"
 
 [project.urls]
 "Source" = "https://github.com/kmike/port-for/"
 "Bug Tracker" = "https://github.com/kmike/port-for/issues"
-"Changelog" = "https://github.com/kmike/port-for/blob/v0.6.3/CHANGES.rst"
+"Changelog" = "https://github.com/kmike/port-for/blob/v0.7.0/CHANGES.rst"
 
 [project.scripts]
 port-for = "port_for.cmd:main"
 
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
@@ -83,15 +83,15 @@
 
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.6.3"
+current = "0.7.0"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

