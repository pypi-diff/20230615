# Comparing `tmp/com.castsoftware.uc.arg-1.5.4.3.tar.gz` & `tmp/com.castsoftware.uc.arg-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.arg-1.5.4.3.tar", last modified: Wed Jun  7 19:21:15 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.arg-1.5.5.tar", last modified: Thu Jun 15 16:12:10 2023, max compression
```

## Comparing `com.castsoftware.uc.arg-1.5.4.3.tar` & `com.castsoftware.uc.arg-1.5.5.tar`

### file list

```diff
@@ -1,26 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 19:21:15.694851 com.castsoftware.uc.arg-1.5.4.3/
--rw-rw-rw-   0        0        0      591 2023-06-07 19:21:15.637968 com.castsoftware.uc.arg-1.5.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-07 19:21:15.520151 com.castsoftware.uc.arg-1.5.4.3/cast_arg/
--rw-rw-rw-   0        0        0     1429 2021-09-15 15:25:49.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/Effort.csv
--rw-rw-rw-   0        0        0        0 2023-01-25 18:38:49.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/__init__.py
--rw-rw-rw-   0        0        0     7714 2023-04-18 19:43:06.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/actionPlan.py
--rw-rw-rw-   0        0        0     1004 2022-12-28 17:17:44.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/cause.json
--rw-rw-rw-   0        0        0     6237 2023-01-25 16:41:12.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/config.py
--rw-rw-rw-   0        0        0    33605 2023-06-06 20:22:02.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/convert.py
--rw-rw-rw-   0        0        0      809 2023-04-19 12:46:04.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/main.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:21:15.554280 com.castsoftware.uc.arg-1.5.4.3/cast_arg/pages/
--rw-rw-rw-   0        0        0        0 2023-03-07 13:55:37.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/pages/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/pages/aip.py
--rw-rw-rw-   0        0        0     1478 2023-03-07 15:35:56.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/pages/green_it.py
--rw-rw-rw-   0        0        0    28453 2023-01-25 23:20:11.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/powerpoint.py
--rw-rw-rw-   0        0        0    33081 2023-06-07 18:51:03.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/restCall.py
--rw-rw-rw-   0        0        0     7182 2023-01-25 18:55:23.000000 com.castsoftware.uc.arg-1.5.4.3/cast_arg/stats.py
-drwxrwxrwx   0        0        0        0 2023-06-07 19:21:15.623847 com.castsoftware.uc.arg-1.5.4.3/com.castsoftware.uc.arg.egg-info/
--rw-rw-rw-   0        0        0      591 2023-06-07 19:21:15.000000 com.castsoftware.uc.arg-1.5.4.3/com.castsoftware.uc.arg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      535 2023-06-07 19:21:15.000000 com.castsoftware.uc.arg-1.5.4.3/com.castsoftware.uc.arg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 19:21:15.000000 com.castsoftware.uc.arg-1.5.4.3/com.castsoftware.uc.arg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-06-07 19:21:15.000000 com.castsoftware.uc.arg-1.5.4.3/com.castsoftware.uc.arg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 19:21:15.000000 com.castsoftware.uc.arg-1.5.4.3/com.castsoftware.uc.arg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      647 2023-06-07 19:19:27.000000 com.castsoftware.uc.arg-1.5.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 19:21:15.694851 com.castsoftware.uc.arg-1.5.4.3/setup.cfg
--rw-rw-rw-   0        0        0      422 2023-01-26 17:04:17.000000 com.castsoftware.uc.arg-1.5.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:12:10.863132 com.castsoftware.uc.arg-1.5.5/
+-rw-rw-rw-   0        0        0      589 2023-06-15 16:12:10.849390 com.castsoftware.uc.arg-1.5.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 16:12:10.729549 com.castsoftware.uc.arg-1.5.5/cast_arg/
+-rw-rw-rw-   0        0        0     1429 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/Effort.csv
+-rw-rw-rw-   0        0        0        0 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/__init__.py
+-rw-rw-rw-   0        0        0     7714 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/actionPlan.py
+-rw-rw-rw-   0        0        0     1004 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/cause.json
+-rw-rw-rw-   0        0        0     6237 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/config.py
+-rw-rw-rw-   0        0        0    33594 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/convert.py
+-rw-rw-rw-   0        0        0      809 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/main.py
+-rw-rw-rw-   0        0        0    28453 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/powerpoint.py
+-rw-rw-rw-   0        0        0    33081 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/restCall.py
+-rw-rw-rw-   0        0        0     7182 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/cast_arg/stats.py
+drwxrwxrwx   0        0        0        0 2023-06-15 16:12:10.838464 com.castsoftware.uc.arg-1.5.5/com.castsoftware.uc.arg.egg-info/
+-rw-rw-rw-   0        0        0      589 2023-06-15 16:12:10.000000 com.castsoftware.uc.arg-1.5.5/com.castsoftware.uc.arg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-06-15 16:12:10.000000 com.castsoftware.uc.arg-1.5.5/com.castsoftware.uc.arg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 16:12:10.000000 com.castsoftware.uc.arg-1.5.5/com.castsoftware.uc.arg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-06-15 16:12:10.000000 com.castsoftware.uc.arg-1.5.5/com.castsoftware.uc.arg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-15 16:12:10.000000 com.castsoftware.uc.arg-1.5.5/com.castsoftware.uc.arg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      645 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-15 16:12:10.863132 com.castsoftware.uc.arg-1.5.5/setup.cfg
+-rw-rw-rw-   0        0        0      422 2023-06-15 16:10:33.000000 com.castsoftware.uc.arg-1.5.5/setup.py
```

### Comparing `com.castsoftware.uc.arg-1.5.4.3/PKG-INFO` & `com.castsoftware.uc.arg-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.5.4.3
+Version: 1.5.5
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `com.castsoftware.uc.arg-1.5.4.3/cast_arg/Effort.csv` & `com.castsoftware.uc.arg-1.5.5/cast_arg/Effort.csv`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.3/cast_arg/actionPlan.py` & `com.castsoftware.uc.arg-1.5.5/cast_arg/actionPlan.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.3/cast_arg/cause.json` & `com.castsoftware.uc.arg-1.5.5/cast_arg/cause.json`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.3/cast_arg/config.py` & `com.castsoftware.uc.arg-1.5.5/cast_arg/config.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.3/cast_arg/convert.py` & `com.castsoftware.uc.arg-1.5.5/cast_arg/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,18 +317,18 @@
                     hl_summary_critical.add_violations(oss_crit.violations)
 
                     hl_summary_high_near.add_components(oss_high.components)
                     hl_summary_high_near.add_components(oss_med.components)
 
                     hl_summary.add_components(components)
 
-                    if not lic.empty:
-                        lic_summary.add_high(lic.high)
-                        lic_summary.add_medium(lic.medium)
-                        lic_summary.add_low(lic.low)
+#                    if not lic.empty:
+                    lic_summary.add_high(lic.high)
+                    lic_summary.add_medium(lic.medium)
+                    lic_summary.add_low(lic.low)
                 except KeyError as ex:
                     self.warning(f'OSS information not found {str(ex)}')
                 """
                     Cloud ready excel sheet generation
                 """
                 try:
                     cloud = self._hl_data.get_cloud_info(hl_id)
```

