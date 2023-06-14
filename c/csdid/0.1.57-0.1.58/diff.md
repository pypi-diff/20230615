# Comparing `tmp/csdid-0.1.57.tar.gz` & `tmp/csdid-0.1.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.57.tar", last modified: Wed Jun 14 22:44:57 2023, max compression
+gzip compressed data, was "csdid-0.1.58.tar", last modified: Wed Jun 14 22:46:05 2023, max compression
```

## Comparing `csdid-0.1.57.tar` & `csdid-0.1.58.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 22:44:57.449753 csdid-0.1.57/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.57/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-14 22:44:57.449753 csdid-0.1.57/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 22:44:57.427747 csdid-0.1.57/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:44:57.438750 csdid-0.1.57/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     4241 2023-06-14 22:38:36.000000 csdid-0.1.57/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:44:57.440750 csdid-0.1.57/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:44:57.446752 csdid-0.1.57/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.57/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     1565 2023-06-14 22:44:45.000000 csdid-0.1.57/csdid/plots/ggdid.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.57/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:44:57.448751 csdid-0.1.57/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.57/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:44:57.435749 csdid-0.1.57/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-14 22:44:57.000000 csdid-0.1.57/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-14 22:44:57.000000 csdid-0.1.57/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 22:44:57.000000 csdid-0.1.57/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 22:44:57.000000 csdid-0.1.57/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 22:44:57.449753 csdid-0.1.57/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-14 22:44:53.000000 csdid-0.1.57/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:46:05.186085 csdid-0.1.58/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.58/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-14 22:46:05.186085 csdid-0.1.58/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 22:46:05.169082 csdid-0.1.58/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:46:05.180085 csdid-0.1.58/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     4257 2023-06-14 22:45:56.000000 csdid-0.1.58/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:46:05.181085 csdid-0.1.58/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:46:05.183085 csdid-0.1.58/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.58/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     1565 2023-06-14 22:44:45.000000 csdid-0.1.58/csdid/plots/ggdid.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.58/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:46:05.185086 csdid-0.1.58/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.58/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:46:05.177083 csdid-0.1.58/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-14 22:46:05.000000 csdid-0.1.58/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-14 22:46:05.000000 csdid-0.1.58/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:46:05.000000 csdid-0.1.58/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 22:46:05.000000 csdid-0.1.58/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 22:46:05.187086 csdid-0.1.58/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-14 22:46:00.000000 csdid-0.1.58/setup.py
```

### Comparing `csdid-0.1.57/LICENSE` & `csdid-0.1.58/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/PKG-INFO` & `csdid-0.1.58/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.57
+Version: 0.1.58
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.57/csdid/aggte_fnc/aggte.py` & `csdid-0.1.58/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.58/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/csdid/aggte_fnc/utils.py` & `csdid-0.1.58/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/csdid/att_gt.py` & `csdid-0.1.58/csdid/att_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,14 +124,15 @@
       'c': rst['c'],
     }
 
     plt = ggdid_attge(
       did_object, ylim, xlab, title, xgap, ncol, legend, group,
       ref_line, theming, grtitle
     )
+    return plt
   
 
 # import yaml, pandas as pd
 
 # with open('configs/data.yml') as f:
 #   dt = yaml.safe_load(f)
```

### Comparing `csdid-0.1.57/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.58/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.58/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/csdid/plots/ggdid.py` & `csdid-0.1.58/csdid/plots/ggdid.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/csdid/plots/gplot.py` & `csdid-0.1.58/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/csdid/utils/bmisc.py` & `csdid-0.1.58/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/csdid/utils/mboot.py` & `csdid-0.1.58/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.57/csdid.egg-info/PKG-INFO` & `csdid-0.1.58/csdid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.57
+Version: 0.1.58
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.57/setup.py` & `csdid-0.1.58/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.57',
+  version='0.1.58',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

