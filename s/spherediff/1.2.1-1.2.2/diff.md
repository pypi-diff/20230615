# Comparing `tmp/spherediff-1.2.1.tar.gz` & `tmp/spherediff-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/kormos/spherediff/dist/.tmp-lzfndteu/spherediff-1.2.1.tar", last modified: Mon Jun  5 07:31:21 2023, max compression
+gzip compressed data, was "/home/kormos/spherediff/dist/.tmp-zd3apyk8/spherediff-1.2.2.tar", last modified: Thu Jun 15 20:05:22 2023, max compression
```

## Comparing `spherediff-1.2.1.tar` & `spherediff-1.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-05 07:31:21.774713 spherediff-1.2.1/
--rw-r--r--   0 kormos    (1000) kormos    (1000)     1068 2023-05-22 22:12:37.000000 spherediff-1.2.1/LICENSE.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)     5856 2023-06-05 07:31:21.774713 spherediff-1.2.1/PKG-INFO
--rw-r--r--   0 kormos    (1000) kormos    (1000)     5360 2023-06-05 07:24:48.000000 spherediff-1.2.1/README.md
--rw-r--r--   0 kormos    (1000) kormos    (1000)      766 2023-06-05 07:03:08.000000 spherediff-1.2.1/pyproject.toml
--rw-r--r--   0 kormos    (1000) kormos    (1000)       38 2023-06-05 07:31:21.774713 spherediff-1.2.1/setup.cfg
--rw-r--r--   0 kormos    (1000) kormos    (1000)       50 2023-05-22 21:59:35.000000 spherediff-1.2.1/setup.py
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-05 07:31:21.764713 spherediff-1.2.1/src/
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-05 07:31:21.774713 spherediff-1.2.1/src/spherediff/
--rw-r--r--   0 kormos    (1000) kormos    (1000)        0 2023-05-08 23:09:07.000000 spherediff-1.2.1/src/spherediff/__init__.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     8087 2023-05-29 03:14:23.000000 spherediff-1.2.1/src/spherediff/coeffs.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)    11140 2023-05-30 02:11:22.000000 spherediff-1.2.1/src/spherediff/kernel.py
--rwxr-xr-x   0 kormos    (1000) kormos    (1000)     4459 2023-05-29 03:14:23.000000 spherediff-1.2.1/src/spherediff/poly.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2332 2023-06-05 07:12:18.000000 spherediff-1.2.1/src/spherediff/sample.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     1423 2023-06-05 07:12:07.000000 spherediff-1.2.1/src/spherediff/score.py
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-05 07:31:21.774713 spherediff-1.2.1/src/spherediff.egg-info/
--rw-r--r--   0 kormos    (1000) kormos    (1000)     5856 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/PKG-INFO
--rw-r--r--   0 kormos    (1000) kormos    (1000)      383 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/SOURCES.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)        1 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/dependency_links.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)       75 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/requires.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)       11 2023-06-05 07:31:21.000000 spherediff-1.2.1/src/spherediff.egg-info/top_level.txt
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-15 20:05:22.345542 spherediff-1.2.2/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     1068 2023-05-22 22:12:37.000000 spherediff-1.2.2/LICENSE.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     5856 2023-06-15 20:05:22.345542 spherediff-1.2.2/PKG-INFO
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     5360 2023-06-15 20:02:08.000000 spherediff-1.2.2/README.md
+-rw-r--r--   0 kormos    (1000) kormos    (1000)      766 2023-06-15 20:03:17.000000 spherediff-1.2.2/pyproject.toml
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       38 2023-06-15 20:05:22.345542 spherediff-1.2.2/setup.cfg
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       50 2023-05-22 21:59:35.000000 spherediff-1.2.2/setup.py
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-15 20:05:22.315542 spherediff-1.2.2/src/
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-15 20:05:22.345542 spherediff-1.2.2/src/spherediff/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)        0 2023-05-08 23:09:07.000000 spherediff-1.2.2/src/spherediff/__init__.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     8087 2023-05-29 03:14:23.000000 spherediff-1.2.2/src/spherediff/coeffs.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)    11140 2023-05-30 02:11:22.000000 spherediff-1.2.2/src/spherediff/kernel.py
+-rwxr-xr-x   0 kormos    (1000) kormos    (1000)     4459 2023-05-29 03:14:23.000000 spherediff-1.2.2/src/spherediff/poly.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     2328 2023-06-15 20:02:32.000000 spherediff-1.2.2/src/spherediff/sample.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     1427 2023-06-15 19:57:50.000000 spherediff-1.2.2/src/spherediff/score.py
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-06-15 20:05:22.345542 spherediff-1.2.2/src/spherediff.egg-info/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     5856 2023-06-15 20:05:22.000000 spherediff-1.2.2/src/spherediff.egg-info/PKG-INFO
+-rw-r--r--   0 kormos    (1000) kormos    (1000)      383 2023-06-15 20:05:22.000000 spherediff-1.2.2/src/spherediff.egg-info/SOURCES.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)        1 2023-06-15 20:05:22.000000 spherediff-1.2.2/src/spherediff.egg-info/dependency_links.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       75 2023-06-15 20:05:22.000000 spherediff-1.2.2/src/spherediff.egg-info/requires.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       11 2023-06-15 20:05:22.000000 spherediff-1.2.2/src/spherediff.egg-info/top_level.txt
```

### Comparing `spherediff-1.2.1/LICENSE.txt` & `spherediff-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spherediff-1.2.1/PKG-INFO` & `spherediff-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherediff
-Version: 1.2.1
+Version: 1.2.2
 Summary: Sample from the diffusion kernel on any n-sphere
 Author-email: Rian Kormos <Rian.Kormos@ucsf.edu>
 Project-URL: Homepage, https://github.com/rckormos/SphereDiff
 Keywords: diffusion,hypersphere,sampling
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -137,13 +137,13 @@
 >>> x
 array([[ 0.92723597,  0.02336567,  0.37374791],
        [ 0.99421791, -0.03878944, -0.10013055],
        [ 0.15771025,  0.6492883 , -0.74401087],
        [ 0.2418101 , -0.41127436, -0.87885225],
        [-0.11192408, -0.71437847, -0.69075061]])
 >>> score_spherical_kernel(3, x, means, vars, hemisphere=True)
