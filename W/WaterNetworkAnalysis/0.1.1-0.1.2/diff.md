# Comparing `tmp/WaterNetworkAnalysis-0.1.1.tar.gz` & `tmp/WaterNetworkAnalysis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WaterNetworkAnalysis-0.1.1.tar", last modified: Mon Feb 13 02:39:17 2023, max compression
+gzip compressed data, was "WaterNetworkAnalysis-0.1.2.tar", last modified: Thu Jun 15 03:42:02 2023, max compression
```

## Comparing `WaterNetworkAnalysis-0.1.1.tar` & `WaterNetworkAnalysis-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:39:17.635667 WaterNetworkAnalysis-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-02-13 02:39:02.000000 WaterNetworkAnalysis-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-13 02:39:02.000000 WaterNetworkAnalysis-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-02-13 02:39:17.635667 WaterNetworkAnalysis-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-02-13 02:39:02.000000 WaterNetworkAnalysis-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:39:17.631667 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis/
--rw-r--r--   0 runner    (1001) docker     (123)    32745 2023-02-13 02:39:02.000000 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis/WaterNetworkAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-13 02:39:02.000000 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:39:17.631667 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-02-13 02:39:17.000000 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-13 02:39:17.000000 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 02:39:17.000000 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 02:39:17.000000 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-13 02:39:17.000000 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-13 02:39:17.000000 WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-13 02:39:17.635667 WaterNetworkAnalysis-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-02-13 02:39:02.000000 WaterNetworkAnalysis-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 02:39:17.635667 WaterNetworkAnalysis-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 02:39:02.000000 WaterNetworkAnalysis-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-02-13 02:39:02.000000 WaterNetworkAnalysis-0.1.1/tests/test_WaterNetworkAnalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:42:02.696019 WaterNetworkAnalysis-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-15 03:41:48.000000 WaterNetworkAnalysis-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 03:41:48.000000 WaterNetworkAnalysis-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-15 03:42:02.696019 WaterNetworkAnalysis-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-15 03:41:48.000000 WaterNetworkAnalysis-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:42:02.696019 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    32134 2023-06-15 03:41:48.000000 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis/WaterNetworkAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-15 03:41:48.000000 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:42:02.696019 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-06-15 03:42:02.000000 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-15 03:42:02.000000 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:42:02.000000 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 03:42:02.000000 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-15 03:42:02.000000 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 03:42:02.000000 WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-15 03:42:02.696019 WaterNetworkAnalysis-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-15 03:41:48.000000 WaterNetworkAnalysis-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 03:42:02.696019 WaterNetworkAnalysis-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 03:41:48.000000 WaterNetworkAnalysis-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-15 03:41:48.000000 WaterNetworkAnalysis-0.1.2/tests/test_WaterNetworkAnalysis.py
```

### Comparing `WaterNetworkAnalysis-0.1.1/LICENSE` & `WaterNetworkAnalysis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `WaterNetworkAnalysis-0.1.1/PKG-INFO` & `WaterNetworkAnalysis-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaterNetworkAnalysis
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/JecaTosovic/WaterNetworkAnalysis
 Download-URL: https://pypi.org/project/WaterNetworkAnalysis/
 Author: Domagoj Fijan, Jelena Tosovic, Marko Jukic, Urban Bren
 Author-email: jecat_90@live.com
 License: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Project-URL: Homepage, https://github.com/JecaTosovic/WaterNetworkAnalysis
 Project-URL: Documentation, https://WaterNetworkAnalysis.readthedocs.io/
```

