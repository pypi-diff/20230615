# Comparing `tmp/pyparrm-1.0.0.tar.gz` & `tmp/pyparrm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyparrm-1.0.0.tar", last modified: Fri May 12 11:43:41 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyparrm-1.0.0.tar` & `pyparrm-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 11:43:41.952776 pyparrm-1.0.0/
--rw-rw-rw-   0        0        0     1095 2023-03-05 19:03:14.000000 pyparrm-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1272 2023-05-12 11:43:41.951762 pyparrm-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-05-12 11:43:32.000000 pyparrm-1.0.0/README.md
--rw-rw-rw-   0        0        0      991 2023-05-12 11:43:32.000000 pyparrm-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 11:43:41.952776 pyparrm-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      199 2023-05-12 11:43:32.000000 pyparrm-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:43:41.905973 pyparrm-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 11:43:41.928899 pyparrm-1.0.0/src/pyparrm/
--rw-rw-rw-   0        0        0       51 2023-05-12 11:43:32.000000 pyparrm-1.0.0/src/pyparrm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:43:41.950722 pyparrm-1.0.0/src/pyparrm/_utils/
--rw-rw-rw-   0        0        0     1892 2023-05-05 19:45:08.000000 pyparrm-1.0.0/src/pyparrm/_utils/_docs.py
--rw-rw-rw-   0        0        0    24665 2023-05-11 22:50:59.000000 pyparrm-1.0.0/src/pyparrm/_utils/_plotting.py
--rw-rw-rw-   0        0        0     1406 2023-05-09 15:21:19.000000 pyparrm-1.0.0/src/pyparrm/_utils/_power.py
--rw-rw-rw-   0        0        0    32813 2023-05-11 22:50:59.000000 pyparrm-1.0.0/src/pyparrm/parrm.py
-drwxrwxrwx   0        0        0        0 2023-05-12 11:43:41.938723 pyparrm-1.0.0/src/pyparrm.egg-info/
--rw-rw-rw-   0        0        0     1272 2023-05-12 11:43:41.000000 pyparrm-1.0.0/src/pyparrm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2023-05-12 11:43:41.000000 pyparrm-1.0.0/src/pyparrm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 11:43:41.000000 pyparrm-1.0.0/src/pyparrm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      183 2023-05-12 11:43:41.000000 pyparrm-1.0.0/src/pyparrm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-12 11:43:41.000000 pyparrm-1.0.0/src/pyparrm.egg-info/top_level.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyparrm-1.1.0/.gitattributes
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 pyparrm-1.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 pyparrm-1.1.0/changelog.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyparrm-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pyparrm-1.1.0/requirements_dev.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 pyparrm-1.1.0/requirements_rtd.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pyparrm-1.1.0/setup.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/api.rst
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/development.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/examples.rst
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/installation.rst
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/parrm.rst
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/refs.bib
+-rw-r--r--   0        0        0   199848 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/_static/param_explorer.png
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/_static/requirements.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/_static/versions.json
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pyparrm-1.1.0/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 pyparrm-1.1.0/examples/README.rst
+-rw-r--r--   0        0        0   960144 2020-02-02 00:00:00.000000 pyparrm-1.1.0/examples/ecog_lfp_data.npy
+-rw-r--r--   0        0        0   153168 2020-02-02 00:00:00.000000 pyparrm-1.1.0/examples/example_data.npy
+-rw-r--r--   0        0        0   153168 2020-02-02 00:00:00.000000 pyparrm-1.1.0/examples/example_data_artefact_free.npy
+-rw-r--r--   0        0        0   153168 2020-02-02 00:00:00.000000 pyparrm-1.1.0/examples/matlab_filtered.npy
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 pyparrm-1.1.0/examples/plot_example_dbs_data.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 pyparrm-1.1.0/examples/plot_use_param_explorer.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 pyparrm-1.1.0/examples/plot_use_parrm.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pyparrm-1.1.0/src/pyparrm/__init__.py
+-rw-r--r--   0        0        0    34264 2020-02-02 00:00:00.000000 pyparrm-1.1.0/src/pyparrm/parrm.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 pyparrm-1.1.0/src/pyparrm/_utils/_docs.py
+-rw-r--r--   0        0        0    30099 2020-02-02 00:00:00.000000 pyparrm-1.1.0/src/pyparrm/_utils/_plotting.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 pyparrm-1.1.0/src/pyparrm/_utils/_power.py
+-rw-r--r--   0        0        0    15280 2020-02-02 00:00:00.000000 pyparrm-1.1.0/tests/test_parrm.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 pyparrm-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 pyparrm-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pyparrm-1.1.0/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pyparrm-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pyparrm-1.1.0/PKG-INFO
```

### Comparing `pyparrm-1.0.0/LICENSE.txt` & `pyparrm-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyparrm-1.0.0/pyproject.toml` & `pyparrm-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyparrm"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
     { name="Thomas Samuel Binns", email="t.s.binns@outlook.com" }
 ]
 description = "A Python port of the PARRM algorithm"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -16,16 +16,16 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 dependencies = [
     "numpy",
     "scipy",
-    "matplotlib",
-    "pqdm"
+    "matplotlib >= 3.7.1",
+    "pqdm >= 0.2.0"
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "flake8",
     "black",
```

### Comparing `pyparrm-1.0.0/src/pyparrm/_utils/_docs.py` & `pyparrm-1.1.0/src/pyparrm/_utils/_docs.py`

 * *Files identical despite different names*

### Comparing `pyparrm-1.0.0/src/pyparrm/_utils/_plotting.py` & `pyparrm-1.1.0/src/pyparrm/_utils/_plotting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,194 +1,297 @@
 """Tools for plotting results."""
 
+# Author(s):
+#   Thomas Samuel Binns | github.com/tsbinns
+
 from copy import deepcopy
 from multiprocessing import cpu_count
 
 from matplotlib import pyplot as plt
-from matplotlib.widgets import RadioButtons, Slider
+from matplotlib.widgets import RadioButtons, TextBox
 import numpy as np
 
 from pyparrm._utils._power import compute_psd
 
 
 class _ExploreParams:
     """Class for interactively exploring filter parameters.
 
     Parameters
     ----------
     parrm : pyparrm.PARRM
         PARRM object containing the data for which filter parameters should be
         explored.
 
-    freq_res : int | float (default 1.0)
+    time_range : list of int or float | None (default None)
+        Range of the times to plot and filter in a list of length two,
+        containing the first and last timepoints, respectively, in seconds. If
+        ``None``, all timepoints are used.
+
+    time_res : int | float (default 0.01)
+        Time resolution, in seconds, to use when plotting the time-series data.
+
+    freq_range : list of int or float | None (default None)
+        Range of the frequencies to plot in a list of length two, containing
+        the first and last frequencies, respectively, in Hz. If ``None``, all
+        frequencies are used.
+
+    freq_res : int | float (default 5.0)
         Frequency resolution, in Hz, to use when computing the power spectra of
         the data.
 
     n_jobs : int (default 1)
         Number of jobs to run in parallel when computing power spectra. Must be
         less than the number of available CPUs and greater than 0 (unless it is
         -1, in which case all available CPUs are used).
 
     Methods
     -------
     plot
         Create and show the parameter exploration plot.
     """
 
-    parrm = None
-    freq_res = None
-    n_jobs = None
-
     figure = None
     sample_period_focused_axis = None
     sample_period_overview_axis = None
     sample_period_focus_highlight = None
     time_data_axis = None
     freq_data_axis = None
 
     slider_period_half_width = None
     slider_filter_half_width = None
     slider_omit_n_samples = None
     buttons_filter_direction = None
 
-    current_channel_idx = 0
     current_period_half_width = None
     current_filter_half_width = None
     current_omit_n_samples = None
     current_filter_direction = None
 
     sample_period_focused_scatter = None
     sample_period_overview_scatter = None
 
-    largest_sample_period_xvals = None
-    largest_sample_period_xvals_range = None
     current_sample_period_yvals = None
     current_sample_period_xvals = None
 
+    valid_filter = True
     filter_error_text = None
 
-    times = None
     filtered_data_time = None
     filtered_data_line_time = None
     unfiltered_data_line_time = None
 
-    freqs = None
     filtered_data_freq = None
     filtered_data_line_freq = None
     unfiltered_psds = None
     unfiltered_data_line_freq = None
 
     def __init__(
-        self, parrm, freq_res: int | float = 5.0, n_jobs: int = 1
+        self,
+        parrm,
+        time_range: list[int | float] | None = None,
+        time_res: int | float = 0.01,
+        freq_range: list[int | float] | None = None,
+        freq_res: int | float = 5.0,
+        n_jobs: int = 1,
     ) -> None:
-        self._check_sort_init_inputs(parrm, freq_res, n_jobs)
+        self._check_sort_init_inputs(
+            parrm, time_range, time_res, freq_range, freq_res, n_jobs
+        )
         self._initialise_parrm_data_info()
 
     def _check_sort_init_inputs(
-        self, parrm, freq_res: float, n_jobs: int
+        self,
+        parrm,
+        time_range: list[int | float] | None,
+        time_res: int | float,
+        freq_range: list[int | float] | None,
+        freq_res: int | float,
+        n_jobs: int,
     ) -> None:
         """Check and sort init. inputs."""
         assert parrm._period is not None, (
             "PyPARRM Internal Error: `_ParamSelection` should only be called "
             "if the period has been estimated. Please contact the PyPARRM "
             "developers."
         )
         self.parrm = deepcopy(parrm)
         self.parrm._verbose = False
-        self.parrm._check_sort_create_filter_inputs(None, 0, "both", None)
-        self.current_period_half_width = self.parrm._period_half_width
-        self.current_filter_half_width = self.parrm._filter_half_width
-        self.current_filter_direction = self.parrm._filter_direction
-        self.current_omit_n_samples = self.parrm._omit_n_samples
-        self.current_sample_period_xvals = np.mod(
-            np.arange(self.current_filter_half_width * 2 - 1),
-            self.parrm._period,
-        )
-        self.current_sample_period_yvals = np.diff(
-            self.parrm._data[
-                self.current_channel_idx, : self.current_filter_half_width * 2
-            ]
-        )
 
+        # time_range
+        if time_range is None:
+            time_range = [0, self.parrm._n_samples / self.parrm._sampling_freq]
+        if not isinstance(time_range, list) or not all(
+            isinstance(entry, (int, float)) for entry in time_range
+        ):
+            raise TypeError("`time_range` must be a list of ints or floats.")
+        if len(time_range) != 2:
+            raise ValueError("`time_range` must have a length of 2.")
+        if (
+            time_range[0] < 0
+            or time_range[1]
+            > self.parrm._n_samples / self.parrm._sampling_freq
+        ):
+            raise ValueError(
+                "Entries of `time_range` must lie in the range [0, "
+                "max. time]."
+            )
+        if time_range[0] >= time_range[1]:
+            raise ValueError("`time_range[1]` must be > `time_range[0]`.")
+        self.time_range = np.arange(
+            time_range[0] * self.parrm._sampling_freq,
+            time_range[1] * self.parrm._sampling_freq,
+        ).astype(int)
+        self.parrm._data = self.parrm._data[:, self.time_range]
+        self.parrm._n_samples = self.parrm._data.shape[1]
+
+        # time_res
+        if not isinstance(time_res, (int, float)):
+            raise TypeError("`time_res` must be an int or a float.")
+        if (
+            time_res <= 0
+            or time_res >= self.time_range[-1] / self.parrm._sampling_freq
+        ):
+            raise ValueError(
+                "`time_res` must lie in the range (0, max. time)."
+            )
+        self.time_res = time_res
+        self.decim = int(np.ceil(self.time_res * self.parrm._sampling_freq))
+
+        # freq_range
+        if freq_range is None:
+            freq_range = [1, self.parrm._sampling_freq / 2]
+        if not isinstance(freq_range, list) or not all(
+            isinstance(entry, (int, float)) for entry in freq_range
+        ):
+            raise TypeError("`freq_range` must be a list of ints or floats.")
+        if len(freq_range) != 2:
+            raise ValueError("`freq_range` must have a length of 2.")
+        if freq_range[0] <= 0 or freq_range[1] > self.parrm._sampling_freq / 2:
+            raise ValueError(
+                "Entries of `freq_range` must lie in the range (0, "
+                "Nyquist frequency]."
+            )
+        if freq_range[0] >= freq_range[1]:
+            raise ValueError("`freq_range[1]` must be > `freq_range[0]`.")
+        self.freq_range = deepcopy(freq_range)
+
+        # freq_res
         if not isinstance(freq_res, (int, float)):
             raise TypeError("`freq_res` must be an int or a float.")
-        if freq_res <= 0 or freq_res > self.parrm._sampling_freq // 2:
+        if freq_res <= 0 or freq_res > self.parrm._sampling_freq / 2:
             raise ValueError(
-                "`freq_res`must be > 0 and <= the Nyquist frequency."
+                "`freq_res` must lie in the range (0, Nyquist frequency]."
             )
         self.freq_res = deepcopy(freq_res)
 
+        # n_jobs
         if not isinstance(n_jobs, int):
             raise TypeError("`n_jobs` must be an int.")
         if n_jobs > cpu_count():
             raise ValueError(
                 "`n_jobs` must be <= the number of available CPUs."
             )
         if n_jobs <= 0 and n_jobs != -1:
             raise ValueError("If `n_jobs` is <= 0, it must be -1.")
         if n_jobs == -1:
             n_jobs = cpu_count()
         self.n_jobs = deepcopy(n_jobs)
 
+        self.parrm._check_sort_create_filter_inputs(None, 0, "both", None)
+        self.current_period_half_width = self.parrm._period_half_width
+        self.current_filter_half_width = self.parrm._filter_half_width
+        self.current_filter_direction = self.parrm._filter_direction
+        self.current_omit_n_samples = self.parrm._omit_n_samples
+
+        self.current_sample_period_xvals = np.mod(
+            np.arange(self.current_filter_half_width * 2 - 1),
+            self.parrm._period,
+        )
+        self.current_channel_idx = 0
+        self.current_sample_period_yvals = np.diff(
+            self.parrm._data[
+                self.current_channel_idx, : self.current_filter_half_width * 2
+            ]
+        )
+
     def _initialise_parrm_data_info(self) -> None:
         """Initialise information from PARRM data for plotting."""
         self.largest_sample_period_xvals = np.mod(
             np.arange((self.parrm._n_samples // 2) - 1),
             self.parrm._period,
         )
         self.largest_sample_period_xvals_range = (
             self.largest_sample_period_xvals.max()
             - self.largest_sample_period_xvals.min()
         )
 
         # filtered data info.
-        self.times = (
-            np.arange(self.parrm._n_samples) / self.parrm._sampling_freq
-        )
+        self.times = (self.time_range / self.parrm._sampling_freq)[
+            :: self.decim
+        ]
 
         # freq data info.
-        n_freqs = int((self.parrm._sampling_freq // 2) // self.freq_res)
-        self.freqs = np.abs(
-            np.fft.fftfreq(n_freqs * 2, 1 / self.parrm._sampling_freq)[
-                1 : n_freqs + 1
-            ]
-        )
-        self.unfiltered_psds = compute_psd(
-            self.parrm._data, self.parrm._sampling_freq, n_freqs, self.n_jobs
+        self.fft_n_points = int(self.parrm._sampling_freq // self.freq_res)
+        self.freqs, self.unfiltered_psds = compute_psd(
+            data=self.parrm._data,
+            sampling_freq=self.parrm._sampling_freq,
+            n_points=self.fft_n_points,
+            max_freq=self.freq_range[1],
+            n_jobs=self.n_jobs,
         )
 
     def plot(self) -> None:
         """Create and show the parameter exploration plot."""
         self._initialise_plot()
         self._initialise_widgets()
 
-        def update_period_half_width(half_width: float) -> None:
-            """Update period half width according to the slider."""
+        def update_period_half_width(half_width: str) -> None:
+            """Update period half width according to the textbox."""
+            half_width = float(half_width)
+            half_width = np.max((half_width, self.period_half_width_limits[0]))
+            half_width = np.min((half_width, self.period_half_width_limits[1]))
+            self.textbox_period_half_width.set_val(f"{half_width :.3f}")
             self.current_period_half_width = half_width
+
             self._update_sample_period_focused_xlim_width(half_width)
             self._update_sample_period_focused_ylim()
             self._update_sample_period_focus_highlight()
             self._update_suptitle()
             self._update_filter()
             self.figure.canvas.draw_idle()
 
-        def update_filter_half_width(half_width: int) -> None:
-            """Update filter half width according to the slider."""
+        def update_filter_half_width(half_width: str) -> None:
+            """Update filter half width according to the textbox."""
+            half_width = int(half_width)
+            half_width = int(
+                np.max((half_width, self.filter_half_width_limits[0]))
+            )
+            half_width = int(
+                np.min((half_width, self.filter_half_width_limits[1]))
+            )
+            self.textbox_filter_half_width.set_val(str(half_width))
             self.current_filter_half_width = half_width
+
             if half_width <= self.current_omit_n_samples:
                 self.slider_omit_n_samples.set_val(half_width - 1)
                 return
             self._update_suptitle()
             self._update_sample_period_vals_plots()
             self._update_filter()
             self.figure.canvas.draw_idle()
 
-        def update_omit_n_samples(n_samples: int) -> None:
-            """Update number of omitted samples according to the slider."""
+        def update_omit_n_samples(n_samples: str) -> None:
+            """Update number of omitted samples according to the textbox."""
+            n_samples = int(n_samples)
+            n_samples = int(np.max((n_samples, self.omit_n_samples_limits[0])))
+            n_samples = int(np.min((n_samples, self.omit_n_samples_limits[1])))
+            self.textbox_omit_n_samples.set_val(str(n_samples))
             self.current_omit_n_samples = n_samples
+
             if n_samples >= self.current_filter_half_width:
                 self.slider_omit_n_samples.set_val(
                     self.current_filter_half_width - 1
                 )
                 return
             self._update_suptitle()
             self._update_filter()
@@ -197,17 +300,17 @@
         def update_filter_direction(direction: str) -> None:
             """Update filter direction according to the button."""
             self.current_filter_direction = direction
             self._update_suptitle()
             self._update_filter()
             self.figure.canvas.draw_idle()
 
-        self.slider_period_half_width.on_changed(update_period_half_width)
-        self.slider_omit_n_samples.on_changed(update_omit_n_samples)
-        self.slider_filter_half_width.on_changed(update_filter_half_width)
+        self.textbox_period_half_width.on_submit(update_period_half_width)
+        self.textbox_omit_n_samples.on_submit(update_omit_n_samples)
+        self.textbox_filter_half_width.on_submit(update_filter_half_width)
         self.buttons_filter_direction.on_clicked(update_filter_direction)
 
         plt.show()
 
     def _initialise_plot(self) -> None:
         """Initialise the plot for exploring parameters."""
         plt.ion()  # needed for fine-tuning layout
@@ -279,25 +382,28 @@
         )
 
         # timeseries data plot
         self.time_data_axis = axes["upper right"]
         # timeseries data plot (unfiltered data)
         self.unfiltered_data_line_time = self.time_data_axis.plot(
             self.times,
-            self.parrm._data[self.current_channel_idx],
+            (
+                self.parrm._data[self.current_channel_idx]
+                - np.mean(self.parrm._data[self.current_channel_idx], axis=0)
+            )[:: self.decim],
             color="black",
             alpha=0.3,
             linewidth=0.5,
         )[0]
         # timeseries data plot (filtered data)
         self.parrm._generate_filter()
         self.filtered_data_time = self.parrm.filter_data()
         self.filtered_data_line_time = self.time_data_axis.plot(
             self.times,
-            self.filtered_data_time[self.current_channel_idx],
+            self.filtered_data_time[self.current_channel_idx][:: self.decim],
             color="#ff7f0e",
             linewidth=0.5,
         )[0]
         self.time_data_axis.set_xlabel("Time (s)")
         self.time_data_axis.set_ylabel("Amplitude (data units)")
 
         # frequency data plot
@@ -307,18 +413,19 @@
             self.freqs,
             self.unfiltered_psds[self.current_channel_idx],
             color="black",
             alpha=0.3,
             label="Unfiltered data",
         )[0]
         # frequency data plot (filtered)
-        self.filtered_data_freq = compute_psd(
-            self.filtered_data_time[self.current_channel_idx],
-            self.parrm._sampling_freq,
-            self.freqs.shape[0],
+        _, self.filtered_data_freq = compute_psd(
+            data=self.filtered_data_time[self.current_channel_idx],
+            sampling_freq=self.parrm._sampling_freq,
+            n_points=self.fft_n_points,
+            max_freq=self.freq_range[1],
         )
         self.filtered_data_line_freq = self.freq_data_axis.loglog(
             self.freqs,
             self.filtered_data_freq,
             color="#ff7f0e",
             label="Filtered data",
         )[0]
@@ -326,48 +433,57 @@
         self.freq_data_axis.set_ylabel("Log power (dB/Hz)")
         self.freq_data_axis.legend(
             loc="upper left", bbox_to_anchor=(0.7, 1.22)
         )
 
     def _initialise_widgets(self) -> None:
         """Initialise widgets to use on the plot."""
-        self.slider_period_half_width = Slider(
-            self.figure.add_axes((0.2, 0.12, 0.27, 0.025)),
-            "Period half-width",
-            valmin=self.largest_sample_period_xvals.min(),
-            valmax=self.largest_sample_period_xvals.max() / 2.0,
-            valinit=self.current_period_half_width,
-            valstep=(
-                self.largest_sample_period_xvals_range
-                / self.largest_sample_period_xvals.shape[0]
-                * 0.25
-            ),
-            valfmt="%0.3f",
+        self.period_half_width_limits = [
+            float(self.largest_sample_period_xvals.min()),
+            self.largest_sample_period_xvals.max() / 2.0,
+        ]
+        if self.largest_sample_period_xvals.min() == 0:
+            period_lower_lim = "0"
+        else:
+            period_lower_lim = f"{self.period_half_width_limits[0] :.3f}"
+
+        self.textbox_period_half_width = TextBox(
+            self.figure.add_axes((0.32, 0.14, 0.15, 0.03)),
+            f"Period half-width [{period_lower_lim} - "
+            f"{self.period_half_width_limits[1] :.3f}]:",
+            f"{self.current_period_half_width :.3f}",
+            textalignment="center",
         )
 
-        self.slider_filter_half_width = Slider(
-            self.figure.add_axes((0.2, 0.08, 0.27, 0.025)),
-            "Filter half-width",
-            valmin=1,
-            valmax=(self.parrm._n_samples - 1) // 2,
-            valinit=self.current_filter_half_width,
-            valstep=1,
-        )
-
-        self.slider_omit_n_samples = Slider(
-            self.figure.add_axes((0.2, 0.05, 0.27, 0.025)),
-            "Omitted samples",
-            valmin=0,
-            valmax=((self.parrm._n_samples - 1) // 2) - 1,
-            valinit=self.current_omit_n_samples,
-            valstep=1,
+        self.filter_half_width_limits = [
+            1,
+            int((self.parrm._n_samples - 1) / 2),
+        ]
+        self.textbox_filter_half_width = TextBox(
+            self.figure.add_axes((0.32, 0.09, 0.15, 0.03)),
+            f"Filter half-width [{self.filter_half_width_limits[0]} - "
+            f"{self.filter_half_width_limits[1]}]:",
+            str(self.current_filter_half_width),
+            textalignment="center",
+        )
+
+        self.omit_n_samples_limits = [
+            0,
+            int(((self.parrm._n_samples - 1) / 2) - 1),
+        ]
+        self.textbox_omit_n_samples = TextBox(
+            self.figure.add_axes((0.32, 0.06, 0.15, 0.03)),
+            f"Omitted samples [{self.omit_n_samples_limits[0]} - "
+            f"{self.omit_n_samples_limits[1]}]:",
+            str(self.current_omit_n_samples),
+            textalignment="center",
         )
 
         buttons_filter_direction_axis = self.figure.add_axes(
-            (0.03, 0.05, 0.05, 0.1)
+            (0.07, 0.06, 0.05, 0.1)
         )
         buttons_filter_direction_axis.set_title("Filter direction")
         self.buttons_filter_direction = RadioButtons(
             buttons_filter_direction_axis,
             ["both", "future", "past"],
             active=0,  # "both"
             activecolor="green",
@@ -475,17 +591,18 @@
         y_vals = self.current_sample_period_yvals[
             (self.current_sample_period_xvals >= xlim[0])
             & (self.current_sample_period_xvals < xlim[1]),
         ]
         y_vals_max = y_vals.max()
         y_vals_min = y_vals.min()
         y_range = y_vals_max - y_vals_min
-        self.sample_period_focused_axis.set_ylim(
-            (y_vals_min - y_range * 0.2, y_vals_max + y_range * 0.2)
-        )
+        if y_range != 0:  # avoids singular ylim warning
+            self.sample_period_focused_axis.set_ylim(
+                (y_vals_min - y_range * 0.2, y_vals_max + y_range * 0.2)
+            )
 
     def _update_sample_period_focus_highlight(self) -> None:
         """Update shaded area displaying current period window."""
         xlim = self.sample_period_focused_axis.get_xlim()
         self.sample_period_focus_highlight.remove()  # clear old patch
         self.sample_period_focus_highlight = (
             self.sample_period_overview_axis.axvspan(
@@ -508,32 +625,35 @@
     def _update_filter(self) -> None:
         """Create a new PARRM filter and apply it to the data."""
         self.parrm._filter_half_width = self.current_filter_half_width
         self.parrm._period_half_width = self.current_period_half_width
         self.parrm._omit_n_samples = self.current_omit_n_samples
         self.parrm._filter_direction = self.current_filter_direction
 
-        self.valid_filter = True
         try:
             self.parrm._generate_filter()
+            self.valid_filter = True
         except RuntimeError:
             self.valid_filter = False
 
         if self.valid_filter:
             self.filtered_data_time = self.parrm.filter_data()
 
         self._update_filtered_data_lines()
 
     def _update_unfiltered_data_lines(self) -> None:
         """Update plotted unfiltered data."""
         # timeseries data
         self.unfiltered_data_line_time.remove()  # clear old line
         self.unfiltered_data_line_time = self.time_data_axis.plot(
             self.times,
-            self.parrm._data[self.current_channel_idx],
+            (
+                self.parrm._data[self.current_channel_idx]
+                - np.mean(self.parrm._data[self.current_channel_idx], axis=0)
+            )[:: self.decim],
             linewidth=0.5,
             color="black",
             alpha=0.3,
             label="Unfiltered data",
         )[0]
 
         # frequency data
@@ -551,48 +671,52 @@
         try:  # clear old lines, if they exist
             self.filtered_data_line_time.remove()
             self.filtered_data_line_freq.remove()
         except ValueError:
             pass
 
         if self.valid_filter:
-            if self.filter_error_text is not None:  # clear old warning text
-                self.time_data_axis.texts[0].remove()
-                self.filter_error_text = None
+            if len(self.time_data_axis.texts) != 0:  # clear warning text
+                for text_i in range(len(self.time_data_axis.texts)):
+                    self.time_data_axis.texts[text_i].remove()
+
             # timeseries data
             self.filtered_data_line_time = self.time_data_axis.plot(
                 self.times,
-                self.filtered_data_time[self.current_channel_idx],
+                self.filtered_data_time[self.current_channel_idx][
+                    :: self.decim
+                ],
                 linewidth=0.5,
                 color="#ff7f0e",
                 label="Filtered data",
             )[0]
             self.time_data_axis.relim()
             self.time_data_axis.autoscale_view(scalex=False, scaley=True)
 
             # frequency data
-            self.filtered_data_freq = compute_psd(
-                self.filtered_data_time[self.current_channel_idx],
-                self.parrm._sampling_freq,
-                self.freqs.shape[0],
+            _, self.filtered_data_freq = compute_psd(
+                data=self.filtered_data_time[self.current_channel_idx],
+                sampling_freq=self.parrm._sampling_freq,
+                n_points=self.fft_n_points,
+                max_freq=self.freq_range[1],
             )
             self.filtered_data_line_freq = self.freq_data_axis.plot(
                 self.freqs,
                 self.filtered_data_freq,
                 color="#ff7f0e",
                 label="Filtered data",
             )[0]
             self.freq_data_axis.relim()
             self.freq_data_axis.autoscale_view(scalex=False, scaley=True)
-        else:
+        elif len(self.time_data_axis.texts) == 0:  # if no warning already
             xlim = self.time_data_axis.get_xlim()
             xlim_mid = xlim[0] + ((xlim[1] - xlim[0]) / 2)
             ylim = self.time_data_axis.get_ylim()
             ylim_mid = ylim[0] + ((ylim[1] - ylim[0]) / 2)
-            self.filter_error_text = self.time_data_axis.text(
+            self.time_data_axis.text(
                 xlim_mid,
                 ylim_mid,
                 "The filter cannot be generated with the current settings",
                 fontsize=10,
                 fontweight="bold",
                 backgroundcolor="red",
                 horizontalalignment="center",
```

### Comparing `pyparrm-1.0.0/src/pyparrm/parrm.py` & `pyparrm-1.1.0/src/pyparrm/parrm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Tools for fitting PARRM filters to data."""
 
+# Author(s):
+#   Thomas Samuel Binns | github.com/tsbinns
+
 from copy import deepcopy
 from multiprocessing import cpu_count
 
 import numpy as np
 from pqdm.threads import pqdm
 from scipy.optimize import fmin
-from scipy.signal import convolve2d
+from scipy.signal import convolve  # faster than convolve2d
 
 from pyparrm._utils._plotting import _ExploreParams
 
 
+np.seterr(all="ignore")  # ignore zero division error
+
+
 class PARRM:
     """Class for removing stimulation artefacts from data using PARRM.
 
     The Period-based Artefact Reconstruction and Removal Method (PARRM) is
     described in Dastin-van Rijn *et al.* (2021) :footcite:`DastinEtAl2021`.
     PARRM assumes that the artefacts are semi-regular, periodic, and linearly
     combined with the signal of interest.
@@ -115,14 +121,20 @@
             raise ValueError("`artefact_freq` must be > 0.")
         self._artefact_freq = deepcopy(artefact_freq)
 
         if not isinstance(verbose, bool):
             raise TypeError("`verbose` must be a bool.")
         self._verbose = deepcopy(verbose)
 
+    def __repr__(self) -> str:  # noqa D107
+        return (
+            f"PARRM object | Data: ({self._n_chans} channels x "
+            f"{self._n_samples} times) | Period: {self._period :.4f}"
+        )
+
     def find_period(
         self,
         search_samples: np.ndarray | None = None,
         assumed_periods: int | float | tuple[int | float] | None = None,
         outlier_boundary: int | float = 3.0,
         random_seed: int | None = None,
         n_jobs: int = 1,
@@ -146,17 +158,16 @@
         random_seed: int | None (default None)
             Seed to use when generating indices of samples to search for the
             period. Only used if the number of available samples is less than
             the number of requested samples.
 
         n_jobs : int (default 1)
             Number of jobs to run in parallel when optimising the period
-            estimates. Must be less than the number of available CPUs and
-            greater than 0 (unless it is -1, in which case all available CPUs
-            are used).
+            estimates. Must lie in the range [1, number of CPUs] (unless it is
+            -1, in which case all available CPUs are used).
         """  # noqa E501
         if self._verbose:
             print("\nFinding the artefact period...")
 
         self._reset_result_attrs()
 
         self._check_sort_find_stim_period_inputs(
@@ -635,30 +646,49 @@
             return np.inf, np.inf
 
         residuals = data - waves @ beta
 
         return residuals**2, beta**2
 
     def explore_filter_params(
-        self, freq_res: int | float = 5.0, n_jobs: int = 1
+        self,
+        time_range: list[int] | None = None,
+        time_res: int | float = 0.01,
+        freq_range: list[int] | None = None,
+        freq_res: int | float = 5.0,
+        n_jobs: int = 1,
     ) -> None:
         """Create an interactive plot to explore filter parameters.
 
         Can only be called after the artefact period has been estimated with
         :meth:`find_period`.
 
         Parameters
         ----------
+        time_range : list of int or float | None (default None)
+            Range of the times to plot and filter in a list of length two,
+            containing the first and last timepoints, respectively, in seconds.
+            If ``None``, all timepoints are used.
+
+        time_res : int | float (default 0.01)
+            Time resolution, in seconds, to use when plotting the time-series
+            data.
+
+        freq_range : list of int or float | None (default None)
+            Range of the frequencies to plot in a list of length two,
+            containing the first and last frequencies, respectively, in Hz. If
+            ``None``, all frequencies are used.
+
         freq_res : int | float (default 5.0)
             Frequency resolution, in Hz, to use when computing the power
-            spectra of the data. Must be > 0 and <= the Nyquist frequency.
+            spectra of the data.
 
         n_jobs : int (default 1)
             Number of jobs to run in parallel when computing the power spectra.
-            Must be < the number of available CPUs and > 0 (unless it is -1, in
+            Must lie in the range [1, number of CPUs] (unless it is -1, in
             which case all available CPUs are used).
 
         Notes
         -----
         It is recommended that you call this method from a script; behaviour in
         notebooks is not guaranteed!
         """
@@ -666,15 +696,17 @@
             print("Opening the filter parameter explorer...")
 
         if self._period is None:
             raise ValueError(
                 "The period has not yet been estimated. The `find_period` "
                 "method must be called first."
             )
-        param_explorer = _ExploreParams(self, freq_res, n_jobs)
+        param_explorer = _ExploreParams(
+            self, time_range, time_res, freq_range, freq_res, n_jobs
+        )
         param_explorer.plot()
 
     def create_filter(
         self,
         filter_half_width: int | None = None,
         omit_n_samples: int = 0,
         filter_direction: str = "both",
@@ -851,35 +883,40 @@
                 "The filter has not yet been created. The `create_filter` "
                 "method must be called first."
             )
 
         data = self._check_sort_filter_data_inputs(data)
 
         numerator = (
-            convolve2d(data.T, self._filter[:, np.newaxis], "same") - data.T
+            convolve(data.T, self._filter[:, np.newaxis], "same") - data.T
         )
-        denominator = 1 - convolve2d(
+        denominator = 1 - convolve(
             np.ones_like(data).T,
             self._filter[:, np.newaxis],
             "same",
         )
 
-        self._filtered_data = (numerator / denominator + data.T).T
+        filtered_data = (numerator / denominator + data.T).T
+        # (close-to) zero numerators may be treated as zero in division,
+        # leading to inf/NaN values which can be replaced with 0
+        filtered_data[np.isinf(filtered_data)] = 0
+        filtered_data[np.isnan(filtered_data)] = 0
+        self._filtered_data = filtered_data
 
         if self._verbose:
             print("    ... Data filtered\n")
 
         return self._filtered_data
 
     def _check_sort_filter_data_inputs(
         self, data: np.ndarray | None
     ) -> np.ndarray:
         """Check and sort `filter_data` inputs."""
         if data is None:
-            data = self.data
+            data = self._data
         if not isinstance(data, np.ndarray):
             raise TypeError("`data` must be a NumPy array.")
         if data.ndim != 2:
             raise ValueError("`data` must be a 2D array.")
 
         return data
```

