# Comparing `tmp/EveryStamp-1.2.0.tar.gz` & `tmp/EveryStamp-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/frits/EveryStamp/dist/.tmp-uma_3dw6/EveryStamp-1.2.0.tar", last modified: Sun Mar 19 16:21:49 2023, max compression
+gzip compressed data, was "EveryStamp-1.3.0.tar", last modified: Thu Jun 15 12:26:58 2023, max compression
```

## Comparing `EveryStamp-1.2.0.tar` & `EveryStamp-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 frits     (1000) frits     (1000)        0 2023-03-19 16:21:49.116090 EveryStamp-1.2.0/
--rw-r--r--   0 frits     (1000) frits     (1000)      563 2023-03-19 16:21:49.113090 EveryStamp-1.2.0/PKG-INFO
--rw-r--r--   0 frits     (1000) frits     (1000)      155 2023-03-10 09:07:03.000000 EveryStamp-1.2.0/README.md
--rw-r--r--   0 frits     (1000) frits     (1000)      871 2023-03-18 12:05:57.000000 EveryStamp-1.2.0/pyproject.toml
--rw-r--r--   0 frits     (1000) frits     (1000)       38 2023-03-19 16:21:49.117090 EveryStamp-1.2.0/setup.cfg
-drwxr-xr-x   0 frits     (1000) frits     (1000)        0 2023-03-19 16:21:49.092090 EveryStamp-1.2.0/src/
-drwxr-xr-x   0 frits     (1000) frits     (1000)        0 2023-03-19 16:21:49.104091 EveryStamp-1.2.0/src/EveryStamp.egg-info/
--rw-r--r--   0 frits     (1000) frits     (1000)      563 2023-03-19 16:21:49.000000 EveryStamp-1.2.0/src/EveryStamp.egg-info/PKG-INFO
--rw-r--r--   0 frits     (1000) frits     (1000)      441 2023-03-19 16:21:49.000000 EveryStamp-1.2.0/src/EveryStamp.egg-info/SOURCES.txt
--rw-r--r--   0 frits     (1000) frits     (1000)        1 2023-03-19 16:21:49.000000 EveryStamp-1.2.0/src/EveryStamp.egg-info/dependency_links.txt
--rw-r--r--   0 frits     (1000) frits     (1000)       58 2023-03-19 16:21:49.000000 EveryStamp-1.2.0/src/EveryStamp.egg-info/entry_points.txt
--rw-r--r--   0 frits     (1000) frits     (1000)      109 2023-03-19 16:21:49.000000 EveryStamp-1.2.0/src/EveryStamp.egg-info/requires.txt
--rw-r--r--   0 frits     (1000) frits     (1000)       11 2023-03-19 16:21:49.000000 EveryStamp-1.2.0/src/EveryStamp.egg-info/top_level.txt
-drwxr-xr-x   0 frits     (1000) frits     (1000)        0 2023-03-19 16:21:49.109090 EveryStamp-1.2.0/src/everystamp/
--rw-r--r--   0 frits     (1000) frits     (1000)        0 2023-03-10 09:07:03.000000 EveryStamp-1.2.0/src/everystamp/__init__.py
--rw-r--r--   0 frits     (1000) frits     (1000)    24548 2023-03-19 16:20:01.000000 EveryStamp-1.2.0/src/everystamp/downloaders.py
--rw-r--r--   0 frits     (1000) frits     (1000)    24392 2023-03-19 16:19:50.000000 EveryStamp-1.2.0/src/everystamp/everystamp.py
--rw-r--r--   0 frits     (1000) frits     (1000)     5775 2023-03-19 16:20:03.000000 EveryStamp-1.2.0/src/everystamp/plotters.py
-drwxr-xr-x   0 frits     (1000) frits     (1000)        0 2023-03-19 16:21:49.111091 EveryStamp-1.2.0/src/everystamp/tonemapping/
--rw-r--r--   0 frits     (1000) frits     (1000)      805 2023-03-10 09:07:03.000000 EveryStamp-1.2.0/src/everystamp/tonemapping/__init__.py
--rw-r--r--   0 frits     (1000) frits     (1000)    19207 2023-03-18 10:55:08.000000 EveryStamp-1.2.0/src/everystamp/tonemapping/lhdr.py
+drwxrwxr-x   0 sweijen   (1001) sweijen   (1001)        0 2023-06-15 12:26:58.402417 EveryStamp-1.3.0/
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)      563 2023-06-15 12:26:58.402417 EveryStamp-1.3.0/PKG-INFO
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)      155 2023-04-22 13:38:04.000000 EveryStamp-1.3.0/README.md
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)      915 2023-06-15 11:25:38.000000 EveryStamp-1.3.0/pyproject.toml
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)       38 2023-06-15 12:26:58.402417 EveryStamp-1.3.0/setup.cfg
+drwxrwxr-x   0 sweijen   (1001) sweijen   (1001)        0 2023-06-15 12:26:58.398417 EveryStamp-1.3.0/src/
+drwxrwxr-x   0 sweijen   (1001) sweijen   (1001)        0 2023-06-15 12:26:58.402417 EveryStamp-1.3.0/src/EveryStamp.egg-info/
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)      563 2023-06-15 12:26:58.000000 EveryStamp-1.3.0/src/EveryStamp.egg-info/PKG-INFO
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)      441 2023-06-15 12:26:58.000000 EveryStamp-1.3.0/src/EveryStamp.egg-info/SOURCES.txt
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)        1 2023-06-15 12:26:58.000000 EveryStamp-1.3.0/src/EveryStamp.egg-info/dependency_links.txt
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)       58 2023-06-15 12:26:58.000000 EveryStamp-1.3.0/src/EveryStamp.egg-info/entry_points.txt
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)      144 2023-06-15 12:26:58.000000 EveryStamp-1.3.0/src/EveryStamp.egg-info/requires.txt
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)       11 2023-06-15 12:26:58.000000 EveryStamp-1.3.0/src/EveryStamp.egg-info/top_level.txt
+drwxrwxr-x   0 sweijen   (1001) sweijen   (1001)        0 2023-06-15 12:26:58.402417 EveryStamp-1.3.0/src/everystamp/
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)        0 2023-04-22 13:38:04.000000 EveryStamp-1.3.0/src/everystamp/__init__.py
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)    25120 2023-06-15 11:25:38.000000 EveryStamp-1.3.0/src/everystamp/downloaders.py
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)    24998 2023-06-15 11:25:38.000000 EveryStamp-1.3.0/src/everystamp/everystamp.py
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)     5977 2023-06-15 11:25:38.000000 EveryStamp-1.3.0/src/everystamp/plotters.py
+drwxrwxr-x   0 sweijen   (1001) sweijen   (1001)        0 2023-06-15 12:26:58.402417 EveryStamp-1.3.0/src/everystamp/tonemapping/
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)      805 2023-04-22 13:38:04.000000 EveryStamp-1.3.0/src/everystamp/tonemapping/__init__.py
+-rw-rw-r--   0 sweijen   (1001) sweijen   (1001)    19694 2023-06-15 11:25:38.000000 EveryStamp-1.3.0/src/everystamp/tonemapping/lhdr.py
```

### Comparing `EveryStamp-1.2.0/PKG-INFO` & `EveryStamp-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EveryStamp
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python interface for retrieving FITS or image cutouts from a variety of astronomical surveys.
 Author: Frits Sweijen
 Project-URL: Homepage, https://tikk3r.github.io/EveryStamp/
 Project-URL: Bug Tracker, https://github.com/tikk3r/EveryStamp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `EveryStamp-1.2.0/pyproject.toml` & `EveryStamp-1.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "EveryStamp"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
     { name = "Frits Sweijen" },
 ]
 description = "A Python interface for retrieving FITS or image cutouts from a variety of astronomical surveys."
 requires-python = ">=3.7"
