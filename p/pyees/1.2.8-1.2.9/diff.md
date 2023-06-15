# Comparing `tmp/pyees-1.2.8.tar.gz` & `tmp/pyees-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.2.8.tar", last modified: Tue May 16 05:20:22 2023, max compression
+gzip compressed data, was "pyees-1.2.9.tar", last modified: Thu Jun 15 11:42:07 2023, max compression
```

## Comparing `pyees-1.2.8.tar` & `pyees-1.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 05:20:22.614370 pyees-1.2.8/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-05-16 05:20:22.620355 pyees-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 05:20:22.458248 pyees-1.2.8/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.2.8/pyees/__init__.py
--rw-rw-rw-   0        0        0    12841 2023-05-16 05:19:59.000000 pyees-1.2.8/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.8/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.8/pyees/prop.py
--rw-rw-rw-   0        0        0    17718 2023-05-12 12:35:32.000000 pyees-1.2.8/pyees/sheet.py
--rw-rw-rw-   0        0        0    10193 2023-04-21 12:20:02.000000 pyees-1.2.8/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.8/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.8/pyees/testFit.py
--rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.8/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.2.8/pyees/testPyees.py
--rw-rw-rw-   0        0        0    15668 2023-05-12 12:42:26.000000 pyees-1.2.8/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.8/pyees/testSolve.py
--rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.2.8/pyees/testUnit.py
--rw-rw-rw-   0        0        0    81858 2023-05-12 06:34:53.000000 pyees-1.2.8/pyees/testVariable.py
--rw-rw-rw-   0        0        0    44518 2023-05-11 12:21:25.000000 pyees-1.2.8/pyees/unit.py
--rw-rw-rw-   0        0        0    35130 2023-05-16 05:20:22.473746 pyees-1.2.8/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-05-16 05:20:22.598413 pyees-1.2.8/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-05-16 05:20:21.000000 pyees-1.2.8/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-05-16 05:20:21.000000 pyees-1.2.8/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 05:20:21.000000 pyees-1.2.8/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-16 05:20:21.000000 pyees-1.2.8/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 05:20:22.607388 pyees-1.2.8/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-16 05:20:22.643293 pyees-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-05-16 05:20:04.000000 pyees-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:42:07.318090 pyees-1.2.9/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-06-15 11:42:07.333715 pyees-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 11:42:07.052459 pyees-1.2.9/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.2.9/pyees/__init__.py
+-rw-rw-rw-   0        0        0    12841 2023-05-16 05:19:59.000000 pyees-1.2.9/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.2.9/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     9126 2023-05-11 09:38:14.000000 pyees-1.2.9/pyees/prop.py
+-rw-rw-rw-   0        0        0    17718 2023-05-12 12:35:32.000000 pyees-1.2.9/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10197 2023-05-16 06:21:10.000000 pyees-1.2.9/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.2.9/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7669 2023-04-27 10:39:41.000000 pyees-1.2.9/pyees/testFit.py
+-rw-rw-rw-   0        0        0    12431 2023-05-11 09:11:30.000000 pyees-1.2.9/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-05-12 12:42:48.000000 pyees-1.2.9/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    15668 2023-05-12 12:42:26.000000 pyees-1.2.9/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.2.9/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     9094 2023-05-12 06:37:13.000000 pyees-1.2.9/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    82221 2023-06-15 11:40:52.000000 pyees-1.2.9/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    44623 2023-06-15 11:34:25.000000 pyees-1.2.9/pyees/unit.py
+-rw-rw-rw-   0        0        0    35132 2023-06-15 11:40:28.000000 pyees-1.2.9/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:42:07.271214 pyees-1.2.9/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-15 11:42:05.000000 pyees-1.2.9/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-15 11:42:07.349341 pyees-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-06-15 11:41:54.000000 pyees-1.2.9/setup.py
```

### Comparing `pyees-1.2.8/LICENSE.txt` & `pyees-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/PKG-INFO` & `pyees-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.8
+Version: 1.2.9
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.8/README.md` & `pyees-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/fit.py` & `pyees-1.2.9/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/profilePyees.py` & `pyees-1.2.9/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/prop.py` & `pyees-1.2.9/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/sheet.py` & `pyees-1.2.9/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/solve.py` & `pyees-1.2.9/pyees/solve.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     for xi in x:
         for bound in xi:
             nVariables += 1 
 
 
     ## check the number of equations and variables
     if (len(out) != nVariables):
-        raise ValueError(f'You supplied {len(out)} equations but {len(x)} variables. The number of equations and the vairables has to match')
+        raise ValueError(f'You supplied {len(out)} equations but {nVariables} variables. The number of equations and the vairables has to match')
 
     def fbounds(*x):
         out = bounds(*x)
         if not isinstance(out[0], list): out = [out]
         return out
 
     # check the bounds
