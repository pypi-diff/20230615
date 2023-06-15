# Comparing `tmp/srxraylib-1.0.8.tar.gz` & `tmp/srxraylib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/srxraylib-1.0.8.tar", last modified: Sun Sep 25 14:11:23 2016, max compression
+gzip compressed data, was "dist/srxraylib-1.0.9.tar", last modified: Mon Dec 19 16:12:35 2016, max compression
```

## Comparing `srxraylib-1.0.8.tar` & `srxraylib-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2016-09-25 14:11:23.000000 srxraylib-1.0.8/
--rw-r--r--   0 root         (0) staff       (20)     1440 2016-09-25 14:11:23.000000 srxraylib-1.0.8/PKG-INFO
--rwxr-xr-x   0 admin      (501) staff       (20)      304 2015-10-15 17:07:48.000000 srxraylib-1.0.8/README.txt
--rw-r--r--   0 root         (0) staff       (20)       59 2016-09-25 14:11:23.000000 srxraylib-1.0.8/setup.cfg
--rwxr-xr-x   0 admin      (501) staff       (20)     4531 2016-09-25 14:11:19.000000 srxraylib-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib/
--rw-r--r--   0 admin      (501) staff       (20)       25 2015-12-14 10:41:55.000000 srxraylib-1.0.8/srxraylib/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib/metrology/
--rw-r--r--   0 admin      (501) staff       (20)        0 2015-10-30 10:25:38.000000 srxraylib-1.0.8/srxraylib/metrology/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    69582 2015-12-21 09:36:25.000000 srxraylib-1.0.8/srxraylib/metrology/dabam.py
--rw-r--r--   0 admin      (501) staff       (20)    27706 2016-09-13 15:19:02.000000 srxraylib-1.0.8/srxraylib/metrology/profiles_simulation.py
--rw-r--r--   0 admin      (501) staff       (20)    14353 2016-08-09 13:24:36.000000 srxraylib-1.0.8/srxraylib/metrology/profiles_simulation_test.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib/plot/
--rw-r--r--   0 admin      (501) staff       (20)       81 2016-06-16 10:37:37.000000 srxraylib-1.0.8/srxraylib/plot/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    14115 2016-09-21 13:30:59.000000 srxraylib-1.0.8/srxraylib/plot/gol.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib/sources/
--rw-r--r--   0 admin      (501) staff       (20)       81 2015-10-15 17:15:58.000000 srxraylib-1.0.8/srxraylib/sources/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    73955 2016-09-23 09:28:17.000000 srxraylib-1.0.8/srxraylib/sources/srfunc.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib/util/
--rw-r--r--   0 admin      (501) staff       (20)       81 2015-10-15 17:15:58.000000 srxraylib-1.0.8/srxraylib/util/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)    10750 2016-08-08 08:47:43.000000 srxraylib-1.0.8/srxraylib/util/data_structures.py
--rw-r--r--   0 admin      (501) staff       (20)    11876 2016-06-16 10:37:37.000000 srxraylib-1.0.8/srxraylib/util/data_structures_test.py
--rw-r--r--   0 admin      (501) staff       (20)      270 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib/version.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib/waveoptics/
--rw-r--r--   0 admin      (501) staff       (20)       81 2015-12-14 10:41:55.000000 srxraylib-1.0.8/srxraylib/waveoptics/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     9460 2016-08-08 08:47:43.000000 srxraylib-1.0.8/srxraylib/waveoptics/CompactAFReader.py
--rw-r--r--   0 admin      (501) staff       (20)     7281 2016-08-23 08:00:47.000000 srxraylib-1.0.8/srxraylib/waveoptics/NumpyToSRW.py
--rw-r--r--   0 admin      (501) staff       (20)     4115 2016-06-16 10:37:37.000000 srxraylib-1.0.8/srxraylib/waveoptics/propagator.py
--rw-r--r--   0 admin      (501) staff       (20)    15285 2016-08-08 08:47:43.000000 srxraylib-1.0.8/srxraylib/waveoptics/propagator2D.py
--rw-r--r--   0 admin      (501) staff       (20)    29762 2016-08-08 08:47:43.000000 srxraylib-1.0.8/srxraylib/waveoptics/propagators_test.py
--rw-r--r--   0 admin      (501) staff       (20)     8909 2016-06-16 10:37:37.000000 srxraylib-1.0.8/srxraylib/waveoptics/wavefront.py
--rw-r--r--   0 admin      (501) staff       (20)    17074 2016-08-08 08:47:43.000000 srxraylib-1.0.8/srxraylib/waveoptics/wavefront2D.py
--rw-r--r--   0 admin      (501) staff       (20)    18289 2016-08-08 08:47:43.000000 srxraylib-1.0.8/srxraylib/waveoptics/wavefronts_test.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)        1 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2015-10-15 17:20:49.000000 srxraylib-1.0.8/srxraylib.egg-info/not-zip-safe
--rw-r--r--   0 admin      (501) staff       (20)     1440 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)       23 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)      948 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)       10 2016-09-25 14:11:23.000000 srxraylib-1.0.8/srxraylib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2016-12-19 16:12:35.000000 srxraylib-1.0.9/
+-rw-r--r--   0 root         (0) staff       (20)     1440 2016-12-19 16:12:35.000000 srxraylib-1.0.9/PKG-INFO
+-rwxr-xr-x   0 admin      (501) staff       (20)      304 2015-10-15 17:07:48.000000 srxraylib-1.0.9/README.txt
+-rw-r--r--   0 root         (0) staff       (20)       59 2016-12-19 16:12:35.000000 srxraylib-1.0.9/setup.cfg
+-rwxr-xr-x   0 admin      (501) staff       (20)     4531 2016-12-19 16:11:39.000000 srxraylib-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib/
+-rw-r--r--   0 admin      (501) staff       (20)       25 2015-12-14 10:41:55.000000 srxraylib-1.0.9/srxraylib/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib/metrology/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2015-10-30 10:25:38.000000 srxraylib-1.0.9/srxraylib/metrology/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    69582 2015-12-21 09:36:25.000000 srxraylib-1.0.9/srxraylib/metrology/dabam.py
+-rw-r--r--   0 admin      (501) staff       (20)    27708 2016-12-19 15:44:54.000000 srxraylib-1.0.9/srxraylib/metrology/profiles_simulation.py
+-rw-r--r--   0 admin      (501) staff       (20)    14353 2016-08-09 13:24:36.000000 srxraylib-1.0.9/srxraylib/metrology/profiles_simulation_test.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib/plot/
+-rw-r--r--   0 admin      (501) staff       (20)       81 2016-06-16 10:37:37.000000 srxraylib-1.0.9/srxraylib/plot/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    14115 2016-09-21 13:30:59.000000 srxraylib-1.0.9/srxraylib/plot/gol.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib/sources/
+-rw-r--r--   0 admin      (501) staff       (20)       81 2015-10-15 17:15:58.000000 srxraylib-1.0.9/srxraylib/sources/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    73955 2016-09-23 09:28:17.000000 srxraylib-1.0.9/srxraylib/sources/srfunc.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib/util/
+-rw-r--r--   0 admin      (501) staff       (20)       81 2015-10-15 17:15:58.000000 srxraylib-1.0.9/srxraylib/util/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    10750 2016-08-08 08:47:43.000000 srxraylib-1.0.9/srxraylib/util/data_structures.py
+-rw-r--r--   0 admin      (501) staff       (20)    11876 2016-06-16 10:37:37.000000 srxraylib-1.0.9/srxraylib/util/data_structures_test.py
+-rw-r--r--   0 admin      (501) staff       (20)      270 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib/version.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib/waveoptics/
+-rw-r--r--   0 admin      (501) staff       (20)       81 2015-12-14 10:41:55.000000 srxraylib-1.0.9/srxraylib/waveoptics/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     9460 2016-08-08 08:47:43.000000 srxraylib-1.0.9/srxraylib/waveoptics/CompactAFReader.py
+-rw-r--r--   0 admin      (501) staff       (20)     2338 2016-12-19 14:11:12.000000 srxraylib-1.0.9/srxraylib/waveoptics/example_arago_poisson.py
+-rw-r--r--   0 admin      (501) staff       (20)    19041 2016-11-18 15:04:22.000000 srxraylib-1.0.9/srxraylib/waveoptics/example_ideal_lens.py
+-rw-r--r--   0 admin      (501) staff       (20)     7281 2016-08-23 08:00:47.000000 srxraylib-1.0.9/srxraylib/waveoptics/NumpyToSRW.py
+-rw-r--r--   0 admin      (501) staff       (20)     4115 2016-06-16 10:37:37.000000 srxraylib-1.0.9/srxraylib/waveoptics/propagator.py
+-rw-r--r--   0 admin      (501) staff       (20)    15284 2016-11-18 15:04:22.000000 srxraylib-1.0.9/srxraylib/waveoptics/propagator2D.py
+-rw-r--r--   0 admin      (501) staff       (20)    30540 2016-11-18 15:04:22.000000 srxraylib-1.0.9/srxraylib/waveoptics/propagators_test.py
+-rw-r--r--   0 admin      (501) staff       (20)     9277 2016-11-18 15:04:22.000000 srxraylib-1.0.9/srxraylib/waveoptics/wavefront.py
+-rw-r--r--   0 admin      (501) staff       (20)    17765 2016-12-19 14:11:12.000000 srxraylib-1.0.9/srxraylib/waveoptics/wavefront2D.py
+-rw-r--r--   0 admin      (501) staff       (20)    18293 2016-11-18 15:04:22.000000 srxraylib-1.0.9/srxraylib/waveoptics/wavefronts_test.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)        1 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2015-10-15 17:20:49.000000 srxraylib-1.0.9/srxraylib.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (501) staff       (20)     1440 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)       23 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)     1037 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)       10 2016-12-19 16:12:35.000000 srxraylib-1.0.9/srxraylib.egg-info/top_level.txt
```

### Comparing `srxraylib-1.0.8/PKG-INFO` & `srxraylib-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: srxraylib
-Version: 1.0.8
+Version: 1.0.9
 Summary: Synchrotron Radiation X-ray library
 Home-page: https://github.com/lucarebuffi/SR-xraylib
 Author: Luca Rebuffi
 Author-email: luca.rebuffi@elettra.eu
 License: GPLv3
 Download-URL: https://github.com/lucarebuffi/SR-xraylib
 Description: SR-xraylib
