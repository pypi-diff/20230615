# Comparing `tmp/prose-3.1.1.tar.gz` & `tmp/prose-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prose-3.1.1.tar", max compression
+gzip compressed data, was "prose-3.2.0.tar", max compression
```

## Comparing `prose-3.1.1.tar` & `prose-3.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1097 2023-05-29 12:33:24.642265 prose-3.1.1/LICENSE
--rw-r--r--   0        0        0     3752 2023-05-29 12:33:24.642265 prose-3.1.1/README.md
--rw-r--r--   0        0        0      651 2023-05-29 12:33:24.746264 prose-3.1.1/prose/__init__.py
--rw-r--r--   0        0        0       84 2023-05-29 12:33:24.746264 prose-3.1.1/prose/archive/__init__.py
--rw-r--r--   0        0        0     2397 2023-05-29 12:33:24.750264 prose-3.1.1/prose/archive/pos1.py
--rw-r--r--   0        0        0     2071 2023-05-29 12:33:24.750264 prose-3.1.1/prose/archive/sdss.py
--rw-r--r--   0        0        0      254 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/__init__.py
--rw-r--r--   0        0        0     3970 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/alignment.py
--rw-r--r--   0        0        0     3680 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/background.py
--rw-r--r--   0        0        0     9026 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/catalogs.py
--rw-r--r--   0        0        0     8768 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/centroids.py
--rw-r--r--   0        0        0    13494 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/detection.py
--rw-r--r--   0        0        0     6717 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/geometry.py
--rw-r--r--   0        0        0     4135 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/photometry.py
--rw-r--r--   0        0        0    13998 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/psf.py
--rw-r--r--   0        0        0     3703 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/shepard.py
--rw-r--r--   0        0        0    20531 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/utils.py
--rw-r--r--   0        0        0     4034 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/visualization.py
--rw-r--r--   0        0        0     4069 2023-05-29 12:33:24.750264 prose-3.1.1/prose/builtins.py
--rw-r--r--   0        0        0    10673 2023-05-29 12:33:24.750264 prose-3.1.1/prose/citations.py
--rw-r--r--   0        0        0     5933 2023-05-29 12:33:24.750264 prose-3.1.1/prose/config.py
--rw-r--r--   0        0        0     3733 2023-05-29 12:33:24.750264 prose-3.1.1/prose/console_utils.py
--rw-r--r--   0        0        0      120 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/__init__.py
--rw-r--r--   0        0        0     3651 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/block.py
--rw-r--r--   0        0        0    24769 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/image.py
--rw-r--r--   0        0        0     9842 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/sequence.py
--rw-r--r--   0        0        0    16539 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/source.py
--rw-r--r--   0        0        0    17451 2023-05-29 12:33:24.750264 prose-3.1.1/prose/fluxes.py
--rw-r--r--   0        0        0      137 2023-05-29 12:33:24.750264 prose-3.1.1/prose/io/__init__.py
--rw-r--r--   0        0        0      686 2023-05-29 12:33:24.750264 prose-3.1.1/prose/io/create_fm_db.sql
--rw-r--r--   0        0        0    25095 2023-05-29 12:33:24.750264 prose-3.1.1/prose/io/fitsmanager.py
--rw-r--r--   0        0        0     6374 2023-05-29 12:33:24.750264 prose-3.1.1/prose/io/io.py
--rw-r--r--   0        0        0    15085 2023-05-29 12:33:24.750264 prose-3.1.1/prose/simulations.py
--rw-r--r--   0        0        0     7901 2023-05-29 12:33:24.750264 prose-3.1.1/prose/telescope.py
--rw-r--r--   0        0        0    14447 2023-05-29 12:33:24.750264 prose-3.1.1/prose/utils.py
--rw-r--r--   0        0        0    29851 2023-05-29 12:33:24.750264 prose-3.1.1/prose/visualization.py
--rw-r--r--   0        0        0     1024 2023-05-29 12:33:24.750264 prose-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 prose-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-06-15 15:57:18.286445 prose-3.2.0/LICENSE
+-rw-r--r--   0        0        0     3752 2023-06-15 15:57:18.286445 prose-3.2.0/README.md
+-rw-r--r--   0        0        0      652 2023-06-15 15:57:18.378447 prose-3.2.0/prose/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-15 15:57:18.378447 prose-3.2.0/prose/archive/__init__.py
+-rw-r--r--   0        0        0     2397 2023-06-15 15:57:18.378447 prose-3.2.0/prose/archive/pos1.py
+-rw-r--r--   0        0        0     2071 2023-06-15 15:57:18.378447 prose-3.2.0/prose/archive/sdss.py
+-rw-r--r--   0        0        0      254 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/__init__.py
+-rw-r--r--   0        0        0     4760 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/alignment.py
+-rw-r--r--   0        0        0     3680 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/background.py
+-rw-r--r--   0        0        0    10501 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/catalogs.py
+-rw-r--r--   0        0        0     8768 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/centroids.py
+-rw-r--r--   0        0        0    13480 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/detection.py
+-rw-r--r--   0        0        0    10037 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/geometry.py
+-rw-r--r--   0        0        0     4135 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/photometry.py
+-rw-r--r--   0        0        0    13998 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/psf.py
+-rw-r--r--   0        0        0     3703 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/shepard.py
+-rw-r--r--   0        0        0    20516 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/utils.py
+-rw-r--r--   0        0        0     4034 2023-06-15 15:57:18.378447 prose-3.2.0/prose/blocks/visualization.py
+-rw-r--r--   0        0        0     4069 2023-06-15 15:57:18.378447 prose-3.2.0/prose/builtins.py
+-rw-r--r--   0        0        0    10673 2023-06-15 15:57:18.378447 prose-3.2.0/prose/citations.py
+-rw-r--r--   0        0        0     5933 2023-06-15 15:57:18.378447 prose-3.2.0/prose/config.py
+-rw-r--r--   0        0        0     3733 2023-06-15 15:57:18.378447 prose-3.2.0/prose/console_utils.py
+-rw-r--r--   0        0        0      120 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/__init__.py
+-rw-r--r--   0        0        0     3651 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/block.py
+-rw-r--r--   0        0        0    24834 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/image.py
+-rw-r--r--   0        0        0     9842 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/sequence.py
+-rw-r--r--   0        0        0    16797 2023-06-15 15:57:18.382447 prose-3.2.0/prose/core/source.py
+-rw-r--r--   0        0        0    17451 2023-06-15 15:57:18.382447 prose-3.2.0/prose/fluxes.py
+-rw-r--r--   0        0        0      137 2023-06-15 15:57:18.382447 prose-3.2.0/prose/io/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-15 15:57:18.382447 prose-3.2.0/prose/io/create_fm_db.sql
+-rw-r--r--   0        0        0    25095 2023-06-15 15:57:18.382447 prose-3.2.0/prose/io/fitsmanager.py
+-rw-r--r--   0        0        0     6374 2023-06-15 15:57:18.382447 prose-3.2.0/prose/io/io.py
+-rw-r--r--   0        0        0    15043 2023-06-15 15:57:18.382447 prose-3.2.0/prose/simulations.py
+-rw-r--r--   0        0        0     7901 2023-06-15 15:57:18.382447 prose-3.2.0/prose/telescope.py
+-rw-r--r--   0        0        0    14009 2023-06-15 15:57:18.382447 prose-3.2.0/prose/utils.py
+-rw-r--r--   0        0        0    29851 2023-06-15 15:57:18.382447 prose-3.2.0/prose/visualization.py
+-rw-r--r--   0        0        0     1030 2023-06-15 15:57:18.382447 prose-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4840 1970-01-01 00:00:00.000000 prose-3.2.0/PKG-INFO
```

### Comparing `prose-3.1.1/LICENSE` & `prose-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/README.md` & `prose-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/__init__.py` & `prose-3.2.0/prose/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 CONFIG = config.ConfigManager()
 CONFIG.check_builtins_changes()
 
 from pkg_resources import get_distribution
 
 from prose import visualization as viz
