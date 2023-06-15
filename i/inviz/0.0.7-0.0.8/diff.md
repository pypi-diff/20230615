# Comparing `tmp/inviz-0.0.7.tar.gz` & `tmp/inviz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inviz-0.0.7.tar", last modified: Fri Apr 28 18:14:07 2023, max compression
+gzip compressed data, was "inviz-0.0.8.tar", last modified: Thu Jun 15 10:12:26 2023, max compression
```

## Comparing `inviz-0.0.7.tar` & `inviz-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-28 18:14:07.748636 inviz-0.0.7/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-04-27 23:20:02.000000 inviz-0.0.7/LICENSE
--rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-04-27 23:20:02.000000 inviz-0.0.7/MANIFEST.in
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1910 2023-04-28 18:14:07.748636 inviz-0.0.7/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1359 2023-04-27 23:20:02.000000 inviz-0.0.7/README.md
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-28 18:14:07.748636 inviz-0.0.7/inviz/
-drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-04-28 18:14:07.748636 inviz-0.0.7/inviz/inviz.egg-info/
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1910 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/PKG-INFO
--rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/SOURCES.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/dependency_links.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)       75 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/requires.txt
--rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-04-28 18:14:07.000000 inviz-0.0.7/inviz/inviz.egg-info/top_level.txt
--rwxr-xr-x   0 jswen     (1000) jswen     (1000)     9062 2023-04-28 17:14:55.000000 inviz-0.0.7/inviz/inviz.py
--rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-04-28 18:14:07.748636 inviz-0.0.7/setup.cfg
--rw-r--r--   0 jswen     (1000) jswen     (1000)     1090 2023-04-28 17:33:46.000000 inviz-0.0.7/setup.py
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 10:12:26.008622 inviz-0.0.8/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1066 2023-03-27 21:46:04.000000 inviz-0.0.8/LICENSE
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       42 2023-03-27 21:46:04.000000 inviz-0.0.8/MANIFEST.in
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2220 2023-06-15 10:12:26.008622 inviz-0.0.8/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1669 2023-06-12 23:22:44.000000 inviz-0.0.8/README.md
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 10:12:26.008622 inviz-0.0.8/inviz/
+drwxr-xr-x   0 jswen     (1000) jswen     (1000)        0 2023-06-15 10:12:26.008622 inviz-0.0.8/inviz/inviz.egg-info/
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     2220 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/PKG-INFO
+-rw-r--r--   0 jswen     (1000) jswen     (1000)      227 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/SOURCES.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        1 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/dependency_links.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       75 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/requires.txt
+-rw-r--r--   0 jswen     (1000) jswen     (1000)        6 2023-06-15 10:12:25.000000 inviz-0.0.8/inviz/inviz.egg-info/top_level.txt
+-rwxr-xr-x   0 jswen     (1000) jswen     (1000)     8891 2023-06-12 23:22:46.000000 inviz-0.0.8/inviz/inviz.py
+-rw-r--r--   0 jswen     (1000) jswen     (1000)       38 2023-06-15 10:12:26.008622 inviz-0.0.8/setup.cfg
+-rw-r--r--   0 jswen     (1000) jswen     (1000)     1090 2023-06-12 23:22:46.000000 inviz-0.0.8/setup.py
```

### Comparing `inviz-0.0.7/LICENSE` & `inviz-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `inviz-0.0.7/PKG-INFO` & `inviz-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.7
+Version: 0.0.8
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# inviz
+# InViz
 
-This tool helps you explore the results of running MCMC posterior sampling on your cosmological model. Selecting a point on the sample distribution will automatically run CLASS on that sample and display the output. 
+InViz (Interactive Visualizer) is a tool for exploratory analysis of high-dimensional datasets where data points from the parameter space are used to calculate to some set of real-world observables. This enables you to easily see how the derived observables change as you traverse the parameter space. If you have pre-computed observables, simply import them alongside the  dataset containing the parameters to start visualizing. Or, write your own function that takes your parameters as inputs, and give it to InViz to compute on the fly!
 
-### Installation
-Installation is straightforward with pip:
+## Installation
+InViz can be installed with pip:
 
     python -m pip install inviz
+
 Or, if you want to test the latest changes, you can clone the repository with
     
     git clone https://github.com/wen-jams/inviz
     cd inviz
     python setup.py install
+
 ### Dependencies
-Currently, only Python versions $\geq$ 3.8 and $<$ 3.11 are supported.  You will also need the Cosmology Boltzmann code CLASS (either the default or your own modified version). Follow the instructions [here](https://cobaya.readthedocs.io/en/latest/theory_class.html) to install classy, the Python wrapper for CLASS.
+- Python versions $\geq$ 3.8 and $<$ 3.11 are supported.
+- Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
 
 ## Getting Started
 
 ### Test Installation
 To verify that inviz and all the dependencies have been installed correctly, open a Jupyter Notebook and run:
 ```python
 from inviz import *
