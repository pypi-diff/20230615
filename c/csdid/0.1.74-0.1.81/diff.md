# Comparing `tmp/csdid-0.1.74.tar.gz` & `tmp/csdid-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.74.tar", last modified: Thu Jun 15 15:34:44 2023, max compression
+gzip compressed data, was "csdid-0.1.81.tar", last modified: Thu Jun 15 20:53:20 2023, max compression
```

## Comparing `csdid-0.1.74.tar` & `csdid-0.1.81.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.942687 csdid-0.1.74/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.74/LICENSE
--rw-rw-rw-   0        0        0      534 2023-06-15 15:34:44.942687 csdid-0.1.74/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.926684 csdid-0.1.74/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.936686 csdid-0.1.74/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.74/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     6269 2023-06-15 15:34:07.000000 csdid-0.1.74/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.938686 csdid-0.1.74/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.939687 csdid-0.1.74/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.74/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.74/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.941687 csdid-0.1.74/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.74/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:34:44.934685 csdid-0.1.74/csdid.egg-info/
--rw-rw-rw-   0        0        0      534 2023-06-15 15:34:44.000000 csdid-0.1.74/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-06-15 15:34:44.000000 csdid-0.1.74/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 15:34:44.000000 csdid-0.1.74/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 15:34:44.000000 csdid-0.1.74/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 15:34:44.943688 csdid-0.1.74/setup.cfg
--rw-rw-rw-   0        0        0      708 2023-06-15 15:34:39.000000 csdid-0.1.74/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.762987 csdid-0.1.81/
+-rw-rw-rw-   0        0        0     1126 2023-06-15 19:08:39.000000 csdid-0.1.81/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-15 20:53:20.762987 csdid-0.1.81/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.738982 csdid-0.1.81/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-06-15 20:53:14.000000 csdid-0.1.81/csdid/_version.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.756986 csdid-0.1.81/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4712 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     6269 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.758986 csdid-0.1.81/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.759986 csdid-0.1.81/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.761987 csdid-0.1.81/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-15 19:08:39.000000 csdid-0.1.81/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 20:53:20.754985 csdid-0.1.81/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 20:53:20.000000 csdid-0.1.81/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 20:53:20.762987 csdid-0.1.81/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-06-15 20:52:55.000000 csdid-0.1.81/setup.py
```

### Comparing `csdid-0.1.74/LICENSE` & `csdid-0.1.81/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/PKG-INFO` & `csdid-0.1.81/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.74
+Version: 0.1.81
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.74/csdid/aggte_fnc/aggte.py` & `csdid-0.1.81/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.81/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/csdid/aggte_fnc/utils.py` & `csdid-0.1.81/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/csdid/att_gt.py` & `csdid-0.1.81/csdid/att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.81/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.81/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/csdid/plots/gplot.py` & `csdid-0.1.81/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/csdid/utils/bmisc.py` & `csdid-0.1.81/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/csdid/utils/mboot.py` & `csdid-0.1.81/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.74/csdid.egg-info/PKG-INFO` & `csdid-0.1.81/csdid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.74
+Version: 0.1.81
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

