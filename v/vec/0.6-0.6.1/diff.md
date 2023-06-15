# Comparing `tmp/vec-0.6.tar.gz` & `tmp/vec-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vec-0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vec-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vec-0.6.tar` & `vec-0.6.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       38 2023-06-14 23:00:47.631077 vec-0.6/.gitignore
--rw-r--r--   0        0        0     1508 2023-06-14 09:50:20.639282 vec-0.6/LICENSE
--rw-r--r--   0        0        0    12444 2023-06-14 23:23:14.082858 vec-0.6/README.md
--rw-r--r--   0        0        0      433 2023-06-13 18:12:35.372308 vec-0.6/pyproject.toml
--rw-r--r--   0        0        0    30480 2023-06-14 23:21:59.014201 vec-0.6/tests/test_all.py
--rw-r--r--   0        0        0    34167 2023-06-14 23:16:15.471195 vec-0.6/vec/__init__.py
--rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 vec-0.6/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-06-14 23:00:47.631077 vec-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1508 2023-06-14 09:50:20.639282 vec-0.6.1/LICENSE
+-rw-r--r--   0        0        0    12926 2023-06-15 03:19:42.417410 vec-0.6.1/README.md
+-rw-r--r--   0        0        0      433 2023-06-13 18:12:35.372308 vec-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    34364 2023-06-15 03:14:50.942899 vec-0.6.1/tests/test_all.py
+-rw-r--r--   0        0        0    39707 2023-06-15 03:18:19.040692 vec-0.6.1/vec/__init__.py
+-rw-r--r--   0        0        0    13358 1970-01-01 00:00:00.000000 vec-0.6.1/PKG-INFO
```

### Comparing `vec-0.6/LICENSE` & `vec-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vec-0.6/README.md` & `vec-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: vec
+Version: 0.6.1
+Summary: A 2-dimensional vector class designed to be convenient
+Home-page: https://github.com/larryhastings/vec/
+Author: Larry Hastings
+Author-email: larry@hastings.org
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3 :: Only
+
 # vec
 
 ## A reasonable, performant 2D vector object for games
 
 ##### Copyright 2019-2023 by Larry Hastings
 
 ## Overview
@@ -66,14 +79,16 @@
 to create one.  Discrete parameters,
 iterables, and objects that support `x` and `y` attributes all work fine:
 
     vec.Vector2(0, 1)
     vec.Vector2(x=0, y=1)
     vec.Vector2((0, 1))
     vec.Vector2([0, 1])
+    vec.Vector2(iter([0, 1]))
+    vec.Vector2({'x':0, 'y':1})
     vec.Vector2(types.SimpleNamespace(x=0, y=1))
 
 All these define the same vector.  That last example is there to demonstrate
 that `vec.Vector2` can create a vector based on any object with `x` and `y`
 attributes.
 
 Once you have a vector object, you can examine its attributes.
@@ -282,15 +297,26 @@
 
 Note that the types you extend `vec` with in this manner
 should behave like numeric types, like `int` and `float`.
 
 
 ## Changelog
 
-**0.6** *2023/06/4*
+**0.6.1** *2023/06/14*
+
+* Enhanced the `Vector2` constructor: now it also accepts
+  mappings.  The mapping must have exactly two elements,
+  `x` and `y`.
+* Enhanced `Vector2.from_polar`.  It now accepts all the same
+  stuff as the `Vector2` constructor: `Vector2` objects,
+  namespaces, mappings, and iterables.  Where it examines
+  names (attributes, keys) it naturally uses `r` and `theta`
+  instead of `x` and `y`.
+
+**0.6** *2023/06/14*
 
 A major improvement!
 
 * `vec` now has a proper test suite.
 * `vec` now passes its test suite with 100% coverage.
 * `vec` explicitly supports Python 3.6+.
 * Added more shortcut optimizations, e.g. rotating a cartesian vector by a multiple of `pi/2`.