```

### Comparing `pyees-1.2.8/pyees/stackOverflowODR.py` & `pyees-1.2.9/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/testFit.py` & `pyees-1.2.9/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/testProp.py` & `pyees-1.2.9/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/testPyees.py` & `pyees-1.2.9/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/testSheet.py` & `pyees-1.2.9/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/testSolve.py` & `pyees-1.2.9/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/testUnit.py` & `pyees-1.2.9/pyees/testUnit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.2.8/pyees/testVariable.py` & `pyees-1.2.9/pyees/testVariable.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,21 @@
             C_vec.uncert,
             np.array([
                 np.sqrt((1 * 2.6 * 1000 * 60)**2 + (1 * 53.9 * 1000 * 60)**2),
                 np.sqrt((1 * 5.4 * 1000 * 60)**2 + (1 * 24.75 * 1000 * 60)**2),
                 np.sqrt((1 * 10.56 * 1000 * 60)**2 + (1 * 6.4 * 1000 * 60)**2),
             ]))
 
+        A = variable(7, '%', 0.1)
+        B = 1 + A
+        self.assertAlmostEqual(B.value, 8)
+        self.assertEqual(B.unit, '%')
+        self.assertEqual(B.uncert, 0.1)
+
+
     def test_sub(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(745.1, 'L/min', uncert=53.9)
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
         B_vec = variable([745.1, 496.13, 120.54], 'L/min', uncert=[53.9, 24.75, 6.4])
 
         C = A - B
@@ -111,14 +118,20 @@
             C_vec.uncert,
             np.array([
                 np.sqrt((1 * 2.6)**2 + (1 * 53.9)**2),
                 np.sqrt((1 * 5.4)**2 + (1 * 24.75)**2),
                 np.sqrt((1 * 10.56)**2 + (1 * 6.4)**2),
             ]))
 
+        A = variable(7, '%', 0.1)
+        B = 1 - A
+        self.assertAlmostEqual(B.value, -6)
+        self.assertEqual(B.unit, '%')
+        self.assertEqual(B.uncert, 0.1)
+
     def test_add_with_different_units(self):
         A = variable(12.3, 'm3/s', uncert=2.6)
         B = variable(745.1, 'L/min', uncert=53.9)
         C = A + B
         self.assertAlmostEqual(C.value, 12.3 + 745.1 / 1000 / 60)
         self.assertEqual(C.unit, 'm3/s')
         self.assertAlmostEqual(C.uncert, np.sqrt(2.6**2 + (53.9 / 1000 / 60)**2))
```

### Comparing `pyees-1.2.8/pyees/unit.py` & `pyees-1.2.9/pyees/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1138,7 +1138,16 @@
         # create the unit string
         self.unitStr = self._createUnitString()
 
         self._SIBaseUnit = self._getSIBaseUnit(self.upper, self.upperExp, self.lower, self.lowerExp)
         otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(self._SIBaseUnit)
         self._converterToSI = self._getConverter(otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp)
 
+
+
+
+if __name__ == "__main__":
+    a = unit('%')
+    b = unit('%')
+    
+    c = a + b
+    print(c)
```

### Comparing `pyees-1.2.8/pyees/variable.py` & `pyees-1.2.9/pyees/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,14 @@
     def __add__(self, other):
         
         if not isinstance(other, scalarVariable):
             return self + variable(other, self.unit)
 
         # determine if the two variable can be added
         isLogarithmicUnit, outputUnit, scaleToSI, scaleSelf, scaleOther = self._unitObject + other._unitObject
-
         if isLogarithmicUnit:
             return logarithmicVariables.__add__(self, other)
 
         # convert self and other to the SI unit system
         selfUnit = copy(self.unit)
         otherUnit = copy(other.unit)
         
@@ -342,15 +341,14 @@
 
     def __sub__(self, other):
         if not isinstance(other, scalarVariable):
             return self - variable(other, self.unit)
 
         # determine if the variables can be subtracted
         isLogarithmicUnit, outputUnit, scaleToSI, scaleSelf, scaleOther = self._unitObject - other._unitObject
-
         if isLogarithmicUnit:
             return logarithmicVariables.__sub__(self, other)
 
         # convert self and other to the SI unit system
         selfUnit = copy(self.unit)
         otherUnit = copy(other.unit)
  
@@ -483,15 +481,17 @@
 
         if var._unitObject._SIBaseUnit == '1' and var._unitObject != '1':
             var.convert('1')
 
         return var
 
     def __neg__(self):
-        return -1 * self
+        out = -1 * self
+        out.convert(self.unit)
+        return out
 
     def log(self):
         if self.unit != '1':
             raise ValueError('You can only take the natural log of a variable if it has no unit')
 
         val = np.log(self.value)
 
@@ -1002,11 +1002,10 @@
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
 
 
 if __name__ == "__main__":
-    diameter = variable(40, 'cm')
-    area = np.pi / 4 * diameter ** 2
-    
-    print(area.value)
+    A = variable(7, '%', 0.1)
+    B = -A
+    print(B)
```

### Comparing `pyees-1.2.8/pyees.egg-info/PKG-INFO` & `pyees-1.2.9/pyees.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.2.8
+Version: 1.2.9
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.2.8/setup.py` & `pyees-1.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.2.8',
+    version='1.2.9',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

