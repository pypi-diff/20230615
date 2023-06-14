# Comparing `tmp/csdid-0.1.62.tar.gz` & `tmp/csdid-0.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.62.tar", last modified: Wed Jun 14 23:04:19 2023, max compression
+gzip compressed data, was "csdid-0.1.63.tar", last modified: Wed Jun 14 23:05:54 2023, max compression
```

## Comparing `csdid-0.1.62.tar` & `csdid-0.1.63.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:04:19.464991 csdid-0.1.62/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.62/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-14 23:04:19.464991 csdid-0.1.62/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 23:04:19.448988 csdid-0.1.62/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:04:19.458991 csdid-0.1.62/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     4568 2023-06-14 23:04:00.000000 csdid-0.1.62/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:04:19.460991 csdid-0.1.62/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:04:19.462991 csdid-0.1.62/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.62/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     1565 2023-06-14 22:49:00.000000 csdid-0.1.62/csdid/plots/ggdid.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.62/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:04:19.463992 csdid-0.1.62/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.62/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:04:19.456989 csdid-0.1.62/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-14 23:04:19.000000 csdid-0.1.62/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-14 23:04:19.000000 csdid-0.1.62/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:04:19.000000 csdid-0.1.62/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 23:04:19.000000 csdid-0.1.62/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 23:04:19.465992 csdid-0.1.62/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-14 23:04:16.000000 csdid-0.1.62/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.463149 csdid-0.1.63/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.63/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-14 23:05:54.462149 csdid-0.1.63/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.446146 csdid-0.1.63/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.456148 csdid-0.1.63/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     4628 2023-06-14 23:05:22.000000 csdid-0.1.63/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.458148 csdid-0.1.63/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.460148 csdid-0.1.63/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.63/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     1565 2023-06-14 22:49:00.000000 csdid-0.1.63/csdid/plots/ggdid.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.63/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.462149 csdid-0.1.63/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.454147 csdid-0.1.63/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-14 23:05:54.000000 csdid-0.1.63/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-14 23:05:54.000000 csdid-0.1.63/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:05:54.000000 csdid-0.1.63/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 23:05:54.000000 csdid-0.1.63/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:05:54.463149 csdid-0.1.63/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-14 23:05:49.000000 csdid-0.1.63/setup.py
```

### Comparing `csdid-0.1.62/LICENSE` & `csdid-0.1.63/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/PKG-INFO` & `csdid-0.1.63/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.62
+Version: 0.1.63
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.62/csdid/aggte_fnc/aggte.py` & `csdid-0.1.63/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.63/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/csdid/aggte_fnc/utils.py` & `csdid-0.1.63/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/csdid/att_gt.py` & `csdid-0.1.63/csdid/att_gt.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,14 +129,17 @@
                 ref_line=0,
                 theming=True, 
                 grtitle="Group"
                 ):
 
     did_object = self.did_object
 
+    grp = did_object['group']
+    t_i = did_object['t']
+
     G = len(np.unique(grp))
     Y = len(np.unique(t_i))
     g = np.unique(grp)[np.argsort(np.unique(grp))].astype(int)
     y = np.unique(t_i)
 
     results = pd.DataFrame({'year': np.tile(y, G)})
     results['group'] = np.repeat(g, Y)
```

### Comparing `csdid-0.1.62/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.63/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.63/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/csdid/plots/ggdid.py` & `csdid-0.1.63/csdid/plots/ggdid.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/csdid/plots/gplot.py` & `csdid-0.1.63/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/csdid/utils/bmisc.py` & `csdid-0.1.63/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/csdid/utils/mboot.py` & `csdid-0.1.63/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.62/csdid.egg-info/PKG-INFO` & `csdid-0.1.63/csdid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.62
+Version: 0.1.63
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.62/setup.py` & `csdid-0.1.63/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.62',
+  version='0.1.63',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

