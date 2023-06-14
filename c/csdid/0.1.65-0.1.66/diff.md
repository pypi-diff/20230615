# Comparing `tmp/csdid-0.1.65.tar.gz` & `tmp/csdid-0.1.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.65.tar", last modified: Wed Jun 14 23:14:35 2023, max compression
+gzip compressed data, was "csdid-0.1.66.tar", last modified: Wed Jun 14 23:18:59 2023, max compression
```

## Comparing `csdid-0.1.65.tar` & `csdid-0.1.66.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:14:34.998808 csdid-0.1.65/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.65/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-14 23:14:34.997808 csdid-0.1.65/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 23:14:34.982804 csdid-0.1.65/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:14:34.992807 csdid-0.1.65/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     5103 2023-06-14 23:14:24.000000 csdid-0.1.65/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:14:34.993807 csdid-0.1.65/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:14:34.995808 csdid-0.1.65/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.65/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     1559 2023-06-14 23:10:46.000000 csdid-0.1.65/csdid/plots/ggdid.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.65/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:14:34.997808 csdid-0.1.65/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.65/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:14:34.989806 csdid-0.1.65/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-14 23:14:34.000000 csdid-0.1.65/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-14 23:14:34.000000 csdid-0.1.65/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:14:34.000000 csdid-0.1.65/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 23:14:34.000000 csdid-0.1.65/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 23:14:34.998808 csdid-0.1.65/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-14 23:14:29.000000 csdid-0.1.65/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.744376 csdid-0.1.66/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.66/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-14 23:18:59.744376 csdid-0.1.66/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.726372 csdid-0.1.66/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.738375 csdid-0.1.66/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     5052 2023-06-14 23:18:42.000000 csdid-0.1.66/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.739375 csdid-0.1.66/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.741375 csdid-0.1.66/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.66/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     1559 2023-06-14 23:10:46.000000 csdid-0.1.66/csdid/plots/ggdid.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.66/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.743376 csdid-0.1.66/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.66/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:18:59.735374 csdid-0.1.66/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-14 23:18:59.000000 csdid-0.1.66/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-14 23:18:59.000000 csdid-0.1.66/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:18:59.000000 csdid-0.1.66/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 23:18:59.000000 csdid-0.1.66/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:18:59.744376 csdid-0.1.66/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-14 23:18:58.000000 csdid-0.1.66/setup.py
```

### Comparing `csdid-0.1.65/LICENSE` & `csdid-0.1.66/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/PKG-INFO` & `csdid-0.1.66/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.65
+Version: 0.1.66
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.65/csdid/aggte_fnc/aggte.py` & `csdid-0.1.66/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.66/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/csdid/aggte_fnc/utils.py` & `csdid-0.1.66/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/csdid/att_gt.py` & `csdid-0.1.66/csdid/att_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,20 +53,20 @@
 
     dp['bstrap'] = bstrap
     dp['est_method'] = est_method
     dp['base_period'] = base_period
     self.dp = dp
     n = dp['n']
 
-    MP = {
+    mp = {
       'group': group, 'att': att, 't': tt,
       'DIDparams': dp, 'inffunc': inf_fnc, 
       'n': n
     }
-    self.MP = MP
+    self.MP = mp
 
 
     cband_lower = att - crit_val * se
     cband_upper = att + crit_val * se
     sig = (cband_upper < 0) | (cband_lower > 0)
     sig[np.isnan(sig)] = False
     sig_text = np.where(sig, "*", "")
@@ -74,17 +74,15 @@
     result.update(
       {
         'se': se, 'l_se': cband_lower,
         'c': crit_val,
         'u_se': cband_upper, 'sig': sig_text
        })
 
-    self.results = result
-    rst = self.results
-    mp = self.MP
+    rst = result
     did_object = {
       'group': mp['group'],
       't': mp['t'],
       'att': rst['att'],
       'se': rst['se'],
       'c': rst['c'],
     }
```

### Comparing `csdid-0.1.65/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.66/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.66/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/csdid/plots/ggdid.py` & `csdid-0.1.66/csdid/plots/ggdid.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/csdid/plots/gplot.py` & `csdid-0.1.66/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/csdid/utils/bmisc.py` & `csdid-0.1.66/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/csdid/utils/mboot.py` & `csdid-0.1.66/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.65/csdid.egg-info/PKG-INFO` & `csdid-0.1.66/csdid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.65
+Version: 0.1.66
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.65/setup.py` & `csdid-0.1.66/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.65',
+  version='0.1.66',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

