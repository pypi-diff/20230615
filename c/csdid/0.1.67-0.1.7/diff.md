# Comparing `tmp/csdid-0.1.67.tar.gz` & `tmp/csdid-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.67.tar", last modified: Thu Jun 15 14:57:29 2023, max compression
+gzip compressed data, was "csdid-0.1.7.tar", last modified: Thu Jun 15 15:08:23 2023, max compression
```

## Comparing `csdid-0.1.67.tar` & `csdid-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.383731 csdid-0.1.67/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.67/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-15 14:57:29.383731 csdid-0.1.67/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.352817 csdid-0.1.67/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.376730 csdid-0.1.67/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.67/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     6142 2023-06-14 23:28:42.000000 csdid-0.1.67/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.378730 csdid-0.1.67/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.380730 csdid-0.1.67/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.67/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.67/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.382731 csdid-0.1.67/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.67/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:57:29.368820 csdid-0.1.67/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-15 14:57:29.000000 csdid-0.1.67/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-06-15 14:57:29.000000 csdid-0.1.67/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:57:29.000000 csdid-0.1.67/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 14:57:29.000000 csdid-0.1.67/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 14:57:29.383731 csdid-0.1.67/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-15 14:57:18.000000 csdid-0.1.67/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.357235 csdid-0.1.7/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      533 2023-06-15 15:08:23.357235 csdid-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.339849 csdid-0.1.7/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.351219 csdid-0.1.7/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.7/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     6206 2023-06-15 14:58:53.000000 csdid-0.1.7/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.353234 csdid-0.1.7/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.354235 csdid-0.1.7/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.7/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.7/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.356235 csdid-0.1.7/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.348022 csdid-0.1.7/csdid.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-06-15 15:08:23.000000 csdid-0.1.7/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-06-15 15:08:23.000000 csdid-0.1.7/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 15:08:23.000000 csdid-0.1.7/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 15:08:23.000000 csdid-0.1.7/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 15:08:23.358235 csdid-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-06-15 15:08:08.000000 csdid-0.1.7/setup.py
```

### Comparing `csdid-0.1.67/LICENSE` & `csdid-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.67/PKG-INFO` & `csdid-0.1.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.67
+Version: 0.1.7
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.67/csdid/aggte_fnc/aggte.py` & `csdid-0.1.7/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.67/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.7/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.67/csdid/aggte_fnc/utils.py` & `csdid-0.1.7/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.67/csdid/att_gt.py` & `csdid-0.1.7/csdid/att_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 
     result.update(
       {
         'se': se, 'l_se': cband_lower,
         'c': crit_val,
         'u_se': cband_upper, 'sig': sig_text
        })
+    
+    self.results = result
 
     rst = result
     did_object = {
       'group': mp['group'],
       't': mp['t'],
       'att': rst['att'],
       'se': rst['se'],
@@ -112,19 +114,21 @@
     
     did_object.update({
       'type': typec
       }
     )
 
 
-    agg_te(
+    atte = agg_te(
       mp, typec=typec, balance_e=balance_e, 
       min_e=min_e, max_e=max_e, na_rm=na_rm, bstrap=bstrap, 
       biters=biters, cband=cband, alp=alp, clustervars=clustervars
     )
+
+    self.atte = atte
     return self
   def plot_attgt(self, ylim=None, 
                 xlab=None, 
                 ylab=None, 
                 title="Group",
                 xgap=1, 
                 ncol=1,
```

### Comparing `csdid-0.1.67/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.7/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.67/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.7/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.67/csdid/plots/gplot.py` & `csdid-0.1.7/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.67/csdid/utils/bmisc.py` & `csdid-0.1.7/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.67/csdid/utils/mboot.py` & `csdid-0.1.7/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.67/csdid.egg-info/PKG-INFO` & `csdid-0.1.7/csdid.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.67
+Version: 0.1.7
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.67/setup.py` & `csdid-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 from setuptools import setup, find_packages
 
+import os
+
+path = 'dist'
+files = os.listdir(path)
+
+for file in files:
+  pth = os.path.join(path, file)
+  os.remove(pth)
+
 setup(
   name = 'csdid',
-  version='0.1.67',
+  version='0.1.7',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
@@ -16,9 +25,8 @@
         "Topic :: Scientific/Engineering",
     ],
   packages=find_packages(),
   package_data={
     'data': ['data/*'],
     'configs': ['configs/*']
   }
-  
 )
```

