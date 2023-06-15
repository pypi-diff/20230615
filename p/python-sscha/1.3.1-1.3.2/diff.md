# Comparing `tmp/python-sscha-1.3.1.tar.gz` & `tmp/python-sscha-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sscha-1.3.1.tar", last modified: Tue Jun  6 11:29:28 2023, max compression
+gzip compressed data, was "python-sscha-1.3.2.tar", last modified: Thu Jun 15 15:28:33 2023, max compression
```

## Comparing `python-sscha-1.3.1.tar` & `python-sscha-1.3.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.528195 python-sscha-1.3.1/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    35149 2023-02-13 14:58:18.000000 python-sscha-1.3.1/LICENSE.txt
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.520195 python-sscha-1.3.1/Modules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10879 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/AdvancedCalculations.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4823 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Calculator.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    66394 2023-05-16 12:51:43.000000 python-sscha-1.3.1/Modules/Cluster.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10288 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Dynamical.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)   139737 2023-06-06 11:28:53.000000 python-sscha-1.3.1/Modules/Ensemble.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    15683 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Minimizer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    15751 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Optimizer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1173 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Parallel.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    33103 2023-06-06 11:28:53.000000 python-sscha-1.3.1/Modules/Relax.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    82564 2023-06-06 11:28:53.000000 python-sscha-1.3.1/Modules/SchaMinimizer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    18362 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Tools.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    24140 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/Utilities.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       80 2023-02-13 14:58:18.000000 python-sscha-1.3.1/Modules/__init__.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      229 2023-06-06 11:29:28.528195 python-sscha-1.3.1/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8066 2023-05-16 12:51:43.000000 python-sscha-1.3.1/README.md
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.524195 python-sscha-1.3.1/SCHAModules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      870 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/cell_force.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3354 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_cmat.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1442 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_emat.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1333 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_g.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    17136 2023-06-06 11:28:53.000000 python-sscha-1.3.1/SCHAModules/get_gradient_supercell.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    14175 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_gradient_supercell_fast.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5029 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_odd_straight.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4215 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_odd_straight_with_v4.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10186 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_stress_tensor.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1997 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_upsilon_matrix.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4044 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_v3.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3540 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/get_v4.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     9696 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/module_anharmonic.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3172 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/module_new_thermodynamic.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8213 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/module_stochastic.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4547 2023-02-13 14:58:18.000000 python-sscha-1.3.1/SCHAModules/multiply_lambda_tensor.f90
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.528195 python-sscha-1.3.1/python_sscha.egg-info/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      229 2023-06-06 11:29:28.000000 python-sscha-1.3.1/python_sscha.egg-info/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1126 2023-06-06 11:29:28.000000 python-sscha-1.3.1/python_sscha.egg-info/SOURCES.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-06 11:29:28.000000 python-sscha-1.3.1/python_sscha.egg-info/dependency_links.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       18 2023-06-06 11:29:28.000000 python-sscha-1.3.1/python_sscha.egg-info/top_level.txt
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-06 11:29:28.528195 python-sscha-1.3.1/scripts/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3585 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/cluster_check.x
--rwxrwxr-x   0 monacell  (1001) monacell  (1001)      842 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/plot_frequencies.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3565 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/read_incomplete_ensemble.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4960 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/sscha
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4715 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/sscha-plot-data.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8052 2023-02-13 14:58:18.000000 python-sscha-1.3.1/scripts/static-vc-relax.pyx
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-06 11:29:28.528195 python-sscha-1.3.1/setup.cfg
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     6938 2023-06-06 11:29:12.000000 python-sscha-1.3.1/setup.py
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:28:33.162982 python-sscha-1.3.2/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    35149 2023-02-13 14:58:18.000000 python-sscha-1.3.2/LICENSE.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:28:33.118981 python-sscha-1.3.2/Modules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10879 2023-02-13 14:58:18.000000 python-sscha-1.3.2/Modules/AdvancedCalculations.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4823 2023-02-13 14:58:18.000000 python-sscha-1.3.2/Modules/Calculator.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    66394 2023-05-16 12:51:43.000000 python-sscha-1.3.2/Modules/Cluster.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10288 2023-02-13 14:58:18.000000 python-sscha-1.3.2/Modules/Dynamical.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   139350 2023-06-13 10:52:30.000000 python-sscha-1.3.2/Modules/Ensemble.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    15683 2023-02-13 14:58:18.000000 python-sscha-1.3.2/Modules/Minimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    15751 2023-02-13 14:58:18.000000 python-sscha-1.3.2/Modules/Optimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1173 2023-02-13 14:58:18.000000 python-sscha-1.3.2/Modules/Parallel.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    33103 2023-06-06 11:28:53.000000 python-sscha-1.3.2/Modules/Relax.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    82564 2023-06-06 11:28:53.000000 python-sscha-1.3.2/Modules/SchaMinimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    18362 2023-02-13 14:58:18.000000 python-sscha-1.3.2/Modules/Tools.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    24140 2023-02-13 14:58:18.000000 python-sscha-1.3.2/Modules/Utilities.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       80 2023-02-13 14:58:18.000000 python-sscha-1.3.2/Modules/__init__.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      229 2023-06-15 15:28:33.162982 python-sscha-1.3.2/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8066 2023-05-16 12:51:43.000000 python-sscha-1.3.2/README.md
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:28:33.150982 python-sscha-1.3.2/SCHAModules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      870 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/cell_force.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3354 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_cmat.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1442 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_emat.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1333 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_g.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    17136 2023-06-06 11:28:53.000000 python-sscha-1.3.2/SCHAModules/get_gradient_supercell.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    14175 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_gradient_supercell_fast.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5029 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_odd_straight.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4215 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_odd_straight_with_v4.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10186 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_stress_tensor.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1997 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_upsilon_matrix.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4044 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_v3.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3540 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/get_v4.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     9696 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/module_anharmonic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3172 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/module_new_thermodynamic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8213 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/module_stochastic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4547 2023-02-13 14:58:18.000000 python-sscha-1.3.2/SCHAModules/multiply_lambda_tensor.f90
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:28:33.150982 python-sscha-1.3.2/python_sscha.egg-info/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      229 2023-06-15 15:28:33.000000 python-sscha-1.3.2/python_sscha.egg-info/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1126 2023-06-15 15:28:33.000000 python-sscha-1.3.2/python_sscha.egg-info/SOURCES.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-15 15:28:33.000000 python-sscha-1.3.2/python_sscha.egg-info/dependency_links.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       18 2023-06-15 15:28:33.000000 python-sscha-1.3.2/python_sscha.egg-info/top_level.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:28:33.162982 python-sscha-1.3.2/scripts/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3585 2023-02-13 14:58:18.000000 python-sscha-1.3.2/scripts/cluster_check.x
+-rwxrwxr-x   0 monacell  (1001) monacell  (1001)      842 2023-02-13 14:58:18.000000 python-sscha-1.3.2/scripts/plot_frequencies.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3565 2023-02-13 14:58:18.000000 python-sscha-1.3.2/scripts/read_incomplete_ensemble.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4960 2023-02-13 14:58:18.000000 python-sscha-1.3.2/scripts/sscha
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4715 2023-02-13 14:58:18.000000 python-sscha-1.3.2/scripts/sscha-plot-data.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8052 2023-02-13 14:58:18.000000 python-sscha-1.3.2/scripts/static-vc-relax.pyx
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-15 15:28:33.162982 python-sscha-1.3.2/setup.cfg
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     6938 2023-06-15 15:28:25.000000 python-sscha-1.3.2/setup.py
```

### Comparing `python-sscha-1.3.1/LICENSE.txt` & `python-sscha-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/AdvancedCalculations.py` & `python-sscha-1.3.2/Modules/AdvancedCalculations.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/Calculator.py` & `python-sscha-1.3.2/Modules/Calculator.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/Cluster.py` & `python-sscha-1.3.2/Modules/Cluster.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/Dynamical.py` & `python-sscha-1.3.2/Modules/Dynamical.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/Ensemble.py` & `python-sscha-1.3.2/Modules/Ensemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -818,28 +818,28 @@
 
         
         ase_structs = []
 
         for i, s in enumerate(self.structures):
             energy = self.energies[i] * Rydberg  # Ry -> eV
             forces = self.forces[i, :, :] * Rydberg  # Ry/A -> eV/A