@@ -40,9 +43,9 @@
 pn.extension()
 ```
 If no errors appear, all the dependencies were installed correctly and we're ready to start visualizing!
 
 ### Example
 Download and run the tutorial notebook in the [tutorials](tutorials) folder to see an example of how inviz can be used.
 
-The result should look like this:
-![example output](images/example1.png)
+Here's an example of InViz in an astrophysics context! The parameters come from a specific dark matter model, and the observables are the matter power spectrum and CMB anisotropy power spectra.
+![example output](images/example2.png)
```

### Comparing `inviz-0.0.7/inviz/inviz.egg-info/PKG-INFO` & `inviz-0.0.8/inviz/inviz.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: inviz
-Version: 0.0.7
+Version: 0.0.8
 Summary: An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model.
 Home-page: http://packages.python.org/inviz
 Author: James Wen
 Author-email: jswen@usc.edu
 License: MIT
 Keywords: interactive visualizer cosmology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# inviz
+# InViz
 
-This tool helps you explore the results of running MCMC posterior sampling on your cosmological model. Selecting a point on the sample distribution will automatically run CLASS on that sample and display the output. 
+InViz (Interactive Visualizer) is a tool for exploratory analysis of high-dimensional datasets where data points from the parameter space are used to calculate to some set of real-world observables. This enables you to easily see how the derived observables change as you traverse the parameter space. If you have pre-computed observables, simply import them alongside the  dataset containing the parameters to start visualizing. Or, write your own function that takes your parameters as inputs, and give it to InViz to compute on the fly!
 
-### Installation
-Installation is straightforward with pip:
+## Installation
+InViz can be installed with pip:
 
     python -m pip install inviz
+
 Or, if you want to test the latest changes, you can clone the repository with
     
     git clone https://github.com/wen-jams/inviz
     cd inviz
     python setup.py install
+
 ### Dependencies