-dependencies = ["astropy", "astroquery", "matplotlib", "panstamps", "Pillow", "python-casacore", "opencv-python", "pyvo", "requests", "scikit-image", "tqdm"]
+dependencies = ["astropy", "aplpy", "astroquery", "matplotlib", "markupsafe<=2.0.1", "numpy<1.23", "panstamps", "Pillow", "python-casacore", "opencv-python", "pyvo", "requests", "scikit-image", "tqdm"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Astronomy",
 ]
```

### Comparing `EveryStamp-1.2.0/src/EveryStamp.egg-info/PKG-INFO` & `EveryStamp-1.3.0/src/EveryStamp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EveryStamp
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python interface for retrieving FITS or image cutouts from a variety of astronomical surveys.
 Author: Frits Sweijen
 Project-URL: Homepage, https://tikk3r.github.io/EveryStamp/
 Project-URL: Bug Tracker, https://github.com/tikk3r/EveryStamp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `EveryStamp-1.2.0/src/everystamp/downloaders.py` & `EveryStamp-1.3.0/src/everystamp/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,19 +142,19 @@
         if (size_pix > 3000) and autoscale:
             # Jump to the next available pixel size by scaling from the (approximate) native pixel scale.
             new_pixscale = pixscale
             new_size_pix = int(size * 3600 / new_pixscale)
             while new_size_pix > 3000:
                 new_pixscale += 0.262
                 new_size_pix = int(size * 3600 / new_pixscale)
-            self.logger.warn('Image size of {:.2f} deg with pixel scale {:.3f} exceeds server limit of 3000 pixels! Automatically adjusting pixel scale to {:.3f} giving {:d} pixels.'.format(size, pixscale, new_pixscale, new_size_pix), Warning, stacklevel=2)
+            self.logger.warn('Image size of {:.2f} deg with pixel scale {:.3f} exceeds server limit of 3000 pixels! Automatically adjusting pixel scale to {:.3f} giving {:d} pixels.'.format(size, pixscale, new_pixscale, new_size_pix), stacklevel=2)
             dlpixscale = new_pixscale
             dlsize_pix = new_size_pix
         elif size_pix > 3000:
-            self.logger.warn('Image size of {:.2f} deg with pixel scale {:.3f} exceeds server limit of 3000 pixels! Image will be truncated! Use --legacy_autoscale or pass autoscale=True to automatically switch pixel scales.'.format(size, pixscale), Warning, stacklevel=2)
+            self.logger.warn('Image size of {:.2f} deg with pixel scale {:.3f} exceeds server limit of 3000 pixels! Image will be truncated! Use --legacy_autoscale or pass autoscale=True to automatically switch pixel scales.'.format(size, pixscale), stacklevel=2)
         return self.url.format(ra=ra, dec=dec, size_pix=dlsize_pix, bands=bands, mode=mode, layer=layer, pixscale=dlpixscale)
 
     def download(self, **kwargs):
         furl = self.format_url(**kwargs)
         self.logger.info('Downloading cutout from %s', furl)
         if not kwargs['ddir']:
             self.logger.info('Download directory not specified, downloading to %s instead', os.getcwd())
