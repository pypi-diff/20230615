# Comparing `tmp/RaspyGeo-0.0.4.tar.gz` & `tmp/RaspyGeo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RaspyGeo-0.0.4.tar", last modified: Mon May  1 20:02:43 2023, max compression
+gzip compressed data, was "RaspyGeo-1.0.0.tar", last modified: Thu Jun 15 17:02:33 2023, max compression
```

## Comparing `RaspyGeo-0.0.4.tar` & `RaspyGeo-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 20:02:43.843059 RaspyGeo-0.0.4/
--rw-rw-rw-   0        0        0    35823 2023-03-16 22:03:16.000000 RaspyGeo-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     6542 2023-05-01 20:02:43.844056 RaspyGeo-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5922 2023-05-01 20:02:15.000000 RaspyGeo-0.0.4/README.md
--rw-rw-rw-   0        0        0        0 2022-05-18 19:11:54.000000 RaspyGeo-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      802 2023-05-01 20:02:43.845054 RaspyGeo-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-01 20:02:43.688850 RaspyGeo-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 20:02:43.778223 RaspyGeo-0.0.4/src/RaspyGeo/
--rw-rw-rw-   0        0        0      156 2023-03-28 20:02:11.000000 RaspyGeo-0.0.4/src/RaspyGeo/__init__.py
--rw-rw-rw-   0        0        0     1463 2023-03-27 15:03:57.000000 RaspyGeo-0.0.4/src/RaspyGeo/display.py
--rw-rw-rw-   0        0        0    13548 2023-05-01 19:54:09.000000 RaspyGeo-0.0.4/src/RaspyGeo/geofun.py
--rw-rw-rw-   0        0        0     5645 2023-03-24 22:15:32.000000 RaspyGeo-0.0.4/src/RaspyGeo/hecgeo.py
--rw-rw-rw-   0        0        0     3628 2023-05-01 19:53:26.000000 RaspyGeo-0.0.4/src/RaspyGeo/iterate.py
--rw-rw-rw-   0        0        0     5175 2023-03-29 20:51:11.000000 RaspyGeo-0.0.4/src/RaspyGeo/parse_geo.py
--rw-rw-rw-   0        0        0     2518 2023-03-28 18:30:20.000000 RaspyGeo-0.0.4/src/RaspyGeo/testing.py
--rw-rw-rw-   0        0        0     7806 2023-03-29 20:52:49.000000 RaspyGeo-0.0.4/src/RaspyGeo/write_geo.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:02:43.842063 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/
--rw-rw-rw-   0        0        0     6542 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 20:02:43.000000 RaspyGeo-0.0.4/src/RaspyGeo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 17:02:33.362283 RaspyGeo-1.0.0/
+-rw-rw-rw-   0        0        0    35823 2023-03-16 22:03:16.000000 RaspyGeo-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     6542 2023-06-15 17:02:33.363280 RaspyGeo-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5922 2023-05-01 20:02:15.000000 RaspyGeo-1.0.0/README.md
+-rw-rw-rw-   0        0        0        0 2022-05-18 19:11:54.000000 RaspyGeo-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      802 2023-06-15 17:02:33.364277 RaspyGeo-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 17:02:33.093305 RaspyGeo-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 17:02:33.269274 RaspyGeo-1.0.0/src/RaspyGeo/
+-rw-rw-rw-   0        0        0      156 2023-03-28 20:02:11.000000 RaspyGeo-1.0.0/src/RaspyGeo/__init__.py
+-rw-rw-rw-   0        0        0     1463 2023-03-27 15:03:57.000000 RaspyGeo-1.0.0/src/RaspyGeo/display.py
+-rw-rw-rw-   0        0        0    14388 2023-06-15 16:38:12.000000 RaspyGeo-1.0.0/src/RaspyGeo/geofun.py
+-rw-rw-rw-   0        0        0     5645 2023-03-24 22:15:32.000000 RaspyGeo-1.0.0/src/RaspyGeo/hecgeo.py
+-rw-rw-rw-   0        0        0     3628 2023-05-01 19:53:26.000000 RaspyGeo-1.0.0/src/RaspyGeo/iterate.py
+-rw-rw-rw-   0        0        0     5175 2023-03-29 20:51:11.000000 RaspyGeo-1.0.0/src/RaspyGeo/parse_geo.py
+-rw-rw-rw-   0        0        0     2518 2023-03-28 18:30:20.000000 RaspyGeo-1.0.0/src/RaspyGeo/testing.py
+-rw-rw-rw-   0        0        0     7806 2023-03-29 20:52:49.000000 RaspyGeo-1.0.0/src/RaspyGeo/write_geo.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:02:33.361287 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/
+-rw-rw-rw-   0        0        0     6542 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 17:02:33.000000 RaspyGeo-1.0.0/src/RaspyGeo.egg-info/top_level.txt
```

### Comparing `RaspyGeo-0.0.4/LICENSE` & `RaspyGeo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.4/PKG-INFO` & `RaspyGeo-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RaspyGeo
-Version: 0.0.4
+Version: 1.0.0
 Summary: Automated geometry scenario runner (loosely analogous to the Geometry Editor tool) for HEC-RAS
 Home-page: https://github.com/quantum-dan/RaspyGeo
 Author: Daniel Philippus
 Author-email: daniel@dphilippus.com
 Project-URL: Bug Tracker, https://github.com/quantum-dan/RaspyGeo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `RaspyGeo-0.0.4/README.md` & `RaspyGeo-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.4/setup.cfg` & `RaspyGeo-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2052 6173 7079 4765 6f0d 0a76 6572   = RaspyGeo..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e34 0d0a 6175  sion = 0.0.4..au
