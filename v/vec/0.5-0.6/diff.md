# Comparing `tmp/vec-0.5.tar.gz` & `tmp/vec-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vec-0.5.tar", last modified: Sat Mar 21 15:45:12 2020, max compression
+gzip compressed data, was "vec-0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vec-0.5.tar` & `vec-0.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       34 2020-03-21 15:27:41.638180 vec-0.5/.gitignore
--rw-r--r--   0        0        0     1507 2020-03-21 15:23:21.426936 vec-0.5/LICENSE
--rw-r--r--   0        0        0     9716 2020-03-21 15:30:48.473038 vec-0.5/README.md
--rw-r--r--   0        0        0      433 2020-03-21 06:15:30.671043 vec-0.5/pyproject.toml
--rw-r--r--   0        0        0     2819 2020-03-21 15:30:10.825473 vec-0.5/tests/test_vec.py
--rw-r--r--   0        0        0    21333 2020-03-21 15:32:35.433069 vec-0.5/vec/__init__.py
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 vec-0.5/setup.py
--rw-r--r--   0        0        0      205 1970-01-01 00:00:00.000000 vec-0.5/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-06-14 23:00:47.631077 vec-0.6/.gitignore
+-rw-r--r--   0        0        0     1508 2023-06-14 09:50:20.639282 vec-0.6/LICENSE
+-rw-r--r--   0        0        0    12444 2023-06-14 23:23:14.082858 vec-0.6/README.md
+-rw-r--r--   0        0        0      433 2023-06-13 18:12:35.372308 vec-0.6/pyproject.toml
+-rw-r--r--   0        0        0    30480 2023-06-14 23:21:59.014201 vec-0.6/tests/test_all.py
+-rw-r--r--   0        0        0    34167 2023-06-14 23:16:15.471195 vec-0.6/vec/__init__.py
+-rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 vec-0.6/PKG-INFO
```

### Comparing `vec-0.5/LICENSE` & `vec-0.6/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 vec
-Copyright 2019-2020 by Larry Hastings
+Copyright 2019-2023 by Larry Hastings
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
     * Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
     * Redistributions in binary form must reproduce the above copyright
