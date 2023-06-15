# Comparing `tmp/ps_eor-0.8.tar.gz` & `tmp/ps_eor-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ps_eor-0.8.tar", max compression
+gzip compressed data, was "ps_eor-0.9.tar", max compression
```

## Comparing `ps_eor-0.8.tar` & `ps_eor-0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     7651 2020-03-25 08:37:44.620212 ps_eor-0.8/LICENSE
--rw-r--r--   0        0        0     5824 2020-10-26 10:04:39.365910 ps_eor-0.8/README.md
--rw-r--r--   0        0        0      167 2021-04-30 16:35:08.706804 ps_eor-0.8/ps_eor/__init__.py
--rw-r--r--   0        0        0    69947 2021-04-30 10:42:09.123492 ps_eor-0.8/ps_eor/datacube.py
--rw-r--r--   0        0        0    19141 2021-04-15 10:26:02.743643 ps_eor-0.8/ps_eor/fgfit.py
--rw-r--r--   0        0        0    34584 2021-04-30 09:41:44.661347 ps_eor-0.8/ps_eor/fitutil.py
--rw-r--r--   0        0        0    18549 2021-04-30 10:40:44.915154 ps_eor-0.8/ps_eor/flagger.py
--rw-r--r--   0        0        0    35683 2021-04-30 10:36:23.426147 ps_eor-0.8/ps_eor/ml_gpr.py
--rw-r--r--   0        0        0    10422 2020-10-26 10:04:39.381909 ps_eor-0.8/ps_eor/pscart.py
--rw-r--r--   0        0        0    67769 2021-04-30 10:43:28.215813 ps_eor-0.8/ps_eor/pspec.py
--rw-r--r--   0        0        0     2149 2019-10-24 08:06:50.545982 ps_eor-0.8/ps_eor/pssph.py
--rw-r--r--   0        0        0    39161 2021-04-29 20:09:19.733750 ps_eor-0.8/ps_eor/psutil.py
--rw-r--r--   0        0        0    29517 2019-10-29 12:28:02.112809 ps_eor-0.8/ps_eor/simu.py
--rw-r--r--   0        0        0    15388 2020-10-26 10:04:39.385909 ps_eor-0.8/ps_eor/sphcube.py
--rw-r--r--   0        0        0    35791 2019-10-31 12:51:05.840964 ps_eor-0.8/ps_eor/sphutil.py
--rw-r--r--   0        0        0    21963 2021-03-10 16:27:47.600431 ps_eor-0.8/ps_eor/tests/test_datacube.py
--rw-r--r--   0        0        0        0 2020-10-26 10:04:39.389909 ps_eor-0.8/ps_eor/tools/__init__.py
--rw-r--r--   0        0        0     2171 2020-10-26 10:04:39.393909 ps_eor-0.8/ps_eor/tools/instru/lofar_statpos.data
--rw-r--r--   0        0        0     1612 2020-10-26 10:04:39.393909 ps_eor-0.8/ps_eor/tools/instru/nenufar52_statpos.data
--rw-r--r--   0        0        0    10976 2020-10-26 10:04:39.393909 ps_eor-0.8/ps_eor/tools/instru/skalow_enu_statpos.data
--rwxr-xr-x   0        0        0    55868 2021-04-30 10:43:57.759934 ps_eor-0.8/ps_eor/tools/pstool.py
--rw-r--r--   0        0        0      797 2021-04-30 16:35:19.930862 ps_eor-0.8/pyproject.toml
--rw-r--r--   0        0        0     7214 2021-04-30 16:41:28.628277 ps_eor-0.8/setup.py
--rw-r--r--   0        0        0     7033 2021-04-30 16:41:28.629536 ps_eor-0.8/PKG-INFO
+-rw-r--r--   0        0        0     7651 2020-03-25 08:37:44.620212 ps_eor-0.9/LICENSE
+-rw-r--r--   0        0        0     5824 2020-10-26 10:04:39.365910 ps_eor-0.9/README.md
+-rw-r--r--   0        0        0      167 2021-04-30 16:35:08.706804 ps_eor-0.9/ps_eor/__init__.py
+-rw-r--r--   0        0        0    69573 2021-05-04 19:53:37.943672 ps_eor-0.9/ps_eor/datacube.py
+-rw-r--r--   0        0        0    19141 2021-04-15 10:26:02.743643 ps_eor-0.9/ps_eor/fgfit.py
+-rw-r--r--   0        0        0    34584 2021-04-30 09:41:44.661347 ps_eor-0.9/ps_eor/fitutil.py
+-rw-r--r--   0        0        0    18549 2021-04-30 10:40:44.915154 ps_eor-0.9/ps_eor/flagger.py
+-rw-r--r--   0        0        0    35683 2021-04-30 10:36:23.426147 ps_eor-0.9/ps_eor/ml_gpr.py
+-rw-r--r--   0        0        0    10422 2020-10-26 10:04:39.381909 ps_eor-0.9/ps_eor/pscart.py
+-rw-r--r--   0        0        0    67701 2021-05-04 19:37:12.225546 ps_eor-0.9/ps_eor/pspec.py
+-rw-r--r--   0        0        0     2149 2019-10-24 08:06:50.545982 ps_eor-0.9/ps_eor/pssph.py
+-rw-r--r--   0        0        0    39629 2021-05-04 20:13:04.353210 ps_eor-0.9/ps_eor/psutil.py
+-rw-r--r--   0        0        0    29517 2019-10-29 12:28:02.112809 ps_eor-0.9/ps_eor/simu.py
+-rw-r--r--   0        0        0    15388 2020-10-26 10:04:39.385909 ps_eor-0.9/ps_eor/sphcube.py
+-rw-r--r--   0        0        0    35791 2019-10-31 12:51:05.840964 ps_eor-0.9/ps_eor/sphutil.py
+-rw-r--r--   0        0        0    21963 2021-03-10 16:27:47.600431 ps_eor-0.9/ps_eor/tests/test_datacube.py
+-rw-r--r--   0        0        0        0 2020-10-26 10:04:39.389909 ps_eor-0.9/ps_eor/tools/__init__.py
+-rw-r--r--   0        0        0     2171 2020-10-26 10:04:39.393909 ps_eor-0.9/ps_eor/tools/instru/lofar_statpos.data
+-rw-r--r--   0        0        0     1612 2020-10-26 10:04:39.393909 ps_eor-0.9/ps_eor/tools/instru/nenufar52_statpos.data
+-rw-r--r--   0        0        0    10976 2020-10-26 10:04:39.393909 ps_eor-0.9/ps_eor/tools/instru/skalow_enu_statpos.data
+-rwxr-xr-x   0        0        0    55868 2021-05-06 13:30:00.382957 ps_eor-0.9/ps_eor/tools/pstool.py
+-rw-r--r--   0        0        0      797 2021-05-06 13:26:37.534395 ps_eor-0.9/pyproject.toml
+-rw-r--r--   0        0        0     7214 2021-05-06 13:31:14.721288 ps_eor-0.9/setup.py
+-rw-r--r--   0        0        0     7033 2021-05-06 13:31:14.722509 ps_eor-0.9/PKG-INFO
```

### Comparing `ps_eor-0.8/LICENSE` & `ps_eor-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/README.md` & `ps_eor-0.9/README.md`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/datacube.py` & `ps_eor-0.9/ps_eor/datacube.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,22 +139,15 @@
         else:
             return WindowFunction('boxcar')
 
     def to_meta(self, image_meta):
         image_meta.set('PEWINFCT', '%s_%s' % (self.name, self.circular))
 
     def generate_window(self, nx):
-        w = get_window(self.name, nx)
-        if self.circular:
-            m = (nx - 1) // 2
-            x = np.linspace(-m, m, nx)
-            xx, yy = np.meshgrid(x, x)
-            return np.interp(np.sqrt(xx ** 2 + yy ** 2), x, w)
-        else:
-            return np.outer(w, w)
+        return psutil.generate_2d_window(self.name, nx, circular=self.circular)
 
     def generate(self, meta_data):
         return self.generate_window(meta_data.shape[0])
 
 
 class BasePrimaryBeam(Mask):
 
@@ -200,21 +193,15 @@
     def get_fwhm(self, freq=None):
         freq = self.get_freq(freq)
         assert freq is not None
         lamb = const.c.value / freq
         return self.alpha_tapering * lamb / self.antenna_diameter
 
     def generate_beam(self, fwhm, res, shape):
-        nx, ny = shape
-
-        thxval = res * np.arange(-nx / 2., nx / 2.)
-        thyval = res * np.arange(-ny / 2., ny / 2.)
-        thx, thy = np.meshgrid(thxval, thyval)
-
-        return psutil.get_beam(np.sqrt(thx ** 2 + thy ** 2), self.beam_type, fwhm, None)
+        return psutil.get_beam_cart(res, tuple(shape), self.beam_type, fwhm, n_sidelobe=None)
 
     def generate(self, meta_data, freq=None):
         fwhm = self.get_fwhm(freq=freq)
         return self.generate_beam(fwhm, meta_data.res, meta_data.shape)
 
 
 class LofarHBAPrimaryBeam(PrimaryBeam):
```