-from prose.core import Block, FITSImage, Image, Sequence, source
+from prose.core import Block, FITSImage, Image, Sequence, Sources
 from prose.fluxes import Fluxes
 from prose.io.fitsmanager import FitsManager
 from prose.simulations import example_image
 from prose.telescope import Telescope
 
 __version__ = get_distribution("prose").version
```

### Comparing `prose-3.1.1/prose/archive/pos1.py` & `prose-3.2.0/prose/archive/pos1.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/archive/sdss.py` & `prose-3.2.0/prose/archive/sdss.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/blocks/alignment.py` & `prose-3.2.0/prose/blocks/alignment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,116 @@
 import numpy as np
 from astropy.wcs.utils import fit_wcs_from_points
 from skimage.transform import warp
+from twirl.match import count_cross_match
 
+from prose.blocks.geometry import ComputeTransformTwirl
 from prose.core import Block, Image
 
-from .geometry import ComputeTransform, SetAffineTransform
-
-__all__ = ["Align", "AlignReferenceSources", "AlignReferenceWCS"]
+__all__ = ["TransformData", "AlignReferenceSources", "AlignReferenceWCS"]
 
 
 # TODO test inverse
-class Align(Block):
-    def __init__(self, reference, name=None):
-        """Align image data to a reference
+class TransformData(Block):
+    def __init__(self, inverse=False, name=None):
+        """Transform image data using its transform
 