```

### Comparing `srxraylib-1.0.8/setup.py` & `srxraylib-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 except ImportError:
     import ez_setup
     ez_setup.use_setuptools()
     from setuptools import setup
 
 NAME = 'srxraylib'
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 ISRELEASED = False
 
 DESCRIPTION = 'Synchrotron Radiation X-ray library'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.txt')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi, Manuel Sanchez del Rio and Mark Glass'
 AUTHOR_EMAIL = 'luca.rebuffi@elettra.eu'
```

### Comparing `srxraylib-1.0.8/srxraylib/metrology/dabam.py` & `srxraylib-1.0.9/srxraylib/metrology/dabam.py`

 * *Files identical despite different names*

### Comparing `srxraylib-1.0.8/srxraylib/metrology/profiles_simulation.py` & `srxraylib-1.0.9/srxraylib/metrology/profiles_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     if npoints_ratio_f_over_x == 1.0:
         f_npoints = n_surface_points
     else:
         f_npoints = int(n_surface_points*npoints_ratio_f_over_x)
 
     freq = numpy.linspace(f_from,f_to,f_npoints)
     #todo: make exponent of power law a parameter
-    ampl = freq**(-power_law_exponent_beta)
+    ampl = freq**(-power_law_exponent_beta/2)
     phases = numpy.random.rand(freq.size)*2*numpy.pi
     ymirr = numpy.zeros(n_surface_points)
     for i in range(f_npoints):
         ymirr += (ampl[i] *  numpy.sin(2*numpy.pi*freq[i]*x_coords + phases[i]))
 
     if renormalize_to_heights_sd != None:
         ymirr = ymirr / ymirr.std() * renormalize_to_heights_sd
