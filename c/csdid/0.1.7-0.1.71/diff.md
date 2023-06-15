# Comparing `tmp/csdid-0.1.7.tar.gz` & `tmp/csdid-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.7.tar", last modified: Thu Jun 15 15:08:23 2023, max compression
+gzip compressed data, was "csdid-0.1.71.tar", last modified: Thu Jun 15 15:12:09 2023, max compression
```

## Comparing `csdid-0.1.7.tar` & `csdid-0.1.71.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.357235 csdid-0.1.7/
--rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      533 2023-06-15 15:08:23.357235 csdid-0.1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.339849 csdid-0.1.7/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.351219 csdid-0.1.7/csdid/aggte_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/aggte_fnc/__init__.py
--rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.7/csdid/aggte_fnc/aggte.py
--rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/aggte_fnc/compute_aggte.py
--rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/aggte_fnc/utils.py
--rw-rw-rw-   0        0        0     6206 2023-06-15 14:58:53.000000 csdid-0.1.7/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.353234 csdid-0.1.7/csdid/attgt_fnc/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/attgt_fnc/__init__.py
--rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/attgt_fnc/compute_att_gt.py
--rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/attgt_fnc/preprocess_did.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.354235 csdid-0.1.7/csdid/plots/
--rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.7/csdid/plots/__init__.py
--rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.7/csdid/plots/gplot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.356235 csdid-0.1.7/csdid/utils/
--rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/utils/__init__.py
--rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/utils/bmisc.py
--rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.7/csdid/utils/mboot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 15:08:23.348022 csdid-0.1.7/csdid.egg-info/
--rw-rw-rw-   0        0        0      533 2023-06-15 15:08:23.000000 csdid-0.1.7/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      484 2023-06-15 15:08:23.000000 csdid-0.1.7/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 15:08:23.000000 csdid-0.1.7/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 15:08:23.000000 csdid-0.1.7/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 15:08:23.358235 csdid-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-06-15 15:08:08.000000 csdid-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:12:09.277006 csdid-0.1.71/
+-rw-rw-rw-   0        0        0     1126 2023-06-14 18:06:31.000000 csdid-0.1.71/LICENSE
+-rw-rw-rw-   0        0        0      534 2023-06-15 15:12:09.277006 csdid-0.1.71/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 15:12:09.261003 csdid-0.1.71/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:12:09.271005 csdid-0.1.71/csdid/aggte_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/aggte_fnc/__init__.py
+-rw-rw-rw-   0        0        0     4712 2023-06-15 14:56:50.000000 csdid-0.1.71/csdid/aggte_fnc/aggte.py
+-rw-rw-rw-   0        0        0    22816 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/aggte_fnc/compute_aggte.py
+-rw-rw-rw-   0        0        0     7182 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/aggte_fnc/utils.py
+-rw-rw-rw-   0        0        0     6206 2023-06-15 14:58:53.000000 csdid-0.1.71/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:12:09.273005 csdid-0.1.71/csdid/attgt_fnc/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/attgt_fnc/__init__.py
+-rw-rw-rw-   0        0        0     5837 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/attgt_fnc/compute_att_gt.py
+-rw-rw-rw-   0        0        0     5389 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/attgt_fnc/preprocess_did.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:12:09.275006 csdid-0.1.71/csdid/plots/
+-rw-rw-rw-   0        0        0        0 2023-06-14 21:31:36.000000 csdid-0.1.71/csdid/plots/__init__.py
+-rw-rw-rw-   0        0        0     4016 2023-06-14 21:38:41.000000 csdid-0.1.71/csdid/plots/gplot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:12:09.276006 csdid-0.1.71/csdid/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/utils/__init__.py
+-rw-rw-rw-   0        0        0     1574 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/utils/bmisc.py
+-rw-rw-rw-   0        0        0     4280 2023-06-14 18:06:31.000000 csdid-0.1.71/csdid/utils/mboot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 15:12:09.269004 csdid-0.1.71/csdid.egg-info/
+-rw-rw-rw-   0        0        0      534 2023-06-15 15:12:09.000000 csdid-0.1.71/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-06-15 15:12:09.000000 csdid-0.1.71/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 15:12:09.000000 csdid-0.1.71/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 15:12:09.000000 csdid-0.1.71/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 15:12:09.278006 csdid-0.1.71/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-06-15 15:12:05.000000 csdid-0.1.71/setup.py
```

### Comparing `csdid-0.1.7/LICENSE` & `csdid-0.1.71/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/PKG-INFO` & `csdid-0.1.71/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.7
+Version: 0.1.71
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.7/csdid/aggte_fnc/aggte.py` & `csdid-0.1.71/csdid/aggte_fnc/aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/csdid/aggte_fnc/compute_aggte.py` & `csdid-0.1.71/csdid/aggte_fnc/compute_aggte.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/csdid/aggte_fnc/utils.py` & `csdid-0.1.71/csdid/aggte_fnc/utils.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/csdid/att_gt.py` & `csdid-0.1.71/csdid/att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/csdid/attgt_fnc/compute_att_gt.py` & `csdid-0.1.71/csdid/attgt_fnc/compute_att_gt.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/csdid/attgt_fnc/preprocess_did.py` & `csdid-0.1.71/csdid/attgt_fnc/preprocess_did.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/csdid/plots/gplot.py` & `csdid-0.1.71/csdid/plots/gplot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/csdid/utils/bmisc.py` & `csdid-0.1.71/csdid/utils/bmisc.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/csdid/utils/mboot.py` & `csdid-0.1.71/csdid/utils/mboot.py`

 * *Files identical despite different names*

### Comparing `csdid-0.1.7/csdid.egg-info/PKG-INFO` & `csdid-0.1.71/csdid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.7
+Version: 0.1.71
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