-        |read| :code:`Image.data`
+        |read| :code:`Image.transform`
 
         |modify|
 
         Parameters
         ----------
-        reference: :py:class:`~prose.Image`
-            reference image to align images on
+        inverse: bool, optional
+            whether to apply the inverse of the image transform by default False
         name : str, optional
             name of the block, by default None
         """
         super().__init__(name)
-        self.reference = reference
-        self.compute_transform = ComputeTransform(self.reference)
+        self.inverse = inverse
 
     def run(self, image: Image):
-        self.compute_transform.run(image)
-
-        # if self.inverse:
-        #    transform = transform.inverse
         try:
             image.data = warp(
                 image.data,
-                image.transform.inverse,
+                image.transform if self.inverse else image.transform,
                 cval=np.nanmedian(image.data),
                 output_shape=image.shape,
             )
         except np.linalg.LinAlgError:
             image.discard = True
 
     @property
     def citations(self) -> list:
         return super().citations + ["scikit-image"]
 
 
 class AlignReferenceSources(Block):
-    def __init__(self, reference: Image, name=None, verbose=False):
-        """Set Image sources to reference Image sources, properly aligned
+    def __init__(
+        self,
+        reference: Image,
+        name=None,
+        verbose=False,
+        discard_tolerance=0.8,
+        match_tolerance=5,
+    ):
+        """Set Image sources to reference sources (from a reference Image)
+        aligned to the Image
 
-        |read| :code:`Image.sources`
+        |read| :code:`Image.transform`, :code:`Image.sources`
 
         |write| :code:`Image.sources`
 
         Parameters
         ----------
         reference : Image
             reference image containing sources
         name : _type_, optional
             _description_, by default None
         verbose : bool, optional
             _description_, by default False
+        discard_tolerance: float, optional
+            fraction of sources that needs to be matched before discarding image
+        match_tolerance: float, optional
+            maximum distance between matched sources in pixels, default 5
         """
         super().__init__(name, verbose)
         self.reference_sources = reference.sources
-        self.compute_transform = ComputeTransform(reference)
         self._parallel_friendly = True
+        self.discard_tolerance = discard_tolerance
+        self.match_tolerance = match_tolerance
+        self._transform_block = ComputeTransformTwirl(reference)
 
     def run(self, image: Image):
-        self.compute_transform.run(image)
         if not image.discard:
             sources = self.reference_sources.copy()
+
+            # backwards compatibility
+            if "transform" not in image.computed:
+                self._transform_block.run(image)
+
             new_sources_coords = image.transform.inverse(sources.coords.copy())
 
             # check if alignment potentially failed