@@ -347,15 +347,15 @@
 
         Returns
         -------
         output_fits : str
             Name of the output FITS file.
         '''
         # Define output name
-        output_fits = imname.rstrip('.fits') + '_poststamp.fits'
+        output_fits = os.path.join('/'.join(imname.split('/')[:-1]), 'VLASS_{:.6f}_{:.6f}_'.format(c.ra.value, c.dec.value) + imname.split('/')[-1].rstrip('.fits') + '_poststamp.fits')
         
         # Get header info
         hdu_list = fits.open(imname)
         header = hdu_list[0].header
         data = hdu_list[0].data[0,0,:,:]
         
         # Obtain header and drop useless axes
@@ -567,27 +567,33 @@
     def __init__(self, survey):
         if not survey:
             raise ValueError('SkyView survey cannot be empty.')
         else:
             self.survey = survey
             self.logger = logging.getLogger('EveryStamp:SkyViewDownloader[{:s}]'.format(self.survey))
 
-    def download(self, ra=0.0, dec=0.0, size=0.1, ddir=os.getcwd(), suffix=''):
+    def download(self, ra=0.0, dec=0.0, size=0.1, pixsize=1, ddir=os.getcwd(), suffix=''):
         ''' Download a cutout from the VLASS survey.
 
         Parameters
         ----------
         ra : float
             Right ascension of the coordinate of interest in degrees.
         dec : float
             Declination of the coordinate of interest in degrees    .
         size : float
             Size of the area of interest in degrees.
+        pixsize
+            Pixel size to use for the cutout.
         ddir : str
             Location to download the cutout to.
         '''
         c = SkyCoord(ra, dec, unit='deg')
         
         sv = SkyView()
-
-        hdul = sv.get_images(c, self.survey, radius=size * u.deg)
+        pixsize_deg = pixsize / 3600.
+        pixels = size / pixsize_deg
+        self.logger.info(f'Requesting a {size} x {size} deg cutout of {pixels} x {pixels} pixels.')
+        hdul = sv.get_images(c, self.survey, radius=size * u.deg, pixels=int(pixels))
+        if not hdul:
+            raise ValueError('SkyView did not return a result. If you requested a large cutout, try increasing the pixel size through --skyview_pixsize or reducing the cutout area.')
         hdul[0].writeto(os.path.join(ddir, '{:s}_{:.4f}_{:.4f}_{:.3f}.fits'.format(self.survey.replace(' ', '_'), ra, dec, size)))
```

### Comparing `EveryStamp-1.2.0/src/everystamp/everystamp.py` & `EveryStamp-1.3.0/src/everystamp/everystamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #!/usr/bin/env python
 ''' Python library aiming to provide a wrapper around various astronomical surveys that offer cutouts.'''
-__version__ = '1.2.0'
+__version__ = '1.3.0'
 __author__ = 'Frits Sweijen'
 __license__ = 'GPLv3'
 from typing import Generator
 
 import argparse
 import logging
 logging.basicConfig(format='[%(name)s] %(asctime)s - %(levelname)s: %(message)s', level=logging.INFO)
 logger = logging.getLogger('EveryStamp')
 import os
 import shutil
+import subprocess
 
 from astroquery.skyview import SkyView #type: ignore
 from collections.abc import Iterable
+from everystamp.tonemapping import lhdr
 import astropy.visualization
 import cv2 #type: ignore
 import requests
 
 # Check if LuminanceHDR is installed.
-HAS_LHDR = shutil.which('luminance-hdr-cli')
+HAS_LHDR = lhdr.has_luminance_hdr() #True if not subprocess.getstatusoutput('luminance-hdr-cli') else False
+#HAS_LHDR = shutil.which('luminance-hdr-cli')
 
 
 def flatten(xs: Iterable) -> Generator:
     ''' Generator to flatten a list of nested lists.
 
     Args:
         xs : list
@@ -59,14 +62,15 @@
     required_args.add_argument('--ra', type=float, required=True, help='Right ascension of cutout centre in degrees.')
     required_args.add_argument('--dec', type=float, required=True, help='Declination of cutout centre in degrees.')
     required_args.add_argument('--mode', type=str, required=True, default='jpeg', choices=['jpeg', 'fits', 'both'], help='Image type to retrieve. Can be "jpeg", "fits" or "both" to retrieve either a JPEG image, FITS file or both. Default value is jpeg.')
 
     optional_args = parser.add_argument_group('Optional arguments')
     optional_args.add_argument('--download_dir', type=str, required=False, default=os.getcwd(), dest='ddir', help='Directory to store downloaded files. If not given will download to $PWD.')
     optional_args.add_argument('--size', type=float, required=False, default=0.01, help='Cutout size in degrees.')