```

### Comparing `srxraylib-1.0.8/srxraylib/metrology/profiles_simulation_test.py` & `srxraylib-1.0.9/srxraylib/metrology/profiles_simulation_test.py`

 * *Files identical despite different names*

### Comparing `srxraylib-1.0.8/srxraylib/plot/gol.py` & `srxraylib-1.0.9/srxraylib/plot/gol.py`

 * *Files identical despite different names*

### Comparing `srxraylib-1.0.8/srxraylib/sources/srfunc.py` & `srxraylib-1.0.9/srxraylib/sources/srfunc.py`

 * *Files identical despite different names*

### Comparing `srxraylib-1.0.8/srxraylib/util/data_structures.py` & `srxraylib-1.0.9/srxraylib/util/data_structures.py`

 * *Files identical despite different names*

### Comparing `srxraylib-1.0.8/srxraylib/util/data_structures_test.py` & `srxraylib-1.0.9/srxraylib/util/data_structures_test.py`

 * *Files identical despite different names*

### Comparing `srxraylib-1.0.8/srxraylib/waveoptics/CompactAFReader.py` & `srxraylib-1.0.9/srxraylib/waveoptics/CompactAFReader.py`

 * *Files identical despite different names*

### Comparing `srxraylib-1.0.8/srxraylib/waveoptics/NumpyToSRW.py` & `srxraylib-1.0.9/srxraylib/waveoptics/NumpyToSRW.py`

 * *Files identical despite different names*

### Comparing `srxraylib-1.0.8/srxraylib/waveoptics/propagator.py` & `srxraylib-1.0.9/srxraylib/waveoptics/propagator.py`

 * *Files identical despite different names*

### Comparing `srxraylib-1.0.8/srxraylib/waveoptics/propagator2D.py` & `srxraylib-1.0.9/srxraylib/waveoptics/propagator2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy
 
 #
 # implements 2D propagators:
 #
 #   propagate_2D_fraunhofer: Far field Fraunhofer propagator. TODO: Check phases, not to be used for downstream propagation