-array([[-1.74036155, -1.77246139,  4.42849462],
-       [-0.0852985 , -1.00528069, -0.45751298],
-       [ 2.51709283,  0.09916178,  0.62009298],
-       [ 4.08775888, -1.8186883 ,  1.97580568],
-       [ 1.8912707 , -0.37819329,  0.08468239]])
+array([[-1.90180502, -1.93688258,  4.83930095],
+       [-0.09346005, -1.10146816, -0.50128883],
+       [ 8.79701439,  0.34656156,  2.16716953],
+       [ 4.43128597, -1.97152723,  2.14184844],
+       [ 2.0106285 , -0.40206101,  0.09002668]])
 ```
```

### Comparing `spherediff-1.2.1/README.md` & `spherediff-1.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -123,13 +123,13 @@
 >>> x
 array([[ 0.92723597,  0.02336567,  0.37374791],
        [ 0.99421791, -0.03878944, -0.10013055],
        [ 0.15771025,  0.6492883 , -0.74401087],
        [ 0.2418101 , -0.41127436, -0.87885225],
        [-0.11192408, -0.71437847, -0.69075061]])
 >>> score_spherical_kernel(3, x, means, vars, hemisphere=True)
-array([[-1.74036155, -1.77246139,  4.42849462],
-       [-0.0852985 , -1.00528069, -0.45751298],
-       [ 2.51709283,  0.09916178,  0.62009298],
-       [ 4.08775888, -1.8186883 ,  1.97580568],
-       [ 1.8912707 , -0.37819329,  0.08468239]])
+array([[-1.90180502, -1.93688258,  4.83930095],
+       [-0.09346005, -1.10146816, -0.50128883],
+       [ 8.79701439,  0.34656156,  2.16716953],
+       [ 4.43128597, -1.97152723,  2.14184844],
+       [ 2.0106285 , -0.40206101,  0.09002668]])
 ```
```