+    optional_args.add_argument('--skyview_pixsize', type=float, required=False, default=1.0, help='Pixel size in arcsec for SkyView cutouts.')
 
     legacy_args = parser.add_argument_group('[DESI Legacy Imaging Surveys]')
     legacy_args.add_argument('--legacy_bands', default='grz', type=str, required=False, help='Bands to download. Allowed values are g, r and z. Multiple bands can be specified as a single string. In the case of a JPEG image a colour image will be generated. In the case of a FITS image a FITS cube will be downloaded. Default: grz')
     legacy_args.add_argument('--legacy_layer', type=str, required=False, default='ls-dr9', help='Layer to make a cutout from. Default value is ls-dr9. Examples are ls-dr9, sdss or unwise-neo4. See Legacy documentation for all possibilies.')
     legacy_args.add_argument('--legacy_autoscale', required=False, default=False, action='store_true', help='Automatically change the pixel size if the resulting image would exceed the server maximum of 3000x3000 pixels.')
 
     ps_args = parser.add_argument_group('[Pan-STARRS]')
@@ -96,21 +100,23 @@
     required_args = parser.add_argument_group('Optional arguments')
     required_args.add_argument('--gamma', type=float, default=1.0, required=False, help='Gamma compress (<1) or expand (>1) an image after tone mapping.')
     required_args.add_argument('--CLAHE', action='store_true', default=False, required=False, help='Apply contrast-limited adaptive histogram equalisation.')
     required_args.add_argument('--CLAHE-gridsize', default=5, type=int, required=False, help='Grid size to use for CLAHE.')
     required_args.add_argument('--CLAHE-cliplim', default=1.0, type=float, required=False, help='Clip limit to use for CLAHE.')
     required_args.add_argument('--stretch', default=None, type=str, required=False, choices=['log', 'sqrt', 'squared', 'asinh', 'sinh'], help='Stretch an image with a certian function.')
 
+    required_args.add_argument('--contour_image', default=None, required=False, help='Plot the given image as contours over the main image.')
+
     if HAS_LHDR:
-        required_args.add_argument('--hdr-tonemap', default=None, type=str, choices=['ashikmin', 'drago', 'duran', 'fattal', 'ferradans', 'ferwerda', 'kimkautz', 'lischinski', 'mantiuk06', 'mantiuk08', 'pattanaik', 'reinhard02', 'reinhard05', 'vanhateren'], required=False, help='HDR tonemapping to apply')
+        required_args.add_argument('--hdr-tonemap', default=None, type=str, choices=['ashikhmin', 'drago', 'duran', 'fattal', 'ferradans', 'ferwerda', 'kimkautz', 'lischinski', 'mantiuk06', 'mantiuk08', 'pattanaik', 'reinhard02', 'reinhard05', 'vanhateren'], required=False, help='HDR tonemapping to apply')
 
-        hdr_ashikmin_args = parser.add_argument_group('HDR Tone mapping -- Ashikmin et al. 2002 arguments')
-        hdr_ashikmin_args.add_argument('--ashikmin-eq2', default=True, type=bool, required=False, help='Equation 2?')
-        hdr_ashikmin_args.add_argument('--ashikmin-simple', default=True, type=bool, required=False, help='Simple?')
-        hdr_ashikmin_args.add_argument('--ashikmin-local_threshold', default=None, type=float, required=False, help='Local threshold.')
+        hdr_ashikhmin_args = parser.add_argument_group('HDR Tone mapping -- Ashikhmin et al. 2002 arguments')
+        hdr_ashikhmin_args.add_argument('--ashikhmin-eq2', default=True, type=bool, required=False, help='Equation 2?')
+        hdr_ashikhmin_args.add_argument('--ashikhmin-simple', default=True, type=bool, required=False, help='Simple?')
+        hdr_ashikhmin_args.add_argument('--ashikhmin-local_threshold', default=None, type=float, required=False, help='Local threshold.')
 
         hdr_drago_args = parser.add_argument_group('HDR Tone mapping -- Drago et al. 2003 arguments')
         hdr_drago_args.add_argument('--drago-bias', default=0.85, type=float, required=False, help='Bias parameter controlling the exponent base.')
 
         hdr_fattal_args = parser.add_argument_group('HDR Tone mapping -- Fattal et al. 2002 arguments')
         hdr_fattal_args.add_argument('--fattal-alpha', default=None, type=float, required=False, help='Controls which gradient magnitude is preserved.')
         hdr_fattal_args.add_argument('--fattal-beta', default=None, type=float, required=False, help='Controls local detail enhancement.')
@@ -140,15 +146,15 @@
         hdr_mantiuk06_args.add_argument('--mantiuk06-saturation', default=None, type=float, required=False, help='Saturation factor.')
         hdr_mantiuk06_args.add_argument('--mantiuk06-detail', default=None, type=float, required=False, help='Detail factor.')
         hdr_mantiuk06_args.add_argument('--mantiuk06-contrast_equalisation', default=True, type=bool, required=False, help='Equalise contrast?')
 
         hdr_mantiuk08_args = parser.add_argument_group('HDR Tone mapping -- Mantiuk et al. 2008 arguments')
         hdr_mantiuk08_args.add_argument('--mantiuk08-contrast_enhancement', default=None, type=float, required=False, help='Contrast enhancement factor.')
         hdr_mantiuk08_args.add_argument('--mantiuk08-colour_saturation', default=None, type=float, required=False, help='Colour saturation factor.')