-            stress = self.stresses[i, :, :] * Rydberg /  Bohr**3 # Ry/Bohr^3 -> eV/A^3
+            stress = -self.stresses[i, :, :] * Rydberg /  Bohr**3 # Ry/Bohr^3 -> eV/A^3 (with ase conventions on sign)
             struct = s.get_ase_atoms()
 
             calculator = ase.calculators.singlepoint.SinglePointCalculator(struct, energy = energy,
                 forces = forces, stress = CC.Methods.transform_voigt(stress))
             
             struct.set_calculator(calculator)
             ase_structs.append(struct)
 
         # Now save the extended xyz
         ase.io.write(filename, ase_structs, format = "extxyz", append = append_mode)
 
 
-    def save_enhanced_xyz(self, filename, append_mode = True, stress_key = "virial", forces_key = "force", energy_key = "energy"):
+    def save_enhanced_xyz(self, filename, append_mode = True, stress_key = "stress", forces_key = "forces", energy_key = "energy"):
         """
         Save the ensemble as an enhanced xyz.
 
         This is the default format for training the GAP potentials with quippy.
 
         Parameters
         ----------
@@ -862,15 +862,16 @@
                 info = 'pbc="T T T" ' # Periodic boundary conditions
                 info += 'Lattice="{:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f}" '.format(*list(struct.unit_cell.ravel()))
 
                 # Add the energy
                 info += '{}={:.16f} '.format(energy_key, self.energies[i] * Rydberg)
 
                 # Add the virial stress
-                info += '{}="{:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f}" '.format(stress_key, *list(self.stresses[i].ravel()))
+                stress_data = - self.stresses[i].ravel * CC.Units.RY_PER_BOHR3_TO_EV_PER_A3
+                info += '{}="{:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f} {:20.16f}" '.format(stress_key, *list(stress_data))
 
                 # Add the secription of the xyz format
                 info += 'Properties=species:S:1:pos:R:3:{}:R:3\n'.format(forces_key)
 
                 lines.append(info)
 
                 # Append the structure and the forces
@@ -1372,15 +1373,14 @@
                 Since it is the most time consuming part, it can be safely avoided.
         """
 
         self.current_T = newT
 
         # Check if the dynamical matrix has changed
         changed_dyn = np.max([np.max(np.abs(self.current_dyn.dynmats[i] - new_dynamical_matrix.dynmats[i])) for i in range(len(self.current_dyn.q_tot))])
