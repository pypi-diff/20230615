# Comparing `tmp/AlgDiff-2.0.2.tar.gz` & `tmp/AlgDiff-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgDiff-2.0.2.tar", last modified: Thu Jun 15 16:03:44 2023, max compression
+gzip compressed data, was "AlgDiff-2.1.tar", last modified: Thu Jun 15 19:47:41 2023, max compression
```

## Comparing `AlgDiff-2.0.2.tar` & `AlgDiff-2.1.tar`

### file list

```diff
@@ -1,7 +1,16 @@
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 16:03:44.653376 AlgDiff-2.0.2/
-drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 16:03:44.653376 AlgDiff-2.0.2/AlgDiff/
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.438138 AlgDiff-2.0.2/AlgDiff/__init__.py
--rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41426 2023-06-15 14:57:11.442138 AlgDiff-2.0.2/AlgDiff/algebraicDifferentiator.py
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     2630 2023-06-15 16:03:44.653376 AlgDiff-2.0.2/PKG-INFO
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       40 2023-06-15 16:02:49.141501 AlgDiff-2.0.2/setup.cfg
--rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1156 2023-06-15 16:03:37.877391 AlgDiff-2.0.2/setup.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 19:47:41.138824 AlgDiff-2.1/
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 19:47:41.138824 AlgDiff-2.1/AlgDiff/
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)       68 2023-06-15 14:57:11.000000 AlgDiff-2.1/AlgDiff/__init__.py
+-rwxrwxr-x   0 aothmane  (1000) aothmane  (1000)    41507 2023-06-15 19:36:33.000000 AlgDiff-2.1/AlgDiff/algebraicDifferentiator.py
+drwxrwxr-x   0 aothmane  (1000) aothmane  (1000)        0 2023-06-15 19:47:41.138824 AlgDiff-2.1/AlgDiff.egg-info/
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    14532 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      260 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/SOURCES.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        1 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/dependency_links.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       19 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/requires.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)        8 2023-06-15 19:47:41.000000 AlgDiff-2.1/AlgDiff.egg-info/top_level.txt
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1458 2023-06-06 12:55:23.000000 AlgDiff-2.1/LICENSE
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    14532 2023-06-15 19:47:41.138824 AlgDiff-2.1/PKG-INFO
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)    12074 2023-06-15 16:15:25.000000 AlgDiff-2.1/README.md
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)      871 2023-06-15 19:36:33.000000 AlgDiff-2.1/pyproject.toml
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)       79 2023-06-15 19:47:41.138824 AlgDiff-2.1/setup.cfg
+-rw-rw-r--   0 aothmane  (1000) aothmane  (1000)     1154 2023-06-15 19:36:33.000000 AlgDiff-2.1/setup.py
```

### Comparing `AlgDiff-2.0.2/AlgDiff/algebraicDifferentiator.py` & `AlgDiff-2.1/AlgDiff/algebraicDifferentiator.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,21 +46,22 @@
         It should take the value None if the cutoff frequency is
         specified.
     :type T: float
     :param wc: Cutoff frequency of the differentiator. Takes a positive values
         if the cutoff frequency has to be specified. The filter window length
         is then computed automatically. It should take the value None 
         if the filter window length is specified.
+    :type wc: float
     :type T: float
     :param display: Boolean variable indicating if all the information
         characterizing the differentiator should be printed.
-    :type display: Bool
+    :type display: bool
     :param corr: Boolean variable that indicates if errors in the DC component of the 
         approximated signal stemming from the discretization should be corrected.
