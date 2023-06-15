# Comparing `tmp/bihc-0.0.8.1.tar.gz` & `tmp/bihc-0.0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/edelafue/BIHC/dist/.tmp-ezemyt_h/bihc-0.0.8.1.tar", last modified: Wed May 31 14:43:34 2023, max compression
+gzip compressed data, was "/home/edelafue/BIHC/dist/.tmp-d8il9hxr/bihc-0.0.8.2.tar", last modified: Thu Jun 15 15:42:59 2023, max compression
```

## Comparing `bihc-0.0.8.1.tar` & `bihc-0.0.8.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-05-31 14:43:34.000000 bihc-0.0.8.1/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      760 2022-12-08 10:22:14.000000 bihc-0.0.8.1/LICENSE
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      105 2022-12-08 10:22:14.000000 bihc-0.0.8.1/MANIFEST.in
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-31 14:43:34.000000 bihc-0.0.8.1/PKG-INFO
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     2686 2023-01-20 08:26:47.000000 bihc-0.0.8.1/README.md
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      172 2023-03-28 09:04:32.000000 bihc-0.0.8.1/bihc/__init__.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)    28294 2023-05-31 14:41:18.000000 bihc-0.0.8.1/bihc/beam.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     6330 2023-05-19 11:33:18.000000 bihc-0.0.8.1/bihc/impedance.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     9085 2023-05-31 14:26:46.000000 bihc-0.0.8.1/bihc/plot.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     4157 2023-03-08 15:02:48.000000 bihc-0.0.8.1/bihc/power.py
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/PKG-INFO
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      334 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/SOURCES.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        1 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/dependency_links.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       23 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/requires.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        5 2023-05-31 14:43:34.000000 bihc-0.0.8.1/bihc.egg-info/top_level.txt
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      128 2022-12-16 15:42:39.000000 bihc-0.0.8.1/pyproject.toml
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       38 2023-05-31 14:43:34.000000 bihc-0.0.8.1/setup.cfg
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1082 2023-05-31 14:42:25.000000 bihc-0.0.8.1/setup.py
-drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-05-31 14:43:34.000000 bihc-0.0.8.1/tests/
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1886 2023-03-23 17:54:24.000000 bihc-0.0.8.1/tests/test_analyticBunchShapes.py
--rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3008 2023-03-23 17:41:58.000000 bihc-0.0.8.1/tests/test_numericBunchShapes.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-06-15 15:42:59.000000 bihc-0.0.8.2/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      760 2022-12-08 10:22:14.000000 bihc-0.0.8.2/LICENSE
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      105 2022-12-08 10:22:14.000000 bihc-0.0.8.2/MANIFEST.in
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-06-15 15:42:59.000000 bihc-0.0.8.2/PKG-INFO
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     2686 2023-01-20 08:26:47.000000 bihc-0.0.8.2/README.md
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      172 2023-03-28 09:04:32.000000 bihc-0.0.8.2/bihc/__init__.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)    28370 2023-05-31 15:03:32.000000 bihc-0.0.8.2/bihc/beam.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        0 2023-06-02 14:25:40.000000 bihc-0.0.8.2/bihc/fillingschemes.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     6330 2023-05-19 11:33:18.000000 bihc-0.0.8.2/bihc/impedance.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     9085 2023-05-31 14:26:46.000000 bihc-0.0.8.2/bihc/plot.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     7267 2023-06-15 15:39:26.000000 bihc-0.0.8.2/bihc/power.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3260 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/PKG-INFO
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      357 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/SOURCES.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        1 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/dependency_links.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       23 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/requires.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)        5 2023-06-15 15:42:59.000000 bihc-0.0.8.2/bihc.egg-info/top_level.txt
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)      128 2022-12-16 15:42:39.000000 bihc-0.0.8.2/pyproject.toml
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)       38 2023-06-15 15:42:59.000000 bihc-0.0.8.2/setup.cfg
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1082 2023-06-15 15:39:56.000000 bihc-0.0.8.2/setup.py
+drwxrwxr-x   0 edelafue  (1000) edelafue  (1000)        0 2023-06-15 15:42:59.000000 bihc-0.0.8.2/tests/
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     1886 2023-03-23 17:54:24.000000 bihc-0.0.8.2/tests/test_analyticBunchShapes.py
+-rw-rw-r--   0 edelafue  (1000) edelafue  (1000)     3008 2023-03-23 17:41:58.000000 bihc-0.0.8.2/tests/test_numericBunchShapes.py
```

### Comparing `bihc-0.0.8.1/LICENSE` & `bihc-0.0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.1/PKG-INFO` & `bihc-0.0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.8.1
+Version: 0.0.8.2
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.8.1/README.md` & `bihc-0.0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.1/bihc/beam.py` & `bihc-0.0.8.2/bihc/beam.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,14 +300,16 @@
             self._isSpectrumReady = True
             
             return self._spectrum
         
     #@spectrum.setter
     def setSpectrum(self, newSpectrum): 
         self._spectrum = newSpectrum
+        [f,s] = self._spectrum
+        self.powerSpectrum=[f, np.abs(s)**2]
         self._isSpectrumReady = True
         #raise Exception("Spectrum can not be assigned")
                      
     def setBunches(self, newLongitudinalProfile, interp=True):
         [t,s] = newlongitudinalProfile
     
         if interp:
```

### Comparing `bihc-0.0.8.1/bihc/impedance.py` & `bihc-0.0.8.2/bihc/impedance.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.1/bihc/plot.py` & `bihc-0.0.8.2/bihc/plot.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.1/bihc.egg-info/PKG-INFO` & `bihc-0.0.8.2/bihc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bihc
-Version: 0.0.8.1
+Version: 0.0.8.2
 Summary: BIHC: Beam-Induced Heating Computation package
 Home-page: https://github.com/LeonardoSito/BIHC
 Author: Francesco Giordano
 Author-email: benoit.salvant@cern.ch
 Project-URL: Bug Tracker, https://github.com/LeonardoSito/BIHC/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bihc-0.0.8.1/setup.py` & `bihc-0.0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #########
 # Setup #
 #########
 
 setup(
     name="bihc",
-    version="0.0.8.1",
+    version="0.0.8.2",
     description="BIHC: Beam-Induced Heating Computation package",
     author="Francesco Giordano",
     author_email="benoit.salvant@cern.ch", 
     packages=['bihc'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LeonardoSito/BIHC",
```

### Comparing `bihc-0.0.8.1/tests/test_analyticBunchShapes.py` & `bihc-0.0.8.2/tests/test_analyticBunchShapes.py`

 * *Files identical despite different names*

### Comparing `bihc-0.0.8.1/tests/test_numericBunchShapes.py` & `bihc-0.0.8.2/tests/test_numericBunchShapes.py`

 * *Files identical despite different names*

