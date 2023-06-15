# Comparing `tmp/EclipsingBinaries-2.8.4a8.tar.gz` & `tmp/EclipsingBinaries-2.8.4a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-2.8.4a8.tar", last modified: Fri May 19 16:50:17 2023, max compression
+gzip compressed data, was "EclipsingBinaries-2.8.4a9.tar", last modified: Tue Jun 13 02:29:56 2023, max compression
```

## Comparing `EclipsingBinaries-2.8.4a8.tar` & `EclipsingBinaries-2.8.4a9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-19 16:49:57.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-19 16:50:17.000000 EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:50:17.500394 EclipsingBinaries-2.8.4a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-19 16:50:03.000000 EclipsingBinaries-2.8.4a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.087896 EclipsingBinaries-2.8.4a9/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20561 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22282 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-06-13 02:29:36.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    31361 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25814 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30132 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39669 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173787 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 02:29:56.000000 EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 02:29:56.091896 EclipsingBinaries-2.8.4a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-13 02:29:42.000000 EclipsingBinaries-2.8.4a9/setup.py
```

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/IRAF_Reduction.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/OC_plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,93 @@
 """
 Author: Kyle Koeller
 Created: 12/19/2022
-Last Edited: 04/27/2023
+Last Edited: 06/12/2023
 
 This calculates O-C values and produces an O-C plot.
 """
 
-from math import sqrt, floor
+from math import sqrt
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.polynomial import Polynomial
 import statsmodels.formula.api as smf
 import seaborn as sns
 from numba import jit
 
 
-def main():
-    print("\n\nThe format of these input files should be the of the raw form given from Dr. Robert Berrginton's"
-          " 'find_minimum' C program.")
-    print("Run TESS data by itself through the TESS option and filtered SARA/BSUO data through the BSU option.\n"
-          "DO NOT combine them in any way unless you have already run them through to get the (O-C) values and"
-          "are about to run the 'All Data' option.")
-    print("Enter the corresponding number to what you would like to do.\n")
-    while True:
+def main(period=None, loop=0, num=None, nights=None):
+    if loop == 0:
+        print("\n\nThe format of these input files should be the of the raw form given from Dr. Robert Berrginton's"
+              " 'find_minimum' C program.")
+        print("Run TESS data by itself through the TESS option and filtered SARA/BSUO data through the BSU option.\n"
+              "DO NOT combine them in any way unless you have already run them through to get the (O-C) values and"
+              "are about to run the 'All Data' option.")
+        print("Enter the corresponding number to what you would like to do.\n")
         try:
             num = int(input("Would you like to use BSUO data(1), TESS data(2), All Data(3), or Close Program(4): "))
-            if num == 1:
-                first_time = input("Do you already have an Epoch value 'Yes' or 'No': ")
-                if first_time.lower() == "no":
-                    T0 = 0
-                    To_err = 0
-                    period = float(input("Please enter the period for your system: "))
-                else:
-                    T0, To_err, period = arguments()
-                    print("Example file pathway: C:\\folder1\\folder2\\[file name]")
-                while True:
-                    inB = input("Please enter your times of minimum file pathway for the Johnson B filter: ")
-                    inV = input("Please enter your times of minimum file pathway for the Johnson V filter: ")
-                    inR = input("Please enter your times of minimum file pathway for the Cousins R filter: ")
-                    try:
-                        db = pd.read_csv(inB, header=None, delim_whitespace=True)
-                        dv = pd.read_csv(inV, header=None, delim_whitespace=True)
-                        dr = pd.read_csv(inR, header=None, delim_whitespace=True)
-                        break
-                    except FileNotFoundError:
-                        print("You have entered in an incorrect file or file pathway. Please try again.\n")
-                _ = BSUO(T0, To_err, period, db, dv, dr)
-            elif num == 2:
-                first_time = input("Do you already have an Epoch value 'Yes' or 'No': ")
-                if first_time.lower() == "no":
-                    T0 = 0
-                    To_err = 0
-                    period = float(input("Please enter the period for your system: "))
-                else:
-                    T0, To_err, period = arguments()
-                    print("Example file pathway: C:\\folder1\\folder2\\[file name]")
-                while True:
-                    infile = input("Please enter your times of minimum file pathway: ")
-                    try:
-                        df = pd.read_csv(infile, header=None, delim_whitespace=True)
-                        break
-                    except FileNotFoundError:
-                        print("You have entered in an incorrect file or file pathway. Please try again.\n")
-                _ = TESS_OC(T0, To_err, period, df)
-            elif num == 3:
-                while True:
-                    try:
-                        nights = int(input("How many files will you be using(i.e. if you have BSUO/SARA and TESS data "
-                                           "then you have 2 files): "))
-                        break
-                    except ValueError:
-                        print("Please enter a valid whole number.\n")
-                total = all_data(nights)
-                data_fit(total)
-            elif num == 4:
-                break
+        except ValueError:
+            print("Please enter either 1, 2, 3, or 4.\n")
+
+    while True:
+        if num == 1:
+            first_time = input("Do you already have an Epoch value 'Yes', 'No', or 'Close' to close the program: ")
+            if first_time.lower() == "no":
+                T0 = 0
+                To_err = 0
+                period = float(input("Please enter the period for your system: "))
+            elif first_time.lower() == "yes":
+                T0, To_err, period = arguments()
+                print("Example file pathway: C:\\folder1\\folder2\\[file name]")
+            else:
                 exit()
+            while True:
+                inB = input("Please enter your times of minimum file pathway for the Johnson B filter: ")
+                inV = input("Please enter your times of minimum file pathway for the Johnson V filter: ")
+                inR = input("Please enter your times of minimum file pathway for the Cousins R filter: ")
+                try:
+                    db = pd.read_csv(inB, header=None, delim_whitespace=True)
+                    dv = pd.read_csv(inV, header=None, delim_whitespace=True)
+                    dr = pd.read_csv(inR, header=None, delim_whitespace=True)
+                    break
+                except FileNotFoundError:
+                    print("You have entered in an incorrect file or file pathway. Please try again.\n")
+            _ = BSUO(T0, To_err, period, db, dv, dr)
+        elif num == 2:
+            first_time = input("Do you already have an Epoch value 'Yes' or 'No': ")
+            if first_time.lower() == "no":
+                T0 = 0
+                To_err = 0
+                period = float(input("Please enter the period for your system: "))
             else:
-                print("Please enter either 1, 2, 3, or 4.\n")
-        except ValueError:
+                T0, To_err, period = arguments()
+                print("Example file pathway: C:\\folder1\\folder2\\[file name]")
+            while True:
+                infile = input("Please enter your times of minimum file pathway: ")
+                try:
+                    df = pd.read_csv(infile, header=None, delim_whitespace=True)
+                    break
+                except FileNotFoundError:
+                    print("You have entered in an incorrect file or file pathway. Please try again.\n")
+            _ = TESS_OC(T0, To_err, period, df)
+        elif num == 3:
+            while True:
+                try:
+                    nights = int(input("How many files will you be using(i.e. if you have BSUO/SARA and TESS data "
+                                       "then you have 2 files): "))
+                    break
+                except ValueError:
+                    print("Please enter a valid whole number.\n")
+            period = float(input("Please enter the period of your system: "))
+            all_data(nights, period, loop)
+        elif num == 4:
+            break
+            exit()
+        else:
             print("Please enter either 1, 2, 3, or 4.\n")
 
 
 def TESS_OC(T0, To_err, period, df):
     """
     This function takes ToM data pre-gathered from TESS data and finds corresponding O-C values.
 
@@ -101,15 +105,15 @@
     E_est = []
     O_C = []
     O_C_err = []
 
     # this for loop, loops through the min_strict list and calculates a variety of values
     for count, val in enumerate(min_strict):
         # call the function to calculate the O-C values
-        e, OC, OC_err, T0, To_err = calculate_oc(val, min_strict_err[count], T0, To_err, period)
+        e, OC, OC_err, T0, To_err = calcualte_oc(val, min_strict_err[count], T0, To_err, period)
 
         E_est.append(e)
         O_C.append(OC)
         O_C_err.append(OC_err)
 
     # create a dataframe for all outputs to be places in for easy output
     dp = pd.DataFrame({
@@ -156,15 +160,15 @@
         minimum = (val + strict_V[count] + strict_R[count]) / 3
         err = sqrt(strict_B_err[count] ** 2 + strict_V_err[count] ** 2 + strict_R_err[count] ** 2) / 3
 
         average_min.append("%.5f" % minimum)
         average_err.append(err)
 
         # call the function to calculate the O-C values
-        e, OC, OC_err, T0, To_err = calculate_oc(minimum, err, T0, To_err, period)
+        e, OC, OC_err, T0, To_err = calcualte_oc(minimum, err, T0, To_err, period)
         E_est.append(e)
         O_C.append(OC)
         O_C_err.append(OC_err)
 
     # create a dataframe for all outputs to be places in for easy output
     dp = pd.DataFrame({
         "Minimums": average_min,
@@ -179,39 +183,49 @@
     # noinspection PyTypeChecker
     dp.to_csv(outfile, index=None, sep="\t")
     print("\nFinished saving file to " + outfile + ". This file is in the same folder as this python program.")
 
     return outfile
 
 
-def all_data(nights):
-    count = 1
+def all_data(nights, period, loop):
+    """
+    Merges all the data into a singular file for ease of use
+
+    :param nights: number of files there are for the first time through
+    :param period: period of the system
+    :param loop: number of loops through the program either o or 1
+
+    :return: None
+    """
+    count = 0
 
     minimum_list = []
     e_list = []
     o_c_list = []
     o_c_err_list = []
 
     while True:
-        print("\n\nPlease make sure that the very first line for each and every file that you have starts with the following\n"
-              "'Minimums	Epoch	O-C	O-C_Error'\n"
-              "With each space entered as a space.\n")
+        print(
+            "\n\nPlease make sure that the very first line for each and every file that you have starts with the following\n"
+            "'Minimums	Epoch	O-C	O-C_Error'\n"
+            "With each space entered as a space.\n")
         fname = input("Please enter a file name and pathway (i.e. C:\\folder1\\folder2\\[file name]): ")
         df = pd.read_csv(fname, header=None, skiprows=[0], delim_whitespace=True)
         minimum = np.array(df[0])
         e = np.array(df[1])
         o_c = np.array(df[2])
         o_c_err = np.array(df[3])
 
         for num, val in enumerate(minimum):
             minimum_list.append("%.5f" % val)
             e_list.append(e[num])
             o_c_list.append("%.5f" % o_c[num])
             o_c_err_list.append("%.5f" % o_c_err[num])
-        if count == nights:
+        if count + 1 == nights:
             break
         else:
             count += 1
             continue
     dp = pd.DataFrame({
         "Minimums": minimum_list,
         "Epoch": e_list,
@@ -236,15 +250,16 @@
     table_header += '$BJD_{\\rm TDB}$ & E & O-C \\\ \n'
     table_header += '\\hline\n' + '\\endhead\n' + '\\hline\n'
     table_header += '\\multicolumn{3}{c}{\\textit{Continued on next page}} \\\ \n'
     table_header += '\\endfoot\n' + '\\endlastfoot\n'
 
     minimum_lines = []
     for i in range(len(minimum)):
-        line = str("%.5f" % minimum[i]) + ' & ' + str(e[i]) + ' & $' + str("%.5f" % o_c[i]) + ' \pm ' + str( "%.5f" %o_c_err[i]) + '$ ' + "\\\ \n"
+        line = str("%.5f" % minimum[i]) + ' & ' + str(e[i]) + ' & $' + str("%.5f" % o_c[i]) + ' \pm ' + str(
+            "%.5f" % o_c_err[i]) + '$ ' + "\\\ \n"
         minimum_lines.append(line)
 
     output = table_header
     for count, line in enumerate(minimum_lines):
         output += line
 
     output += '\\hline\n' + '\\caption{NSVS 896797 O-C. The first column is the \n' \
@@ -261,15 +276,15 @@
     # outputfile = input("Please enter an output file name without the extension: ")
     file = open(outfile + ".tex", "w")
     file.write(output)
     file.close()
 
     outfile += ".txt"
 
-    return outfile
+    data_fit(outfile, period, loop, nights)
 
 
 def arguments():
     """
     This function asks the user for the T0
 
     :return: T0, To_err, and period float values
@@ -282,15 +297,15 @@
             break
         except ValueError:
             print("You have entered an invalid value. Please only enter float values and please try again.\n")
     return T0, To_err, period
 
 
 @jit(forceobj=True)
-def calculate_oc(m, err, T0, T0_err, p):
+def calcualte_oc(m, err, T0, T0_err, p):
     """
     Calculates O-C values and errors and find the eclipse number for primary and secondary eclipses
     :param m: ToM
     :param err: ToM error
     :param T0: first ToM
     :param T0_err: error for the T0
     :param p: period of the system
@@ -299,41 +314,47 @@
     """
     if T0 == 0:
         T0 = m
         T0_err = err
     # get the exact E value
     E_act = (m - T0) / p
     # estimate for the primary or secondary eclipse by rounding to the nearest 0.5
-    e = floor(E_act * 2) / 2
-    # caluclate the calculated ToM and find the O-C value
+    e = round(E_act * 2) / 2
+    # calculate the calculated ToM and find the O-C value
     T_calc = T0 + (e * p)
     OC = "%.5f" % (m - T_calc)
 
     # determine the error of the O-C
     OC_err = "%.5f" % sqrt(T0_err ** 2 + err ** 2)
 
     return e, OC, OC_err, T0, T0_err
 
 
-def data_fit(input_file):
+def data_fit(input_file, period, loop, nights):
     """
     Create a linear fit by hand and then use scipy to create a polynomial fit given an equation along with their
     respective residual plots
+
+    :param nights: number of files the user has
+    :param loop: number of loops the program has gone through either 0 or 1
+    :param period: period of the system
     :param input_file: input file from either TESS or BSUO
 
     :return: None
     """
     # read in the text file
     df = pd.read_csv(input_file, header=0, delim_whitespace=True)
 
     # append values to their respective lists for further and future potential use
     x = df["Epoch"]
     y = df["O-C"]
     y_err = df["O-C_Error"]
 
+    weights = 1/(y_err**2)
+
     # these next parts are mainly for O-C data as I just want to plot primary minima's and not both primary/secondary
     x1_prim = []
     y1_prim = []
     y_err_new_prim = []
 
     x1_sec = []
     y1_sec = []
@@ -372,81 +393,96 @@
             \\usepackage{booktabs}
             \\begin{document}"""
     endtex = "\end{document}"
 
     # opens a file with this name to begin writing to the file
     output_test = None
     while not output_test:
-        output_file = input("What is the output file name and pathway for the regression tables (either .txt or .tex): ")
+        output_file = input(
+            "\nWhat is the output file name and pathway for the regression tables (either .txt or .tex): ")
         if output_file.endswith((".txt", ".tex")):
             output_test = True
         else:
             print("This is not an allowed file output. Please make sure the file has the extension .txt or .tex.\n")
 
     # noinspection PyUnboundLocalVariable
     f = open(output_file, 'w')
     f.write(beginningtex)
 
     # sets up the fitting parameters
     xs = np.linspace(x.min(), x.max(), 1000)
     degree = 2
     degree_list = ["Linear", "Quadratic"]
     # noinspection PyUnboundLocalVariable
-    for i in range(1, degree+1):
+    for i in range(1, degree + 1):
         """
         Inside the model variable:
         'np.polynomial.polynomial.polyfit(x, y, i)' gathers the coefficients of the line fit
 
         'Polynomial' then finds an array of y values given a set of x data
         """
         model = Polynomial(np.polynomial.polynomial.polyfit(x1_prim, y1_prim, i))
 
         # plot the main graph with both fits (linear and poly) onto the same graph
-        plt.plot(xs, model(xs), color="black", label=degree_list[i-1] + " fit",
+        plt.plot(xs, model(xs), color="black", label=degree_list[i - 1] + " fit",
                  linestyle=line_style[line_count])
         line_count += 1
 
         # this if statement adds a string together to be used in the regression analysis
         # pretty much however many degrees in the polynomial there are, there will be that many I values
         if i >= 2:
             i_string = i_string + " + I(x**" + str(i) + ")"
-            mod = smf.ols(formula='y ~ x' + i_string, data=df)
+            mod = smf.wls(formula='y ~ x' + i_string, data=df, weights=weights)
             res = mod.fit()
             f.write(res.summary().as_latex())
         elif i == 1:
-            mod = smf.ols(formula='y ~ x', data=df)
+            mod = smf.wls(formula='y ~ x', data=df, weights=weights)
             res = mod.fit()
+            if loop == 0:
+                period_add = res.params[1]
+                new_period = period + period_add
+                print("The amount added to the period to get the adjusted period is " + str(period_add) + " days.")
+                print("The new period then becomes " + str(new_period) + " days.")
             f.write(res.summary().as_latex())
 
     f.write(endtex)
     # writes to the file the end latex code and then saves the file
     f.close()
     print("\nFinished saving latex/text file.\n\n")
 
     fontsize = 14
     plt.errorbar(x1_prim, y1_prim, yerr=y_err_new_prim, fmt="o", color="blue", label="Primary")
     plt.errorbar(x1_sec, y1_sec, yerr=y_err_new_sec, fmt="s", color="green", label="Secondary")
     # allows the legend to be moved wherever the user wants the legend to be placed rather than in a fixed location
     print("\n\nNOTE:")
-    print("You can drag the legend to move it wherever you would like, the default is the top right. Just click and drag"
-          " to move around the figure.\n")
+    print(
+        "You can drag the legend to move it wherever you would like, the default is the top right. Just click and drag"
+        " to move around the figure.\n")
     plt.legend(loc="upper right", fontsize=fontsize).set_draggable(True)
 
     x_label = "Epoch"
     y_label = "O-C (days)"
 
+    if loop == 0:
+        print("\nThe figure just plotted is with the original period. The program will start over using a "
+              "new period based on the linear fit.\n")
+
     # noinspection PyUnboundLocalVariable
     plt.xlabel(x_label, fontsize=fontsize)
     plt.xticks(fontsize=fontsize)
     # noinspection PyUnboundLocalVariable
     plt.ylabel(y_label, fontsize=fontsize)
     plt.yticks(fontsize=fontsize)
     plt.grid()
     plt.show()
 
+    if loop == 0:
+        loop += 1
+        main(new_period, loop, nights)
+
     # residuals(x1_prim, y1_prim, x_label, y_label, degree, model, xs)
 
 
 def residuals(x, y, x_label, y_label, degree, model, xs):
     """
     This plots the residuals of the data from the input file
     :param x: original x data
@@ -475,20 +511,14 @@
 
     # allows for easy change of the format of the subplots
     rows = 2
     cols = 1
     # creates the figure subplot for appending next
     fig, (ax1, ax2) = plt.subplots(rows, cols)
     # adds gridlines to both subplots
-    """
-    a[0].grid(visible=True, which='major', color='black', linewidth=1.0)
-    a[0].grid(visible=True, which='minor', color='black', linewidth=0.5)
-    a[1].grid(visible=True, which='major', color='black', linewidth=1.0)
-    a[1].grid(visible=True, which='minor', color='black', linewidth=0.5)
-    """
     ax1.grid()
     ax2.grid()
     # creates the model line fit
     sns.lineplot(x=x_label, y=y_label, data=model_dat, ax=ax1, color="red")
     # plots the original data to the same subplot as the model fit
     # edge color is removed to any sort of weird visual overlay on the plots as the normal edge color is white
     sns.scatterplot(x=x_label, y=y_label, data=raw_dat, ax=ax1, color="black", edgecolor="none")
@@ -497,12 +527,12 @@
                   scatter_kws=dict(edgecolor="none"))
     # adds a horizontal line to the residual plot to represent the model line fit with the same color
     ax2.axhline(y=0, color="red")
 
     plt.show()
 
 
-# data_fit('254037_OC.txt')
+# data_fit('254037_OC.txt', 0.31297, 1, 2)
 # data_fit('896797_OC.txt')
 
 if __name__ == '__main__':
     main()
```

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/apass.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/color_light_curve.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/find_min.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/gaia.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/menu.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Analyze images using aperture photometry within Python and not with Astro ImageJ (AIJ)
 
 Author: Kyle Koeller
 Created: 05/07/2023
