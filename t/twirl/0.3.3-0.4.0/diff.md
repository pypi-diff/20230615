# Comparing `tmp/twirl-0.3.3.tar.gz` & `tmp/twirl-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twirl-0.3.3.tar", max compression
+gzip compressed data, was "twirl-0.4.0.tar", max compression
```

## Comparing `twirl-0.3.3.tar` & `twirl-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     5037 2023-06-01 13:52:02.904590 twirl-0.3.3/README.md
--rw-r--r--   0        0        0     2902 2023-06-01 13:52:02.912590 twirl-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     5151 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/__init__.py
--rw-r--r--   0        0        0     3535 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/geometry.py
--rw-r--r--   0        0        0     3520 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/match.py
--rw-r--r--   0        0        0     2145 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/quads.py
--rw-r--r--   0        0        0     2174 2023-06-01 13:52:02.916590 twirl-0.3.3/twirl/triangles.py
--rw-r--r--   0        0        0     6100 1970-01-01 00:00:00.000000 twirl-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     4814 2023-06-15 12:56:06.841498 twirl-0.4.0/README.md
+-rw-r--r--   0        0        0     2902 2023-06-15 12:56:06.849498 twirl-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5225 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/__init__.py
+-rw-r--r--   0        0        0     4620 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/geometry.py
+-rw-r--r--   0        0        0     4138 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/match.py
+-rw-r--r--   0        0        0     2554 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/quads.py
+-rw-r--r--   0        0        0     2174 2023-06-15 12:56:06.853498 twirl-0.4.0/twirl/triangles.py
+-rw-r--r--   0        0        0     5877 1970-01-01 00:00:00.000000 twirl-0.4.0/PKG-INFO
```

### Comparing `twirl-0.3.3/README.md` & `twirl-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -30,89 +30,75 @@
 1. detection of stars in the image if not provided
 2. catalog query using image known center
 3. asterisms building and matching
 4. image recombination and wcs fit using astropy.wcs
 
 Astersisms are made of 3 or 4 points. 4 points asterisms are built following Lang et al. 2009 while 3 points asterims are based on an original algorithm.
 
----
-
 ## Installation
 
 twirl can be installed using pip:
 
 ```shell
 pip install twirl
 ```
 
 or using poetry:
 
 ```shell
 poetry add twirl
 ```
 
----
-
 ## Example Usage
 
-twirl is designed to be complementary to the astropy package. It is used to compute a WCS from a set of stars detected in an image. 
-
-As a prerequisite, star detection and plate solving is suited for when the image center and field of view are known. 
+*twirl* is designed to be complementary to the *astropy* package. It is used to compute a WCS by matching an image detected stars with catalog stars. To query the catalog stars, the center coordinates of the image must be known, as well as the size of the field of view. If not available, the latter can be computed using the known pixel scale of the detector.
 
-In this case, the image center and field of view can be provided as a SkyCoord object and a Quantity object respectively.
-
-Use any specified header that has been stored on the FITS primary HDU to obtain the center equatorial coordinate and field of view, for this example we will assum "RA" and "DEC" are the keywords for the center equatorial coordinate.
-
-### Setup
+Hence, the process starts by extracting the image RA-DEC center equatorial coordinate and compute the instrument field of view
 
 ```python
 import numpy as np
 
 from astropy.io import fits
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 
-# Open some FITS image: 
-hdul = fits.open("...")
-
-# ra, dec in degrees
-ra, dec = header["RA"], header["DEC"]
+# Open some FITS image
+hdu = fits.open("...")[0]
 
-# Provide the center as a SkyCoord object:
+# get the center of the image
+ra, dec = hdu.header["RA"], hdu.header["DEC"]
 center = SkyCoord(ra, dec, unit=["deg", "deg"])
 
-center = [center.ra.value, center.dec.value]
+# and the size of its field of view
+pixel = 0.66 * u.arcsec  # known pixel scale
+shape = hdu.data.shape
+fov = np.max(shape) * pixel.to(u.deg)
+```
 
-# Utilise the image shape and pixel size in arcseconds " to obtain the field of view in degrees:
-shape = data.shape
+We can then query the gaia stars in the field using this information
 
-# Pixel size in arcseconds:
-pixel = 0.66 * u.arcsec
+```python
+import twirl
 
-# Field of view in degrees:
-fov = np.max(shape)*pixel.to(u.deg).value
+sky_coords = twirl.gaia_radecs(center, 1.2 * fov)[0:12]
 ```
 