@@ -307,7 +333,8 @@
 
 * Bugfix: `vec.Vector2.dot()` was simply wrong, it was adding where it should
   have been multiplying.  Fixes #3.
 
 **0.5** *2021/03/21*
 
 Initial version.
+
```

### Comparing `vec-0.6/tests/test_all.py` & `vec-0.6.1/tests/test_all.py`

 * *Files 10% similar despite different names*

```diff
@@ -261,14 +261,18 @@
             with self.assertRaises(ValueError):
                 Vector2(**kwargs)
 
         def raises_type(**kwargs):
             with self.assertRaises(TypeError):
                 Vector2(**kwargs)
 
+        def raises_key(**kwargs):
+            with self.assertRaises(KeyError):
+                Vector2(**kwargs)
+
         equal = self.assertEqual
 
         #
         # x is a Vector2
         #
 
         # nothing else should be set
@@ -292,33 +296,59 @@
         raises_value(x=namespace, theta=5)
         raises_value(x=namespace, r_squared=5)
 
         # passes
         equal(Vector2(namespace), Vector2(3, 4))
 
         #
+        # x has a '__getitem__'
+        d = {'x': 33, 'y': 44}
+        equal(Vector2(d), Vector2(33, 44))
+        raises_key(x={1: 'b', 2: 'd'})
+        raises_value(x={'x': 33, 'y': 45, 'z': 22})
+        raises_value(x=d, y=45)
+        raises_value(x=d, r=22)
+        raises_value(x=d, theta=pi)
+        raises_value(x=d, r_squared=16)
+
+
+        #
         # x has an '__iter__'
         #
 
-        # must not be a set or dict
+        # must not be a set
         raises_type(x={1, 2})
-        raises_type(x={1: 'b', 2: 'd'})
 
         # nothing else should be set
         t4_5 = (4, 5)
         raises_value(x=t4_5, y=5)
         raises_value(x=t4_5, r=5)
         raises_value(x=t4_5, theta=5)
         raises_value(x=t4_5, r_squared=5)
         l6_7 = [6, 7]
         raises_value(x=l6_7, y=5)
         raises_value(x=l6_7, r=5)
         raises_value(x=l6_7, theta=5)
         raises_value(x=l6_7, r_squared=5)
 
+        i = iter([6, 7])
+        equal(Vector2(i), Vector2(6, 7))
+        i = iter([6, 7])
+        raises_value(x=i, y=5)
+        i = iter([6, 7])
+        raises_value(x=i, r=5)
+        i = iter([6, 7])
+        raises_value(x=i, theta=5)
+        i = iter([6, 7])
+        raises_value(x=i, r_squared=5)
+        i = iter([6, ])
+        raises_value(x=i)
+        i = iter([6, 7, 8])
+        raises_value(x=i)
+
         # must contain exactly two items
         raises_value(x=tuple())
         raises_value(x=[])
         raises_value(x=(1,))
         raises_value(x=[1,])
         raises_value(x=(1, 2, 3))
         raises_value(x=[1, 2, 3])
@@ -396,17 +426,90 @@
         # r and theta both set, r is not 0
         raises_value(theta=pi, r=1, r_squared=0)
 
 
     def test_from_polar(self):
         self.assertIs(Vector2.from_polar(0, None), vector2_zero)
 