-Last Updated: 05/16/2023
+Last Updated: 06/12/2023
 """
 
 # Python imports
 import numpy as np
 import pandas as pd
 from pathlib import Path
 import matplotlib.pyplot as plt
@@ -16,43 +16,46 @@
 
 # Astropy imports
 import ccdproc as ccdp
 from astropy.coordinates import SkyCoord
 from astropy.io import fits
 # from astropy.nddata import CCDData
 # from astropy.stats import sigma_clipped_stats
-from photutils.aperture import CircularAperture, CircularAnnulus, aperture_photometry
+from photutils.aperture import CircularAperture, CircularAnnulus, aperture_photometry, ApertureStats
 from astropy.wcs import WCS
 import astropy.units as u
 from astropy import wcs
+# from astropy.visualization import ZScaleInterval
 
 # turn off this warning that just tells the user,
 # "The warning raised when the contents of the FITS header have been modified to be standards compliant."
 warnings.filterwarnings("ignore", category=wcs.FITSFixedWarning)
 
 
 def main():
-    path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the reduced images are or type "
-                 "the word 'Close' to leave: ")
+    # path = input("Please enter a file pathway (i.e. C:\\folder1\\folder2\\[raw]) to where the reduced images are or type "
+    #             "the word 'Close' to leave: ")
+
+    path = "D:\\BSUO data\\2022.09.29-reduced"  # For testing purposes
 
     if path.lower() == "close":
         exit()
 
     science_imagetyp = 'LIGHT'
+
     images_path = Path(path)
     files = ccdp.ImageFileCollection(images_path)
-    image_list = files.files_filtered(imagetyp=science_imagetyp)
-    print(type(image_list))
+    image_list = files.files_filtered(imagetyp=science_imagetyp, filter="Empty/V")
 
-    multi_aperture_photometry(image_list, images_path)
+    single_MAP(image_list, images_path)
 
 
-def multi_aperture_photometry(image_list, path):
+def single_MAP(image_list, path):
     """
