# Comparing `tmp/csdid-0.1.72.tar.gz` & `tmp/csdid-0.1.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.72.tar", last modified: Thu Jun 15 15:22:00 2023, max compression
+gzip compressed data, was "csdid-0.1.73.tar", last modified: Thu Jun 15 15:26:53 2023, max compression
```

## Comparing `csdid-0.1.72.tar` & `csdid-0.1.73.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:00.919434 csdid-0.1.72/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.72/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-15 15:22:00.918435 csdid-0.1.72/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:00.898430 csdid-0.1.72/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:00.912433 csdid-0.1.72/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.72/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     6228 2023-06-15 15:21:40.000000 csdid-0.1.72/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:00.914434 csdid-0.1.72/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:00.915434 csdid-0.1.72/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.72/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.72/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:00.918435 csdid-0.1.72/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.72/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:22:00.909433 csdid-0.1.72/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-15 15:22:00.000000 csdid-0.1.72/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-06-15 15:22:00.000000 csdid-0.1.72/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 15:22:00.000000 csdid-0.1.72/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 15:22:00.000000 csdid-0.1.72/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 15:22:00.919434 csdid-0.1.72/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-15 15:21:51.000000 csdid-0.1.72/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.068709 csdid-0.1.73/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.73/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-15 15:26:53.068709 csdid-0.1.73/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.048704 csdid-0.1.73/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.062707 csdid-0.1.73/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.73/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     6247 2023-06-15 15:26:26.000000 csdid-0.1.73/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.064708 csdid-0.1.73/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.065708 csdid-0.1.73/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.73/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.73/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.067709 csdid-0.1.73/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.73/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:26:53.059707 csdid-0.1.73/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-15 15:26:52.000000 csdid-0.1.73/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-06-15 15:26:53.000000 csdid-0.1.73/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 15:26:52.000000 csdid-0.1.73/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 15:26:52.000000 csdid-0.1.73/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 15:26:53.068709 csdid-0.1.73/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-15 15:26:44.000000 csdid-0.1.73/setup.py
```

### Comparing `csdid-0.1.72/LICENSE` & `csdid-0.1.73/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.72/PKG-INFO` & `csdid-0.1.73/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.72
+Version: 0.1.73
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.72/csdid/aggte_fnc/aggte.py` & `csdid-0.1.73/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.72/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.73/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.72/csdid/aggte_fnc/utils.py` & `csdid-0.1.73/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.72/csdid/att_gt.py` & `csdid-0.1.73/csdid/att_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
       'c': rst['c'],
     }
     self.did_object = did_object
     return self
   def summ_attgt(self, n = 4):
     result = self.results
     att_gt = pd.DataFrame(result)
+    print(att_gt)
     name_attgt_df = ['Group', 'Time', 'ATT(g, t)', 'Post', "Std. Error", "[95% Pointwise", 'Conf. Band]', '']
     att_gt.columns = name_attgt_df
     att_gt = att_gt.round(n)
     self.summary2 = att_gt
     return self
   def aggte(
     self,
```

### Comparing `csdid-0.1.72/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.73/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.72/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.73/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.72/csdid/plots/gplot.py` & `csdid-0.1.73/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.72/csdid/utils/bmisc.py` & `csdid-0.1.73/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.72/csdid/utils/mboot.py` & `csdid-0.1.73/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.72/csdid.egg-info/PKG-INFO` & `csdid-0.1.73/csdid.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.72
+Version: 0.1.73
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.72/setup.py` & `csdid-0.1.73/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 
 
 setup(
   name = 'csdid',
-  version='0.1.72',
+  version='0.1.73',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

