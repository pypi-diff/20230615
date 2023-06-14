# Comparing `tmp/csdid-0.1.52.tar.gz` & `tmp/csdid-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.52.tar", last modified: Wed Jun 14 19:58:20 2023, max compression
+gzip compressed data, was "csdid-0.1.53.tar", last modified: Wed Jun 14 22:07:52 2023, max compression
```

## Comparing `csdid-0.1.52.tar` & `csdid-0.1.53.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.255183 csdid-0.1.52/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.52/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-14 19:58:20.255183 csdid-0.1.52/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.238178 csdid-0.1.52/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.250181 csdid-0.1.52/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     3890 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.252182 csdid-0.1.52/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.254184 csdid-0.1.52/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.52/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 19:58:20.248180 csdid-0.1.52/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-14 19:58:20.000000 csdid-0.1.52/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2023-06-14 19:58:20.000000 csdid-0.1.52/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 19:58:20.000000 csdid-0.1.52/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 19:58:20.000000 csdid-0.1.52/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 19:58:20.255183 csdid-0.1.52/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-14 19:57:46.000000 csdid-0.1.52/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:07:52.264865 csdid-0.1.53/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.53/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-14 22:07:52.264865 csdid-0.1.53/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 22:07:52.241860 csdid-0.1.53/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:07:52.257864 csdid-0.1.53/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     3474 2023-06-14 21:53:39.000000 csdid-0.1.53/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:07:52.259864 csdid-0.1.53/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:07:52.261865 csdid-0.1.53/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.53/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-06-14 21:38:37.000000 csdid-0.1.53/csdid/plots/ggdid.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.53/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:07:52.263865 csdid-0.1.53/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.53/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:07:52.254863 csdid-0.1.53/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-14 22:07:52.000000 csdid-0.1.53/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-14 22:07:52.000000 csdid-0.1.53/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:07:52.000000 csdid-0.1.53/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 22:07:52.000000 csdid-0.1.53/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 22:07:52.264865 csdid-0.1.53/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-14 22:07:50.000000 csdid-0.1.53/setup.py
```

### Comparing `csdid-0.1.52/LICENSE` & `csdid-0.1.53/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.52/PKG-INFO` & `csdid-0.1.53/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.52
+Version: 0.1.53
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.52/csdid/aggte_fnc/aggte.py` & `csdid-0.1.53/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.52/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.53/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.52/csdid/aggte_fnc/utils.py` & `csdid-0.1.53/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.52/csdid/att_gt.py` & `csdid-0.1.53/csdid/att_gt.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from csdid.aggte_fnc.aggte import aggte as agg_te
 
 from csdid.attgt_fnc.preprocess_did import pre_process_did
 from csdid.attgt_fnc.compute_att_gt import compute_att_gt
 
 from csdid.utils.mboot import mboot
 
-import numpy as np
+import numpy as np, pandas as pd
 
 # class ATTgt(AGGte):
 class ATTgt:
   def __init__(self, yname, tname, idname, gname, data, control_group = ['nevertreated', 'notyertreated'], 
   xformla: str = None, panel = True, allow_unbalanced_panel = True, 
   clustervar = None, weights_name = None, anticipation = 0, 
   cband = False, biters = 1000, alp = 0.05
@@ -61,15 +61,16 @@
     cband_upper = att + crit_val * se
     sig = (cband_upper < 0) | (cband_lower > 0)
     sig[np.isnan(sig)] = False
     sig_text = np.where(sig, "*", "")
 
     result.update(
       {
-        'std': se, 'l_se': cband_lower,
+        'se': se, 'l_se': cband_lower,
+        'c': crit_val,
         'u_se': cband_upper, 'sig': sig_text
        })
 
     self.results = result
     return self
   def summ_attgt(self, n = 4):
     result = self.results
@@ -98,36 +99,14 @@
       min_e=min_e, max_e=max_e, na_rm=na_rm, bstrap=bstrap, 
       biters=biters, cband=cband, alp=alp, clustervars=clustervars
     )
     return self
     
   
 
-
-# import yaml, pandas as pd
-
-# with open('configs/data.yml') as f:
-#   dt = yaml.safe_load(f)
-
-# data = pd.read_csv(dt['mpdata'])
-
-
-# yname = "lemp"
-# gname = "first.treat"
-# idname = "countyreal"
-# tname = "year"
-# xformla = f"lemp~1"
-# # data = mpdta
-# # print(data)
-# # print(tname)
-# b = ATTgt(yname, tname, idname, gname, data = data, xformla=xformla).fit()
-# c = b.summ_attgt().summary2
-# b.aggte(balance_e=1)
-# # print(c)
-
 # # print(aggte(b.MP, typec='dynamic'))
 # # data = pd.read_csv(dt['simdata'])
 
 # # yname = "Y"
 # # tname = "period"
 # # idname = "id"
 # # gname = "G"
```

### Comparing `csdid-0.1.52/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.53/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.52/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.53/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.52/csdid/utils/bmisc.py` & `csdid-0.1.53/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.52/csdid/utils/mboot.py` & `csdid-0.1.53/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.52/csdid.egg-info/PKG-INFO` & `csdid-0.1.53/csdid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.52
+Version: 0.1.53
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.52/setup.py` & `csdid-0.1.53/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.52',
+  version='0.1.53',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

