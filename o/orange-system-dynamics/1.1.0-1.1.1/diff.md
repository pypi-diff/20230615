# Comparing `tmp/orange-system-dynamics-1.1.0.tar.gz` & `tmp/orange-system-dynamics-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orange-system-dynamics-1.1.0.tar", last modified: Wed Jun 14 15:45:46 2023, max compression
+gzip compressed data, was "orange-system-dynamics-1.1.1.tar", last modified: Thu Jun 15 15:45:43 2023, max compression
```

## Comparing `orange-system-dynamics-1.1.0.tar` & `orange-system-dynamics-1.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:45:46.541020 orange-system-dynamics-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6413 2023-06-14 15:45:46.545020 orange-system-dynamics-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5915 2023-06-14 15:38:24.000000 orange-system-dynamics-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:45:46.537020 orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6413 2023-06-14 15:45:46.000000 orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-14 15:45:46.000000 orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 15:45:46.000000 orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-14 15:45:46.000000 orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-14 15:45:46.000000 orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 15:45:46.000000 orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-14 15:45:46.000000 orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-14 15:45:46.000000 orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:45:46.533020 orange-system-dynamics-1.1.0/orangecontrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:45:46.545020 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-14 15:45:46.545020 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:45:46.537020 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     2939 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/DTDL.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7762 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/agent.py
--rw-rw-rw-   0 root         (0) root         (0)     5667 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/azure.py
--rw-rw-rw-   0 root         (0) root         (0)     6425 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/geolocalization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 15:45:46.541020 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/
--rw-rw-rw-   0 root         (0) root         (0)     1031 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/DTDL.svg
--rw-rw-rw-   0 root         (0) root         (0)     1279 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/agent.svg
--rw-rw-rw-   0 root         (0) root         (0)      796 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/azure.svg
--rw-rw-rw-   0 root         (0) root         (0)      457 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/category.svg
--rw-rw-rw-   0 root         (0) root         (0)     1619 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/environment.svg
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/geolocation.svg
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/load_simulation.svg
--rw-rw-rw-   0 root         (0) root         (0)     1626 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/name.svg
--rw-rw-rw-   0 root         (0) root         (0)     6390 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/service.svg
--rw-rw-rw-   0 root         (0) root         (0)     4932 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/statemachine.svg
--rw-rw-rw-   0 root         (0) root         (0)     1909 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/twin.svg
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/load_simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     3822 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/name_table.py
--rw-rw-rw-   0 root         (0) root         (0)    14523 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/service_table.py
--rw-rw-rw-   0 root         (0) root         (0)     7175 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     2315 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/statemachine.py
--rw-rw-rw-   0 root         (0) root         (0)     5147 2023-06-14 15:34:19.000000 orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/twin.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-14 15:23:41.000000 orange-system-dynamics-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1189 2023-06-14 15:45:46.545020 orange-system-dynamics-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:45:43.736523 orange-system-dynamics-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-06-15 15:45:43.736523 orange-system-dynamics-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5915 2023-06-14 15:38:24.000000 orange-system-dynamics-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:45:43.728523 orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6413 2023-06-15 15:45:43.000000 orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-15 15:45:43.000000 orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 15:45:43.000000 orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-15 15:45:43.000000 orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-15 15:45:43.000000 orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 15:45:43.000000 orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      356 2023-06-15 15:45:43.000000 orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-15 15:45:43.000000 orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:45:43.720523 orange-system-dynamics-1.1.1/orangecontrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:45:43.740523 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-15 15:45:43.740523 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:45:43.732523 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/DTDL.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/agent.py
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2023-06-15 15:42:36.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/azure.py
+-rw-rw-rw-   0 root         (0) root         (0)     6425 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/geolocalization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 15:45:43.736523 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     1031 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/DTDL.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/agent.svg
+-rw-rw-rw-   0 root         (0) root         (0)      796 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/azure.svg
+-rw-rw-rw-   0 root         (0) root         (0)      457 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/category.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1619 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/environment.svg
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/geolocation.svg
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/load_simulation.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/name.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6390 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/service.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4932 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/statemachine.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1909 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/twin.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/load_simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3822 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/name_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    14523 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/service_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     7175 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2315 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/statemachine.py
+-rw-rw-rw-   0 root         (0) root         (0)     5147 2023-06-14 15:34:19.000000 orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/twin.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-06-15 15:40:00.000000 orange-system-dynamics-1.1.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1189 2023-06-15 15:45:43.740523 orange-system-dynamics-1.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2023-05-15 09:43:21.000000 orange-system-dynamics-1.1.1/versioneer.py
```

### Comparing `orange-system-dynamics-1.1.0/PKG-INFO` & `orange-system-dynamics-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-system-dynamics
-Version: 1.1.0
+Version: 1.1.1
 Summary: Add-on containing widgets for system dynamics operations
 Home-page: https://gitlab.com/drb-python/samples/odm/sd_addon
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
```

### Comparing `orange-system-dynamics-1.1.0/README.md` & `orange-system-dynamics-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/PKG-INFO` & `orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orange-system-dynamics
-Version: 1.1.0
+Version: 1.1.1
 Summary: Add-on containing widgets for system dynamics operations
 Home-page: https://gitlab.com/drb-python/samples/odm/sd_addon
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: Plugins
```

### Comparing `orange-system-dynamics-1.1.0/orange_system_dynamics.egg-info/SOURCES.txt` & `orange-system-dynamics-1.1.1/orange_system_dynamics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/DTDL.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/DTDL.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/agent.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/agent.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/azure.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
     def create_twin(self):
         twin_id = self.twins_combobox.currentIndex()
         twin = self.twins[twin_id]
         model_id = twin['$metadata']['$model']
         display_name = ''
         for m in self.models:
-            if m['id'] == model_id:
+            if m['Id'] == model_id:
                 model = m
                 display_name = model['display_name'][0]
 
         contents = []
         for k, v in twin.items():
             if k not in ['$dtId', '$etag', '$metadata']:
                 content = {'name': k, 'value': v}
```

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/environment.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/environment.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/geolocalization.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/geolocalization.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/DTDL.svg` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/DTDL.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/agent.svg` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/agent.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/azure.svg` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/azure.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/environment.svg` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/environment.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/name.svg` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/name.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/service.svg` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/service.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/statemachine.svg` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/statemachine.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/icons/twin.svg` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/icons/twin.svg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/load_simulation.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/load_simulation.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/name_table.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/name_table.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/service_table.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/service_table.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/simulation.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/simulation.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/statemachine.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/statemachine.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/orangecontrib/system_dynamics/widgets/twin.py` & `orange-system-dynamics-1.1.1/orangecontrib/system_dynamics/widgets/twin.py`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/setup.cfg` & `orange-system-dynamics-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `orange-system-dynamics-1.1.0/versioneer.py` & `orange-system-dynamics-1.1.1/versioneer.py`

 * *Files identical despite different names*

