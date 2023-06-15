# Comparing `tmp/jupyter-utility-widgets-0.0.0a4.tar.gz` & `tmp/jupyter-utility-widgets-0.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-utility-widgets-0.0.0a4.tar", last modified: Tue Jun 13 08:52:56 2023, max compression
+gzip compressed data, was "jupyter-utility-widgets-0.0.0a5.tar", last modified: Thu Jun 15 07:36:59 2023, max compression
```

## Comparing `jupyter-utility-widgets-0.0.0a4.tar` & `jupyter-utility-widgets-0.0.0a5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.660205 jupyter-utility-widgets-0.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 08:52:56.660205 jupyter-utility-widgets-0.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.656205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/file_explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.656205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.656205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/specgram.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/specgram_examiner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.660205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/selector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/selector/index_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:52:56.656205 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 08:52:56.000000 jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-13 08:52:43.000000 jupyter-utility-widgets-0.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 08:52:56.660205 jupyter-utility-widgets-0.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:36:59.579669 jupyter-utility-widgets-0.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 07:36:59.579669 jupyter-utility-widgets-0.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:36:59.579669 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/file_explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:36:59.579669 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:36:59.579669 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/figures/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/figures/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/figures/specgram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/specgram_examiner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:36:59.579669 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/selector/index_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 07:36:59.579669 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-15 07:36:59.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-15 07:36:59.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 07:36:59.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 07:36:59.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-15 07:36:59.000000 jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-15 07:36:46.000000 jupyter-utility-widgets-0.0.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 07:36:59.579669 jupyter-utility-widgets-0.0.0a5/setup.cfg
```

### Comparing `jupyter-utility-widgets-0.0.0a4/LICENSE` & `jupyter-utility-widgets-0.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a4/PKG-INFO` & `jupyter-utility-widgets-0.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.0a4
+Version: 0.0.0a5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.0a4/README.md` & `jupyter-utility-widgets-0.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/file_explorer.py` & `jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/file_explorer.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/base.py` & `jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/figures/base.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/lines.py` & `jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/figures/lines.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/figures/specgram.py` & `jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/figures/specgram.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/filter.py` & `jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/filter.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/plot/specgram_examiner.py` & `jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/plot/specgram_examiner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from jupyter_utility_widgets.plot.figures.specgram import SpecgramPlot
 from matplotlib.widgets import SpanSelector
 from ipywidgets import HBox
 from matplotlib import pyplot as plt
-from functools import wraps
+from functools import wraps, update_wrapper
 
 class SpectrogramExaminer(HBox):
-    def __init__(self, **kwargs):
+    def __init__(self, keep_selection=False, **kwargs):
+        """Widget that displays a signal in a spectrogram with the ability to zoom
+
+        Parameters
+        ----------
+        keep_selection : bool, optional
+            If set to true keeps the previous selection after update, by default False
+        """
         self.full_spec = SpecgramPlot()
         self.zoom_spec = SpecgramPlot()
+        self.keep_selection = keep_selection
+        self.last_span = None
 
         # FIX: https://github.com/matplotlib/matplotlib/issues/10009
         self.span_ax = self.full_spec.fig.add_subplot(1,1,1)
         self.span_ax.patch.set_visible(False)
         self.span_ax.axis("off")
         
         self.selector = SpanSelector(
@@ -22,23 +31,35 @@
             props=dict(alpha=0.5, facecolor="tab:gray"),
             interactive=True,
             drag_from_anywhere=True,
         )
 
         super().__init__(children=[self.full_spec, self.zoom_spec], **kwargs)
         self.data = None
+        
+        self.set_params = update_wrapper(lambda *args, **kwargs: self._set_params, plt.specgram)
+
+    def test(self, *args):
+        print(self, *args)
 
     def on_select(self, tmin, tmax):
+        self.last_span = (tmin, tmax)
         xmin, xmax = int(tmin * self.full_spec.sample_rate), int(tmax * self.full_spec.sample_rate)
         self.zoom_spec.update(self.data[max(0,xmin):min(len(self.data),xmax)])
 
-    @wraps(plt.specgram)
-    def set_params(self, *args, **kwargs):
+    def _set_params(self, *args, **kwargs):
         self.full_spec.set_params(*args, **kwargs)
         self.zoom_spec.set_params(*args, **kwargs)
 
     def update(self, data):
         self.data = data
         self.full_spec.update(data)
-        self.span_ax.set_xlim(*self.full_spec.ax.get_xlim())
+        
         self.selector.new_axes(self.span_ax)
         self.zoom_spec.update(None)
+
+        if not self.keep_selection:
+            self.span_ax.patches[0].remove()
+        elif self.last_span != None:
+            self.on_select(*self.last_span)
+        
+        self.span_ax.set_xlim(*self.full_spec.ax.get_xlim())
```

### Comparing `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets/selector/index_selector.py` & `jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets/selector/index_selector.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/PKG-INFO` & `jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.0a4
+Version: 0.0.0a5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-utility
 
 Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
```

### Comparing `jupyter-utility-widgets-0.0.0a4/jupyter_utility_widgets.egg-info/SOURCES.txt` & `jupyter-utility-widgets-0.0.0a5/jupyter_utility_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

