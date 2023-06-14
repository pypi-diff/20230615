# Comparing `tmp/np_services-0.1.8.tar.gz` & `tmp/np_services-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_services-0.1.8.tar", max compression
+gzip compressed data, was "np_services-0.1.9.tar", max compression
```

## Comparing `np_services-0.1.8.tar` & `np_services-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-02-11 07:56:28.374825 np_services-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       50 2023-02-02 07:22:03.439216 np_services-0.1.8/README.md
--rw-r--r--   0        0        0      145 2023-02-09 01:20:09.212810 np_services-0.1.8/src/np_services/__init__.py
--rw-r--r--   0        0        0     8230 2023-02-09 02:12:58.338405 np_services-0.1.8/src/np_services/mvr.py
--rw-r--r--   0        0        0    10514 2023-02-10 17:53:01.796555 np_services-0.1.8/src/np_services/open_ephys.py
--rw-r--r--   0        0        0     5552 2023-02-08 18:16:16.047207 np_services-0.1.8/src/np_services/protocols.py
--rw-r--r--   0        0        0    51883 2023-02-11 07:55:50.339434 np_services-0.1.8/src/np_services/proxies.py
--rw-r--r--   0        0        0     5343 2023-02-11 02:00:35.857604 np_services-0.1.8/src/np_services/utils.py
--rw-r--r--   0        0        0    10246 2023-02-09 02:12:58.451405 np_services-0.1.8/src/np_services/zro.py
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 np_services-0.1.8/setup.py
--rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 np_services-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-11 08:25:08.951052 np_services-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-02-02 07:22:03.439216 np_services-0.1.9/README.md
+-rw-r--r--   0        0        0      145 2023-02-09 01:20:09.212810 np_services-0.1.9/src/np_services/__init__.py
+-rw-r--r--   0        0        0     8230 2023-02-09 02:12:58.338405 np_services-0.1.9/src/np_services/mvr.py
+-rw-r--r--   0        0        0    10514 2023-02-10 17:53:01.796555 np_services-0.1.9/src/np_services/open_ephys.py
+-rw-r--r--   0        0        0     5552 2023-02-08 18:16:16.047207 np_services-0.1.9/src/np_services/protocols.py
+-rw-r--r--   0        0        0    52014 2023-02-11 08:22:26.264083 np_services-0.1.9/src/np_services/proxies.py
+-rw-r--r--   0        0        0     5343 2023-02-11 02:00:35.857604 np_services-0.1.9/src/np_services/utils.py
+-rw-r--r--   0        0        0    10246 2023-02-09 02:12:58.451405 np_services-0.1.9/src/np_services/zro.py
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 np_services-0.1.9/setup.py
+-rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 np_services-0.1.9/PKG-INFO
```

### Comparing `np_services-0.1.8/pyproject.toml` & `np_services-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "np-services"
-version = "0.1.8"
+version = "0.1.9"
 description = "Tools for interfacing with devices and services used in Mindscope Neuropixels experiments at the Allen Institute."
 authors = ["bjhardcastle <ben.hardcastle@alleninstitute.org>"]
 readme = "README.md"
 packages = [{include = "np_services", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `np_services-0.1.8/src/np_services/mvr.py` & `np_services-0.1.9/src/np_services/mvr.py`

 * *Files identical despite different names*

### Comparing `np_services-0.1.8/src/np_services/open_ephys.py` & `np_services-0.1.9/src/np_services/open_ephys.py`

 * *Files identical despite different names*

### Comparing `np_services-0.1.8/src/np_services/protocols.py` & `np_services-0.1.9/src/np_services/protocols.py`

 * *Files identical despite different names*

### Comparing `np_services-0.1.8/src/np_services/proxies.py` & `np_services-0.1.9/src/np_services/proxies.py`

 * *Files 0% similar despite different names*

```diff
@@ -764,44 +764,50 @@
         logger.debug(f"{cls.__name__} | Initializing")
         if not hasattr(cls, 'label') or not cls.label:
             raise AttributeError(f"{cls.__name__} | Must specify a label")
         super().initialize()
         if not cls.is_ready_to_start():
             cls.reenable_cameras()
             
-        time.sleep(.5)
+        time.sleep(1)
     @classmethod
     def reenable_cameras(cls) -> None:
-        # cls.get_proxy().release_cameras()
+        cls.get_proxy().release_cameras()
+        time.sleep(1)
         cls.get_proxy().enable_cameras()
-        time.sleep(.5)
-        # cls.get_proxy().stop_capture()
+        time.sleep(1)
+        cls.get_proxy().stop_capture()
+        time.sleep(1)
         cls.get_proxy().start_capture()
-        time.sleep(.5)
+        time.sleep(1)
         
     @classmethod
     def generate_image_paths(cls) -> tuple[pathlib.Path, pathlib.Path]:
         def path(side: str) -> pathlib.Path:
             # return np_config.unc_to_local((cls.data_root / f"{datetime.datetime.now():%Y%m%d_%H%M%S}_{cls.label}_{side}.png"))
             return cls.data_root / f"{datetime.datetime.now():%Y%m%d_%H%M%S}_{cls.label}_{side}.png"
         return path('left'), path('right')
     
     @classmethod
     def start(cls) -> None:
         logger.debug(f"{cls.__name__} | Starting")
         cls.latest_start = time.time()
         left, right = cls.generate_image_paths()
         cls.reenable_cameras()
+        time.sleep(1)
         # _ = cls.get_proxy().get_left_image()
         cls.get_proxy().save_left_image(str(left))
+        time.sleep(1)
         # logger.info(_)
         cls.reenable_cameras()
+        time.sleep(1)
         # _ = cls.get_proxy().get_right_image()
         # logger.info(_)
         cls.get_proxy().save_right_image(str(right))
+        time.sleep(1)
         for path, side in zip((left, right), ('Left', 'Right')):
             if path.exists():
                 logger.debug(f"{cls.__name__} | {side} image saved to {path}")
             else:
                 logger.debug(f"{cls.__name__} | {side} image capture request sent, but image not saved")
     
     @classmethod
```

### Comparing `np_services-0.1.8/src/np_services/utils.py` & `np_services-0.1.9/src/np_services/utils.py`

 * *Files identical despite different names*

### Comparing `np_services-0.1.8/src/np_services/zro.py` & `np_services-0.1.9/src/np_services/zro.py`

 * *Files identical despite different names*

### Comparing `np_services-0.1.8/setup.py` & `np_services-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'requests']
 
 extras_require = \
 {'dev': ['pip-tools', 'isort', 'mypy', 'black', 'pytest', 'poetry']}
 
 setup_kwargs = {
     'name': 'np-services',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Tools for interfacing with devices and services used in Mindscope Neuropixels experiments at the Allen Institute.',
     'long_description': '# service usage\n![Services](./services.drawio.svg)',
     'author': 'bjhardcastle',
     'author_email': 'ben.hardcastle@alleninstitute.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `np_services-0.1.8/PKG-INFO` & `np_services-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-services
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tools for interfacing with devices and services used in Mindscope Neuropixels experiments at the Allen Institute.
 Author: bjhardcastle
 Author-email: ben.hardcastle@alleninstitute.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