-    :type corr: Bool
+    :type corr: bool
 
     """
 
     ## The constructor    
     def __init__(self, ts=0.01, alpha=1., beta=1., N=0, T=1., wc =
                  None,display=True,corr=True):
         # Sampling period
@@ -129,41 +130,36 @@
 
         :param der: Order of the derivative to be estimated.
         :type der: int
         :param method: Discretization scheme: "mid-point", "trapezoidal",\
             "analytic", "simpson rule".
         :type method: string
         :param reduceFilLength: Reduce or not the filter window length.
-        :type reduceFilLength: Bool
+        :type reduceFilLength: bool
         :param redTol: Tolerance to be used when the filter length is reduced.
         :type redTol: float.
         :param discreteSpectrum: If it is set, then the parameter \
             :math:`\\theta` used in the discretization is returned. See survey paper
             for more details.
-        :type discreteSpectrum: Bool
+        :type discreteSpectrum: bool
         
-        Returns
-        -------
-        coeff: dictionary
-            Discretized filter in a dict where the keys are the derivative
-            for which a filter has been discretized. Each element is a dict. with
-            keys the used discretization methods. If the correction of the DC
-            component has been enabled with the parameter corr of the class
-            initialization, this output contains the corrected filter coefficients.
-
-        tau_1: float
-            If redFilLength is set, tau_1 is the time where the filter window is reduced
-            before at the left side of the interval. The estimation delay is 
-            reduced by tau_1.
-        tau_2: float
-            If redFilLength is set, tau_2 is the time where the filter window is reduced
-            before at the right side of the interval. This value does not affect the
-            delay.
-        theta: float
-            If discreteSpectrum is set then the parameter :math:`\\theta` is also returned.
+        :returns:
+        	- coeff (dictionary) - Discretized filter in a dict where the keys are the derivative \
+            		for which a filter has been discretized. Each element is a dict. with \
+            		keys the used discretization methods. If the correction of the DC \
+            		component has been enabled with the parameter corr of the class \
+            		initialization, this output contains the corrected filter coefficients.
+        	- tau_1 (:py:class:`float`) - If redFilLength is set, tau_1 is the time where the filter \
+        		window is reduced \
+            		before at the left side of the interval. The estimation delay is reduced by tau_1.
+        	- tau_2 (:py:class:`float`) - If redFilLength is set, tau_2 is the time where the filter \
+        	 	window is reduced\
+            		before at the right side of the interval. This value does not affect the delay.
+        	- theta (:py:class:`float`) - If discreteSpectrum is set then the parameter\
+        		 :math:`\\theta` is also returned.
         """
         theta0 = 0
         theta = theta0
         L0 = int(self.__T/self.__ts)
         red = ""
         tau1 = 0
         
@@ -414,15 +410,15 @@
                 "trapezoidal", "analytic"
 
         :type method: string
         :type conv: string
         :param reduceFilterLength: Specify whether or not the filter window
                 length should be reduced or not. See the discretize method for more
                 details.
-        :type reduceFilterLength: Bool
+        :type reduceFilterLength: bool
         :param redTol: Tolerance to be used when the filter length is reduced
         :type redTol: float.
         :return: Estimated derivative in a numpy array with the same dimensions
             as the variable x
         """
         red = ""
         if redFilLength:
@@ -652,20 +648,17 @@
         Fourier transform of the algebraic differentiator\
         at the frequencies omega.
 
         :param omega: Frequencies where the amplitude and phase should be \
                         evaluated
         :type omega: numpy array
         
-        Returns
-        -------
-        amp: numpy array
-            Amplitude of the Fourier transform of the filter.
-        phase: numpy array 
-            Phase of the Fourier transform of the filter.
+        :returns:
+        	- amp (:py:class:`numpy array`) - Amplitude of the Fourier transform of the filter.
+        	- phase (:py:class:`numpy array`) - Phase of the Fourier transform of the filter.
         """
 
         mp.dps = 150; mp.pretty = True
         a = self.__alpha
         b = self.__beta
         theta = self.__theta
         F = 0
@@ -700,22 +693,17 @@
         :param n: Derivative to be estimated.
         :type n: integer
 
         :param method: Method used for the discretization: "mid-point",
             "trapezoidal", "analytic".
         :type method: string 
         
-        Returns
-        -------
-        amplitude: numpy array
-            Amplitude of the Fourier transform of the discretized
-            filter evaluated at omega. 
-        phase: numpy array 
-            Phase of the Fourier transform of the discretized
-            filter evaluated at omega.
+        :returns:
+        	- amplitude (:py:class:`numpy array`) - Amplitude of the Fourier transform of the discretized filter evaluated at omega. 
+        	- phase (:py:class:`numpy array`) - Phase of the Fourier transform of the discretized filter evaluated at omega.
         """
         w,theta = self.discretize(n,method,discreteSpectrum=True)
         k = np.arange(0,len(w[n][method]))
         Gdis =  np.array([np.exp(-1j*omegai*(k+theta)*self.__ts).dot(w[n][method]) for omegai in omega])
         return np.abs(Gdis), np.unwrap(np.angle(Gdis))
 
     def get_asymptotesAmpFilter(self,omega):
@@ -726,22 +714,18 @@
         frequencies greater than the cutoff frequency.
 
         The function also return the approximation as a low pass filter.
 
         :param omega: Frequencies where the bounds should be evaluated
         :type omega: numpy array
 
-        Returns
-        -------
-        up: numpy array
-            Upper bound for the amplitude spectrum evaluated at omega..
-        lb: numpy array
-            Lower bound for the amplitude spectrum evaluated at omega..
-        mb: numpy array
-            Lowpass approximation of the filter evaluated at omega..
+        :returns:
+	        - ub - (:py:class:`numpy array`) - Upper bound for the amplitude spectrum evaluated at omega..
+        	- lb - (:py:class:`numpy array`) -  Lower bound for the amplitude spectrum evaluated at omega..
+        	- mb - (:py:class:`numpy array`) - Lowpass approximation of the filter evaluated at omega..
         """
 
         kappa = np.abs(self.__beta-self.__alpha)
         mu = 1+np.minimum(self.__beta,self.__alpha)
         if self.__beta>=self.__alpha:
             sigma = 1
         else:
@@ -779,17 +763,18 @@
 
     def computeTfromWc(self,wc):
         """
         This function computes the filter window length for a desired
         cutoff frequency.
 
         :param wc: Cutoff frequency.
-        :param type: float
+        :type wc: float
 
-        :return: T as a float
+        :returns:
+        	- T (:py:class:`float`) -  filter window length
         """
 
         kappa = np.abs(self.__beta-self.__alpha)
         mu = 1+np.minimum(self.__beta,self.__alpha)
         if self.__beta>=self.__alpha:
             sigma = 1
         else:
@@ -935,15 +920,15 @@
 
         :param theta: Parameter :math:`\\vartheta` of the algebraic
             differentiator.
         :type theta: float
         :param rootJacobiPol: True if the value theta is equal to a zero of\
         the jacobi polynomial of order :math:`N+1`. For the delay-free
             approximation use False, since :math:`1` is not a zero.
-        :type rootJacobiPol: Bool
+        :type rootJacobiPol: bool
         """
 
         self.__thetaBool = rootJacobiPol
         self.__theta = theta
         for der in self.__w.keys():
             for m in self.__w[der].keys():
                 tmp = self.discretize(der,m)
@@ -1016,35 +1001,29 @@
     def reduceFilterLength(self,der,tol=0.01):
         """ This function returns a distribution function that can
         be used to reduce the filter window length. The length is reduced such
         that the truncation is of the same amount on both sides of the filter
         window.
 
         :param der: The sought derivative.
-        :type der: integer
+        :type der: int
         
         :param tol: The tolerance that for reducing the filter length
         :type tol: float
         
-        Returns
-        -------
-        tau1: float
-            New starting point of the window. The value 0, i.e., the old
-            starting point, is taken as the reference.
-        tau2: float
-            New end point of the window. The value 0, i.e., the old starting
-            point, is taken as the reference.
-        d: numpy array
-            Distribution function used for the truncation.
-        t: numpy array
-            Times instants where distribution function has been evaluated.
-        n: int
-            Factor relating the sampling rate of the measurements and the
-            sampling rate used for the evaluation of the distribution
-            function.
+        :returns:
+        	- tau1 (:py:class:`float`) - New starting point of the window. The value 0, i.e., the old
+            		starting point, is taken as the reference.
+        	- tau2 (:py:class:`float`) - New end point of the window. The value 0, i.e., the old starting
+           	 	point, is taken as the reference.
+        	- d (:py:class:`numpy array`) - Distribution function used for the truncation.
+        	- t (:py:class:`numpy array`) - Times instants where distribution function has been evaluated.
+        	- n (:py:class:`int`) - Factor relating the sampling rate of the measurements and the
+			    sampling rate used for the evaluation of the distribution
+			    function.
         """
         # Compute the first moment of the n-th derivative of the kernel
         n = 10
         t = np.arange(0,self.__T,self.__ts/n)
         g = self.evalKernelDer(t,der)
         m0 = np.trapz(np.abs(g),x=t)
```

### Comparing `AlgDiff-2.0.2/setup.py` & `AlgDiff-2.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "docs/source/usage.rst").read_text()
 
 setup(
   name = 'AlgDiff',
   packages = ['AlgDiff'],
-  version = '2.0.2',
+  version = '2.1',
   license='bsd-3-clause',
   description = 'AlgDiff is a Python class implementing all necessary tools for the design, analysis, and discretization of algebraic differentiators. An interface to Matlab is also provided.',
   
   long_description = long_description,
   long_description_content_type='text/x-rst',
   
   author = 'Amine Othmane',
   author_email = 'amine.othmane@uni-saarland.de',
   url = 'https://github.com/aothmane-control/Algebraic-differentiators',
-  download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.0',
+  download_url = 'https://github.com/aothmane-control/Algebraic-differentiators/releases/tag/v2.1',
   keywords = ['numerical-differentiation ', 'fir-filters', 'orthogonal-polynomials', 'numerical-methods '],
   install_requires=[            # I get to this in a second
           'scipy',
           'mpmath',
           'numpy',
       ],
   classifiers=[
```

