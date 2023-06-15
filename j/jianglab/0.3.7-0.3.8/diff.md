# Comparing `tmp/jianglab-0.3.7.tar.gz` & `tmp/jianglab-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.3.7.tar", last modified: Thu Jun 15 16:13:38 2023, max compression
+gzip compressed data, was "jianglab-0.3.8.tar", last modified: Thu Jun 15 16:49:35 2023, max compression
```

## Comparing `jianglab-0.3.7.tar` & `jianglab-0.3.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:13:38.646161 jianglab-0.3.7/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 16:13:38.645734 jianglab-0.3.7/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.7/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:13:38.642160 jianglab-0.3.7/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.7/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    20571 2023-06-15 16:12:53.000000 jianglab-0.3.7/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.7/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:13:38.644868 jianglab-0.3.7/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 16:13:38.000000 jianglab-0.3.7/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-15 16:13:38.000000 jianglab-0.3.7/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-15 16:13:38.000000 jianglab-0.3.7/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-15 16:13:38.000000 jianglab-0.3.7/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-15 16:13:38.000000 jianglab-0.3.7/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-15 16:13:38.646319 jianglab-0.3.7/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-15 16:12:51.000000 jianglab-0.3.7/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:49:35.511139 jianglab-0.3.8/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 16:49:35.510657 jianglab-0.3.8/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.8/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:49:35.506884 jianglab-0.3.8/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.8/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    21046 2023-06-15 16:49:19.000000 jianglab-0.3.8/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.8/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-15 16:49:35.509548 jianglab-0.3.8/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      644 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-15 16:49:35.000000 jianglab-0.3.8/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-15 16:49:35.511457 jianglab-0.3.8/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      974 2023-06-15 16:49:24.000000 jianglab-0.3.8/setup.py
```

### Comparing `jianglab-0.3.7/PKG-INFO` & `jianglab-0.3.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.7
+Version: 0.3.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.3.7/README.md` & `jianglab-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.3.7/jianglab/common_functions.py` & `jianglab-0.3.8/jianglab/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,61 +66,70 @@
     test_light_ref = frame_ref[:,0:visualize_window[1]]
     frame_ref_to_onset_plot(test_light_ref, first_onset_index=0) # find the first onset index by showing the plot indexed frames from 0
     frame_ref_to_onset_plot(test_light_ref, first_onset_index=first_onset_index, find_first_onset=False) # validate the position of the first onset index by showing the plot indexed frames from first_onset_index
     onset_index, offset_index, peaks, first_onset_index = frame_ref_to_onset_plot(frame_ref, first_onset_index=first_onset_index, find_first_onset=False, visualize_window= (0,0))
     plt.rcdefaults()
     return onset_index, offset_index, peaks, first_onset_index
 
-
+def get_acquisition_rate(filepath):
+    raw_data = McsCMOSMEA.McsData(filepath)
+    return 1/(float(raw_data.Acquisition.Sensor_Data.SensorMeta["Tick"])*1e-6) # in Hz
 
 def load_light_ref(filepath, sampling_rate=2000):
     ''' load light reference from .cmcr file
     filepath: path to the .cmcr or .cmtr file
     sampling_rate: sampling rate of the light reference
     '''
     raw_data = McsCMOSMEA.McsData(filepath)
     light_ref = raw_data.Acquisition.Analog_Data.ChannelData_1[:,::sampling_rate]
     return light_ref
 
-def get_on_times_off_times_of_steps(light_ref, height = 5e4, distance = 400):
+def get_on_times_off_times_of_steps(light_ref, height = 5e4, distance = 400, verbose = True):
     on_times, _ = find_peaks(np.diff(light_ref), height = 5e4, distance = 400)
-    print(on_times.shape)
-    print(np.diff(on_times))
+    if verbose:
+        print(on_times.shape)
+        print(np.diff(on_times))
     off_times, _ = find_peaks(-np.diff(light_ref), height = 5e4, distance = 400)
-    print(off_times - on_times)
+    if verbose:
+        print(off_times - on_times)
     return on_times, off_times
 
-def import_cmtr(filename):
+def import_cmtr(filename, light_ref_resample_rate = 200):
     all_units = {"units_data":[], "meta_data":[]}
     processed = McsCMOSMEA.McsData(filename)
     for unit in tqdm(range(processed.Spike_Sorter.Units.shape[0])):
         data = eval("np.array(processed.Spike_Sorter.Unit_" + str(unit+1)+".get_peaks_timestamps())")
         col = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".attributes['Column']")
         row = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".attributes['Row']")
         waveform = eval("processed.Spike_Sorter.Unit_" + str(unit+1) + ".get_peaks_cutouts().T.mean(axis=1)")
         all_units["units_data"].append({"unitID": unit+1, "data": data, "col": col, "row": row, \
             "waveform": waveform, "filename": filename, "globalID": -1})
-    all_units["meta_data"].append({"analog":None})
+    # check if a file exist
+    cmcr_file_path = filename[:-6]+".cmcr"
+    if os.path.exists(cmcr_file_path):
+        all_units["meta_data"].append({"acq_rate": get_acquisition_rate(cmcr_file_path)})
+        all_units["meta_data"].append({"light_ref" :load_light_ref(cmcr_file_path, light_ref_resample_rate)})
+    else:
+        all_units["meta_data"].append({"acq_rate":None})
+        all_units["meta_data"].append({"light_ref":None})
     return all_units
 
 def event_rate_in_interval(timestamps, length, interval):
     bins = np.arange(0, length, interval)
     hist, _ = np.histogram(timestamps, bins=bins)
     event_rate = hist / interval *1_000_000
     return event_rate
 
 def load_raw_data(filepath):
     ''' load raw data from .cmcr or .cmtr file
     filepath: path to the .cmcr or .cmtr file'''
     raw_data = McsCMOSMEA.McsData(filepath)
     return raw_data
 
-def get_acquisition_rate(filepath):
-    raw_data = McsCMOSMEA.McsData(filepath)
-    return 1/(float(raw_data.Acquisition.Sensor_Data.SensorMeta["Tick"])*1e-6) # in Hz
+
 
 def cmcr_to_nparray(filepath):
     data = McsCMOSMEA.McsData(filepath)
     data = np.array(data.Acquisition.Sensor_Data.SensorData_1_1)
     return data
 
 def import_cmtr_firing_rate(filename, bin_size = 100):
```

### Comparing `jianglab-0.3.7/jianglab.egg-info/PKG-INFO` & `jianglab-0.3.8/jianglab.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.7
+Version: 0.3.8
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.3.7/setup.py` & `jianglab-0.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.3.7',
+    version='0.3.8',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