### Comparing `ps_eor-0.8/ps_eor/fgfit.py` & `ps_eor-0.9/ps_eor/fgfit.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/fitutil.py` & `ps_eor-0.9/ps_eor/fitutil.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/flagger.py` & `ps_eor-0.9/ps_eor/flagger.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/ml_gpr.py` & `ps_eor-0.9/ps_eor/ml_gpr.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/pscart.py` & `ps_eor-0.9/ps_eor/pscart.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/pspec.py` & `ps_eor-0.9/ps_eor/pspec.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,14 @@
         self.primary_beam.set_freq(self.eor.mfreq)
 
         self.set_redshift(self.eor.z)
 
         self._setup_cache()
 
     def _setup_cache(self):
-        self.omega_cache = psutil.Cache(self.get_omega)
         self.ps_cov_cache = psutil.Cache(self._get_ps_cov_err)
         self.ps2d_cov_cache = psutil.Cache(self._get_ps2d_cov_err)
         self.ps3d_cov_cache = psutil.Cache(self._get_ps3d_cov_err)
         self.window_cache = psutil.Cache(self._compute_window)
 
     def _compute_delays(self):
         self.delay = psutil.get_delay(self.eor.freqs, M=self.eor.M, half=self.config.ps2d_pos_only,
@@ -666,15 +665,15 @@
             ps_config (PowerSpectraConfig): A PS configuration
             primary_beam (PrimaryBeam): The primary beam of the instrument
         """
         BasePowerSpectra.__init__(self, eor_bin, ps_config, primary_beam)
 
     def get_ps_norm(self, data_cube):
         '''Normalization factor for spatial PS'''
-        return self.X ** 2 / self.omega_cache.get(data_cube.meta)
+        return self.X ** 2 / self.get_omega(data_cube.meta)
 
     def get_ps_err_norm(self, data_cube, with_pb=False):
         mask = datacube.WindowFunction.from_meta(data_cube.meta)
         if with_pb:
             mask = mask * self.primary_beam
         return 1 / (mask.get_area(data_cube.meta, normalize=True) ** 0.5)
 
@@ -880,15 +879,15 @@
             primary_beam (PrimaryBeam): The primary beam of the instrument
         """
 
         BasePowerSpectra.__init__(self, eor_bin, ps_config, primary_beam)
 
     def get_ps_norm(self, alm_cube):
         # Normalization factor for 1D (spacial/frequency) PS
-        return self.X ** 2 / self.omega_cache.get(alm_cube.meta)
+        return self.X ** 2 / self.get_omega(alm_cube.meta)
 
     def get_omega(self, cube_meta):
         '''Primary Beam normalization factor'''
         mask = self.primary_beam * sphcube.SphWindowFunction.from_meta(cube_meta)
         omega = mask.get_power(cube_meta)
 
         return omega
```

### Comparing `ps_eor-0.8/ps_eor/pssph.py` & `ps_eor-0.9/ps_eor/pssph.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/psutil.py` & `ps_eor-0.9/ps_eor/psutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 except ImportError:  # will be 3.x series
     pass
 
 import re
 import os
 import sys
 import time
+import functools
 import itertools
 import configparser
 
 from scipy import stats
 from scipy.sparse import diags
+from scipy.signal import get_window
 
 import numpy as np
 
 
 NUM_POOL = int(os.environ.get('OMP_NUM_THREADS', 2))
 
 try:
@@ -1046,24 +1048,39 @@
         beam = tophat_beam(thetas, fwhm)
     else:
         return None
 
     return beam
 
 
+@functools.lru_cache(maxsize=20, typed=False)
 def get_beam_cart(res, img_shape, beam_type, fwhm, n_sidelobe=None):
     nx, ny = img_shape
 
     thxval = res * np.arange(-nx / 2., nx / 2.)
     thyval = res * np.arange(-ny / 2., ny / 2.)
     thx, thy = np.meshgrid(thxval, thyval)
 
     return get_beam(np.sqrt(thx ** 2 + thy ** 2), beam_type, fwhm, n_sidelobe)
 
 
+@functools.lru_cache(maxsize=20, typed=False)
+def generate_2d_window(window_name, nx, circular=False):
+    w = get_window(window_name, nx)
+    if circular:
+        m = (nx - 1) // 2
+        x = np.linspace(-m, m, nx)
+        xx, yy = np.meshgrid(x, x)
+        w2d = np.interp(np.sqrt(xx ** 2 + yy ** 2), x, w)
+    else:
+        w2d = np.outer(w, w)
+
+    return w2d
+  
+
 def robust_std_idl(inputData, Zero=False, axis=None, dtype=None):
     """
     Robust estimator of the standard deviation of a data set.
     Based on the robust_sigma function from the AstroIDL User's Library.
 
     Args:
         inputData (TYPE): Description
```

### Comparing `ps_eor-0.8/ps_eor/simu.py` & `ps_eor-0.9/ps_eor/simu.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/sphcube.py` & `ps_eor-0.9/ps_eor/sphcube.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/sphutil.py` & `ps_eor-0.9/ps_eor/sphutil.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/tests/test_datacube.py` & `ps_eor-0.9/ps_eor/tests/test_datacube.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/tools/instru/lofar_statpos.data` & `ps_eor-0.9/ps_eor/tools/instru/lofar_statpos.data`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/tools/instru/nenufar52_statpos.data` & `ps_eor-0.9/ps_eor/tools/instru/nenufar52_statpos.data`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/tools/instru/skalow_enu_statpos.data` & `ps_eor-0.9/ps_eor/tools/instru/skalow_enu_statpos.data`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/ps_eor/tools/pstool.py` & `ps_eor-0.9/ps_eor/tools/pstool.py`

 * *Files identical despite different names*

### Comparing `ps_eor-0.8/setup.py` & `ps_eor-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 {':python_version < "3.8"': ['importlib-metadata>=1.0,<2.0']}
 
 entry_points = \
 {'console_scripts': ['pstool = ps_eor.tools.pstool:main']}
 
 setup_kwargs = {
     'name': 'ps-eor',
-    'version': '0.8',
+    'version': '0.9',
     'description': 'Foreground modeling/removal and Power Spectra generation',
     'long_description': 'Python package for foreground removal and power spectra calculation:\n===================================================================\n\nInstallation\n------------\n\nFrom git (development version):\n\n    git clone https://gitlab.com/flomertens/ps_eor.git\n    pip install -f ./ps_eor\n\nfrom [pypi](https://pypi.org/project/ps-eor/) (latest stable version):\n\n    pip install ps_eor\n\nThe following packages will also be installed:\n\n- click\n- numpy\n- scipy\n- astropy\n- matplotlib\n- pytable (for saving loading in h5 format)\n- pyfftw (optional, can save time)\n- sklearn (for PCA)\n- GPy (for GPR)\n- healpy,reproject (optional)\n\n\nCommand-line usage:\n-------------------\n\nThe ps_eor package comes with a command line tool: pstool, which can:\n- Generate gridded visibility cube from fits images cubes (gen_vus_cube)\n- Produce power-spectra from gridded visibility cube (make_ps)\n- Combine different visibility cube (combine)\n- Remove foregrounds using GPR (run_gpr)\n- ... and several more\n\nUsage of pstool is as follow:\n\n    Usage: pstool [OPTIONS] COMMAND [ARGS]...\n\n    Options:\n      --version  Show the version and exit.\n      --help     Show this message and exit.\n\n    Commands:\n      combine               Combine all datacubes listed in FILE_LIST...\n      combine_sph           Combine all sph datacubes listed in FILE_LIST...\n      diff_cube             Compute the difference between CUBE1 and CUBE2\n      even_odd_to_sum_diff  Create SUM / DIFF datacubes from EVEN / ODD...\n      gen_vis_cube          Create a datacube from image and psf fits files.\n      make_ps               Produce power-spectra of datacubes FILE_I: Input...\n      run_flagger           Run flagger on datacubes and save flag.\n      run_gpr               Run GPR & generate power spectra FILE_I: Input...\n      simu_noise_img        Compute noise fits cube from a simulated UV\n                            coverage...\n\n      simu_noise_ps         Compute noise PS from a simulated UV coverage...\n      simu_uv               Compute gridded UV coverage.\n      vis_to_sph            Load visibilities datacubes VIS_CUBE, transform to...\n\n\nTo get help for any of the pstool command, execute:\n\n    pstool CMD --help\n\n\nAPI usage:\n----------\n\nThis package provide a simple interface for Foreground removal and PS estimation tasks which can complete the command line tool.\n\nBelow we briefly document the main tasks that can be perform with this package:\n\n\n1. Loading your data: \n---------------------\n\n    data_cube_i = datacube.CartDataCube.load_from_fits_image(files, umin, umax, theta_fov)\n\nThis will do the following steps:\n- Read Fits image file\n- Trim image to theta_fov\n- Convert image from Jy/PSF to K, using imager_scale_factor or WSCNORMF\n attribute to get PSF "solid angle" (otherwise use Gaussian approx of the PSF)\n- FFT image per frequencies to get visibilities\n- Keep only non-zero visibilities between umin and umax.\nand return a CartDataCube object storing the visibilities in an ungridded way.\n\nIt is possible (recommended) to save/load to an h5 format with the save()/load() method.\n\nOne can also regrid the data and make an image with the regrid() and image() method.\n\n\n2. Run FG removal algorithm:\n----------------------------\n\nThe main FG removal code is GPR, but PCA, GMCA (the python version) and Polynamial fitting are also implemented.\n\nTo run GPR, one do the following:\n\n    data_cube_i = datacube.CartDataCube.load_from_fits_image(files_i, umin, umax, theta_fov)\n    data_cube_v = datacube.CartDataCube.load_from_fits_image(files_v, umin, umax, theta_fov)\n\n    eor_bin_list = pspec.EorBinList(data_cube_i.freqs)\n    # Create an EoR bin 122-134 MHz with a 120-136MHz range for the FG fitting\n    eor_bin_list.add_freq(1, 122, 134, 120, 136)\n    eor = eor_bin_list.get(1)\n\n    gpr_config = fitutil.GprConfig.load(gpr_config_filename)\n    gpr_fit = fgfit.GprForegroundFit(gpr_config)\n    gpr_res = gpr_fit.run(eor.get_slice_fg(data_cube_i), eor.get_slice_fg(data_cube_v))\n\nThis return a GprForegroundResult object which have the following attributes:\n- fit: The FG model in a form of a CartDataCube object\n- sub: The residual \n- pre_fit: The pre-fit FG model\n- post_fit: The post-fit FG model\n\nAnd the following method:\n- get_fg_model(): return the GPR fg model\n- get_eor_model(): return the GPR eor model\n\nOn can then save/load those CartDataCube as needed for later processing.\n\nThe CartDataCube cubes of the GPR model and residual contains the error covariance \nfrom the GPR model that need to be taken into account when generating the \npower spectra.\n\nLook at gpr_config.parset and gpr_config_v.parset for examples of GPR configuration.\n\n\n3. Generate Power Spectra:\n--------------------------\n\nThe PS code into account automatically the error covariance of the GPR model.\n\nIt is possible to generate spatial only PS, Cylindrically averaged PS (2D) or spherically averaged PS (3D).\n\n    # Create a PS configuration\n    el = 2 * np.pi * (np.arange(data_cube.ru.min(), data_cube.ru.max(), du))\n    ps_conf = pspec.PowerSpectraConfig(el)\n\n    pb = datacube.LofarHBAPrimaryBeam()\n    \n    # Create a PS generation object\n    ps_gen = pspec.PowerSpectraCart(eor, ps_conf, pb)\n\n    # Create a Spatial PS, plot it and save it to a file\n    ps = ps_gen.get_ps(data_cube)\n    ps.plot(title=\'Spatial power spectra\')\n    plt.savefig(\'ps.pdf\')\n    ps.save_to_txt(\'ps.txt\')\n\n    # Create a Cylindrically averaged PS\n    ps2d = ps_gen.get_ps2d(data_cube)\n    ps2d.plot(title=\'Cylindrically averaged power spectra\')\n    plt.savefig(\'ps2d.pdf\')\n    ps2d.save_to_txt(\'ps2d.txt\')\n\n    # Create a Spherically averaged PS\n    kbins = np.logspace(np.log10(ps_gen.kmin), np.log10(0.5), 10)\n    ps3d = ps_gen.get_ps3d(kbins, data_cube)\n    ps3d.plot(title=\'Spherically averaged power spectra\')\n    plt.savefig(\'ps3d.pdf\')\n    ps3d.save_to_txt(\'ps3d.txt\')\n\n',
     'author': 'Florent Mertens',
     'author_email': 'flomertens@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/flomertens/ps_eor',
```

### Comparing `ps_eor-0.8/PKG-INFO` & `ps_eor-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ps-eor
-Version: 0.8
+Version: 0.9
 Summary: Foreground modeling/removal and Power Spectra generation
 Home-page: https://gitlab.com/flomertens/ps_eor
 License: GPL-3.0+
 Author: Florent Mertens
 Author-email: flomertens@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

