# Comparing `tmp/xcoll-0.2.0.tar.gz` & `tmp/xcoll-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcoll-0.2.0.tar", max compression
+gzip compressed data, was "xcoll-0.2.1.tar", max compression
```

## Comparing `xcoll-0.2.0.tar` & `xcoll-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-01-26 20:47:21.412402 xcoll-0.2.0/LICENSE
--rw-r--r--   0        0        0       74 2023-01-26 20:47:21.413402 xcoll-0.2.0/NOTICE
--rw-r--r--   0        0        0     1642 2023-06-13 14:41:55.412931 xcoll-0.2.0/README.md
--rw-r--r--   0        0        0      805 2023-06-13 14:45:56.696082 xcoll-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      392 2023-06-13 14:45:57.324077 xcoll-0.2.0/xcoll/__init__.py
--rw-r--r--   0        0        0      224 2023-06-13 14:41:23.114175 xcoll-0.2.0/xcoll/beam_elements/__init__.py
--rw-r--r--   0        0        0     1248 2023-06-13 14:41:23.114175 xcoll-0.2.0/xcoll/beam_elements/absorber.py
--rw-r--r--   0        0        0    14594 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/base_collimator.py
--rw-r--r--   0        0        0     8598 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/absorber.h
--rw-r--r--   0        0        0      413 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/base_collimator.h
--rw-r--r--   0        0        0     3772 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/everest_collimator.h
--rw-r--r--   0        0        0     4669 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/everest_crystal.h
--rw-r--r--   0        0        0      433 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/collimators_src/invalid_collimator.h
--rw-r--r--   0        0        0     6559 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/beam_elements/everest_collimator.py
--rw-r--r--   0        0        0    39298 2023-06-13 14:41:23.115175 xcoll-0.2.0/xcoll/colldb.py
--rw-r--r--   0        0        0    17015 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/collimator_settings.py
--rw-r--r--   0        0        0       71 2023-04-01 09:07:08.962808 xcoll-0.2.0/xcoll/general.py
--rw-r--r--   0        0        0      639 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/headers/particle_states.h
--rw-r--r--   0        0        0    43926 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/manager.py
--rw-r--r--   0        0        0       84 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/scattering_routines/everest/__init__.py
--rw-r--r--   0        0        0    53426 2023-06-13 14:41:23.116175 xcoll-0.2.0/xcoll/scattering_routines/everest/crystal.h
--rw-r--r--   0        0        0     1059 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/everest.h
--rw-r--r--   0        0        0      970 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/everest.py
--rw-r--r--   0        0        0    12414 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/jaw.h
--rw-r--r--   0        0        0     8742 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/materials.py
--rw-r--r--   0        0        0    10362 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/scatter.h
--rw-r--r--   0        0        0     9368 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/scatter_crystal.h
--rw-r--r--   0        0        0     2863 2023-06-13 14:41:23.117175 xcoll-0.2.0/xcoll/scattering_routines/everest/scatter_init.h
--rw-r--r--   0        0        0     1919 2023-04-01 09:07:08.965808 xcoll-0.2.0/xcoll/tables.py
--rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 xcoll-0.2.0/setup.py
--rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 xcoll-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-26 20:47:21.412402 xcoll-0.2.1/LICENSE
+-rw-r--r--   0        0        0       74 2023-01-26 20:47:21.413402 xcoll-0.2.1/NOTICE
+-rw-r--r--   0        0        0     1642 2023-06-13 14:41:55.412931 xcoll-0.2.1/README.md
+-rw-r--r--   0        0        0      805 2023-06-15 07:45:09.198845 xcoll-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      392 2023-06-15 07:45:09.199844 xcoll-0.2.1/xcoll/__init__.py
+-rw-r--r--   0        0        0      224 2023-06-13 14:41:23.114175 xcoll-0.2.1/xcoll/beam_elements/__init__.py
+-rw-r--r--   0        0        0     1248 2023-06-13 14:41:23.114175 xcoll-0.2.1/xcoll/beam_elements/absorber.py
+-rw-r--r--   0        0        0    14594 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/base_collimator.py
+-rw-r--r--   0        0        0     8598 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/absorber.h
+-rw-r--r--   0        0        0      413 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/base_collimator.h
+-rw-r--r--   0        0        0     3772 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/everest_collimator.h
+-rw-r--r--   0        0        0     4669 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/everest_crystal.h
+-rw-r--r--   0        0        0      433 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/invalid_collimator.h
+-rw-r--r--   0        0        0     6559 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/everest_collimator.py
+-rw-r--r--   0        0        0    39298 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/colldb.py
+-rw-r--r--   0        0        0    17015 2023-06-13 14:41:23.116175 xcoll-0.2.1/xcoll/collimator_settings.py
+-rw-r--r--   0        0        0       71 2023-04-01 09:07:08.962808 xcoll-0.2.1/xcoll/general.py
+-rw-r--r--   0        0        0      639 2023-06-13 14:41:23.116175 xcoll-0.2.1/xcoll/headers/particle_states.h
+-rw-r--r--   0        0        0    43926 2023-06-13 14:41:23.116175 xcoll-0.2.1/xcoll/manager.py
+-rw-r--r--   0        0        0       84 2023-06-15 07:13:43.384589 xcoll-0.2.1/xcoll/scattering_routines/everest/__init__.py
+-rw-r--r--   0        0        0    53426 2023-06-13 14:41:23.116175 xcoll-0.2.1/xcoll/scattering_routines/everest/crystal.h
+-rw-r--r--   0        0        0     1059 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/everest.h
+-rw-r--r--   0        0        0      970 2023-06-15 07:13:43.384589 xcoll-0.2.1/xcoll/scattering_routines/everest/everest.py
+-rw-r--r--   0        0        0    12414 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/jaw.h
+-rw-r--r--   0        0        0     8742 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/materials.py
+-rw-r--r--   0        0        0    10362 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/scatter.h
+-rw-r--r--   0        0        0     9368 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/scatter_crystal.h
+-rw-r--r--   0        0        0     2863 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/scatter_init.h
+-rw-r--r--   0        0        0     1919 2023-04-01 09:07:08.965808 xcoll-0.2.1/xcoll/tables.py
+-rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 xcoll-0.2.1/setup.py
+-rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 xcoll-0.2.1/PKG-INFO
```

### Comparing `xcoll-0.2.0/LICENSE` & `xcoll-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/README.md` & `xcoll-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/pyproject.toml` & `xcoll-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcoll"
-version = "0.2.0"
+version = "0.2.1"
 description = "Xsuite collimation package"
 homepage = "https://github.com/xsuite/xcoll"
 repository = "https://github.com/xsuite/xcoll"
 authors = [
            "Frederik F. Van der Veken <frederik@cern.ch>",
            "Despina Demetriadou <despina.demetriadou@cern.ch>",
            "Andrey Abramov <andrey.abramov@cern.ch>",
```

### Comparing `xcoll-0.2.0/xcoll/beam_elements/absorber.py` & `xcoll-0.2.1/xcoll/beam_elements/absorber.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/beam_elements/base_collimator.py` & `xcoll-0.2.1/xcoll/beam_elements/base_collimator.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/beam_elements/collimators_src/absorber.h` & `xcoll-0.2.1/xcoll/beam_elements/collimators_src/absorber.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/beam_elements/collimators_src/everest_collimator.h` & `xcoll-0.2.1/xcoll/beam_elements/collimators_src/everest_collimator.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/beam_elements/collimators_src/everest_crystal.h` & `xcoll-0.2.1/xcoll/beam_elements/collimators_src/everest_crystal.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/beam_elements/everest_collimator.py` & `xcoll-0.2.1/xcoll/beam_elements/everest_collimator.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/colldb.py` & `xcoll-0.2.1/xcoll/colldb.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/collimator_settings.py` & `xcoll-0.2.1/xcoll/collimator_settings.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/headers/particle_states.h` & `xcoll-0.2.1/xcoll/headers/particle_states.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/manager.py` & `xcoll-0.2.1/xcoll/manager.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/scattering_routines/everest/crystal.h` & `xcoll-0.2.1/xcoll/scattering_routines/everest/crystal.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/scattering_routines/everest/everest.h` & `xcoll-0.2.1/xcoll/scattering_routines/everest/everest.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/scattering_routines/everest/everest.py` & `xcoll-0.2.1/xcoll/scattering_routines/everest/everest.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/scattering_routines/everest/jaw.h` & `xcoll-0.2.1/xcoll/scattering_routines/everest/jaw.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/scattering_routines/everest/materials.py` & `xcoll-0.2.1/xcoll/scattering_routines/everest/materials.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/scattering_routines/everest/scatter.h` & `xcoll-0.2.1/xcoll/scattering_routines/everest/scatter.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/scattering_routines/everest/scatter_crystal.h` & `xcoll-0.2.1/xcoll/scattering_routines/everest/scatter_crystal.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/scattering_routines/everest/scatter_init.h` & `xcoll-0.2.1/xcoll/scattering_routines/everest/scatter_init.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/xcoll/tables.py` & `xcoll-0.2.1/xcoll/tables.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.0/setup.py` & `xcoll-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 package_data = \
 {'': ['*'],
  'xcoll': ['headers/*'],
  'xcoll.beam_elements': ['collimators_src/*']}
 
 setup_kwargs = {
     'name': 'xcoll',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Xsuite collimation package',
     'long_description': '# xcoll\n\n<!---![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xcoll?logo=PyPI?style=plastic) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/xcoll?logo=PyPI?style=plastic)-->\n\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/xsuite/xcoll?style=plastic) ![GitHub](https://img.shields.io/github/license/xsuite/xcoll?style=plastic) ![GitHub all releases](https://img.shields.io/github/downloads/xsuite/xcoll/total?logo=GitHub&style=plastic) ![GitHub issues](https://img.shields.io/github/issues/xsuite/xcoll?logo=GitHub&style=plastic) ![GitHub pull requests](https://img.shields.io/github/issues-pr/xsuite/xcoll?logo=GitHub&style=plastic) ![GitHub repo size](https://img.shields.io/github/repo-size/xsuite/xcoll?logo=GitHub&style=plastic)\n\nCollimation in xtrack simulations\n\n## Description\n\n## Getting Started\n\n### Dependencies\n\n* python >= 3.8\n    * numpy\n    * pandas\n    * xsuite (in particular xobjects, xdeps, xtrack, xpart)\n\n### Installing\n`xcoll` is packaged using `poetry`, and can be easily installed with `pip`:\n```bash\npip install xcoll\n```\nFor a local installation, clone and install in editable mode (need to have `pip` >22):\n```bash\ngit clone git@github.com:xsuite/xcoll.git\npip install -e xcoll\n```\n\n### Example\n\n## Features\n\n## Authors\n\n* [Frederik Van der Veken](https://github.com/freddieknets) (frederik@cern.ch)\n* [Despina Demetriadou](https://github.com/ddemetriadou)\n* [Andrey Abramov](https://github.com/anabramo)\n* [Giovanni Iadarola](https://github.com/giadarol)\n\n\n## Version History\n\n* 0.1\n    * Initial Release\n\n## License\n\nThis project is [Apache 2.0 licensed](./LICENSE).\n',
     'author': 'Frederik F. Van der Veken',
     'author_email': 'frederik@cern.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/xsuite/xcoll',
```

### Comparing `xcoll-0.2.0/PKG-INFO` & `xcoll-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcoll
-Version: 0.2.0
+Version: 0.2.1
 Summary: Xsuite collimation package
 Home-page: https://github.com/xsuite/xcoll
 License: Apache 2.0
 Author: Frederik F. Van der Veken
 Author-email: frederik@cern.ch
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
```

