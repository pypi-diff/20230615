# Comparing `tmp/phonoLAMMPS-0.9.0.tar.gz` & `tmp/phonoLAMMPS-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonoLAMMPS-0.9.0.tar", last modified: Mon Sep 26 21:37:26 2022, max compression
+gzip compressed data, was "phonoLAMMPS-0.9.1.tar", last modified: Thu Jun 15 11:40:29 2023, max compression
```

## Comparing `phonoLAMMPS-0.9.0.tar` & `phonoLAMMPS-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 21:37:26.980355 phonoLAMMPS-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-09-26 21:37:26.980355 phonoLAMMPS-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3551 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 21:37:26.976355 phonoLAMMPS-0.9.0/phonoLAMMPS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-09-26 21:37:26.000000 phonoLAMMPS-0.9.0/phonoLAMMPS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-09-26 21:37:26.000000 phonoLAMMPS-0.9.0/phonoLAMMPS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 21:37:26.000000 phonoLAMMPS-0.9.0/phonoLAMMPS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-26 21:37:26.000000 phonoLAMMPS-0.9.0/phonoLAMMPS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-26 21:37:26.000000 phonoLAMMPS-0.9.0/phonoLAMMPS.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 21:37:26.976355 phonoLAMMPS-0.9.0/phonolammps/
--rw-r--r--   0 runner    (1001) docker     (121)    33007 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/phonolammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5425 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/phonolammps/arrange.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/phonolammps/capture.py
--rw-r--r--   0 runner    (1001) docker     (121)    16005 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/phonolammps/iofile.py
--rw-r--r--   0 runner    (1001) docker     (121)     6340 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/phonolammps/phonopy_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     3823 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/phonolammps/swissparam.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 21:37:26.976355 phonoLAMMPS-0.9.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)     7118 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/scripts/phonolammps
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-26 21:37:26.980355 phonoLAMMPS-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-09-26 21:37:17.000000 phonoLAMMPS-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:40:29.763106 phonoLAMMPS-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-15 11:40:29.763106 phonoLAMMPS-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:40:29.759106 phonoLAMMPS-0.9.1/phonoLAMMPS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-06-15 11:40:29.000000 phonoLAMMPS-0.9.1/phonoLAMMPS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 11:40:29.000000 phonoLAMMPS-0.9.1/phonoLAMMPS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:40:29.000000 phonoLAMMPS-0.9.1/phonoLAMMPS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 11:40:29.000000 phonoLAMMPS-0.9.1/phonoLAMMPS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 11:40:29.000000 phonoLAMMPS-0.9.1/phonoLAMMPS.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:40:29.759106 phonoLAMMPS-0.9.1/phonolammps/
+-rw-r--r--   0 runner    (1001) docker     (123)    33116 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/phonolammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/phonolammps/arrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/phonolammps/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16250 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/phonolammps/iofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/phonolammps/phonopy_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/phonolammps/swissparam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:40:29.763106 phonoLAMMPS-0.9.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7118 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/scripts/phonolammps
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:40:29.763106 phonoLAMMPS-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-15 11:40:20.000000 phonoLAMMPS-0.9.1/setup.py
```

### Comparing `phonoLAMMPS-0.9.0/LICENSE` & `phonoLAMMPS-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phonoLAMMPS-0.9.0/PKG-INFO` & `phonoLAMMPS-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonoLAMMPS
-Version: 0.9.0
+Version: 0.9.1
 Summary: phonoLAMMPS module
 Home-page: https://github.com/abelcarreras/phonolammps
 Author: Abel Carreras
 Author-email: abelcarreras83@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `phonoLAMMPS-0.9.0/README.md` & `phonoLAMMPS-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `phonoLAMMPS-0.9.0/phonoLAMMPS.egg-info/PKG-INFO` & `phonoLAMMPS-0.9.1/phonoLAMMPS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonoLAMMPS
