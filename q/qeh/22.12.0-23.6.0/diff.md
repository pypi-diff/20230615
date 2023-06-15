# Comparing `tmp/qeh-22.12.0.tar.gz` & `tmp/qeh-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qeh-22.12.0.tar", last modified: Mon Dec 12 10:54:25 2022, max compression
+gzip compressed data, was "qeh-23.6.0.tar", last modified: Thu Jun 15 11:27:25 2023, max compression
```

## Comparing `qeh-22.12.0.tar` & `qeh-23.6.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2022-12-12 10:54:25.752431 qeh-22.12.0/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    35147 2022-12-12 09:43:49.000000 qeh-22.12.0/COPYING.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      585 2022-12-12 09:43:49.000000 qeh-22.12.0/LICENSE
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1088 2022-12-12 10:54:25.752431 qeh-22.12.0/PKG-INFO
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      336 2022-12-12 09:43:49.000000 qeh-22.12.0/README.md
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2022-12-12 10:54:25.752431 qeh-22.12.0/qeh/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      249 2022-12-12 10:53:07.000000 qeh-22.12.0/qeh/__init__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       32 2022-12-12 09:43:49.000000 qeh-22.12.0/qeh/__main__.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    10571 2022-12-12 09:43:49.000000 qeh-22.12.0/qeh/buildingblocks.py
--rw-rw-r--   0 jensj     (1000) jensj     (1000)    76898 2022-12-12 10:52:50.000000 qeh-22.12.0/qeh/qeh.py
-drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2022-12-12 10:54:25.752431 qeh-22.12.0/qeh.egg-info/
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1088 2022-12-12 10:54:25.000000 qeh-22.12.0/qeh.egg-info/PKG-INFO
--rw-rw-r--   0 jensj     (1000) jensj     (1000)      267 2022-12-12 10:54:25.000000 qeh-22.12.0/qeh.egg-info/SOURCES.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        1 2022-12-12 10:54:25.000000 qeh-22.12.0/qeh.egg-info/dependency_links.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       56 2022-12-12 10:54:25.000000 qeh-22.12.0/qeh.egg-info/entry_points.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       47 2022-12-12 10:54:25.000000 qeh-22.12.0/qeh.egg-info/requires.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)        4 2022-12-12 10:54:25.000000 qeh-22.12.0/qeh.egg-info/top_level.txt
--rw-rw-r--   0 jensj     (1000) jensj     (1000)       38 2022-12-12 10:54:25.752431 qeh-22.12.0/setup.cfg
--rw-rw-r--   0 jensj     (1000) jensj     (1000)     1214 2022-12-12 09:43:49.000000 qeh-22.12.0/setup.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-15 11:27:25.703298 qeh-23.6.0/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    35147 2022-12-02 08:37:06.000000 qeh-23.6.0/COPYING.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      585 2022-12-02 08:37:06.000000 qeh-23.6.0/LICENSE
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1050 2023-06-15 11:27:25.703298 qeh-23.6.0/PKG-INFO
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      336 2022-12-02 08:37:06.000000 qeh-23.6.0/README.md
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-15 11:27:25.703298 qeh-23.6.0/qeh/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      248 2023-06-15 10:22:05.000000 qeh-23.6.0/qeh/__init__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       32 2022-12-02 08:37:06.000000 qeh-23.6.0/qeh/__main__.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    10571 2022-12-02 08:37:06.000000 qeh-23.6.0/qeh/buildingblocks.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1188 2023-06-15 11:25:45.000000 qeh-23.6.0/qeh/mos2_test.py
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)    77103 2023-06-15 10:21:42.000000 qeh-23.6.0/qeh/qeh.py
+drwxrwxr-x   0 jensj     (1000) jensj     (1000)        0 2023-06-15 11:27:25.703298 qeh-23.6.0/qeh.egg-info/
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1050 2023-06-15 11:27:25.000000 qeh-23.6.0/qeh.egg-info/PKG-INFO
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)      284 2023-06-15 11:27:25.000000 qeh-23.6.0/qeh.egg-info/SOURCES.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        1 2023-06-15 11:27:25.000000 qeh-23.6.0/qeh.egg-info/dependency_links.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       37 2023-06-15 11:27:25.000000 qeh-23.6.0/qeh.egg-info/entry_points.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       47 2023-06-15 11:27:25.000000 qeh-23.6.0/qeh.egg-info/requires.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)        4 2023-06-15 11:27:25.000000 qeh-23.6.0/qeh.egg-info/top_level.txt
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)       38 2023-06-15 11:27:25.703298 qeh-23.6.0/setup.cfg
+-rw-rw-r--   0 jensj     (1000) jensj     (1000)     1214 2022-12-02 08:37:06.000000 qeh-23.6.0/setup.py
```

### Comparing `qeh-22.12.0/COPYING.txt` & `qeh-23.6.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `qeh-22.12.0/LICENSE` & `qeh-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qeh-22.12.0/PKG-INFO` & `qeh-23.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: qeh
-Version: 22.12.0
+Version: 23.6.0
 Summary: Quantum Electrostatic Heterostructure Model
 Home-page: https://gitlab.com/camd/qeh
 Author: CAMD
 Author-email: mogje@fysik.dtu.dk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -24,9 +22,7 @@
 ===========================================
 The quantum electrostatic heterostructure (QEH) model is a
 fast and accurate model for simulating optical properties
 of stacks of 2D materials (heterostructures).
 
 - Documentation: https://qeh.readthedocs.io
 - Code: https://gitlab.com/camd/qeh.git
-
-
```