-        print("DYN CHANGED BY:", changed_dyn)
         changed_dyn = changed_dyn > 1e-30
 
         # Prepare the new displacements
         super_struct0 = self.dyn_0.structure.generate_supercell(self.supercell)
         super_structure = new_dynamical_matrix.structure.generate_supercell(self.supercell)
         old_disps = np.zeros(np.shape(self.u_disps), dtype = np.double)
         Nat_sc = super_structure.N_atoms
@@ -1898,22 +1898,19 @@
 
     def get_preconditioned_gradient_parallel(self, *args, timer=None, **kwargs):
         """
         Compute the gradient using multiprocessing.
         For documentation, see get_preconditioned_gradient
         """
 
-        print("force length:", len(self.force_computed))
 
         def work_function(argument, timer=None):
-            print("force length [inside]:", len(self.force_computed))
             ensemble_start_config, ensemble_end_config = argument
             mask = np.zeros(self.N, dtype = bool)
             mask[ensemble_start_config : ensemble_end_config] = True
-            print("mask length:", np.sum(mask.astype(int))," total N:", len(mask))
             new_ensemble = self.split(mask)
 
             gradient, _ = new_ensemble.get_preconditioned_gradient(*args, timer=timer, **kwargs)
 
             av_ensemble = np.sum(new_ensemble.rho)
             
             return gradient * av_ensemble
