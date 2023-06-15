# Comparing `tmp/jianglab-0.4.0.tar.gz` & `tmp/jianglab-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.4.0.tar", last modified: Thu Jun 15 17:04:44 2023, max compression
+gzip compressed data, was "jianglab-0.4.1.tar", last modified: Thu Jun 15 17:27:23 2023, max compression
```

## Comparing `jianglab-0.4.0.tar` & `jianglab-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 17:04:44.530255 jianglab-0.4.0/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 17:04:44.529939 jianglab-0.4.0/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.0/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 17:04:44.526966 jianglab-0.4.0/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.0/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    21023 2023-06-15 17:04:18.000000 jianglab-0.4.0/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.0/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 17:04:44.529433 jianglab-0.4.0/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 17:04:44.000000 jianglab-0.4.0/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-15 17:04:44.000000 jianglab-0.4.0/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-15 17:04:44.000000 jianglab-0.4.0/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-15 17:04:44.000000 jianglab-0.4.0/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-15 17:04:44.000000 jianglab-0.4.0/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-15 17:04:44.530372 jianglab-0.4.0/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-15 17:04:32.000000 jianglab-0.4.0/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 17:27:23.220547 jianglab-0.4.1/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 17:27:23.220136 jianglab-0.4.1/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.4.1/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 17:27:23.215746 jianglab-0.4.1/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.4.1/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    21129 2023-06-15 17:27:13.000000 jianglab-0.4.1/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.4.1/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 17:27:23.219332 jianglab-0.4.1/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 17:27:23.000000 jianglab-0.4.1/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-15 17:27:23.000000 jianglab-0.4.1/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-15 17:27:23.000000 jianglab-0.4.1/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-15 17:27:23.000000 jianglab-0.4.1/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-15 17:27:23.000000 jianglab-0.4.1/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-15 17:27:23.220745 jianglab-0.4.1/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-15 17:27:18.000000 jianglab-0.4.1/setup.py
```

### Comparing `jianglab-0.4.0/PKG-INFO` & `jianglab-0.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.0
+Version: 0.4.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.0/README.md` & `jianglab-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.4.0/jianglab/common_functions.py` & `jianglab-0.4.1/jianglab/common_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,28 +89,30 @@
         print(on_times.shape)
         print(np.diff(on_times))
     off_times, _ = find_peaks(-np.diff(light_ref), height = 5e4, distance = 400)
     if verbose:
         print(off_times - on_times)
     return on_times, off_times
 
-def import_cmtr(filename, light_ref_resample_rate = 200):
+def import_cmtr(filename, light_ref_resample_rate_hz = 100):
     all_units = {"units_data":{}, "meta_data":{}}
     processed = McsCMOSMEA.McsData(filename)
     for unit in tqdm(range(processed.Spike_Sorter.Units.shape[0])):
         data = eval("np.array(processed.Spike_Sorter.Unit_" + str(unit+1)+".get_peaks_timestamps())")
         col = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".attributes['Column']")
         row = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".attributes['Row']")
         waveform = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".get_peaks_cutouts().T.mean(axis=1)")
         all_units["units_data"][str(unit+1)] = {"unitID": unit+1, "data": data, "col": col, "row": row, \
             "waveform": waveform, "filename": filename, "globalID": -1}
     # check if a file exist
     cmcr_file_path = filename[:-6]+".cmcr"
     if os.path.exists(cmcr_file_path):
-        all_units["meta_data"]["acq_rate"] = get_acquisition_rate(cmcr_file_path)
+        acq_rate = get_acquisition_rate(cmcr_file_path)
+        all_units["meta_data"]["acq_rate"] = acq_rate
+        light_ref_resample_rate = int(acq_rate/light_ref_resample_rate_hz)
         all_units["meta_data"]["light_ref"] = load_light_ref(cmcr_file_path, light_ref_resample_rate)
     else:
         all_units["meta_data"]["acq_rate"] = None
         all_units["meta_data"]["light_ref"] = None
     return all_units
 
 def event_rate_in_interval(timestamps, length, interval):
```

### Comparing `jianglab-0.4.0/jianglab.egg-info/PKG-INFO` & `jianglab-0.4.1/jianglab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.4.0
+Version: 0.4.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.4.0/setup.py` & `jianglab-0.4.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.4.0',
+    version='0.4.1',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

