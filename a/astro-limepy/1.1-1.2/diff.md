# Comparing `tmp/astro-limepy-1.1.tar.gz` & `tmp/astro-limepy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/astro-limepy-1.1.tar", last modified: Fri Oct 15 12:16:04 2021, max compression
+gzip compressed data, was "astro-limepy-1.2.tar", last modified: Thu Jun 15 15:46:42 2023, max compression
```

## Comparing `astro-limepy-1.1.tar` & `astro-limepy-1.2.tar`

### file list

```diff
@@ -1,17 +1,30 @@
-drwxrwxr-x   0 balbinot  (1000) balbinot  (1000)        0 2021-10-15 12:16:04.080529 astro-limepy-1.1/
--rw-rw-r--   0 balbinot  (1000) balbinot  (1000)     2591 2021-10-15 12:16:04.080529 astro-limepy-1.1/PKG-INFO
--rwxrwxr-x   0 balbinot  (1000) balbinot  (1000)     1374 2021-10-15 12:13:55.000000 astro-limepy-1.1/README.rst
-drwxrwxr-x   0 balbinot  (1000) balbinot  (1000)        0 2021-10-15 12:16:04.080529 astro-limepy-1.1/astro_limepy.egg-info/
--rw-rw-r--   0 balbinot  (1000) balbinot  (1000)     2591 2021-10-15 12:16:04.000000 astro-limepy-1.1/astro_limepy.egg-info/PKG-INFO
--rw-rw-r--   0 balbinot  (1000) balbinot  (1000)      311 2021-10-15 12:16:04.000000 astro-limepy-1.1/astro_limepy.egg-info/SOURCES.txt
--rw-rw-r--   0 balbinot  (1000) balbinot  (1000)        1 2021-10-15 12:16:04.000000 astro-limepy-1.1/astro_limepy.egg-info/dependency_links.txt
--rw-rw-r--   0 balbinot  (1000) balbinot  (1000)        1 2021-10-15 12:14:33.000000 astro-limepy-1.1/astro_limepy.egg-info/not-zip-safe
--rw-rw-r--   0 balbinot  (1000) balbinot  (1000)       20 2021-10-15 12:16:04.000000 astro-limepy-1.1/astro_limepy.egg-info/requires.txt
--rw-rw-r--   0 balbinot  (1000) balbinot  (1000)        7 2021-10-15 12:16:04.000000 astro-limepy-1.1/astro_limepy.egg-info/top_level.txt
-drwxrwxr-x   0 balbinot  (1000) balbinot  (1000)        0 2021-10-15 12:16:04.080529 astro-limepy-1.1/limepy/
--rwxrwxr-x   0 balbinot  (1000) balbinot  (1000)      227 2021-10-15 12:13:55.000000 astro-limepy-1.1/limepy/__init__.py
--rwxrwxr-x   0 balbinot  (1000) balbinot  (1000)    44596 2021-10-15 12:13:55.000000 astro-limepy-1.1/limepy/limepy.py
--rwxrwxr-x   0 balbinot  (1000) balbinot  (1000)    10321 2021-10-15 12:13:55.000000 astro-limepy-1.1/limepy/sample.py
--rwxrwxr-x   0 balbinot  (1000) balbinot  (1000)    30448 2021-10-15 12:13:55.000000 astro-limepy-1.1/limepy/spes.py
--rwxrwxr-x   0 balbinot  (1000) balbinot  (1000)       61 2021-10-15 12:16:04.084529 astro-limepy-1.1/setup.cfg
--rwxrwxr-x   0 balbinot  (1000) balbinot  (1000)     1585 2021-10-15 12:15:16.000000 astro-limepy-1.1/setup.py
+drwxr-xr-x   0 mgieles    (501) wheel        (0)        0 2023-06-15 15:46:42.261183 astro-limepy-1.2/
+-rwxr--r--   0 mgieles    (501) wheel        (0)      136 2015-02-27 18:30:58.000000 astro-limepy-1.2/AUTHORS.rst
+-rw-r--r--   0 mgieles    (501) wheel        (0)     1068 2019-12-18 12:54:44.000000 astro-limepy-1.2/LICENSE
+-rw-r--r--   0 mgieles    (501) wheel        (0)     2102 2023-06-15 15:46:42.261251 astro-limepy-1.2/PKG-INFO
+-rwxr--r--   0 mgieles    (501) wheel        (0)     1374 2019-12-18 12:54:44.000000 astro-limepy-1.2/README.rst
+drwxr-xr-x   0 mgieles    (501) wheel        (0)        0 2023-06-15 15:46:42.252648 astro-limepy-1.2/astro_limepy.egg-info/
+-rw-r--r--   0 mgieles    (501) wheel        (0)     2102 2023-06-15 15:46:42.000000 astro-limepy-1.2/astro_limepy.egg-info/PKG-INFO
+-rw-r--r--   0 mgieles    (501) wheel        (0)      519 2023-06-15 15:46:42.000000 astro-limepy-1.2/astro_limepy.egg-info/SOURCES.txt
+-rw-r--r--   0 mgieles    (501) wheel        (0)        1 2023-06-15 15:46:42.000000 astro-limepy-1.2/astro_limepy.egg-info/dependency_links.txt
+-rw-r--r--   0 mgieles    (501) wheel        (0)        1 2020-02-26 10:12:50.000000 astro-limepy-1.2/astro_limepy.egg-info/not-zip-safe
+-rw-r--r--   0 mgieles    (501) wheel        (0)       20 2023-06-15 15:46:42.000000 astro-limepy-1.2/astro_limepy.egg-info/requires.txt
+-rw-r--r--   0 mgieles    (501) wheel        (0)        7 2023-06-15 15:46:42.000000 astro-limepy-1.2/astro_limepy.egg-info/top_level.txt
+drwxr-xr-x   0 mgieles    (501) wheel        (0)        0 2023-06-15 15:46:42.260558 astro-limepy-1.2/limepy/
+-rwxr--r--   0 mgieles    (501) wheel        (0)      227 2018-10-18 18:39:31.000000 astro-limepy-1.2/limepy/__init__.py
+-rw-r--r--   0 mgieles    (501) wheel        (0)      150 2020-04-09 08:37:12.000000 astro-limepy-1.2/limepy/dfspes.py
+-rwxr--r--   0 mgieles    (501) wheel        (0)    44739 2023-06-08 08:24:41.000000 astro-limepy-1.2/limepy/limepy.py
+-rwxr-xr-x   0 mgieles    (501) wheel        (0)    10315 2023-05-31 18:01:40.000000 astro-limepy-1.2/limepy/sample.py
+-rw-r--r--   0 mgieles    (501) wheel        (0)    10086 2020-02-26 09:51:06.000000 astro-limepy-1.2/limepy/sample2.py
+-rw-r--r--   0 mgieles    (501) wheel        (0)    10122 2020-02-26 09:52:20.000000 astro-limepy-1.2/limepy/sample3.py
+-rwxr--r--   0 mgieles    (501) wheel        (0)    30454 2023-06-15 15:23:45.000000 astro-limepy-1.2/limepy/spes.py
+-rwxr--r--   0 mgieles    (501) wheel        (0)    31471 2018-11-16 01:05:18.000000 astro-limepy-1.2/limepy/spes2.py
+-rw-r--r--   0 mgieles    (501) wheel        (0)      308 2020-12-28 20:24:34.000000 astro-limepy-1.2/limepy/test.py
+-rw-r--r--   0 mgieles    (501) wheel        (0)     2230 2018-10-18 18:56:01.000000 astro-limepy-1.2/limepy/test2.py
+-rw-r--r--   0 mgieles    (501) wheel        (0)      641 2020-12-28 20:40:53.000000 astro-limepy-1.2/limepy/test3.py
+-rw-r--r--   0 mgieles    (501) wheel        (0)      726 2020-04-09 08:42:11.000000 astro-limepy-1.2/limepy/test_normalisation.py
+-rw-r--r--   0 mgieles    (501) wheel        (0)      602 2021-10-06 10:40:36.000000 astro-limepy-1.2/limepy/test_sample.py
+-rwxr--r--   0 mgieles    (501) wheel        (0)       61 2023-06-15 15:46:42.261442 astro-limepy-1.2/setup.cfg
+-rwxr--r--   0 mgieles    (501) wheel        (0)     1536 2023-06-15 15:46:11.000000 astro-limepy-1.2/setup.py
+drwxr-xr-x   0 mgieles    (501) wheel        (0)        0 2023-06-15 15:46:42.260862 astro-limepy-1.2/tests/
+-rwxr--r--   0 mgieles    (501) wheel        (0)      378 2015-02-27 18:30:58.000000 astro-limepy-1.2/tests/test_limepy.py
```

### Comparing `astro-limepy-1.1/PKG-INFO` & `astro-limepy-1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 Metadata-Version: 2.1
 Name: astro-limepy
