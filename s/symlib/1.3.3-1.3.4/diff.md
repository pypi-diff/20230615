# Comparing `tmp/symlib-1.3.3.tar.gz` & `tmp/symlib-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.3.3.tar", last modified: Fri Jun  2 20:23:33 2023, max compression
+gzip compressed data, was "symlib-1.3.4.tar", last modified: Wed Jun 14 22:30:24 2023, max compression
```

## Comparing `symlib-1.3.3.tar` & `symlib-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 20:23:33.481546 symlib-1.3.3/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.3/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-02 20:23:33.481428 symlib-1.3.3/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.3/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.3/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-02 20:23:33.481578 symlib-1.3.3/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-02 20:23:27.000000 symlib-1.3.3/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 20:23:33.480599 symlib-1.3.3/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1658 2023-05-25 11:19:28.000000 symlib-1.3.3/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.3/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    52489 2023-05-25 11:19:28.000000 symlib-1.3.3/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)    36176 2023-06-02 20:23:27.000000 symlib-1.3.3/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     8508 2023-05-06 00:43:01.000000 symlib-1.3.3/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-02 20:23:33.481284 symlib-1.3.3/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      287 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-02 20:23:33.000000 symlib-1.3.3/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-14 22:30:24.781653 symlib-1.3.4/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.4/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-14 22:30:24.781537 symlib-1.3.4/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.4/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.4/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-14 22:30:24.781685 symlib-1.3.4/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-14 22:30:22.000000 symlib-1.3.4/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-14 22:30:24.780836 symlib-1.3.4/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1658 2023-05-25 11:19:28.000000 symlib-1.3.4/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.4/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    53111 2023-06-14 22:30:07.000000 symlib-1.3.4/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)    36176 2023-06-02 20:23:27.000000 symlib-1.3.4/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     9876 2023-06-14 22:30:07.000000 symlib-1.3.4/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-14 22:30:24.781359 symlib-1.3.4/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      287 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-14 22:30:24.000000 symlib-1.3.4/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.3.3/LICENSE` & `symlib-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.3.3/PKG-INFO` & `symlib-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.3
+Version: 1.3.4
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.3.3/setup.py` & `symlib-1.3.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.3.3"
+version = "1.3.4"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.3.3/symlib/__init__.py` & `symlib-1.3.4/symlib/__init__.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.3/symlib/file_management.py` & `symlib-1.3.4/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.3/symlib/lib.py` & `symlib-1.3.4/symlib/lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -257,42 +257,50 @@
 "ns"), the particle mass in Msun/h, "mp", the Plummer-equivalent force
 softening scale in comoving kpc/h, "eps", and for convience, "h100". "n_snap" is
 the number of snapshots in the suite.
 """
 parameter_table = {
     "SymphonyLMC": _chinchilla_cosmology.copy(),
     "SymphonyMilkyWay": _chinchilla_cosmology.copy(),
+    "SymphonyMilkyWayDisk": _chinchilla_cosmology.copy(),
+    "SymphonyMilkyWayDiskDMO": _chinchilla_cosmology.copy(),
     "SymphonyMilkyWayLR": _chinchilla_cosmology.copy(),
     "SymphonyMilkyWayHR": _chinchilla_cosmology.copy(),
     "SymphonyGroup": _chinchilla_cosmology.copy(),
     "SymphonyLCluster": _banerjee_cosmology.copy(),
     "SymphonyCluster": _carmen_cosmology.copy(),
     "MWest": _chinchilla_cosmology.copy(),
 }
 
 parameter_table["SymphonyLMC"]["eps"] = 0.080
 parameter_table["SymphonyMilkyWay"]["eps"] = 0.170
+parameter_table["SymphonyMilkyWayDisk"]["eps"] = 0.170*2
+parameter_table["SymphonyMilkyWayDiskDMO"]["eps"] = 0.170*2
 parameter_table["SymphonyMilkyWayLR"]["eps"] = 0.170
 parameter_table["SymphonyMilkyWayHR"]["eps"] = 0.170/2
 parameter_table["SymphonyGroup"]["eps"] = 0.360
 parameter_table["SymphonyLCluster"]["eps"] = 1.200
 parameter_table["SymphonyCluster"]["eps"] = 3.250
 parameter_table["MWest"]["eps"] = 0.170
 
 parameter_table["SymphonyLMC"]["mp"] = 3.52476e4
 parameter_table["SymphonyMilkyWay"]["mp"] = 2.81981e5
+parameter_table["SymphonyMilkyWayDisk"]["mp"] = 2.81981e5*8
+parameter_table["SymphonyMilkyWayDiskDMO"]["mp"] = 2.81981e5*8
 parameter_table["SymphonyMilkyWayLR"]["mp"] = 2.81981e5
 parameter_table["SymphonyMilkyWayHR"]["mp"] = 2.81981e5/8
 parameter_table["SymphonyGroup"]["mp"] = 2.25585e6
 parameter_table["SymphonyLCluster"]["mp"] = 1.51441632e8
 parameter_table["SymphonyCluster"]["mp"] = 1.26201360e8
 parameter_table["MWest"]["mp"] = 2.81981e5
 
 parameter_table["SymphonyLMC"]["n_snap"] = 236
 parameter_table["SymphonyMilkyWay"]["n_snap"] = 236
+parameter_table["SymphonyMilkyWayDisk"]["n_snap"] = 236
+parameter_table["SymphonyMilkyWayDiskDMO"]["n_snap"] = 236
 parameter_table["SymphonyMilkyWayLR"]["n_snap"] = 236
 parameter_table["SymphonyMilkyWayHR"]["n_snap"] = 236
 parameter_table["SymphonyGroup"]["n_snap"] = 236
 parameter_table["SymphonyLCluster"]["n_snap"] = 200
 parameter_table["SymphonyCluster"]["n_snap"] = 200
 parameter_table["MWest"]["n_snap"] = 236
 
@@ -348,18 +356,20 @@
     the given directory.
     """
     if dir_name in _SCALE_FACTOR_CACHE:
         return _SCALE_FACTOR_CACHE[dir_name]
 
     # TODO: individual halo-by-halo scale factors
     suite_name = halo_dir_to_suite_name(dir_name)