-            if (
-                np.abs(
-                    np.std(new_sources_coords) - np.std(self.reference_sources.coords)
+            if self.discard_tolerance is not None:
+                matches = count_cross_match(
+                    new_sources_coords,
+                    image.sources.coords,
+                    tol=self.match_tolerance,
                 )
-                > 100
-            ):
-                image.discard = True
-            else:
-                sources.coords = new_sources_coords
-                image.sources = sources
+                if matches < np.min(
+                    [
+                        self.discard_tolerance * len(image.sources),
+                        len(self.reference_sources),
+                    ]
+                ):
+                    image.discard = True
+
+            sources.coords = new_sources_coords
+            image.sources = sources
 
     @property
     def citations(self) -> list:
         return super().citations + ["scikit-image"]
 
 
 class AlignReferenceWCS(Block):
```

### Comparing `prose-3.1.1/prose/blocks/background.py` & `prose-3.2.0/prose/blocks/background.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/blocks/catalogs.py` & `prose-3.2.0/prose/blocks/catalogs.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 import astropy.units as u
 import numpy as np
 import pandas as pd
 import twirl
 from astropy.coordinates import SkyCoord
 from astropy.time import Time
 from astroquery.mast import Catalogs
+from twirl.geometry import sparsify
 
 from prose import Block
 from prose import visualization as viz
 from prose.core.source import PointSource, Sources
-from prose.utils import cross_match, gaia_query, sparsify
+from prose.utils import cross_match, gaia_query
 
 __all__ = ["GaiaCatalog", "TESSCatalog"]
 
 
 def image_gaia_query(
     image, limit=3000, correct_pm=True, wcs=True, circular=True, fov=None
 ):
@@ -70,21 +71,15 @@
         stars_coords = stars_coords.T
 
         if self.mode == "replace":
             mask = np.all(stars_coords < image.shape[::-1], 1) & np.all(
                 stars_coords > 0, 1
             )
             mask = mask & ~np.any(np.isnan(stars_coords), 1)
-            image.sources = Sources(
-                [
-                    PointSource(coords=s, i=i)
-                    for i, s in enumerate(stars_coords[mask][0 : self.limit])
-                ],
-                source_type="PointSource",
-            )
+            image.sources = Sources(stars_coords[mask][0 : self.limit])
             catalog = catalog.iloc[np.flatnonzero(mask)].reset_index()
 
         elif self.mode == "crossmatch":
             coords_1 = image.sources.coords
             coords_2 = catalog[["x", "y"]].values
 
             _coords_2 = dict(zip(range(len(coords_2)), coords_2))
@@ -117,60 +112,100 @@
 
             catalog = pd.DataFrame(new_df_dict)
 
         image.catalogs[self.catalog_name] = catalog.iloc[0 : self.limit]
 
 
 class PlateSolve(Block):
-    def __init__(
-        self, reference=None, n=30, tolerance=10, radius=1.2, debug=False, **kwargs
-    ):
-        """Plate solve an image using twirl
-
-        |read| :code:`Image.sources`
+    """
+    A block that performs plate solving on an astronomical image using a Gaia catalog.
 
-        |write| :code:`Image.wcs`, :code:`Image.plate_solved_success`
+    Parameters
+    ----------
+    reference : `None` or `~prose.Image`
+        A reference image containing a Gaia catalog to use for plate solving.
+        If `None`, a new catalog will be queried using `image_gaia_query`.
+        Default is `None`.
+    n : int
+        The number of stars from catalog to use for plate solving.
+        Default is 30.
+    tolerance : float, optional
+        The minimum distance between two coordinates to be considered cross-matched
+        (in `pixels` units). This serves to compute the number of coordinates being
+        matched between `radecs` and `pixels` for a given transform.
+        By default 12.
+    radius : `None` or `~astropy.units.Quantity`
+        The search radius (in degrees) for the Gaia catalog.
+        If `None`, the radius will be set to 1/12th of the maximum field of view of the image.
+        Default is `None`.
+    debug : bool
+        If `True`, the image and the matched stars will be plotted for debugging purposes.
+        Default is `False`.
+    quads_tolerance : float, optional
+        The minimum euclidean distance between two quads to be matched and tested.
+        By default 0.1.
+    field : float
+        The field of view to use for the Gaia catalog query, in fraction of the image field of view.
+        Default is 1.2.
+    min_match : float, optional
+        The fraction of `pixels` coordinates that must be matched to stop the search.
+        I.e., if the number of matched points is `>= min_match * len(pixels)`, the
+        search stops and return the found transform. By default 0.7.
+    name : str
+        The name of the block.
+        Default is `None`.
+    """
 
-        Parameters
-        ----------
-        reference : Image, optional
-            _description_, by default None
-        n : int, optional
-            _description_, by default 30
-        tolerance : int, optional
-            _description_, by default 10
-        radius : float, optional
-            _description_, by default 1.2
-        debug : bool, optional
-            _description_, by default False
-        """
-        super().__init__(**kwargs)
-        self.radius = radius * u.arcmin.to("deg")
+    def __init__(
+        self,
+        reference=None,
+        n=30,
+        tolerance=10,
+        radius=None,
+        debug=False,
+        quads_tolerance=0.1,
+        field=1.2,
+        min_match=0.8,
+        name=None,
+    ):
+        super().__init__(name=name)
+        self.radius = radius
         self.n = n
         self.reference = reference
         self.tolerance = tolerance
+        self.quads_tolerance = quads_tolerance
         self.debug = debug
+        self.field = field
+        self.min_match = min_match
 
     def run(self, image):
-        stars = image.sources.coords * image.pixel_scale.to("deg").value
-        stars = sparsify(stars, self.radius) / image.pixel_scale.to("deg").value
+        radius = image.fov.max() / 12 if self.radius is None else self.radius
+        stars = image.sources.coords * image.pixel_scale.to("arcmin").value
+        stars = (
+            sparsify(stars, radius.to("arcmin").value)
+            / image.pixel_scale.to("arcmin").value
+        )
 
         if self.reference is None:
             table = image_gaia_query(
-                image, wcs=False, circular=True, fov=image.fov.max()
+                image, wcs=False, circular=True, fov=image.fov.max() * self.field
             ).to_pandas()
             gaias = np.array([table.ra, table.dec]).T
             gaias = gaias[~np.any(np.isnan(gaias), 1)]
         else:
             gaias = self.reference.catalogs["gaia"][["ra", "dec"]].values
 
-        gaias = sparsify(gaias, self.radius)
+        gaias = sparsify(gaias, radius.to("deg").value)
 
-        new_wcs = twirl._compute_wcs(
-            stars[0 : self.n], gaias[0 : self.n], n=self.n, tolerance=self.tolerance
+        new_wcs = twirl.compute_wcs(
+            stars,
+            gaias[0 : self.n],
+            tolerance=self.tolerance,
+            quads_tolerance=self.quads_tolerance,
+            min_match=self.min_match,
         )
         image.wcs = new_wcs
         coords = np.array(image.wcs.world_to_pixel(SkyCoord(gaias, unit="deg"))).T
         idxs = cross_match(image.sources.coords, coords, return_idxs=True)
         image.computed["plat_solve_success"] = np.count_nonzero(
             ~np.isnan(idxs[:, 1])
         ) / len(gaias)
```

### Comparing `prose-3.1.1/prose/blocks/centroids.py` & `prose-3.2.0/prose/blocks/centroids.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/blocks/detection.py` & `prose-3.2.0/prose/blocks/detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         if self.unit_euler:
             idxs = np.flatnonzero([r.euler_number == 1 for r in regions])
             regions = [regions[i] for i in idxs]
 
         sources = Sources(
             np.array([PointSource.from_region(region) for region in regions])
         )
-        image.sources = Sources(self.clean(sources), source_type="PointSource")
+        image.sources = Sources(self.clean(sources), type="PointSource")
 
 
 class TraceDetection(_SourceDetection):
     def __init__(self, minor_length=5, **kwargs):
         """Detect trace sources  (as :py:class:`~prose.core.source.TraceSource`)
 
         Parameters
@@ -285,15 +285,15 @@
         super().__init__(n=n_stars, sort=sort, min_separation=min_separation, name=name)
 
     def run(self, image):
         coordinates, peaks = self.detect(image)
         sources = np.array(
             [PointSource(coords=c, peak=p) for c, p in zip(coordinates, peaks)]
         )
-        image.sources = Sources(self.clean(sources), source_type="PointSource")
+        image.sources = Sources(self.clean(sources), type="PointSource")
 
 
 class DAOFindStars(_SimplePointSourceDetection):
     """
     DAOPHOT stars detection with :code:`photutils` implementation.
 
     |write| ``Image.stars_coords`` and ``Image.peaks``
```

### Comparing `prose-3.1.1/prose/blocks/photometry.py` & `prose-3.2.0/prose/blocks/photometry.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/blocks/psf.py` & `prose-3.2.0/prose/blocks/psf.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/blocks/shepard.py` & `prose-3.2.0/prose/blocks/shepard.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/blocks/utils.py` & `prose-3.2.0/prose/blocks/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         TODO
 
         """
         super().__init__(name=name)
         new_getters = {}
 
         def get_from_header(image, key=None):
-            return image.fits_header[key]
+            return image.header[key]
 
         def get(image, key=None):
             return getattr(image, key)
 
         for attr in attributes:
             if "keyword:" in attr:
                 attr = attr.split("keyword:")[-1]
@@ -583,18 +583,18 @@
 
         self.files = []
 
     def run(self, image):
         self.destination.mkdir(exist_ok=True, parents=True)
 
         new_hdu = fits.PrimaryHDU(image.data)
-        new_hdu.header = image.fits_header
+        new_hdu.header = image.header
 
         if self.imtype is not None:
-            image.fits_header[image.telescope.keyword_image_type] = self.imtype
+            image.header[image.telescope.keyword_image_type] = self.imtype
 
         fits_new_path = self.destination / (
             Path(image.metadata["path"]).stem + f"_{self.label}.fits"
         )
 
         new_hdu.writeto(fits_new_path, overwrite=self.overwrite)
         self.files.append(fits_new_path)
```

### Comparing `prose-3.1.1/prose/blocks/visualization.py` & `prose-3.2.0/prose/blocks/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/builtins.py` & `prose-3.2.0/prose/builtins.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/citations.py` & `prose-3.2.0/prose/citations.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/config.py` & `prose-3.2.0/prose/config.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/console_utils.py` & `prose-3.2.0/prose/console_utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/core/block.py` & `prose-3.2.0/prose/core/block.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/core/image.py` & `prose-3.2.0/prose/core/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pickle
 from copy import deepcopy
 from dataclasses import asdict, dataclass
 from datetime import timedelta
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 
 import astropy.units as u
 import matplotlib.pyplot as plt
 import numpy as np
 from astropy.coordinates import Angle, SkyCoord
 from astropy.io import fits
 from astropy.io.fits.hdu.base import _BaseHDU
@@ -30,36 +30,36 @@
     """
     Image object containing image data and metadata.
 
     This is a Python Data Class, so that most attributes described below can be used as
     keyword-arguments when instantiated.
     """
 
-    data: np.ndarray = None
+    data: Optional[np.ndarray] = None
     """Image data"""
 
-    metadata: dict = None
+    metadata: Optional[dict] = None
     """Image metadata"""
 
-    catalogs: dict = None
+    catalogs: Optional[dict] = None
     """Catalogs associated with the image contained in a dictionary of 
     pandas dataframes"""
 
-    _sources: Union[Sources, dict] = None
+    _sources: Optional[Union[Sources, dict]] = None
 
     origin: tuple = (0, 0)
     """Image origin"""
 
     discard: bool = False
     """Whether image as been discarded by a block"""
 
-    computed: dict = None
+    computed: Optional[dict] = None
     """A dictionary containing any user and block-defined attributes"""
 
-    header: Header = None
+    header: Optional[Header] = None
     """FITS header associated with the image (optional)"""
 
     _wcs = None
 
     def __post_init__(self):
         assert (
             isinstance(self.data, np.ndarray) or self.data is None
@@ -713,15 +713,15 @@
                 "pixel_scale_unit": "arcsec",
             }
         )
 
     image = Image(values, metadata, {})
     if image.metadata["jd"] is None:
         image.metadata["jd"] = Time(image.date).jd
-    image.fits_header = header
+    image.header = header
     if not skip_wcs:
         image.wcs = WCS(header)
     image.telescope = telescope
 
     return image
```

### Comparing `prose-3.1.1/prose/core/sequence.py` & `prose-3.2.0/prose/core/sequence.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/core/source.py` & `prose-3.2.0/prose/core/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,26 +493,35 @@
 
     def annulus(self, r0=1.05, r1=1.4, scale=True):
         return self.rectangular_annulus(r0, r1, scale=scale)
 
 
 @dataclass
 class Sources:
-    sources: Union[list, np.ndarray] = None
-    source_type: Literal["PointSource", None] = None
+    sources: list = None
+    """List of sources"""
+    type: Literal["PointSource", None] = None
+    """Source type"""
 
     def __post_init__(self):
         if self.sources is None:
             self.sources = []
 
-        if self.source_type is not None:
+        if isinstance(self.sources, np.ndarray):
+            if self.sources.dtype != object:
+                self.sources = [
+                    PointSource(coords=s, i=i) for i, s in enumerate(self.sources)
+                ]
+                self.type = "PointSource"
+
+        if self.type is not None:
             for s in self.sources:
                 assert (
-                    s.__class__.__name__ == self.source_type
-                ), f"list can only contain {self.source_type}"
+                    s.__class__.__name__ == self.type
+                ), f"list can only contain {self.type}"
         self.sources = np.array(self.sources)
 
     def __getitem__(self, i):
         if np.isscalar(i):
             i = int(i)
             return self.sources[i]
         else:
@@ -539,21 +548,21 @@
 
     @coords.setter
     def coords(self, new_coords):
         for source, new_coord in zip(self.sources, new_coords):
             source.coords = new_coord
 
     def apertures(self, r, scale=False):
-        if self.source_type == "PointSource":
+        if self.type == "PointSource":
             return CircularAperture(self.coords, r)
         else:
             return [source.aperture(r, scale=scale) for source in self.sources]
 
     def annulus(self, rin, rout, scale=False):
-        if self.source_type == "PointSource":
+        if self.type == "PointSource":
             return CircularAnnulus(self.coords, rin, rout)
         else:
             return [source.annulus(rin, rout, scale=scale) for source in self.sources]
 
     def plot(self, *args, **kwargs):
         for s in self.sources:
             s.plot(*args, **kwargs)
```

### Comparing `prose-3.1.1/prose/fluxes.py` & `prose-3.2.0/prose/fluxes.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/io/create_fm_db.sql` & `prose-3.2.0/prose/io/create_fm_db.sql`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/io/fitsmanager.py` & `prose-3.2.0/prose/io/fitsmanager.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/io/io.py` & `prose-3.2.0/prose/io/io.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/simulations.py` & `prose-3.2.0/prose/simulations.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,25 +32,26 @@
         for f, (x0, y0) in zip(_fluxes, _coords):
             im[int(x0), int(y0)] += f
         Im = Image(im, metadata={"jd": None})
         images.append(Im)
     return images
 
 
-def fits_image(data, header, destination):
+def fits_image(data, header, destination, **kwargs):
     header = dict(
         TELESCOP=header.get("TELESCOP", "fake"),
         EXPTIME=header.get("EXPTIME", 1),
         FILTER=header.get("FILTER", ""),
         OBJECT=header.get("OBJECT", "prose"),
         IMAGETYP=header.get("IMAGETYP", "light"),
         AIRMASS=header.get("AIRMASS", 1),
         JD=header.get("JD", 0),
         RA=header.get("RA", 12.84412),
         DEC=header.get("DEC", -22.85886),
+        **kwargs,
     )
     header["DATE-OBS"] = header.get("DATE-OBS", Time(datetime.now()).to_value("fits"))
     hdu = fits.PrimaryHDU(data, header=fits.Header(header))
     hdu.writeto(destination, overwrite=True)
 
 
 def cutouts(image, stars, size):
@@ -235,75 +236,79 @@
                 )
                 < radius
             ).flatten(),
             self.target,
         )
         self.remove_stars(close_by)
 
-    def save_fits(self, destination, calibration=False, verbose=True):
+    def save_fits(self, destination, calibration=False, verbose=True, **kwargs):
         progress = lambda x: tqdm(x) if verbose else x
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
 
         if not path.exists(destination):
             os.makedirs(destination)
 
-            for i, time in enumerate(progress(self.time)):
-                with warnings.catch_warnings():
-                    warnings.simplefilter("ignore")
-                    date = Time(time, format="jd", scale="utc").to_value("fits")
-                    im = self.image(i, 300)
-                    fits_image(
-                        im,
-                        {
-                            "TELESCOP": self.telescope.name,
-                            "JD": time,
-                            "DATE-OBS": date,
-                            "FILTER": "a",
-                        },
-                        path.join(destination, f"fake-im-{i}.fits"),
-                    )
-
-            if calibration:
+        for i, time in enumerate(progress(self.time)):
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                date = Time(time, format="jd", scale="utc").to_value("fits")
+                im = self.image(i, 300)
                 fits_image(
-                    np.zeros_like(im),
+                    im,
                     {
                         "TELESCOP": self.telescope.name,
                         "JD": time,
                         "DATE-OBS": date,
-                        "IMAGETYP": "dark",
+                        "FILTER": "a",
                     },
-                    path.join(destination, f"fake-dark.fits"),
+                    path.join(destination, f"fake-im-{i}.fits"),
+                    **kwargs,
                 )
 
+        if calibration:
+            fits_image(
+                np.zeros_like(im),
+                {
+                    "TELESCOP": self.telescope.name,
+                    "JD": time,
+                    "DATE-OBS": date,
+                    "IMAGETYP": "dark",
+                },
+                path.join(destination, f"fake-dark.fits"),
+                **kwargs,
+            )
+
+            fits_image(
+                np.zeros_like(im),
+                {
+                    "TELESCOP": self.telescope.name,
+                    "JD": time,
+                    "DATE-OBS": date,
+                    "IMAGETYP": "bias",
+                },
+                path.join(destination, f"fake-C001-bias.fits"),
+                **kwargs,
+            )
+
+            for i in range(0, 4):
                 fits_image(
-                    np.zeros_like(im),
+                    np.ones_like(im),
                     {
                         "TELESCOP": self.telescope.name,
                         "JD": time,
                         "DATE-OBS": date,
-                        "IMAGETYP": "bias",
+                        "IMAGETYP": "flat",
+                        "FILTER": "a",
                     },
-                    path.join(destination, f"fake-C001-bias.fits"),
+                    path.join(destination, f"fake-flat-{i}.fits"),
+                    **kwargs,
                 )
 
-                for i in range(0, 4):
-                    fits_image(
-                        np.ones_like(im),
-                        {
-                            "TELESCOP": self.telescope.name,
-                            "JD": time,
-                            "DATE-OBS": date,
-                            "IMAGETYP": "flat",
-                            "FILTER": "a",
-                        },
-                        path.join(destination, f"fake-flat-{i}.fits"),
-                    )
-
 
 def xo_lightcurve(time, period=3, r=0.1, t0=0, plot=False):
     import exoplanet as xo
 
     orbit = xo.orbits.KeplerianOrbit(period=0.7, t0=0.1)
     light_curve = (
         xo.LimbDarkLightCurve([0.1, 0.4])
```

### Comparing `prose-3.1.1/prose/telescope.py` & `prose-3.2.0/prose/telescope.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/prose/utils.py` & `prose-3.2.0/prose/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,29 +405,14 @@
             f"dec BETWEEN {dec-dec_fov/2} AND {dec+dec_fov/2} "
             "order by phot_g_mean_mag"
         )
 
     return job.get_results()
 
 
-def sparsify(stars, radius):
-    _stars = stars.copy()
-    deleted_stars = np.zeros([], dtype=int)
-    sparse_stars = []
-
-    for i, s in enumerate(_stars):
-        if not i in deleted_stars:
-            distances = np.linalg.norm(_stars - s, axis=1)
-            idxs = np.flatnonzero(distances < radius)
-            sparse_stars.append(s)
-            deleted_stars = np.hstack([deleted_stars, idxs])
-
-    return np.array(sparse_stars)
-
-
 def full_class_name(o):
     # https://stackoverflow.com/questions/2020014/get-fully-qualified-class-name-of-an-object-in-python
     klass = o.__class__
     module = klass.__module__
     if module == "builtins":
         return klass.__qualname__  # avoid outputs like 'builtins.str'
     return module + "." + klass.__qualname__
```

### Comparing `prose-3.1.1/prose/visualization.py` & `prose-3.2.0/prose/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.1/pyproject.toml` & `prose-3.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prose"
-version = "3.1.1"
+version = "3.2.0"
 description = "Modular image processing pipelines for Astronomy"
 authors = ["Lionel Garcia"]
 license = "MIT"
 readme = "README.md"
 include = ["prose/io/*.sql"]
 
 [tool.poetry.dependencies]
@@ -12,23 +12,23 @@
 numpy = "^1.23.5"
 astropy = "^5.1.1"
 astroquery = "^0.4.6"
 requests = "^2.31.0"
 ipython = "*"
 scipy = "*"
 matplotlib = "*"
-scikit-image = "*"
+scikit-image = "^0.21.0"
 pandas = ">1.1"
 tqdm = "*"
 photutils = "^1.6.0"
 pyyaml = "*"
 tabulate = "*"
 sep = "*"
 celerite2 = "*"
-twirl = "0.1.3"
+twirl = "0.4.0"
 multiprocess = "*"
 pytest = "*"
 imageio = { version = "*", extras = ["ffmpeg"] }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 black = "*"
```

### Comparing `prose-3.1.1/PKG-INFO` & `prose-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prose
-Version: 3.1.1
+Version: 3.2.0
 Summary: Modular image processing pipelines for Astronomy
 License: MIT
 Author: Lionel Garcia
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -20,20 +20,20 @@
 Requires-Dist: multiprocess
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>1.1)
 Requires-Dist: photutils (>=1.6.0,<2.0.0)
 Requires-Dist: pytest
 Requires-Dist: pyyaml
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: scikit-image
+Requires-Dist: scikit-image (>=0.21.0,<0.22.0)
 Requires-Dist: scipy
 Requires-Dist: sep
 Requires-Dist: tabulate
 Requires-Dist: tqdm
-Requires-Dist: twirl (==0.1.3)
+Requires-Dist: twirl (==0.4.0)
 Description-Content-Type: text/markdown
 
 # prose
 
 <p align="center" style="margin-bottom:-50px">
     <img src="docs/_static/prose3.png" width="450">
 </p>
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: prose Version: 3.1.1 Summary: Modular image
+Metadata-Version: 2.1 Name: prose Version: 3.2.0 Summary: Modular image
 processing pipelines for Astronomy License: MIT Author: Lionel Garcia Requires-
 Python: >=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: astropy (>=5.1.1,<6.0.0) Requires-
 Dist: astroquery (>=0.4.6,<0.5.0) Requires-Dist: celerite2 Requires-Dist:
 imageio[ffmpeg] Requires-Dist: ipython Requires-Dist: matplotlib Requires-Dist:
 multiprocess Requires-Dist: numpy (>=1.23.5,<2.0.0) Requires-Dist: pandas
 (>1.1) Requires-Dist: photutils (>=1.6.0,<2.0.0) Requires-Dist: pytest
 Requires-Dist: pyyaml Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
-scikit-image Requires-Dist: scipy Requires-Dist: sep Requires-Dist: tabulate
-Requires-Dist: tqdm Requires-Dist: twirl (==0.1.3) Description-Content-Type:
-text/markdown # prose
+scikit-image (>=0.21.0,<0.22.0) Requires-Dist: scipy Requires-Dist: sep
+Requires-Dist: tabulate Requires-Dist: tqdm Requires-Dist: twirl (==0.4.0)
+Description-Content-Type: text/markdown # prose
                            [docs/_static/prose3.png]
                Modular image processing pipelines for Astronomy
                   [github] [license] [paper] [documentation]
 *prose* is a Python package to build image processing pipelines for Astronomy.
 Beyond featuring the blocks to build pipelines from scratch, it provides pre-
 implemented ones to perform common tasks such as automated calibration,
 reduction and photometry. *powered by [astropy](https://www.astropy.org/) and
```

