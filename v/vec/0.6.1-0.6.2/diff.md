# Comparing `tmp/vec-0.6.1.tar.gz` & `tmp/vec-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vec-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vec-0.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vec-0.6.1.tar` & `vec-0.6.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       38 2023-06-14 23:00:47.631077 vec-0.6.1/.gitignore
--rw-r--r--   0        0        0     1508 2023-06-14 09:50:20.639282 vec-0.6.1/LICENSE
--rw-r--r--   0        0        0    12926 2023-06-15 03:19:42.417410 vec-0.6.1/README.md
--rw-r--r--   0        0        0      433 2023-06-13 18:12:35.372308 vec-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    34364 2023-06-15 03:14:50.942899 vec-0.6.1/tests/test_all.py
--rw-r--r--   0        0        0    39707 2023-06-15 03:18:19.040692 vec-0.6.1/vec/__init__.py
--rw-r--r--   0        0        0    13358 1970-01-01 00:00:00.000000 vec-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-06-14 23:00:47.631077 vec-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1508 2023-06-14 09:50:20.639282 vec-0.6.2/LICENSE
+-rw-r--r--   0        0        0    14873 2023-06-15 05:23:06.185304 vec-0.6.2/README.md
+-rw-r--r--   0        0        0      433 2023-06-13 18:12:35.372308 vec-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    35442 2023-06-15 05:17:48.370558 vec-0.6.2/tests/test_all.py
+-rw-r--r--   0        0        0    40248 2023-06-15 05:26:54.547280 vec-0.6.2/vec/__init__.py
+-rw-r--r--   0        0        0    15305 1970-01-01 00:00:00.000000 vec-0.6.2/PKG-INFO
```

### Comparing `vec-0.6.1/LICENSE` & `vec-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vec-0.6.1/README.md` & `vec-0.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: vec
+Version: 0.6.2
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
@@ -12,14 +25,16 @@
 Features:
 
 * `Vector2` objects are immutable.
 * `Vector2` support all the usual features, including operator overloading.
 * Attributes of `Vector2` objects are lazily-computed where possible.
 * `Vector2` objects effortlessly support both cartesian and polar coordinates.
 
+`vec` supports Python 3.6+, and passes its unit test suite with 100% coverage.
+
 
 ## Why Another Vector Class?
 
 I've participated in three PyWeek gaming challenges.  In two of those three times,
 mid-week I wrote my own vector class out of sheer frustration.
 
 The biggest problem with most Python vector objects in is that they're mutable.
@@ -139,31 +154,41 @@
 *either* both `x` and `y` *or* both `r` and `theta`.
 Any attributes not passed in at construction time will be lazily
 computed at the time they are evaluated.
 
 You can also pass in a single object which will initialize the
 vector.  Supported objects include:
 
-* an existing `vec.Vector2` object (just returns that object)
-* an object which has `.x` and `.y` attributes
-* an ordered iterable object with exactly two elements
+* an existing `vec.Vector2` object (just returns that object),
+* an object which has `.x` and `.y` attributes,
+* a mapping object with exactly two keys, `'x'` and `'y'`, and
+* an ordered iterable object with exactly two elements.
 
 `vec.Vector2` only does *some* validation of its arguments.
 It ensures that `r` and `theta` are normalized.  However,
 it doesn't check that `(x, y)` and `(r, theta)` describe the
 same vector.
-If you pass in `x` and `y`, and a `theta` and `r` that don't
-match, you'll get back the `vec.Vector2` that you asked for.
-Good luck.
+If you pass in `x` and `y`, and also pass in a `theta` and `r`
+that don't match, you'll get back the `vec.Vector2` that you
+asked for.  Good luck!
+
+### Attributes
 
 `vec.Vector2` objects support five attributes:
-`x`, `y`, `r`, `theta`, and `r_squared`.  It doesn't matter whether
-the object was defined with cartesian or polar coordinates, they
-will all work.  `r_squared` is equivalent to `r*r` but it's much
+`x`, `y`, `r`, `theta`, and `r_squared`.  It doesn't matter
+whether the object was defined with cartesian or polar
+coordinates, they'll all work.
+
+`r_squared` is equivalent to `r*r`, but it's much
 cheaper to compute based on cartesian coordinates.