-        hdr_mantiuk08_args.add_argument('--mantiuk08-luminance_level', default=True, type=float, required=False, help='Luminance level.')
+        hdr_mantiuk08_args.add_argument('--mantiuk08-luminance_level', default=0.0, type=float, required=False, help='Luminance level.')
         hdr_mantiuk08_args.add_argument('--mantiuk08-set_luminance', default=True, type=bool, required=False, help='Set luminance level?')
 
         hdr_duran_args = parser.add_argument_group('HDR Tone mapping -- Durand and Dorsey et al. 2002 arguments')
         hdr_duran_args.add_argument('--duran-sigma_spatial', default=None, type=float, required=False, help='Spatial kernel size.')
         hdr_duran_args.add_argument('--duran-sigma_range', default=None, type=float, required=False, help='Range kernel size.')
         hdr_duran_args.add_argument('--duran-base_contrast', default=None, type=float, required=False, help='Base contrast.')
 
@@ -226,62 +232,62 @@
         vd = VODownloader(url='https://vo.astron.nl/tgssadr/q_fits/cutout/siap.xml', name='TGSS')
         vd.download(ra=args.ra, dec=args.dec, size=args.size, ddir=args.ddir)
     else:
         if args.mode == 'both' or args.mode == 'jpeg':
             raise ValueError('SkyView download does not support JPEG (yet).')
         from everystamp.downloaders import SkyViewDownloader
         sd = SkyViewDownloader(args.survey)
-        sd.download(ra=args.ra, dec=args.dec, size=args.size, ddir=args.ddir)
+        sd.download(ra=args.ra, dec=args.dec, size=args.size, pixsize=args.skyview_pixsize, ddir=args.ddir)
 
 
 def _process_args_plot(args):
     ''' Process arguments to the argparse instance for plotting images.
     
     Args:
         parser : ArgumentParser
             ArgumentParser instance to which to add entries.
     '''
     logger.info('Plotting image %s', args.image)
     from everystamp.plotters import BasicFITSPlot, BasicImagePlot
     from everystamp.tonemapping import gamma, make_nonnegative
     import numpy as np
-    from everystamp.tonemapping.lhdr import ashikmin, drago, duran, fattal, ferradans, ferwerda, kimkautz, lischinski, mantiuk06, mantiuk08, reinhard02, reinhard05, pattanaik, vanhateren
+    from everystamp.tonemapping.lhdr import ashikhmin, drago, duran, fattal, ferradans, ferwerda, kimkautz, lischinski, mantiuk06, mantiuk08, reinhard02, reinhard05, pattanaik, vanhateren
     if args.image.lower().endswith('fits'):
         bp = BasicFITSPlot(args.image)
     else:
         # Probably an image format.
         bp = BasicImagePlot(args.image)
     if HAS_LHDR and args.hdr_tonemap:
-        if args.hdr_tonemap == 'ashikmin':
-            logger.info('Tonemapping image with ashikmin')
-            bp.data = ashikmin(bp.data, eq2=args.ashikmin_eq2, simple=args.ashikmin_simple, local_threshold=args.ashikmin_local_threshol)
+        if args.hdr_tonemap == 'ashikhmin':
+            logger.info('Tonemapping image with ashikhmin')
+            bp.data = ashikhmin(bp.data, eq2=args.ashikhmin_eq2, simple=args.ashikhmin_simple, local_threshold=args.ashikhmin_local_threshold)
         if args.hdr_tonemap == 'fattal':
             logger.info('Tonemapping image with fattal')
             bp.data = fattal(bp.data, alpha=args.fattal_alpha, beta=args.fattal_beta, colour_saturation=args.fattal_colour_saturation, noise=args.fattal_noise)
         if args.hdr_tonemap == 'drago':
             logger.info('Tonemapping image with drago')
             bp.data = drago(bp.data, bias=args.drago_bias)
         if args.hdr_tonemap == 'ferradans':
             logger.info('Tonemapping image with ferradans')
-            bp.data = ferradans(bp.data, rho=args.ferradans_rho, inv_alpha=args.ferradans_inv_alpha)
+            bp.data = ferradans(bp.data, rho=args.ferradans_rho, inv_alpha=args.ferradans_inverse_alpha)
         if args.hdr_tonemap == 'ferwerda':
             logger.info('Tonemapping image with ferwerda')
             bp.data = ferwerda(bp.data, multiplier=args.ferwerda_multiplier, luminance_adaptation=args.ferwerda_luminance_adaptation)
         if args.hdr_tonemap == 'kimkautz':
             logger.info('Tonemapping image with kimkautz')
             bp.data = kimkautz(bp.data, c1=args.kimkautz_c1, c2=args.kimkautz_c2)
         if args.hdr_tonemap == 'lischinski':
             logger.info('Tonemapping with lischinski')
             bp.data = lischinski(bp.data, alpha=args.lischinski_alpha)
         if args.hdr_tonemap == 'mantiuk06':
             logger.info('Tonemapping image with mantiuk06')
             bp.data = mantiuk06(bp.data, contrast=args.mantiuk06_contrast, saturation=args.mantiuk06_saturation, detail=args.mantiuk06_detail, contrast_equalisation=args.mantiuk06_contrast_equalisation)
         if args.hdr_tonemap == 'mantiuk08':
             logger.info('Tonemapping image with mantiuk08')