-Version: 0.9.0
+Version: 0.9.1
 Summary: phonoLAMMPS module
 Home-page: https://github.com/abelcarreras/phonolammps
 Author: Abel Carreras
 Author-email: abelcarreras83@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `phonoLAMMPS-0.9.0/phonolammps/__init__.py` & `phonoLAMMPS-0.9.1/phonolammps/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 import numpy as np
 import warnings
 
 from phonopy.file_IO import write_FORCE_CONSTANTS, write_force_constants_to_hdf5, write_FORCE_SETS
 from phonolammps.arrange import get_correct_arrangement, rebuild_connectivity_tinker
 from phonolammps.phonopy_link import obtain_phonon_dispersion_bands, get_phonon
@@ -104,32 +104,34 @@
             self._data_set = data_set
 
         if include_data_set:
             return [self._force_constants, self._data_set]
         else:
             return self._force_constants
 
-    def plot_phonon_dispersion_bands(self):
+    def plot_phonon_dispersion_bands(self, bands_and_labels=None):
         """
         Plot phonon band structure using seekpath automatic k-path
         Warning: The labels may be wrong if the structure is not standarized
 
+        :param bands_and_labels: Custom energy band path
         """
         import matplotlib.pyplot as plt
 
         def replace_list(text_string):
             substitutions = {'GAMMA': u'$\Gamma$',
                              }
 
             for item in substitutions.items():
                 text_string = text_string.replace(item[0], item[1])
             return text_string
 
         force_constants = self.get_force_constants()
-        bands_and_labels = self.get_path_using_seek_path()
+        if bands_and_labels is None:
+            bands_and_labels = self.get_path_using_seek_path()
 
         _bands = obtain_phonon_dispersion_bands(self._structure,
                                                 bands_and_labels['ranges'],
                                                 force_constants,
                                                 self._supercell_matrix,
                                                 primitive_matrix=self._primitive_matrix,
                                                 band_resolution=30)
@@ -305,16 +307,16 @@
         """
         Get the units label for LAMMPS "units" command from a list of LAMMPS input commands
 
         :param commands_list: list of LAMMPS input commands (strings)
         :return units: string containing the units
         """
         for line in commands_list:
-                if line.startswith('units'):
-                    return line.split()[1]
+            if line.startswith('units'):
+                return line.split()[1]
         return 'lj'
 
     def get_forces(self, cell_with_disp):
         """
         Calculate the forces of a supercell using lammps
 
         :param cell_with_disp: supercell from which determine the forces
@@ -723,15 +725,15 @@
         return file
 
     def get_tpr(self, supercell_wd):
         import gmxapi as gmx
 
         #gmx genconf -f molecule.gro -o multi_mol.gro -nbox 2 2 2
 
-            # print(self._filename_dir + '.gro')
+        # print(self._filename_dir + '.gro')
 
         #create_gro(supercell_wd, self._structure, self._filename_dir + '.gro')
 
         generate_g96(supercell_wd, self._structure, self._filename_dir + '.g96')
 
 
         grompp = gmx.commandline_operation('gmx', 'grompp',
```

### Comparing `phonoLAMMPS-0.9.0/phonolammps/arrange.py` & `phonoLAMMPS-0.9.1/phonolammps/arrange.py`

 * *Files identical despite different names*

### Comparing `phonoLAMMPS-0.9.0/phonolammps/capture.py` & `phonoLAMMPS-0.9.1/phonolammps/capture.py`

 * *Files identical despite different names*

### Comparing `phonoLAMMPS-0.9.0/phonolammps/iofile.py` & `phonoLAMMPS-0.9.1/phonolammps/iofile.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,14 +138,22 @@
 
     masses = np.array([type_mass[type[i]] for i in range(na)], dtype=float)
     symbols = [mass_to_symbol(masses[i]) for i in range(na)]
 
     xp = lmp.extract_atom("x", 3)
     positions = np.array([[xp[i][0], xp[i][1], xp[i][2]] for i in range(na)], dtype=float)
 
+    # set order of ID's
+    id = lmp.extract_atom("id", 0)
+    id = np.array([id[i] - 1 for i in range(na)], dtype=int)
+
+    positions = positions[id.argsort()]
+    symbols = [symbols[i] for i in id.argsort()]
+    masses = masses[id.argsort()]
+
     return PhonopyAtoms(positions=positions,
                         masses=masses,
                         symbols=symbols,
                         cell=unitcell)
 
 def generate_VASP_structure(structure, scaled=True, supercell=(1, 1, 1)):
```

### Comparing `phonoLAMMPS-0.9.0/phonolammps/phonopy_link.py` & `phonoLAMMPS-0.9.1/phonolammps/phonopy_link.py`

 * *Files identical despite different names*

### Comparing `phonoLAMMPS-0.9.0/phonolammps/swissparam.py` & `phonoLAMMPS-0.9.1/phonolammps/swissparam.py`

 * *Files identical despite different names*

### Comparing `phonoLAMMPS-0.9.0/scripts/phonolammps` & `phonoLAMMPS-0.9.1/scripts/phonolammps`

 * *Files identical despite different names*

### Comparing `phonoLAMMPS-0.9.0/setup.py` & `phonoLAMMPS-0.9.1/setup.py`

 * *Files identical despite different names*

