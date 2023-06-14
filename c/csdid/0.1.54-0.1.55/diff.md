# Comparing `tmp/csdid-0.1.54.tar.gz` & `tmp/csdid-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.54.tar", last modified: Wed Jun 14 22:37:20 2023, max compression
+gzip compressed data, was "csdid-0.1.55.tar", last modified: Wed Jun 14 22:38:48 2023, max compression
```

## Comparing `csdid-0.1.54.tar` & `csdid-0.1.55.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 22:37:20.941857 csdid-0.1.54/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.54/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-14 22:37:20.941857 csdid-0.1.54/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 22:37:20.925853 csdid-0.1.54/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:37:20.935855 csdid-0.1.54/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     4219 2023-06-14 22:33:45.000000 csdid-0.1.54/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:37:20.937855 csdid-0.1.54/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:37:20.938856 csdid-0.1.54/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.54/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     1537 2023-06-14 22:34:08.000000 csdid-0.1.54/csdid/plots/ggdid.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.54/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:37:20.940857 csdid-0.1.54/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.54/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 22:37:20.932855 csdid-0.1.54/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-14 22:37:20.000000 csdid-0.1.54/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-14 22:37:20.000000 csdid-0.1.54/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 22:37:20.000000 csdid-0.1.54/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 22:37:20.000000 csdid-0.1.54/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 22:37:20.941857 csdid-0.1.54/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-14 22:37:08.000000 csdid-0.1.54/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:38:48.223108 csdid-0.1.55/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.55/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-14 22:38:48.222108 csdid-0.1.55/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 22:38:48.206104 csdid-0.1.55/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:38:48.216107 csdid-0.1.55/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     4241 2023-06-14 22:38:36.000000 csdid-0.1.55/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:38:48.218107 csdid-0.1.55/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:38:48.220108 csdid-0.1.55/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.55/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     1537 2023-06-14 22:34:08.000000 csdid-0.1.55/csdid/plots/ggdid.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.55/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:38:48.222108 csdid-0.1.55/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.55/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 22:38:48.214107 csdid-0.1.55/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-14 22:38:48.000000 csdid-0.1.55/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-14 22:38:48.000000 csdid-0.1.55/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 22:38:48.000000 csdid-0.1.55/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 22:38:48.000000 csdid-0.1.55/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 22:38:48.223108 csdid-0.1.55/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-14 22:38:43.000000 csdid-0.1.55/setup.py
```

### Comparing `csdid-0.1.54/LICENSE` & `csdid-0.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/PKG-INFO` & `csdid-0.1.55/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.54
+Version: 0.1.55
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.54/csdid/aggte_fnc/aggte.py` & `csdid-0.1.55/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.55/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/csdid/aggte_fnc/utils.py` & `csdid-0.1.55/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/csdid/att_gt.py` & `csdid-0.1.55/csdid/att_gt.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,28 +126,28 @@
 
     plt = ggdid_attge(
       did_object, ylim, xlab, title, xgap, ncol, legend, group,
       ref_line, theming, grtitle
     )
   
 
-import yaml, pandas as pd
+# import yaml, pandas as pd
 
-with open('configs/data.yml') as f:
-  dt = yaml.safe_load(f)
+# with open('configs/data.yml') as f:
+#   dt = yaml.safe_load(f)
 
-data = pd.read_csv(dt['mpdata'])
-yname = "lemp"
-gname = "first.treat"
-idname = "countyreal"
-tname = "year"
-xformla = f"lemp~1"
+# data = pd.read_csv(dt['mpdata'])
+# yname = "lemp"
+# gname = "first.treat"
+# idname = "countyreal"
+# tname = "year"
+# xformla = f"lemp~1"
 
-b = ATTgt(yname, tname, idname, gname, data = data, xformla=xformla).fit()
-b.plot_attgt()
+# b = ATTgt(yname, tname, idname, gname, data = data, xformla=xformla).fit()
+# b.plot_attgt()
 
 # b = aggte(mp, typec='simple')
 # # print(b)
 
 # print(b)
 
 # print(a)
```

### Comparing `csdid-0.1.54/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.55/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.55/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/csdid/plots/ggdid.py` & `csdid-0.1.55/csdid/plots/ggdid.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/csdid/plots/gplot.py` & `csdid-0.1.55/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/csdid/utils/bmisc.py` & `csdid-0.1.55/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/csdid/utils/mboot.py` & `csdid-0.1.55/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.54/csdid.egg-info/PKG-INFO` & `csdid-0.1.55/csdid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.54
+Version: 0.1.55
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.54/setup.py` & `csdid-0.1.55/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.54',
+  version='0.1.55',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