-            bp.data = mantiuk08(bp.data, contrast_enhancement=args.mantiuk08_saturation, colour_saturation=args.mantiuk08_colour_saturation, luminance_level=args.mantiuk08_luminance_level, set_luminance=args.mantiuk08_set_luminance)
+            bp.data = mantiuk08(bp.data, contrast_enhancement=args.mantiuk08_colour_saturation, colour_saturation=args.mantiuk08_colour_saturation, luminance_level=args.mantiuk08_luminance_level, set_luminance=args.mantiuk08_set_luminance)
         if args.hdr_tonemap == 'duran':
             logger.info('Tonemapping image with duran')
             bp.data = duran(bp.data, sigma_spatial=args.duran_sigma_spatial, sigma_range=args.duran_sigma_range, base_contrast=args.duran_base_contrast)
         if args.hdr_tonemap == 'pattanaik':
             logger.info('Tonemapping image with pattanaik')
             bp.data = pattanaik(bp.data, multiplier=args.pattanaik_multiplier, local_tonemap=args.pattanaik_local_tonemap, auto_lum=args.pattanaik_auto_lum, cone_level=args.pattanaik_cone_level, rod_level=args.pattanaik_rod_level)
         if args.hdr_tonemap == 'reinhard02':
@@ -334,18 +340,21 @@
             stretch = astropy.visualization.SquaredStretch()
         elif args.stretch == 'asinh':
             stretch = astropy.visualization.AsinhStretch()
         elif args.stretch == 'sinh':
             stretch = astropy.visualization.SinhStretch()
         bp.data = stretch(bp.data / np.nanmax(bp.data), min)
     
+    if args.contour_image:
+        bp.plot2D(contour_image = args.contour_image)
+    else:
+        bp.plot2D()
     if args.image.lower().endswith('fits'):
         bp.savedata(args.image.replace('.fits', '.tonemapped.fits'))
         bp.plot_noaxes()
-    bp.plot2D()
 
 
 def main():
     '''Main entry point if called as a standalone executable.
     '''
     parser = argparse.ArgumentParser(description='EveryStamp {:s} by {:s}'.format(__version__, __author__))
     parser._action_groups.pop()
@@ -362,8 +371,8 @@
     if args.cmd == 'download':
         _process_args_download(args)
     if args.cmd == 'plot':
         _process_args_plot(args)
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `EveryStamp-1.2.0/src/everystamp/plotters.py` & `EveryStamp-1.3.0/src/everystamp/plotters.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Sub-module for plotting FITS images."""
 import os
 
 from astropy.io import fits
 from astropy.wcs import WCS
 from matplotlib.image import imread
 from matplotlib.pyplot import figure, show
+from typing import Union
 
 import matplotlib.pyplot as plt
+import numpy
 
 
 class BasicFITSPlot():
     """ Creates a basic plot of a FITS file."""
     def __init__(self, fitsname):
         """ Initialise a basic plotting object for 2D FITS files.
         
@@ -23,42 +25,42 @@
         self.fitsimage = fitsname
         self.fitsdata = fits.getdata(fitsname).squeeze()
         if len(self.fitsdata.shape) > 2:
             raise NotImplementedError('Supplied FITS file appears to have dimensions besides RA and DEC. BasicPlot only supports 2D FITS files.')
         self.data = self.fitsdata
         self.wcs = WCS(fits.getheader(fitsname)).celestial
 
-    def plot2D(self, plot_colourbar=False):
+    def plot2D(self, plot_colourbar=False, contour_image: numpy.ndarray = None, contour_levels: Union[int, list] = 7):
         """ Save a 2D plot of the loaded FITS file.
 
         Args:
             plot_colourbar : bool
                 Add a colour bar to the plot.
+            contour_image:
+                Add contours based on this image.
+            contour_levels:
+                Number of contour levels to draw if an integer or contour levels if a list. Defaults to 5.
         """
         figsize = [self.fitsdata.shape[0] // self.dpi, self.fitsdata.shape[1] // self.dpi]
         if figsize[0] < 12:
             figsize[0] = 12
         if figsize[1] < 8:
             figsize[1] = 8
-        fig = figure(figsize=figsize, dpi=self.dpi)
-        try:
-            ax = fig.add_subplot(111, projection=self.wcs)
-            origin='lower'
-        except IndexError:
-            print('WCS from FITS header broken or incompatible, ignoring.')
-            origin='upper'
-            ax = fig.add_subplot(111)
-        if self.data is not None:
-            im = ax.imshow(self.data, origin=origin, interpolation='none')
-        else:
-            ax.imshow(self.fitsdata, origin=origin, interpolation='none')
-        ax.set(xlabel='Right ascension', ylabel='Declination')
+        from aplpy import FITSFigure
+        # hdu = fits.open(self.fitsimage)
+        hdu = fits.PrimaryHDU(header=fits.getheader(self.fitsimage), data=self.data)
+        f = FITSFigure(hdu, figsize=figsize)
+        f.show_grayscale()
+        if contour_image:
+                hdu_c = fits.open(contour_image)
+                # f.show_contour(hdu_c, levels=contour_levels, colors='white', cmap='plasma')
+                f.show_contour(hdu_c, levels=contour_levels, colors='C0')
         if plot_colourbar:
             plt.colorbar(im)
-        fig.savefig(self.fitsimage.replace('fits', 'png'), bbox_inches='tight', dpi=self.dpi)
+        f.savefig(self.fitsimage.replace('fits', 'png'), dpi=self.dpi)
 
     def plot_noaxes(self):
         """ Save a plot of the FITS image without any axes."""
         figsize = [self.fitsdata.shape[0] // self.dpi, self.fitsdata.shape[1] // self.dpi]
         fig = figure(figsize=figsize)
         try:
             ax = fig.add_subplot(111, projection=self.wcs)
```