### Comparing `com.castsoftware.uc.arg-1.5.4.3/cast_arg/main.py` & `com.castsoftware.uc.arg-1.5.5/cast_arg/main.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.3/cast_arg/powerpoint.py` & `com.castsoftware.uc.arg-1.5.5/cast_arg/powerpoint.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.3/cast_arg/restCall.py` & `com.castsoftware.uc.arg-1.5.5/cast_arg/restCall.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.3/cast_arg/stats.py` & `com.castsoftware.uc.arg-1.5.5/cast_arg/stats.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.arg-1.5.4.3/com.castsoftware.uc.arg.egg-info/PKG-INFO` & `com.castsoftware.uc.arg-1.5.5/com.castsoftware.uc.arg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.arg
-Version: 1.5.4.3
+Version: 1.5.5
 Summary: Assessment Report Generator (ARG)
 Home-page: https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `com.castsoftware.uc.arg-1.5.4.3/pyproject.toml` & `com.castsoftware.uc.arg-1.5.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name='com.castsoftware.uc.arg'
 description="Assessment Report Generator (ARG)"
-version='1.5.4.3' #prod version
-dependencies = ['pandas', 'python-pptx==0.6.18', 'com.castsoftware.uc.python.common==0.1.7', 'IPython', 'requests', 'Jinja2']
+version='1.5.5' #prod version
+dependencies = ['pandas', 'python-pptx==0.6.18', 'com.castsoftware.uc.python.common==1.0.7', 'IPython', 'requests', 'Jinja2']
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 requires-python = ">=3.6"
 readme = "README.md"
```