+There are a lot of use cases where `r_squared` works
+just as well as `r`, for example in collision detection
+in a game.
+
+### Operators and protocols
 
 `vec.Vector2` objects support the *iterator protocol.*
 `len()` on a `vec.Vector2` object will always return 2.
 You can also iterate over a `vec.Vector2` object,
 which will yield the `x` and `y` attributes in that order.
 
 `vec.Vector2` objects support the *sequence protocol.*  You can subscript
@@ -171,33 +196,68 @@
 2 containing the `x` and `y` attributes.
 
 `vec.Vector2` objects also support the *boolean* protocol; you may use them
 with boolean operators, and you may call `bool()` on them.  When used in
 a boolean context, the zero vector evaluates to `False`, and all other
 vectors evaluate to `True`.
 
-`vec.Vector2` objects are hashable.
+`vec.Vector2` objects are *hashable,* but they're not *ordered*.
+(You can't ask if one vector is *less than* another.)
 
 `vec.Vector2` objects support the following operators:
 
 * `v1 + v2` adds the two vectors together.
 * `v1 - v2` subtracts the right vector from the left vector.
 * `v1 * scalar` mulitplies the vector by a scalar amount, equivalent to `v1.scale(scalar)`.
 * `v1 / scalar` divides the vector by a scalar amount.
 * `+v1` is exactly the same as `v1`.
 * `-v1` returns the opposite of `v1`, such that `v1 + (-v1)` should be the zero vector.
    (This may not always be the case due to compounding floating-point errors.)
 * `v1 == v2` is `True` if the two vectors are *exactly* the same, and `False` otherwise.
+  For consistency, this only compares cartesian coordinates.
+  Note that floating-point imprecision may result in two vectors that *should* be the
+  same failing an `==` check.
 * `v1 != v2` is `False` if the two vectors are *exactly* the same, and `True` otherwise.
+  For consistency, this only compares cartesian coordinates.
+  Note that floating-point imprecision may result in two vectors that *should* be the
+  same passing an `!=` check.
 * `v[0] == v.x`
 * `v[1] == v.y`
 * `list(v) == [v.x, v.y]`
 
+### Class methods
+
+`vec.from_polar(r, theta)`
+
+Constructs a `vec.Vector2` object from the two polar coordinates
+`r` and `theta`.
+
+You can also pass in a single object which will be used to
+initialize the vector.  Supported objects include:
+
+* an existing `vec.Vector2` object (just returns that object),
+* an object which has `.r` and `.theta` attributes,
+* a mapping object with exactly two keys, `'r'` and `'theta'`, and
+* an ordered iterable object with exactly two elements.
+
+If `r` is `0`, `theta` must be `None`, and `from_polar` will
+return the zero vector.  If `r` is not `0`, `theta` must not
+be `None`.
+
+### Methods
+
 `vec.Vector2` objects support the following methods:
 
+`vec.Vector2.almost_equal(other, places)`
+
+Returns `True` if the vector and `other` are the same vector,
+down to `places` decimal places.  Like the `Vector2` class's
+support for the `==` operator, the comparison is only done
+using cartesian coordinates, for consistency.
+
 `vec.Vector2.scaled(scalar)`
 
 Returns a new `vec.Vector2` object, equivalent to the original vector multiplied by that scalar.
 
 `vec.Vector2.scaled_to_length(r)`
 
 Returns a new `vec.Vector2` object, equivalent to the original vector with its length set to `r`.
@@ -242,26 +302,30 @@
 
 `vec.Vector2.nlerp(other, ratio)`
 
 Returns a vector representing a normalized linear interpolation between `self` and `other`,
 according to the scalar ratio `ratio`.  `ratio` should be a value between (and including)
 `0` and `1`.  If `ratio` is `0`, this returns `self`.  If `ratio` is `1`, this returns `other`.
 
+### Constants
+
 `vec.vector2_zero`
 
 The immutable, eternal "zero" `vec.Vector2` vector object.
 `vec` guarantees that every zero vector is a reference to this object:
 
     >>> v = vec.Vector2(0, 0)
     >>> v is vec.vector2_zero
     True
 
 Mathematically-speaking, the zero vector when expressed in polar coordinates
 doesn't have a defined angle.  Therefore `vec` defines its zero vector as
-having an angle of `None`.
+having an angle of `None`.  The zero vector must have `r` set to zero
+and `theta` set to `None`, and any other vector must have a non-zero `r`
+and `theta` set to a value besides `None`.
 
 
 ## Extending vec to handle other types
 
 `vec` does some input verification on its inputs.
 Coordinates--`x`, `y`, `r`, `theta`--are required to be
 either `int` or `long`.
@@ -284,14 +348,19 @@
 
 Note that the types you extend `vec` with in this manner
 should behave like numeric types, like `int` and `float`.
 
 
 ## Changelog
 
+**0.6.2** *2023/06/14*
+
+* Added `Vector2.almost_equal`, which supports testing
+  for slightly-inexact equality.
+
 **0.6.1** *2023/06/14*
 
 * Enhanced the `Vector2` constructor: now it also accepts
   mappings.  The mapping must have exactly two elements,
   `x` and `y`.
 * Enhanced `Vector2.from_polar`.  It now accepts all the same
   stuff as the `Vector2` constructor: `Vector2` objects,
@@ -320,7 +389,8 @@
 
 * Bugfix: `vec.Vector2.dot()` was simply wrong, it was adding where it should
   have been multiplying.  Fixes #3.
 
 **0.5** *2021/03/21*
 
 Initial version.
+
```

### Comparing `vec-0.6.1/tests/test_all.py` & `vec-0.6.2/tests/test_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,16 +57,15 @@
 
 
 places = 14
 
 class VecTests(unittest.TestCase):
 
     def assertAlmostEqualVector(self, v1, v2):
-        self.assertAlmostEqual(v1.x, v2.x, places=places)
-        self.assertAlmostEqual(v1.y, v2.y, places=places)
+        self.assertTrue(v1.almost_equal(v2, places=places))
 
     # if everything is broken, fix this first!
     def test_eq(self):
         # note: assertNotEqual uses !=, which uses __ne__
         # so if you want to test a falsity use assertFalse
 
         vc = Vector2(3, 7)
@@ -829,14 +828,43 @@
             Vector2(r=1, theta=5)[2] = 33
 
     def test_polar(self):
         self.assertEqual(vector2_zero.polar(), (0, None))
         self.assertEqual(Vector2(1, 0).polar(), (1, 0))
         self.assertEqual(Vector2(-1, 0).polar(), (1, -pi))
 
+    def test_almost_equal(self):
+        v1 = Vector2(0.99991111, 0)
+        v2 = Vector2(0.99992222, 0)
+        self.assertTrue(v1.almost_equal(v2, 1))
+        self.assertTrue(v1.almost_equal(v2, 2))
+        self.assertTrue(v1.almost_equal(v2, 3))
+        self.assertTrue(v1.almost_equal(v2, 4))
+        self.assertFalse(v1.almost_equal(v2, 5))
+        self.assertFalse(v1.almost_equal(v2, 6))
+
+        v1 = Vector2(0, 0.99991111)
+        v2 = Vector2(0, 0.99992222)
+        self.assertTrue(v1.almost_equal(v2, 1))
+        self.assertTrue(v1.almost_equal(v2, 2))
+        self.assertTrue(v1.almost_equal(v2, 3))
+        self.assertTrue(v1.almost_equal(v2, 4))
+        self.assertFalse(v1.almost_equal(v2, 5))
+        self.assertFalse(v1.almost_equal(v2, 6))
+
+        v1 = Vector2(0.99991111, 0.99992222)
+        v2 = [0.99992222, 0.99991111]
+        self.assertTrue(v1.almost_equal(v2, 1))
+        self.assertTrue(v1.almost_equal(v2, 2))
+        self.assertTrue(v1.almost_equal(v2, 3))
+        self.assertTrue(v1.almost_equal(v2, 4))
+        self.assertFalse(v1.almost_equal(v2, 5))
+        self.assertFalse(v1.almost_equal(v2, 6))
+
+
     def test_scaled_to_length(self):
         vp_4_4 = Vector2(r=4, theta=4)
         self.assertEqual(vp_4_4.scaled_to_length(4), vp_4_4)
         self.assertEqual(vp_4_4.scaled_to_length(2), Vector2(r=2, theta=4))
         self.assertIs(vp_4_4.scaled_to_length(0), vector2_zero)
 
         v = Vector2(1, 0)
```

### Comparing `vec-0.6.1/vec/__init__.py` & `vec-0.6.2/vec/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 A 2-dimensional vector class designed to be convenient
 and performant enough for use in video games.
 """
 
 from math import acos, atan2, cos, pi, sin, sqrt, tau
 from collections.abc import Iterable, Set, Mapping
 
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 
 
 pi_over_two = pi/2
 negative_pi = -pi
 negative_pi_over_two = -pi_over_two
 
 
@@ -869,14 +869,28 @@
     def __hash__(self):
         return self._hash
 
     ##
     ## methods
     ##
 
+    def almost_equal(self, other, places):
+        """
+        Returns True if 'self' and 'other' have matching
+        cartesian coordinates down to 'places' decimal places.
+        """
+        if not isinstance(other, Vector2):
+            other = self.__class__(other)
+        if (self is other) or (self == other):
+            return True
+
+        delta = self - other
+        # print(f"{places} :: {a} - {b} = {delta=} <= {fraction=} = {delta <= fraction}")
+        return (not round(delta.x, places)) and (not round(delta.y, places))
+
     def scaled(self, multiplier):
         """
         Multiplies vector by a scalar.
         Equivalent to v * multiplier.
         """
         return self * multiplier
```

### Comparing `vec-0.6.1/PKG-INFO` & `vec-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: vec
-Version: 0.6.1
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
@@ -25,14 +12,16 @@
 Features:
 
 * `Vector2` objects are immutable.
 * `Vector2` support all the usual features, including operator overloading.
 * Attributes of `Vector2` objects are lazily-computed where possible.
 * `Vector2` objects effortlessly support both cartesian and polar coordinates.
 
+`vec` supports Python 3.6+, and passes its unit test suite with 100% coverage.
+
 
 ## Why Another Vector Class?
 
 I've participated in three PyWeek gaming challenges.  In two of those three times,
 mid-week I wrote my own vector class out of sheer frustration.
 
 The biggest problem with most Python vector objects in is that they're mutable.
@@ -152,31 +141,41 @@
 *either* both `x` and `y` *or* both `r` and `theta`.
 Any attributes not passed in at construction time will be lazily
 computed at the time they are evaluated.
 
 You can also pass in a single object which will initialize the
 vector.  Supported objects include:
 
-* an existing `vec.Vector2` object (just returns that object)
-* an object which has `.x` and `.y` attributes
-* an ordered iterable object with exactly two elements
+* an existing `vec.Vector2` object (just returns that object),
+* an object which has `.x` and `.y` attributes,
+* a mapping object with exactly two keys, `'x'` and `'y'`, and
+* an ordered iterable object with exactly two elements.
 
 `vec.Vector2` only does *some* validation of its arguments.
 It ensures that `r` and `theta` are normalized.  However,
 it doesn't check that `(x, y)` and `(r, theta)` describe the
 same vector.
-If you pass in `x` and `y`, and a `theta` and `r` that don't
-match, you'll get back the `vec.Vector2` that you asked for.
-Good luck.
+If you pass in `x` and `y`, and also pass in a `theta` and `r`
+that don't match, you'll get back the `vec.Vector2` that you
+asked for.  Good luck!
+
+### Attributes
 
 `vec.Vector2` objects support five attributes:
-`x`, `y`, `r`, `theta`, and `r_squared`.  It doesn't matter whether
-the object was defined with cartesian or polar coordinates, they
-will all work.  `r_squared` is equivalent to `r*r` but it's much
+`x`, `y`, `r`, `theta`, and `r_squared`.  It doesn't matter
+whether the object was defined with cartesian or polar
+coordinates, they'll all work.
+
+`r_squared` is equivalent to `r*r`, but it's much
 cheaper to compute based on cartesian coordinates.
+There are a lot of use cases where `r_squared` works
+just as well as `r`, for example in collision detection
+in a game.
+
+### Operators and protocols
 
 `vec.Vector2` objects support the *iterator protocol.*
 `len()` on a `vec.Vector2` object will always return 2.
 You can also iterate over a `vec.Vector2` object,
 which will yield the `x` and `y` attributes in that order.
 
 `vec.Vector2` objects support the *sequence protocol.*  You can subscript
@@ -184,33 +183,68 @@
 2 containing the `x` and `y` attributes.
 
 `vec.Vector2` objects also support the *boolean* protocol; you may use them
 with boolean operators, and you may call `bool()` on them.  When used in
 a boolean context, the zero vector evaluates to `False`, and all other
 vectors evaluate to `True`.
 
-`vec.Vector2` objects are hashable.
+`vec.Vector2` objects are *hashable,* but they're not *ordered*.
+(You can't ask if one vector is *less than* another.)
 
 `vec.Vector2` objects support the following operators:
 
 * `v1 + v2` adds the two vectors together.
 * `v1 - v2` subtracts the right vector from the left vector.
 * `v1 * scalar` mulitplies the vector by a scalar amount, equivalent to `v1.scale(scalar)`.
 * `v1 / scalar` divides the vector by a scalar amount.
 * `+v1` is exactly the same as `v1`.
 * `-v1` returns the opposite of `v1`, such that `v1 + (-v1)` should be the zero vector.
    (This may not always be the case due to compounding floating-point errors.)
 * `v1 == v2` is `True` if the two vectors are *exactly* the same, and `False` otherwise.
+  For consistency, this only compares cartesian coordinates.
+  Note that floating-point imprecision may result in two vectors that *should* be the
+  same failing an `==` check.
 * `v1 != v2` is `False` if the two vectors are *exactly* the same, and `True` otherwise.
+  For consistency, this only compares cartesian coordinates.
+  Note that floating-point imprecision may result in two vectors that *should* be the
+  same passing an `!=` check.
 * `v[0] == v.x`
 * `v[1] == v.y`
 * `list(v) == [v.x, v.y]`
 
+### Class methods
+
+`vec.from_polar(r, theta)`
+
+Constructs a `vec.Vector2` object from the two polar coordinates
+`r` and `theta`.
+
+You can also pass in a single object which will be used to
+initialize the vector.  Supported objects include:
+
+* an existing `vec.Vector2` object (just returns that object),
+* an object which has `.r` and `.theta` attributes,
+* a mapping object with exactly two keys, `'r'` and `'theta'`, and
+* an ordered iterable object with exactly two elements.
+
+If `r` is `0`, `theta` must be `None`, and `from_polar` will
+return the zero vector.  If `r` is not `0`, `theta` must not
+be `None`.
+
+### Methods
+
 `vec.Vector2` objects support the following methods:
 
+`vec.Vector2.almost_equal(other, places)`
+
+Returns `True` if the vector and `other` are the same vector,
+down to `places` decimal places.  Like the `Vector2` class's
+support for the `==` operator, the comparison is only done
+using cartesian coordinates, for consistency.
+
 `vec.Vector2.scaled(scalar)`
 
 Returns a new `vec.Vector2` object, equivalent to the original vector multiplied by that scalar.
 
 `vec.Vector2.scaled_to_length(r)`
 
 Returns a new `vec.Vector2` object, equivalent to the original vector with its length set to `r`.
@@ -255,26 +289,30 @@
 
 `vec.Vector2.nlerp(other, ratio)`
 
 Returns a vector representing a normalized linear interpolation between `self` and `other`,
 according to the scalar ratio `ratio`.  `ratio` should be a value between (and including)
 `0` and `1`.  If `ratio` is `0`, this returns `self`.  If `ratio` is `1`, this returns `other`.
 
+### Constants
+
 `vec.vector2_zero`
 
 The immutable, eternal "zero" `vec.Vector2` vector object.
 `vec` guarantees that every zero vector is a reference to this object:
 
     >>> v = vec.Vector2(0, 0)
     >>> v is vec.vector2_zero
     True
 
 Mathematically-speaking, the zero vector when expressed in polar coordinates
 doesn't have a defined angle.  Therefore `vec` defines its zero vector as
-having an angle of `None`.
+having an angle of `None`.  The zero vector must have `r` set to zero
+and `theta` set to `None`, and any other vector must have a non-zero `r`
+and `theta` set to a value besides `None`.
 
 
 ## Extending vec to handle other types
 
 `vec` does some input verification on its inputs.
 Coordinates--`x`, `y`, `r`, `theta`--are required to be
 either `int` or `long`.
@@ -297,14 +335,19 @@
 
 Note that the types you extend `vec` with in this manner
 should behave like numeric types, like `int` and `float`.
 
 
 ## Changelog
 
+**0.6.2** *2023/06/14*
+
+* Added `Vector2.almost_equal`, which supports testing
+  for slightly-inexact equality.
+
 **0.6.1** *2023/06/14*
 
 * Enhanced the `Vector2` constructor: now it also accepts
   mappings.  The mapping must have exactly two elements,
   `x` and `y`.
 * Enhanced `Vector2.from_polar`.  It now accepts all the same
   stuff as the `Vector2` constructor: `Vector2` objects,
@@ -333,8 +376,7 @@
 
 * Bugfix: `vec.Vector2.dot()` was simply wrong, it was adding where it should
   have been multiplying.  Fixes #3.
 
 **0.5** *2021/03/21*
 
 Initial version.
-
```