-        for theta in (0, pi/3, pi/2, pi, 4*pi/3):
-            for r in range(1, 5):
-                self.assertEqual(Vector2.from_polar(r, theta), Vector2(r=r, theta=theta))
+        self.assertEqual(Vector2.from_polar(1, 0), Vector2(r=1, theta=0))
+        self.assertEqual(Vector2.from_polar(1, pi/3), Vector2(r=1, theta=pi/3))
+        self.assertEqual(Vector2.from_polar(1, pi/2), Vector2(r=1, theta=pi/2))
+        self.assertEqual(Vector2.from_polar(1, pi), Vector2(r=1, theta=pi))
+
+        self.assertEqual(Vector2.from_polar(2, 0), Vector2(r=2, theta=0))
+        self.assertEqual(Vector2.from_polar(2, pi/3), Vector2(r=2, theta=pi/3))
+        self.assertEqual(Vector2.from_polar(2, pi/2), Vector2(r=2, theta=pi/2))
+        self.assertEqual(Vector2.from_polar(2, pi), Vector2(r=2, theta=pi))
+
+        with self.assertRaises(TypeError):
+            Vector2.from_polar(3)
+        with self.assertRaises(TypeError):
+            Vector2.from_polar(3, None)
+        with self.assertRaises(TypeError):
+            Vector2.from_polar(0, 0)
+        with self.assertRaises(TypeError):
+            Vector2.from_polar(1+2j, 5)
+        with self.assertRaises(TypeError):
+            Vector2.from_polar(1, 5+2j)
+
+        v1 = Vector2(1, 3)
+        self.assertIs(Vector2.from_polar(v1), v1)
+        with self.assertRaises(ValueError):
+            Vector2.from_polar(v1, theta=5)
+
+        namespace = types.SimpleNamespace(r=1, theta=pi)
+        self.assertEqual(Vector2.from_polar(namespace), Vector2(r=1, theta=pi))
+        with self.assertRaises(ValueError):
+            Vector2.from_polar(namespace, theta=2)
+
+        d = {'r':1, 'theta':pi}
+        self.assertEqual(Vector2.from_polar(d), Vector2(r=1, theta=pi))
+        with self.assertRaises(ValueError):
+            Vector2.from_polar(d, theta=2)
+        with self.assertRaises(KeyError):
+            Vector2.from_polar({1:2, 3:4})
+        d['funk'] = 'town'
+        with self.assertRaises(ValueError):
+            Vector2.from_polar(d)
+
+        iterable = [1, pi]
+        self.assertEqual(Vector2.from_polar(iterable), Vector2(r=1, theta=pi))
+        with self.assertRaises(ValueError):
+            Vector2.from_polar(iterable, theta=2)
+        with self.assertRaises(ValueError):
+            Vector2.from_polar([1])
+        with self.assertRaises(ValueError):
+            Vector2.from_polar([1, pi, 5])
+
+        iterable = (1, pi)
+        self.assertEqual(Vector2.from_polar(iterable), Vector2(r=1, theta=pi))
+        with self.assertRaises(ValueError):
+            Vector2.from_polar(iterable, theta=2)
+        with self.assertRaises(ValueError):
+            Vector2.from_polar((1,))
+        with self.assertRaises(ValueError):
+            Vector2.from_polar((1, pi, 5))
+
+        s = set((1, pi))
+        with self.assertRaises(TypeError):
+            Vector2.from_polar(s)
+
+        i = iter((1, pi))
+        self.assertEqual(Vector2.from_polar(i), Vector2(r=1, theta=pi))
+        i = iter((1, pi))
+        with self.assertRaises(ValueError):
+            Vector2.from_polar(i, theta=2)
+        i = iter((1, pi, 55))
+        with self.assertRaises(ValueError):
+            Vector2.from_polar(i)
+
+
+        self.assertEqual(Vector2.from_polar({'r': 33, 'theta': 55}), Vector2(r=33, theta=55))
+
+
 
     def test_vector_math(self):
         def base_test(v, x, y, r_squared, theta):
             r = sqrt(r_squared)
 
             self.assertAlmostEqual(v.x, x, places=places)
             self.assertAlmostEqual(v.y, y, places=places)
@@ -446,15 +549,21 @@
         self.assertEqual(vec.normalize_angle(-pi), -pi)
         self.assertEqual(vec.normalize_angle(-2 * pi), 0)
         self.assertEqual(vec.normalize_angle(2 * pi), 0)
 
         self.assertEqual(vec.normalize_polar(3, pi/2), (3, pi/2))
         self.assertEqual(vec.normalize_polar(-3, pi/2), (3, -pi/2))
 