### Comparing `spherediff-1.2.1/pyproject.toml` & `spherediff-1.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spherediff"
-version = "1.2.1"
+version = "1.2.2"
 description = "Sample from the diffusion kernel on any n-sphere"
 readme = "README.md"
 authors = [{name = "Rian Kormos", email = "Rian.Kormos@ucsf.edu"}]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License", 
     "Programming Language :: Python",
```

### Comparing `spherediff-1.2.1/src/spherediff/coeffs.py` & `spherediff-1.2.2/src/spherediff/coeffs.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.2.1/src/spherediff/kernel.py` & `spherediff-1.2.2/src/spherediff/kernel.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.2.1/src/spherediff/poly.py` & `spherediff-1.2.2/src/spherediff/poly.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.2.1/src/spherediff/sample.py` & `spherediff-1.2.2/src/spherediff/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     rejections /= np.linalg.norm(rejections, axis=1, keepdims=True)
     phi = newton_raphson(n, np.random.random(N), var, hemisphere)
     cosines, sines = np.cos(phi).reshape((-1, 1)), np.sin(phi).reshape((-1, 1))
     return mean * cosines + rejections * sines
 
 @nb.jit(nopython=True, cache=True)
 def newton_raphson(n, u_phi, var, hemisphere=False):
-    """Invert F_angle - u_phi by Newton-Raphson iteration.
+    """Invert CDF - u_phi by Newton-Raphson iteration.
 
     Parameters
     ----------
     n : int
         The dimensionality of the space in which the spherical surface is 
         embedded.
     u_omega : np.array [N]
```

### Comparing `spherediff-1.2.1/src/spherediff/score.py` & `spherediff-1.2.2/src/spherediff/score.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     N = len(var)
     projections = (x * mean).sum(axis=1, keepdims=True)
     phi = np.arccos(projections)
     rejections = mean - projections * x
     rejections /= -np.linalg.norm(rejections, axis=1, keepdims=True)
     ker, ker_deriv = raw_kernel(n, var, phi)
     if hemisphere:
-        ker_rev, ker_deriv_rev = kernel(n, var, np.pi - phi)
+        ker_rev, ker_deriv_rev = raw_kernel(n, var, np.pi - phi)
         ker += ker_rev
         ker_deriv += ker_deriv_rev
     return rejections * ker_deriv / ker
```

### Comparing `spherediff-1.2.1/src/spherediff.egg-info/PKG-INFO` & `spherediff-1.2.2/src/spherediff.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherediff
-Version: 1.2.1
+Version: 1.2.2
 Summary: Sample from the diffusion kernel on any n-sphere
 Author-email: Rian Kormos <Rian.Kormos@ucsf.edu>
 Project-URL: Homepage, https://github.com/rckormos/SphereDiff
 Keywords: diffusion,hypersphere,sampling
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -137,13 +137,13 @@
 >>> x
 array([[ 0.92723597,  0.02336567,  0.37374791],
        [ 0.99421791, -0.03878944, -0.10013055],
        [ 0.15771025,  0.6492883 , -0.74401087],
        [ 0.2418101 , -0.41127436, -0.87885225],
        [-0.11192408, -0.71437847, -0.69075061]])
 >>> score_spherical_kernel(3, x, means, vars, hemisphere=True)
-array([[-1.74036155, -1.77246139,  4.42849462],
-       [-0.0852985 , -1.00528069, -0.45751298],
-       [ 2.51709283,  0.09916178,  0.62009298],
-       [ 4.08775888, -1.8186883 ,  1.97580568],
-       [ 1.8912707 , -0.37819329,  0.08468239]])
+array([[-1.90180502, -1.93688258,  4.83930095],
+       [-0.09346005, -1.10146816, -0.50128883],
+       [ 8.79701439,  0.34656156,  2.16716953],
+       [ 4.43128597, -1.97152723,  2.14184844],
+       [ 2.0106285 , -0.40206101,  0.09002668]])
 ```
```

