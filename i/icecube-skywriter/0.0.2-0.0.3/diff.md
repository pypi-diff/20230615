# Comparing `tmp/icecube-skywriter-0.0.2.tar.gz` & `tmp/icecube-skywriter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skywriter-0.0.2.tar", last modified: Tue Apr 18 22:32:32 2023, max compression
+gzip compressed data, was "icecube-skywriter-0.0.3.tar", last modified: Thu Jun 15 20:39:55 2023, max compression
```

## Comparing `icecube-skywriter-0.0.2.tar` & `icecube-skywriter-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1926 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1013 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1926 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      305 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1655 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/skywriter/
--rw-r--r--   0 root         (0) root         (0)      592 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/skywriter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8376 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/skywriter/i3_to_json.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/skywriter/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:39:55.283385 icecube-skywriter-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-06-15 20:39:52.000000 icecube-skywriter-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-06-15 20:39:55.283385 icecube-skywriter-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-06-15 20:39:52.000000 icecube-skywriter-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:39:55.283385 icecube-skywriter-0.0.3/icecube_skywriter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-06-15 20:39:55.000000 icecube-skywriter-0.0.3/icecube_skywriter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-15 20:39:55.000000 icecube-skywriter-0.0.3/icecube_skywriter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 20:39:55.000000 icecube-skywriter-0.0.3/icecube_skywriter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-15 20:39:55.000000 icecube-skywriter-0.0.3/icecube_skywriter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-15 20:39:55.000000 icecube-skywriter-0.0.3/icecube_skywriter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-06-15 20:39:55.283385 icecube-skywriter-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-15 20:39:52.000000 icecube-skywriter-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 20:39:55.283385 icecube-skywriter-0.0.3/skywriter/
+-rw-r--r--   0 root         (0) root         (0)      592 2023-06-15 20:39:53.000000 icecube-skywriter-0.0.3/skywriter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8374 2023-06-15 20:39:52.000000 icecube-skywriter-0.0.3/skywriter/i3_to_json.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-15 20:39:52.000000 icecube-skywriter-0.0.3/skywriter/py.typed
```

### Comparing `icecube-skywriter-0.0.2/LICENSE` & `icecube-skywriter-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skywriter-0.0.2/PKG-INFO` & `icecube-skywriter-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skywriter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Upstream Tools for SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skywriter
 Download-URL: https://pypi.org/project/icecube-skywriter/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skywriter/issues
```

### Comparing `icecube-skywriter-0.0.2/README.md` & `icecube-skywriter-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skywriter-0.0.2/icecube_skywriter.egg-info/PKG-INFO` & `icecube-skywriter-0.0.3/icecube_skywriter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icecube-skywriter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Upstream Tools for SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skywriter
 Download-URL: https://pypi.org/project/icecube-skywriter/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skywriter/issues
```

### Comparing `icecube-skywriter-0.0.2/setup.cfg` & `icecube-skywriter-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `icecube-skywriter-0.0.2/skywriter/__init__.py` & `icecube-skywriter-0.0.3/skywriter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skywriter-0.0.2/skywriter/i3_to_json.py` & `icecube-skywriter-0.0.3/skywriter/i3_to_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 frame['I3EventHeader'].start_time.mod_julian_day_double)
             fullmsg[extra_namer.get(i3part_key, i3part_key)] = {'ra':ra.item(), 'dec':dec.item()}
     except KeyError as e:
         print('Q-frame was split into multiple P-frames, skipping subevents not in input i3 file', e)
         return False
 
     if 'I3MCTree' in frame:
-        prim = dataclasses.get_most_energetic_primary(frame['I3MCTree'])
+        prim = dataclasses.get_most_energetic_inice(frame['I3MCTree'])
         muhi = dataclasses.get_most_energetic_muon(frame['I3MCTree'])
         ra, dec = astro.dir_to_equa(prim.dir.zenith, prim.dir.azimuth,
                                     frame['I3EventHeader'].start_time.mod_julian_day_double)
 
         fullmsg['true'] = {'ra':ra.item(), 'dec':dec.item(), 'eprim': prim.energy}
 
         if muhi is not None:
```

