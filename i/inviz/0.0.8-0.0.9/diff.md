# Comparing `tmp/inviz-0.0.8.tar.gz` & `tmp/inviz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.0.8.tar", last modified: Thu Jun 15 10:12:26 2023, max compression
+gzip compressed data, was "inviz-0.0.9.tar", last modified: Thu Jun 15 14:05:06 2023, max compression
```

## Comparing `inviz-0.0.8.tar` & `inviz-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 10:12:26.008622 inviz-0.0.8/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.0.8/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.0.8/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2220 2023-06-15 10:12:26.008622 inviz-0.0.8/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1669 2023-06-12 23:22:44.000000 inviz-0.0.8/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 10:12:26.008622 inviz-0.0.8/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 10:12:26.008622 inviz-0.0.8/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     2220 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)       75 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)     8891 2023-06-12 23:22:46.000000 inviz-0.0.8/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-06-15 10:12:26.008622 inviz-0.0.8/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1090 2023-06-12 23:22:46.000000 inviz-0.0.8/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 14:05:06.205949 inviz-0.0.9/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.0.9/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.0.9/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2220 2023-06-15 14:05:06.205949 inviz-0.0.9/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1669 2023-06-12 23:22:44.000000 inviz-0.0.9/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 14:05:06.195949 inviz-0.0.9/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 14:05:06.205949 inviz-0.0.9/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2220 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       75 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-06-15 14:05:06.000000 inviz-0.0.9/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)     8997 2023-06-15 13:55:49.000000 inviz-0.0.9/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-06-15 14:05:06.205949 inviz-0.0.9/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1090 2023-06-15 14:04:05.000000 inviz-0.0.9/setup.py
```

### Comparing `inviz-0.0.8/LICENSE` & `inviz-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.0.8/PKG-INFO` & `inviz-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.8
+Version: 0.0.9
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.0.8/README.md` & `inviz-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `inviz-0.0.8/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.0.9/inviz/inviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.8
+Version: 0.0.9
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inviz-0.0.8/inviz/inviz.py` & `inviz-0.0.9/inviz/inviz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,83 @@
 import holoviews as hv
 from holoviews import dim, opts, streams
 import pandas as pd
 import numpy as np
-import re
+# import re
 import panel as pn
 import spatialpandas
 from bokeh.models import HoverTool
-from classy import Class
+# from classy import Class
 import matplotlib.pyplot as plt
-from multiprocessing import Pool
+# from multiprocessing import Pool
 
 hv.extension('bokeh')
 pn.extension()
 
-# read in the .paramnames file and put it into list format
-def load_params(filename):
-    params_list = []
-    with open(filename, 'r') as f:
-        for line in f:
-            line = line.strip()
-            params = re.split(' \t ', line)
-            params_list.append(params)
-    return [item[0] for item in params_list], [item[1] for item in params_list]
-
-
-# create a DataFrame with the chain files as rows and use a list of parameters as the column names
-def load_data(filename, column_names):
-    data = np.loadtxt(filename)
-    df = pd.DataFrame(data[:,1:], columns=column_names)
-    return df
-
-
-def run_class(selection):
-    # run class on the user's selection
-    cosmo = Class()
-    cosmo.set(selection)
-    cosmo.set({'output':'mPk, tCl, pCl, lCl','P_k_max_1/Mpc':3.0, 'lensing':'yes'})
-    cosmo.compute()
-
-    # set variables for matter power spectrum and lensed CMB angular power spectra
-    kk = np.logspace(-4,np.log10(3),1000)
-    Pk = []
-    h = cosmo.h()
-    for k in kk:
-        Pk.append(cosmo.pk(k*h,0.)*h**3)
-    Pk = np.array(Pk)
-    l = np.array(range(2,2501))
-    factor = l*(l+1)/(2*np.pi)
-    lensed_cl = cosmo.lensed_cl(2500)
+# # read in the .paramnames file and put it into list format
+# def load_params(filename):
+#     params_list = []
+#     with open(filename, 'r') as f:
+#         for line in f:
+#             line = line.strip()
+#             params = re.split(' \t ', line)
+#             params_list.append(params)
+#     return [item[0] for item in params_list], [item[1] for item in params_list]
+
+
+# # create a DataFrame with the chain files as rows and use a list of parameters as the column names
+# def load_data(filename, column_names):
+#     data = np.loadtxt(filename)
+#     df = pd.DataFrame(data[:,1:], columns=column_names)
+#     return df
+
+
+# def run_class(selection):
+#     # run class on the user's selection
+#     cosmo = Class()
+#     cosmo.set(selection)
+#     cosmo.set({'output':'mPk, tCl, pCl, lCl','P_k_max_1/Mpc':3.0, 'lensing':'yes'})
+#     cosmo.compute()
+
+#     # set variables for matter power spectrum and lensed CMB angular power spectra
+#     kk = np.logspace(-4,np.log10(3),1000)
+#     Pk = []
+#     h = cosmo.h()
+#     for k in kk:
+#         Pk.append(cosmo.pk(k*h,0.)*h**3)
+#     Pk = np.array(Pk)
+#     l = np.array(range(2,2501))
+#     factor = l*(l+1)/(2*np.pi)
+#     lensed_cl = cosmo.lensed_cl(2500)
     
-    results = {'k': kk, 'Pk': Pk, 'l': l, 'Cl_tt': factor*lensed_cl['tt'][2:], 'Cl_ee': factor*lensed_cl['ee'][2:]}
+#     results = {'k': kk, 'Pk': Pk, 'l': l, 'Cl_tt': factor*lensed_cl['tt'][2:], 'Cl_ee': factor*lensed_cl['ee'][2:]}
     
-    cosmo.struct_cleanup()
-    cosmo.empty()
-    return results
-
-
-def compute_residuals(index, sample, sample_CDM):
-    selection = sample.iloc[[index]].to_dict('index')
-    selection_CDM = sample_CDM.iloc[[index]].to_dict('index')
-    if __name__ == '__main__':
-        with Pool() as p:
-            [mycosmo, LambdaCDM] = p.map(run_class, [selection[index], selection_CDM[index]])
-    else:
-        mycosmo = run_class(selection[index])
-        LambdaCDM = run_class(selection_CDM[index])
-
-    pk_residuals = (mycosmo['Pk'] - LambdaCDM['Pk'])/LambdaCDM['Pk']*100
-    cl_tt_residuals = (mycosmo['Cl_tt'] - LambdaCDM['Cl_tt'])/LambdaCDM['Cl_tt']*100
-    cl_ee_residuals = (mycosmo['Cl_ee'] - LambdaCDM['Cl_ee'])/LambdaCDM['Cl_ee']*100
+#     cosmo.struct_cleanup()
+#     cosmo.empty()
+#     return results
+
+
+# def compute_residuals(index, sample, sample_CDM):
+#     selection = sample.iloc[[index]].to_dict('index')
+#     selection_CDM = sample_CDM.iloc[[index]].to_dict('index')
+#     if __name__ == '__main__':
+#         with Pool() as p:
+#             [mycosmo, LambdaCDM] = p.map(run_class, [selection[index], selection_CDM[index]])
+#     else:
+#         mycosmo = run_class(selection[index])
+#         LambdaCDM = run_class(selection_CDM[index])
+
+#     pk_residuals = (mycosmo['Pk'] - LambdaCDM['Pk'])/LambdaCDM['Pk']*100
+#     cl_tt_residuals = (mycosmo['Cl_tt'] - LambdaCDM['Cl_tt'])/LambdaCDM['Cl_tt']*100
+#     cl_ee_residuals = (mycosmo['Cl_ee'] - LambdaCDM['Cl_ee'])/LambdaCDM['Cl_ee']*100
     
-    residuals = {'pk_residuals': {'k': mycosmo['k'], 'Pk': pk_residuals}, 
-                 'cl_tt_residuals': {'l': mycosmo['l'], 'Cl_TT': cl_tt_residuals}, 
-                 'cl_ee_residuals': {'l': mycosmo['l'], 'Cl_EE': cl_ee_residuals}}
-    return residuals
+#     residuals = {'pk_residuals': {'k': mycosmo['k'], 'Pk': pk_residuals}, 
+#                  'cl_tt_residuals': {'l': mycosmo['l'], 'Cl_TT': cl_tt_residuals}, 
+#                  'cl_ee_residuals': {'l': mycosmo['l'], 'Cl_EE': cl_ee_residuals}}
+#     return residuals
 
 
 # generate a scatter plot using the key dimensions from a holoviews.Dataset object, with the CLASS output displayed alongside it
 def viz(data, data_observable=None, myfunction=None, myfunction_args=None, show_observables=True, latex_dict=None, curve_opts=None):
     # handle default case of no latex paramname dictionary
     if latex_dict is None:
         latex_dict = dict()
```

### Comparing `inviz-0.0.8/setup.py` & `inviz-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.0.8",
+    version = "0.0.9",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
```