-#   propagate_2D_integral: Simplification of the Kirchhoff-Fresnel integral. TODO: Very slow and and give some problems
+#   propagate_2D_integral: Simplification of the Kirchhoff-Fresnel integral. TODO: Very slow and give some problems
 #
 #
 #   propagate_2D_fresnel               \
 #   propagate_2D_fresnel_convolution   | Near field Fresnel propagators via convolution in Fourier space. Three methods
 #   propagate_2D_fresnel_srw           /
 #
 #          three methods available: 'fft': fft -> multiply by kernel in freq -> ifft
@@ -23,23 +23,30 @@
 #    The fraunhoffer method cannot be used in a compound system (more than one element) and in connection with lenses
 #    The integral propagator is extremely slow for 2D, so by default it only calculates the horizontal and vertical
 #        profiles. Therefore, it cannot be used with compound systems.
 #
 #     >>> Prefer propagate_2D_fresnel <<<
 #       Prefer EVEN number of bins.
 #       Set shift_half_pixel=1 (now the default)
-#    Under these circunstances, the results agree very well with SRW
+#    Under these circumstances, the results agree very well with SRW
 #
 #
 #
 
 from srxraylib.util.data_structures import ScaledMatrix
 from srxraylib.waveoptics.wavefront2D import Wavefront2D
 
 
+try:
+    import srwlib
+    SRWLIB_AVAILABLE = True
+except:
+    SRWLIB_AVAILABLE = False
+    print("SRW is not available")
+
 # TODO: check resulting amplitude normalization (fft and srw likely agree, convolution gives too high amplitudes, so needs normalization)
 
 #TODO: add these elements (like in Timm's application)
 #   -slit with absorption
 #   -two slits
 #   -lens with absorption
 #   -gold grid
