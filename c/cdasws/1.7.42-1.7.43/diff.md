# Comparing `tmp/cdasws-1.7.42.tar.gz` & `tmp/cdasws-1.7.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdasws-1.7.42.tar", last modified: Tue Oct 25 14:35:56 2022, max compression
+gzip compressed data, was "dist/cdasws-1.7.43.tar", last modified: Thu Jun 15 16:19:31 2023, max compression
```

## Comparing `cdasws-1.7.42.tar` & `cdasws-1.7.43.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwx---   0 btharris   (503) btharris   (503)        0 2022-10-25 14:35:56.000000 cdasws-1.7.42/
-drwxrwx---   0 btharris   (503) btharris   (503)        0 2022-10-25 14:35:56.000000 cdasws-1.7.42/cdasws/
--rw-rw----   0 btharris   (503) btharris   (503)    73010 2022-10-20 10:46:31.000000 cdasws-1.7.42/cdasws/__init__.py
--rw-rw----   0 btharris   (503) btharris   (503)    12241 2022-10-20 10:26:35.000000 cdasws-1.7.42/cdasws/__main__.py
--rw-rw----   0 btharris   (503) btharris   (503)     2165 2022-03-16 18:03:02.000000 cdasws-1.7.42/cdasws/datarepresentation.py
--rw-rw----   0 btharris   (503) btharris   (503)    20594 2021-03-02 11:56:27.000000 cdasws-1.7.42/cdasws/datarequest.py
--rw-rw----   0 btharris   (503) btharris   (503)     5664 2021-03-02 11:49:06.000000 cdasws-1.7.42/cdasws/timeinterval.py
-drwxrwx---   0 btharris   (503) btharris   (503)        0 2022-10-25 14:35:56.000000 cdasws-1.7.42/cdasws.egg-info/
--rw-rw----   0 btharris   (503) btharris   (503)     6322 2022-10-25 14:35:56.000000 cdasws-1.7.42/cdasws.egg-info/PKG-INFO
--rw-rw----   0 btharris   (503) btharris   (503)      279 2022-10-25 14:35:56.000000 cdasws-1.7.42/cdasws.egg-info/SOURCES.txt
--rw-rw----   0 btharris   (503) btharris   (503)        1 2022-10-25 14:35:56.000000 cdasws-1.7.42/cdasws.egg-info/dependency_links.txt
--rw-rw----   0 btharris   (503) btharris   (503)       85 2022-10-25 14:35:56.000000 cdasws-1.7.42/cdasws.egg-info/requires.txt
--rw-rw----   0 btharris   (503) btharris   (503)        7 2022-10-25 14:35:56.000000 cdasws-1.7.42/cdasws.egg-info/top_level.txt
--rw-rw----   0 btharris   (503) btharris   (503)     4448 2022-10-07 11:09:20.000000 cdasws-1.7.42/README.md
--rw-rw----   0 btharris   (503) btharris   (503)     1939 2022-10-18 12:51:32.000000 cdasws-1.7.42/setup.py
--rw-rw----   0 btharris   (503) btharris   (503)     6322 2022-10-25 14:35:56.000000 cdasws-1.7.42/PKG-INFO
--rw-rw----   0 btharris   (503) btharris   (503)       38 2022-10-25 14:35:56.000000 cdasws-1.7.42/setup.cfg
+drwxrwx---   0 btharris   (503) btharris   (503)        0 2023-06-15 16:19:31.000000 cdasws-1.7.43/
+drwxrwx---   0 btharris   (503) btharris   (503)        0 2023-06-15 16:19:31.000000 cdasws-1.7.43/cdasws/
+-rw-rw----   0 btharris   (503) btharris   (503)    73578 2023-06-15 16:16:14.000000 cdasws-1.7.43/cdasws/__init__.py
+-rw-rw----   0 btharris   (503) btharris   (503)    12241 2023-06-15 16:13:03.000000 cdasws-1.7.43/cdasws/__main__.py
+-rw-rw----   0 btharris   (503) btharris   (503)     2165 2023-06-15 16:13:03.000000 cdasws-1.7.43/cdasws/datarepresentation.py
+-rw-rw----   0 btharris   (503) btharris   (503)    20594 2023-06-15 16:13:03.000000 cdasws-1.7.43/cdasws/datarequest.py
+-rw-rw----   0 btharris   (503) btharris   (503)     5664 2023-06-15 16:13:03.000000 cdasws-1.7.43/cdasws/timeinterval.py
+drwxrwx---   0 btharris   (503) btharris   (503)        0 2023-06-15 16:19:31.000000 cdasws-1.7.43/cdasws.egg-info/
+-rw-rw----   0 btharris   (503) btharris   (503)     6419 2023-06-15 16:19:31.000000 cdasws-1.7.43/cdasws.egg-info/PKG-INFO
+-rw-rw----   0 btharris   (503) btharris   (503)      279 2023-06-15 16:19:31.000000 cdasws-1.7.43/cdasws.egg-info/SOURCES.txt
+-rw-rw----   0 btharris   (503) btharris   (503)        1 2023-06-15 16:19:31.000000 cdasws-1.7.43/cdasws.egg-info/dependency_links.txt
+-rw-rw----   0 btharris   (503) btharris   (503)       85 2023-06-15 16:19:31.000000 cdasws-1.7.43/cdasws.egg-info/requires.txt
+-rw-rw----   0 btharris   (503) btharris   (503)        7 2023-06-15 16:19:31.000000 cdasws-1.7.43/cdasws.egg-info/top_level.txt
+-rw-rw----   0 btharris   (503) btharris   (503)     4529 2023-06-15 16:13:03.000000 cdasws-1.7.43/README.md
+-rw-rw----   0 btharris   (503) btharris   (503)     1939 2023-06-15 16:14:53.000000 cdasws-1.7.43/setup.py
+-rw-rw----   0 btharris   (503) btharris   (503)     6419 2023-06-15 16:19:31.000000 cdasws-1.7.43/PKG-INFO
+-rw-rw----   0 btharris   (503) btharris   (503)       38 2023-06-15 16:19:31.000000 cdasws-1.7.43/setup.cfg
```

### Comparing `cdasws-1.7.42/cdasws/__init__.py` & `cdasws-1.7.43/cdasws/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,26 +20,26 @@
 # docs/NASA_Open_Source_Agreement_1.3.txt.  If applicable, add the
 # following below this NOSA HEADER, with the fields enclosed by
 # brackets "[]" replaced with your own identifying information:
 # Portions Copyright [yyyy] [name of copyright owner]
 #
 # NOSA HEADER END
 #
