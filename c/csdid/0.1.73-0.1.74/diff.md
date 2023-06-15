# Comparing `tmp/csdid-0.1.73.tar.gz` & `tmp/csdid-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.73.tar", last modified: Thu Jun 15 15:26:53 2023, max compression
+gzip compressed data, was "csdid-0.1.74.tar", last modified: Thu Jun 15 15:34:44 2023, max compression
```

## Comparing `csdid-0.1.73.tar` & `csdid-0.1.74.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.068709 csdid-0.1.73/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.73/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-15 15:26:53.068709 csdid-0.1.73/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.048704 csdid-0.1.73/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.062707 csdid-0.1.73/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.73/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     6247 2023-06-15 15:26:26.000000 csdid-0.1.73/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.064708 csdid-0.1.73/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.065708 csdid-0.1.73/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.73/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.73/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.067709 csdid-0.1.73/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.059707 csdid-0.1.73/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-15 15:26:52.000000 csdid-0.1.73/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-06-15 15:26:53.000000 csdid-0.1.73/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 15:26:52.000000 csdid-0.1.73/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 15:26:52.000000 csdid-0.1.73/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 15:26:53.068709 csdid-0.1.73/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-15 15:26:44.000000 csdid-0.1.73/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.942687 csdid-0.1.74/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.74/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-15 15:34:44.942687 csdid-0.1.74/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.926684 csdid-0.1.74/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.936686 csdid-0.1.74/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.74/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     6269 2023-06-15 15:34:07.000000 csdid-0.1.74/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.938686 csdid-0.1.74/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.939687 csdid-0.1.74/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.74/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.74/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.941687 csdid-0.1.74/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.934685 csdid-0.1.74/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-15 15:34:44.000000 csdid-0.1.74/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-06-15 15:34:44.000000 csdid-0.1.74/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 15:34:44.000000 csdid-0.1.74/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 15:34:44.000000 csdid-0.1.74/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 15:34:44.943688 csdid-0.1.74/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-15 15:34:39.000000 csdid-0.1.74/setup.py
```

### Comparing `csdid-0.1.73/LICENSE` & `csdid-0.1.74/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.73/PKG-INFO` & `csdid-0.1.74/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.73
+Version: 0.1.74
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.73/csdid/aggte_fnc/aggte.py` & `csdid-0.1.74/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.73/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.74/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.73/csdid/aggte_fnc/utils.py` & `csdid-0.1.74/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.73/csdid/att_gt.py` & `csdid-0.1.74/csdid/att_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,20 +87,21 @@
       'c': rst['c'],
     }
     self.did_object = did_object
     return self
   def summ_attgt(self, n = 4):
     result = self.results
     att_gt = pd.DataFrame(result)
-    print(att_gt)
+    att_gt = att_gt.drop('c', axis=1)
     name_attgt_df = ['Group', 'Time', 'ATT(g, t)', 'Post', "Std. Error", "[95% Pointwise", 'Conf. Band]', '']
     att_gt.columns = name_attgt_df
     att_gt = att_gt.round(n)
     self.summary2 = att_gt
     return self
+
   def aggte(
     self, 
     typec         = "group",
     balance_e     = None,
     min_e         = float('-inf'),
     max_e         = float('inf'),
     na_rm         = False,
```

### Comparing `csdid-0.1.73/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.74/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.73/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.74/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.73/csdid/plots/gplot.py` & `csdid-0.1.74/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.73/csdid/utils/bmisc.py` & `csdid-0.1.74/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.73/csdid/utils/mboot.py` & `csdid-0.1.74/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.73/csdid.egg-info/PKG-INFO` & `csdid-0.1.74/csdid.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.73
+Version: 0.1.74
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.73/setup.py` & `csdid-0.1.74/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
   name = 'csdid',
-  version='0.1.73',
+  version='0.1.74',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