@@ -3225,18 +3222,15 @@
         """
 
         structs = [self.structures[x] for x in np.arange(len(split_mask))[split_mask]]
 
         N = np.sum(split_mask.astype(int))
         ens = Ensemble(self.dyn_0, self.T0, self.dyn_0.GetSupercell())
         ens.init_from_structures(structs)
-        print("Split length:", len(split_mask))
-        print("original force legnth:", len(self.force_computed))
-        print("Expected length:", len(ens.force_computed))
-        print("Splitting force length:", len(self.force_computed[split_mask]))
+        
 
         ens.force_computed[:] = self.force_computed[split_mask]
         ens.stress_computed[:] = self.stress_computed[split_mask]
         ens.energies[:] = self.energies[split_mask]
         ens.forces[:, :, :] = self.forces[split_mask, :, :]
         ens.has_stress = self.has_stress
         ens.ignore_small_w = self.ignore_small_w
```

### Comparing `python-sscha-1.3.1/Modules/Minimizer.py` & `python-sscha-1.3.2/Modules/Minimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/Optimizer.py` & `python-sscha-1.3.2/Modules/Optimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/Parallel.py` & `python-sscha-1.3.2/Modules/Parallel.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/Relax.py` & `python-sscha-1.3.2/Modules/Relax.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/SchaMinimizer.py` & `python-sscha-1.3.2/Modules/SchaMinimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/Tools.py` & `python-sscha-1.3.2/Modules/Tools.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/Modules/Utilities.py` & `python-sscha-1.3.2/Modules/Utilities.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/README.md` & `python-sscha-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/cell_force.f90` & `python-sscha-1.3.2/SCHAModules/cell_force.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_cmat.f90` & `python-sscha-1.3.2/SCHAModules/get_cmat.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_emat.f90` & `python-sscha-1.3.2/SCHAModules/get_emat.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_g.f90` & `python-sscha-1.3.2/SCHAModules/get_g.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_gradient_supercell.f90` & `python-sscha-1.3.2/SCHAModules/get_gradient_supercell.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_gradient_supercell_fast.f90` & `python-sscha-1.3.2/SCHAModules/get_gradient_supercell_fast.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_odd_straight.f90` & `python-sscha-1.3.2/SCHAModules/get_odd_straight.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_odd_straight_with_v4.f90` & `python-sscha-1.3.2/SCHAModules/get_odd_straight_with_v4.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_stress_tensor.f90` & `python-sscha-1.3.2/SCHAModules/get_stress_tensor.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_upsilon_matrix.f90` & `python-sscha-1.3.2/SCHAModules/get_upsilon_matrix.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_v3.f90` & `python-sscha-1.3.2/SCHAModules/get_v3.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/get_v4.f90` & `python-sscha-1.3.2/SCHAModules/get_v4.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/module_anharmonic.f90` & `python-sscha-1.3.2/SCHAModules/module_anharmonic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/module_new_thermodynamic.f90` & `python-sscha-1.3.2/SCHAModules/module_new_thermodynamic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/module_stochastic.f90` & `python-sscha-1.3.2/SCHAModules/module_stochastic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/SCHAModules/multiply_lambda_tensor.f90` & `python-sscha-1.3.2/SCHAModules/multiply_lambda_tensor.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/python_sscha.egg-info/SOURCES.txt` & `python-sscha-1.3.2/python_sscha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/scripts/cluster_check.x` & `python-sscha-1.3.2/scripts/cluster_check.x`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/scripts/plot_frequencies.py` & `python-sscha-1.3.2/scripts/plot_frequencies.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/scripts/read_incomplete_ensemble.py` & `python-sscha-1.3.2/scripts/read_incomplete_ensemble.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/scripts/sscha` & `python-sscha-1.3.2/scripts/sscha`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/scripts/sscha-plot-data.py` & `python-sscha-1.3.2/scripts/sscha-plot-data.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/scripts/static-vc-relax.pyx` & `python-sscha-1.3.2/scripts/static-vc-relax.pyx`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.1/setup.py` & `python-sscha-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 #                   extra_link_args = mpi_link_args + extra_link_args_c
 #                   )
 
 
 
 # Prepare the compilation of the Python Conde
 setup( name = "python-sscha",
-       version = "1.3.1",
+       version = "1.3.2",
        description = "Python implementation of the sscha code",
        author = "Lorenzo Monacelli",
        url = "https://github.com/mesonepigreco/python-sscha",
        packages = ["sscha"],
        package_dir = {"sscha": "Modules"},
        setup_requires = ["numpy", "ase", "scipy", "cellconstructor", "spglib", "matplotlib"],
        ext_modules = [SCHAModules], # odd_HP
```