-From here, we can pass the data, the center equatorial coordinate and the field-of-view to twirl to compute the World Coordinate System (WCS):
-
-### Twirl Usage
+and match the queried stars to stars detected in the image
 
 ```python
-import twirl
-
-# Find some starts in the image:
-stars = twirl.find_peaks(data)[0:15]
+# detect stars in the image
+pixel_coords = twirl.find_peaks(hdu.data)[0:12]
 
-# Compute the World Coordinate System:
-wcs = twirl.compute_wcs(stars, center, fov)
+# compute the World Coordinate System
+wcs = twirl.compute_wcs(pixel_coords, sky_coords)
 ```
+leading to a World Coordinate System object.
 
-A more complete example is provided in [docs/notebooks](https://github.com/lgrcia/twirl/tree/master/docs/notebooks)
+A more complete example is provided in [docs/ipynb/wcs.ipynb](https://twirl.readthedocs.io/en/latest/ipynb/wcs.html)
 
----
 
 ## Development
 
 ### Project Requirements
 
 - [Python](https://www.python.org/) 3.11.*
 - [Poetry](https://python-poetry.org/) for Python package and environment management.
@@ -139,15 +125,14 @@
 
 ```console
 $ poetry install
 ```
 
 **N.B.** _Ensure that any dependency changes are committed to source control, so everyone has a consistenct package dependecy list._
 
----
 
 ## Acknowledgements
 
 This package has made use of the algorithm from
 
 Lang, D. et al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary Astronomical Images_. The Astronomical Journal, 139(5), pp.1782–1800. [doi:10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-6256/139/5/1782).
```

#### html2text {}

```diff
@@ -6,54 +6,51 @@
 cases where the Right Ascension and Declination (RA, dec) coordinates of the
 image center and the field of view is known, computing a World Coordinate
 System (WCS) based on GAIA reference stars. twirl compute a WCS following these
 steps: 1. detection of stars in the image if not provided 2. catalog query
 using image known center 3. asterisms building and matching 4. image
 recombination and wcs fit using astropy.wcs Astersisms are made of 3 or 4
 points. 4 points asterisms are built following Lang et al. 2009 while 3 points
-asterims are based on an original algorithm. --- ## Installation twirl can be
+asterims are based on an original algorithm. ## Installation twirl can be
 installed using pip: ```shell pip install twirl ``` or using poetry: ```shell
-poetry add twirl ``` --- ## Example Usage twirl is designed to be complementary
-to the astropy package. It is used to compute a WCS from a set of stars
-detected in an image. As a prerequisite, star detection and plate solving is
-suited for when the image center and field of view are known. In this case, the
-image center and field of view can be provided as a SkyCoord object and a
-Quantity object respectively. Use any specified header that has been stored on
-the FITS primary HDU to obtain the center equatorial coordinate and field of
-view, for this example we will assum "RA" and "DEC" are the keywords for the
-center equatorial coordinate. ### Setup ```python import numpy as np from
-astropy.io import fits from astropy import units as u from astropy.coordinates
-import SkyCoord # Open some FITS image: hdul = fits.open("...") # ra, dec in
-degrees ra, dec = header["RA"], header["DEC"] # Provide the center as a
-SkyCoord object: center = SkyCoord(ra, dec, unit=["deg", "deg"]) center =
-[center.ra.value, center.dec.value] # Utilise the image shape and pixel size in
-arcseconds " to obtain the field of view in degrees: shape = data.shape # Pixel
-size in arcseconds: pixel = 0.66 * u.arcsec # Field of view in degrees: fov =
-np.max(shape)*pixel.to(u.deg).value ``` From here, we can pass the data, the
-center equatorial coordinate and the field-of-view to twirl to compute the
-World Coordinate System (WCS): ### Twirl Usage ```python import twirl # Find
-some starts in the image: stars = twirl.find_peaks(data)[0:15] # Compute the
-World Coordinate System: wcs = twirl.compute_wcs(stars, center, fov) ``` A more
-complete example is provided in [docs/notebooks](https://github.com/lgrcia/
-twirl/tree/master/docs/notebooks) --- ## Development ### Project Requirements -
-[Python](https://www.python.org/) 3.11.* - [Poetry](https://python-poetry.org/
-) for Python package and environment management. ### Installing Dependencies
-The twirl project manages Python package dependencies using [Poetry](https://
-python-poetry.org/). You'll need to follow the instructions for installation
-there. Then you can start a shell session with the new environment with:
-```console $ poetry shell ``` **N.B.** For development with vscode you will
-need to run the following command: ```console $ poetry config virtualenvs.in-
-project true ``` This will installed the poetry `.venv` in the root of the
-project and allow vscode to setup the environment correctly for development. To
-start development, install all of the dependencies as: ```console $ poetry
-install ``` **N.B.** _Ensure that any dependency changes are committed to
-source control, so everyone has a consistenct package dependecy list._ --- ##
-Acknowledgements This package has made use of the algorithm from Lang, D. et
-al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary
-Astronomical Images_. The Astronomical Journal, 139(5), pp.1782â1800. [doi:
-10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-
-6256/139/5/1782). implemented in Garcia, L. J. et al. (2022). prose: a Python
-framework for modular astronomical images processing. MNRAS, vol. 509, no. 4,
-pp. 4817â4828, 2022. [doi:10.1093/mnras/stab3113](https://academic.oup.com/
-mnras/article-abstract/509/4/4817/6414007). See this [documentation page]
-(https://twirl.readthedocs.io/en/latest/md/acknowledgement.html) for the BibTeX
-entries.
+poetry add twirl ``` ## Example Usage *twirl* is designed to be complementary
+to the *astropy* package. It is used to compute a WCS by matching an image
+detected stars with catalog stars. To query the catalog stars, the center
+coordinates of the image must be known, as well as the size of the field of
+view. If not available, the latter can be computed using the known pixel scale
+of the detector. Hence, the process starts by extracting the image RA-DEC
+center equatorial coordinate and compute the instrument field of view ```python
+import numpy as np from astropy.io import fits from astropy import units as u
+from astropy.coordinates import SkyCoord # Open some FITS image hdu = fits.open
+("...")[0] # get the center of the image ra, dec = hdu.header["RA"], hdu.header
+["DEC"] center = SkyCoord(ra, dec, unit=["deg", "deg"]) # and the size of its
+field of view pixel = 0.66 * u.arcsec # known pixel scale shape =
+hdu.data.shape fov = np.max(shape) * pixel.to(u.deg) ``` We can then query the
+gaia stars in the field using this information ```python import twirl
+sky_coords = twirl.gaia_radecs(center, 1.2 * fov)[0:12] ``` and match the
+queried stars to stars detected in the image ```python # detect stars in the
+image pixel_coords = twirl.find_peaks(hdu.data)[0:12] # compute the World
+Coordinate System wcs = twirl.compute_wcs(pixel_coords, sky_coords) ``` leading
+to a World Coordinate System object. A more complete example is provided in
+[docs/ipynb/wcs.ipynb](https://twirl.readthedocs.io/en/latest/ipynb/wcs.html)
+## Development ### Project Requirements - [Python](https://www.python.org/
+) 3.11.* - [Poetry](https://python-poetry.org/) for Python package and
+environment management. ### Installing Dependencies The twirl project manages
+Python package dependencies using [Poetry](https://python-poetry.org/). You'll
+need to follow the instructions for installation there. Then you can start a
+shell session with the new environment with: ```console $ poetry shell ```
+**N.B.** For development with vscode you will need to run the following
+command: ```console $ poetry config virtualenvs.in-project true ``` This will
+installed the poetry `.venv` in the root of the project and allow vscode to
+setup the environment correctly for development. To start development, install
+all of the dependencies as: ```console $ poetry install ``` **N.B.** _Ensure
+that any dependency changes are committed to source control, so everyone has a
+consistenct package dependecy list._ ## Acknowledgements This package has made
+use of the algorithm from Lang, D. et al. (2010). _Astrometry.net: Blind
+Astrometric Calibration of Arbitrary Astronomical Images_. The Astronomical
+Journal, 139(5), pp.1782â1800. [doi:10.1088/0004-6256/139/5/1782](https://
+iopscience.iop.org/article/10.1088/0004-6256/139/5/1782). implemented in
+Garcia, L. J. et al. (2022). prose: a Python framework for modular astronomical
+images processing. MNRAS, vol. 509, no. 4, pp. 4817â4828, 2022. [doi:10.1093/
+mnras/stab3113](https://academic.oup.com/mnras/article-abstract/509/4/4817/
+6414007). See this [documentation page](https://twirl.readthedocs.io/en/latest/
+md/acknowledgement.html) for the BibTeX entries.
```

### Comparing `twirl-0.3.3/pyproject.toml` & `twirl-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twirl"
-version = "0.3.3"
+version = "0.4.0"
 description = "Astrometric plate solving in Python"
 authors = ["Lionel J. Garcia <lionel_garcia@live.fr>"]
 maintainers = [
   "Lionel J. Garcia <lionel_garcia@live.fr>",
   "Michael J. Roberts <michael@observerly.com>",
 ]
 license = "MIT"
@@ -16,15 +16,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 astropy = "^5.1.1"
 astroquery = "^0.4.6"
 matplotlib = "^3.6.2"
 numpy = "^1.23.5"
 requests = "^2.28.1"
-scikit-image = "^0.19.3"
+scikit-image = "^0.21.0"
 scipy = "^1.9.3"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.261"
 pytest = "^7.3.1"
```

### Comparing `twirl-0.3.3/twirl/__init__.py` & `twirl-0.4.0/twirl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 from twirl.match import cross_match, find_transform, get_transform_matrix
 
 
 def compute_wcs(
     pixel_coords: np.ndarray,
     radecs: np.ndarray,
     tolerance: int = 5,
+    quads_tolerance: float = 0.1,
     asterism=4,
-    min_match=None,
+    min_match=0.8,
 ) -> WCS:
     """
     Compute the WCS solution for an image given pixel coordinates and some unordered RA-DEC values.
 
     Parameters
     ----------
     pixel_coords : np.ndarray
@@ -42,14 +43,15 @@
     """
     M = find_transform(
         radecs,
         pixel_coords,
         tolerance=tolerance,
         asterism=asterism,
         min_match=min_match,
+        quads_tolerance=quads_tolerance,
     )
     radecs_xy = (M @ pad(radecs).T)[0:2].T
     i, j = cross_match(pixel_coords, radecs_xy).T
     M = get_transform_matrix(radecs[j], pixel_coords[i])
     radecs_xy = (M @ pad(radecs).T)[0:2].T
     i, j = cross_match(pixel_coords, radecs_xy).T
     return fit_wcs_from_points(pixel_coords[i].T, SkyCoord(radecs[j], unit="deg"))
```

### Comparing `twirl-0.3.3/twirl/match.py` & `twirl-0.4.0/twirl/match.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 
 import numpy as np
+from scipy.spatial import cKDTree
 
 from twirl.geometry import get_transform_matrix, pad
 from twirl.quads import hashes as hash4
 from twirl.triangles import hashes as hash3
 
 
 def count_cross_match(coords1, coords2, tol=1e-3):
@@ -58,63 +59,79 @@
         if distances[closest] < tolerance:
             matches.append([i, closest])
 
     return np.array(matches)
 
 
 def find_transform(
-    coords2: np.ndarray,
-    coords1: np.ndarray,
-    tolerance: int = 12,
-    min_match: Optional[int] = None,
+    radecs: np.ndarray,
+    pixels: np.ndarray,
+    min_match: float = 0.7,
     asterism: int = 4,
+    quads_tolerance: float = 0.02,
+    tolerance: float = 12,
 ) -> np.ndarray:
     """
-    Finds the transformation matrix that maps the coordinates in `coords2` to the coordinates in `coords1`.
+    Finds the transformation matrix from `radecs` to `pixels`.
 
     Parameters
     ----------
-    coords2 : np.ndarray
+    radecs : np.ndarray
         The coordinates to be transformed, shape (n, 2).
-    coords1 : np.ndarray
+    pixels : np.ndarray
         The target coordinates, shape (m, 2).
-    tolerance : int, optional
-        The tolerance of the match, given in `coords1` points units, by default 12.
-    min_match : Optional[int], optional
-        The minimum number of matches required to stop the search, by default None.
+    min_match : float, optional
+        The fraction of `pixels` coordinates that must be matched to stop the search.
+        I.e., if the number of matched points is `>= min_match * len(pixels)`, the
+        search stops and return the found transform. By default 0.7.
     asterism : int, optional
         The asterism to use for hashing, either 3 or 4, by default 4.
+    quads_tolerance : float, optional
+        The minimum euclidean distance between two quads to be matched and tested.
+        By default 0.02.
+    tolerance : float, optional
+        The minimum distance between two coordinates to be considered cross-matched
+        (in `pixels` units). This serves to compute the number of coordinates being
+        matched between `radecs` and `pixels` for a given transform.
+        By default 12.
 
     Returns
     -------
     np.ndarray
-        The transformation matrix that maps `coords2` to `coords1`.
+        The transformation matrix from `radecs` to `pixels`.
     """
 
     if asterism == 3:
         asterism_function = hash3
     elif asterism == 4:
         asterism_function = hash4
     else:
         raise ValueError("available asterisms are 3 and 4")
 
-    hash1, asterism_coords1 = asterism_function(coords1)
-    hash2, asterism_coords2 = asterism_function(coords2)
-    distances = np.linalg.norm(hash1[:, None, :] - hash2[None, :, :], axis=2)
-    shortest_hash = np.argmin(distances, 1)
-    ns = []
-
-    for i, j in enumerate(shortest_hash):
-        M = get_transform_matrix(asterism_coords2[j], asterism_coords1[i])
-        test = (M @ pad(coords2).T)[0:2].T
-        n = count_cross_match(coords1, test, tolerance)
-        ns.append(n)
+    hashes_pixels, asterism_pixels = asterism_function(pixels)
+    hashes_radecs, asterism_radecs = asterism_function(radecs)
+
+    tree_pixels = cKDTree(hashes_pixels)
+    tree_radecs = cKDTree(hashes_radecs)
+    pairs = []
+
+    ball_query = tree_pixels.query_ball_tree(tree_radecs, r=quads_tolerance)
+    matches = []
+
+    for i, j in enumerate(ball_query):
+        if len(j) > 0:
+            pairs += [[i, k] for k in j]
+
+    for i, j in pairs:
+        M = get_transform_matrix(asterism_radecs[j], asterism_pixels[i])
+        test = (M @ pad(radecs).T)[0:2].T
+        match = count_cross_match(pixels, test, tolerance)
+        matches.append(match)
+
         if min_match is not None:
-            if n >= min_match:
+            if match >= min_match * len(pixels):
                 break
 
-        i = np.argmax(ns)
-        M = get_transform_matrix(
-            asterism_coords2[np.argmin(distances, 1)[i]], asterism_coords1[i]
-        )
+    i, j = pairs[np.argmax(matches)]
+    M = get_transform_matrix(asterism_radecs[j], asterism_pixels[i])
 
     return M
```

### Comparing `twirl-0.3.3/twirl/quads.py` & `twirl-0.4.0/twirl/quads.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 from itertools import combinations
 
 import numpy as np
 
 from twirl.geometry import proj, u1u2
 
 
-def _reorder(q):
-    """
-    order coordinates from closest to first one
-    """
-    distances = np.linalg.norm(q[:, :, None] - q.T[None, :, :], axis=1)
-    q0i = np.min(np.unravel_index(np.argmax(distances), distances.shape))
-    q0 = q[q0i]
-    q123 = np.delete(q.copy(), q0i, axis=0)
-    distance_from_q0 = np.linalg.norm(q123 - q0, axis=1)
-    idxs = np.argsort(1 / distance_from_q0)
-    return np.array([q0, *q123[idxs]])
-
-
-reorder = np.vectorize(_reorder, signature="(n, m)->(n, m)")
+def reorder(quads):
+    distances = np.linalg.norm(
+        quads[:, :, :, None] - np.rollaxis(quads.T, 2)[:, None, :, :], axis=2
+    )
+    i = np.argmax(np.max(distances, 1), 1)
+    idxs = np.roll(
+        np.argsort(distances[range(len(quads)), i], axis=1)[:, ::-1], 1, axis=1
+    )
+    return np.array([q[i] for q, i in zip(quads, idxs)])
 
 
 def good_quads(quads, circletol=0.01):
     """
     whether all points are contained in a circle (see Lang2009)
     """
     q0, q1 = quads[:, 0], quads[:, 1]
@@ -30,32 +25,50 @@
     center = q0 + (q1 - q0) / 2
     in_circle = np.linalg.norm(quads - center[:, None, :], axis=2) <= r[:, None] * (
         1 + circletol
     )
     return np.all(in_circle, axis=1)
 
 
-def _quad_hash(quad):
-    """
-    from 4 coordinates produce the quad hash code
-    """
-    a, b, c, d = quad
-    u1, u2 = u1u2(a, b)
-    h = np.linalg.norm(b - a)
-    return np.array(
-        [
-            proj(c, a, u1, norm=True) / h,
-            proj(d, a, u1, norm=True) / h,
-            proj(c, a, u2, norm=True) / h,
-            proj(d, a, u2, norm=True) / h,
-        ]
-    ), np.array([a, b])
+def quad_hash(quads):
+    a, b, c, d = np.rollaxis(quads, 1)
+
+    norm = np.linalg.norm(b - a, axis=1)
 
+    def u1u2(a, b):
+        """compute x, y basis as defined in Lang2009"""
+        co_m = np.cos(-np.pi / 4)
+        si_m = np.sin(-np.pi / 4)
+        co_p = np.cos(np.pi / 4)
+        si_p = np.sin(np.pi / 4)
+        rm = np.array([[co_m, -si_m], [si_m, co_m]])
+        rp = np.array([[co_p, -si_p], [si_p, co_p]])
+        x = (rm @ (b - a).T).T + a
+        y = (rp @ (b - a).T).T + a
+        return x, y
 
-quad_hash = np.vectorize(_quad_hash, signature="(n,m)->(k), (l, 2)")
+    u1, u2 = u1u2(a, b)
+
+    def proj(p, origin, axe):
+        """projection of a point p on a segment from origin to axe"""
+        n = axe - origin
+        n /= np.linalg.norm(n, axis=1)[:, None]
+        return np.sum((p - origin) * n, 1)
+
+    return (
+        np.array(
+            [
+                proj(c, a, u1) / norm,
+                proj(d, a, u1) / norm,
+                proj(c, a, u2) / norm,
+                proj(d, a, u2) / norm,
+            ]
+        ).T,
+        np.rollaxis(np.array([a, b]), 1),
+    )
 
 
 def clean_quads(xy):
     assert xy.shape[1] == 2
     quads_idxs = np.array(list(combinations(np.arange(xy.shape[0]), 4)))
     quads = xy[quads_idxs]
     ordered_quads = reorder(quads)
```

### Comparing `twirl-0.3.3/twirl/triangles.py` & `twirl-0.4.0/twirl/triangles.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.3/PKG-INFO` & `twirl-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twirl
-Version: 0.3.3
+Version: 0.4.0
 Summary: Astrometric plate solving in Python
 Home-page: https://twirl.readthedocs.io
 License: MIT
 Keywords: astronomy,astrometry,plate-solving
 Author: Lionel J. Garcia
 Author-email: lionel_garcia@live.fr
 Maintainer: Lionel J. Garcia
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: astropy (>=5.1.1,<6.0.0)
 Requires-Dist: astroquery (>=0.4.6,<0.5.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
+Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Project-URL: Repository, https://github.com/lgrcia/twirl
 Description-Content-Type: text/markdown
 
 # twirl
 
 <p align="center">
@@ -59,89 +59,75 @@
 1. detection of stars in the image if not provided
 2. catalog query using image known center
 3. asterisms building and matching
 4. image recombination and wcs fit using astropy.wcs
 
 Astersisms are made of 3 or 4 points. 4 points asterisms are built following Lang et al. 2009 while 3 points asterims are based on an original algorithm.
 
----
-
 ## Installation
 
 twirl can be installed using pip:
 
 ```shell
 pip install twirl
 ```
 
 or using poetry:
 
 ```shell
 poetry add twirl
 ```
 
----
-
 ## Example Usage
 
-twirl is designed to be complementary to the astropy package. It is used to compute a WCS from a set of stars detected in an image. 
-
-As a prerequisite, star detection and plate solving is suited for when the image center and field of view are known. 
+*twirl* is designed to be complementary to the *astropy* package. It is used to compute a WCS by matching an image detected stars with catalog stars. To query the catalog stars, the center coordinates of the image must be known, as well as the size of the field of view. If not available, the latter can be computed using the known pixel scale of the detector.
 
-In this case, the image center and field of view can be provided as a SkyCoord object and a Quantity object respectively.
-
-Use any specified header that has been stored on the FITS primary HDU to obtain the center equatorial coordinate and field of view, for this example we will assum "RA" and "DEC" are the keywords for the center equatorial coordinate.
-
-### Setup
+Hence, the process starts by extracting the image RA-DEC center equatorial coordinate and compute the instrument field of view
 
 ```python
 import numpy as np
 
 from astropy.io import fits
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 
-# Open some FITS image: 
-hdul = fits.open("...")
-
-# ra, dec in degrees
-ra, dec = header["RA"], header["DEC"]
+# Open some FITS image
+hdu = fits.open("...")[0]
 
-# Provide the center as a SkyCoord object:
+# get the center of the image
+ra, dec = hdu.header["RA"], hdu.header["DEC"]
 center = SkyCoord(ra, dec, unit=["deg", "deg"])
 
-center = [center.ra.value, center.dec.value]
+# and the size of its field of view
+pixel = 0.66 * u.arcsec  # known pixel scale
+shape = hdu.data.shape
+fov = np.max(shape) * pixel.to(u.deg)
+```
 
-# Utilise the image shape and pixel size in arcseconds " to obtain the field of view in degrees:
-shape = data.shape
+We can then query the gaia stars in the field using this information
 
-# Pixel size in arcseconds:
-pixel = 0.66 * u.arcsec
+```python
+import twirl
 
-# Field of view in degrees:
-fov = np.max(shape)*pixel.to(u.deg).value
+sky_coords = twirl.gaia_radecs(center, 1.2 * fov)[0:12]
 ```
 
-From here, we can pass the data, the center equatorial coordinate and the field-of-view to twirl to compute the World Coordinate System (WCS):
-
-### Twirl Usage
+and match the queried stars to stars detected in the image
 
 ```python
-import twirl
-
-# Find some starts in the image:
-stars = twirl.find_peaks(data)[0:15]
+# detect stars in the image
+pixel_coords = twirl.find_peaks(hdu.data)[0:12]
 
-# Compute the World Coordinate System:
-wcs = twirl.compute_wcs(stars, center, fov)
+# compute the World Coordinate System
+wcs = twirl.compute_wcs(pixel_coords, sky_coords)
 ```
+leading to a World Coordinate System object.
 
-A more complete example is provided in [docs/notebooks](https://github.com/lgrcia/twirl/tree/master/docs/notebooks)
+A more complete example is provided in [docs/ipynb/wcs.ipynb](https://twirl.readthedocs.io/en/latest/ipynb/wcs.html)
 
----
 
 ## Development
 
 ### Project Requirements
 
 - [Python](https://www.python.org/) 3.11.*
 - [Poetry](https://python-poetry.org/) for Python package and environment management.
@@ -168,15 +154,14 @@
 
 ```console
 $ poetry install
 ```
 
 **N.B.** _Ensure that any dependency changes are committed to source control, so everyone has a consistenct package dependecy list._
 
----
 
 ## Acknowledgements
 
 This package has made use of the algorithm from
 
 Lang, D. et al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary Astronomical Images_. The Astronomical Journal, 139(5), pp.1782–1800. [doi:10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-6256/139/5/1782).
```

#### html2text {}

```diff
@@ -1,73 +1,70 @@
-Metadata-Version: 2.1 Name: twirl Version: 0.3.3 Summary: Astrometric plate
+Metadata-Version: 2.1 Name: twirl Version: 0.4.0 Summary: Astrometric plate
 solving in Python Home-page: https://twirl.readthedocs.io License: MIT
 Keywords: astronomy,astrometry,plate-solving Author: Lionel J. Garcia Author-
 email: lionel_garcia@live.fr Maintainer: Lionel J. Garcia Maintainer-email:
 lionel_garcia@live.fr Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: docs
 Requires-Dist: astropy (>=5.1.1,<6.0.0) Requires-Dist: astroquery
 (>=0.4.6,<0.5.0) Requires-Dist: matplotlib (>=3.6.2,<4.0.0) Requires-Dist:
 numpy (>=1.23.5,<2.0.0) Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-
-Dist: scikit-image (>=0.19.3,<0.20.0) Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Dist: scikit-image (>=0.21.0,<0.22.0) Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Project-URL: Repository, https://github.com/lgrcia/twirl Description-Content-
 Type: text/markdown # twirl
       [https://github.com/lgrcia/twirl/blob/main/docs/_static/twirl.png]
                  Python package for astrometric plate solving
                   [github] [license] [paper] [documentation]
 twirl is an astrometric plate solving package for Python. It is suited for
 cases where the Right Ascension and Declination (RA, dec) coordinates of the
 image center and the field of view is known, computing a World Coordinate
 System (WCS) based on GAIA reference stars. twirl compute a WCS following these
 steps: 1. detection of stars in the image if not provided 2. catalog query
 using image known center 3. asterisms building and matching 4. image
 recombination and wcs fit using astropy.wcs Astersisms are made of 3 or 4
 points. 4 points asterisms are built following Lang et al. 2009 while 3 points
-asterims are based on an original algorithm. --- ## Installation twirl can be
+asterims are based on an original algorithm. ## Installation twirl can be
 installed using pip: ```shell pip install twirl ``` or using poetry: ```shell
-poetry add twirl ``` --- ## Example Usage twirl is designed to be complementary
-to the astropy package. It is used to compute a WCS from a set of stars
-detected in an image. As a prerequisite, star detection and plate solving is
-suited for when the image center and field of view are known. In this case, the
-image center and field of view can be provided as a SkyCoord object and a
-Quantity object respectively. Use any specified header that has been stored on
-the FITS primary HDU to obtain the center equatorial coordinate and field of
-view, for this example we will assum "RA" and "DEC" are the keywords for the
-center equatorial coordinate. ### Setup ```python import numpy as np from
-astropy.io import fits from astropy import units as u from astropy.coordinates
-import SkyCoord # Open some FITS image: hdul = fits.open("...") # ra, dec in
-degrees ra, dec = header["RA"], header["DEC"] # Provide the center as a
-SkyCoord object: center = SkyCoord(ra, dec, unit=["deg", "deg"]) center =
-[center.ra.value, center.dec.value] # Utilise the image shape and pixel size in
-arcseconds " to obtain the field of view in degrees: shape = data.shape # Pixel
-size in arcseconds: pixel = 0.66 * u.arcsec # Field of view in degrees: fov =
-np.max(shape)*pixel.to(u.deg).value ``` From here, we can pass the data, the
-center equatorial coordinate and the field-of-view to twirl to compute the
-World Coordinate System (WCS): ### Twirl Usage ```python import twirl # Find
-some starts in the image: stars = twirl.find_peaks(data)[0:15] # Compute the
-World Coordinate System: wcs = twirl.compute_wcs(stars, center, fov) ``` A more
-complete example is provided in [docs/notebooks](https://github.com/lgrcia/
-twirl/tree/master/docs/notebooks) --- ## Development ### Project Requirements -
-[Python](https://www.python.org/) 3.11.* - [Poetry](https://python-poetry.org/
-) for Python package and environment management. ### Installing Dependencies
-The twirl project manages Python package dependencies using [Poetry](https://
-python-poetry.org/). You'll need to follow the instructions for installation
-there. Then you can start a shell session with the new environment with:
-```console $ poetry shell ``` **N.B.** For development with vscode you will
-need to run the following command: ```console $ poetry config virtualenvs.in-
-project true ``` This will installed the poetry `.venv` in the root of the
-project and allow vscode to setup the environment correctly for development. To
-start development, install all of the dependencies as: ```console $ poetry
-install ``` **N.B.** _Ensure that any dependency changes are committed to
-source control, so everyone has a consistenct package dependecy list._ --- ##
-Acknowledgements This package has made use of the algorithm from Lang, D. et
-al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary
-Astronomical Images_. The Astronomical Journal, 139(5), pp.1782â1800. [doi:
-10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-
-6256/139/5/1782). implemented in Garcia, L. J. et al. (2022). prose: a Python
-framework for modular astronomical images processing. MNRAS, vol. 509, no. 4,
-pp. 4817â4828, 2022. [doi:10.1093/mnras/stab3113](https://academic.oup.com/
-mnras/article-abstract/509/4/4817/6414007). See this [documentation page]
-(https://twirl.readthedocs.io/en/latest/md/acknowledgement.html) for the BibTeX
-entries.
+poetry add twirl ``` ## Example Usage *twirl* is designed to be complementary
+to the *astropy* package. It is used to compute a WCS by matching an image
+detected stars with catalog stars. To query the catalog stars, the center
+coordinates of the image must be known, as well as the size of the field of
+view. If not available, the latter can be computed using the known pixel scale
+of the detector. Hence, the process starts by extracting the image RA-DEC
+center equatorial coordinate and compute the instrument field of view ```python
+import numpy as np from astropy.io import fits from astropy import units as u
+from astropy.coordinates import SkyCoord # Open some FITS image hdu = fits.open
+("...")[0] # get the center of the image ra, dec = hdu.header["RA"], hdu.header
+["DEC"] center = SkyCoord(ra, dec, unit=["deg", "deg"]) # and the size of its
+field of view pixel = 0.66 * u.arcsec # known pixel scale shape =
+hdu.data.shape fov = np.max(shape) * pixel.to(u.deg) ``` We can then query the
+gaia stars in the field using this information ```python import twirl
+sky_coords = twirl.gaia_radecs(center, 1.2 * fov)[0:12] ``` and match the
+queried stars to stars detected in the image ```python # detect stars in the
+image pixel_coords = twirl.find_peaks(hdu.data)[0:12] # compute the World
+Coordinate System wcs = twirl.compute_wcs(pixel_coords, sky_coords) ``` leading
+to a World Coordinate System object. A more complete example is provided in
+[docs/ipynb/wcs.ipynb](https://twirl.readthedocs.io/en/latest/ipynb/wcs.html)
+## Development ### Project Requirements - [Python](https://www.python.org/
+) 3.11.* - [Poetry](https://python-poetry.org/) for Python package and
+environment management. ### Installing Dependencies The twirl project manages
+Python package dependencies using [Poetry](https://python-poetry.org/). You'll
+need to follow the instructions for installation there. Then you can start a
+shell session with the new environment with: ```console $ poetry shell ```
+**N.B.** For development with vscode you will need to run the following
+command: ```console $ poetry config virtualenvs.in-project true ``` This will
+installed the poetry `.venv` in the root of the project and allow vscode to
+setup the environment correctly for development. To start development, install
+all of the dependencies as: ```console $ poetry install ``` **N.B.** _Ensure
+that any dependency changes are committed to source control, so everyone has a
+consistenct package dependecy list._ ## Acknowledgements This package has made
+use of the algorithm from Lang, D. et al. (2010). _Astrometry.net: Blind
+Astrometric Calibration of Arbitrary Astronomical Images_. The Astronomical
+Journal, 139(5), pp.1782â1800. [doi:10.1088/0004-6256/139/5/1782](https://
+iopscience.iop.org/article/10.1088/0004-6256/139/5/1782). implemented in
+Garcia, L. J. et al. (2022). prose: a Python framework for modular astronomical
+images processing. MNRAS, vol. 509, no. 4, pp. 4817â4828, 2022. [doi:10.1093/
+mnras/stab3113](https://academic.oup.com/mnras/article-abstract/509/4/4817/
+6414007). See this [documentation page](https://twirl.readthedocs.io/en/latest/
+md/acknowledgement.html) for the BibTeX entries.
```

