# Comparing `tmp/csdid-0.1.6.tar.gz` & `tmp/csdid-0.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.6.tar", last modified: Wed Jun 14 22:52:46 2023, max compression
+gzip compressed data, was "csdid-0.1.61.tar", last modified: Wed Jun 14 22:56:08 2023, max compression
```

## Comparing `csdid-0.1.6.tar` & `csdid-0.1.61.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:46.219562 csdid-0.1.6/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      533 2023-06-14 22:52:46.219562 csdid-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:46.203560 csdid-0.1.6/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:46.213562 csdid-0.1.6/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     4269 2023-06-14 22:51:13.000000 csdid-0.1.6/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:46.215562 csdid-0.1.6/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:46.217563 csdid-0.1.6/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.6/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     1565 2023-06-14 22:49:00.000000 csdid-0.1.6/csdid/plots/ggdid.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.6/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:46.218562 csdid-0.1.6/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.6/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:52:46.210561 csdid-0.1.6/csdid.egg-info/
--rw-rw-rw-   0        0        0      533 2023-06-14 22:52:46.000000 csdid-0.1.6/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-14 22:52:46.000000 csdid-0.1.6/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 22:52:46.000000 csdid-0.1.6/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 22:52:46.000000 csdid-0.1.6/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 22:52:46.219562 csdid-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-06-14 22:52:41.000000 csdid-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:56:08.901347 csdid-0.1.61/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.61/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-14 22:56:08.901347 csdid-0.1.61/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 22:56:08.884342 csdid-0.1.61/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:56:08.894345 csdid-0.1.61/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     4303 2023-06-14 22:55:57.000000 csdid-0.1.61/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:56:08.896345 csdid-0.1.61/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:56:08.898347 csdid-0.1.61/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.61/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     1565 2023-06-14 22:49:00.000000 csdid-0.1.61/csdid/plots/ggdid.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.61/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:56:08.900346 csdid-0.1.61/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.61/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:56:08.892345 csdid-0.1.61/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-14 22:56:08.000000 csdid-0.1.61/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-14 22:56:08.000000 csdid-0.1.61/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:56:08.000000 csdid-0.1.61/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 22:56:08.000000 csdid-0.1.61/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 22:56:08.901347 csdid-0.1.61/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-14 22:56:04.000000 csdid-0.1.61/setup.py
```

### Comparing `csdid-0.1.6/LICENSE` & `csdid-0.1.61/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/PKG-INFO` & `csdid-0.1.61/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.6
+Version: 0.1.61
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.6/csdid/aggte_fnc/aggte.py` & `csdid-0.1.61/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.61/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/csdid/aggte_fnc/utils.py` & `csdid-0.1.61/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/csdid/att_gt.py` & `csdid-0.1.61/csdid/att_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,24 @@
       {
         'se': se, 'l_se': cband_lower,
         'c': crit_val,
         'u_se': cband_upper, 'sig': sig_text
        })
 
     self.results = result
+    rst = self.results
+    mp = self.MP
+    did_object = {
+      'group': mp['group'],
+      't': mp['t'],
+      'att': rst['att'],
+      'se': rst['se'],
+      'c': rst['c'],
+    }
+    self.did_object = did_object
     return self
   def summ_attgt(self, n = 4):
     result = self.results
     att_gt = pd.DataFrame(result)
     name_attgt_df = ['Group', 'Time', 'ATT(g, t)', 'Post', "Std. Error", "[95% Pointwise", 'Conf. Band]', '']
     att_gt.columns = name_attgt_df
     att_gt = att_gt.round(n)
@@ -110,25 +120,16 @@
                 ncol=1, 
                 legend=True, 
                 group=None, 
                 ref_line=0,
                 theming=True, 
                 grtitle="Group"
                 ):
-    rst = self.results
-    mp = self.MP
-    did_object = {
-      'group': mp['group'],
-      't': mp['t'],
-      'att': rst['att'],
-      'se': rst['se'],
-      'c': rst['c'],
-    }
-    self.did_object = did_object
 
+    did_object = self.did_object
     ggdid_attge(
       did_object, ylim, xlab, title, xgap, ncol, legend, group,
       ref_line, theming, grtitle
     )
   
 
 # import yaml, pandas as pd
```

### Comparing `csdid-0.1.6/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.61/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.61/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/csdid/plots/ggdid.py` & `csdid-0.1.61/csdid/plots/ggdid.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/csdid/plots/gplot.py` & `csdid-0.1.61/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/csdid/utils/bmisc.py` & `csdid-0.1.61/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/csdid/utils/mboot.py` & `csdid-0.1.61/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.6/csdid.egg-info/PKG-INFO` & `csdid-0.1.61/csdid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.6
+Version: 0.1.61
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.6/setup.py` & `csdid-0.1.61/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.6',
+  version='0.1.61',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