-        self.assertEqual(vec.normalize_polar(0, pi/2), (0, None))
+        self.assertEqual(vec.normalize_polar(0, None), (0, None))
+
+        with self.assertRaises(TypeError):
+            vec.normalize_polar(3, None)
+
+        with self.assertRaises(TypeError):
+            vec.normalize_polar(0, pi)
 
     def test_repr(self):
         def test(s, **kwargs):
             v = Vector2(**kwargs)
             self.assertEqual(s, repr(v))
 
         test("Vector2(1, 5)", x=(1, 5))
```

### Comparing `vec-0.6/vec/__init__.py` & `vec-0.6.1/vec/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -34,28 +34,30 @@
 #                  * return vector2_zero
 #                  * raise ValueError with this message
 #                  * raise TypeError with this message
 #        * compute table by splitting off the nest of boolean logic
 #          into its own function, driving it with every value,
 #          and observing what it does
 #        * rewrite exception messages to need .format
+#   * Vector2 constructor: allow reading 'r', 'theta', and 'r_squared'
+#     from namespaces and mappings.  still be strict about it for mappings.
 #
 #   * Rect2
 #   * Vector3
 #   * rewrite as C extension for speedy speeds
 
 """
 A 2-dimensional vector class designed to be convenient
 and performant enough for use in video games.
 """
 
 from math import acos, atan2, cos, pi, sin, sqrt, tau
 from collections.abc import Iterable, Set, Mapping
 
-__version__ = "0.6"
+__version__ = "0.6.1"
 
 
 pi_over_two = pi/2
 negative_pi = -pi
 negative_pi_over_two = -pi_over_two
 
 