-    Perform aperture photometry on a list of images.
+    Perform multi-aperture photometry on a list of images for a single target
 
     Parameters
     ----------
     path : path
         Path to the folder containing the images.
     image_list : table
         Table of images to perform aperture photometry on.
@@ -60,19 +63,20 @@
     Returns
     -------
     None
     """
 
     # Define the aperture parameters
     # Define the aperture and annulus radii
-    aperture_radius = 25
-    annulus_radii = (40, 60)
+    aperture_radius = 20
+    annulus_radii = (30, 50)
 
     read_noise = 10.83  # * u.electron  # gathered from fits headers manually
     gain = 1.43  # * u.electron / u.adu  # gathered from fits headers manually
+    F_dark = 0.01  # dark current in u.electron / u.pix / u.s
 
     # Magnitudes of the comparison stars (replace with your values)
     df = pd.read_csv('254037_B.radec', skiprows=7, sep=",", header=None)
     magnitudes_comp = df[4]
     ra = df[0]
     dec = df[1]
     ref_star = df[2]
@@ -84,97 +88,238 @@
     bjd = []
 
     # Start interactive mode
     plt.ion()
 
     # Create a figure and axis
     fig, ax = plt.subplots()
+    plt.show()
 
-    for _, image_file in enumerate(image_list):
+    for icount, image_file in enumerate(image_list):
         image_data, header = fits.getdata(path / image_file, header=True)
-        wcs = WCS(header)
+        wcs_ = WCS(header)
 
         # ccd = CCDData(image_data, wcs=wcs, unit='adu')
 
         # Convert RA and DEC to pixel positions
         sky_coords = SkyCoord(ra, dec, unit=(u.h, u.deg), frame='icrs')
-        pixel_coords = wcs.world_to_pixel(sky_coords)
+        pixel_coords = wcs_.world_to_pixel(sky_coords)
 
-        target_position = pixel_coords[0]
-        comparison_positions = pixel_coords[1:]
+        target_position = list(pixel_coords[0])
+        comparison_positions = list(pixel_coords[1:])
 
         hjd.append(header['HJD-OBS'])
         bjd.append(header['BJD-OBS'])
 
         # Create the apertures and annuli
         target_aperture = CircularAperture(target_position, r=aperture_radius)
-        comparison_apertures = CircularAperture(comparison_positions, r=aperture_radius)
         target_annulus = CircularAnnulus(target_position, *annulus_radii)
-        comparison_annuli = CircularAnnulus(comparison_positions, *annulus_radii)
 
-        # Perform aperture photometry
         target_phot_table = aperture_photometry(image_data, target_aperture)
-        comparison_phot_tables = [aperture_photometry(image_data, aperture) for aperture in comparison_apertures]
 
         # Perform annulus photometry to estimate the background
-        target_annulus_table = aperture_photometry(image_data, target_annulus)
-        comparison_annuli_tables = [aperture_photometry(image_data, annulus) for annulus in comparison_annuli]
+        target_bkg_mean = ApertureStats(image_data, target_annulus).mean
+
+        # Calculate the total background
+        if np.isnan(target_bkg_mean) or np.isinf(target_bkg_mean):
+            target_bkg_mean = 0
+
+        target_bkg = ApertureStats(image_data, target_aperture, local_bkg=target_bkg_mean).sum
+
+        # Calculate the background subtracted counts
+        target_flx = target_phot_table['aperture_sum'] - target_bkg
 
-        # Calculate the background mean and standard deviation
-        target_background_mean = target_annulus_table['aperture_sum'][0] / target_annulus.area
-        target_background_stddev = np.sqrt(target_background_mean)
-
-        comparison_background_means = [table['aperture_sum'][0] / annulus.area
-                                       for table, annulus in zip(comparison_annuli_tables, comparison_annuli)]
-        comparison_background_stddevs = [np.sqrt(mean) for mean in comparison_background_means]
-
-        # Subtract the background: Calculate net integrated counts
-        target_sum = target_phot_table['aperture_sum'][0] - target_aperture.area * target_background_mean
-        comparison_sums = [table['aperture_sum'][0] - aperture.area * mean
-                           for table, aperture, mean in
-                           zip(comparison_phot_tables, comparison_apertures, comparison_background_means)]
-
-        # Calculate the errors
-        target_error = np.sqrt(
-            target_sum / gain + target_aperture.area * target_background_stddev ** 2 + target_aperture.area ** 2 * read_noise ** 2)
-        comparison_errors = [
-            np.sqrt(comp_sums / gain + aperture.area * stddev ** 2 + aperture.area ** 2 * read_noise ** 2)
-            for comp_sums, aperture, stddev in zip(comparison_sums, comparison_apertures, comparison_background_stddevs)]
-
-        # Calculate the magnitude and error of the target star
-        target_magnitude = -2.5 * np.log10(target_sum / np.mean(comparison_sums))
-
-        # Calculate the error in the magnitude
-        target_magnitude_error = (2.5 / np.log(10)) * np.sqrt((target_error / target_sum) ** 2 + np.mean(
-            [error ** 2 / star_sum ** 2 for error, star_sum in zip(comparison_errors, comparison_sums)]) / len(comparison_sums))
+        target_flx_err = np.sqrt(target_phot_table['aperture_sum'])
 
-        print('Target magnitude: ', target_magnitude, '+/-', target_magnitude_error)
+        target_magnitude = 25 - 2.5*np.log10(target_flx)
+        target_magnitude_error = (2.5/np.log(10)) * (target_flx_err/target_flx)
 
         # Append the calculated magnitude and error to the lists
-        magnitudes.append(target_magnitude)
-        mag_err.append(target_magnitude_error)
+        magnitudes.append(target_magnitude[0])
+        mag_err.append(target_magnitude_error[0])
 
         # Clear the axis
         ax.clear()
 
         # Plot the magnitudes with error bars
-        ax.errorbar(hjd, magnitudes, yerr=mag_err, fmt='o')
+        # ax.errorbar(hjd, magnitudes, yerr=mag_err, fmt='o')
+        ax.scatter(hjd, magnitudes, marker='o', color='black')
 
         # Set the labels
         ax.set_xlabel('HJD')
         ax.set_ylabel('Source_AMag_T1')
 
         # Draw the figure
         fig.canvas.draw()
 
         # Pause for a bit to allow the figure to update
         time.sleep(0.1)
+        plt.pause(0.0001)
 
     # Disable interactive mode
     plt.ioff()
 
-    # Show the final figure
+
+def multiple_MAP(image_list, path):
+    """
+    Perform multi-aperture photometry on a list of images for multiple targets
+    Parameters
+    ----------
+    image_list
+    path
+
+    Returns
+    -------
+
+    """
+
+    """
+        Perform multi-aperture photometry on a list of images for a single target
+
+        Parameters
+        ----------
+        path : path
+            Path to the folder containing the images.
+        image_list : table
+            Table of images to perform aperture photometry on.
+
+        Returns
+        -------
+        None
+        """
+
+    # Define the aperture parameters
+    # Define the aperture and annulus radii
+    aperture_radius = 20
+    annulus_radii = (30, 50)
+
+    read_noise = 10.83  # * u.electron  # gathered from fits headers manually
+    gain = 1.43  # * u.electron / u.adu  # gathered from fits headers manually
+    F_dark = 0.01  # dark current in u.electron / u.pix / u.s
+
+    # Magnitudes of the comparison stars (replace with your values)
+    df = pd.read_csv('254037_B.radec', skiprows=7, sep=",", header=None)
+    magnitudes_comp = df[4]
+    ra = df[0]
+    dec = df[1]
+    # ref_star = df[2]
+    # centroid = df[3]  # Not used (I don't think at least)
+
+    magnitudes = []
+    mag_err = []
+    hjd = []
+    bjd = []
+
+    # Start interactive mode
+    plt.ion()
+
+    # Create a figure and axis
+    fig, ax = plt.subplots()
     plt.show()
 
+    for icount, image_file in enumerate(image_list):
+        image_data, header = fits.getdata(path / image_file, header=True)
+        wcs_ = WCS(header)
+
+        # ccd = CCDData(image_data, wcs=wcs, unit='adu')
+
+        # Convert RA and DEC to pixel positions
+        sky_coords = SkyCoord(ra, dec, unit=(u.h, u.deg), frame='icrs')
+        pixel_coords = wcs_.world_to_pixel(sky_coords)
+
+        target_position = list(pixel_coords[0])
+        comparison_positions = list(pixel_coords[1:])
+
+        hjd.append(header['HJD-OBS'])
+        bjd.append(header['BJD-OBS'])
+
+        # Create the apertures and annuli
+        target_aperture = CircularAperture(target_position, r=aperture_radius)
+        target_annulus = CircularAnnulus(target_position, *annulus_radii)
+
+        comparison_aperture = CircularAperture(comparison_positions, r=aperture_radius)
+        comparison_annulus = CircularAnnulus(comparison_positions, *annulus_radii)
+
+        target_phot_table = aperture_photometry(image_data, target_aperture)
+        comparison_phot_table = aperture_photometry(image_data, comparison_aperture)
+
+        # Perform annulus photometry to estimate the background
+        target_bkg_mean = ApertureStats(image_data, target_annulus).mean
+        comparison_bkg_mean = ApertureStats(image_data, comparison_annulus).mean
+
+        # Calculate the total background
+        if np.isnan(target_bkg_mean) or np.isinf(target_bkg_mean) \
+                or np.isnan(comparison_bkg_mean) or np.isinf(comparison_bkg_mean):
+            target_bkg_mean = 0
+            comparison_bkg_mean = 0
+
+        target_bkg = ApertureStats(image_data, target_aperture, local_bkg=target_bkg_mean).sum
+        comparison_bkg = ApertureStats(image_data, comparison_aperture, local_bkg=comparison_bkg_mean).sum
+
+        # Calculate the background subtracted counts
+        target_flx = target_phot_table['aperture_sum'] - target_bkg
+        comparison_flx = comparison_phot_table['aperture_sum'] - comparison_bkg
+
+        # calculate the relative flux for each comparison star
+        rel_flx_T1 = target_flx / sum(comparison_flx)
+        count = 0
+        for i in comparison_flx:
+            if i == comparison_flx[count]:
+                rel_flux_comp = i / (sum(comparison_flx) - i)
+            count += 1
+
+        # find the number of pixels used to estimate the sky background
+        n_b_mask_comp = comparison_annulus.to_mask(method="center")
+        n_b_comp = np.sum(n_b_mask_comp)
+
+        n_b_mask_tar = target_annulus.to_mask(method="center")
+        n_b_tar = np.sum(n_b_mask_tar)
+
+        # find the number of pixels used in the aperture
+        n_pix_mask_comp = comparison_aperture.to_mask(method="center")
+        n_pix_comp = np.sum(n_pix_mask_comp)
+
+        n_pix_tar = target_aperture.to_mask(method="center")
+        n_pix_tar = np.sum(n_pix_tar)
+
+        # Calculate the total noise
+        sigma_f = 0.289  # quoted from Collins 2017 https://iopscience.iop.org/article/10.3847/1538-3881/153/2/77/pdf
+        F_s = 0.01  # number of sky background counts per pixel in ADU
+
+        N_comp = np.sqrt(gain*comparison_flx + n_pix_comp*(1 + (n_pix_comp/n_b_comp))*(gain*F_s + F_dark + read_noise**2 + gain**2 + sigma_f**2)) / gain
+        N_tar = np.sqrt(gain*target_flx + n_pix_tar*(1 + (n_pix_tar/n_b_tar))*(gain*F_s + F_dark + read_noise**2 + gain**2 + sigma_f**2)) / gain
+
+        # calculate the total comparison ensemble noise
+        N_e_comp = np.sqrt(np.sum(N_comp**2))
+        
+        # calculate the total target magnitude and error
+        target_magnitude = [0]
+        target_magnitude_error = [0]
+
+        # Append the calculated magnitude and error to the lists
+        magnitudes.append(target_magnitude[0])
+        mag_err.append(target_magnitude_error[0])
+
+        # Clear the axis
+        ax.clear()
+
+        # Plot the magnitudes with error bars
+        # ax.errorbar(hjd, magnitudes, yerr=mag_err, fmt='o')
+        ax.scatter(hjd, magnitudes, marker='o', color='black')
+
+        # Set the labels
+        ax.set_xlabel('HJD')
+        ax.set_ylabel('Source_AMag_T1')
+
+        # Draw the figure
+        fig.canvas.draw()
+
+        # Pause for a bit to allow the figure to update
+        time.sleep(0.1)
+        plt.pause(0.0001)
+
+    # Disable interactive mode
+    plt.ioff()
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/tests/test_OC_plot.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/tests/test_OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a8
+Version: 2.8.4a9
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.4a8/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-2.8.4a9/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/LICENSE` & `EclipsingBinaries-2.8.4a9/LICENSE`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/PKG-INFO` & `EclipsingBinaries-2.8.4a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 2.8.4a8
+Version: 2.8.4a9
 Summary: Binary Star Package for Ball State University's Astronomy Research Group
 Home-page: https://github.com/kjkoeller/EclipsingBinaries
 Author: Kyle Koeller
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `EclipsingBinaries-2.8.4a8/README.md` & `EclipsingBinaries-2.8.4a9/README.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-2.8.4a8/setup.py` & `EclipsingBinaries-2.8.4a9/setup.py`

 * *Files identical despite different names*

