# Comparing `tmp/pyequations-0.1.3.tar.gz` & `tmp/pyequations-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyequations-0.1.3.tar", max compression
+gzip compressed data, was "pyequations-0.1.4.tar", max compression
```

## Comparing `pyequations-0.1.3.tar` & `pyequations-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-05-29 01:58:26.642083 pyequations-0.1.3/LICENSE
--rw-r--r--   0        0        0    12419 2023-06-11 22:14:30.784358 pyequations-0.1.3/README.md
--rw-r--r--   0        0        0      426 2023-06-11 22:26:08.185092 pyequations-0.1.3/pyequations/__init__.py
--rw-r--r--   0        0        0     6303 2023-06-10 18:08:24.869111 pyequations-0.1.3/pyequations/context_stack.py
--rw-r--r--   0        0        0      471 2023-05-31 00:06:36.282730 pyequations-0.1.3/pyequations/decorators.py
--rw-r--r--   0        0        0     9349 2023-06-10 18:08:24.869275 pyequations-0.1.3/pyequations/generate_units_subs.py
--rw-r--r--   0        0        0    24128 2023-06-10 20:37:48.132386 pyequations-0.1.3/pyequations/inheritables.py
--rw-r--r--   0        0        0     9294 2023-06-10 18:08:24.869792 pyequations-0.1.3/pyequations/utils.py
--rw-r--r--   0        0        0      538 2023-06-11 22:26:08.181772 pyequations-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    13011 1970-01-01 00:00:00.000000 pyequations-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 01:58:26.642083 pyequations-0.1.4/LICENSE
+-rw-r--r--   0        0        0    12659 2023-06-14 22:14:50.088264 pyequations-0.1.4/README.md
+-rw-r--r--   0        0        0      426 2023-06-14 22:14:50.114267 pyequations-0.1.4/pyequations/__init__.py
+-rw-r--r--   0        0        0     6303 2023-06-10 18:08:24.869111 pyequations-0.1.4/pyequations/context_stack.py
+-rw-r--r--   0        0        0      471 2023-05-31 00:06:36.282730 pyequations-0.1.4/pyequations/decorators.py
+-rw-r--r--   0        0        0     9349 2023-06-10 18:08:24.869275 pyequations-0.1.4/pyequations/generate_units_subs.py
+-rw-r--r--   0        0        0    24128 2023-06-10 20:37:48.132386 pyequations-0.1.4/pyequations/inheritables.py
+-rw-r--r--   0        0        0     9294 2023-06-10 18:08:24.869792 pyequations-0.1.4/pyequations/utils.py
+-rw-r--r--   0        0        0      538 2023-06-14 22:14:50.110671 pyequations-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    13251 1970-01-01 00:00:00.000000 pyequations-0.1.4/PKG-INFO
```

### Comparing `pyequations-0.1.3/LICENSE` & `pyequations-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.3/README.md` & `pyequations-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 After how long does the ball hit the ground and with what velocity?
 
 This is a simple problem if one has studied physics. Everything can be solved for using the kinematic equations (of constant acceleration):
 
 
 $$ v_f = v_0 + at $$
 
-$$ x_f = x_0 + v_0 + \frac{1}{2}at^2 $$
+$$ x_f = x_0 + v_0t + \frac{1}{2}at^2 $$
 
 $$ v_f^2 = v_0^2 + 2a(x_f - x_0) $$
 
 $$ x_f = x_0 + \frac{1}{2}(v_0 + v_f)t $$
 
 
 Let's demonstrate how to solve this problem with PyEquations.
@@ -75,15 +75,15 @@
     @eq
     def calc_v_f(self):
         # v_f = v_0 + at
         return self.v_f, self.v_0 + self.a * self.t
 
     @eq
     def calc_x_f(self):
-        # x_f = x_0 + v_0 + 0.5at^2
+        # x_f = x_0 + v_0t + 0.5at^2
         return self.x_f, self.x_0 + self.v_0 * self.t + 0.5 * self.a * self.t ** 2
 
     @eq
     def calc_v_f_2(self):
         # v_f^2 = v_0^2 + 2a(x_f - x_0)
         return self.v_f ** 2, self.v_0 ** 2 + 2 * self.a * (self.x_f - self.x_0)
 