@@ -68,26 +70,30 @@
     """
     while theta >= pi:
         theta -= tau
     while theta < negative_pi:
         theta += tau
     return theta
 
+def negate_angle(theta):
+    return normalize_angle(theta - pi)
 
 def normalize_polar(r, theta):
     if r == 0:
-        return 0, None
+        if theta is not None:
+            raise TypeError(f"normalize_polar: theta is {theta}, must be None when r is 0")
+        return (0, None)
+
+    if theta is None:
+        raise TypeError(f"normalize_polar: theta is None, can't be None when r is {r}")
     if r < 0:
         r = -r
         theta = theta - pi
     return r, normalize_angle(theta)
 
-def negate_angle(theta):
-    return normalize_angle(theta + pi)
-
 #
 # All these return vector2_zero:
 #   Vector2()
 #   Vector2(None, None)
 #   Vector2(None)
 #   Vector2(0, 0)
 #   Vector2((0, 0))
@@ -99,15 +105,16 @@
 #   Vector2(any_vector2_object_that_isnt_0_0)
 #   Vector2((1, 2))
 #   Vector2([1, 2])
 #   Vector2(types.SimpleNamespace(x=1, y=2))
 #   Vector2(r=1, theta=math.pi/2)
 #
 
-_invalid_types_for_iterable_x = (Set, Mapping)
+# we check mappings separately
+_invalid_types_for_iterable = (Set, Mapping)
 permitted_coordinate_types = ()
 
 def permit_coordinate_type(t):
     global permitted_coordinate_types
     permitted_coordinate_types = permitted_coordinate_types + (t,)
 
 permit_coordinate_type(int)
@@ -134,46 +141,14 @@
         # may specify any additional arguments you like.
         #
         # print(f"Vector2Metaclass(self={self}, x={x}, y={y}, r={r}, theta={theta}, r_squared={r_squared})")
 
         x_source = "x"
         y_source = "y"
 
-        if x is not _sentinel:
-            # handle x if it's a special object
-            if isinstance(x, Vector2):
-                if (y is not _sentinel) or (r is not _sentinel) or (theta is not _sentinel) or (r_squared is not _sentinel):
-                    raise ValueError(f"{self.__name__}: when x is an object, you must not specify y, r, or theta")
-                return x
-            elif (hasattr(x, 'x') and hasattr(x, 'y')):
-                if (y is not _sentinel) or (r is not _sentinel) or (theta is not _sentinel) or (r_squared is not _sentinel):
-                    raise ValueError(f"{self.__name__}: when x is an object, you must not specify y, r, or theta")
-                x_source = "x.x"
-                y_source = "x.y"
-                y = x.y
-                x = x.x
-            elif hasattr(x, "__iter__"):
-                if isinstance(x, _invalid_types_for_iterable_x):
-                    raise TypeError(f"{self.__name__}: if x is an iterable, it must be ordered, not {x.__class__.__name__}")
-                if (y is not _sentinel) or (r is not _sentinel) or (theta is not _sentinel) or (r_squared is not _sentinel):
-                    raise ValueError(f"{self.__name__}: when x is an object, you must not specify y, r, or theta")
-                i = iter(x)
-                x_source = "x[0]"
-                y_source = "x[1]"
-                try:
-                    x = next(i)
-                    y = next(i)
-                except StopIteration:
-                    raise ValueError(f"{self.__name__}: if x is an iterable, it must contain exactly 2 items")
-                try:
-                    next(i)
-                    raise ValueError(f"{self.__name__}: if x is an iterable, it must contain exactly 2 items")
-                except StopIteration:
-                    pass
-
         x_is_not_set = x is _sentinel
         x_is_set = not x_is_not_set
 
         y_is_not_set = y is _sentinel
         y_is_set = not y_is_not_set
 
         x_and_y = x_is_set and y_is_set
@@ -186,14 +161,81 @@
         theta_is_set = not theta_is_not_set
 
         r_and_theta = r_is_set and theta_is_set
         not_r_or_theta = r_is_not_set and theta_is_not_set
 
         r_squared_is_set = r_squared is not _sentinel
 
+        if x_is_set and (not isinstance(x, permitted_coordinate_types)):
+            # handle x if it's a special object
+            something_besides_x_is_set = y_is_set or r_is_set or theta_is_set or r_squared_is_set
+            if isinstance(x, Vector2):
+                if something_besides_x_is_set:
+                    raise ValueError(f"{self.__name__}: when x is an object, you must not specify y, r, or theta")
+                return x
+            # the while loop is here just so we can early-exit break out of processing.
+            # we never actually loop.
+            while True:
+                if hasattr(x, 'x') and hasattr(x, 'y'):
+                    if something_besides_x_is_set:
+                        raise ValueError(f"{self.__name__}: when x is an object, you must not specify y, r, or theta")
+                    x_source = "x.x"
+                    y_source = "x.y"
+                    y = x.y
+                    x = x.x
+                    not_x_or_y = y_is_not_set = False
+                    x_and_y = y_is_set = True
+                    x_is_set and y_is_set
+                    break
+
+                if hasattr(x, "__getitem__"):
+                    if something_besides_x_is_set:
+                        raise ValueError(f"{self.__name__}: when x is an object, you must not specify y, r, or theta")
+                    try:
+                        maybe_x = x['x']
+                        y = x['y']
+                        x_source = "x['x']"
+                        y_source = "x['y']"
+                        if len(x) != 2:
+                            raise ValueError(f"{self.__name__}: if x is a mapping, it must contain exactly 2 items")
+                        x = maybe_x
+                        not_x_or_y = y_is_not_set = False
+                        x_and_y = y_is_set = True
+                        x_is_set and y_is_set
+                        break
+                    except KeyError:
+                        raise KeyError(f"{self.__name__}: if x is an mapping, it must contain elements 'x' and 'y'") from None
+                    except TypeError:
+                        pass
+
+                if hasattr(x, "__iter__"):
+                    if isinstance(x, _invalid_types_for_iterable):
+                        raise TypeError(f"{self.__name__}: if x is an iterable, it must be ordered, not {x.__class__.__name__}")
+                    if something_besides_x_is_set:
+                        raise ValueError(f"{self.__name__}: when x is an object, you must not specify y, r, or theta")
+                    i = iter(x)
+                    x_source = "x[0]"
+                    y_source = "x[1]"
+                    try:
+                        x = next(i)
+                        y = next(i)
+                    except StopIteration:
+                        raise ValueError(f"{self.__name__}: if x is an iterable, it must contain exactly 2 items")
+                    try:
+                        next(i)
+                        raise ValueError(f"{self.__name__}: if x is an iterable, it must contain exactly 2 items")
+                    except StopIteration:
+                        pass
+                    not_x_or_y = y_is_not_set = False
+                    x_and_y = y_is_set = True
+                    x_is_set and y_is_set
+                    break
+
+                break
+
 
         if not_x_or_y and not_r_or_theta:
             return vector2_zero
 
         if not_r_or_theta:
             # neither r nor theta is set.
             # either x or y must be set.
@@ -231,20 +273,15 @@
                 if not isinstance(theta, permitted_coordinate_types):
                     raise TypeError(f"{self.__name__}: theta must be int or float, not {theta}")
                 if r_is_set and (not r):
                     raise TypeError(f"{self.__name__}: theta is {theta}, must be None when r is 0")
                 theta = normalize_angle(theta)
 
         if r_is_set and theta_is_set:
-            # normalize r
-            if r < 0:
-                r = -r
-                args['r'] = r
-                theta = negate_angle(theta)
-
+            r, theta = normalize_polar(r, theta)
             args['r'] = r
             args['theta'] = theta
         elif r_is_set:
             if r < 0:
                 raise ValueError(f"{self.__name__}: can't specify r < 0 if you don't specify theta")
             args['r'] = r
         else:
@@ -367,15 +404,91 @@
             except AttributeError:
                 pass
 
         text = ", ".join(fields)
         return f"{self.__class__.__name__}({text})"
 
     @classmethod
-    def from_polar(cls, r, theta):
+    def from_polar(cls, r, theta=_sentinel):
+        theta_is_not_set = theta is _sentinel
+        theta_is_set = not theta_is_not_set
+
+        r_source = "r"
+        theta_source = "theta"
+        if isinstance(r, permitted_coordinate_types):
+            if theta_is_not_set:
+                raise TypeError(f"{cls.__name__}() missing 1 required positional argument: 'theta'")
+        else:
+            if isinstance(r, Vector2):
+                if theta_is_set:
+                    raise ValueError(f"{cls.__name__}.from_polar: when r is an object, you must not specify theta")
+                return r
+            while True:
+                if hasattr(r, 'r') and hasattr(r, 'theta'):
+                    if theta_is_set:
+                        raise ValueError(f"{cls.__name__}.from_polar: when r is an object, you must not specify theta")
+                    r_source = "r.r"
+                    theta_source = "r.theta"
+                    theta = r.theta
+                    r = r.r
+                    break
+                if hasattr(r, "__getitem__"):
+                    if theta_is_set:
+                        raise ValueError(f"{cls.__name__}.from_polar: when r is an object, you must not specify theta")
+                    try:
+                        maybe_r = r['r']
+                        theta = r['theta']
+                        r_source = "r['r']"
+                        theta_source = "r['theta']"
+                        if len(r) != 2:
+                            raise ValueError(f"{cls.__name__}: if r is a mapping, it must contain exactly 2 items")
+                        r = maybe_r
+                        break
+                    except KeyError:
+                        raise KeyError(f"{cls.__name__}: if r is an mapping, it must contain elements 'r' and 'theta'") from None
+                    except TypeError:
+                        pass
+
+                if hasattr(r, "__iter__"):
+                    if isinstance(r, _invalid_types_for_iterable):
+                        raise TypeError(f"{cls.__name__}.from_polar: if r is an iterable, it must be ordered, not {r.__class__.__name__}")
+                    if theta_is_set:
+                        raise ValueError(f"{cls.__name__}.from_polar: when r is an object, you must not specify theta")
+                    i = iter(r)
+                    r_source = "r[0]"
+                    theta_source = "r[1]"
+                    try:
+                        r = next(i)
+                        theta = next(i)
+                    except StopIteration:
+                        raise ValueError(f"{cls.__name__}.from_polar: if r is an iterable, it must contain exactly 2 items")
+                    try:
+                        next(i)
+                        raise ValueError(f"{cls.__name__}.from_polar: if r is an iterable, it must contain exactly 2 items")
+                    except StopIteration:
+                        pass
+                    break
+                break
+
+        if not isinstance(r, permitted_coordinate_types):
+            raise TypeError(f"{cls.__name__}.from_polar: {r_source} must be int or float, not {r}")
+
+        if theta is None:
+            if r:
+                raise TypeError(f"{cls.__name__}.from_polar: {theta_source} is {theta}, must not be None when {r_source} != 0")
+            return vector2_zero
+
+        if not isinstance(theta, permitted_coordinate_types):
+            raise TypeError(f"{cls.__name__}.from_polar: {theta_source} must be int, float, or None, not {theta}")
+        # we already know theta is not None
+        if not r:
+            raise TypeError(f"{cls.__name__}.from_polar: {theta_source} is {theta}, must be None when {r_source}=0")
+
+        r, theta = normalize_polar(r, theta)
+
         return cls(r=r, theta=theta)
 
     def polar(self):
         return (self.r, self.theta)
 
     ##
     ## descriptor protocol
```

### Comparing `vec-0.6/PKG-INFO` & `vec-0.6.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: vec
-Version: 0.6
-Summary: A 2-dimensional vector class designed to be convenient
-Home-page: https://github.com/larryhastings/vec/
-Author: Larry Hastings
-Author-email: larry@hastings.org
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3 :: Only
-
 # vec
 
 ## A reasonable, performant 2D vector object for games
 
 ##### Copyright 2019-2023 by Larry Hastings
 
 ## Overview
@@ -79,14 +66,16 @@
 to create one.  Discrete parameters,
 iterables, and objects that support `x` and `y` attributes all work fine:
 
     vec.Vector2(0, 1)
     vec.Vector2(x=0, y=1)
     vec.Vector2((0, 1))
     vec.Vector2([0, 1])
+    vec.Vector2(iter([0, 1]))
+    vec.Vector2({'x':0, 'y':1})
     vec.Vector2(types.SimpleNamespace(x=0, y=1))
 
 All these define the same vector.  That last example is there to demonstrate
 that `vec.Vector2` can create a vector based on any object with `x` and `y`
 attributes.
 
 Once you have a vector object, you can examine its attributes.
@@ -295,15 +284,26 @@
 
 Note that the types you extend `vec` with in this manner
 should behave like numeric types, like `int` and `float`.
 
 
 ## Changelog
 
-**0.6** *2023/06/4*
+**0.6.1** *2023/06/14*
+
+* Enhanced the `Vector2` constructor: now it also accepts
+  mappings.  The mapping must have exactly two elements,
+  `x` and `y`.
+* Enhanced `Vector2.from_polar`.  It now accepts all the same
+  stuff as the `Vector2` constructor: `Vector2` objects,
+  namespaces, mappings, and iterables.  Where it examines
+  names (attributes, keys) it naturally uses `r` and `theta`
+  instead of `x` and `y`.
+
+**0.6** *2023/06/14*
 
 A major improvement!
 
 * `vec` now has a proper test suite.
 * `vec` now passes its test suite with 100% coverage.
 * `vec` explicitly supports Python 3.6+.
 * Added more shortcut optimizations, e.g. rotating a cartesian vector by a multiple of `pi/2`.
@@ -320,8 +320,7 @@
 
 * Bugfix: `vec.Vector2.dot()` was simply wrong, it was adding where it should
   have been multiplying.  Fixes #3.
 
 **0.5** *2021/03/21*
 
 Initial version.
-
```