+00000020: 7369 6f6e 203d 2031 2e30 2e30 0d0a 6175  sion = 1.0.0..au
 00000030: 7468 6f72 203d 2044 616e 6965 6c20 5068  thor = Daniel Ph
 00000040: 696c 6970 7075 730d 0a61 7574 686f 725f  ilippus..author_
 00000050: 656d 6169 6c20 3d20 6461 6e69 656c 4064  email = daniel@d
 00000060: 7068 696c 6970 7075 732e 636f 6d0d 0a64  philippus.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2041 7574  escription = Aut
 00000080: 6f6d 6174 6564 2067 656f 6d65 7472 7920  omated geometry 
 00000090: 7363 656e 6172 696f 2072 756e 6e65 7220  scenario runner
```

### Comparing `RaspyGeo-0.0.4/src/RaspyGeo/display.py` & `RaspyGeo-1.0.0/src/RaspyGeo/display.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.4/src/RaspyGeo/geofun.py` & `RaspyGeo-1.0.0/src/RaspyGeo/geofun.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 
 
 def set_afp(
         lfc_w,
         lfc_h,
         lfc_z,
         afp_wfun,
+        afp_h,
         afp_z,
         afpside_n,
         afp_n,
         lfcside_n,
         lfc_n
         ):
     """
@@ -128,15 +129,16 @@
         - Active floodplain side slope (x:y); if the AFP edges are above the
             current channel, then it will fill up to the maximum channel
             height.
         - Active floodplain width as a function of available channel width
             (allowing either constant
             or fraction, etc.)  This is provided as half-width, i.e.
             available per side.
-        - Daylight slope (AFP side slope) roughness
+        - AFP height; above the AFP height, it will daylight horizontally
+        - AFP side slope roughness
         - AFP roughness
         - LFC side slope roughness
         - LFC bottom roughness
     Bank stations are set at the top edges of the LFC.
     Units are assumed to be consistent with geometry and not accounted for.
     """
     def geofun(coordinates, roughness, banks):
@@ -174,29 +176,45 @@
         afp_bleft = lfc_tleft - afp_w
         afp_bright = lfc_tright + afp_w
         # Now the trickiest part: where do the side slopes intersect with
         # the existing channel (where do they daylight?)  Identifying
         # the daylight point gets its own function, for simplicity.
         # daylight(x, y, start, z, direction) returns the x-coordinate of
         # daylight.
+        # If the channel is close, just daylight it.  Otherwise, use
+        # the AFP height.
+        #
+        # Current bugs:
+            # Not setting n at AFP-outer if it is the channel edge
+            # Duplicate points at AFP-outer
+            # Sometimes just randomly losing roughness?
+        afp_dx = afp_h * afp_z
         afp_tleft = daylight(xs0, ys0, afp_bleft,
                              lfc_ty, afp_z, -1) if avail > 0 else \
             afp_bleft - 0.1
+        afp_tleft = afp_tleft if afp_bleft - afp_tleft <= afp_dx else \
+            afp_bleft - afp_dx
         afp_tleft = afp_tleft if afp_bleft - afp_tleft > 0.01 else \
             afp_bleft - 0.1
         afp_tright = daylight(xs0, ys0, afp_bright,
                               lfc_ty, afp_z, 1) if avail > 0 else \
             afp_bright + 0.1
+        afp_tright = afp_tright if afp_tright - afp_bright <= afp_dx else \
+            afp_bright + afp_dx
         afp_tright = afp_tright if afp_tright - afp_bright > 0.01 else \
             afp_bright + 0.1
         # Compute height based on side slope width and slope
         afp_tyleft = lfc_ty + (afp_bleft - afp_tleft) / afp_z if \
             avail > 0 else lfc_ty
         afp_tyright = lfc_ty + (afp_tright - afp_bright) / afp_z if \
             avail > 0 else lfc_ty
+
+        # Next, find the outer points for a flat main channel.
+        # afp_oleft = daylight(xs0, ys0, afp_tleft, afp_tyleft, 999, -1)
+        # afp_oright = daylight(xs0, ys0, afp_tright, afp_tyright, 999, 1)
         # We now have all key points.  Next, we rebuild the coordinates
         # and specify roughness.
         # The first step is to determine what, if any, of the channel is kept.
         # Also need a way to account for [near-]vertical walls at daylight
         keepl = [(x, ys0[ix]) for (ix, x) in enumerate(xs0)
                  if x < (afp_tleft - 0.1) or
                  (
```

### Comparing `RaspyGeo-0.0.4/src/RaspyGeo/hecgeo.py` & `RaspyGeo-1.0.0/src/RaspyGeo/hecgeo.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.4/src/RaspyGeo/iterate.py` & `RaspyGeo-1.0.0/src/RaspyGeo/iterate.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.4/src/RaspyGeo/parse_geo.py` & `RaspyGeo-1.0.0/src/RaspyGeo/parse_geo.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.4/src/RaspyGeo/testing.py` & `RaspyGeo-1.0.0/src/RaspyGeo/testing.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.4/src/RaspyGeo/write_geo.py` & `RaspyGeo-1.0.0/src/RaspyGeo/write_geo.py`

 * *Files identical despite different names*

### Comparing `RaspyGeo-0.0.4/src/RaspyGeo.egg-info/PKG-INFO` & `RaspyGeo-1.0.0/src/RaspyGeo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RaspyGeo
-Version: 0.0.4
+Version: 1.0.0
 Summary: Automated geometry scenario runner (loosely analogous to the Geometry Editor tool) for HEC-RAS
 Home-page: https://github.com/quantum-dan/RaspyGeo
 Author: Daniel Philippus
 Author-email: daniel@dphilippus.com
 Project-URL: Bug Tracker, https://github.com/quantum-dan/RaspyGeo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

