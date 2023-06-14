# Comparing `tmp/dequeai-0.782.tar.gz` & `tmp/dequeai-0.784.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.782.tar", last modified: Fri Jun  9 20:57:39 2023, max compression
+gzip compressed data, was "dequeai-0.784.tar", last modified: Wed Jun 14 22:38:21 2023, max compression
```

## Comparing `dequeai-0.782.tar` & `dequeai-0.784.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:57:39.043174 dequeai-0.782/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 20:57:39.043174 dequeai-0.782/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:57:39.043174 dequeai-0.782/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.782/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14780 2023-06-09 20:56:38.000000 dequeai-0.782/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.782/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.782/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.782/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    30266 2023-05-12 17:14:03.000000 dequeai-0.782/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.782/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.782/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.782/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.782/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 20:57:39.043174 dequeai-0.782/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-09 20:57:38.000000 dequeai-0.782/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-09 20:57:39.000000 dequeai-0.782/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 20:57:38.000000 dequeai-0.782/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-09 20:57:38.000000 dequeai-0.782/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-09 20:57:38.000000 dequeai-0.782/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 20:57:39.043174 dequeai-0.782/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-09 20:57:25.000000 dequeai-0.782/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:38:21.405068 dequeai-0.784/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-14 22:38:21.405068 dequeai-0.784/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:38:21.405068 dequeai-0.784/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.784/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.784/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.784/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.784/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.784/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    30266 2023-05-12 17:14:03.000000 dequeai-0.784/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.784/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.784/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.784/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.784/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:38:21.405068 dequeai-0.784/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-14 22:38:20.000000 dequeai-0.784/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-14 22:38:21.000000 dequeai-0.784/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 22:38:21.000000 dequeai-0.784/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-14 22:38:21.000000 dequeai-0.784/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-14 22:38:21.000000 dequeai-0.784/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 22:38:21.405068 dequeai-0.784/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      583 2023-06-14 22:38:06.000000 dequeai-0.784/setup.py
```

### Comparing `dequeai-0.782/dequeai/datatypes.py` & `dequeai-0.784/dequeai/datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,33 +68,35 @@
                         raise ValueError("All elements in box_data list must be BoundingBox2d objects")
                 self._box_data.append(box_data)
 
         self._validate_size()
 
     def _process_image(self, d, mode):
         if isinstance(d, PILImage.Image):
-            self._images.append(d)
+            self._images.append(np.array(d))
         elif util.is_type_torch_tensor(util.get_full_typename(d)):
             torch_module = util.get_module(
                 "torch", "torch is required to render images"
             )
-            self._images.append(self._tensor_to_pil_image(torch_module=torch_module, pic=d, mode=mode))
+            self._images.append(self._tensor_to_numpy_image(torch_module=torch_module, pic=d, mode=mode))
         else:
             if hasattr(d, "numpy"):  # TF data eager tensors
                 d = d.numpy()
             if d.ndim > 2:
                 d = d.squeeze()  # get rid of trivial dimensions as a convenience
-            self._images.append(PILImage.fromarray(
-                self.to_uint8(d), mode=mode or self.guess_mode(d)
-            ))
+            self._images.append(
+                self.to_uint8(d)
+            )
+
+
 
     def _validate_size(self):
         pass
 
-    def _tensor_to_pil_image(self, torch_module, pic, mode):
+    def _tensor_to_numpy_image(self, torch_module, pic, mode):
 
         if not (isinstance(pic, torch_module.Tensor) or isinstance(pic, np.ndarray)):
             raise TypeError(f"pic should be Tensor or ndarray. Got {type(pic)}.")
 
         elif isinstance(pic, torch_module.Tensor):
             if pic.ndimension() not in {2, 3}:
                 raise ValueError(f"pic should be 2/3 dimensional. Got {pic.ndimension()} dimensions.")
@@ -165,15 +167,15 @@
                 raise ValueError(f"Only modes {permitted_3_channel_modes} are supported for 3D inputs")
             if mode is None and npimg.dtype == np.uint8:
                 mode = "RGB"
 
         if mode is None:
             raise TypeError(f"Input type {npimg.dtype} is not supported")
 
-        return PILImage.fromarray(npimg, mode=mode)
+        return npimg
 
     def guess_mode(self, data: "np.ndarray") -> str:
         """
         Guess what type of image the np.array is representing
         """
         # TODO: do we want to support dimensions being at the beginning of the array?
         if data.ndim == 2:
```

### Comparing `dequeai-0.782/dequeai/dequeai.py` & `dequeai-0.784/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.782/dequeai/dequeai_run.py` & `dequeai-0.784/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.782/dequeai/parsing_service.py` & `dequeai-0.784/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.782/dequeai/rest_connect.py` & `dequeai-0.784/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.782/dequeai/util.py` & `dequeai-0.784/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.782/setup.py` & `dequeai-0.784/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000782',
+    version='0.00000784',
     description='Python Experiment Tracking Package for Deque AI DLOps Platform',
     author="The Deque AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```

