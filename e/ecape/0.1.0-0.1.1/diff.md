# Comparing `tmp/ecape-0.1.0.tar.gz` & `tmp/ecape-0.1.1.tar.gz`

## Comparing `ecape-0.1.0.tar` & `ecape-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/a29a86d92757c5f3
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/b19916efceeeaf7a
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/dbc4039e534a1a09
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/e094db35918da83a
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.1.0/.ruff_cache/content/ebce8b83716b5643
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.1.0/src/ecape/__about__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.1.0/src/ecape/__init__.py
--rw-r--r--   0        0        0    13652 2020-02-02 00:00:00.000000 ecape-0.1.0/src/ecape/calc.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.1.0/.gitignore
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ecape-0.1.0/README.md
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 ecape-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ecape-0.1.1/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.1.1/.ruff_cache/content/a29a86d92757c5f3
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 ecape-0.1.1/.ruff_cache/content/b19916efceeeaf7a
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 ecape-0.1.1/.ruff_cache/content/dbc4039e534a1a09
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 ecape-0.1.1/.ruff_cache/content/e094db35918da83a
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 ecape-0.1.1/.ruff_cache/content/ebce8b83716b5643
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ecape-0.1.1/src/ecape/__about__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ecape-0.1.1/src/ecape/__init__.py
+-rw-r--r--   0        0        0    13659 2020-02-02 00:00:00.000000 ecape-0.1.1/src/ecape/calc.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 ecape-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 ecape-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 ecape-0.1.1/README.md
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 ecape-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 ecape-0.1.1/PKG-INFO
```

### Comparing `ecape-0.1.0/.ruff_cache/content/b19916efceeeaf7a` & `ecape-0.1.1/.ruff_cache/content/b19916efceeeaf7a`

 * *Files identical despite different names*

### Comparing `ecape-0.1.0/.ruff_cache/content/dbc4039e534a1a09` & `ecape-0.1.1/.ruff_cache/content/dbc4039e534a1a09`

 * *Files identical despite different names*

### Comparing `ecape-0.1.0/.ruff_cache/content/e094db35918da83a` & `ecape-0.1.1/.ruff_cache/content/e094db35918da83a`

 * *Files identical despite different names*

### Comparing `ecape-0.1.0/src/ecape/calc.py` & `ecape-0.1.1/src/ecape/calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import metpy.calc as mpcalc
 import numpy as np
 import pint
 from metpy.constants import dry_air_spec_heat_press, earth_gravity
 from metpy.units import check_units, units
 
-PintList = np.ndarray[pint.Quantity]
+PintList = np.typing.NDArray[pint.Quantity]
 
 
 @check_units("[pressure]", "[temperature]", "[temperature]")
 def _get_parcel_profile(
     pressure: PintList, temperature: PintList, dew_point_temperature: PintList, parcel_func: Callable = None
 ) -> PintList:
     """
```

### Comparing `ecape-0.1.0/LICENSE.txt` & `ecape-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ecape-0.1.0/README.md` & `ecape-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -60,12 +60,12 @@
 
 
 ### References
 Ryan M. May, Sean C. Arms, Patrick Marsh, Eric Bruning, John R. Leeman, Kevin Goebbert, Jonathan E. Thielen, Zachary S Bruick, and M. Drew. Camron. Metpy: a Python package for meteorological data. 2023. URL: Unidata/MetPy, doi:10.5065/D6WW7G29.
 
 John Peters. ECAPE scripts. 2 2023. URL: https://figshare.com/articles/software/ECAPE_scripts/21859818, doi:10.6084/m9.figshare.21859818.v4.
 
-John M. Peters, Daniel R. Chavas, Hugh Morrison, Chun-Yian Su, and Brice E. Coffer. An analytic formula for entraining cape in mid-latitude storm environments. 2023. arXiv:2301.04712.
+Peters, J. M., D. R. Chavas, C. Su, H. Morrison, and B. E. Coffer, 2023: An analytic formula for entraining CAPE in mid-latitude storm environments. J. Atmos. Sci., https://doi.org/10.1175/JAS-D-23-0003.1, in press.
 
 ### Licence
 
 `ecape` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `ecape-0.1.0/pyproject.toml` & `ecape-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "MetPy>=1.2.0",
-  "numpy>=1.18.0",
+  "numpy>=1.21.0",
   "pytest"
 ]
 
 [project.urls]
 Documentation = "https://citylikeamradio.github.io/ecape"
 Issues = "https://github.com/citylikeamradio/ecape/issues"
 Source = "https://github.com/citylikeamradio/ecape"
```

### Comparing `ecape-0.1.0/PKG-INFO` & `ecape-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecape
-Version: 0.1.0
+Version: 0.1.1
 Summary: Calculate the entraining CAPE (ECAPE) of a parcel.
 Project-URL: Documentation, https://citylikeamradio.github.io/ecape
 Project-URL: Issues, https://github.com/citylikeamradio/ecape/issues
 Project-URL: Source, https://github.com/citylikeamradio/ecape
 Author-email: Robert Capella <bob.capella@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: metpy>=1.2.0
-Requires-Dist: numpy>=1.18.0
+Requires-Dist: numpy>=1.21.0
 Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # ecape
 
 ecape is a simple module that contains an entraining CAPE, or ECAPE, calculation described by Peters et. al. 2023.
 Peters-provided MatLab scripts serve as a reference and test verification data.
@@ -82,12 +82,12 @@
 
 
 ### References
 Ryan M. May, Sean C. Arms, Patrick Marsh, Eric Bruning, John R. Leeman, Kevin Goebbert, Jonathan E. Thielen, Zachary S Bruick, and M. Drew. Camron. Metpy: a Python package for meteorological data. 2023. URL: Unidata/MetPy, doi:10.5065/D6WW7G29.
 
 John Peters. ECAPE scripts. 2 2023. URL: https://figshare.com/articles/software/ECAPE_scripts/21859818, doi:10.6084/m9.figshare.21859818.v4.
 
-John M. Peters, Daniel R. Chavas, Hugh Morrison, Chun-Yian Su, and Brice E. Coffer. An analytic formula for entraining cape in mid-latitude storm environments. 2023. arXiv:2301.04712.
+Peters, J. M., D. R. Chavas, C. Su, H. Morrison, and B. E. Coffer, 2023: An analytic formula for entraining CAPE in mid-latitude storm environments. J. Atmos. Sci., https://doi.org/10.1175/JAS-D-23-0003.1, in press.
 
 ### Licence
 
 `ecape` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