-Version: 1.1
+Version: 1.2
 Summary: Code to solve lowered isothermal model
 Home-page: https://github.com/mgieles/limepy
 Author: Mark Gieles, Alice Zocchi
 Author-email: m.gieles@surrey.ac.uk, a.zocchi@surrey.ac.uk
 License: MIT
-Description: LIMEPY 
-        ========
-        
-        Lowered Isothermal Model Explorer in PYthon
-        -------------------------------------------
-        
-        .. .. image:: https://badge.fury.io/py/limepy.png
-        ..     :target: http://badge.fury.io/py/limepy
-        ..
-        .. .. image:: https://travis-ci.org/mgieles/limepy.png?branch=master
-        ..         :target: https://travis-ci.org/mgieles/limepy
-        ..
-        .. .. image:: https://pypip.in/d/limepy/badge.png
-        ..         :target: https://pypi.python.org/pypi/limepy
-        
-        
-        Python environment for solving distribution function (DF) based
-        lowered isothermal models as described in Gieles & Zocchi 2015, MNRAS,
-        454, 576 (http://arxiv.org/abs/1508.02120)
-        
-        
-        Notebooks with example can be found in <https://github.com/mgieles/limepy/tree/master/notebooks>
-        
-        Also check out LIMEPY within the browser with mybinder
-        
-           .. image:: http://mybinder.org/badge.svg 
-                :target: http://mybinder.org/repo/mgieles/limepy
-        
-        
-        * Free software: BSD license
-        * Documentation: https://limepy.readthedocs.org. 
-        
-        .. image:: https://readthedocs.org/projects/limepy/badge/?version=latest
-        
-        :target: https://limepy.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-        
-        Features
-        --------
-        
-        * Solves Poisson's equation used on input parameters
-        * Fast solutions for isotropic/anisotropic, single/multi-mass models
-        * Normalised DF values
-        * Density and velocity moments
-        * Projected properties 
-        * Generate discrete samples
-        
-        
-        
-        
-        History
-        -------
-        
-        0.1.0 (2014-01-11)
-        ---------------------
-        
-        * First release on github. 
-        
 Keywords: limepy
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+LIMEPY 
+========
+
+Lowered Isothermal Model Explorer in PYthon
+-------------------------------------------
+
+.. .. image:: https://badge.fury.io/py/limepy.png
+..     :target: http://badge.fury.io/py/limepy
+..
+.. .. image:: https://travis-ci.org/mgieles/limepy.png?branch=master
+..         :target: https://travis-ci.org/mgieles/limepy
+..
+.. .. image:: https://pypip.in/d/limepy/badge.png
+..         :target: https://pypi.python.org/pypi/limepy
+
+
+Python environment for solving distribution function (DF) based
+lowered isothermal models as described in Gieles & Zocchi 2015, MNRAS,
+454, 576 (http://arxiv.org/abs/1508.02120)
+
+
+Notebooks with example can be found in <https://github.com/mgieles/limepy/tree/master/notebooks>
+
+Also check out LIMEPY within the browser with mybinder
+
+   .. image:: http://mybinder.org/badge.svg 
+        :target: http://mybinder.org/repo/mgieles/limepy
+
+
+* Free software: BSD license
+* Documentation: https://limepy.readthedocs.org. 
+
+.. image:: https://readthedocs.org/projects/limepy/badge/?version=latest
+
+:target: https://limepy.readthedocs.io/en/latest/?badge=latest
+:alt: Documentation Status
+
+Features
+--------
+
+* Solves Poisson's equation used on input parameters
+* Fast solutions for isotropic/anisotropic, single/multi-mass models
+* Normalised DF values
+* Density and velocity moments
+* Projected properties 
+* Generate discrete samples
+
+
+
+
+History
+-------
+
+0.1.0 (2014-01-11)
+---------------------
+
+* First release on github.
```

### Comparing `astro-limepy-1.1/README.rst` & `astro-limepy-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `astro-limepy-1.1/astro_limepy.egg-info/PKG-INFO` & `astro-limepy-1.2/astro_limepy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 Metadata-Version: 2.1
 Name: astro-limepy
-Version: 1.1
+Version: 1.2
 Summary: Code to solve lowered isothermal model
 Home-page: https://github.com/mgieles/limepy
 Author: Mark Gieles, Alice Zocchi
 Author-email: m.gieles@surrey.ac.uk, a.zocchi@surrey.ac.uk
 License: MIT
-Description: LIMEPY 
-        ========
-        
-        Lowered Isothermal Model Explorer in PYthon
-        -------------------------------------------
-        
-        .. .. image:: https://badge.fury.io/py/limepy.png
-        ..     :target: http://badge.fury.io/py/limepy
-        ..
-        .. .. image:: https://travis-ci.org/mgieles/limepy.png?branch=master
-        ..         :target: https://travis-ci.org/mgieles/limepy
-        ..
-        .. .. image:: https://pypip.in/d/limepy/badge.png
-        ..         :target: https://pypi.python.org/pypi/limepy
-        
-        
-        Python environment for solving distribution function (DF) based
-        lowered isothermal models as described in Gieles & Zocchi 2015, MNRAS,
-        454, 576 (http://arxiv.org/abs/1508.02120)
-        
-        
-        Notebooks with example can be found in <https://github.com/mgieles/limepy/tree/master/notebooks>
-        
-        Also check out LIMEPY within the browser with mybinder
-        
-           .. image:: http://mybinder.org/badge.svg 
-                :target: http://mybinder.org/repo/mgieles/limepy
-        
-        
-        * Free software: BSD license
-        * Documentation: https://limepy.readthedocs.org. 
-        
-        .. image:: https://readthedocs.org/projects/limepy/badge/?version=latest
-        
-        :target: https://limepy.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-        
-        Features
-        --------
-        
-        * Solves Poisson's equation used on input parameters
-        * Fast solutions for isotropic/anisotropic, single/multi-mass models
-        * Normalised DF values
-        * Density and velocity moments
-        * Projected properties 
-        * Generate discrete samples
-        
-        
-        
-        
-        History
-        -------
-        
-        0.1.0 (2014-01-11)
-        ---------------------
-        
-        * First release on github. 
-        
 Keywords: limepy
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+LIMEPY 
+========
+
+Lowered Isothermal Model Explorer in PYthon
+-------------------------------------------
+
+.. .. image:: https://badge.fury.io/py/limepy.png
+..     :target: http://badge.fury.io/py/limepy
+..
+.. .. image:: https://travis-ci.org/mgieles/limepy.png?branch=master
+..         :target: https://travis-ci.org/mgieles/limepy
+..
+.. .. image:: https://pypip.in/d/limepy/badge.png
+..         :target: https://pypi.python.org/pypi/limepy
+
+
+Python environment for solving distribution function (DF) based
+lowered isothermal models as described in Gieles & Zocchi 2015, MNRAS,
+454, 576 (http://arxiv.org/abs/1508.02120)
+
+
+Notebooks with example can be found in <https://github.com/mgieles/limepy/tree/master/notebooks>
+
+Also check out LIMEPY within the browser with mybinder
+
+   .. image:: http://mybinder.org/badge.svg 
+        :target: http://mybinder.org/repo/mgieles/limepy
+
+
+* Free software: BSD license
+* Documentation: https://limepy.readthedocs.org. 
+
+.. image:: https://readthedocs.org/projects/limepy/badge/?version=latest
+
+:target: https://limepy.readthedocs.io/en/latest/?badge=latest
+:alt: Documentation Status
+
+Features
+--------
+
+* Solves Poisson's equation used on input parameters
+* Fast solutions for isotropic/anisotropic, single/multi-mass models
+* Normalised DF values
+* Density and velocity moments
+* Projected properties 
+* Generate discrete samples
+
+
+
+
+History
+-------
+
+0.1.0 (2014-01-11)
+---------------------
+
+* First release on github.
```

### Comparing `astro-limepy-1.1/limepy/limepy.py` & `astro-limepy-1.2/limepy/limepy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 # -*- coding: utf-8 -*-
 
 import numpy
 import scipy
 from scipy.interpolate import BPoly, interp1d, UnivariateSpline
 from numpy import exp, sqrt, pi, sin, cos, log10
 from scipy.special import gamma, gammainc, hyp1f1
@@ -241,14 +242,16 @@
 
     def _set_kwargs(self, phi0, g, **kwargs):
         """ Set parameters and scales """
 
         if (g<0): raise ValueError("Error: g must be larger or equal to 0")
         if (g>=3.5): raise ValueError("Error: for g>=3.5 models are infinite")
 
+        if (phi0<=0): raise ValueError("Error: phi0 must be larger than 0")
+
         self.model = "limepy"
         
         # ROT
         self.omega = 0
 
         self.phi0, self.g = phi0, g
         self._MS, self._RS, self._GS = None, None, None
@@ -279,37 +282,37 @@
         self.nstep=1
         self.converged=True
         self._interpolator_set=False
 
         if kwargs is not None:
             for key, value in kwargs.items():
                 # Check for scaling input
-                if key is 'G':
+                if key == 'G':
                     self._GS, self.scale = value, True
-                elif key is 'M':
+                elif key == 'M':
                     self._MS, self.scale = value, True
-                elif key is 'r0':
+                elif key == 'r0':
                     if self.scale_radius is None:
                         self._RS,self.scale_radius,self.scale = value,'r0', True
                     else:
                         error="Can not set scale radius to r0,already set to %s"
                         raise ValueError(error%self.scale_radius)
-                elif key is 'rh':
+                elif key == 'rh':
                     if self.scale_radius is None:
                         self._RS, self.scale_radius, self.scale=value,'rh', True
                     else:
                         error="Can not set scale radius to rh,already set to %s"
                         raise ValueError(error%self.scale_radius)
-                elif key is 'rv':
+                elif key == 'rv':
                     if self.scale_radius is None:
                         self._RS, self.scale_radius, self.scale=value,'rv', True
                     else:
                         error="Can not set scale radius to rv,already set to %s"
                         raise ValueError(error%self.scale_radius)
-                elif key is 'rt':
+                elif key == 'rt':
                     if self.scale_radius is None:
                         self._RS, self.scale_radius, self.scale=value,'rt', True
                     else:
                         error="Can not set scale radius to rt,already set to %s"
                         raise ValueError(error%self.scale_radius)
                 else:
                     # Set input parameters
@@ -447,15 +450,14 @@
 
         # Extrapolate to r_t:
         # phi(r) =~ a(r_t -r)
         # a = GM/r_t^2
         GM = -self.G*sum(sol.y[1:1+self.nmbin])
         p = 2*sol.y[0]*self.r[-1]/GM
 
-#        print(" TEST ",sol.y)
         if (p<=0.5):
             rtfac = (1 - sqrt(1-2*p))/p
             self.rt = rtfac*self.r[-1] if (rtfac > 1) else 1.0000001*self.r[-1]
         else:
             self.rt = 1.000001*self.r[-1]
 
         # Set the converged flag to True if successful
@@ -677,20 +679,19 @@
     def _odes(self, x, y, potonly):
         """ Solve ODEs """
         # y = [phi, u_j, U, K_j], where u = -M(<r)/G
         if (self.multi):
             derivs = [numpy.sum(y[1:1+self.nmbin])/x**2] if (x>0) else [0]
             for j in range(self.nmbin):
                 phi = y[0]/self.s2j[j]
-                derivs.append(-9.0*x**2*self.alpha[j]*self._rhohat(phi, x, j))
-#            print(" DERIVS = ",x,derivs,self.nmbin)
+                derivs.append(-9.0*x**2*self.alpha[j]*self._rhohat(phi, x, j)[0])
             dUdx  = 2.0*pi*numpy.sum(derivs[1:1+self.nmbin])*y[0]/9.
         else:
             derivs = [y[1]/x**2] if (x>0) else [0]
-            derivs.append(-9.0*x**2*self._rhohat(y[0], x, 0))
+            derivs.append(-9.0*x**2*self._rhohat(y[0], x, 0)[0])
 
             dUdx  = 2.0*pi*derivs[1]*y[0]/9.
 
         derivs.append(dUdx)
 
         # Calculate pressure tensor components for all the mass bins
         if (not potonly): #dK_j/dx
@@ -708,14 +709,15 @@
                 derivs.append(rhov2j[j])
 
             for j in range(self.nmbin):
                 derivs.append(rhov2rj[j])
 
         dVdvdr = (4*pi)**2*x**2 * (2*y[0])**1.5/3 if (x>0) and (y[0]>0) else 0
         derivs.append(dVdvdr)
+#        print("TEST",derivs)
         return derivs
 
     
     # ROT: UNDER CONSTRUCTIONS  ##############
     def _poisson_rot(self):
         self._init_rot()
         diff_rot = 1e99
@@ -856,14 +858,15 @@
             if (self.multi):
                 self.rhoj = self.rhohatj * Mstar/Rstar**3
                 for j in range(self.nmbin):
                     self.rhoj[j] *= self.alpha[j]
                 self.Mj *= Mstar # 28/1/19 Thanks to William
 
                 self.mcj *= Mstar
+                self.r0j *= Rstar
                 self.rhj *= Rstar
                 self.v2j,self.v2rj,self.v2tj=(q*v2star for q in
                                               [self.v2j, self.v2rj,self.v2tj])
 
                 self.kj *= Mstar*v2star
                 self.Krj *= Mstar*v2star
                 self.Ktj *= Mstar*v2star
@@ -1163,7 +1166,9 @@
             DF[c] *= self.A[j]
 
         else:
 	        DF = numpy.zeros(max(len(r),len(v)))
 
         return DF
 
+
+###k=limepy(4,1,project=True,M=1,G=1,rv=1,mj=[0.1,1],Mj=[1,0.1],verbose=True)
```

### Comparing `astro-limepy-1.1/limepy/sample.py` & `astro-limepy-1.2/limepy/sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from __future__ import division
 import numpy
 import scipy
 from numpy import exp, sqrt, pi, sin, cos
 from scipy.special import  gammainc, dawsn, erfi
-from scipy import random
+from numpy import random
 from scipy import optimize
 from math import factorial
 
 class sample:
     def __init__(self, mod, **kwargs):
         r""""
 
@@ -218,15 +218,15 @@
             else:
                 xsamp = numpy.r_[xsamp, xtmp[~c]]
                 r = numpy.r_[r, rtmp[~c]]
             iter+=1
 
         # Shuffle before assigning to avoid correlations (6/10/21)
         id = numpy.arange(len(r))
-        numpy.random.shuffle(id)
+        random.shuffle(id)
         xsamp = xsamp[id]
         r = r[id]
             
         # Assign final velocities and update r because of shuffling
         self.k = numpy.r_[self.k, xsamp**(2./3)]
         self.v = numpy.r_[self.v, sqrt(2*xsamp**(2./3)*self.mod.s2)]
         self.rfinal = numpy.r_[self.rfinal, r]
```

### Comparing `astro-limepy-1.1/limepy/spes.py` & `astro-limepy-1.2/limepy/spes.py`

 * *Files 1% similar despite different names*

```diff
@@ -842,11 +842,10 @@
             
             # Compute the DF: eq. (3) in C19
             DF[c] = exp(E[c]) - self.B - self.C*E[c]
             DF[~c] = (1-self.B)*exp(E[~c]/self.eta**2)
             
             DF *= self.A
         else:
-	    DF = numpy.zeros(max(len(r),len(v)))
-
+            DF = numpy.zeros(max(len(r),len(v)))
         return DF
```

### Comparing `astro-limepy-1.1/setup.py` & `astro-limepy-1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 test_requirements = [
     # TODO: put package test requirements here
 ]
 
 setup(
     name='astro-limepy',
-    version='1.1',
+    version='1.2',
     description='Code to solve lowered isothermal model',
     long_description=long_description + "\n\n" + history,
     long_description_content_type='text/x-rst',
     author='Mark Gieles, Alice Zocchi',
     author_email='m.gieles@surrey.ac.uk, a.zocchi@surrey.ac.uk',
     url='https://github.com/mgieles/limepy',
     packages=[
@@ -40,14 +40,13 @@
     zip_safe=False,
     keywords='limepy',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
-        "Programming Language :: Python :: 2",
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
+        "Programming Language :: Python :: 3",
+        'Programming Language :: Python :: 3.9',
     ],
     test_suite='tests',
     tests_require=test_requirements
 )
```