@@ -370,14 +370,18 @@
   * Used in `@func` decorated methods
 * `var_description(self, name: str) -> str` 
   * Used for getting the description of a variable
 * `get_var_vals(self, name: str) -> list`
   * Used for getting the values of a variable spanning all branches
 * `get_var_vals_decimal(self, name: str) -> list`
   * Used for getting the decimal values of a variable spanning all branches
+* `solved(*variables) -> bool`
+  * Used for checking if all the provided variables has been solved
+  * Example usage: `solved(self.x, self.y, self.z)` would return `True` if all three variables have been solved in the 
+    current branch
 
 
 ## Additional Notes
 
 * Systems can only be solved once
   * A given object that inherits from PyEquations can only be solved once
   * This is to avoid manually setting values resulting in invalid states
```

### Comparing `pyequations-0.1.3/pyequations/context_stack.py` & `pyequations-0.1.4/pyequations/context_stack.py`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.3/pyequations/generate_units_subs.py` & `pyequations-0.1.4/pyequations/generate_units_subs.py`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.3/pyequations/inheritables.py` & `pyequations-0.1.4/pyequations/inheritables.py`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.3/pyequations/utils.py` & `pyequations-0.1.4/pyequations/utils.py`

 * *Files identical despite different names*

### Comparing `pyequations-0.1.3/pyproject.toml` & `pyequations-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyequations"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Python package for solving a bunch of equations with a bunch of unknowns."
 authors = ["Michael Bryant <mbryant2025@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/mbryant2025/PyEquations"
 keywords = ["Math"]
 
 [tool.poetry.dependencies]
```

### Comparing `pyequations-0.1.3/PKG-INFO` & `pyequations-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyequations
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python package for solving a bunch of equations with a bunch of unknowns.
 Home-page: https://github.com/mbryant2025/PyEquations
 Keywords: Math
 Author: Michael Bryant
 Author-email: mbryant2025@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -53,15 +53,15 @@
 After how long does the ball hit the ground and with what velocity?
 
 This is a simple problem if one has studied physics. Everything can be solved for using the kinematic equations (of constant acceleration):
 
 
 $$ v_f = v_0 + at $$
 
-$$ x_f = x_0 + v_0 + \frac{1}{2}at^2 $$
+$$ x_f = x_0 + v_0t + \frac{1}{2}at^2 $$
 
 $$ v_f^2 = v_0^2 + 2a(x_f - x_0) $$
 
 $$ x_f = x_0 + \frac{1}{2}(v_0 + v_f)t $$
 
 
 Let's demonstrate how to solve this problem with PyEquations.
@@ -91,15 +91,15 @@
     @eq
     def calc_v_f(self):
         # v_f = v_0 + at
         return self.v_f, self.v_0 + self.a * self.t
 
     @eq
     def calc_x_f(self):
-        # x_f = x_0 + v_0 + 0.5at^2
+        # x_f = x_0 + v_0t + 0.5at^2
         return self.x_f, self.x_0 + self.v_0 * self.t + 0.5 * self.a * self.t ** 2
 
     @eq
     def calc_v_f_2(self):
         # v_f^2 = v_0^2 + 2a(x_f - x_0)
         return self.v_f ** 2, self.v_0 ** 2 + 2 * self.a * (self.x_f - self.x_0)
 
@@ -386,14 +386,18 @@
   * Used in `@func` decorated methods
 * `var_description(self, name: str) -> str` 
   * Used for getting the description of a variable
 * `get_var_vals(self, name: str) -> list`
   * Used for getting the values of a variable spanning all branches
 * `get_var_vals_decimal(self, name: str) -> list`
   * Used for getting the decimal values of a variable spanning all branches
+* `solved(*variables) -> bool`
+  * Used for checking if all the provided variables has been solved
+  * Example usage: `solved(self.x, self.y, self.z)` would return `True` if all three variables have been solved in the 
+    current branch
 
 
 ## Additional Notes
 
 * Systems can only be solved once
   * A given object that inherits from PyEquations can only be solved once
   * This is to avoid manually setting values resulting in invalid states
```

