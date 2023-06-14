# Comparing `tmp/csdid-0.1.63.tar.gz` & `tmp/csdid-0.1.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.63.tar", last modified: Wed Jun 14 23:05:54 2023, max compression
+gzip compressed data, was "csdid-0.1.64.tar", last modified: Wed Jun 14 23:11:36 2023, max compression
```

## Comparing `csdid-0.1.63.tar` & `csdid-0.1.64.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.463149 csdid-0.1.63/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.63/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-14 23:05:54.462149 csdid-0.1.63/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.446146 csdid-0.1.63/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.456148 csdid-0.1.63/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     4628 2023-06-14 23:05:22.000000 csdid-0.1.63/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.458148 csdid-0.1.63/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.460148 csdid-0.1.63/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.63/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     1565 2023-06-14 22:49:00.000000 csdid-0.1.63/csdid/plots/ggdid.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.63/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.462149 csdid-0.1.63/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.63/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:05:54.454147 csdid-0.1.63/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-14 23:05:54.000000 csdid-0.1.63/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-14 23:05:54.000000 csdid-0.1.63/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:05:54.000000 csdid-0.1.63/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 23:05:54.000000 csdid-0.1.63/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 23:05:54.463149 csdid-0.1.63/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-14 23:05:49.000000 csdid-0.1.63/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:36.003994 csdid-0.1.64/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.64/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-14 23:11:36.003994 csdid-0.1.64/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:35.986989 csdid-0.1.64/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:35.996992 csdid-0.1.64/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4700 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     4891 2023-06-14 23:11:20.000000 csdid-0.1.64/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:35.998992 csdid-0.1.64/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:36.000993 csdid-0.1.64/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.64/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     1559 2023-06-14 23:10:46.000000 csdid-0.1.64/csdid/plots/ggdid.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.64/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:36.002993 csdid-0.1.64/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.64/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-14 23:11:35.994992 csdid-0.1.64/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-14 23:11:35.000000 csdid-0.1.64/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-14 23:11:35.000000 csdid-0.1.64/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 23:11:35.000000 csdid-0.1.64/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-14 23:11:35.000000 csdid-0.1.64/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-14 23:11:36.003994 csdid-0.1.64/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-14 23:11:31.000000 csdid-0.1.64/setup.py
```

### Comparing `csdid-0.1.63/LICENSE` & `csdid-0.1.64/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.63/PKG-INFO` & `csdid-0.1.64/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.63
+Version: 0.1.64
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.63/csdid/aggte_fnc/aggte.py` & `csdid-0.1.64/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.63/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.64/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.63/csdid/aggte_fnc/utils.py` & `csdid-0.1.64/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.63/csdid/att_gt.py` & `csdid-0.1.64/csdid/att_gt.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,9 +145,17 @@
     results['group'] = np.repeat(g, Y)
     results['grtitle'] = grtitle + ' ' + results['group'].astype(str)
     results['att'] = did_object['att']
     results['att_se'] = did_object['se']
     results['post'] = np.where(results['year'] >= grp, 1, 0)
     results['year'] = results['year']
     results['c'] = did_object['c']
+    results = results.query(
+      'group in @group'
+      )
+    
+    self.data_plot_attgt = results
 
-    return results 
+    mplots = gplot(results, ylim, xlab, ylab, title, xgap, legend, ref_line, theming) + \
+              facet_wrap('~ grtitle', ncol=ncol, scales='free')
+
+    return mplots
```

### Comparing `csdid-0.1.63/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.64/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.63/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.64/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.63/csdid/plots/ggdid.py` & `csdid-0.1.64/csdid/plots/ggdid.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,17 +32,17 @@
   results['grtitle'] = grtitle + ' ' + results['group'].astype(str)
   results['att'] = did_object['att']
   results['att_se'] = did_object['se']
   results['post'] = np.where(results['year'] >= grp, 1, 0)
   results['year'] = results['year']
   results['c'] = did_object['c']
 
-  # results = results.query(
-  #   'group in @group'
-  # )
+  results = results.query(
+    'group in @group'
+  )
 
   if group is None:
     group = g
     if any(group not in g for group in group):
       raise ValueError("Some of the specified groups do not exist in the data. Reporting all available groups.")
       group = g
```

### Comparing `csdid-0.1.63/csdid/plots/gplot.py` & `csdid-0.1.64/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.63/csdid/utils/bmisc.py` & `csdid-0.1.64/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.63/csdid/utils/mboot.py` & `csdid-0.1.64/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.63/csdid.egg-info/PKG-INFO` & `csdid-0.1.64/csdid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.63
+Version: 0.1.64
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.63/setup.py` & `csdid-0.1.64/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'csdid',
-  version='0.1.63',
+  version='0.1.64',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