@@ -199,18 +206,15 @@
     :param srw_autosetting:set to 1 for automatic SRW redimensionate wavefront
     :return:
     """
 
     #
     # convolving with the Fresnel kernel via SRW package
     #
-    try:
-        import srwlib
-    except:
-        raise ImportError("Please install srwlib before attempting to us it")
+
 
     from srxraylib.waveoptics.NumpyToSRW import numpyArrayToSRWArray, SRWWavefrontFromElectricField, SRWEFieldAsNumpy
 
     import scipy.constants as codata
     angstroms_to_eV = codata.h*codata.c/codata.e*1e10
```

### Comparing `srxraylib-1.0.8/srxraylib/waveoptics/propagators_test.py` & `srxraylib-1.0.9/srxraylib/waveoptics/propagators_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,25 @@
 from srxraylib.waveoptics.propagator import propagate_1D_fraunhofer
 from srxraylib.waveoptics.propagator import propagate_1D_integral
 from srxraylib.waveoptics.propagator import propagate_1D_fresnel, propagate_1D_fresnel_convolution
 from srxraylib.waveoptics.propagator2D import propagate_2D_fraunhofer
 from srxraylib.waveoptics.propagator2D import propagate_2D_integral
 from srxraylib.waveoptics.propagator2D import propagate_2D_fresnel, propagate_2D_fresnel_convolution, propagate_2D_fresnel_srw
 
-do_plot = 0
+do_plot = True
 
 if do_plot:
     from srxraylib.plot.gol import plot,plot_image,plot_table
 
+try:
+    import srwlib
+    SRWLIB_AVAILABLE = True
+except:
+    SRWLIB_AVAILABLE = False
+    print("SRW is not available")
 
 #
 # some common tools
 #
 def get_theoretical_diffraction_pattern(angle_x,
                                         aperture_type='square',aperture_diameter=40e-6,
                                         wavelength=1.24e-10,normalization=True):
@@ -81,15 +87,15 @@
 
     def propagate_1D(self,do_plot=do_plot,method='fft',
                                 wavelength=1.24e-10,aperture_type='square',aperture_diameter=40e-6,
                                 wavefront_length=100e-6,npoints=500,
                                 propagation_distance = 30.0,show=1):
 
 
-        print("#                                                            ")
+        print("\n#                                                            ")
         print("# far field 1D (fraunhofer) diffraction from a %s aperture  "%aperture_type)
         print("#                                                            ")
 
         wf = Wavefront1D.initialize_wavefront_from_range(x_min=-wavefront_length/2, x_max=wavefront_length/2,
                                                                 number_of_points=npoints,wavelength=wavelength)
 
         wf.set_plane_wave_from_complex_amplitude((2.0+1.0j)) # an arbitraty value
@@ -149,15 +155,15 @@
 
         aperture_type="square"
         aperture_diameter = 40e-6
         wavefront_length = 800e-6
         wavelength = 1.24e-10
         npoints=1024
 
-        print("#                                                            ")
+        print("\n#                                                            ")
         print("# far field 1D (fraunhofer) diffraction from a %s aperture  "%aperture_type)
         print("#                                                            ")
 
 
 
         angle, intensity_calculated,intensity_theory = self.propagate_1D(do_plot=do_plot,method="fraunhofer",
                                 wavelength=wavelength,aperture_type=aperture_type,aperture_diameter=aperture_diameter,
@@ -171,15 +177,15 @@
         aperture_type="square"
         aperture_diameter = 40e-6
         wavefront_length = 800e-6
         wavelength = 1.24e-10
         propagation_distance = 30.0
         npoints=1024
 
-        print("#                                                            ")
+        print("\n#                                                            ")
         print("# far field 1D (fraunhofer) diffraction from a %s aperture  "%aperture_type)
         print("#                                                            ")
 
 
 
         angle, intensity_calculated,intensity_theory = self.propagate_1D(do_plot=do_plot,method="fft",
                                 wavelength=wavelength,aperture_type=aperture_type,aperture_diameter=aperture_diameter,
@@ -194,15 +200,15 @@
         aperture_type="square"
         aperture_diameter = 40e-6
         wavefront_length = 800e-6
         wavelength = 1.24e-10
         propagation_distance = 30.0
         npoints=1024
 
-        print("#                                                            ")
+        print("\n#                                                            ")
         print("# far field 1D (fraunhofer) diffraction from a %s aperture  "%aperture_type)
         print("#                                                            ")
 
 
 
         angle, intensity_calculated,intensity_theory = self.propagate_1D(do_plot=do_plot,method="convolution",
                                 wavelength=wavelength,aperture_type=aperture_type,aperture_diameter=aperture_diameter,
@@ -216,15 +222,15 @@
         aperture_type="square"
         aperture_diameter = 40e-6
         wavefront_length = 800e-6
         wavelength = 1.24e-10
         propagation_distance = 30.0
         npoints=1024
 
-        print("#                                                            ")
+        print("\n#                                                            ")
         print("# far field 1D (fraunhofer) diffraction from a %s aperture  "%aperture_type)
         print("#                                                            ")
 
 
 
         angle, intensity_calculated,intensity_theory = self.propagate_1D(do_plot=do_plot,method="integral",
                                 wavelength=wavelength,aperture_type=aperture_type,aperture_diameter=aperture_diameter,
@@ -248,15 +254,15 @@
     def propagate_2D_fresnel(self,do_plot=do_plot,method='fft',
                                 wavelength=1.24e-10,aperture_type='square',aperture_diameter=40e-6,
                                 pixelsize_x=1e-6,pixelsize_y=1e-6,npixels_x=1024,npixels_y=1024,
                                 propagation_distance = 30.0,show=1):
 
 
         method_label = "fresnel (%s)"%method
-        print("#                                                             ")
+        print("\n#                                                             ")
         print("# 2D near field fresnel (%s) diffraction from a %s aperture  "%(method_label,aperture_type))
         print("#                                                             ")
 
 
         # wf = Wavefront2D.initialize_wavefront_from_steps(x_start=-pixelsize_x*npixels_x/2,
         #                                                         x_step=pixelsize_x,
         #                                                         y_start=-pixelsize_y*npixels_y/2,
@@ -338,15 +344,15 @@
     def propagation_with_lens(self,do_plot=do_plot,method='fft',
                                 wavelength=1.24e-10,
                                 pixelsize_x=1e-6,npixels_x=2000,pixelsize_y=1e-6,npixels_y=2000,
                                 propagation_distance=30.0,defocus_factor=1.0,propagation_steps=1,show=1):
 
 
         method_label = "fresnel (%s)"%method
-        print("#                                                             ")
+        print("\n#                                                             ")
         print("# near field fresnel (%s) diffraction and focusing  "%(method_label))
         print("#                                                             ")
 
         #                               \ |  /
         #   *                           | | |                      *
         #                               / | \
         #   <-------    d  ---------------><---------   d   ------->
@@ -430,15 +436,15 @@
         :param pixelsize_y:
         :param npixels_x:
         :param npixels_y:
         :param wavelength:
         :return:
         """
 
-        print("#                                                            ")
+        print("\n#                                                            ")
         print("# far field 2D (fraunhofer) diffraction from a square aperture  ")
         print("#                                                            ")
 
         method = "fraunhofer"
 
         print("Fraunhoffer diffraction valid for distances > > a^2/lambda = %f m"%((aperture_diameter/2)**2/wavelength))
 
@@ -515,14 +521,19 @@
                                 aperture_diameter=40e-6,
                                 pixelsize_x=1e-6,pixelsize_y=1e-6,npixels_x=1024,npixels_y=1024,
                                 propagation_distance=30.0,wavelength=1.24e-10)
 
         numpy.testing.assert_almost_equal(ycalc/10,ytheory/10,1)
 
     def test_propagate_2D_fresnel_srw_square(self):
