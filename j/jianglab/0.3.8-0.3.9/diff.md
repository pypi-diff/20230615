# Comparing `tmp/jianglab-0.3.8.tar.gz` & `tmp/jianglab-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.3.8.tar", last modified: Thu Jun 15 16:49:35 2023, max compression
+gzip compressed data, was "jianglab-0.3.9.tar", last modified: Thu Jun 15 16:54:50 2023, max compression
```

## Comparing `jianglab-0.3.8.tar` & `jianglab-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:49:35.511139 jianglab-0.3.8/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 16:49:35.510657 jianglab-0.3.8/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.8/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:49:35.506884 jianglab-0.3.8/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.8/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    21046 2023-06-15 16:49:19.000000 jianglab-0.3.8/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.8/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:49:35.509548 jianglab-0.3.8/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-15 16:49:35.511457 jianglab-0.3.8/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-15 16:49:24.000000 jianglab-0.3.8/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:54:50.477793 jianglab-0.3.9/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 16:54:50.477339 jianglab-0.3.9/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.9/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:54:50.473453 jianglab-0.3.9/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.9/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    21016 2023-06-15 16:54:29.000000 jianglab-0.3.9/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.9/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:54:50.476752 jianglab-0.3.9/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 16:54:50.000000 jianglab-0.3.9/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-15 16:54:50.000000 jianglab-0.3.9/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-15 16:54:50.000000 jianglab-0.3.9/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-15 16:54:50.000000 jianglab-0.3.9/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-15 16:54:50.000000 jianglab-0.3.9/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-15 16:54:50.478002 jianglab-0.3.9/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-15 16:54:45.000000 jianglab-0.3.9/setup.py
```

### Comparing `jianglab-0.3.8/README.md` & `jianglab-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.3.8/jianglab/common_functions.py` & `jianglab-0.3.9/jianglab/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,19 +102,19 @@
         row = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".attributes['Row']")
         waveform = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".get_peaks_cutouts().T.mean(axis=1)")
         all_units["units_data"].append({"unitID": unit+1, "data": data, "col": col, "row": row, \
             "waveform": waveform, "filename": filename, "globalID": -1})
     # check if a file exist
     cmcr_file_path = filename[:-6]+".cmcr"
     if os.path.exists(cmcr_file_path):
-        all_units["meta_data"].append({"acq_rate": get_acquisition_rate(cmcr_file_path)})
-        all_units["meta_data"].append({"light_ref" :load_light_ref(cmcr_file_path, light_ref_resample_rate)})
+        all_units["meta_data"]["acq_rate"] = get_acquisition_rate(cmcr_file_path)
+        all_units["meta_data"]["light_ref"] = load_light_ref(cmcr_file_path, light_ref_resample_rate)
     else:
-        all_units["meta_data"].append({"acq_rate":None})
-        all_units["meta_data"].append({"light_ref":None})
+        all_units["meta_data"]["acq_rate"] = None
+        all_units["meta_data"]["light_ref"] = None
     return all_units
 
 def event_rate_in_interval(timestamps, length, interval):
     bins = np.arange(0, length, interval)
     hist, _ = np.histogram(timestamps, bins=bins)
     event_rate = hist / interval *1_000_000
     return event_rate
```

### Comparing `jianglab-0.3.8/setup.py` & `jianglab-0.3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.3.8',
+    version='0.3.9',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

