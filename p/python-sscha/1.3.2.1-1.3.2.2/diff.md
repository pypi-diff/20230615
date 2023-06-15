# Comparing `tmp/python-sscha-1.3.2.1.tar.gz` & `tmp/python-sscha-1.3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sscha-1.3.2.1.tar", last modified: Thu Jun 15 15:30:49 2023, max compression
+gzip compressed data, was "python-sscha-1.3.2.2.tar", last modified: Thu Jun 15 15:33:04 2023, max compression
```

## Comparing `python-sscha-1.3.2.1.tar` & `python-sscha-1.3.2.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:30:49.129135 python-sscha-1.3.2.1/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    35149 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/LICENSE.txt
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:30:49.125135 python-sscha-1.3.2.1/Modules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10879 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/Modules/AdvancedCalculations.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4823 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/Modules/Calculator.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    66394 2023-05-16 12:51:43.000000 python-sscha-1.3.2.1/Modules/Cluster.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10288 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/Modules/Dynamical.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)   139352 2023-06-15 15:30:08.000000 python-sscha-1.3.2.1/Modules/Ensemble.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    15683 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/Modules/Minimizer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    15751 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/Modules/Optimizer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1173 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/Modules/Parallel.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    33103 2023-06-06 11:28:53.000000 python-sscha-1.3.2.1/Modules/Relax.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    82564 2023-06-06 11:28:53.000000 python-sscha-1.3.2.1/Modules/SchaMinimizer.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    18362 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/Modules/Tools.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    24140 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/Modules/Utilities.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       80 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/Modules/__init__.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      231 2023-06-15 15:30:49.129135 python-sscha-1.3.2.1/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8066 2023-05-16 12:51:43.000000 python-sscha-1.3.2.1/README.md
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:30:49.129135 python-sscha-1.3.2.1/SCHAModules/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      870 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/cell_force.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3354 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_cmat.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1442 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_emat.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1333 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_g.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    17136 2023-06-06 11:28:53.000000 python-sscha-1.3.2.1/SCHAModules/get_gradient_supercell.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    14175 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_gradient_supercell_fast.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     5029 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_odd_straight.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4215 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_odd_straight_with_v4.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)    10186 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_stress_tensor.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1997 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_upsilon_matrix.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4044 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_v3.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3540 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/get_v4.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     9696 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/module_anharmonic.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3172 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/module_new_thermodynamic.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8213 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/module_stochastic.f90
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4547 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/SCHAModules/multiply_lambda_tensor.f90
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:30:49.129135 python-sscha-1.3.2.1/python_sscha.egg-info/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)      231 2023-06-15 15:30:49.000000 python-sscha-1.3.2.1/python_sscha.egg-info/PKG-INFO
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     1126 2023-06-15 15:30:49.000000 python-sscha-1.3.2.1/python_sscha.egg-info/SOURCES.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-15 15:30:49.000000 python-sscha-1.3.2.1/python_sscha.egg-info/dependency_links.txt
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       18 2023-06-15 15:30:49.000000 python-sscha-1.3.2.1/python_sscha.egg-info/top_level.txt
-drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:30:49.129135 python-sscha-1.3.2.1/scripts/
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3585 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/scripts/cluster_check.x
--rwxrwxr-x   0 monacell  (1001) monacell  (1001)      842 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/scripts/plot_frequencies.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     3565 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/scripts/read_incomplete_ensemble.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4960 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/scripts/sscha
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     4715 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/scripts/sscha-plot-data.py
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     8052 2023-02-13 14:58:18.000000 python-sscha-1.3.2.1/scripts/static-vc-relax.pyx
--rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-15 15:30:49.129135 python-sscha-1.3.2.1/setup.cfg
--rw-rw-r--   0 monacell  (1001) monacell  (1001)     6940 2023-06-15 15:30:34.000000 python-sscha-1.3.2.1/setup.py
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:33:04.847284 python-sscha-1.3.2.2/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    35149 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/LICENSE.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:33:04.847284 python-sscha-1.3.2.2/Modules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10879 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/Modules/AdvancedCalculations.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4823 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/Modules/Calculator.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    66394 2023-05-16 12:51:43.000000 python-sscha-1.3.2.2/Modules/Cluster.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10288 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/Modules/Dynamical.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)   139352 2023-06-15 15:30:08.000000 python-sscha-1.3.2.2/Modules/Ensemble.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    15683 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/Modules/Minimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    15751 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/Modules/Optimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1173 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/Modules/Parallel.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    33103 2023-06-06 11:28:53.000000 python-sscha-1.3.2.2/Modules/Relax.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    82564 2023-06-06 11:28:53.000000 python-sscha-1.3.2.2/Modules/SchaMinimizer.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    18362 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/Modules/Tools.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    24140 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/Modules/Utilities.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       80 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/Modules/__init__.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      231 2023-06-15 15:33:04.847284 python-sscha-1.3.2.2/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8066 2023-05-16 12:51:43.000000 python-sscha-1.3.2.2/README.md
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:33:04.847284 python-sscha-1.3.2.2/SCHAModules/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      870 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/cell_force.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3354 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_cmat.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1442 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_emat.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1333 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_g.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    17136 2023-06-06 11:28:53.000000 python-sscha-1.3.2.2/SCHAModules/get_gradient_supercell.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    14175 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_gradient_supercell_fast.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     5029 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_odd_straight.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4215 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_odd_straight_with_v4.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)    10186 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_stress_tensor.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1997 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_upsilon_matrix.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4044 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_v3.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3540 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/get_v4.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     9696 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/module_anharmonic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3172 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/module_new_thermodynamic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8213 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/module_stochastic.f90
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4547 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/SCHAModules/multiply_lambda_tensor.f90
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:33:04.847284 python-sscha-1.3.2.2/python_sscha.egg-info/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)      231 2023-06-15 15:33:04.000000 python-sscha-1.3.2.2/python_sscha.egg-info/PKG-INFO
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     1126 2023-06-15 15:33:04.000000 python-sscha-1.3.2.2/python_sscha.egg-info/SOURCES.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)        1 2023-06-15 15:33:04.000000 python-sscha-1.3.2.2/python_sscha.egg-info/dependency_links.txt
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       18 2023-06-15 15:33:04.000000 python-sscha-1.3.2.2/python_sscha.egg-info/top_level.txt
+drwxrwxr-x   0 monacell  (1001) monacell  (1001)        0 2023-06-15 15:33:04.847284 python-sscha-1.3.2.2/scripts/
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3585 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/scripts/cluster_check.x
+-rwxrwxr-x   0 monacell  (1001) monacell  (1001)      842 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/scripts/plot_frequencies.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     3565 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/scripts/read_incomplete_ensemble.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4960 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/scripts/sscha
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     4715 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/scripts/sscha-plot-data.py
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     8052 2023-02-13 14:58:18.000000 python-sscha-1.3.2.2/scripts/static-vc-relax.pyx
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)       38 2023-06-15 15:33:04.847284 python-sscha-1.3.2.2/setup.cfg
+-rw-rw-r--   0 monacell  (1001) monacell  (1001)     6940 2023-06-15 15:33:00.000000 python-sscha-1.3.2.2/setup.py
```

### Comparing `python-sscha-1.3.2.1/LICENSE.txt` & `python-sscha-1.3.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/AdvancedCalculations.py` & `python-sscha-1.3.2.2/Modules/AdvancedCalculations.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Calculator.py` & `python-sscha-1.3.2.2/Modules/Calculator.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Cluster.py` & `python-sscha-1.3.2.2/Modules/Cluster.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Dynamical.py` & `python-sscha-1.3.2.2/Modules/Dynamical.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Ensemble.py` & `python-sscha-1.3.2.2/Modules/Ensemble.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Minimizer.py` & `python-sscha-1.3.2.2/Modules/Minimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Optimizer.py` & `python-sscha-1.3.2.2/Modules/Optimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Parallel.py` & `python-sscha-1.3.2.2/Modules/Parallel.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Relax.py` & `python-sscha-1.3.2.2/Modules/Relax.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/SchaMinimizer.py` & `python-sscha-1.3.2.2/Modules/SchaMinimizer.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Tools.py` & `python-sscha-1.3.2.2/Modules/Tools.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/Modules/Utilities.py` & `python-sscha-1.3.2.2/Modules/Utilities.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/README.md` & `python-sscha-1.3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/cell_force.f90` & `python-sscha-1.3.2.2/SCHAModules/cell_force.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_cmat.f90` & `python-sscha-1.3.2.2/SCHAModules/get_cmat.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_emat.f90` & `python-sscha-1.3.2.2/SCHAModules/get_emat.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_g.f90` & `python-sscha-1.3.2.2/SCHAModules/get_g.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_gradient_supercell.f90` & `python-sscha-1.3.2.2/SCHAModules/get_gradient_supercell.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_gradient_supercell_fast.f90` & `python-sscha-1.3.2.2/SCHAModules/get_gradient_supercell_fast.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_odd_straight.f90` & `python-sscha-1.3.2.2/SCHAModules/get_odd_straight.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_odd_straight_with_v4.f90` & `python-sscha-1.3.2.2/SCHAModules/get_odd_straight_with_v4.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_stress_tensor.f90` & `python-sscha-1.3.2.2/SCHAModules/get_stress_tensor.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_upsilon_matrix.f90` & `python-sscha-1.3.2.2/SCHAModules/get_upsilon_matrix.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_v3.f90` & `python-sscha-1.3.2.2/SCHAModules/get_v3.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/get_v4.f90` & `python-sscha-1.3.2.2/SCHAModules/get_v4.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/module_anharmonic.f90` & `python-sscha-1.3.2.2/SCHAModules/module_anharmonic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/module_new_thermodynamic.f90` & `python-sscha-1.3.2.2/SCHAModules/module_new_thermodynamic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/module_stochastic.f90` & `python-sscha-1.3.2.2/SCHAModules/module_stochastic.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/SCHAModules/multiply_lambda_tensor.f90` & `python-sscha-1.3.2.2/SCHAModules/multiply_lambda_tensor.f90`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/python_sscha.egg-info/SOURCES.txt` & `python-sscha-1.3.2.2/python_sscha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/scripts/cluster_check.x` & `python-sscha-1.3.2.2/scripts/cluster_check.x`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/scripts/plot_frequencies.py` & `python-sscha-1.3.2.2/scripts/plot_frequencies.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/scripts/read_incomplete_ensemble.py` & `python-sscha-1.3.2.2/scripts/read_incomplete_ensemble.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/scripts/sscha` & `python-sscha-1.3.2.2/scripts/sscha`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/scripts/sscha-plot-data.py` & `python-sscha-1.3.2.2/scripts/sscha-plot-data.py`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/scripts/static-vc-relax.pyx` & `python-sscha-1.3.2.2/scripts/static-vc-relax.pyx`

 * *Files identical despite different names*

### Comparing `python-sscha-1.3.2.1/setup.py` & `python-sscha-1.3.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 #                   extra_link_args = mpi_link_args + extra_link_args_c
 #                   )
 
 
 
 # Prepare the compilation of the Python Conde
 setup( name = "python-sscha",
-       version = "1.3.2.1",
+       version = "1.3.2.2",
        description = "Python implementation of the sscha code",
        author = "Lorenzo Monacelli",
        url = "https://github.com/mesonepigreco/python-sscha",
        packages = ["sscha"],
        package_dir = {"sscha": "Modules"},
        setup_requires = ["numpy", "ase", "scipy", "cellconstructor", "spglib", "matplotlib"],
        ext_modules = [SCHAModules], # odd_HP
```