+
+        if not SRWLIB_AVAILABLE:
+            print("SRW not available, skipping test_propagate_2D_fresnel_srw_square")
+            return
+
         xcalc, ycalc, xtheory, ytheory = self.propagate_2D_fresnel(do_plot=do_plot,method='srw',aperture_type='square',
                                 aperture_diameter=40e-6,
                                 #pixelsize_x=1e-6,pixelsize_y=1e-6,npixels_x=1024,npixels_y=1024,
                                 pixelsize_x=1e-6*2,pixelsize_y=1e-6*4,npixels_x=1024/2,npixels_y=1024/4,
                                 propagation_distance=30.0,wavelength=1.24e-10)
 
         numpy.testing.assert_almost_equal(ycalc/10,ytheory/10,1)
@@ -540,35 +551,35 @@
     def test_propagate_2D_fresnel_all_circle(self):
 
         xcalc_fft, ycalc_fft, xtheory, ytheory = self.propagate_2D_fresnel(do_plot=0,method='fft',aperture_type='square',
                                 aperture_diameter=40e-6,
                                 pixelsize_x=1e-6,pixelsize_y=1e-6,npixels_x=1024,npixels_y=1024,
                                 propagation_distance=5.0,wavelength=1.24e-10)
 
-        xcalc_srw, ycalc_srw, xtheory, ytheory = self.propagate_2D_fresnel(do_plot=0,method='srw',aperture_type='square',
-                                aperture_diameter=40e-6,
-                                pixelsize_x=1e-6,pixelsize_y=1e-6,npixels_x=1024,npixels_y=1024,
-                                propagation_distance=5.0,wavelength=1.24e-10)
-
-        xcalc_srw, ycalc_convolution, xtheory, ytheory = self.propagate_2D_fresnel(do_plot=0,method='convolution',aperture_type='square',
-                                aperture_diameter=40e-6,
-                                pixelsize_x=1e-6,pixelsize_y=1e-6,npixels_x=1024,npixels_y=1024,
-                                propagation_distance=5.0,wavelength=1.24e-10)
+        if  SRWLIB_AVAILABLE:
 
+            xcalc_srw, ycalc_srw, xtheory, ytheory = self.propagate_2D_fresnel(do_plot=0,method='srw',aperture_type='square',
+                                    aperture_diameter=40e-6,
+                                    pixelsize_x=1e-6,pixelsize_y=1e-6,npixels_x=1024,npixels_y=1024,
+                                    propagation_distance=5.0,wavelength=1.24e-10)
+
+            xcalc_srw, ycalc_convolution, xtheory, ytheory = self.propagate_2D_fresnel(do_plot=0,method='convolution',aperture_type='square',
+                                    aperture_diameter=40e-6,
+                                    pixelsize_x=1e-6,pixelsize_y=1e-6,npixels_x=1024,npixels_y=1024,
+                                    propagation_distance=5.0,wavelength=1.24e-10)
+
+
+            if do_plot:
+               x = xcalc_srw
+               y = numpy.vstack((ycalc_fft,ycalc_srw,ycalc_convolution))
+               plot_table(1e6*x,y,legend=["fft","srw","convolution"],ytitle="Intensity",xtitle="x coodinate [um]",
+                              title="Comparison circular aperture - near field")
 
-
-
-        if do_plot:
-           x = xcalc_srw
-           y = numpy.vstack((ycalc_fft,ycalc_srw,ycalc_convolution))
-           plot_table(1e6*x,y,legend=["fft","srw","convolution"],ytitle="Intensity",xtitle="x coodinate [um]",
-                          title="Comparison circular aperture - near field")
-
-        numpy.testing.assert_almost_equal(ycalc_fft,ycalc_srw,1)
-        numpy.testing.assert_almost_equal(ycalc_convolution,ycalc_srw,1)
+            numpy.testing.assert_almost_equal(ycalc_fft,ycalc_srw,1)
+            numpy.testing.assert_almost_equal(ycalc_convolution,ycalc_srw,1)
 
     def test_lens(self):
 
         lens_diameter = 0.002
         npixels_x = 2048
         pixelsize_x = lens_diameter / npixels_x
         print("pixelsize: ",pixelsize_x)
@@ -585,32 +596,41 @@
         propagation_steps = 1
 
         x_fft, y_fft = self.propagation_with_lens(do_plot=0,method='fft',
                                 propagation_steps=propagation_steps,
                                 wavelength=wavelength,
                                 pixelsize_x=pixelsize_x,npixels_x=npixels_x,pixelsize_y=pixelsize_y,npixels_y=npixels_y,
                                 propagation_distance = propagation_distance, defocus_factor=defocus_factor)
