# Comparing `tmp/encomp-0.9.6.tar.gz` & `tmp/encomp-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encomp-0.9.6.tar", max compression
+gzip compressed data, was "encomp-0.9.7.tar", max compression
```

## Comparing `encomp-0.9.6.tar` & `encomp-0.9.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1072 2023-04-25 07:41:03.603957 encomp-0.9.6/LICENSE
--rw-r--r--   0        0        0    10423 2023-06-12 08:10:46.714920 encomp-0.9.6/README.md
--rw-r--r--   0        0        0       78 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/__init__.py
--rw-r--r--   0        0        0      710 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/constants.py
--rw-r--r--   0        0        0     1895 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/context.py
--rw-r--r--   0        0        0     1976 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/conversion.py
--rw-r--r--   0        0        0     4453 2023-03-12 08:05:11.060958 encomp-0.9.6/encomp/defs/constants.txt
--rw-r--r--   0        0        0    31139 2023-03-12 08:05:11.060958 encomp-0.9.6/encomp/defs/units.txt
--rw-r--r--   0        0        0    44819 2023-05-11 17:03:16.518616 encomp-0.9.6/encomp/fluids.py
--rw-r--r--   0        0        0    12415 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/gases.py
--rw-r--r--   0        0        0     7133 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/math.py
--rw-r--r--   0        0        0     5269 2023-04-25 08:07:46.797762 encomp-0.9.6/encomp/misc.py
--rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.6/encomp/py.typed
--rw-r--r--   0        0        0    14354 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/serialize.py
--rw-r--r--   0        0        0      416 2023-04-25 07:32:25.073969 encomp-0.9.6/encomp/session.py
--rw-r--r--   0        0        0     2645 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/settings.py
--rw-r--r--   0        0        0     2882 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/structures.py
--rw-r--r--   0        0        0    23410 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/sympy.py
--rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.6/encomp/tests/__init__.py
--rw-r--r--   0        0        0      197 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_constants.py
--rw-r--r--   0        0        0      904 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_context.py
--rw-r--r--   0        0        0      934 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_conversion.py
--rw-r--r--   0        0        0    10665 2023-05-11 17:03:39.366721 encomp-0.9.6/encomp/tests/test_fluids.py
--rw-r--r--   0        0        0     3065 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_fluids_types.py
--rw-r--r--   0        0        0     2542 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_function_signatures.py
--rw-r--r--   0        0        0     1103 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_gases.py
--rw-r--r--   0        0        0      189 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_math.py
--rw-r--r--   0        0        0     2066 2023-04-25 08:08:32.357986 encomp-0.9.6/encomp/tests/test_misc.py
--rw-r--r--   0        0        0     1544 2023-05-11 10:09:11.799816 encomp-0.9.6/encomp/tests/test_pandas.py
--rw-r--r--   0        0        0      777 2023-05-11 10:07:40.203132 encomp-0.9.6/encomp/tests/test_polars.py
--rw-r--r--   0        0        0     5478 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_quantity_combined.py
--rw-r--r--   0        0        0     1243 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_quantity_guard.py
--rw-r--r--   0        0        0     5200 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_quantity_inferred.py
--rw-r--r--   0        0        0      649 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_quantity_magnitude.py
--rw-r--r--   0        0        0    23222 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_quantity_types.py
--rw-r--r--   0        0        0     3453 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_serialize.py
--rw-r--r--   0        0        0      124 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_settings.py
--rw-r--r--   0        0        0     1768 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_structures.py
--rw-r--r--   0        0        0     1812 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_sympy.py
--rw-r--r--   0        0        0      929 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/tests/test_thermo.py
--rw-r--r--   0        0        0    36826 2023-06-12 08:14:20.991078 encomp-0.9.6/encomp/tests/test_units.py
--rw-r--r--   0        0        0     6402 2023-04-25 07:41:03.603957 encomp-0.9.6/encomp/thermo.py
--rw-r--r--   0        0        0    43273 2023-06-12 08:15:21.999121 encomp-0.9.6/encomp/units.py
--rw-r--r--   0        0        0    79936 2023-05-29 07:00:53.820668 encomp-0.9.6/encomp/units.pyi
--rw-r--r--   0        0        0    21664 2023-05-11 10:41:15.866326 encomp-0.9.6/encomp/utypes.py
--rw-r--r--   0        0        0     2969 2023-06-12 09:05:06.712687 encomp-0.9.6/pyproject.toml
--rw-r--r--   0        0        0    11645 1970-01-01 00:00:00.000000 encomp-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-25 07:41:03.603957 encomp-0.9.7/LICENSE
+-rw-r--r--   0        0        0    10423 2023-06-12 08:10:46.714920 encomp-0.9.7/README.md
+-rw-r--r--   0        0        0       78 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/__init__.py
+-rw-r--r--   0        0        0      710 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/constants.py
+-rw-r--r--   0        0        0     1895 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/context.py
+-rw-r--r--   0        0        0     1976 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/conversion.py
+-rw-r--r--   0        0        0     4453 2023-03-12 08:05:11.060958 encomp-0.9.7/encomp/defs/constants.txt
+-rw-r--r--   0        0        0    31157 2023-06-15 14:33:16.292593 encomp-0.9.7/encomp/defs/units.txt
+-rw-r--r--   0        0        0    44819 2023-05-11 17:03:16.518616 encomp-0.9.7/encomp/fluids.py
+-rw-r--r--   0        0        0    12415 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/gases.py
+-rw-r--r--   0        0        0     7133 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/math.py
+-rw-r--r--   0        0        0     5269 2023-04-25 08:07:46.797762 encomp-0.9.7/encomp/misc.py
+-rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.7/encomp/py.typed
+-rw-r--r--   0        0        0    14354 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/serialize.py
+-rw-r--r--   0        0        0      416 2023-04-25 07:32:25.073969 encomp-0.9.7/encomp/session.py
+-rw-r--r--   0        0        0     2645 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/settings.py
+-rw-r--r--   0        0        0     2882 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/structures.py
+-rw-r--r--   0        0        0    23410 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/sympy.py
+-rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.7/encomp/tests/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_constants.py
+-rw-r--r--   0        0        0      904 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_context.py
+-rw-r--r--   0        0        0      934 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_conversion.py
+-rw-r--r--   0        0        0    10665 2023-05-11 17:03:39.366721 encomp-0.9.7/encomp/tests/test_fluids.py
+-rw-r--r--   0        0        0     3065 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_fluids_types.py
+-rw-r--r--   0        0        0     2542 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_function_signatures.py
+-rw-r--r--   0        0        0     1103 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_gases.py
+-rw-r--r--   0        0        0      189 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_math.py
+-rw-r--r--   0        0        0     2066 2023-04-25 08:08:32.357986 encomp-0.9.7/encomp/tests/test_misc.py
+-rw-r--r--   0        0        0     1544 2023-05-11 10:09:11.799816 encomp-0.9.7/encomp/tests/test_pandas.py
+-rw-r--r--   0        0        0      777 2023-05-11 10:07:40.203132 encomp-0.9.7/encomp/tests/test_polars.py
+-rw-r--r--   0        0        0     5478 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_quantity_combined.py
+-rw-r--r--   0        0        0     1243 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_quantity_guard.py
+-rw-r--r--   0        0        0     5200 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_quantity_inferred.py
+-rw-r--r--   0        0        0      649 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_quantity_magnitude.py
+-rw-r--r--   0        0        0    23222 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_quantity_types.py
+-rw-r--r--   0        0        0     3453 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_serialize.py
+-rw-r--r--   0        0        0      124 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_settings.py
+-rw-r--r--   0        0        0     1768 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_structures.py
+-rw-r--r--   0        0        0     1812 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_sympy.py
+-rw-r--r--   0        0        0      929 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/tests/test_thermo.py
+-rw-r--r--   0        0        0    36826 2023-06-12 08:14:20.991078 encomp-0.9.7/encomp/tests/test_units.py
+-rw-r--r--   0        0        0     6402 2023-04-25 07:41:03.603957 encomp-0.9.7/encomp/thermo.py
+-rw-r--r--   0        0        0    43273 2023-06-12 08:15:21.999121 encomp-0.9.7/encomp/units.py
+-rw-r--r--   0        0        0    79936 2023-05-29 07:00:53.820668 encomp-0.9.7/encomp/units.pyi
+-rw-r--r--   0        0        0    21664 2023-05-11 10:41:15.866326 encomp-0.9.7/encomp/utypes.py
+-rw-r--r--   0        0        0     2969 2023-06-15 14:33:23.776622 encomp-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0    11645 1970-01-01 00:00:00.000000 encomp-0.9.7/PKG-INFO
```

### Comparing `encomp-0.9.6/LICENSE` & `encomp-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/README.md` & `encomp-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/constants.py` & `encomp-0.9.7/encomp/constants.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/context.py` & `encomp-0.9.7/encomp/context.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/conversion.py` & `encomp-0.9.7/encomp/conversion.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/defs/constants.txt` & `encomp-0.9.7/encomp/defs/constants.txt`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/defs/units.txt` & `encomp-0.9.7/encomp/defs/units.txt`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 #### UNITS ####
 # Common and less common, grouped by quantity.
 # Conversion factors are exact (except when noted),
 # although floating-point conversion may introduce inaccuracies
 
 percent = 1 / 100 = _ = pct = procent
 permille = 1 / 1000 = permil = promille