-# Copyright (c) 2018-2022 United States Government as represented by
+# Copyright (c) 2018-2023 United States Government as represented by
 # the National Aeronautics and Space Administration. No copyright is
 # claimed in the United States under Title 17, U.S.Code. All Other
 # Rights Reserved.
 #
 
 
 """
 Package for accessing the Coordinate Data Analysis System (CDAS)
 web services <https://cdaweb.gsfc.nasa.gov/WebServices/REST/>.<br>
 
-Copyright &copy; 2018-2022 United States Government as represented by the
+Copyright &copy; 2018-2023 United States Government as represented by the
 National Aeronautics and Space Administration. No copyright is claimed in
 the United States under Title 17, U.S.Code. All Other Rights Reserved.
 
 Notes
 -----
 Due to rate limiting implemented by the CDAS web services, an attempt
 to make simultaneous requests from many threads is likely to actually
@@ -75,22 +75,32 @@
 try:
     import spacepy.datamodel as spdm    # type: ignore
     SPDM_AVAILABLE = True
 except ImportError:
     SPDM_AVAILABLE = False
 
 try:
-    import cdflib as cdf
+    from cdflib.xarray import cdf_to_xarray
     import xarray as xr
     CDF_XARRAY_AVAILABLE = True
 except ImportError:
-    CDF_XARRAY_AVAILABLE = False
+    try:
+        import cdflib as cdf
+        import xarray as xr
+        CDF_XARRAY_AVAILABLE = True
+        def cdf_to_xarray(filename, to_datetime=False, to_unixtime=False,
+                          fillval_to_nan=False):
+            return cdf.cdf_to_xarray(filename, to_datetime=to_datetime, 
+                                     to_unixtime=to_unixtime, 
+                                     fillval_to_nan=fillval_to_nan)
+    except ImportError:
+        CDF_XARRAY_AVAILABLE = False
 
 
-__version__ = "1.7.42"
+__version__ = "1.7.43"
 
 
 #
 # Limit on the number of times an HTTP request which returns a
 # 429 or 503 status with a Retry-After header will be retried.
 #
 RETRY_LIMIT = 100
@@ -1179,23 +1189,24 @@
             If neither the spacepy.datamodel nor the cdflib and xarray
             modules are installed.
         """
         if data_representation is None:
             if SPDM_AVAILABLE:
                 return spdm.fromCDF(filename)
             if CDF_XARRAY_AVAILABLE:
-                return cdf.cdf_to_xarray(filename)
+                return cdf_to_xarray(filename, to_datetime=True,
+                                     fillval_to_nan=True)
             raise ModuleNotFoundError(
                 'neither the spacepy.datamodel nor the cdflib and '
                 'xarray modules are installed')
         if data_representation is DataRepresentation.SPACEPY:
             return spdm.fromCDF(filename)
         if data_representation is DataRepresentation.XARRAY:
-            return cdf.cdf_to_xarray(filename, to_datetime=True,
-                                     fillval_to_nan=True)
+            return cdf_to_xarray(filename, to_datetime=True,
+                                 fillval_to_nan=True)
         return None
 
 
     def get_data(
             self,
             dataset: str,
             variables: List[str],
@@ -1257,19 +1268,20 @@
             <b>progressUserValue</b> - is an Any value that is passsed
             to the progressCallback function.<br>
         Returns
         -------
         Tuple
             [0] contains a dictionary of HTTP and CDAS status information.
             When successful, ['http']['status_code'] will be 200.<br>
-            [1] contains the requested data (SpaceData object) or None.
+            [1] contains the requested data (SpaceData or xarray.Dateset 
+            object) or None.
         Raises
         ------
         ValueError
-            If no variables are given or if the given start/end datetime 
+            If no variables are given or if the given start/end datetime
             values are invalid.
         """
         # pylint: disable=too-many-locals
         # pylint: disable=too-many-return-statements
         # pylint: disable=too-many-statements
         # pylint: disable=too-many-branches
         # pylint: disable=import-outside-toplevel
@@ -1796,16 +1808,16 @@
             self,
             dataset: str,
             start: Union[datetime, str],
             end: Union[datetime, str],
             **keywords
         ) -> Tuple[int, Dict]:
         """
-        Gets original data files from a dataset.  Original data files 
-        lack updated meta-data and virtual variable values contained 
+        Gets original data files from a dataset.  Original data files
+        lack updated meta-data and virtual variable values contained
         in files obtained from the `CdasWs.get_data`.  Most callers
         should probably use `CdasWs.get_data` instead of this function.
 
         Parameters
         ----------
         dataset
             dataset identifier of data to get.
```

### Comparing `cdasws-1.7.42/cdasws/__main__.py` & `cdasws-1.7.43/cdasws/__main__.py`

 * *Files identical despite different names*

### Comparing `cdasws-1.7.42/cdasws/datarepresentation.py` & `cdasws-1.7.43/cdasws/datarepresentation.py`

 * *Files identical despite different names*

### Comparing `cdasws-1.7.42/cdasws/datarequest.py` & `cdasws-1.7.43/cdasws/datarequest.py`

 * *Files identical despite different names*

### Comparing `cdasws-1.7.42/cdasws/timeinterval.py` & `cdasws-1.7.43/cdasws/timeinterval.py`

 * *Files identical despite different names*

### Comparing `cdasws-1.7.42/cdasws.egg-info/PKG-INFO` & `cdasws-1.7.43/cdasws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdasws
-Version: 1.7.42
+Version: 1.7.43
 Summary: NASA's Coordinated Data Analysis System Web Service Client Library
 Home-page: https://cdaweb.gsfc.nasa.gov/WebServices/REST
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Description: 
         ## Synopsis
@@ -31,15 +31,15 @@
             python -m cdasws
         
         ---
         Also, the following [Jupyter notebooks](https://jupyter.org/) demonstrate
         different features of the library:
         1. [Basic Example](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExample.html) ([ipynb file](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExample.ipynb)) demonstrating use of library with results returned in [SpacePy data model](https://spacepy.github.io/datamodel.html).
         2. [Basic Example](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.html) ([ipynb file](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.ipynb)) demonstrating use of library with results returned in an [xarray.Dataset](https://docs.xarray.dev/en/stable/generated/xarray.Dataset.html). [Launch on Binder](https://mybinder.org/v2/gh/berniegsfc/cdasws-notebooks/main?labpath=CdasWsExampleXarray.ipynb).
-        3. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/). [Lauch on Binder](https://mybinder.org/v2/gh/berniegsfc/sscws-notebooks/main?labpath=SscWsConjunctionExample.ipynb).
+        3. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/). [Launch on Binder](https://mybinder.org/v2/gh/berniegsfc/sscws-notebooks/main?labpath=SscWsConjunctionExample.ipynb).
         ---
         And at the bottom of each 
         [CDAWeb dataset description](https://cdaweb.gsfc.nasa.gov/misc/Notes.html) 
         is a "Data Access Code Examples" link that contains dataset-specific code 
         utilizing this package to access the data.
         
         ## Motivation
@@ -66,17 +66,19 @@
         ## Installation
         
         As noted in the dependencies above, if you intend to call the get_data
         method, you must install either
         1. [SpacePy](https://pythonhosted.org/SpacePy/) and the 
            [CDF](https://cdf.gsfc.nasa.gov) library (following the
            procedures at the SpacePy and CDF web sites).
-        2. [cdflib](https://pypi.org/project/cdflib/).
+        2. [cdflib](https://pypi.org/project/cdflib/) and 
+           [xarray](https://pypi.org/project/xarray/) .
         
             $ pip install -U cdflib
+            $ pip install -U xarray
         
         Then, to install this package
         
             $ pip install -U cdasws
         
         
         ## API Reference
```

### Comparing `cdasws-1.7.42/README.md` & `cdasws-1.7.43/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     python -m cdasws
 
 ---
 Also, the following [Jupyter notebooks](https://jupyter.org/) demonstrate
 different features of the library:
 1. [Basic Example](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExample.html) ([ipynb file](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExample.ipynb)) demonstrating use of library with results returned in [SpacePy data model](https://spacepy.github.io/datamodel.html).
 2. [Basic Example](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.html) ([ipynb file](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.ipynb)) demonstrating use of library with results returned in an [xarray.Dataset](https://docs.xarray.dev/en/stable/generated/xarray.Dataset.html). [Launch on Binder](https://mybinder.org/v2/gh/berniegsfc/cdasws-notebooks/main?labpath=CdasWsExampleXarray.ipynb).
-3. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/). [Lauch on Binder](https://mybinder.org/v2/gh/berniegsfc/sscws-notebooks/main?labpath=SscWsConjunctionExample.ipynb).
+3. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/). [Launch on Binder](https://mybinder.org/v2/gh/berniegsfc/sscws-notebooks/main?labpath=SscWsConjunctionExample.ipynb).
 ---
 And at the bottom of each 
 [CDAWeb dataset description](https://cdaweb.gsfc.nasa.gov/misc/Notes.html) 
 is a "Data Access Code Examples" link that contains dataset-specific code 
 utilizing this package to access the data.
 
 ## Motivation
@@ -58,17 +58,19 @@
 ## Installation
 
 As noted in the dependencies above, if you intend to call the get_data
 method, you must install either
 1. [SpacePy](https://pythonhosted.org/SpacePy/) and the 
    [CDF](https://cdf.gsfc.nasa.gov) library (following the
    procedures at the SpacePy and CDF web sites).
-2. [cdflib](https://pypi.org/project/cdflib/).
+2. [cdflib](https://pypi.org/project/cdflib/) and 
+   [xarray](https://pypi.org/project/xarray/) .
 
     $ pip install -U cdflib
+    $ pip install -U xarray
 
 Then, to install this package
 
     $ pip install -U cdasws
 
 
 ## API Reference
```

### Comparing `cdasws-1.7.42/setup.py` & `cdasws-1.7.43/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="cdasws",
-    version="1.7.42",
+    version="1.7.43",
     description="NASA's Coordinated Data Analysis System Web Service Client Library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://cdaweb.gsfc.nasa.gov/WebServices/REST",
     author="Bernie Harris",
     author_email="NASA-SPDF-Support@nasa.onmicrosoft.com",
     license="NOSA",
```

### Comparing `cdasws-1.7.42/PKG-INFO` & `cdasws-1.7.43/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdasws
-Version: 1.7.42
+Version: 1.7.43
 Summary: NASA's Coordinated Data Analysis System Web Service Client Library
 Home-page: https://cdaweb.gsfc.nasa.gov/WebServices/REST
 Author: Bernie Harris
 Author-email: NASA-SPDF-Support@nasa.onmicrosoft.com
 License: NOSA
 Description: 
         ## Synopsis
@@ -31,15 +31,15 @@
             python -m cdasws
         
         ---
         Also, the following [Jupyter notebooks](https://jupyter.org/) demonstrate
         different features of the library:
         1. [Basic Example](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExample.html) ([ipynb file](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExample.ipynb)) demonstrating use of library with results returned in [SpacePy data model](https://spacepy.github.io/datamodel.html).
         2. [Basic Example](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.html) ([ipynb file](https://cdaweb.gsfc.nasa.gov/WebServices/REST/jupyter/CdasWsExampleXarray.ipynb)) demonstrating use of library with results returned in an [xarray.Dataset](https://docs.xarray.dev/en/stable/generated/xarray.Dataset.html). [Launch on Binder](https://mybinder.org/v2/gh/berniegsfc/cdasws-notebooks/main?labpath=CdasWsExampleXarray.ipynb).
-        3. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/). [Lauch on Binder](https://mybinder.org/v2/gh/berniegsfc/sscws-notebooks/main?labpath=SscWsConjunctionExample.ipynb).
+        3. [Magnetic Field Line Conjunction Example](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.html) ([ipynb file](https://sscweb.gsfc.nasa.gov/WebServices/REST/jupyter/SscWsConjunctionExample.ipynb)) with related data retrieval/plotting using [cdasws](https://pypi.org/project/cdasws/). [Launch on Binder](https://mybinder.org/v2/gh/berniegsfc/sscws-notebooks/main?labpath=SscWsConjunctionExample.ipynb).
         ---
         And at the bottom of each 
         [CDAWeb dataset description](https://cdaweb.gsfc.nasa.gov/misc/Notes.html) 
         is a "Data Access Code Examples" link that contains dataset-specific code 
         utilizing this package to access the data.
         
         ## Motivation
@@ -66,17 +66,19 @@
         ## Installation
         
         As noted in the dependencies above, if you intend to call the get_data
         method, you must install either
         1. [SpacePy](https://pythonhosted.org/SpacePy/) and the 
            [CDF](https://cdf.gsfc.nasa.gov) library (following the
            procedures at the SpacePy and CDF web sites).
-        2. [cdflib](https://pypi.org/project/cdflib/).
+        2. [cdflib](https://pypi.org/project/cdflib/) and 
+           [xarray](https://pypi.org/project/xarray/) .
         
             $ pip install -U cdflib
+            $ pip install -U xarray
         
         Then, to install this package
         
             $ pip install -U cdasws
         
         
         ## API Reference
```