-
-        x_srw, y_srw = self.propagation_with_lens(do_plot=0,method='srw',
-                                propagation_steps=propagation_steps,
-                                wavelength=wavelength,
-                                pixelsize_x=pixelsize_x,npixels_x=npixels_x,pixelsize_y=pixelsize_y,npixels_y=npixels_y,
-                                propagation_distance = propagation_distance, defocus_factor=defocus_factor)
+        if SRWLIB_AVAILABLE:
+            x_srw, y_srw = self.propagation_with_lens(do_plot=0,method='srw',
+                                    propagation_steps=propagation_steps,
+                                    wavelength=wavelength,
+                                    pixelsize_x=pixelsize_x,npixels_x=npixels_x,pixelsize_y=pixelsize_y,npixels_y=npixels_y,
+                                    propagation_distance = propagation_distance, defocus_factor=defocus_factor)
 
 
         x_convolution, y_convolution = self.propagation_with_lens(do_plot=0,method='convolution',
                                 propagation_steps=propagation_steps,
                                 wavelength=wavelength,
                                 pixelsize_x=pixelsize_x,npixels_x=npixels_x,pixelsize_y=pixelsize_y,npixels_y=npixels_y,
                                 propagation_distance = propagation_distance, defocus_factor=defocus_factor)
 
         if do_plot:
-            x = x_fft
-            y = numpy.vstack((y_fft,y_srw,y_convolution))
+            if SRWLIB_AVAILABLE:
+                x = x_fft
+                y = numpy.vstack((y_fft,y_srw,y_convolution))
 
-            plot_table(1e6*x,y,legend=["fft","srw","convolution"],ytitle="Intensity",xtitle="x coodinate [um]",
-                       title="Comparison 1:1 focusing")
+                plot_table(1e6*x,y,legend=["fft","srw","convolution"],ytitle="Intensity",xtitle="x coordinate [um]",
+                           title="Comparison 1:1 focusing")
+            else:
+                x = x_fft
+                y = numpy.vstack((y_fft,y_convolution))
+
+                plot_table(1e6*x,y,legend=["fft","convolution"],ytitle="Intensity",xtitle="x coordinate [um]",
+                           title="Comparison 1:1 focusing")
 
         numpy.testing.assert_almost_equal(y_fft,y_convolution,1)
-        numpy.testing.assert_almost_equal(y_fft,y_srw,1)
-        numpy.testing.assert_almost_equal(y_convolution,y_srw,1)
+
+        if SRWLIB_AVAILABLE:
+            numpy.testing.assert_almost_equal(y_fft,y_srw,1)
+            numpy.testing.assert_almost_equal(y_convolution,y_srw,1)
```

### Comparing `srxraylib-1.0.8/srxraylib/waveoptics/wavefront.py` & `srxraylib-1.0.9/srxraylib/waveoptics/wavefront.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 import numpy
 
 
-from srxraylib.util.data_structures import ScaledArray, ScaledMatrix
+from srxraylib.util.data_structures import ScaledArray
+import scipy.constants as codata
 
 #------------------------------------------------
 #
 #
 #
 #
 #------------------------------------------------
@@ -116,14 +117,23 @@
     #TODO: this is obsolete call, to be removed after updating shadowOui
     # new name is get_interpolated_complex_amplitudes. 
     def get_complex_amplitude_from_abscissas(self, abscissa_values):
         return self.electric_field_array.interpolate_values(abscissa_values)
 
     # modifiers
 
+    def set_wavelength(self,wavelength):
+        self.wavelength = wavelength
+
+    def set_wavenumber(self,wavenumber):
+        self.wavelength = 2*numpy.pi / wavenumber
+
+    def set_photon_energy(self,photon_energy):
+        m2ev = codata.c * codata.h / codata.e      # lambda(m)  = m2eV / energy(eV)
+        self.wavelength = m2ev / photon_energy
 
     def set_complex_amplitude(self,complex_amplitude):
         if complex_amplitude.size != self.electric_field_array.size():
             raise Exception("Complex amplitude array has different dimension")
         self.electric_field_array.np_array = complex_amplitude
 
     def set_plane_wave_from_complex_amplitude(self, complex_amplitude=(1.0 + 0.0j)):
```

### Comparing `srxraylib-1.0.8/srxraylib/waveoptics/wavefront2D.py` & `srxraylib-1.0.9/srxraylib/waveoptics/wavefront2D.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 
 import numpy
 from srxraylib.util.data_structures import ScaledMatrix
+import scipy.constants as codata
+
 
 #------------------------------------------------
 #
 # Implements Wavefront2D object
 #
 #------------------------------------------------
+#
+#TODO: Add duplicate method
 
 class Wavefront2D(object):
     wavelength = 0.0
     electric_field_array = None
 
     def __init__(self, wavelength=1e-10, electric_field_array=None):
         self.wavelength = wavelength
@@ -64,14 +68,18 @@
 
     def get_wavelength(self):
         return self.wavelength
 
     def get_wavenumber(self):
         return 2*numpy.pi/self.wavelength
 