+ppm = 1 / 1000000
 
 # NOTE: these are only approximate, don't use for currency conversion
 SEK = 1 * currency
 EUR = 10 * currency
 USD = 10 * currency
```

### Comparing `encomp-0.9.6/encomp/fluids.py` & `encomp-0.9.7/encomp/fluids.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/gases.py` & `encomp-0.9.7/encomp/gases.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/math.py` & `encomp-0.9.7/encomp/math.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/misc.py` & `encomp-0.9.7/encomp/misc.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/serialize.py` & `encomp-0.9.7/encomp/serialize.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/settings.py` & `encomp-0.9.7/encomp/settings.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/structures.py` & `encomp-0.9.7/encomp/structures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/sympy.py` & `encomp-0.9.7/encomp/sympy.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_context.py` & `encomp-0.9.7/encomp/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_conversion.py` & `encomp-0.9.7/encomp/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_fluids.py` & `encomp-0.9.7/encomp/tests/test_fluids.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_fluids_types.py` & `encomp-0.9.7/encomp/tests/test_fluids_types.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_function_signatures.py` & `encomp-0.9.7/encomp/tests/test_function_signatures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_gases.py` & `encomp-0.9.7/encomp/tests/test_gases.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_misc.py` & `encomp-0.9.7/encomp/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_pandas.py` & `encomp-0.9.7/encomp/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_polars.py` & `encomp-0.9.7/encomp/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_quantity_combined.py` & `encomp-0.9.7/encomp/tests/test_quantity_combined.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_quantity_guard.py` & `encomp-0.9.7/encomp/tests/test_quantity_guard.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_quantity_inferred.py` & `encomp-0.9.7/encomp/tests/test_quantity_inferred.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_quantity_magnitude.py` & `encomp-0.9.7/encomp/tests/test_quantity_magnitude.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_quantity_types.py` & `encomp-0.9.7/encomp/tests/test_quantity_types.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_serialize.py` & `encomp-0.9.7/encomp/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_structures.py` & `encomp-0.9.7/encomp/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_sympy.py` & `encomp-0.9.7/encomp/tests/test_sympy.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_thermo.py` & `encomp-0.9.7/encomp/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/tests/test_units.py` & `encomp-0.9.7/encomp/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/thermo.py` & `encomp-0.9.7/encomp/thermo.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/units.py` & `encomp-0.9.7/encomp/units.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/units.pyi` & `encomp-0.9.7/encomp/units.pyi`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/encomp/utypes.py` & `encomp-0.9.7/encomp/utypes.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.6/pyproject.toml` & `encomp-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encomp"
-version = "0.9.6"
+version = "0.9.7"
 description = "General-purpose library for engineering calculations"
 authors = ["William Laurén <lauren.william.a@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "encomp" }]
 include = ["encomp/defs"]
```

### Comparing `encomp-0.9.6/PKG-INFO` & `encomp-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encomp
-Version: 0.9.6
+Version: 0.9.7
 Summary: General-purpose library for engineering calculations
 License: MIT
 Author: William Laurén
 Author-email: lauren.william.a@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