### Comparing `EveryStamp-1.2.0/src/everystamp/tonemapping/__init__.py` & `EveryStamp-1.3.0/src/everystamp/tonemapping/__init__.py`

 * *Files identical despite different names*

### Comparing `EveryStamp-1.2.0/src/everystamp/tonemapping/lhdr.py` & `EveryStamp-1.3.0/src/everystamp/tonemapping/lhdr.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,25 @@
 
 import os
 import subprocess
 
 from astropy.io import fits
 from PIL import Image
 from skimage import io
+import cv2
 import numpy
+import imageio
 
 BASECOMMAND = 'luminance-hdr-cli'
+if 'EVERYSTAMP_LUMINANCE_HDR' in os.environ:
+    BASECOMMAND = os.environ['EVERYSTAMP_LUMINANCE_HDR']
+
+def has_luminance_hdr():
+    x = subprocess.run(BASECOMMAND, shell=True, env=dict(os.environ), stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    return not x.returncode
 
 
 def run_command(cmd: Union[list, str]) -> None:
     ''' Run a command through subprocess.
     
     Args:
         cmd : list
@@ -44,15 +52,16 @@
         as_gray : bool
             Treat the image as gray scale or not. Default: True.
             
     Returns:
         data : numpy.ndarray
             NumPy array containing the image.
     '''
-    return io.imread(name)
+    # return imageio.imread(name)
+    return io.imread(name, as_gray=as_gray)
     # return io.imread(name, as_gray=as_gray)
 
 
 def _store_tmpfile(data: numpy.ndarray, name: str, header=None) -> str:
     ''' Store the data to tonemap to a temporary FITS file to pass to LuminanceHDR.
     
     Args:
@@ -60,22 +69,25 @@
             NumPy array containing the image.
 
     Returns:
         path : str
             Absolute path to the temporary file.
     '''
     if name.lower().endswith('fits'):
-        fits.writeto(data=data, filename=name, header=header, overwrite=True)
+        print(data.shape)
+        fits.writeto(data=data.squeeze(), filename=name, header=header, overwrite=True)
+    elif name.lower().endswith('exr'):
+        cv2.imwrite(name, data.astype('float32'))
     else:
         im = Image.fromarray(data)
         im.convert(mode='RGB').save(name)
     return os.path.abspath(name)
 
 
-def ashikmin(data, eq2: bool = True, simple: Optional[float] = None, local_threshold: Optional[float] = None) -> numpy.ndarray:
+def ashikhmin(data, eq2: bool = True, simple: Optional[float] = None, local_threshold: Optional[float] = None) -> numpy.ndarray:
     ''' Tonemap the image using the human vision based method described in Ashikmin 2002.
 
     Parameters set to None will take their default values as set in LuminanceHDR.
 
     Args:
         data : numpy.ndarray
             Input data to tonemap.
@@ -86,16 +98,16 @@
         local_threshold : float
             Default: None.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_ashikmin.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_ashikmin.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo ashikmin '
     cmd += f'--tmoAshEq2 {eq2} '
     cmd += f'--tmoAshSimple {simple} '
     if local_threshold is not None:
         cmd += f'--tmoAshLocal {local_threshold} '
     cmd += f'-o {tmpname_out} {tmpname}'
     run_command(cmd.split(' '))
@@ -116,16 +128,16 @@
         bias : float
             Bias the logarithmic base towards lower or higher values. Default: 0.85.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_drago.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_drago.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo drago '
     if bias is not None:
         cmd += f'--tmoDrgBias {bias} '
     cmd += f'-o {tmpname_out} {tmpname}'
     run_command(cmd.split(' '))
     data_tm = _load_tonemapped_tmpdata(tmpname_out)
     # os.remove(tmpname)
@@ -148,16 +160,16 @@
         base_contrast : float
             Base contrast. Default: None.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_durand.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_durand.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo durand '
     if sigma_spatial is not None:
         cmd += f'--tmoDurSigmaS {sigma_spatial} '
     if sigma_range is not None:
         cmd += f'--tmoDurSigmaR {sigma_range} '
     if base_contrast is not None:
         cmd += f'--tmoDurBase {base_contrast} '
@@ -186,16 +198,16 @@
         noise : float
             Controls the threshold for what is seen as noise, where detail enhancement is reduced.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_fattal.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_fattal.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo fattal '
     if alpha is not None:
         cmd += f'--tmoFatAlpha {alpha} '
     if beta is not None:
         cmd += f'--tmoFatBeta {beta} '
     if colour_saturation is not None:
         cmd += f'--tmoFatAlpha {colour_saturation} '
@@ -222,16 +234,16 @@
         beta : float
             Controls detail enhancement. Larger values yield more detail enhancement. Default is 5.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_ferradans.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_ferradans.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo ferradans '
     if rho is not None:
         cmd += f'--tmoFerRho {rho} '
     if inv_alpha is not None:
         cmd += f'--tmoFerInvAlpha {inv_alpha} '
     cmd += f'-o {tmpname_out} {tmpname}'
     run_command(cmd.split(' '))
@@ -254,16 +266,16 @@
         luminance_adaptation : float
             Default is None.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_ferwerda.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_ferwerda.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo ferradans '
     if multiplier is not None:
         cmd += f'--tmoFerwerdaMul {multiplier} '
     if luminance_adaptation is not None:
         cmd += f'--tmoFerwerdaAdaptLum {luminance_adaptation} '
     cmd += f'-o {tmpname_out} {tmpname}'
     run_command(cmd.split(' '))
@@ -286,16 +298,16 @@
         c2 : float
             Default is None.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_kimkautz.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_kimkautz.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo kimkautz '
     if c1 is not None:
         cmd += f'--tmoKimKautzC1 {c1} '
     if c2 is not None:
         cmd += f'--tmoKimKautzC2 {c2} '
     cmd += f'-o {tmpname_out} {tmpname}'
     run_command(cmd.split(' '))
@@ -316,16 +328,16 @@
         alpha : float
             Default: None.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_lischinski.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_lischinski.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo lischinski '
     if alpha is not None:
         cmd += f'--tmoLischinskiAlpha {alpha} '
     cmd += f'-o {tmpname_out} {tmpname}'
     run_command(cmd.split(' '))
     data_tm = _load_tonemapped_tmpdata(tmpname_out)
     os.remove(tmpname)
@@ -350,16 +362,16 @@
         contrast_equalisation : bool
             Default is False.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_mantiuk06.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_mantiuk06.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo mantiuk06 '
     if contrast is not None:
         cmd += f'--tmoM06Contrast {contrast} '
     if saturation is not None:
         cmd += f'--tmoM06Saturation {saturation} '
     if detail is not None:
         cmd += f'--tmoM06Detail {detail} '
@@ -389,29 +401,29 @@
         set_luminance : bool
             Default is False
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_mantiuk08.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_mantiuk08.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo mantiuk08 '
     if colour_saturation is not None:
         cmd += f'--tmoM08ColorSaturation {colour_saturation} '
     if contrast_enhancement is not None:
         cmd += f'--tmoM08ContrastEnh {contrast_enhancement} '
     if luminance_level is not None:
         cmd += f'--tmoM08LuminanceLvl {luminance_level} '
     cmd += f'--tmoM08SetLuminance {set_luminance} '
     cmd += f'-o {tmpname_out} {tmpname}'
     run_command(cmd.split(' '))
     data_tm = _load_tonemapped_tmpdata(tmpname_out)
-    os.remove(tmpname)
-    os.remove(tmpname_out)
+    # os.remove(tmpname)
+    # os.remove(tmpname_out)
     return data_tm
 
 
 def reinhard02(data, key: Optional[float] = None, phi: Optional[float] = None, use_scales: bool = True, range: Optional[float] = None, low: Optional[float] = None, high: Optional[float] = None) -> numpy.ndarray:
     ''' Tonemap the image using the human vision based method described in Mantiuk 2008.
 
     Parameters set to None will take their default values as set in LuminanceHDR.
@@ -432,16 +444,16 @@
         high : float
             Default: None.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_reinhard02.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_reinhard02.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo reinhard02 '
     if key is not None:
         cmd += f'--tmoR02Key {key} '
     if phi is not None:
         cmd += f'--tmoR02Phi {phi} '
     if use_scales is not None:
         cmd += f'--tmoR02Scales {use_scales} '
@@ -474,16 +486,16 @@
         lightness : float
             Default: None.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_reinhard05.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_reinhard05.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo reinhard05 '
     if brightness is not None:
         cmd += f'--tmoR05Brightness {brightness} '
     if chroma is not None:
         cmd += f'--tmoR05Chroma {chroma} '
     if lightness is not None:
         cmd += f'--tmoR05Lightness {lightness} '
@@ -514,16 +526,16 @@
         rod_level : float
             Default: None.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_pattanaik.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_pattanaik.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo pattanaik '
     if multiplier is not None:
         cmd += f'--tmoPatMultiplier {multiplier} '
     if cone_level is not None:
         cmd += f'--tmoPatCone {cone_level} '
     if rod_level is not None:
         cmd += f'--tmoPatCone {rod_level} '
@@ -548,16 +560,16 @@
         pupil_area : float
             Default: None.
 
     Returns:
         data_tm : numpy.ndarray
             Tonemapped data.
     '''
-    tmpname = _store_tmpfile(data, 'tmp_vanhateren.tiff')
-    tmpname_out = tmpname.replace('.tiff', '.tonemapped.tiff')
+    tmpname = _store_tmpfile(data, 'tmp_vanhateren.fits')
+    tmpname_out = tmpname.replace('.fits', '.tonemapped.tiff')
     cmd = BASECOMMAND + ' -e 0 --tmo vanhateren '
     if pupil_area is not None:
         cmd += f'--tmoVanHaterenPupilArea {pupil_area} '
     cmd += f'-o {tmpname_out} {tmpname}'
     run_command(cmd.split(' '))
     data_tm = _load_tonemapped_tmpdata(tmpname_out)
     os.remove(tmpname)
```