### Comparing `qeh-22.12.0/qeh/buildingblocks.py` & `qeh-23.6.0/qeh/buildingblocks.py`

 * *Files identical despite different names*

### Comparing `qeh-22.12.0/qeh/qeh.py` & `qeh-23.6.0/qeh/qeh.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             drho_dipole[i] = np.array(drho_dipole[i])[self.q1: self.q2]
 
         # layers and distances
         self.d = np.array(d) / Bohr  # interlayer distances
         if self.n_layers > 1:
             # space around each layer
             if thicknesses is not None:
-                self.s = thicknesses / Bohr
+                self.s = np.asarray(thicknesses) / Bohr
             else:
                 self.s = (np.insert(self.d, 0, self.d[0]) +
                           np.append(self.d, self.d[-1])) / 2.
 
         else:  # Monolayer calculation
             self.s = [d0 / Bohr]  # Width of single layer
         self.d0 = d0 / Bohr
@@ -276,15 +276,22 @@
         self.poisson_lim = 1000  # above this limit use potential model
         assert system_size < self.poisson_lim
 
         self.z_lim = system_size
         self.dz = 0.05
         # master grid
         self.z_big = np.arange(0, self.z_lim, self.dz)
-        self.z_big -= self.z_big[-1]/2.0
+
+        # If substrate: have symmetric grid w r t 0
+        # else: grid starts at -edgesize/2
+        if self.substrate is None:
+            self.z_big -= edgesize / 2.0
+        else:
+            self.z_big -= self.z_big[-1] / 2.0
+
         self.z0 = np.append(np.array([0]), np.cumsum(self.d))
 
         # arange potential and density
         self.chi_monopole = chi_monopole
         if include_dipole:
             self.chi_dipole = chi_dipole
         self.drho_monopole, self.drho_dipole, self.basis_array, \
```

### Comparing `qeh-22.12.0/qeh.egg-info/PKG-INFO` & `qeh-23.6.0/qeh.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: qeh
-Version: 22.12.0
+Version: 23.6.0
 Summary: Quantum Electrostatic Heterostructure Model
 Home-page: https://gitlab.com/camd/qeh
 Author: CAMD
 Author-email: mogje@fysik.dtu.dk
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -24,9 +22,7 @@
 ===========================================
 The quantum electrostatic heterostructure (QEH) model is a
 fast and accurate model for simulating optical properties
 of stacks of 2D materials (heterostructures).
 
 - Documentation: https://qeh.readthedocs.io
 - Code: https://gitlab.com/camd/qeh.git
-
-
```

### Comparing `qeh-22.12.0/setup.py` & `qeh-23.6.0/setup.py`

 * *Files identical despite different names*

