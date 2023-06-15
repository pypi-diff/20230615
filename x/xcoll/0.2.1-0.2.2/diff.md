# Comparing `tmp/xcoll-0.2.1.tar.gz` & `tmp/xcoll-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcoll-0.2.1.tar", max compression
+gzip compressed data, was "xcoll-0.2.2.tar", max compression
```

## Comparing `xcoll-0.2.1.tar` & `xcoll-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    11357 2023-01-26 20:47:21.412402 xcoll-0.2.1/LICENSE
--rw-r--r--   0        0        0       74 2023-01-26 20:47:21.413402 xcoll-0.2.1/NOTICE
--rw-r--r--   0        0        0     1642 2023-06-13 14:41:55.412931 xcoll-0.2.1/README.md
--rw-r--r--   0        0        0      805 2023-06-15 07:45:09.198845 xcoll-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      392 2023-06-15 07:45:09.199844 xcoll-0.2.1/xcoll/__init__.py
--rw-r--r--   0        0        0      224 2023-06-13 14:41:23.114175 xcoll-0.2.1/xcoll/beam_elements/__init__.py
--rw-r--r--   0        0        0     1248 2023-06-13 14:41:23.114175 xcoll-0.2.1/xcoll/beam_elements/absorber.py
--rw-r--r--   0        0        0    14594 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/base_collimator.py
--rw-r--r--   0        0        0     8598 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/absorber.h
--rw-r--r--   0        0        0      413 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/base_collimator.h
--rw-r--r--   0        0        0     3772 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/everest_collimator.h
--rw-r--r--   0        0        0     4669 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/everest_crystal.h
--rw-r--r--   0        0        0      433 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/collimators_src/invalid_collimator.h
--rw-r--r--   0        0        0     6559 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/beam_elements/everest_collimator.py
--rw-r--r--   0        0        0    39298 2023-06-13 14:41:23.115175 xcoll-0.2.1/xcoll/colldb.py
--rw-r--r--   0        0        0    17015 2023-06-13 14:41:23.116175 xcoll-0.2.1/xcoll/collimator_settings.py
--rw-r--r--   0        0        0       71 2023-04-01 09:07:08.962808 xcoll-0.2.1/xcoll/general.py
--rw-r--r--   0        0        0      639 2023-06-13 14:41:23.116175 xcoll-0.2.1/xcoll/headers/particle_states.h
--rw-r--r--   0        0        0    43926 2023-06-13 14:41:23.116175 xcoll-0.2.1/xcoll/manager.py
--rw-r--r--   0        0        0       84 2023-06-15 07:13:43.384589 xcoll-0.2.1/xcoll/scattering_routines/everest/__init__.py
--rw-r--r--   0        0        0    53426 2023-06-13 14:41:23.116175 xcoll-0.2.1/xcoll/scattering_routines/everest/crystal.h
--rw-r--r--   0        0        0     1059 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/everest.h
--rw-r--r--   0        0        0      970 2023-06-15 07:13:43.384589 xcoll-0.2.1/xcoll/scattering_routines/everest/everest.py
--rw-r--r--   0        0        0    12414 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/jaw.h
--rw-r--r--   0        0        0     8742 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/materials.py
--rw-r--r--   0        0        0    10362 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/scatter.h
--rw-r--r--   0        0        0     9368 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/scatter_crystal.h
--rw-r--r--   0        0        0     2863 2023-06-13 14:41:23.117175 xcoll-0.2.1/xcoll/scattering_routines/everest/scatter_init.h
--rw-r--r--   0        0        0     1919 2023-04-01 09:07:08.965808 xcoll-0.2.1/xcoll/tables.py
--rw-r--r--   0        0        0     2376 1970-01-01 00:00:00.000000 xcoll-0.2.1/setup.py
--rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 xcoll-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-26 20:47:21.412402 xcoll-0.2.2/LICENSE
+-rw-r--r--   0        0        0       74 2023-01-26 20:47:21.413402 xcoll-0.2.2/NOTICE
+-rw-r--r--   0        0        0     1713 2023-06-15 15:54:59.927458 xcoll-0.2.2/README.md
+-rw-r--r--   0        0        0     1008 2023-06-15 15:54:59.927458 xcoll-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      392 2023-06-15 15:54:59.928458 xcoll-0.2.2/xcoll/__init__.py
+-rw-r--r--   0        0        0      224 2023-06-13 14:41:23.114175 xcoll-0.2.2/xcoll/beam_elements/__init__.py
+-rw-r--r--   0        0        0     1248 2023-06-13 14:41:23.114175 xcoll-0.2.2/xcoll/beam_elements/absorber.py
+-rw-r--r--   0        0        0    14594 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/beam_elements/base_collimator.py
+-rw-r--r--   0        0        0     8600 2023-06-15 15:54:59.928458 xcoll-0.2.2/xcoll/beam_elements/collimators_src/absorber.h
+-rw-r--r--   0        0        0      413 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/beam_elements/collimators_src/base_collimator.h
+-rw-r--r--   0        0        0     3774 2023-06-15 15:54:59.928458 xcoll-0.2.2/xcoll/beam_elements/collimators_src/everest_collimator.h
+-rw-r--r--   0        0        0     4672 2023-06-15 15:54:59.928458 xcoll-0.2.2/xcoll/beam_elements/collimators_src/everest_crystal.h
+-rw-r--r--   0        0        0      433 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/beam_elements/collimators_src/invalid_collimator.h
+-rw-r--r--   0        0        0     6559 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/beam_elements/everest_collimator.py
+-rw-r--r--   0        0        0    39298 2023-06-13 14:41:23.115175 xcoll-0.2.2/xcoll/colldb.py
+-rw-r--r--   0        0        0    17015 2023-06-13 14:41:23.116175 xcoll-0.2.2/xcoll/collimator_settings.py
+-rw-r--r--   0        0        0       71 2023-04-01 09:07:08.962808 xcoll-0.2.2/xcoll/general.py
+-rw-r--r--   0        0        0      639 2023-06-13 14:41:23.116175 xcoll-0.2.2/xcoll/headers/particle_states.h
+-rw-r--r--   0        0        0    43926 2023-06-13 14:41:23.116175 xcoll-0.2.2/xcoll/manager.py
+-rw-r--r--   0        0        0       84 2023-06-15 14:24:13.343504 xcoll-0.2.2/xcoll/scattering_routines/everest/__init__.py
+-rw-r--r--   0        0        0    53426 2023-06-13 14:41:23.116175 xcoll-0.2.2/xcoll/scattering_routines/everest/crystal.h
+-rw-r--r--   0        0        0     1059 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/everest.h
+-rw-r--r--   0        0        0      970 2023-06-15 14:24:13.343504 xcoll-0.2.2/xcoll/scattering_routines/everest/everest.py
+-rw-r--r--   0        0        0    12414 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/jaw.h
+-rw-r--r--   0        0        0     8742 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/materials.py
+-rw-r--r--   0        0        0    10362 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/scatter.h
+-rw-r--r--   0        0        0     9368 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/scatter_crystal.h
+-rw-r--r--   0        0        0     2863 2023-06-13 14:41:23.117175 xcoll-0.2.2/xcoll/scattering_routines/everest/scatter_init.h
+-rw-r--r--   0        0        0     1919 2023-04-01 09:07:08.965808 xcoll-0.2.2/xcoll/tables.py
+-rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 xcoll-0.2.2/setup.py
+-rw-r--r--   0        0        0     2733 1970-01-01 00:00:00.000000 xcoll-0.2.2/PKG-INFO
```

### Comparing `xcoll-0.2.1/LICENSE` & `xcoll-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/README.md` & `xcoll-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # xcoll
 
 <!---![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xcoll?logo=PyPI?style=plastic) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/xcoll?logo=PyPI?style=plastic)-->
 
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/xsuite/xcoll?style=plastic) ![GitHub](https://img.shields.io/github/license/xsuite/xcoll?style=plastic) ![GitHub all releases](https://img.shields.io/github/downloads/xsuite/xcoll/total?logo=GitHub&style=plastic) ![GitHub issues](https://img.shields.io/github/issues/xsuite/xcoll?logo=GitHub&style=plastic) ![GitHub pull requests](https://img.shields.io/github/issues-pr/xsuite/xcoll?logo=GitHub&style=plastic) ![GitHub repo size](https://img.shields.io/github/repo-size/xsuite/xcoll?logo=GitHub&style=plastic)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/xsuite/xcoll?style=plastic)
+![GitHub](https://img.shields.io/github/license/xsuite/xcoll?style=plastic)
+![PyPi](https://img.shields.io/pypi/dm/xcoll?logo=PyPI&style=plastic)
+![GitHub all releases](https://img.shields.io/github/downloads/xsuite/xcoll/total?logo=GitHub&style=plastic)
+
+![GitHub pull requests](https://img.shields.io/github/issues-pr/xsuite/xcoll?logo=GitHub&style=plastic)
+![GitHub issues](https://img.shields.io/github/issues/xsuite/xcoll?logo=GitHub&style=plastic)
+![GitHub repo size](https://img.shields.io/github/repo-size/xsuite/xcoll?logo=GitHub&style=plastic)
 
 Collimation in xtrack simulations
 
 ## Description
 
 ## Getting Started
```

### Comparing `xcoll-0.2.1/pyproject.toml` & `xcoll-0.2.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcoll"
-version = "0.2.1"
+version = "0.2.2"
 description = "Xsuite collimation package"
 homepage = "https://github.com/xsuite/xcoll"
 repository = "https://github.com/xsuite/xcoll"
 authors = [
            "Frederik F. Van der Veken <frederik@cern.ch>",
            "Despina Demetriadou <despina.demetriadou@cern.ch>",
            "Andrey Abramov <andrey.abramov@cern.ch>",
@@ -13,22 +13,27 @@
 readme = "README.md"
 license = "Apache 2.0"
 include = [ "LICENSE", "NOTICE" ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-#numpy
-#pandas
-#scipy
-#xobjects
-#xdeps
-#xpart
-#xtrack
+ruamel-yaml = { version = "^0.17.31", optional = true }
+numpy = ">=1.0"
+pandas = ">=1.4"
+xobjects = "^0.2.6"
+xdeps = "^0.1.1"
+xpart = "^0.15.0"
+xtrack = "^0.36.5"
+xfields = "^0.12.1"
+xcoll = "^0.2.1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = ">=7.3"
+
+[tool.poetry.extras]
+tests = ["pytest", "ruamel-yaml"]
 
 [build-system]
 # Needed for pip install -e (BTW: need pip version 22)
 requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `xcoll-0.2.1/xcoll/beam_elements/absorber.py` & `xcoll-0.2.2/xcoll/beam_elements/absorber.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/beam_elements/base_collimator.py` & `xcoll-0.2.2/xcoll/beam_elements/base_collimator.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/beam_elements/collimators_src/absorber.h` & `xcoll-0.2.2/xcoll/beam_elements/collimators_src/absorber.h`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     double const jaw_RD = jaw_R + sin_yR*active_length/2.;
     // TODO: need shortening of active length!
     // Collimator reference frame
     double const sin_zL = BlackAbsorberData_get_sin_zL(el);
     double const cos_zL = BlackAbsorberData_get_cos_zL(el);
     double const sin_zR = BlackAbsorberData_get_sin_zR(el);
     double const cos_zR = BlackAbsorberData_get_cos_zR(el);
-    if (abs(sin_zL-sin_zR) > 1.e-10 || abs(cos_zL-cos_zR) > 1.e-10 ){
+    if (fabs(sin_zL-sin_zR) > 1.e-10 || fabs(cos_zL-cos_zR) > 1.e-10 ){
         kill_all_particles(part0, XC_ERR_NOT_IMPLEMENTED);
     };
     double const dx = BlackAbsorberData_get_ref_x(el);
     double const dy = BlackAbsorberData_get_ref_y(el);
     // Impact table
     CollimatorImpactsData record = BlackAbsorberData_getp_internal_record(el, part0);
     RecordIndex record_index = NULL;
```

### Comparing `xcoll-0.2.1/xcoll/beam_elements/collimators_src/everest_collimator.h` & `xcoll-0.2.2/xcoll/beam_elements/collimators_src/everest_collimator.h`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     double const co_y       = EverestCollimatorData_get_ref_y(el);
     // TODO: use xtrack C-code for rotation element
     // TODO: we are ignoring the angle of the right jaw
     double const sin_zL     = EverestCollimatorData_get_sin_zL(el);
     double const cos_zL     = EverestCollimatorData_get_cos_zL(el);
     double const sin_zR     = EverestCollimatorData_get_sin_zR(el);
     double const cos_zR     = EverestCollimatorData_get_cos_zR(el);
-    if (abs(sin_zL-sin_zR) > 1.e-10 || abs(cos_zL-cos_zR) > 1.e-10 ){
+    if (fabs(sin_zL-sin_zR) > 1.e-10 || fabs(cos_zL-cos_zR) > 1.e-10 ){
         kill_all_particles(part0, XC_ERR_NOT_IMPLEMENTED);
     };
     double const c_aperture = EverestCollimatorData_get_jaw_L(el) - EverestCollimatorData_get_jaw_R(el);
     double const c_offset   = ( EverestCollimatorData_get_jaw_L(el) + EverestCollimatorData_get_jaw_R(el) ) /2;
     double const c_tilt0    = asin(EverestCollimatorData_get_sin_yL(el));
     double const c_tilt1    = asin(EverestCollimatorData_get_sin_yR(el));
     int    const side       = EverestCollimatorData_get__side(el);
```

### Comparing `xcoll-0.2.1/xcoll/beam_elements/collimators_src/everest_crystal.h` & `xcoll-0.2.2/xcoll/beam_elements/collimators_src/everest_crystal.h`

 * *Files 0% similar despite different names*

```diff
@@ -28,22 +28,22 @@
     // TODO: use xtrack C-code for rotation element
     // TODO: we are ignoring the angle of the right jaw
     // TODO: is a crystal always one-sided...?
     double const sin_zL     = EverestCrystalData_get_sin_zL(el);
     double const cos_zL     = EverestCrystalData_get_cos_zL(el);
     double const sin_zR     = EverestCrystalData_get_sin_zR(el);
     double const cos_zR     = EverestCrystalData_get_cos_zR(el);
-    if (abs(sin_zL-sin_zR) > 1.e-10 || abs(cos_zL-cos_zR) > 1.e-10 ){
+    if (fabs(sin_zL-sin_zR) > 1.e-10 || fabs(cos_zL-cos_zR) > 1.e-10 ){
         kill_all_particles(part0, XC_ERR_NOT_IMPLEMENTED);
     };
     double const c_aperture = EverestCrystalData_get_jaw_L(el) - EverestCrystalData_get_jaw_R(el);
     double const c_offset   = ( EverestCrystalData_get_jaw_L(el) + EverestCrystalData_get_jaw_R(el) ) /2;
     double const c_tilt0    = asin(EverestCrystalData_get_sin_yL(el));
     double const c_tilt1    = asin(EverestCrystalData_get_sin_yR(el));
-    if (abs(c_tilt1) > 1.e-10){
+    if (fabs(c_tilt1) > 1.e-10){
         kill_all_particles(part0, XC_ERR_INVALID_XOFIELD);
     };
     int    const side       = EverestCrystalData_get__side(el);
     double const bend       = EverestCrystalData_get_bend(el);
     // TODO: cry_tilt should be given by jaw positions...?
     double const cry_tilt   = EverestCrystalData_get_align_angle(el) + c_tilt0;
     double const bend_ang   = length/bend;    // temporary value
```

### Comparing `xcoll-0.2.1/xcoll/beam_elements/everest_collimator.py` & `xcoll-0.2.2/xcoll/beam_elements/everest_collimator.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/colldb.py` & `xcoll-0.2.2/xcoll/colldb.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/collimator_settings.py` & `xcoll-0.2.2/xcoll/collimator_settings.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/headers/particle_states.h` & `xcoll-0.2.2/xcoll/headers/particle_states.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/manager.py` & `xcoll-0.2.2/xcoll/manager.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/scattering_routines/everest/crystal.h` & `xcoll-0.2.2/xcoll/scattering_routines/everest/crystal.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/scattering_routines/everest/everest.h` & `xcoll-0.2.2/xcoll/scattering_routines/everest/everest.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/scattering_routines/everest/everest.py` & `xcoll-0.2.2/xcoll/scattering_routines/everest/everest.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/scattering_routines/everest/jaw.h` & `xcoll-0.2.2/xcoll/scattering_routines/everest/jaw.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/scattering_routines/everest/materials.py` & `xcoll-0.2.2/xcoll/scattering_routines/everest/materials.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/scattering_routines/everest/scatter.h` & `xcoll-0.2.2/xcoll/scattering_routines/everest/scatter.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/scattering_routines/everest/scatter_crystal.h` & `xcoll-0.2.2/xcoll/scattering_routines/everest/scatter_crystal.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/scattering_routines/everest/scatter_init.h` & `xcoll-0.2.2/xcoll/scattering_routines/everest/scatter_init.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/xcoll/tables.py` & `xcoll-0.2.2/xcoll/tables.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.2.1/setup.py` & `xcoll-0.2.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,24 +5,39 @@
 ['xcoll', 'xcoll.beam_elements', 'xcoll.scattering_routines.everest']
 
 package_data = \
 {'': ['*'],
  'xcoll': ['headers/*'],
  'xcoll.beam_elements': ['collimators_src/*']}
 
+install_requires = \
+['numpy>=1.0',
+ 'pandas>=1.4',
+ 'xcoll>=0.2.1,<0.3.0',
+ 'xdeps>=0.1.1,<0.2.0',
+ 'xfields>=0.12.1,<0.13.0',
+ 'xobjects>=0.2.6,<0.3.0',
+ 'xpart>=0.15.0,<0.16.0',
+ 'xtrack>=0.36.5,<0.37.0']
+
+extras_require = \
+{'tests': ['ruamel-yaml>=0.17.31,<0.18.0']}
+
 setup_kwargs = {
     'name': 'xcoll',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Xsuite collimation package',
-    'long_description': '# xcoll\n\n<!---![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xcoll?logo=PyPI?style=plastic) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/xcoll?logo=PyPI?style=plastic)-->\n\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/xsuite/xcoll?style=plastic) ![GitHub](https://img.shields.io/github/license/xsuite/xcoll?style=plastic) ![GitHub all releases](https://img.shields.io/github/downloads/xsuite/xcoll/total?logo=GitHub&style=plastic) ![GitHub issues](https://img.shields.io/github/issues/xsuite/xcoll?logo=GitHub&style=plastic) ![GitHub pull requests](https://img.shields.io/github/issues-pr/xsuite/xcoll?logo=GitHub&style=plastic) ![GitHub repo size](https://img.shields.io/github/repo-size/xsuite/xcoll?logo=GitHub&style=plastic)\n\nCollimation in xtrack simulations\n\n## Description\n\n## Getting Started\n\n### Dependencies\n\n* python >= 3.8\n    * numpy\n    * pandas\n    * xsuite (in particular xobjects, xdeps, xtrack, xpart)\n\n### Installing\n`xcoll` is packaged using `poetry`, and can be easily installed with `pip`:\n```bash\npip install xcoll\n```\nFor a local installation, clone and install in editable mode (need to have `pip` >22):\n```bash\ngit clone git@github.com:xsuite/xcoll.git\npip install -e xcoll\n```\n\n### Example\n\n## Features\n\n## Authors\n\n* [Frederik Van der Veken](https://github.com/freddieknets) (frederik@cern.ch)\n* [Despina Demetriadou](https://github.com/ddemetriadou)\n* [Andrey Abramov](https://github.com/anabramo)\n* [Giovanni Iadarola](https://github.com/giadarol)\n\n\n## Version History\n\n* 0.1\n    * Initial Release\n\n## License\n\nThis project is [Apache 2.0 licensed](./LICENSE).\n',
+    'long_description': '# xcoll\n\n<!---![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xcoll?logo=PyPI?style=plastic) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/xcoll?logo=PyPI?style=plastic)-->\n\n![GitHub release (latest by date)](https://img.shields.io/github/v/release/xsuite/xcoll?style=plastic)\n![GitHub](https://img.shields.io/github/license/xsuite/xcoll?style=plastic)\n![PyPi](https://img.shields.io/pypi/dm/xcoll?logo=PyPI&style=plastic)\n![GitHub all releases](https://img.shields.io/github/downloads/xsuite/xcoll/total?logo=GitHub&style=plastic)\n\n![GitHub pull requests](https://img.shields.io/github/issues-pr/xsuite/xcoll?logo=GitHub&style=plastic)\n![GitHub issues](https://img.shields.io/github/issues/xsuite/xcoll?logo=GitHub&style=plastic)\n![GitHub repo size](https://img.shields.io/github/repo-size/xsuite/xcoll?logo=GitHub&style=plastic)\n\nCollimation in xtrack simulations\n\n## Description\n\n## Getting Started\n\n### Dependencies\n\n* python >= 3.8\n    * numpy\n    * pandas\n    * xsuite (in particular xobjects, xdeps, xtrack, xpart)\n\n### Installing\n`xcoll` is packaged using `poetry`, and can be easily installed with `pip`:\n```bash\npip install xcoll\n```\nFor a local installation, clone and install in editable mode (need to have `pip` >22):\n```bash\ngit clone git@github.com:xsuite/xcoll.git\npip install -e xcoll\n```\n\n### Example\n\n## Features\n\n## Authors\n\n* [Frederik Van der Veken](https://github.com/freddieknets) (frederik@cern.ch)\n* [Despina Demetriadou](https://github.com/ddemetriadou)\n* [Andrey Abramov](https://github.com/anabramo)\n* [Giovanni Iadarola](https://github.com/giadarol)\n\n\n## Version History\n\n* 0.1\n    * Initial Release\n\n## License\n\nThis project is [Apache 2.0 licensed](./LICENSE).\n',
     'author': 'Frederik F. Van der Veken',
     'author_email': 'frederik@cern.ch',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/xsuite/xcoll',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `xcoll-0.2.1/PKG-INFO` & `xcoll-0.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 Metadata-Version: 2.1
 Name: xcoll
-Version: 0.2.1
+Version: 0.2.2
 Summary: Xsuite collimation package
 Home-page: https://github.com/xsuite/xcoll
 License: Apache 2.0
 Author: Frederik F. Van der Veken
 Author-email: frederik@cern.ch
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: tests
+Requires-Dist: numpy (>=1.0)
+Requires-Dist: pandas (>=1.4)
+Requires-Dist: ruamel-yaml (>=0.17.31,<0.18.0); extra == "tests"
+Requires-Dist: xcoll (>=0.2.1,<0.3.0)
+Requires-Dist: xdeps (>=0.1.1,<0.2.0)
+Requires-Dist: xfields (>=0.12.1,<0.13.0)
+Requires-Dist: xobjects (>=0.2.6,<0.3.0)
+Requires-Dist: xpart (>=0.15.0,<0.16.0)
+Requires-Dist: xtrack (>=0.36.5,<0.37.0)
 Project-URL: Repository, https://github.com/xsuite/xcoll
 Description-Content-Type: text/markdown
 
 # xcoll
 
 <!---![PyPI - Python Version](https://img.shields.io/pypi/pyversions/xcoll?logo=PyPI?style=plastic) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/xcoll?logo=PyPI?style=plastic)-->
 
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/xsuite/xcoll?style=plastic) ![GitHub](https://img.shields.io/github/license/xsuite/xcoll?style=plastic) ![GitHub all releases](https://img.shields.io/github/downloads/xsuite/xcoll/total?logo=GitHub&style=plastic) ![GitHub issues](https://img.shields.io/github/issues/xsuite/xcoll?logo=GitHub&style=plastic) ![GitHub pull requests](https://img.shields.io/github/issues-pr/xsuite/xcoll?logo=GitHub&style=plastic) ![GitHub repo size](https://img.shields.io/github/repo-size/xsuite/xcoll?logo=GitHub&style=plastic)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/xsuite/xcoll?style=plastic)
+![GitHub](https://img.shields.io/github/license/xsuite/xcoll?style=plastic)
+![PyPi](https://img.shields.io/pypi/dm/xcoll?logo=PyPI&style=plastic)
+![GitHub all releases](https://img.shields.io/github/downloads/xsuite/xcoll/total?logo=GitHub&style=plastic)
+
+![GitHub pull requests](https://img.shields.io/github/issues-pr/xsuite/xcoll?logo=GitHub&style=plastic)
+![GitHub issues](https://img.shields.io/github/issues/xsuite/xcoll?logo=GitHub&style=plastic)
+![GitHub repo size](https://img.shields.io/github/repo-size/xsuite/xcoll?logo=GitHub&style=plastic)
 
 Collimation in xtrack simulations
 
 ## Description
 
 ## Getting Started
```

