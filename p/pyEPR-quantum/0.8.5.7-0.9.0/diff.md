# Comparing `tmp/pyEPR-quantum-0.8.5.7.tar.gz` & `tmp/pyEPR-quantum-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyEPR/pyEPR/dist/tmpdjkf_xyn/pyEPR-quantum-0.8.5.7.tar", last modified: Fri Jul 22 20:57:52 2022, max compression
+gzip compressed data, was "/home/runner/work/pyEPR/pyEPR/dist/.tmp-wfmpkfqv/pyEPR-quantum-0.9.0.tar", last modified: Wed Jun 14 22:04:34 2023, max compression
```

## Comparing `pyEPR-quantum-0.8.5.7.tar` & `pyEPR-quantum-0.9.0.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    21535 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    20483 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/pyEPR/
--rw-r--r--   0 runner    (1001) docker     (121)     2592 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/__config_user_old.py
--rw-r--r--   0 runner    (1001) docker     (121)     8137 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6018 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/_config_default.py
--rw-r--r--   0 runner    (1001) docker     (121)     2965 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/_config_user.py
--rw-r--r--   0 runner    (1001) docker     (121)   116941 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/ansys.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/pyEPR/calcs/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/calcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13185 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/calcs/back_box_numeric.py
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/calcs/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)      462 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/calcs/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     7278 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/calcs/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/calcs/hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/calcs/quantum.py
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/calcs/transmon.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    61972 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/core_distributed_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    45049 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/core_quantum_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    18760 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/project_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/pyEPR/toolbox/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/toolbox/_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4711 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/toolbox/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    11159 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/pyEPR/toolbox/pythonic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/pyEPR_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    21535 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/pyEPR_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/pyEPR_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/pyEPR_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/pyEPR_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/pyEPR_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-22 20:57:52.000000 pyEPR-quantum-0.8.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2602 2022-07-22 20:57:40.000000 pyEPR-quantum-0.8.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20483 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/pyEPR/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/__config_user_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/_config_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/_config_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117738 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/ansys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/pyEPR/calcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/calcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/calcs/back_box_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/calcs/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/calcs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/calcs/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/calcs/hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/calcs/quantum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/calcs/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62140 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/core_distributed_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44974 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/core_quantum_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18897 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/project_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/pyEPR/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/toolbox/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/toolbox/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/pyEPR/toolbox/pythonic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/pyEPR_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/pyEPR_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/pyEPR_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/pyEPR_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/pyEPR_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/pyEPR_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 22:04:34.000000 pyEPR-quantum-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/tests/test_project_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-14 22:04:22.000000 pyEPR-quantum-0.9.0/tests/test_quantum_analysis.py
```

### Comparing `pyEPR-quantum-0.8.5.7/LICENSE` & `pyEPR-quantum-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/PKG-INFO` & `pyEPR-quantum-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEPR-quantum
-Version: 0.8.5.7
+Version: 0.9.0
 Home-page: https://github.com/zlatko-minev/pyEPR
 Author: Zlatko K. Minev
 Author-email: zlatko.minev@aya.yale.edu
 Maintainer: Zlatko Minev, pyEPR team
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyEPR-quantum-0.8.5.7/README.md` & `pyEPR-quantum-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/__config_user_old.py` & `pyEPR-quantum-0.9.0/pyEPR/__config_user_old.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/__init__.py` & `pyEPR-quantum-0.9.0/pyEPR/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 Here, in this package, all routines of the EPR approach are fully automated.
 An interface with ansys is provided.
 Automated analysis of lumped and distributed circuits is provided.
 
 @author: Zlatko Minev, Zaki Leghas, ... and the pyEPR team
 @site: https://github.com/zlatko-minev/pyEPR
 @license: "BSD-3-Clause"
-@version: 0.8.5.7
+@version: 0.9.0
 @maintainer: Zlatko K. Minev and  Asaf Diringer
 @email: zlatko.minev@aya.yale.edu
 @url: https://github.com/zlatko-minev/pyEPR
 @status: "Dev-Production"
 """
 # pylint: disable= wrong-import-position, invalid-name
 
@@ -82,15 +82,15 @@
 __author__ = "Zlatko Minev, Zaki Leghas, and the pyEPR team"
 __copyright__ = "Copyright 2015-2020, pyEPR team"
 __credits__ = [
     "Zlatko Minev", "Zaki Leghtas,", "Phil Rheinhold", "Asaf Diringer",
     "Will Livingston", "Steven Touzard"
 ]
 __license__ = "BSD-3-Clause"
-__version__ = "0.8.5.7"
+__version__ = "0.9.0"
 __maintainer__ = "Zlatko K. Minev and  Asaf Diringer"
 __email__ = "zlatko.minev@aya.yale.edu"
 __url__ = r'https://github.com/zlatko-minev/pyEPR'
 __status__ = "Dev-Production"
 
 ##############################################################################
 # Config setup
```

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/_config_default.py` & `pyEPR-quantum-0.9.0/pyEPR/_config_default.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/_config_user.py` & `pyEPR-quantum-0.9.0/pyEPR/_config_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,30 @@
         eps_r=10,
 
         # Surface dielectric (dirt) loss tangent
         # units: unitless, since this is tan(delta)
         tan_delta_surf=1e-3,
 
         ##################################################
+        # Surface object specific dielectric properties.
+        # These will override ones above when applicable
+        dielectric_surfaces=Dict(
+            trace=Dict(
+                tan_delta_surf=0.001,
+                th=5e-9,
+                eps_r=10
+            ),
+            gap=Dict(
+                tan_delta_surf=0.001,
+                th=2e-9,
+                eps_r=10
+            )
+        ),
+
+        ##################################################
         # Thin-film surface loss
         # units:  Ohms
         # ref:    https://arxiv.org/abs/1308.1743
         surface_Rs=250e-9,
 
         ##################################################
         # Seam current loss
```

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/ansys.py` & `pyEPR-quantum-0.9.0/pyEPR/ansys.py`

 * *Files 2% similar despite different names*

```diff
@@ -3743,3567 +3743,3617 @@
 0000e9e0: 6173 735f 6e61 6d65 3d27 4c61 7374 4164  ass_name='LastAd
 0000e9f0: 6170 7469 7665 2729 3a0a 2020 2020 2020  aptive'):.      
 0000ea00: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
 0000ea10: 7373 5f6e 616d 653a 2041 6461 7074 6976  ss_name: Adaptiv
 0000ea20: 6550 6173 732c 204c 6173 7441 6461 7074  ePass, LastAdapt
 0000ea30: 6976 650a 0a20 2020 2020 2020 2045 7861  ive..        Exa
 0000ea40: 6d70 6c65 0a20 2020 2020 2020 202d 2d2d  mple.        ---
-0000ea50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ea60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ea70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ea80: 2d2d 2d0a 2020 2020 2020 2020 4578 616d  ---.        Exam
-0000ea90: 706c 6520 706c 6f74 2066 6f72 2061 2073  ple plot for a s
-0000eaa0: 696e 676c 6520 7661 7269 6174 696f 6e20  ingle variation 
-0000eab0: 616c 6c20 7061 7373 2063 6f6e 7665 7267  all pass converg
-0000eac0: 6520 6f66 206d 6f64 6520 6672 6571 0a20  e of mode freq. 
-0000ead0: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
-0000eae0: 6c6f 636b 2070 7974 686f 6e0a 2020 2020  lock python.    
-0000eaf0: 2020 2020 2020 2020 7963 6f6d 7020 3d20          ycomp = 
-0000eb00: 5b66 2272 6528 4d6f 6465 287b 697d 2929  [f"re(Mode({i}))
-0000eb10: 2220 666f 7220 6920 696e 2072 616e 6765  " for i in range
-0000eb20: 2831 2c31 2b65 7072 5f68 6673 732e 6e5f  (1,1+epr_hfss.n_
-0000eb30: 6d6f 6465 7329 5d0a 2020 2020 2020 2020  modes)].        
-0000eb40: 2020 2020 7061 7261 6d73 203d 205b 2250      params = ["P
-0000eb50: 6173 733a 3d22 2c20 5b22 416c 6c22 5d5d  ass:=", ["All"]]
-0000eb60: 2b76 6172 6961 7469 6f6e 0a20 2020 2020  +variation.     
-0000eb70: 2020 2020 2020 2073 6574 7570 2e63 7265         setup.cre
-0000eb80: 6174 655f 7265 706f 7274 2822 4672 6571  ate_report("Freq
-0000eb90: 2e20 7673 2e20 7061 7373 222c 2022 5061  . vs. pass", "Pa
-0000eba0: 7373 222c 2079 636f 6d70 2c20 7061 7261  ss", ycomp, para
-0000ebb0: 6d73 2c20 7061 7373 5f6e 616d 653d 2741  ms, pass_name='A
-0000ebc0: 6461 7074 6976 6550 6173 7327 290a 2020  daptivePass').  
-0000ebd0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-0000ebe0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-0000ebf0: 6e63 6528 7963 6f6d 702c 206c 6973 7429  nce(ycomp, list)
-0000ec00: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000ec10: 6973 696e 7374 616e 6365 2870 6172 616d  isinstance(param
-0000ec20: 732c 206c 6973 7429 0a0a 2020 2020 2020  s, list)..      
-0000ec30: 2020 7365 7475 7020 3d20 7365 6c66 2e70    setup = self.p
-0000ec40: 6172 656e 740a 2020 2020 2020 2020 7265  arent.        re
-0000ec50: 706f 7274 6572 203d 2073 6574 7570 2e5f  porter = setup._
-0000ec60: 7265 706f 7274 6572 0a20 2020 2020 2020  reporter.       
-0000ec70: 2072 6574 7572 6e20 7265 706f 7274 6572   return reporter
-0000ec80: 2e43 7265 6174 6552 6570 6f72 7428 0a20  .CreateReport(. 
-0000ec90: 2020 2020 2020 2020 2020 2070 6c6f 745f             plot_
-0000eca0: 6e61 6d65 2c20 2245 6967 656e 6d6f 6465  name, "Eigenmode
-0000ecb0: 2050 6172 616d 6574 6572 7322 2c20 2252   Parameters", "R
-0000ecc0: 6563 7461 6e67 756c 6172 2050 6c6f 7422  ectangular Plot"
-0000ecd0: 2c0a 2020 2020 2020 2020 2020 2020 6622  ,.            f"
-0000ece0: 7b73 6574 7570 2e6e 616d 657d 203a 207b  {setup.name} : {
-0000ecf0: 7061 7373 5f6e 616d 657d 222c 205b 5d2c  pass_name}", [],
-0000ed00: 2070 6172 616d 732c 0a20 2020 2020 2020   params,.       
-0000ed10: 2020 2020 205b 2258 2043 6f6d 706f 6e65       ["X Compone
-0000ed20: 6e74 3a3d 222c 2078 636f 6d70 2c20 2259  nt:=", xcomp, "Y
-0000ed30: 2043 6f6d 706f 6e65 6e74 3a3d 222c 2079   Component:=", y
-0000ed40: 636f 6d70 5d2c 205b 5d29 0a0a 0a63 6c61  comp], [])...cla
-0000ed50: 7373 2048 6673 7344 4d44 6573 6967 6e53  ss HfssDMDesignS
-0000ed60: 6f6c 7574 696f 6e73 2848 6673 7344 6573  olutions(HfssDes
-0000ed70: 6967 6e53 6f6c 7574 696f 6e73 293a 0a20  ignSolutions):. 
-0000ed80: 2020 2070 6173 730a 0a63 6c61 7373 2048     pass..class H
-0000ed90: 6673 7344 5444 6573 6967 6e53 6f6c 7574  fssDTDesignSolut
-0000eda0: 696f 6e73 2848 6673 7344 6573 6967 6e53  ions(HfssDesignS
-0000edb0: 6f6c 7574 696f 6e73 293a 0a20 2020 2070  olutions):.    p
-0000edc0: 6173 730a 0a63 6c61 7373 2048 6673 7351  ass..class HfssQ
-0000edd0: 3344 4465 7369 676e 536f 6c75 7469 6f6e  3DDesignSolution
-0000ede0: 7328 4866 7373 4465 7369 676e 536f 6c75  s(HfssDesignSolu
-0000edf0: 7469 6f6e 7329 3a0a 2020 2020 7061 7373  tions):.    pass
-0000ee00: 0a0a 0a63 6c61 7373 2048 6673 7346 7265  ...class HfssFre
-0000ee10: 7175 656e 6379 5377 6565 7028 434f 4d57  quencySweep(COMW
-0000ee20: 7261 7070 6572 293a 0a20 2020 2070 726f  rapper):.    pro
-0000ee30: 705f 7461 6220 3d20 2248 6673 7354 6162  p_tab = "HfssTab
-0000ee40: 220a 2020 2020 7374 6172 745f 6672 6571  ".    start_freq
-0000ee50: 203d 206d 616b 655f 666c 6f61 745f 7072   = make_float_pr
-0000ee60: 6f70 2822 5374 6172 7422 290a 2020 2020  op("Start").    
-0000ee70: 7374 6f70 5f66 7265 7120 3d20 6d61 6b65  stop_freq = make
-0000ee80: 5f66 6c6f 6174 5f70 726f 7028 2253 746f  _float_prop("Sto
-0000ee90: 7022 290a 2020 2020 7374 6570 5f73 697a  p").    step_siz
-0000eea0: 6520 3d20 6d61 6b65 5f66 6c6f 6174 5f70  e = make_float_p
-0000eeb0: 726f 7028 2253 7465 7020 5369 7a65 2229  rop("Step Size")
-0000eec0: 0a20 2020 2063 6f75 6e74 203d 206d 616b  .    count = mak
-0000eed0: 655f 666c 6f61 745f 7072 6f70 2822 436f  e_float_prop("Co
-0000eee0: 756e 7422 290a 2020 2020 7377 6565 705f  unt").    sweep_
-0000eef0: 7479 7065 203d 206d 616b 655f 7374 725f  type = make_str_
-0000ef00: 7072 6f70 2822 5479 7065 2229 0a0a 2020  prop("Type")..  
-0000ef10: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0000ef20: 656c 662c 2073 6574 7570 2c20 6e61 6d65  elf, setup, name
-0000ef30: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000ef40: 2020 2020 2020 203a 7479 7065 2073 6574         :type set
-0000ef50: 7570 3a20 4866 7373 5365 7475 700a 2020  up: HfssSetup.  
-0000ef60: 2020 2020 2020 3a74 7970 6520 6e61 6d65        :type name
-0000ef70: 3a20 7374 720a 2020 2020 2020 2020 2222  : str.        ""
-0000ef80: 220a 2020 2020 2020 2020 7375 7065 7228  ".        super(
-0000ef90: 4866 7373 4672 6571 7565 6e63 7953 7765  HfssFrequencySwe
-0000efa0: 6570 2c20 7365 6c66 292e 5f5f 696e 6974  ep, self).__init
-0000efb0: 5f5f 2829 0a20 2020 2020 2020 2073 656c  __().        sel
-0000efc0: 662e 7061 7265 6e74 203d 2073 6574 7570  f.parent = setup
-0000efd0: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
-0000efe0: 6d65 203d 206e 616d 650a 2020 2020 2020  me = name.      
-0000eff0: 2020 7365 6c66 2e73 6f6c 7574 696f 6e5f    self.solution_
-0000f000: 6e61 6d65 203d 2073 656c 662e 7061 7265  name = self.pare
-0000f010: 6e74 2e6e 616d 6520 2b20 2220 3a20 2220  nt.name + " : " 
-0000f020: 2b20 6e61 6d65 0a20 2020 2020 2020 2073  + name.        s
-0000f030: 656c 662e 7072 6f70 5f68 6f6c 6465 7220  elf.prop_holder 
-0000f040: 3d20 7365 6c66 2e70 6172 656e 742e 7072  = self.parent.pr
-0000f050: 6f70 5f68 6f6c 6465 720a 2020 2020 2020  op_holder.      
-0000f060: 2020 7365 6c66 2e70 726f 705f 7365 7276    self.prop_serv
-0000f070: 6572 203d 2073 656c 662e 7061 7265 6e74  er = self.parent
-0000f080: 2e70 726f 705f 7365 7276 6572 202b 2022  .prop_server + "
-0000f090: 3a22 202b 206e 616d 650a 2020 2020 2020  :" + name.      
-0000f0a0: 2020 7365 6c66 2e5f 616e 7379 735f 7665    self._ansys_ve
-0000f0b0: 7273 696f 6e20 3d20 7365 6c66 2e70 6172  rsion = self.par
-0000f0c0: 656e 742e 5f61 6e73 7973 5f76 6572 7369  ent._ansys_versi
-0000f0d0: 6f6e 0a0a 2020 2020 6465 6620 616e 616c  on..    def anal
-0000f0e0: 797a 655f 7377 6565 7028 7365 6c66 293a  yze_sweep(self):
-0000f0f0: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
-0000f100: 7265 6e74 2e61 6e61 6c79 7a65 2873 656c  rent.analyze(sel
-0000f110: 662e 736f 6c75 7469 6f6e 5f6e 616d 6529  f.solution_name)
-0000f120: 0a0a 2020 2020 6465 6620 6765 745f 6e65  ..    def get_ne
-0000f130: 7477 6f72 6b5f 6461 7461 2873 656c 662c  twork_data(self,
-0000f140: 2066 6f72 6d61 7473 293a 0a20 2020 2020   formats):.     
-0000f150: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000f160: 2866 6f72 6d61 7473 2c20 7374 7229 3a0a  (formats, str):.
-0000f170: 2020 2020 2020 2020 2020 2020 666f 726d              form
-0000f180: 6174 7320 3d20 666f 726d 6174 732e 7370  ats = formats.sp
-0000f190: 6c69 7428 222c 2229 0a20 2020 2020 2020  lit(",").       
-0000f1a0: 2066 6f72 6d61 7473 203d 205b 662e 7570   formats = [f.up
-0000f1b0: 7065 7228 2920 666f 7220 6620 696e 2066  per() for f in f
-0000f1c0: 6f72 6d61 7473 5d0a 0a20 2020 2020 2020  ormats]..       
-0000f1d0: 2066 6d74 735f 6c69 7374 7320 3d20 7b27   fmts_lists = {'
-0000f1e0: 5327 3a20 5b5d 2c20 2759 273a 205b 5d2c  S': [], 'Y': [],
-0000f1f0: 2027 5a27 3a20 5b5d 7d0a 0a20 2020 2020   'Z': []}..     
-0000f200: 2020 2066 6f72 2066 2069 6e20 666f 726d     for f in form
-0000f210: 6174 733a 0a20 2020 2020 2020 2020 2020  ats:.           
-0000f220: 2066 6d74 735f 6c69 7374 735b 665b 305d   fmts_lists[f[0]
-0000f230: 5d2e 6170 7065 6e64 2828 696e 7428 665b  ].append((int(f[
-0000f240: 315d 292c 2069 6e74 2866 5b32 5d29 2929  1]), int(f[2])))
-0000f250: 0a20 2020 2020 2020 2072 6574 203d 205b  .        ret = [
-0000f260: 4e6f 6e65 5d20 2a20 6c65 6e28 666f 726d  None] * len(form
-0000f270: 6174 7329 0a20 2020 2020 2020 2066 7265  ats).        fre
-0000f280: 7120 3d20 4e6f 6e65 0a0a 2020 2020 2020  q = None..      
-0000f290: 2020 666f 7220 6461 7461 5f74 7970 652c    for data_type,
-0000f2a0: 206c 6973 7420 696e 2066 6d74 735f 6c69   list in fmts_li
-0000f2b0: 7374 732e 6974 656d 7328 293a 0a20 2020  sts.items():.   
-0000f2c0: 2020 2020 2020 2020 2069 6620 6c69 7374           if list
-0000f2d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f2e0: 2020 666e 203d 2074 656d 7066 696c 652e    fn = tempfile.
-0000f2f0: 6d6b 7465 6d70 2829 0a20 2020 2020 2020  mktemp().       
-0000f300: 2020 2020 2020 2020 2073 656c 662e 7061           self.pa
-0000f310: 7265 6e74 2e5f 736f 6c75 7469 6f6e 732e  rent._solutions.
-0000f320: 4578 706f 7274 4e65 7477 6f72 6b44 6174  ExportNetworkDat
-0000f330: 6128 0a20 2020 2020 2020 2020 2020 2020  a(.             
-0000f340: 2020 2020 2020 205b 5d2c 2073 656c 662e         [], self.
-0000f350: 7061 7265 6e74 2e6e 616d 6520 2b20 2220  parent.name + " 
-0000f360: 3a20 2220 2b20 7365 6c66 2e6e 616d 652c  : " + self.name,
-0000f370: 2032 2c20 666e 2c20 5b22 616c 6c22 5d2c   2, fn, ["all"],
-0000f380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f390: 2020 2020 2046 616c 7365 2c20 302c 2064       False, 0, d
-0000f3a0: 6174 615f 7479 7065 2c20 2d31 2c20 312c  ata_type, -1, 1,
-0000f3b0: 2031 3529 0a20 2020 2020 2020 2020 2020   15).           
-0000f3c0: 2020 2020 2077 6974 6820 6f70 656e 2866       with open(f
-0000f3d0: 6e29 2061 7320 663a 0a20 2020 2020 2020  n) as f:.       
-0000f3e0: 2020 2020 2020 2020 2020 2020 2066 2e72               f.r
-0000f3f0: 6561 646c 696e 6528 290a 2020 2020 2020  eadline().      
-0000f400: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000f410: 6c6e 616d 6573 203d 2066 2e72 6561 646c  lnames = f.readl
-0000f420: 696e 6528 292e 7370 6c69 7428 290a 2020  ine().split().  
-0000f430: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-0000f440: 7261 7920 3d20 6e70 2e6c 6f61 6474 7874  ray = np.loadtxt
-0000f450: 2866 6e2c 2073 6b69 7072 6f77 733d 3229  (fn, skiprows=2)
-0000f460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f470: 2023 2057 4152 4e49 4e47 2066 6f72 2070   # WARNING for p
-0000f480: 7974 686f 6e20 3320 7072 6f62 6162 6c79  ython 3 probably
-0000f490: 206e 6565 6420 746f 2075 7365 2067 656e   need to use gen
-0000f4a0: 6672 6f6d 7478 740a 2020 2020 2020 2020  fromtxt.        
-0000f4b0: 2020 2020 2020 2020 6966 2066 7265 7120          if freq 
-0000f4c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000f4d0: 2020 2020 2020 2020 2020 2020 2066 7265               fre
-0000f4e0: 7120 3d20 6172 7261 795b 3a2c 2030 5d0a  q = array[:, 0].
-0000f4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f500: 2320 544f 444f 3a20 4966 2041 6e73 7973  # TODO: If Ansys
-0000f510: 2076 6572 7369 6f6e 2069 7320 3230 3139   version is 2019
-0000f520: 2c20 7573 6520 2752 6561 6c27 2061 6e64  , use 'Real' and
-0000f530: 2027 496d 6167 270a 2020 2020 2020 2020   'Imag'.        
-0000f540: 2020 2020 2020 2020 2320 696e 2070 6c61          # in pla
-0000f550: 6365 206f 6620 2752 6527 2061 6e64 2027  ce of 'Re' and '
-0000f560: 496d 0a20 2020 2020 2020 2020 2020 2020  Im.             
-0000f570: 2020 2066 6f72 2069 2c20 6a20 696e 206c     for i, j in l
-0000f580: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-0000f590: 2020 2020 2020 2020 2072 6561 6c5f 6964           real_id
-0000f5a0: 7820 3d20 636f 6c6e 616d 6573 2e69 6e64  x = colnames.ind
-0000f5b0: 6578 2822 2573 5b25 642c 2564 5d5f 5265  ex("%s[%d,%d]_Re
-0000f5c0: 2220 250a 2020 2020 2020 2020 2020 2020  " %.            
-0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5f0: 2864 6174 615f 7479 7065 2c20 692c 206a  (data_type, i, j
-0000f600: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-0000f610: 2020 2020 2020 2069 6d61 675f 6964 7820         imag_idx 
-0000f620: 3d20 636f 6c6e 616d 6573 2e69 6e64 6578  = colnames.index
-0000f630: 2822 2573 5b25 642c 2564 5d5f 496d 2220  ("%s[%d,%d]_Im" 
-0000f640: 250a 2020 2020 2020 2020 2020 2020 2020  %.              
-0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f660: 2020 2020 2020 2020 2020 2020 2020 2864                (d
-0000f670: 6174 615f 7479 7065 2c20 692c 206a 2929  ata_type, i, j))
-0000f680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f690: 2020 2020 2063 5f61 7272 203d 2061 7272       c_arr = arr
-0000f6a0: 6179 5b3a 2c20 7265 616c 5f69 6478 5d20  ay[:, real_idx] 
-0000f6b0: 2b20 316a 202a 2061 7272 6179 5b3a 2c20  + 1j * array[:, 
-0000f6c0: 696d 6167 5f69 6478 5d0a 2020 2020 2020  imag_idx].      
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000f6e0: 745b 666f 726d 6174 732e 696e 6465 7828  t[formats.index(
-0000f6f0: 2225 7325 6425 6422 2025 2028 6461 7461  "%s%d%d" % (data
-0000f700: 5f74 7970 652c 2069 2c20 6a29 295d 203d  _type, i, j))] =
-0000f710: 2063 5f61 7272 0a0a 2020 2020 2020 2020   c_arr..        
-0000f720: 7265 7475 726e 2066 7265 712c 2072 6574  return freq, ret
-0000f730: 0a0a 2020 2020 6465 6620 6372 6561 7465  ..    def create
-0000f740: 5f72 6570 6f72 7428 7365 6c66 2c20 6e61  _report(self, na
-0000f750: 6d65 2c20 6578 7072 293a 0a20 2020 2020  me, expr):.     
-0000f760: 2020 2065 7869 7374 696e 6720 3d20 7365     existing = se
-0000f770: 6c66 2e70 6172 656e 742e 5f72 6570 6f72  lf.parent._repor
-0000f780: 7465 722e 4765 7441 6c6c 5265 706f 7274  ter.GetAllReport
-0000f790: 4e61 6d65 7328 290a 2020 2020 2020 2020  Names().        
-0000f7a0: 6e61 6d65 203d 2069 6e63 7265 6d65 6e74  name = increment
-0000f7b0: 5f6e 616d 6528 6e61 6d65 2c20 6578 6973  _name(name, exis
-0000f7c0: 7469 6e67 290a 2020 2020 2020 2020 7661  ting).        va
-0000f7d0: 725f 6e61 6d65 7320 3d20 7365 6c66 2e70  r_names = self.p
-0000f7e0: 6172 656e 742e 7061 7265 6e74 2e67 6574  arent.parent.get
-0000f7f0: 5f76 6172 6961 626c 655f 6e61 6d65 7328  _variable_names(
-0000f800: 290a 2020 2020 2020 2020 7661 725f 6172  ).        var_ar
-0000f810: 6773 203d 2073 756d 285b 5b22 2573 3a3d  gs = sum([["%s:=
-0000f820: 2220 2520 765f 6e61 6d65 2c20 5b22 4e6f  " % v_name, ["No
-0000f830: 6d69 6e61 6c22 5d5d 0a20 2020 2020 2020  minal"]].       
-0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f850: 2066 6f72 2076 5f6e 616d 6520 696e 2076   for v_name in v
-0000f860: 6172 5f6e 616d 6573 5d2c 205b 5d29 0a20  ar_names], []). 
-0000f870: 2020 2020 2020 2073 656c 662e 7061 7265         self.pare
-0000f880: 6e74 2e5f 7265 706f 7274 6572 2e43 7265  nt._reporter.Cre
-0000f890: 6174 6552 6570 6f72 7428 0a20 2020 2020  ateReport(.     
-0000f8a0: 2020 2020 2020 206e 616d 652c 2022 4d6f         name, "Mo
-0000f8b0: 6461 6c20 536f 6c75 7469 6f6e 2044 6174  dal Solution Dat
-0000f8c0: 6122 2c20 2252 6563 7461 6e67 756c 6172  a", "Rectangular
-0000f8d0: 2050 6c6f 7422 2c0a 2020 2020 2020 2020   Plot",.        
-0000f8e0: 2020 2020 7365 6c66 2e73 6f6c 7574 696f      self.solutio
-0000f8f0: 6e5f 6e61 6d65 2c20 5b22 446f 6d61 696e  n_name, ["Domain
-0000f900: 3a3d 222c 2022 5377 6565 7022 5d2c 0a20  :=", "Sweep"],. 
-0000f910: 2020 2020 2020 2020 2020 205b 2246 7265             ["Fre
-0000f920: 713a 3d22 2c20 5b22 416c 6c22 5d5d 202b  q:=", ["All"]] +
-0000f930: 2076 6172 5f61 7267 732c 0a20 2020 2020   var_args,.     
-0000f940: 2020 2020 2020 205b 2258 2043 6f6d 706f         ["X Compo
-0000f950: 6e65 6e74 3a3d 222c 2022 4672 6571 222c  nent:=", "Freq",
-0000f960: 2022 5920 436f 6d70 6f6e 656e 743a 3d22   "Y Component:="
-0000f970: 2c20 5b65 7870 725d 5d2c 205b 5d29 0a20  , [expr]], []). 
-0000f980: 2020 2020 2020 2072 6574 7572 6e20 4866         return Hf
-0000f990: 7373 5265 706f 7274 2873 656c 662e 7061  ssReport(self.pa
-0000f9a0: 7265 6e74 2e70 6172 656e 742c 206e 616d  rent.parent, nam
-0000f9b0: 6529 0a0a 2020 2020 6465 6620 6765 745f  e)..    def get_
-0000f9c0: 7265 706f 7274 5f61 7272 6179 7328 7365  report_arrays(se
-0000f9d0: 6c66 2c20 6578 7072 293a 0a20 2020 2020  lf, expr):.     
-0000f9e0: 2020 2072 203d 2073 656c 662e 6372 6561     r = self.crea
-0000f9f0: 7465 5f72 6570 6f72 7428 2254 656d 7022  te_report("Temp"
-0000fa00: 2c20 6578 7072 290a 2020 2020 2020 2020  , expr).        
-0000fa10: 7265 7475 726e 2072 2e67 6574 5f61 7272  return r.get_arr
-0000fa20: 6179 7328 290a 0a0a 636c 6173 7320 4866  ays()...class Hf
-0000fa30: 7373 5265 706f 7274 2843 4f4d 5772 6170  ssReport(COMWrap
-0000fa40: 7065 7229 3a0a 2020 2020 6465 6620 5f5f  per):.    def __
-0000fa50: 696e 6974 5f5f 2873 656c 662c 2064 6573  init__(self, des
-0000fa60: 6967 6e2c 206e 616d 6529 3a0a 2020 2020  ign, name):.    
-0000fa70: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000fa80: 3a74 7970 6520 6465 7369 676e 3a20 4866  :type design: Hf
-0000fa90: 7373 4465 7369 676e 0a20 2020 2020 2020  ssDesign.       
-0000faa0: 203a 7479 7065 206e 616d 653a 2073 7472   :type name: str
-0000fab0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000fac0: 2020 2020 2073 7570 6572 2848 6673 7352       super(HfssR
-0000fad0: 6570 6f72 742c 2073 656c 6629 2e5f 5f69  eport, self).__i
-0000fae0: 6e69 745f 5f28 290a 2020 2020 2020 2020  nit__().        
-0000faf0: 7365 6c66 2e70 6172 656e 745f 6465 7369  self.parent_desi
-0000fb00: 676e 203d 2064 6573 6967 6e0a 2020 2020  gn = design.    
-0000fb10: 2020 2020 7365 6c66 2e6e 616d 6520 3d20      self.name = 
-0000fb20: 6e61 6d65 0a0a 2020 2020 6465 6620 6578  name..    def ex
-0000fb30: 706f 7274 5f74 6f5f 6669 6c65 2873 656c  port_to_file(sel
-0000fb40: 662c 2066 696c 656e 616d 6529 3a0a 2020  f, filename):.  
-0000fb50: 2020 2020 2020 6669 6c65 7061 7468 203d        filepath =
-0000fb60: 206f 732e 7061 7468 2e61 6273 7061 7468   os.path.abspath
-0000fb70: 2866 696c 656e 616d 6529 0a20 2020 2020  (filename).     
-0000fb80: 2020 2073 656c 662e 7061 7265 6e74 5f64     self.parent_d
-0000fb90: 6573 6967 6e2e 5f72 6570 6f72 7465 722e  esign._reporter.
-0000fba0: 4578 706f 7274 546f 4669 6c65 2873 656c  ExportToFile(sel
-0000fbb0: 662e 6e61 6d65 2c20 6669 6c65 7061 7468  f.name, filepath
-0000fbc0: 290a 0a20 2020 2064 6566 2067 6574 5f61  )..    def get_a
-0000fbd0: 7272 6179 7328 7365 6c66 293a 0a20 2020  rrays(self):.   
-0000fbe0: 2020 2020 2066 6e20 3d20 7465 6d70 6669       fn = tempfi
-0000fbf0: 6c65 2e6d 6b74 656d 7028 7375 6666 6978  le.mktemp(suffix
-0000fc00: 3d22 2e63 7376 2229 0a20 2020 2020 2020  =".csv").       
-0000fc10: 2073 656c 662e 6578 706f 7274 5f74 6f5f   self.export_to_
-0000fc20: 6669 6c65 2866 6e29 0a20 2020 2020 2020  file(fn).       
-0000fc30: 2072 6574 7572 6e20 6e70 2e6c 6f61 6474   return np.loadt
-0000fc40: 7874 2866 6e2c 2073 6b69 7072 6f77 733d  xt(fn, skiprows=
-0000fc50: 312c 2064 656c 696d 6974 6572 3d27 2c27  1, delimiter=','
-0000fc60: 292e 7472 616e 7370 6f73 6528 290a 2020  ).transpose().  
-0000fc70: 2020 2020 2020 2320 7761 726e 696e 6720        # warning 
-0000fc80: 666f 7220 7079 7468 6f6e 2033 2070 726f  for python 3 pro
-0000fc90: 6261 626c 7920 6e65 6564 2074 6f20 7573  bably need to us
-0000fca0: 6520 6765 6e66 726f 6d74 7874 0a0a 0a63  e genfromtxt...c
-0000fcb0: 6c61 7373 204f 7074 696d 6574 7269 6373  lass Optimetrics
-0000fcc0: 2843 4f4d 5772 6170 7065 7229 3a0a 2020  (COMWrapper):.  
-0000fcd0: 2020 2222 220a 2020 2020 4f70 7469 6d65    """.    Optime
-0000fce0: 7472 6963 7320 7363 7269 7074 2063 6f6d  trics script com
-0000fcf0: 6d61 6e64 7320 6578 6563 7574 6564 2062  mands executed b
-0000fd00: 7920 7468 6520 224f 7074 696d 6574 7269  y the "Optimetri
-0000fd10: 6373 2220 6d6f 6475 6c65 2e0a 0a20 2020  cs" module...   
-0000fd20: 2045 7861 6d70 6c65 2075 7365 3a0a 2020   Example use:.  
-0000fd30: 2020 2e2e 2063 6f64 652d 626c 6f63 6b20    .. code-block 
-0000fd40: 7079 7468 6f6e 0a20 2020 2020 2020 2020  python.         
-0000fd50: 2020 206f 7074 6920 3d20 4f70 7469 6d65     opti = Optime
-0000fd60: 7472 6963 7328 7069 6e66 6f2e 6465 7369  trics(pinfo.desi
-0000fd70: 676e 290a 2020 2020 2020 2020 2020 2020  gn).            
-0000fd80: 6e61 6d65 7320 3d20 6f70 7469 2e67 6574  names = opti.get
-0000fd90: 5f73 6574 7570 5f6e 616d 6573 2829 0a20  _setup_names(). 
-0000fda0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000fdb0: 2827 4e61 6d65 7320 6f66 206f 7074 696d  ('Names of optim
-0000fdc0: 6574 7269 6373 3a20 272c 206e 616d 6573  etrics: ', names
-0000fdd0: 290a 2020 2020 2020 2020 2020 2020 6f70  ).            op
-0000fde0: 7469 2e73 6f6c 7665 5f73 6574 7570 286e  ti.solve_setup(n
-0000fdf0: 616d 6573 5b30 5d29 0a0a 2020 2020 4e6f  ames[0])..    No
-0000fe00: 7465 2074 6861 7420 7275 6e6e 696e 6720  te that running 
-0000fe10: 6f70 7469 6d65 7472 6963 7320 7265 7175  optimetrics requ
-0000fe20: 6972 6573 2074 6865 206c 6963 656e 7365  ires the license
-0000fe30: 2066 6f72 204f 7074 696d 6574 7269 6373   for Optimetrics
-0000fe40: 2062 7920 416e 7379 732e 0a20 2020 2022   by Ansys..    "
-0000fe50: 2222 0a20 2020 2064 6566 205f 5f69 6e69  "".    def __ini
-0000fe60: 745f 5f28 7365 6c66 2c20 6465 7369 676e  t__(self, design
-0000fe70: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
-0000fe80: 284f 7074 696d 6574 7269 6373 2c20 7365  (Optimetrics, se
-0000fe90: 6c66 292e 5f5f 696e 6974 5f5f 2829 0a0a  lf).__init__()..
-0000fea0: 2020 2020 2020 2020 7365 6c66 2e64 6573          self.des
-0000feb0: 6967 6e20 3d20 6465 7369 676e 2020 2320  ign = design  # 
-0000fec0: 7061 7265 6e74 0a20 2020 2020 2020 2073  parent.        s
-0000fed0: 656c 662e 5f6f 7074 696d 6574 7269 6373  elf._optimetrics
-0000fee0: 203d 2073 656c 662e 6465 7369 676e 2e5f   = self.design._
-0000fef0: 6f70 7469 6d65 7472 6963 7320 2023 203c  optimetrics  # <
-0000ff00: 434f 4d4f 626a 6563 7420 4765 744d 6f64  COMObject GetMod
-0000ff10: 756c 653e 0a20 2020 2020 2020 2073 656c  ule>.        sel
-0000ff20: 662e 7365 7475 705f 6e61 6d65 7320 3d20  f.setup_names = 
-0000ff30: 4e6f 6e65 0a0a 2020 2020 6465 6620 6765  None..    def ge
-0000ff40: 745f 7365 7475 705f 6e61 6d65 7328 7365  t_setup_names(se
-0000ff50: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-0000ff60: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
-0000ff70: 6c69 7374 206f 6620 4f70 7469 6d65 7472  list of Optimetr
-0000ff80: 6963 7320 7365 7475 7020 6e61 6d65 730a  ics setup names.
-0000ff90: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000ffa0: 2020 2020 7365 6c66 2e73 6574 7570 5f6e      self.setup_n
-0000ffb0: 616d 6573 203d 206c 6973 7428 7365 6c66  ames = list(self
-0000ffc0: 2e5f 6f70 7469 6d65 7472 6963 732e 4765  ._optimetrics.Ge
-0000ffd0: 7453 6574 7570 4e61 6d65 7328 2929 0a20  tSetupNames()). 
-0000ffe0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000fff0: 6c66 2e73 6574 7570 5f6e 616d 6573 2e63  lf.setup_names.c
-00010000: 6f70 7928 290a 0a20 2020 2064 6566 2073  opy()..    def s
-00010010: 6f6c 7665 5f73 6574 7570 2873 656c 662c  olve_setup(self,
-00010020: 2073 6574 7570 5f6e 616d 653a 2073 7472   setup_name: str
-00010030: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00010040: 2020 2020 2020 2053 6f6c 7665 7320 7468         Solves th
-00010050: 6520 7370 6563 6966 6965 6420 4f70 7469  e specified Opti
-00010060: 6d65 7472 6963 7320 7365 7475 702e 0a20  metrics setup.. 
-00010070: 2020 2020 2020 2043 6f72 7265 7370 6f6e         Correspon
-00010080: 6473 2074 6f3a 2020 5269 6768 742d 636c  ds to:  Right-cl
-00010090: 6963 6b20 7468 6520 7365 7475 7020 696e  ick the setup in
-000100a0: 2074 6865 2070 726f 6a65 6374 2074 7265   the project tre
-000100b0: 652c 2061 6e64 2074 6865 6e20 636c 6963  e, and then clic
-000100c0: 6b0a 2020 2020 2020 2020 416e 616c 797a  k.        Analyz
-000100d0: 6520 6f6e 2074 6865 2073 686f 7274 6375  e on the shortcu
-000100e0: 7420 6d65 6e75 2e0a 0a20 2020 2020 2020  t menu...       
-000100f0: 2073 6574 7570 5f6e 616d 6520 2873 7472   setup_name (str
-00010100: 2920 3a20 6e61 6d65 206f 6620 7365 7475  ) : name of setu
-00010110: 702c 2073 686f 756c 6420 6265 2069 6e20  p, should be in 
-00010120: 6765 745f 7365 7475 705f 6e61 6d65 730a  get_setup_names.
-00010130: 0a20 2020 2020 2020 2042 6c6f 636b 7320  .        Blocks 
-00010140: 6578 6563 7574 696f 6e20 756e 7469 6c20  execution until 
-00010150: 7265 6164 7920 746f 2075 7365 2e0a 0a20  ready to use... 
-00010160: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
-00010170: 2074 6869 7320 7265 7175 6972 6573 2074   this requires t
-00010180: 6865 206c 6963 656e 7365 2066 6f72 204f  he license for O
-00010190: 7074 696d 6574 7269 6373 2062 7920 416e  ptimetrics by An
-000101a0: 7379 732e 0a20 2020 2020 2020 2022 2222  sys..        """
-000101b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000101c0: 7365 6c66 2e5f 6f70 7469 6d65 7472 6963  self._optimetric
-000101d0: 732e 536f 6c76 6553 6574 7570 2873 6574  s.SolveSetup(set
-000101e0: 7570 5f6e 616d 6529 0a0a 2020 2020 6465  up_name)..    de
-000101f0: 6620 6372 6561 7465 5f73 6574 7570 2873  f create_setup(s
-00010200: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-00010210: 2020 2020 2020 2020 2020 7661 7269 6162            variab
-00010220: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
-00010230: 2020 2020 2020 2020 2073 7770 5f70 6172           swp_par
-00010240: 616d 732c 0a20 2020 2020 2020 2020 2020  ams,.           
-00010250: 2020 2020 2020 2020 2020 6e61 6d65 3d22            name="
-00010260: 5061 7261 6d65 7472 6963 5365 7475 7031  ParametricSetup1
-00010270: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010280: 2020 2020 2020 2020 7377 705f 7479 7065          swp_type
-00010290: 3d27 6c69 6e65 6172 5f73 7465 7027 2c0a  ='linear_step',.
-000102a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102b0: 2020 2020 2073 6574 7570 5f6e 616d 653d       setup_name=
-000102c0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-000102d0: 2020 2020 2020 2020 2020 2073 6176 655f             save_
-000102e0: 6669 656c 6473 3d54 7275 652c 0a20 2020  fields=True,.   
-000102f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010300: 2020 636f 7079 5f6d 6573 683d 5472 7565    copy_mesh=True
+0000ea50: 2d2d 2d2d 0a20 2020 2020 2020 2045 7861  ----.        Exa
+0000ea60: 6d70 6c65 2070 6c6f 7420 666f 7220 6120  mple plot for a 
+0000ea70: 7369 6e67 6c65 2076 6172 6961 7469 6f6e  single variation
+0000ea80: 2061 6c6c 2070 6173 7320 636f 6e76 6572   all pass conver
+0000ea90: 6765 206f 6620 6d6f 6465 2066 7265 710a  ge of mode freq.
+0000eaa0: 0a20 2020 2020 2020 202e 2e20 636f 6465  .        .. code
+0000eab0: 2d62 6c6f 636b 3a3a 2070 7974 686f 6e0a  -block:: python.
+0000eac0: 0a20 2020 2020 2020 2020 2020 2079 636f  .            yco
+0000ead0: 6d70 203d 205b 6622 7265 284d 6f64 6528  mp = [f"re(Mode(
+0000eae0: 7b69 7d29 2922 2066 6f72 2069 2069 6e20  {i}))" for i in 
+0000eaf0: 7261 6e67 6528 312c 312b 6570 725f 6866  range(1,1+epr_hf
+0000eb00: 7373 2e6e 5f6d 6f64 6573 295d 0a20 2020  ss.n_modes)].   
+0000eb10: 2020 2020 2020 2020 2070 6172 616d 7320           params 
+0000eb20: 3d20 5b22 5061 7373 3a3d 222c 205b 2241  = ["Pass:=", ["A
+0000eb30: 6c6c 225d 5d2b 7661 7269 6174 696f 6e0a  ll"]]+variation.
+0000eb40: 2020 2020 2020 2020 2020 2020 7365 7475              setu
+0000eb50: 702e 6372 6561 7465 5f72 6570 6f72 7428  p.create_report(
+0000eb60: 2246 7265 712e 2076 732e 2070 6173 7322  "Freq. vs. pass"
+0000eb70: 2c20 2250 6173 7322 2c20 7963 6f6d 702c  , "Pass", ycomp,
+0000eb80: 2070 6172 616d 732c 2070 6173 735f 6e61   params, pass_na
+0000eb90: 6d65 3d27 4164 6170 7469 7665 5061 7373  me='AdaptivePass
+0000eba0: 2729 0a20 2020 2020 2020 2027 2727 0a20  ').        '''. 
+0000ebb0: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
+0000ebc0: 696e 7374 616e 6365 2879 636f 6d70 2c20  instance(ycomp, 
+0000ebd0: 6c69 7374 290a 2020 2020 2020 2020 6173  list).        as
+0000ebe0: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
+0000ebf0: 7061 7261 6d73 2c20 6c69 7374 290a 0a20  params, list).. 
+0000ec00: 2020 2020 2020 2073 6574 7570 203d 2073         setup = s
+0000ec10: 656c 662e 7061 7265 6e74 0a20 2020 2020  elf.parent.     
+0000ec20: 2020 2072 6570 6f72 7465 7220 3d20 7365     reporter = se
+0000ec30: 7475 702e 5f72 6570 6f72 7465 720a 2020  tup._reporter.  
+0000ec40: 2020 2020 2020 7265 7475 726e 2072 6570        return rep
+0000ec50: 6f72 7465 722e 4372 6561 7465 5265 706f  orter.CreateRepo
+0000ec60: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
+0000ec70: 706c 6f74 5f6e 616d 652c 2022 4569 6765  plot_name, "Eige
+0000ec80: 6e6d 6f64 6520 5061 7261 6d65 7465 7273  nmode Parameters
+0000ec90: 222c 2022 5265 6374 616e 6775 6c61 7220  ", "Rectangular 
+0000eca0: 506c 6f74 222c 0a20 2020 2020 2020 2020  Plot",.         
+0000ecb0: 2020 2066 227b 7365 7475 702e 6e61 6d65     f"{setup.name
+0000ecc0: 7d20 3a20 7b70 6173 735f 6e61 6d65 7d22  } : {pass_name}"
+0000ecd0: 2c20 5b5d 2c20 7061 7261 6d73 2c0a 2020  , [], params,.  
+0000ece0: 2020 2020 2020 2020 2020 5b22 5820 436f            ["X Co
+0000ecf0: 6d70 6f6e 656e 743a 3d22 2c20 7863 6f6d  mponent:=", xcom
+0000ed00: 702c 2022 5920 436f 6d70 6f6e 656e 743a  p, "Y Component:
+0000ed10: 3d22 2c20 7963 6f6d 705d 2c20 5b5d 290a  =", ycomp], []).
+0000ed20: 0a0a 636c 6173 7320 4866 7373 444d 4465  ..class HfssDMDe
+0000ed30: 7369 676e 536f 6c75 7469 6f6e 7328 4866  signSolutions(Hf
+0000ed40: 7373 4465 7369 676e 536f 6c75 7469 6f6e  ssDesignSolution
+0000ed50: 7329 3a0a 2020 2020 7061 7373 0a0a 636c  s):.    pass..cl
+0000ed60: 6173 7320 4866 7373 4454 4465 7369 676e  ass HfssDTDesign
+0000ed70: 536f 6c75 7469 6f6e 7328 4866 7373 4465  Solutions(HfssDe
+0000ed80: 7369 676e 536f 6c75 7469 6f6e 7329 3a0a  signSolutions):.
+0000ed90: 2020 2020 7061 7373 0a0a 636c 6173 7320      pass..class 
+0000eda0: 4866 7373 5133 4444 6573 6967 6e53 6f6c  HfssQ3DDesignSol
+0000edb0: 7574 696f 6e73 2848 6673 7344 6573 6967  utions(HfssDesig
+0000edc0: 6e53 6f6c 7574 696f 6e73 293a 0a20 2020  nSolutions):.   
+0000edd0: 2070 6173 730a 0a0a 636c 6173 7320 4866   pass...class Hf
+0000ede0: 7373 4672 6571 7565 6e63 7953 7765 6570  ssFrequencySweep
+0000edf0: 2843 4f4d 5772 6170 7065 7229 3a0a 2020  (COMWrapper):.  
+0000ee00: 2020 7072 6f70 5f74 6162 203d 2022 4866    prop_tab = "Hf
+0000ee10: 7373 5461 6222 0a20 2020 2073 7461 7274  ssTab".    start
+0000ee20: 5f66 7265 7120 3d20 6d61 6b65 5f66 6c6f  _freq = make_flo
+0000ee30: 6174 5f70 726f 7028 2253 7461 7274 2229  at_prop("Start")
+0000ee40: 0a20 2020 2073 746f 705f 6672 6571 203d  .    stop_freq =
+0000ee50: 206d 616b 655f 666c 6f61 745f 7072 6f70   make_float_prop
+0000ee60: 2822 5374 6f70 2229 0a20 2020 2073 7465  ("Stop").    ste
+0000ee70: 705f 7369 7a65 203d 206d 616b 655f 666c  p_size = make_fl
+0000ee80: 6f61 745f 7072 6f70 2822 5374 6570 2053  oat_prop("Step S
+0000ee90: 697a 6522 290a 2020 2020 636f 756e 7420  ize").    count 
+0000eea0: 3d20 6d61 6b65 5f66 6c6f 6174 5f70 726f  = make_float_pro
+0000eeb0: 7028 2243 6f75 6e74 2229 0a20 2020 2073  p("Count").    s
+0000eec0: 7765 6570 5f74 7970 6520 3d20 6d61 6b65  weep_type = make
+0000eed0: 5f73 7472 5f70 726f 7028 2254 7970 6522  _str_prop("Type"
+0000eee0: 290a 0a20 2020 2064 6566 205f 5f69 6e69  )..    def __ini
+0000eef0: 745f 5f28 7365 6c66 2c20 7365 7475 702c  t__(self, setup,
+0000ef00: 206e 616d 6529 3a0a 2020 2020 2020 2020   name):.        
+0000ef10: 2222 220a 2020 2020 2020 2020 3a74 7970  """.        :typ
+0000ef20: 6520 7365 7475 703a 2048 6673 7353 6574  e setup: HfssSet
+0000ef30: 7570 0a20 2020 2020 2020 203a 7479 7065  up.        :type
+0000ef40: 206e 616d 653a 2073 7472 0a20 2020 2020   name: str.     
+0000ef50: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+0000ef60: 7570 6572 2848 6673 7346 7265 7175 656e  uper(HfssFrequen
+0000ef70: 6379 5377 6565 702c 2073 656c 6629 2e5f  cySweep, self)._
+0000ef80: 5f69 6e69 745f 5f28 290a 2020 2020 2020  _init__().      
+0000ef90: 2020 7365 6c66 2e70 6172 656e 7420 3d20    self.parent = 
+0000efa0: 7365 7475 700a 2020 2020 2020 2020 7365  setup.        se
+0000efb0: 6c66 2e6e 616d 6520 3d20 6e61 6d65 0a20  lf.name = name. 
+0000efc0: 2020 2020 2020 2073 656c 662e 736f 6c75         self.solu
+0000efd0: 7469 6f6e 5f6e 616d 6520 3d20 7365 6c66  tion_name = self
+0000efe0: 2e70 6172 656e 742e 6e61 6d65 202b 2022  .parent.name + "
+0000eff0: 203a 2022 202b 206e 616d 650a 2020 2020   : " + name.    
+0000f000: 2020 2020 7365 6c66 2e70 726f 705f 686f      self.prop_ho
+0000f010: 6c64 6572 203d 2073 656c 662e 7061 7265  lder = self.pare
+0000f020: 6e74 2e70 726f 705f 686f 6c64 6572 0a20  nt.prop_holder. 
+0000f030: 2020 2020 2020 2073 656c 662e 7072 6f70         self.prop
+0000f040: 5f73 6572 7665 7220 3d20 7365 6c66 2e70  _server = self.p
+0000f050: 6172 656e 742e 7072 6f70 5f73 6572 7665  arent.prop_serve
+0000f060: 7220 2b20 223a 2220 2b20 6e61 6d65 0a20  r + ":" + name. 
+0000f070: 2020 2020 2020 2073 656c 662e 5f61 6e73         self._ans
+0000f080: 7973 5f76 6572 7369 6f6e 203d 2073 656c  ys_version = sel
+0000f090: 662e 7061 7265 6e74 2e5f 616e 7379 735f  f.parent._ansys_
+0000f0a0: 7665 7273 696f 6e0a 0a20 2020 2064 6566  version..    def
+0000f0b0: 2061 6e61 6c79 7a65 5f73 7765 6570 2873   analyze_sweep(s
+0000f0c0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0000f0d0: 6c66 2e70 6172 656e 742e 616e 616c 797a  lf.parent.analyz
+0000f0e0: 6528 7365 6c66 2e73 6f6c 7574 696f 6e5f  e(self.solution_
+0000f0f0: 6e61 6d65 290a 0a20 2020 2064 6566 2067  name)..    def g
+0000f100: 6574 5f6e 6574 776f 726b 5f64 6174 6128  et_network_data(
+0000f110: 7365 6c66 2c20 666f 726d 6174 7329 3a0a  self, formats):.
+0000f120: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+0000f130: 7461 6e63 6528 666f 726d 6174 732c 2073  tance(formats, s
+0000f140: 7472 293a 0a20 2020 2020 2020 2020 2020  tr):.           
+0000f150: 2066 6f72 6d61 7473 203d 2066 6f72 6d61   formats = forma
+0000f160: 7473 2e73 706c 6974 2822 2c22 290a 2020  ts.split(",").  
+0000f170: 2020 2020 2020 666f 726d 6174 7320 3d20        formats = 
+0000f180: 5b66 2e75 7070 6572 2829 2066 6f72 2066  [f.upper() for f
+0000f190: 2069 6e20 666f 726d 6174 735d 0a0a 2020   in formats]..  
+0000f1a0: 2020 2020 2020 666d 7473 5f6c 6973 7473        fmts_lists
+0000f1b0: 203d 207b 2753 273a 205b 5d2c 2027 5927   = {'S': [], 'Y'
+0000f1c0: 3a20 5b5d 2c20 275a 273a 205b 5d7d 0a0a  : [], 'Z': []}..
+0000f1d0: 2020 2020 2020 2020 666f 7220 6620 696e          for f in
+0000f1e0: 2066 6f72 6d61 7473 3a0a 2020 2020 2020   formats:.      
+0000f1f0: 2020 2020 2020 666d 7473 5f6c 6973 7473        fmts_lists
+0000f200: 5b66 5b30 5d5d 2e61 7070 656e 6428 2869  [f[0]].append((i
+0000f210: 6e74 2866 5b31 5d29 2c20 696e 7428 665b  nt(f[1]), int(f[
+0000f220: 325d 2929 290a 2020 2020 2020 2020 7265  2]))).        re
+0000f230: 7420 3d20 5b4e 6f6e 655d 202a 206c 656e  t = [None] * len
+0000f240: 2866 6f72 6d61 7473 290a 2020 2020 2020  (formats).      
+0000f250: 2020 6672 6571 203d 204e 6f6e 650a 0a20    freq = None.. 
+0000f260: 2020 2020 2020 2066 6f72 2064 6174 615f         for data_
+0000f270: 7479 7065 2c20 6c69 7374 2069 6e20 666d  type, list in fm
+0000f280: 7473 5f6c 6973 7473 2e69 7465 6d73 2829  ts_lists.items()
+0000f290: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000f2a0: 206c 6973 743a 0a20 2020 2020 2020 2020   list:.         
+0000f2b0: 2020 2020 2020 2066 6e20 3d20 7465 6d70         fn = temp
+0000f2c0: 6669 6c65 2e6d 6b74 656d 7028 290a 2020  file.mktemp().  
+0000f2d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000f2e0: 6c66 2e70 6172 656e 742e 5f73 6f6c 7574  lf.parent._solut
+0000f2f0: 696f 6e73 2e45 7870 6f72 744e 6574 776f  ions.ExportNetwo
+0000f300: 726b 4461 7461 280a 2020 2020 2020 2020  rkData(.        
+0000f310: 2020 2020 2020 2020 2020 2020 5b5d 2c20              [], 
+0000f320: 7365 6c66 2e70 6172 656e 742e 6e61 6d65  self.parent.name
+0000f330: 202b 2022 203a 2022 202b 2073 656c 662e   + " : " + self.
+0000f340: 6e61 6d65 2c20 322c 2066 6e2c 205b 2261  name, 2, fn, ["a
+0000f350: 6c6c 225d 2c0a 2020 2020 2020 2020 2020  ll"],.          
+0000f360: 2020 2020 2020 2020 2020 4661 6c73 652c            False,
+0000f370: 2030 2c20 6461 7461 5f74 7970 652c 202d   0, data_type, -
+0000f380: 312c 2031 2c20 3135 290a 2020 2020 2020  1, 1, 15).      
+0000f390: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+0000f3a0: 7065 6e28 666e 2920 6173 2066 3a0a 2020  pen(fn) as f:.  
+0000f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3c0: 2020 662e 7265 6164 6c69 6e65 2829 0a20    f.readline(). 
+0000f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f3e0: 2020 2063 6f6c 6e61 6d65 7320 3d20 662e     colnames = f.
+0000f3f0: 7265 6164 6c69 6e65 2829 2e73 706c 6974  readline().split
+0000f400: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000f410: 2020 2061 7272 6179 203d 206e 702e 6c6f     array = np.lo
+0000f420: 6164 7478 7428 666e 2c20 736b 6970 726f  adtxt(fn, skipro
+0000f430: 7773 3d32 290a 2020 2020 2020 2020 2020  ws=2).          
+0000f440: 2020 2020 2020 2320 5741 524e 494e 4720        # WARNING 
+0000f450: 666f 7220 7079 7468 6f6e 2033 2070 726f  for python 3 pro
+0000f460: 6261 626c 7920 6e65 6564 2074 6f20 7573  bably need to us
+0000f470: 6520 6765 6e66 726f 6d74 7874 0a20 2020  e genfromtxt.   
+0000f480: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000f490: 6672 6571 2069 7320 4e6f 6e65 3a0a 2020  freq is None:.  
+0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f4b0: 2020 6672 6571 203d 2061 7272 6179 5b3a    freq = array[:
+0000f4c0: 2c20 305d 0a20 2020 2020 2020 2020 2020  , 0].           
+0000f4d0: 2020 2020 2023 2054 4f44 4f3a 2049 6620       # TODO: If 
+0000f4e0: 416e 7379 7320 7665 7273 696f 6e20 6973  Ansys version is
+0000f4f0: 2032 3031 392c 2075 7365 2027 5265 616c   2019, use 'Real
+0000f500: 2720 616e 6420 2749 6d61 6727 0a20 2020  ' and 'Imag'.   
+0000f510: 2020 2020 2020 2020 2020 2020 2023 2069               # i
+0000f520: 6e20 706c 6163 6520 6f66 2027 5265 2720  n place of 'Re' 
+0000f530: 616e 6420 2749 6d0a 2020 2020 2020 2020  and 'Im.        
+0000f540: 2020 2020 2020 2020 666f 7220 692c 206a          for i, j
+0000f550: 2069 6e20 6c69 7374 3a0a 2020 2020 2020   in list:.      
+0000f560: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000f570: 616c 5f69 6478 203d 2063 6f6c 6e61 6d65  al_idx = colname
+0000f580: 732e 696e 6465 7828 2225 735b 2564 2c25  s.index("%s[%d,%
+0000f590: 645d 5f52 6522 2025 0a20 2020 2020 2020  d]_Re" %.       
+0000f5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5c0: 2020 2020 2028 6461 7461 5f74 7970 652c       (data_type,
+0000f5d0: 2069 2c20 6a29 290a 2020 2020 2020 2020   i, j)).        
+0000f5e0: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+0000f5f0: 5f69 6478 203d 2063 6f6c 6e61 6d65 732e  _idx = colnames.
+0000f600: 696e 6465 7828 2225 735b 2564 2c25 645d  index("%s[%d,%d]
+0000f610: 5f49 6d22 2025 0a20 2020 2020 2020 2020  _Im" %.         
+0000f620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f640: 2020 2028 6461 7461 5f74 7970 652c 2069     (data_type, i
+0000f650: 2c20 6a29 290a 2020 2020 2020 2020 2020  , j)).          
+0000f660: 2020 2020 2020 2020 2020 635f 6172 7220            c_arr 
+0000f670: 3d20 6172 7261 795b 3a2c 2072 6561 6c5f  = array[:, real_
+0000f680: 6964 785d 202b 2031 6a20 2a20 6172 7261  idx] + 1j * arra
+0000f690: 795b 3a2c 2069 6d61 675f 6964 785d 0a20  y[:, imag_idx]. 
+0000f6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6b0: 2020 2072 6574 5b66 6f72 6d61 7473 2e69     ret[formats.i
+0000f6c0: 6e64 6578 2822 2573 2564 2564 2220 2520  ndex("%s%d%d" % 
+0000f6d0: 2864 6174 615f 7479 7065 2c20 692c 206a  (data_type, i, j
+0000f6e0: 2929 5d20 3d20 635f 6172 720a 0a20 2020  ))] = c_arr..   
+0000f6f0: 2020 2020 2072 6574 7572 6e20 6672 6571       return freq
+0000f700: 2c20 7265 740a 0a20 2020 2064 6566 2063  , ret..    def c
+0000f710: 7265 6174 655f 7265 706f 7274 2873 656c  reate_report(sel
+0000f720: 662c 206e 616d 652c 2065 7870 7229 3a0a  f, name, expr):.
+0000f730: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
+0000f740: 203d 2073 656c 662e 7061 7265 6e74 2e5f   = self.parent._
+0000f750: 7265 706f 7274 6572 2e47 6574 416c 6c52  reporter.GetAllR
+0000f760: 6570 6f72 744e 616d 6573 2829 0a20 2020  eportNames().   
+0000f770: 2020 2020 206e 616d 6520 3d20 696e 6372       name = incr
+0000f780: 656d 656e 745f 6e61 6d65 286e 616d 652c  ement_name(name,
+0000f790: 2065 7869 7374 696e 6729 0a20 2020 2020   existing).     
+0000f7a0: 2020 2076 6172 5f6e 616d 6573 203d 2073     var_names = s
+0000f7b0: 656c 662e 7061 7265 6e74 2e70 6172 656e  elf.parent.paren
+0000f7c0: 742e 6765 745f 7661 7269 6162 6c65 5f6e  t.get_variable_n
+0000f7d0: 616d 6573 2829 0a20 2020 2020 2020 2076  ames().        v
+0000f7e0: 6172 5f61 7267 7320 3d20 7375 6d28 5b5b  ar_args = sum([[
+0000f7f0: 2225 733a 3d22 2025 2076 5f6e 616d 652c  "%s:=" % v_name,
+0000f800: 205b 224e 6f6d 696e 616c 225d 5d0a 2020   ["Nominal"]].  
+0000f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f820: 2020 2020 2020 666f 7220 765f 6e61 6d65        for v_name
+0000f830: 2069 6e20 7661 725f 6e61 6d65 735d 2c20   in var_names], 
+0000f840: 5b5d 290a 2020 2020 2020 2020 7365 6c66  []).        self
+0000f850: 2e70 6172 656e 742e 5f72 6570 6f72 7465  .parent._reporte
+0000f860: 722e 4372 6561 7465 5265 706f 7274 280a  r.CreateReport(.
+0000f870: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+0000f880: 2c20 224d 6f64 616c 2053 6f6c 7574 696f  , "Modal Solutio
+0000f890: 6e20 4461 7461 222c 2022 5265 6374 616e  n Data", "Rectan
+0000f8a0: 6775 6c61 7220 506c 6f74 222c 0a20 2020  gular Plot",.   
+0000f8b0: 2020 2020 2020 2020 2073 656c 662e 736f           self.so
+0000f8c0: 6c75 7469 6f6e 5f6e 616d 652c 205b 2244  lution_name, ["D
+0000f8d0: 6f6d 6169 6e3a 3d22 2c20 2253 7765 6570  omain:=", "Sweep
+0000f8e0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+0000f8f0: 5b22 4672 6571 3a3d 222c 205b 2241 6c6c  ["Freq:=", ["All
+0000f900: 225d 5d20 2b20 7661 725f 6172 6773 2c0a  "]] + var_args,.
+0000f910: 2020 2020 2020 2020 2020 2020 5b22 5820              ["X 
+0000f920: 436f 6d70 6f6e 656e 743a 3d22 2c20 2246  Component:=", "F
+0000f930: 7265 7122 2c20 2259 2043 6f6d 706f 6e65  req", "Y Compone
+0000f940: 6e74 3a3d 222c 205b 6578 7072 5d5d 2c20  nt:=", [expr]], 
+0000f950: 5b5d 290a 2020 2020 2020 2020 7265 7475  []).        retu
+0000f960: 726e 2048 6673 7352 6570 6f72 7428 7365  rn HfssReport(se
+0000f970: 6c66 2e70 6172 656e 742e 7061 7265 6e74  lf.parent.parent
+0000f980: 2c20 6e61 6d65 290a 0a20 2020 2064 6566  , name)..    def
+0000f990: 2067 6574 5f72 6570 6f72 745f 6172 7261   get_report_arra
+0000f9a0: 7973 2873 656c 662c 2065 7870 7229 3a0a  ys(self, expr):.
+0000f9b0: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
+0000f9c0: 2e63 7265 6174 655f 7265 706f 7274 2822  .create_report("
+0000f9d0: 5465 6d70 222c 2065 7870 7229 0a20 2020  Temp", expr).   
+0000f9e0: 2020 2020 2072 6574 7572 6e20 722e 6765       return r.ge
+0000f9f0: 745f 6172 7261 7973 2829 0a0a 0a63 6c61  t_arrays()...cla
+0000fa00: 7373 2048 6673 7352 6570 6f72 7428 434f  ss HfssReport(CO
+0000fa10: 4d57 7261 7070 6572 293a 0a20 2020 2064  MWrapper):.    d
+0000fa20: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0000fa30: 2c20 6465 7369 676e 2c20 6e61 6d65 293a  , design, name):
+0000fa40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000fa50: 2020 2020 203a 7479 7065 2064 6573 6967       :type desig
+0000fa60: 6e3a 2048 6673 7344 6573 6967 6e0a 2020  n: HfssDesign.  
+0000fa70: 2020 2020 2020 3a74 7970 6520 6e61 6d65        :type name
+0000fa80: 3a20 7374 720a 2020 2020 2020 2020 2222  : str.        ""
+0000fa90: 220a 2020 2020 2020 2020 7375 7065 7228  ".        super(
+0000faa0: 4866 7373 5265 706f 7274 2c20 7365 6c66  HfssReport, self
+0000fab0: 292e 5f5f 696e 6974 5f5f 2829 0a20 2020  ).__init__().   
+0000fac0: 2020 2020 2073 656c 662e 7061 7265 6e74       self.parent
+0000fad0: 5f64 6573 6967 6e20 3d20 6465 7369 676e  _design = design
+0000fae0: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
+0000faf0: 6d65 203d 206e 616d 650a 0a20 2020 2064  me = name..    d
+0000fb00: 6566 2065 7870 6f72 745f 746f 5f66 696c  ef export_to_fil
+0000fb10: 6528 7365 6c66 2c20 6669 6c65 6e61 6d65  e(self, filename
+0000fb20: 293a 0a20 2020 2020 2020 2066 696c 6570  ):.        filep
+0000fb30: 6174 6820 3d20 6f73 2e70 6174 682e 6162  ath = os.path.ab
+0000fb40: 7370 6174 6828 6669 6c65 6e61 6d65 290a  spath(filename).
+0000fb50: 2020 2020 2020 2020 7365 6c66 2e70 6172          self.par
+0000fb60: 656e 745f 6465 7369 676e 2e5f 7265 706f  ent_design._repo
+0000fb70: 7274 6572 2e45 7870 6f72 7454 6f46 696c  rter.ExportToFil
+0000fb80: 6528 7365 6c66 2e6e 616d 652c 2066 696c  e(self.name, fil
+0000fb90: 6570 6174 6829 0a0a 2020 2020 6465 6620  epath)..    def 
+0000fba0: 6765 745f 6172 7261 7973 2873 656c 6629  get_arrays(self)
+0000fbb0: 3a0a 2020 2020 2020 2020 666e 203d 2074  :.        fn = t
+0000fbc0: 656d 7066 696c 652e 6d6b 7465 6d70 2873  empfile.mktemp(s
+0000fbd0: 7566 6669 783d 222e 6373 7622 290a 2020  uffix=".csv").  
+0000fbe0: 2020 2020 2020 7365 6c66 2e65 7870 6f72        self.expor
+0000fbf0: 745f 746f 5f66 696c 6528 666e 290a 2020  t_to_file(fn).  
+0000fc00: 2020 2020 2020 7265 7475 726e 206e 702e        return np.
+0000fc10: 6c6f 6164 7478 7428 666e 2c20 736b 6970  loadtxt(fn, skip
+0000fc20: 726f 7773 3d31 2c20 6465 6c69 6d69 7465  rows=1, delimite
+0000fc30: 723d 272c 2729 2e74 7261 6e73 706f 7365  r=',').transpose
+0000fc40: 2829 0a20 2020 2020 2020 2023 2077 6172  ().        # war
+0000fc50: 6e69 6e67 2066 6f72 2070 7974 686f 6e20  ning for python 
+0000fc60: 3320 7072 6f62 6162 6c79 206e 6565 6420  3 probably need 
+0000fc70: 746f 2075 7365 2067 656e 6672 6f6d 7478  to use genfromtx
+0000fc80: 740a 0a0a 636c 6173 7320 4f70 7469 6d65  t...class Optime
+0000fc90: 7472 6963 7328 434f 4d57 7261 7070 6572  trics(COMWrapper
+0000fca0: 293a 0a20 2020 2022 2222 0a20 2020 204f  ):.    """.    O
+0000fcb0: 7074 696d 6574 7269 6373 2073 6372 6970  ptimetrics scrip
+0000fcc0: 7420 636f 6d6d 616e 6473 2065 7865 6375  t commands execu
+0000fcd0: 7465 6420 6279 2074 6865 2022 4f70 7469  ted by the "Opti
+0000fce0: 6d65 7472 6963 7322 206d 6f64 756c 652e  metrics" module.
+0000fcf0: 0a0a 2020 2020 4578 616d 706c 6520 7573  ..    Example us
+0000fd00: 653a 0a0a 2020 2020 2e2e 2063 6f64 652d  e:..    .. code-
+0000fd10: 626c 6f63 6b3a 3a20 7079 7468 6f6e 0a0a  block:: python..
+0000fd20: 2020 2020 2020 2020 6f70 7469 203d 204f          opti = O
+0000fd30: 7074 696d 6574 7269 6373 2870 696e 666f  ptimetrics(pinfo
+0000fd40: 2e64 6573 6967 6e29 0a20 2020 2020 2020  .design).       
+0000fd50: 206e 616d 6573 203d 206f 7074 692e 6765   names = opti.ge
+0000fd60: 745f 7365 7475 705f 6e61 6d65 7328 290a  t_setup_names().
+0000fd70: 2020 2020 2020 2020 7072 696e 7428 274e          print('N
+0000fd80: 616d 6573 206f 6620 6f70 7469 6d65 7472  ames of optimetr
+0000fd90: 6963 733a 2027 2c20 6e61 6d65 7329 0a20  ics: ', names). 
+0000fda0: 2020 2020 2020 206f 7074 692e 736f 6c76         opti.solv
+0000fdb0: 655f 7365 7475 7028 6e61 6d65 735b 305d  e_setup(names[0]
+0000fdc0: 290a 0a20 2020 204e 6f74 6520 7468 6174  )..    Note that
+0000fdd0: 2072 756e 6e69 6e67 206f 7074 696d 6574   running optimet
+0000fde0: 7269 6373 2072 6571 7569 7265 7320 7468  rics requires th
+0000fdf0: 6520 6c69 6365 6e73 6520 666f 7220 4f70  e license for Op
+0000fe00: 7469 6d65 7472 6963 7320 6279 2041 6e73  timetrics by Ans
+0000fe10: 7973 2e0a 2020 2020 2222 220a 2020 2020  ys..    """.    
+0000fe20: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0000fe30: 662c 2064 6573 6967 6e29 3a0a 2020 2020  f, design):.    
+0000fe40: 2020 2020 7375 7065 7228 4f70 7469 6d65      super(Optime
+0000fe50: 7472 6963 732c 2073 656c 6629 2e5f 5f69  trics, self).__i
+0000fe60: 6e69 745f 5f28 290a 0a20 2020 2020 2020  nit__()..       
+0000fe70: 2073 656c 662e 6465 7369 676e 203d 2064   self.design = d
+0000fe80: 6573 6967 6e20 2023 2070 6172 656e 740a  esign  # parent.
+0000fe90: 2020 2020 2020 2020 7365 6c66 2e5f 6f70          self._op
+0000fea0: 7469 6d65 7472 6963 7320 3d20 7365 6c66  timetrics = self
+0000feb0: 2e64 6573 6967 6e2e 5f6f 7074 696d 6574  .design._optimet
+0000fec0: 7269 6373 2020 2320 3c43 4f4d 4f62 6a65  rics  # <COMObje
+0000fed0: 6374 2047 6574 4d6f 6475 6c65 3e0a 2020  ct GetModule>.  
+0000fee0: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+0000fef0: 5f6e 616d 6573 203d 204e 6f6e 650a 0a20  _names = None.. 
+0000ff00: 2020 2064 6566 2067 6574 5f73 6574 7570     def get_setup
+0000ff10: 5f6e 616d 6573 2873 656c 6629 3a0a 2020  _names(self):.  
+0000ff20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000ff30: 2020 5265 7475 726e 206c 6973 7420 6f66    Return list of
+0000ff40: 204f 7074 696d 6574 7269 6373 2073 6574   Optimetrics set
+0000ff50: 7570 206e 616d 6573 0a20 2020 2020 2020  up names.       
+0000ff60: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+0000ff70: 662e 7365 7475 705f 6e61 6d65 7320 3d20  f.setup_names = 
+0000ff80: 6c69 7374 2873 656c 662e 5f6f 7074 696d  list(self._optim
+0000ff90: 6574 7269 6373 2e47 6574 5365 7475 704e  etrics.GetSetupN
+0000ffa0: 616d 6573 2829 290a 2020 2020 2020 2020  ames()).        
+0000ffb0: 7265 7475 726e 2073 656c 662e 7365 7475  return self.setu
+0000ffc0: 705f 6e61 6d65 732e 636f 7079 2829 0a0a  p_names.copy()..
+0000ffd0: 2020 2020 6465 6620 736f 6c76 655f 7365      def solve_se
+0000ffe0: 7475 7028 7365 6c66 2c20 7365 7475 705f  tup(self, setup_
+0000fff0: 6e61 6d65 3a20 7374 7229 3a0a 2020 2020  name: str):.    
+00010000: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00010010: 536f 6c76 6573 2074 6865 2073 7065 6369  Solves the speci
+00010020: 6669 6564 204f 7074 696d 6574 7269 6373  fied Optimetrics
+00010030: 2073 6574 7570 2e0a 2020 2020 2020 2020   setup..        
+00010040: 436f 7272 6573 706f 6e64 7320 746f 3a20  Corresponds to: 
+00010050: 2052 6967 6874 2d63 6c69 636b 2074 6865   Right-click the
+00010060: 2073 6574 7570 2069 6e20 7468 6520 7072   setup in the pr
+00010070: 6f6a 6563 7420 7472 6565 2c20 616e 6420  oject tree, and 
+00010080: 7468 656e 2063 6c69 636b 0a20 2020 2020  then click.     
+00010090: 2020 2041 6e61 6c79 7a65 206f 6e20 7468     Analyze on th
+000100a0: 6520 7368 6f72 7463 7574 206d 656e 752e  e shortcut menu.
+000100b0: 0a0a 2020 2020 2020 2020 7365 7475 705f  ..        setup_
+000100c0: 6e61 6d65 2028 7374 7229 203a 206e 616d  name (str) : nam
+000100d0: 6520 6f66 2073 6574 7570 2c20 7368 6f75  e of setup, shou
+000100e0: 6c64 2062 6520 696e 2067 6574 5f73 6574  ld be in get_set
+000100f0: 7570 5f6e 616d 6573 0a0a 2020 2020 2020  up_names..      
+00010100: 2020 426c 6f63 6b73 2065 7865 6375 7469    Blocks executi
+00010110: 6f6e 2075 6e74 696c 2072 6561 6479 2074  on until ready t
+00010120: 6f20 7573 652e 0a0a 2020 2020 2020 2020  o use...        
+00010130: 4e6f 7465 2074 6861 7420 7468 6973 2072  Note that this r
+00010140: 6571 7569 7265 7320 7468 6520 6c69 6365  equires the lice
+00010150: 6e73 6520 666f 7220 4f70 7469 6d65 7472  nse for Optimetr
+00010160: 6963 7320 6279 2041 6e73 7973 2e0a 2020  ics by Ansys..  
+00010170: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010180: 2020 7265 7475 726e 2073 656c 662e 5f6f    return self._o
+00010190: 7074 696d 6574 7269 6373 2e53 6f6c 7665  ptimetrics.Solve
+000101a0: 5365 7475 7028 7365 7475 705f 6e61 6d65  Setup(setup_name
+000101b0: 290a 0a20 2020 2064 6566 2063 7265 6174  )..    def creat
+000101c0: 655f 7365 7475 7028 7365 6c66 2c0a 2020  e_setup(self,.  
+000101d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101e0: 2020 2076 6172 6961 626c 652c 0a20 2020     variable,.   
+000101f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010200: 2020 7377 705f 7061 7261 6d73 2c0a 2020    swp_params,.  
+00010210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010220: 2020 206e 616d 653d 2250 6172 616d 6574     name="Paramet
+00010230: 7269 6353 6574 7570 3122 2c0a 2020 2020  ricSetup1",.    
+00010240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010250: 2073 7770 5f74 7970 653d 276c 696e 6561   swp_type='linea
+00010260: 725f 7374 6570 272c 0a20 2020 2020 2020  r_step',.       
+00010270: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00010280: 7475 705f 6e61 6d65 3d4e 6f6e 652c 0a20  tup_name=None,. 
+00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102a0: 2020 2020 7361 7665 5f66 6965 6c64 733d      save_fields=
+000102b0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+000102c0: 2020 2020 2020 2020 2020 2063 6f70 795f             copy_
+000102d0: 6d65 7368 3d54 7275 652c 0a20 2020 2020  mesh=True,.     
+000102e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102f0: 736f 6c76 655f 7769 7468 5f63 6f70 6965  solve_with_copie
+00010300: 645f 6d65 7368 5f6f 6e6c 793d 5472 7565  d_mesh_only=True
 00010310: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010320: 2020 2020 2020 2073 6f6c 7665 5f77 6974         solve_wit
-00010330: 685f 636f 7069 6564 5f6d 6573 685f 6f6e  h_copied_mesh_on
-00010340: 6c79 3d54 7275 652c 0a20 2020 2020 2020  ly=True,.       
-00010350: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00010360: 7475 705f 7479 7065 3d27 7061 7261 6d65  tup_type='parame
-00010370: 7472 6963 2729 3a0a 2020 2020 2020 2020  tric'):.        
-00010380: 2222 220a 2020 2020 2020 2020 496e 7365  """.        Inse
-00010390: 7274 7320 6120 6e65 7720 7061 7261 6d65  rts a new parame
-000103a0: 7472 6963 2073 6574 7570 206f 6620 6f6e  tric setup of on
-000103b0: 6520 7661 7269 6162 6c65 2e20 4569 7468  e variable. Eith
-000103c0: 6572 2077 6974 6820 7377 6565 7020 0a20  er with sweep . 
-000103d0: 2020 2020 2020 2064 6566 696e 6974 696f         definitio
-000103e0: 6e20 6f72 2066 726f 6d20 6669 6c65 2e0a  n or from file..
-000103f0: 0a20 2020 2020 2020 2043 6f72 7265 7370  .        Corresp
-00010400: 6f6e 6473 2074 6f20 7569 2061 6363 6573  onds to ui acces
-00010410: 733a 0a20 2020 2020 2020 2052 6967 6874  s:.        Right
-00010420: 2d63 6c69 636b 2074 6865 204f 7074 696d  -click the Optim
-00010430: 6574 7269 6373 2066 6f6c 6465 7220 696e  etrics folder in
-00010440: 2074 6865 2070 726f 6a65 6374 2074 7265   the project tre
-00010450: 652c 2061 6e64 2074 6865 6e20 636c 6963  e, and then clic
-00010460: 6b20 0a20 2020 2020 2020 2041 6464 3e20  k .        Add> 
-00010470: 5061 7261 6d65 7472 6963 206f 6e20 7468  Parametric on th
-00010480: 6520 7368 6f72 7463 7574 206d 656e 752e  e shortcut menu.
-00010490: 0a0a 2020 2020 2020 2020 416e 7379 7320  ..        Ansys 
-000104a0: 7072 6f76 6964 6573 2073 6978 2073 7765  provides six swe
-000104b0: 6570 2064 6566 696e 6974 696f 6e73 2074  ep definitions t
-000104c0: 7970 6573 2073 7065 6369 6669 6564 2075  ypes specified u
-000104d0: 7369 6e67 2074 6865 2073 7770 5f74 7970  sing the swp_typ
-000104e0: 650a 2020 2020 2020 2020 7661 7269 6162  e.        variab
-000104f0: 6c65 2e0a 0a20 2020 2020 2020 2053 7765  le...        Swe
-00010500: 6570 2074 7970 6520 6465 6669 6e69 7469  ep type definiti
-00010510: 6f6e 733a 0a20 2020 2020 2020 202d 2027  ons:.        - '
-00010520: 7369 6e67 6c65 5f76 616c 7565 2720 2020  single_value'   
-00010530: 2020 2020 2020 2009 0a20 2020 2020 2020         ..       
-00010540: 2020 2020 2053 7065 6369 6679 2061 2073       Specify a s
-00010550: 696e 676c 6520 7661 6c75 6520 666f 7220  ingle value for 
-00010560: 7468 6520 7377 6565 7020 6465 6669 6e69  the sweep defini
-00010570: 7469 6f6e 2e0a 2020 2020 2020 2020 2d20  tion..        - 
-00010580: 276c 696e 6561 725f 7374 6570 270a 2020  'linear_step'.  
-00010590: 2020 2020 2020 2020 2020 5370 6563 6966            Specif
-000105a0: 7920 6120 6c69 6e65 6172 2072 616e 6765  y a linear range
-000105b0: 206f 6620 7661 6c75 6573 2077 6974 6820   of values with 
-000105c0: 6120 636f 6e73 7461 6e74 2073 7465 7020  a constant step 
-000105d0: 7369 7a65 2e0a 2020 2020 2020 2020 2d20  size..        - 
-000105e0: 276c 696e 6561 725f 636f 756e 7427 0a20  'linear_count'. 
-000105f0: 2020 2020 2020 2020 2020 2053 7065 6369             Speci
-00010600: 6679 2061 206c 696e 6561 7220 7261 6e67  fy a linear rang
-00010610: 6520 6f66 2076 616c 7565 7320 616e 6420  e of values and 
-00010620: 7468 6520 6e75 6d62 6572 2c20 6f72 2063  the number, or c
-00010630: 6f75 6e74 206f 6620 706f 696e 7473 0a20  ount of points. 
-00010640: 2020 2020 2020 2020 2020 2077 6974 6869             withi
-00010650: 6e20 7468 6973 2072 616e 6765 2e0a 2020  n this range..  
-00010660: 2020 2020 2020 2d20 2764 6563 6164 655f        - 'decade_
-00010670: 636f 756e 7427 0a20 2020 2020 2020 2020  count'.         
-00010680: 2020 2053 7065 6369 6679 2061 206c 6f67     Specify a log
-00010690: 6172 6974 686d 6963 2028 6261 7365 2031  arithmic (base 1
-000106a0: 3029 2073 6572 6965 7320 6f66 2076 616c  0) series of val
-000106b0: 7565 732c 2061 6e64 2074 6865 206e 756d  ues, and the num
-000106c0: 6265 7220 6f66 0a20 2020 2020 2020 2020  ber of.         
-000106d0: 2020 2076 616c 7565 7320 746f 2063 616c     values to cal
-000106e0: 6375 6c61 7465 2069 6e20 6561 6368 2064  culate in each d
-000106f0: 6563 6164 652e 0a20 2020 2020 2020 202d  ecade..        -
-00010700: 2027 6f63 7461 7665 5f63 6f75 6e74 270a   'octave_count'.
-00010710: 2020 2020 2020 2020 2020 2020 5370 6563              Spec
-00010720: 6966 7920 6120 6c6f 6761 7269 7468 6d69  ify a logarithmi
-00010730: 6320 2862 6173 6520 3229 2073 6572 6965  c (base 2) serie
-00010740: 7320 6f66 2076 616c 7565 732c 2061 6e64  s of values, and
-00010750: 2074 6865 206e 756d 6265 7220 6f66 200a   the number of .
-00010760: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
-00010770: 6573 2074 6f20 6361 6c63 756c 6174 6520  es to calculate 
-00010780: 696e 2065 6163 6820 6f63 7461 7665 2e0a  in each octave..
-00010790: 2020 2020 2020 2020 2d20 2765 7870 6f6e          - 'expon
-000107a0: 656e 7469 616c 5f63 6f75 6e74 270a 2020  ential_count'.  
-000107b0: 2020 2020 2020 2020 2020 5370 6563 6966            Specif
-000107c0: 7920 616e 2065 7870 6f6e 656e 7469 616c  y an exponential
-000107d0: 2028 6261 7365 2065 2920 7365 7269 6573   (base e) series
-000107e0: 206f 6620 7661 6c75 6573 2c20 616e 6420   of values, and 
-000107f0: 7468 6520 6e75 6d62 6572 206f 6620 0a20  the number of . 
-00010800: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00010810: 7320 746f 2063 616c 6375 6c61 7465 2e0a  s to calculate..
-00010820: 0a20 2020 2020 2020 2046 6f72 2073 7770  .        For swp
-00010830: 5f74 7970 653d 2773 696e 676c 655f 7661  _type='single_va
-00010840: 6c75 6527 2073 7770 5f70 6172 616d 7320  lue' swp_params 
-00010850: 6973 2074 6865 2073 696e 676c 6520 7661  is the single va
-00010860: 6c75 652e 0a0a 2020 2020 2020 2020 466f  lue...        Fo
-00010870: 7220 2073 7770 5f74 7970 653d 276c 696e  r  swp_type='lin
-00010880: 6561 725f 7374 6570 2720 7377 705f 7061  ear_step' swp_pa
-00010890: 7261 6d73 2069 7320 7374 6172 742c 2073  rams is start, s
-000108a0: 746f 702c 2073 7465 703a 0a20 2020 2020  top, step:.     
-000108b0: 2020 2020 2020 2073 7770 5f70 6172 616d         swp_param
-000108c0: 7320 3d20 2822 3132 2e38 6e48 222c 2022  s = ("12.8nH", "
-000108d0: 3133 2e36 6e48 222c 2022 302e 326e 4822  13.6nH", "0.2nH"
-000108e0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
-000108f0: 2020 2041 6c6c 206f 7468 6572 2074 7970     All other typ
-00010900: 6573 2073 7770 5f70 6172 616d 7320 6973  es swp_params is
-00010910: 2073 7461 7274 2c20 7374 6f70 2c20 636f   start, stop, co
-00010920: 756e 743a 0a20 2020 2020 2020 2020 2020  unt:.           
-00010930: 2073 7770 5f70 6172 616d 7320 3d20 2822   swp_params = ("
-00010940: 3132 2e38 6e48 222c 2022 3133 2e36 6e48  12.8nH", "13.6nH
-00010950: 222c 2034 290a 2020 2020 2020 2020 2020  ", 4).          
-00010960: 2020 5468 6520 6465 6669 6e69 7469 6f6e    The definition
-00010970: 206f 6620 636f 756e 7420 7661 7269 6573   of count varies
-00010980: 2061 6d6f 6e67 7374 2074 6865 2061 7661   amongst the ava
-00010990: 696c 6162 6c65 2074 7970 6573 2e20 0a0a  ilable types. ..
-000109a0: 2020 2020 2020 2020 466f 7220 4465 6361          For Deca
-000109b0: 6465 2063 6f75 6e74 2061 6e64 204f 6374  de count and Oct
-000109c0: 6176 6520 636f 756e 742c 2074 6865 2043  ave count, the C
-000109d0: 6f75 6e74 2076 616c 7565 2073 7065 6369  ount value speci
-000109e0: 6669 6573 2074 6865 206e 756d 6265 720a  fies the number.
-000109f0: 2020 2020 2020 2020 6f66 2070 6f69 6e74          of point
-00010a00: 7320 746f 2063 616c 6375 6c61 7465 2069  s to calculate i
-00010a10: 6e20 6576 6572 7920 6465 6361 6465 206f  n every decade o
-00010a20: 7220 6f63 7461 7665 2e20 466f 7220 4578  r octave. For Ex
-00010a30: 706f 6e65 6e74 6961 6c20 636f 756e 742c  ponential count,
-00010a40: 0a20 2020 2020 2020 2074 6865 2043 6f75  .        the Cou
-00010a50: 6e74 2076 616c 7565 2069 7320 7468 6520  nt value is the 
-00010a60: 746f 7461 6c20 6e75 6d62 6572 206f 6620  total number of 
-00010a70: 706f 696e 7473 2e20 5468 6520 746f 7461  points. The tota
-00010a80: 6c20 6e75 6d62 6572 206f 6620 0a20 2020  l number of .   
-00010a90: 2020 2020 2070 6f69 6e74 7320 696e 636c       points incl
-00010aa0: 7564 6573 2074 6865 2073 7461 7274 2061  udes the start a
-00010ab0: 6e64 2073 746f 7020 7661 6c75 6573 2e0a  nd stop values..
-00010ac0: 0a20 2020 2020 2020 2046 6f72 2070 6172  .        For par
-00010ad0: 616d 6574 7269 6320 6672 6f6d 2066 696c  ametric from fil
-00010ae0: 652c 2073 6574 7570 5f74 7970 653d 2770  e, setup_type='p
-00010af0: 6172 616d 6574 7269 635f 6669 6c65 272c  arametric_file',
-00010b00: 2070 6173 7320 696e 2061 2066 696c 650a   pass in a file.
-00010b10: 2020 2020 2020 2020 6e61 6d65 2061 6e64          name and
-00010b20: 2070 6174 6820 746f 2073 7770 5f70 6172   path to swp_par
-00010b30: 616d 7320 6c69 6b65 2022 433a 5c5c 7465  ams like "C:\\te
-00010b40: 7374 2e63 7376 2220 6f72 2022 433a 5c5c  st.csv" or "C:\\
-00010b50: 7465 7374 2e74 7874 2220 666f 7220 0a20  test.txt" for . 
-00010b60: 2020 2020 2020 2065 7861 6d70 6c65 2e0a         example..
-00010b70: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00010b80: 2063 7376 2066 6f72 6d61 7474 696e 673a   csv formatting:
-00010b90: 0a20 2020 2020 2020 202a 2c4c 6a5f 7175  .        *,Lj_qu
-00010ba0: 6269 740a 2020 2020 2020 2020 312c 3132  bit.        1,12
-00010bb0: 2e32 6e48 0a20 2020 2020 2020 2032 2c39  .2nH.        2,9
-00010bc0: 2e37 6e48 0a20 2020 2020 2020 2033 2c31  .7nH.        3,1
-00010bd0: 302e 326e 480a 0a20 2020 2020 2020 2053  0.2nH..        S
-00010be0: 6565 2041 6e73 7973 2064 6f63 756d 656e  ee Ansys documen
-00010bf0: 7461 7469 6f6e 2066 6f72 2061 6464 6974  tation for addit
-00010c00: 696f 6e61 6c20 666f 726d 6174 7469 6e67  ional formatting
-00010c10: 2069 6e73 7472 7563 7469 6f6e 732e 200a   instructions. .
-00010c20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010c30: 2020 2020 7365 7475 705f 6e61 6d65 203d      setup_name =
-00010c40: 2073 6574 7570 5f6e 616d 6520 6f72 2073   setup_name or s
-00010c50: 656c 662e 6465 7369 676e 2e67 6574 5f73  elf.design.get_s
-00010c60: 6574 7570 5f6e 616d 6573 2829 5b30 5d0a  etup_names()[0].
-00010c70: 2020 2020 2020 2020 7072 696e 7428 0a20          print(. 
-00010c80: 2020 2020 2020 2020 2020 2066 2249 6e73             f"Ins
-00010c90: 6572 7469 6e67 206f 7074 696d 6574 7269  erting optimetri
-00010ca0: 6373 2073 6574 7570 2060 7b6e 616d 657d  cs setup `{name}
-00010cb0: 6020 666f 7220 7369 6d75 6c61 7469 6f6e  ` for simulation
-00010cc0: 2073 6574 7570 3a20 607b 7365 7475 705f   setup: `{setup_
-00010cd0: 6e61 6d65 7d60 220a 2020 2020 2020 2020  name}`".        
-00010ce0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00010cf0: 7475 705f 7479 7065 203d 3d20 2770 6172  tup_type == 'par
-00010d00: 616d 6574 7269 6327 3a0a 2020 2020 2020  ametric':.      
-00010d10: 2020 2020 2020 7661 6c69 645f 7377 705f        valid_swp_
-00010d20: 7479 7065 7320 3d20 5b27 7369 6e67 6c65  types = ['single
-00010d30: 5f76 616c 7565 272c 2027 6c69 6e65 6172  _value', 'linear
-00010d40: 5f73 7465 7027 2c20 276c 696e 6561 725f  _step', 'linear_
-00010d50: 636f 756e 7427 2c20 0a20 2020 2020 2020  count', .       
-00010d60: 2020 2020 2027 6465 6361 6465 5f63 6f75       'decade_cou
-00010d70: 6e74 272c 2027 6f63 7461 7665 5f63 6f75  nt', 'octave_cou
-00010d80: 6e74 272c 2027 6578 706f 6e65 6e74 6961  nt', 'exponentia
-00010d90: 6c5f 636f 756e 7427 5d0a 0a20 2020 2020  l_count']..     
-00010da0: 2020 2020 2020 2069 6620 7377 705f 7479         if swp_ty
-00010db0: 7065 206e 6f74 2069 6e20 7661 6c69 645f  pe not in valid_
-00010dc0: 7377 705f 7479 7065 733a 0a20 2020 2020  swp_types:.     
-00010dd0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00010de0: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-00010df0: 7272 6f72 2829 0a20 2020 2020 2020 2020  rror().         
-00010e00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00010e10: 2020 2020 2020 2020 2069 6620 7377 705f           if swp_
-00010e20: 7479 7065 203d 3d20 2773 696e 676c 655f  type == 'single_
-00010e30: 7661 6c75 6527 3a0a 2020 2020 2020 2020  value':.        
-00010e40: 2020 2020 2020 2020 2020 2020 2320 5369              # Si
-00010e50: 6e67 6c65 2074 616b 6573 2073 7472 696e  ngle takes strin
-00010e60: 6720 6f66 2073 696e 676c 6520 7661 7269  g of single vari
-00010e70: 6162 6c65 206e 6f20 7377 705f 7479 7065  able no swp_type
-00010e80: 5f6e 616d 650a 2020 2020 2020 2020 2020  _name.          
-00010e90: 2020 2020 2020 2020 2020 7377 705f 7374            swp_st
-00010ea0: 7220 3d20 6622 7b73 7770 5f70 6172 616d  r = f"{swp_param
-00010eb0: 737d 220a 0a20 2020 2020 2020 2020 2020  s}"..           
-00010ec0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00010ed0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00010ee0: 2063 6f72 7265 6374 206e 756d 6265 7220   correct number 
-00010ef0: 6f66 2069 6e70 7574 730a 2020 2020 2020  of inputs.      
-00010f00: 2020 2020 2020 2020 2020 2020 2020 6173                as
-00010f10: 7365 7274 206c 656e 2873 7770 5f70 6172  sert len(swp_par
-00010f20: 616d 7329 203d 3d20 332c 2022 496e 636f  ams) == 3, "Inco
-00010f30: 7272 6563 7420 6e75 6d62 6572 206f 6620  rrect number of 
-00010f40: 7377 6565 7020 7061 7261 6d65 7465 7273  sweep parameters
-00010f50: 2e22 0a0a 2020 2020 2020 2020 2020 2020  ."..            
-00010f60: 2020 2020 2020 2020 2320 4e6f 7420 6368          # Not ch
-00010f70: 6563 6b69 6e67 2066 6f72 2063 6f6d 7061  ecking for compa
-00010f80: 7469 626c 6520 756e 6974 2074 7970 6573  tible unit types
-00010f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010fa0: 2020 2020 2069 6620 7377 705f 7479 7065       if swp_type
-00010fb0: 203d 3d20 276c 696e 6561 725f 7374 6570   == 'linear_step
-00010fc0: 273a 0a20 2020 2020 2020 2020 2020 2020  ':.             
-00010fd0: 2020 2020 2020 2020 2020 2073 7770 5f74             swp_t
-00010fe0: 7970 655f 6e61 6d65 203d 2022 4c49 4e22  ype_name = "LIN"
-00010ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011000: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011020: 2020 2023 2063 6f75 6e74 7320 6e65 6564     # counts need
-00011030: 7320 746f 2062 6520 616e 2069 6e74 6567  s to be an integ
-00011040: 6572 206e 756d 6265 720a 2020 2020 2020  er number.      
-00011050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011060: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-00011070: 6e63 6528 7377 705f 7061 7261 6d73 5b32  nce(swp_params[2
-00011080: 5d2c 2069 6e74 292c 2022 436f 756e 7420  ], int), "Count 
-00011090: 6d75 7374 2062 6520 696e 7465 6765 722e  must be integer.
-000110a0: 220a 0a20 2020 2020 2020 2020 2020 2020  "..             
-000110b0: 2020 2020 2020 2020 2020 2069 6620 7377             if sw
-000110c0: 705f 7479 7065 203d 3d20 276c 696e 6561  p_type == 'linea
-000110d0: 725f 636f 756e 7427 3a0a 2020 2020 2020  r_count':.      
-000110e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110f0: 2020 2020 2020 7377 705f 7479 7065 5f6e        swp_type_n
-00011100: 616d 6520 3d20 224c 494e 4322 0a20 2020  ame = "LINC".   
-00011110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011120: 2020 2020 2065 6c69 6620 7377 705f 7479       elif swp_ty
-00011130: 7065 203d 3d20 2764 6563 6164 655f 636f  pe == 'decade_co
-00011140: 756e 7427 3a0a 2020 2020 2020 2020 2020  unt':.          
-00011150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011160: 2020 7377 705f 7479 7065 5f6e 616d 6520    swp_type_name 
-00011170: 3d20 2244 4543 220a 2020 2020 2020 2020  = "DEC".        
-00011180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011190: 656c 6966 2073 7770 5f74 7970 6520 3d3d  elif swp_type ==
-000111a0: 2027 6f63 7461 7665 5f63 6f75 6e74 273a   'octave_count':
-000111b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000111c0: 2020 2020 2020 2020 2020 2020 2073 7770               swp
-000111d0: 5f74 7970 655f 6e61 6d65 203d 2022 4f43  _type_name = "OC
-000111e0: 5422 0a20 2020 2020 2020 2020 2020 2020  T".             
-000111f0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00011200: 7377 705f 7479 7065 203d 3d20 2765 7870  swp_type == 'exp
-00011210: 6f6e 656e 7469 616c 5f63 6f75 6e74 273a  onential_count':
-00011220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011230: 2020 2020 2020 2020 2020 2020 2073 7770               swp
-00011240: 5f74 7970 655f 6e61 6d65 203d 2022 4553  _type_name = "ES
-00011250: 5450 220a 0a20 2020 2020 2020 2020 2020  TP"..           
-00011260: 2020 2020 2020 2020 2023 2070 7265 7061           # prepa
-00011270: 7265 2074 6865 2073 7472 696e 6720 746f  re the string to
-00011280: 2070 6173 7320 746f 2041 6e73 7973 0a20   pass to Ansys. 
-00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112a0: 2020 2073 7770 5f73 7472 203d 2066 227b     swp_str = f"{
-000112b0: 7377 705f 7479 7065 5f6e 616d 657d 207b  swp_type_name} {
-000112c0: 7377 705f 7061 7261 6d73 5b30 5d7d 207b  swp_params[0]} {
-000112d0: 7377 705f 7061 7261 6d73 5b31 5d7d 207b  swp_params[1]} {
-000112e0: 7377 705f 7061 7261 6d73 5b32 5d7d 220a  swp_params[2]}".
-000112f0: 0a20 2020 2020 2020 2020 2020 2023 2074  .            # t
-00011300: 616c 6b20 7769 7468 2041 6e73 7973 0a20  alk with Ansys. 
-00011310: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00011320: 5f6f 7074 696d 6574 7269 6373 2e49 6e73  _optimetrics.Ins
-00011330: 6572 7453 6574 7570 2822 4f70 7469 5061  ertSetup("OptiPa
-00011340: 7261 6d65 7472 6963 222c 205b 0a20 2020  rametric", [.   
-00011350: 2020 2020 2020 2020 2020 2020 2066 224e               f"N
-00011360: 414d 453a 7b6e 616d 657d 222c 2022 4973  AME:{name}", "Is
-00011370: 456e 6162 6c65 643a 3d22 2c20 5472 7565  Enabled:=", True
-00011380: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011390: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000113a0: 2020 2020 2020 2020 224e 414d 453a 5072          "NAME:Pr
-000113b0: 6f64 4f70 7469 5365 7475 7044 6174 6156  odOptiSetupDataV
-000113c0: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
-000113d0: 2020 2020 2020 2020 2253 6176 6546 6965          "SaveFie
-000113e0: 6c64 733a 3d22 2c0a 2020 2020 2020 2020  lds:=",.        
-000113f0: 2020 2020 2020 2020 2020 2020 7361 7665              save
-00011400: 5f66 6965 6c64 732c 0a20 2020 2020 2020  _fields,.       
-00011410: 2020 2020 2020 2020 2020 2020 2022 436f               "Co
-00011420: 7079 4d65 7368 3a3d 222c 0a20 2020 2020  pyMesh:=",.     
-00011430: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00011440: 6f70 795f 6d65 7368 2c0a 2020 2020 2020  opy_mesh,.      
-00011450: 2020 2020 2020 2020 2020 2020 2020 2253                "S
-00011460: 6f6c 7665 5769 7468 436f 7069 6564 4d65  olveWithCopiedMe
-00011470: 7368 4f6e 6c79 3a3d 222c 0a20 2020 2020  shOnly:=",.     
-00011480: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00011490: 6f6c 7665 5f77 6974 685f 636f 7069 6564  olve_with_copied
-000114a0: 5f6d 6573 685f 6f6e 6c79 2c0a 2020 2020  _mesh_only,.    
-000114b0: 2020 2020 2020 2020 2020 2020 5d2c 205b              ], [
-000114c0: 224e 414d 453a 5374 6172 7469 6e67 506f  "NAME:StartingPo
-000114d0: 696e 7422 5d2c 2022 5369 6d2e 2053 6574  int"], "Sim. Set
-000114e0: 7570 733a 3d22 2c20 5b73 6574 7570 5f6e  ups:=", [setup_n
-000114f0: 616d 655d 2c0a 2020 2020 2020 2020 2020  ame],.          
-00011500: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
-00011510: 2020 2020 2020 2020 2020 2020 224e 414d              "NAM
-00011520: 453a 5377 6565 7073 222c 0a20 2020 2020  E:Sweeps",.     
-00011530: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00011540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011550: 2020 2020 2020 2020 2022 4e41 4d45 3a53           "NAME:S
-00011560: 7765 6570 4465 6669 6e69 7469 6f6e 222c  weepDefinition",
-00011570: 2022 5661 7269 6162 6c65 3a3d 222c 2076   "Variable:=", v
-00011580: 6172 6961 626c 652c 2022 4461 7461 3a3d  ariable, "Data:=
-00011590: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000115a0: 2020 2020 2020 2020 2020 2073 7770 5f73             swp_s
-000115b0: 7472 2c20 224f 6666 7365 7446 313a 3d22  tr, "OffsetF1:="
-000115c0: 2c20 4661 6c73 652c 2022 5379 6e63 6872  , False, "Synchr
-000115d0: 6f6e 697a 653a 3d22 2c20 300a 2020 2020  onize:=", 0.    
-000115e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115f0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00011600: 2020 5d2c 205b 224e 414d 453a 5377 6565    ], ["NAME:Swee
-00011610: 7020 4f70 6572 6174 696f 6e73 225d 2c20  p Operations"], 
-00011620: 5b22 4e41 4d45 3a47 6f61 6c73 225d 0a20  ["NAME:Goals"]. 
-00011630: 2020 2020 2020 2020 2020 205d 290a 2020             ]).  
-00011640: 2020 2020 2020 656c 6966 2073 6574 7570        elif setup
-00011650: 5f74 7970 6520 3d3d 2027 7061 7261 6d65  _type == 'parame
-00011660: 7472 6963 5f66 696c 6527 3a0a 2020 2020  tric_file':.    
-00011670: 2020 2020 2020 2020 2320 5573 6573 2074          # Uses t
-00011680: 6865 2066 696c 6520 6e61 6d65 2061 7320  he file name as 
-00011690: 7468 6520 7377 705f 7061 7261 6d73 200a  the swp_params .
-000116a0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-000116b0: 6e61 6d65 203d 2073 7770 5f70 6172 616d  name = swp_param
-000116c0: 730a 0a20 2020 2020 2020 2020 2020 2073  s..            s
-000116d0: 656c 662e 5f6f 7074 696d 6574 7269 6373  elf._optimetrics
-000116e0: 2e49 6d70 6f72 7453 6574 7570 2822 4f70  .ImportSetup("Op
-000116f0: 7469 5061 7261 6d65 7472 6963 222c 0a20  tiParametric",. 
-00011700: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00011710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011720: 2066 224e 414d 453a 7b6e 616d 657d 222c   f"NAME:{name}",
-00011730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011740: 2066 696c 656e 616d 652c 0a20 2020 2020   filename,.     
-00011750: 2020 2020 2020 2020 2020 205d 290a 2020             ]).  
-00011760: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-00011770: 6f70 7469 6d65 7472 6963 732e 4564 6974  optimetrics.Edit
-00011780: 5365 7475 7028 6622 7b6e 616d 657d 222c  Setup(f"{name}",
-00011790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000117a0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-000117b0: 2020 2020 2020 2066 224e 414d 453a 7b6e         f"NAME:{n
-000117c0: 616d 657d 222c 0a20 2020 2020 2020 2020  ame}",.         
-000117d0: 2020 2009 095b 0a20 2020 2020 2020 2020     ..[.         
-000117e0: 2020 2009 0909 224e 414d 453a 5072 6f64     ..."NAME:Prod
-000117f0: 4f70 7469 5365 7475 7044 6174 6156 3222  OptiSetupDataV2"
-00011800: 2c0a 2020 2020 2020 2020 2020 2020 0909  ,.            ..
-00011810: 0922 5361 7665 4669 656c 6473 3a3d 2209  ."SaveFields:=".
-00011820: 092c 2073 6176 655f 6669 656c 6473 2c0a  ., save_fields,.
-00011830: 2020 2020 2020 2020 2020 2020 0909 0922              ..."
-00011840: 436f 7079 4d65 7368 3a3d 2209 092c 2063  CopyMesh:=".., c
-00011850: 6f70 795f 6d65 7368 2c0a 2020 2020 2020  opy_mesh,.      
-00011860: 2020 2020 2020 0909 0922 536f 6c76 6557        ..."SolveW
-00011870: 6974 6843 6f70 6965 644d 6573 684f 6e6c  ithCopiedMeshOnl
-00011880: 793a 3d22 2c20 736f 6c76 655f 7769 7468  y:=", solve_with
-00011890: 5f63 6f70 6965 645f 6d65 7368 5f6f 6e6c  _copied_mesh_onl
-000118a0: 792c 0a20 2020 2020 2020 2020 2020 2009  y,.            .
-000118b0: 095d 2c0a 2020 2020 2020 2020 2020 2020  .],.            
-000118c0: 5d29 0a20 2020 2020 2020 2065 6c73 653a  ]).        else:
-000118d0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000118e0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
-000118f0: 6445 7272 6f72 2829 0a0a 0a63 6c61 7373  dError()...class
-00011900: 2048 6673 734d 6f64 656c 6572 2843 4f4d   HfssModeler(COM
-00011910: 5772 6170 7065 7229 3a0a 2020 2020 6465  Wrapper):.    de
-00011920: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00011930: 2064 6573 6967 6e2c 206d 6f64 656c 6572   design, modeler
-00011940: 2c20 626f 756e 6461 7269 6573 2c20 6d65  , boundaries, me
-00011950: 7368 293a 0a20 2020 2020 2020 2022 2222  sh):.        """
-00011960: 0a20 2020 2020 2020 203a 7479 7065 2064  .        :type d
-00011970: 6573 6967 6e3a 2048 6673 7344 6573 6967  esign: HfssDesig
-00011980: 6e0a 2020 2020 2020 2020 2222 220a 2020  n.        """.  
-00011990: 2020 2020 2020 7375 7065 7228 4866 7373        super(Hfss
-000119a0: 4d6f 6465 6c65 722c 2073 656c 6629 2e5f  Modeler, self)._
-000119b0: 5f69 6e69 745f 5f28 290a 2020 2020 2020  _init__().      
-000119c0: 2020 7365 6c66 2e70 6172 656e 7420 3d20    self.parent = 
-000119d0: 6465 7369 676e 0a20 2020 2020 2020 2073  design.        s
-000119e0: 656c 662e 5f6d 6f64 656c 6572 203d 206d  elf._modeler = m
-000119f0: 6f64 656c 6572 0a20 2020 2020 2020 2073  odeler.        s
-00011a00: 656c 662e 5f62 6f75 6e64 6172 6965 7320  elf._boundaries 
-00011a10: 3d20 626f 756e 6461 7269 6573 0a20 2020  = boundaries.   
-00011a20: 2020 2020 2073 656c 662e 5f6d 6573 6820       self._mesh 
-00011a30: 3d20 6d65 7368 2020 2320 4d65 7368 206d  = mesh  # Mesh m
-00011a40: 6f64 756c 650a 0a20 2020 2064 6566 2073  odule..    def s
-00011a50: 6574 5f75 6e69 7473 2873 656c 662c 2075  et_units(self, u
-00011a60: 6e69 7473 2c20 7265 7363 616c 653d 5472  nits, rescale=Tr
-00011a70: 7565 293a 0a20 2020 2020 2020 2073 656c  ue):.        sel
-00011a80: 662e 5f6d 6f64 656c 6572 2e53 6574 4d6f  f._modeler.SetMo
-00011a90: 6465 6c55 6e69 7473 280a 2020 2020 2020  delUnits(.      
-00011aa0: 2020 2020 2020 5b22 4e41 4d45 3a55 6e69        ["NAME:Uni
-00011ab0: 7473 2050 6172 616d 6574 6572 222c 2022  ts Parameter", "
-00011ac0: 556e 6974 733a 3d22 2c20 756e 6974 732c  Units:=", units,
-00011ad0: 2022 5265 7363 616c 653a 3d22 2c20 7265   "Rescale:=", re
-00011ae0: 7363 616c 655d 290a 0a20 2020 2064 6566  scale])..    def
-00011af0: 2067 6574 5f75 6e69 7473 2873 656c 6629   get_units(self)
-00011b00: 3a0a 2020 2020 2020 2020 2222 2247 6574  :.        """Get
-00011b10: 2074 6865 206d 6f64 656c 2075 6e69 7473   the model units
-00011b20: 2e0a 2020 2020 2020 2020 2020 2020 5265  ..            Re
-00011b30: 7475 726e 2056 616c 7565 3a20 2020 2041  turn Value:    A
-00011b40: 2073 7472 696e 6720 636f 6e74 6169 6e73   string contains
-00011b50: 2063 7572 7265 6e74 206d 6f64 656c 2075   current model u
-00011b60: 6e69 7473 2e20 2222 220a 2020 2020 2020  nits. """.      
-00011b70: 2020 7265 7475 726e 2073 7472 2873 656c    return str(sel
-00011b80: 662e 5f6d 6f64 656c 6572 2e47 6574 4d6f  f._modeler.GetMo
-00011b90: 6465 6c55 6e69 7473 2829 290a 0a20 2020  delUnits())..   
-00011ba0: 2064 6566 2067 6574 5f61 6c6c 5f70 726f   def get_all_pro
-00011bb0: 7065 7274 6965 7328 7365 6c66 2c20 6f62  perties(self, ob
-00011bc0: 6a5f 6e61 6d65 2c20 5072 6f70 5461 623d  j_name, PropTab=
-00011bd0: 2747 656f 6d65 7472 7933 4441 7474 7269  'Geometry3DAttri
-00011be0: 6275 7465 5461 6227 293a 0a20 2020 2020  buteTab'):.     
-00011bf0: 2020 2027 2727 0a20 2020 2020 2020 2020     '''.         
-00011c00: 2020 2047 6574 2061 6c6c 2070 726f 7065     Get all prope
-00011c10: 7274 6965 7320 666f 7220 6d6f 6465 6c65  rties for modele
-00011c20: 7220 5072 6f70 5461 622c 2050 726f 7053  r PropTab, PropS
-00011c30: 6572 7665 720a 2020 2020 2020 2020 2727  erver.        ''
-00011c40: 270a 2020 2020 2020 2020 5072 6f70 5365  '.        PropSe
-00011c50: 7276 6572 203d 206f 626a 5f6e 616d 650a  rver = obj_name.
-00011c60: 2020 2020 2020 2020 7072 6f70 6572 7469          properti
-00011c70: 6573 203d 207b 7d0a 2020 2020 2020 2020  es = {}.        
-00011c80: 666f 7220 6b65 7920 696e 2073 656c 662e  for key in self.
-00011c90: 5f6d 6f64 656c 6572 2e47 6574 5072 6f70  _modeler.GetProp
-00011ca0: 6572 7469 6573 2850 726f 7054 6162 2c20  erties(PropTab, 
-00011cb0: 5072 6f70 5365 7276 6572 293a 0a20 2020  PropServer):.   
-00011cc0: 2020 2020 2020 2020 2070 726f 7065 7274           propert
-00011cd0: 6965 735b 6b65 795d 203d 2073 656c 662e  ies[key] = self.
-00011ce0: 5f6d 6f64 656c 6572 2e47 6574 5072 6f70  _modeler.GetProp
-00011cf0: 6572 7479 5661 6c75 6528 0a20 2020 2020  ertyValue(.     
-00011d00: 2020 2020 2020 2020 2020 2050 726f 7054             PropT
-00011d10: 6162 2c20 5072 6f70 5365 7276 6572 2c20  ab, PropServer, 
-00011d20: 6b65 7929 0a20 2020 2020 2020 2072 6574  key).        ret
-00011d30: 7572 6e20 7072 6f70 6572 7469 6573 0a0a  urn properties..
-00011d40: 2020 2020 6465 6620 5f61 7474 7269 6275      def _attribu
-00011d50: 7465 735f 6172 7261 7928 0a20 2020 2020  tes_array(.     
-00011d60: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-00011d70: 2020 2020 2020 2020 206e 616d 653d 4e6f           name=No
-00011d80: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00011d90: 6e6f 6e6d 6f64 656c 3d46 616c 7365 2c0a  nonmodel=False,.
-00011da0: 2020 2020 2020 2020 2020 2020 7769 7265              wire
-00011db0: 6672 616d 653d 4661 6c73 652c 0a20 2020  frame=False,.   
-00011dc0: 2020 2020 2020 2020 2063 6f6c 6f72 3d4e           color=N
-00011dd0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00011de0: 2074 7261 6e73 7061 7265 6e63 793d 302e   transparency=0.
-00011df0: 392c 0a20 2020 2020 2020 2020 2020 206d  9,.            m
-00011e00: 6174 6572 6961 6c3d 4e6f 6e65 2c20 2023  aterial=None,  #
-00011e10: 2073 7472 0a20 2020 2020 2020 2020 2020   str.           
-00011e20: 2073 6f6c 7665 5f69 6e73 6964 653d 4e6f   solve_inside=No
-00011e30: 6e65 2c20 2023 2062 6f6f 6c0a 2020 2020  ne,  # bool.    
-00011e40: 2020 2020 2020 2020 636f 6f72 6469 6e61          coordina
-00011e50: 7465 5f73 7973 7465 6d3d 2247 6c6f 6261  te_system="Globa
-00011e60: 6c22 293a 0a20 2020 2020 2020 2061 7272  l"):.        arr
-00011e70: 203d 205b 224e 414d 453a 4174 7472 6962   = ["NAME:Attrib
-00011e80: 7574 6573 222c 2022 5061 7274 436f 6f72  utes", "PartCoor
-00011e90: 6469 6e61 7465 5379 7374 656d 3a3d 222c  dinateSystem:=",
-00011ea0: 2063 6f6f 7264 696e 6174 655f 7379 7374   coordinate_syst
-00011eb0: 656d 5d0a 2020 2020 2020 2020 6966 206e  em].        if n
-00011ec0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-00011ed0: 0a20 2020 2020 2020 2020 2020 2061 7272  .            arr
-00011ee0: 2e65 7874 656e 6428 5b22 4e61 6d65 3a3d  .extend(["Name:=
-00011ef0: 222c 206e 616d 655d 290a 0a20 2020 2020  ", name])..     
-00011f00: 2020 2069 6620 6e6f 6e6d 6f64 656c 206f     if nonmodel o
-00011f10: 7220 7769 7265 6672 616d 653a 0a20 2020  r wireframe:.   
-00011f20: 2020 2020 2020 2020 2066 6c61 6773 203d           flags =
-00011f30: 2027 4e6f 6e4d 6f64 656c 2720 6966 206e   'NonModel' if n
-00011f40: 6f6e 6d6f 6465 6c20 656c 7365 2027 2720  onmodel else '' 
-00011f50: 2023 2063 616e 2062 6520 646f 6e65 2073   # can be done s
-00011f60: 6d61 7274 6572 0a20 2020 2020 2020 2020  marter.         
-00011f70: 2020 2069 6620 7769 7265 6672 616d 653a     if wireframe:
-00011f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011f90: 2066 6c61 6773 202b 3d20 2723 2720 6966   flags += '#' if
-00011fa0: 206c 656e 2866 6c61 6773 2920 3e20 3020   len(flags) > 0 
-00011fb0: 656c 7365 2027 270a 2020 2020 2020 2020  else ''.        
-00011fc0: 2020 2020 2020 2020 666c 6167 7320 2b3d          flags +=
-00011fd0: 2027 5769 7265 6672 616d 6527 0a20 2020   'Wireframe'.   
-00011fe0: 2020 2020 2020 2020 2061 7272 2e65 7874           arr.ext
-00011ff0: 656e 6428 5b22 466c 6167 733a 3d22 2c20  end(["Flags:=", 
-00012000: 666c 6167 735d 290a 0a20 2020 2020 2020  flags])..       
-00012010: 2069 6620 636f 6c6f 7220 6973 206e 6f74   if color is not
-00012020: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00012030: 2020 2061 7272 2e65 7874 656e 6428 5b22     arr.extend(["
-00012040: 436f 6c6f 723a 3d22 2c20 2228 2564 2025  Color:=", "(%d %
-00012050: 6420 2564 2922 2025 2063 6f6c 6f72 5d29  d %d)" % color])
-00012060: 0a20 2020 2020 2020 2069 6620 7472 616e  .        if tran
-00012070: 7370 6172 656e 6379 2069 7320 6e6f 7420  sparency is not 
-00012080: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00012090: 2020 6172 722e 6578 7465 6e64 285b 2254    arr.extend(["T
-000120a0: 7261 6e73 7061 7265 6e63 793a 3d22 2c20  ransparency:=", 
-000120b0: 7472 616e 7370 6172 656e 6379 5d29 0a20  transparency]). 
-000120c0: 2020 2020 2020 2069 6620 6d61 7465 7269         if materi
-000120d0: 616c 2069 7320 6e6f 7420 4e6f 6e65 3a0a  al is not None:.
-000120e0: 2020 2020 2020 2020 2020 2020 6172 722e              arr.
-000120f0: 6578 7465 6e64 285b 224d 6174 6572 6961  extend(["Materia
-00012100: 6c4e 616d 653a 3d22 2c20 6d61 7465 7269  lName:=", materi
-00012110: 616c 5d29 0a20 2020 2020 2020 2069 6620  al]).        if 
-00012120: 736f 6c76 655f 696e 7369 6465 2069 7320  solve_inside is 
-00012130: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00012140: 2020 2020 2020 6172 722e 6578 7465 6e64        arr.extend
-00012150: 285b 2253 6f6c 7665 496e 7369 6465 3a3d  (["SolveInside:=
-00012160: 222c 2073 6f6c 7665 5f69 6e73 6964 655d  ", solve_inside]
-00012170: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00012180: 6e20 6172 720a 0a20 2020 2064 6566 205f  n arr..    def _
-00012190: 7365 6c65 6374 696f 6e73 5f61 7272 6179  selections_array
-000121a0: 2873 656c 662c 202a 6e61 6d65 7329 3a0a  (self, *names):.
-000121b0: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-000121c0: 224e 414d 453a 5365 6c65 6374 696f 6e73  "NAME:Selections
-000121d0: 222c 2022 5365 6c65 6374 696f 6e73 3a3d  ", "Selections:=
-000121e0: 222c 2022 2c22 2e6a 6f69 6e28 6e61 6d65  ", ",".join(name
-000121f0: 7329 5d0a 0a20 2020 2064 6566 206d 6573  s)]..    def mes
-00012200: 685f 6c65 6e67 7468 2873 656c 662c 0a20  h_length(self,. 
-00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012220: 2020 206e 616d 655f 6d65 7368 2c0a 2020     name_mesh,.  
-00012230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012240: 2020 6f62 6a65 6374 733a 206c 6973 742c    objects: list,
-00012250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012260: 2020 2020 204d 6178 4c65 6e67 7468 3d27       MaxLength='
-00012270: 302e 316d 6d27 2c0a 2020 2020 2020 2020  0.1mm',.        
-00012280: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
-00012290: 6172 6773 293a 0a20 2020 2020 2020 2027  args):.        '
-000122a0: 2727 0a20 2020 2020 2020 2022 5265 6669  ''.        "Refi
-000122b0: 6e65 496e 7369 6465 3a3d 2209 2c20 4661  neInside:="., Fa
-000122c0: 6c73 652c 0a20 2020 2020 2020 2022 456e  lse,.        "En
-000122d0: 6162 6c65 643a 3d22 0909 2c20 5472 7565  abled:=".., True
-000122e0: 2c0a 2020 2020 2020 2020 2252 6573 7472  ,.        "Restr
-000122f0: 6963 7445 6c65 6d3a 3d22 092c 2046 616c  ictElem:="., Fal
-00012300: 7365 2c0a 2020 2020 2020 2020 224e 756d  se,.        "Num
-00012310: 4d61 7845 6c65 6d3a 3d22 0909 2c20 2231  MaxElem:=".., "1
-00012320: 3030 3022 2c0a 2020 2020 2020 2020 2252  000",.        "R
-00012330: 6573 7472 6963 744c 656e 6774 683a 3d22  estrictLength:="
-00012340: 092c 2054 7275 652c 0a20 2020 2020 2020  ., True,.       
-00012350: 2022 4d61 784c 656e 6774 683a 3d22 0909   "MaxLength:="..
-00012360: 2c20 2230 2e31 6d6d 220a 0a20 2020 2020  , "0.1mm"..     
-00012370: 2020 2045 7861 6d70 6c65 2075 7365 3a0a     Example use:.
-00012380: 2020 2020 2020 2020 6d6f 6465 6c65 722e          modeler.
-00012390: 6173 7369 676e 5f6d 6573 685f 6c65 6e67  assign_mesh_leng
-000123a0: 7468 2827 6d65 7368 3227 2c20 5b22 5131  th('mesh2', ["Q1
-000123b0: 5f6d 6573 6822 5d2c 204d 6178 4c65 6e67  _mesh"], MaxLeng
-000123c0: 7468 3d30 2e31 290a 2020 2020 2020 2020  th=0.1).        
-000123d0: 2727 270a 2020 2020 2020 2020 6173 7365  '''.        asse
-000123e0: 7274 2069 7369 6e73 7461 6e63 6528 6f62  rt isinstance(ob
-000123f0: 6a65 6374 732c 206c 6973 7429 0a0a 2020  jects, list)..  
-00012400: 2020 2020 2020 6172 7220 3d20 5b0a 2020        arr = [.  
-00012410: 2020 2020 2020 2020 2020 6622 4e41 4d45            f"NAME
-00012420: 3a7b 6e61 6d65 5f6d 6573 687d 222c 2022  :{name_mesh}", "
-00012430: 4f62 6a65 6374 733a 3d22 2c20 6f62 6a65  Objects:=", obje
-00012440: 6374 732c 2027 4d61 784c 656e 6774 683a  cts, 'MaxLength:
-00012450: 3d27 2c20 4d61 784c 656e 6774 680a 2020  =', MaxLength.  
-00012460: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00012470: 6f70 7320 3d20 5b0a 2020 2020 2020 2020  ops = [.        
-00012480: 2020 2020 2752 6566 696e 6549 6e73 6964      'RefineInsid
-00012490: 6527 2c20 2745 6e61 626c 6564 272c 2027  e', 'Enabled', '
-000124a0: 5265 7374 7269 6374 456c 656d 272c 2027  RestrictElem', '
-000124b0: 4e75 6d4d 6178 456c 656d 272c 0a20 2020  NumMaxElem',.   
-000124c0: 2020 2020 2020 2020 2027 5265 7374 7269           'Restri
-000124d0: 6374 4c65 6e67 7468 270a 2020 2020 2020  ctLength'.      
-000124e0: 2020 5d0a 2020 2020 2020 2020 666f 7220    ].        for 
-000124f0: 6b65 792c 2076 616c 2069 6e20 6b77 6172  key, val in kwar
-00012500: 6773 2e69 7465 6d73 2829 3a0a 2020 2020  gs.items():.    
-00012510: 2020 2020 2020 2020 6966 206b 6579 2069          if key i
-00012520: 6e20 6f70 733a 0a20 2020 2020 2020 2020  n ops:.         
-00012530: 2020 2020 2020 2061 7272 202b 3d20 5b6b         arr += [k
-00012540: 6579 202b 2027 3a3d 272c 2073 7472 2876  ey + ':=', str(v
-00012550: 616c 295d 0a20 2020 2020 2020 2020 2020  al)].           
-00012560: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00012570: 2020 2020 2020 206c 6f67 6765 722e 6572         logger.er
-00012580: 726f 7228 274b 4559 2060 7b6b 6579 7d60  ror('KEY `{key}`
-00012590: 204e 4f54 2049 4e20 6f70 7321 2729 0a0a   NOT IN ops!')..
-000125a0: 2020 2020 2020 2020 7365 6c66 2e5f 6d65          self._me
-000125b0: 7368 2e41 7373 6967 6e4c 656e 6774 684f  sh.AssignLengthO
-000125c0: 7028 6172 7229 0a0a 2020 2020 6465 6620  p(arr)..    def 
-000125d0: 6d65 7368 5f72 6561 7373 6967 6e28 7365  mesh_reassign(se
-000125e0: 6c66 2c20 6e61 6d65 5f6d 6573 682c 206f  lf, name_mesh, o
-000125f0: 626a 6563 7473 3a20 6c69 7374 293a 0a20  bjects: list):. 
-00012600: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
-00012610: 696e 7374 616e 6365 286f 626a 6563 7473  instance(objects
-00012620: 2c20 6c69 7374 290a 2020 2020 2020 2020  , list).        
-00012630: 7365 6c66 2e5f 6d65 7368 2e52 6561 7373  self._mesh.Reass
-00012640: 6967 6e4f 7028 6e61 6d65 5f6d 6573 682c  ignOp(name_mesh,
-00012650: 205b 224f 626a 6563 7473 3a3d 222c 206f   ["Objects:=", o
-00012660: 626a 6563 7473 5d29 0a0a 2020 2020 6465  bjects])..    de
-00012670: 6620 6d65 7368 5f67 6574 5f6e 616d 6573  f mesh_get_names
-00012680: 2873 656c 662c 206b 696e 643d 224c 656e  (self, kind="Len
-00012690: 6774 6820 4261 7365 6422 293a 0a20 2020  gth Based"):.   
-000126a0: 2020 2020 2027 2727 2022 4c65 6e67 7468       ''' "Length
-000126b0: 2042 6173 6564 222c 2022 536b 696e 2044   Based", "Skin D
-000126c0: 6570 7468 2042 6173 6564 222c 202e 2e2e  epth Based", ...
-000126d0: 2727 270a 2020 2020 2020 2020 7265 7475  '''.        retu
-000126e0: 726e 206c 6973 7428 7365 6c66 2e5f 6d65  rn list(self._me
-000126f0: 7368 2e47 6574 4f70 6572 6174 696f 6e4e  sh.GetOperationN
-00012700: 616d 6573 286b 696e 6429 290a 0a20 2020  ames(kind))..   
-00012710: 2064 6566 206d 6573 685f 6765 745f 616c   def mesh_get_al
-00012720: 6c5f 7072 6f70 7328 7365 6c66 2c20 6d65  l_props(self, me
-00012730: 7368 5f6e 616d 6529 3a0a 2020 2020 2020  sh_name):.      
-00012740: 2020 2320 544f 444f 3a20 6d61 6b65 206d    # TODO: make m
-00012750: 6573 6820 7469 7320 6f77 6e20 2063 6c61  esh tis own  cla
-00012760: 7373 2077 6974 6820 7072 6f70 6572 7469  ss with properti
-00012770: 6573 0a20 2020 2020 2020 2070 726f 705f  es.        prop_
-00012780: 7461 6220 3d20 274d 6573 6853 6574 7570  tab = 'MeshSetup
-00012790: 5461 6227 0a20 2020 2020 2020 2070 726f  Tab'.        pro
-000127a0: 705f 7365 7276 6572 203d 2066 274d 6573  p_server = f'Mes
-000127b0: 6853 6574 7570 3a7b 6d65 7368 5f6e 616d  hSetup:{mesh_nam
-000127c0: 657d 270a 2020 2020 2020 2020 7072 6f70  e}'.        prop
-000127d0: 5f6e 616d 6573 203d 2073 656c 662e 7061  _names = self.pa
-000127e0: 7265 6e74 2e5f 6465 7369 676e 2e47 6574  rent._design.Get
-000127f0: 5072 6f70 6572 7469 6573 2827 4d65 7368  Properties('Mesh
-00012800: 5365 7475 7054 6162 272c 0a20 2020 2020  SetupTab',.     
-00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012840: 2020 7072 6f70 5f73 6572 7665 7229 0a20    prop_server). 
-00012850: 2020 2020 2020 2064 6963 203d 207b 7d0a         dic = {}.
-00012860: 2020 2020 2020 2020 666f 7220 6e61 6d65          for name
-00012870: 2069 6e20 7072 6f70 5f6e 616d 6573 3a0a   in prop_names:.
-00012880: 2020 2020 2020 2020 2020 2020 6469 635b              dic[
-00012890: 6e61 6d65 5d20 3d20 7365 6c66 2e5f 6d6f  name] = self._mo
-000128a0: 6465 6c65 722e 4765 7450 726f 7065 7274  deler.GetPropert
-000128b0: 7956 616c 7565 2870 726f 705f 7461 622c  yValue(prop_tab,
-000128c0: 2070 726f 705f 7365 7276 6572 2c0a 2020   prop_server,.  
-000128d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012900: 2020 2020 206e 616d 6529 0a20 2020 2020       name).     
-00012910: 2020 2072 6574 7572 6e20 6469 630a 0a20     return dic.. 
-00012920: 2020 2064 6566 2064 7261 775f 626f 785f     def draw_box_
-00012930: 636f 726e 6572 2873 656c 662c 2070 6f73  corner(self, pos
-00012940: 2c20 7369 7a65 2c20 2a2a 6b77 6172 6773  , size, **kwargs
-00012950: 293a 0a20 2020 2020 2020 206e 616d 6520  ):.        name 
-00012960: 3d20 7365 6c66 2e5f 6d6f 6465 6c65 722e  = self._modeler.
-00012970: 4372 6561 7465 426f 7828 5b0a 2020 2020  CreateBox([.    
-00012980: 2020 2020 2020 2020 224e 414d 453a 426f          "NAME:Bo
-00012990: 7850 6172 616d 6574 6572 7322 2c20 2258  xParameters", "X
-000129a0: 506f 7369 7469 6f6e 3a3d 222c 0a20 2020  Position:=",.   
-000129b0: 2020 2020 2020 2020 2073 7472 2870 6f73           str(pos
-000129c0: 5b30 5d29 2c20 2259 506f 7369 7469 6f6e  [0]), "YPosition
-000129d0: 3a3d 222c 0a20 2020 2020 2020 2020 2020  :=",.           
-000129e0: 2073 7472 2870 6f73 5b31 5d29 2c20 225a   str(pos[1]), "Z
-000129f0: 506f 7369 7469 6f6e 3a3d 222c 0a20 2020  Position:=",.   
-00012a00: 2020 2020 2020 2020 2073 7472 2870 6f73           str(pos
-00012a10: 5b32 5d29 2c20 2258 5369 7a65 3a3d 222c  [2]), "XSize:=",
-00012a20: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00012a30: 2873 697a 655b 305d 292c 2022 5953 697a  (size[0]), "YSiz
-00012a40: 653a 3d22 2c0a 2020 2020 2020 2020 2020  e:=",.          
-00012a50: 2020 7374 7228 7369 7a65 5b31 5d29 2c20    str(size[1]), 
-00012a60: 225a 5369 7a65 3a3d 222c 0a20 2020 2020  "ZSize:=",.     
-00012a70: 2020 2020 2020 2073 7472 2873 697a 655b         str(size[
-00012a80: 325d 290a 2020 2020 2020 2020 5d2c 2073  2]).        ], s
-00012a90: 656c 662e 5f61 7474 7269 6275 7465 735f  elf._attributes_
-00012aa0: 6172 7261 7928 2a2a 6b77 6172 6773 2929  array(**kwargs))
-00012ab0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012ac0: 426f 7828 6e61 6d65 2c20 7365 6c66 2c20  Box(name, self, 
-00012ad0: 706f 732c 2073 697a 6529 0a0a 2020 2020  pos, size)..    
-00012ae0: 6465 6620 6472 6177 5f62 6f78 5f63 656e  def draw_box_cen
-00012af0: 7465 7228 7365 6c66 2c20 706f 732c 2073  ter(self, pos, s
-00012b00: 697a 652c 202a 2a6b 7761 7267 7329 3a0a  ize, **kwargs):.
-00012b10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012b20: 2020 2020 4372 6561 7465 7320 6120 332d      Creates a 3-
-00012b30: 4420 626f 7820 6365 6e74 6572 6564 2061  D box centered a
-00012b40: 7420 706f 7320 5b78 302c 2079 302c 207a  t pos [x0, y0, z
-00012b50: 305d 2c20 7769 7468 2077 6964 7468 0a20  0], with width. 
-00012b60: 2020 2020 2020 2073 697a 6520 5b78 7769         size [xwi
-00012b70: 6474 682c 2079 7769 6474 682c 207a 7769  dth, ywidth, zwi
-00012b80: 6474 685d 2061 6c6f 6e67 2065 6163 6820  dth] along each 
-00012b90: 7265 7370 6563 7469 7665 2064 6972 6563  respective direc
-00012ba0: 7469 6f6e 2e0a 0a20 2020 2020 2020 2041  tion...        A
-00012bb0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00012bc0: 2070 6f73 2028 6c69 7374 293a 2043 6f6f   pos (list): Coo
-00012bd0: 7264 696e 6174 6573 206f 6620 6365 6e74  rdinates of cent
-00012be0: 6572 206f 6620 626f 782c 205b 7830 2c20  er of box, [x0, 
-00012bf0: 7930 2c20 7a30 5d0a 2020 2020 2020 2020  y0, z0].        
-00012c00: 2020 2020 7369 7a65 2028 6c69 7374 293a      size (list):
-00012c10: 2057 6964 7468 206f 6620 626f 7820 616c   Width of box al
-00012c20: 6f6e 6720 6561 6368 2064 6972 6563 7469  ong each directi
-00012c30: 6f6e 2c20 5b78 7769 6474 682c 2079 7769  on, [xwidth, ywi
-00012c40: 6474 682c 207a 7769 6474 685d 0a20 2020  dth, zwidth].   
-00012c50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012c60: 2063 6f72 6e65 725f 706f 7320 3d20 5b76   corner_pos = [v
-00012c70: 6172 2870 2920 2d20 7661 7228 7329 202f  ar(p) - var(s) /
-00012c80: 2032 2066 6f72 2070 2c20 7320 696e 207a   2 for p, s in z
-00012c90: 6970 2870 6f73 2c20 7369 7a65 295d 0a20  ip(pos, size)]. 
-00012ca0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00012cb0: 6c66 2e64 7261 775f 626f 785f 636f 726e  lf.draw_box_corn
-00012cc0: 6572 2863 6f72 6e65 725f 706f 732c 2073  er(corner_pos, s
-00012cd0: 697a 652c 202a 2a6b 7761 7267 7329 0a0a  ize, **kwargs)..
-00012ce0: 2020 2020 6465 6620 6472 6177 5f70 6f6c      def draw_pol
-00012cf0: 796c 696e 6528 7365 6c66 2c20 706f 696e  yline(self, poin
-00012d00: 7473 2c20 636c 6f73 6564 3d54 7275 652c  ts, closed=True,
-00012d10: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00012d20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012d30: 4472 6177 7320 6120 636c 6f73 6564 206f  Draws a closed o
-00012d40: 7220 6f70 656e 2070 6f6c 796c 696e 652e  r open polyline.
-00012d50: 0a20 2020 2020 2020 2049 6620 636c 6f73  .        If clos
-00012d60: 6564 203d 2054 7275 652c 2074 6865 6e20  ed = True, then 
-00012d70: 7769 6c6c 206d 616b 6520 696e 746f 2061  will make into a
-00012d80: 2073 6865 6574 2e0a 2020 2020 2020 2020   sheet..        
-00012d90: 706f 696e 7473 203a 206e 6565 6420 746f  points : need to
-00012da0: 2062 6520 696e 2074 6865 2063 6f72 7265   be in the corre
-00012db0: 6374 2075 6e69 7473 0a0a 2020 2020 2020  ct units..      
-00012dc0: 2020 466f 7220 6f70 7469 6f6e 616c 2061    For optional a
-00012dd0: 7267 756d 656e 7473 2c20 7365 6520 5f61  rguments, see _a
-00012de0: 7474 7269 6275 7465 735f 6172 7261 793b  ttributes_array;
-00012df0: 2074 6865 7365 2069 6e63 6c75 6465 3a0a   these include:.
-00012e00: 2020 2020 2020 2020 6060 600a 2020 2020          ```.    
-00012e10: 2020 2020 2020 2020 6e6f 6e6d 6f64 656c          nonmodel
-00012e20: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00012e30: 2020 2020 7769 7265 6672 616d 653d 4661      wireframe=Fa
-00012e40: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00012e50: 2063 6f6c 6f72 3d4e 6f6e 652c 0a20 2020   color=None,.   
-00012e60: 2020 2020 2020 2020 2074 7261 6e73 7061           transpa
-00012e70: 7265 6e63 793d 302e 392c 0a20 2020 2020  rency=0.9,.     
-00012e80: 2020 2020 2020 206d 6174 6572 6961 6c3d         material=
-00012e90: 4e6f 6e65 2c20 2023 2073 7472 0a20 2020  None,  # str.   
-00012ea0: 2020 2020 2020 2020 2073 6f6c 7665 5f69           solve_i
-00012eb0: 6e73 6964 653d 4e6f 6e65 2c20 2023 2062  nside=None,  # b
-00012ec0: 6f6f 6c0a 2020 2020 2020 2020 2020 2020  ool.            
-00012ed0: 636f 6f72 6469 6e61 7465 5f73 7973 7465  coordinate_syste
-00012ee0: 6d3d 2247 6c6f 6261 6c22 0a20 2020 2020  m="Global".     
-00012ef0: 2020 2060 6060 0a20 2020 2020 2020 2022     ```.        "
-00012f00: 2222 0a20 2020 2020 2020 2070 6f69 6e74  "".        point
-00012f10: 7353 7472 203d 205b 224e 414d 453a 506f  sStr = ["NAME:Po
-00012f20: 6c79 6c69 6e65 506f 696e 7473 225d 0a20  lylinePoints"]. 
-00012f30: 2020 2020 2020 2069 6e64 6578 7353 7472         indexsStr
-00012f40: 203d 205b 224e 414d 453a 506f 6c79 6c69   = ["NAME:Polyli
-00012f50: 6e65 5365 676d 656e 7473 225d 0a20 2020  neSegments"].   
-00012f60: 2020 2020 2066 6f72 2069 692c 2070 6f69       for ii, poi
-00012f70: 6e74 2069 6e20 656e 756d 6572 6174 6528  nt in enumerate(
-00012f80: 706f 696e 7473 293a 0a20 2020 2020 2020  points):.       
-00012f90: 2020 2020 2070 6f69 6e74 7353 7472 2e61       pointsStr.a
-00012fa0: 7070 656e 6428 5b0a 2020 2020 2020 2020  ppend([.        
-00012fb0: 2020 2020 2020 2020 224e 414d 453a 504c          "NAME:PL
-00012fc0: 506f 696e 7422 2c20 2258 3a3d 222c 0a20  Point", "X:=",. 
-00012fd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012fe0: 7472 2870 6f69 6e74 5b30 5d29 2c20 2259  tr(point[0]), "Y
-00012ff0: 3a3d 222c 0a20 2020 2020 2020 2020 2020  :=",.           
-00013000: 2020 2020 2073 7472 2870 6f69 6e74 5b31       str(point[1
-00013010: 5d29 2c20 225a 3a3d 222c 0a20 2020 2020  ]), "Z:=",.     
-00013020: 2020 2020 2020 2020 2020 2073 7472 2870             str(p
-00013030: 6f69 6e74 5b32 5d29 0a20 2020 2020 2020  oint[2]).       
-00013040: 2020 2020 205d 290a 2020 2020 2020 2020       ]).        
-00013050: 2020 2020 696e 6465 7873 5374 722e 6170      indexsStr.ap
-00013060: 7065 6e64 285b 0a20 2020 2020 2020 2020  pend([.         
-00013070: 2020 2020 2020 2022 4e41 4d45 3a50 4c53         "NAME:PLS
-00013080: 6567 6d65 6e74 222c 2022 5365 676d 656e  egment", "Segmen
-00013090: 7454 7970 653a 3d22 2c20 224c 696e 6522  tType:=", "Line"
-000130a0: 2c20 2253 7461 7274 496e 6465 783a 3d22  , "StartIndex:="
-000130b0: 2c20 6969 2c0a 2020 2020 2020 2020 2020  , ii,.          
-000130c0: 2020 2020 2020 224e 6f4f 6650 6f69 6e74        "NoOfPoint
-000130d0: 733a 3d22 2c20 320a 2020 2020 2020 2020  s:=", 2.        
-000130e0: 2020 2020 5d29 0a20 2020 2020 2020 2069      ]).        i
-000130f0: 6620 636c 6f73 6564 3a0a 2020 2020 2020  f closed:.      
-00013100: 2020 2020 2020 706f 696e 7473 5374 722e        pointsStr.
-00013110: 6170 7065 6e64 285b 0a20 2020 2020 2020  append([.       
-00013120: 2020 2020 2020 2020 2022 4e41 4d45 3a50           "NAME:P
-00013130: 4c50 6f69 6e74 222c 2022 583a 3d22 2c0a  LPoint", "X:=",.
-00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013150: 7374 7228 706f 696e 7473 5b30 5d5b 305d  str(points[0][0]
-00013160: 292c 2022 593a 3d22 2c0a 2020 2020 2020  ), "Y:=",.      
-00013170: 2020 2020 2020 2020 2020 7374 7228 706f            str(po
-00013180: 696e 7473 5b30 5d5b 315d 292c 2022 5a3a  ints[0][1]), "Z:
-00013190: 3d22 2c0a 2020 2020 2020 2020 2020 2020  =",.            
-000131a0: 2020 2020 7374 7228 706f 696e 7473 5b30      str(points[0
-000131b0: 5d5b 325d 290a 2020 2020 2020 2020 2020  ][2]).          
-000131c0: 2020 5d29 0a20 2020 2020 2020 2020 2020    ]).           
-000131d0: 2070 6172 616d 735f 636c 6f73 6564 203d   params_closed =
-000131e0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-000131f0: 2020 2022 4973 506f 6c79 6c69 6e65 436f     "IsPolylineCo
-00013200: 7665 7265 643a 3d22 2c20 5472 7565 2c20  vered:=", True, 
-00013210: 2249 7350 6f6c 796c 696e 6543 6c6f 7365  "IsPolylineClose
-00013220: 643a 3d22 2c20 5472 7565 0a20 2020 2020  d:=", True.     
-00013230: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00013240: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00013250: 2020 2069 6e64 6578 7353 7472 203d 2069     indexsStr = i
-00013260: 6e64 6578 7353 7472 5b3a 2d31 5d0a 2020  ndexsStr[:-1].  
-00013270: 2020 2020 2020 2020 2020 7061 7261 6d73            params
-00013280: 5f63 6c6f 7365 6420 3d20 5b0a 2020 2020  _closed = [.    
-00013290: 2020 2020 2020 2020 2020 2020 2249 7350              "IsP
-000132a0: 6f6c 796c 696e 6543 6f76 6572 6564 3a3d  olylineCovered:=
-000132b0: 222c 2054 7275 652c 2022 4973 506f 6c79  ", True, "IsPoly
-000132c0: 6c69 6e65 436c 6f73 6564 3a3d 222c 2046  lineClosed:=", F
-000132d0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-000132e0: 205d 0a0a 2020 2020 2020 2020 6e61 6d65   ]..        name
-000132f0: 203d 2073 656c 662e 5f6d 6f64 656c 6572   = self._modeler
-00013300: 2e43 7265 6174 6550 6f6c 796c 696e 6528  .CreatePolyline(
-00013310: 0a20 2020 2020 2020 2020 2020 205b 224e  .            ["N
-00013320: 414d 453a 506f 6c79 6c69 6e65 5061 7261  AME:PolylinePara
-00013330: 6d65 7465 7273 222c 202a 7061 7261 6d73  meters", *params
-00013340: 5f63 6c6f 7365 642c 2070 6f69 6e74 7353  _closed, pointsS
-00013350: 7472 2c20 696e 6465 7873 5374 725d 2c0a  tr, indexsStr],.
-00013360: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013370: 2e5f 6174 7472 6962 7574 6573 5f61 7272  ._attributes_arr
-00013380: 6179 282a 2a6b 7761 7267 7329 290a 0a20  ay(**kwargs)).. 
-00013390: 2020 2020 2020 2069 6620 636c 6f73 6564         if closed
-000133a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000133b0: 7475 726e 2050 6f6c 796c 696e 6528 6e61  turn Polyline(na
-000133c0: 6d65 2c20 7365 6c66 2c20 706f 696e 7473  me, self, points
-000133d0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-000133e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000133f0: 726e 204f 7065 6e50 6f6c 796c 696e 6528  rn OpenPolyline(
-00013400: 6e61 6d65 2c20 7365 6c66 2c20 706f 696e  name, self, poin
-00013410: 7473 290a 0a20 2020 2064 6566 2064 7261  ts)..    def dra
-00013420: 775f 7265 6374 5f63 6f72 6e65 7228 7365  w_rect_corner(se
-00013430: 6c66 2c20 706f 732c 2078 5f73 697a 653d  lf, pos, x_size=
-00013440: 302c 2079 5f73 697a 653d 302c 207a 5f73  0, y_size=0, z_s
-00013450: 697a 653d 302c 202a 2a6b 7761 7267 7329  ize=0, **kwargs)
-00013460: 3a0a 2020 2020 2020 2020 7369 7a65 203d  :.        size =
-00013470: 205b 785f 7369 7a65 2c20 795f 7369 7a65   [x_size, y_size
-00013480: 2c20 7a5f 7369 7a65 5d0a 2020 2020 2020  , z_size].      
-00013490: 2020 6173 7365 7274 2030 2069 6e20 7369    assert 0 in si
-000134a0: 7a65 0a20 2020 2020 2020 2061 7869 7320  ze.        axis 
-000134b0: 3d20 2258 595a 225b 7369 7a65 2e69 6e64  = "XYZ"[size.ind
-000134c0: 6578 2830 295d 0a20 2020 2020 2020 2077  ex(0)].        w
-000134d0: 5f69 6478 2c20 685f 6964 7820 3d20 7b27  _idx, h_idx = {'
-000134e0: 5827 3a20 2831 2c20 3229 2c20 2759 273a  X': (1, 2), 'Y':
-000134f0: 2028 322c 2030 292c 2027 5a27 3a20 2830   (2, 0), 'Z': (0
-00013500: 2c20 3129 7d5b 6178 6973 5d0a 0a20 2020  , 1)}[axis]..   
-00013510: 2020 2020 206e 616d 6520 3d20 7365 6c66       name = self
-00013520: 2e5f 6d6f 6465 6c65 722e 4372 6561 7465  ._modeler.Create
-00013530: 5265 6374 616e 676c 6528 5b0a 2020 2020  Rectangle([.    
-00013540: 2020 2020 2020 2020 224e 414d 453a 5265          "NAME:Re
-00013550: 6374 616e 676c 6550 6172 616d 6574 6572  ctangleParameter
-00013560: 7322 2c20 2258 5374 6172 743a 3d22 2c0a  s", "XStart:=",.
-00013570: 2020 2020 2020 2020 2020 2020 7374 7228              str(
-00013580: 706f 735b 305d 292c 2022 5953 7461 7274  pos[0]), "YStart
-00013590: 3a3d 222c 0a20 2020 2020 2020 2020 2020  :=",.           
-000135a0: 2073 7472 2870 6f73 5b31 5d29 2c20 225a   str(pos[1]), "Z
-000135b0: 5374 6172 743a 3d22 2c0a 2020 2020 2020  Start:=",.      
-000135c0: 2020 2020 2020 7374 7228 706f 735b 325d        str(pos[2]
-000135d0: 292c 2022 5769 6474 683a 3d22 2c0a 2020  ), "Width:=",.  
-000135e0: 2020 2020 2020 2020 2020 7374 7228 7369            str(si
-000135f0: 7a65 5b77 5f69 6478 5d29 2c20 2248 6569  ze[w_idx]), "Hei
-00013600: 6768 743a 3d22 2c0a 2020 2020 2020 2020  ght:=",.        
-00013610: 2020 2020 7374 7228 7369 7a65 5b68 5f69      str(size[h_i
-00013620: 6478 5d29 2c20 2257 6869 6368 4178 6973  dx]), "WhichAxis
-00013630: 3a3d 222c 2061 7869 730a 2020 2020 2020  :=", axis.      
-00013640: 2020 5d2c 2073 656c 662e 5f61 7474 7269    ], self._attri
-00013650: 6275 7465 735f 6172 7261 7928 2a2a 6b77  butes_array(**kw
-00013660: 6172 6773 2929 0a20 2020 2020 2020 2072  args)).        r
-00013670: 6574 7572 6e20 5265 6374 286e 616d 652c  eturn Rect(name,
-00013680: 2073 656c 662c 2070 6f73 2c20 7369 7a65   self, pos, size
-00013690: 290a 0a20 2020 2064 6566 2064 7261 775f  )..    def draw_
-000136a0: 7265 6374 5f63 656e 7465 7228 7365 6c66  rect_center(self
-000136b0: 2c20 706f 732c 2078 5f73 697a 653d 302c  , pos, x_size=0,
-000136c0: 2079 5f73 697a 653d 302c 207a 5f73 697a   y_size=0, z_siz
-000136d0: 653d 302c 202a 2a6b 7761 7267 7329 3a0a  e=0, **kwargs):.
-000136e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000136f0: 2020 2020 4372 6561 7465 7320 6120 7265      Creates a re
-00013700: 6374 616e 676c 6520 6365 6e74 6572 6564  ctangle centered
-00013710: 2061 7420 706f 7320 5b78 302c 2079 302c   at pos [x0, y0,
-00013720: 207a 305d 2e0a 2020 2020 2020 2020 4974   z0]..        It
-00013730: 2069 7320 6173 7375 6d65 6420 7468 6174   is assumed that
-00013740: 2074 6865 2072 6563 7461 6e67 6c65 206c   the rectangle l
-00013750: 6965 7320 7061 7261 6c6c 656c 2074 6f20  ies parallel to 
-00013760: 7468 6520 7879 2c20 797a 2c20 6f72 2078  the xy, yz, or x
-00013770: 7a20 706c 616e 652e 0a20 2020 2020 2020  z plane..       
-00013780: 2055 7365 7220 696e 7075 7473 2032 206f   User inputs 2 o
-00013790: 6620 3320 6f66 2074 6865 2066 6f6c 6c6f  f 3 of the follo
-000137a0: 7769 6e67 3a20 785f 7369 7a65 2c20 795f  wing: x_size, y_
-000137b0: 7369 7a65 2c20 616e 6420 7a5f 7369 7a65  size, and z_size
-000137c0: 0a20 2020 2020 2020 2064 6570 656e 6469  .        dependi
-000137d0: 6e67 206f 6e20 686f 7720 7468 6520 7265  ng on how the re
-000137e0: 6374 616e 676c 6520 6973 206f 7269 656e  ctangle is orien
-000137f0: 7465 642e 0a0a 2020 2020 2020 2020 4172  ted...        Ar
-00013800: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00013810: 706f 7320 286c 6973 7429 3a20 436f 6f72  pos (list): Coor
-00013820: 6469 6e61 7465 7320 6f66 2072 6563 7461  dinates of recta
-00013830: 6e67 6c65 2063 656e 7465 722c 205b 7830  ngle center, [x0
-00013840: 2c20 7930 2c20 7a30 5d0a 2020 2020 2020  , y0, z0].      
-00013850: 2020 2020 2020 785f 7369 7a65 2028 696e        x_size (in
-00013860: 742c 206f 7074 696f 6e61 6c29 3a20 5769  t, optional): Wi
-00013870: 6474 6820 616c 6f6e 6720 7468 6520 7820  dth along the x 
-00013880: 6469 7265 6374 696f 6e2e 2044 6566 6175  direction. Defau
-00013890: 6c74 7320 746f 2030 2e0a 2020 2020 2020  lts to 0..      
-000138a0: 2020 2020 2020 795f 7369 7a65 2028 696e        y_size (in
-000138b0: 742c 206f 7074 696f 6e61 6c29 3a20 2057  t, optional):  W
-000138c0: 6964 7468 2061 6c6f 6e67 2074 6865 2079  idth along the y
-000138d0: 2064 6972 6563 7469 6f6e 2e20 4465 6661   direction. Defa
-000138e0: 756c 7473 2074 6f20 302e 0a20 2020 2020  ults to 0..     
-000138f0: 2020 2020 2020 207a 5f73 697a 6520 2869         z_size (i
-00013900: 6e74 2c20 6f70 7469 6f6e 616c 293a 2020  nt, optional):  
-00013910: 5769 6474 6820 616c 6f6e 6720 7468 6520  Width along the 
-00013920: 7a20 6469 7265 6374 696f 6e5d 2e20 4465  z direction]. De
-00013930: 6661 756c 7473 2074 6f20 302e 0a20 2020  faults to 0..   
-00013940: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013950: 2063 6f72 6e65 725f 706f 7320 3d20 5b0a   corner_pos = [.
-00013960: 2020 2020 2020 2020 2020 2020 7661 7228              var(
-00013970: 7029 202d 2076 6172 2873 2920 2f20 322e  p) - var(s) / 2.
-00013980: 2066 6f72 2070 2c20 7320 696e 207a 6970   for p, s in zip
-00013990: 2870 6f73 2c20 5b78 5f73 697a 652c 2079  (pos, [x_size, y
-000139a0: 5f73 697a 652c 207a 5f73 697a 655d 290a  _size, z_size]).
-000139b0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000139c0: 2020 7265 7475 726e 2073 656c 662e 6472    return self.dr
-000139d0: 6177 5f72 6563 745f 636f 726e 6572 2863  aw_rect_corner(c
-000139e0: 6f72 6e65 725f 706f 732c 2078 5f73 697a  orner_pos, x_siz
-000139f0: 652c 2079 5f73 697a 652c 207a 5f73 697a  e, y_size, z_siz
-00013a00: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00013a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013a20: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-00013a30: 290a 0a20 2020 2064 6566 2064 7261 775f  )..    def draw_
-00013a40: 6379 6c69 6e64 6572 2873 656c 662c 2070  cylinder(self, p
-00013a50: 6f73 2c20 7261 6469 7573 2c20 6865 6967  os, radius, heig
-00013a60: 6874 2c20 6178 6973 2c20 2a2a 6b77 6172  ht, axis, **kwar
-00013a70: 6773 293a 0a20 2020 2020 2020 2061 7373  gs):.        ass
-00013a80: 6572 7420 6178 6973 2069 6e20 2258 595a  ert axis in "XYZ
-00013a90: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00013aa0: 2073 656c 662e 5f6d 6f64 656c 6572 2e43   self._modeler.C
-00013ab0: 7265 6174 6543 796c 696e 6465 7228 5b0a  reateCylinder([.
-00013ac0: 2020 2020 2020 2020 2020 2020 224e 414d              "NAM
-00013ad0: 453a 4379 6c69 6e64 6572 5061 7261 6d65  E:CylinderParame
-00013ae0: 7465 7273 222c 2022 5843 656e 7465 723a  ters", "XCenter:
-00013af0: 3d22 2c20 706f 735b 305d 2c20 2259 4365  =", pos[0], "YCe
-00013b00: 6e74 6572 3a3d 222c 0a20 2020 2020 2020  nter:=",.       
-00013b10: 2020 2020 2070 6f73 5b31 5d2c 2022 5a43       pos[1], "ZC
-00013b20: 656e 7465 723a 3d22 2c20 706f 735b 325d  enter:=", pos[2]
-00013b30: 2c20 2252 6164 6975 733a 3d22 2c20 7261  , "Radius:=", ra
-00013b40: 6469 7573 2c20 2248 6569 6768 743a 3d22  dius, "Height:="
-00013b50: 2c0a 2020 2020 2020 2020 2020 2020 6865  ,.            he
-00013b60: 6967 6874 2c20 2257 6869 6368 4178 6973  ight, "WhichAxis
-00013b70: 3a3d 222c 2061 7869 732c 2022 4e75 6d53  :=", axis, "NumS
-00013b80: 6964 6573 3a3d 222c 2030 0a20 2020 2020  ides:=", 0.     
-00013b90: 2020 205d 2c20 7365 6c66 2e5f 6174 7472     ], self._attr
-00013ba0: 6962 7574 6573 5f61 7272 6179 282a 2a6b  ibutes_array(**k
-00013bb0: 7761 7267 7329 290a 0a20 2020 2064 6566  wargs))..    def
-00013bc0: 2064 7261 775f 6379 6c69 6e64 6572 5f63   draw_cylinder_c
-00013bd0: 656e 7465 7228 7365 6c66 2c20 706f 732c  enter(self, pos,
-00013be0: 2072 6164 6975 732c 2068 6569 6768 742c   radius, height,
-00013bf0: 2061 7869 732c 202a 2a6b 7761 7267 7329   axis, **kwargs)
-00013c00: 3a0a 2020 2020 2020 2020 6178 6973 5f69  :.        axis_i
-00013c10: 6478 203d 205b 2258 222c 2022 5922 2c20  dx = ["X", "Y", 
-00013c20: 225a 225d 2e69 6e64 6578 2861 7869 7329  "Z"].index(axis)
-00013c30: 0a20 2020 2020 2020 2065 6467 655f 706f  .        edge_po
-00013c40: 7320 3d20 636f 7079 2870 6f73 290a 2020  s = copy(pos).  
-00013c50: 2020 2020 2020 6564 6765 5f70 6f73 5b61        edge_pos[a
-00013c60: 7869 735f 6964 785d 203d 2076 6172 2870  xis_idx] = var(p
-00013c70: 6f73 5b61 7869 735f 6964 785d 2920 2d20  os[axis_idx]) - 
-00013c80: 7661 7228 6865 6967 6874 2920 2f20 320a  var(height) / 2.
-00013c90: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00013ca0: 656c 662e 6472 6177 5f63 796c 696e 6465  elf.draw_cylinde
-00013cb0: 7228 6564 6765 5f70 6f73 2c20 7261 6469  r(edge_pos, radi
-00013cc0: 7573 2c20 6865 6967 6874 2c20 6178 6973  us, height, axis
-00013cd0: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
-00013ce0: 2064 6566 2064 7261 775f 7769 7265 626f   def draw_wirebo
-00013cf0: 6e64 2873 656c 662c 0a20 2020 2020 2020  nd(self,.       
-00013d00: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00013d10: 6f73 2c0a 2020 2020 2020 2020 2020 2020  os,.            
-00013d20: 2020 2020 2020 2020 2020 6f72 692c 0a20            ori,. 
+00010320: 2020 2020 2020 2073 6574 7570 5f74 7970         setup_typ
+00010330: 653d 2770 6172 616d 6574 7269 6327 293a  e='parametric'):
+00010340: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010350: 2020 2020 2049 6e73 6572 7473 2061 206e       Inserts a n
+00010360: 6577 2070 6172 616d 6574 7269 6320 7365  ew parametric se
+00010370: 7475 7020 6f66 206f 6e65 2076 6172 6961  tup of one varia
+00010380: 626c 652e 2045 6974 6865 7220 7769 7468  ble. Either with
+00010390: 2073 7765 6570 0a20 2020 2020 2020 2064   sweep.        d
+000103a0: 6566 696e 6974 696f 6e20 6f72 2066 726f  efinition or fro
+000103b0: 6d20 6669 6c65 2e0a 2020 2020 2020 2020  m file..        
+000103c0: 0a20 2020 2020 2020 202a 5379 6e63 6872  .        *Synchr
+000103d0: 6f6e 697a 6564 2a20 7377 6565 7073 2028  onized* sweeps (
+000103e0: 6d6f 7265 2074 6861 6e20 6f6e 6520 7661  more than one va
+000103f0: 7269 6162 6c65 2063 6861 6e67 696e 6720  riable changing 
+00010400: 6174 206f 6e63 6529 0a20 2020 2020 2020  at once).       
+00010410: 2063 616e 2062 6520 696d 706c 656d 656e   can be implemen
+00010420: 7465 6420 6279 2067 6976 696e 6720 6120  ted by giving a 
+00010430: 6c69 7374 206f 6620 7661 7269 6162 6c65  list of variable
+00010440: 7320 746f 2060 6076 6172 6961 626c 6560  s to ``variable`
+00010450: 600a 2020 2020 2020 2020 616e 6420 636f  `.        and co
+00010460: 7272 6573 706f 6e64 696e 6720 6c69 7374  rresponding list
+00010470: 7320 746f 2060 6073 7770 5f70 6172 616d  s to ``swp_param
+00010480: 7360 6020 616e 6420 6060 7377 705f 7479  s`` and ``swp_ty
+00010490: 7065 6060 2e0a 2020 2020 2020 2020 5468  pe``..        Th
+000104a0: 6520 6c65 6e67 7468 7320 6f66 2074 6865  e lengths of the
+000104b0: 2073 7765 6570 2074 7970 6573 2073 686f   sweep types sho
+000104c0: 756c 6420 6d61 7463 6820 2865 7863 6c75  uld match (exclu
+000104d0: 6469 6e67 2073 696e 676c 6520 7661 6c75  ding single valu
+000104e0: 6529 2e0a 0a20 2020 2020 2020 2043 6f72  e)...        Cor
+000104f0: 7265 7370 6f6e 6473 2074 6f20 7569 2061  responds to ui a
+00010500: 6363 6573 733a 0a20 2020 2020 2020 2052  ccess:.        R
+00010510: 6967 6874 2d63 6c69 636b 2074 6865 204f  ight-click the O
+00010520: 7074 696d 6574 7269 6373 2066 6f6c 6465  ptimetrics folde
+00010530: 7220 696e 2074 6865 2070 726f 6a65 6374  r in the project
+00010540: 2074 7265 652c 2061 6e64 2074 6865 6e20   tree, and then 
+00010550: 636c 6963 6b0a 2020 2020 2020 2020 4164  click.        Ad
+00010560: 643e 2050 6172 616d 6574 7269 6320 6f6e  d> Parametric on
+00010570: 2074 6865 2073 686f 7274 6375 7420 6d65   the shortcut me
+00010580: 6e75 2e0a 0a20 2020 2020 2020 2041 6e73  nu...        Ans
+00010590: 7973 2070 726f 7669 6465 7320 7369 7820  ys provides six 
+000105a0: 7377 6565 7020 6465 6669 6e69 7469 6f6e  sweep definition
+000105b0: 7320 7479 7065 7320 7370 6563 6966 6965  s types specifie
+000105c0: 6420 7573 696e 6720 7468 6520 7377 705f  d using the swp_
+000105d0: 7479 7065 0a20 2020 2020 2020 2076 6172  type.        var
+000105e0: 6961 626c 652e 0a0a 2020 2020 2020 2020  iable...        
+000105f0: 5377 6565 7020 7479 7065 2064 6566 696e  Sweep type defin
+00010600: 6974 696f 6e73 3a0a 0a20 2020 2020 2020  itions:..       
+00010610: 202d 2027 7369 6e67 6c65 5f76 616c 7565   - 'single_value
+00010620: 270a 2020 2020 2020 2020 2020 2020 5370  '.            Sp
+00010630: 6563 6966 7920 6120 7369 6e67 6c65 2076  ecify a single v
+00010640: 616c 7565 2066 6f72 2074 6865 2073 7765  alue for the swe
+00010650: 6570 2064 6566 696e 6974 696f 6e2e 0a20  ep definition.. 
+00010660: 2020 2020 2020 202d 2027 6c69 6e65 6172         - 'linear
+00010670: 5f73 7465 7027 0a20 2020 2020 2020 2020  _step'.         
+00010680: 2020 2053 7065 6369 6679 2061 206c 696e     Specify a lin
+00010690: 6561 7220 7261 6e67 6520 6f66 2076 616c  ear range of val
+000106a0: 7565 7320 7769 7468 2061 2063 6f6e 7374  ues with a const
+000106b0: 616e 7420 7374 6570 2073 697a 652e 0a20  ant step size.. 
+000106c0: 2020 2020 2020 202d 2027 6c69 6e65 6172         - 'linear
+000106d0: 5f63 6f75 6e74 270a 2020 2020 2020 2020  _count'.        
+000106e0: 2020 2020 5370 6563 6966 7920 6120 6c69      Specify a li
+000106f0: 6e65 6172 2072 616e 6765 206f 6620 7661  near range of va
+00010700: 6c75 6573 2061 6e64 2074 6865 206e 756d  lues and the num
+00010710: 6265 722c 206f 7220 636f 756e 7420 6f66  ber, or count of
+00010720: 2070 6f69 6e74 730a 2020 2020 2020 2020   points.        
+00010730: 2020 2020 7769 7468 696e 2074 6869 7320      within this 
+00010740: 7261 6e67 652e 0a20 2020 2020 2020 202d  range..        -
+00010750: 2027 6465 6361 6465 5f63 6f75 6e74 270a   'decade_count'.
+00010760: 2020 2020 2020 2020 2020 2020 5370 6563              Spec
+00010770: 6966 7920 6120 6c6f 6761 7269 7468 6d69  ify a logarithmi
+00010780: 6320 2862 6173 6520 3130 2920 7365 7269  c (base 10) seri
+00010790: 6573 206f 6620 7661 6c75 6573 2c20 616e  es of values, an
+000107a0: 6420 7468 6520 6e75 6d62 6572 206f 660a  d the number of.
+000107b0: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+000107c0: 6573 2074 6f20 6361 6c63 756c 6174 6520  es to calculate 
+000107d0: 696e 2065 6163 6820 6465 6361 6465 2e0a  in each decade..
+000107e0: 2020 2020 2020 2020 2d20 276f 6374 6176          - 'octav
+000107f0: 655f 636f 756e 7427 0a20 2020 2020 2020  e_count'.       
+00010800: 2020 2020 2053 7065 6369 6679 2061 206c       Specify a l
+00010810: 6f67 6172 6974 686d 6963 2028 6261 7365  ogarithmic (base
+00010820: 2032 2920 7365 7269 6573 206f 6620 7661   2) series of va
+00010830: 6c75 6573 2c20 616e 6420 7468 6520 6e75  lues, and the nu
+00010840: 6d62 6572 206f 660a 2020 2020 2020 2020  mber of.        
+00010850: 2020 2020 7661 6c75 6573 2074 6f20 6361      values to ca
+00010860: 6c63 756c 6174 6520 696e 2065 6163 6820  lculate in each 
+00010870: 6f63 7461 7665 2e0a 2020 2020 2020 2020  octave..        
+00010880: 2d20 2765 7870 6f6e 656e 7469 616c 5f63  - 'exponential_c
+00010890: 6f75 6e74 270a 2020 2020 2020 2020 2020  ount'.          
+000108a0: 2020 5370 6563 6966 7920 616e 2065 7870    Specify an exp
+000108b0: 6f6e 656e 7469 616c 2028 6261 7365 2065  onential (base e
+000108c0: 2920 7365 7269 6573 206f 6620 7661 6c75  ) series of valu
+000108d0: 6573 2c20 616e 6420 7468 6520 6e75 6d62  es, and the numb
+000108e0: 6572 206f 660a 2020 2020 2020 2020 2020  er of.          
+000108f0: 2020 7661 6c75 6573 2074 6f20 6361 6c63    values to calc
+00010900: 756c 6174 652e 0a0a 2020 2020 2020 2020  ulate...        
+00010910: 466f 7220 7377 705f 7479 7065 3d27 7369  For swp_type='si
+00010920: 6e67 6c65 5f76 616c 7565 2720 7377 705f  ngle_value' swp_
+00010930: 7061 7261 6d73 2069 7320 7468 6520 7369  params is the si
+00010940: 6e67 6c65 2076 616c 7565 2e0a 0a20 2020  ngle value...   
+00010950: 2020 2020 2046 6f72 2073 7770 5f74 7970       For swp_typ
+00010960: 653d 276c 696e 6561 725f 7374 6570 2720  e='linear_step' 
+00010970: 7377 705f 7061 7261 6d73 2069 7320 7374  swp_params is st
+00010980: 6172 742c 2073 746f 702c 2073 7465 703a  art, stop, step:
+00010990: 0a20 2020 2020 2020 2020 2020 2073 7770  .            swp
+000109a0: 5f70 6172 616d 7320 3d20 2822 3132 2e38  _params = ("12.8
+000109b0: 6e48 222c 2022 3133 2e36 6e48 222c 2022  nH", "13.6nH", "
+000109c0: 302e 326e 4822 290a 2020 2020 2020 2020  0.2nH").        
+000109d0: 0a20 2020 2020 2020 2041 6c6c 206f 7468  .        All oth
+000109e0: 6572 2074 7970 6573 2073 7770 5f70 6172  er types swp_par
+000109f0: 616d 7320 6973 2073 7461 7274 2c20 7374  ams is start, st
+00010a00: 6f70 2c20 636f 756e 743a 0a20 2020 2020  op, count:.     
+00010a10: 2020 2020 2020 2073 7770 5f70 6172 616d         swp_param
+00010a20: 7320 3d20 2822 3132 2e38 6e48 222c 2022  s = ("12.8nH", "
+00010a30: 3133 2e36 6e48 222c 2034 290a 2020 2020  13.6nH", 4).    
+00010a40: 2020 2020 2020 2020 5468 6520 6465 6669          The defi
+00010a50: 6e69 7469 6f6e 206f 6620 636f 756e 7420  nition of count 
+00010a60: 7661 7269 6573 2061 6d6f 6e67 7374 2074  varies amongst t
+00010a70: 6865 2061 7661 696c 6162 6c65 2074 7970  he available typ
+00010a80: 6573 2e0a 0a20 2020 2020 2020 2046 6f72  es...        For
+00010a90: 2044 6563 6164 6520 636f 756e 7420 616e   Decade count an
+00010aa0: 6420 4f63 7461 7665 2063 6f75 6e74 2c20  d Octave count, 
+00010ab0: 7468 6520 436f 756e 7420 7661 6c75 6520  the Count value 
+00010ac0: 7370 6563 6966 6965 7320 7468 6520 6e75  specifies the nu
+00010ad0: 6d62 6572 0a20 2020 2020 2020 206f 6620  mber.        of 
+00010ae0: 706f 696e 7473 2074 6f20 6361 6c63 756c  points to calcul
+00010af0: 6174 6520 696e 2065 7665 7279 2064 6563  ate in every dec
+00010b00: 6164 6520 6f72 206f 6374 6176 652e 2046  ade or octave. F
+00010b10: 6f72 2045 7870 6f6e 656e 7469 616c 2063  or Exponential c
+00010b20: 6f75 6e74 2c0a 2020 2020 2020 2020 7468  ount,.        th
+00010b30: 6520 436f 756e 7420 7661 6c75 6520 6973  e Count value is
+00010b40: 2074 6865 2074 6f74 616c 206e 756d 6265   the total numbe
+00010b50: 7220 6f66 2070 6f69 6e74 732e 2054 6865  r of points. The
+00010b60: 2074 6f74 616c 206e 756d 6265 7220 6f66   total number of
+00010b70: 0a20 2020 2020 2020 2070 6f69 6e74 7320  .        points 
+00010b80: 696e 636c 7564 6573 2074 6865 2073 7461  includes the sta
+00010b90: 7274 2061 6e64 2073 746f 7020 7661 6c75  rt and stop valu
+00010ba0: 6573 2e0a 0a20 2020 2020 2020 2046 6f72  es...        For
+00010bb0: 2070 6172 616d 6574 7269 6320 6672 6f6d   parametric from
+00010bc0: 2066 696c 652c 2073 6574 7570 5f74 7970   file, setup_typ
+00010bd0: 653d 2770 6172 616d 6574 7269 635f 6669  e='parametric_fi
+00010be0: 6c65 272c 2070 6173 7320 696e 2061 2066  le', pass in a f
+00010bf0: 696c 650a 2020 2020 2020 2020 6e61 6d65  ile.        name
+00010c00: 2061 6e64 2070 6174 6820 746f 2073 7770   and path to swp
+00010c10: 5f70 6172 616d 7320 6c69 6b65 2022 433a  _params like "C:
+00010c20: 5c5c 7465 7374 2e63 7376 2220 6f72 2022  \\test.csv" or "
+00010c30: 433a 5c5c 7465 7374 2e74 7874 2220 666f  C:\\test.txt" fo
+00010c40: 720a 2020 2020 2020 2020 6578 616d 706c  r.        exampl
+00010c50: 652e 0a0a 2020 2020 2020 2020 4578 616d  e...        Exam
+00010c60: 706c 6520 6373 7620 666f 726d 6174 7469  ple csv formatti
+00010c70: 6e67 3a0a 2020 2020 2020 2020 2a2c 4c6a  ng:.        *,Lj
+00010c80: 5f71 7562 6974 0a20 2020 2020 2020 2031  _qubit.        1
+00010c90: 2c31 322e 326e 480a 2020 2020 2020 2020  ,12.2nH.        
+00010ca0: 322c 392e 376e 480a 2020 2020 2020 2020  2,9.7nH.        
+00010cb0: 332c 3130 2e32 6e48 0a0a 2020 2020 2020  3,10.2nH..      
+00010cc0: 2020 5365 6520 416e 7379 7320 646f 6375    See Ansys docu
+00010cd0: 6d65 6e74 6174 696f 6e20 666f 7220 6164  mentation for ad
+00010ce0: 6469 7469 6f6e 616c 2066 6f72 6d61 7474  ditional formatt
+00010cf0: 696e 6720 696e 7374 7275 6374 696f 6e73  ing instructions
+00010d00: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00010d10: 2020 2020 2020 7365 7475 705f 6e61 6d65        setup_name
+00010d20: 203d 2073 6574 7570 5f6e 616d 6520 6f72   = setup_name or
+00010d30: 2073 656c 662e 6465 7369 676e 2e67 6574   self.design.get
+00010d40: 5f73 6574 7570 5f6e 616d 6573 2829 5b30  _setup_names()[0
+00010d50: 5d0a 2020 2020 2020 2020 7072 696e 7428  ].        print(
+00010d60: 0a20 2020 2020 2020 2020 2020 2066 2249  .            f"I
+00010d70: 6e73 6572 7469 6e67 206f 7074 696d 6574  nserting optimet
+00010d80: 7269 6373 2073 6574 7570 2060 7b6e 616d  rics setup `{nam
+00010d90: 657d 6020 666f 7220 7369 6d75 6c61 7469  e}` for simulati
+00010da0: 6f6e 2073 6574 7570 3a20 607b 7365 7475  on setup: `{setu
+00010db0: 705f 6e61 6d65 7d60 220a 2020 2020 2020  p_name}`".      
+00010dc0: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
+00010dd0: 7365 7475 705f 7479 7065 203d 3d20 2770  setup_type == 'p
+00010de0: 6172 616d 6574 7269 6327 3a0a 0a20 2020  arametric':..   
+00010df0: 2020 2020 2020 2020 2074 7970 655f 6d61           type_ma
+00010e00: 7020 3d20 7b0a 2020 2020 2020 2020 2020  p = {.          
+00010e10: 2020 2020 2020 276c 696e 6561 725f 636f        'linear_co
+00010e20: 756e 7427 3a20 274c 494e 4327 2c0a 2020  unt': 'LINC',.  
+00010e30: 2020 2020 2020 2020 2020 2020 2020 2764                'd
+00010e40: 6563 6164 655f 636f 756e 7427 3a20 2744  ecade_count': 'D
+00010e50: 4543 272c 0a20 2020 2020 2020 2020 2020  EC',.           
+00010e60: 2020 2020 2027 6f63 7461 7665 5f63 6f75       'octave_cou
+00010e70: 6e74 273a 2027 4f43 5427 2c0a 2020 2020  nt': 'OCT',.    
+00010e80: 2020 2020 2020 2020 2020 2020 2765 7870              'exp
+00010e90: 6f6e 656e 7469 616c 5f63 6f75 6e74 273a  onential_count':
+00010ea0: 2027 4553 5450 272c 0a20 2020 2020 2020   'ESTP',.       
+00010eb0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00010ec0: 2020 2076 616c 6964 5f73 7770 5f74 7970     valid_swp_typ
+00010ed0: 6573 203d 207b 2773 696e 676c 655f 7661  es = {'single_va
+00010ee0: 6c75 6527 2c20 276c 696e 6561 725f 7374  lue', 'linear_st
+00010ef0: 6570 277d 207c 2073 6574 2874 7970 655f  ep'} | set(type_
+00010f00: 6d61 702e 6b65 7973 2829 290a 0a20 2020  map.keys())..   
+00010f10: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00010f20: 7374 616e 6365 2876 6172 6961 626c 652c  stance(variable,
+00010f30: 2049 7465 7261 626c 6529 2061 6e64 206e   Iterable) and n
+00010f40: 6f74 2069 7369 6e73 7461 6e63 6528 7661  ot isinstance(va
+00010f50: 7269 6162 6c65 2c20 7374 7229 3a0a 2020  riable, str):.  
+00010f60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00010f70: 7379 6e63 6872 6f6e 697a 6564 2073 7765  synchronized swe
+00010f80: 6570 2c20 6368 6563 6b20 7468 6174 2064  ep, check that d
+00010f90: 6174 6120 6973 2069 6e20 636f 7272 6563  ata is in correc
+00010fa0: 7420 666f 726d 6174 0a20 2020 2020 2020  t format.       
+00010fb0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+00010fc0: 6c65 6e28 7377 705f 7061 7261 6d73 2920  len(swp_params) 
+00010fd0: 3d3d 206c 656e 2873 7770 5f74 7970 6529  == len(swp_type)
+00010fe0: 203d 3d20 6c65 6e28 7661 7269 6162 6c65   == len(variable
+00010ff0: 292c 205c 0a20 2020 2020 2020 2020 2020  ), \.           
+00011000: 2020 2020 2020 2020 2027 496e 636f 7272           'Incorr
+00011010: 6563 7420 7377 705f 7061 7261 6d73 206f  ect swp_params o
+00011020: 7220 7377 705f 7479 7065 2066 6f72 6d61  r swp_type forma
+00011030: 7420 666f 7220 7379 6e63 6872 6f6e 6973  t for synchronis
+00011040: 6564 2073 7765 6570 2e27 0a20 2020 2020  ed sweep.'.     
+00011050: 2020 2020 2020 2020 2020 2073 796e 6368             synch
+00011060: 726f 6e69 7a65 203d 2054 7275 650a 2020  ronize = True.  
+00011070: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00011080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011090: 2320 636f 6e76 6572 7420 616c 6c20 746f  # convert all to
+000110a0: 206c 6973 7473 2061 7320 7765 2063 616e   lists as we can
+000110b0: 2072 6575 7365 2073 616d 6520 636f 6465   reuse same code
+000110c0: 2066 6f72 2073 796e 6368 726f 6e69 7a65   for synchronize
+000110d0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+000110e0: 2020 7377 705f 7479 7065 203d 205b 7377    swp_type = [sw
+000110f0: 705f 7479 7065 5d0a 2020 2020 2020 2020  p_type].        
+00011100: 2020 2020 2020 2020 7377 705f 7061 7261          swp_para
+00011110: 6d73 203d 205b 7377 705f 7061 7261 6d73  ms = [swp_params
+00011120: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00011130: 2020 7661 7269 6162 6c65 203d 205b 7661    variable = [va
+00011140: 7269 6162 6c65 5d0a 2020 2020 2020 2020  riable].        
+00011150: 2020 2020 2020 2020 7379 6e63 6872 6f6e          synchron
+00011160: 697a 6520 3d20 4661 6c73 650a 0a20 2020  ize = False..   
+00011170: 2020 2020 2020 2020 2069 6620 616e 7928           if any(
+00011180: 6520 6e6f 7420 696e 2076 616c 6964 5f73  e not in valid_s
+00011190: 7770 5f74 7970 6573 2066 6f72 2065 2069  wp_types for e i
+000111a0: 6e20 7377 705f 7479 7065 293a 0a20 2020  n swp_type):.   
+000111b0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+000111c0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+000111d0: 6445 7272 6f72 2829 0a20 2020 2020 2020  dError().       
+000111e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000111f0: 2020 2020 2020 2020 2020 2073 7770 5f73             swp_s
+00011200: 7472 203d 206c 6973 7428 290a 2020 2020  tr = list().    
+00011210: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00011220: 692c 2065 2069 6e20 656e 756d 6572 6174  i, e in enumerat
+00011230: 6528 7377 705f 7479 7065 293a 0a20 2020  e(swp_type):.   
+00011240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011250: 2069 6620 6520 3d3d 2027 7369 6e67 6c65   if e == 'single
+00011260: 5f76 616c 7565 273a 0a20 2020 2020 2020  _value':.       
+00011270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011280: 2023 2053 696e 676c 6520 7461 6b65 7320   # Single takes 
+00011290: 7374 7269 6e67 206f 6620 7369 6e67 6c65  string of single
+000112a0: 2076 6172 6961 626c 6520 6e6f 2073 7770   variable no swp
+000112b0: 5f74 7970 655f 6e61 6d65 0a20 2020 2020  _type_name.     
+000112c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000112d0: 2020 2073 7770 5f73 7472 2e61 7070 656e     swp_str.appen
+000112e0: 6428 6622 7b73 7770 5f70 6172 616d 735b  d(f"{swp_params[
+000112f0: 695d 7d22 290a 2020 2020 2020 2020 2020  i]}").          
+00011300: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 2020 2020 2020 2020 2320 636f 7272 6563          # correc
+00011330: 7420 6e75 6d62 6572 206f 6620 696e 7075  t number of inpu
+00011340: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+00011350: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00011360: 7420 6c65 6e28 7377 705f 7061 7261 6d73  t len(swp_params
+00011370: 5b69 5d29 203d 3d20 332c 2022 496e 636f  [i]) == 3, "Inco
+00011380: 7272 6563 7420 6e75 6d62 6572 206f 6620  rrect number of 
+00011390: 7377 6565 7020 7061 7261 6d65 7465 7273  sweep parameters
+000113a0: 2e22 0a0a 2020 2020 2020 2020 2020 2020  ."..            
+000113b0: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
+000113c0: 7420 6368 6563 6b69 6e67 2066 6f72 2063  t checking for c
+000113d0: 6f6d 7061 7469 626c 6520 756e 6974 2074  ompatible unit t
+000113e0: 7970 6573 0a20 2020 2020 2020 2020 2020  ypes.           
+000113f0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00011400: 6520 3d3d 2027 6c69 6e65 6172 5f73 7465  e == 'linear_ste
+00011410: 7027 3a0a 2020 2020 2020 2020 2020 2020  p':.            
+00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011430: 7377 705f 7479 7065 5f6e 616d 6520 3d20  swp_type_name = 
+00011440: 224c 494e 220a 2020 2020 2020 2020 2020  "LIN".          
+00011450: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00011460: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00011470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011480: 2320 636f 756e 7473 206e 6565 6473 2074  # counts needs t
+00011490: 6f20 6265 2061 6e20 696e 7465 6765 7220  o be an integer 
+000114a0: 6e75 6d62 6572 0a20 2020 2020 2020 2020  number.         
+000114b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114c0: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
+000114d0: 616e 6365 2873 7770 5f70 6172 616d 735b  ance(swp_params[
+000114e0: 695d 5b32 5d2c 2069 6e74 292c 2022 436f  i][2], int), "Co
+000114f0: 756e 7420 6d75 7374 2062 6520 696e 7465  unt must be inte
+00011500: 6765 722e 220a 0a20 2020 2020 2020 2020  ger."..         
+00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011520: 2020 2073 7770 5f74 7970 655f 6e61 6d65     swp_type_name
+00011530: 203d 2074 7970 655f 6d61 705b 655d 0a0a   = type_map[e]..
+00011540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011550: 2020 2020 2020 2020 2320 7072 6570 6172          # prepar
+00011560: 6520 7468 6520 7374 7269 6e67 2074 6f20  e the string to 
+00011570: 7061 7373 2074 6f20 416e 7379 730a 2020  pass to Ansys.  
+00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011590: 2020 2020 2020 7377 705f 7374 722e 6170        swp_str.ap
+000115a0: 7065 6e64 2866 227b 7377 705f 7479 7065  pend(f"{swp_type
+000115b0: 5f6e 616d 657d 207b 7377 705f 7061 7261  _name} {swp_para
+000115c0: 6d73 5b69 5d5b 305d 7d20 7b73 7770 5f70  ms[i][0]} {swp_p
+000115d0: 6172 616d 735b 695d 5b31 5d7d 207b 7377  arams[i][1]} {sw
+000115e0: 705f 7061 7261 6d73 5b69 5d5b 325d 7d22  p_params[i][2]}"
+000115f0: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00011600: 656c 662e 5f6f 7074 696d 6574 7269 6373  elf._optimetrics
+00011610: 2e49 6e73 6572 7453 6574 7570 2822 4f70  .InsertSetup("Op
+00011620: 7469 5061 7261 6d65 7472 6963 222c 205b  tiParametric", [
+00011630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011640: 2066 224e 414d 453a 7b6e 616d 657d 222c   f"NAME:{name}",
+00011650: 2022 4973 456e 6162 6c65 643a 3d22 2c20   "IsEnabled:=", 
+00011660: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00011670: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00011680: 2020 2020 2020 2020 2020 2020 224e 414d              "NAM
+00011690: 453a 5072 6f64 4f70 7469 5365 7475 7044  E:ProdOptiSetupD
+000116a0: 6174 6156 3222 2c0a 2020 2020 2020 2020  ataV2",.        
+000116b0: 2020 2020 2020 2020 2020 2020 2253 6176              "Sav
+000116c0: 6546 6965 6c64 733a 3d22 2c0a 2020 2020  eFields:=",.    
+000116d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000116e0: 7361 7665 5f66 6965 6c64 732c 0a20 2020  save_fields,.   
+000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011700: 2022 436f 7079 4d65 7368 3a3d 222c 0a20   "CopyMesh:=",. 
+00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011720: 2020 2063 6f70 795f 6d65 7368 2c0a 2020     copy_mesh,.  
+00011730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011740: 2020 2253 6f6c 7665 5769 7468 436f 7069    "SolveWithCopi
+00011750: 6564 4d65 7368 4f6e 6c79 3a3d 222c 0a20  edMeshOnly:=",. 
+00011760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011770: 2020 2073 6f6c 7665 5f77 6974 685f 636f     solve_with_co
+00011780: 7069 6564 5f6d 6573 685f 6f6e 6c79 2c0a  pied_mesh_only,.
+00011790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000117a0: 5d2c 205b 224e 414d 453a 5374 6172 7469  ], ["NAME:Starti
+000117b0: 6e67 506f 696e 7422 5d2c 2022 5369 6d2e  ngPoint"], "Sim.
+000117c0: 2053 6574 7570 733a 3d22 2c20 5b73 6574   Setups:=", [set
+000117d0: 7570 5f6e 616d 655d 2c0a 2020 2020 2020  up_name],.      
+000117e0: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+000117f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011800: 224e 414d 453a 5377 6565 7073 222c 0a20  "NAME:Sweeps",. 
+00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011820: 2020 202a 5b5b 0a20 2020 2020 2020 2020     *[[.         
+00011830: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011840: 4e41 4d45 3a53 7765 6570 4465 6669 6e69  NAME:SweepDefini
+00011850: 7469 6f6e 222c 2022 5661 7269 6162 6c65  tion", "Variable
+00011860: 3a3d 222c 2076 6172 5f6e 616d 652c 2022  :=", var_name, "
+00011870: 4461 7461 3a3d 222c 0a20 2020 2020 2020  Data:=",.       
+00011880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011890: 2073 7770 2c20 224f 6666 7365 7446 313a   swp, "OffsetF1:
+000118a0: 3d22 2c20 4661 6c73 652c 2022 5379 6e63  =", False, "Sync
+000118b0: 6872 6f6e 697a 653a 3d22 2c20 696e 7428  hronize:=", int(
+000118c0: 7379 6e63 6872 6f6e 697a 6529 0a20 2020  synchronize).   
+000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118e0: 205d 2066 6f72 2076 6172 5f6e 616d 652c   ] for var_name,
+000118f0: 2073 7770 2069 6e20 7a69 7028 7661 7269   swp in zip(vari
+00011900: 6162 6c65 2c20 7377 705f 7374 7229 5d0a  able, swp_str)].
+00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011920: 5d2c 205b 224e 414d 453a 5377 6565 7020  ], ["NAME:Sweep 
+00011930: 4f70 6572 6174 696f 6e73 225d 2c20 5b22  Operations"], ["
+00011940: 4e41 4d45 3a47 6f61 6c73 225d 0a20 2020  NAME:Goals"].   
+00011950: 2020 2020 2020 2020 205d 290a 2020 2020           ]).    
+00011960: 2020 2020 656c 6966 2073 6574 7570 5f74      elif setup_t
+00011970: 7970 6520 3d3d 2027 7061 7261 6d65 7472  ype == 'parametr
+00011980: 6963 5f66 696c 6527 3a0a 2020 2020 2020  ic_file':.      
+00011990: 2020 2020 2020 2320 5573 6573 2074 6865        # Uses the
+000119a0: 2066 696c 6520 6e61 6d65 2061 7320 7468   file name as th
+000119b0: 6520 7377 705f 7061 7261 6d73 0a20 2020  e swp_params.   
+000119c0: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+000119d0: 6520 3d20 7377 705f 7061 7261 6d73 0a0a  e = swp_params..
+000119e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000119f0: 2e5f 6f70 7469 6d65 7472 6963 732e 496d  ._optimetrics.Im
+00011a00: 706f 7274 5365 7475 7028 224f 7074 6950  portSetup("OptiP
+00011a10: 6172 616d 6574 7269 6322 2c0a 2020 2020  arametric",.    
+00011a20: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+00011a30: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00011a40: 4e41 4d45 3a7b 6e61 6d65 7d22 2c0a 2020  NAME:{name}",.  
+00011a50: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00011a60: 6c65 6e61 6d65 2c0a 2020 2020 2020 2020  lename,.        
+00011a70: 2020 2020 2020 2020 5d29 0a20 2020 2020          ]).     
+00011a80: 2020 2020 2020 2073 656c 662e 5f6f 7074         self._opt
+00011a90: 696d 6574 7269 6373 2e45 6469 7453 6574  imetrics.EditSet
+00011aa0: 7570 2866 227b 6e61 6d65 7d22 2c0a 2020  up(f"{name}",.  
+00011ab0: 2020 2020 2020 2020 2020 2020 2020 5b0a                [.
+00011ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ad0: 2020 2020 6622 4e41 4d45 3a7b 6e61 6d65      f"NAME:{name
+00011ae0: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
+00011af0: 0909 5b0a 2020 2020 2020 2020 2020 2020  ..[.            
+00011b00: 0909 0922 4e41 4d45 3a50 726f 644f 7074  ..."NAME:ProdOpt
+00011b10: 6953 6574 7570 4461 7461 5632 222c 0a20  iSetupDataV2",. 
+00011b20: 2020 2020 2020 2020 2020 2009 0909 2253             ..."S
+00011b30: 6176 6546 6965 6c64 733a 3d22 0909 2c20  aveFields:=".., 
+00011b40: 7361 7665 5f66 6965 6c64 732c 0a20 2020  save_fields,.   
+00011b50: 2020 2020 2020 2020 2009 0909 2243 6f70           ..."Cop
+00011b60: 794d 6573 683a 3d22 0909 2c20 636f 7079  yMesh:=".., copy
+00011b70: 5f6d 6573 682c 0a20 2020 2020 2020 2020  _mesh,.         
+00011b80: 2020 2009 0909 2253 6f6c 7665 5769 7468     ..."SolveWith
+00011b90: 436f 7069 6564 4d65 7368 4f6e 6c79 3a3d  CopiedMeshOnly:=
+00011ba0: 222c 2073 6f6c 7665 5f77 6974 685f 636f  ", solve_with_co
+00011bb0: 7069 6564 5f6d 6573 685f 6f6e 6c79 2c0a  pied_mesh_only,.
+00011bc0: 2020 2020 2020 2020 2020 2020 0909 5d2c              ..],
+00011bd0: 0a20 2020 2020 2020 2020 2020 205d 290a  .            ]).
+00011be0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00011bf0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00011c00: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
+00011c10: 726f 7228 290a 0a0a 636c 6173 7320 4866  ror()...class Hf
+00011c20: 7373 4d6f 6465 6c65 7228 434f 4d57 7261  ssModeler(COMWra
+00011c30: 7070 6572 293a 0a20 2020 2064 6566 205f  pper):.    def _
+00011c40: 5f69 6e69 745f 5f28 7365 6c66 2c20 6465  _init__(self, de
+00011c50: 7369 676e 2c20 6d6f 6465 6c65 722c 2062  sign, modeler, b
+00011c60: 6f75 6e64 6172 6965 732c 206d 6573 6829  oundaries, mesh)
+00011c70: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00011c80: 2020 2020 2020 3a74 7970 6520 6465 7369        :type desi
+00011c90: 676e 3a20 4866 7373 4465 7369 676e 0a20  gn: HfssDesign. 
+00011ca0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011cb0: 2020 2073 7570 6572 2848 6673 734d 6f64     super(HfssMod
+00011cc0: 656c 6572 2c20 7365 6c66 292e 5f5f 696e  eler, self).__in
+00011cd0: 6974 5f5f 2829 0a20 2020 2020 2020 2073  it__().        s
+00011ce0: 656c 662e 7061 7265 6e74 203d 2064 6573  elf.parent = des
+00011cf0: 6967 6e0a 2020 2020 2020 2020 7365 6c66  ign.        self
+00011d00: 2e5f 6d6f 6465 6c65 7220 3d20 6d6f 6465  ._modeler = mode
+00011d10: 6c65 720a 2020 2020 2020 2020 7365 6c66  ler.        self
+00011d20: 2e5f 626f 756e 6461 7269 6573 203d 2062  ._boundaries = b
+00011d30: 6f75 6e64 6172 6965 730a 2020 2020 2020  oundaries.      
+00011d40: 2020 7365 6c66 2e5f 6d65 7368 203d 206d    self._mesh = m
+00011d50: 6573 6820 2023 204d 6573 6820 6d6f 6475  esh  # Mesh modu
+00011d60: 6c65 0a0a 2020 2020 6465 6620 7365 745f  le..    def set_
+00011d70: 756e 6974 7328 7365 6c66 2c20 756e 6974  units(self, unit
+00011d80: 732c 2072 6573 6361 6c65 3d54 7275 6529  s, rescale=True)
+00011d90: 3a0a 2020 2020 2020 2020 7365 6c66 2e5f  :.        self._
+00011da0: 6d6f 6465 6c65 722e 5365 744d 6f64 656c  modeler.SetModel
+00011db0: 556e 6974 7328 0a20 2020 2020 2020 2020  Units(.         
+00011dc0: 2020 205b 224e 414d 453a 556e 6974 7320     ["NAME:Units 
+00011dd0: 5061 7261 6d65 7465 7222 2c20 2255 6e69  Parameter", "Uni
+00011de0: 7473 3a3d 222c 2075 6e69 7473 2c20 2252  ts:=", units, "R
+00011df0: 6573 6361 6c65 3a3d 222c 2072 6573 6361  escale:=", resca
+00011e00: 6c65 5d29 0a0a 2020 2020 6465 6620 6765  le])..    def ge
+00011e10: 745f 756e 6974 7328 7365 6c66 293a 0a20  t_units(self):. 
+00011e20: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
+00011e30: 6520 6d6f 6465 6c20 756e 6974 732e 0a20  e model units.. 
+00011e40: 2020 2020 2020 2020 2020 2052 6574 7572             Retur
+00011e50: 6e20 5661 6c75 653a 2020 2020 4120 7374  n Value:    A st
+00011e60: 7269 6e67 2063 6f6e 7461 696e 7320 6375  ring contains cu
+00011e70: 7272 656e 7420 6d6f 6465 6c20 756e 6974  rrent model unit
+00011e80: 732e 2022 2222 0a20 2020 2020 2020 2072  s. """.        r
+00011e90: 6574 7572 6e20 7374 7228 7365 6c66 2e5f  eturn str(self._
+00011ea0: 6d6f 6465 6c65 722e 4765 744d 6f64 656c  modeler.GetModel
+00011eb0: 556e 6974 7328 2929 0a0a 2020 2020 6465  Units())..    de
+00011ec0: 6620 6765 745f 616c 6c5f 7072 6f70 6572  f get_all_proper
+00011ed0: 7469 6573 2873 656c 662c 206f 626a 5f6e  ties(self, obj_n
+00011ee0: 616d 652c 2050 726f 7054 6162 3d27 4765  ame, PropTab='Ge
+00011ef0: 6f6d 6574 7279 3344 4174 7472 6962 7574  ometry3DAttribut
+00011f00: 6554 6162 2729 3a0a 2020 2020 2020 2020  eTab'):.        
+00011f10: 2727 270a 2020 2020 2020 2020 2020 2020  '''.            
+00011f20: 4765 7420 616c 6c20 7072 6f70 6572 7469  Get all properti
+00011f30: 6573 2066 6f72 206d 6f64 656c 6572 2050  es for modeler P
+00011f40: 726f 7054 6162 2c20 5072 6f70 5365 7276  ropTab, PropServ
+00011f50: 6572 0a20 2020 2020 2020 2027 2727 0a20  er.        '''. 
+00011f60: 2020 2020 2020 2050 726f 7053 6572 7665         PropServe
+00011f70: 7220 3d20 6f62 6a5f 6e61 6d65 0a20 2020  r = obj_name.   
+00011f80: 2020 2020 2070 726f 7065 7274 6965 7320       properties 
+00011f90: 3d20 7b7d 0a20 2020 2020 2020 2066 6f72  = {}.        for
+00011fa0: 206b 6579 2069 6e20 7365 6c66 2e5f 6d6f   key in self._mo
+00011fb0: 6465 6c65 722e 4765 7450 726f 7065 7274  deler.GetPropert
+00011fc0: 6965 7328 5072 6f70 5461 622c 2050 726f  ies(PropTab, Pro
+00011fd0: 7053 6572 7665 7229 3a0a 2020 2020 2020  pServer):.      
+00011fe0: 2020 2020 2020 7072 6f70 6572 7469 6573        properties
+00011ff0: 5b6b 6579 5d20 3d20 7365 6c66 2e5f 6d6f  [key] = self._mo
+00012000: 6465 6c65 722e 4765 7450 726f 7065 7274  deler.GetPropert
+00012010: 7956 616c 7565 280a 2020 2020 2020 2020  yValue(.        
+00012020: 2020 2020 2020 2020 5072 6f70 5461 622c          PropTab,
+00012030: 2050 726f 7053 6572 7665 722c 206b 6579   PropServer, key
+00012040: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00012050: 2070 726f 7065 7274 6965 730a 0a20 2020   properties..   
+00012060: 2064 6566 205f 6174 7472 6962 7574 6573   def _attributes
+00012070: 5f61 7272 6179 280a 2020 2020 2020 2020  _array(.        
+00012080: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00012090: 2020 2020 2020 6e61 6d65 3d4e 6f6e 652c        name=None,
+000120a0: 0a20 2020 2020 2020 2020 2020 206e 6f6e  .            non
+000120b0: 6d6f 6465 6c3d 4661 6c73 652c 0a20 2020  model=False,.   
+000120c0: 2020 2020 2020 2020 2077 6972 6566 7261           wirefra
+000120d0: 6d65 3d46 616c 7365 2c0a 2020 2020 2020  me=False,.      
+000120e0: 2020 2020 2020 636f 6c6f 723d 4e6f 6e65        color=None
+000120f0: 2c0a 2020 2020 2020 2020 2020 2020 7472  ,.            tr
+00012100: 616e 7370 6172 656e 6379 3d30 2e39 2c0a  ansparency=0.9,.
+00012110: 2020 2020 2020 2020 2020 2020 6d61 7465              mate
+00012120: 7269 616c 3d4e 6f6e 652c 2020 2320 7374  rial=None,  # st
+00012130: 720a 2020 2020 2020 2020 2020 2020 736f  r.            so
+00012140: 6c76 655f 696e 7369 6465 3d4e 6f6e 652c  lve_inside=None,
+00012150: 2020 2320 626f 6f6c 0a20 2020 2020 2020    # bool.       
+00012160: 2020 2020 2063 6f6f 7264 696e 6174 655f       coordinate_
+00012170: 7379 7374 656d 3d22 476c 6f62 616c 2229  system="Global")
+00012180: 3a0a 2020 2020 2020 2020 6172 7220 3d20  :.        arr = 
+00012190: 5b22 4e41 4d45 3a41 7474 7269 6275 7465  ["NAME:Attribute
+000121a0: 7322 2c20 2250 6172 7443 6f6f 7264 696e  s", "PartCoordin
+000121b0: 6174 6553 7973 7465 6d3a 3d22 2c20 636f  ateSystem:=", co
+000121c0: 6f72 6469 6e61 7465 5f73 7973 7465 6d5d  ordinate_system]
+000121d0: 0a20 2020 2020 2020 2069 6620 6e61 6d65  .        if name
+000121e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000121f0: 2020 2020 2020 2020 2020 6172 722e 6578            arr.ex
+00012200: 7465 6e64 285b 224e 616d 653a 3d22 2c20  tend(["Name:=", 
+00012210: 6e61 6d65 5d29 0a0a 2020 2020 2020 2020  name])..        
+00012220: 6966 206e 6f6e 6d6f 6465 6c20 6f72 2077  if nonmodel or w
+00012230: 6972 6566 7261 6d65 3a0a 2020 2020 2020  ireframe:.      
+00012240: 2020 2020 2020 666c 6167 7320 3d20 274e        flags = 'N
+00012250: 6f6e 4d6f 6465 6c27 2069 6620 6e6f 6e6d  onModel' if nonm
+00012260: 6f64 656c 2065 6c73 6520 2727 2020 2320  odel else ''  # 
+00012270: 6361 6e20 6265 2064 6f6e 6520 736d 6172  can be done smar
+00012280: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
+00012290: 6966 2077 6972 6566 7261 6d65 3a0a 2020  if wireframe:.  
+000122a0: 2020 2020 2020 2020 2020 2020 2020 666c                fl
+000122b0: 6167 7320 2b3d 2027 2327 2069 6620 6c65  ags += '#' if le
+000122c0: 6e28 666c 6167 7329 203e 2030 2065 6c73  n(flags) > 0 els
+000122d0: 6520 2727 0a20 2020 2020 2020 2020 2020  e ''.           
+000122e0: 2020 2020 2066 6c61 6773 202b 3d20 2757       flags += 'W
+000122f0: 6972 6566 7261 6d65 270a 2020 2020 2020  ireframe'.      
+00012300: 2020 2020 2020 6172 722e 6578 7465 6e64        arr.extend
+00012310: 285b 2246 6c61 6773 3a3d 222c 2066 6c61  (["Flags:=", fla
+00012320: 6773 5d29 0a0a 2020 2020 2020 2020 6966  gs])..        if
+00012330: 2063 6f6c 6f72 2069 7320 6e6f 7420 4e6f   color is not No
+00012340: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00012350: 6172 722e 6578 7465 6e64 285b 2243 6f6c  arr.extend(["Col
+00012360: 6f72 3a3d 222c 2022 2825 6420 2564 2025  or:=", "(%d %d %
+00012370: 6429 2220 2520 636f 6c6f 725d 290a 2020  d)" % color]).  
+00012380: 2020 2020 2020 6966 2074 7261 6e73 7061        if transpa
+00012390: 7265 6e63 7920 6973 206e 6f74 204e 6f6e  rency is not Non
+000123a0: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+000123b0: 7272 2e65 7874 656e 6428 5b22 5472 616e  rr.extend(["Tran
+000123c0: 7370 6172 656e 6379 3a3d 222c 2074 7261  sparency:=", tra
+000123d0: 6e73 7061 7265 6e63 795d 290a 2020 2020  nsparency]).    
+000123e0: 2020 2020 6966 206d 6174 6572 6961 6c20      if material 
+000123f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00012400: 2020 2020 2020 2020 2061 7272 2e65 7874           arr.ext
+00012410: 656e 6428 5b22 4d61 7465 7269 616c 4e61  end(["MaterialNa
+00012420: 6d65 3a3d 222c 206d 6174 6572 6961 6c5d  me:=", material]
+00012430: 290a 2020 2020 2020 2020 6966 2073 6f6c  ).        if sol
+00012440: 7665 5f69 6e73 6964 6520 6973 206e 6f74  ve_inside is not
+00012450: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00012460: 2020 2061 7272 2e65 7874 656e 6428 5b22     arr.extend(["
+00012470: 536f 6c76 6549 6e73 6964 653a 3d22 2c20  SolveInside:=", 
+00012480: 736f 6c76 655f 696e 7369 6465 5d29 0a0a  solve_inside])..
+00012490: 2020 2020 2020 2020 7265 7475 726e 2061          return a
+000124a0: 7272 0a0a 2020 2020 6465 6620 5f73 656c  rr..    def _sel
+000124b0: 6563 7469 6f6e 735f 6172 7261 7928 7365  ections_array(se
+000124c0: 6c66 2c20 2a6e 616d 6573 293a 0a20 2020  lf, *names):.   
+000124d0: 2020 2020 2072 6574 7572 6e20 5b22 4e41       return ["NA
+000124e0: 4d45 3a53 656c 6563 7469 6f6e 7322 2c20  ME:Selections", 
+000124f0: 2253 656c 6563 7469 6f6e 733a 3d22 2c20  "Selections:=", 
+00012500: 222c 222e 6a6f 696e 286e 616d 6573 295d  ",".join(names)]
+00012510: 0a0a 2020 2020 6465 6620 6d65 7368 5f6c  ..    def mesh_l
+00012520: 656e 6774 6828 7365 6c66 2c0a 2020 2020  ength(self,.    
+00012530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012540: 6e61 6d65 5f6d 6573 682c 0a20 2020 2020  name_mesh,.     
+00012550: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00012560: 626a 6563 7473 3a20 6c69 7374 2c0a 2020  bjects: list,.  
+00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012580: 2020 4d61 784c 656e 6774 683d 2730 2e31    MaxLength='0.1
+00012590: 6d6d 272c 0a20 2020 2020 2020 2020 2020  mm',.           
+000125a0: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
+000125b0: 7329 3a0a 2020 2020 2020 2020 2727 270a  s):.        '''.
+000125c0: 2020 2020 2020 2020 2252 6566 696e 6549          "RefineI
+000125d0: 6e73 6964 653a 3d22 092c 2046 616c 7365  nside:="., False
+000125e0: 2c0a 2020 2020 2020 2020 2245 6e61 626c  ,.        "Enabl
+000125f0: 6564 3a3d 2209 092c 2054 7275 652c 0a20  ed:=".., True,. 
+00012600: 2020 2020 2020 2022 5265 7374 7269 6374         "Restrict
+00012610: 456c 656d 3a3d 2209 2c20 4661 6c73 652c  Elem:="., False,
+00012620: 0a20 2020 2020 2020 2022 4e75 6d4d 6178  .        "NumMax
+00012630: 456c 656d 3a3d 2209 092c 2022 3130 3030  Elem:=".., "1000
+00012640: 222c 0a20 2020 2020 2020 2022 5265 7374  ",.        "Rest
+00012650: 7269 6374 4c65 6e67 7468 3a3d 2209 2c20  rictLength:="., 
+00012660: 5472 7565 2c0a 2020 2020 2020 2020 224d  True,.        "M
+00012670: 6178 4c65 6e67 7468 3a3d 2209 092c 2022  axLength:=".., "
+00012680: 302e 316d 6d22 0a0a 2020 2020 2020 2020  0.1mm"..        
+00012690: 4578 616d 706c 6520 7573 653a 0a20 2020  Example use:.   
+000126a0: 2020 2020 206d 6f64 656c 6572 2e61 7373       modeler.ass
+000126b0: 6967 6e5f 6d65 7368 5f6c 656e 6774 6828  ign_mesh_length(
+000126c0: 276d 6573 6832 272c 205b 2251 315f 6d65  'mesh2', ["Q1_me
+000126d0: 7368 225d 2c20 4d61 784c 656e 6774 683d  sh"], MaxLength=
+000126e0: 302e 3129 0a20 2020 2020 2020 2027 2727  0.1).        '''
+000126f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00012700: 6973 696e 7374 616e 6365 286f 626a 6563  isinstance(objec
+00012710: 7473 2c20 6c69 7374 290a 0a20 2020 2020  ts, list)..     
+00012720: 2020 2061 7272 203d 205b 0a20 2020 2020     arr = [.     
+00012730: 2020 2020 2020 2066 224e 414d 453a 7b6e         f"NAME:{n
+00012740: 616d 655f 6d65 7368 7d22 2c20 224f 626a  ame_mesh}", "Obj
+00012750: 6563 7473 3a3d 222c 206f 626a 6563 7473  ects:=", objects
+00012760: 2c20 274d 6178 4c65 6e67 7468 3a3d 272c  , 'MaxLength:=',
+00012770: 204d 6178 4c65 6e67 7468 0a20 2020 2020   MaxLength.     
+00012780: 2020 205d 0a20 2020 2020 2020 206f 7073     ].        ops
+00012790: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+000127a0: 2027 5265 6669 6e65 496e 7369 6465 272c   'RefineInside',
+000127b0: 2027 456e 6162 6c65 6427 2c20 2752 6573   'Enabled', 'Res
+000127c0: 7472 6963 7445 6c65 6d27 2c20 274e 756d  trictElem', 'Num
+000127d0: 4d61 7845 6c65 6d27 2c0a 2020 2020 2020  MaxElem',.      
+000127e0: 2020 2020 2020 2752 6573 7472 6963 744c        'RestrictL
+000127f0: 656e 6774 6827 0a20 2020 2020 2020 205d  ength'.        ]
+00012800: 0a20 2020 2020 2020 2066 6f72 206b 6579  .        for key
+00012810: 2c20 7661 6c20 696e 206b 7761 7267 732e  , val in kwargs.
+00012820: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
+00012830: 2020 2020 2069 6620 6b65 7920 696e 206f       if key in o
+00012840: 7073 3a0a 2020 2020 2020 2020 2020 2020  ps:.            
+00012850: 2020 2020 6172 7220 2b3d 205b 6b65 7920      arr += [key 
+00012860: 2b20 273a 3d27 2c20 7374 7228 7661 6c29  + ':=', str(val)
+00012870: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
+00012880: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012890: 2020 2020 6c6f 6767 6572 2e65 7272 6f72      logger.error
+000128a0: 2827 4b45 5920 607b 6b65 797d 6020 4e4f  ('KEY `{key}` NO
+000128b0: 5420 494e 206f 7073 2127 290a 0a20 2020  T IN ops!')..   
+000128c0: 2020 2020 2073 656c 662e 5f6d 6573 682e       self._mesh.
+000128d0: 4173 7369 676e 4c65 6e67 7468 4f70 2861  AssignLengthOp(a
+000128e0: 7272 290a 0a20 2020 2064 6566 206d 6573  rr)..    def mes
+000128f0: 685f 7265 6173 7369 676e 2873 656c 662c  h_reassign(self,
+00012900: 206e 616d 655f 6d65 7368 2c20 6f62 6a65   name_mesh, obje
+00012910: 6374 733a 206c 6973 7429 3a0a 2020 2020  cts: list):.    
+00012920: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
+00012930: 7461 6e63 6528 6f62 6a65 6374 732c 206c  tance(objects, l
+00012940: 6973 7429 0a20 2020 2020 2020 2073 656c  ist).        sel
+00012950: 662e 5f6d 6573 682e 5265 6173 7369 676e  f._mesh.Reassign
+00012960: 4f70 286e 616d 655f 6d65 7368 2c20 5b22  Op(name_mesh, ["
+00012970: 4f62 6a65 6374 733a 3d22 2c20 6f62 6a65  Objects:=", obje
+00012980: 6374 735d 290a 0a20 2020 2064 6566 206d  cts])..    def m
+00012990: 6573 685f 6765 745f 6e61 6d65 7328 7365  esh_get_names(se
+000129a0: 6c66 2c20 6b69 6e64 3d22 4c65 6e67 7468  lf, kind="Length
+000129b0: 2042 6173 6564 2229 3a0a 2020 2020 2020   Based"):.      
+000129c0: 2020 2727 2720 224c 656e 6774 6820 4261    ''' "Length Ba
+000129d0: 7365 6422 2c20 2253 6b69 6e20 4465 7074  sed", "Skin Dept
+000129e0: 6820 4261 7365 6422 2c20 2e2e 2e27 2727  h Based", ...'''
+000129f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012a00: 6c69 7374 2873 656c 662e 5f6d 6573 682e  list(self._mesh.
+00012a10: 4765 744f 7065 7261 7469 6f6e 4e61 6d65  GetOperationName
+00012a20: 7328 6b69 6e64 2929 0a0a 2020 2020 6465  s(kind))..    de
+00012a30: 6620 6d65 7368 5f67 6574 5f61 6c6c 5f70  f mesh_get_all_p
+00012a40: 726f 7073 2873 656c 662c 206d 6573 685f  rops(self, mesh_
+00012a50: 6e61 6d65 293a 0a20 2020 2020 2020 2023  name):.        #
+00012a60: 2054 4f44 4f3a 206d 616b 6520 6d65 7368   TODO: make mesh
+00012a70: 2074 6973 206f 776e 2020 636c 6173 7320   tis own  class 
+00012a80: 7769 7468 2070 726f 7065 7274 6965 730a  with properties.
+00012a90: 2020 2020 2020 2020 7072 6f70 5f74 6162          prop_tab
+00012aa0: 203d 2027 4d65 7368 5365 7475 7054 6162   = 'MeshSetupTab
+00012ab0: 270a 2020 2020 2020 2020 7072 6f70 5f73  '.        prop_s
+00012ac0: 6572 7665 7220 3d20 6627 4d65 7368 5365  erver = f'MeshSe
+00012ad0: 7475 703a 7b6d 6573 685f 6e61 6d65 7d27  tup:{mesh_name}'
+00012ae0: 0a20 2020 2020 2020 2070 726f 705f 6e61  .        prop_na
+00012af0: 6d65 7320 3d20 7365 6c66 2e70 6172 656e  mes = self.paren
+00012b00: 742e 5f64 6573 6967 6e2e 4765 7450 726f  t._design.GetPro
+00012b10: 7065 7274 6965 7328 274d 6573 6853 6574  perties('MeshSet
+00012b20: 7570 5461 6227 2c0a 2020 2020 2020 2020  upTab',.        
+00012b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00012b60: 726f 705f 7365 7276 6572 290a 2020 2020  rop_server).    
+00012b70: 2020 2020 6469 6320 3d20 7b7d 0a20 2020      dic = {}.   
+00012b80: 2020 2020 2066 6f72 206e 616d 6520 696e       for name in
+00012b90: 2070 726f 705f 6e61 6d65 733a 0a20 2020   prop_names:.   
+00012ba0: 2020 2020 2020 2020 2064 6963 5b6e 616d           dic[nam
+00012bb0: 655d 203d 2073 656c 662e 5f6d 6f64 656c  e] = self._model
+00012bc0: 6572 2e47 6574 5072 6f70 6572 7479 5661  er.GetPropertyVa
+00012bd0: 6c75 6528 7072 6f70 5f74 6162 2c20 7072  lue(prop_tab, pr
+00012be0: 6f70 5f73 6572 7665 722c 0a20 2020 2020  op_server,.     
+00012bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c20: 2020 6e61 6d65 290a 2020 2020 2020 2020    name).        
+00012c30: 7265 7475 726e 2064 6963 0a0a 2020 2020  return dic..    
+00012c40: 6465 6620 6472 6177 5f62 6f78 5f63 6f72  def draw_box_cor
+00012c50: 6e65 7228 7365 6c66 2c20 706f 732c 2073  ner(self, pos, s
+00012c60: 697a 652c 202a 2a6b 7761 7267 7329 3a0a  ize, **kwargs):.
+00012c70: 2020 2020 2020 2020 6e61 6d65 203d 2073          name = s
+00012c80: 656c 662e 5f6d 6f64 656c 6572 2e43 7265  elf._modeler.Cre
+00012c90: 6174 6542 6f78 285b 0a20 2020 2020 2020  ateBox([.       
+00012ca0: 2020 2020 2022 4e41 4d45 3a42 6f78 5061       "NAME:BoxPa
+00012cb0: 7261 6d65 7465 7273 222c 2022 5850 6f73  rameters", "XPos
+00012cc0: 6974 696f 6e3a 3d22 2c0a 2020 2020 2020  ition:=",.      
+00012cd0: 2020 2020 2020 7374 7228 706f 735b 305d        str(pos[0]
+00012ce0: 292c 2022 5950 6f73 6974 696f 6e3a 3d22  ), "YPosition:="
+00012cf0: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+00012d00: 7228 706f 735b 315d 292c 2022 5a50 6f73  r(pos[1]), "ZPos
+00012d10: 6974 696f 6e3a 3d22 2c0a 2020 2020 2020  ition:=",.      
+00012d20: 2020 2020 2020 7374 7228 706f 735b 325d        str(pos[2]
+00012d30: 292c 2022 5853 697a 653a 3d22 2c0a 2020  ), "XSize:=",.  
+00012d40: 2020 2020 2020 2020 2020 7374 7228 7369            str(si
+00012d50: 7a65 5b30 5d29 2c20 2259 5369 7a65 3a3d  ze[0]), "YSize:=
+00012d60: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
+00012d70: 7472 2873 697a 655b 315d 292c 2022 5a53  tr(size[1]), "ZS
+00012d80: 697a 653a 3d22 2c0a 2020 2020 2020 2020  ize:=",.        
+00012d90: 2020 2020 7374 7228 7369 7a65 5b32 5d29      str(size[2])
+00012da0: 0a20 2020 2020 2020 205d 2c20 7365 6c66  .        ], self
+00012db0: 2e5f 6174 7472 6962 7574 6573 5f61 7272  ._attributes_arr
+00012dc0: 6179 282a 2a6b 7761 7267 7329 290a 2020  ay(**kwargs)).  
+00012dd0: 2020 2020 2020 7265 7475 726e 2042 6f78        return Box
+00012de0: 286e 616d 652c 2073 656c 662c 2070 6f73  (name, self, pos
+00012df0: 2c20 7369 7a65 290a 0a20 2020 2064 6566  , size)..    def
+00012e00: 2064 7261 775f 626f 785f 6365 6e74 6572   draw_box_center
+00012e10: 2873 656c 662c 2070 6f73 2c20 7369 7a65  (self, pos, size
+00012e20: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00012e30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012e40: 2043 7265 6174 6573 2061 2033 2d44 2062   Creates a 3-D b
+00012e50: 6f78 2063 656e 7465 7265 6420 6174 2070  ox centered at p
+00012e60: 6f73 205b 7830 2c20 7930 2c20 7a30 5d2c  os [x0, y0, z0],
+00012e70: 2077 6974 6820 7769 6474 680a 2020 2020   with width.    
+00012e80: 2020 2020 7369 7a65 205b 7877 6964 7468      size [xwidth
+00012e90: 2c20 7977 6964 7468 2c20 7a77 6964 7468  , ywidth, zwidth
+00012ea0: 5d20 616c 6f6e 6720 6561 6368 2072 6573  ] along each res
+00012eb0: 7065 6374 6976 6520 6469 7265 6374 696f  pective directio
+00012ec0: 6e2e 0a0a 2020 2020 2020 2020 4172 6773  n...        Args
+00012ed0: 3a0a 2020 2020 2020 2020 2020 2020 706f  :.            po
+00012ee0: 7320 286c 6973 7429 3a20 436f 6f72 6469  s (list): Coordi
+00012ef0: 6e61 7465 7320 6f66 2063 656e 7465 7220  nates of center 
+00012f00: 6f66 2062 6f78 2c20 5b78 302c 2079 302c  of box, [x0, y0,
+00012f10: 207a 305d 0a20 2020 2020 2020 2020 2020   z0].           
+00012f20: 2073 697a 6520 286c 6973 7429 3a20 5769   size (list): Wi
+00012f30: 6474 6820 6f66 2062 6f78 2061 6c6f 6e67  dth of box along
+00012f40: 2065 6163 6820 6469 7265 6374 696f 6e2c   each direction,
+00012f50: 205b 7877 6964 7468 2c20 7977 6964 7468   [xwidth, ywidth
+00012f60: 2c20 7a77 6964 7468 5d0a 2020 2020 2020  , zwidth].      
+00012f70: 2020 2222 220a 2020 2020 2020 2020 636f    """.        co
+00012f80: 726e 6572 5f70 6f73 203d 205b 7661 7228  rner_pos = [var(
+00012f90: 7029 202d 2076 6172 2873 2920 2f20 3220  p) - var(s) / 2 
+00012fa0: 666f 7220 702c 2073 2069 6e20 7a69 7028  for p, s in zip(
+00012fb0: 706f 732c 2073 697a 6529 5d0a 2020 2020  pos, size)].    
+00012fc0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00012fd0: 6472 6177 5f62 6f78 5f63 6f72 6e65 7228  draw_box_corner(
+00012fe0: 636f 726e 6572 5f70 6f73 2c20 7369 7a65  corner_pos, size
+00012ff0: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
+00013000: 2064 6566 2064 7261 775f 706f 6c79 6c69   def draw_polyli
+00013010: 6e65 2873 656c 662c 2070 6f69 6e74 732c  ne(self, points,
+00013020: 2063 6c6f 7365 643d 5472 7565 2c20 2a2a   closed=True, **
+00013030: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00013040: 2022 2222 0a20 2020 2020 2020 2044 7261   """.        Dra
+00013050: 7773 2061 2063 6c6f 7365 6420 6f72 206f  ws a closed or o
+00013060: 7065 6e20 706f 6c79 6c69 6e65 2e0a 2020  pen polyline..  
+00013070: 2020 2020 2020 4966 2063 6c6f 7365 6420        If closed 
+00013080: 3d20 5472 7565 2c20 7468 656e 2077 696c  = True, then wil
+00013090: 6c20 6d61 6b65 2069 6e74 6f20 6120 7368  l make into a sh
+000130a0: 6565 742e 0a20 2020 2020 2020 2070 6f69  eet..        poi
+000130b0: 6e74 7320 3a20 6e65 6564 2074 6f20 6265  nts : need to be
+000130c0: 2069 6e20 7468 6520 636f 7272 6563 7420   in the correct 
+000130d0: 756e 6974 730a 0a20 2020 2020 2020 2046  units..        F
+000130e0: 6f72 206f 7074 696f 6e61 6c20 6172 6775  or optional argu
+000130f0: 6d65 6e74 732c 2073 6565 205f 6174 7472  ments, see _attr
+00013100: 6962 7574 6573 5f61 7272 6179 3b20 7468  ibutes_array; th
+00013110: 6573 6520 696e 636c 7564 653a 0a20 2020  ese include:.   
+00013120: 2020 2020 2060 6060 0a20 2020 2020 2020       ```.       
+00013130: 2020 2020 206e 6f6e 6d6f 6465 6c3d 4661       nonmodel=Fa
+00013140: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00013150: 2077 6972 6566 7261 6d65 3d46 616c 7365   wireframe=False
+00013160: 2c0a 2020 2020 2020 2020 2020 2020 636f  ,.            co
+00013170: 6c6f 723d 4e6f 6e65 2c0a 2020 2020 2020  lor=None,.      
+00013180: 2020 2020 2020 7472 616e 7370 6172 656e        transparen
+00013190: 6379 3d30 2e39 2c0a 2020 2020 2020 2020  cy=0.9,.        
+000131a0: 2020 2020 6d61 7465 7269 616c 3d4e 6f6e      material=Non
+000131b0: 652c 2020 2320 7374 720a 2020 2020 2020  e,  # str.      
+000131c0: 2020 2020 2020 736f 6c76 655f 696e 7369        solve_insi
+000131d0: 6465 3d4e 6f6e 652c 2020 2320 626f 6f6c  de=None,  # bool
+000131e0: 0a20 2020 2020 2020 2020 2020 2063 6f6f  .            coo
+000131f0: 7264 696e 6174 655f 7379 7374 656d 3d22  rdinate_system="
+00013200: 476c 6f62 616c 220a 2020 2020 2020 2020  Global".        
+00013210: 6060 600a 2020 2020 2020 2020 2222 220a  ```.        """.
+00013220: 2020 2020 2020 2020 706f 696e 7473 5374          pointsSt
+00013230: 7220 3d20 5b22 4e41 4d45 3a50 6f6c 796c  r = ["NAME:Polyl
+00013240: 696e 6550 6f69 6e74 7322 5d0a 2020 2020  inePoints"].    
+00013250: 2020 2020 696e 6465 7873 5374 7220 3d20      indexsStr = 
+00013260: 5b22 4e41 4d45 3a50 6f6c 796c 696e 6553  ["NAME:PolylineS
+00013270: 6567 6d65 6e74 7322 5d0a 2020 2020 2020  egments"].      
+00013280: 2020 666f 7220 6969 2c20 706f 696e 7420    for ii, point 
+00013290: 696e 2065 6e75 6d65 7261 7465 2870 6f69  in enumerate(poi
+000132a0: 6e74 7329 3a0a 2020 2020 2020 2020 2020  nts):.          
+000132b0: 2020 706f 696e 7473 5374 722e 6170 7065    pointsStr.appe
+000132c0: 6e64 285b 0a20 2020 2020 2020 2020 2020  nd([.           
+000132d0: 2020 2020 2022 4e41 4d45 3a50 4c50 6f69       "NAME:PLPoi
+000132e0: 6e74 222c 2022 583a 3d22 2c0a 2020 2020  nt", "X:=",.    
+000132f0: 2020 2020 2020 2020 2020 2020 7374 7228              str(
+00013300: 706f 696e 745b 305d 292c 2022 593a 3d22  point[0]), "Y:="
+00013310: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013320: 2020 7374 7228 706f 696e 745b 315d 292c    str(point[1]),
+00013330: 2022 5a3a 3d22 2c0a 2020 2020 2020 2020   "Z:=",.        
+00013340: 2020 2020 2020 2020 7374 7228 706f 696e          str(poin
+00013350: 745b 325d 290a 2020 2020 2020 2020 2020  t[2]).          
+00013360: 2020 5d29 0a20 2020 2020 2020 2020 2020    ]).           
+00013370: 2069 6e64 6578 7353 7472 2e61 7070 656e   indexsStr.appen
+00013380: 6428 5b0a 2020 2020 2020 2020 2020 2020  d([.            
+00013390: 2020 2020 224e 414d 453a 504c 5365 676d      "NAME:PLSegm
+000133a0: 656e 7422 2c20 2253 6567 6d65 6e74 5479  ent", "SegmentTy
+000133b0: 7065 3a3d 222c 2022 4c69 6e65 222c 2022  pe:=", "Line", "
+000133c0: 5374 6172 7449 6e64 6578 3a3d 222c 2069  StartIndex:=", i
+000133d0: 692c 0a20 2020 2020 2020 2020 2020 2020  i,.             
+000133e0: 2020 2022 4e6f 4f66 506f 696e 7473 3a3d     "NoOfPoints:=
+000133f0: 222c 2032 0a20 2020 2020 2020 2020 2020  ", 2.           
+00013400: 205d 290a 2020 2020 2020 2020 6966 2063   ]).        if c
+00013410: 6c6f 7365 643a 0a20 2020 2020 2020 2020  losed:.         
+00013420: 2020 2070 6f69 6e74 7353 7472 2e61 7070     pointsStr.app
+00013430: 656e 6428 5b0a 2020 2020 2020 2020 2020  end([.          
+00013440: 2020 2020 2020 224e 414d 453a 504c 506f        "NAME:PLPo
+00013450: 696e 7422 2c20 2258 3a3d 222c 0a20 2020  int", "X:=",.   
+00013460: 2020 2020 2020 2020 2020 2020 2073 7472               str
+00013470: 2870 6f69 6e74 735b 305d 5b30 5d29 2c20  (points[0][0]), 
+00013480: 2259 3a3d 222c 0a20 2020 2020 2020 2020  "Y:=",.         
+00013490: 2020 2020 2020 2073 7472 2870 6f69 6e74         str(point
+000134a0: 735b 305d 5b31 5d29 2c20 225a 3a3d 222c  s[0][1]), "Z:=",
+000134b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000134c0: 2073 7472 2870 6f69 6e74 735b 305d 5b32   str(points[0][2
+000134d0: 5d29 0a20 2020 2020 2020 2020 2020 205d  ]).            ]
+000134e0: 290a 2020 2020 2020 2020 2020 2020 7061  ).            pa
+000134f0: 7261 6d73 5f63 6c6f 7365 6420 3d20 5b0a  rams_closed = [.
+00013500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013510: 2249 7350 6f6c 796c 696e 6543 6f76 6572  "IsPolylineCover
+00013520: 6564 3a3d 222c 2054 7275 652c 2022 4973  ed:=", True, "Is
+00013530: 506f 6c79 6c69 6e65 436c 6f73 6564 3a3d  PolylineClosed:=
+00013540: 222c 2054 7275 650a 2020 2020 2020 2020  ", True.        
+00013550: 2020 2020 5d0a 2020 2020 2020 2020 656c      ].        el
+00013560: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00013570: 696e 6465 7873 5374 7220 3d20 696e 6465  indexsStr = inde
+00013580: 7873 5374 725b 3a2d 315d 0a20 2020 2020  xsStr[:-1].     
+00013590: 2020 2020 2020 2070 6172 616d 735f 636c         params_cl
+000135a0: 6f73 6564 203d 205b 0a20 2020 2020 2020  osed = [.       
+000135b0: 2020 2020 2020 2020 2022 4973 506f 6c79           "IsPoly
+000135c0: 6c69 6e65 436f 7665 7265 643a 3d22 2c20  lineCovered:=", 
+000135d0: 5472 7565 2c20 2249 7350 6f6c 796c 696e  True, "IsPolylin
+000135e0: 6543 6c6f 7365 643a 3d22 2c20 4661 6c73  eClosed:=", Fals
+000135f0: 650a 2020 2020 2020 2020 2020 2020 5d0a  e.            ].
+00013600: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
+00013610: 7365 6c66 2e5f 6d6f 6465 6c65 722e 4372  self._modeler.Cr
+00013620: 6561 7465 506f 6c79 6c69 6e65 280a 2020  eatePolyline(.  
+00013630: 2020 2020 2020 2020 2020 5b22 4e41 4d45            ["NAME
+00013640: 3a50 6f6c 796c 696e 6550 6172 616d 6574  :PolylineParamet
+00013650: 6572 7322 2c20 2a70 6172 616d 735f 636c  ers", *params_cl
+00013660: 6f73 6564 2c20 706f 696e 7473 5374 722c  osed, pointsStr,
+00013670: 2069 6e64 6578 7353 7472 5d2c 0a20 2020   indexsStr],.   
+00013680: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+00013690: 7474 7269 6275 7465 735f 6172 7261 7928  ttributes_array(
+000136a0: 2a2a 6b77 6172 6773 2929 0a0a 2020 2020  **kwargs))..    
+000136b0: 2020 2020 6966 2063 6c6f 7365 643a 0a20      if closed:. 
+000136c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000136d0: 6e20 506f 6c79 6c69 6e65 286e 616d 652c  n Polyline(name,
+000136e0: 2073 656c 662c 2070 6f69 6e74 7329 0a20   self, points). 
+000136f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00013700: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00013710: 4f70 656e 506f 6c79 6c69 6e65 286e 616d  OpenPolyline(nam
+00013720: 652c 2073 656c 662c 2070 6f69 6e74 7329  e, self, points)
+00013730: 0a0a 2020 2020 6465 6620 6472 6177 5f72  ..    def draw_r
+00013740: 6563 745f 636f 726e 6572 2873 656c 662c  ect_corner(self,
+00013750: 2070 6f73 2c20 785f 7369 7a65 3d30 2c20   pos, x_size=0, 
+00013760: 795f 7369 7a65 3d30 2c20 7a5f 7369 7a65  y_size=0, z_size
+00013770: 3d30 2c20 2a2a 6b77 6172 6773 293a 0a20  =0, **kwargs):. 
+00013780: 2020 2020 2020 2073 697a 6520 3d20 5b78         size = [x
+00013790: 5f73 697a 652c 2079 5f73 697a 652c 207a  _size, y_size, z
+000137a0: 5f73 697a 655d 0a20 2020 2020 2020 2061  _size].        a
+000137b0: 7373 6572 7420 3020 696e 2073 697a 650a  ssert 0 in size.
+000137c0: 2020 2020 2020 2020 6178 6973 203d 2022          axis = "
+000137d0: 5859 5a22 5b73 697a 652e 696e 6465 7828  XYZ"[size.index(
+000137e0: 3029 5d0a 2020 2020 2020 2020 775f 6964  0)].        w_id
+000137f0: 782c 2068 5f69 6478 203d 207b 2758 273a  x, h_idx = {'X':
+00013800: 2028 312c 2032 292c 2027 5927 3a20 2832   (1, 2), 'Y': (2
+00013810: 2c20 3029 2c20 275a 273a 2028 302c 2031  , 0), 'Z': (0, 1
+00013820: 297d 5b61 7869 735d 0a0a 2020 2020 2020  )}[axis]..      
+00013830: 2020 6e61 6d65 203d 2073 656c 662e 5f6d    name = self._m
+00013840: 6f64 656c 6572 2e43 7265 6174 6552 6563  odeler.CreateRec
+00013850: 7461 6e67 6c65 285b 0a20 2020 2020 2020  tangle([.       
+00013860: 2020 2020 2022 4e41 4d45 3a52 6563 7461       "NAME:Recta
+00013870: 6e67 6c65 5061 7261 6d65 7465 7273 222c  ngleParameters",
+00013880: 2022 5853 7461 7274 3a3d 222c 0a20 2020   "XStart:=",.   
+00013890: 2020 2020 2020 2020 2073 7472 2870 6f73           str(pos
+000138a0: 5b30 5d29 2c20 2259 5374 6172 743a 3d22  [0]), "YStart:="
+000138b0: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+000138c0: 7228 706f 735b 315d 292c 2022 5a53 7461  r(pos[1]), "ZSta
+000138d0: 7274 3a3d 222c 0a20 2020 2020 2020 2020  rt:=",.         
+000138e0: 2020 2073 7472 2870 6f73 5b32 5d29 2c20     str(pos[2]), 
+000138f0: 2257 6964 7468 3a3d 222c 0a20 2020 2020  "Width:=",.     
+00013900: 2020 2020 2020 2073 7472 2873 697a 655b         str(size[
+00013910: 775f 6964 785d 292c 2022 4865 6967 6874  w_idx]), "Height
+00013920: 3a3d 222c 0a20 2020 2020 2020 2020 2020  :=",.           
+00013930: 2073 7472 2873 697a 655b 685f 6964 785d   str(size[h_idx]
+00013940: 292c 2022 5768 6963 6841 7869 733a 3d22  ), "WhichAxis:="
+00013950: 2c20 6178 6973 0a20 2020 2020 2020 205d  , axis.        ]
+00013960: 2c20 7365 6c66 2e5f 6174 7472 6962 7574  , self._attribut
+00013970: 6573 5f61 7272 6179 282a 2a6b 7761 7267  es_array(**kwarg
+00013980: 7329 290a 2020 2020 2020 2020 7265 7475  s)).        retu
+00013990: 726e 2052 6563 7428 6e61 6d65 2c20 7365  rn Rect(name, se
+000139a0: 6c66 2c20 706f 732c 2073 697a 6529 0a0a  lf, pos, size)..
+000139b0: 2020 2020 6465 6620 6472 6177 5f72 6563      def draw_rec
+000139c0: 745f 6365 6e74 6572 2873 656c 662c 2070  t_center(self, p
+000139d0: 6f73 2c20 785f 7369 7a65 3d30 2c20 795f  os, x_size=0, y_
+000139e0: 7369 7a65 3d30 2c20 7a5f 7369 7a65 3d30  size=0, z_size=0
+000139f0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+00013a00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013a10: 2043 7265 6174 6573 2061 2072 6563 7461   Creates a recta
+00013a20: 6e67 6c65 2063 656e 7465 7265 6420 6174  ngle centered at
+00013a30: 2070 6f73 205b 7830 2c20 7930 2c20 7a30   pos [x0, y0, z0
+00013a40: 5d2e 0a20 2020 2020 2020 2049 7420 6973  ]..        It is
+00013a50: 2061 7373 756d 6564 2074 6861 7420 7468   assumed that th
+00013a60: 6520 7265 6374 616e 676c 6520 6c69 6573  e rectangle lies
+00013a70: 2070 6172 616c 6c65 6c20 746f 2074 6865   parallel to the
+00013a80: 2078 792c 2079 7a2c 206f 7220 787a 2070   xy, yz, or xz p
+00013a90: 6c61 6e65 2e0a 2020 2020 2020 2020 5573  lane..        Us
+00013aa0: 6572 2069 6e70 7574 7320 3220 6f66 2033  er inputs 2 of 3
+00013ab0: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
+00013ac0: 673a 2078 5f73 697a 652c 2079 5f73 697a  g: x_size, y_siz
+00013ad0: 652c 2061 6e64 207a 5f73 697a 650a 2020  e, and z_size.  
+00013ae0: 2020 2020 2020 6465 7065 6e64 696e 6720        depending 
+00013af0: 6f6e 2068 6f77 2074 6865 2072 6563 7461  on how the recta
+00013b00: 6e67 6c65 2069 7320 6f72 6965 6e74 6564  ngle is oriented
+00013b10: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00013b20: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
+00013b30: 2028 6c69 7374 293a 2043 6f6f 7264 696e   (list): Coordin
+00013b40: 6174 6573 206f 6620 7265 6374 616e 676c  ates of rectangl
+00013b50: 6520 6365 6e74 6572 2c20 5b78 302c 2079  e center, [x0, y
+00013b60: 302c 207a 305d 0a20 2020 2020 2020 2020  0, z0].         
+00013b70: 2020 2078 5f73 697a 6520 2869 6e74 2c20     x_size (int, 
+00013b80: 6f70 7469 6f6e 616c 293a 2057 6964 7468  optional): Width
+00013b90: 2061 6c6f 6e67 2074 6865 2078 2064 6972   along the x dir
+00013ba0: 6563 7469 6f6e 2e20 4465 6661 756c 7473  ection. Defaults
+00013bb0: 2074 6f20 302e 0a20 2020 2020 2020 2020   to 0..         
+00013bc0: 2020 2079 5f73 697a 6520 2869 6e74 2c20     y_size (int, 
+00013bd0: 6f70 7469 6f6e 616c 293a 2020 5769 6474  optional):  Widt
+00013be0: 6820 616c 6f6e 6720 7468 6520 7920 6469  h along the y di
+00013bf0: 7265 6374 696f 6e2e 2044 6566 6175 6c74  rection. Default
+00013c00: 7320 746f 2030 2e0a 2020 2020 2020 2020  s to 0..        
+00013c10: 2020 2020 7a5f 7369 7a65 2028 696e 742c      z_size (int,
+00013c20: 206f 7074 696f 6e61 6c29 3a20 2057 6964   optional):  Wid
+00013c30: 7468 2061 6c6f 6e67 2074 6865 207a 2064  th along the z d
+00013c40: 6972 6563 7469 6f6e 5d2e 2044 6566 6175  irection]. Defau
+00013c50: 6c74 7320 746f 2030 2e0a 2020 2020 2020  lts to 0..      
+00013c60: 2020 2222 220a 2020 2020 2020 2020 636f    """.        co
+00013c70: 726e 6572 5f70 6f73 203d 205b 0a20 2020  rner_pos = [.   
+00013c80: 2020 2020 2020 2020 2076 6172 2870 2920           var(p) 
+00013c90: 2d20 7661 7228 7329 202f 2032 2e20 666f  - var(s) / 2. fo
+00013ca0: 7220 702c 2073 2069 6e20 7a69 7028 706f  r p, s in zip(po
+00013cb0: 732c 205b 785f 7369 7a65 2c20 795f 7369  s, [x_size, y_si
+00013cc0: 7a65 2c20 7a5f 7369 7a65 5d29 0a20 2020  ze, z_size]).   
+00013cd0: 2020 2020 205d 0a20 2020 2020 2020 2072       ].        r
+00013ce0: 6574 7572 6e20 7365 6c66 2e64 7261 775f  eturn self.draw_
+00013cf0: 7265 6374 5f63 6f72 6e65 7228 636f 726e  rect_corner(corn
+00013d00: 6572 5f70 6f73 2c20 785f 7369 7a65 2c20  er_pos, x_size, 
+00013d10: 795f 7369 7a65 2c20 7a5f 7369 7a65 2c0a  y_size, z_size,.
+00013d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d40: 2020 2020 2077 6964 7468 2c0a 2020 2020       width,.    
-00013d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d60: 2020 6865 6967 6874 3d27 302e 316d 6d27    height='0.1mm'
-00013d70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013d80: 2020 2020 2020 2020 7a3d 302c 0a20 2020          z=0,.   
-00013d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013da0: 2020 2077 6972 655f 6469 616d 6574 6572     wire_diameter
-00013db0: 3d22 302e 3032 6d6d 222c 0a20 2020 2020  ="0.02mm",.     
-00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dd0: 204e 756d 5369 6465 733d 362c 0a20 2020   NumSides=6,.   
-00013de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013df0: 2020 202a 2a6b 7761 7267 7329 3a0a 2020     **kwargs):.  
-00013e00: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00013e10: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00013e20: 2020 2020 2020 2020 2020 2020 706f 733a              pos:
-00013e30: 2032 4420 706f 7369 7469 6f6e 2076 6563   2D position vec
-00013e40: 746f 7220 2028 7370 6563 6966 7920 6365  tor  (specify ce
-00013e50: 6e74 6572 2070 6f69 6e74 290a 2020 2020  nter point).    
-00013e60: 2020 2020 2020 2020 2020 2020 6f72 693a              ori:
-00013e70: 2073 686f 756c 6420 6265 206e 6f72 6d65   should be norme
-00013e80: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00013e90: 2020 7a3a 207a 2070 6f73 6974 696f 6e0a    z: z position.
-00013ea0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00013eb0: 4f44 4f20 6372 6561 7465 2057 6972 6562  ODO create Wireb
-00013ec0: 6f6e 6420 636c 6173 730a 2020 2020 2020  ond class.      
-00013ed0: 2020 2020 2020 706f 7369 7469 6f6e 2069        position i
-00013ee0: 7320 7468 6520 6f72 6967 696e 206f 6620  s the origin of 
-00013ef0: 6f6e 6520 706f 696e 740a 2020 2020 2020  one point.      
-00013f00: 2020 2020 2020 6f72 6920 6973 2074 6865        ori is the
-00013f10: 206f 7269 656e 7461 7469 6f6e 2076 6563   orientation vec
-00013f20: 746f 722c 2077 6869 6368 2067 6574 7320  tor, which gets 
-00013f30: 6e6f 726d 616c 697a 6564 0a20 2020 2020  normalized.     
-00013f40: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00013f50: 203d 206e 702e 6172 7261 7928 706f 7329   = np.array(pos)
-00013f60: 0a20 2020 2020 2020 206f 203d 206e 702e  .        o = np.
-00013f70: 6172 7261 7928 6f72 6929 0a20 2020 2020  array(ori).     
-00013f80: 2020 2070 6164 3120 3d20 7020 2d20 6f20     pad1 = p - o 
-00013f90: 2a20 7769 6474 6820 2f20 322e 0a20 2020  * width / 2..   
-00013fa0: 2020 2020 206e 616d 6520 3d20 7365 6c66       name = self
-00013fb0: 2e5f 6d6f 6465 6c65 722e 4372 6561 7465  ._modeler.Create
-00013fc0: 426f 6e64 7769 7265 285b 0a20 2020 2020  Bondwire([.     
-00013fd0: 2020 2020 2020 2022 4e41 4d45 3a42 6f6e         "NAME:Bon
-00013fe0: 6477 6972 6550 6172 616d 6574 6572 7322  dwireParameters"
-00013ff0: 2c20 2257 6972 6554 7970 653a 3d22 2c20  , "WireType:=", 
-00014000: 224c 6f77 222c 2022 5769 7265 4469 616d  "Low", "WireDiam
-00014010: 6574 6572 3a3d 222c 0a20 2020 2020 2020  eter:=",.       
-00014020: 2020 2020 2077 6972 655f 6469 616d 6574       wire_diamet
-00014030: 6572 2c20 224e 756d 5369 6465 733a 3d22  er, "NumSides:="
-00014040: 2c20 4e75 6d53 6964 6573 2c20 2258 5061  , NumSides, "XPa
-00014050: 6450 6f73 3a3d 222c 2070 6164 315b 305d  dPos:=", pad1[0]
-00014060: 2c0a 2020 2020 2020 2020 2020 2020 2259  ,.            "Y
-00014070: 5061 6450 6f73 3a3d 222c 2070 6164 315b  PadPos:=", pad1[
-00014080: 315d 2c20 225a 5061 6450 6f73 3a3d 222c  1], "ZPadPos:=",
-00014090: 207a 2c20 2258 4469 723a 3d22 2c20 6f72   z, "XDir:=", or
-000140a0: 695b 305d 2c20 2259 4469 723a 3d22 2c0a  i[0], "YDir:=",.
-000140b0: 2020 2020 2020 2020 2020 2020 6f72 695b              ori[
-000140c0: 315d 2c20 225a 4469 723a 3d22 2c20 302c  1], "ZDir:=", 0,
-000140d0: 2022 4469 7374 616e 6365 3a3d 222c 2077   "Distance:=", w
-000140e0: 6964 7468 2c20 2268 313a 3d22 2c20 6865  idth, "h1:=", he
-000140f0: 6967 6874 2c20 2268 323a 3d22 2c0a 2020  ight, "h2:=",.  
-00014100: 2020 2020 2020 2020 2020 2230 6d6d 222c            "0mm",
-00014110: 2022 616c 7068 613a 3d22 2c20 2238 3064   "alpha:=", "80d
-00014120: 6567 222c 2022 6265 7461 3a3d 222c 2022  eg", "beta:=", "
-00014130: 3830 6465 6722 2c20 2257 6869 6368 4178  80deg", "WhichAx
-00014140: 6973 3a3d 222c 2022 5a22 0a20 2020 2020  is:=", "Z".     
-00014150: 2020 205d 2c20 7365 6c66 2e5f 6174 7472     ], self._attr
-00014160: 6962 7574 6573 5f61 7272 6179 282a 2a6b  ibutes_array(**k
-00014170: 7761 7267 7329 290a 0a20 2020 2020 2020  wargs))..       
-00014180: 2072 6574 7572 6e20 6e61 6d65 0a0a 2020   return name..  
-00014190: 2020 6465 6620 6472 6177 5f72 6567 696f    def draw_regio
-000141a0: 6e28 7365 6c66 2c0a 2020 2020 2020 2020  n(self,.        
-000141b0: 2020 2020 2020 2020 2020 2020 5061 6464              Padd
-000141c0: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
-000141d0: 2020 2020 2020 2020 2050 6164 6469 6e67           Padding
-000141e0: 5479 7065 3d22 5065 7263 656e 7461 6765  Type="Percentage
-000141f0: 204f 6666 7365 7422 2c0a 2020 2020 2020   Offset",.      
-00014200: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00014210: 6d65 3d27 5265 6769 6f6e 272c 0a20 2020  me='Region',.   
-00014220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014230: 206d 6174 6572 6961 6c3d 225c 2276 6163   material="\"vac
-00014240: 7575 6d5c 2222 293a 0a20 2020 2020 2020  uum\""):.       
-00014250: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
-00014260: 2050 6164 6469 6e67 5479 7065 203a 2027   PaddingType : '
-00014270: 4162 736f 6c75 7465 204f 6666 7365 7427  Absolute Offset'
-00014280: 2c20 2250 6572 6365 6e74 6167 6520 4f66  , "Percentage Of
-00014290: 6673 6574 220a 2020 2020 2020 2020 2222  fset".        ""
-000142a0: 220a 2020 2020 2020 2020 2320 544f 444f  ".        # TODO
-000142b0: 3a20 4164 6420 6f70 7469 6f6e 2074 6f20  : Add option to 
-000142c0: 6d6f 6469 6679 2074 6865 7365 0a20 2020  modify these.   
-000142d0: 2020 2020 2052 6567 696f 6e41 7474 7269       RegionAttri
-000142e0: 6275 7465 7320 3d20 5b0a 2020 2020 2020  butes = [.      
-000142f0: 2020 2020 2020 224e 414d 453a 4174 7472        "NAME:Attr
-00014300: 6962 7574 6573 222c 2022 4e61 6d65 3a3d  ibutes", "Name:=
-00014310: 222c 206e 616d 652c 2022 466c 6167 733a  ", name, "Flags:
-00014320: 3d22 2c20 2257 6972 6566 7261 6d65 2322  =", "Wireframe#"
-00014330: 2c0a 2020 2020 2020 2020 2020 2020 2243  ,.            "C
-00014340: 6f6c 6f72 3a3d 222c 2022 2832 3535 2030  olor:=", "(255 0
-00014350: 2030 2922 2c20 2254 7261 6e73 7061 7265   0)", "Transpare
-00014360: 6e63 793a 3d22 2c20 312c 0a20 2020 2020  ncy:=", 1,.     
-00014370: 2020 2020 2020 2022 5061 7274 436f 6f72         "PartCoor
-00014380: 6469 6e61 7465 5379 7374 656d 3a3d 222c  dinateSystem:=",
-00014390: 2022 476c 6f62 616c 222c 2022 5544 4d49   "Global", "UDMI
-000143a0: 643a 3d22 2c20 2222 2c0a 2020 2020 2020  d:=", "",.      
-000143b0: 2020 2020 2020 2249 7341 6c77 6179 7348        "IsAlwaysH
-000143c0: 6964 656e 3a3d 222c 2046 616c 7365 2c20  iden:=", False, 
-000143d0: 224d 6174 6572 6961 6c56 616c 7565 3a3d  "MaterialValue:=
-000143e0: 222c 206d 6174 6572 6961 6c2c 0a20 2020  ", material,.   
-000143f0: 2020 2020 2020 2020 2022 536f 6c76 6549           "SolveI
-00014400: 6e73 6964 653a 3d22 2c20 5472 7565 0a20  nside:=", True. 
-00014410: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
-00014420: 2020 7365 6c66 2e5f 6d6f 6465 6c65 722e    self._modeler.
-00014430: 4372 6561 7465 5265 6769 6f6e 285b 0a20  CreateRegion([. 
-00014440: 2020 2020 2020 2020 2020 2022 4e41 4d45             "NAME
-00014450: 3a52 6567 696f 6e50 6172 616d 6574 6572  :RegionParameter
-00014460: 7322 2c20 222b 5850 6164 6469 6e67 5479  s", "+XPaddingTy
-00014470: 7065 3a3d 222c 2050 6164 6469 6e67 5479  pe:=", PaddingTy
-00014480: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
-00014490: 222b 5850 6164 6469 6e67 3a3d 222c 2050  "+XPadding:=", P
-000144a0: 6164 6469 6e67 5b30 5d5b 305d 2c20 222d  adding[0][0], "-
-000144b0: 5850 6164 6469 6e67 5479 7065 3a3d 222c  XPaddingType:=",
-000144c0: 2050 6164 6469 6e67 5479 7065 2c0a 2020   PaddingType,.  
-000144d0: 2020 2020 2020 2020 2020 222d 5850 6164            "-XPad
-000144e0: 6469 6e67 3a3d 222c 2050 6164 6469 6e67  ding:=", Padding
-000144f0: 5b30 5d5b 315d 2c20 222b 5950 6164 6469  [0][1], "+YPaddi
-00014500: 6e67 5479 7065 3a3d 222c 2050 6164 6469  ngType:=", Paddi
-00014510: 6e67 5479 7065 2c0a 2020 2020 2020 2020  ngType,.        
-00014520: 2020 2020 222b 5950 6164 6469 6e67 3a3d      "+YPadding:=
-00014530: 222c 2050 6164 6469 6e67 5b31 5d5b 305d  ", Padding[1][0]
-00014540: 2c20 222d 5950 6164 6469 6e67 5479 7065  , "-YPaddingType
-00014550: 3a3d 222c 2050 6164 6469 6e67 5479 7065  :=", PaddingType
-00014560: 2c0a 2020 2020 2020 2020 2020 2020 222d  ,.            "-
-00014570: 5950 6164 6469 6e67 3a3d 222c 2050 6164  YPadding:=", Pad
-00014580: 6469 6e67 5b31 5d5b 315d 2c20 222b 5a50  ding[1][1], "+ZP
-00014590: 6164 6469 6e67 5479 7065 3a3d 222c 2050  addingType:=", P
-000145a0: 6164 6469 6e67 5479 7065 2c0a 2020 2020  addingType,.    
-000145b0: 2020 2020 2020 2020 222b 5a50 6164 6469          "+ZPaddi
-000145c0: 6e67 3a3d 222c 2050 6164 6469 6e67 5b32  ng:=", Padding[2
-000145d0: 5d5b 305d 2c20 222d 5a50 6164 6469 6e67  ][0], "-ZPadding
-000145e0: 5479 7065 3a3d 222c 2050 6164 6469 6e67  Type:=", Padding
-000145f0: 5479 7065 2c0a 2020 2020 2020 2020 2020  Type,.          
-00014600: 2020 222d 5a50 6164 6469 6e67 3a3d 222c    "-ZPadding:=",
-00014610: 2050 6164 6469 6e67 5b32 5d5b 315d 0a20   Padding[2][1]. 
-00014620: 2020 2020 2020 205d 2c20 5265 6769 6f6e         ], Region
-00014630: 4174 7472 6962 7574 6573 290a 0a20 2020  Attributes)..   
-00014640: 2064 6566 2075 6e69 7465 2873 656c 662c   def unite(self,
-00014650: 206e 616d 6573 2c20 6b65 6570 5f6f 7269   names, keep_ori
-00014660: 6769 6e61 6c73 3d46 616c 7365 293a 0a20  ginals=False):. 
-00014670: 2020 2020 2020 2073 656c 662e 5f6d 6f64         self._mod
-00014680: 656c 6572 2e55 6e69 7465 280a 2020 2020  eler.Unite(.    
-00014690: 2020 2020 2020 2020 7365 6c66 2e5f 7365          self._se
-000146a0: 6c65 6374 696f 6e73 5f61 7272 6179 282a  lections_array(*
-000146b0: 6e61 6d65 7329 2c0a 2020 2020 2020 2020  names),.        
-000146c0: 2020 2020 5b22 4e41 4d45 3a55 6e69 7465      ["NAME:Unite
-000146d0: 5061 7261 6d65 7465 7273 222c 2022 4b65  Parameters", "Ke
-000146e0: 6570 4f72 6967 696e 616c 733a 3d22 2c20  epOriginals:=", 
-000146f0: 6b65 6570 5f6f 7269 6769 6e61 6c73 5d29  keep_originals])
-00014700: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014710: 6e61 6d65 735b 305d 0a0a 2020 2020 6465  names[0]..    de
-00014720: 6620 696e 7465 7273 6563 7428 7365 6c66  f intersect(self
-00014730: 2c20 6e61 6d65 732c 206b 6565 705f 6f72  , names, keep_or
-00014740: 6967 696e 616c 733d 4661 6c73 6529 3a0a  iginals=False):.
-00014750: 2020 2020 2020 2020 7365 6c66 2e5f 6d6f          self._mo
-00014760: 6465 6c65 722e 496e 7465 7273 6563 7428  deler.Intersect(
-00014770: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00014780: 662e 5f73 656c 6563 7469 6f6e 735f 6172  f._selections_ar
-00014790: 7261 7928 2a6e 616d 6573 292c 0a20 2020  ray(*names),.   
-000147a0: 2020 2020 2020 2020 205b 224e 414d 453a           ["NAME:
-000147b0: 496e 7465 7273 6563 7450 6172 616d 6574  IntersectParamet
-000147c0: 6572 7322 2c20 224b 6565 704f 7269 6769  ers", "KeepOrigi
-000147d0: 6e61 6c73 3a3d 222c 206b 6565 705f 6f72  nals:=", keep_or
-000147e0: 6967 696e 616c 735d 290a 2020 2020 2020  iginals]).      
-000147f0: 2020 7265 7475 726e 206e 616d 6573 5b30    return names[0
-00014800: 5d0a 0a20 2020 2064 6566 2074 7261 6e73  ]..    def trans
-00014810: 6c61 7465 2873 656c 662c 206e 616d 652c  late(self, name,
-00014820: 2076 6563 746f 7229 3a0a 2020 2020 2020   vector):.      
-00014830: 2020 7365 6c66 2e5f 6d6f 6465 6c65 722e    self._modeler.
-00014840: 4d6f 7665 2873 656c 662e 5f73 656c 6563  Move(self._selec
-00014850: 7469 6f6e 735f 6172 7261 7928 6e61 6d65  tions_array(name
-00014860: 292c 205b 0a20 2020 2020 2020 2020 2020  ), [.           
-00014870: 2022 4e41 4d45 3a54 7261 6e73 6c61 7465   "NAME:Translate
-00014880: 5061 7261 6d65 7465 7273 222c 2022 5472  Parameters", "Tr
-00014890: 616e 736c 6174 6556 6563 746f 7258 3a3d  anslateVectorX:=
-000148a0: 222c 2076 6563 746f 725b 305d 2c0a 2020  ", vector[0],.  
-000148b0: 2020 2020 2020 2020 2020 2254 7261 6e73            "Trans
-000148c0: 6c61 7465 5665 6374 6f72 593a 3d22 2c20  lateVectorY:=", 
-000148d0: 7665 6374 6f72 5b31 5d2c 2022 5472 616e  vector[1], "Tran
-000148e0: 736c 6174 6556 6563 746f 725a 3a3d 222c  slateVectorZ:=",
-000148f0: 2076 6563 746f 725b 325d 0a20 2020 2020   vector[2].     
-00014900: 2020 205d 290a 0a20 2020 2064 6566 2067     ])..    def g
-00014910: 6574 5f62 6f75 6e64 6172 795f 6173 7369  et_boundary_assi
-00014920: 676e 6d65 6e74 2873 656c 662c 2062 6f75  gnment(self, bou
-00014930: 6e64 6172 795f 6e61 6d65 3a20 7374 7229  ndary_name: str)
-00014940: 3a0a 2020 2020 2020 2020 2320 4765 7473  :.        # Gets
-00014950: 2061 206c 6973 7420 6f66 2066 6163 6520   a list of face 
-00014960: 4944 7320 6173 736f 6369 6174 6564 2077  IDs associated w
-00014970: 6974 6820 7468 6520 6769 7665 6e20 626f  ith the given bo
-00014980: 756e 6461 7279 206f 7220 6578 6369 7461  undary or excita
-00014990: 7469 6f6e 2061 7373 6967 6e6d 656e 742e  tion assignment.
-000149a0: 0a20 2020 2020 2020 206f 626a 6563 7473  .        objects
-000149b0: 203d 2073 656c 662e 5f62 6f75 6e64 6172   = self._boundar
-000149c0: 6965 732e 4765 7442 6f75 6e64 6172 7941  ies.GetBoundaryA
-000149d0: 7373 6967 6e6d 656e 7428 626f 756e 6461  ssignment(bounda
-000149e0: 7279 5f6e 616d 6529 0a20 2020 2020 2020  ry_name).       
-000149f0: 2023 2047 6574 7320 616e 206f 626a 6563   # Gets an objec
-00014a00: 7420 6e61 6d65 2063 6f72 7265 7370 6f6e  t name correspon
-00014a10: 6469 6e67 2074 6f20 7468 6520 696e 7075  ding to the inpu
-00014a20: 7420 6661 6365 2069 642e 2052 6574 7572  t face id. Retur
-00014a30: 6e73 2074 6865 206e 616d 6520 6f66 2074  ns the name of t
-00014a40: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-00014a50: 206f 626a 6563 7420 6e61 6d65 2e0a 2020   object name..  
-00014a60: 2020 2020 2020 6f62 6a65 6374 7320 3d20        objects = 
-00014a70: 5b73 656c 662e 5f6d 6f64 656c 6572 2e47  [self._modeler.G
-00014a80: 6574 4f62 6a65 6374 4e61 6d65 4279 4661  etObjectNameByFa
-00014a90: 6365 4944 286b 2920 666f 7220 6b20 696e  ceID(k) for k in
-00014aa0: 206f 626a 6563 7473 5d0a 2020 2020 2020   objects].      
-00014ab0: 2020 7265 7475 726e 206f 626a 6563 7473    return objects
-00014ac0: 0a0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
-00014ad0: 5f50 6572 6645 5f61 7373 6967 6e6d 656e  _PerfE_assignmen
-00014ae0: 7428 7365 6c66 2c20 626f 756e 6461 7279  t(self, boundary
-00014af0: 5f6e 616d 653a 2073 7472 2c20 6f62 6a65  _name: str, obje
-00014b00: 6374 5f6e 616d 6573 3a20 6c69 7374 293a  ct_names: list):
-00014b10: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00014b20: 2020 2020 2020 2020 2054 6869 7320 7769           This wi
-00014b30: 6c6c 2063 7265 6174 6520 6120 6e65 7720  ll create a new 
-00014b40: 626f 756e 6461 7279 2069 6620 6e65 6564  boundary if need
-00014b50: 2c20 616e 6420 7769 6c6c 0a20 2020 2020  , and will.     
-00014b60: 2020 2020 2020 206f 7468 6572 7769 7365         otherwise
-00014b70: 2061 7070 656e 6420 6769 7665 6e20 6e61   append given na
-00014b80: 6d65 7320 746f 2061 6e20 6578 6973 7469  mes to an existi
-00014b90: 6e67 2062 6f75 6e64 6172 790a 2020 2020  ng boundary.    
-00014ba0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00014bb0: 2320 656e 666f 7263 650a 2020 2020 2020  # enforce.      
-00014bc0: 2020 626f 756e 6461 7279 5f6e 616d 6520    boundary_name 
-00014bd0: 3d20 7374 7228 626f 756e 6461 7279 5f6e  = str(boundary_n
-00014be0: 616d 6529 0a20 2020 2020 2020 2069 6620  ame).        if 
-00014bf0: 6973 696e 7374 616e 6365 286f 626a 6563  isinstance(objec
-00014c00: 745f 6e61 6d65 732c 2073 7472 293a 0a20  t_names, str):. 
-00014c10: 2020 2020 2020 2020 2020 206f 626a 6563             objec
-00014c20: 745f 6e61 6d65 7320 3d20 5b6f 626a 6563  t_names = [objec
-00014c30: 745f 6e61 6d65 735d 0a20 2020 2020 2020  t_names].       
-00014c40: 206f 626a 6563 745f 6e61 6d65 7320 3d20   object_names = 
-00014c50: 6c69 7374 286f 626a 6563 745f 6e61 6d65  list(object_name
-00014c60: 7329 2020 2320 656e 666f 7263 6520 6c69  s)  # enforce li
-00014c70: 7374 0a0a 2020 2020 2020 2020 2320 646f  st..        # do
-00014c80: 2061 6374 7561 6c20 776f 726b 0a20 2020   actual work.   
-00014c90: 2020 2020 2069 6620 626f 756e 6461 7279       if boundary
-00014ca0: 5f6e 616d 6520 6e6f 7420 696e 2073 656c  _name not in sel
-00014cb0: 662e 5f62 6f75 6e64 6172 6965 732e 4765  f._boundaries.Ge
-00014cc0: 7442 6f75 6e64 6172 6965 7328 0a20 2020  tBoundaries(.   
-00014cd0: 2020 2020 2029 3a20 2023 2047 6574 426f       ):  # GetBo
-00014ce0: 756e 6461 7269 6573 4f66 5479 7065 2822  undariesOfType("
-00014cf0: 5065 7266 6563 7420 4522 290a 2020 2020  Perfect E").    
-00014d00: 2020 2020 2020 2020 2320 6e65 6564 2074          # need t
-00014d10: 6f20 6d61 6b65 2061 206e 6577 2062 6f75  o make a new bou
-00014d20: 6e64 6172 790a 2020 2020 2020 2020 2020  ndary.          
-00014d30: 2020 7365 6c66 2e61 7373 6967 6e5f 7065    self.assign_pe
-00014d40: 7266 6563 745f 4528 6f62 6a65 6374 5f6e  rfect_E(object_n
-00014d50: 616d 6573 2c20 6e61 6d65 3d62 6f75 6e64  ames, name=bound
-00014d60: 6172 795f 6e61 6d65 290a 2020 2020 2020  ary_name).      
-00014d70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00014d80: 2020 2020 2320 6e65 6564 2074 6f20 6170      # need to ap
-00014d90: 7065 6e64 0a20 2020 2020 2020 2020 2020  pend.           
-00014da0: 206f 626a 6563 7473 203d 206c 6973 7428   objects = list(
-00014db0: 7365 6c66 2e67 6574 5f62 6f75 6e64 6172  self.get_boundar
-00014dc0: 795f 6173 7369 676e 6d65 6e74 2862 6f75  y_assignment(bou
-00014dd0: 6e64 6172 795f 6e61 6d65 2929 0a20 2020  ndary_name)).   
-00014de0: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
-00014df0: 6f75 6e64 6172 6965 732e 5265 6173 7369  oundaries.Reassi
-00014e00: 676e 426f 756e 6461 7279 285b 0a20 2020  gnBoundary([.   
-00014e10: 2020 2020 2020 2020 2020 2020 2022 4e41               "NA
-00014e20: 4d45 3a22 202b 2062 6f75 6e64 6172 795f  ME:" + boundary_
-00014e30: 6e61 6d65 2c20 224f 626a 6563 7473 3a3d  name, "Objects:=
-00014e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00014e50: 2020 206c 6973 7428 7365 7428 6f62 6a65     list(set(obje
-00014e60: 6374 7320 2b20 6f62 6a65 6374 5f6e 616d  cts + object_nam
-00014e70: 6573 2929 0a20 2020 2020 2020 2020 2020  es)).           
-00014e80: 205d 290a 0a20 2020 2064 6566 2061 7070   ])..    def app
-00014e90: 656e 645f 6d65 7368 2873 656c 662c 206d  end_mesh(self, m
-00014ea0: 6573 685f 6e61 6d65 3a20 7374 722c 206f  esh_name: str, o
-00014eb0: 626a 6563 745f 6e61 6d65 733a 206c 6973  bject_names: lis
-00014ec0: 742c 206f 6c64 5f6f 626a 733a 206c 6973  t, old_objs: lis
-00014ed0: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
-00014ee0: 2020 2020 2020 202a 2a6b 7761 7267 7329         **kwargs)
-00014ef0: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
-00014f00: 2020 2020 2020 5468 6973 2077 696c 6c20        This will 
-00014f10: 6372 6561 7465 2061 206e 6577 2062 6f75  create a new bou
-00014f20: 6e64 6172 7920 6966 206e 6565 642c 2061  ndary if need, a
-00014f30: 6e64 2077 696c 6c0a 2020 2020 2020 2020  nd will.        
-00014f40: 6f74 6865 7277 6973 6520 6170 7065 6e64  otherwise append
-00014f50: 2067 6976 656e 206e 616d 6573 2074 6f20   given names to 
-00014f60: 616e 2065 7869 7374 696e 6720 626f 756e  an existing boun
-00014f70: 6461 7279 0a20 2020 2020 2020 206f 6c64  dary.        old
-00014f80: 5f6f 626a 203d 2063 6972 632e 5f6d 6573  _obj = circ._mes
-00014f90: 685f 6173 7369 676e 0a20 2020 2020 2020  h_assign.       
-00014fa0: 2027 2727 0a20 2020 2020 2020 206d 6573   '''.        mes
-00014fb0: 685f 6e61 6d65 203d 2073 7472 286d 6573  h_name = str(mes
-00014fc0: 685f 6e61 6d65 290a 2020 2020 2020 2020  h_name).        
-00014fd0: 6966 2069 7369 6e73 7461 6e63 6528 6f62  if isinstance(ob
-00014fe0: 6a65 6374 5f6e 616d 6573 2c20 7374 7229  ject_names, str)
-00014ff0: 3a0a 2020 2020 2020 2020 2020 2020 6f62  :.            ob
-00015000: 6a65 6374 5f6e 616d 6573 203d 205b 6f62  ject_names = [ob
-00015010: 6a65 6374 5f6e 616d 6573 5d0a 2020 2020  ject_names].    
-00015020: 2020 2020 6f62 6a65 6374 5f6e 616d 6573      object_names
-00015030: 203d 206c 6973 7428 6f62 6a65 6374 5f6e   = list(object_n
-00015040: 616d 6573 2920 2023 2065 6e66 6f72 6365  ames)  # enforce
-00015050: 206c 6973 740a 0a20 2020 2020 2020 2069   list..        i
-00015060: 6620 6d65 7368 5f6e 616d 6520 6e6f 7420  f mesh_name not 
-00015070: 696e 2073 656c 662e 6d65 7368 5f67 6574  in self.mesh_get
-00015080: 5f6e 616d 6573 280a 2020 2020 2020 2020  _names(.        
-00015090: 293a 2020 2320 6e65 6564 2074 6f20 6d61  ):  # need to ma
-000150a0: 6b65 2061 206e 6577 2062 6f75 6e64 6172  ke a new boundar
-000150b0: 790a 2020 2020 2020 2020 2020 2020 6f62  y.            ob
-000150c0: 6a73 203d 206f 626a 6563 745f 6e61 6d65  js = object_name
-000150d0: 730a 2020 2020 2020 2020 2020 2020 7365  s.            se
-000150e0: 6c66 2e6d 6573 685f 6c65 6e67 7468 286d  lf.mesh_length(m
-000150f0: 6573 685f 6e61 6d65 2c20 6f62 6a65 6374  esh_name, object
-00015100: 5f6e 616d 6573 2c20 2a2a 6b77 6172 6773  _names, **kwargs
-00015110: 290a 2020 2020 2020 2020 656c 7365 3a20  ).        else: 
-00015120: 2023 206e 6565 6420 746f 2061 7070 656e   # need to appen
-00015130: 640a 2020 2020 2020 2020 2020 2020 6f62  d.            ob
-00015140: 6a73 203d 206c 6973 7428 7365 7428 6f6c  js = list(set(ol
-00015150: 645f 6f62 6a73 202b 206f 626a 6563 745f  d_objs + object_
-00015160: 6e61 6d65 7329 290a 2020 2020 2020 2020  names)).        
-00015170: 2020 2020 7365 6c66 2e6d 6573 685f 7265      self.mesh_re
-00015180: 6173 7369 676e 286d 6573 685f 6e61 6d65  assign(mesh_name
-00015190: 2c20 6f62 6a73 290a 0a20 2020 2020 2020  , objs)..       
-000151a0: 2072 6574 7572 6e20 6f62 6a73 0a0a 2020   return objs..  
-000151b0: 2020 6465 6620 6173 7369 676e 5f70 6572    def assign_per
-000151c0: 6665 6374 5f45 2873 656c 662c 206f 626a  fect_E(self, obj
-000151d0: 3a20 4c69 7374 5b73 7472 5d2c 206e 616d  : List[str], nam
-000151e0: 653a 2073 7472 203d 2027 5065 7266 4527  e: str = 'PerfE'
-000151f0: 293a 0a20 2020 2020 2020 2027 2727 0a20  ):.        '''. 
-00015200: 2020 2020 2020 2041 7373 6967 6e20 6120         Assign a 
-00015210: 626f 756e 6461 7279 2063 6f6e 6469 7469  boundary conditi
-00015220: 6f6e 2074 6f20 6120 6c69 7374 206f 6620  on to a list of 
-00015230: 6f62 6a65 6374 732e 0a0a 2020 2020 2020  objects...      
-00015240: 2020 4172 673a 0a20 2020 2020 2020 2020    Arg:.         
-00015250: 2020 206f 626a 7320 284c 6973 745b 7374     objs (List[st
-00015260: 725d 293a 2054 616b 6573 2061 206e 616d  r]): Takes a nam
-00015270: 6520 6f66 2061 6e20 6f62 6a65 6374 206f  e of an object o
-00015280: 7220 6120 6c69 7374 206f 6620 6f62 6a65  r a list of obje
-00015290: 6374 206e 616d 6573 2e0a 2020 2020 2020  ct names..      
-000152a0: 2020 2020 2020 6e61 6d65 2873 7472 293a        name(str):
-000152b0: 2049 6620 606e 616d 6560 2069 7320 6e6f   If `name` is no
-000152c0: 7420 7370 6563 6966 6965 6420 6050 6572  t specified `Per
-000152d0: 6645 6020 6973 2061 7070 656e 6465 6420  fE` is appended 
-000152e0: 746f 206f 626a 6563 7420 6e61 6d65 2066  to object name f
-000152f0: 6f72 2074 6865 206e 616d 652e 0a20 2020  or the name..   
-00015300: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00015310: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
-00015320: 6365 286f 626a 2c20 6c69 7374 293a 0a20  ce(obj, list):. 
-00015330: 2020 2020 2020 2020 2020 206f 626a 203d             obj =
-00015340: 205b 6f62 6a5d 0a20 2020 2020 2020 2020   [obj].         
-00015350: 2020 2069 6620 6e61 6d65 203d 3d20 2750     if name == 'P
-00015360: 6572 6645 273a 0a20 2020 2020 2020 2020  erfE':.         
-00015370: 2020 2020 2020 206e 616d 6520 3d20 7374         name = st
-00015380: 7228 6f62 6a29 202b 2027 5f27 202b 206e  r(obj) + '_' + n
-00015390: 616d 650a 2020 2020 2020 2020 6e61 6d65  ame.        name
-000153a0: 203d 2069 6e63 7265 6d65 6e74 5f6e 616d   = increment_nam
-000153b0: 6528 6e61 6d65 2c20 7365 6c66 2e5f 626f  e(name, self._bo
-000153c0: 756e 6461 7269 6573 2e47 6574 426f 756e  undaries.GetBoun
-000153d0: 6461 7269 6573 2829 290a 2020 2020 2020  daries()).      
-000153e0: 2020 7365 6c66 2e5f 626f 756e 6461 7269    self._boundari
-000153f0: 6573 2e41 7373 6967 6e50 6572 6665 6374  es.AssignPerfect
-00015400: 4528 0a20 2020 2020 2020 2020 2020 205b  E(.            [
-00015410: 224e 414d 453a 2220 2b20 6e61 6d65 2c20  "NAME:" + name, 
-00015420: 224f 626a 6563 7473 3a3d 222c 206f 626a  "Objects:=", obj
-00015430: 2c20 2249 6e66 4772 6f75 6e64 506c 616e  , "InfGroundPlan
-00015440: 653a 3d22 2c20 4661 6c73 655d 290a 0a20  e:=", False]).. 
-00015450: 2020 2064 6566 205f 6d61 6b65 5f6c 756d     def _make_lum
-00015460: 7065 645f 726c 6328 7365 6c66 2c20 722c  ped_rlc(self, r,
-00015470: 206c 2c20 632c 2073 7461 7274 2c20 656e   l, c, start, en
-00015480: 642c 206f 626a 5f61 7272 2c20 6e61 6d65  d, obj_arr, name
-00015490: 3d22 4c75 6d70 524c 4322 293a 0a20 2020  ="LumpRLC"):.   
-000154a0: 2020 2020 206e 616d 6520 3d20 696e 6372       name = incr
-000154b0: 656d 656e 745f 6e61 6d65 286e 616d 652c  ement_name(name,
-000154c0: 2073 656c 662e 5f62 6f75 6e64 6172 6965   self._boundarie
-000154d0: 732e 4765 7442 6f75 6e64 6172 6965 7328  s.GetBoundaries(
-000154e0: 2929 0a20 2020 2020 2020 2070 6172 616d  )).        param
-000154f0: 7320 3d20 5b22 4e41 4d45 3a22 202b 206e  s = ["NAME:" + n
-00015500: 616d 655d 0a20 2020 2020 2020 2070 6172  ame].        par
-00015510: 616d 7320 2b3d 206f 626a 5f61 7272 0a20  ams += obj_arr. 
-00015520: 2020 2020 2020 2070 6172 616d 732e 6170         params.ap
-00015530: 7065 6e64 285b 0a20 2020 2020 2020 2020  pend([.         
-00015540: 2020 2022 4e41 4d45 3a43 7572 7265 6e74     "NAME:Current
-00015550: 4c69 6e65 222c 0a20 2020 2020 2020 2020  Line",.         
-00015560: 2020 2023 2066 6f72 2073 6f6d 6520 7265     # for some re
-00015570: 6173 6f6e 2068 6572 6520 6974 2073 6565  ason here it see
-00015580: 6d73 2074 6f20 7377 6974 6368 2074 6f20  ms to switch to 
-00015590: 7573 6520 7468 6520 6d6f 6465 6c20 756e  use the model un
-000155a0: 6974 732c 2072 6174 6865 7220 7468 616e  its, rather than
-000155b0: 206d 6574 6572 730a 2020 2020 2020 2020   meters.        
-000155c0: 2020 2020 2253 7461 7274 3a3d 222c 0a20      "Start:=",. 
-000155d0: 2020 2020 2020 2020 2020 2066 6978 5f75             fix_u
-000155e0: 6e69 7473 2873 7461 7274 2c20 756e 6974  nits(start, unit
-000155f0: 5f61 7373 756d 6564 3d4c 454e 4754 485f  _assumed=LENGTH_
-00015600: 554e 4954 292c 0a20 2020 2020 2020 2020  UNIT),.         
-00015610: 2020 2022 456e 643a 3d22 2c0a 2020 2020     "End:=",.    
-00015620: 2020 2020 2020 2020 6669 785f 756e 6974          fix_unit
-00015630: 7328 656e 642c 2075 6e69 745f 6173 7375  s(end, unit_assu
-00015640: 6d65 643d 4c45 4e47 5448 5f55 4e49 5429  med=LENGTH_UNIT)
-00015650: 0a20 2020 2020 2020 205d 290a 2020 2020  .        ]).    
-00015660: 2020 2020 7061 7261 6d73 202b 3d20 5b0a      params += [.
-00015670: 2020 2020 2020 2020 2020 2020 2255 7365              "Use
-00015680: 5265 7369 7374 3a3d 222c 2072 2021 3d20  Resist:=", r != 
-00015690: 302c 2022 5265 7369 7374 616e 6365 3a3d  0, "Resistance:=
-000156a0: 222c 2072 2c20 2255 7365 496e 6475 6374  ", r, "UseInduct
-000156b0: 3a3d 222c 206c 2021 3d20 302c 0a20 2020  :=", l != 0,.   
-000156c0: 2020 2020 2020 2020 2022 496e 6475 6374           "Induct
-000156d0: 616e 6365 3a3d 222c 206c 2c20 2255 7365  ance:=", l, "Use
-000156e0: 4361 703a 3d22 2c20 6320 213d 2030 2c20  Cap:=", c != 0, 
-000156f0: 2243 6170 6163 6974 616e 6365 3a3d 222c  "Capacitance:=",
-00015700: 2063 0a20 2020 2020 2020 205d 0a20 2020   c.        ].   
-00015710: 2020 2020 2073 656c 662e 5f62 6f75 6e64       self._bound
-00015720: 6172 6965 732e 4173 7369 676e 4c75 6d70  aries.AssignLump
-00015730: 6564 524c 4328 7061 7261 6d73 290a 0a20  edRLC(params).. 
-00015740: 2020 2064 6566 205f 6d61 6b65 5f6c 756d     def _make_lum
-00015750: 7065 645f 706f 7274 2873 656c 662c 0a20  ped_port(self,. 
-00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015770: 2020 2020 2020 2020 2073 7461 7274 2c0a           start,.
-00015780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015790: 2020 2020 2020 2020 2020 656e 642c 0a20            end,. 
-000157a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157b0: 2020 2020 2020 2020 206f 626a 5f61 7272           obj_arr
-000157c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000157d0: 2020 2020 2020 2020 2020 2020 7a30 3d22              z0="
-000157e0: 3530 6f68 6d22 2c0a 2020 2020 2020 2020  50ohm",.        
-000157f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015800: 2020 6e61 6d65 3d22 4c75 6d70 506f 7274    name="LumpPort
-00015810: 2229 3a0a 2020 2020 2020 2020 7374 6172  "):.        star
-00015820: 7420 3d20 6669 785f 756e 6974 7328 7374  t = fix_units(st
-00015830: 6172 742c 2075 6e69 745f 6173 7375 6d65  art, unit_assume
-00015840: 643d 4c45 4e47 5448 5f55 4e49 5429 0a20  d=LENGTH_UNIT). 
-00015850: 2020 2020 2020 2065 6e64 203d 2066 6978         end = fix
-00015860: 5f75 6e69 7473 2865 6e64 2c20 756e 6974  _units(end, unit
-00015870: 5f61 7373 756d 6564 3d4c 454e 4754 485f  _assumed=LENGTH_
-00015880: 554e 4954 290a 0a20 2020 2020 2020 206e  UNIT)..        n
-00015890: 616d 6520 3d20 696e 6372 656d 656e 745f  ame = increment_
-000158a0: 6e61 6d65 286e 616d 652c 2073 656c 662e  name(name, self.
-000158b0: 5f62 6f75 6e64 6172 6965 732e 4765 7442  _boundaries.GetB
-000158c0: 6f75 6e64 6172 6965 7328 2929 0a20 2020  oundaries()).   
-000158d0: 2020 2020 2070 6172 616d 7320 3d20 5b22       params = ["
-000158e0: 4e41 4d45 3a22 202b 206e 616d 655d 0a20  NAME:" + name]. 
-000158f0: 2020 2020 2020 2070 6172 616d 7320 2b3d         params +=
-00015900: 206f 626a 5f61 7272 0a20 2020 2020 2020   obj_arr.       
-00015910: 2070 6172 616d 7320 2b3d 205b 0a20 2020   params += [.   
-00015920: 2020 2020 2020 2020 2022 5265 6e6f 726d           "Renorm
-00015930: 616c 697a 6541 6c6c 5465 726d 696e 616c  alizeAllTerminal
-00015940: 733a 3d22 2c20 5472 7565 2c20 2244 6f44  s:=", True, "DoD
-00015950: 6565 6d62 6564 3a3d 222c 2046 616c 7365  eembed:=", False
-00015960: 2c0a 2020 2020 2020 2020 2020 2020 5b0a  ,.            [.
-00015970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015980: 224e 414d 453a 4d6f 6465 7322 2c0a 2020  "NAME:Modes",.  
-00015990: 2020 2020 2020 2020 2020 2020 2020 5b0a                [.
-000159a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159b0: 2020 2020 224e 414d 453a 4d6f 6465 3122      "NAME:Mode1"
-000159c0: 2c20 224d 6f64 654e 756d 3a3d 222c 2031  , "ModeNum:=", 1
-000159d0: 2c20 2255 7365 496e 744c 696e 653a 3d22  , "UseIntLine:="
-000159e0: 2c20 5472 7565 2c0a 2020 2020 2020 2020  , True,.        
-000159f0: 2020 2020 2020 2020 2020 2020 5b22 4e41              ["NA
-00015a00: 4d45 3a49 6e74 4c69 6e65 222c 2022 5374  ME:IntLine", "St
-00015a10: 6172 743a 3d22 2c20 7374 6172 742c 2022  art:=", start, "
-00015a20: 456e 643a 3d22 2c0a 2020 2020 2020 2020  End:=",.        
-00015a30: 2020 2020 2020 2020 2020 2020 2065 6e64               end
-00015a40: 5d2c 2022 4368 6172 496d 703a 3d22 2c20  ], "CharImp:=", 
-00015a50: 225a 7069 222c 2022 416c 6967 6e6d 656e  "Zpi", "Alignmen
-00015a60: 7447 726f 7570 3a3d 222c 2030 2c0a 2020  tGroup:=", 0,.  
-00015a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a80: 2020 2252 656e 6f72 6d49 6d70 3a3d 222c    "RenormImp:=",
-00015a90: 2022 3530 6f68 6d22 0a20 2020 2020 2020   "50ohm".       
-00015aa0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00015ab0: 2020 2020 2020 205d 2c20 2253 686f 7752         ], "ShowR
-00015ac0: 6570 6f72 7465 7246 696c 7465 723a 3d22  eporterFilter:="
-00015ad0: 2c20 4661 6c73 652c 2022 5265 706f 7274  , False, "Report
-00015ae0: 6572 4669 6c74 6572 3a3d 222c 205b 5472  erFilter:=", [Tr
-00015af0: 7565 5d2c 0a20 2020 2020 2020 2020 2020  ue],.           
-00015b00: 2022 4675 6c6c 5265 7369 7374 616e 6365   "FullResistance
-00015b10: 3a3d 222c 207a 302c 2022 4675 6c6c 5265  :=", z0, "FullRe
-00015b20: 6163 7461 6e63 653a 3d22 2c20 2230 6f68  actance:=", "0oh
-00015b30: 6d22 0a20 2020 2020 2020 205d 0a0a 2020  m".        ]..  
-00015b40: 2020 2020 2020 7365 6c66 2e5f 626f 756e        self._boun
-00015b50: 6461 7269 6573 2e41 7373 6967 6e4c 756d  daries.AssignLum
-00015b60: 7065 6450 6f72 7428 7061 7261 6d73 290a  pedPort(params).
-00015b70: 0a20 2020 2064 6566 2067 6574 5f66 6163  .    def get_fac
-00015b80: 655f 6964 7328 7365 6c66 2c20 6f62 6a29  e_ids(self, obj)
-00015b90: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00015ba0: 2073 656c 662e 5f6d 6f64 656c 6572 2e47   self._modeler.G
-00015bb0: 6574 4661 6365 4944 7328 6f62 6a29 0a0a  etFaceIDs(obj)..
-00015bc0: 2020 2020 6465 6620 6765 745f 6f62 6a65      def get_obje
-00015bd0: 6374 5f6e 616d 655f 6279 5f66 6163 655f  ct_name_by_face_
-00015be0: 6964 2873 656c 662c 2049 443a 2073 7472  id(self, ID: str
-00015bf0: 293a 0a20 2020 2020 2020 2027 2727 2047  ):.        ''' G
-00015c00: 6574 7320 616e 206f 626a 6563 7420 6e61  ets an object na
-00015c10: 6d65 2063 6f72 7265 7370 6f6e 6469 6e67  me corresponding
-00015c20: 2074 6f20 7468 6520 696e 7075 7420 6661   to the input fa
-00015c30: 6365 2069 642e 2027 2727 0a20 2020 2020  ce id. '''.     
-00015c40: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00015c50: 6d6f 6465 6c65 722e 4765 744f 626a 6563  modeler.GetObjec
-00015c60: 744e 616d 6542 7946 6163 6549 4428 4944  tNameByFaceID(ID
-00015c70: 290a 0a20 2020 2064 6566 2067 6574 5f76  )..    def get_v
-00015c80: 6572 7465 785f 6964 7328 7365 6c66 2c20  ertex_ids(self, 
-00015c90: 6f62 6a29 3a0a 2020 2020 2020 2020 2222  obj):.        ""
-00015ca0: 220a 2020 2020 2020 2020 2020 2020 4765  ".            Ge
-00015cb0: 7420 7468 6520 7665 7274 6578 2049 4473  t the vertex IDs
-00015cc0: 206f 6620 6769 7665 6e20 616e 206f 626a   of given an obj
-00015cd0: 6563 7420 6e61 6d65 0a20 2020 2020 2020  ect name.       
-00015ce0: 2020 2020 206f 5665 7274 6578 4944 7320       oVertexIDs 
-00015cf0: 3d20 6f45 6469 746f 722e 4765 7456 6572  = oEditor.GetVer
-00015d00: 7465 7849 4473 4672 6f6d 4f62 6a65 6374  texIDsFromObject
-00015d10: 28e2 809c 426f 7831 e280 9d29 0a20 2020  (...Box1...).   
-00015d20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00015d30: 2072 6574 7572 6e20 7365 6c66 2e5f 6d6f   return self._mo
-00015d40: 6465 6c65 722e 4765 7456 6572 7465 7849  deler.GetVertexI
-00015d50: 4473 4672 6f6d 4f62 6a65 6374 286f 626a  DsFromObject(obj
-00015d60: 290a 0a20 2020 2064 6566 2065 7661 6c5f  )..    def eval_
-00015d70: 6578 7072 2873 656c 662c 2065 7870 722c  expr(self, expr,
-00015d80: 2075 6e69 7473 3d22 6d6d 2229 3a0a 2020   units="mm"):.  
-00015d90: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
-00015da0: 6e73 7461 6e63 6528 6578 7072 2c20 7374  nstance(expr, st
-00015db0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00015dc0: 7265 7475 726e 2065 7870 720a 2020 2020  return expr.    
-00015dd0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00015de0: 7061 7265 6e74 2e65 7661 6c5f 6578 7072  parent.eval_expr
-00015df0: 2865 7870 722c 2075 6e69 7473 290a 0a20  (expr, units).. 
-00015e00: 2020 2064 6566 2067 6574 5f6f 626a 6563     def get_objec
-00015e10: 7473 5f69 6e5f 6772 6f75 7028 7365 6c66  ts_in_group(self
-00015e20: 2c20 6772 6f75 7029 3a0a 2020 2020 2020  , group):.      
-00015e30: 2020 2222 220a 2020 2020 2020 2020 5573    """.        Us
-00015e40: 653a 2020 2020 2020 2020 2020 2020 2020  e:              
-00015e50: 5265 7475 726e 7320 7468 6520 6f62 6a65  Returns the obje
-00015e60: 6374 7320 666f 7220 7468 6520 7370 6563  cts for the spec
-00015e70: 6966 6965 6420 6772 6f75 702e 0a20 2020  ified group..   
-00015e80: 2020 2020 2052 6574 7572 6e20 5661 6c75       Return Valu
-00015e90: 653a 2020 2020 5468 6520 6f62 6a65 6374  e:    The object
-00015ea0: 7320 696e 2074 6865 2067 726f 7570 2e0a  s in the group..
-00015eb0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00015ec0: 7273 3a20 2020 2020 203c 6772 6f75 704e  rs:      <groupN
-00015ed0: 616d 653e 2020 5479 7065 3a20 3c73 7472  ame>  Type: <str
-00015ee0: 696e 673e 0a20 2020 2020 2020 204f 6e65  ing>.        One
-00015ef0: 206f 6620 203c 6d61 7465 7269 616c 4e61   of  <materialNa
-00015f00: 6d65 3e2c 203c 6173 7369 676e 6d65 6e74  me>, <assignment
-00015f10: 4e61 6d65 3e2c 2022 4e6f 6e20 4d6f 6465  Name>, "Non Mode
-00015f20: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
-00015f30: 2020 2020 2253 6f6c 6964 7322 2c20 2255      "Solids", "U
-00015f40: 6e63 6c61 7373 69c2 ad66 6965 6422 2c20  nclassi..fied", 
-00015f50: 2253 6865 6574 7322 2c20 224c 696e 6573  "Sheets", "Lines
-00015f60: 220a 2020 2020 2020 2020 2222 220a 2020  ".        """.  
-00015f70: 2020 2020 2020 6966 2073 656c 662e 5f6d        if self._m
-00015f80: 6f64 656c 6572 3a0a 2020 2020 2020 2020  odeler:.        
-00015f90: 2020 2020 7265 7475 726e 206c 6973 7428      return list(
-00015fa0: 7365 6c66 2e5f 6d6f 6465 6c65 722e 4765  self._modeler.Ge
-00015fb0: 744f 626a 6563 7473 496e 4772 6f75 7028  tObjectsInGroup(
-00015fc0: 6772 6f75 7029 290a 2020 2020 2020 2020  group)).        
-00015fd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00015fe0: 2020 7265 7475 726e 206c 6973 7428 290a    return list().
-00015ff0: 0a20 2020 2064 6566 2073 6574 5f77 6f72  .    def set_wor
-00016000: 6b69 6e67 5f63 6f6f 7264 696e 6174 655f  king_coordinate_
-00016010: 7379 7374 656d 2873 656c 662c 2063 735f  system(self, cs_
-00016020: 6e61 6d65 3d22 476c 6f62 616c 2229 3a0a  name="Global"):.
-00016030: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00016040: 2020 2020 5573 653a 2020 2020 2020 2020      Use:        
-00016050: 2020 2020 2020 2020 2020 2053 6574 7320             Sets 
-00016060: 7468 6520 776f 726b 696e 6720 636f 6f72  the working coor
-00016070: 6469 6e61 7465 2073 7973 7465 6d2e 0a20  dinate system.. 
-00016080: 2020 2020 2020 2043 6f6d 6d61 6e64 3a20         Command: 
-00016090: 2020 2020 2020 2020 4d6f 6465 6c65 723e          Modeler>
-000160a0: 436f 6f72 6469 6e61 7465 2053 7973 7465  Coordinate Syste
-000160b0: 6d3e 5365 7420 576f 726b 696e 6720 4353  m>Set Working CS
-000160c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000160d0: 2020 2020 2073 656c 662e 5f6d 6f64 656c       self._model
-000160e0: 6572 2e53 6574 5743 5328 5b0a 2020 2020  er.SetWCS([.    
-000160f0: 2020 2020 2020 2020 224e 414d 453a 5365          "NAME:Se
-00016100: 7457 4353 2050 6172 616d 6574 6572 222c  tWCS Parameter",
-00016110: 0a20 2020 2020 2020 2020 2020 2022 576f  .            "Wo
-00016120: 726b 696e 6720 436f 6f72 6469 6e61 7465  rking Coordinate
-00016130: 2053 7973 7465 6d3a 3d22 2c0a 2020 2020   System:=",.    
-00016140: 2020 2020 2020 2020 6373 5f6e 616d 652c          cs_name,
-00016150: 0a20 2020 2020 2020 2020 2020 2022 5265  .            "Re
-00016160: 6769 6f6e 4465 7043 534f 6b3a 3d22 2c0a  gionDepCSOk:=",.
-00016170: 2020 2020 2020 2020 2020 2020 4661 6c73              Fals
-00016180: 6520 2023 2074 6869 7320 6f6e 6520 6973  e  # this one is
-00016190: 2070 726f 6220 6e6f 7420 6e65 6564 6564   prob not needed
-000161a0: 2c20 6275 7420 636f 6d65 7320 7769 7468  , but comes with
-000161b0: 2074 6865 2072 6563 6f72 6420 746f 6f6c   the record tool
-000161c0: 0a20 2020 2020 2020 205d 290a 0a20 2020  .        ])..   
-000161d0: 2064 6566 2063 7265 6174 655f 7265 6c61   def create_rela
-000161e0: 7469 7665 5f63 6f6f 7269 6e61 7465 5f73  tive_coorinate_s
-000161f0: 7973 7465 6d5f 626f 7468 2873 656c 662c  ystem_both(self,
-00016200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016220: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00016230: 735f 6e61 6d65 2c0a 2020 2020 2020 2020  s_name,.        
-00016240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016260: 2020 2020 2020 6f72 6967 696e 3d5b 2230        origin=["0
-00016270: 756d 222c 2022 3075 6d22 2c20 2230 756d  um", "0um", "0um
-00016280: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-00016290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162b0: 2020 5841 7869 7356 6563 3d5b 2231 756d    XAxisVec=["1um
-000162c0: 222c 2022 3075 6d22 2c20 2230 756d 225d  ", "0um", "0um"]
-000162d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000162e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016300: 5941 7869 7356 6563 3d5b 2230 756d 222c  YAxisVec=["0um",
-00016310: 2022 3175 6d22 2c20 2230 756d 225d 293a   "1um", "0um"]):
-00016320: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016330: 2020 2020 2055 7365 3a20 2020 2020 4372       Use:     Cr
-00016340: 6561 7465 7320 6120 7265 6c61 7469 7665  eates a relative
-00016350: 2063 6f6f 7264 696e 6174 6520 7379 7374   coordinate syst
-00016360: 656d 2e20 4f6e 6c79 2074 6865 2020 2020  em. Only the    
-00016370: 4e61 6d65 2061 7474 7269 6275 7465 206f  Name attribute o
-00016380: 6620 7468 6520 3c41 7474 7269 6275 7465  f the <Attribute
-00016390: 7341 7272 6179 3e20 7061 7261 6d65 7465  sArray> paramete
-000163a0: 7220 6973 2073 7570 706f 7274 6564 2e0a  r is supported..
-000163b0: 2020 2020 2020 2020 436f 6d6d 616e 643a          Command:
-000163c0: 204d 6f64 656c 6572 3e43 6f6f 7264 696e   Modeler>Coordin
-000163d0: 6174 6520 5379 7374 656d 3e43 7265 6174  ate System>Creat
-000163e0: 653e 5265 6c61 7469 7665 2043 532d 3e4f  e>Relative CS->O
-000163f0: 6666 7365 740a 2020 2020 2020 2020 4d6f  ffset.        Mo
-00016400: 6465 6c65 723e 436f 6f72 6469 6e61 7465  deler>Coordinate
-00016410: 2053 7973 7465 6d3e 4372 6561 7465 3e52   System>Create>R
-00016420: 656c 6174 6976 6520 4353 2d3e 526f 7461  elative CS->Rota
-00016430: 7465 640a 2020 2020 2020 2020 4d6f 6465  ted.        Mode
-00016440: 6c65 723e 436f 6f72 6469 6e61 7465 2053  ler>Coordinate S
-00016450: 7973 7465 6d3e 4372 6561 7465 3e52 656c  ystem>Create>Rel
-00016460: 6174 6976 6520 4353 2d3e 426f 7468 0a0a  ative CS->Both..
-00016470: 2020 2020 2020 2020 4375 7272 656e 7420          Current 
-00016480: 636f 6f72 6469 6e61 7465 2073 7973 7465  coordinate syste
-00016490: 6d20 6973 2073 6574 2072 6967 6874 2061  m is set right a
-000164a0: 6674 6572 2074 6869 732e 0a0a 2020 2020  fter this...    
-000164b0: 2020 2020 6373 5f6e 616d 6520 3a20 6e61      cs_name : na
-000164c0: 6d65 206f 6620 636f 6f72 642e 2073 7973  me of coord. sys
-000164d0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
-000164e0: 7468 6520 6e61 6d65 2061 6c72 6561 6479  the name already
-000164f0: 2065 7869 7374 732c 2074 6865 6e20 6120   exists, then a 
-00016500: 6e65 7720 636f 6f72 6469 6e61 7465 2073  new coordinate s
-00016510: 7973 7465 6d20 7769 7468 205f 3120 6973  ystem with _1 is
-00016520: 2063 7265 6174 6564 2e0a 0a20 2020 2020   created...     
-00016530: 2020 206f 7269 6769 6e2c 2058 4178 6973     origin, XAxis
-00016540: 5665 632c 2059 4178 6973 5665 633a 2033  Vec, YAxisVec: 3
-00016550: 2d76 6563 746f 7273 0a20 2020 2020 2020  -vectors.       
-00016560: 2020 2020 2059 6f75 2063 616e 2061 6c73       You can als
-00016570: 6f20 7061 7373 2069 6e20 7061 7261 6d73  o pass in params
-00016580: 2073 7563 6820 6173 206f 7269 6769 6e20   such as origin 
-00016590: 3d20 5b30 2c31 2c30 5d20 7261 7468 6572  = [0,1,0] rather
-000165a0: 2074 6861 6e20 5b22 3075 6d22 2c22 3175   than ["0um","1u
-000165b0: 6d22 2c22 3075 6d22 5d2c 2062 7574 2074  m","0um"], but t
-000165c0: 6865 7365 2077 696c 6c20 6265 2069 6e74  hese will be int
-000165d0: 6572 7072 6574 6564 2069 6e20 6465 6661  erpreted in defa
-000165e0: 756c 7420 756e 6974 732c 2073 6f20 6974  ult units, so it
-000165f0: 2069 7320 7361 6665 7220 746f 2062 6520   is safer to be 
-00016600: 6578 706c 6963 6974 2e20 4578 706c 6963  explicit. Explic
-00016610: 6974 206f 7665 7220 696d 706c 6963 6974  it over implicit
-00016620: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00016630: 2020 2020 2020 7365 6c66 2e5f 6d6f 6465        self._mode
-00016640: 6c65 722e 4372 6561 7465 5265 6c61 7469  ler.CreateRelati
-00016650: 7665 4353 285b 0a20 2020 2020 2020 2020  veCS([.         
-00016660: 2020 2022 4e41 4d45 3a52 656c 6174 6976     "NAME:Relativ
-00016670: 6543 5350 6172 616d 6574 6572 7322 2c20  eCSParameters", 
-00016680: 224d 6f64 653a 3d22 2c20 2241 7869 732f  "Mode:=", "Axis/
-00016690: 506f 7369 7469 6f6e 222c 0a20 2020 2020  Position",.     
-000166a0: 2020 2020 2020 2022 4f72 6967 696e 583a         "OriginX:
-000166b0: 3d22 2c20 6f72 6967 696e 5b30 5d2c 2022  =", origin[0], "
-000166c0: 4f72 6967 696e 593a 3d22 2c20 6f72 6967  OriginY:=", orig
-000166d0: 696e 5b31 5d2c 2022 4f72 6967 696e 5a3a  in[1], "OriginZ:
-000166e0: 3d22 2c0a 2020 2020 2020 2020 2020 2020  =",.            
-000166f0: 6f72 6967 696e 5b32 5d2c 2022 5841 7869  origin[2], "XAxi
-00016700: 7358 7665 633a 3d22 2c20 5841 7869 7356  sXvec:=", XAxisV
-00016710: 6563 5b30 5d2c 2022 5841 7869 7359 7665  ec[0], "XAxisYve
-00016720: 633a 3d22 2c20 5841 7869 7356 6563 5b31  c:=", XAxisVec[1
-00016730: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
-00016740: 5841 7869 735a 7665 633a 3d22 2c20 5841  XAxisZvec:=", XA
-00016750: 7869 7356 6563 5b32 5d2c 2022 5941 7869  xisVec[2], "YAxi
-00016760: 7358 7665 633a 3d22 2c20 5941 7869 7356  sXvec:=", YAxisV
-00016770: 6563 5b30 5d2c 0a20 2020 2020 2020 2020  ec[0],.         
-00016780: 2020 2022 5941 7869 7359 7665 633a 3d22     "YAxisYvec:="
-00016790: 2c20 5941 7869 7356 6563 5b31 5d2c 2022  , YAxisVec[1], "
-000167a0: 5941 7869 735a 7665 633a 3d22 2c20 5941  YAxisZvec:=", YA
-000167b0: 7869 7356 6563 5b31 5d0a 2020 2020 2020  xisVec[1].      
-000167c0: 2020 5d2c 205b 224e 414d 453a 4174 7472    ], ["NAME:Attr
-000167d0: 6962 7574 6573 222c 2022 4e61 6d65 3a3d  ibutes", "Name:=
-000167e0: 222c 2063 735f 6e61 6d65 5d29 0a0a 2020  ", cs_name])..  
-000167f0: 2020 6465 6620 7375 6274 7261 6374 2873    def subtract(s
-00016800: 656c 662c 2062 6c61 6e6b 5f6e 616d 652c  elf, blank_name,
-00016810: 2074 6f6f 6c5f 6e61 6d65 732c 206b 6565   tool_names, kee
-00016820: 705f 6f72 6967 696e 616c 733d 4661 6c73  p_originals=Fals
-00016830: 6529 3a0a 2020 2020 2020 2020 7365 6c65  e):.        sele
-00016840: 6374 696f 6e5f 6172 7261 7920 3d20 5b0a  ction_array = [.
-00016850: 2020 2020 2020 2020 2020 2020 224e 414d              "NAM
-00016860: 453a 5365 6c65 6374 696f 6e73 222c 2022  E:Selections", "
-00016870: 426c 616e 6b20 5061 7274 733a 3d22 2c20  Blank Parts:=", 
-00016880: 626c 616e 6b5f 6e61 6d65 2c20 2254 6f6f  blank_name, "Too
-00016890: 6c20 5061 7274 733a 3d22 2c0a 2020 2020  l Parts:=",.    
-000168a0: 2020 2020 2020 2020 222c 222e 6a6f 696e          ",".join
-000168b0: 2874 6f6f 6c5f 6e61 6d65 7329 0a20 2020  (tool_names).   
-000168c0: 2020 2020 205d 0a20 2020 2020 2020 2073       ].        s
-000168d0: 656c 662e 5f6d 6f64 656c 6572 2e53 7562  elf._modeler.Sub
-000168e0: 7472 6163 7428 0a20 2020 2020 2020 2020  tract(.         
-000168f0: 2020 2073 656c 6563 7469 6f6e 5f61 7272     selection_arr
-00016900: 6179 2c0a 2020 2020 2020 2020 2020 2020  ay,.            
-00016910: 5b22 4e41 4d45 3a55 6e69 7465 5061 7261  ["NAME:UnitePara
-00016920: 6d65 7465 7273 222c 2022 4b65 6570 4f72  meters", "KeepOr
-00016930: 6967 696e 616c 733a 3d22 2c20 6b65 6570  iginals:=", keep
-00016940: 5f6f 7269 6769 6e61 6c73 5d29 0a20 2020  _originals]).   
-00016950: 2020 2020 2072 6574 7572 6e20 626c 616e       return blan
-00016960: 6b5f 6e61 6d65 0a0a 2020 2020 6465 6620  k_name..    def 
-00016970: 5f66 696c 6c65 7428 7365 6c66 2c20 7261  _fillet(self, ra
-00016980: 6469 7573 2c20 7665 7274 6578 5f69 6e64  dius, vertex_ind
-00016990: 6578 2c20 6f62 6a29 3a0a 2020 2020 2020  ex, obj):.      
-000169a0: 2020 7665 7274 6963 6573 203d 2073 656c    vertices = sel
-000169b0: 662e 5f6d 6f64 656c 6572 2e47 6574 5665  f._modeler.GetVe
-000169c0: 7274 6578 4944 7346 726f 6d4f 626a 6563  rtexIDsFromObjec
-000169d0: 7428 6f62 6a29 0a20 2020 2020 2020 2069  t(obj).        i
-000169e0: 6620 6973 696e 7374 616e 6365 2876 6572  f isinstance(ver
-000169f0: 7465 785f 696e 6465 782c 206c 6973 7429  tex_index, list)
-00016a00: 3a0a 2020 2020 2020 2020 2020 2020 746f  :.            to
-00016a10: 5f66 696c 6c65 7420 3d20 5b69 6e74 2876  _fillet = [int(v
-00016a20: 6572 7469 6365 735b 765d 2920 666f 7220  ertices[v]) for 
-00016a30: 7620 696e 2076 6572 7465 785f 696e 6465  v in vertex_inde
-00016a40: 785d 0a20 2020 2020 2020 2065 6c73 653a  x].        else:
-00016a50: 0a20 2020 2020 2020 2020 2020 2074 6f5f  .            to_
-00016a60: 6669 6c6c 6574 203d 205b 696e 7428 7665  fillet = [int(ve
-00016a70: 7274 6963 6573 5b76 6572 7465 785f 696e  rtices[vertex_in
-00016a80: 6465 785d 295d 0a0a 0a23 2020 2020 2020  dex])]...#      
-00016a90: 2020 7072 696e 7428 7665 7274 6963 6573    print(vertices
-00016aa0: 290a 2320 2020 2020 2020 2070 7269 6e74  ).#        print
-00016ab0: 2872 6164 6975 7329 0a20 2020 2020 2020  (radius).       
-00016ac0: 2073 656c 662e 5f6d 6f64 656c 6572 2e46   self._modeler.F
-00016ad0: 696c 6c65 7428 5b22 4e41 4d45 3a53 656c  illet(["NAME:Sel
-00016ae0: 6563 7469 6f6e 7322 2c20 2253 656c 6563  ections", "Selec
-00016af0: 7469 6f6e 733a 3d22 2c20 6f62 6a5d 2c20  tions:=", obj], 
-00016b00: 5b0a 2020 2020 2020 2020 2020 2020 224e  [.            "N
-00016b10: 414d 453a 5061 7261 6d65 7465 7273 222c  AME:Parameters",
-00016b20: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
-00016b30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00016b40: 4e41 4d45 3a46 696c 6c65 7450 6172 616d  NAME:FilletParam
-00016b50: 6574 6572 7322 2c20 2245 6467 6573 3a3d  eters", "Edges:=
-00016b60: 222c 205b 5d2c 2022 5665 7274 6963 6573  ", [], "Vertices
-00016b70: 3a3d 222c 0a20 2020 2020 2020 2020 2020  :=",.           
-00016b80: 2020 2020 2074 6f5f 6669 6c6c 6574 2c20       to_fillet, 
-00016b90: 2252 6164 6975 733a 3d22 2c20 7261 6469  "Radius:=", radi
-00016ba0: 7573 2c20 2253 6574 6261 636b 3a3d 222c  us, "Setback:=",
-00016bb0: 2022 306d 6d22 0a20 2020 2020 2020 2020   "0mm".         
-00016bc0: 2020 205d 0a20 2020 2020 2020 205d 290a     ].        ]).
-00016bd0: 0a20 2020 2064 6566 205f 6669 6c6c 6574  .    def _fillet
-00016be0: 5f65 6467 6573 2873 656c 662c 2072 6164  _edges(self, rad
-00016bf0: 6975 732c 2065 6467 655f 696e 6465 782c  ius, edge_index,
-00016c00: 206f 626a 293a 0a20 2020 2020 2020 2065   obj):.        e
-00016c10: 6467 6573 203d 2073 656c 662e 5f6d 6f64  dges = self._mod
-00016c20: 656c 6572 2e47 6574 4564 6765 4944 7346  eler.GetEdgeIDsF
-00016c30: 726f 6d4f 626a 6563 7428 6f62 6a29 0a20  romObject(obj). 
-00016c40: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00016c50: 616e 6365 2865 6467 655f 696e 6465 782c  ance(edge_index,
-00016c60: 206c 6973 7429 3a0a 2020 2020 2020 2020   list):.        
-00016c70: 2020 2020 746f 5f66 696c 6c65 7420 3d20      to_fillet = 
-00016c80: 5b69 6e74 2865 6467 6573 5b65 5d29 2066  [int(edges[e]) f
-00016c90: 6f72 2065 2069 6e20 6564 6765 5f69 6e64  or e in edge_ind
-00016ca0: 6578 5d0a 2020 2020 2020 2020 656c 7365  ex].        else
-00016cb0: 3a0a 2020 2020 2020 2020 2020 2020 746f  :.            to
-00016cc0: 5f66 696c 6c65 7420 3d20 5b69 6e74 2865  _fillet = [int(e
-00016cd0: 6467 6573 5b65 6467 655f 696e 6465 785d  dges[edge_index]
-00016ce0: 295d 0a0a 2020 2020 2020 2020 7365 6c66  )]..        self
-00016cf0: 2e5f 6d6f 6465 6c65 722e 4669 6c6c 6574  ._modeler.Fillet
-00016d00: 285b 224e 414d 453a 5365 6c65 6374 696f  (["NAME:Selectio
-00016d10: 6e73 222c 2022 5365 6c65 6374 696f 6e73  ns", "Selections
-00016d20: 3a3d 222c 206f 626a 5d2c 205b 0a20 2020  :=", obj], [.   
-00016d30: 2020 2020 2020 2020 2022 4e41 4d45 3a50           "NAME:P
-00016d40: 6172 616d 6574 6572 7322 2c0a 2020 2020  arameters",.    
-00016d50: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-00016d60: 2020 2020 2020 2020 2020 224e 414d 453a            "NAME:
-00016d70: 4669 6c6c 6574 5061 7261 6d65 7465 7273  FilletParameters
-00016d80: 222c 2022 4564 6765 733a 3d22 2c20 746f  ", "Edges:=", to
-00016d90: 5f66 696c 6c65 742c 2022 5665 7274 6963  _fillet, "Vertic
-00016da0: 6573 3a3d 222c 0a20 2020 2020 2020 2020  es:=",.         
-00016db0: 2020 2020 2020 205b 5d2c 2022 5261 6469         [], "Radi
-00016dc0: 7573 3a3d 222c 2072 6164 6975 732c 2022  us:=", radius, "
-00016dd0: 5365 7462 6163 6b3a 3d22 2c20 2230 6d6d  Setback:=", "0mm
-00016de0: 220a 2020 2020 2020 2020 2020 2020 5d0a  ".            ].
-00016df0: 2020 2020 2020 2020 5d29 0a0a 2020 2020          ])..    
-00016e00: 6465 6620 5f66 696c 6c65 7473 2873 656c  def _fillets(sel
-00016e10: 662c 2072 6164 6975 732c 2076 6572 7469  f, radius, verti
-00016e20: 6365 732c 206f 626a 293a 0a20 2020 2020  ces, obj):.     
-00016e30: 2020 2073 656c 662e 5f6d 6f64 656c 6572     self._modeler
-00016e40: 2e46 696c 6c65 7428 5b22 4e41 4d45 3a53  .Fillet(["NAME:S
-00016e50: 656c 6563 7469 6f6e 7322 2c20 2253 656c  elections", "Sel
-00016e60: 6563 7469 6f6e 733a 3d22 2c20 6f62 6a5d  ections:=", obj]
-00016e70: 2c20 5b0a 2020 2020 2020 2020 2020 2020  , [.            
-00016e80: 224e 414d 453a 5061 7261 6d65 7465 7273  "NAME:Parameters
-00016e90: 222c 0a20 2020 2020 2020 2020 2020 205b  ",.            [
-00016ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016eb0: 2022 4e41 4d45 3a46 696c 6c65 7450 6172   "NAME:FilletPar
-00016ec0: 616d 6574 6572 7322 2c20 2245 6467 6573  ameters", "Edges
-00016ed0: 3a3d 222c 205b 5d2c 2022 5665 7274 6963  :=", [], "Vertic
-00016ee0: 6573 3a3d 222c 2076 6572 7469 6365 732c  es:=", vertices,
-00016ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016f00: 2022 5261 6469 7573 3a3d 222c 2072 6164   "Radius:=", rad
-00016f10: 6975 732c 2022 5365 7462 6163 6b3a 3d22  ius, "Setback:="
-00016f20: 2c20 2230 6d6d 220a 2020 2020 2020 2020  , "0mm".        
-00016f30: 2020 2020 5d0a 2020 2020 2020 2020 5d29      ].        ])
-00016f40: 0a0a 2020 2020 6465 6620 5f73 7765 6570  ..    def _sweep
-00016f50: 5f61 6c6f 6e67 5f70 6174 6828 7365 6c66  _along_path(self
-00016f60: 2c20 746f 5f73 7765 6570 2c20 7061 7468  , to_sweep, path
-00016f70: 5f6f 626a 293a 0a20 2020 2020 2020 2022  _obj):.        "
-00016f80: 2222 0a20 2020 2020 2020 2041 6464 7320  "".        Adds 
-00016f90: 7468 6963 6b6e 6573 7320 746f 2070 6174  thickness to pat
-00016fa0: 685f 6f62 6a20 6279 2065 7874 656e 6469  h_obj by extendi
-00016fb0: 6e67 2074 6f20 6120 6e65 7720 6469 6d65  ng to a new dime
-00016fc0: 6e73 696f 6e2e 0a20 2020 2020 2020 2074  nsion..        t
-00016fd0: 6f5f 7377 6565 7020 6163 7473 2061 7320  o_sweep acts as 
-00016fe0: 6120 7075 7474 7920 6b6e 6966 6520 7468  a putty knife th
-00016ff0: 6174 2064 6574 6572 6d69 6e65 7320 7468  at determines th
-00017000: 6520 7468 6963 6b6e 6573 732e 0a0a 2020  e thickness...  
-00017010: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00017020: 2020 2020 2020 2020 746f 5f73 7765 6570          to_sweep
-00017030: 2028 706f 6c79 6c69 6e65 293a 2053 6d61   (polyline): Sma
-00017040: 6c6c 2070 6f6c 796c 696e 6520 7275 6e6e  ll polyline runn
-00017050: 696e 6720 7065 7270 656e 6469 6375 6c61  ing perpendicula
-00017060: 7220 746f 2070 6174 685f 6f62 6a0a 2020  r to path_obj.  
-00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017090: 2020 7768 6f73 6520 6c65 6e67 7468 2069    whose length i
-000170a0: 7320 7468 6520 6465 7369 7265 6420 7265  s the desired re
-000170b0: 7375 6c74 696e 6720 7468 6963 6b6e 6573  sulting thicknes
-000170c0: 730a 2020 2020 2020 2020 2020 2020 7061  s.            pa
-000170d0: 7468 5f6f 626a 2028 706f 6c79 6c69 6e65  th_obj (polyline
-000170e0: 293a 204f 7269 6769 6e61 6c20 706f 6c79  ): Original poly
-000170f0: 6c69 6e65 3b20 7761 6e74 2074 6f20 6272  line; want to br
-00017100: 6f61 6465 6e20 7468 6973 0a20 2020 2020  oaden this.     
-00017110: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00017120: 656c 662e 7265 6e61 6d65 5f6f 626a 2870  elf.rename_obj(p
-00017130: 6174 685f 6f62 6a2c 2073 7472 2870 6174  ath_obj, str(pat
-00017140: 685f 6f62 6a29 202b 2027 5f70 6174 6827  h_obj) + '_path'
-00017150: 290a 2020 2020 2020 2020 6e65 775f 6e61  ).        new_na
-00017160: 6d65 203d 2073 656c 662e 7265 6e61 6d65  me = self.rename
-00017170: 5f6f 626a 2874 6f5f 7377 6565 702c 2070  _obj(to_sweep, p
-00017180: 6174 685f 6f62 6a29 0a20 2020 2020 2020  ath_obj).       
-00017190: 206e 616d 6573 203d 205b 7061 7468 5f6f   names = [path_o
-000171a0: 626a 2c20 7374 7228 7061 7468 5f6f 626a  bj, str(path_obj
-000171b0: 2920 2b20 275f 7061 7468 275d 0a20 2020  ) + '_path'].   
-000171c0: 2020 2020 2073 656c 662e 5f6d 6f64 656c       self._model
-000171d0: 6572 2e53 7765 6570 416c 6f6e 6750 6174  er.SweepAlongPat
-000171e0: 6828 7365 6c66 2e5f 7365 6c65 6374 696f  h(self._selectio
-000171f0: 6e73 5f61 7272 6179 282a 6e61 6d65 7329  ns_array(*names)
-00017200: 2c20 5b0a 2020 2020 2020 2020 2020 2020  , [.            
-00017210: 224e 414d 453a 5061 7468 5377 6565 7050  "NAME:PathSweepP
-00017220: 6172 616d 6574 6572 7322 2c20 2244 7261  arameters", "Dra
-00017230: 6674 416e 676c 653a 3d22 2c20 2230 6465  ftAngle:=", "0de
-00017240: 6722 2c20 2244 7261 6674 5479 7065 3a3d  g", "DraftType:=
-00017250: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00017260: 526f 756e 6422 2c20 2243 6865 636b 4661  Round", "CheckFa
-00017270: 6365 4661 6365 496e 7465 7273 6563 7469  ceFaceIntersecti
-00017280: 6f6e 3a3d 222c 2046 616c 7365 2c20 2254  on:=", False, "T
-00017290: 7769 7374 416e 676c 653a 3d22 2c0a 2020  wistAngle:=",.  
-000172a0: 2020 2020 2020 2020 2020 2230 6465 6722            "0deg"
-000172b0: 0a20 2020 2020 2020 205d 290a 2020 2020  .        ]).    
-000172c0: 2020 2020 7265 7475 726e 2050 6f6c 796c      return Polyl
-000172d0: 696e 6528 6e65 775f 6e61 6d65 2c20 7365  ine(new_name, se
-000172e0: 6c66 290a 0a20 2020 2064 6566 2073 7765  lf)..    def swe
-000172f0: 6570 5f61 6c6f 6e67 5f76 6563 746f 7228  ep_along_vector(
-00017300: 7365 6c66 2c20 6e61 6d65 732c 2076 6563  self, names, vec
-00017310: 746f 7229 3a0a 2020 2020 2020 2020 7365  tor):.        se
-00017320: 6c66 2e5f 6d6f 6465 6c65 722e 5377 6565  lf._modeler.Swee
-00017330: 7041 6c6f 6e67 5665 6374 6f72 2873 656c  pAlongVector(sel
-00017340: 662e 5f73 656c 6563 7469 6f6e 735f 6172  f._selections_ar
-00017350: 7261 7928 2a6e 616d 6573 292c 205b 0a20  ray(*names), [. 
-00017360: 2020 2020 2020 2020 2020 2022 4e41 4d45             "NAME
-00017370: 3a56 6563 746f 7253 7765 6570 5061 7261  :VectorSweepPara
-00017380: 6d65 7465 7273 222c 2022 4472 6166 7441  meters", "DraftA
-00017390: 6e67 6c65 3a3d 222c 2022 3064 6567 222c  ngle:=", "0deg",
-000173a0: 0a20 2020 2020 2020 2020 2020 2022 4472  .            "Dr
-000173b0: 6166 7454 7970 653a 3d22 2c20 2252 6f75  aftType:=", "Rou
-000173c0: 6e64 222c 2022 4368 6563 6b46 6163 6546  nd", "CheckFaceF
-000173d0: 6163 6549 6e74 6572 7365 6374 696f 6e3a  aceIntersection:
-000173e0: 3d22 2c20 4661 6c73 652c 0a20 2020 2020  =", False,.     
-000173f0: 2020 2020 2020 2022 5377 6565 7056 6563         "SweepVec
-00017400: 746f 7258 3a3d 222c 2076 6563 746f 725b  torX:=", vector[
-00017410: 305d 2c20 2253 7765 6570 5665 6374 6f72  0], "SweepVector
-00017420: 593a 3d22 2c20 7665 6374 6f72 5b31 5d2c  Y:=", vector[1],
-00017430: 0a20 2020 2020 2020 2020 2020 2022 5377  .            "Sw
-00017440: 6565 7056 6563 746f 725a 3a3d 222c 2076  eepVectorZ:=", v
-00017450: 6563 746f 725b 325d 0a20 2020 2020 2020  ector[2].       
-00017460: 205d 290a 0a20 2020 2064 6566 2072 656e   ])..    def ren
-00017470: 616d 655f 6f62 6a28 7365 6c66 2c20 6f62  ame_obj(self, ob
-00017480: 6a2c 206e 616d 6529 3a0a 2020 2020 2020  j, name):.      
-00017490: 2020 7365 6c66 2e5f 6d6f 6465 6c65 722e    self._modeler.
-000174a0: 4368 616e 6765 5072 6f70 6572 7479 285b  ChangeProperty([
-000174b0: 0a20 2020 2020 2020 2020 2020 2022 4e41  .            "NA
-000174c0: 4d45 3a41 6c6c 5461 6273 222c 0a20 2020  ME:AllTabs",.   
-000174d0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-000174e0: 2020 2020 2020 2020 2020 2022 4e41 4d45             "NAME
-000174f0: 3a47 656f 6d65 7472 7933 4441 7474 7269  :Geometry3DAttri
-00017500: 6275 7465 5461 6222 2c20 5b22 4e41 4d45  buteTab", ["NAME
-00017510: 3a50 726f 7053 6572 7665 7273 222c 0a20  :PropServers",. 
-00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017540: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00017550: 7472 286f 626a 295d 2c0a 2020 2020 2020  tr(obj)],.      
-00017560: 2020 2020 2020 2020 2020 5b22 4e41 4d45            ["NAME
-00017570: 3a43 6861 6e67 6564 5072 6f70 7322 2c20  :ChangedProps", 
-00017580: 5b22 4e41 4d45 3a4e 616d 6522 2c20 2256  ["NAME:Name", "V
-00017590: 616c 7565 3a3d 222c 0a20 2020 2020 2020  alue:=",.       
-000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175c0: 7374 7228 6e61 6d65 295d 5d0a 2020 2020  str(name)]].    
-000175d0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-000175e0: 2020 5d29 0a20 2020 2020 2020 2072 6574    ]).        ret
-000175f0: 7572 6e20 6e61 6d65 0a0a 0a63 6c61 7373  urn name...class
-00017600: 204d 6f64 656c 456e 7469 7479 2873 7472   ModelEntity(str
-00017610: 2c20 4866 7373 5072 6f70 6572 7479 4f62  , HfssPropertyOb
-00017620: 6a65 6374 293a 0a20 2020 2070 726f 705f  ject):.    prop_
-00017630: 7461 6220 3d20 2247 656f 6d65 7472 7933  tab = "Geometry3
-00017640: 4443 6d64 5461 6222 0a20 2020 206d 6f64  DCmdTab".    mod
-00017650: 656c 5f63 6f6d 6d61 6e64 203d 204e 6f6e  el_command = Non
-00017660: 650a 2020 2020 7472 616e 7370 6172 656e  e.    transparen
-00017670: 6379 203d 206d 616b 655f 666c 6f61 745f  cy = make_float_
-00017680: 7072 6f70 2822 5472 616e 7370 6172 656e  prop("Transparen
-00017690: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-000176a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176b0: 2020 2020 2020 2070 726f 705f 7461 623d         prop_tab=
-000176c0: 2247 656f 6d65 7472 7933 4441 7474 7269  "Geometry3DAttri
-000176d0: 6275 7465 5461 6222 2c0a 2020 2020 2020  buteTab",.      
-000176e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000176f0: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-00017700: 705f 7365 7276 6572 3d6c 616d 6264 6120  p_server=lambda 
-00017710: 7365 6c66 3a20 7365 6c66 290a 2020 2020  self: self).    
-00017720: 6d61 7465 7269 616c 203d 206d 616b 655f  material = make_
-00017730: 7374 725f 7072 6f70 2822 4d61 7465 7269  str_prop("Materi
-00017740: 616c 222c 0a20 2020 2020 2020 2020 2020  al",.           
-00017750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017760: 2020 7072 6f70 5f74 6162 3d22 4765 6f6d    prop_tab="Geom
-00017770: 6574 7279 3344 4174 7472 6962 7574 6554  etry3DAttributeT
-00017780: 6162 222c 0a20 2020 2020 2020 2020 2020  ab",.           
-00017790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177a0: 2020 7072 6f70 5f73 6572 7665 723d 6c61    prop_server=la
-000177b0: 6d62 6461 2073 656c 663a 2073 656c 6629  mbda self: self)
-000177c0: 0a20 2020 2077 6972 6566 7261 6d65 203d  .    wireframe =
-000177d0: 206d 616b 655f 666c 6f61 745f 7072 6f70   make_float_prop
-000177e0: 2822 4469 7370 6c61 7920 5769 7265 6672  ("Display Wirefr
-000177f0: 616d 6522 2c0a 2020 2020 2020 2020 2020  ame",.          
-00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017810: 2020 2020 2020 7072 6f70 5f74 6162 3d22        prop_tab="
-00017820: 4765 6f6d 6574 7279 3344 4174 7472 6962  Geometry3DAttrib
-00017830: 7574 6554 6162 222c 0a20 2020 2020 2020  uteTab",.       
+00013d40: 2020 2020 202a 2a6b 7761 7267 7329 0a0a       **kwargs)..
+00013d50: 2020 2020 6465 6620 6472 6177 5f63 796c      def draw_cyl
+00013d60: 696e 6465 7228 7365 6c66 2c20 706f 732c  inder(self, pos,
+00013d70: 2072 6164 6975 732c 2068 6569 6768 742c   radius, height,
+00013d80: 2061 7869 732c 202a 2a6b 7761 7267 7329   axis, **kwargs)
+00013d90: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
+00013da0: 2061 7869 7320 696e 2022 5859 5a22 0a20   axis in "XYZ". 
+00013db0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00013dc0: 6c66 2e5f 6d6f 6465 6c65 722e 4372 6561  lf._modeler.Crea
+00013dd0: 7465 4379 6c69 6e64 6572 285b 0a20 2020  teCylinder([.   
+00013de0: 2020 2020 2020 2020 2022 4e41 4d45 3a43           "NAME:C
+00013df0: 796c 696e 6465 7250 6172 616d 6574 6572  ylinderParameter
+00013e00: 7322 2c20 2258 4365 6e74 6572 3a3d 222c  s", "XCenter:=",
+00013e10: 2070 6f73 5b30 5d2c 2022 5943 656e 7465   pos[0], "YCente
+00013e20: 723a 3d22 2c0a 2020 2020 2020 2020 2020  r:=",.          
+00013e30: 2020 706f 735b 315d 2c20 225a 4365 6e74    pos[1], "ZCent
+00013e40: 6572 3a3d 222c 2070 6f73 5b32 5d2c 2022  er:=", pos[2], "
+00013e50: 5261 6469 7573 3a3d 222c 2072 6164 6975  Radius:=", radiu
+00013e60: 732c 2022 4865 6967 6874 3a3d 222c 0a20  s, "Height:=",. 
+00013e70: 2020 2020 2020 2020 2020 2068 6569 6768             heigh
+00013e80: 742c 2022 5768 6963 6841 7869 733a 3d22  t, "WhichAxis:="
+00013e90: 2c20 6178 6973 2c20 224e 756d 5369 6465  , axis, "NumSide
+00013ea0: 733a 3d22 2c20 300a 2020 2020 2020 2020  s:=", 0.        
+00013eb0: 5d2c 2073 656c 662e 5f61 7474 7269 6275  ], self._attribu
+00013ec0: 7465 735f 6172 7261 7928 2a2a 6b77 6172  tes_array(**kwar
+00013ed0: 6773 2929 0a0a 2020 2020 6465 6620 6472  gs))..    def dr
+00013ee0: 6177 5f63 796c 696e 6465 725f 6365 6e74  aw_cylinder_cent
+00013ef0: 6572 2873 656c 662c 2070 6f73 2c20 7261  er(self, pos, ra
+00013f00: 6469 7573 2c20 6865 6967 6874 2c20 6178  dius, height, ax
+00013f10: 6973 2c20 2a2a 6b77 6172 6773 293a 0a20  is, **kwargs):. 
+00013f20: 2020 2020 2020 2061 7869 735f 6964 7820         axis_idx 
+00013f30: 3d20 5b22 5822 2c20 2259 222c 2022 5a22  = ["X", "Y", "Z"
+00013f40: 5d2e 696e 6465 7828 6178 6973 290a 2020  ].index(axis).  
+00013f50: 2020 2020 2020 6564 6765 5f70 6f73 203d        edge_pos =
+00013f60: 2063 6f70 7928 706f 7329 0a20 2020 2020   copy(pos).     
+00013f70: 2020 2065 6467 655f 706f 735b 6178 6973     edge_pos[axis
+00013f80: 5f69 6478 5d20 3d20 7661 7228 706f 735b  _idx] = var(pos[
+00013f90: 6178 6973 5f69 6478 5d29 202d 2076 6172  axis_idx]) - var
+00013fa0: 2868 6569 6768 7429 202f 2032 0a20 2020  (height) / 2.   
+00013fb0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00013fc0: 2e64 7261 775f 6379 6c69 6e64 6572 2865  .draw_cylinder(e
+00013fd0: 6467 655f 706f 732c 2072 6164 6975 732c  dge_pos, radius,
+00013fe0: 2068 6569 6768 742c 2061 7869 732c 202a   height, axis, *
+00013ff0: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
+00014000: 6620 6472 6177 5f77 6972 6562 6f6e 6428  f draw_wirebond(
+00014010: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00014020: 2020 2020 2020 2020 2020 2020 706f 732c              pos,
+00014030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014040: 2020 2020 2020 206f 7269 2c0a 2020 2020         ori,.    
+00014050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014060: 2020 7769 6474 682c 0a20 2020 2020 2020    width,.       
+00014070: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00014080: 6569 6768 743d 2730 2e31 6d6d 272c 0a20  eight='0.1mm',. 
+00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140a0: 2020 2020 207a 3d30 2c0a 2020 2020 2020       z=0,.      
+000140b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140c0: 7769 7265 5f64 6961 6d65 7465 723d 2230  wire_diameter="0
+000140d0: 2e30 326d 6d22 2c0a 2020 2020 2020 2020  .02mm",.        
+000140e0: 2020 2020 2020 2020 2020 2020 2020 4e75                Nu
+000140f0: 6d53 6964 6573 3d36 2c0a 2020 2020 2020  mSides=6,.      
+00014100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014110: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
+00014120: 2020 2027 2727 0a20 2020 2020 2020 2020     '''.         
+00014130: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00014140: 2020 2020 2020 2020 2070 6f73 3a20 3244           pos: 2D
+00014150: 2070 6f73 6974 696f 6e20 7665 6374 6f72   position vector
+00014160: 2020 2873 7065 6369 6679 2063 656e 7465    (specify cente
+00014170: 7220 706f 696e 7429 0a20 2020 2020 2020  r point).       
+00014180: 2020 2020 2020 2020 206f 7269 3a20 7368           ori: sh
+00014190: 6f75 6c64 2062 6520 6e6f 726d 6564 0a20  ould be normed. 
+000141a0: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+000141b0: 3a20 7a20 706f 7369 7469 6f6e 0a0a 2020  : z position..  
+000141c0: 2020 2020 2020 2020 2020 2320 544f 444f            # TODO
+000141d0: 2063 7265 6174 6520 5769 7265 626f 6e64   create Wirebond
+000141e0: 2063 6c61 7373 0a20 2020 2020 2020 2020   class.         
+000141f0: 2020 2070 6f73 6974 696f 6e20 6973 2074     position is t
+00014200: 6865 206f 7269 6769 6e20 6f66 206f 6e65  he origin of one
+00014210: 2070 6f69 6e74 0a20 2020 2020 2020 2020   point.         
+00014220: 2020 206f 7269 2069 7320 7468 6520 6f72     ori is the or
+00014230: 6965 6e74 6174 696f 6e20 7665 6374 6f72  ientation vector
+00014240: 2c20 7768 6963 6820 6765 7473 206e 6f72  , which gets nor
+00014250: 6d61 6c69 7a65 640a 2020 2020 2020 2020  malized.        
+00014260: 2727 270a 2020 2020 2020 2020 7020 3d20  '''.        p = 
+00014270: 6e70 2e61 7272 6179 2870 6f73 290a 2020  np.array(pos).  
+00014280: 2020 2020 2020 6f20 3d20 6e70 2e61 7272        o = np.arr
+00014290: 6179 286f 7269 290a 2020 2020 2020 2020  ay(ori).        
+000142a0: 7061 6431 203d 2070 202d 206f 202a 2077  pad1 = p - o * w
+000142b0: 6964 7468 202f 2032 2e0a 2020 2020 2020  idth / 2..      
+000142c0: 2020 6e61 6d65 203d 2073 656c 662e 5f6d    name = self._m
+000142d0: 6f64 656c 6572 2e43 7265 6174 6542 6f6e  odeler.CreateBon
+000142e0: 6477 6972 6528 5b0a 2020 2020 2020 2020  dwire([.        
+000142f0: 2020 2020 224e 414d 453a 426f 6e64 7769      "NAME:Bondwi
+00014300: 7265 5061 7261 6d65 7465 7273 222c 2022  reParameters", "
+00014310: 5769 7265 5479 7065 3a3d 222c 2022 4c6f  WireType:=", "Lo
+00014320: 7722 2c20 2257 6972 6544 6961 6d65 7465  w", "WireDiamete
+00014330: 723a 3d22 2c0a 2020 2020 2020 2020 2020  r:=",.          
+00014340: 2020 7769 7265 5f64 6961 6d65 7465 722c    wire_diameter,
+00014350: 2022 4e75 6d53 6964 6573 3a3d 222c 204e   "NumSides:=", N
+00014360: 756d 5369 6465 732c 2022 5850 6164 506f  umSides, "XPadPo
+00014370: 733a 3d22 2c20 7061 6431 5b30 5d2c 0a20  s:=", pad1[0],. 
+00014380: 2020 2020 2020 2020 2020 2022 5950 6164             "YPad
+00014390: 506f 733a 3d22 2c20 7061 6431 5b31 5d2c  Pos:=", pad1[1],
+000143a0: 2022 5a50 6164 506f 733a 3d22 2c20 7a2c   "ZPadPos:=", z,
+000143b0: 2022 5844 6972 3a3d 222c 206f 7269 5b30   "XDir:=", ori[0
+000143c0: 5d2c 2022 5944 6972 3a3d 222c 0a20 2020  ], "YDir:=",.   
+000143d0: 2020 2020 2020 2020 206f 7269 5b31 5d2c           ori[1],
+000143e0: 2022 5a44 6972 3a3d 222c 2030 2c20 2244   "ZDir:=", 0, "D
+000143f0: 6973 7461 6e63 653a 3d22 2c20 7769 6474  istance:=", widt
+00014400: 682c 2022 6831 3a3d 222c 2068 6569 6768  h, "h1:=", heigh
+00014410: 742c 2022 6832 3a3d 222c 0a20 2020 2020  t, "h2:=",.     
+00014420: 2020 2020 2020 2022 306d 6d22 2c20 2261         "0mm", "a
+00014430: 6c70 6861 3a3d 222c 2022 3830 6465 6722  lpha:=", "80deg"
+00014440: 2c20 2262 6574 613a 3d22 2c20 2238 3064  , "beta:=", "80d
+00014450: 6567 222c 2022 5768 6963 6841 7869 733a  eg", "WhichAxis:
+00014460: 3d22 2c20 225a 220a 2020 2020 2020 2020  =", "Z".        
+00014470: 5d2c 2073 656c 662e 5f61 7474 7269 6275  ], self._attribu
+00014480: 7465 735f 6172 7261 7928 2a2a 6b77 6172  tes_array(**kwar
+00014490: 6773 2929 0a0a 2020 2020 2020 2020 7265  gs))..        re
+000144a0: 7475 726e 206e 616d 650a 0a20 2020 2064  turn name..    d
+000144b0: 6566 2064 7261 775f 7265 6769 6f6e 2873  ef draw_region(s
+000144c0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+000144d0: 2020 2020 2020 2020 2050 6164 6469 6e67           Padding
+000144e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000144f0: 2020 2020 2020 5061 6464 696e 6754 7970        PaddingTyp
+00014500: 653d 2250 6572 6365 6e74 6167 6520 4f66  e="Percentage Of
+00014510: 6673 6574 222c 0a20 2020 2020 2020 2020  fset",.         
+00014520: 2020 2020 2020 2020 2020 206e 616d 653d             name=
+00014530: 2752 6567 696f 6e27 2c0a 2020 2020 2020  'Region',.      
+00014540: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00014550: 7465 7269 616c 3d22 5c22 7661 6375 756d  terial="\"vacuum
+00014560: 5c22 2229 3a0a 2020 2020 2020 2020 2222  \""):.        ""
+00014570: 220a 2020 2020 2020 2020 2020 2020 5061  ".            Pa
+00014580: 6464 696e 6754 7970 6520 3a20 2741 6273  ddingType : 'Abs
+00014590: 6f6c 7574 6520 4f66 6673 6574 272c 2022  olute Offset', "
+000145a0: 5065 7263 656e 7461 6765 204f 6666 7365  Percentage Offse
+000145b0: 7422 0a20 2020 2020 2020 2022 2222 0a20  t".        """. 
+000145c0: 2020 2020 2020 2023 2054 4f44 4f3a 2041         # TODO: A
+000145d0: 6464 206f 7074 696f 6e20 746f 206d 6f64  dd option to mod
+000145e0: 6966 7920 7468 6573 650a 2020 2020 2020  ify these.      
+000145f0: 2020 5265 6769 6f6e 4174 7472 6962 7574    RegionAttribut
+00014600: 6573 203d 205b 0a20 2020 2020 2020 2020  es = [.         
+00014610: 2020 2022 4e41 4d45 3a41 7474 7269 6275     "NAME:Attribu
+00014620: 7465 7322 2c20 224e 616d 653a 3d22 2c20  tes", "Name:=", 
+00014630: 6e61 6d65 2c20 2246 6c61 6773 3a3d 222c  name, "Flags:=",
+00014640: 2022 5769 7265 6672 616d 6523 222c 0a20   "Wireframe#",. 
+00014650: 2020 2020 2020 2020 2020 2022 436f 6c6f             "Colo
+00014660: 723a 3d22 2c20 2228 3235 3520 3020 3029  r:=", "(255 0 0)
+00014670: 222c 2022 5472 616e 7370 6172 656e 6379  ", "Transparency
+00014680: 3a3d 222c 2031 2c0a 2020 2020 2020 2020  :=", 1,.        
+00014690: 2020 2020 2250 6172 7443 6f6f 7264 696e      "PartCoordin
+000146a0: 6174 6553 7973 7465 6d3a 3d22 2c20 2247  ateSystem:=", "G
+000146b0: 6c6f 6261 6c22 2c20 2255 444d 4964 3a3d  lobal", "UDMId:=
+000146c0: 222c 2022 222c 0a20 2020 2020 2020 2020  ", "",.         
+000146d0: 2020 2022 4973 416c 7761 7973 4869 6465     "IsAlwaysHide
+000146e0: 6e3a 3d22 2c20 4661 6c73 652c 2022 4d61  n:=", False, "Ma
+000146f0: 7465 7269 616c 5661 6c75 653a 3d22 2c20  terialValue:=", 
+00014700: 6d61 7465 7269 616c 2c0a 2020 2020 2020  material,.      
+00014710: 2020 2020 2020 2253 6f6c 7665 496e 7369        "SolveInsi
+00014720: 6465 3a3d 222c 2054 7275 650a 2020 2020  de:=", True.    
+00014730: 2020 2020 5d0a 0a20 2020 2020 2020 2073      ]..        s
+00014740: 656c 662e 5f6d 6f64 656c 6572 2e43 7265  elf._modeler.Cre
+00014750: 6174 6552 6567 696f 6e28 5b0a 2020 2020  ateRegion([.    
+00014760: 2020 2020 2020 2020 224e 414d 453a 5265          "NAME:Re
+00014770: 6769 6f6e 5061 7261 6d65 7465 7273 222c  gionParameters",
+00014780: 2022 2b58 5061 6464 696e 6754 7970 653a   "+XPaddingType:
+00014790: 3d22 2c20 5061 6464 696e 6754 7970 652c  =", PaddingType,
+000147a0: 0a20 2020 2020 2020 2020 2020 2022 2b58  .            "+X
+000147b0: 5061 6464 696e 673a 3d22 2c20 5061 6464  Padding:=", Padd
+000147c0: 696e 675b 305d 5b30 5d2c 2022 2d58 5061  ing[0][0], "-XPa
+000147d0: 6464 696e 6754 7970 653a 3d22 2c20 5061  ddingType:=", Pa
+000147e0: 6464 696e 6754 7970 652c 0a20 2020 2020  ddingType,.     
+000147f0: 2020 2020 2020 2022 2d58 5061 6464 696e         "-XPaddin
+00014800: 673a 3d22 2c20 5061 6464 696e 675b 305d  g:=", Padding[0]
+00014810: 5b31 5d2c 2022 2b59 5061 6464 696e 6754  [1], "+YPaddingT
+00014820: 7970 653a 3d22 2c20 5061 6464 696e 6754  ype:=", PaddingT
+00014830: 7970 652c 0a20 2020 2020 2020 2020 2020  ype,.           
+00014840: 2022 2b59 5061 6464 696e 673a 3d22 2c20   "+YPadding:=", 
+00014850: 5061 6464 696e 675b 315d 5b30 5d2c 2022  Padding[1][0], "
+00014860: 2d59 5061 6464 696e 6754 7970 653a 3d22  -YPaddingType:="
+00014870: 2c20 5061 6464 696e 6754 7970 652c 0a20  , PaddingType,. 
+00014880: 2020 2020 2020 2020 2020 2022 2d59 5061             "-YPa
+00014890: 6464 696e 673a 3d22 2c20 5061 6464 696e  dding:=", Paddin
+000148a0: 675b 315d 5b31 5d2c 2022 2b5a 5061 6464  g[1][1], "+ZPadd
+000148b0: 696e 6754 7970 653a 3d22 2c20 5061 6464  ingType:=", Padd
+000148c0: 696e 6754 7970 652c 0a20 2020 2020 2020  ingType,.       
+000148d0: 2020 2020 2022 2b5a 5061 6464 696e 673a       "+ZPadding:
+000148e0: 3d22 2c20 5061 6464 696e 675b 325d 5b30  =", Padding[2][0
+000148f0: 5d2c 2022 2d5a 5061 6464 696e 6754 7970  ], "-ZPaddingTyp
+00014900: 653a 3d22 2c20 5061 6464 696e 6754 7970  e:=", PaddingTyp
+00014910: 652c 0a20 2020 2020 2020 2020 2020 2022  e,.            "
+00014920: 2d5a 5061 6464 696e 673a 3d22 2c20 5061  -ZPadding:=", Pa
+00014930: 6464 696e 675b 325d 5b31 5d0a 2020 2020  dding[2][1].    
+00014940: 2020 2020 5d2c 2052 6567 696f 6e41 7474      ], RegionAtt
+00014950: 7269 6275 7465 7329 0a0a 2020 2020 6465  ributes)..    de
+00014960: 6620 756e 6974 6528 7365 6c66 2c20 6e61  f unite(self, na
+00014970: 6d65 732c 206b 6565 705f 6f72 6967 696e  mes, keep_origin
+00014980: 616c 733d 4661 6c73 6529 3a0a 2020 2020  als=False):.    
+00014990: 2020 2020 7365 6c66 2e5f 6d6f 6465 6c65      self._modele
+000149a0: 722e 556e 6974 6528 0a20 2020 2020 2020  r.Unite(.       
+000149b0: 2020 2020 2073 656c 662e 5f73 656c 6563       self._selec
+000149c0: 7469 6f6e 735f 6172 7261 7928 2a6e 616d  tions_array(*nam
+000149d0: 6573 292c 0a20 2020 2020 2020 2020 2020  es),.           
+000149e0: 205b 224e 414d 453a 556e 6974 6550 6172   ["NAME:UnitePar
+000149f0: 616d 6574 6572 7322 2c20 224b 6565 704f  ameters", "KeepO
+00014a00: 7269 6769 6e61 6c73 3a3d 222c 206b 6565  riginals:=", kee
+00014a10: 705f 6f72 6967 696e 616c 735d 290a 2020  p_originals]).  
+00014a20: 2020 2020 2020 7265 7475 726e 206e 616d        return nam
+00014a30: 6573 5b30 5d0a 0a20 2020 2064 6566 2069  es[0]..    def i
+00014a40: 6e74 6572 7365 6374 2873 656c 662c 206e  ntersect(self, n
+00014a50: 616d 6573 2c20 6b65 6570 5f6f 7269 6769  ames, keep_origi
+00014a60: 6e61 6c73 3d46 616c 7365 293a 0a20 2020  nals=False):.   
+00014a70: 2020 2020 2073 656c 662e 5f6d 6f64 656c       self._model
+00014a80: 6572 2e49 6e74 6572 7365 6374 280a 2020  er.Intersect(.  
+00014a90: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00014aa0: 7365 6c65 6374 696f 6e73 5f61 7272 6179  selections_array
+00014ab0: 282a 6e61 6d65 7329 2c0a 2020 2020 2020  (*names),.      
+00014ac0: 2020 2020 2020 5b22 4e41 4d45 3a49 6e74        ["NAME:Int
+00014ad0: 6572 7365 6374 5061 7261 6d65 7465 7273  ersectParameters
+00014ae0: 222c 2022 4b65 6570 4f72 6967 696e 616c  ", "KeepOriginal
+00014af0: 733a 3d22 2c20 6b65 6570 5f6f 7269 6769  s:=", keep_origi
+00014b00: 6e61 6c73 5d29 0a20 2020 2020 2020 2072  nals]).        r
+00014b10: 6574 7572 6e20 6e61 6d65 735b 305d 0a0a  eturn names[0]..
+00014b20: 2020 2020 6465 6620 7472 616e 736c 6174      def translat
+00014b30: 6528 7365 6c66 2c20 6e61 6d65 2c20 7665  e(self, name, ve
+00014b40: 6374 6f72 293a 0a20 2020 2020 2020 2073  ctor):.        s
+00014b50: 656c 662e 5f6d 6f64 656c 6572 2e4d 6f76  elf._modeler.Mov
+00014b60: 6528 7365 6c66 2e5f 7365 6c65 6374 696f  e(self._selectio
+00014b70: 6e73 5f61 7272 6179 286e 616d 6529 2c20  ns_array(name), 
+00014b80: 5b0a 2020 2020 2020 2020 2020 2020 224e  [.            "N
+00014b90: 414d 453a 5472 616e 736c 6174 6550 6172  AME:TranslatePar
+00014ba0: 616d 6574 6572 7322 2c20 2254 7261 6e73  ameters", "Trans
+00014bb0: 6c61 7465 5665 6374 6f72 583a 3d22 2c20  lateVectorX:=", 
+00014bc0: 7665 6374 6f72 5b30 5d2c 0a20 2020 2020  vector[0],.     
+00014bd0: 2020 2020 2020 2022 5472 616e 736c 6174         "Translat
+00014be0: 6556 6563 746f 7259 3a3d 222c 2076 6563  eVectorY:=", vec
+00014bf0: 746f 725b 315d 2c20 2254 7261 6e73 6c61  tor[1], "Transla
+00014c00: 7465 5665 6374 6f72 5a3a 3d22 2c20 7665  teVectorZ:=", ve
+00014c10: 6374 6f72 5b32 5d0a 2020 2020 2020 2020  ctor[2].        
+00014c20: 5d29 0a0a 2020 2020 6465 6620 6765 745f  ])..    def get_
+00014c30: 626f 756e 6461 7279 5f61 7373 6967 6e6d  boundary_assignm
+00014c40: 656e 7428 7365 6c66 2c20 626f 756e 6461  ent(self, bounda
+00014c50: 7279 5f6e 616d 653a 2073 7472 293a 0a20  ry_name: str):. 
+00014c60: 2020 2020 2020 2023 2047 6574 7320 6120         # Gets a 
+00014c70: 6c69 7374 206f 6620 6661 6365 2049 4473  list of face IDs
+00014c80: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+00014c90: 2074 6865 2067 6976 656e 2062 6f75 6e64   the given bound
+00014ca0: 6172 7920 6f72 2065 7863 6974 6174 696f  ary or excitatio
+00014cb0: 6e20 6173 7369 676e 6d65 6e74 2e0a 2020  n assignment..  
+00014cc0: 2020 2020 2020 6f62 6a65 6374 7320 3d20        objects = 
+00014cd0: 7365 6c66 2e5f 626f 756e 6461 7269 6573  self._boundaries
+00014ce0: 2e47 6574 426f 756e 6461 7279 4173 7369  .GetBoundaryAssi
+00014cf0: 676e 6d65 6e74 2862 6f75 6e64 6172 795f  gnment(boundary_
+00014d00: 6e61 6d65 290a 2020 2020 2020 2020 2320  name).        # 
+00014d10: 4765 7473 2061 6e20 6f62 6a65 6374 206e  Gets an object n
+00014d20: 616d 6520 636f 7272 6573 706f 6e64 696e  ame correspondin
+00014d30: 6720 746f 2074 6865 2069 6e70 7574 2066  g to the input f
+00014d40: 6163 6520 6964 2e20 5265 7475 726e 7320  ace id. Returns 
+00014d50: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
+00014d60: 636f 7272 6573 706f 6e64 696e 6720 6f62  corresponding ob
+00014d70: 6a65 6374 206e 616d 652e 0a20 2020 2020  ject name..     
+00014d80: 2020 206f 626a 6563 7473 203d 205b 7365     objects = [se
+00014d90: 6c66 2e5f 6d6f 6465 6c65 722e 4765 744f  lf._modeler.GetO
+00014da0: 626a 6563 744e 616d 6542 7946 6163 6549  bjectNameByFaceI
+00014db0: 4428 6b29 2066 6f72 206b 2069 6e20 6f62  D(k) for k in ob
+00014dc0: 6a65 6374 735d 0a20 2020 2020 2020 2072  jects].        r
+00014dd0: 6574 7572 6e20 6f62 6a65 6374 730a 0a20  eturn objects.. 
+00014de0: 2020 2064 6566 2061 7070 656e 645f 5065     def append_Pe
+00014df0: 7266 455f 6173 7369 676e 6d65 6e74 2873  rfE_assignment(s
+00014e00: 656c 662c 2062 6f75 6e64 6172 795f 6e61  elf, boundary_na
+00014e10: 6d65 3a20 7374 722c 206f 626a 6563 745f  me: str, object_
+00014e20: 6e61 6d65 733a 206c 6973 7429 3a0a 2020  names: list):.  
+00014e30: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00014e40: 2020 2020 2020 5468 6973 2077 696c 6c20        This will 
+00014e50: 6372 6561 7465 2061 206e 6577 2062 6f75  create a new bou
+00014e60: 6e64 6172 7920 6966 206e 6565 642c 2061  ndary if need, a
+00014e70: 6e64 2077 696c 6c0a 2020 2020 2020 2020  nd will.        
+00014e80: 2020 2020 6f74 6865 7277 6973 6520 6170      otherwise ap
+00014e90: 7065 6e64 2067 6976 656e 206e 616d 6573  pend given names
+00014ea0: 2074 6f20 616e 2065 7869 7374 696e 6720   to an existing 
+00014eb0: 626f 756e 6461 7279 0a20 2020 2020 2020  boundary.       
+00014ec0: 2027 2727 0a20 2020 2020 2020 2023 2065   '''.        # e
+00014ed0: 6e66 6f72 6365 0a20 2020 2020 2020 2062  nforce.        b
+00014ee0: 6f75 6e64 6172 795f 6e61 6d65 203d 2073  oundary_name = s
+00014ef0: 7472 2862 6f75 6e64 6172 795f 6e61 6d65  tr(boundary_name
+00014f00: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
+00014f10: 6e73 7461 6e63 6528 6f62 6a65 6374 5f6e  nstance(object_n
+00014f20: 616d 6573 2c20 7374 7229 3a0a 2020 2020  ames, str):.    
+00014f30: 2020 2020 2020 2020 6f62 6a65 6374 5f6e          object_n
+00014f40: 616d 6573 203d 205b 6f62 6a65 6374 5f6e  ames = [object_n
+00014f50: 616d 6573 5d0a 2020 2020 2020 2020 6f62  ames].        ob
+00014f60: 6a65 6374 5f6e 616d 6573 203d 206c 6973  ject_names = lis
+00014f70: 7428 6f62 6a65 6374 5f6e 616d 6573 2920  t(object_names) 
+00014f80: 2023 2065 6e66 6f72 6365 206c 6973 740a   # enforce list.
+00014f90: 0a20 2020 2020 2020 2023 2064 6f20 6163  .        # do ac
+00014fa0: 7475 616c 2077 6f72 6b0a 2020 2020 2020  tual work.      
+00014fb0: 2020 6966 2062 6f75 6e64 6172 795f 6e61    if boundary_na
+00014fc0: 6d65 206e 6f74 2069 6e20 7365 6c66 2e5f  me not in self._
+00014fd0: 626f 756e 6461 7269 6573 2e47 6574 426f  boundaries.GetBo
+00014fe0: 756e 6461 7269 6573 280a 2020 2020 2020  undaries(.      
+00014ff0: 2020 293a 2020 2320 4765 7442 6f75 6e64    ):  # GetBound
+00015000: 6172 6965 734f 6654 7970 6528 2250 6572  ariesOfType("Per
+00015010: 6665 6374 2045 2229 0a20 2020 2020 2020  fect E").       
+00015020: 2020 2020 2023 206e 6565 6420 746f 206d       # need to m
+00015030: 616b 6520 6120 6e65 7720 626f 756e 6461  ake a new bounda
+00015040: 7279 0a20 2020 2020 2020 2020 2020 2073  ry.            s
+00015050: 656c 662e 6173 7369 676e 5f70 6572 6665  elf.assign_perfe
+00015060: 6374 5f45 286f 626a 6563 745f 6e61 6d65  ct_E(object_name
+00015070: 732c 206e 616d 653d 626f 756e 6461 7279  s, name=boundary
+00015080: 5f6e 616d 6529 0a20 2020 2020 2020 2065  _name).        e
+00015090: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000150a0: 2023 206e 6565 6420 746f 2061 7070 656e   # need to appen
+000150b0: 640a 2020 2020 2020 2020 2020 2020 6f62  d.            ob
+000150c0: 6a65 6374 7320 3d20 6c69 7374 2873 656c  jects = list(sel
+000150d0: 662e 6765 745f 626f 756e 6461 7279 5f61  f.get_boundary_a
+000150e0: 7373 6967 6e6d 656e 7428 626f 756e 6461  ssignment(bounda
+000150f0: 7279 5f6e 616d 6529 290a 2020 2020 2020  ry_name)).      
+00015100: 2020 2020 2020 7365 6c66 2e5f 626f 756e        self._boun
+00015110: 6461 7269 6573 2e52 6561 7373 6967 6e42  daries.ReassignB
+00015120: 6f75 6e64 6172 7928 5b0a 2020 2020 2020  oundary([.      
+00015130: 2020 2020 2020 2020 2020 224e 414d 453a            "NAME:
+00015140: 2220 2b20 626f 756e 6461 7279 5f6e 616d  " + boundary_nam
+00015150: 652c 2022 4f62 6a65 6374 733a 3d22 2c0a  e, "Objects:=",.
+00015160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015170: 6c69 7374 2873 6574 286f 626a 6563 7473  list(set(objects
+00015180: 202b 206f 626a 6563 745f 6e61 6d65 7329   + object_names)
+00015190: 290a 2020 2020 2020 2020 2020 2020 5d29  ).            ])
+000151a0: 0a0a 2020 2020 6465 6620 6170 7065 6e64  ..    def append
+000151b0: 5f6d 6573 6828 7365 6c66 2c20 6d65 7368  _mesh(self, mesh
+000151c0: 5f6e 616d 653a 2073 7472 2c20 6f62 6a65  _name: str, obje
+000151d0: 6374 5f6e 616d 6573 3a20 6c69 7374 2c20  ct_names: list, 
+000151e0: 6f6c 645f 6f62 6a73 3a20 6c69 7374 2c0a  old_objs: list,.
+000151f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015200: 2020 2020 2a2a 6b77 6172 6773 293a 0a20      **kwargs):. 
+00015210: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00015220: 2020 2054 6869 7320 7769 6c6c 2063 7265     This will cre
+00015230: 6174 6520 6120 6e65 7720 626f 756e 6461  ate a new bounda
+00015240: 7279 2069 6620 6e65 6564 2c20 616e 6420  ry if need, and 
+00015250: 7769 6c6c 0a20 2020 2020 2020 206f 7468  will.        oth
+00015260: 6572 7769 7365 2061 7070 656e 6420 6769  erwise append gi
+00015270: 7665 6e20 6e61 6d65 7320 746f 2061 6e20  ven names to an 
+00015280: 6578 6973 7469 6e67 2062 6f75 6e64 6172  existing boundar
+00015290: 790a 2020 2020 2020 2020 6f6c 645f 6f62  y.        old_ob
+000152a0: 6a20 3d20 6369 7263 2e5f 6d65 7368 5f61  j = circ._mesh_a
+000152b0: 7373 6967 6e0a 2020 2020 2020 2020 2727  ssign.        ''
+000152c0: 270a 2020 2020 2020 2020 6d65 7368 5f6e  '.        mesh_n
+000152d0: 616d 6520 3d20 7374 7228 6d65 7368 5f6e  ame = str(mesh_n
+000152e0: 616d 6529 0a20 2020 2020 2020 2069 6620  ame).        if 
+000152f0: 6973 696e 7374 616e 6365 286f 626a 6563  isinstance(objec
+00015300: 745f 6e61 6d65 732c 2073 7472 293a 0a20  t_names, str):. 
+00015310: 2020 2020 2020 2020 2020 206f 626a 6563             objec
+00015320: 745f 6e61 6d65 7320 3d20 5b6f 626a 6563  t_names = [objec
+00015330: 745f 6e61 6d65 735d 0a20 2020 2020 2020  t_names].       
+00015340: 206f 626a 6563 745f 6e61 6d65 7320 3d20   object_names = 
+00015350: 6c69 7374 286f 626a 6563 745f 6e61 6d65  list(object_name
+00015360: 7329 2020 2320 656e 666f 7263 6520 6c69  s)  # enforce li
+00015370: 7374 0a0a 2020 2020 2020 2020 6966 206d  st..        if m
+00015380: 6573 685f 6e61 6d65 206e 6f74 2069 6e20  esh_name not in 
+00015390: 7365 6c66 2e6d 6573 685f 6765 745f 6e61  self.mesh_get_na
+000153a0: 6d65 7328 0a20 2020 2020 2020 2029 3a20  mes(.        ): 
+000153b0: 2023 206e 6565 6420 746f 206d 616b 6520   # need to make 
+000153c0: 6120 6e65 7720 626f 756e 6461 7279 0a20  a new boundary. 
+000153d0: 2020 2020 2020 2020 2020 206f 626a 7320             objs 
+000153e0: 3d20 6f62 6a65 6374 5f6e 616d 6573 0a20  = object_names. 
+000153f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015400: 6d65 7368 5f6c 656e 6774 6828 6d65 7368  mesh_length(mesh
+00015410: 5f6e 616d 652c 206f 626a 6563 745f 6e61  _name, object_na
+00015420: 6d65 732c 202a 2a6b 7761 7267 7329 0a20  mes, **kwargs). 
+00015430: 2020 2020 2020 2065 6c73 653a 2020 2320         else:  # 
+00015440: 6e65 6564 2074 6f20 6170 7065 6e64 0a20  need to append. 
+00015450: 2020 2020 2020 2020 2020 206f 626a 7320             objs 
+00015460: 3d20 6c69 7374 2873 6574 286f 6c64 5f6f  = list(set(old_o
+00015470: 626a 7320 2b20 6f62 6a65 6374 5f6e 616d  bjs + object_nam
+00015480: 6573 2929 0a20 2020 2020 2020 2020 2020  es)).           
+00015490: 2073 656c 662e 6d65 7368 5f72 6561 7373   self.mesh_reass
+000154a0: 6967 6e28 6d65 7368 5f6e 616d 652c 206f  ign(mesh_name, o
+000154b0: 626a 7329 0a0a 2020 2020 2020 2020 7265  bjs)..        re
+000154c0: 7475 726e 206f 626a 730a 0a20 2020 2064  turn objs..    d
+000154d0: 6566 2061 7373 6967 6e5f 7065 7266 6563  ef assign_perfec
+000154e0: 745f 4528 7365 6c66 2c20 6f62 6a3a 204c  t_E(self, obj: L
+000154f0: 6973 745b 7374 725d 2c20 6e61 6d65 3a20  ist[str], name: 
+00015500: 7374 7220 3d20 2750 6572 6645 2729 3a0a  str = 'PerfE'):.
+00015510: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00015520: 2020 2020 4173 7369 676e 2061 2062 6f75      Assign a bou
+00015530: 6e64 6172 7920 636f 6e64 6974 696f 6e20  ndary condition 
+00015540: 746f 2061 206c 6973 7420 6f66 206f 626a  to a list of obj
+00015550: 6563 7473 2e0a 0a20 2020 2020 2020 2041  ects...        A
+00015560: 7267 3a0a 2020 2020 2020 2020 2020 2020  rg:.            
+00015570: 6f62 6a73 2028 4c69 7374 5b73 7472 5d29  objs (List[str])
+00015580: 3a20 5461 6b65 7320 6120 6e61 6d65 206f  : Takes a name o
+00015590: 6620 616e 206f 626a 6563 7420 6f72 2061  f an object or a
+000155a0: 206c 6973 7420 6f66 206f 626a 6563 7420   list of object 
+000155b0: 6e61 6d65 732e 0a20 2020 2020 2020 2020  names..         
+000155c0: 2020 206e 616d 6528 7374 7229 3a20 4966     name(str): If
+000155d0: 2060 6e61 6d65 6020 6973 206e 6f74 2073   `name` is not s
+000155e0: 7065 6369 6669 6564 2060 5065 7266 4560  pecified `PerfE`
+000155f0: 2069 7320 6170 7065 6e64 6564 2074 6f20   is appended to 
+00015600: 6f62 6a65 6374 206e 616d 6520 666f 7220  object name for 
+00015610: 7468 6520 6e61 6d65 2e0a 2020 2020 2020  the name..      
+00015620: 2020 2727 270a 2020 2020 2020 2020 6966    '''.        if
+00015630: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+00015640: 6f62 6a2c 206c 6973 7429 3a0a 2020 2020  obj, list):.    
+00015650: 2020 2020 2020 2020 6f62 6a20 3d20 5b6f          obj = [o
+00015660: 626a 5d0a 2020 2020 2020 2020 2020 2020  bj].            
+00015670: 6966 206e 616d 6520 3d3d 2027 5065 7266  if name == 'Perf
+00015680: 4527 3a0a 2020 2020 2020 2020 2020 2020  E':.            
+00015690: 2020 2020 6e61 6d65 203d 2073 7472 286f      name = str(o
+000156a0: 626a 2920 2b20 275f 2720 2b20 6e61 6d65  bj) + '_' + name
+000156b0: 0a20 2020 2020 2020 206e 616d 6520 3d20  .        name = 
+000156c0: 696e 6372 656d 656e 745f 6e61 6d65 286e  increment_name(n
+000156d0: 616d 652c 2073 656c 662e 5f62 6f75 6e64  ame, self._bound
+000156e0: 6172 6965 732e 4765 7442 6f75 6e64 6172  aries.GetBoundar
+000156f0: 6965 7328 2929 0a20 2020 2020 2020 2073  ies()).        s
+00015700: 656c 662e 5f62 6f75 6e64 6172 6965 732e  elf._boundaries.
+00015710: 4173 7369 676e 5065 7266 6563 7445 280a  AssignPerfectE(.
+00015720: 2020 2020 2020 2020 2020 2020 5b22 4e41              ["NA
+00015730: 4d45 3a22 202b 206e 616d 652c 2022 4f62  ME:" + name, "Ob
+00015740: 6a65 6374 733a 3d22 2c20 6f62 6a2c 2022  jects:=", obj, "
+00015750: 496e 6647 726f 756e 6450 6c61 6e65 3a3d  InfGroundPlane:=
+00015760: 222c 2046 616c 7365 5d29 0a0a 2020 2020  ", False])..    
+00015770: 6465 6620 5f6d 616b 655f 6c75 6d70 6564  def _make_lumped
+00015780: 5f72 6c63 2873 656c 662c 2072 2c20 6c2c  _rlc(self, r, l,
+00015790: 2063 2c20 7374 6172 742c 2065 6e64 2c20   c, start, end, 
+000157a0: 6f62 6a5f 6172 722c 206e 616d 653d 224c  obj_arr, name="L
+000157b0: 756d 7052 4c43 2229 3a0a 2020 2020 2020  umpRLC"):.      
+000157c0: 2020 6e61 6d65 203d 2069 6e63 7265 6d65    name = increme
+000157d0: 6e74 5f6e 616d 6528 6e61 6d65 2c20 7365  nt_name(name, se
+000157e0: 6c66 2e5f 626f 756e 6461 7269 6573 2e47  lf._boundaries.G
+000157f0: 6574 426f 756e 6461 7269 6573 2829 290a  etBoundaries()).
+00015800: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
+00015810: 205b 224e 414d 453a 2220 2b20 6e61 6d65   ["NAME:" + name
+00015820: 5d0a 2020 2020 2020 2020 7061 7261 6d73  ].        params
+00015830: 202b 3d20 6f62 6a5f 6172 720a 2020 2020   += obj_arr.    
+00015840: 2020 2020 7061 7261 6d73 2e61 7070 656e      params.appen
+00015850: 6428 5b0a 2020 2020 2020 2020 2020 2020  d([.            
+00015860: 224e 414d 453a 4375 7272 656e 744c 696e  "NAME:CurrentLin
+00015870: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00015880: 2320 666f 7220 736f 6d65 2072 6561 736f  # for some reaso
+00015890: 6e20 6865 7265 2069 7420 7365 656d 7320  n here it seems 
+000158a0: 746f 2073 7769 7463 6820 746f 2075 7365  to switch to use
+000158b0: 2074 6865 206d 6f64 656c 2075 6e69 7473   the model units
+000158c0: 2c20 7261 7468 6572 2074 6861 6e20 6d65  , rather than me
+000158d0: 7465 7273 0a20 2020 2020 2020 2020 2020  ters.           
+000158e0: 2022 5374 6172 743a 3d22 2c0a 2020 2020   "Start:=",.    
+000158f0: 2020 2020 2020 2020 6669 785f 756e 6974          fix_unit
+00015900: 7328 7374 6172 742c 2075 6e69 745f 6173  s(start, unit_as
+00015910: 7375 6d65 643d 4c45 4e47 5448 5f55 4e49  sumed=LENGTH_UNI
+00015920: 5429 2c0a 2020 2020 2020 2020 2020 2020  T),.            
+00015930: 2245 6e64 3a3d 222c 0a20 2020 2020 2020  "End:=",.       
+00015940: 2020 2020 2066 6978 5f75 6e69 7473 2865       fix_units(e
+00015950: 6e64 2c20 756e 6974 5f61 7373 756d 6564  nd, unit_assumed
+00015960: 3d4c 454e 4754 485f 554e 4954 290a 2020  =LENGTH_UNIT).  
+00015970: 2020 2020 2020 5d29 0a20 2020 2020 2020        ]).       
+00015980: 2070 6172 616d 7320 2b3d 205b 0a20 2020   params += [.   
+00015990: 2020 2020 2020 2020 2022 5573 6552 6573           "UseRes
+000159a0: 6973 743a 3d22 2c20 7220 213d 2030 2c20  ist:=", r != 0, 
+000159b0: 2252 6573 6973 7461 6e63 653a 3d22 2c20  "Resistance:=", 
+000159c0: 722c 2022 5573 6549 6e64 7563 743a 3d22  r, "UseInduct:="
+000159d0: 2c20 6c20 213d 2030 2c0a 2020 2020 2020  , l != 0,.      
+000159e0: 2020 2020 2020 2249 6e64 7563 7461 6e63        "Inductanc
+000159f0: 653a 3d22 2c20 6c2c 2022 5573 6543 6170  e:=", l, "UseCap
+00015a00: 3a3d 222c 2063 2021 3d20 302c 2022 4361  :=", c != 0, "Ca
+00015a10: 7061 6369 7461 6e63 653a 3d22 2c20 630a  pacitance:=", c.
+00015a20: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00015a30: 2020 7365 6c66 2e5f 626f 756e 6461 7269    self._boundari
+00015a40: 6573 2e41 7373 6967 6e4c 756d 7065 6452  es.AssignLumpedR
+00015a50: 4c43 2870 6172 616d 7329 0a0a 2020 2020  LC(params)..    
+00015a60: 6465 6620 5f6d 616b 655f 6c75 6d70 6564  def _make_lumped
+00015a70: 5f70 6f72 7428 7365 6c66 2c0a 2020 2020  _port(self,.    
+00015a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a90: 2020 2020 2020 7374 6172 742c 0a20 2020        start,.   
+00015aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ab0: 2020 2020 2020 2065 6e64 2c0a 2020 2020         end,.    
+00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ad0: 2020 2020 2020 6f62 6a5f 6172 722c 0a20        obj_arr,. 
+00015ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015af0: 2020 2020 2020 2020 207a 303d 2235 306f           z0="50o
+00015b00: 686d 222c 0a20 2020 2020 2020 2020 2020  hm",.           
+00015b10: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00015b20: 616d 653d 224c 756d 7050 6f72 7422 293a  ame="LumpPort"):
+00015b30: 0a20 2020 2020 2020 2073 7461 7274 203d  .        start =
+00015b40: 2066 6978 5f75 6e69 7473 2873 7461 7274   fix_units(start
+00015b50: 2c20 756e 6974 5f61 7373 756d 6564 3d4c  , unit_assumed=L
+00015b60: 454e 4754 485f 554e 4954 290a 2020 2020  ENGTH_UNIT).    
+00015b70: 2020 2020 656e 6420 3d20 6669 785f 756e      end = fix_un
+00015b80: 6974 7328 656e 642c 2075 6e69 745f 6173  its(end, unit_as
+00015b90: 7375 6d65 643d 4c45 4e47 5448 5f55 4e49  sumed=LENGTH_UNI
+00015ba0: 5429 0a0a 2020 2020 2020 2020 6e61 6d65  T)..        name
+00015bb0: 203d 2069 6e63 7265 6d65 6e74 5f6e 616d   = increment_nam
+00015bc0: 6528 6e61 6d65 2c20 7365 6c66 2e5f 626f  e(name, self._bo
+00015bd0: 756e 6461 7269 6573 2e47 6574 426f 756e  undaries.GetBoun
+00015be0: 6461 7269 6573 2829 290a 2020 2020 2020  daries()).      
+00015bf0: 2020 7061 7261 6d73 203d 205b 224e 414d    params = ["NAM
+00015c00: 453a 2220 2b20 6e61 6d65 5d0a 2020 2020  E:" + name].    
+00015c10: 2020 2020 7061 7261 6d73 202b 3d20 6f62      params += ob
+00015c20: 6a5f 6172 720a 2020 2020 2020 2020 7061  j_arr.        pa
+00015c30: 7261 6d73 202b 3d20 5b0a 2020 2020 2020  rams += [.      
+00015c40: 2020 2020 2020 2252 656e 6f72 6d61 6c69        "Renormali
+00015c50: 7a65 416c 6c54 6572 6d69 6e61 6c73 3a3d  zeAllTerminals:=
+00015c60: 222c 2054 7275 652c 2022 446f 4465 656d  ", True, "DoDeem
+00015c70: 6265 643a 3d22 2c20 4661 6c73 652c 0a20  bed:=", False,. 
+00015c80: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+00015c90: 2020 2020 2020 2020 2020 2020 2022 4e41               "NA
+00015ca0: 4d45 3a4d 6f64 6573 222c 0a20 2020 2020  ME:Modes",.     
+00015cb0: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
+00015cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cd0: 2022 4e41 4d45 3a4d 6f64 6531 222c 2022   "NAME:Mode1", "
+00015ce0: 4d6f 6465 4e75 6d3a 3d22 2c20 312c 2022  ModeNum:=", 1, "
+00015cf0: 5573 6549 6e74 4c69 6e65 3a3d 222c 2054  UseIntLine:=", T
+00015d00: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00015d10: 2020 2020 2020 2020 205b 224e 414d 453a           ["NAME:
+00015d20: 496e 744c 696e 6522 2c20 2253 7461 7274  IntLine", "Start
+00015d30: 3a3d 222c 2073 7461 7274 2c20 2245 6e64  :=", start, "End
+00015d40: 3a3d 222c 0a20 2020 2020 2020 2020 2020  :=",.           
+00015d50: 2020 2020 2020 2020 2020 656e 645d 2c20            end], 
+00015d60: 2243 6861 7249 6d70 3a3d 222c 2022 5a70  "CharImp:=", "Zp
+00015d70: 6922 2c20 2241 6c69 676e 6d65 6e74 4772  i", "AlignmentGr
+00015d80: 6f75 703a 3d22 2c20 302c 0a20 2020 2020  oup:=", 0,.     
+00015d90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00015da0: 5265 6e6f 726d 496d 703a 3d22 2c20 2235  RenormImp:=", "5
+00015db0: 306f 686d 220a 2020 2020 2020 2020 2020  0ohm".          
+00015dc0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00015dd0: 2020 2020 5d2c 2022 5368 6f77 5265 706f      ], "ShowRepo
+00015de0: 7274 6572 4669 6c74 6572 3a3d 222c 2046  rterFilter:=", F
+00015df0: 616c 7365 2c20 2252 6570 6f72 7465 7246  alse, "ReporterF
+00015e00: 696c 7465 723a 3d22 2c20 5b54 7275 655d  ilter:=", [True]
+00015e10: 2c0a 2020 2020 2020 2020 2020 2020 2246  ,.            "F
+00015e20: 756c 6c52 6573 6973 7461 6e63 653a 3d22  ullResistance:="
+00015e30: 2c20 7a30 2c20 2246 756c 6c52 6561 6374  , z0, "FullReact
+00015e40: 616e 6365 3a3d 222c 2022 306f 686d 220a  ance:=", "0ohm".
+00015e50: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
+00015e60: 2020 2073 656c 662e 5f62 6f75 6e64 6172     self._boundar
+00015e70: 6965 732e 4173 7369 676e 4c75 6d70 6564  ies.AssignLumped
+00015e80: 506f 7274 2870 6172 616d 7329 0a0a 2020  Port(params)..  
+00015e90: 2020 6465 6620 6765 745f 6661 6365 5f69    def get_face_i
+00015ea0: 6473 2873 656c 662c 206f 626a 293a 0a20  ds(self, obj):. 
+00015eb0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00015ec0: 6c66 2e5f 6d6f 6465 6c65 722e 4765 7446  lf._modeler.GetF
+00015ed0: 6163 6549 4473 286f 626a 290a 0a20 2020  aceIDs(obj)..   
+00015ee0: 2064 6566 2067 6574 5f6f 626a 6563 745f   def get_object_
+00015ef0: 6e61 6d65 5f62 795f 6661 6365 5f69 6428  name_by_face_id(
+00015f00: 7365 6c66 2c20 4944 3a20 7374 7229 3a0a  self, ID: str):.
+00015f10: 2020 2020 2020 2020 2727 2720 4765 7473          ''' Gets
+00015f20: 2061 6e20 6f62 6a65 6374 206e 616d 6520   an object name 
+00015f30: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
+00015f40: 2074 6865 2069 6e70 7574 2066 6163 6520   the input face 
+00015f50: 6964 2e20 2727 270a 2020 2020 2020 2020  id. '''.        
+00015f60: 7265 7475 726e 2073 656c 662e 5f6d 6f64  return self._mod
+00015f70: 656c 6572 2e47 6574 4f62 6a65 6374 4e61  eler.GetObjectNa
+00015f80: 6d65 4279 4661 6365 4944 2849 4429 0a0a  meByFaceID(ID)..
+00015f90: 2020 2020 6465 6620 6765 745f 7665 7274      def get_vert
+00015fa0: 6578 5f69 6473 2873 656c 662c 206f 626a  ex_ids(self, obj
+00015fb0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00015fc0: 2020 2020 2020 2020 2020 2047 6574 2074             Get t
+00015fd0: 6865 2076 6572 7465 7820 4944 7320 6f66  he vertex IDs of
+00015fe0: 2067 6976 656e 2061 6e20 6f62 6a65 6374   given an object
+00015ff0: 206e 616d 650a 2020 2020 2020 2020 2020   name.          
+00016000: 2020 6f56 6572 7465 7849 4473 203d 206f    oVertexIDs = o
+00016010: 4564 6974 6f72 2e47 6574 5665 7274 6578  Editor.GetVertex
+00016020: 4944 7346 726f 6d4f 626a 6563 7428 e280  IDsFromObject(..
+00016030: 9c42 6f78 31e2 809d 290a 2020 2020 2020  .Box1...).      
+00016040: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00016050: 7475 726e 2073 656c 662e 5f6d 6f64 656c  turn self._model
+00016060: 6572 2e47 6574 5665 7274 6578 4944 7346  er.GetVertexIDsF
+00016070: 726f 6d4f 626a 6563 7428 6f62 6a29 0a0a  romObject(obj)..
+00016080: 2020 2020 6465 6620 6576 616c 5f65 7870      def eval_exp
+00016090: 7228 7365 6c66 2c20 6578 7072 2c20 756e  r(self, expr, un
+000160a0: 6974 733d 226d 6d22 293a 0a20 2020 2020  its="mm"):.     
+000160b0: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
+000160c0: 616e 6365 2865 7870 722c 2073 7472 293a  ance(expr, str):
+000160d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000160e0: 7572 6e20 6578 7072 0a20 2020 2020 2020  urn expr.       
+000160f0: 2072 6574 7572 6e20 7365 6c66 2e70 6172   return self.par
+00016100: 656e 742e 6576 616c 5f65 7870 7228 6578  ent.eval_expr(ex
+00016110: 7072 2c20 756e 6974 7329 0a0a 2020 2020  pr, units)..    
+00016120: 6465 6620 6765 745f 6f62 6a65 6374 735f  def get_objects_
+00016130: 696e 5f67 726f 7570 2873 656c 662c 2067  in_group(self, g
+00016140: 726f 7570 293a 0a20 2020 2020 2020 2022  roup):.        "
+00016150: 2222 0a20 2020 2020 2020 2055 7365 3a20  "".        Use: 
+00016160: 2020 2020 2020 2020 2020 2020 2052 6574               Ret
+00016170: 7572 6e73 2074 6865 206f 626a 6563 7473  urns the objects
+00016180: 2066 6f72 2074 6865 2073 7065 6369 6669   for the specifi
+00016190: 6564 2067 726f 7570 2e0a 2020 2020 2020  ed group..      
+000161a0: 2020 5265 7475 726e 2056 616c 7565 3a20    Return Value: 
+000161b0: 2020 2054 6865 206f 626a 6563 7473 2069     The objects i
+000161c0: 6e20 7468 6520 6772 6f75 702e 0a20 2020  n the group..   
+000161d0: 2020 2020 2050 6172 616d 6574 6572 733a       Parameters:
+000161e0: 2020 2020 2020 3c67 726f 7570 4e61 6d65        <groupName
+000161f0: 3e20 2054 7970 653a 203c 7374 7269 6e67  >  Type: <string
+00016200: 3e0a 2020 2020 2020 2020 4f6e 6520 6f66  >.        One of
+00016210: 2020 3c6d 6174 6572 6961 6c4e 616d 653e    <materialName>
+00016220: 2c20 3c61 7373 6967 6e6d 656e 744e 616d  , <assignmentNam
+00016230: 653e 2c20 224e 6f6e 204d 6f64 656c 222c  e>, "Non Model",
+00016240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016250: 2022 536f 6c69 6473 222c 2022 556e 636c   "Solids", "Uncl
+00016260: 6173 7369 c2ad 6669 6564 222c 2022 5368  assi..fied", "Sh
+00016270: 6565 7473 222c 2022 4c69 6e65 7322 0a20  eets", "Lines". 
+00016280: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016290: 2020 2069 6620 7365 6c66 2e5f 6d6f 6465     if self._mode
+000162a0: 6c65 723a 0a20 2020 2020 2020 2020 2020  ler:.           
+000162b0: 2072 6574 7572 6e20 6c69 7374 2873 656c   return list(sel
+000162c0: 662e 5f6d 6f64 656c 6572 2e47 6574 4f62  f._modeler.GetOb
+000162d0: 6a65 6374 7349 6e47 726f 7570 2867 726f  jectsInGroup(gro
+000162e0: 7570 2929 0a20 2020 2020 2020 2065 6c73  up)).        els
+000162f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00016300: 6574 7572 6e20 6c69 7374 2829 0a0a 2020  eturn list()..  
+00016310: 2020 6465 6620 7365 745f 776f 726b 696e    def set_workin
+00016320: 675f 636f 6f72 6469 6e61 7465 5f73 7973  g_coordinate_sys
+00016330: 7465 6d28 7365 6c66 2c20 6373 5f6e 616d  tem(self, cs_nam
+00016340: 653d 2247 6c6f 6261 6c22 293a 0a20 2020  e="Global"):.   
+00016350: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00016360: 2055 7365 3a20 2020 2020 2020 2020 2020   Use:           
+00016370: 2020 2020 2020 2020 5365 7473 2074 6865          Sets the
+00016380: 2077 6f72 6b69 6e67 2063 6f6f 7264 696e   working coordin
+00016390: 6174 6520 7379 7374 656d 2e0a 2020 2020  ate system..    
+000163a0: 2020 2020 436f 6d6d 616e 643a 2020 2020      Command:    
+000163b0: 2020 2020 204d 6f64 656c 6572 3e43 6f6f       Modeler>Coo
+000163c0: 7264 696e 6174 6520 5379 7374 656d 3e53  rdinate System>S
+000163d0: 6574 2057 6f72 6b69 6e67 2043 530a 2020  et Working CS.  
+000163e0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000163f0: 2020 7365 6c66 2e5f 6d6f 6465 6c65 722e    self._modeler.
+00016400: 5365 7457 4353 285b 0a20 2020 2020 2020  SetWCS([.       
+00016410: 2020 2020 2022 4e41 4d45 3a53 6574 5743       "NAME:SetWC
+00016420: 5320 5061 7261 6d65 7465 7222 2c0a 2020  S Parameter",.  
+00016430: 2020 2020 2020 2020 2020 2257 6f72 6b69            "Worki
+00016440: 6e67 2043 6f6f 7264 696e 6174 6520 5379  ng Coordinate Sy
+00016450: 7374 656d 3a3d 222c 0a20 2020 2020 2020  stem:=",.       
+00016460: 2020 2020 2063 735f 6e61 6d65 2c0a 2020       cs_name,.  
+00016470: 2020 2020 2020 2020 2020 2252 6567 696f            "Regio
+00016480: 6e44 6570 4353 4f6b 3a3d 222c 0a20 2020  nDepCSOk:=",.   
+00016490: 2020 2020 2020 2020 2046 616c 7365 2020           False  
+000164a0: 2320 7468 6973 206f 6e65 2069 7320 7072  # this one is pr
+000164b0: 6f62 206e 6f74 206e 6565 6465 642c 2062  ob not needed, b
+000164c0: 7574 2063 6f6d 6573 2077 6974 6820 7468  ut comes with th
+000164d0: 6520 7265 636f 7264 2074 6f6f 6c0a 2020  e record tool.  
+000164e0: 2020 2020 2020 5d29 0a0a 2020 2020 6465        ])..    de
+000164f0: 6620 6372 6561 7465 5f72 656c 6174 6976  f create_relativ
+00016500: 655f 636f 6f72 696e 6174 655f 7379 7374  e_coorinate_syst
+00016510: 656d 5f62 6f74 6828 7365 6c66 2c0a 2020  em_both(self,.  
+00016520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016540: 2020 2020 2020 2020 2020 2020 6373 5f6e              cs_n
+00016550: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00016560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016580: 2020 206f 7269 6769 6e3d 5b22 3075 6d22     origin=["0um"
+00016590: 2c20 2230 756d 222c 2022 3075 6d22 5d2c  , "0um", "0um"],
+000165a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000165b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000165c0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+000165d0: 4178 6973 5665 633d 5b22 3175 6d22 2c20  AxisVec=["1um", 
+000165e0: 2230 756d 222c 2022 3075 6d22 5d2c 0a20  "0um", "0um"],. 
+000165f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016610: 2020 2020 2020 2020 2020 2020 2059 4178               YAx
+00016620: 6973 5665 633d 5b22 3075 6d22 2c20 2231  isVec=["0um", "1
+00016630: 756d 222c 2022 3075 6d22 5d29 3a0a 2020  um", "0um"]):.  
+00016640: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00016650: 2020 5573 653a 2020 2020 2043 7265 6174    Use:     Creat
+00016660: 6573 2061 2072 656c 6174 6976 6520 636f  es a relative co
+00016670: 6f72 6469 6e61 7465 2073 7973 7465 6d2e  ordinate system.
+00016680: 204f 6e6c 7920 7468 6520 2020 204e 616d   Only the    Nam
+00016690: 6520 6174 7472 6962 7574 6520 6f66 2074  e attribute of t
+000166a0: 6865 203c 4174 7472 6962 7574 6573 4172  he <AttributesAr
+000166b0: 7261 793e 2070 6172 616d 6574 6572 2069  ray> parameter i
+000166c0: 7320 7375 7070 6f72 7465 642e 0a20 2020  s supported..   
+000166d0: 2020 2020 2043 6f6d 6d61 6e64 3a20 4d6f       Command: Mo
+000166e0: 6465 6c65 723e 436f 6f72 6469 6e61 7465  deler>Coordinate
+000166f0: 2053 7973 7465 6d3e 4372 6561 7465 3e52   System>Create>R
+00016700: 656c 6174 6976 6520 4353 2d3e 4f66 6673  elative CS->Offs
+00016710: 6574 0a20 2020 2020 2020 204d 6f64 656c  et.        Model
+00016720: 6572 3e43 6f6f 7264 696e 6174 6520 5379  er>Coordinate Sy
+00016730: 7374 656d 3e43 7265 6174 653e 5265 6c61  stem>Create>Rela
+00016740: 7469 7665 2043 532d 3e52 6f74 6174 6564  tive CS->Rotated
+00016750: 0a20 2020 2020 2020 204d 6f64 656c 6572  .        Modeler
+00016760: 3e43 6f6f 7264 696e 6174 6520 5379 7374  >Coordinate Syst
+00016770: 656d 3e43 7265 6174 653e 5265 6c61 7469  em>Create>Relati
+00016780: 7665 2043 532d 3e42 6f74 680a 0a20 2020  ve CS->Both..   
+00016790: 2020 2020 2043 7572 7265 6e74 2063 6f6f       Current coo
+000167a0: 7264 696e 6174 6520 7379 7374 656d 2069  rdinate system i
+000167b0: 7320 7365 7420 7269 6768 7420 6166 7465  s set right afte
+000167c0: 7220 7468 6973 2e0a 0a20 2020 2020 2020  r this...       
+000167d0: 2063 735f 6e61 6d65 203a 206e 616d 6520   cs_name : name 
+000167e0: 6f66 2063 6f6f 7264 2e20 7379 730a 2020  of coord. sys.  
+000167f0: 2020 2020 2020 2020 2020 4966 2074 6865            If the
+00016800: 206e 616d 6520 616c 7265 6164 7920 6578   name already ex
+00016810: 6973 7473 2c20 7468 656e 2061 206e 6577  ists, then a new
+00016820: 2063 6f6f 7264 696e 6174 6520 7379 7374   coordinate syst
+00016830: 656d 2077 6974 6820 5f31 2069 7320 6372  em with _1 is cr
+00016840: 6561 7465 642e 0a0a 2020 2020 2020 2020  eated...        
+00016850: 6f72 6967 696e 2c20 5841 7869 7356 6563  origin, XAxisVec
+00016860: 2c20 5941 7869 7356 6563 3a20 332d 7665  , YAxisVec: 3-ve
+00016870: 6374 6f72 730a 2020 2020 2020 2020 2020  ctors.          
+00016880: 2020 596f 7520 6361 6e20 616c 736f 2070    You can also p
+00016890: 6173 7320 696e 2070 6172 616d 7320 7375  ass in params su
+000168a0: 6368 2061 7320 6f72 6967 696e 203d 205b  ch as origin = [
+000168b0: 302c 312c 305d 2072 6174 6865 7220 7468  0,1,0] rather th
+000168c0: 616e 205b 2230 756d 222c 2231 756d 222c  an ["0um","1um",
+000168d0: 2230 756d 225d 2c20 6275 7420 7468 6573  "0um"], but thes
+000168e0: 6520 7769 6c6c 2062 6520 696e 7465 7270  e will be interp
+000168f0: 7265 7465 6420 696e 2064 6566 6175 6c74  reted in default
+00016900: 2075 6e69 7473 2c20 736f 2069 7420 6973   units, so it is
+00016910: 2073 6166 6572 2074 6f20 6265 2065 7870   safer to be exp
+00016920: 6c69 6369 742e 2045 7870 6c69 6369 7420  licit. Explicit 
+00016930: 6f76 6572 2069 6d70 6c69 6369 742e 0a20  over implicit.. 
+00016940: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016950: 2020 2073 656c 662e 5f6d 6f64 656c 6572     self._modeler
+00016960: 2e43 7265 6174 6552 656c 6174 6976 6543  .CreateRelativeC
+00016970: 5328 5b0a 2020 2020 2020 2020 2020 2020  S([.            
+00016980: 224e 414d 453a 5265 6c61 7469 7665 4353  "NAME:RelativeCS
+00016990: 5061 7261 6d65 7465 7273 222c 2022 4d6f  Parameters", "Mo
+000169a0: 6465 3a3d 222c 2022 4178 6973 2f50 6f73  de:=", "Axis/Pos
+000169b0: 6974 696f 6e22 2c0a 2020 2020 2020 2020  ition",.        
+000169c0: 2020 2020 224f 7269 6769 6e58 3a3d 222c      "OriginX:=",
+000169d0: 206f 7269 6769 6e5b 305d 2c20 224f 7269   origin[0], "Ori
+000169e0: 6769 6e59 3a3d 222c 206f 7269 6769 6e5b  ginY:=", origin[
+000169f0: 315d 2c20 224f 7269 6769 6e5a 3a3d 222c  1], "OriginZ:=",
+00016a00: 0a20 2020 2020 2020 2020 2020 206f 7269  .            ori
+00016a10: 6769 6e5b 325d 2c20 2258 4178 6973 5876  gin[2], "XAxisXv
+00016a20: 6563 3a3d 222c 2058 4178 6973 5665 635b  ec:=", XAxisVec[
+00016a30: 305d 2c20 2258 4178 6973 5976 6563 3a3d  0], "XAxisYvec:=
+00016a40: 222c 2058 4178 6973 5665 635b 315d 2c0a  ", XAxisVec[1],.
+00016a50: 2020 2020 2020 2020 2020 2020 2258 4178              "XAx
+00016a60: 6973 5a76 6563 3a3d 222c 2058 4178 6973  isZvec:=", XAxis
+00016a70: 5665 635b 325d 2c20 2259 4178 6973 5876  Vec[2], "YAxisXv
+00016a80: 6563 3a3d 222c 2059 4178 6973 5665 635b  ec:=", YAxisVec[
+00016a90: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+00016aa0: 2259 4178 6973 5976 6563 3a3d 222c 2059  "YAxisYvec:=", Y
+00016ab0: 4178 6973 5665 635b 315d 2c20 2259 4178  AxisVec[1], "YAx
+00016ac0: 6973 5a76 6563 3a3d 222c 2059 4178 6973  isZvec:=", YAxis
+00016ad0: 5665 635b 315d 0a20 2020 2020 2020 205d  Vec[1].        ]
+00016ae0: 2c20 5b22 4e41 4d45 3a41 7474 7269 6275  , ["NAME:Attribu
+00016af0: 7465 7322 2c20 224e 616d 653a 3d22 2c20  tes", "Name:=", 
+00016b00: 6373 5f6e 616d 655d 290a 0a20 2020 2064  cs_name])..    d
+00016b10: 6566 2073 7562 7472 6163 7428 7365 6c66  ef subtract(self
+00016b20: 2c20 626c 616e 6b5f 6e61 6d65 2c20 746f  , blank_name, to
+00016b30: 6f6c 5f6e 616d 6573 2c20 6b65 6570 5f6f  ol_names, keep_o
+00016b40: 7269 6769 6e61 6c73 3d46 616c 7365 293a  riginals=False):
+00016b50: 0a20 2020 2020 2020 2073 656c 6563 7469  .        selecti
+00016b60: 6f6e 5f61 7272 6179 203d 205b 0a20 2020  on_array = [.   
+00016b70: 2020 2020 2020 2020 2022 4e41 4d45 3a53           "NAME:S
+00016b80: 656c 6563 7469 6f6e 7322 2c20 2242 6c61  elections", "Bla
+00016b90: 6e6b 2050 6172 7473 3a3d 222c 2062 6c61  nk Parts:=", bla
+00016ba0: 6e6b 5f6e 616d 652c 2022 546f 6f6c 2050  nk_name, "Tool P
+00016bb0: 6172 7473 3a3d 222c 0a20 2020 2020 2020  arts:=",.       
+00016bc0: 2020 2020 2022 2c22 2e6a 6f69 6e28 746f       ",".join(to
+00016bd0: 6f6c 5f6e 616d 6573 290a 2020 2020 2020  ol_names).      
+00016be0: 2020 5d0a 2020 2020 2020 2020 7365 6c66    ].        self
+00016bf0: 2e5f 6d6f 6465 6c65 722e 5375 6274 7261  ._modeler.Subtra
+00016c00: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
+00016c10: 7365 6c65 6374 696f 6e5f 6172 7261 792c  selection_array,
+00016c20: 0a20 2020 2020 2020 2020 2020 205b 224e  .            ["N
+00016c30: 414d 453a 556e 6974 6550 6172 616d 6574  AME:UniteParamet
+00016c40: 6572 7322 2c20 224b 6565 704f 7269 6769  ers", "KeepOrigi
+00016c50: 6e61 6c73 3a3d 222c 206b 6565 705f 6f72  nals:=", keep_or
+00016c60: 6967 696e 616c 735d 290a 2020 2020 2020  iginals]).      
+00016c70: 2020 7265 7475 726e 2062 6c61 6e6b 5f6e    return blank_n
+00016c80: 616d 650a 0a20 2020 2064 6566 205f 6669  ame..    def _fi
+00016c90: 6c6c 6574 2873 656c 662c 2072 6164 6975  llet(self, radiu
+00016ca0: 732c 2076 6572 7465 785f 696e 6465 782c  s, vertex_index,
+00016cb0: 206f 626a 293a 0a20 2020 2020 2020 2076   obj):.        v
+00016cc0: 6572 7469 6365 7320 3d20 7365 6c66 2e5f  ertices = self._
+00016cd0: 6d6f 6465 6c65 722e 4765 7456 6572 7465  modeler.GetVerte
+00016ce0: 7849 4473 4672 6f6d 4f62 6a65 6374 286f  xIDsFromObject(o
+00016cf0: 626a 290a 2020 2020 2020 2020 6966 2069  bj).        if i
+00016d00: 7369 6e73 7461 6e63 6528 7665 7274 6578  sinstance(vertex
+00016d10: 5f69 6e64 6578 2c20 6c69 7374 293a 0a20  _index, list):. 
+00016d20: 2020 2020 2020 2020 2020 2074 6f5f 6669             to_fi
+00016d30: 6c6c 6574 203d 205b 696e 7428 7665 7274  llet = [int(vert
+00016d40: 6963 6573 5b76 5d29 2066 6f72 2076 2069  ices[v]) for v i
+00016d50: 6e20 7665 7274 6578 5f69 6e64 6578 5d0a  n vertex_index].
+00016d60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00016d70: 2020 2020 2020 2020 2020 746f 5f66 696c            to_fil
+00016d80: 6c65 7420 3d20 5b69 6e74 2876 6572 7469  let = [int(verti
+00016d90: 6365 735b 7665 7274 6578 5f69 6e64 6578  ces[vertex_index
+00016da0: 5d29 5d0a 0a0a 2320 2020 2020 2020 2070  ])]...#        p
+00016db0: 7269 6e74 2876 6572 7469 6365 7329 0a23  rint(vertices).#
+00016dc0: 2020 2020 2020 2020 7072 696e 7428 7261          print(ra
+00016dd0: 6469 7573 290a 2020 2020 2020 2020 7365  dius).        se
+00016de0: 6c66 2e5f 6d6f 6465 6c65 722e 4669 6c6c  lf._modeler.Fill
+00016df0: 6574 285b 224e 414d 453a 5365 6c65 6374  et(["NAME:Select
+00016e00: 696f 6e73 222c 2022 5365 6c65 6374 696f  ions", "Selectio
+00016e10: 6e73 3a3d 222c 206f 626a 5d2c 205b 0a20  ns:=", obj], [. 
+00016e20: 2020 2020 2020 2020 2020 2022 4e41 4d45             "NAME
+00016e30: 3a50 6172 616d 6574 6572 7322 2c0a 2020  :Parameters",.  
+00016e40: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+00016e50: 2020 2020 2020 2020 2020 2020 224e 414d              "NAM
+00016e60: 453a 4669 6c6c 6574 5061 7261 6d65 7465  E:FilletParamete
+00016e70: 7273 222c 2022 4564 6765 733a 3d22 2c20  rs", "Edges:=", 
+00016e80: 5b5d 2c20 2256 6572 7469 6365 733a 3d22  [], "Vertices:="
+00016e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016ea0: 2020 746f 5f66 696c 6c65 742c 2022 5261    to_fillet, "Ra
+00016eb0: 6469 7573 3a3d 222c 2072 6164 6975 732c  dius:=", radius,
+00016ec0: 2022 5365 7462 6163 6b3a 3d22 2c20 2230   "Setback:=", "0
+00016ed0: 6d6d 220a 2020 2020 2020 2020 2020 2020  mm".            
+00016ee0: 5d0a 2020 2020 2020 2020 5d29 0a0a 2020  ].        ])..  
+00016ef0: 2020 6465 6620 5f66 696c 6c65 745f 6564    def _fillet_ed
+00016f00: 6765 7328 7365 6c66 2c20 7261 6469 7573  ges(self, radius
+00016f10: 2c20 6564 6765 5f69 6e64 6578 2c20 6f62  , edge_index, ob
+00016f20: 6a29 3a0a 2020 2020 2020 2020 6564 6765  j):.        edge
+00016f30: 7320 3d20 7365 6c66 2e5f 6d6f 6465 6c65  s = self._modele
+00016f40: 722e 4765 7445 6467 6549 4473 4672 6f6d  r.GetEdgeIDsFrom
+00016f50: 4f62 6a65 6374 286f 626a 290a 2020 2020  Object(obj).    
+00016f60: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00016f70: 6528 6564 6765 5f69 6e64 6578 2c20 6c69  e(edge_index, li
+00016f80: 7374 293a 0a20 2020 2020 2020 2020 2020  st):.           
+00016f90: 2074 6f5f 6669 6c6c 6574 203d 205b 696e   to_fillet = [in
+00016fa0: 7428 6564 6765 735b 655d 2920 666f 7220  t(edges[e]) for 
+00016fb0: 6520 696e 2065 6467 655f 696e 6465 785d  e in edge_index]
+00016fc0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00016fd0: 2020 2020 2020 2020 2020 2074 6f5f 6669             to_fi
+00016fe0: 6c6c 6574 203d 205b 696e 7428 6564 6765  llet = [int(edge
+00016ff0: 735b 6564 6765 5f69 6e64 6578 5d29 5d0a  s[edge_index])].
+00017000: 0a20 2020 2020 2020 2073 656c 662e 5f6d  .        self._m
+00017010: 6f64 656c 6572 2e46 696c 6c65 7428 5b22  odeler.Fillet(["
+00017020: 4e41 4d45 3a53 656c 6563 7469 6f6e 7322  NAME:Selections"
+00017030: 2c20 2253 656c 6563 7469 6f6e 733a 3d22  , "Selections:="
+00017040: 2c20 6f62 6a5d 2c20 5b0a 2020 2020 2020  , obj], [.      
+00017050: 2020 2020 2020 224e 414d 453a 5061 7261        "NAME:Para
+00017060: 6d65 7465 7273 222c 0a20 2020 2020 2020  meters",.       
+00017070: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00017080: 2020 2020 2020 2022 4e41 4d45 3a46 696c         "NAME:Fil
+00017090: 6c65 7450 6172 616d 6574 6572 7322 2c20  letParameters", 
+000170a0: 2245 6467 6573 3a3d 222c 2074 6f5f 6669  "Edges:=", to_fi
+000170b0: 6c6c 6574 2c20 2256 6572 7469 6365 733a  llet, "Vertices:
+000170c0: 3d22 2c0a 2020 2020 2020 2020 2020 2020  =",.            
+000170d0: 2020 2020 5b5d 2c20 2252 6164 6975 733a      [], "Radius:
+000170e0: 3d22 2c20 7261 6469 7573 2c20 2253 6574  =", radius, "Set
+000170f0: 6261 636b 3a3d 222c 2022 306d 6d22 0a20  back:=", "0mm". 
+00017100: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00017110: 2020 2020 205d 290a 0a20 2020 2064 6566       ])..    def
+00017120: 205f 6669 6c6c 6574 7328 7365 6c66 2c20   _fillets(self, 
+00017130: 7261 6469 7573 2c20 7665 7274 6963 6573  radius, vertices
+00017140: 2c20 6f62 6a29 3a0a 2020 2020 2020 2020  , obj):.        
+00017150: 7365 6c66 2e5f 6d6f 6465 6c65 722e 4669  self._modeler.Fi
+00017160: 6c6c 6574 285b 224e 414d 453a 5365 6c65  llet(["NAME:Sele
+00017170: 6374 696f 6e73 222c 2022 5365 6c65 6374  ctions", "Select
+00017180: 696f 6e73 3a3d 222c 206f 626a 5d2c 205b  ions:=", obj], [
+00017190: 0a20 2020 2020 2020 2020 2020 2022 4e41  .            "NA
+000171a0: 4d45 3a50 6172 616d 6574 6572 7322 2c0a  ME:Parameters",.
+000171b0: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+000171c0: 2020 2020 2020 2020 2020 2020 2020 224e                "N
+000171d0: 414d 453a 4669 6c6c 6574 5061 7261 6d65  AME:FilletParame
+000171e0: 7465 7273 222c 2022 4564 6765 733a 3d22  ters", "Edges:="
+000171f0: 2c20 5b5d 2c20 2256 6572 7469 6365 733a  , [], "Vertices:
+00017200: 3d22 2c20 7665 7274 6963 6573 2c0a 2020  =", vertices,.  
+00017210: 2020 2020 2020 2020 2020 2020 2020 2252                "R
+00017220: 6164 6975 733a 3d22 2c20 7261 6469 7573  adius:=", radius
+00017230: 2c20 2253 6574 6261 636b 3a3d 222c 2022  , "Setback:=", "
+00017240: 306d 6d22 0a20 2020 2020 2020 2020 2020  0mm".           
+00017250: 205d 0a20 2020 2020 2020 205d 290a 0a20   ].        ]).. 
+00017260: 2020 2064 6566 205f 7377 6565 705f 616c     def _sweep_al
+00017270: 6f6e 675f 7061 7468 2873 656c 662c 2074  ong_path(self, t
+00017280: 6f5f 7377 6565 702c 2070 6174 685f 6f62  o_sweep, path_ob
+00017290: 6a29 3a0a 2020 2020 2020 2020 2222 220a  j):.        """.
+000172a0: 2020 2020 2020 2020 4164 6473 2074 6869          Adds thi
+000172b0: 636b 6e65 7373 2074 6f20 7061 7468 5f6f  ckness to path_o
+000172c0: 626a 2062 7920 6578 7465 6e64 696e 6720  bj by extending 
+000172d0: 746f 2061 206e 6577 2064 696d 656e 7369  to a new dimensi
+000172e0: 6f6e 2e0a 2020 2020 2020 2020 746f 5f73  on..        to_s
+000172f0: 7765 6570 2061 6374 7320 6173 2061 2070  weep acts as a p
+00017300: 7574 7479 206b 6e69 6665 2074 6861 7420  utty knife that 
+00017310: 6465 7465 726d 696e 6573 2074 6865 2074  determines the t
+00017320: 6869 636b 6e65 7373 2e0a 0a20 2020 2020  hickness...     
+00017330: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00017340: 2020 2020 2074 6f5f 7377 6565 7020 2870       to_sweep (p
+00017350: 6f6c 796c 696e 6529 3a20 536d 616c 6c20  olyline): Small 
+00017360: 706f 6c79 6c69 6e65 2072 756e 6e69 6e67  polyline running
+00017370: 2070 6572 7065 6e64 6963 756c 6172 2074   perpendicular t
+00017380: 6f20 7061 7468 5f6f 626a 0a20 2020 2020  o path_obj.     
+00017390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000173a0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+000173b0: 686f 7365 206c 656e 6774 6820 6973 2074  hose length is t
+000173c0: 6865 2064 6573 6972 6564 2072 6573 756c  he desired resul
+000173d0: 7469 6e67 2074 6869 636b 6e65 7373 0a20  ting thickness. 
+000173e0: 2020 2020 2020 2020 2020 2070 6174 685f             path_
+000173f0: 6f62 6a20 2870 6f6c 796c 696e 6529 3a20  obj (polyline): 
+00017400: 4f72 6967 696e 616c 2070 6f6c 796c 696e  Original polylin
+00017410: 653b 2077 616e 7420 746f 2062 726f 6164  e; want to broad
+00017420: 656e 2074 6869 730a 2020 2020 2020 2020  en this.        
+00017430: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+00017440: 2e72 656e 616d 655f 6f62 6a28 7061 7468  .rename_obj(path
+00017450: 5f6f 626a 2c20 7374 7228 7061 7468 5f6f  _obj, str(path_o
+00017460: 626a 2920 2b20 275f 7061 7468 2729 0a20  bj) + '_path'). 
+00017470: 2020 2020 2020 206e 6577 5f6e 616d 6520         new_name 
+00017480: 3d20 7365 6c66 2e72 656e 616d 655f 6f62  = self.rename_ob
+00017490: 6a28 746f 5f73 7765 6570 2c20 7061 7468  j(to_sweep, path
+000174a0: 5f6f 626a 290a 2020 2020 2020 2020 6e61  _obj).        na
+000174b0: 6d65 7320 3d20 5b70 6174 685f 6f62 6a2c  mes = [path_obj,
+000174c0: 2073 7472 2870 6174 685f 6f62 6a29 202b   str(path_obj) +
+000174d0: 2027 5f70 6174 6827 5d0a 2020 2020 2020   '_path'].      
+000174e0: 2020 7365 6c66 2e5f 6d6f 6465 6c65 722e    self._modeler.
+000174f0: 5377 6565 7041 6c6f 6e67 5061 7468 2873  SweepAlongPath(s
+00017500: 656c 662e 5f73 656c 6563 7469 6f6e 735f  elf._selections_
+00017510: 6172 7261 7928 2a6e 616d 6573 292c 205b  array(*names), [
+00017520: 0a20 2020 2020 2020 2020 2020 2022 4e41  .            "NA
+00017530: 4d45 3a50 6174 6853 7765 6570 5061 7261  ME:PathSweepPara
+00017540: 6d65 7465 7273 222c 2022 4472 6166 7441  meters", "DraftA
+00017550: 6e67 6c65 3a3d 222c 2022 3064 6567 222c  ngle:=", "0deg",
+00017560: 2022 4472 6166 7454 7970 653a 3d22 2c0a   "DraftType:=",.
+00017570: 2020 2020 2020 2020 2020 2020 2252 6f75              "Rou
+00017580: 6e64 222c 2022 4368 6563 6b46 6163 6546  nd", "CheckFaceF
+00017590: 6163 6549 6e74 6572 7365 6374 696f 6e3a  aceIntersection:
+000175a0: 3d22 2c20 4661 6c73 652c 2022 5477 6973  =", False, "Twis
+000175b0: 7441 6e67 6c65 3a3d 222c 0a20 2020 2020  tAngle:=",.     
+000175c0: 2020 2020 2020 2022 3064 6567 220a 2020         "0deg".  
+000175d0: 2020 2020 2020 5d29 0a20 2020 2020 2020        ]).       
+000175e0: 2072 6574 7572 6e20 506f 6c79 6c69 6e65   return Polyline
+000175f0: 286e 6577 5f6e 616d 652c 2073 656c 6629  (new_name, self)
+00017600: 0a0a 2020 2020 6465 6620 7377 6565 705f  ..    def sweep_
+00017610: 616c 6f6e 675f 7665 6374 6f72 2873 656c  along_vector(sel
+00017620: 662c 206e 616d 6573 2c20 7665 6374 6f72  f, names, vector
+00017630: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00017640: 5f6d 6f64 656c 6572 2e53 7765 6570 416c  _modeler.SweepAl
+00017650: 6f6e 6756 6563 746f 7228 7365 6c66 2e5f  ongVector(self._
+00017660: 7365 6c65 6374 696f 6e73 5f61 7272 6179  selections_array
+00017670: 282a 6e61 6d65 7329 2c20 5b0a 2020 2020  (*names), [.    
+00017680: 2020 2020 2020 2020 224e 414d 453a 5665          "NAME:Ve
+00017690: 6374 6f72 5377 6565 7050 6172 616d 6574  ctorSweepParamet
+000176a0: 6572 7322 2c20 2244 7261 6674 416e 676c  ers", "DraftAngl
+000176b0: 653a 3d22 2c20 2230 6465 6722 2c0a 2020  e:=", "0deg",.  
+000176c0: 2020 2020 2020 2020 2020 2244 7261 6674            "Draft
+000176d0: 5479 7065 3a3d 222c 2022 526f 756e 6422  Type:=", "Round"
+000176e0: 2c20 2243 6865 636b 4661 6365 4661 6365  , "CheckFaceFace
+000176f0: 496e 7465 7273 6563 7469 6f6e 3a3d 222c  Intersection:=",
+00017700: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00017710: 2020 2020 2253 7765 6570 5665 6374 6f72      "SweepVector
+00017720: 583a 3d22 2c20 7665 6374 6f72 5b30 5d2c  X:=", vector[0],
+00017730: 2022 5377 6565 7056 6563 746f 7259 3a3d   "SweepVectorY:=
+00017740: 222c 2076 6563 746f 725b 315d 2c0a 2020  ", vector[1],.  
+00017750: 2020 2020 2020 2020 2020 2253 7765 6570            "Sweep
+00017760: 5665 6374 6f72 5a3a 3d22 2c20 7665 6374  VectorZ:=", vect
+00017770: 6f72 5b32 5d0a 2020 2020 2020 2020 5d29  or[2].        ])
+00017780: 0a0a 2020 2020 6465 6620 7265 6e61 6d65  ..    def rename
+00017790: 5f6f 626a 2873 656c 662c 206f 626a 2c20  _obj(self, obj, 
+000177a0: 6e61 6d65 293a 0a20 2020 2020 2020 2073  name):.        s
+000177b0: 656c 662e 5f6d 6f64 656c 6572 2e43 6861  elf._modeler.Cha
+000177c0: 6e67 6550 726f 7065 7274 7928 5b0a 2020  ngeProperty([.  
+000177d0: 2020 2020 2020 2020 2020 224e 414d 453a            "NAME:
+000177e0: 416c 6c54 6162 7322 2c0a 2020 2020 2020  AllTabs",.      
+000177f0: 2020 2020 2020 5b0a 2020 2020 2020 2020        [.        
+00017800: 2020 2020 2020 2020 224e 414d 453a 4765          "NAME:Ge
+00017810: 6f6d 6574 7279 3344 4174 7472 6962 7574  ometry3DAttribut
+00017820: 6554 6162 222c 205b 224e 414d 453a 5072  eTab", ["NAME:Pr
+00017830: 6f70 5365 7276 6572 7322 2c0a 2020 2020  opServers",.    
 00017840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017850: 2020 2020 2020 2020 2070 726f 705f 7365           prop_se
-00017860: 7276 6572 3d6c 616d 6264 6120 7365 6c66  rver=lambda self
-00017870: 3a20 7365 6c66 290a 2020 2020 636f 6f72  : self).    coor
-00017880: 6469 6e61 7465 5f73 7973 7465 6d20 3d20  dinate_system = 
-00017890: 6d61 6b65 5f73 7472 5f70 726f 7028 2243  make_str_prop("C
-000178a0: 6f6f 7264 696e 6174 6520 5379 7374 656d  oordinate System
-000178b0: 2229 0a0a 2020 2020 6465 6620 5f5f 6e65  ")..    def __ne
-000178c0: 775f 5f28 7365 6c66 2c20 7661 6c2c 202a  w__(self, val, *
-000178d0: 6172 6773 2c20 2a2a 6b77 6172 6773 293a  args, **kwargs):
-000178e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000178f0: 7374 722e 5f5f 6e65 775f 5f28 7365 6c66  str.__new__(self
-00017900: 2c20 7661 6c29 0a0a 2020 2020 6465 6620  , val)..    def 
-00017910: 5f5f 696e 6974 5f5f 2873 656c 662c 2076  __init__(self, v
-00017920: 616c 2c20 6d6f 6465 6c65 7229 3a0a 2020  al, modeler):.  
-00017930: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00017940: 2020 3a74 7970 6520 7661 6c3a 2073 7472    :type val: str
-00017950: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
-00017960: 6f64 656c 6572 3a20 4866 7373 4d6f 6465  odeler: HfssMode
-00017970: 6c65 720a 2020 2020 2020 2020 2222 220a  ler.        """.
-00017980: 2020 2020 2020 2020 7375 7065 7228 4d6f          super(Mo
-00017990: 6465 6c45 6e74 6974 792c 0a20 2020 2020  delEntity,.     
-000179a0: 2020 2020 2020 2020 2073 656c 6629 2e5f           self)._
-000179b0: 5f69 6e69 745f 5f28 2920 2023 2076 616c  _init__()  # val
-000179c0: 2920 2343 6f6d 6d65 6e74 206f 7574 206b  ) #Comment out k
-000179d0: 6579 776f 7264 2074 6f20 6d61 7463 6820  eyword to match 
-000179e0: 6172 6775 6d65 6e74 730a 2020 2020 2020  arguments.      
-000179f0: 2020 7365 6c66 2e6d 6f64 656c 6572 203d    self.modeler =
-00017a00: 206d 6f64 656c 6572 0a20 2020 2020 2020   modeler.       
-00017a10: 2073 656c 662e 7072 6f70 5f73 6572 7665   self.prop_serve
-00017a20: 7220 3d20 7365 6c66 202b 2022 3a22 202b  r = self + ":" +
-00017a30: 2073 656c 662e 6d6f 6465 6c5f 636f 6d6d   self.model_comm
-00017a40: 616e 6420 2b20 223a 3122 0a0a 0a63 6c61  and + ":1"...cla
-00017a50: 7373 2042 6f78 284d 6f64 656c 456e 7469  ss Box(ModelEnti
-00017a60: 7479 293a 0a20 2020 206d 6f64 656c 5f63  ty):.    model_c
-00017a70: 6f6d 6d61 6e64 203d 2022 4372 6561 7465  ommand = "Create
-00017a80: 426f 7822 0a20 2020 2070 6f73 6974 696f  Box".    positio
-00017a90: 6e20 3d20 6d61 6b65 5f66 6c6f 6174 5f70  n = make_float_p
-00017aa0: 726f 7028 2250 6f73 6974 696f 6e22 290a  rop("Position").
-00017ab0: 2020 2020 785f 7369 7a65 203d 206d 616b      x_size = mak
-00017ac0: 655f 666c 6f61 745f 7072 6f70 2822 5853  e_float_prop("XS
-00017ad0: 697a 6522 290a 2020 2020 795f 7369 7a65  ize").    y_size
-00017ae0: 203d 206d 616b 655f 666c 6f61 745f 7072   = make_float_pr
-00017af0: 6f70 2822 5953 697a 6522 290a 2020 2020  op("YSize").    
-00017b00: 7a5f 7369 7a65 203d 206d 616b 655f 666c  z_size = make_fl
-00017b10: 6f61 745f 7072 6f70 2822 5a53 697a 6522  oat_prop("ZSize"
-00017b20: 290a 0a20 2020 2064 6566 205f 5f69 6e69  )..    def __ini
-00017b30: 745f 5f28 7365 6c66 2c20 6e61 6d65 2c20  t__(self, name, 
-00017b40: 6d6f 6465 6c65 722c 2063 6f72 6e65 722c  modeler, corner,
-00017b50: 2073 697a 6529 3a0a 2020 2020 2020 2020   size):.        
-00017b60: 2222 220a 2020 2020 2020 2020 3a74 7970  """.        :typ
-00017b70: 6520 6e61 6d65 3a20 7374 720a 2020 2020  e name: str.    
-00017b80: 2020 2020 3a74 7970 6520 6d6f 6465 6c65      :type modele
-00017b90: 723a 2048 6673 734d 6f64 656c 6572 0a20  r: HfssModeler. 
-00017ba0: 2020 2020 2020 203a 7479 7065 2063 6f72         :type cor
-00017bb0: 6e65 723a 205b 2856 6172 6961 626c 6553  ner: [(VariableS
-00017bc0: 7472 696e 672c 2056 6172 6961 626c 6553  tring, VariableS
-00017bd0: 7472 696e 672c 2056 6172 6961 626c 6553  tring, VariableS
-00017be0: 7472 696e 6729 5d0a 2020 2020 2020 2020  tring)].        
-00017bf0: 3a70 6172 616d 2073 697a 653a 205b 2856  :param size: [(V
-00017c00: 6172 6961 626c 6553 7472 696e 672c 2056  ariableString, V
-00017c10: 6172 6961 626c 6553 7472 696e 672c 2056  ariableString, V
-00017c20: 6172 6961 626c 6553 7472 696e 6729 5d0a  ariableString)].
-00017c30: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00017c40: 2020 2020 7375 7065 7228 426f 782c 2073      super(Box, s
-00017c50: 656c 6629 2e5f 5f69 6e69 745f 5f28 6e61  elf).__init__(na
-00017c60: 6d65 2c20 6d6f 6465 6c65 7229 0a20 2020  me, modeler).   
-00017c70: 2020 2020 2073 656c 662e 6d6f 6465 6c65       self.modele
-00017c80: 7220 3d20 6d6f 6465 6c65 720a 2020 2020  r = modeler.    
-00017c90: 2020 2020 7365 6c66 2e70 726f 705f 686f      self.prop_ho
-00017ca0: 6c64 6572 203d 206d 6f64 656c 6572 2e5f  lder = modeler._
-00017cb0: 6d6f 6465 6c65 720a 2020 2020 2020 2020  modeler.        
-00017cc0: 7365 6c66 2e63 6f72 6e65 7220 3d20 636f  self.corner = co
-00017cd0: 726e 6572 0a20 2020 2020 2020 2073 656c  rner.        sel
-00017ce0: 662e 7369 7a65 203d 2073 697a 650a 2020  f.size = size.  
-00017cf0: 2020 2020 2020 7365 6c66 2e63 656e 7465        self.cente
-00017d00: 7220 3d20 5b63 202b 2073 202f 2032 2066  r = [c + s / 2 f
-00017d10: 6f72 2063 2c20 7320 696e 207a 6970 2863  or c, s in zip(c
-00017d20: 6f72 6e65 722c 2073 697a 6529 5d0a 2020  orner, size)].  
-00017d30: 2020 2020 2020 6661 6365 7320 3d20 6d6f        faces = mo
-00017d40: 6465 6c65 722e 6765 745f 6661 6365 5f69  deler.get_face_i
-00017d50: 6473 2873 656c 6629 0a20 2020 2020 2020  ds(self).       
-00017d60: 2073 656c 662e 7a5f 6261 636b 5f66 6163   self.z_back_fac
-00017d70: 652c 2073 656c 662e 7a5f 6672 6f6e 745f  e, self.z_front_
-00017d80: 6661 6365 203d 2066 6163 6573 5b30 5d2c  face = faces[0],
-00017d90: 2066 6163 6573 5b31 5d0a 2020 2020 2020   faces[1].      
-00017da0: 2020 7365 6c66 2e79 5f62 6163 6b5f 6661    self.y_back_fa
-00017db0: 6365 2c20 7365 6c66 2e79 5f66 726f 6e74  ce, self.y_front
-00017dc0: 5f66 6163 6520 3d20 6661 6365 735b 325d  _face = faces[2]
-00017dd0: 2c20 6661 6365 735b 345d 0a20 2020 2020  , faces[4].     
-00017de0: 2020 2073 656c 662e 785f 6261 636b 5f66     self.x_back_f
-00017df0: 6163 652c 2073 656c 662e 785f 6672 6f6e  ace, self.x_fron
-00017e00: 745f 6661 6365 203d 2066 6163 6573 5b33  t_face = faces[3
-00017e10: 5d2c 2066 6163 6573 5b35 5d0a 0a0a 636c  ], faces[5]...cl
-00017e20: 6173 7320 5265 6374 284d 6f64 656c 456e  ass Rect(ModelEn
-00017e30: 7469 7479 293a 0a20 2020 206d 6f64 656c  tity):.    model
-00017e40: 5f63 6f6d 6d61 6e64 203d 2022 4372 6561  _command = "Crea
-00017e50: 7465 5265 6374 616e 676c 6522 0a0a 2020  teRectangle"..  
-00017e60: 2020 2320 544f 444f 3a20 4164 6420 6120    # TODO: Add a 
-00017e70: 726f 7461 7465 6420 7265 6374 616e 676c  rotated rectangl
-00017e80: 6520 6f62 6a65 6374 2e0a 2020 2020 2320  e object..    # 
-00017e90: 5769 6c6c 206e 6565 6420 746f 2066 6972  Will need to fir
-00017ea0: 7374 2063 7265 6174 6520 7265 6374 2c20  st create rect, 
-00017eb0: 7468 656e 2061 7070 6c79 2072 6f74 6174  then apply rotat
-00017ec0: 6520 6f70 6572 6174 696f 6e2e 0a0a 2020  e operation...  
-00017ed0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00017ee0: 656c 662c 206e 616d 652c 206d 6f64 656c  elf, name, model
-00017ef0: 6572 2c20 636f 726e 6572 2c20 7369 7a65  er, corner, size
-00017f00: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
-00017f10: 2852 6563 742c 2073 656c 6629 2e5f 5f69  (Rect, self).__i
-00017f20: 6e69 745f 5f28 6e61 6d65 2c20 6d6f 6465  nit__(name, mode
-00017f30: 6c65 7229 0a20 2020 2020 2020 2073 656c  ler).        sel
-00017f40: 662e 7072 6f70 5f68 6f6c 6465 7220 3d20  f.prop_holder = 
-00017f50: 6d6f 6465 6c65 722e 5f6d 6f64 656c 6572  modeler._modeler
-00017f60: 0a20 2020 2020 2020 2073 656c 662e 636f  .        self.co
-00017f70: 726e 6572 203d 2063 6f72 6e65 720a 2020  rner = corner.  
-00017f80: 2020 2020 2020 7365 6c66 2e73 697a 6520        self.size 
-00017f90: 3d20 7369 7a65 0a20 2020 2020 2020 2073  = size.        s
-00017fa0: 656c 662e 6365 6e74 6572 203d 205b 6320  elf.center = [c 
-00017fb0: 2b20 7320 2f20 3220 6966 2073 2065 6c73  + s / 2 if s els
-00017fc0: 6520 6320 666f 7220 632c 2073 2069 6e20  e c for c, s in 
-00017fd0: 7a69 7028 636f 726e 6572 2c20 7369 7a65  zip(corner, size
-00017fe0: 295d 0a0a 2020 2020 6465 6620 6d61 6b65  )]..    def make
-00017ff0: 5f63 656e 7465 725f 6c69 6e65 2873 656c  _center_line(sel
-00018000: 662c 2061 7869 7329 3a0a 2020 2020 2020  f, axis):.      
-00018010: 2020 2727 270a 2020 2020 2020 2020 5265    '''.        Re
-00018020: 7475 726e 7320 6073 7461 7274 6020 616e  turns `start` an
-00018030: 6420 6065 6e64 6020 6c69 7374 206f 6620  d `end` list of 
-00018040: 3320 636f 6f72 6469 6e61 7465 730a 2020  3 coordinates.  
-00018050: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00018060: 2020 6178 6973 5f69 6478 203d 205b 2278    axis_idx = ["x
-00018070: 222c 2022 7922 2c20 227a 225d 2e69 6e64  ", "y", "z"].ind
-00018080: 6578 2861 7869 732e 6c6f 7765 7228 2929  ex(axis.lower())
-00018090: 0a20 2020 2020 2020 2073 7461 7274 203d  .        start =
-000180a0: 205b 6320 666f 7220 6320 696e 2073 656c   [c for c in sel
-000180b0: 662e 6365 6e74 6572 5d0a 2020 2020 2020  f.center].      
-000180c0: 2020 7374 6172 745b 6178 6973 5f69 6478    start[axis_idx
-000180d0: 5d20 2d3d 2073 656c 662e 7369 7a65 5b61  ] -= self.size[a
-000180e0: 7869 735f 6964 785d 202f 2032 0a20 2020  xis_idx] / 2.   
-000180f0: 2020 2020 2073 7461 7274 203d 205b 7365       start = [se
-00018100: 6c66 2e6d 6f64 656c 6572 2e65 7661 6c5f  lf.modeler.eval_
-00018110: 6578 7072 2873 2920 666f 7220 7320 696e  expr(s) for s in
-00018120: 2073 7461 7274 5d0a 2020 2020 2020 2020   start].        
-00018130: 656e 6420 3d20 5b63 2066 6f72 2063 2069  end = [c for c i
-00018140: 6e20 7365 6c66 2e63 656e 7465 725d 0a20  n self.center]. 
-00018150: 2020 2020 2020 2065 6e64 5b61 7869 735f         end[axis_
-00018160: 6964 785d 202b 3d20 7365 6c66 2e73 697a  idx] += self.siz
-00018170: 655b 6178 6973 5f69 6478 5d20 2f20 320a  e[axis_idx] / 2.
-00018180: 2020 2020 2020 2020 656e 6420 3d20 5b73          end = [s
-00018190: 656c 662e 6d6f 6465 6c65 722e 6576 616c  elf.modeler.eval
-000181a0: 5f65 7870 7228 7329 2066 6f72 2073 2069  _expr(s) for s i
-000181b0: 6e20 656e 645d 0a20 2020 2020 2020 2072  n end].        r
-000181c0: 6574 7572 6e20 7374 6172 742c 2065 6e64  eturn start, end
-000181d0: 0a0a 2020 2020 6465 6620 6d61 6b65 5f72  ..    def make_r
-000181e0: 6c63 5f62 6f75 6e64 6172 7928 7365 6c66  lc_boundary(self
-000181f0: 2c20 6178 6973 2c20 723d 302c 206c 3d30  , axis, r=0, l=0
-00018200: 2c20 633d 302c 206e 616d 653d 224c 756d  , c=0, name="Lum
-00018210: 7052 4c43 2229 3a0a 2020 2020 2020 2020  pRLC"):.        
-00018220: 7374 6172 742c 2065 6e64 203d 2073 656c  start, end = sel
-00018230: 662e 6d61 6b65 5f63 656e 7465 725f 6c69  f.make_center_li
-00018240: 6e65 2861 7869 7329 0a20 2020 2020 2020  ne(axis).       
-00018250: 2073 656c 662e 6d6f 6465 6c65 722e 5f6d   self.modeler._m
-00018260: 616b 655f 6c75 6d70 6564 5f72 6c63 2872  ake_lumped_rlc(r
-00018270: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00018280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018290: 2020 2020 2020 2020 6c2c 0a20 2020 2020          l,.     
-000182a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182c0: 2063 2c0a 2020 2020 2020 2020 2020 2020   c,.            
-000182d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182e0: 2020 2020 2020 2020 2020 7374 6172 742c            start,
-000182f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018310: 2020 2020 2020 2065 6e64 2c20 5b22 4f62         end, ["Ob
-00018320: 6a65 6374 733a 3d22 2c20 5b73 656c 665d  jects:=", [self]
-00018330: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018350: 2020 2020 2020 2020 206e 616d 653d 6e61           name=na
-00018360: 6d65 290a 0a20 2020 2064 6566 206d 616b  me)..    def mak
-00018370: 655f 6c75 6d70 6564 5f70 6f72 7428 7365  e_lumped_port(se
-00018380: 6c66 2c20 6178 6973 2c20 7a30 3d22 3530  lf, axis, z0="50
-00018390: 6f68 6d22 2c20 6e61 6d65 3d22 4c75 6d70  ohm", name="Lump
-000183a0: 506f 7274 2229 3a0a 2020 2020 2020 2020  Port"):.        
-000183b0: 7374 6172 742c 2065 6e64 203d 2073 656c  start, end = sel
-000183c0: 662e 6d61 6b65 5f63 656e 7465 725f 6c69  f.make_center_li
-000183d0: 6e65 2861 7869 7329 0a20 2020 2020 2020  ne(axis).       
-000183e0: 2073 656c 662e 6d6f 6465 6c65 722e 5f6d   self.modeler._m
-000183f0: 616b 655f 6c75 6d70 6564 5f70 6f72 7428  ake_lumped_port(
-00018400: 7374 6172 742c 0a20 2020 2020 2020 2020  start,.         
-00018410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018420: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00018430: 642c 205b 224f 626a 6563 7473 3a3d 222c  d, ["Objects:=",
-00018440: 205b 7365 6c66 5d5d 2c0a 2020 2020 2020   [self]],.      
-00018450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018470: 207a 303d 7a30 2c0a 2020 2020 2020 2020   z0=z0,.        
-00018480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018490: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000184a0: 616d 653d 6e61 6d65 290a 0a0a 636c 6173  ame=name)...clas
-000184b0: 7320 506f 6c79 6c69 6e65 284d 6f64 656c  s Polyline(Model
-000184c0: 456e 7469 7479 293a 0a20 2020 2027 2727  Entity):.    '''
-000184d0: 0a20 2020 2041 7373 756d 6520 636c 6f73  .    Assume clos
-000184e0: 6564 2070 6f6c 796c 696e 652c 2077 6869  ed polyline, whi
-000184f0: 6368 2063 7265 6174 6573 2061 2070 6f6c  ch creates a pol
-00018500: 7967 6f6e 2e0a 2020 2020 2727 270a 0a20  ygon..    '''.. 
-00018510: 2020 206d 6f64 656c 5f63 6f6d 6d61 6e64     model_command
-00018520: 203d 2022 4372 6561 7465 506f 6c79 6c69   = "CreatePolyli
-00018530: 6e65 220a 0a20 2020 2064 6566 205f 5f69  ne"..    def __i
-00018540: 6e69 745f 5f28 7365 6c66 2c20 6e61 6d65  nit__(self, name
-00018550: 2c20 6d6f 6465 6c65 722c 2070 6f69 6e74  , modeler, point
-00018560: 733d 4e6f 6e65 293a 0a20 2020 2020 2020  s=None):.       
-00018570: 2073 7570 6572 2850 6f6c 796c 696e 652c   super(Polyline,
-00018580: 2073 656c 6629 2e5f 5f69 6e69 745f 5f28   self).__init__(
-00018590: 6e61 6d65 2c20 6d6f 6465 6c65 7229 0a20  name, modeler). 
-000185a0: 2020 2020 2020 2073 656c 662e 7072 6f70         self.prop
-000185b0: 5f68 6f6c 6465 7220 3d20 6d6f 6465 6c65  _holder = modele
-000185c0: 722e 5f6d 6f64 656c 6572 0a20 2020 2020  r._modeler.     
-000185d0: 2020 2069 6620 706f 696e 7473 2069 7320     if points is 
-000185e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000185f0: 2020 2020 2020 7365 6c66 2e70 6f69 6e74        self.point
-00018600: 7320 3d20 706f 696e 7473 0a20 2020 2020  s = points.     
-00018610: 2020 2020 2020 2073 656c 662e 6e5f 706f         self.n_po
-00018620: 696e 7473 203d 206c 656e 2870 6f69 6e74  ints = len(point
-00018630: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
-00018640: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-00018650: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-00018660: 544f 444f 3a20 706f 696e 7473 203d 2063  TODO: points = c
-00018670: 6f6c 6c65 6374 696f 6e20 6f66 2070 6f69  ollection of poi
-00018680: 6e74 730a 0a0a 2320 2020 2020 2020 2061  nts...#        a
-00018690: 7869 7320 3d20 6669 6e64 5f6f 7274 685f  xis = find_orth_
-000186a0: 6178 6973 2829 0a0a 2320 544f 444f 3a20  axis()..# TODO: 
-000186b0: 6669 6e64 2074 6865 2070 6c61 6e65 206f  find the plane o
-000186c0: 6620 7468 6520 706f 6c79 6c69 6e65 2066  f the polyline f
-000186d0: 6f72 206e 6f77 2c20 6173 7375 6d65 205a  or now, assume Z
-000186e0: 0a23 2020 2020 6465 6620 6669 6e64 5f6f  .#    def find_o
-000186f0: 7274 685f 6178 6973 2829 3a0a 2320 2020  rth_axis():.#   
-00018700: 2020 2020 2058 2c20 592c 205a 203d 2028       X, Y, Z = (
-00018710: 5472 7565 2c20 5472 7565 2c20 5472 7565  True, True, True
-00018720: 290a 2320 2020 2020 2020 2066 6f72 2070  ).#        for p
-00018730: 6f69 6e74 2069 6e20 706f 696e 7473 3a0a  oint in points:.
-00018740: 2320 2020 2020 2020 2020 2020 2058 203d  #            X =
-00018750: 0a0a 2020 2020 6465 6620 756e 6974 6528  ..    def unite(
-00018760: 7365 6c66 2c20 6c69 7374 5f6f 7468 6572  self, list_other
-00018770: 293a 0a20 2020 2020 2020 2075 6e69 6f6e  ):.        union
-00018780: 203d 2073 656c 662e 6d6f 6465 6c65 722e   = self.modeler.
-00018790: 756e 6974 6528 7365 6c66 202b 206c 6973  unite(self + lis
-000187a0: 745f 6f74 6865 7229 0a20 2020 2020 2020  t_other).       
-000187b0: 2072 6574 7572 6e20 506f 6c79 6c69 6e65   return Polyline
-000187c0: 2875 6e69 6f6e 2c20 7365 6c66 2e6d 6f64  (union, self.mod
-000187d0: 656c 6572 290a 0a20 2020 2064 6566 206d  eler)..    def m
-000187e0: 616b 655f 6365 6e74 6572 5f6c 696e 6528  ake_center_line(
-000187f0: 7365 6c66 2c20 6178 6973 293a 2020 2320  self, axis):  # 
-00018800: 4578 7065 6374 7320 746f 2061 6374 206f  Expects to act o
-00018810: 6e20 6120 7265 6374 616e 676c 652e 2e2e  n a rectangle...
-00018820: 0a20 2020 2020 2020 2023 2066 6972 7374  .        # first
-00018830: 203a 2066 696e 6420 6365 6e74 6572 2061   : find center a
-00018840: 6e64 2073 697a 650a 2020 2020 2020 2020  nd size.        
-00018850: 6365 6e74 6572 203d 205b 302c 2030 2c20  center = [0, 0, 
-00018860: 305d 0a0a 2020 2020 2020 2020 666f 7220  0]..        for 
-00018870: 706f 696e 7420 696e 2073 656c 662e 706f  point in self.po
-00018880: 696e 7473 3a0a 2020 2020 2020 2020 2020  ints:.          
-00018890: 2020 6365 6e74 6572 203d 205b 0a20 2020    center = [.   
-000188a0: 2020 2020 2020 2020 2020 2020 2063 656e               cen
-000188b0: 7465 725b 305d 202b 2070 6f69 6e74 5b30  ter[0] + point[0
-000188c0: 5d20 2f20 7365 6c66 2e6e 5f70 6f69 6e74  ] / self.n_point
-000188d0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000188e0: 2020 2063 656e 7465 725b 315d 202b 2070     center[1] + p
-000188f0: 6f69 6e74 5b31 5d20 2f20 7365 6c66 2e6e  oint[1] / self.n
-00018900: 5f70 6f69 6e74 732c 0a20 2020 2020 2020  _points,.       
-00018910: 2020 2020 2020 2020 2063 656e 7465 725b           center[
-00018920: 325d 202b 2070 6f69 6e74 5b32 5d20 2f20  2] + point[2] / 
-00018930: 7365 6c66 2e6e 5f70 6f69 6e74 730a 2020  self.n_points.  
-00018940: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
-00018950: 2020 2020 7369 7a65 203d 205b 0a20 2020      size = [.   
-00018960: 2020 2020 2020 2020 2032 202a 2028 6365           2 * (ce
-00018970: 6e74 6572 5b30 5d20 2d20 7365 6c66 2e70  nter[0] - self.p
-00018980: 6f69 6e74 735b 305d 5b30 5d29 2c0a 2020  oints[0][0]),.  
-00018990: 2020 2020 2020 2020 2020 3220 2a20 2863            2 * (c
-000189a0: 656e 7465 725b 315d 202d 2073 656c 662e  enter[1] - self.
-000189b0: 706f 696e 7473 5b30 5d5b 315d 292c 0a20  points[0][1]),. 
-000189c0: 2020 2020 2020 2020 2020 2032 202a 2028             2 * (
-000189d0: 6365 6e74 6572 5b31 5d20 2d20 7365 6c66  center[1] - self
-000189e0: 2e70 6f69 6e74 735b 305d 5b32 5d29 0a20  .points[0][2]). 
-000189f0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00018a00: 2061 7869 735f 6964 7820 3d20 5b22 7822   axis_idx = ["x"
-00018a10: 2c20 2279 222c 2022 7a22 5d2e 696e 6465  , "y", "z"].inde
-00018a20: 7828 6178 6973 2e6c 6f77 6572 2829 290a  x(axis.lower()).
-00018a30: 2020 2020 2020 2020 7374 6172 7420 3d20          start = 
-00018a40: 5b63 2066 6f72 2063 2069 6e20 6365 6e74  [c for c in cent
-00018a50: 6572 5d0a 2020 2020 2020 2020 7374 6172  er].        star
-00018a60: 745b 6178 6973 5f69 6478 5d20 2d3d 2073  t[axis_idx] -= s
-00018a70: 697a 655b 6178 6973 5f69 6478 5d20 2f20  ize[axis_idx] / 
-00018a80: 320a 2020 2020 2020 2020 7374 6172 7420  2.        start 
-00018a90: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00018aa0: 7365 6c66 2e6d 6f64 656c 6572 2e65 7661  self.modeler.eva
-00018ab0: 6c5f 7661 725f 7374 7228 732c 2075 6e69  l_var_str(s, uni
-00018ac0: 743d 4c45 4e47 5448 5f55 4e49 5429 2066  t=LENGTH_UNIT) f
-00018ad0: 6f72 2073 2069 6e20 7374 6172 740a 2020  or s in start.  
-00018ae0: 2020 2020 2020 5d20 2023 2054 4f44 4f0a        ]  # TODO.
-00018af0: 2020 2020 2020 2020 656e 6420 3d20 5b63          end = [c
-00018b00: 2066 6f72 2063 2069 6e20 6365 6e74 6572   for c in center
-00018b10: 5d0a 2020 2020 2020 2020 656e 645b 6178  ].        end[ax
-00018b20: 6973 5f69 6478 5d20 2b3d 2073 697a 655b  is_idx] += size[
-00018b30: 6178 6973 5f69 6478 5d20 2f20 320a 2020  axis_idx] / 2.  
-00018b40: 2020 2020 2020 656e 6420 3d20 5b73 656c        end = [sel
-00018b50: 662e 6d6f 6465 6c65 722e 6576 616c 5f76  f.modeler.eval_v
-00018b60: 6172 5f73 7472 2873 2c20 756e 6974 3d4c  ar_str(s, unit=L
-00018b70: 454e 4754 485f 554e 4954 2920 666f 7220  ENGTH_UNIT) for 
-00018b80: 7320 696e 2065 6e64 5d0a 2020 2020 2020  s in end].      
-00018b90: 2020 7265 7475 726e 2073 7461 7274 2c20    return start, 
-00018ba0: 656e 640a 0a20 2020 2064 6566 206d 616b  end..    def mak
-00018bb0: 655f 726c 635f 626f 756e 6461 7279 2873  e_rlc_boundary(s
-00018bc0: 656c 662c 2061 7869 732c 2072 3d30 2c20  elf, axis, r=0, 
-00018bd0: 6c3d 302c 2063 3d30 2c20 6e61 6d65 3d22  l=0, c=0, name="
-00018be0: 4c75 6d70 524c 4322 293a 0a20 2020 2020  LumpRLC"):.     
-00018bf0: 2020 206e 616d 6520 3d20 7374 7228 7365     name = str(se
-00018c00: 6c66 2920 2b20 275f 2720 2b20 6e61 6d65  lf) + '_' + name
-00018c10: 0a20 2020 2020 2020 2073 7461 7274 2c20  .        start, 
-00018c20: 656e 6420 3d20 7365 6c66 2e6d 616b 655f  end = self.make_
-00018c30: 6365 6e74 6572 5f6c 696e 6528 6178 6973  center_line(axis
-00018c40: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-00018c50: 6f64 656c 6572 2e5f 6d61 6b65 5f6c 756d  odeler._make_lum
-00018c60: 7065 645f 726c 6328 722c 0a20 2020 2020  ped_rlc(r,.     
-00018c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c90: 206c 2c0a 2020 2020 2020 2020 2020 2020   l,.            
-00018ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cb0: 2020 2020 2020 2020 2020 632c 0a20 2020            c,.   
-00018cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 2020 2073 7461 7274 2c0a 2020 2020 2020     start,.      
-00018cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d10: 656e 642c 205b 224f 626a 6563 7473 3a3d  end, ["Objects:=
-00018d20: 222c 205b 7365 6c66 5d5d 2c0a 2020 2020  ", [self]],.    
-00018d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d50: 2020 6e61 6d65 3d6e 616d 6529 0a0a 2020    name=name)..  
-00018d60: 2020 6465 6620 6669 6c6c 6574 2873 656c    def fillet(sel
-00018d70: 662c 2072 6164 6975 732c 2076 6572 7465  f, radius, verte
-00018d80: 785f 696e 6465 7829 3a0a 2020 2020 2020  x_index):.      
-00018d90: 2020 7365 6c66 2e6d 6f64 656c 6572 2e5f    self.modeler._
-00018da0: 6669 6c6c 6574 2872 6164 6975 732c 2076  fillet(radius, v
-00018db0: 6572 7465 785f 696e 6465 782c 2073 656c  ertex_index, sel
-00018dc0: 6629 0a0a 2020 2020 6465 6620 7665 7274  f)..    def vert
-00018dd0: 6963 6573 2873 656c 6629 3a0a 2020 2020  ices(self):.    
-00018de0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00018df0: 6d6f 6465 6c65 722e 6765 745f 7665 7274  modeler.get_vert
-00018e00: 6578 5f69 6473 2873 656c 6629 0a0a 2020  ex_ids(self)..  
-00018e10: 2020 6465 6620 7265 6e61 6d65 2873 656c    def rename(sel
-00018e20: 662c 206e 6577 5f6e 616d 6529 3a0a 2020  f, new_name):.  
-00018e30: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00018e40: 2020 2020 2020 5761 726e 696e 673a 2054        Warning: T
-00018e50: 6865 2069 6e63 7265 6d65 6e74 5f6e 616d  he increment_nam
-00018e60: 6520 6f6e 6c79 2077 6f72 6b73 2069 6620  e only works if 
-00018e70: 7468 6520 7368 6565 7420 6861 7320 6e6f  the sheet has no
-00018e80: 7420 6265 656e 2073 7472 6163 7465 6420  t been stracted 
-00018e90: 6f72 2075 7365 6420 6173 2061 2074 6f6f  or used as a too
-00018ea0: 6c20 656c 7365 7768 6572 652e 0a20 2020  l elsewhere..   
-00018eb0: 2020 2020 2020 2020 2054 6865 7365 206e           These n
-00018ec0: 616d 6573 2061 7265 206e 6f74 2063 6865  ames are not che
-00018ed0: 636b 6564 3b20 7468 6579 2072 6571 7569  cked; they requi
-00018ee0: 7265 206d 6f64 6966 7969 6e67 2067 6574  re modifying get
-00018ef0: 5f6f 626a 6563 7473 5f69 6e5f 6772 6f75  _objects_in_grou
-00018f00: 702e 0a0a 2020 2020 2020 2020 2727 270a  p...        '''.
-00018f10: 2020 2020 2020 2020 6e65 775f 6e61 6d65          new_name
-00018f20: 203d 2069 6e63 7265 6d65 6e74 5f6e 616d   = increment_nam
-00018f30: 6528 0a20 2020 2020 2020 2020 2020 206e  e(.            n
-00018f40: 6577 5f6e 616d 652c 2073 656c 662e 6d6f  ew_name, self.mo
-00018f50: 6465 6c65 722e 6765 745f 6f62 6a65 6374  deler.get_object
-00018f60: 735f 696e 5f67 726f 7570 280a 2020 2020  s_in_group(.    
-00018f70: 2020 2020 2020 2020 2020 2020 2253 6865              "She
-00018f80: 6574 7322 2929 2020 2320 7468 6973 2069  ets"))  # this i
-00018f90: 7320 666f 7220 6120 636c 6f73 6564 2070  s for a closed p
-00018fa0: 6f6c 796c 696e 650a 0a20 2020 2020 2020  olyline..       
-00018fb0: 2023 2063 6865 636b 2074 6f20 6765 7420   # check to get 
-00018fc0: 7468 6520 6163 7475 616c 206e 6577 206e  the actual new n
-00018fd0: 616d 6520 696e 2063 6173 6520 7468 6572  ame in case ther
-00018fe0: 6520 7761 7320 6120 7375 6273 7472 6163  e was a substrac
-00018ff0: 7465 6420 6f62 6a65 6374 2077 6974 6820  ted object with 
-00019000: 7468 6174 206e 616d 650a 2020 2020 2020  that name.      
-00019010: 2020 6661 6365 5f69 6473 203d 2073 656c    face_ids = sel
-00019020: 662e 6d6f 6465 6c65 722e 6765 745f 6661  f.modeler.get_fa
-00019030: 6365 5f69 6473 2873 7472 2873 656c 6629  ce_ids(str(self)
-00019040: 290a 2020 2020 2020 2020 7365 6c66 2e6d  ).        self.m
-00019050: 6f64 656c 6572 2e72 656e 616d 655f 6f62  odeler.rename_ob
-00019060: 6a28 7365 6c66 2c20 6e65 775f 6e61 6d65  j(self, new_name
-00019070: 2920 2023 206e 6f77 2072 656e 616d 650a  )  # now rename.
-00019080: 2020 2020 2020 2020 6966 206c 656e 2866          if len(f
-00019090: 6163 655f 6964 7329 203e 2030 3a0a 2020  ace_ids) > 0:.  
-000190a0: 2020 2020 2020 2020 2020 6e65 775f 6e61            new_na
-000190b0: 6d65 203d 2073 656c 662e 6d6f 6465 6c65  me = self.modele
-000190c0: 722e 6765 745f 6f62 6a65 6374 5f6e 616d  r.get_object_nam
-000190d0: 655f 6279 5f66 6163 655f 6964 2866 6163  e_by_face_id(fac
-000190e0: 655f 6964 735b 305d 290a 2020 2020 2020  e_ids[0]).      
-000190f0: 2020 7265 7475 726e 2050 6f6c 796c 696e    return Polylin
-00019100: 6528 7374 7228 6e65 775f 6e61 6d65 292c  e(str(new_name),
-00019110: 2073 656c 662e 6d6f 6465 6c65 7229 0a0a   self.modeler)..
-00019120: 0a63 6c61 7373 204f 7065 6e50 6f6c 796c  .class OpenPolyl
-00019130: 696e 6528 4d6f 6465 6c45 6e74 6974 7929  ine(ModelEntity)
-00019140: 3a20 2023 2041 7373 756d 6520 636c 6f73  :  # Assume clos
-00019150: 6564 2070 6f6c 796c 696e 650a 2020 2020  ed polyline.    
-00019160: 6d6f 6465 6c5f 636f 6d6d 616e 6420 3d20  model_command = 
-00019170: 2243 7265 6174 6550 6f6c 796c 696e 6522  "CreatePolyline"
-00019180: 0a20 2020 2073 686f 775f 6469 7265 6374  .    show_direct
-00019190: 696f 6e20 3d20 6d61 6b65 5f70 726f 7028  ion = make_prop(
-000191a0: 2753 686f 7720 4469 7265 6374 696f 6e27  'Show Direction'
-000191b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000191c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191d0: 2070 726f 705f 7461 623d 2247 656f 6d65   prop_tab="Geome
-000191e0: 7472 7933 4441 7474 7269 6275 7465 5461  try3DAttributeTa
-000191f0: 6222 2c0a 2020 2020 2020 2020 2020 2020  b",.            
-00019200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019210: 2020 2070 726f 705f 7365 7276 6572 3d6c     prop_server=l
-00019220: 616d 6264 6120 7365 6c66 3a20 7365 6c66  ambda self: self
-00019230: 290a 0a20 2020 2064 6566 205f 5f69 6e69  )..    def __ini
-00019240: 745f 5f28 7365 6c66 2c20 6e61 6d65 2c20  t__(self, name, 
-00019250: 6d6f 6465 6c65 722c 2070 6f69 6e74 733d  modeler, points=
-00019260: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-00019270: 7570 6572 284f 7065 6e50 6f6c 796c 696e  uper(OpenPolylin
-00019280: 652c 2073 656c 6629 2e5f 5f69 6e69 745f  e, self).__init_
-00019290: 5f28 6e61 6d65 2c20 6d6f 6465 6c65 7229  _(name, modeler)
-000192a0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
-000192b0: 6f70 5f68 6f6c 6465 7220 3d20 6d6f 6465  op_holder = mode
-000192c0: 6c65 722e 5f6d 6f64 656c 6572 0a20 2020  ler._modeler.   
-000192d0: 2020 2020 2069 6620 706f 696e 7473 2069       if points i
-000192e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000192f0: 2020 2020 2020 2020 7365 6c66 2e70 6f69          self.poi
-00019300: 6e74 7320 3d20 706f 696e 7473 0a20 2020  nts = points.   
-00019310: 2020 2020 2020 2020 2073 656c 662e 6e5f           self.n_
-00019320: 706f 696e 7473 203d 206c 656e 2870 6f69  points = len(poi
-00019330: 6e74 7329 0a20 2020 2020 2020 2065 6c73  nts).        els
-00019340: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-00019350: 6173 730a 0a0a 2320 2020 2020 2020 2061  ass...#        a
-00019360: 7869 7320 3d20 6669 6e64 5f6f 7274 685f  xis = find_orth_
-00019370: 6178 6973 2829 0a0a 2320 544f 444f 3a20  axis()..# TODO: 
-00019380: 6669 6e64 2074 6865 2070 6c61 6e65 206f  find the plane o
-00019390: 6620 7468 6520 706f 6c79 6c69 6e65 2066  f the polyline f
-000193a0: 6f72 206e 6f77 2c20 6173 7375 6d65 205a  or now, assume Z
-000193b0: 0a23 2020 2020 6465 6620 6669 6e64 5f6f  .#    def find_o
-000193c0: 7274 685f 6178 6973 2829 3a0a 2320 2020  rth_axis():.#   
-000193d0: 2020 2020 2058 2c20 592c 205a 203d 2028       X, Y, Z = (
-000193e0: 5472 7565 2c20 5472 7565 2c20 5472 7565  True, True, True
-000193f0: 290a 2320 2020 2020 2020 2066 6f72 2070  ).#        for p
-00019400: 6f69 6e74 2069 6e20 706f 696e 7473 3a0a  oint in points:.
-00019410: 2320 2020 2020 2020 2020 2020 2058 203d  #            X =
-00019420: 0a0a 2020 2020 6465 6620 7665 7274 6963  ..    def vertic
-00019430: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
-00019440: 2020 7265 7475 726e 2073 656c 662e 6d6f    return self.mo
-00019450: 6465 6c65 722e 6765 745f 7665 7274 6578  deler.get_vertex
-00019460: 5f69 6473 2873 656c 6629 0a0a 2020 2020  _ids(self)..    
-00019470: 6465 6620 6669 6c6c 6574 2873 656c 662c  def fillet(self,
-00019480: 2072 6164 6975 732c 2076 6572 7465 785f   radius, vertex_
-00019490: 696e 6465 7829 3a0a 2020 2020 2020 2020  index):.        
-000194a0: 7365 6c66 2e6d 6f64 656c 6572 2e5f 6669  self.modeler._fi
-000194b0: 6c6c 6574 2872 6164 6975 732c 2076 6572  llet(radius, ver
-000194c0: 7465 785f 696e 6465 782c 2073 656c 6629  tex_index, self)
-000194d0: 0a0a 2020 2020 6465 6620 6669 6c6c 6574  ..    def fillet
-000194e0: 7328 7365 6c66 2c20 7261 6469 7573 2c20  s(self, radius, 
-000194f0: 646f 5f6e 6f74 5f66 696c 6c65 743d 5b5d  do_not_fillet=[]
-00019500: 293a 0a20 2020 2020 2020 2027 2727 0a20  ):.        '''. 
-00019510: 2020 2020 2020 2020 2020 2064 6f5f 6e6f             do_no
-00019520: 745f 6669 6c6c 6574 203a 2049 6e64 6578  t_fillet : Index
-00019530: 206c 6973 7420 6f66 2076 6572 7469 6365   list of vertice
-00019540: 7320 746f 206e 6f74 2066 696c 6c65 7465  s to not fillete
-00019550: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00019560: 2020 2020 2072 6177 5f6c 6973 745f 7665       raw_list_ve
-00019570: 7274 6963 6573 203d 2073 656c 662e 6d6f  rtices = self.mo
-00019580: 6465 6c65 722e 6765 745f 7665 7274 6578  deler.get_vertex
-00019590: 5f69 6473 2873 656c 6629 0a20 2020 2020  _ids(self).     
-000195a0: 2020 206c 6973 745f 7665 7274 6963 6573     list_vertices
-000195b0: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
-000195c0: 7220 7665 7274 6578 2069 6e20 7261 775f  r vertex in raw_
-000195d0: 6c69 7374 5f76 6572 7469 6365 735b 313a  list_vertices[1:
-000195e0: 2d31 5d3a 2020 2320 6967 6e6f 7265 2074  -1]:  # ignore t
-000195f0: 6865 2073 7461 7274 2061 6e64 2066 696e  he start and fin
-00019600: 6973 680a 2020 2020 2020 2020 2020 2020  ish.            
-00019610: 6c69 7374 5f76 6572 7469 6365 732e 6170  list_vertices.ap
-00019620: 7065 6e64 2869 6e74 2876 6572 7465 7829  pend(int(vertex)
-00019630: 290a 2020 2020 2020 2020 6c69 7374 5f76  ).        list_v
-00019640: 6572 7469 6365 7320 3d20 6c69 7374 280a  ertices = list(.
-00019650: 2020 2020 2020 2020 2020 2020 6d61 7028              map(
-00019660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019670: 2069 6e74 2c0a 2020 2020 2020 2020 2020   int,.          
-00019680: 2020 2020 2020 6e70 2e64 656c 6574 6528        np.delete(
-00019690: 6c69 7374 5f76 6572 7469 6365 732c 0a20  list_vertices,. 
-000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196b0: 2020 2020 2020 2020 206e 702e 6172 7261           np.arra
-000196c0: 7928 646f 5f6e 6f74 5f66 696c 6c65 742c  y(do_not_fillet,
-000196d0: 2064 7479 7065 3d69 6e74 2920 2d20 3129   dtype=int) - 1)
-000196e0: 2929 0a20 2020 2020 2020 2023 7072 696e  )).        #prin
-000196f0: 7428 6c69 7374 5f76 6572 7469 6365 732c  t(list_vertices,
-00019700: 2074 7970 6528 6c69 7374 5f76 6572 7469   type(list_verti
-00019710: 6365 735b 305d 2929 0a20 2020 2020 2020  ces[0])).       
-00019720: 2069 6620 6c65 6e28 6c69 7374 5f76 6572   if len(list_ver
-00019730: 7469 6365 7329 2021 3d20 303a 0a20 2020  tices) != 0:.   
-00019740: 2020 2020 2020 2020 2073 656c 662e 6d6f           self.mo
-00019750: 6465 6c65 722e 5f66 696c 6c65 7473 2872  deler._fillets(r
-00019760: 6164 6975 732c 206c 6973 745f 7665 7274  adius, list_vert
-00019770: 6963 6573 2c20 7365 6c66 290a 2020 2020  ices, self).    
-00019780: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00019790: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-000197a0: 6465 6620 7377 6565 705f 616c 6f6e 675f  def sweep_along_
-000197b0: 7061 7468 2873 656c 662c 2074 6f5f 7377  path(self, to_sw
-000197c0: 6565 7029 3a0a 2020 2020 2020 2020 7265  eep):.        re
-000197d0: 7475 726e 2073 656c 662e 6d6f 6465 6c65  turn self.modele
-000197e0: 722e 5f73 7765 6570 5f61 6c6f 6e67 5f70  r._sweep_along_p
-000197f0: 6174 6828 746f 5f73 7765 6570 2c20 7365  ath(to_sweep, se
-00019800: 6c66 290a 0a20 2020 2064 6566 2072 656e  lf)..    def ren
-00019810: 616d 6528 7365 6c66 2c20 6e65 775f 6e61  ame(self, new_na
-00019820: 6d65 293a 0a20 2020 2020 2020 2027 2727  me):.        '''
-00019830: 0a20 2020 2020 2020 2020 2020 2057 6172  .            War
-00019840: 6e69 6e67 3a20 5468 6520 2069 6e63 7265  ning: The  incre
-00019850: 6d65 6e74 5f6e 616d 6520 6f6e 6c79 2077  ment_name only w
-00019860: 6f72 6b73 2069 6620 7468 6520 7368 6565  orks if the shee
-00019870: 7420 6861 7320 6e6f 7420 6265 656e 2073  t has not been s
-00019880: 7472 6163 7465 6420 6f72 2075 7365 6420  tracted or used 
-00019890: 6173 2061 2074 6f6f 6c20 656c 7365 7768  as a tool elsewh
-000198a0: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
-000198b0: 5468 6573 6520 6e61 6d65 7320 6172 6520  These names are 
-000198c0: 6e6f 7420 6368 6563 6b65 6420 2d20 5468  not checked - Th
-000198d0: 6579 2072 6571 7569 7265 206d 6f64 6966  ey require modif
-000198e0: 7969 6e67 2067 6574 5f6f 626a 6563 7473  ying get_objects
-000198f0: 5f69 6e5f 6772 6f75 700a 2020 2020 2020  _in_group.      
-00019900: 2020 2727 270a 2020 2020 2020 2020 6e65    '''.        ne
-00019910: 775f 6e61 6d65 203d 2069 6e63 7265 6d65  w_name = increme
-00019920: 6e74 5f6e 616d 6528 6e65 775f 6e61 6d65  nt_name(new_name
-00019930: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019950: 2020 2020 7365 6c66 2e6d 6f64 656c 6572      self.modeler
-00019960: 2e67 6574 5f6f 626a 6563 7473 5f69 6e5f  .get_objects_in_
-00019970: 6772 6f75 7028 224c 696e 6573 2229 290a  group("Lines")).
-00019980: 2020 2020 2020 2020 2320 2c20 7365 6c66          # , self
-00019990: 2e70 6f69 6e74 7329 0a20 2020 2020 2020  .points).       
-000199a0: 2072 6574 7572 6e20 4f70 656e 506f 6c79   return OpenPoly
-000199b0: 6c69 6e65 2873 656c 662e 6d6f 6465 6c65  line(self.modele
-000199c0: 722e 7265 6e61 6d65 5f6f 626a 2873 656c  r.rename_obj(sel
-000199d0: 662c 206e 6577 5f6e 616d 6529 2c0a 2020  f, new_name),.  
-000199e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199f0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00019a00: 6f64 656c 6572 290a 0a20 2020 2064 6566  odeler)..    def
-00019a10: 2063 6f70 7928 7365 6c66 2c20 6e65 775f   copy(self, new_
-00019a20: 6e61 6d65 293a 0a20 2020 2020 2020 206e  name):.        n
-00019a30: 6577 5f6f 626a 203d 204f 7065 6e50 6f6c  ew_obj = OpenPol
-00019a40: 796c 696e 6528 7365 6c66 2e6d 6f64 656c  yline(self.model
-00019a50: 6572 2e63 6f70 7928 7365 6c66 292c 2073  er.copy(self), s
-00019a60: 656c 662e 6d6f 6465 6c65 7229 0a20 2020  elf.modeler).   
-00019a70: 2020 2020 2072 6574 7572 6e20 6e65 775f       return new_
-00019a80: 6f62 6a2e 7265 6e61 6d65 286e 6577 5f6e  obj.rename(new_n
-00019a90: 616d 6529 0a0a 0a63 6c61 7373 2048 6673  ame)...class Hfs
-00019aa0: 7346 6965 6c64 7343 616c 6328 434f 4d57  sFieldsCalc(COMW
-00019ab0: 7261 7070 6572 293a 0a20 2020 2064 6566  rapper):.    def
-00019ac0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00019ad0: 7365 7475 7029 3a0a 2020 2020 2020 2020  setup):.        
-00019ae0: 2222 220a 2020 2020 2020 2020 3a74 7970  """.        :typ
-00019af0: 6520 7365 7475 703a 2048 6673 7353 6574  e setup: HfssSet
-00019b00: 7570 0a20 2020 2020 2020 2022 2222 0a20  up.        """. 
-00019b10: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-00019b20: 7020 3d20 7365 7475 700a 2020 2020 2020  p = setup.      
-00019b30: 2020 7375 7065 7228 4866 7373 4669 656c    super(HfssFiel
-00019b40: 6473 4361 6c63 2c20 7365 6c66 292e 5f5f  dsCalc, self).__
-00019b50: 696e 6974 5f5f 2829 0a20 2020 2020 2020  init__().       
-00019b60: 2073 656c 662e 7061 7265 6e74 203d 2073   self.parent = s
-00019b70: 6574 7570 0a20 2020 2020 2020 2073 656c  etup.        sel
-00019b80: 662e 4d61 675f 4520 3d20 4e61 6d65 6443  f.Mag_E = NamedC
-00019b90: 616c 634f 626a 6563 7428 224d 6167 5f45  alcObject("Mag_E
-00019ba0: 222c 2073 6574 7570 290a 2020 2020 2020  ", setup).      
-00019bb0: 2020 7365 6c66 2e4d 6167 5f48 203d 204e    self.Mag_H = N
-00019bc0: 616d 6564 4361 6c63 4f62 6a65 6374 2822  amedCalcObject("
-00019bd0: 4d61 675f 4822 2c20 7365 7475 7029 0a20  Mag_H", setup). 
-00019be0: 2020 2020 2020 2073 656c 662e 4d61 675f         self.Mag_
-00019bf0: 4a73 7572 6620 3d20 4e61 6d65 6443 616c  Jsurf = NamedCal
-00019c00: 634f 626a 6563 7428 224d 6167 5f4a 7375  cObject("Mag_Jsu
-00019c10: 7266 222c 2073 6574 7570 290a 2020 2020  rf", setup).    
-00019c20: 2020 2020 7365 6c66 2e4d 6167 5f4a 766f      self.Mag_Jvo
-00019c30: 6c20 3d20 4e61 6d65 6443 616c 634f 626a  l = NamedCalcObj
-00019c40: 6563 7428 224d 6167 5f4a 766f 6c22 2c20  ect("Mag_Jvol", 
-00019c50: 7365 7475 7029 0a20 2020 2020 2020 2073  setup).        s
-00019c60: 656c 662e 5665 6374 6f72 5f45 203d 204e  elf.Vector_E = N
-00019c70: 616d 6564 4361 6c63 4f62 6a65 6374 2822  amedCalcObject("
-00019c80: 5665 6374 6f72 5f45 222c 2073 6574 7570  Vector_E", setup
-00019c90: 290a 2020 2020 2020 2020 7365 6c66 2e56  ).        self.V
-00019ca0: 6563 746f 725f 4820 3d20 4e61 6d65 6443  ector_H = NamedC
-00019cb0: 616c 634f 626a 6563 7428 2256 6563 746f  alcObject("Vecto
-00019cc0: 725f 4822 2c20 7365 7475 7029 0a20 2020  r_H", setup).   
-00019cd0: 2020 2020 2073 656c 662e 5665 6374 6f72       self.Vector
-00019ce0: 5f4a 7375 7266 203d 204e 616d 6564 4361  _Jsurf = NamedCa
-00019cf0: 6c63 4f62 6a65 6374 2822 5665 6374 6f72  lcObject("Vector
-00019d00: 5f4a 7375 7266 222c 2073 6574 7570 290a  _Jsurf", setup).
-00019d10: 2020 2020 2020 2020 7365 6c66 2e56 6563          self.Vec
-00019d20: 746f 725f 4a76 6f6c 203d 204e 616d 6564  tor_Jvol = Named
-00019d30: 4361 6c63 4f62 6a65 6374 2822 5665 6374  CalcObject("Vect
-00019d40: 6f72 5f4a 766f 6c22 2c20 7365 7475 7029  or_Jvol", setup)
-00019d50: 0a20 2020 2020 2020 2073 656c 662e 436f  .        self.Co
-00019d60: 6d70 6c65 784d 6167 5f45 203d 204e 616d  mplexMag_E = Nam
-00019d70: 6564 4361 6c63 4f62 6a65 6374 2822 436f  edCalcObject("Co
-00019d80: 6d70 6c65 784d 6167 5f45 222c 2073 6574  mplexMag_E", set
-00019d90: 7570 290a 2020 2020 2020 2020 7365 6c66  up).        self
-00019da0: 2e43 6f6d 706c 6578 4d61 675f 4820 3d20  .ComplexMag_H = 
-00019db0: 4e61 6d65 6443 616c 634f 626a 6563 7428  NamedCalcObject(
-00019dc0: 2243 6f6d 706c 6578 4d61 675f 4822 2c20  "ComplexMag_H", 
-00019dd0: 7365 7475 7029 0a20 2020 2020 2020 2073  setup).        s
-00019de0: 656c 662e 436f 6d70 6c65 784d 6167 5f4a  elf.ComplexMag_J
-00019df0: 7375 7266 203d 204e 616d 6564 4361 6c63  surf = NamedCalc
-00019e00: 4f62 6a65 6374 2822 436f 6d70 6c65 784d  Object("ComplexM
-00019e10: 6167 5f4a 7375 7266 222c 2073 6574 7570  ag_Jsurf", setup
-00019e20: 290a 2020 2020 2020 2020 7365 6c66 2e43  ).        self.C
-00019e30: 6f6d 706c 6578 4d61 675f 4a76 6f6c 203d  omplexMag_Jvol =
-00019e40: 204e 616d 6564 4361 6c63 4f62 6a65 6374   NamedCalcObject
-00019e50: 2822 436f 6d70 6c65 784d 6167 5f4a 766f  ("ComplexMag_Jvo
-00019e60: 6c22 2c20 7365 7475 7029 0a20 2020 2020  l", setup).     
-00019e70: 2020 2073 656c 662e 505f 4a20 3d20 4e61     self.P_J = Na
-00019e80: 6d65 6443 616c 634f 626a 6563 7428 2250  medCalcObject("P
-00019e90: 5f4a 222c 2073 6574 7570 290a 0a20 2020  _J", setup)..   
-00019ea0: 2020 2020 2073 656c 662e 6e61 6d65 645f       self.named_
-00019eb0: 6578 7072 6573 7369 6f6e 203d 207b 0a20  expression = {. 
-00019ec0: 2020 2020 2020 207d 2020 2320 6469 6374         }  # dict
-00019ed0: 696f 6e61 7279 2074 6f20 686f 6c64 2061  ionary to hold a
-00019ee0: 6464 6974 696f 6e61 6c20 6e61 6d65 6420  dditional named 
-00019ef0: 6578 7072 6573 7369 6f6e 730a 0a20 2020  expressions..   
-00019f00: 2064 6566 2063 6c65 6172 5f6e 616d 6564   def clear_named
-00019f10: 5f65 7870 7265 7373 696f 6e73 2873 656c  _expressions(sel
-00019f20: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00019f30: 2e70 6172 656e 742e 7061 7265 6e74 2e5f  .parent.parent._
-00019f40: 6669 656c 6473 5f63 616c 632e 436c 6561  fields_calc.Clea
-00019f50: 7241 6c6c 4e61 6d65 6445 7870 7228 290a  rAllNamedExpr().
-00019f60: 0a20 2020 2064 6566 2064 6563 6c61 7265  .    def declare
-00019f70: 5f6e 616d 6564 5f65 7870 7265 7373 696f  _named_expressio
-00019f80: 6e28 7365 6c66 2c20 6e61 6d65 293a 0a20  n(self, name):. 
-00019f90: 2020 2020 2020 2022 2222 220a 2020 2020         """".    
-00019fa0: 2020 2020 4966 2061 206e 616d 6564 2065      If a named e
-00019fb0: 7870 7265 7373 696f 6e20 6861 7320 6265  xpression has be
-00019fc0: 656e 2063 7265 6174 6564 2069 6e20 7468  en created in th
-00019fd0: 6520 6669 656c 6473 2063 616c 6375 6c61  e fields calcula
-00019fe0: 746f 722c 2074 6869 730a 2020 2020 2020  tor, this.      
-00019ff0: 2020 6675 6e63 7469 6f6e 2063 616e 2062    function can b
-0001a000: 6520 6361 6c6c 6564 2074 6f20 696e 6974  e called to init
-0001a010: 6961 6c69 7a65 2074 6865 206e 616d 6520  ialize the name 
-0001a020: 746f 2077 6f72 6b20 7769 7468 2074 6865  to work with the
-0001a030: 2066 6965 6c64 7320 6f62 6a65 6374 0a20   fields object. 
-0001a040: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0001a050: 2020 2073 656c 662e 6e61 6d65 645f 6578     self.named_ex
-0001a060: 7072 6573 7369 6f6e 5b6e 616d 655d 203d  pression[name] =
-0001a070: 204e 616d 6564 4361 6c63 4f62 6a65 6374   NamedCalcObject
-0001a080: 286e 616d 652c 2073 656c 662e 7365 7475  (name, self.setu
-0001a090: 7029 0a0a 2020 2020 6465 6620 7573 655f  p)..    def use_
-0001a0a0: 6e61 6d65 645f 6578 7072 6573 7369 6f6e  named_expression
-0001a0b0: 2873 656c 662c 206e 616d 6529 3a0a 2020  (self, name):.  
-0001a0c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0001a0d0: 2020 4578 7072 6573 7369 6f6e 2063 616e    Expression can
-0001a0e0: 2062 6520 7573 6564 2074 6f20 6163 6365   be used to acce
-0001a0f0: 7373 2064 6963 7469 6f6e 6172 7920 6f66  ss dictionary of
-0001a100: 206e 616d 6564 2065 7870 7265 7373 696f   named expressio
-0001a110: 6e73 2c0a 2020 2020 2020 2020 416c 7465  ns,.        Alte
-0001a120: 726e 6174 656c 7920 7573 6572 2063 616e  rnately user can
-0001a130: 2061 6363 6573 7320 6469 6374 696f 6e61   access dictiona
-0001a140: 7279 2064 6972 6563 746c 7920 7669 6120  ry directly via 
-0001a150: 6e61 6d65 645f 6578 7072 6573 7369 6f6e  named_expression
-0001a160: 2829 0a20 2020 2020 2020 2022 2222 0a20  ().        """. 
-0001a170: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001a180: 6c66 2e6e 616d 6564 5f65 7870 7265 7373  lf.named_express
-0001a190: 696f 6e5b 6e61 6d65 5d0a 0a0a 636c 6173  ion[name]...clas
-0001a1a0: 7320 4361 6c63 4f62 6a65 6374 2843 4f4d  s CalcObject(COM
-0001a1b0: 5772 6170 7065 7229 3a0a 2020 2020 6465  Wrapper):.    de
-0001a1c0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0001a1d0: 2073 7461 636b 2c20 7365 7475 7029 3a0a   stack, setup):.
-0001a1e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0001a1f0: 2020 2020 3a74 7970 6520 7374 6163 6b3a      :type stack:
-0001a200: 205b 2873 7472 2c20 7374 7229 5d0a 2020   [(str, str)].  
-0001a210: 2020 2020 2020 3a74 7970 6520 7365 7475        :type setu
-0001a220: 703a 2048 6673 7353 6574 7570 0a20 2020  p: HfssSetup.   
-0001a230: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001a240: 2073 7570 6572 2843 616c 634f 626a 6563   super(CalcObjec
-0001a250: 742c 2073 656c 6629 2e5f 5f69 6e69 745f  t, self).__init_
-0001a260: 5f28 290a 2020 2020 2020 2020 7365 6c66  _().        self
-0001a270: 2e73 7461 636b 203d 2073 7461 636b 0a20  .stack = stack. 
-0001a280: 2020 2020 2020 2073 656c 662e 7365 7475         self.setu
-0001a290: 7020 3d20 7365 7475 700a 2020 2020 2020  p = setup.      
-0001a2a0: 2020 7365 6c66 2e63 616c 635f 6d6f 6475    self.calc_modu
-0001a2b0: 6c65 203d 2073 6574 7570 2e70 6172 656e  le = setup.paren
-0001a2c0: 742e 5f66 6965 6c64 735f 6361 6c63 0a0a  t._fields_calc..
-0001a2d0: 2020 2020 6465 6620 5f62 696e 5f6f 7028      def _bin_op(
-0001a2e0: 7365 6c66 2c20 6f74 6865 722c 206f 7029  self, other, op)
-0001a2f0: 3a0a 2020 2020 2020 2020 6966 2069 7369  :.        if isi
-0001a300: 6e73 7461 6e63 6528 6f74 6865 722c 2028  nstance(other, (
-0001a310: 696e 742c 2066 6c6f 6174 2929 3a0a 2020  int, float)):.  
-0001a320: 2020 2020 2020 2020 2020 6f74 6865 7220            other 
-0001a330: 3d20 436f 6e73 7461 6e74 4361 6c63 4f62  = ConstantCalcOb
-0001a340: 6a65 6374 286f 7468 6572 2c20 7365 6c66  ject(other, self
-0001a350: 2e73 6574 7570 290a 0a20 2020 2020 2020  .setup)..       
-0001a360: 2073 7461 636b 203d 2073 656c 662e 7374   stack = self.st
-0001a370: 6163 6b20 2b20 6f74 6865 722e 7374 6163  ack + other.stac
-0001a380: 6b0a 2020 2020 2020 2020 7374 6163 6b2e  k.        stack.
-0001a390: 6170 7065 6e64 2828 2243 616c 634f 7022  append(("CalcOp"
-0001a3a0: 2c20 6f70 2929 0a20 2020 2020 2020 2072  , op)).        r
-0001a3b0: 6574 7572 6e20 4361 6c63 4f62 6a65 6374  eturn CalcObject
-0001a3c0: 2873 7461 636b 2c20 7365 6c66 2e73 6574  (stack, self.set
-0001a3d0: 7570 290a 0a20 2020 2064 6566 205f 756e  up)..    def _un
-0001a3e0: 6172 795f 6f70 2873 656c 662c 206f 7029  ary_op(self, op)
-0001a3f0: 3a0a 2020 2020 2020 2020 7374 6163 6b20  :.        stack 
-0001a400: 3d20 7365 6c66 2e73 7461 636b 5b3a 5d0a  = self.stack[:].
-0001a410: 2020 2020 2020 2020 7374 6163 6b2e 6170          stack.ap
-0001a420: 7065 6e64 2828 2243 616c 634f 7022 2c20  pend(("CalcOp", 
-0001a430: 6f70 2929 0a20 2020 2020 2020 2072 6574  op)).        ret
-0001a440: 7572 6e20 4361 6c63 4f62 6a65 6374 2873  urn CalcObject(s
-0001a450: 7461 636b 2c20 7365 6c66 2e73 6574 7570  tack, self.setup
-0001a460: 290a 0a20 2020 2064 6566 205f 5f61 6464  )..    def __add
-0001a470: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
-0001a480: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001a490: 7365 6c66 2e5f 6269 6e5f 6f70 286f 7468  self._bin_op(oth
-0001a4a0: 6572 2c20 222b 2229 0a0a 2020 2020 6465  er, "+")..    de
-0001a4b0: 6620 5f5f 7261 6464 5f5f 2873 656c 662c  f __radd__(self,
-0001a4c0: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-0001a4d0: 2072 6574 7572 6e20 7365 6c66 202b 206f   return self + o
-0001a4e0: 7468 6572 0a0a 2020 2020 6465 6620 5f5f  ther..    def __
-0001a4f0: 7375 625f 5f28 7365 6c66 2c20 6f74 6865  sub__(self, othe
-0001a500: 7229 3a0a 2020 2020 2020 2020 7265 7475  r):.        retu
-0001a510: 726e 2073 656c 662e 5f62 696e 5f6f 7028  rn self._bin_op(
-0001a520: 6f74 6865 722c 2022 2d22 290a 0a20 2020  other, "-")..   
-0001a530: 2064 6566 205f 5f72 7375 625f 5f28 7365   def __rsub__(se
-0001a540: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-0001a550: 2020 2020 7265 7475 726e 2028 2d73 656c      return (-sel
-0001a560: 6629 202b 206f 7468 6572 0a0a 2020 2020  f) + other..    
-0001a570: 6465 6620 5f5f 6d75 6c5f 5f28 7365 6c66  def __mul__(self
-0001a580: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-0001a590: 2020 7265 7475 726e 2073 656c 662e 5f62    return self._b
-0001a5a0: 696e 5f6f 7028 6f74 6865 722c 2022 2a22  in_op(other, "*"
-0001a5b0: 290a 0a20 2020 2064 6566 205f 5f72 6d75  )..    def __rmu
-0001a5c0: 6c5f 5f28 7365 6c66 2c20 6f74 6865 7229  l__(self, other)
-0001a5d0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001a5e0: 2073 656c 6620 2a20 6f74 6865 720a 0a20   self * other.. 
-0001a5f0: 2020 2064 6566 205f 5f64 6976 5f5f 2873     def __div__(s
-0001a600: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-0001a610: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001a620: 2e5f 6269 6e5f 6f70 286f 7468 6572 2c20  ._bin_op(other, 
-0001a630: 222f 2229 0a0a 2020 2020 6465 6620 5f5f  "/")..    def __
-0001a640: 7264 6976 5f5f 2873 656c 662c 206f 7468  rdiv__(self, oth
-0001a650: 6572 293a 0a20 2020 2020 2020 206f 7468  er):.        oth
-0001a660: 6572 203d 2043 6f6e 7374 616e 7443 616c  er = ConstantCal
-0001a670: 634f 626a 6563 7428 6f74 6865 722c 2073  cObject(other, s
-0001a680: 656c 662e 7365 7475 7029 0a20 2020 2020  elf.setup).     
-0001a690: 2020 2072 6574 7572 6e20 6f74 6865 7220     return other 
-0001a6a0: 2f20 7365 6c66 0a0a 2020 2020 6465 6620  / self..    def 
-0001a6b0: 5f5f 706f 775f 5f28 7365 6c66 2c20 6f74  __pow__(self, ot
-0001a6c0: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
-0001a6d0: 7475 726e 2073 656c 662e 5f62 696e 5f6f  turn self._bin_o
-0001a6e0: 7028 6f74 6865 722c 2022 506f 7722 290a  p(other, "Pow").
-0001a6f0: 0a20 2020 2064 6566 2064 6f74 2873 656c  .    def dot(sel
-0001a700: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
-0001a710: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0001a720: 6269 6e5f 6f70 286f 7468 6572 2c20 2244  bin_op(other, "D
-0001a730: 6f74 2229 0a0a 2020 2020 6465 6620 5f5f  ot")..    def __
-0001a740: 6e65 675f 5f28 7365 6c66 293a 0a20 2020  neg__(self):.   
-0001a750: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001a760: 2e5f 756e 6172 795f 6f70 2822 4e65 6722  ._unary_op("Neg"
-0001a770: 290a 0a20 2020 2064 6566 205f 5f61 6273  )..    def __abs
-0001a780: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-0001a790: 2020 7265 7475 726e 2073 656c 662e 5f75    return self._u
-0001a7a0: 6e61 7279 5f6f 7028 2241 6273 2229 0a0a  nary_op("Abs")..
-0001a7b0: 2020 2020 6465 6620 5f5f 6d61 675f 5f28      def __mag__(
-0001a7c0: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-0001a7d0: 6574 7572 6e20 7365 6c66 2e5f 756e 6172  eturn self._unar
-0001a7e0: 795f 6f70 2822 4d61 6722 290a 0a20 2020  y_op("Mag")..   
-0001a7f0: 2064 6566 206d 6167 2873 656c 6629 3a0a   def mag(self):.
-0001a800: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001a810: 656c 662e 5f75 6e61 7279 5f6f 7028 224d  elf._unary_op("M
-0001a820: 6167 2229 0a0a 2020 2020 6465 6620 736d  ag")..    def sm
-0001a830: 6f6f 7468 2873 656c 6629 3a0a 2020 2020  ooth(self):.    
-0001a840: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001a850: 5f75 6e61 7279 5f6f 7028 2253 6d6f 6f74  _unary_op("Smoot
-0001a860: 6822 290a 0a20 2020 2064 6566 2063 6f6e  h")..    def con
-0001a870: 6a28 7365 6c66 293a 0a20 2020 2020 2020  j(self):.       
-0001a880: 2072 6574 7572 6e20 7365 6c66 2e5f 756e   return self._un
-0001a890: 6172 795f 6f70 2822 436f 6e6a 2229 2020  ary_op("Conj")  
-0001a8a0: 2320 6d61 6b65 2074 6869 7320 7269 6768  # make this righ
-0001a8b0: 740a 0a20 2020 2064 6566 2073 6361 6c61  t..    def scala
-0001a8c0: 725f 7828 7365 6c66 293a 0a20 2020 2020  r_x(self):.     
-0001a8d0: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-0001a8e0: 756e 6172 795f 6f70 2822 5363 616c 6172  unary_op("Scalar
-0001a8f0: 5822 290a 0a20 2020 2064 6566 2073 6361  X")..    def sca
-0001a900: 6c61 725f 7928 7365 6c66 293a 0a20 2020  lar_y(self):.   
-0001a910: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001a920: 2e5f 756e 6172 795f 6f70 2822 5363 616c  ._unary_op("Scal
-0001a930: 6172 5922 290a 0a20 2020 2064 6566 2073  arY")..    def s
-0001a940: 6361 6c61 725f 7a28 7365 6c66 293a 0a20  calar_z(self):. 
-0001a950: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001a960: 6c66 2e5f 756e 6172 795f 6f70 2822 5363  lf._unary_op("Sc
-0001a970: 616c 6172 5a22 290a 0a20 2020 2064 6566  alarZ")..    def
-0001a980: 206e 6f72 6d5f 3228 7365 6c66 293a 0a0a   norm_2(self):..
-0001a990: 2020 2020 2020 2020 7265 7475 726e 2028          return (
-0001a9a0: 7365 6c66 2e5f 5f6d 6167 5f5f 2829 292e  self.__mag__()).
-0001a9b0: 5f5f 706f 775f 5f28 3229 0a20 2020 2020  __pow__(2).     
-0001a9c0: 2020 2023 2072 6574 7572 6e20 7365 6c66     # return self
-0001a9d0: 2e5f 756e 6172 795f 6f70 2822 5363 616c  ._unary_op("Scal
-0001a9e0: 6172 5822 292a 2a32 2b73 656c 662e 5f75  arX")**2+self._u
-0001a9f0: 6e61 7279 5f6f 7028 2253 6361 6c61 7259  nary_op("ScalarY
-0001aa00: 2229 2a2a 322b 7365 6c66 2e5f 756e 6172  ")**2+self._unar
-0001aa10: 795f 6f70 2822 5363 616c 6172 5a22 292a  y_op("ScalarZ")*
-0001aa20: 2a32 0a0a 2020 2020 6465 6620 7265 616c  *2..    def real
-0001aa30: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0001aa40: 7265 7475 726e 2073 656c 662e 5f75 6e61  return self._una
-0001aa50: 7279 5f6f 7028 2252 6561 6c22 290a 0a20  ry_op("Real").. 
-0001aa60: 2020 2064 6566 2069 6d61 6728 7365 6c66     def imag(self
-0001aa70: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-0001aa80: 6e20 7365 6c66 2e5f 756e 6172 795f 6f70  n self._unary_op
-0001aa90: 2822 496d 6167 2229 0a0a 2020 2020 6465  ("Imag")..    de
-0001aaa0: 6620 636f 6d70 6c65 786d 6167 2873 656c  f complexmag(sel
-0001aab0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-0001aac0: 726e 2073 656c 662e 5f75 6e61 7279 5f6f  rn self._unary_o
-0001aad0: 7028 2243 6d70 6c78 4d61 6722 290a 0a20  p("CmplxMag").. 
-0001aae0: 2020 2064 6566 205f 696e 7465 6772 6174     def _integrat
-0001aaf0: 6528 7365 6c66 2c20 6e61 6d65 2c20 7479  e(self, name, ty
-0001ab00: 7065 293a 0a20 2020 2020 2020 2073 7461  pe):.        sta
-0001ab10: 636b 203d 2073 656c 662e 7374 6163 6b20  ck = self.stack 
-0001ab20: 2b20 5b28 7479 7065 2c20 6e61 6d65 292c  + [(type, name),
-0001ab30: 2028 2243 616c 634f 7022 2c20 2249 6e74   ("CalcOp", "Int
-0001ab40: 6567 7261 7465 2229 5d0a 2020 2020 2020  egrate")].      
-0001ab50: 2020 7265 7475 726e 2043 616c 634f 626a    return CalcObj
-0001ab60: 6563 7428 7374 6163 6b2c 2073 656c 662e  ect(stack, self.
-0001ab70: 7365 7475 7029 0a0a 2020 2020 6465 6620  setup)..    def 
-0001ab80: 5f6d 6178 696d 756d 2873 656c 662c 206e  _maximum(self, n
-0001ab90: 616d 652c 2074 7970 6529 3a0a 2020 2020  ame, type):.    
-0001aba0: 2020 2020 7374 6163 6b20 3d20 7365 6c66      stack = self
-0001abb0: 2e73 7461 636b 202b 205b 2874 7970 652c  .stack + [(type,
-0001abc0: 206e 616d 6529 2c20 2822 4361 6c63 4f70   name), ("CalcOp
-0001abd0: 222c 2022 4d61 7869 6d75 6d22 295d 0a20  ", "Maximum")]. 
-0001abe0: 2020 2020 2020 2072 6574 7572 6e20 4361         return Ca
-0001abf0: 6c63 4f62 6a65 6374 2873 7461 636b 2c20  lcObject(stack, 
-0001ac00: 7365 6c66 2e73 6574 7570 290a 0a20 2020  self.setup)..   
-0001ac10: 2064 6566 2067 6574 5174 7928 7365 6c66   def getQty(self
-0001ac20: 2c20 6e61 6d65 293a 0a20 2020 2020 2020  , name):.       
-0001ac30: 2073 7461 636b 203d 2073 656c 662e 7374   stack = self.st
-0001ac40: 6163 6b20 2b20 5b28 2245 6e74 6572 5174  ack + [("EnterQt
-0001ac50: 7922 2c20 6e61 6d65 295d 0a20 2020 2020  y", name)].     
-0001ac60: 2020 2072 6574 7572 6e20 4361 6c63 4f62     return CalcOb
-0001ac70: 6a65 6374 2873 7461 636b 2c20 7365 6c66  ject(stack, self
-0001ac80: 2e73 6574 7570 290a 0a20 2020 2064 6566  .setup)..    def
-0001ac90: 2069 6e74 6567 7261 7465 5f6c 696e 6528   integrate_line(
-0001aca0: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
-0001acb0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001acc0: 2e5f 696e 7465 6772 6174 6528 6e61 6d65  ._integrate(name
-0001acd0: 2c20 2245 6e74 6572 4c69 6e65 2229 0a0a  , "EnterLine")..
-0001ace0: 2020 2020 6465 6620 6e6f 726d 616c 3273      def normal2s
-0001acf0: 7572 6661 6365 2873 656c 662c 206e 616d  urface(self, nam
-0001ad00: 6529 3a0a 2020 2020 2020 2020 2727 2720  e):.        ''' 
-0001ad10: 7265 7475 726e 2074 6865 2070 6172 7420  return the part 
-0001ad20: 6e6f 726d 616c 2074 6f20 7375 7266 6163  normal to surfac
-0001ad30: 652e 0a20 2020 2020 2020 2020 2020 2043  e..            C
-0001ad40: 6f6d 706c 6578 2056 6563 746f 722e 2027  omplex Vector. '
-0001ad50: 2727 0a20 2020 2020 2020 2073 7461 636b  ''.        stack
-0001ad60: 203d 2073 656c 662e 7374 6163 6b20 2b20   = self.stack + 
-0001ad70: 5b28 2245 6e74 6572 5375 7266 222c 206e  [("EnterSurf", n
-0001ad80: 616d 6529 2c0a 2020 2020 2020 2020 2020  ame),.          
-0001ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ada0: 2020 2020 2020 2822 4361 6c63 4f70 222c        ("CalcOp",
-0001adb0: 2020 2020 224e 6f72 6d61 6c22 295d 0a20      "Normal")]. 
-0001adc0: 2020 2020 2020 2073 7461 636b 2e61 7070         stack.app
-0001add0: 656e 6428 2822 4361 6c63 4f70 222c 2022  end(("CalcOp", "
-0001ade0: 446f 7422 2929 0a20 2020 2020 2020 2073  Dot")).        s
-0001adf0: 7461 636b 2e61 7070 656e 6428 2822 456e  tack.append(("En
-0001ae00: 7465 7253 7572 6622 2c20 6e61 6d65 2929  terSurf", name))
-0001ae10: 0a20 2020 2020 2020 2073 7461 636b 2e61  .        stack.a
-0001ae20: 7070 656e 6428 2822 4361 6c63 4f70 222c  ppend(("CalcOp",
-0001ae30: 2020 2020 224e 6f72 6d61 6c22 2929 0a20      "Normal")). 
-0001ae40: 2020 2020 2020 2073 7461 636b 2e61 7070         stack.app
-0001ae50: 656e 6428 2822 4361 6c63 4f70 222c 2022  end(("CalcOp", "
-0001ae60: 2a22 2929 0a20 2020 2020 2020 2072 6574  *")).        ret
-0001ae70: 7572 6e20 4361 6c63 4f62 6a65 6374 2873  urn CalcObject(s
-0001ae80: 7461 636b 2c20 7365 6c66 2e73 6574 7570  tack, self.setup
-0001ae90: 290a 0a20 2020 2064 6566 2074 616e 6765  )..    def tange
-0001aea0: 6e74 3273 7572 6661 6365 2873 656c 662c  nt2surface(self,
-0001aeb0: 206e 616d 6529 3a0a 2020 2020 2020 2020   name):.        
-0001aec0: 2727 2720 7265 7475 726e 2074 6865 2070  ''' return the p
-0001aed0: 6172 7420 7461 6e67 656e 7420 746f 2073  art tangent to s
-0001aee0: 7572 6661 6365 2e0a 2020 2020 2020 2020  urface..        
-0001aef0: 2020 2020 436f 6d70 6c65 7820 5665 6374      Complex Vect
-0001af00: 6f72 2e20 2727 270a 2020 2020 2020 2020  or. '''.        
-0001af10: 7374 6163 6b20 3d20 7365 6c66 2e73 7461  stack = self.sta
-0001af20: 636b 202b 205b 2822 456e 7465 7253 7572  ck + [("EnterSur
-0001af30: 6622 2c20 6e61 6d65 292c 0a20 2020 2020  f", name),.     
-0001af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af50: 2020 2020 2020 2020 2020 2028 2243 616c             ("Cal
-0001af60: 634f 7022 2c20 2020 2022 4e6f 726d 616c  cOp",    "Normal
-0001af70: 2229 5d0a 2020 2020 2020 2020 7374 6163  ")].        stac
-0001af80: 6b2e 6170 7065 6e64 2828 2243 616c 634f  k.append(("CalcO
-0001af90: 7022 2c20 2244 6f74 2229 290a 2020 2020  p", "Dot")).    
-0001afa0: 2020 2020 7374 6163 6b2e 6170 7065 6e64      stack.append
-0001afb0: 2828 2245 6e74 6572 5375 7266 222c 206e  (("EnterSurf", n
-0001afc0: 616d 6529 290a 2020 2020 2020 2020 7374  ame)).        st
-0001afd0: 6163 6b2e 6170 7065 6e64 2828 2243 616c  ack.append(("Cal
-0001afe0: 634f 7022 2c20 2020 2022 4e6f 726d 616c  cOp",    "Normal
-0001aff0: 2229 290a 2020 2020 2020 2020 7374 6163  ")).        stac
-0001b000: 6b2e 6170 7065 6e64 2828 2243 616c 634f  k.append(("CalcO
-0001b010: 7022 2c20 222a 2229 290a 2020 2020 2020  p", "*")).      
-0001b020: 2020 7374 6163 6b20 3d20 7365 6c66 2e73    stack = self.s
-0001b030: 7461 636b 202b 2073 7461 636b 0a20 2020  tack + stack.   
-0001b040: 2020 2020 2073 7461 636b 2e61 7070 656e       stack.appen
-0001b050: 6428 2822 4361 6c63 4f70 222c 2022 2d22  d(("CalcOp", "-"
-0001b060: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-0001b070: 6e20 4361 6c63 4f62 6a65 6374 2873 7461  n CalcObject(sta
-0001b080: 636b 2c20 7365 6c66 2e73 6574 7570 290a  ck, self.setup).
-0001b090: 0a20 2020 2064 6566 2069 6e74 6567 7261  .    def integra
-0001b0a0: 7465 5f6c 696e 655f 7461 6e67 656e 7428  te_line_tangent(
-0001b0b0: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
-0001b0c0: 2020 2020 2027 2727 2069 6e74 6567 7261       ''' integra
-0001b0d0: 7465 206c 696e 6520 7461 6e67 656e 7420  te line tangent 
-0001b0e0: 746f 2076 6563 746f 7220 6578 7072 6573  to vector expres
-0001b0f0: 7369 6f6e 205c 6e0a 2020 2020 2020 2020  sion \n.        
-0001b100: 2020 2020 6e61 6d65 203d 206f 6620 6c69      name = of li
-0001b110: 6e65 2074 6f20 696e 7465 6772 6174 6520  ne to integrate 
-0001b120: 6f76 6572 2027 2727 0a20 2020 2020 2020  over '''.       
-0001b130: 2073 656c 662e 7374 6163 6b20 3d20 7365   self.stack = se
-0001b140: 6c66 2e73 7461 636b 202b 205b 2822 456e  lf.stack + [("En
-0001b150: 7465 724c 696e 6522 2c20 6e61 6d65 292c  terLine", name),
-0001b160: 2028 2243 616c 634f 7022 2c20 2254 616e   ("CalcOp", "Tan
-0001b170: 6765 6e74 2229 2c0a 2020 2020 2020 2020  gent"),.        
-0001b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b190: 2020 2020 2020 2020 2020 2028 2243 616c             ("Cal
-0001b1a0: 634f 7022 2c20 2244 6f74 2229 5d0a 2020  cOp", "Dot")].  
-0001b1b0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001b1c0: 662e 696e 7465 6772 6174 655f 6c69 6e65  f.integrate_line
-0001b1d0: 286e 616d 6529 0a0a 2020 2020 6465 6620  (name)..    def 
-0001b1e0: 6c69 6e65 5f74 616e 6765 6e74 5f63 6f6f  line_tangent_coo
-0001b1f0: 7228 7365 6c66 2c20 6e61 6d65 2c20 636f  r(self, name, co
-0001b200: 6f72 6469 6e61 7465 293a 0a20 2020 2020  ordinate):.     
-0001b210: 2020 2027 2727 2069 6e74 6567 7261 7465     ''' integrate
-0001b220: 206c 696e 6520 7461 6e67 656e 7420 746f   line tangent to
-0001b230: 2076 6563 746f 7220 6578 7072 6573 7369   vector expressi
-0001b240: 6f6e 205c 6e0a 2020 2020 2020 2020 2020  on \n.          
-0001b250: 2020 6e61 6d65 203d 206f 6620 6c69 6e65    name = of line
-0001b260: 2074 6f20 696e 7465 6772 6174 6520 6f76   to integrate ov
-0001b270: 6572 2027 2727 0a20 2020 2020 2020 2069  er '''.        i
-0001b280: 6620 636f 6f72 6469 6e61 7465 206e 6f74  f coordinate not
-0001b290: 2069 6e20 5b27 5827 2c20 2759 272c 2027   in ['X', 'Y', '
-0001b2a0: 5a27 5d3a 0a20 2020 2020 2020 2020 2020  Z']:.           
-0001b2b0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0001b2c0: 720a 2020 2020 2020 2020 7365 6c66 2e73  r.        self.s
-0001b2d0: 7461 636b 203d 2073 656c 662e 7374 6163  tack = self.stac
-0001b2e0: 6b20 2b20 5b28 2245 6e74 6572 4c69 6e65  k + [("EnterLine
-0001b2f0: 222c 206e 616d 6529 2c20 2822 4361 6c63  ", name), ("Calc
-0001b300: 4f70 222c 2022 5461 6e67 656e 7422 292c  Op", "Tangent"),
-0001b310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b330: 2020 2020 2822 4361 6c63 4f70 222c 2022      ("CalcOp", "
-0001b340: 5363 616c 6172 2220 2b20 636f 6f72 6469  Scalar" + coordi
-0001b350: 6e61 7465 295d 0a20 2020 2020 2020 2072  nate)].        r
-0001b360: 6574 7572 6e20 7365 6c66 2e69 6e74 6567  eturn self.integ
-0001b370: 7261 7465 5f6c 696e 6528 6e61 6d65 290a  rate_line(name).
-0001b380: 0a20 2020 2064 6566 2069 6e74 6567 7261  .    def integra
-0001b390: 7465 5f73 7572 6628 7365 6c66 2c20 6e61  te_surf(self, na
-0001b3a0: 6d65 3d22 416c 6c4f 626a 6563 7473 2229  me="AllObjects")
-0001b3b0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0001b3c0: 2073 656c 662e 5f69 6e74 6567 7261 7465   self._integrate
-0001b3d0: 286e 616d 652c 2022 456e 7465 7253 7572  (name, "EnterSur
-0001b3e0: 6622 290a 0a20 2020 2064 6566 2069 6e74  f")..    def int
-0001b3f0: 6567 7261 7465 5f76 6f6c 2873 656c 662c  egrate_vol(self,
-0001b400: 206e 616d 653d 2241 6c6c 4f62 6a65 6374   name="AllObject
-0001b410: 7322 293a 0a20 2020 2020 2020 2072 6574  s"):.        ret
-0001b420: 7572 6e20 7365 6c66 2e5f 696e 7465 6772  urn self._integr
-0001b430: 6174 6528 6e61 6d65 2c20 2245 6e74 6572  ate(name, "Enter
-0001b440: 566f 6c22 290a 0a20 2020 2064 6566 206d  Vol")..    def m
-0001b450: 6178 696d 756d 5f76 6f6c 2873 656c 662c  aximum_vol(self,
-0001b460: 206e 616d 653d 2741 6c6c 4f62 6a65 6374   name='AllObject
-0001b470: 7327 293a 0a20 2020 2020 2020 2072 6574  s'):.        ret
-0001b480: 7572 6e20 7365 6c66 2e5f 6d61 7869 6d75  urn self._maximu
-0001b490: 6d28 6e61 6d65 2c20 2745 6e74 6572 566f  m(name, 'EnterVo
-0001b4a0: 6c27 290a 0a20 2020 2064 6566 2074 696d  l')..    def tim
-0001b4b0: 6573 5f65 7073 2873 656c 6629 3a0a 2020  es_eps(self):.  
-0001b4c0: 2020 2020 2020 7374 6163 6b20 3d20 7365        stack = se
-0001b4d0: 6c66 2e73 7461 636b 202b 205b 2822 436c  lf.stack + [("Cl
-0001b4e0: 634d 6174 6572 6961 6c22 2c20 2822 5065  cMaterial", ("Pe
-0001b4f0: 726d 6974 7469 7669 7479 2028 6570 7369  rmittivity (epsi
-0001b500: 2922 2c20 226d 756c 7422 2929 5d0a 2020  )", "mult"))].  
-0001b510: 2020 2020 2020 7265 7475 726e 2043 616c        return Cal
-0001b520: 634f 626a 6563 7428 7374 6163 6b2c 2073  cObject(stack, s
-0001b530: 656c 662e 7365 7475 7029 0a0a 2020 2020  elf.setup)..    
-0001b540: 6465 6620 7469 6d65 735f 6d75 2873 656c  def times_mu(sel
-0001b550: 6629 3a0a 2020 2020 2020 2020 7374 6163  f):.        stac
-0001b560: 6b20 3d20 7365 6c66 2e73 7461 636b 202b  k = self.stack +
-0001b570: 205b 2822 436c 634d 6174 6572 6961 6c22   [("ClcMaterial"
-0001b580: 2c20 2822 5065 726d 6561 6269 6c69 7479  , ("Permeability
-0001b590: 2028 6d75 2922 2c20 226d 756c 7422 2929   (mu)", "mult"))
-0001b5a0: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-0001b5b0: 2043 616c 634f 626a 6563 7428 7374 6163   CalcObject(stac
-0001b5c0: 6b2c 2073 656c 662e 7365 7475 7029 0a0a  k, self.setup)..
-0001b5d0: 2020 2020 6465 6620 7772 6974 655f 7374      def write_st
-0001b5e0: 6163 6b28 7365 6c66 293a 0a20 2020 2020  ack(self):.     
-0001b5f0: 2020 2066 6f72 2066 6e2c 2061 7267 2069     for fn, arg i
-0001b600: 6e20 7365 6c66 2e73 7461 636b 3a0a 2020  n self.stack:.  
-0001b610: 2020 2020 2020 2020 2020 6966 206e 702e            if np.
-0001b620: 7369 7a65 2861 7267 2920 3e20 3120 616e  size(arg) > 1 an
-0001b630: 6420 666e 206e 6f74 2069 6e20 5b27 456e  d fn not in ['En
-0001b640: 7465 7256 6563 746f 7227 5d3a 0a20 2020  terVector']:.   
-0001b650: 2020 2020 2020 2020 2020 2020 2067 6574               get
-0001b660: 6174 7472 2873 656c 662e 6361 6c63 5f6d  attr(self.calc_m
-0001b670: 6f64 756c 652c 2066 6e29 282a 6172 6729  odule, fn)(*arg)
-0001b680: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001b690: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001b6a0: 2020 2067 6574 6174 7472 2873 656c 662e     getattr(self.
-0001b6b0: 6361 6c63 5f6d 6f64 756c 652c 2066 6e29  calc_module, fn)
-0001b6c0: 2861 7267 290a 0a20 2020 2064 6566 2073  (arg)..    def s
-0001b6d0: 6176 655f 6173 2873 656c 662c 206e 616d  ave_as(self, nam
-0001b6e0: 6529 3a0a 2020 2020 2020 2020 2222 2269  e):.        """i
-0001b6f0: 6620 7468 6520 6f62 6a65 6374 2061 6c72  f the object alr
-0001b700: 6561 6479 2065 7869 7374 732c 2074 7279  eady exists, try
-0001b710: 2063 6c65 6172 696e 6720 796f 7572 0a20   clearing your. 
-0001b720: 2020 2020 2020 206e 616d 6564 2065 7870         named exp
-0001b730: 7265 7373 696f 6e73 2066 6972 7374 2077  ressions first w
-0001b740: 6974 6820 6669 656c 6473 2e63 6c65 6172  ith fields.clear
-0001b750: 5f6e 616d 6564 5f65 7870 7265 7373 696f  _named_expressio
-0001b760: 6e73 2222 220a 2020 2020 2020 2020 7365  ns""".        se
-0001b770: 6c66 2e77 7269 7465 5f73 7461 636b 2829  lf.write_stack()
-0001b780: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
-0001b790: 6c63 5f6d 6f64 756c 652e 4164 644e 616d  lc_module.AddNam
-0001b7a0: 6564 4578 7072 286e 616d 6529 0a20 2020  edExpr(name).   
-0001b7b0: 2020 2020 2072 6574 7572 6e20 4e61 6d65       return Name
-0001b7c0: 6443 616c 634f 626a 6563 7428 6e61 6d65  dCalcObject(name
-0001b7d0: 2c20 7365 6c66 2e73 6574 7570 290a 0a20  , self.setup).. 
-0001b7e0: 2020 2064 6566 2065 7661 6c75 6174 6528     def evaluate(
-0001b7f0: 7365 6c66 2c20 7068 6173 653d 302c 206c  self, phase=0, l
-0001b800: 763d 4e6f 6e65 2c20 7072 696e 745f 6465  v=None, print_de
-0001b810: 6275 673d 4661 6c73 6529 3a20 2023 202c  bug=False):  # ,
-0001b820: 206e 5f6d 6f64 653d 3129 3a0a 2020 2020   n_mode=1):.    
-0001b830: 2020 2020 7365 6c66 2e77 7269 7465 5f73      self.write_s
-0001b840: 7461 636b 2829 0a20 2020 2020 2020 2069  tack().        i
-0001b850: 6620 7072 696e 745f 6465 6275 673a 0a20  f print_debug:. 
-0001b860: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0001b870: 2827 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ('--------------
-0001b880: 2d2d 2d2d 2d2d 2d27 290a 2020 2020 2020  -------').      
-0001b890: 2020 2020 2020 7072 696e 7428 2777 7269        print('wri
-0001b8a0: 7469 6e67 2074 6f20 7374 6163 6b3a 204f  ting to stack: O
-0001b8b0: 4b27 290a 2020 2020 2020 2020 2020 2020  K').            
-0001b8c0: 7072 696e 7428 272d 2d2d 2d2d 2d2d 2d2d  print('---------
-0001b8d0: 2d2d 2d2d 2d2d 2d2d 2729 0a20 2020 2020  --------').     
-0001b8e0: 2020 2023 7365 6c66 2e63 616c 635f 6d6f     #self.calc_mo
-0001b8f0: 6475 6c65 2e73 6574 5f6d 6f64 6528 6e5f  dule.set_mode(n_
-0001b900: 6d6f 6465 2c20 3029 0a20 2020 2020 2020  mode, 0).       
-0001b910: 2073 6574 7570 5f6e 616d 6520 3d20 7365   setup_name = se
-0001b920: 6c66 2e73 6574 7570 2e73 6f6c 7574 696f  lf.setup.solutio
-0001b930: 6e5f 6e61 6d65 0a0a 2020 2020 2020 2020  n_name..        
-0001b940: 6966 206c 7620 6973 206e 6f74 204e 6f6e  if lv is not Non
-0001b950: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
-0001b960: 7267 7320 3d20 6c76 0a20 2020 2020 2020  rgs = lv.       
-0001b970: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001b980: 2020 2061 7267 7320 3d20 5b5d 0a0a 2020     args = []..  
-0001b990: 2020 2020 2020 6172 6773 2e61 7070 656e        args.appen
-0001b9a0: 6428 2250 6861 7365 3a3d 2229 0a20 2020  d("Phase:=").   
-0001b9b0: 2020 2020 2061 7267 732e 6170 7065 6e64       args.append
-0001b9c0: 2873 7472 2869 6e74 2870 6861 7365 2929  (str(int(phase))
-0001b9d0: 202b 2022 6465 6722 290a 0a20 2020 2020   + "deg")..     
-0001b9e0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0001b9f0: 2873 656c 662e 7365 7475 702c 2048 6673  (self.setup, Hfs
-0001ba00: 7344 4d53 6574 7570 293a 0a20 2020 2020  sDMSetup):.     
-0001ba10: 2020 2020 2020 2061 7267 732e 6578 7465         args.exte
-0001ba20: 6e64 285b 2246 7265 713a 3d22 2c20 7365  nd(["Freq:=", se
-0001ba30: 6c66 2e73 6574 7570 2e73 6f6c 7574 696f  lf.setup.solutio
-0001ba40: 6e5f 6672 6571 5d29 0a0a 2020 2020 2020  n_freq])..      
-0001ba50: 2020 7365 6c66 2e63 616c 635f 6d6f 6475    self.calc_modu
-0001ba60: 6c65 2e43 6c63 4576 616c 2873 6574 7570  le.ClcEval(setup
-0001ba70: 5f6e 616d 652c 2061 7267 7329 0a20 2020  _name, args).   
-0001ba80: 2020 2020 2072 6574 7572 6e20 666c 6f61       return floa
-0001ba90: 7428 7365 6c66 2e63 616c 635f 6d6f 6475  t(self.calc_modu
-0001baa0: 6c65 2e47 6574 546f 7045 6e74 7279 5661  le.GetTopEntryVa
-0001bab0: 6c75 6528 7365 7475 705f 6e61 6d65 2c20  lue(setup_name, 
-0001bac0: 6172 6773 295b 305d 290a 0a0a 636c 6173  args)[0])...clas
-0001bad0: 7320 4e61 6d65 6443 616c 634f 626a 6563  s NamedCalcObjec
-0001bae0: 7428 4361 6c63 4f62 6a65 6374 293a 0a20  t(CalcObject):. 
-0001baf0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-0001bb00: 7365 6c66 2c20 6e61 6d65 2c20 7365 7475  self, name, setu
-0001bb10: 7029 3a0a 2020 2020 2020 2020 7365 6c66  p):.        self
-0001bb20: 2e6e 616d 6520 3d20 6e61 6d65 0a20 2020  .name = name.   
-0001bb30: 2020 2020 2073 7461 636b 203d 205b 2822       stack = [("
-0001bb40: 436f 7079 4e61 6d65 6445 7870 7254 6f53  CopyNamedExprToS
-0001bb50: 7461 636b 222c 206e 616d 6529 5d0a 2020  tack", name)].  
-0001bb60: 2020 2020 2020 7375 7065 7228 4e61 6d65        super(Name
-0001bb70: 6443 616c 634f 626a 6563 742c 2073 656c  dCalcObject, sel
-0001bb80: 6629 2e5f 5f69 6e69 745f 5f28 7374 6163  f).__init__(stac
-0001bb90: 6b2c 2073 6574 7570 290a 0a0a 636c 6173  k, setup)...clas
-0001bba0: 7320 436f 6e73 7461 6e74 4361 6c63 4f62  s ConstantCalcOb
-0001bbb0: 6a65 6374 2843 616c 634f 626a 6563 7429  ject(CalcObject)
-0001bbc0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0001bbd0: 5f5f 2873 656c 662c 206e 756d 2c20 7365  __(self, num, se
-0001bbe0: 7475 7029 3a0a 2020 2020 2020 2020 7374  tup):.        st
-0001bbf0: 6163 6b20 3d20 5b28 2245 6e74 6572 5363  ack = [("EnterSc
-0001bc00: 616c 6172 222c 206e 756d 295d 0a20 2020  alar", num)].   
-0001bc10: 2020 2020 2073 7570 6572 2843 6f6e 7374       super(Const
-0001bc20: 616e 7443 616c 634f 626a 6563 742c 2073  antCalcObject, s
-0001bc30: 656c 6629 2e5f 5f69 6e69 745f 5f28 7374  elf).__init__(st
-0001bc40: 6163 6b2c 2073 6574 7570 290a 0a0a 636c  ack, setup)...cl
-0001bc50: 6173 7320 436f 6e73 7461 6e74 5665 6343  ass ConstantVecC
-0001bc60: 616c 634f 626a 6563 7428 4361 6c63 4f62  alcObject(CalcOb
-0001bc70: 6a65 6374 293a 0a20 2020 2064 6566 205f  ject):.    def _
-0001bc80: 5f69 6e69 745f 5f28 7365 6c66 2c20 7665  _init__(self, ve
-0001bc90: 632c 2073 6574 7570 293a 0a20 2020 2020  c, setup):.     
-0001bca0: 2020 2073 7461 636b 203d 205b 2822 456e     stack = [("En
-0001bcb0: 7465 7256 6563 746f 7222 2c20 7665 6329  terVector", vec)
-0001bcc0: 5d0a 2020 2020 2020 2020 7375 7065 7228  ].        super(
-0001bcd0: 436f 6e73 7461 6e74 5665 6343 616c 634f  ConstantVecCalcO
-0001bce0: 626a 6563 742c 2073 656c 6629 2e5f 5f69  bject, self).__i
-0001bcf0: 6e69 745f 5f28 7374 6163 6b2c 2073 6574  nit__(stack, set
-0001bd00: 7570 290a 0a0a 6465 6620 6765 745f 6163  up)...def get_ac
-0001bd10: 7469 7665 5f70 726f 6a65 6374 2829 3a0a  tive_project():.
-0001bd20: 2020 2020 2727 2720 4966 2079 6f75 2073      ''' If you s
-0001bd30: 6565 2074 6865 2065 7272 6f72 3a0a 2020  ee the error:.  
-0001bd40: 2020 2020 2020 2254 6865 2072 6571 7565        "The reque
-0001bd50: 7374 6564 206f 7065 7261 7469 6f6e 2072  sted operation r
-0001bd60: 6571 7569 7265 7320 656c 6576 6174 696f  equires elevatio
-0001bd70: 6e2e 220a 2020 2020 2020 2020 7468 656e  n.".        then
-0001bd80: 2079 6f75 206e 6565 6420 746f 2072 756e   you need to run
-0001bd90: 2079 6f75 7220 7079 7468 6f6e 2061 7320   your python as 
-0001bda0: 616e 2061 646d 696e 2e0a 2020 2020 2727  an admin..    ''
-0001bdb0: 270a 2020 2020 696d 706f 7274 2063 7479  '.    import cty
-0001bdc0: 7065 730a 2020 2020 696d 706f 7274 206f  pes.    import o
-0001bdd0: 730a 2020 2020 7472 793a 0a20 2020 2020  s.    try:.     
-0001bde0: 2020 2069 735f 6164 6d69 6e20 3d20 6f73     is_admin = os
-0001bdf0: 2e67 6574 7569 6428 2920 3d3d 2030 0a20  .getuid() == 0. 
-0001be00: 2020 2065 7863 6570 7420 4174 7472 6962     except Attrib
-0001be10: 7574 6545 7272 6f72 3a0a 2020 2020 2020  uteError:.      
-0001be20: 2020 6973 5f61 646d 696e 203d 2063 7479    is_admin = cty
-0001be30: 7065 732e 7769 6e64 6c6c 2e73 6865 6c6c  pes.windll.shell
-0001be40: 3332 2e49 7355 7365 7241 6e41 646d 696e  32.IsUserAnAdmin
-0001be50: 2829 2021 3d20 300a 2020 2020 6966 206e  () != 0.    if n
-0001be60: 6f74 2069 735f 6164 6d69 6e3a 0a20 2020  ot is_admin:.   
-0001be70: 2020 2020 2070 7269 6e74 2827 5c30 3333       print('\033
-0001be80: 5b39 336d 2057 4152 4e49 4e47 3a20 796f  [93m WARNING: yo
-0001be90: 7520 6172 6520 6e6f 7420 7275 6e6e 696e  u are not runnin
-0001bea0: 6720 6173 2061 6e20 6164 6d69 6e21 205c  g as an admin! \
-0001beb0: 0a20 2020 2020 2020 2020 2020 2059 6f75  .            You
-0001bec0: 206e 6565 6420 746f 2072 756e 2061 7320   need to run as 
-0001bed0: 616e 2061 646d 696e 2e20 596f 7520 7769  an admin. You wi
-0001bee0: 6c6c 2070 726f 6261 626c 7920 6765 7420  ll probably get 
-0001bef0: 616e 2065 7272 6f72 206e 6578 742e 5c0a  an error next.\.
-0001bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf10: 205c 3033 335b 306d 2729 0a0a 2020 2020   \033[0m')..    
-0001bf20: 6170 7020 3d20 4866 7373 4170 7028 290a  app = HfssApp().
-0001bf30: 2020 2020 6465 736b 746f 7020 3d20 6170      desktop = ap
-0001bf40: 702e 6765 745f 6170 705f 6465 736b 746f  p.get_app_deskto
-0001bf50: 7028 290a 2020 2020 7265 7475 726e 2064  p().    return d
-0001bf60: 6573 6b74 6f70 2e67 6574 5f61 6374 6976  esktop.get_activ
-0001bf70: 655f 7072 6f6a 6563 7428 290a 0a0a 6465  e_project()...de
-0001bf80: 6620 6765 745f 6163 7469 7665 5f64 6573  f get_active_des
-0001bf90: 6967 6e28 293a 0a20 2020 2070 726f 6a65  ign():.    proje
-0001bfa0: 6374 203d 2067 6574 5f61 6374 6976 655f  ct = get_active_
-0001bfb0: 7072 6f6a 6563 7428 290a 2020 2020 7265  project().    re
-0001bfc0: 7475 726e 2070 726f 6a65 6374 2e67 6574  turn project.get
-0001bfd0: 5f61 6374 6976 655f 6465 7369 676e 2829  _active_design()
-0001bfe0: 0a0a 0a64 6566 2067 6574 5f72 6570 6f72  ...def get_repor
-0001bff0: 745f 6172 7261 7973 286e 616d 653a 2073  t_arrays(name: s
-0001c000: 7472 293a 0a20 2020 2064 203d 2067 6574  tr):.    d = get
-0001c010: 5f61 6374 6976 655f 6465 7369 676e 2829  _active_design()
-0001c020: 0a20 2020 2072 203d 2048 6673 7352 6570  .    r = HfssRep
-0001c030: 6f72 7428 642c 206e 616d 6529 0a20 2020  ort(d, name).   
-0001c040: 2072 6574 7572 6e20 722e 6765 745f 6172   return r.get_ar
-0001c050: 7261 7973 2829 0a0a 0a64 6566 206c 6f61  rays()...def loa
-0001c060: 645f 616e 7379 735f 7072 6f6a 6563 7428  d_ansys_project(
-0001c070: 7072 6f6a 5f6e 616d 653a 2073 7472 2c0a  proj_name: str,.
-0001c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c090: 2020 2020 2020 2070 726f 6a65 6374 5f70         project_p
-0001c0a0: 6174 683a 2073 7472 203d 204e 6f6e 652c  ath: str = None,
-0001c0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c0c0: 2020 2020 2020 2020 6578 7465 6e73 696f          extensio
-0001c0d0: 6e3a 2073 7472 203d 2027 2e61 6564 7427  n: str = '.aedt'
-0001c0e0: 293a 0a20 2020 2027 2727 0a20 2020 2055  ):.    '''.    U
-0001c0f0: 7469 6c69 7479 2066 756e 6374 696f 6e20  tility function 
-0001c100: 746f 206c 6f61 6420 616e 2041 6e73 7973  to load an Ansys
-0001c110: 2070 726f 6a65 6374 2e0a 0a20 2020 2041   project...    A
-0001c120: 7267 733a 0a20 2020 2020 2020 2070 726f  rgs:.        pro
-0001c130: 6a5f 6e61 6d65 203a 204e 6f6e 6520 202d  j_name : None  -
-0001c140: 2d3e 2067 6574 2061 6374 6976 652e 2028  -> get active. (
-0001c150: 6d61 6b65 2073 7572 6520 3220 7275 6e20  make sure 2 run 
-0001c160: 6173 2061 646d 696e 290a 2020 2020 2020  as admin).      
-0001c170: 2020 6578 7465 6e73 696f 6e20 3a20 6061    extension : `a
-0001c180: 6564 7460 2069 7320 666f 7220 3230 3136  edt` is for 2016
-0001c190: 2076 6572 7369 6f6e 2061 6e64 206e 6577   version and new
-0001c1a0: 6572 0a20 2020 2027 2727 0a20 2020 2069  er.    '''.    i
-0001c1b0: 6620 7072 6f6a 6563 745f 7061 7468 3a0a  f project_path:.
-0001c1c0: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
-0001c1d0: 7420 736c 6173 6865 7320 636f 7272 6563  t slashes correc
-0001c1e0: 746c 7920 666f 7220 7379 7374 656d 0a20  tly for system. 
-0001c1f0: 2020 2020 2020 2070 726f 6a65 6374 5f70         project_p
-0001c200: 6174 6820 3d20 5061 7468 2870 726f 6a65  ath = Path(proje
-0001c210: 6374 5f70 6174 6829 0a0a 2020 2020 2020  ct_path)..      
-0001c220: 2020 2320 4368 6563 6b73 0a20 2020 2020    # Checks.     
-0001c230: 2020 2061 7373 6572 7420 7072 6f6a 6563     assert projec
-0001c240: 745f 7061 7468 2e69 735f 6469 7228 0a20  t_path.is_dir(. 
-0001c250: 2020 2020 2020 2029 2c20 2245 5252 4f52         ), "ERROR
-0001c260: 2120 7072 6f6a 6563 745f 7061 7468 2069  ! project_path i
-0001c270: 7320 6e6f 7420 6120 7661 6c69 6420 6469  s not a valid di
-0001c280: 7265 6374 6f72 7920 5c4e 7b6c 6f75 646c  rectory \N{loudl
-0001c290: 7920 6372 7969 6e67 2066 6163 657d 2e5c  y crying face}.\
-0001c2a0: 0a20 2020 2020 2020 2020 2020 2043 6865  .            Che
-0001c2b0: 636b 2074 6865 2070 6174 682c 2061 6e64  ck the path, and
-0001c2c0: 2065 7370 6563 6961 6c6c 7920 5c5c 2063   especially \\ c
-0001c2d0: 6861 7261 6374 6572 732e 220a 0a20 2020  haracters."..   
-0001c2e0: 2020 2020 2070 726f 6a65 6374 5f70 6174       project_pat
-0001c2f0: 6820 2f3d 2070 726f 6a65 6374 5f70 6174  h /= project_pat
-0001c300: 6820 2f20 5061 7468 2870 726f 6a5f 6e61  h / Path(proj_na
-0001c310: 6d65 202b 2065 7874 656e 7369 6f6e 290a  me + extension).
-0001c320: 0a20 2020 2020 2020 2069 6620 2870 726f  .        if (pro
-0001c330: 6a65 6374 5f70 6174 6829 2e69 735f 6669  ject_path).is_fi
-0001c340: 6c65 2829 3a0a 2020 2020 2020 2020 2020  le():.          
-0001c350: 2020 6c6f 6767 6572 2e69 6e66 6f28 275c    logger.info('\
-0001c360: 7446 696c 6520 7061 7468 2074 6f20 4846  tFile path to HF
-0001c370: 5353 2070 726f 6a65 6374 2066 6f75 6e64  SS project found
-0001c380: 2e27 290a 2020 2020 2020 2020 656c 7365  .').        else
-0001c390: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0001c3a0: 6973 6520 4578 6365 7074 696f 6e28 0a20  ise Exception(. 
-0001c3b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001c3c0: 4552 524f 5221 2056 616c 6964 2064 6972  ERROR! Valid dir
-0001c3d0: 6563 746f 7279 2c20 6275 7420 696e 7661  ectory, but inva
-0001c3e0: 6c69 6420 7072 6f6a 6563 7420 6669 6c65  lid project file
-0001c3f0: 6e61 6d65 2e20 5c4e 7b6c 6f75 646c 7920  name. \N{loudly 
-0001c400: 6372 7969 6e67 2066 6163 657d 204e 6f74  crying face} Not
-0001c410: 2066 6f75 6e64 215c 0a20 2020 2020 2020   found!\.       
-0001c420: 2020 2020 2020 2020 2020 2020 2020 506c                Pl
-0001c430: 6561 7365 2063 6865 636b 2079 6f75 7220  ease check your 
-0001c440: 6669 6c65 6e61 6d65 2e5c 6e25 735c 6e22  filename.\n%s\n"
-0001c450: 2025 2070 726f 6a65 6374 5f70 6174 6829   % project_path)
-0001c460: 0a0a 2020 2020 2020 2020 6966 2028 7072  ..        if (pr
-0001c470: 6f6a 6563 745f 7061 7468 202f 2027 2e6c  oject_path / '.l
-0001c480: 6f63 6b27 292e 6973 5f66 696c 6528 293a  ock').is_file():
-0001c490: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-0001c4a0: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
-0001c4b0: 2020 2020 2020 2020 2020 2020 2027 5c74               '\t
-0001c4c0: 5c74 4669 6c65 2069 7320 6c6f 636b 6564  \tFile is locked
-0001c4d0: 2e20 5c4e 7b66 6561 7266 756c 2066 6163  . \N{fearful fac
-0001c4e0: 657d 2049 6620 636f 6e6e 6563 7469 6f6e  e} If connection
-0001c4f0: 2066 6169 6c73 2c20 6465 6c65 7465 2074   fails, delete t
-0001c500: 6865 202e 6c6f 636b 2066 696c 652e 270a  he .lock file.'.
-0001c510: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0001c520: 2020 2061 7070 203d 2048 6673 7341 7070     app = HfssApp
-0001c530: 2829 0a20 2020 206c 6f67 6765 722e 696e  ().    logger.in
-0001c540: 666f 2822 5c74 4f70 656e 6564 2041 6e73  fo("\tOpened Ans
-0001c550: 7973 2041 7070 2229 0a0a 2020 2020 6465  ys App")..    de
-0001c560: 736b 746f 7020 3d20 6170 702e 6765 745f  sktop = app.get_
-0001c570: 6170 705f 6465 736b 746f 7028 290a 2020  app_desktop().  
-0001c580: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
-0001c590: 5c74 4f70 656e 6564 2041 6e73 7973 2044  \tOpened Ansys D
-0001c5a0: 6573 6b74 6f70 2076 7b64 6573 6b74 6f70  esktop v{desktop
-0001c5b0: 2e67 6574 5f76 6572 7369 6f6e 2829 7d22  .get_version()}"
-0001c5c0: 290a 2020 2020 236c 6f67 6765 722e 6465  ).    #logger.de
-0001c5d0: 6275 6728 6622 5c74 4f70 656e 2070 726f  bug(f"\tOpen pro
-0001c5e0: 6a65 6374 733a 207b 6465 736b 746f 702e  jects: {desktop.
-0001c5f0: 6765 745f 7072 6f6a 6563 745f 6e61 6d65  get_project_name
-0001c600: 7328 297d 2229 0a0a 2020 2020 6966 2070  s()}")..    if p
-0001c610: 726f 6a5f 6e61 6d65 2069 7320 6e6f 7420  roj_name is not 
-0001c620: 4e6f 6e65 3a0a 2020 2020 2020 2020 6966  None:.        if
-0001c630: 2070 726f 6a5f 6e61 6d65 2069 6e20 6465   proj_name in de
-0001c640: 736b 746f 702e 6765 745f 7072 6f6a 6563  sktop.get_projec
-0001c650: 745f 6e61 6d65 7328 293a 0a20 2020 2020  t_names():.     
-0001c660: 2020 2020 2020 2064 6573 6b74 6f70 2e73         desktop.s
-0001c670: 6574 5f61 6374 6976 655f 7072 6f6a 6563  et_active_projec
-0001c680: 7428 7072 6f6a 5f6e 616d 6529 0a20 2020  t(proj_name).   
-0001c690: 2020 2020 2020 2020 2070 726f 6a65 6374           project
-0001c6a0: 203d 2064 6573 6b74 6f70 2e67 6574 5f61   = desktop.get_a
-0001c6b0: 6374 6976 655f 7072 6f6a 6563 7428 290a  ctive_project().
-0001c6c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001c6d0: 2020 2020 2020 2020 2020 7072 6f6a 6563            projec
-0001c6e0: 7420 3d20 6465 736b 746f 702e 6f70 656e  t = desktop.open
-0001c6f0: 5f70 726f 6a65 6374 2873 7472 2870 726f  _project(str(pro
-0001c700: 6a65 6374 5f70 6174 6829 290a 2020 2020  ject_path)).    
-0001c710: 656c 7365 3a0a 2020 2020 2020 2020 7072  else:.        pr
-0001c720: 6f6a 6563 7473 5f69 6e5f 6170 7020 3d20  ojects_in_app = 
-0001c730: 6465 736b 746f 702e 6765 745f 7072 6f6a  desktop.get_proj
-0001c740: 6563 7473 2829 0a20 2020 2020 2020 2069  ects().        i
-0001c750: 6620 7072 6f6a 6563 7473 5f69 6e5f 6170  f projects_in_ap
-0001c760: 703a 0a20 2020 2020 2020 2020 2020 2070  p:.            p
-0001c770: 726f 6a65 6374 203d 2064 6573 6b74 6f70  roject = desktop
-0001c780: 2e67 6574 5f61 6374 6976 655f 7072 6f6a  .get_active_proj
-0001c790: 6563 7428 290a 2020 2020 2020 2020 656c  ect().        el
-0001c7a0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001c7b0: 7072 6f6a 6563 7420 3d20 4e6f 6e65 0a0a  project = None..
-0001c7c0: 2020 2020 6966 2070 726f 6a65 6374 3a0a      if project:.
-0001c7d0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-0001c7e0: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-0001c7f0: 2066 225c 744f 7065 6e65 6420 416e 7379   f"\tOpened Ansy
-0001c800: 7320 5072 6f6a 6563 745c 6e5c 7446 6f6c  s Project\n\tFol
-0001c810: 6465 723a 2020 2020 7b70 726f 6a65 6374  der:    {project
-0001c820: 2e67 6574 5f70 6174 6828 297d 5c6e 5c74  .get_path()}\n\t
-0001c830: 5072 6f6a 6563 743a 2020 207b 7072 6f6a  Project:   {proj
-0001c840: 6563 742e 6e61 6d65 7d22 0a20 2020 2020  ect.name}".     
-0001c850: 2020 2029 0a20 2020 2065 6c73 653a 0a20     ).    else:. 
-0001c860: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-0001c870: 666f 2866 225c 7441 6e73 7973 2050 726f  fo(f"\tAnsys Pro
-0001c880: 6a65 6374 2077 6173 206e 6f74 2066 6f75  ject was not fou
-0001c890: 6e64 2e5c 6e5c 7420 5072 6f6a 6563 7420  nd.\n\t Project 
-0001c8a0: 6973 204e 6f6e 652e 2229 0a0a 2020 2020  is None.")..    
-0001c8b0: 7265 7475 726e 2061 7070 2c20 6465 736b  return app, desk
-0001c8c0: 746f 702c 2070 726f 6a65 6374 0a         top, project.
+00017850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017860: 2020 2020 2020 2020 2020 2020 7374 7228              str(
+00017870: 6f62 6a29 5d2c 0a20 2020 2020 2020 2020  obj)],.         
+00017880: 2020 2020 2020 205b 224e 414d 453a 4368         ["NAME:Ch
+00017890: 616e 6765 6450 726f 7073 222c 205b 224e  angedProps", ["N
+000178a0: 414d 453a 4e61 6d65 222c 2022 5661 6c75  AME:Name", "Valu
+000178b0: 653a 3d22 2c0a 2020 2020 2020 2020 2020  e:=",.          
+000178c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000178d0: 2020 2020 2020 2020 2020 2020 2073 7472               str
+000178e0: 286e 616d 6529 5d5d 0a20 2020 2020 2020  (name)]].       
+000178f0: 2020 2020 205d 0a20 2020 2020 2020 205d       ].        ]
+00017900: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00017910: 206e 616d 650a 0a0a 636c 6173 7320 4d6f   name...class Mo
+00017920: 6465 6c45 6e74 6974 7928 7374 722c 2048  delEntity(str, H
+00017930: 6673 7350 726f 7065 7274 794f 626a 6563  fssPropertyObjec
+00017940: 7429 3a0a 2020 2020 7072 6f70 5f74 6162  t):.    prop_tab
+00017950: 203d 2022 4765 6f6d 6574 7279 3344 436d   = "Geometry3DCm
+00017960: 6454 6162 220a 2020 2020 6d6f 6465 6c5f  dTab".    model_
+00017970: 636f 6d6d 616e 6420 3d20 4e6f 6e65 0a20  command = None. 
+00017980: 2020 2074 7261 6e73 7061 7265 6e63 7920     transparency 
+00017990: 3d20 6d61 6b65 5f66 6c6f 6174 5f70 726f  = make_float_pro
+000179a0: 7028 2254 7261 6e73 7061 7265 6e74 222c  p("Transparent",
+000179b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000179c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179d0: 2020 2020 7072 6f70 5f74 6162 3d22 4765      prop_tab="Ge
+000179e0: 6f6d 6574 7279 3344 4174 7472 6962 7574  ometry3DAttribut
+000179f0: 6554 6162 222c 0a20 2020 2020 2020 2020  eTab",.         
+00017a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a10: 2020 2020 2020 2020 2020 7072 6f70 5f73            prop_s
+00017a20: 6572 7665 723d 6c61 6d62 6461 2073 656c  erver=lambda sel
+00017a30: 663a 2073 656c 6629 0a20 2020 206d 6174  f: self).    mat
+00017a40: 6572 6961 6c20 3d20 6d61 6b65 5f73 7472  erial = make_str
+00017a50: 5f70 726f 7028 224d 6174 6572 6961 6c22  _prop("Material"
+00017a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017a70: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00017a80: 726f 705f 7461 623d 2247 656f 6d65 7472  rop_tab="Geometr
+00017a90: 7933 4441 7474 7269 6275 7465 5461 6222  y3DAttributeTab"
+00017aa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017ab0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00017ac0: 726f 705f 7365 7276 6572 3d6c 616d 6264  rop_server=lambd
+00017ad0: 6120 7365 6c66 3a20 7365 6c66 290a 2020  a self: self).  
+00017ae0: 2020 7769 7265 6672 616d 6520 3d20 6d61    wireframe = ma
+00017af0: 6b65 5f66 6c6f 6174 5f70 726f 7028 2244  ke_float_prop("D
+00017b00: 6973 706c 6179 2057 6972 6566 7261 6d65  isplay Wireframe
+00017b10: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b30: 2020 2070 726f 705f 7461 623d 2247 656f     prop_tab="Geo
+00017b40: 6d65 7472 7933 4441 7474 7269 6275 7465  metry3DAttribute
+00017b50: 5461 6222 2c0a 2020 2020 2020 2020 2020  Tab",.          
+00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b70: 2020 2020 2020 7072 6f70 5f73 6572 7665        prop_serve
+00017b80: 723d 6c61 6d62 6461 2073 656c 663a 2073  r=lambda self: s
+00017b90: 656c 6629 0a20 2020 2063 6f6f 7264 696e  elf).    coordin
+00017ba0: 6174 655f 7379 7374 656d 203d 206d 616b  ate_system = mak
+00017bb0: 655f 7374 725f 7072 6f70 2822 436f 6f72  e_str_prop("Coor
+00017bc0: 6469 6e61 7465 2053 7973 7465 6d22 290a  dinate System").
+00017bd0: 0a20 2020 2064 6566 205f 5f6e 6577 5f5f  .    def __new__
+00017be0: 2873 656c 662c 2076 616c 2c20 2a61 7267  (self, val, *arg
+00017bf0: 732c 202a 2a6b 7761 7267 7329 3a0a 2020  s, **kwargs):.  
+00017c00: 2020 2020 2020 7265 7475 726e 2073 7472        return str
+00017c10: 2e5f 5f6e 6577 5f5f 2873 656c 662c 2076  .__new__(self, v
+00017c20: 616c 290a 0a20 2020 2064 6566 205f 5f69  al)..    def __i
+00017c30: 6e69 745f 5f28 7365 6c66 2c20 7661 6c2c  nit__(self, val,
+00017c40: 206d 6f64 656c 6572 293a 0a20 2020 2020   modeler):.     
+00017c50: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00017c60: 7479 7065 2076 616c 3a20 7374 720a 2020  type val: str.  
+00017c70: 2020 2020 2020 3a74 7970 6520 6d6f 6465        :type mode
+00017c80: 6c65 723a 2048 6673 734d 6f64 656c 6572  ler: HfssModeler
+00017c90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00017ca0: 2020 2020 2073 7570 6572 284d 6f64 656c       super(Model
+00017cb0: 456e 7469 7479 2c0a 2020 2020 2020 2020  Entity,.        
+00017cc0: 2020 2020 2020 7365 6c66 292e 5f5f 696e        self).__in
+00017cd0: 6974 5f5f 2829 2020 2320 7661 6c29 2023  it__()  # val) #
+00017ce0: 436f 6d6d 656e 7420 6f75 7420 6b65 7977  Comment out keyw
+00017cf0: 6f72 6420 746f 206d 6174 6368 2061 7267  ord to match arg
+00017d00: 756d 656e 7473 0a20 2020 2020 2020 2073  uments.        s
+00017d10: 656c 662e 6d6f 6465 6c65 7220 3d20 6d6f  elf.modeler = mo
+00017d20: 6465 6c65 720a 2020 2020 2020 2020 7365  deler.        se
+00017d30: 6c66 2e70 726f 705f 7365 7276 6572 203d  lf.prop_server =
+00017d40: 2073 656c 6620 2b20 223a 2220 2b20 7365   self + ":" + se
+00017d50: 6c66 2e6d 6f64 656c 5f63 6f6d 6d61 6e64  lf.model_command
+00017d60: 202b 2022 3a31 220a 0a0a 636c 6173 7320   + ":1"...class 
+00017d70: 426f 7828 4d6f 6465 6c45 6e74 6974 7929  Box(ModelEntity)
+00017d80: 3a0a 2020 2020 6d6f 6465 6c5f 636f 6d6d  :.    model_comm
+00017d90: 616e 6420 3d20 2243 7265 6174 6542 6f78  and = "CreateBox
+00017da0: 220a 2020 2020 706f 7369 7469 6f6e 203d  ".    position =
+00017db0: 206d 616b 655f 666c 6f61 745f 7072 6f70   make_float_prop
+00017dc0: 2822 506f 7369 7469 6f6e 2229 0a20 2020  ("Position").   
+00017dd0: 2078 5f73 697a 6520 3d20 6d61 6b65 5f66   x_size = make_f
+00017de0: 6c6f 6174 5f70 726f 7028 2258 5369 7a65  loat_prop("XSize
+00017df0: 2229 0a20 2020 2079 5f73 697a 6520 3d20  ").    y_size = 
+00017e00: 6d61 6b65 5f66 6c6f 6174 5f70 726f 7028  make_float_prop(
+00017e10: 2259 5369 7a65 2229 0a20 2020 207a 5f73  "YSize").    z_s
+00017e20: 697a 6520 3d20 6d61 6b65 5f66 6c6f 6174  ize = make_float
+00017e30: 5f70 726f 7028 225a 5369 7a65 2229 0a0a  _prop("ZSize")..
+00017e40: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00017e50: 2873 656c 662c 206e 616d 652c 206d 6f64  (self, name, mod
+00017e60: 656c 6572 2c20 636f 726e 6572 2c20 7369  eler, corner, si
+00017e70: 7a65 293a 0a20 2020 2020 2020 2022 2222  ze):.        """
+00017e80: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
+00017e90: 616d 653a 2073 7472 0a20 2020 2020 2020  ame: str.       
+00017ea0: 203a 7479 7065 206d 6f64 656c 6572 3a20   :type modeler: 
+00017eb0: 4866 7373 4d6f 6465 6c65 720a 2020 2020  HfssModeler.    
+00017ec0: 2020 2020 3a74 7970 6520 636f 726e 6572      :type corner
+00017ed0: 3a20 5b28 5661 7269 6162 6c65 5374 7269  : [(VariableStri
+00017ee0: 6e67 2c20 5661 7269 6162 6c65 5374 7269  ng, VariableStri
+00017ef0: 6e67 2c20 5661 7269 6162 6c65 5374 7269  ng, VariableStri
+00017f00: 6e67 295d 0a20 2020 2020 2020 203a 7061  ng)].        :pa
+00017f10: 7261 6d20 7369 7a65 3a20 5b28 5661 7269  ram size: [(Vari
+00017f20: 6162 6c65 5374 7269 6e67 2c20 5661 7269  ableString, Vari
+00017f30: 6162 6c65 5374 7269 6e67 2c20 5661 7269  ableString, Vari
+00017f40: 6162 6c65 5374 7269 6e67 295d 0a20 2020  ableString)].   
+00017f50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00017f60: 2073 7570 6572 2842 6f78 2c20 7365 6c66   super(Box, self
+00017f70: 292e 5f5f 696e 6974 5f5f 286e 616d 652c  ).__init__(name,
+00017f80: 206d 6f64 656c 6572 290a 2020 2020 2020   modeler).      
+00017f90: 2020 7365 6c66 2e6d 6f64 656c 6572 203d    self.modeler =
+00017fa0: 206d 6f64 656c 6572 0a20 2020 2020 2020   modeler.       
+00017fb0: 2073 656c 662e 7072 6f70 5f68 6f6c 6465   self.prop_holde
+00017fc0: 7220 3d20 6d6f 6465 6c65 722e 5f6d 6f64  r = modeler._mod
+00017fd0: 656c 6572 0a20 2020 2020 2020 2073 656c  eler.        sel
+00017fe0: 662e 636f 726e 6572 203d 2063 6f72 6e65  f.corner = corne
+00017ff0: 720a 2020 2020 2020 2020 7365 6c66 2e73  r.        self.s
+00018000: 697a 6520 3d20 7369 7a65 0a20 2020 2020  ize = size.     
+00018010: 2020 2073 656c 662e 6365 6e74 6572 203d     self.center =
+00018020: 205b 6320 2b20 7320 2f20 3220 666f 7220   [c + s / 2 for 
+00018030: 632c 2073 2069 6e20 7a69 7028 636f 726e  c, s in zip(corn
+00018040: 6572 2c20 7369 7a65 295d 0a20 2020 2020  er, size)].     
+00018050: 2020 2066 6163 6573 203d 206d 6f64 656c     faces = model
+00018060: 6572 2e67 6574 5f66 6163 655f 6964 7328  er.get_face_ids(
+00018070: 7365 6c66 290a 2020 2020 2020 2020 7365  self).        se
+00018080: 6c66 2e7a 5f62 6163 6b5f 6661 6365 2c20  lf.z_back_face, 
+00018090: 7365 6c66 2e7a 5f66 726f 6e74 5f66 6163  self.z_front_fac
+000180a0: 6520 3d20 6661 6365 735b 305d 2c20 6661  e = faces[0], fa
+000180b0: 6365 735b 315d 0a20 2020 2020 2020 2073  ces[1].        s
+000180c0: 656c 662e 795f 6261 636b 5f66 6163 652c  elf.y_back_face,
+000180d0: 2073 656c 662e 795f 6672 6f6e 745f 6661   self.y_front_fa
+000180e0: 6365 203d 2066 6163 6573 5b32 5d2c 2066  ce = faces[2], f
+000180f0: 6163 6573 5b34 5d0a 2020 2020 2020 2020  aces[4].        
+00018100: 7365 6c66 2e78 5f62 6163 6b5f 6661 6365  self.x_back_face
+00018110: 2c20 7365 6c66 2e78 5f66 726f 6e74 5f66  , self.x_front_f
+00018120: 6163 6520 3d20 6661 6365 735b 335d 2c20  ace = faces[3], 
+00018130: 6661 6365 735b 355d 0a0a 0a63 6c61 7373  faces[5]...class
+00018140: 2052 6563 7428 4d6f 6465 6c45 6e74 6974   Rect(ModelEntit
+00018150: 7929 3a0a 2020 2020 6d6f 6465 6c5f 636f  y):.    model_co
+00018160: 6d6d 616e 6420 3d20 2243 7265 6174 6552  mmand = "CreateR
+00018170: 6563 7461 6e67 6c65 220a 0a20 2020 2023  ectangle"..    #
+00018180: 2054 4f44 4f3a 2041 6464 2061 2072 6f74   TODO: Add a rot
+00018190: 6174 6564 2072 6563 7461 6e67 6c65 206f  ated rectangle o
+000181a0: 626a 6563 742e 0a20 2020 2023 2057 696c  bject..    # Wil
+000181b0: 6c20 6e65 6564 2074 6f20 6669 7273 7420  l need to first 
+000181c0: 6372 6561 7465 2072 6563 742c 2074 6865  create rect, the
+000181d0: 6e20 6170 706c 7920 726f 7461 7465 206f  n apply rotate o
+000181e0: 7065 7261 7469 6f6e 2e0a 0a20 2020 2064  peration...    d
+000181f0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00018200: 2c20 6e61 6d65 2c20 6d6f 6465 6c65 722c  , name, modeler,
+00018210: 2063 6f72 6e65 722c 2073 697a 6529 3a0a   corner, size):.
+00018220: 2020 2020 2020 2020 7375 7065 7228 5265          super(Re
+00018230: 6374 2c20 7365 6c66 292e 5f5f 696e 6974  ct, self).__init
+00018240: 5f5f 286e 616d 652c 206d 6f64 656c 6572  __(name, modeler
+00018250: 290a 2020 2020 2020 2020 7365 6c66 2e70  ).        self.p
+00018260: 726f 705f 686f 6c64 6572 203d 206d 6f64  rop_holder = mod
+00018270: 656c 6572 2e5f 6d6f 6465 6c65 720a 2020  eler._modeler.  
+00018280: 2020 2020 2020 7365 6c66 2e63 6f72 6e65        self.corne
+00018290: 7220 3d20 636f 726e 6572 0a20 2020 2020  r = corner.     
+000182a0: 2020 2073 656c 662e 7369 7a65 203d 2073     self.size = s
+000182b0: 697a 650a 2020 2020 2020 2020 7365 6c66  ize.        self
+000182c0: 2e63 656e 7465 7220 3d20 5b63 202b 2073  .center = [c + s
+000182d0: 202f 2032 2069 6620 7320 656c 7365 2063   / 2 if s else c
+000182e0: 2066 6f72 2063 2c20 7320 696e 207a 6970   for c, s in zip
+000182f0: 2863 6f72 6e65 722c 2073 697a 6529 5d0a  (corner, size)].
+00018300: 0a20 2020 2064 6566 206d 616b 655f 6365  .    def make_ce
+00018310: 6e74 6572 5f6c 696e 6528 7365 6c66 2c20  nter_line(self, 
+00018320: 6178 6973 293a 0a20 2020 2020 2020 2027  axis):.        '
+00018330: 2727 0a20 2020 2020 2020 2052 6574 7572  ''.        Retur
+00018340: 6e73 2060 7374 6172 7460 2061 6e64 2060  ns `start` and `
+00018350: 656e 6460 206c 6973 7420 6f66 2033 2063  end` list of 3 c
+00018360: 6f6f 7264 696e 6174 6573 0a20 2020 2020  oordinates.     
+00018370: 2020 2027 2727 0a20 2020 2020 2020 2061     '''.        a
+00018380: 7869 735f 6964 7820 3d20 5b22 7822 2c20  xis_idx = ["x", 
+00018390: 2279 222c 2022 7a22 5d2e 696e 6465 7828  "y", "z"].index(
+000183a0: 6178 6973 2e6c 6f77 6572 2829 290a 2020  axis.lower()).  
+000183b0: 2020 2020 2020 7374 6172 7420 3d20 5b63        start = [c
+000183c0: 2066 6f72 2063 2069 6e20 7365 6c66 2e63   for c in self.c
+000183d0: 656e 7465 725d 0a20 2020 2020 2020 2073  enter].        s
+000183e0: 7461 7274 5b61 7869 735f 6964 785d 202d  tart[axis_idx] -
+000183f0: 3d20 7365 6c66 2e73 697a 655b 6178 6973  = self.size[axis
+00018400: 5f69 6478 5d20 2f20 320a 2020 2020 2020  _idx] / 2.      
+00018410: 2020 7374 6172 7420 3d20 5b73 656c 662e    start = [self.
+00018420: 6d6f 6465 6c65 722e 6576 616c 5f65 7870  modeler.eval_exp
+00018430: 7228 7329 2066 6f72 2073 2069 6e20 7374  r(s) for s in st
+00018440: 6172 745d 0a20 2020 2020 2020 2065 6e64  art].        end
+00018450: 203d 205b 6320 666f 7220 6320 696e 2073   = [c for c in s
+00018460: 656c 662e 6365 6e74 6572 5d0a 2020 2020  elf.center].    
+00018470: 2020 2020 656e 645b 6178 6973 5f69 6478      end[axis_idx
+00018480: 5d20 2b3d 2073 656c 662e 7369 7a65 5b61  ] += self.size[a
+00018490: 7869 735f 6964 785d 202f 2032 0a20 2020  xis_idx] / 2.   
+000184a0: 2020 2020 2065 6e64 203d 205b 7365 6c66       end = [self
+000184b0: 2e6d 6f64 656c 6572 2e65 7661 6c5f 6578  .modeler.eval_ex
+000184c0: 7072 2873 2920 666f 7220 7320 696e 2065  pr(s) for s in e
+000184d0: 6e64 5d0a 2020 2020 2020 2020 7265 7475  nd].        retu
+000184e0: 726e 2073 7461 7274 2c20 656e 640a 0a20  rn start, end.. 
+000184f0: 2020 2064 6566 206d 616b 655f 726c 635f     def make_rlc_
+00018500: 626f 756e 6461 7279 2873 656c 662c 2061  boundary(self, a
+00018510: 7869 732c 2072 3d30 2c20 6c3d 302c 2063  xis, r=0, l=0, c
+00018520: 3d30 2c20 6e61 6d65 3d22 4c75 6d70 524c  =0, name="LumpRL
+00018530: 4322 293a 0a20 2020 2020 2020 2073 7461  C"):.        sta
+00018540: 7274 2c20 656e 6420 3d20 7365 6c66 2e6d  rt, end = self.m
+00018550: 616b 655f 6365 6e74 6572 5f6c 696e 6528  ake_center_line(
+00018560: 6178 6973 290a 2020 2020 2020 2020 7365  axis).        se
+00018570: 6c66 2e6d 6f64 656c 6572 2e5f 6d61 6b65  lf.modeler._make
+00018580: 5f6c 756d 7065 645f 726c 6328 722c 0a20  _lumped_rlc(r,. 
+00018590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185b0: 2020 2020 206c 2c0a 2020 2020 2020 2020       l,.        
+000185c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185d0: 2020 2020 2020 2020 2020 2020 2020 632c                c,
+000185e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000185f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018600: 2020 2020 2020 2073 7461 7274 2c0a 2020         start,.  
+00018610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018630: 2020 2020 656e 642c 205b 224f 626a 6563      end, ["Objec
+00018640: 7473 3a3d 222c 205b 7365 6c66 5d5d 2c0a  ts:=", [self]],.
+00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018670: 2020 2020 2020 6e61 6d65 3d6e 616d 6529        name=name)
+00018680: 0a0a 2020 2020 6465 6620 6d61 6b65 5f6c  ..    def make_l
+00018690: 756d 7065 645f 706f 7274 2873 656c 662c  umped_port(self,
+000186a0: 2061 7869 732c 207a 303d 2235 306f 686d   axis, z0="50ohm
+000186b0: 222c 206e 616d 653d 224c 756d 7050 6f72  ", name="LumpPor
+000186c0: 7422 293a 0a20 2020 2020 2020 2073 7461  t"):.        sta
+000186d0: 7274 2c20 656e 6420 3d20 7365 6c66 2e6d  rt, end = self.m
+000186e0: 616b 655f 6365 6e74 6572 5f6c 696e 6528  ake_center_line(
+000186f0: 6178 6973 290a 2020 2020 2020 2020 7365  axis).        se
+00018700: 6c66 2e6d 6f64 656c 6572 2e5f 6d61 6b65  lf.modeler._make
+00018710: 5f6c 756d 7065 645f 706f 7274 2873 7461  _lumped_port(sta
+00018720: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
+00018730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018740: 2020 2020 2020 2020 2020 2065 6e64 2c20             end, 
+00018750: 5b22 4f62 6a65 6374 733a 3d22 2c20 5b73  ["Objects:=", [s
+00018760: 656c 665d 5d2c 0a20 2020 2020 2020 2020  elf]],.         
+00018770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018780: 2020 2020 2020 2020 2020 2020 2020 7a30                z0
+00018790: 3d7a 302c 0a20 2020 2020 2020 2020 2020  =z0,.           
+000187a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000187c0: 3d6e 616d 6529 0a0a 0a63 6c61 7373 2050  =name)...class P
+000187d0: 6f6c 796c 696e 6528 4d6f 6465 6c45 6e74  olyline(ModelEnt
+000187e0: 6974 7929 3a0a 2020 2020 2727 270a 2020  ity):.    '''.  
+000187f0: 2020 4173 7375 6d65 2063 6c6f 7365 6420    Assume closed 
+00018800: 706f 6c79 6c69 6e65 2c20 7768 6963 6820  polyline, which 
+00018810: 6372 6561 7465 7320 6120 706f 6c79 676f  creates a polygo
+00018820: 6e2e 0a20 2020 2027 2727 0a0a 2020 2020  n..    '''..    
+00018830: 6d6f 6465 6c5f 636f 6d6d 616e 6420 3d20  model_command = 
+00018840: 2243 7265 6174 6550 6f6c 796c 696e 6522  "CreatePolyline"
+00018850: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00018860: 5f5f 2873 656c 662c 206e 616d 652c 206d  __(self, name, m
+00018870: 6f64 656c 6572 2c20 706f 696e 7473 3d4e  odeler, points=N
+00018880: 6f6e 6529 3a0a 2020 2020 2020 2020 7375  one):.        su
+00018890: 7065 7228 506f 6c79 6c69 6e65 2c20 7365  per(Polyline, se
+000188a0: 6c66 292e 5f5f 696e 6974 5f5f 286e 616d  lf).__init__(nam
+000188b0: 652c 206d 6f64 656c 6572 290a 2020 2020  e, modeler).    
+000188c0: 2020 2020 7365 6c66 2e70 726f 705f 686f      self.prop_ho
+000188d0: 6c64 6572 203d 206d 6f64 656c 6572 2e5f  lder = modeler._
+000188e0: 6d6f 6465 6c65 720a 2020 2020 2020 2020  modeler.        
+000188f0: 6966 2070 6f69 6e74 7320 6973 206e 6f74  if points is not
+00018900: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00018910: 2020 2073 656c 662e 706f 696e 7473 203d     self.points =
+00018920: 2070 6f69 6e74 730a 2020 2020 2020 2020   points.        
+00018930: 2020 2020 7365 6c66 2e6e 5f70 6f69 6e74      self.n_point
+00018940: 7320 3d20 6c65 6e28 706f 696e 7473 290a  s = len(points).
+00018950: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00018960: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+00018970: 2020 2020 2020 2020 2020 2023 2054 4f44             # TOD
+00018980: 4f3a 2070 6f69 6e74 7320 3d20 636f 6c6c  O: points = coll
+00018990: 6563 7469 6f6e 206f 6620 706f 696e 7473  ection of points
+000189a0: 0a0a 0a23 2020 2020 2020 2020 6178 6973  ...#        axis
+000189b0: 203d 2066 696e 645f 6f72 7468 5f61 7869   = find_orth_axi
+000189c0: 7328 290a 0a23 2054 4f44 4f3a 2066 696e  s()..# TODO: fin
+000189d0: 6420 7468 6520 706c 616e 6520 6f66 2074  d the plane of t
+000189e0: 6865 2070 6f6c 796c 696e 6520 666f 7220  he polyline for 
+000189f0: 6e6f 772c 2061 7373 756d 6520 5a0a 2320  now, assume Z.# 
+00018a00: 2020 2064 6566 2066 696e 645f 6f72 7468     def find_orth
+00018a10: 5f61 7869 7328 293a 0a23 2020 2020 2020  _axis():.#      
+00018a20: 2020 582c 2059 2c20 5a20 3d20 2854 7275    X, Y, Z = (Tru
+00018a30: 652c 2054 7275 652c 2054 7275 6529 0a23  e, True, True).#
+00018a40: 2020 2020 2020 2020 666f 7220 706f 696e          for poin
+00018a50: 7420 696e 2070 6f69 6e74 733a 0a23 2020  t in points:.#  
+00018a60: 2020 2020 2020 2020 2020 5820 3d0a 0a20            X =.. 
+00018a70: 2020 2064 6566 2075 6e69 7465 2873 656c     def unite(sel
+00018a80: 662c 206c 6973 745f 6f74 6865 7229 3a0a  f, list_other):.
+00018a90: 2020 2020 2020 2020 756e 696f 6e20 3d20          union = 
+00018aa0: 7365 6c66 2e6d 6f64 656c 6572 2e75 6e69  self.modeler.uni
+00018ab0: 7465 2873 656c 6620 2b20 6c69 7374 5f6f  te(self + list_o
+00018ac0: 7468 6572 290a 2020 2020 2020 2020 7265  ther).        re
+00018ad0: 7475 726e 2050 6f6c 796c 696e 6528 756e  turn Polyline(un
+00018ae0: 696f 6e2c 2073 656c 662e 6d6f 6465 6c65  ion, self.modele
+00018af0: 7229 0a0a 2020 2020 6465 6620 6d61 6b65  r)..    def make
+00018b00: 5f63 656e 7465 725f 6c69 6e65 2873 656c  _center_line(sel
+00018b10: 662c 2061 7869 7329 3a20 2023 2045 7870  f, axis):  # Exp
+00018b20: 6563 7473 2074 6f20 6163 7420 6f6e 2061  ects to act on a
+00018b30: 2072 6563 7461 6e67 6c65 2e2e 2e0a 2020   rectangle....  
+00018b40: 2020 2020 2020 2320 6669 7273 7420 3a20        # first : 
+00018b50: 6669 6e64 2063 656e 7465 7220 616e 6420  find center and 
+00018b60: 7369 7a65 0a20 2020 2020 2020 2063 656e  size.        cen
+00018b70: 7465 7220 3d20 5b30 2c20 302c 2030 5d0a  ter = [0, 0, 0].
+00018b80: 0a20 2020 2020 2020 2066 6f72 2070 6f69  .        for poi
+00018b90: 6e74 2069 6e20 7365 6c66 2e70 6f69 6e74  nt in self.point
+00018ba0: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00018bb0: 656e 7465 7220 3d20 5b0a 2020 2020 2020  enter = [.      
+00018bc0: 2020 2020 2020 2020 2020 6365 6e74 6572            center
+00018bd0: 5b30 5d20 2b20 706f 696e 745b 305d 202f  [0] + point[0] /
+00018be0: 2073 656c 662e 6e5f 706f 696e 7473 2c0a   self.n_points,.
+00018bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c00: 6365 6e74 6572 5b31 5d20 2b20 706f 696e  center[1] + poin
+00018c10: 745b 315d 202f 2073 656c 662e 6e5f 706f  t[1] / self.n_po
+00018c20: 696e 7473 2c0a 2020 2020 2020 2020 2020  ints,.          
+00018c30: 2020 2020 2020 6365 6e74 6572 5b32 5d20        center[2] 
+00018c40: 2b20 706f 696e 745b 325d 202f 2073 656c  + point[2] / sel
+00018c50: 662e 6e5f 706f 696e 7473 0a20 2020 2020  f.n_points.     
+00018c60: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00018c70: 2073 697a 6520 3d20 5b0a 2020 2020 2020   size = [.      
+00018c80: 2020 2020 2020 3220 2a20 2863 656e 7465        2 * (cente
+00018c90: 725b 305d 202d 2073 656c 662e 706f 696e  r[0] - self.poin
+00018ca0: 7473 5b30 5d5b 305d 292c 0a20 2020 2020  ts[0][0]),.     
+00018cb0: 2020 2020 2020 2032 202a 2028 6365 6e74         2 * (cent
+00018cc0: 6572 5b31 5d20 2d20 7365 6c66 2e70 6f69  er[1] - self.poi
+00018cd0: 6e74 735b 305d 5b31 5d29 2c0a 2020 2020  nts[0][1]),.    
+00018ce0: 2020 2020 2020 2020 3220 2a20 2863 656e          2 * (cen
+00018cf0: 7465 725b 315d 202d 2073 656c 662e 706f  ter[1] - self.po
+00018d00: 696e 7473 5b30 5d5b 325d 290a 2020 2020  ints[0][2]).    
+00018d10: 2020 2020 5d0a 2020 2020 2020 2020 6178      ].        ax
+00018d20: 6973 5f69 6478 203d 205b 2278 222c 2022  is_idx = ["x", "
+00018d30: 7922 2c20 227a 225d 2e69 6e64 6578 2861  y", "z"].index(a
+00018d40: 7869 732e 6c6f 7765 7228 2929 0a20 2020  xis.lower()).   
+00018d50: 2020 2020 2073 7461 7274 203d 205b 6320       start = [c 
+00018d60: 666f 7220 6320 696e 2063 656e 7465 725d  for c in center]
+00018d70: 0a20 2020 2020 2020 2073 7461 7274 5b61  .        start[a
+00018d80: 7869 735f 6964 785d 202d 3d20 7369 7a65  xis_idx] -= size
+00018d90: 5b61 7869 735f 6964 785d 202f 2032 0a20  [axis_idx] / 2. 
+00018da0: 2020 2020 2020 2073 7461 7274 203d 205b         start = [
+00018db0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00018dc0: 662e 6d6f 6465 6c65 722e 6576 616c 5f76  f.modeler.eval_v
+00018dd0: 6172 5f73 7472 2873 2c20 756e 6974 3d4c  ar_str(s, unit=L
+00018de0: 454e 4754 485f 554e 4954 2920 666f 7220  ENGTH_UNIT) for 
+00018df0: 7320 696e 2073 7461 7274 0a20 2020 2020  s in start.     
+00018e00: 2020 205d 2020 2320 544f 444f 0a20 2020     ]  # TODO.   
+00018e10: 2020 2020 2065 6e64 203d 205b 6320 666f       end = [c fo
+00018e20: 7220 6320 696e 2063 656e 7465 725d 0a20  r c in center]. 
+00018e30: 2020 2020 2020 2065 6e64 5b61 7869 735f         end[axis_
+00018e40: 6964 785d 202b 3d20 7369 7a65 5b61 7869  idx] += size[axi
+00018e50: 735f 6964 785d 202f 2032 0a20 2020 2020  s_idx] / 2.     
+00018e60: 2020 2065 6e64 203d 205b 7365 6c66 2e6d     end = [self.m
+00018e70: 6f64 656c 6572 2e65 7661 6c5f 7661 725f  odeler.eval_var_
+00018e80: 7374 7228 732c 2075 6e69 743d 4c45 4e47  str(s, unit=LENG
+00018e90: 5448 5f55 4e49 5429 2066 6f72 2073 2069  TH_UNIT) for s i
+00018ea0: 6e20 656e 645d 0a20 2020 2020 2020 2072  n end].        r
+00018eb0: 6574 7572 6e20 7374 6172 742c 2065 6e64  eturn start, end
+00018ec0: 0a0a 2020 2020 6465 6620 6d61 6b65 5f72  ..    def make_r
+00018ed0: 6c63 5f62 6f75 6e64 6172 7928 7365 6c66  lc_boundary(self
+00018ee0: 2c20 6178 6973 2c20 723d 302c 206c 3d30  , axis, r=0, l=0
+00018ef0: 2c20 633d 302c 206e 616d 653d 224c 756d  , c=0, name="Lum
+00018f00: 7052 4c43 2229 3a0a 2020 2020 2020 2020  pRLC"):.        
+00018f10: 6e61 6d65 203d 2073 7472 2873 656c 6629  name = str(self)
+00018f20: 202b 2027 5f27 202b 206e 616d 650a 2020   + '_' + name.  
+00018f30: 2020 2020 2020 7374 6172 742c 2065 6e64        start, end
+00018f40: 203d 2073 656c 662e 6d61 6b65 5f63 656e   = self.make_cen
+00018f50: 7465 725f 6c69 6e65 2861 7869 7329 0a20  ter_line(axis). 
+00018f60: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+00018f70: 6c65 722e 5f6d 616b 655f 6c75 6d70 6564  ler._make_lumped
+00018f80: 5f72 6c63 2872 2c0a 2020 2020 2020 2020  _rlc(r,.        
+00018f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fa0: 2020 2020 2020 2020 2020 2020 2020 6c2c                l,
+00018fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018fd0: 2020 2020 2020 2063 2c0a 2020 2020 2020         c,.      
+00018fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019000: 7374 6172 742c 0a20 2020 2020 2020 2020  start,.         
+00019010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019020: 2020 2020 2020 2020 2020 2020 2065 6e64               end
+00019030: 2c20 5b22 4f62 6a65 6374 733a 3d22 2c20  , ["Objects:=", 
+00019040: 5b73 656c 665d 5d2c 0a20 2020 2020 2020  [self]],.       
+00019050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019060: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00019070: 616d 653d 6e61 6d65 290a 0a20 2020 2064  ame=name)..    d
+00019080: 6566 2066 696c 6c65 7428 7365 6c66 2c20  ef fillet(self, 
+00019090: 7261 6469 7573 2c20 7665 7274 6578 5f69  radius, vertex_i
+000190a0: 6e64 6578 293a 0a20 2020 2020 2020 2073  ndex):.        s
+000190b0: 656c 662e 6d6f 6465 6c65 722e 5f66 696c  elf.modeler._fil
+000190c0: 6c65 7428 7261 6469 7573 2c20 7665 7274  let(radius, vert
+000190d0: 6578 5f69 6e64 6578 2c20 7365 6c66 290a  ex_index, self).
+000190e0: 0a20 2020 2064 6566 2076 6572 7469 6365  .    def vertice
+000190f0: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+00019100: 2072 6574 7572 6e20 7365 6c66 2e6d 6f64   return self.mod
+00019110: 656c 6572 2e67 6574 5f76 6572 7465 785f  eler.get_vertex_
+00019120: 6964 7328 7365 6c66 290a 0a20 2020 2064  ids(self)..    d
+00019130: 6566 2072 656e 616d 6528 7365 6c66 2c20  ef rename(self, 
+00019140: 6e65 775f 6e61 6d65 293a 0a20 2020 2020  new_name):.     
+00019150: 2020 2027 2727 0a20 2020 2020 2020 2020     '''.         
+00019160: 2020 2057 6172 6e69 6e67 3a20 5468 6520     Warning: The 
+00019170: 696e 6372 656d 656e 745f 6e61 6d65 206f  increment_name o
+00019180: 6e6c 7920 776f 726b 7320 6966 2074 6865  nly works if the
+00019190: 2073 6865 6574 2068 6173 206e 6f74 2062   sheet has not b
+000191a0: 6565 6e20 7374 7261 6374 6564 206f 7220  een stracted or 
+000191b0: 7573 6564 2061 7320 6120 746f 6f6c 2065  used as a tool e
+000191c0: 6c73 6577 6865 7265 2e0a 2020 2020 2020  lsewhere..      
+000191d0: 2020 2020 2020 5468 6573 6520 6e61 6d65        These name
+000191e0: 7320 6172 6520 6e6f 7420 6368 6563 6b65  s are not checke
+000191f0: 643b 2074 6865 7920 7265 7175 6972 6520  d; they require 
+00019200: 6d6f 6469 6679 696e 6720 6765 745f 6f62  modifying get_ob
+00019210: 6a65 6374 735f 696e 5f67 726f 7570 2e0a  jects_in_group..
+00019220: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+00019230: 2020 2020 206e 6577 5f6e 616d 6520 3d20       new_name = 
+00019240: 696e 6372 656d 656e 745f 6e61 6d65 280a  increment_name(.
+00019250: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00019260: 6e61 6d65 2c20 7365 6c66 2e6d 6f64 656c  name, self.model
+00019270: 6572 2e67 6574 5f6f 626a 6563 7473 5f69  er.get_objects_i
+00019280: 6e5f 6772 6f75 7028 0a20 2020 2020 2020  n_group(.       
+00019290: 2020 2020 2020 2020 2022 5368 6565 7473           "Sheets
+000192a0: 2229 2920 2023 2074 6869 7320 6973 2066  "))  # this is f
+000192b0: 6f72 2061 2063 6c6f 7365 6420 706f 6c79  or a closed poly
+000192c0: 6c69 6e65 0a0a 2020 2020 2020 2020 2320  line..        # 
+000192d0: 6368 6563 6b20 746f 2067 6574 2074 6865  check to get the
+000192e0: 2061 6374 7561 6c20 6e65 7720 6e61 6d65   actual new name
+000192f0: 2069 6e20 6361 7365 2074 6865 7265 2077   in case there w
+00019300: 6173 2061 2073 7562 7374 7261 6374 6564  as a substracted
+00019310: 206f 626a 6563 7420 7769 7468 2074 6861   object with tha
+00019320: 7420 6e61 6d65 0a20 2020 2020 2020 2066  t name.        f
+00019330: 6163 655f 6964 7320 3d20 7365 6c66 2e6d  ace_ids = self.m
+00019340: 6f64 656c 6572 2e67 6574 5f66 6163 655f  odeler.get_face_
+00019350: 6964 7328 7374 7228 7365 6c66 2929 0a20  ids(str(self)). 
+00019360: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+00019370: 6c65 722e 7265 6e61 6d65 5f6f 626a 2873  ler.rename_obj(s
+00019380: 656c 662c 206e 6577 5f6e 616d 6529 2020  elf, new_name)  
+00019390: 2320 6e6f 7720 7265 6e61 6d65 0a20 2020  # now rename.   
+000193a0: 2020 2020 2069 6620 6c65 6e28 6661 6365       if len(face
+000193b0: 5f69 6473 2920 3e20 303a 0a20 2020 2020  _ids) > 0:.     
+000193c0: 2020 2020 2020 206e 6577 5f6e 616d 6520         new_name 
+000193d0: 3d20 7365 6c66 2e6d 6f64 656c 6572 2e67  = self.modeler.g
+000193e0: 6574 5f6f 626a 6563 745f 6e61 6d65 5f62  et_object_name_b
+000193f0: 795f 6661 6365 5f69 6428 6661 6365 5f69  y_face_id(face_i
+00019400: 6473 5b30 5d29 0a20 2020 2020 2020 2072  ds[0]).        r
+00019410: 6574 7572 6e20 506f 6c79 6c69 6e65 2873  eturn Polyline(s
+00019420: 7472 286e 6577 5f6e 616d 6529 2c20 7365  tr(new_name), se
+00019430: 6c66 2e6d 6f64 656c 6572 290a 0a0a 636c  lf.modeler)...cl
+00019440: 6173 7320 4f70 656e 506f 6c79 6c69 6e65  ass OpenPolyline
+00019450: 284d 6f64 656c 456e 7469 7479 293a 2020  (ModelEntity):  
+00019460: 2320 4173 7375 6d65 2063 6c6f 7365 6420  # Assume closed 
+00019470: 706f 6c79 6c69 6e65 0a20 2020 206d 6f64  polyline.    mod
+00019480: 656c 5f63 6f6d 6d61 6e64 203d 2022 4372  el_command = "Cr
+00019490: 6561 7465 506f 6c79 6c69 6e65 220a 2020  eatePolyline".  
+000194a0: 2020 7368 6f77 5f64 6972 6563 7469 6f6e    show_direction
+000194b0: 203d 206d 616b 655f 7072 6f70 2827 5368   = make_prop('Sh
+000194c0: 6f77 2044 6972 6563 7469 6f6e 272c 0a20  ow Direction',. 
+000194d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194e0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000194f0: 6f70 5f74 6162 3d22 4765 6f6d 6574 7279  op_tab="Geometry
+00019500: 3344 4174 7472 6962 7574 6554 6162 222c  3DAttributeTab",
+00019510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019530: 7072 6f70 5f73 6572 7665 723d 6c61 6d62  prop_server=lamb
+00019540: 6461 2073 656c 663a 2073 656c 6629 0a0a  da self: self)..
+00019550: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00019560: 2873 656c 662c 206e 616d 652c 206d 6f64  (self, name, mod
+00019570: 656c 6572 2c20 706f 696e 7473 3d4e 6f6e  eler, points=Non
+00019580: 6529 3a0a 2020 2020 2020 2020 7375 7065  e):.        supe
+00019590: 7228 4f70 656e 506f 6c79 6c69 6e65 2c20  r(OpenPolyline, 
+000195a0: 7365 6c66 292e 5f5f 696e 6974 5f5f 286e  self).__init__(n
+000195b0: 616d 652c 206d 6f64 656c 6572 290a 2020  ame, modeler).  
+000195c0: 2020 2020 2020 7365 6c66 2e70 726f 705f        self.prop_
+000195d0: 686f 6c64 6572 203d 206d 6f64 656c 6572  holder = modeler
+000195e0: 2e5f 6d6f 6465 6c65 720a 2020 2020 2020  ._modeler.      
+000195f0: 2020 6966 2070 6f69 6e74 7320 6973 206e    if points is n
+00019600: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00019610: 2020 2020 2073 656c 662e 706f 696e 7473       self.points
+00019620: 203d 2070 6f69 6e74 730a 2020 2020 2020   = points.      
+00019630: 2020 2020 2020 7365 6c66 2e6e 5f70 6f69        self.n_poi
+00019640: 6e74 7320 3d20 6c65 6e28 706f 696e 7473  nts = len(points
+00019650: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00019660: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00019670: 0a0a 0a23 2020 2020 2020 2020 6178 6973  ...#        axis
+00019680: 203d 2066 696e 645f 6f72 7468 5f61 7869   = find_orth_axi
+00019690: 7328 290a 0a23 2054 4f44 4f3a 2066 696e  s()..# TODO: fin
+000196a0: 6420 7468 6520 706c 616e 6520 6f66 2074  d the plane of t
+000196b0: 6865 2070 6f6c 796c 696e 6520 666f 7220  he polyline for 
+000196c0: 6e6f 772c 2061 7373 756d 6520 5a0a 2320  now, assume Z.# 
+000196d0: 2020 2064 6566 2066 696e 645f 6f72 7468     def find_orth
+000196e0: 5f61 7869 7328 293a 0a23 2020 2020 2020  _axis():.#      
+000196f0: 2020 582c 2059 2c20 5a20 3d20 2854 7275    X, Y, Z = (Tru
+00019700: 652c 2054 7275 652c 2054 7275 6529 0a23  e, True, True).#
+00019710: 2020 2020 2020 2020 666f 7220 706f 696e          for poin
+00019720: 7420 696e 2070 6f69 6e74 733a 0a23 2020  t in points:.#  
+00019730: 2020 2020 2020 2020 2020 5820 3d0a 0a20            X =.. 
+00019740: 2020 2064 6566 2076 6572 7469 6365 7328     def vertices(
+00019750: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+00019760: 6574 7572 6e20 7365 6c66 2e6d 6f64 656c  eturn self.model
+00019770: 6572 2e67 6574 5f76 6572 7465 785f 6964  er.get_vertex_id
+00019780: 7328 7365 6c66 290a 0a20 2020 2064 6566  s(self)..    def
+00019790: 2066 696c 6c65 7428 7365 6c66 2c20 7261   fillet(self, ra
+000197a0: 6469 7573 2c20 7665 7274 6578 5f69 6e64  dius, vertex_ind
+000197b0: 6578 293a 0a20 2020 2020 2020 2073 656c  ex):.        sel
+000197c0: 662e 6d6f 6465 6c65 722e 5f66 696c 6c65  f.modeler._fille
+000197d0: 7428 7261 6469 7573 2c20 7665 7274 6578  t(radius, vertex
+000197e0: 5f69 6e64 6578 2c20 7365 6c66 290a 0a20  _index, self).. 
+000197f0: 2020 2064 6566 2066 696c 6c65 7473 2873     def fillets(s
+00019800: 656c 662c 2072 6164 6975 732c 2064 6f5f  elf, radius, do_
+00019810: 6e6f 745f 6669 6c6c 6574 3d5b 5d29 3a0a  not_fillet=[]):.
+00019820: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+00019830: 2020 2020 2020 2020 646f 5f6e 6f74 5f66          do_not_f
+00019840: 696c 6c65 7420 3a20 496e 6465 7820 6c69  illet : Index li
+00019850: 7374 206f 6620 7665 7274 6963 6573 2074  st of vertices t
+00019860: 6f20 6e6f 7420 6669 6c6c 6574 650a 2020  o not fillete.  
+00019870: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00019880: 2020 7261 775f 6c69 7374 5f76 6572 7469    raw_list_verti
+00019890: 6365 7320 3d20 7365 6c66 2e6d 6f64 656c  ces = self.model
+000198a0: 6572 2e67 6574 5f76 6572 7465 785f 6964  er.get_vertex_id
+000198b0: 7328 7365 6c66 290a 2020 2020 2020 2020  s(self).        
+000198c0: 6c69 7374 5f76 6572 7469 6365 7320 3d20  list_vertices = 
+000198d0: 5b5d 0a20 2020 2020 2020 2066 6f72 2076  [].        for v
+000198e0: 6572 7465 7820 696e 2072 6177 5f6c 6973  ertex in raw_lis
+000198f0: 745f 7665 7274 6963 6573 5b31 3a2d 315d  t_vertices[1:-1]
+00019900: 3a20 2023 2069 676e 6f72 6520 7468 6520  :  # ignore the 
+00019910: 7374 6172 7420 616e 6420 6669 6e69 7368  start and finish
+00019920: 0a20 2020 2020 2020 2020 2020 206c 6973  .            lis
+00019930: 745f 7665 7274 6963 6573 2e61 7070 656e  t_vertices.appen
+00019940: 6428 696e 7428 7665 7274 6578 2929 0a20  d(int(vertex)). 
+00019950: 2020 2020 2020 206c 6973 745f 7665 7274         list_vert
+00019960: 6963 6573 203d 206c 6973 7428 0a20 2020  ices = list(.   
+00019970: 2020 2020 2020 2020 206d 6170 280a 2020           map(.  
+00019980: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00019990: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+000199a0: 2020 206e 702e 6465 6c65 7465 286c 6973     np.delete(lis
+000199b0: 745f 7665 7274 6963 6573 2c0a 2020 2020  t_vertices,.    
+000199c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199d0: 2020 2020 2020 6e70 2e61 7272 6179 2864        np.array(d
+000199e0: 6f5f 6e6f 745f 6669 6c6c 6574 2c20 6474  o_not_fillet, dt
+000199f0: 7970 653d 696e 7429 202d 2031 2929 290a  ype=int) - 1))).
+00019a00: 2020 2020 2020 2020 2370 7269 6e74 286c          #print(l
+00019a10: 6973 745f 7665 7274 6963 6573 2c20 7479  ist_vertices, ty
+00019a20: 7065 286c 6973 745f 7665 7274 6963 6573  pe(list_vertices
+00019a30: 5b30 5d29 290a 2020 2020 2020 2020 6966  [0])).        if
+00019a40: 206c 656e 286c 6973 745f 7665 7274 6963   len(list_vertic
+00019a50: 6573 2920 213d 2030 3a0a 2020 2020 2020  es) != 0:.      
+00019a60: 2020 2020 2020 7365 6c66 2e6d 6f64 656c        self.model
+00019a70: 6572 2e5f 6669 6c6c 6574 7328 7261 6469  er._fillets(radi
+00019a80: 7573 2c20 6c69 7374 5f76 6572 7469 6365  us, list_vertice
+00019a90: 732c 2073 656c 6629 0a20 2020 2020 2020  s, self).       
+00019aa0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00019ab0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00019ac0: 2073 7765 6570 5f61 6c6f 6e67 5f70 6174   sweep_along_pat
+00019ad0: 6828 7365 6c66 2c20 746f 5f73 7765 6570  h(self, to_sweep
+00019ae0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00019af0: 6e20 7365 6c66 2e6d 6f64 656c 6572 2e5f  n self.modeler._
+00019b00: 7377 6565 705f 616c 6f6e 675f 7061 7468  sweep_along_path
+00019b10: 2874 6f5f 7377 6565 702c 2073 656c 6629  (to_sweep, self)
+00019b20: 0a0a 2020 2020 6465 6620 7265 6e61 6d65  ..    def rename
+00019b30: 2873 656c 662c 206e 6577 5f6e 616d 6529  (self, new_name)
+00019b40: 3a0a 2020 2020 2020 2020 2727 270a 2020  :.        '''.  
+00019b50: 2020 2020 2020 2020 2020 5761 726e 696e            Warnin
+00019b60: 673a 2054 6865 2020 696e 6372 656d 656e  g: The  incremen
+00019b70: 745f 6e61 6d65 206f 6e6c 7920 776f 726b  t_name only work
+00019b80: 7320 6966 2074 6865 2073 6865 6574 2068  s if the sheet h
+00019b90: 6173 206e 6f74 2062 6565 6e20 7374 7261  as not been stra
+00019ba0: 6374 6564 206f 7220 7573 6564 2061 7320  cted or used as 
+00019bb0: 6120 746f 6f6c 2065 6c73 6577 6865 722e  a tool elsewher.
+00019bc0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00019bd0: 7365 206e 616d 6573 2061 7265 206e 6f74  se names are not
+00019be0: 2063 6865 636b 6564 202d 2054 6865 7920   checked - They 
+00019bf0: 7265 7175 6972 6520 6d6f 6469 6679 696e  require modifyin
+00019c00: 6720 6765 745f 6f62 6a65 6374 735f 696e  g get_objects_in
+00019c10: 5f67 726f 7570 0a20 2020 2020 2020 2027  _group.        '
+00019c20: 2727 0a20 2020 2020 2020 206e 6577 5f6e  ''.        new_n
+00019c30: 616d 6520 3d20 696e 6372 656d 656e 745f  ame = increment_
+00019c40: 6e61 6d65 286e 6577 5f6e 616d 652c 0a20  name(new_name,. 
+00019c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c70: 2073 656c 662e 6d6f 6465 6c65 722e 6765   self.modeler.ge
+00019c80: 745f 6f62 6a65 6374 735f 696e 5f67 726f  t_objects_in_gro
+00019c90: 7570 2822 4c69 6e65 7322 2929 0a20 2020  up("Lines")).   
+00019ca0: 2020 2020 2023 202c 2073 656c 662e 706f       # , self.po
+00019cb0: 696e 7473 290a 2020 2020 2020 2020 7265  ints).        re
+00019cc0: 7475 726e 204f 7065 6e50 6f6c 796c 696e  turn OpenPolylin
+00019cd0: 6528 7365 6c66 2e6d 6f64 656c 6572 2e72  e(self.modeler.r
+00019ce0: 656e 616d 655f 6f62 6a28 7365 6c66 2c20  ename_obj(self, 
+00019cf0: 6e65 775f 6e61 6d65 292c 0a20 2020 2020  new_name),.     
+00019d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d10: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+00019d20: 6c65 7229 0a0a 2020 2020 6465 6620 636f  ler)..    def co
+00019d30: 7079 2873 656c 662c 206e 6577 5f6e 616d  py(self, new_nam
+00019d40: 6529 3a0a 2020 2020 2020 2020 6e65 775f  e):.        new_
+00019d50: 6f62 6a20 3d20 4f70 656e 506f 6c79 6c69  obj = OpenPolyli
+00019d60: 6e65 2873 656c 662e 6d6f 6465 6c65 722e  ne(self.modeler.
+00019d70: 636f 7079 2873 656c 6629 2c20 7365 6c66  copy(self), self
+00019d80: 2e6d 6f64 656c 6572 290a 2020 2020 2020  .modeler).      
+00019d90: 2020 7265 7475 726e 206e 6577 5f6f 626a    return new_obj
+00019da0: 2e72 656e 616d 6528 6e65 775f 6e61 6d65  .rename(new_name
+00019db0: 290a 0a0a 636c 6173 7320 4866 7373 4669  )...class HfssFi
+00019dc0: 656c 6473 4361 6c63 2843 4f4d 5772 6170  eldsCalc(COMWrap
+00019dd0: 7065 7229 3a0a 2020 2020 6465 6620 5f5f  per):.    def __
+00019de0: 696e 6974 5f5f 2873 656c 662c 2073 6574  init__(self, set
+00019df0: 7570 293a 0a20 2020 2020 2020 2022 2222  up):.        """
+00019e00: 0a20 2020 2020 2020 203a 7479 7065 2073  .        :type s
+00019e10: 6574 7570 3a20 4866 7373 5365 7475 700a  etup: HfssSetup.
+00019e20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00019e30: 2020 2020 7365 6c66 2e73 6574 7570 203d      self.setup =
+00019e40: 2073 6574 7570 0a20 2020 2020 2020 2073   setup.        s
+00019e50: 7570 6572 2848 6673 7346 6965 6c64 7343  uper(HfssFieldsC
+00019e60: 616c 632c 2073 656c 6629 2e5f 5f69 6e69  alc, self).__ini
+00019e70: 745f 5f28 290a 2020 2020 2020 2020 7365  t__().        se
+00019e80: 6c66 2e70 6172 656e 7420 3d20 7365 7475  lf.parent = setu
+00019e90: 700a 2020 2020 2020 2020 7365 6c66 2e4d  p.        self.M
+00019ea0: 6167 5f45 203d 204e 616d 6564 4361 6c63  ag_E = NamedCalc
+00019eb0: 4f62 6a65 6374 2822 4d61 675f 4522 2c20  Object("Mag_E", 
+00019ec0: 7365 7475 7029 0a20 2020 2020 2020 2073  setup).        s
+00019ed0: 656c 662e 4d61 675f 4820 3d20 4e61 6d65  elf.Mag_H = Name
+00019ee0: 6443 616c 634f 626a 6563 7428 224d 6167  dCalcObject("Mag
+00019ef0: 5f48 222c 2073 6574 7570 290a 2020 2020  _H", setup).    
+00019f00: 2020 2020 7365 6c66 2e4d 6167 5f4a 7375      self.Mag_Jsu
+00019f10: 7266 203d 204e 616d 6564 4361 6c63 4f62  rf = NamedCalcOb
+00019f20: 6a65 6374 2822 4d61 675f 4a73 7572 6622  ject("Mag_Jsurf"
+00019f30: 2c20 7365 7475 7029 0a20 2020 2020 2020  , setup).       
+00019f40: 2073 656c 662e 4d61 675f 4a76 6f6c 203d   self.Mag_Jvol =
+00019f50: 204e 616d 6564 4361 6c63 4f62 6a65 6374   NamedCalcObject
+00019f60: 2822 4d61 675f 4a76 6f6c 222c 2073 6574  ("Mag_Jvol", set
+00019f70: 7570 290a 2020 2020 2020 2020 7365 6c66  up).        self
+00019f80: 2e56 6563 746f 725f 4520 3d20 4e61 6d65  .Vector_E = Name
+00019f90: 6443 616c 634f 626a 6563 7428 2256 6563  dCalcObject("Vec
+00019fa0: 746f 725f 4522 2c20 7365 7475 7029 0a20  tor_E", setup). 
+00019fb0: 2020 2020 2020 2073 656c 662e 5665 6374         self.Vect
+00019fc0: 6f72 5f48 203d 204e 616d 6564 4361 6c63  or_H = NamedCalc
+00019fd0: 4f62 6a65 6374 2822 5665 6374 6f72 5f48  Object("Vector_H
+00019fe0: 222c 2073 6574 7570 290a 2020 2020 2020  ", setup).      
+00019ff0: 2020 7365 6c66 2e56 6563 746f 725f 4a73    self.Vector_Js
+0001a000: 7572 6620 3d20 4e61 6d65 6443 616c 634f  urf = NamedCalcO
+0001a010: 626a 6563 7428 2256 6563 746f 725f 4a73  bject("Vector_Js
+0001a020: 7572 6622 2c20 7365 7475 7029 0a20 2020  urf", setup).   
+0001a030: 2020 2020 2073 656c 662e 5665 6374 6f72       self.Vector
+0001a040: 5f4a 766f 6c20 3d20 4e61 6d65 6443 616c  _Jvol = NamedCal
+0001a050: 634f 626a 6563 7428 2256 6563 746f 725f  cObject("Vector_
+0001a060: 4a76 6f6c 222c 2073 6574 7570 290a 2020  Jvol", setup).  
+0001a070: 2020 2020 2020 7365 6c66 2e43 6f6d 706c        self.Compl
+0001a080: 6578 4d61 675f 4520 3d20 4e61 6d65 6443  exMag_E = NamedC
+0001a090: 616c 634f 626a 6563 7428 2243 6f6d 706c  alcObject("Compl
+0001a0a0: 6578 4d61 675f 4522 2c20 7365 7475 7029  exMag_E", setup)
+0001a0b0: 0a20 2020 2020 2020 2073 656c 662e 436f  .        self.Co
+0001a0c0: 6d70 6c65 784d 6167 5f48 203d 204e 616d  mplexMag_H = Nam
+0001a0d0: 6564 4361 6c63 4f62 6a65 6374 2822 436f  edCalcObject("Co
+0001a0e0: 6d70 6c65 784d 6167 5f48 222c 2073 6574  mplexMag_H", set
+0001a0f0: 7570 290a 2020 2020 2020 2020 7365 6c66  up).        self
+0001a100: 2e43 6f6d 706c 6578 4d61 675f 4a73 7572  .ComplexMag_Jsur
+0001a110: 6620 3d20 4e61 6d65 6443 616c 634f 626a  f = NamedCalcObj
+0001a120: 6563 7428 2243 6f6d 706c 6578 4d61 675f  ect("ComplexMag_
+0001a130: 4a73 7572 6622 2c20 7365 7475 7029 0a20  Jsurf", setup). 
+0001a140: 2020 2020 2020 2073 656c 662e 436f 6d70         self.Comp
+0001a150: 6c65 784d 6167 5f4a 766f 6c20 3d20 4e61  lexMag_Jvol = Na
+0001a160: 6d65 6443 616c 634f 626a 6563 7428 2243  medCalcObject("C
+0001a170: 6f6d 706c 6578 4d61 675f 4a76 6f6c 222c  omplexMag_Jvol",
+0001a180: 2073 6574 7570 290a 2020 2020 2020 2020   setup).        
+0001a190: 7365 6c66 2e50 5f4a 203d 204e 616d 6564  self.P_J = Named
+0001a1a0: 4361 6c63 4f62 6a65 6374 2822 505f 4a22  CalcObject("P_J"
+0001a1b0: 2c20 7365 7475 7029 0a0a 2020 2020 2020  , setup)..      
+0001a1c0: 2020 7365 6c66 2e6e 616d 6564 5f65 7870    self.named_exp
+0001a1d0: 7265 7373 696f 6e20 3d20 7b0a 2020 2020  ression = {.    
+0001a1e0: 2020 2020 7d20 2023 2064 6963 7469 6f6e      }  # diction
+0001a1f0: 6172 7920 746f 2068 6f6c 6420 6164 6469  ary to hold addi
+0001a200: 7469 6f6e 616c 206e 616d 6564 2065 7870  tional named exp
+0001a210: 7265 7373 696f 6e73 0a0a 2020 2020 6465  ressions..    de
+0001a220: 6620 636c 6561 725f 6e61 6d65 645f 6578  f clear_named_ex
+0001a230: 7072 6573 7369 6f6e 7328 7365 6c66 293a  pressions(self):
+0001a240: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
+0001a250: 7265 6e74 2e70 6172 656e 742e 5f66 6965  rent.parent._fie
+0001a260: 6c64 735f 6361 6c63 2e43 6c65 6172 416c  lds_calc.ClearAl
+0001a270: 6c4e 616d 6564 4578 7072 2829 0a0a 2020  lNamedExpr()..  
+0001a280: 2020 6465 6620 6465 636c 6172 655f 6e61    def declare_na
+0001a290: 6d65 645f 6578 7072 6573 7369 6f6e 2873  med_expression(s
+0001a2a0: 656c 662c 206e 616d 6529 3a0a 2020 2020  elf, name):.    
+0001a2b0: 2020 2020 2222 2222 0a20 2020 2020 2020      """".       
+0001a2c0: 2049 6620 6120 6e61 6d65 6420 6578 7072   If a named expr
+0001a2d0: 6573 7369 6f6e 2068 6173 2062 6565 6e20  ession has been 
+0001a2e0: 6372 6561 7465 6420 696e 2074 6865 2066  created in the f
+0001a2f0: 6965 6c64 7320 6361 6c63 756c 6174 6f72  ields calculator
+0001a300: 2c20 7468 6973 0a20 2020 2020 2020 2066  , this.        f
+0001a310: 756e 6374 696f 6e20 6361 6e20 6265 2063  unction can be c
+0001a320: 616c 6c65 6420 746f 2069 6e69 7469 616c  alled to initial
+0001a330: 697a 6520 7468 6520 6e61 6d65 2074 6f20  ize the name to 
+0001a340: 776f 726b 2077 6974 6820 7468 6520 6669  work with the fi
+0001a350: 656c 6473 206f 626a 6563 740a 2020 2020  elds object.    
+0001a360: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0001a370: 7365 6c66 2e6e 616d 6564 5f65 7870 7265  self.named_expre
+0001a380: 7373 696f 6e5b 6e61 6d65 5d20 3d20 4e61  ssion[name] = Na
+0001a390: 6d65 6443 616c 634f 626a 6563 7428 6e61  medCalcObject(na
+0001a3a0: 6d65 2c20 7365 6c66 2e73 6574 7570 290a  me, self.setup).
+0001a3b0: 0a20 2020 2064 6566 2075 7365 5f6e 616d  .    def use_nam
+0001a3c0: 6564 5f65 7870 7265 7373 696f 6e28 7365  ed_expression(se
+0001a3d0: 6c66 2c20 6e61 6d65 293a 0a20 2020 2020  lf, name):.     
+0001a3e0: 2020 2022 2222 0a20 2020 2020 2020 2045     """.        E
+0001a3f0: 7870 7265 7373 696f 6e20 6361 6e20 6265  xpression can be
+0001a400: 2075 7365 6420 746f 2061 6363 6573 7320   used to access 
+0001a410: 6469 6374 696f 6e61 7279 206f 6620 6e61  dictionary of na
+0001a420: 6d65 6420 6578 7072 6573 7369 6f6e 732c  med expressions,
+0001a430: 0a20 2020 2020 2020 2041 6c74 6572 6e61  .        Alterna
+0001a440: 7465 6c79 2075 7365 7220 6361 6e20 6163  tely user can ac
+0001a450: 6365 7373 2064 6963 7469 6f6e 6172 7920  cess dictionary 
+0001a460: 6469 7265 6374 6c79 2076 6961 206e 616d  directly via nam
+0001a470: 6564 5f65 7870 7265 7373 696f 6e28 290a  ed_expression().
+0001a480: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0001a490: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0001a4a0: 6e61 6d65 645f 6578 7072 6573 7369 6f6e  named_expression
+0001a4b0: 5b6e 616d 655d 0a0a 0a63 6c61 7373 2043  [name]...class C
+0001a4c0: 616c 634f 626a 6563 7428 434f 4d57 7261  alcObject(COMWra
+0001a4d0: 7070 6572 293a 0a20 2020 2064 6566 205f  pper):.    def _
+0001a4e0: 5f69 6e69 745f 5f28 7365 6c66 2c20 7374  _init__(self, st
+0001a4f0: 6163 6b2c 2073 6574 7570 293a 0a20 2020  ack, setup):.   
+0001a500: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001a510: 203a 7479 7065 2073 7461 636b 3a20 5b28   :type stack: [(
+0001a520: 7374 722c 2073 7472 295d 0a20 2020 2020  str, str)].     
+0001a530: 2020 203a 7479 7065 2073 6574 7570 3a20     :type setup: 
+0001a540: 4866 7373 5365 7475 700a 2020 2020 2020  HfssSetup.      
+0001a550: 2020 2222 220a 2020 2020 2020 2020 7375    """.        su
+0001a560: 7065 7228 4361 6c63 4f62 6a65 6374 2c20  per(CalcObject, 
+0001a570: 7365 6c66 292e 5f5f 696e 6974 5f5f 2829  self).__init__()
+0001a580: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+0001a590: 6163 6b20 3d20 7374 6163 6b0a 2020 2020  ack = stack.    
+0001a5a0: 2020 2020 7365 6c66 2e73 6574 7570 203d      self.setup =
+0001a5b0: 2073 6574 7570 0a20 2020 2020 2020 2073   setup.        s
+0001a5c0: 656c 662e 6361 6c63 5f6d 6f64 756c 6520  elf.calc_module 
+0001a5d0: 3d20 7365 7475 702e 7061 7265 6e74 2e5f  = setup.parent._
+0001a5e0: 6669 656c 6473 5f63 616c 630a 0a20 2020  fields_calc..   
+0001a5f0: 2064 6566 205f 6269 6e5f 6f70 2873 656c   def _bin_op(sel
+0001a600: 662c 206f 7468 6572 2c20 6f70 293a 0a20  f, other, op):. 
+0001a610: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+0001a620: 616e 6365 286f 7468 6572 2c20 2869 6e74  ance(other, (int
+0001a630: 2c20 666c 6f61 7429 293a 0a20 2020 2020  , float)):.     
+0001a640: 2020 2020 2020 206f 7468 6572 203d 2043         other = C
+0001a650: 6f6e 7374 616e 7443 616c 634f 626a 6563  onstantCalcObjec
+0001a660: 7428 6f74 6865 722c 2073 656c 662e 7365  t(other, self.se
+0001a670: 7475 7029 0a0a 2020 2020 2020 2020 7374  tup)..        st
+0001a680: 6163 6b20 3d20 7365 6c66 2e73 7461 636b  ack = self.stack
+0001a690: 202b 206f 7468 6572 2e73 7461 636b 0a20   + other.stack. 
+0001a6a0: 2020 2020 2020 2073 7461 636b 2e61 7070         stack.app
+0001a6b0: 656e 6428 2822 4361 6c63 4f70 222c 206f  end(("CalcOp", o
+0001a6c0: 7029 290a 2020 2020 2020 2020 7265 7475  p)).        retu
+0001a6d0: 726e 2043 616c 634f 626a 6563 7428 7374  rn CalcObject(st
+0001a6e0: 6163 6b2c 2073 656c 662e 7365 7475 7029  ack, self.setup)
+0001a6f0: 0a0a 2020 2020 6465 6620 5f75 6e61 7279  ..    def _unary
+0001a700: 5f6f 7028 7365 6c66 2c20 6f70 293a 0a20  _op(self, op):. 
+0001a710: 2020 2020 2020 2073 7461 636b 203d 2073         stack = s
+0001a720: 656c 662e 7374 6163 6b5b 3a5d 0a20 2020  elf.stack[:].   
+0001a730: 2020 2020 2073 7461 636b 2e61 7070 656e       stack.appen
+0001a740: 6428 2822 4361 6c63 4f70 222c 206f 7029  d(("CalcOp", op)
+0001a750: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001a760: 2043 616c 634f 626a 6563 7428 7374 6163   CalcObject(stac
+0001a770: 6b2c 2073 656c 662e 7365 7475 7029 0a0a  k, self.setup)..
+0001a780: 2020 2020 6465 6620 5f5f 6164 645f 5f28      def __add__(
+0001a790: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+0001a7a0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001a7b0: 662e 5f62 696e 5f6f 7028 6f74 6865 722c  f._bin_op(other,
+0001a7c0: 2022 2b22 290a 0a20 2020 2064 6566 205f   "+")..    def _
+0001a7d0: 5f72 6164 645f 5f28 7365 6c66 2c20 6f74  _radd__(self, ot
+0001a7e0: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
+0001a7f0: 7475 726e 2073 656c 6620 2b20 6f74 6865  turn self + othe
+0001a800: 720a 0a20 2020 2064 6566 205f 5f73 7562  r..    def __sub
+0001a810: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
+0001a820: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a830: 7365 6c66 2e5f 6269 6e5f 6f70 286f 7468  self._bin_op(oth
+0001a840: 6572 2c20 222d 2229 0a0a 2020 2020 6465  er, "-")..    de
+0001a850: 6620 5f5f 7273 7562 5f5f 2873 656c 662c  f __rsub__(self,
+0001a860: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+0001a870: 2072 6574 7572 6e20 282d 7365 6c66 2920   return (-self) 
+0001a880: 2b20 6f74 6865 720a 0a20 2020 2064 6566  + other..    def
+0001a890: 205f 5f6d 756c 5f5f 2873 656c 662c 206f   __mul__(self, o
+0001a8a0: 7468 6572 293a 0a20 2020 2020 2020 2072  ther):.        r
+0001a8b0: 6574 7572 6e20 7365 6c66 2e5f 6269 6e5f  eturn self._bin_
+0001a8c0: 6f70 286f 7468 6572 2c20 222a 2229 0a0a  op(other, "*")..
+0001a8d0: 2020 2020 6465 6620 5f5f 726d 756c 5f5f      def __rmul__
+0001a8e0: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
+0001a8f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001a900: 6c66 202a 206f 7468 6572 0a0a 2020 2020  lf * other..    
+0001a910: 6465 6620 5f5f 6469 765f 5f28 7365 6c66  def __div__(self
+0001a920: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+0001a930: 2020 7265 7475 726e 2073 656c 662e 5f62    return self._b
+0001a940: 696e 5f6f 7028 6f74 6865 722c 2022 2f22  in_op(other, "/"
+0001a950: 290a 0a20 2020 2064 6566 205f 5f72 6469  )..    def __rdi
+0001a960: 765f 5f28 7365 6c66 2c20 6f74 6865 7229  v__(self, other)
+0001a970: 3a0a 2020 2020 2020 2020 6f74 6865 7220  :.        other 
+0001a980: 3d20 436f 6e73 7461 6e74 4361 6c63 4f62  = ConstantCalcOb
+0001a990: 6a65 6374 286f 7468 6572 2c20 7365 6c66  ject(other, self
+0001a9a0: 2e73 6574 7570 290a 2020 2020 2020 2020  .setup).        
+0001a9b0: 7265 7475 726e 206f 7468 6572 202f 2073  return other / s
+0001a9c0: 656c 660a 0a20 2020 2064 6566 205f 5f70  elf..    def __p
+0001a9d0: 6f77 5f5f 2873 656c 662c 206f 7468 6572  ow__(self, other
+0001a9e0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+0001a9f0: 6e20 7365 6c66 2e5f 6269 6e5f 6f70 286f  n self._bin_op(o
+0001aa00: 7468 6572 2c20 2250 6f77 2229 0a0a 2020  ther, "Pow")..  
+0001aa10: 2020 6465 6620 646f 7428 7365 6c66 2c20    def dot(self, 
+0001aa20: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+0001aa30: 7265 7475 726e 2073 656c 662e 5f62 696e  return self._bin
+0001aa40: 5f6f 7028 6f74 6865 722c 2022 446f 7422  _op(other, "Dot"
+0001aa50: 290a 0a20 2020 2064 6566 205f 5f6e 6567  )..    def __neg
+0001aa60: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+0001aa70: 2020 7265 7475 726e 2073 656c 662e 5f75    return self._u
+0001aa80: 6e61 7279 5f6f 7028 224e 6567 2229 0a0a  nary_op("Neg")..
+0001aa90: 2020 2020 6465 6620 5f5f 6162 735f 5f28      def __abs__(
+0001aaa0: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
+0001aab0: 6574 7572 6e20 7365 6c66 2e5f 756e 6172  eturn self._unar
+0001aac0: 795f 6f70 2822 4162 7322 290a 0a20 2020  y_op("Abs")..   
+0001aad0: 2064 6566 205f 5f6d 6167 5f5f 2873 656c   def __mag__(sel
+0001aae0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+0001aaf0: 726e 2073 656c 662e 5f75 6e61 7279 5f6f  rn self._unary_o
+0001ab00: 7028 224d 6167 2229 0a0a 2020 2020 6465  p("Mag")..    de
+0001ab10: 6620 6d61 6728 7365 6c66 293a 0a20 2020  f mag(self):.   
+0001ab20: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001ab30: 2e5f 756e 6172 795f 6f70 2822 4d61 6722  ._unary_op("Mag"
+0001ab40: 290a 0a20 2020 2064 6566 2073 6d6f 6f74  )..    def smoot
+0001ab50: 6828 7365 6c66 293a 0a20 2020 2020 2020  h(self):.       
+0001ab60: 2072 6574 7572 6e20 7365 6c66 2e5f 756e   return self._un
+0001ab70: 6172 795f 6f70 2822 536d 6f6f 7468 2229  ary_op("Smooth")
+0001ab80: 0a0a 2020 2020 6465 6620 636f 6e6a 2873  ..    def conj(s
+0001ab90: 656c 6629 3a0a 2020 2020 2020 2020 7265  elf):.        re
+0001aba0: 7475 726e 2073 656c 662e 5f75 6e61 7279  turn self._unary
+0001abb0: 5f6f 7028 2243 6f6e 6a22 2920 2023 206d  _op("Conj")  # m
+0001abc0: 616b 6520 7468 6973 2072 6967 6874 0a0a  ake this right..
+0001abd0: 2020 2020 6465 6620 7363 616c 6172 5f78      def scalar_x
+0001abe0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001abf0: 7265 7475 726e 2073 656c 662e 5f75 6e61  return self._una
+0001ac00: 7279 5f6f 7028 2253 6361 6c61 7258 2229  ry_op("ScalarX")
+0001ac10: 0a0a 2020 2020 6465 6620 7363 616c 6172  ..    def scalar
+0001ac20: 5f79 2873 656c 6629 3a0a 2020 2020 2020  _y(self):.      
+0001ac30: 2020 7265 7475 726e 2073 656c 662e 5f75    return self._u
+0001ac40: 6e61 7279 5f6f 7028 2253 6361 6c61 7259  nary_op("ScalarY
+0001ac50: 2229 0a0a 2020 2020 6465 6620 7363 616c  ")..    def scal
+0001ac60: 6172 5f7a 2873 656c 6629 3a0a 2020 2020  ar_z(self):.    
+0001ac70: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+0001ac80: 5f75 6e61 7279 5f6f 7028 2253 6361 6c61  _unary_op("Scala
+0001ac90: 725a 2229 0a0a 2020 2020 6465 6620 6e6f  rZ")..    def no
+0001aca0: 726d 5f32 2873 656c 6629 3a0a 0a20 2020  rm_2(self):..   
+0001acb0: 2020 2020 2072 6574 7572 6e20 2873 656c       return (sel
+0001acc0: 662e 5f5f 6d61 675f 5f28 2929 2e5f 5f70  f.__mag__()).__p
+0001acd0: 6f77 5f5f 2832 290a 2020 2020 2020 2020  ow__(2).        
+0001ace0: 2320 7265 7475 726e 2073 656c 662e 5f75  # return self._u
+0001acf0: 6e61 7279 5f6f 7028 2253 6361 6c61 7258  nary_op("ScalarX
+0001ad00: 2229 2a2a 322b 7365 6c66 2e5f 756e 6172  ")**2+self._unar
+0001ad10: 795f 6f70 2822 5363 616c 6172 5922 292a  y_op("ScalarY")*
+0001ad20: 2a32 2b73 656c 662e 5f75 6e61 7279 5f6f  *2+self._unary_o
+0001ad30: 7028 2253 6361 6c61 725a 2229 2a2a 320a  p("ScalarZ")**2.
+0001ad40: 0a20 2020 2064 6566 2072 6561 6c28 7365  .    def real(se
+0001ad50: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+0001ad60: 7572 6e20 7365 6c66 2e5f 756e 6172 795f  urn self._unary_
+0001ad70: 6f70 2822 5265 616c 2229 0a0a 2020 2020  op("Real")..    
+0001ad80: 6465 6620 696d 6167 2873 656c 6629 3a0a  def imag(self):.
+0001ad90: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0001ada0: 656c 662e 5f75 6e61 7279 5f6f 7028 2249  elf._unary_op("I
+0001adb0: 6d61 6722 290a 0a20 2020 2064 6566 2063  mag")..    def c
+0001adc0: 6f6d 706c 6578 6d61 6728 7365 6c66 293a  omplexmag(self):
+0001add0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001ade0: 7365 6c66 2e5f 756e 6172 795f 6f70 2822  self._unary_op("
+0001adf0: 436d 706c 784d 6167 2229 0a0a 2020 2020  CmplxMag")..    
+0001ae00: 6465 6620 5f69 6e74 6567 7261 7465 2873  def _integrate(s
+0001ae10: 656c 662c 206e 616d 652c 2074 7970 6529  elf, name, type)
+0001ae20: 3a0a 2020 2020 2020 2020 7374 6163 6b20  :.        stack 
+0001ae30: 3d20 7365 6c66 2e73 7461 636b 202b 205b  = self.stack + [
+0001ae40: 2874 7970 652c 206e 616d 6529 2c20 2822  (type, name), ("
+0001ae50: 4361 6c63 4f70 222c 2022 496e 7465 6772  CalcOp", "Integr
+0001ae60: 6174 6522 295d 0a20 2020 2020 2020 2072  ate")].        r
+0001ae70: 6574 7572 6e20 4361 6c63 4f62 6a65 6374  eturn CalcObject
+0001ae80: 2873 7461 636b 2c20 7365 6c66 2e73 6574  (stack, self.set
+0001ae90: 7570 290a 0a20 2020 2064 6566 205f 6d61  up)..    def _ma
+0001aea0: 7869 6d75 6d28 7365 6c66 2c20 6e61 6d65  ximum(self, name
+0001aeb0: 2c20 7479 7065 293a 0a20 2020 2020 2020  , type):.       
+0001aec0: 2073 7461 636b 203d 2073 656c 662e 7374   stack = self.st
+0001aed0: 6163 6b20 2b20 5b28 7479 7065 2c20 6e61  ack + [(type, na
+0001aee0: 6d65 292c 2028 2243 616c 634f 7022 2c20  me), ("CalcOp", 
+0001aef0: 224d 6178 696d 756d 2229 5d0a 2020 2020  "Maximum")].    
+0001af00: 2020 2020 7265 7475 726e 2043 616c 634f      return CalcO
+0001af10: 626a 6563 7428 7374 6163 6b2c 2073 656c  bject(stack, sel
+0001af20: 662e 7365 7475 7029 0a0a 2020 2020 6465  f.setup)..    de
+0001af30: 6620 6765 7451 7479 2873 656c 662c 206e  f getQty(self, n
+0001af40: 616d 6529 3a0a 2020 2020 2020 2020 7374  ame):.        st
+0001af50: 6163 6b20 3d20 7365 6c66 2e73 7461 636b  ack = self.stack
+0001af60: 202b 205b 2822 456e 7465 7251 7479 222c   + [("EnterQty",
+0001af70: 206e 616d 6529 5d0a 2020 2020 2020 2020   name)].        
+0001af80: 7265 7475 726e 2043 616c 634f 626a 6563  return CalcObjec
+0001af90: 7428 7374 6163 6b2c 2073 656c 662e 7365  t(stack, self.se
+0001afa0: 7475 7029 0a0a 2020 2020 6465 6620 696e  tup)..    def in
+0001afb0: 7465 6772 6174 655f 6c69 6e65 2873 656c  tegrate_line(sel
+0001afc0: 662c 206e 616d 6529 3a0a 2020 2020 2020  f, name):.      
+0001afd0: 2020 7265 7475 726e 2073 656c 662e 5f69    return self._i
+0001afe0: 6e74 6567 7261 7465 286e 616d 652c 2022  ntegrate(name, "
+0001aff0: 456e 7465 724c 696e 6522 290a 0a20 2020  EnterLine")..   
+0001b000: 2064 6566 206e 6f72 6d61 6c32 7375 7266   def normal2surf
+0001b010: 6163 6528 7365 6c66 2c20 6e61 6d65 293a  ace(self, name):
+0001b020: 0a20 2020 2020 2020 2027 2727 2072 6574  .        ''' ret
+0001b030: 7572 6e20 7468 6520 7061 7274 206e 6f72  urn the part nor
+0001b040: 6d61 6c20 746f 2073 7572 6661 6365 2e0a  mal to surface..
+0001b050: 2020 2020 2020 2020 2020 2020 436f 6d70              Comp
+0001b060: 6c65 7820 5665 6374 6f72 2e20 2727 270a  lex Vector. '''.
+0001b070: 2020 2020 2020 2020 7374 6163 6b20 3d20          stack = 
+0001b080: 7365 6c66 2e73 7461 636b 202b 205b 2822  self.stack + [("
+0001b090: 456e 7465 7253 7572 6622 2c20 6e61 6d65  EnterSurf", name
+0001b0a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0c0: 2020 2028 2243 616c 634f 7022 2c20 2020     ("CalcOp",   
+0001b0d0: 2022 4e6f 726d 616c 2229 5d0a 2020 2020   "Normal")].    
+0001b0e0: 2020 2020 7374 6163 6b2e 6170 7065 6e64      stack.append
+0001b0f0: 2828 2243 616c 634f 7022 2c20 2244 6f74  (("CalcOp", "Dot
+0001b100: 2229 290a 2020 2020 2020 2020 7374 6163  ")).        stac
+0001b110: 6b2e 6170 7065 6e64 2828 2245 6e74 6572  k.append(("Enter
+0001b120: 5375 7266 222c 206e 616d 6529 290a 2020  Surf", name)).  
+0001b130: 2020 2020 2020 7374 6163 6b2e 6170 7065        stack.appe
+0001b140: 6e64 2828 2243 616c 634f 7022 2c20 2020  nd(("CalcOp",   
+0001b150: 2022 4e6f 726d 616c 2229 290a 2020 2020   "Normal")).    
+0001b160: 2020 2020 7374 6163 6b2e 6170 7065 6e64      stack.append
+0001b170: 2828 2243 616c 634f 7022 2c20 222a 2229  (("CalcOp", "*")
+0001b180: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001b190: 2043 616c 634f 626a 6563 7428 7374 6163   CalcObject(stac
+0001b1a0: 6b2c 2073 656c 662e 7365 7475 7029 0a0a  k, self.setup)..
+0001b1b0: 2020 2020 6465 6620 7461 6e67 656e 7432      def tangent2
+0001b1c0: 7375 7266 6163 6528 7365 6c66 2c20 6e61  surface(self, na
+0001b1d0: 6d65 293a 0a20 2020 2020 2020 2027 2727  me):.        '''
+0001b1e0: 2072 6574 7572 6e20 7468 6520 7061 7274   return the part
+0001b1f0: 2074 616e 6765 6e74 2074 6f20 7375 7266   tangent to surf
+0001b200: 6163 652e 0a20 2020 2020 2020 2020 2020  ace..           
+0001b210: 2043 6f6d 706c 6578 2056 6563 746f 722e   Complex Vector.
+0001b220: 2027 2727 0a20 2020 2020 2020 2073 7461   '''.        sta
+0001b230: 636b 203d 2073 656c 662e 7374 6163 6b20  ck = self.stack 
+0001b240: 2b20 5b28 2245 6e74 6572 5375 7266 222c  + [("EnterSurf",
+0001b250: 206e 616d 6529 2c0a 2020 2020 2020 2020   name),.        
+0001b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b270: 2020 2020 2020 2020 2822 4361 6c63 4f70          ("CalcOp
+0001b280: 222c 2020 2020 224e 6f72 6d61 6c22 295d  ",    "Normal")]
+0001b290: 0a20 2020 2020 2020 2073 7461 636b 2e61  .        stack.a
+0001b2a0: 7070 656e 6428 2822 4361 6c63 4f70 222c  ppend(("CalcOp",
+0001b2b0: 2022 446f 7422 2929 0a20 2020 2020 2020   "Dot")).       
+0001b2c0: 2073 7461 636b 2e61 7070 656e 6428 2822   stack.append(("
+0001b2d0: 456e 7465 7253 7572 6622 2c20 6e61 6d65  EnterSurf", name
+0001b2e0: 2929 0a20 2020 2020 2020 2073 7461 636b  )).        stack
+0001b2f0: 2e61 7070 656e 6428 2822 4361 6c63 4f70  .append(("CalcOp
+0001b300: 222c 2020 2020 224e 6f72 6d61 6c22 2929  ",    "Normal"))
+0001b310: 0a20 2020 2020 2020 2073 7461 636b 2e61  .        stack.a
+0001b320: 7070 656e 6428 2822 4361 6c63 4f70 222c  ppend(("CalcOp",
+0001b330: 2022 2a22 2929 0a20 2020 2020 2020 2073   "*")).        s
+0001b340: 7461 636b 203d 2073 656c 662e 7374 6163  tack = self.stac
+0001b350: 6b20 2b20 7374 6163 6b0a 2020 2020 2020  k + stack.      
+0001b360: 2020 7374 6163 6b2e 6170 7065 6e64 2828    stack.append((
+0001b370: 2243 616c 634f 7022 2c20 222d 2229 290a  "CalcOp", "-")).
+0001b380: 2020 2020 2020 2020 7265 7475 726e 2043          return C
+0001b390: 616c 634f 626a 6563 7428 7374 6163 6b2c  alcObject(stack,
+0001b3a0: 2073 656c 662e 7365 7475 7029 0a0a 2020   self.setup)..  
+0001b3b0: 2020 6465 6620 696e 7465 6772 6174 655f    def integrate_
+0001b3c0: 6c69 6e65 5f74 616e 6765 6e74 2873 656c  line_tangent(sel
+0001b3d0: 662c 206e 616d 6529 3a0a 2020 2020 2020  f, name):.      
+0001b3e0: 2020 2727 2720 696e 7465 6772 6174 6520    ''' integrate 
+0001b3f0: 6c69 6e65 2074 616e 6765 6e74 2074 6f20  line tangent to 
+0001b400: 7665 6374 6f72 2065 7870 7265 7373 696f  vector expressio
+0001b410: 6e20 5c6e 0a20 2020 2020 2020 2020 2020  n \n.           
+0001b420: 206e 616d 6520 3d20 6f66 206c 696e 6520   name = of line 
+0001b430: 746f 2069 6e74 6567 7261 7465 206f 7665  to integrate ove
+0001b440: 7220 2727 270a 2020 2020 2020 2020 7365  r '''.        se
+0001b450: 6c66 2e73 7461 636b 203d 2073 656c 662e  lf.stack = self.
+0001b460: 7374 6163 6b20 2b20 5b28 2245 6e74 6572  stack + [("Enter
+0001b470: 4c69 6e65 222c 206e 616d 6529 2c20 2822  Line", name), ("
+0001b480: 4361 6c63 4f70 222c 2022 5461 6e67 656e  CalcOp", "Tangen
+0001b490: 7422 292c 0a20 2020 2020 2020 2020 2020  t"),.           
+0001b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4b0: 2020 2020 2020 2020 2822 4361 6c63 4f70          ("CalcOp
+0001b4c0: 222c 2022 446f 7422 295d 0a20 2020 2020  ", "Dot")].     
+0001b4d0: 2020 2072 6574 7572 6e20 7365 6c66 2e69     return self.i
+0001b4e0: 6e74 6567 7261 7465 5f6c 696e 6528 6e61  ntegrate_line(na
+0001b4f0: 6d65 290a 0a20 2020 2064 6566 206c 696e  me)..    def lin
+0001b500: 655f 7461 6e67 656e 745f 636f 6f72 2873  e_tangent_coor(s
+0001b510: 656c 662c 206e 616d 652c 2063 6f6f 7264  elf, name, coord
+0001b520: 696e 6174 6529 3a0a 2020 2020 2020 2020  inate):.        
+0001b530: 2727 2720 696e 7465 6772 6174 6520 6c69  ''' integrate li
+0001b540: 6e65 2074 616e 6765 6e74 2074 6f20 7665  ne tangent to ve
+0001b550: 6374 6f72 2065 7870 7265 7373 696f 6e20  ctor expression 
+0001b560: 5c6e 0a20 2020 2020 2020 2020 2020 206e  \n.            n
+0001b570: 616d 6520 3d20 6f66 206c 696e 6520 746f  ame = of line to
+0001b580: 2069 6e74 6567 7261 7465 206f 7665 7220   integrate over 
+0001b590: 2727 270a 2020 2020 2020 2020 6966 2063  '''.        if c
+0001b5a0: 6f6f 7264 696e 6174 6520 6e6f 7420 696e  oordinate not in
+0001b5b0: 205b 2758 272c 2027 5927 2c20 275a 275d   ['X', 'Y', 'Z']
+0001b5c0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0001b5d0: 6973 6520 5661 6c75 6545 7272 6f72 0a20  ise ValueError. 
+0001b5e0: 2020 2020 2020 2073 656c 662e 7374 6163         self.stac
+0001b5f0: 6b20 3d20 7365 6c66 2e73 7461 636b 202b  k = self.stack +
+0001b600: 205b 2822 456e 7465 724c 696e 6522 2c20   [("EnterLine", 
+0001b610: 6e61 6d65 292c 2028 2243 616c 634f 7022  name), ("CalcOp"
+0001b620: 2c20 2254 616e 6765 6e74 2229 2c0a 2020  , "Tangent"),.  
+0001b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b650: 2028 2243 616c 634f 7022 2c20 2253 6361   ("CalcOp", "Sca
+0001b660: 6c61 7222 202b 2063 6f6f 7264 696e 6174  lar" + coordinat
+0001b670: 6529 5d0a 2020 2020 2020 2020 7265 7475  e)].        retu
+0001b680: 726e 2073 656c 662e 696e 7465 6772 6174  rn self.integrat
+0001b690: 655f 6c69 6e65 286e 616d 6529 0a0a 2020  e_line(name)..  
+0001b6a0: 2020 6465 6620 696e 7465 6772 6174 655f    def integrate_
+0001b6b0: 7375 7266 2873 656c 662c 206e 616d 653d  surf(self, name=
+0001b6c0: 2241 6c6c 4f62 6a65 6374 7322 293a 0a20  "AllObjects"):. 
+0001b6d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001b6e0: 6c66 2e5f 696e 7465 6772 6174 6528 6e61  lf._integrate(na
+0001b6f0: 6d65 2c20 2245 6e74 6572 5375 7266 2229  me, "EnterSurf")
+0001b700: 0a0a 2020 2020 6465 6620 696e 7465 6772  ..    def integr
+0001b710: 6174 655f 766f 6c28 7365 6c66 2c20 6e61  ate_vol(self, na
+0001b720: 6d65 3d22 416c 6c4f 626a 6563 7473 2229  me="AllObjects")
+0001b730: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001b740: 2073 656c 662e 5f69 6e74 6567 7261 7465   self._integrate
+0001b750: 286e 616d 652c 2022 456e 7465 7256 6f6c  (name, "EnterVol
+0001b760: 2229 0a0a 2020 2020 6465 6620 6d61 7869  ")..    def maxi
+0001b770: 6d75 6d5f 766f 6c28 7365 6c66 2c20 6e61  mum_vol(self, na
+0001b780: 6d65 3d27 416c 6c4f 626a 6563 7473 2729  me='AllObjects')
+0001b790: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+0001b7a0: 2073 656c 662e 5f6d 6178 696d 756d 286e   self._maximum(n
+0001b7b0: 616d 652c 2027 456e 7465 7256 6f6c 2729  ame, 'EnterVol')
+0001b7c0: 0a0a 2020 2020 6465 6620 7469 6d65 735f  ..    def times_
+0001b7d0: 6570 7328 7365 6c66 293a 0a20 2020 2020  eps(self):.     
+0001b7e0: 2020 2073 7461 636b 203d 2073 656c 662e     stack = self.
+0001b7f0: 7374 6163 6b20 2b20 5b28 2243 6c63 4d61  stack + [("ClcMa
+0001b800: 7465 7269 616c 222c 2028 2250 6572 6d69  terial", ("Permi
+0001b810: 7474 6976 6974 7920 2865 7073 6929 222c  ttivity (epsi)",
+0001b820: 2022 6d75 6c74 2229 295d 0a20 2020 2020   "mult"))].     
+0001b830: 2020 2072 6574 7572 6e20 4361 6c63 4f62     return CalcOb
+0001b840: 6a65 6374 2873 7461 636b 2c20 7365 6c66  ject(stack, self
+0001b850: 2e73 6574 7570 290a 0a20 2020 2064 6566  .setup)..    def
+0001b860: 2074 696d 6573 5f6d 7528 7365 6c66 293a   times_mu(self):
+0001b870: 0a20 2020 2020 2020 2073 7461 636b 203d  .        stack =
+0001b880: 2073 656c 662e 7374 6163 6b20 2b20 5b28   self.stack + [(
+0001b890: 2243 6c63 4d61 7465 7269 616c 222c 2028  "ClcMaterial", (
+0001b8a0: 2250 6572 6d65 6162 696c 6974 7920 286d  "Permeability (m
+0001b8b0: 7529 222c 2022 6d75 6c74 2229 295d 0a20  u)", "mult"))]. 
+0001b8c0: 2020 2020 2020 2072 6574 7572 6e20 4361         return Ca
+0001b8d0: 6c63 4f62 6a65 6374 2873 7461 636b 2c20  lcObject(stack, 
+0001b8e0: 7365 6c66 2e73 6574 7570 290a 0a20 2020  self.setup)..   
+0001b8f0: 2064 6566 2077 7269 7465 5f73 7461 636b   def write_stack
+0001b900: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0001b910: 666f 7220 666e 2c20 6172 6720 696e 2073  for fn, arg in s
+0001b920: 656c 662e 7374 6163 6b3a 0a20 2020 2020  elf.stack:.     
+0001b930: 2020 2020 2020 2069 6620 6e70 2e73 697a         if np.siz
+0001b940: 6528 6172 6729 203e 2031 2061 6e64 2066  e(arg) > 1 and f
+0001b950: 6e20 6e6f 7420 696e 205b 2745 6e74 6572  n not in ['Enter
+0001b960: 5665 6374 6f72 275d 3a0a 2020 2020 2020  Vector']:.      
+0001b970: 2020 2020 2020 2020 2020 6765 7461 7474            getatt
+0001b980: 7228 7365 6c66 2e63 616c 635f 6d6f 6475  r(self.calc_modu
+0001b990: 6c65 2c20 666e 2928 2a61 7267 290a 2020  le, fn)(*arg).  
+0001b9a0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0001b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9c0: 6765 7461 7474 7228 7365 6c66 2e63 616c  getattr(self.cal
+0001b9d0: 635f 6d6f 6475 6c65 2c20 666e 2928 6172  c_module, fn)(ar
+0001b9e0: 6729 0a0a 2020 2020 6465 6620 7361 7665  g)..    def save
+0001b9f0: 5f61 7328 7365 6c66 2c20 6e61 6d65 293a  _as(self, name):
+0001ba00: 0a20 2020 2020 2020 2022 2222 6966 2074  .        """if t
+0001ba10: 6865 206f 626a 6563 7420 616c 7265 6164  he object alread
+0001ba20: 7920 6578 6973 7473 2c20 7472 7920 636c  y exists, try cl
+0001ba30: 6561 7269 6e67 2079 6f75 720a 2020 2020  earing your.    
+0001ba40: 2020 2020 6e61 6d65 6420 6578 7072 6573      named expres
+0001ba50: 7369 6f6e 7320 6669 7273 7420 7769 7468  sions first with
+0001ba60: 2066 6965 6c64 732e 636c 6561 725f 6e61   fields.clear_na
+0001ba70: 6d65 645f 6578 7072 6573 7369 6f6e 7322  med_expressions"
+0001ba80: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
+0001ba90: 7772 6974 655f 7374 6163 6b28 290a 2020  write_stack().  
+0001baa0: 2020 2020 2020 7365 6c66 2e63 616c 635f        self.calc_
+0001bab0: 6d6f 6475 6c65 2e41 6464 4e61 6d65 6445  module.AddNamedE
+0001bac0: 7870 7228 6e61 6d65 290a 2020 2020 2020  xpr(name).      
+0001bad0: 2020 7265 7475 726e 204e 616d 6564 4361    return NamedCa
+0001bae0: 6c63 4f62 6a65 6374 286e 616d 652c 2073  lcObject(name, s
+0001baf0: 656c 662e 7365 7475 7029 0a0a 2020 2020  elf.setup)..    
+0001bb00: 6465 6620 6576 616c 7561 7465 2873 656c  def evaluate(sel
+0001bb10: 662c 2070 6861 7365 3d30 2c20 6c76 3d4e  f, phase=0, lv=N
+0001bb20: 6f6e 652c 2070 7269 6e74 5f64 6562 7567  one, print_debug
+0001bb30: 3d46 616c 7365 293a 2020 2320 2c20 6e5f  =False):  # , n_
+0001bb40: 6d6f 6465 3d31 293a 0a20 2020 2020 2020  mode=1):.       
+0001bb50: 2073 656c 662e 7772 6974 655f 7374 6163   self.write_stac
+0001bb60: 6b28 290a 2020 2020 2020 2020 6966 2070  k().        if p
+0001bb70: 7269 6e74 5f64 6562 7567 3a0a 2020 2020  rint_debug:.    
+0001bb80: 2020 2020 2020 2020 7072 696e 7428 272d          print('-
+0001bb90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001bba0: 2d2d 2d2d 2729 0a20 2020 2020 2020 2020  ----').         
+0001bbb0: 2020 2070 7269 6e74 2827 7772 6974 696e     print('writin
+0001bbc0: 6720 746f 2073 7461 636b 3a20 4f4b 2729  g to stack: OK')
+0001bbd0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0001bbe0: 6e74 2827 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  nt('------------
+0001bbf0: 2d2d 2d2d 2d27 290a 2020 2020 2020 2020  -----').        
+0001bc00: 2373 656c 662e 6361 6c63 5f6d 6f64 756c  #self.calc_modul
+0001bc10: 652e 7365 745f 6d6f 6465 286e 5f6d 6f64  e.set_mode(n_mod
+0001bc20: 652c 2030 290a 2020 2020 2020 2020 7365  e, 0).        se
+0001bc30: 7475 705f 6e61 6d65 203d 2073 656c 662e  tup_name = self.
+0001bc40: 7365 7475 702e 736f 6c75 7469 6f6e 5f6e  setup.solution_n
+0001bc50: 616d 650a 0a20 2020 2020 2020 2069 6620  ame..        if 
+0001bc60: 6c76 2069 7320 6e6f 7420 4e6f 6e65 3a0a  lv is not None:.
+0001bc70: 2020 2020 2020 2020 2020 2020 6172 6773              args
+0001bc80: 203d 206c 760a 2020 2020 2020 2020 656c   = lv.        el
+0001bc90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001bca0: 6172 6773 203d 205b 5d0a 0a20 2020 2020  args = []..     
+0001bcb0: 2020 2061 7267 732e 6170 7065 6e64 2822     args.append("
+0001bcc0: 5068 6173 653a 3d22 290a 2020 2020 2020  Phase:=").      
+0001bcd0: 2020 6172 6773 2e61 7070 656e 6428 7374    args.append(st
+0001bce0: 7228 696e 7428 7068 6173 6529 2920 2b20  r(int(phase)) + 
+0001bcf0: 2264 6567 2229 0a0a 2020 2020 2020 2020  "deg")..        
+0001bd00: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
+0001bd10: 6c66 2e73 6574 7570 2c20 4866 7373 444d  lf.setup, HfssDM
+0001bd20: 5365 7475 7029 3a0a 2020 2020 2020 2020  Setup):.        
+0001bd30: 2020 2020 6172 6773 2e65 7874 656e 6428      args.extend(
+0001bd40: 5b22 4672 6571 3a3d 222c 2073 656c 662e  ["Freq:=", self.
+0001bd50: 7365 7475 702e 736f 6c75 7469 6f6e 5f66  setup.solution_f
+0001bd60: 7265 715d 290a 0a20 2020 2020 2020 2073  req])..        s
+0001bd70: 656c 662e 6361 6c63 5f6d 6f64 756c 652e  elf.calc_module.
+0001bd80: 436c 6345 7661 6c28 7365 7475 705f 6e61  ClcEval(setup_na
+0001bd90: 6d65 2c20 6172 6773 290a 2020 2020 2020  me, args).      
+0001bda0: 2020 7265 7475 726e 2066 6c6f 6174 2873    return float(s
+0001bdb0: 656c 662e 6361 6c63 5f6d 6f64 756c 652e  elf.calc_module.
+0001bdc0: 4765 7454 6f70 456e 7472 7956 616c 7565  GetTopEntryValue
+0001bdd0: 2873 6574 7570 5f6e 616d 652c 2061 7267  (setup_name, arg
+0001bde0: 7329 5b30 5d29 0a0a 0a63 6c61 7373 204e  s)[0])...class N
+0001bdf0: 616d 6564 4361 6c63 4f62 6a65 6374 2843  amedCalcObject(C
+0001be00: 616c 634f 626a 6563 7429 3a0a 2020 2020  alcObject):.    
+0001be10: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+0001be20: 662c 206e 616d 652c 2073 6574 7570 293a  f, name, setup):
+0001be30: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
+0001be40: 6d65 203d 206e 616d 650a 2020 2020 2020  me = name.      
+0001be50: 2020 7374 6163 6b20 3d20 5b28 2243 6f70    stack = [("Cop
+0001be60: 794e 616d 6564 4578 7072 546f 5374 6163  yNamedExprToStac
+0001be70: 6b22 2c20 6e61 6d65 295d 0a20 2020 2020  k", name)].     
+0001be80: 2020 2073 7570 6572 284e 616d 6564 4361     super(NamedCa
+0001be90: 6c63 4f62 6a65 6374 2c20 7365 6c66 292e  lcObject, self).
+0001bea0: 5f5f 696e 6974 5f5f 2873 7461 636b 2c20  __init__(stack, 
+0001beb0: 7365 7475 7029 0a0a 0a63 6c61 7373 2043  setup)...class C
+0001bec0: 6f6e 7374 616e 7443 616c 634f 626a 6563  onstantCalcObjec
+0001bed0: 7428 4361 6c63 4f62 6a65 6374 293a 0a20  t(CalcObject):. 
+0001bee0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+0001bef0: 7365 6c66 2c20 6e75 6d2c 2073 6574 7570  self, num, setup
+0001bf00: 293a 0a20 2020 2020 2020 2073 7461 636b  ):.        stack
+0001bf10: 203d 205b 2822 456e 7465 7253 6361 6c61   = [("EnterScala
+0001bf20: 7222 2c20 6e75 6d29 5d0a 2020 2020 2020  r", num)].      
+0001bf30: 2020 7375 7065 7228 436f 6e73 7461 6e74    super(Constant
+0001bf40: 4361 6c63 4f62 6a65 6374 2c20 7365 6c66  CalcObject, self
+0001bf50: 292e 5f5f 696e 6974 5f5f 2873 7461 636b  ).__init__(stack
+0001bf60: 2c20 7365 7475 7029 0a0a 0a63 6c61 7373  , setup)...class
+0001bf70: 2043 6f6e 7374 616e 7456 6563 4361 6c63   ConstantVecCalc
+0001bf80: 4f62 6a65 6374 2843 616c 634f 626a 6563  Object(CalcObjec
+0001bf90: 7429 3a0a 2020 2020 6465 6620 5f5f 696e  t):.    def __in
+0001bfa0: 6974 5f5f 2873 656c 662c 2076 6563 2c20  it__(self, vec, 
+0001bfb0: 7365 7475 7029 3a0a 2020 2020 2020 2020  setup):.        
+0001bfc0: 7374 6163 6b20 3d20 5b28 2245 6e74 6572  stack = [("Enter
+0001bfd0: 5665 6374 6f72 222c 2076 6563 295d 0a20  Vector", vec)]. 
+0001bfe0: 2020 2020 2020 2073 7570 6572 2843 6f6e         super(Con
+0001bff0: 7374 616e 7456 6563 4361 6c63 4f62 6a65  stantVecCalcObje
+0001c000: 6374 2c20 7365 6c66 292e 5f5f 696e 6974  ct, self).__init
+0001c010: 5f5f 2873 7461 636b 2c20 7365 7475 7029  __(stack, setup)
+0001c020: 0a0a 0a64 6566 2067 6574 5f61 6374 6976  ...def get_activ
+0001c030: 655f 7072 6f6a 6563 7428 293a 0a20 2020  e_project():.   
+0001c040: 2027 2727 2049 6620 796f 7520 7365 6520   ''' If you see 
+0001c050: 7468 6520 6572 726f 723a 0a20 2020 2020  the error:.     
+0001c060: 2020 2022 5468 6520 7265 7175 6573 7465     "The requeste
+0001c070: 6420 6f70 6572 6174 696f 6e20 7265 7175  d operation requ
+0001c080: 6972 6573 2065 6c65 7661 7469 6f6e 2e22  ires elevation."
+0001c090: 0a20 2020 2020 2020 2074 6865 6e20 796f  .        then yo
+0001c0a0: 7520 6e65 6564 2074 6f20 7275 6e20 796f  u need to run yo
+0001c0b0: 7572 2070 7974 686f 6e20 6173 2061 6e20  ur python as an 
+0001c0c0: 6164 6d69 6e2e 0a20 2020 2027 2727 0a20  admin..    '''. 
+0001c0d0: 2020 2069 6d70 6f72 7420 6374 7970 6573     import ctypes
+0001c0e0: 0a20 2020 2069 6d70 6f72 7420 6f73 0a20  .    import os. 
+0001c0f0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001c100: 6973 5f61 646d 696e 203d 206f 732e 6765  is_admin = os.ge
+0001c110: 7475 6964 2829 203d 3d20 300a 2020 2020  tuid() == 0.    
+0001c120: 6578 6365 7074 2041 7474 7269 6275 7465  except Attribute
+0001c130: 4572 726f 723a 0a20 2020 2020 2020 2069  Error:.        i
+0001c140: 735f 6164 6d69 6e20 3d20 6374 7970 6573  s_admin = ctypes
+0001c150: 2e77 696e 646c 6c2e 7368 656c 6c33 322e  .windll.shell32.
+0001c160: 4973 5573 6572 416e 4164 6d69 6e28 2920  IsUserAnAdmin() 
+0001c170: 213d 2030 0a20 2020 2069 6620 6e6f 7420  != 0.    if not 
+0001c180: 6973 5f61 646d 696e 3a0a 2020 2020 2020  is_admin:.      
+0001c190: 2020 7072 696e 7428 275c 3033 335b 3933    print('\033[93
+0001c1a0: 6d20 5741 524e 494e 473a 2079 6f75 2061  m WARNING: you a
+0001c1b0: 7265 206e 6f74 2072 756e 6e69 6e67 2061  re not running a
+0001c1c0: 7320 616e 2061 646d 696e 2120 5c0a 2020  s an admin! \.  
+0001c1d0: 2020 2020 2020 2020 2020 596f 7520 6e65            You ne
+0001c1e0: 6564 2074 6f20 7275 6e20 6173 2061 6e20  ed to run as an 
+0001c1f0: 6164 6d69 6e2e 2059 6f75 2077 696c 6c20  admin. You will 
+0001c200: 7072 6f62 6162 6c79 2067 6574 2061 6e20  probably get an 
+0001c210: 6572 726f 7220 6e65 7874 2e5c 0a20 2020  error next.\.   
+0001c220: 2020 2020 2020 2020 2020 2020 2020 5c30                \0
+0001c230: 3333 5b30 6d27 290a 0a20 2020 2061 7070  33[0m')..    app
+0001c240: 203d 2048 6673 7341 7070 2829 0a20 2020   = HfssApp().   
+0001c250: 2064 6573 6b74 6f70 203d 2061 7070 2e67   desktop = app.g
+0001c260: 6574 5f61 7070 5f64 6573 6b74 6f70 2829  et_app_desktop()
+0001c270: 0a20 2020 2072 6574 7572 6e20 6465 736b  .    return desk
+0001c280: 746f 702e 6765 745f 6163 7469 7665 5f70  top.get_active_p
+0001c290: 726f 6a65 6374 2829 0a0a 0a64 6566 2067  roject()...def g
+0001c2a0: 6574 5f61 6374 6976 655f 6465 7369 676e  et_active_design
+0001c2b0: 2829 3a0a 2020 2020 7072 6f6a 6563 7420  ():.    project 
+0001c2c0: 3d20 6765 745f 6163 7469 7665 5f70 726f  = get_active_pro
+0001c2d0: 6a65 6374 2829 0a20 2020 2072 6574 7572  ject().    retur
+0001c2e0: 6e20 7072 6f6a 6563 742e 6765 745f 6163  n project.get_ac
+0001c2f0: 7469 7665 5f64 6573 6967 6e28 290a 0a0a  tive_design()...
+0001c300: 6465 6620 6765 745f 7265 706f 7274 5f61  def get_report_a
+0001c310: 7272 6179 7328 6e61 6d65 3a20 7374 7229  rrays(name: str)
+0001c320: 3a0a 2020 2020 6420 3d20 6765 745f 6163  :.    d = get_ac
+0001c330: 7469 7665 5f64 6573 6967 6e28 290a 2020  tive_design().  
+0001c340: 2020 7220 3d20 4866 7373 5265 706f 7274    r = HfssReport
+0001c350: 2864 2c20 6e61 6d65 290a 2020 2020 7265  (d, name).    re
+0001c360: 7475 726e 2072 2e67 6574 5f61 7272 6179  turn r.get_array
+0001c370: 7328 290a 0a0a 6465 6620 6c6f 6164 5f61  s()...def load_a
+0001c380: 6e73 7973 5f70 726f 6a65 6374 2870 726f  nsys_project(pro
+0001c390: 6a5f 6e61 6d65 3a20 7374 722c 0a20 2020  j_name: str,.   
+0001c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3b0: 2020 2020 7072 6f6a 6563 745f 7061 7468      project_path
+0001c3c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0001c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3e0: 2020 2020 2065 7874 656e 7369 6f6e 3a20       extension: 
+0001c3f0: 7374 7220 3d20 272e 6165 6474 2729 3a0a  str = '.aedt'):.
+0001c400: 2020 2020 2727 270a 2020 2020 5574 696c      '''.    Util
+0001c410: 6974 7920 6675 6e63 7469 6f6e 2074 6f20  ity function to 
+0001c420: 6c6f 6164 2061 6e20 416e 7379 7320 7072  load an Ansys pr
+0001c430: 6f6a 6563 742e 0a0a 2020 2020 4172 6773  oject...    Args
+0001c440: 3a0a 2020 2020 2020 2020 7072 6f6a 5f6e  :.        proj_n
+0001c450: 616d 6520 3a20 4e6f 6e65 2020 2d2d 3e20  ame : None  --> 
+0001c460: 6765 7420 6163 7469 7665 2e20 286d 616b  get active. (mak
+0001c470: 6520 7375 7265 2032 2072 756e 2061 7320  e sure 2 run as 
+0001c480: 6164 6d69 6e29 0a20 2020 2020 2020 2065  admin).        e
+0001c490: 7874 656e 7369 6f6e 203a 2060 6165 6474  xtension : `aedt
+0001c4a0: 6020 6973 2066 6f72 2032 3031 3620 7665  ` is for 2016 ve
+0001c4b0: 7273 696f 6e20 616e 6420 6e65 7765 720a  rsion and newer.
+0001c4c0: 2020 2020 2727 270a 2020 2020 6966 2070      '''.    if p
+0001c4d0: 726f 6a65 6374 5f70 6174 683a 0a20 2020  roject_path:.   
+0001c4e0: 2020 2020 2023 2063 6f6e 7665 7274 2073       # convert s
+0001c4f0: 6c61 7368 6573 2063 6f72 7265 6374 6c79  lashes correctly
+0001c500: 2066 6f72 2073 7973 7465 6d0a 2020 2020   for system.    
+0001c510: 2020 2020 7072 6f6a 6563 745f 7061 7468      project_path
+0001c520: 203d 2050 6174 6828 7072 6f6a 6563 745f   = Path(project_
+0001c530: 7061 7468 290a 0a20 2020 2020 2020 2023  path)..        #
+0001c540: 2043 6865 636b 730a 2020 2020 2020 2020   Checks.        
+0001c550: 6173 7365 7274 2070 726f 6a65 6374 5f70  assert project_p
+0001c560: 6174 682e 6973 5f64 6972 280a 2020 2020  ath.is_dir(.    
+0001c570: 2020 2020 292c 2022 4552 524f 5221 2070      ), "ERROR! p
+0001c580: 726f 6a65 6374 5f70 6174 6820 6973 206e  roject_path is n
+0001c590: 6f74 2061 2076 616c 6964 2064 6972 6563  ot a valid direc
+0001c5a0: 746f 7279 205c 4e7b 6c6f 7564 6c79 2063  tory \N{loudly c
+0001c5b0: 7279 696e 6720 6661 6365 7d2e 5c0a 2020  rying face}.\.  
+0001c5c0: 2020 2020 2020 2020 2020 4368 6563 6b20            Check 
+0001c5d0: 7468 6520 7061 7468 2c20 616e 6420 6573  the path, and es
+0001c5e0: 7065 6369 616c 6c79 205c 5c20 6368 6172  pecially \\ char
+0001c5f0: 6163 7465 7273 2e22 0a0a 2020 2020 2020  acters."..      
+0001c600: 2020 7072 6f6a 6563 745f 7061 7468 202f    project_path /
+0001c610: 3d20 7072 6f6a 6563 745f 7061 7468 202f  = project_path /
+0001c620: 2050 6174 6828 7072 6f6a 5f6e 616d 6520   Path(proj_name 
+0001c630: 2b20 6578 7465 6e73 696f 6e29 0a0a 2020  + extension)..  
+0001c640: 2020 2020 2020 6966 2028 7072 6f6a 6563        if (projec
+0001c650: 745f 7061 7468 292e 6973 5f66 696c 6528  t_path).is_file(
+0001c660: 293a 0a20 2020 2020 2020 2020 2020 206c  ):.            l
+0001c670: 6f67 6765 722e 696e 666f 2827 5c74 4669  ogger.info('\tFi
+0001c680: 6c65 2070 6174 6820 746f 2048 4653 5320  le path to HFSS 
+0001c690: 7072 6f6a 6563 7420 666f 756e 642e 2729  project found.')
+0001c6a0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0001c6b0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0001c6c0: 2045 7863 6570 7469 6f6e 280a 2020 2020   Exception(.    
+0001c6d0: 2020 2020 2020 2020 2020 2020 2245 5252              "ERR
+0001c6e0: 4f52 2120 5661 6c69 6420 6469 7265 6374  OR! Valid direct
+0001c6f0: 6f72 792c 2062 7574 2069 6e76 616c 6964  ory, but invalid
+0001c700: 2070 726f 6a65 6374 2066 696c 656e 616d   project filenam
+0001c710: 652e 205c 4e7b 6c6f 7564 6c79 2063 7279  e. \N{loudly cry
+0001c720: 696e 6720 6661 6365 7d20 4e6f 7420 666f  ing face} Not fo
+0001c730: 756e 6421 5c0a 2020 2020 2020 2020 2020  und!\.          
+0001c740: 2020 2020 2020 2020 2020 2050 6c65 6173             Pleas
+0001c750: 6520 6368 6563 6b20 796f 7572 2066 696c  e check your fil
+0001c760: 656e 616d 652e 5c6e 2573 5c6e 2220 2520  ename.\n%s\n" % 
+0001c770: 7072 6f6a 6563 745f 7061 7468 290a 0a20  project_path).. 
+0001c780: 2020 2020 2020 2069 6620 2870 726f 6a65         if (proje
+0001c790: 6374 5f70 6174 6820 2f20 272e 6c6f 636b  ct_path / '.lock
+0001c7a0: 2729 2e69 735f 6669 6c65 2829 3a0a 2020  ').is_file():.  
+0001c7b0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0001c7c0: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+0001c7d0: 2020 2020 2020 2020 2020 275c 745c 7446            '\t\tF
+0001c7e0: 696c 6520 6973 206c 6f63 6b65 642e 205c  ile is locked. \
+0001c7f0: 4e7b 6665 6172 6675 6c20 6661 6365 7d20  N{fearful face} 
+0001c800: 4966 2063 6f6e 6e65 6374 696f 6e20 6661  If connection fa
+0001c810: 696c 732c 2064 656c 6574 6520 7468 6520  ils, delete the 
+0001c820: 2e6c 6f63 6b20 6669 6c65 2e27 0a20 2020  .lock file.'.   
+0001c830: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0001c840: 6170 7020 3d20 4866 7373 4170 7028 290a  app = HfssApp().
+0001c850: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+0001c860: 225c 744f 7065 6e65 6420 416e 7379 7320  "\tOpened Ansys 
+0001c870: 4170 7022 290a 0a20 2020 2064 6573 6b74  App")..    deskt
+0001c880: 6f70 203d 2061 7070 2e67 6574 5f61 7070  op = app.get_app
+0001c890: 5f64 6573 6b74 6f70 2829 0a20 2020 206c  _desktop().    l
+0001c8a0: 6f67 6765 722e 696e 666f 2866 225c 744f  ogger.info(f"\tO
+0001c8b0: 7065 6e65 6420 416e 7379 7320 4465 736b  pened Ansys Desk
+0001c8c0: 746f 7020 767b 6465 736b 746f 702e 6765  top v{desktop.ge
+0001c8d0: 745f 7665 7273 696f 6e28 297d 2229 0a20  t_version()}"). 
+0001c8e0: 2020 2023 6c6f 6767 6572 2e64 6562 7567     #logger.debug
+0001c8f0: 2866 225c 744f 7065 6e20 7072 6f6a 6563  (f"\tOpen projec
+0001c900: 7473 3a20 7b64 6573 6b74 6f70 2e67 6574  ts: {desktop.get
+0001c910: 5f70 726f 6a65 6374 5f6e 616d 6573 2829  _project_names()
+0001c920: 7d22 290a 0a20 2020 2069 6620 7072 6f6a  }")..    if proj
+0001c930: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
+0001c940: 653a 0a20 2020 2020 2020 2069 6620 7072  e:.        if pr
+0001c950: 6f6a 5f6e 616d 6520 696e 2064 6573 6b74  oj_name in deskt
+0001c960: 6f70 2e67 6574 5f70 726f 6a65 6374 5f6e  op.get_project_n
+0001c970: 616d 6573 2829 3a0a 2020 2020 2020 2020  ames():.        
+0001c980: 2020 2020 6465 736b 746f 702e 7365 745f      desktop.set_
+0001c990: 6163 7469 7665 5f70 726f 6a65 6374 2870  active_project(p
+0001c9a0: 726f 6a5f 6e61 6d65 290a 2020 2020 2020  roj_name).      
+0001c9b0: 2020 2020 2020 7072 6f6a 6563 7420 3d20        project = 
+0001c9c0: 6465 736b 746f 702e 6765 745f 6163 7469  desktop.get_acti
+0001c9d0: 7665 5f70 726f 6a65 6374 2829 0a20 2020  ve_project().   
+0001c9e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001c9f0: 2020 2020 2020 2070 726f 6a65 6374 203d         project =
+0001ca00: 2064 6573 6b74 6f70 2e6f 7065 6e5f 7072   desktop.open_pr
+0001ca10: 6f6a 6563 7428 7374 7228 7072 6f6a 6563  oject(str(projec
+0001ca20: 745f 7061 7468 2929 0a20 2020 2065 6c73  t_path)).    els
+0001ca30: 653a 0a20 2020 2020 2020 2070 726f 6a65  e:.        proje
+0001ca40: 6374 735f 696e 5f61 7070 203d 2064 6573  cts_in_app = des
+0001ca50: 6b74 6f70 2e67 6574 5f70 726f 6a65 6374  ktop.get_project
+0001ca60: 7328 290a 2020 2020 2020 2020 6966 2070  s().        if p
+0001ca70: 726f 6a65 6374 735f 696e 5f61 7070 3a0a  rojects_in_app:.
+0001ca80: 2020 2020 2020 2020 2020 2020 7072 6f6a              proj
+0001ca90: 6563 7420 3d20 6465 736b 746f 702e 6765  ect = desktop.ge
+0001caa0: 745f 6163 7469 7665 5f70 726f 6a65 6374  t_active_project
+0001cab0: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+0001cac0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+0001cad0: 6a65 6374 203d 204e 6f6e 650a 0a20 2020  ject = None..   
+0001cae0: 2069 6620 7072 6f6a 6563 743a 0a20 2020   if project:.   
+0001caf0: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0001cb00: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+0001cb10: 5c74 4f70 656e 6564 2041 6e73 7973 2050  \tOpened Ansys P
+0001cb20: 726f 6a65 6374 5c6e 5c74 466f 6c64 6572  roject\n\tFolder
+0001cb30: 3a20 2020 207b 7072 6f6a 6563 742e 6765  :    {project.ge
+0001cb40: 745f 7061 7468 2829 7d5c 6e5c 7450 726f  t_path()}\n\tPro
+0001cb50: 6a65 6374 3a20 2020 7b70 726f 6a65 6374  ject:   {project
+0001cb60: 2e6e 616d 657d 220a 2020 2020 2020 2020  .name}".        
+0001cb70: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+0001cb80: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+0001cb90: 6622 5c74 416e 7379 7320 5072 6f6a 6563  f"\tAnsys Projec
+0001cba0: 7420 7761 7320 6e6f 7420 666f 756e 642e  t was not found.
+0001cbb0: 5c6e 5c74 2050 726f 6a65 6374 2069 7320  \n\t Project is 
+0001cbc0: 4e6f 6e65 2e22 290a 0a20 2020 2072 6574  None.")..    ret
+0001cbd0: 7572 6e20 6170 702c 2064 6573 6b74 6f70  urn app, desktop
+0001cbe0: 2c20 7072 6f6a 6563 740a                 , project.
```

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/calcs/back_box_numeric.py` & `pyEPR-quantum-0.9.0/pyEPR/calcs/back_box_numeric.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     freqs, Ljs, ϕzpf = map(np.array, (freqs, Ljs, ϕzpf))
     assert(all(freqs < 1E6)
            ), "Please input the frequencies in GHz. \N{nauseated face}"
     assert(all(Ljs < 1E-3)
            ), "Please input the inductances in Henries. \N{nauseated face}"
 
-    Hs = black_box_hamiltonian(freqs * 1E9, Ljs.astype(np.float), fluxQ*ϕzpf,
+    Hs = black_box_hamiltonian(freqs * 1E9, Ljs.astype(float), fluxQ*ϕzpf,
                                cos_trunc, fock_trunc, individual=use_1st_order,
                                non_linear_potential = non_linear_potential)
     f_ND, χ_ND, _, _ = make_dispersive(
         Hs, fock_trunc, ϕzpf, freqs, use_1st_order=use_1st_order)
     χ_ND = -1*χ_ND * 1E-6  # convert to MHz, and flip sign so that down shift is positive
 
     return (f_ND, χ_ND, Hs) if return_H else (f_ND, χ_ND)
```

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/calcs/basic.py` & `pyEPR-quantum-0.9.0/pyEPR/calcs/basic.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/calcs/convert.py` & `pyEPR-quantum-0.9.0/pyEPR/calcs/convert.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/calcs/hamiltonian.py` & `pyEPR-quantum-0.9.0/pyEPR/calcs/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/calcs/quantum.py` & `pyEPR-quantum-0.9.0/pyEPR/calcs/quantum.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/calcs/transmon.py` & `pyEPR-quantum-0.9.0/pyEPR/calcs/transmon.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/core.py` & `pyEPR-quantum-0.9.0/pyEPR/core.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/core_distributed_analysis.py` & `pyEPR-quantum-0.9.0/pyEPR/core_distributed_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -653,39 +653,39 @@
 
         lv = self._get_lv(variation)
         return A.evaluate(lv=lv)
 
     def calc_p_electric_volume(self,
                                name_dielectric3D,
                                relative_to='AllObjects',
+                               variation=None,
                                E_total=None
                                ):
         r'''
-        Calculate the dielectric energy-participatio ratio
+        Calculate the dielectric energy-participation ratio
         of a 3D object (one that has volume) relative to the dielectric energy of
-        a list of object objects.
+        a list of objects.
 
         This is as a function relative to another object or all objects.
 
         When all objects are specified, this does not include any energy
         that might be stored in any lumped elements or lumped capacitors.
 
         Returns:
-        ---------
             ℰ_object/ℰ_total, (ℰ_object, _total)
         '''
 
         if E_total is None:
             logger.debug('Calculating ℰ_total')
-            ℰ_total = self.calc_energy_electric(obj=relative_to)
+            ℰ_total = self.calc_energy_electric(obj=relative_to, variation=variation)
         else:
             ℰ_total = E_total
 
         logger.debug('Calculating ℰ_object')
-        ℰ_object = self.calc_energy_electric(obj=name_dielectric3D)
+        ℰ_object = self.calc_energy_electric(obj=name_dielectric3D, variation=variation)
 
         return ℰ_object/ℰ_total, (ℰ_object, ℰ_total)
 
     def calc_current(self, fields, line: str):
         '''
         Function to calculate Current based on line. Not in use.
 
@@ -874,45 +874,47 @@
         Qdielectric = OrderedDict()
         print('Calculating Qdielectric_' + dielectric + ' for mode ' +
               str(mode) + ' (' + str(mode) + '/' + str(self.n_modes-1) + ')')
 
         U_dielectric = self.calc_energy_electric(variation, obj=dielectric)
         p_dielectric = U_dielectric/U_E
         # TODO: Update make p saved sep. and get Q for diff materials, indep. specify in pinfo
-        Qdielectric['Qdielectric_'+dielectric+'_' +
-                    str(mode)] = 1/(p_dielectric*config.dissipation.tan_delta_sapp)
-        print('p_dielectric'+'_'+dielectric+'_' +
-              str(mode)+' = ' + str(p_dielectric))
+        Qdielectric['Qdielectric_' + dielectric] = 1/(p_dielectric*config.dissipation.tan_delta_sapp)
+        print('p_dielectric'+'_'+dielectric+'_' + str(mode) + ' = ' + str(p_dielectric))
         return pd.Series(Qdielectric)
 
-    def get_Qsurface(self, mode, variation, name, U_E=None):
+    def get_Qsurface(self, mode, variation, name, U_E=None, material_properties=None):
         '''
         Calculate the contribution to Q of a dielectric layer of dirt on a given surface.
         Set the dirt thickness and loss tangent in the config file
         ref: http://arxiv.org/pdf/1509.01854.pdf
         '''
         if U_E is None:
             U_E = self.calc_energy_electric(variation)
+        if material_properties is None:
+            material_properties = {}
+        th = material_properties.get('th', config.dissipation.th)
+        eps_r = material_properties.get('eps_r', config.dissipation.eps_r)
+        tan_delta_surf = material_properties.get('tan_delta_surf', config.dissipation.tan_delta_surf)
+
         lv = self._get_lv(variation)
         Qsurf = OrderedDict()
-        print('Calculating Qsurface for mode ' + str(mode) +
-              ' (' + str(mode) + '/' + str(self.n_modes-1) + ')')
+        print(f'Calculating Qsurface {name} for mode ({mode}/{self.n_modes-1})')
         calcobject = CalcObject([], self.setup)
         vecE = calcobject.getQty("E")
         A = vecE
         B = vecE.conj()
         A = A.dot(B)
         A = A.real()
         A = A.integrate_surf(name=name)
         U_surf = A.evaluate(lv=lv)
-        U_surf *= config.dissipation.th*epsilon_0*config.dissipation.eps_r
+        U_surf *= th * epsilon_0 * eps_r
         p_surf = U_surf/U_E
-        Qsurf['Qsurf_'+str(mode)] = 1 / \
-            (p_surf*config.dissipation.tan_delta_surf)
-        print('p_surf'+'_'+str(mode)+' = ' + str(p_surf))
+        Qsurf[f'Qsurf_{name}'] = 1 / (p_surf * tan_delta_surf)
+        print(f'p_surf_{name}_{mode} = {p_surf}')
         return pd.Series(Qsurf)
 
     def get_Qsurface_all(self, mode, variation, U_E=None):
         '''
         Calculate the contribution to Q of a dielectric layer of dirt on all surfaces.
         Set the dirt thickness and loss tangent in the config file
         ref: http://arxiv.org/pdf/1509.01854.pdf
@@ -926,15 +928,15 @@
 
         Args:
             variation (str): A string identifier of the variation,
             such as '0', '1', ...
         '''
         if U_E is None:
             U_E = self.calc_energy_electric(variation)
-        Qp = pd.Series({})
+        Qp = pd.Series({}, dtype='float64')
 
         freq = freq_GHz * 1e9  # freq in Hz
         for port_nm, port in self.pinfo.ports.items():
             I_peak = self.calc_avg_current_J_surf_mag(variation, port['rect'],
                                                       port['line'])
             U_dissip = 0.5 * port['R'] * I_peak**2 * 1 / freq
             p = U_dissip / (U_E/2)  # U_E is 2x the peak electrical energy
@@ -974,15 +976,15 @@
         '''
 
         # ------------------------------------------------------------
         # Calculate all peak voltage and currents for all junctions in a given mode
         method = self.pinfo.options.method_calc_P_mj
         I_peak_ = {}
         V_peak_ = {}
-        Sj = pd.Series({})
+        Sj = pd.Series({}, dtype='float64')
         for j_name, j_props in self.pinfo.junctions.items():
             logger.debug(f'Calculating participations for {(j_name, j_props)}')
             Lj = Ljs[j_name]
             Cj = Cjs[j_name]
             line_name = j_props['line']
 
             if method == 'J_surf_mag':  # old method
@@ -1094,16 +1096,16 @@
             variation (str) : label such as '0' or 'all', in which case return
             pandas table for all variations
         """
         if variation == 'all':
             # for all variations and concat
             raise NotImplementedError()  # TODO
         else:
-            Ljs = pd.Series({})
-            Cjs = pd.Series({})
+            Ljs = pd.Series({}, dtype='float64')
+            Cjs = pd.Series({}, dtype='float64')
 
             for junc_name, val in self.pinfo.junctions.items():  # junction nickname
                 _variables = self._hfss_variables[variation]
                 def _parse(name): return ureg.Quantity(
                     _variables['_'+val[name]]).to_base_units().magnitude
                 Ljs[junc_name] = _parse('Lj_variable')
                 Cjs[junc_name] = 2E-15  # _parse(
@@ -1238,15 +1240,15 @@
 
             for mode in modes:  # integer of mode number [0,1,2,3,..]
 
                 # Load fields for mode
                 self.set_mode(mode)
 
                 # Get HFSS  solved frequencies
-                _Om = pd.Series({})
+                _Om = pd.Series({}, dtype='float64')
                 temp_freq = freqs_bare_GHz[mode]
                 _Om['freq_GHz'] = temp_freq  # freq
                 Om[mode] = _Om
                 print(
                     '\n'f'  \033[1mMode {mode} at {"%.2f" % temp_freq} GHz   [{mode+1}/{self.n_modes}]\033[0m')
 
                 # EPR Hamiltonian calculations
@@ -1295,34 +1297,28 @@
                 Qm_coupling[mode] = self.calc_Q_external(variation,
                                                          freqs_bare_GHz[mode],
                                                          self.U_E)
 
                 # get seam Q
                 if self.pinfo.dissipative['seams']:
                     for seam in self.pinfo.dissipative['seams']:
-                        sol = sol.append(self.get_Qseam(seam, mode, variation, self.U_H))
+                        sol = pd.concat([sol, self.get_Qseam(seam, mode, variation, self.U_H)])
 
                 # get Q dielectric
                 if self.pinfo.dissipative['dielectrics_bulk']:
                     for dielectric in self.pinfo.dissipative['dielectrics_bulk']:
-                        sol = sol.append(self.get_Qdielectric(
-                            dielectric, mode, variation, self.U_E))
+                        sol = pd.concat([sol, self.get_Qdielectric(dielectric, mode, variation, self.U_E)])
 
                 # get Q surface
-                if self.pinfo.dissipative['resistive_surfaces']:
-                    if self.pinfo.dissipative['resistive_surfaces'] == 'all':
-                        sol = sol.append(
-                            self.get_Qsurface_all(mode, variation, self.U_E))
+                if self.pinfo.dissipative['dielectric_surfaces']:
+                    if self.pinfo.dissipative['dielectric_surfaces'] == 'all':
+                        sol = pd.concat([sol, self.get_Qsurface_all(mode, variation, self.U_E)])
                     else:
-                        raise NotImplementedError(
-                            "Join the team, by helping contribute this piece of code.")
-
-                if self.pinfo.dissipative['resistive_surfaces'] is not None:
-                    raise NotImplementedError(
-                        "Join the team, by helping contribute this piece of code.")
+                        for surface, properties in self.pinfo.dissipative['dielectric_surfaces'].items():
+                            sol = pd.concat([sol, self.get_Qsurface(mode, variation, surface, self.U_E, properties)])
 
                 SOL[mode] = sol
 
             # Save
             self._update_results(variation, Om, Pm, Sm, Qm_coupling, SOL,
                                  freqs_bare_GHz, Qs_bare, Ljs, Cjs,
                                  Pm_cap, I_peak, V_peak,
@@ -1621,15 +1617,15 @@
             gs = mpl.gridspec.GridSpec(1, 3, width_ratios=[1.2, 1.5, 1])
             axs = [fig.add_subplot(gs[i]) for i in range(3)]
 
             logger.info(f'Creating report for variation {variation}')
             convergence_t = self.get_convergence(variation=variation)
             convergence_f = self.hfss_report_f_convergence(variation=variation)
 
-            axs[0].set_ylabel(variation_labels, fontsize='large')  # add variation labels to y-axis of first plot
+            axs[0].set_ylabel(variation_labels.replace(' ', '\n'))  # add variation labels to y-axis of first plot
 
             ax0t = axs[1].twinx()
             plot_convergence_f_vspass(axs[0], convergence_f)
             plot_convergence_max_df(axs[1], convergence_t.iloc[:, 1])
             plot_convergence_solved_elem(ax0t, convergence_t.iloc[:, 0])
             plot_convergence_maxdf_vs_sol(axs[2], convergence_t.iloc[:, 1],
                                           convergence_t.iloc[:, 0])
```

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/core_quantum_analysis.py` & `pyEPR-quantum-0.9.0/pyEPR/core_quantum_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     It is a dictionary based class to contain the results stored.
     """
 
     file_name_extra = ' HamiltonianResultsContainer.npz'
 
     def __init__(self, dict_file=None, data_dir=None):
         """ input:
-           dict file - 1. ethier None to create an empty results hamiltonian as
+           dict file - 1. either None to create an empty results hamiltonian as
                        as was done in the original code
 
                        2. or a string with the name of the file where the file of the
                        previously saved HamiltonianResultsContainer instance we wish
                        to load
 
                        3. or an existing instance of a dict class which will be
@@ -660,19 +660,18 @@
             PJ = PJ[:, junctions]
             SJ = SJ[:, junctions]
             EJ = EJ[:, junctions][junctions, :]
             PHI_zpf = PHI_zpf[:, junctions]
             PJ_cap = PJ_cap[:, junctions]
 
         if modes is not None:
-            freqs_hfss = freqs_hfss[range(len(self.modes[variation])), ]
-            PJ = PJ[range(len(modes)), :]
-            SJ = SJ[range(len(modes)), :]
-            Om = Om[range(len(modes)), :][:, range(len(modes))]
-            PHI_zpf = PHI_zpf[range(len(modes)), :]
+            PJ = PJ[modes, :]
+            SJ = SJ[modes, :]
+            Om = Om[modes, :][:, modes]
+            PHI_zpf = PHI_zpf[modes, :]
             PJ_cap = PJ_cap[:, junctions]
 
         # Analytic 4-th order
         CHI_O1 = 0.25 * Om @ PJ @ inv(EJ) @ PJ.T @ Om * 1000.  # MHz
         f1s = np.diag(Om) - 0.5*np.ndarray.flatten(np.array(CHI_O1.sum(1))) / \
             1000.                  # 1st order PT expect freq to be dressed down by alpha
         CHI_O1 = divide_diagonal_by_2(CHI_O1)   # Make the diagonals alpha
@@ -707,20 +706,23 @@
         # just propagate
         result['hfss_variables'] = self._hfss_variables[variation]
         result['Ljs'] = self.Ljs[variation]
         result['Cjs'] = self.Cjs[variation]
         try:
             result['Q_coupling'] = self.Qm_coupling[variation][self.Qm_coupling[variation].columns[junctions]][modes]#TODO change the columns to junctions
         except:
-             result['Q_coupling'] = self.Qm_coupling[variation]
+            result['Q_coupling'] = self.Qm_coupling[variation]
         
         try:
             result['Qs'] = self.Qs[variation][self.PM[variation].columns[junctions]][modes] #TODO change the columns to junctions
         except:
-             result['Qs'] = self.Qs[variation][modes]
+            result['Qs'] = self.Qs[variation][modes]
+
+        result['sol'] = self.sols[variation]
+
         result['fock_trunc'] = fock_trunc
         result['cos_trunc'] = cos_trunc
 
         self.results[variation] = result
         self.results.save()
         
         if print_result:
@@ -729,15 +731,16 @@
     
         self.n_modes = tmp_n_modes # TODO is this smart should consider defining the modes of interest in the initialisation of the quantum object
         self.modes[variation]=tmp_modes 
         return result
 
     def full_report_variations(self, var_list: list=None):
         """see full_variation_report"""
-        if var_list is None: var_list =self.variations
+        if var_list is None:
+            var_list = self.variations
         for variation in var_list: 
             self.full_variation_report(variation)
     
     def full_variation_report(self, variation):
         """
         prints the results and parameters of a specific variation
```

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/project_info.py` & `pyEPR-quantum-0.9.0/pyEPR/project_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,18 +116,20 @@
             for opt in diss_opt:
                 self[opt] = None
 
         def __setitem__(self, key, value):
             # --- check valid inputs ---
             if not (key in diss_opt or key == 'pinfo'):
                 raise ValueError(f"No such parameter {key}")
-            if key != 'pinfo' and (not isinstance(value, list) or \
+            if key != 'pinfo' and (not isinstance(value, (list, dict)) or \
                     not all(isinstance(x, str) for x in value)) and (value != None):
                 raise ValueError(f'dissipative[\'{key}\'] must be a list of strings ' \
-                    'containing names of models in the project!')
+                    'containing names of models in the project or dictionary of strings of models containing ' \
+                    'material loss properties!'
+                )
             if key != 'pinfo' and hasattr(self['pinfo'], 'design'):
                 for x in value:
                     if x not in self['pinfo'].get_all_object_names():
                         raise ValueError(
                             f'\'{x}\' is not an object in the HFSS project')
             super().__setattr__(key, value)
 
@@ -232,15 +234,15 @@
     def save(self):
         '''
         Return all the data in a dictionary form that can be used to be saved
         '''
         return dict(
             pinfo=pd.Series(get_instance_vars(self, self._Forbidden)),
             dissip=pd.Series(self.dissipative.data()),
-            options=pd.Series(get_instance_vars(self.options)),
+            options=pd.Series(get_instance_vars(self.options), dtype='object'),
             junctions=pd.DataFrame(self.junctions),
             ports=pd.DataFrame(self.ports),
         )
 
     def connect_project(self):
         """Sets 
         self.app
```

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/reports.py` & `pyEPR-quantum-0.9.0/pyEPR/reports.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/toolbox/_logging.py` & `pyEPR-quantum-0.9.0/pyEPR/toolbox/_logging.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/toolbox/plotting.py` & `pyEPR-quantum-0.9.0/pyEPR/toolbox/plotting.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR/toolbox/pythonic.py` & `pyEPR-quantum-0.9.0/pyEPR/toolbox/pythonic.py`

 * *Files identical despite different names*

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR_quantum.egg-info/PKG-INFO` & `pyEPR-quantum-0.9.0/pyEPR_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyEPR-quantum
-Version: 0.8.5.7
+Version: 0.9.0
 Home-page: https://github.com/zlatko-minev/pyEPR
 Author: Zlatko K. Minev
 Author-email: zlatko.minev@aya.yale.edu
 Maintainer: Zlatko Minev, pyEPR team
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pyEPR-quantum-0.8.5.7/pyEPR_quantum.egg-info/SOURCES.txt` & `pyEPR-quantum-0.9.0/pyEPR_quantum.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -23,8 +23,10 @@
 pyEPR/toolbox/_logging.py
 pyEPR/toolbox/plotting.py
 pyEPR/toolbox/pythonic.py
 pyEPR_quantum.egg-info/PKG-INFO
 pyEPR_quantum.egg-info/SOURCES.txt
 pyEPR_quantum.egg-info/dependency_links.txt
 pyEPR_quantum.egg-info/requires.txt
-pyEPR_quantum.egg-info/top_level.txt
+pyEPR_quantum.egg-info/top_level.txt
+tests/test_project_info.py
+tests/test_quantum_analysis.py
```

### Comparing `pyEPR-quantum-0.8.5.7/setup.py` & `pyEPR-quantum-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 with open(here / "requirements.txt", encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
 doclines = __doc__.split('\n')
 
 setup(
     name='pyEPR-quantum',
-    version='0.8.5.7',
+    version='0.9.0',
     description=doclines[0],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Zlatko K. Minev',
     packages=find_packages(),
     author_email='zlatko.minev@aya.yale.edu',
     maintainer='Zlatko Minev, pyEPR team',
```

