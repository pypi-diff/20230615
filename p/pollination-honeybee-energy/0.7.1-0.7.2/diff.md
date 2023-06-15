# Comparing `tmp/pollination-honeybee-energy-0.7.1.tar.gz` & `tmp/pollination-honeybee-energy-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-honeybee-energy-0.7.1.tar", last modified: Sat Feb 11 21:34:22 2023, max compression
+gzip compressed data, was "dist/pollination-honeybee-energy-0.7.2.tar", last modified: Thu Jun 15 17:21:19 2023, max compression
```

## Comparing `pollination-honeybee-energy-0.7.1.tar` & `pollination-honeybee-energy-0.7.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/pollination_honeybee_energy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/pollination_honeybee_energy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/pollination_honeybee_energy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/pollination_honeybee_energy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 21:33:46.000000 pollination-honeybee-energy-0.7.1/pollination_honeybee_energy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/pollination_honeybee_energy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/pollination_honeybee_energy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 21:34:22.000000 pollination-honeybee-energy-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/tests/baseline_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/tests/result_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/tests/settings_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/tests/simulate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-11 21:33:21.000000 pollination-honeybee-energy-0.7.1/tests/translate_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/pollination_honeybee_energy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/pollination_honeybee_energy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/pollination_honeybee_energy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/pollination_honeybee_energy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:20:40.000000 pollination-honeybee-energy-0.7.2/pollination_honeybee_energy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/pollination_honeybee_energy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/pollination_honeybee_energy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:21:19.000000 pollination-honeybee-energy-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/tests/baseline_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/tests/result_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/tests/settings_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/tests/simulate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-15 17:20:16.000000 pollination-honeybee-energy-0.7.2/tests/translate_test.py
```

### Comparing `pollination-honeybee-energy-0.7.1/.github/workflows/ci.yaml` & `pollination-honeybee-energy-0.7.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/.github/workflows/dependency-release.yaml` & `pollination-honeybee-energy-0.7.2/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/LICENSE` & `pollination-honeybee-energy-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/PKG-INFO` & `pollination-honeybee-energy-0.7.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-energy
-Version: 0.7.1
+Version: 0.7.2
 Summary: Honeybee energy plugin for Pollination.
 Home-page: https://github.com/pollination/honeybee-energy
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_bugs/grasshopper_tabs/HB-Energy.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-energy
-Description: # Pollination Honeybee Energy plugin
-        
-        A plugin adds energy simulation functions to Pollination.
-        
-        ## Sources
-        
-        The following packages and engines are included with this plugin:
-        
-        - `honeybee-energy` Python package. [PyPI](https://pypi.org/project/honeybee-energy/), [source](https://github.com/ladybug-tools/honeybee-energy)
-        - `honeybee-energy-standards` Python package. [PyPI](https://pypi.org/project/honeybee-energy-standards/), [source](https://github.com/ladybug-tools/honeybee-energy-standards)
-        - `honeybee-openstudio-gem` Ruby gem. [Rubygems](https://rubygems.org/gems/honeybee-openstudio), [source](https://github.com/ladybug-tools/honeybee-openstudio-gem)
-        - `Ironbug` Ironbug. [source](https://github.com/MingboPeng/Ironbug), including OpenStudio .NET bindings
-        - `OpenStudio` [source](https://github.com/NREL/OpenStudio/releases), including OpenStudio CLI
-        - `EnergyPlus` [source](https://github.com/NREL/EnergyPlus/releases)
-        
 Keywords: honeybee,energy,ladybug-tools
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Pollination Honeybee Energy plugin
+
+A plugin adds energy simulation functions to Pollination.
+
+## Sources
+
+The following packages and engines are included with this plugin:
+
+- `honeybee-energy` Python package. [PyPI](https://pypi.org/project/honeybee-energy/), [source](https://github.com/ladybug-tools/honeybee-energy)
+- `honeybee-energy-standards` Python package. [PyPI](https://pypi.org/project/honeybee-energy-standards/), [source](https://github.com/ladybug-tools/honeybee-energy-standards)
+- `honeybee-openstudio-gem` Ruby gem. [Rubygems](https://rubygems.org/gems/honeybee-openstudio), [source](https://github.com/ladybug-tools/honeybee-openstudio-gem)
+- `Ironbug` Ironbug. [source](https://github.com/MingboPeng/Ironbug), including OpenStudio .NET bindings
+- `OpenStudio` [source](https://github.com/NREL/OpenStudio/releases), including OpenStudio CLI
+- `EnergyPlus` [source](https://github.com/NREL/EnergyPlus/releases)
```

### Comparing `pollination-honeybee-energy-0.7.1/README.md` & `pollination-honeybee-energy-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/baseline.py` & `pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/baseline.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/result.py` & `pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/result.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/settings.py` & `pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/settings.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/simulate.py` & `pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/simulate.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/pollination/honeybee_energy/translate.py` & `pollination-honeybee-energy-0.7.2/pollination/honeybee_energy/translate.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/pollination_honeybee_energy.egg-info/PKG-INFO` & `pollination-honeybee-energy-0.7.2/pollination_honeybee_energy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pollination-honeybee-energy
-Version: 0.7.1
+Version: 0.7.2
 Summary: Honeybee energy plugin for Pollination.
 Home-page: https://github.com/pollination/honeybee-energy
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: chris, ladybug-tools
 Maintainer-email: chris@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
 Project-URL: icon, https://raw.githubusercontent.com/ladybug-tools/artwork/master/icons_bugs/grasshopper_tabs/HB-Energy.png
 Project-URL: docker, https://hub.docker.com/r/ladybugtools/honeybee-energy
-Description: # Pollination Honeybee Energy plugin
-        
-        A plugin adds energy simulation functions to Pollination.
-        
-        ## Sources
-        
-        The following packages and engines are included with this plugin:
-        
-        - `honeybee-energy` Python package. [PyPI](https://pypi.org/project/honeybee-energy/), [source](https://github.com/ladybug-tools/honeybee-energy)
-        - `honeybee-energy-standards` Python package. [PyPI](https://pypi.org/project/honeybee-energy-standards/), [source](https://github.com/ladybug-tools/honeybee-energy-standards)
-        - `honeybee-openstudio-gem` Ruby gem. [Rubygems](https://rubygems.org/gems/honeybee-openstudio), [source](https://github.com/ladybug-tools/honeybee-openstudio-gem)
-        - `Ironbug` Ironbug. [source](https://github.com/MingboPeng/Ironbug), including OpenStudio .NET bindings
-        - `OpenStudio` [source](https://github.com/NREL/OpenStudio/releases), including OpenStudio CLI
-        - `EnergyPlus` [source](https://github.com/NREL/EnergyPlus/releases)
-        
 Keywords: honeybee,energy,ladybug-tools
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Pollination Honeybee Energy plugin
+
+A plugin adds energy simulation functions to Pollination.
+
+## Sources
+
+The following packages and engines are included with this plugin:
+
+- `honeybee-energy` Python package. [PyPI](https://pypi.org/project/honeybee-energy/), [source](https://github.com/ladybug-tools/honeybee-energy)
+- `honeybee-energy-standards` Python package. [PyPI](https://pypi.org/project/honeybee-energy-standards/), [source](https://github.com/ladybug-tools/honeybee-energy-standards)
+- `honeybee-openstudio-gem` Ruby gem. [Rubygems](https://rubygems.org/gems/honeybee-openstudio), [source](https://github.com/ladybug-tools/honeybee-openstudio-gem)
+- `Ironbug` Ironbug. [source](https://github.com/MingboPeng/Ironbug), including OpenStudio .NET bindings
+- `OpenStudio` [source](https://github.com/NREL/OpenStudio/releases), including OpenStudio CLI
+- `EnergyPlus` [source](https://github.com/NREL/EnergyPlus/releases)
```

### Comparing `pollination-honeybee-energy-0.7.1/pollination_honeybee_energy.egg-info/SOURCES.txt` & `pollination-honeybee-energy-0.7.2/pollination_honeybee_energy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/setup.py` & `pollination-honeybee-energy-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/tests/baseline_test.py` & `pollination-honeybee-energy-0.7.2/tests/baseline_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/tests/result_test.py` & `pollination-honeybee-energy-0.7.2/tests/result_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/tests/settings_test.py` & `pollination-honeybee-energy-0.7.2/tests/settings_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/tests/simulate_test.py` & `pollination-honeybee-energy-0.7.2/tests/simulate_test.py`

 * *Files identical despite different names*

### Comparing `pollination-honeybee-energy-0.7.1/tests/translate_test.py` & `pollination-honeybee-energy-0.7.2/tests/translate_test.py`

 * *Files identical despite different names*

