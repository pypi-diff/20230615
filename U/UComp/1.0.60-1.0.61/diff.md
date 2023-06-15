# Comparing `tmp/UComp-1.0.60.tar.gz` & `tmp/UComp-1.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.60.tar", last modified: Wed Jun 14 17:03:10 2023, max compression
+gzip compressed data, was "UComp-1.0.61.tar", last modified: Thu Jun 15 07:07:01 2023, max compression
```

## Comparing `UComp-1.0.60.tar` & `UComp-1.0.61.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 17:03:10.482523 UComp-1.0.60/
--rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.60/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2023-06-14 17:03:10.482523 UComp-1.0.60/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.60/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 17:03:10.482523 UComp-1.0.60/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.60/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.60/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0    11378 2023-06-14 17:01:33.000000 UComp-1.0.60/UComp/ETSmodule.py
--rw-rw-rw-   0        0        0    11790 2023-06-14 14:49:10.000000 UComp-1.0.60/UComp/PTSmodule.py
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.60/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.60/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    24515 2023-06-14 14:47:37.000000 UComp-1.0.60/UComp/UCmodule.py
--rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.60/UComp/__init__.py
--rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.60/UComp/airpas.bin
--rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.60/UComp/gdp.bin
--rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.60/UComp/ipi.bin
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.60/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    29855 2023-06-14 14:47:37.000000 UComp-1.0.60/UComp/tools.py
--rw-rw-rw-   0        0        0      570 2023-06-09 15:36:47.000000 UComp-1.0.60/UComp/tsfile.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:03:10.482523 UComp-1.0.60/UComp.egg-info/
--rw-rw-rw-   0        0        0      304 2023-06-14 17:03:09.000000 UComp-1.0.60/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-06-14 17:03:09.000000 UComp-1.0.60/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 17:03:09.000000 UComp-1.0.60/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-14 17:03:09.000000 UComp-1.0.60/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-14 17:03:09.000000 UComp-1.0.60/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 17:03:10.482523 UComp-1.0.60/setup.cfg
--rw-rw-rw-   0        0        0      667 2023-06-14 17:02:47.000000 UComp-1.0.60/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:07:01.032080 UComp-1.0.61/
+-rw-rw-rw-   0        0        0      380 2023-06-09 15:39:05.000000 UComp-1.0.61/MANIFEST.in
+-rw-rw-rw-   0        0        0      343 2023-06-15 07:07:01.032080 UComp-1.0.61/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.61/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 07:07:00.978691 UComp-1.0.61/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.61/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.61/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0    11378 2023-06-14 17:01:33.000000 UComp-1.0.61/UComp/ETSmodule.py
+-rw-rw-rw-   0        0        0    11790 2023-06-14 14:49:10.000000 UComp-1.0.61/UComp/PTSmodule.py
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.61/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.61/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    24515 2023-06-14 14:47:37.000000 UComp-1.0.61/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0      149 2023-06-09 15:38:31.000000 UComp-1.0.61/UComp/__init__.py
+-rw-rw-rw-   0        0        0    16459 2023-06-14 08:43:27.000000 UComp-1.0.61/UComp/airpas.bin
+-rw-rw-rw-   0        0        0     3645 2023-06-14 08:43:27.000000 UComp-1.0.61/UComp/gdp.bin
+-rw-rw-rw-   0        0        0    14731 2023-06-14 08:43:27.000000 UComp-1.0.61/UComp/ipi.bin
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.61/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    29855 2023-06-14 14:47:37.000000 UComp-1.0.61/UComp/tools.py
+-rw-rw-rw-   0        0        0      641 2023-06-15 07:05:30.000000 UComp-1.0.61/UComp/tsfile.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:07:01.032080 UComp-1.0.61/UComp.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      450 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 07:07:00.000000 UComp-1.0.61/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 07:07:01.032080 UComp-1.0.61/setup.cfg
+-rw-rw-rw-   0        0        0      667 2023-06-15 07:06:27.000000 UComp-1.0.61/setup.py
```

### Comparing `UComp-1.0.60/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.61/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/ETSmodule.py` & `UComp-1.0.61/UComp/ETSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/PTSmodule.py` & `UComp-1.0.61/UComp/PTSmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.61/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/UCmodule.py` & `UComp-1.0.61/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/airpas.bin` & `UComp-1.0.61/UComp/airpas.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/gdp.bin` & `UComp-1.0.61/UComp/gdp.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/ipi.bin` & `UComp-1.0.61/UComp/ipi.bin`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/libopenblas.dll` & `UComp-1.0.61/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/tools.py` & `UComp-1.0.61/UComp/tools.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.60/UComp/tsfile.py` & `UComp-1.0.61/UComp/tsfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 def ts(y, start='1990', freq='A'):
     """
     Converts a numpy vector or matrix into a pandas time series
     """
     if isinstance(y, list):
         y = np.array(y)
     elif isinstance(y, pd.Series) or isinstance(y, pd.DataFrame):
-        return y
+        if start == '1990':
+            return y
+        else:
+            y = y.values
     if len(y.shape) > 1 and y.shape[0] < y.shape[1]:
         y = y.T
     time = pd.date_range(start=start, periods=y.shape[0], freq=freq)
     y = np.array(y, dtype=float)
     if len(y.shape) > 1:
         return pd.DataFrame(y, time)
     else:
```

### Comparing `UComp-1.0.60/setup.py` & `UComp-1.0.61/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.60',
+    version='1.0.61',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