-Currently, only Python versions $\geq$ 3.8 and $<$ 3.11 are supported.  You will also need the Cosmology Boltzmann code CLASS (either the default or your own modified version). Follow the instructions [here](https://cobaya.readthedocs.io/en/latest/theory_class.html) to install classy, the Python wrapper for CLASS.
+- Python versions $\geq$ 3.8 and $<$ 3.11 are supported.
+- Holoviews $\leq$ 1.15.4 (this package and its dependencies will be installed automatically)
 
 ## Getting Started
 
 ### Test Installation
 To verify that inviz and all the dependencies have been installed correctly, open a Jupyter Notebook and run:
 ```python
 from inviz import *
@@ -40,9 +43,9 @@
 pn.extension()
 ```
 If no errors appear, all the dependencies were installed correctly and we're ready to start visualizing!
 
 ### Example
 Download and run the tutorial notebook in the [tutorials](tutorials) folder to see an example of how inviz can be used.
 
-The result should look like this:
-![example output](images/example1.png)
+Here's an example of InViz in an astrophysics context! The parameters come from a specific dark matter model, and the observables are the matter power spectrum and CMB anisotropy power spectra.
+![example output](images/example2.png)
```

### Comparing `inviz-0.0.7/inviz/inviz.py` & `inviz-0.0.8/inviz/inviz.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 import holoviews as hv
 from holoviews import dim, opts, streams
-# from holoviews.selection import link_selections
-# import hvplot.pandas
 import pandas as pd
-from itertools import combinations
 import numpy as np
-from tqdm import trange, tqdm
 import re
 import panel as pn
 import spatialpandas
-import os
 from bokeh.models import HoverTool
 from classy import Class
 import matplotlib.pyplot as plt
-# import copy
 from multiprocessing import Pool
 
-# pn.extension(loading_spinner='dots', loading_color='#00aa41', sizing_mode="stretch_width")
 hv.extension('bokeh')
-# hv.Store.set_current_backend('bokeh')
-# pn.extension('tabulator')
 pn.extension()
 
 # read in the .paramnames file and put it into list format
 def load_params(filename):
     params_list = []
     with open(filename, 'r') as f:
         for line in f:
@@ -55,27 +46,50 @@
         Pk.append(cosmo.pk(k*h,0.)*h**3)
     Pk = np.array(Pk)
     l = np.array(range(2,2501))
     factor = l*(l+1)/(2*np.pi)
     lensed_cl = cosmo.lensed_cl(2500)
     
     results = {'k': kk, 'Pk': Pk, 'l': l, 'Cl_tt': factor*lensed_cl['tt'][2:], 'Cl_ee': factor*lensed_cl['ee'][2:]}
+    
+    cosmo.struct_cleanup()
+    cosmo.empty()
     return results
 
 
+def compute_residuals(index, sample, sample_CDM):
+    selection = sample.iloc[[index]].to_dict('index')
+    selection_CDM = sample_CDM.iloc[[index]].to_dict('index')
+    if __name__ == '__main__':
+        with Pool() as p:
+            [mycosmo, LambdaCDM] = p.map(run_class, [selection[index], selection_CDM[index]])
+    else:
+        mycosmo = run_class(selection[index])
+        LambdaCDM = run_class(selection_CDM[index])
+
+    pk_residuals = (mycosmo['Pk'] - LambdaCDM['Pk'])/LambdaCDM['Pk']*100
+    cl_tt_residuals = (mycosmo['Cl_tt'] - LambdaCDM['Cl_tt'])/LambdaCDM['Cl_tt']*100
+    cl_ee_residuals = (mycosmo['Cl_ee'] - LambdaCDM['Cl_ee'])/LambdaCDM['Cl_ee']*100
+    
+    residuals = {'pk_residuals': {'k': mycosmo['k'], 'Pk': pk_residuals}, 
+                 'cl_tt_residuals': {'l': mycosmo['l'], 'Cl_TT': cl_tt_residuals}, 
+                 'cl_ee_residuals': {'l': mycosmo['l'], 'Cl_EE': cl_ee_residuals}}
+    return residuals
+
+
 # generate a scatter plot using the key dimensions from a holoviews.Dataset object, with the CLASS output displayed alongside it
-def viz(data, data_classy_input, data_classy_CDM, class_enabled=True, latex_dict=None):
+def viz(data, data_observable=None, myfunction=None, myfunction_args=None, show_observables=True, latex_dict=None, curve_opts=None):
     # handle default case of no latex paramname dictionary
     if latex_dict is None:
         latex_dict = dict()
     # setting Panel widgets for user interaction
     variables = data.columns.values.tolist()
-    var1 = pn.widgets.Select(value=variables[0], name='Horizontal Axis', options=variables)
-    var2 = pn.widgets.Select(value=variables[1], name='Vertical Axis', options=variables)
-    cmap_var = pn.widgets.Select(value=variables[2], name='Colormapped Parameter', options=variables)
+    var1 = pn.widgets.Select(value=variables[1], name='Horizontal Axis', options=variables)
+    var2 = pn.widgets.Select(value=variables[2], name='Vertical Axis', options=variables)
+    cmap_var = pn.widgets.Select(value=variables[0], name='Colormapped Parameter', options=variables)
     cmap_option = pn.widgets.Checkbox(value=True, name='Show Colormap', align='end')
     
     #  given a param name, find corresponding latex-formatted param name
     def lookup_latex_label(param):
         try:
             latex_param = latex_dict[param]
             label = r'$${}$$'.format(latex_param)
@@ -86,21 +100,22 @@
     
     # function for generating the scatter plot, given 2 dimensions as x and y axes, and an additional dimension to colormap
     # to the points on the plot. Also has an option to show or hide the colormap
     def plot_data(kdim1, kdim2, colordim, showcmap):
         if showcmap == True:
             cmapping = opts.Points(color=dim(colordim),
                 colorbar=True,
-                cmap='Viridis')
+                cmap='GnBu_r')
         else:
             cmapping = opts.Points(color='grey', colorbar=True)
         hover = HoverTool(tooltips=None)
         xlabel = lookup_latex_label(kdim1)
         ylabel = lookup_latex_label(kdim2)
         popts = opts.Points(
+            bgcolor='#E5E9F0',
             fontscale=1.1,
             xlabel=xlabel,
             ylabel=ylabel,
             toolbar='above',
             line_color='black',
             #alpha=0.75, selection_alpha=1, nonselection_alpha=0.1,
             tools=[hover, 'box_select','lasso_select','tap'],
@@ -120,81 +135,74 @@
     def hook(plot, element):
         plot.handles['table'].autosize_mode = "none"
         for column in plot.handles['table'].columns:
             column.width = 100
     
     # function to generate a table of all the selected points
     def make_table(kdim1, kdim2, colordim):
-        table_options = opts.Table(height=300, width=1000, hooks=[hook])
+        table_options = opts.Table(height=300, width=1000, hooks=[hook], bgcolor='#f5f5f5')
         table = hv.DynamicMap(lambda index: hv.Table(data.iloc[index], kdims=[kdim1, kdim2, colordim]), streams=[selection])
         return table.opts(table_options).relabel('Selected Points')
     
     
     # generate the table
     selected_table = pn.bind(make_table, kdim1=var1, kdim2=var2, colordim=cmap_var)
     
     #table_stream = streams.Selection1D(source=selected_table)
     
     # function to run CLASS on data from the selection. 
-    # first create an empty plot to handle the null selection case
-    empty_plot = hv.Curve(np.random.rand(0, 2))
-    def plot_class_results(index):
+    # handles the null selection case and multiple selections
+    curves = {}
+    empty_plot = hv.Curve(np.random.rand(0, 2)).opts(framewise=True)
+    if data_observable is not None:
+        data_observable = data_observable.to_dict('index')
+    def plot_observables(index):
         if not index:
-            empty_pk = empty_plot.relabel('P(k) Residuals - no selection').opts(
-                xlabel=r'$$k~[h/\mathrm{Mpc}]$$', 
-                ylabel=r'$$(P(k)-P_{CDM}(k))/P_{CDM}(k)*100~[\%]$$')
-            empty_cl_tt = empty_plot.relabel('Lensed Cl_TT Residuals - no selection').opts(
-                xlabel=r"$$\ell$$", 
-                ylabel=r"$$(C_{\ell}^{TT} - C_{\ell, CDM}^{TT})/C_{\ell, CDM}^{TT}*100~[\%]$$")
-            empty_cl_ee = empty_plot.relabel('Lensed Cl_EE Residuals - no selection').opts(
-                xlabel=r"$$\ell$$", 
-                ylabel=r"$$(C_{\ell}^{EE} - C_{\ell, CDM}^{EE})/C_{\ell, CDM}^{EE}*100~[\%]$$")
-            empty_layout = empty_pk + empty_cl_tt + empty_cl_ee            
-            return empty_layout
-
-        # the Selection1D stream returns an index number. index into the approprate dataframe and turn it into a dictionary for CLASS to read
-        selection = data_classy_input.iloc[index]
-        selection_CDM = data_classy_CDM.iloc[index]
-        sel_dict_list = selection.to_dict('records')
-        CDM_dict_list = selection_CDM.to_dict('records')
-        
-        # compute stats for user's cosmology and LambdaCDM
-        # in parallel:
-        # if __name__ == '__main__':
-        #     with Pool() as p:
-        #         [mycosmo, LambdaCDM] = p.map(run_class, [sel_dict_list[0], CDM_dict_list[0]])
-        # in serial:
-        mycosmo = run_class(sel_dict_list[0])
-        LambdaCDM = run_class(CDM_dict_list[0])
-
-        # compute residuals
-        pk_residuals = (mycosmo['Pk'] - LambdaCDM['Pk'])/LambdaCDM['Pk']*100
-        cl_tt_residuals = (mycosmo['Cl_tt'] - LambdaCDM['Cl_tt'])/LambdaCDM['Cl_tt']*100
-        cl_ee_residuals = (mycosmo['Cl_ee'] - LambdaCDM['Cl_ee'])/LambdaCDM['Cl_ee']*100
-
-        plot_pk_residuals = hv.Curve((mycosmo['k'], pk_residuals)).relabel('P(k) Residuals').opts(
-            xlabel=r'$$k~[h/\mathrm{Mpc}]$$', 
-            ylabel=r'$$(P(k)-P_{CDM}(k))/P_{CDM}(k)*100~[\%]$$')
-
-        plot_cl_tt_residuals = hv.Curve((mycosmo['l'],cl_tt_residuals)).relabel('Cl_TT Residuals').opts(
-            xlabel=r"$$\ell$$", 
-            ylabel=r"$$(C_{\ell}^{TT}-C_{\ell, CDM}^{TT})/C_{\ell, CDM}^{TT}*100~[\%]$$")
-
-        plot_cl_ee_residuals = hv.Curve((mycosmo['l'],cl_ee_residuals)).relabel('Cl_EE Residuals').opts(
-            xlabel=r"$$\ell$$", 
-            ylabel=r"$$(C_{\ell}^{EE}-C_{\ell, CDM}^{EE})/C_{\ell, CDM}^{EE}*100~[\%]$$")
-        
-        layout = (plot_pk_residuals + plot_cl_tt_residuals + plot_cl_ee_residuals)
+            curves_list = [[empty_plot.relabel('Plot 1 - No Selection')], 
+                           [empty_plot.relabel('Plot 2 - No Selection')], 
+                           [empty_plot.relabel('Plot 3 - No Selection')]]
+        else:
+            new_index = [x for x in index if x not in list(curves.keys())]
+            for element in new_index:
+                if data_observable is not None:
+                    observables = data_observable[element]
+                elif myfunction is not None:
+                    observables = myfunction(element, *myfunction_args)
+                observables_keys = list(observables.keys())
+
+                new_plots = []
+                for key in observables_keys:
+                    dataset = observables[key]
+                    kdim = list(dataset.keys())[0]
+                    vdim = list(dataset.keys())[1]
+                    plot_observable = hv.Curve(dataset, kdim, vdim, label=key).opts(framewise=True)
+                    new_plots.append(plot_observable)
+                curves[element] = {plot.label: plot for plot in new_plots}
+
+            curves_list = []
+            for index_item in index:
+                curve_types = list(curves[index_item].keys())
+
+            for curve_item in curve_types:
+                same_type = [curves[key][curve_item] for key in index]
+                curves_list.append(same_type)
+            
+        layout = hv.Layout()
+        for list_of_curves in curves_list:
+            overlay = hv.Overlay(list_of_curves)
+            layout = layout + overlay    
         return layout
     
+    
     # put it all together using Panel
     dashboard = pn.Column(pn.Row(var1, var2, cmap_var, cmap_option), pn.Row(points_dmap, selected_table))
     
-    if class_enabled == True:
-        classy_output = hv.DynamicMap(plot_class_results, streams=[selection]).opts(
-            opts.Curve(color='black', logx=True, width=500, height=400, padding=0.1, framewise=True),
-            opts.Layout(shared_axes=False))
-        classy_output_pane = pn.panel(classy_output)
-        # pn.param.set_values(classy_output_pane, loading_indicator=True)
-        dashboard = pn.Column(dashboard, classy_output_pane)
+    if show_observables == True:
+        observables_dmap = hv.DynamicMap(plot_observables, streams=[selection]).opts(
+            curve_opts, 
+            opts.Layout(shared_axes=False),
+            opts.Overlay(show_legend=False)
+        )
+        observables_pane = pn.panel(observables_dmap)
+        dashboard = pn.Column(dashboard, observables_pane)
     
     return dashboard
```

### Comparing `inviz-0.0.7/setup.py` & `inviz-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "inviz",
-    version = "0.0.7",
+    version = "0.0.8",
     author = "James Wen",
     author_email = "jswen@usc.edu",
     description = ("An interactive visualizer to help explore the results of running MCMC posterior sampling on a cosmological model."),
     license = "MIT",
     keywords = "interactive visualizer cosmology",
     url = "http://packages.python.org/inviz",
     py_modules=["inviz"],
```