### Comparing `WaterNetworkAnalysis-0.1.1/README.rst` & `WaterNetworkAnalysis-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis/WaterNetworkAnalysis.py` & `WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis/WaterNetworkAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,16 +307,14 @@
 def extract_waters_from_trajectory(
     selection_center: np.ndarray,
     trajectory: str,
     topology: str | None = None,
     dist: float = 12.0,
     SOL: str = "SOL",
     OW: str = "OW",
-    HW1: str = "HW1",
-    HW2: str = "HW2",
     save_file: str | None = None,
 ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Extract waters for clustering analysis.
 
     Calculates water (oxygen and hydrogen) coordinates for all the
     waters in the aligned trajectory using MDAnalysis for further use in water
     clustering. The trajectory should be aligned previously.
@@ -327,18 +325,14 @@
         trajectory (str): Trajectory file name.
         topology (str | None, optional): Topology file name. Defaults to None.
         dist (float, optional): Distance around the center of selection
             inside which water molecules will be sampled. Defaults to 12.0.
         SOL (str, optional): Residue name for waters. Defaults to "SOL".
         OW (str, optional): Name of the oxygen atom in water molecules.
             Defaults to "OW".
-        HW1 (str, optional): Name of hydrogen 1 atom in water molecules.
-            Defaults to "HW1".
-        HW2 (str, optional): Name of hydrogen 2 atom in water molecules.
-            Defaults to "HW2".
         save_file (str | None, optional): File to which coordinates will
             be saved. If none doesn't save to a file. Defaults to None.
 
     Returns:
         tuple[np.ndarray, np.ndarray]:
             returns xyz numpy arrays that contain coordinates of oxygens,
             and combined array of hydrogen 1 and hydrogen 2
@@ -349,21 +343,23 @@
         resids = [8,12,143,144]
         coordO, coordH = extract_waters_from_trajectory(
             get_center_of_selection(get_selection_string_from_resnums(resids)),
             trajectory = 'trajectory.xtc',
             topology = 'topology.tpr'
         )
     """
-    # think about another method of selecting waters - ie within some distance of an atom index?
     if topology:
         u = mda.Universe(topology, trajectory)
     else:
         u = mda.Universe(trajectory)
     coordsH = []
     coordsO = []
+    waters = u.select_atoms(f'resname {SOL}')
+    if len(waters.bonds) == 0:
+        waters.guess_bonds()
     # loop over
     for nn, k in enumerate(u.trajectory):
         Os = u.select_atoms(
             "name "
             + str(OW)
             + " and resname "
             + str(SOL)
@@ -372,31 +368,20 @@
             + " "
             + str(selection_center[1])
             + " "
             + str(selection_center[2])
             + " "
             + str(dist)
         )
-        for i, j in zip(Os.positions, Os.indices):
-            Hs = u.select_atoms(
-                "(name "
-                + str(HW1)
-                + " or name "
-                + str(HW2)
-                + ") and around 1.0 index "
-                + str(j)
-            )
+        for i, j in zip(Os.positions, Os):
+            Hs = j.bonded_atoms
             if len(Hs) != 2:
-                # raise Exception(
-                #    f"Water {j} in snapshot {i} has too many hydrogens ({len(Hs)})."
-                # )
-                print(
-                    f"Water {j} in snapshot {i} has too many hydrogens ({len(Hs)}). Skipping."
+                raise Exception(
+                   f"Water {j} in snapshot {i} has too many hydrogens ({len(Hs)})."
                 )
-                continue
             for l in Hs.positions:
                 coordsH.append(l)
             coordsO.append(i)
     Odata: np.ndarray = np.asarray(coordsO)
     coordsH = np.asarray(coordsH)
     Opos, H1, H2 = get_orientations_from_positions(Odata, coordsH)
     # SAVEs full XYZ coordinates, not O coordinates and h orientations!!!!!
```

### Comparing `WaterNetworkAnalysis-0.1.1/WaterNetworkAnalysis.egg-info/PKG-INFO` & `WaterNetworkAnalysis-0.1.2/WaterNetworkAnalysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WaterNetworkAnalysis
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/JecaTosovic/WaterNetworkAnalysis
 Download-URL: https://pypi.org/project/WaterNetworkAnalysis/
 Author: Domagoj Fijan, Jelena Tosovic, Marko Jukic, Urban Bren
 Author-email: jecat_90@live.com
 License: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Project-URL: Homepage, https://github.com/JecaTosovic/WaterNetworkAnalysis
 Project-URL: Documentation, https://WaterNetworkAnalysis.readthedocs.io/
```

### Comparing `WaterNetworkAnalysis-0.1.1/setup.py` & `WaterNetworkAnalysis-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         long_description = handle.read()
 except:
     long_description = "\n".join(short_description[2:])
 
 
 setup(
     name="WaterNetworkAnalysis",
-    version="0.1.1",
+    version="0.1.2",
     author="Domagoj Fijan, Jelena Tosovic, Marko Jukic, Urban Bren",
     author_email="jecat_90@live.com",
     description=short_description[0],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     license="License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     keywords=("simulation analysis molecular dynamics biosimulation conserved water "),
```

### Comparing `WaterNetworkAnalysis-0.1.1/tests/test_WaterNetworkAnalysis.py` & `WaterNetworkAnalysis-0.1.2/tests/test_WaterNetworkAnalysis.py`

 * *Files identical despite different names*