@@ -18,8 +18,8 @@
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> BE LIABLE FOR ANY
 DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `vec-0.5/README.md` & `vec-0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # vec
 
 ## A reasonable, performant 2D vector object for games
 
-##### Copyright 2019-2020 by Larry Hastings
+##### Copyright 2019-2023 by Larry Hastings
 
 ## Overview
 
 `vec` is a module currently containing one class: `Vector2`, a 2D
 vector object designed for game development.
 
 Features:
@@ -44,19 +44,20 @@
 On a related note, many vector classes make polar coordinates
 second-class citizens.  Most vector classes only store vectors in
 cartesian coordinates, so either the programmer must perform all polar
 operations externally to the vector objects, or they incur the
 overhead and cumulative error of translating to polar and
 back again with every operation.
 
-`vec.Vector2` avoids all these problems.  `vec.Vector2` objects
-are immutable,
-they support vectors defined with either polar or cartesian coordinates,
-and
-they strictly use radians for polar operations.
+`vec.Vector2` avoids all these problems:
+
+* `vec.Vector2` objects are immutable,
+* they support vectors defined with either polar or cartesian coordinates,
+  and
+* they strictly use radians for polar coordinates.
 
 ## The Conceptual Model
 
 `vec.Vector2` objects conceptually represent a vector.  They can be
 defined using either cartesian or polar coordinates, and any `vec.Vector2`
 can be queried for both its cartesian and polar coordinates.
 
@@ -81,83 +82,90 @@
 
     v = vec.Vector2(0, 1)
     print(v.theta, v.r)
 
 prints `1.5707963267948966 1.0`.  That first number is π/2 (approximately).
 
 Conversely, you can also define `vec.Vector2` objects using polar
-coordinates, and then ask for its cartesian coordinates:
+coordinates, and then ask it for its cartesian coordinates:
 
     v2 = vec.Vector2(r=1, theta=1.5707963267948966)
     print(v2.x, v2.y)
 
 This prints `6.123233995736766e-17 1.0`.  Conceptually this should
-print `0.0, 1.0`--but `math.pi` is only an approximation, which means
-sadly our result is off by an infinitesimal amount.
+print `0.0, 1.0`--but `math.pi` is only an approximation, which means,
+sadly, that our result has an infinitesimal error.
 
 ### Implementation Details
 
-Internally `vec.Vector2` objects are either "cartesian" or "polar".
+Internally `vec.Vector2` objects are either "cartesian", "polar",
+or both.
 "cartesian" vector objects are defined in terms of `x` and `y`;
 "polar" vector objects are defined in terms of `r` and `theta`.
 All other attributes are lazily computed as needed.
 
 `vec.Vector2` objects use slots, and rely on `__getattr__`
 to implement this lazy computation.  Only the known values of the
 vector are set when it's created.  If the user refers to an attribute
 that hasn't been computed yet, Python will call `vec.Vector2.__getattr__()`,
-which computes and then sets that value.  Future references to that
+which computes, caches, and returns that value.  Future references to that
 attribute skip this mechanism and simply return the cached value, which
 is only as expensive as an attribute lookup on a conventional object.
 
 Operations on `vec.Vector2` objects compute their result
 using the cheapest approach.  If you have a `vec.Vector2` object
 defined using polar coordinates, and you call `.rotate()` or `.scale()`
 on it, all the math is done in the polar domain.  On the other
-hand, adding vectors is always done in the cartesian domain, so
-if you add a polar vector to any other vector, its cartesian
-coordinates will be computed--and the resulting vector will always
+hand, adding vectors is *almost* always done in the cartesian domain,
+so if you add a polar vector to any other vector, its cartesian
+coordinates will likely be computed--and the resulting vector will always
 be defined using cartesian coordinates.
 
-Actually, that last statement isn't always true.  There's a special
-case for adding two polar vectors which have the exact same `theta`:
-just add their `r` values. That approach is much cheaper than
-converting to cartesian, and more precise as well, returning a vector
-defined using polar coordinates!  `vec.Vector2` takes advantage of
-many such serendipities, computing your vectors as cheaply and accurately
-as possible.
+What's the exception?  There's a special case for adding two polar vectors
+which have the exact same `theta`: just add their `r` values.
+That approach is much cheaper than converting to cartesian,
+and more precise as well, returning a vector defined using polar
+coordinates!  `vec.Vector2` takes advantage of many such serendipities,
+computing your vectors as cheaply and accurately as possible.
 
 
 ## The API
 
 `vec.Vector2(x=None, y=None, *, r=None, theta=None, r_squared=None)`
 
 Constructs a `vec.Vector2` object.  You may pass in as many or as
 few of these arguments as you like; however, you *must* pass in
 *either* both `x` and `y` *or* both `r` and `theta`.
 Any attributes not passed in at construction time will be lazily
 computed at the time they are evaluated.
 
-(`vec.Vector2` only does *some* validation of its arguments.
+You can also pass in a single object which will initialize the
+vector.  Supported objects include:
+
+* an existing `vec.Vector2` object (just returns that object)
+* an object which has `.x` and `.y` attributes
+* an ordered iterable object with exactly two elements
+
+`vec.Vector2` only does *some* validation of its arguments.
 It ensures that `r` and `theta` are normalized.  However,
 it doesn't check that `(x, y)` and `(r, theta)` describe the
 same vector.
 If you pass in `x` and `y`, and a `theta` and `r` that don't
 match, you'll get back the `vec.Vector2` that you asked for.
-Good luck.)
+Good luck.
 
 `vec.Vector2` objects support five attributes:
 `x`, `y`, `r`, `theta`, and `r_squared`.  It doesn't matter whether
-the object was defined with cartesian or polar coordinates; these
-all work.  `r_squared` is equivalent to `r*r` but it's much cheaper
-to compute based on cartesian coordinates.
-
-`vec.Vector2` objects support the *iterator protocol.*  You can call
-`len()` on `vec.Vector2` objects--and it'll always return 2.
-You can also iterate over them,
+the object was defined with cartesian or polar coordinates, they
+will all work.  `r_squared` is equivalent to `r*r` but it's much
+cheaper to compute based on cartesian coordinates.
+
+`vec.Vector2` objects support the *iterator protocol.*
+`len()` on a `vec.Vector2` object will always return 2.
+You can also iterate over a `vec.Vector2` object,
 which will yield the `x` and `y` attributes in that order.
 
 `vec.Vector2` objects support the *sequence protocol.*  You can subscript
 them, which behaves as if the `vec.Vector2` object is a tuple of length
 2 containing the `x` and `y` attributes.
 
 `vec.Vector2` objects also support the *boolean* protocol; you may use them
@@ -174,14 +182,17 @@
 * `v1 * scalar` mulitplies the vector by a scalar amount, equivalent to `v1.scale(scalar)`.
 * `v1 / scalar` divides the vector by a scalar amount.
 * `+v1` is exactly the same as `v1`.
 * `-v1` returns the opposite of `v1`, such that `v1 + (-v1)` should be the zero vector.
    (This may not always be the case due to compounding floating-point errors.)
 * `v1 == v2` is `True` if the two vectors are *exactly* the same, and `False` otherwise.
 * `v1 != v2` is `False` if the two vectors are *exactly* the same, and `True` otherwise.
+* `v[0] == v.x`
+* `v[1] == v.y`
+* `list(v) == [v.x, v.y]`
 
 `vec.Vector2` objects support the following methods:
 
 `vec.Vector2.scaled(scalar)`
 
 Returns a new `vec.Vector2` object, equivalent to the original vector multiplied by that scalar.
 
@@ -217,19 +228,86 @@
 `vec.Vector2.lerp(other, ratio)`
 
 Returns a vector representing a linear interpolation between `self` and `other`, according
 to the scalar ratio `ratio`.  `ratio` should be a value between (and including) `0` and `1`.
 If `ratio` is `0`, this returns `self`.  If `ratio` is `1`, this returns `other`.
 If `ratio` is `0.4`, this returns `(self * 0.6) + (other * 0.4)`.
 
+`vec.Vector2.slerp(other, ratio)`
+
+Returns a vector representing a spherical interpolation between `self` and `other`, according
+to the scalar ratio `ratio`.  `ratio` should be a value between (and including) `0` and `1`.
+If `ratio` is `0`, this returns `self`.  If `ratio` is `1`, this returns `other`.
+
+`vec.Vector2.nlerp(other, ratio)`
+
+Returns a vector representing a normalized linear interpolation between `self` and `other`,
+according to the scalar ratio `ratio`.  `ratio` should be a value between (and including)
+`0` and `1`.  If `ratio` is `0`, this returns `self`.  If `ratio` is `1`, this returns `other`.
+
 `vec.vector2_zero`
 
 The immutable, eternal "zero" `vec.Vector2` vector object.
 `vec` guarantees that every zero vector is a reference to this object:
 
     >>> v = vec.Vector2(0, 0)
     >>> v is vec.vector2_zero
     True
 
 Mathematically-speaking, the zero vector when expressed in polar coordinates
 doesn't have a defined angle.  Therefore `vec` defines its zero vector as
 having an angle of `None`.
+
+
+## Extending vec to handle other types
+
+`vec` does some input verification on its inputs.
+Coordinates--`x`, `y`, `r`, `theta`--are required to be
+either `int` or `long`.
+(Technically `theta` can also be `None`.)  This best serves
+the intended use case of `vec` as a 2D vector library for
+game programming in Python.
+
+If you want to experiment with `vec` for other use cases,
+you may want `vec` to permit other types to be valid
+coordinates.  `vec` provides a simple mechanism to allow
+this.  Simply call:
+
+```
+    vec.permit_coordinate_type(T)
+```
+
+before creating your vector, passing in the type you want
+to use as a coordinate as `T`, and `vec` will now accept
+objects of that type as coordinates.
+
+Note that the types you extend `vec` with in this manner
+should behave like numeric types, like `int` and `float`.
+
+
+## Changelog
+
+**0.6** *2023/06/4*
+
+A major improvement!
+
+* `vec` now has a proper test suite.
+* `vec` now passes its test suite with 100% coverage.
+* `vec` explicitly supports Python 3.6+.
+* Added more shortcut optimizations, e.g. rotating a cartesian vector by a multiple of `pi/2`.
+* Tightened up the metaclass `__call__` logic a great deal.
+* Implemented `vec.Vector2.slerp`, and added `vec.Vector2.nlerp`.
+* Allowed `vec.permit_coordinate_type`, to allow extending the
+  set of permissible types for coordinates.
+* Internal details:
+
+    - Now cache `_cartesian` and `_hash` internally, as well as `_polar`.
+      (A vector can have a complete set of both cartesian and polar coordinates,
+      so it's nice to know everything that's available--that can make some
+      operations faster.)
+
+* Bugfix: `vec.Vector2.dot()` was simply wrong, it was adding where it should
+  have been multiplying.  Fixes #3.
+
+**0.5** *2021/03/21*
+
+Initial version.
```

