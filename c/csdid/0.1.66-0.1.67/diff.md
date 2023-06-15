# Comparing `tmp/csdid-0.1.66.tar.gz` & `tmp/csdid-0.1.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.66.tar", last modified: Wed Jun 14 23:18:59 2023, max compression
+gzip compressed data, was "csdid-0.1.67.tar", last modified: Thu Jun 15 14:57:29 2023, max compression
```

## Comparing `csdid-0.1.66.tar` & `csdid-0.1.67.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.744376 csdid-0.1.66/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.66/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-14 23:18:59.744376 csdid-0.1.66/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.726372 csdid-0.1.66/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.738375 csdid-0.1.66/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     5052 2023-06-14 23:18:42.000000 csdid-0.1.66/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.739375 csdid-0.1.66/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.741375 csdid-0.1.66/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.66/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     1559 2023-06-14 23:10:46.000000 csdid-0.1.66/csdid/plots/ggdid.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.66/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.743376 csdid-0.1.66/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.735374 csdid-0.1.66/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-14 23:18:59.000000 csdid-0.1.66/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-14 23:18:59.000000 csdid-0.1.66/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:18:59.000000 csdid-0.1.66/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 23:18:59.000000 csdid-0.1.66/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 23:18:59.744376 csdid-0.1.66/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-14 23:18:58.000000 csdid-0.1.66/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.383731 csdid-0.1.67/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.67/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-15 14:57:29.383731 csdid-0.1.67/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.352817 csdid-0.1.67/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.376730 csdid-0.1.67/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.67/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     6142 2023-06-14 23:28:42.000000 csdid-0.1.67/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.378730 csdid-0.1.67/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.380730 csdid-0.1.67/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.67/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.67/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.382731 csdid-0.1.67/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.368820 csdid-0.1.67/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-15 14:57:29.000000 csdid-0.1.67/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-06-15 14:57:29.000000 csdid-0.1.67/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 14:57:29.000000 csdid-0.1.67/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 14:57:29.000000 csdid-0.1.67/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 14:57:29.383731 csdid-0.1.67/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-15 14:57:18.000000 csdid-0.1.67/setup.py
```

### Comparing `csdid-0.1.66/LICENSE` & `csdid-0.1.67/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.66/PKG-INFO` & `csdid-0.1.67/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.66
+Version: 0.1.67
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.66/csdid/aggte_fnc/aggte.py` & `csdid-0.1.67/csdid/aggte_fnc/aggte.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,20 +92,22 @@
           bstrap=None, 
           biters=None, 
           cband=None, 
           alp=None, 
           clustervars=None):
     call = inspect.currentframe().f_back.f_locals.copy()
 
-    compute_aggte(MP=MP, 
+    return compute_aggte(MP=MP, 
                   typec=typec, 
                   balance_e=balance_e, 
                   min_e=min_e, 
                   max_e=max_e, 
                   na_rm=na_rm,
                   bstrap=bstrap, 
                   biters=biters, 
                   cband=cband, 
                   alp=alp, 
                   clustervars=clustervars, 
                   call=call)
 
+ 
+
```

### Comparing `csdid-0.1.66/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.67/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.66/csdid/aggte_fnc/utils.py` & `csdid-0.1.67/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.66/csdid/att_gt.py` & `csdid-0.1.67/csdid/att_gt.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 from csdid.aggte_fnc.aggte import aggte as agg_te
 
 from csdid.attgt_fnc.preprocess_did import pre_process_did
 from csdid.attgt_fnc.compute_att_gt import compute_att_gt
 
 from csdid.utils.mboot import mboot
 
-from csdid.plots.gplot import gplot
-from plotnine import ggplot, aes, geom_point, geom_errorbar, scale_y_continuous, scale_x_continuous, \
-    scale_color_manual, labs, geom_hline, theme, element_text, element_rect, element_line, \
-    scale_x_discrete
+from csdid.plots.gplot import gplot, splot
+
 
 from plotnine import ggplot, facet_wrap
 
 
 import numpy as np, pandas as pd
 
 # class ATTgt(AGGte):
@@ -106,14 +104,22 @@
     bstrap        = None,
     biters        = None,
     cband         = None,
     alp           = None,
     clustervars   = None,
     ):
     mp = self.MP
+    did_object = self.did_object
+    
+    did_object.update({
+      'type': typec
+      }
+    )
+
+
     agg_te(
       mp, typec=typec, balance_e=balance_e, 
       min_e=min_e, max_e=max_e, na_rm=na_rm, bstrap=bstrap, 
       biters=biters, cband=cband, alp=alp, clustervars=clustervars
     )
     return self
   def plot_attgt(self, ylim=None, 
@@ -159,8 +165,45 @@
       )
     
     self.data_plot_attgt = results
 
     mplots = gplot(results, ylim, xlab, ylab, title, xgap, legend, ref_line, theming) + \
               facet_wrap('~ grtitle', ncol=ncol, scales='free')
 
-    return mplots 
+    return mplots 
+  def plot_aggte(self, ylim=None, 
+                   xlab=None, 
+                   ylab=None, 
+                   title="", 
+                   xgap=1, 
+                   legend=True, 
+                   ref_line=0, 
+                   theming=True,
+                   **kwargs):
+    did_object = self.did_object
+
+    post_treat = 1 * (np.asarray(did_object["egt"]).astype(int) >= 0)
+    
+    results = {
+        "year": list(map(int, did_object["egt"])),
+        "att": did_object["att_egt"],
+        "att_se": did_object["se_egt"][0],
+        "post": post_treat
+    }
+    
+    results = pd.DataFrame(results)
+    
+    if did_object['crit_val_egt'] is None:
+        results['c'] = abs(norm.ppf(0.025))
+    else:
+        results['c'] = did_object['crit_val_egt']
+
+    if title == "":
+        title = "Average Effect by Group" if did_object["type"] == "group" else "Average Effect by Length of Exposure"
+
+    if did_object['type'] == 'group':
+        p = splot(results, ylim, xlab, ylab, title, legend, ref_line, theming)
+    else:
+        p = gplot(results, ylim, xlab, ylab, title, xgap, legend, ref_line, theming)
+    # p
+    # print(p) 
+    return p
```

### Comparing `csdid-0.1.66/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.67/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.66/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.67/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.66/csdid/plots/gplot.py` & `csdid-0.1.67/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.66/csdid/utils/bmisc.py` & `csdid-0.1.67/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.66/csdid/utils/mboot.py` & `csdid-0.1.67/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.66/csdid.egg-info/PKG-INFO` & `csdid-0.1.67/csdid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.66
+Version: 0.1.67
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.66/setup.py` & `csdid-0.1.67/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.66',
+  version='0.1.67',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