+    def get_photon_energy(self):
+        m2ev = codata.c * codata.h / codata.e      # lambda(m)  = m2eV / energy(eV)
+        return  m2ev / self.wavelength
+
     def get_coordinate_x(self):
         return self.electric_field_array.get_x_values()
 
     def get_coordinate_y(self):
         return self.electric_field_array.get_y_values()
 
 
@@ -168,14 +176,24 @@
 
     def get_mesh_y(self):
         XY = numpy.meshgrid(self.get_coordinate_x(),self.get_coordinate_y())
         return XY[1].T
 
     # modifiers
 
+    def set_wavelength(self,wavelength):
+        self.wavelength = wavelength
+
+    def set_wavenumber(self,wavenumber):
+        self.wavelength = 2*numpy.pi / wavenumber
+
+    def set_photon_energy(self,photon_energy):
+        m2ev = codata.c * codata.h / codata.e      # lambda(m)  = m2eV / energy(eV)
+        self.wavelength = m2ev / photon_energy
+
     def set_complex_amplitude(self,complex_amplitude):
         if self.electric_field_array.shape() != complex_amplitude.shape:
             raise Exception("Incompatible shape")
         self.electric_field_array.set_z_values(complex_amplitude)
 
     def set_plane_wave_from_complex_amplitude(self, complex_amplitude=(1.0 + 0.0j)):
         new_value = self.electric_field_array.get_z_values()
@@ -241,21 +259,24 @@
         if len(upper_window_x) > 0: window[upper_window_x,:] = 0
         if len(lower_window_y) > 0: window[:,lower_window_y] = 0
         if len(upper_window_y) > 0: window[:,upper_window_y] = 0
 
         self.rescale_amplitudes(window)
 
     # new
-    def apply_pinhole(self, radius, x_center=0.0, y_center=0.0):
+    def apply_pinhole(self, radius, x_center=0.0, y_center=0.0, negative=False):
         window = numpy.zeros(self.electric_field_array.shape())
         X = self.get_mesh_x()
         Y = self.get_mesh_y()
         distance_to_center = numpy.sqrt( (X-x_center)**2 + (Y-y_center)**2 )
-        indices_inside = numpy.where(distance_to_center <= radius)
-        window[indices_inside] = 1.0
+        if negative:
+            indices_good = numpy.where(distance_to_center >= radius)
+        else:
+            indices_good = numpy.where(distance_to_center <= radius)
+        window[indices_good] = 1.0
 
         self.rescale_amplitudes(window)
 
     #
     def rebin(self,expansion_points_horizontal, expansion_points_vertical, expansion_range_horizontal, expansion_range_vertical,
               keep_the_same_intensity=0,set_extrapolation_to_zero=0):
```

### Comparing `srxraylib-1.0.8/srxraylib/waveoptics/wavefronts_test.py` & `srxraylib-1.0.9/srxraylib/waveoptics/wavefronts_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 import numpy
 
 from srxraylib.waveoptics.wavefront import Wavefront1D
 from srxraylib.waveoptics.wavefront2D import Wavefront2D
 
 
-do_plot = 0
+do_plot = False
 
 #
 # 1D tests
 #
 class Wavefront1DTest(unittest.TestCase):
     def test_initializers(self,do_plot=do_plot):
```

### Comparing `srxraylib-1.0.8/srxraylib.egg-info/PKG-INFO` & `srxraylib-1.0.9/srxraylib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: srxraylib
-Version: 1.0.8
+Version: 1.0.9
 Summary: Synchrotron Radiation X-ray library
 Home-page: https://github.com/lucarebuffi/SR-xraylib
 Author: Luca Rebuffi
 Author-email: luca.rebuffi@elettra.eu
 License: GPLv3
 Download-URL: https://github.com/lucarebuffi/SR-xraylib
 Description: SR-xraylib
```

### Comparing `srxraylib-1.0.8/srxraylib.egg-info/SOURCES.txt` & `srxraylib-1.0.9/srxraylib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,13 +18,15 @@
 srxraylib/sources/srfunc.py
 srxraylib/util/__init__.py
 srxraylib/util/data_structures.py
 srxraylib/util/data_structures_test.py
 srxraylib/waveoptics/CompactAFReader.py
 srxraylib/waveoptics/NumpyToSRW.py
 srxraylib/waveoptics/__init__.py
+srxraylib/waveoptics/example_arago_poisson.py
+srxraylib/waveoptics/example_ideal_lens.py
 srxraylib/waveoptics/propagator.py
 srxraylib/waveoptics/propagator2D.py
 srxraylib/waveoptics/propagators_test.py
 srxraylib/waveoptics/wavefront.py
 srxraylib/waveoptics/wavefront2D.py
 srxraylib/waveoptics/wavefronts_test.py
```