-    if (suite_name in ["SymphonyLMC", "SymphonyGroup",
+    if (suite_name in ["SymphonyLMC", "SymphonyGroup", "SymphonyMilkyWayDisk",
+                       "SymphonyMilkyWayDiskDMO",
                       "SymphonyMilkyWay", "MWest", "SymphonyMilkyWayLR",
                        "SymphonyMilkyWayHR"] or
-        dir_name in ["SymphonyLMC", "SymphonyGroup",
+        dir_name in ["SymphonyLMC", "SymphonyGroup", "SymphonyMilkyWayDisk",
+                       "SymphonyMilkyWayDiskDMO",
                      "SymphonyMilkyWay", "MWest", "SymphonyMilkyWayLR",
                      "SymphonyMilkyWayHR"]):
         default = 10**np.linspace(np.log10(0.05), np.log10(1), 236)
     elif (suite_name in ["SymphonyLCluster",  "SymphonyCluster"] or
           dir_name in ["SymphonyLCluster",  "SymphonyCluster"]):
         default = 10**np.linspace(np.log10(0.075), np.log10(1), 200)
     else:
```

### Comparing `symlib-1.3.3/symlib/star_tagging.py` & `symlib-1.3.4/symlib/star_tagging.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.3/symlib/util.py` & `symlib-1.3.4/symlib/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -80,21 +80,25 @@
             h["v"][hi,:,dim] -= v0
                 
             h["x"][hi,:,dim] *= 1e3*scale/param["h100"]
             
             if dim == 0:
                 h["rvir"][hi,:] *= 1e3*scale/param["h100"]
                 h["mvir"][hi,:] *= 1/param["h100"]
-
+                h["rvmax"][hi,:] *= scale/param["h100"]
     
     for hi in range(len(h)):
-        invalid = h[hi]["rvir"] < 0
-        h[hi, invalid]["rvir"] = -1
-        h[hi, invalid]["x"] = -1
-        h[hi, invalid]["v"] = -1
+        invalid = np.where(~h[hi,:]["ok"])[0]
+        h["mvir"][hi,invalid] = -1
+        h["rvir"][hi,invalid] = -1
+        h["rvmax"][hi,invalid] = -1
+        h["x"][hi,invalid] = -1
+        h["v"][hi,invalid] = -1
+        h["vmax"][hi,invalid] = -1
+        h["cvir"][hi,invalid] = -1
         
     return h
 
 DEFAULT_HALO_NAMES = {
     "SymphonyLMC": sorted([
         "Halo032", "Halo097", "Halo218", "Halo374", "Halo463", "Halo567", "Halo721", "Halo853",
         "Halo059", "Halo104", "Halo296", "Halo380", "Halo4662", "Halo575", "Halo767", "Halo914",
@@ -105,14 +109,28 @@
     "SymphonyMilkyWay": sorted([
         "Halo023", "Halo268", "Halo364", "Halo440", "Halo558", "Halo641", "Halo797", "Halo878", "Halo939",
         "Halo088", "Halo270", "Halo374", "Halo460", "Halo567", "Halo675", "Halo800", "Halo881", "Halo967",
         "Halo119", "Halo288", "Halo414", "Halo469", "Halo570", "Halo718", "Halo825", "Halo925", "Halo9749",
         "Halo188", "Halo327", "Halo415", "Halo490", "Halo606", "Halo738", "Halo829", "Halo926", "Halo9829",
         "Halo247", "Halo349", "Halo416", "Halo530", "Halo628", "Halo749", "Halo852", "Halo937", "Halo990"
     ]),
+    "SymphonyMilkyWayDisk": sorted([
+        "Halo023", "Halo268", "Halo364", "Halo440", "Halo558", "Halo641", "Halo797", "Halo878", "Halo939",
+        "Halo088", "Halo270", "Halo374", "Halo460", "Halo567", "Halo675", "Halo800", "Halo881", "Halo967",
+        "Halo119", "Halo288", "Halo414", "Halo469", "Halo570", "Halo718", "Halo825", "Halo925", "Halo9749",
+        "Halo188", "Halo327", "Halo415", "Halo490", "Halo606", "Halo738", "Halo829", "Halo926", "Halo9829",
+        "Halo247", "Halo349", "Halo416", "Halo530", "Halo628", "Halo749", "Halo852", "Halo937", "Halo990"
+    ]),
+    "SymphonyMilkyWayDiskDMO": sorted([
+        "Halo023", "Halo268", "Halo364", "Halo440", "Halo558", "Halo641", "Halo797", "Halo878", "Halo939",
+        "Halo088", "Halo270", "Halo374", "Halo460", "Halo567", "Halo675", "Halo800", "Halo881", "Halo967",
+        "Halo119", "Halo288", "Halo414", "Halo469", "Halo570", "Halo718", "Halo825", "Halo925", "Halo9749",
+        "Halo188", "Halo327", "Halo415", "Halo490", "Halo606", "Halo738", "Halo829", "Halo926", "Halo9829",
+        "Halo247", "Halo349", "Halo416", "Halo530", "Halo628", "Halo749", "Halo852", "Halo937", "Halo990"
+    ]),
 
     "SymphonyMilkyWayLR": sorted([
         "Halo023", "Halo247", "Halo268", "Halo530", "Halo829"
     ]),
 
     "SymphonyMilkyWayHR": sorted([
         "Halo023", "Halo247", "Halo268", "Halo530", "Halo829"
```

### Comparing `symlib-1.3.3/symlib.egg-info/PKG-INFO` & `symlib-1.3.4/symlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.3
+Version: 1.3.4
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

