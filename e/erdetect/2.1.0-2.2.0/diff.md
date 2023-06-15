# Comparing `tmp/erdetect-2.1.0.tar.gz` & `tmp/erdetect-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erdetect-2.1.0.tar", last modified: Tue May  2 18:53:36 2023, max compression
+gzip compressed data, was "erdetect-2.2.0.tar", last modified: Thu Jun 15 17:56:01 2023, max compression
```

## Comparing `erdetect-2.1.0.tar` & `erdetect-2.2.0.tar`

### file list

```diff
@@ -1,37 +1,33 @@
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:36.006484 erdetect-2.1.0/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    35823 2022-01-28 21:02:26.000000 erdetect-2.1.0/LICENSE
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4752 2023-05-02 18:53:36.006651 erdetect-2.1.0/PKG-INFO
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3745 2023-05-02 18:50:51.000000 erdetect-2.1.0/README.md
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.872543 erdetect-2.1.0/erdetect/
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      645 2023-04-11 21:39:35.000000 erdetect-2.1.0/erdetect/__init__.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1318 2022-09-14 18:21:38.000000 erdetect-2.1.0/erdetect/__main__.py
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    46285 2023-05-02 18:40:17.000000 erdetect-2.1.0/erdetect/_erdetect.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.920078 erdetect-2.1.0/erdetect/core/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.1.0/erdetect/core/__init__.py
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    43840 2022-11-11 02:45:10.000000 erdetect-2.1.0/erdetect/core/config.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    13275 2022-09-13 16:33:39.000000 erdetect-2.1.0/erdetect/core/detection.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.935451 erdetect-2.1.0/erdetect/core/metrics/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3088 2022-09-13 23:06:23.000000 erdetect-2.1.0/erdetect/core/metrics/metric_cross_proj.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3876 2023-04-22 23:02:05.000000 erdetect-2.1.0/erdetect/core/metrics/metric_waveform.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     8720 2022-09-13 16:33:39.000000 erdetect-2.1.0/erdetect/core/peak_finder.py
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    28225 2023-04-12 23:50:34.000000 erdetect-2.1.0/erdetect/main_cli.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.945484 erdetect-2.1.0/erdetect/utils/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.1.0/erdetect/utils/__init__.py
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4002 2023-04-11 17:56:08.000000 erdetect-2.1.0/erdetect/utils/misc.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       22 2023-05-02 18:09:18.000000 erdetect-2.1.0/erdetect/version.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.977898 erdetect-2.1.0/erdetect/views/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:17.000000 erdetect-2.1.0/erdetect/views/__init__.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    26184 2023-05-02 18:51:47.000000 erdetect-2.1.0/erdetect/views/gui.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     7934 2022-09-13 16:33:39.000000 erdetect-2.1.0/erdetect/views/output_images.py
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:35.886980 erdetect-2.1.0/erdetect.egg-info/
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4752 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/PKG-INFO
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      688 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/SOURCES.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        1 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/dependency_links.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       83 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/requires.txt
--rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        9 2023-05-02 18:53:35.000000 erdetect-2.1.0/erdetect.egg-info/top_level.txt
--rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1412 2023-05-02 18:52:08.000000 erdetect-2.1.0/pyproject.toml
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      192 2023-05-02 18:53:36.008703 erdetect-2.1.0/setup.cfg
-drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-05-02 18:53:36.005727 erdetect-2.1.0/tests/
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      968 2023-04-11 21:42:57.000000 erdetect-2.1.0/tests/test_fileio.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       43 2023-04-11 21:43:02.000000 erdetect-2.1.0/tests/test_gui.py
--rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      211 2023-04-11 21:42:59.000000 erdetect-2.1.0/tests/test_process.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.552957 erdetect-2.2.0/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    35823 2022-01-28 21:02:26.000000 erdetect-2.2.0/LICENSE
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4846 2023-06-15 17:56:01.553121 erdetect-2.2.0/PKG-INFO
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3844 2023-06-15 17:54:10.000000 erdetect-2.2.0/README.md
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.473294 erdetect-2.2.0/erdetect/
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      645 2023-04-11 21:39:35.000000 erdetect-2.2.0/erdetect/__init__.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1318 2022-09-14 18:21:38.000000 erdetect-2.2.0/erdetect/__main__.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    46689 2023-06-15 17:43:57.000000 erdetect-2.2.0/erdetect/_erdetect.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.521631 erdetect-2.2.0/erdetect/core/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.2.0/erdetect/core/__init__.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    44920 2023-06-14 22:16:11.000000 erdetect-2.2.0/erdetect/core/config.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    13275 2022-09-13 16:33:39.000000 erdetect-2.2.0/erdetect/core/detection.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.533029 erdetect-2.2.0/erdetect/core/metrics/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3088 2022-09-13 23:06:23.000000 erdetect-2.2.0/erdetect/core/metrics/metric_cross_proj.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     3876 2023-04-22 23:02:05.000000 erdetect-2.2.0/erdetect/core/metrics/metric_waveform.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     8720 2022-09-13 16:33:39.000000 erdetect-2.2.0/erdetect/core/peak_finder.py
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    30091 2023-06-15 17:12:32.000000 erdetect-2.2.0/erdetect/main_cli.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.536848 erdetect-2.2.0/erdetect/utils/
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:10.000000 erdetect-2.2.0/erdetect/utils/__init__.py
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4002 2023-04-11 17:56:08.000000 erdetect-2.2.0/erdetect/utils/misc.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       22 2023-06-15 17:36:43.000000 erdetect-2.2.0/erdetect/version.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.552275 erdetect-2.2.0/erdetect/views/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       45 2023-04-11 17:08:17.000000 erdetect-2.2.0/erdetect/views/__init__.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)    34975 2023-06-15 17:44:19.000000 erdetect-2.2.0/erdetect/views/gui.py
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     7934 2022-09-13 16:33:39.000000 erdetect-2.2.0/erdetect/views/output_images.py
+drwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        0 2023-06-15 17:56:01.486917 erdetect-2.2.0/erdetect.egg-info/
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     4846 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/PKG-INFO
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      627 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/SOURCES.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        1 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/dependency_links.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)       83 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/requires.txt
+-rw-r--r--   0 m218483  (1058270505) MFAD\Domain Users (1387956079)        9 2023-06-15 17:56:01.000000 erdetect-2.2.0/erdetect.egg-info/top_level.txt
+-rwxr-xr-x   0 m218483  (1058270505) MFAD\Domain Users (1387956079)     1411 2023-06-15 17:54:39.000000 erdetect-2.2.0/pyproject.toml
+-rwxrwxrwx   0 m218483  (1058270505) MFAD\Domain Users (1387956079)      192 2023-06-15 17:56:01.555985 erdetect-2.2.0/setup.cfg
```

### Comparing `erdetect-2.1.0/LICENSE` & `erdetect-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erdetect-2.1.0/PKG-INFO` & `erdetect-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdetect
-Version: 2.1.0
+Version: 2.2.0
 Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
 Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
 License: GPLv3
 Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
@@ -46,20 +46,25 @@
 
 1. First install ERdetect, in the command-line run:
 ```
 pip install erdetect
 ```
 
 2. To run:
-- a) From the commandline:
+- a) With a graphical user interface:
+```
+python -m erdetect ~/bids_data ~/output/ --gui
+```
+
+- b) From the commandline:
 ```
 python -m erdetect ~/bids_data ~/output/ [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
 ```
 
-- b) To process a subset directly in a python script:
+- c) To process a subset directly in a python script:
 ```
 import erdetect
 erdetect.process_subset('/bids_data_root/subj-01/ieeg/sub-01_run-06.edf', '/output_path/')
 ```
```

### Comparing `erdetect-2.1.0/README.md` & `erdetect-2.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,20 +22,25 @@
 
 1. First install ERdetect, in the command-line run:
 ```
 pip install erdetect
 ```
 
 2. To run:
-- a) From the commandline:
+- a) With a graphical user interface:
+```
+python -m erdetect ~/bids_data ~/output/ --gui
+```
+
+- b) From the commandline:
 ```
 python -m erdetect ~/bids_data ~/output/ [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
 ```
 
-- b) To process a subset directly in a python script:
+- c) To process a subset directly in a python script:
 ```
 import erdetect
 erdetect.process_subset('/bids_data_root/subj-01/ieeg/sub-01_run-06.edf', '/output_path/')
 ```
```

### Comparing `erdetect-2.1.0/erdetect/__init__.py` & `erdetect-2.2.0/erdetect/__init__.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.1.0/erdetect/__main__.py` & `erdetect-2.2.0/erdetect/__main__.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.1.0/erdetect/_erdetect.py` & `erdetect-2.2.0/erdetect/_erdetect.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,16 +269,21 @@
             logging.info(multi_line_list(channels_late_reref_excl_by_type, LOGGING_CAPTION_INDENT_LENGTH, 'Channels excluded by type for late re-ref:', 14, ' '))
             logging.error('Late re-referencing is enabled but (after filtering by type) no channels were found, exiting...')
             raise RuntimeError('No channels were found for late re-referencing')
 
         # generate a late re-referencing object
         if cfg('preprocess', 'late_re_referencing', 'method') == 'CAR':
             late_reref = RerefStruct.generate_car(channels_late_reref_incl_names)
+            if cfg('preprocess', 'late_re_referencing', 'CAR_by_variance') != -1:
+                late_reref.late_group_reselect_varPerc = cfg('preprocess', 'late_re_referencing', 'CAR_by_variance')
+
         elif cfg('preprocess', 'late_re_referencing', 'method') == 'CAR_headbox':
             late_reref = RerefStruct.generate_car_per_headbox(channels_late_reref_incl_names, channels_late_reref_incl_headbox)
+            if cfg('preprocess', 'late_re_referencing', 'CAR_by_variance') != -1:
+                late_reref.late_group_reselect_varPerc = cfg('preprocess', 'late_re_referencing', 'CAR_by_variance')
 
             # print CAR headbox info
             logging.info('')
             log_indented_line('Late re-referencing groups:', '')
             for ind, group in enumerate(late_reref.groups):
                 logging.info(multi_line_list(group, LOGGING_CAPTION_INDENT_LENGTH, '      CAR group ' + str(ind) + ':', 14, ' '))
```

### Comparing `erdetect-2.1.0/erdetect/core/config.py` & `erdetect-2.2.0/erdetect/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     config['preprocess']['early_re_referencing']['method']          = 'CAR'                     #
     config['preprocess']['early_re_referencing']['stim_excl_epoch'] = (-1.0, 2.0)
     config['preprocess']['early_re_referencing']['channel_types']   = ('ECOG', 'SEEG', 'DBS')   # the type of channels that will be included for early re-referencing
     config['preprocess']['line_noise_removal']                      = 'off'                     # TODO: off, json, 60, 50, 60Hz 50Hz
     config['preprocess']['late_re_referencing'] = dict()
     config['preprocess']['late_re_referencing']['enabled']          = False                     #
     config['preprocess']['late_re_referencing']['method']           = 'CAR'                     #
+    config['preprocess']['late_re_referencing']['CAR_by_variance']  = -1                        #
     config['preprocess']['late_re_referencing']['stim_excl_epoch']  = (-1.0, 2.0)
     config['preprocess']['late_re_referencing']['channel_types']    = ('ECOG', 'SEEG', 'DBS')   # the type of channels that will be included for late re-referencing
 
     config['trials'] = dict()
     config['trials']['trial_epoch']                                 = (-1.0, 2.0)               # the time-span (in seconds) relative to the stimulus onset that will be used to extract the signal for each trial
     config['trials']['out_of_bounds_handling']                      = 'first_last_only'         #
     config['trials']['baseline_epoch']                             = (-0.5, -0.02)              # the time-span (in seconds) relative to the stimulus onset that will be considered as the start and end of the baseline epoch within each trial
@@ -371,21 +372,30 @@
     if not retrieve_config_string(json_config, config, 'preprocess', 'line_noise_removal', options=('off', 'json', '50', '60', '50hz', '60hz')):
         return False
     if config['preprocess']['line_noise_removal'].lower() == '50hz':
         config['preprocess']['line_noise_removal'] = '50'
     if config['preprocess']['line_noise_removal'].lower() == '60hz':
         config['preprocess']['line_noise_removal'] = '60'
     # TODO: load line noise removal, try also to accept a number instead of a string
+    #        should include a check on range
 
     if not retrieve_config_bool(json_config, config, 'preprocess', 'late_re_referencing', 'enabled'):
         return False
     if not retrieve_config_string(json_config, config, 'preprocess', 'late_re_referencing', 'method', options=('CAR', 'CAR_headbox')):
         return False
-    # TODO: load early re-referencing channels
-    # TODO: load late re-referencing channels
+
+    if config['preprocess']['late_re_referencing']['method'] in ('CAR', 'CAR_headbox'):
+        retrieve_config_number(json_config, config, 'preprocess', 'late_re_referencing', 'CAR_by_variance')
+        if not config['preprocess']['late_re_referencing']['CAR_by_variance'] == -1:
+            if config['preprocess']['late_re_referencing']['CAR_by_variance'] < 0 or config['preprocess']['late_re_referencing']['CAR_by_variance'] > 1:
+                logging.error('Invalid value in the configuration file for preprocess->late_re_referencing->CAR_by_variance, should be a (quantile) value between 0 and 1 (default is 0.2)')
+                return False
+
+    # TODO: load early re-referencing channel types
+    # TODO: load late re-referencing channel types
 
 
     # trials settings
     if not retrieve_config_range(json_config, config, 'trials', 'trial_epoch'):
         return False
     if not retrieve_config_string(json_config, config, 'trials', 'out_of_bounds_handling', options=('error', 'first_last_only', 'allow')):
         return False
@@ -516,48 +526,52 @@
                  '            "method":                       "' + _config['preprocess']['early_re_referencing']['method'] + '",\n' \
                  '            "stim_excl_epoch":              [' + numbers_to_padded_string(_config['preprocess']['early_re_referencing']['stim_excl_epoch'], 16) + '],\n' \
                  '            "channel_types":                ' + json.dumps(_config['preprocess']['early_re_referencing']['channel_types']) + '\n' \
                  '        },\n' \
                  '        "line_noise_removal":               "' + _config['preprocess']['line_noise_removal'] + '",\n' \
                  '        "late_re_referencing": {\n' \
                  '            "enabled":                      ' + ('true' if _config['preprocess']['late_re_referencing']['enabled'] else 'false') + ',\n' \
-                 '            "method":                       "' + _config['preprocess']['late_re_referencing']['method'] + '",\n' \
-                 '            "stim_excl_epoch":              [' + numbers_to_padded_string(_config['preprocess']['late_re_referencing']['stim_excl_epoch'], 16) + '],\n' \
-                 '            "channel_types":                ' + json.dumps(_config['preprocess']['late_re_referencing']['channel_types']) + '\n' \
-                 '        }\n' \
-                 '    },\n\n' \
-                 '    "trials": {\n' \
-                 '        "trial_epoch":                      [' + numbers_to_padded_string(_config['trials']['trial_epoch'], 16) + '],\n' \
-                 '        "out_of_bounds_handling":           "' + _config['trials']['out_of_bounds_handling'] + '",\n' \
-                 '        "baseline_epoch":                   [' + numbers_to_padded_string(_config['trials']['baseline_epoch'], 16) + '],\n' \
-                 '        "baseline_norm":                    "' + _config['trials']['baseline_norm'] + '",\n' \
-                 '        "concat_bidirectional_pairs":       ' + ('true' if _config['trials']['concat_bidirectional_pairs'] else 'false') + ',\n' \
-                 '        "minimum_stimpair_trials":          ' + str(_config['trials']['minimum_stimpair_trials']) + '\n' \
-                 '    },\n\n' \
-                 '    "channels": {\n' \
-                 '        "measured_types":                   ' + json.dumps(_config['channels']['measured_types']) + ',\n' \
-                 '        "stim_types":                       ' + json.dumps(_config['channels']['stim_types']) + '\n' \
-                 '    },\n\n' \
-                 '    "metrics": {\n' \
-                 '        "cross_proj": {\n' \
-                 '            "enabled":                      ' + ('true' if _config['metrics']['cross_proj']['enabled'] else 'false') + ',\n' \
-                 '            "epoch":                        [' + numbers_to_padded_string(_config['metrics']['cross_proj']['epoch'], 16) + ']\n' \
-                 '        },\n' \
-                 '        "waveform": {\n' \
-                 '            "enabled":                      ' + ('true' if _config['metrics']['waveform']['enabled'] else 'false') + ',\n' \
-                 '            "epoch":                        [' + numbers_to_padded_string(_config['metrics']['waveform']['epoch'], 16) + '],\n' \
-                 '            "bandpass":                     [' + numbers_to_padded_string(_config['metrics']['waveform']['bandpass'], 16) + ']\n' \
-                 '        }\n' \
-                 '    },\n\n' \
-                 '    "detection": {\n' \
-                 '        "negative":                         ' + ('true' if _config['detection']['negative'] else 'false') + ',\n' \
-                 '        "positive":                         ' + ('true' if _config['detection']['positive'] else 'false') + ',\n' \
-                 '        "peak_search_epoch":                [' + numbers_to_padded_string(_config['detection']['peak_search_epoch'], 16) + '],\n' \
-                 '        "response_search_epoch":            [' + numbers_to_padded_string(_config['detection']['response_search_epoch'], 16) + '],\n' \
-                 '        "method":                           "' + _config['detection']['method'] + '",\n'
+                 '            "method":                       "' + _config['preprocess']['late_re_referencing']['method'] + '",\n'
+
+    if _config['preprocess']['late_re_referencing']['CAR_by_variance'] != -1:
+        config_str += '            "CAR_by_variance":              ' + str(_config['preprocess']['late_re_referencing']['CAR_by_variance']) + ',\n'
+
+    config_str += '            "stim_excl_epoch":              [' + numbers_to_padded_string(_config['preprocess']['late_re_referencing']['stim_excl_epoch'], 16) + '],\n' \
+                  '            "channel_types":                ' + json.dumps(_config['preprocess']['late_re_referencing']['channel_types']) + '\n' \
+                  '        }\n' \
+                  '    },\n\n' \
+                  '    "trials": {\n' \
+                  '        "trial_epoch":                      [' + numbers_to_padded_string(_config['trials']['trial_epoch'], 16) + '],\n' \
+                  '        "out_of_bounds_handling":           "' + _config['trials']['out_of_bounds_handling'] + '",\n' \
+                  '        "baseline_epoch":                   [' + numbers_to_padded_string(_config['trials']['baseline_epoch'], 16) + '],\n' \
+                  '        "baseline_norm":                    "' + _config['trials']['baseline_norm'] + '",\n' \
+                  '        "concat_bidirectional_pairs":       ' + ('true' if _config['trials']['concat_bidirectional_pairs'] else 'false') + ',\n' \
+                  '        "minimum_stimpair_trials":          ' + str(_config['trials']['minimum_stimpair_trials']) + '\n' \
+                  '    },\n\n' \
+                  '    "channels": {\n' \
+                  '        "measured_types":                   ' + json.dumps(_config['channels']['measured_types']) + ',\n' \
+                  '        "stim_types":                       ' + json.dumps(_config['channels']['stim_types']) + '\n' \
+                  '    },\n\n' \
+                  '    "metrics": {\n' \
+                  '        "cross_proj": {\n' \
+                  '            "enabled":                      ' + ('true' if _config['metrics']['cross_proj']['enabled'] else 'false') + ',\n' \
+                  '            "epoch":                        [' + numbers_to_padded_string(_config['metrics']['cross_proj']['epoch'], 16) + ']\n' \
+                  '        },\n' \
+                  '        "waveform": {\n' \
+                  '            "enabled":                      ' + ('true' if _config['metrics']['waveform']['enabled'] else 'false') + ',\n' \
+                  '            "epoch":                        [' + numbers_to_padded_string(_config['metrics']['waveform']['epoch'], 16) + '],\n' \
+                  '            "bandpass":                     [' + numbers_to_padded_string(_config['metrics']['waveform']['bandpass'], 16) + ']\n' \
+                  '        }\n' \
+                  '    },\n\n' \
+                  '    "detection": {\n' \
+                  '        "negative":                         ' + ('true' if _config['detection']['negative'] else 'false') + ',\n' \
+                  '        "positive":                         ' + ('true' if _config['detection']['positive'] else 'false') + ',\n' \
+                  '        "peak_search_epoch":                [' + numbers_to_padded_string(_config['detection']['peak_search_epoch'], 16) + '],\n' \
+                  '        "response_search_epoch":            [' + numbers_to_padded_string(_config['detection']['response_search_epoch'], 16) + '],\n' \
+                  '        "method":                           "' + _config['detection']['method'] + '",\n'
 
     if _config['detection']['method'] == 'std_base':
         config_str += '        "std_base": {\n' \
                       '            "baseline_epoch":               [' + numbers_to_padded_string(_config['detection']['std_base']['baseline_epoch'], 16) + '],\n' \
                       '            "baseline_threshold_factor":    ' + str(_config['detection']['std_base']['baseline_threshold_factor']) + '\n' \
                       '        }\n'
     elif _config['detection']['method'] == 'cross_proj':
```

### Comparing `erdetect-2.1.0/erdetect/core/detection.py` & `erdetect-2.2.0/erdetect/core/detection.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.1.0/erdetect/core/metrics/metric_cross_proj.py` & `erdetect-2.2.0/erdetect/core/metrics/metric_cross_proj.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.1.0/erdetect/core/metrics/metric_waveform.py` & `erdetect-2.2.0/erdetect/core/metrics/metric_waveform.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.1.0/erdetect/core/peak_finder.py` & `erdetect-2.2.0/erdetect/core/peak_finder.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.1.0/erdetect/main_cli.py` & `erdetect-2.2.0/erdetect/main_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     CONFIG_DETECTION_STD_BASE_BASELINE_THRESHOLD_FACTOR, CONFIG_DETECTION_CROSS_PROJ_THRESHOLD, CONFIG_DETECTION_WAVEFORM_PROJ_THRESHOLD
 from erdetect._erdetect import process_subset
 from ieegprep import VALID_FORMAT_EXTENSIONS
 from ieegprep.bids.data_structure import list_bids_datasets
 from ieegprep.utils.console import multi_line_list
 from ieegprep.utils.misc import is_number
 from erdetect._erdetect import log_indented_line
+from erdetect.views.gui import open_gui
 
 
 def execute():
 
     #
     # define and parse the input arguments
     #
@@ -53,14 +54,17 @@
                         help='Show this help message and exit\n\n')
     parser.add_argument('bids_dir',
                         help='The directory with the input dataset formatted according to the BIDS standard.\n\n')
     parser.add_argument('output_dir',
                         help='The directory where the output files should be stored. If you are running group\n'
                              'level analysis this folder should be prepopulated with the results of the\n'
                              'participant level analysis.\n\n')
+    parser.add_argument('--gui',
+                        help='Run with the graphical user interface\n\n',
+                        action='store_true')
     parser.add_argument('--participant_label',
                         help='This argument can be used to indicate which specific participant(s) in the BIDS\n'
                              'directory should be analyzed. The given label(s) should correspond to the\n'
                              'sub-<participant_label> as described in the BIDS specification. Label matching is\n'
                              'case-insensitive and \'sub-\' prefixes in any of the labels will be ignored.\n'
                              'If this parameter is not provided then all subjects will be analyzed. Multiple\n'
                              'participant can be specified with a space separated list.\n\n',
@@ -83,22 +87,16 @@
                         help='Configures the app according to the settings in the JSON configuration file\n\n')
     parser.add_argument('--apply_bids_validator',
                         help='Apply the BIDS data-set validation\n\n',
                         action='store_true')
     parser.add_argument('--preproc_prioritize_speed',
                         help='Prioritize preprocessing for speed rather than for memory. By default, while preprocessing,\n'
                              'priority is given to use as little memory as possible, which can require channel-data to be\n'
-                             'retrieved twice, taking longer. This flag allows the preprocessing to keep all channel-data\n'
-                             'in memory, requiring much more memory at its peak, but speeding up the process.\n'
-                             'Note: In particular the speed processing when re-referencing MEF3 data will be influenced by\n'
-                             '      this setting since MEF3 has the ability to read partial data from the disk, allowing for\n'
-                             '      minimal memory usage. In contrast, EDF and BrainVision are loaded by MNE which holds the\n'
-                             '      entire dataset in memory, so retrieval is already fast. As a result, with EDF and BrainVision,\n'
-                             '      it might be counterproductive to set priority to speed since there is little gain and the\n'
-                             '      memory use would double.\n\n',
+                             'retrieved twice, taking longer. This flag allows the preprocessing to keep channel-data\n'
+                             'in memory, requiring much more memory at it''s peak, but speeding up the process.\n\n',
                         action='store_true')
     parser.add_argument('--high_pass',
                         help='Perform high-pass filtering (with a cut-off at 0.50Hz) before detection and visualization.\n'
                              'Note: If a configuration file is provided, then this command-line argument will overrule the\n'
                              '      high-pass setting in the configuration file\n\n',
                         action='store_true')
     parser.add_argument('--early_reref',
@@ -125,14 +123,18 @@
                              '      - CAR          = Common Average Re-referencing (e.g. \'--late_reref CAR\')\n'
                              '      - CAR_headbox  = Common Average Re-referencing per headbox (e.g. \'--late_reref CAR_headbox\').'
                              '                       The headbox number should be indicated for each channel in '
                              '                       the _channels.tsv file in a column with the heading \'headbox\'.\n'
                              'Note: If a configuration file is provided, then this command-line argument will overrule the\n'
                              '      late re-referencing setting in the configuration file\n\n',
                         nargs=1)
+    parser.add_argument('--late_reref_CAR_by_variance',
+                        help='Perform late re-referencing by calculating a common average for each stim-pair condition\n'
+                             '(per group) over only the channels with the lowest trial signal variance.\n\n',
+                        nargs='?', const='0.2')
     parser.add_argument('--include_positive_responses',
                         help='Detect and visualize positive evoked responses in addition to the negative responses\n\n',
                         action='store_true')
     parser.add_argument('--method',
                         help='The method that should be used to detect evoked responses. the options are:\n'
                              '      - std_base   = The standard deviation of a baseline-epoch is used as a threshold\n'
                              '                     (multiplied by a factor) to determine whether the average evoked deflection\n'
@@ -196,37 +198,52 @@
     if args.line_noise_removal:
         if str(args.line_noise_removal).lower() == 'json' or str(args.line_noise_removal).lower() == 'sidecar':
             cfg_set('json', 'preprocess', 'line_noise_removal')
         elif is_number(args.line_noise_removal):
             # TODO: valid number
             cfg_set(str(args.line_noise_removal), 'preprocess', 'line_noise_removal')
         else:
-            logging.error('Invalid line_noise_removal argument \'' + args.line_noise_removal + '\', either set to \'json\' or \'sidecar\' to retrieve the line-noise frequency from the *_ieeg.json file, or provide the line-noise frequency as a number.')
+            logging.error('Invalid \'line_noise_removal\' argument \'' + args.line_noise_removal + '\', either set to \'json\' or \'sidecar\' to retrieve the line-noise frequency from the *_ieeg.json file, or provide the line-noise frequency as a number.')
             return 1
 
     if args.early_reref:
         if str(args.early_reref[0]).lower() == 'car':
             cfg_set(True, 'preprocess', 'early_re_referencing', 'enabled')
             cfg_set('CAR', 'preprocess', 'early_re_referencing', 'method')
         elif str(args.early_reref[0]).lower() == 'car_headbox':
             cfg_set(True, 'preprocess', 'early_re_referencing', 'enabled')
             cfg_set('CAR_headbox', 'preprocess', 'early_re_referencing', 'method')
         else:
-            logging.error('Invalid early_reref argument \'' + args.early_reref[0] + '\'')
+            logging.error('Invalid \'early_reref\' argument \'' + args.early_reref[0] + '\'')
             return 1
 
     if args.late_reref:
         if str(args.late_reref[0]).lower() == 'car':
             cfg_set(True, 'preprocess', 'late_re_referencing', 'enabled')
             cfg_set('CAR', 'preprocess', 'late_re_referencing', 'method')
         elif str(args.late_reref[0]).lower() == 'car_headbox':
             cfg_set(True, 'preprocess', 'late_re_referencing', 'enabled')
             cfg_set('CAR_headbox', 'preprocess', 'late_re_referencing', 'method')
         else:
-            logging.error('Invalid late_reref argument \'' + args.late_reref[0] + '\'')
+            logging.error('Invalid \'late_reref\' argument \'' + args.late_reref[0] + '\'')
+            return 1
+
+    if args.late_reref_CAR_by_variance:
+        if not cfg('preprocess', 'late_re_referencing', 'enabled') or not cfg('preprocess', 'late_re_referencing', 'method') in ('CAR', 'CAR_headbox'):
+            logging.error('The \'late_reref_CAR_by_variance\' argument is set, but can only be used while using a late CAR re-referencing method.\n'
+                          'Make sure the \'late_reref\' argument is set to either CAR or CAR_headbox')
+            return 1
+        if is_number(args.late_reref_CAR_by_variance):
+            late_reref_CAR_by_variance = float(args.late_reref_CAR_by_variance)
+            if late_reref_CAR_by_variance < 0 or late_reref_CAR_by_variance > 1:
+                logging.error('Invalid \'late_reref_CAR_by_variance\' argument \'' + str(late_reref_CAR_by_variance) + '\', should be a value between 0 and 1 (default is 0.2).')
+                return 1
+            cfg_set(late_reref_CAR_by_variance, 'preprocess', 'late_re_referencing', 'CAR_by_variance')
+        else:
+            logging.error('Invalid \'late_reref_CAR_by_variance\' argument \'' + args.late_reref_CAR_by_variance + '\', provide a quantile as a value between 0 and 1 (default is 0.2).')
             return 1
 
     # check for methodological arguments
     if args.include_positive_responses:
         cfg_set(True, 'detection', 'positive')
         cfg_set(True, 'visualization', 'positive')
 
@@ -272,14 +289,16 @@
         log_indented_line('    Method:', str(cfg('preprocess', 'early_re_referencing', 'method')))
         log_indented_line('    Stim exclude epoch:', str(cfg('preprocess', 'early_re_referencing', 'stim_excl_epoch')[0]) + 's : ' + str(cfg('preprocess', 'early_re_referencing', 'stim_excl_epoch')[1]) + 's')
         logging.info(multi_line_list(cfg('preprocess', 'early_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 14, ' '))
     log_indented_line('Line-noise removal:', cfg('preprocess', 'line_noise_removal') + (' Hz' if is_number(cfg('preprocess', 'line_noise_removal')) else ''))
     log_indented_line('Late re-referencing:', ('Yes' if cfg('preprocess', 'late_re_referencing', 'enabled') else 'No'))
     if cfg('preprocess', 'late_re_referencing', 'enabled'):
         log_indented_line('    Method:', str(cfg('preprocess', 'late_re_referencing', 'method')))
+        if cfg('preprocess', 'late_re_referencing', 'method') in ('CAR', 'CAR_headbox'):
+            log_indented_line('    CAR by variance:', ('Off' if cfg('preprocess', 'late_re_referencing', 'CAR_by_variance') == -1 else 'Channels with lowest (' + str(cfg('preprocess', 'late_re_referencing', 'CAR_by_variance')) + ' quantile) trial variance'))
         log_indented_line('    Stim exclude epoch:', str(cfg('preprocess', 'late_re_referencing', 'stim_excl_epoch')[0]) + 's : ' + str(cfg('preprocess', 'late_re_referencing', 'stim_excl_epoch')[1]) + 's')
         logging.info(multi_line_list(cfg('preprocess', 'late_re_referencing', 'channel_types'), LOGGING_CAPTION_INDENT_LENGTH, '    Included channels types:', 14, ' '))
     logging.info('')
     log_indented_line('Trial epoch window:', str(cfg('trials', 'trial_epoch')[0]) + 's < stim onset < ' + str(cfg('trials', 'trial_epoch')[1]) + 's  (window size ' + str(abs(cfg('trials', 'trial_epoch')[1] - cfg('trials', 'trial_epoch')[0])) + 's)')
     log_indented_line('Trial out-of-bounds handling:', str(cfg('trials', 'out_of_bounds_handling')))
     log_indented_line('Trial baseline window:', str(cfg('trials', 'baseline_epoch')[0]) + 's : ' + str(cfg('trials', 'baseline_epoch')[1]) + 's')
     log_indented_line('Trial baseline normalization:', str(cfg('trials', 'baseline_norm')))
@@ -318,116 +337,123 @@
     log_indented_line('    Generate electrode images:', ('Yes' if cfg('visualization', 'generate_electrode_images') else 'No'))
     log_indented_line('    Generate stimulation-pair images:', ('Yes' if cfg('visualization', 'generate_stimpair_images') else 'No'))
     log_indented_line('    Generate matrix images:', ('Yes' if cfg('visualization', 'generate_matrix_images') else 'No'))
     logging.info('')
     logging.info('')
     logging.info('')
 
+    if args.gui:
 
-    #
-    # Find and process participants and their datasets
-    #
-
-    args.bids_dir = os.path.abspath(os.path.expanduser(os.path.expandvars(args.bids_dir)))
-    args.output_dir = os.path.abspath(os.path.expanduser(os.path.expandvars(args.output_dir)))
+        # open and run on theGUI
+        open_gui()
+        # TODO: transfer CLI arguments to GUI
 
-    logging.info('--------------------------------- Participants and data subsets ----------------------------------')
-    log_indented_line('BIDS input path:', args.bids_dir)
-    log_indented_line('Output path:', args.output_dir)
-    logging.info('')
+    else:
 
-    # print optional search arguments
-    optional_search_argument = False
-    if args.participant_label:
-        log_indented_line('Participant(s) to include:', ", ".join(args.participant_label))
-        optional_search_argument = True
-    if args.subset_search_pattern:
-        log_indented_line('Subset search pattern(s):', ", ".join(args.subset_search_pattern))
-        optional_search_argument = True
-    if args.format_extension:
-        log_indented_line('Only include subsets with data extension(s):', ", ".join(args.format_extension))
-        optional_search_argument = True
-    if optional_search_argument:
+        #
+        # Find and process participants and their datasets
+        #
+
+        args.bids_dir = os.path.abspath(os.path.expanduser(os.path.expandvars(args.bids_dir)))
+        args.output_dir = os.path.abspath(os.path.expanduser(os.path.expandvars(args.output_dir)))
+
+        logging.info('--------------------------------- Participants and data subsets ----------------------------------')
+        log_indented_line('BIDS input path:', args.bids_dir)
+        log_indented_line('Output path:', args.output_dir)
         logging.info('')
 
-    # check if the input is a valid BIDS dataset
-    if args.apply_bids_validator:
-        #process = run_cmd('bids-validator %s' % args.bids_dir)
-        #logging.info(process.stdout)
-        #if process.returncode != 0:
-        #    logging.error('BIDS input dataset did not pass BIDS validator. Datasets can be validated online '
-        #                    'using the BIDS Validator (http://incf.github.io/bids-validator/).\nRun the detection '
-        #                    'without the --apply_bids_validator argument to skip prior BIDS validation.')
-        #    return 1
-        bids_error = False
-        for dir_, d, files in os.walk(args.bids_dir):
-            for file in files:
-                rel_file = os.path.relpath(dir_, args.bids_dir)
-                if rel_file[0] == '.':
-                    rel_file = rel_file[1:]
-                rel_file = os.path.join(rel_file, file)
-                if not BIDSValidator().is_bids('/' + rel_file):
-                    logging.error('Invalid BIDS-file: ' + rel_file)
-                    bids_error = True
-        if bids_error:
-            logging.error('BIDS input dataset did not pass the BIDS validator. Datasets can be validated online '
-                          'using the BIDS Validator (http://incf.github.io/bids-validator/).\nRun the detection '
-                          'without the --apply_bids_validator argument to skip prior BIDS validation.')
-            return 1
-
-    # list the datasets
-    strict_search = True if args.apply_bids_validator else False
-    datasets = list_bids_datasets(args.bids_dir,
-                                  dataset_extensions=VALID_FORMAT_EXTENSIONS,
-                                  subjects_filter=args.participant_label,
-                                  subset_search_pattern=args.subset_search_pattern, strict_search=strict_search,
-                                  only_subjects_with_subsets=True)
+        # print optional search arguments
+        optional_search_argument = False
+        if args.participant_label:
+            log_indented_line('Participant(s) to include:', ", ".join(args.participant_label))
+            optional_search_argument = True
+        if args.subset_search_pattern:
+            log_indented_line('Subset search pattern(s):', ", ".join(args.subset_search_pattern))
+            optional_search_argument = True
+        if args.format_extension:
+            log_indented_line('Only include subsets with data extension(s):', ", ".join(args.format_extension))
+            optional_search_argument = True
+        if optional_search_argument:
+            logging.info('')
 
-    #
-    if len(datasets) == 0:
+        # check if the input is a valid BIDS dataset
+        if args.apply_bids_validator:
+            #process = run_cmd('bids-validator %s' % args.bids_dir)
+            #logging.info(process.stdout)
+            #if process.returncode != 0:
+            #    logging.error('BIDS input dataset did not pass BIDS validator. Datasets can be validated online '
+            #                    'using the BIDS Validator (http://incf.github.io/bids-validator/).\nRun the detection '
+            #                    'without the --apply_bids_validator argument to skip prior BIDS validation.')
+            #    return 1
+            bids_error = False
+            for dir_, d, files in os.walk(args.bids_dir):
+                for file in files:
+                    rel_file = os.path.relpath(dir_, args.bids_dir)
+                    if rel_file[0] == '.':
+                        rel_file = rel_file[1:]
+                    rel_file = os.path.join(rel_file, file)
+                    if not BIDSValidator().is_bids('/' + rel_file):
+                        logging.error('Invalid BIDS-file: ' + rel_file)
+                        bids_error = True
+            if bids_error:
+                logging.error('BIDS input dataset did not pass the BIDS validator. Datasets can be validated online '
+                              'using the BIDS Validator (http://incf.github.io/bids-validator/).\nRun the detection '
+                              'without the --apply_bids_validator argument to skip prior BIDS validation.')
+                return 1
+
+        # list the datasets
+        strict_search = True if args.apply_bids_validator else False
+        datasets = list_bids_datasets(args.bids_dir,
+                                      dataset_extensions=VALID_FORMAT_EXTENSIONS,
+                                      subjects_filter=args.participant_label,
+                                      subset_search_pattern=args.subset_search_pattern, strict_search=strict_search,
+                                      only_subjects_with_subsets=True)
+
+        #
+        if len(datasets) == 0:
+
+            logging.info('')
+            if optional_search_argument:
+                logging.warning('No datasets were found...\n'
+                                'Input arguments might have limited the search, make sure to check your CLI arguments')
+            else:
+                logging.warning('No datasets were found...')
 
-        logging.info('')
-        if optional_search_argument:
-            logging.warning('No datasets were found...\n'
-                            'Input arguments might have limited the search, make sure to check your CLI arguments')
         else:
-            logging.warning('No datasets were found...')
 
-    else:
+            # display subject/subset information
+            logging.info('Participant(s) and subset(s) found:')
+            for (subject, subsets) in datasets.items():
+                short_subsets = [os.path.splitext(os.path.basename(os.path.normpath(x)))[0] for x in subsets]
+                short_subsets = [x[0:-5] if x.endswith('_ieeg') else x for x in short_subsets]
+                short_subsets = [x[0:-4] if x.endswith('_eeg') else x for x in short_subsets]
+                logging.info(multi_line_list(list(short_subsets), LOGGING_CAPTION_INDENT_LENGTH, '    ' + subject + ':', 1, ' '))
+            logging.info('')
+
+            # process
+            for (subject, subsets) in datasets.items():
+                for subset in subsets:
+
+                    # empty space
+                    logging.info('')
+                    logging.info('')
+                    logging.info('')
+
+                    # process
+                    try:
+                        process_subset(subset, args.output_dir, preproc_prioritize_speed)
+                    except RuntimeError:
+                        logging.error('Error while processing dataset, exiting...')
+                        return 1
 
-        # display subject/subset information
-        logging.info('Participant(s) and subset(s) found:')
-        for (subject, subsets) in datasets.items():
-            short_subsets = [os.path.splitext(os.path.basename(os.path.normpath(x)))[0] for x in subsets]
-            short_subsets = [x[0:-5] if x.endswith('_ieeg') else x for x in short_subsets]
-            short_subsets = [x[0:-4] if x.endswith('_eeg') else x for x in short_subsets]
-            logging.info(multi_line_list(list(short_subsets), LOGGING_CAPTION_INDENT_LENGTH, '    ' + subject + ':', 1, ' '))
+        # empty space and end message
         logging.info('')
-
-        # process
-        for (subject, subsets) in datasets.items():
-            for subset in subsets:
-
-                # empty space
-                logging.info('')
-                logging.info('')
-                logging.info('')
-
-                # process
-                try:
-                    process_subset(subset, args.output_dir, preproc_prioritize_speed)
-                except RuntimeError:
-                    logging.error('Error while processing dataset, exiting...')
-                    return 1
-
-    # empty space and end message
-    logging.info('')
-    logging.info('')
-    logging.info('')
-    logging.info('--------------------------------------   Finished running   --------------------------------------')
+        logging.info('')
+        logging.info('')
+        logging.info('--------------------------------------   Finished running   --------------------------------------')
 
     # return success exit code
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(execute())
```

### Comparing `erdetect-2.1.0/erdetect/utils/misc.py` & `erdetect-2.2.0/erdetect/utils/misc.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.1.0/erdetect/views/output_images.py` & `erdetect-2.2.0/erdetect/views/output_images.py`

 * *Files identical despite different names*

### Comparing `erdetect-2.1.0/erdetect.egg-info/PKG-INFO` & `erdetect-2.2.0/erdetect.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erdetect
-Version: 2.1.0
+Version: 2.2.0
 Summary: A package for the automatic detection of evoked responses in SPES/CCEP data
 Author-email: Max van den Boom <m.a.vandenboom84@gmail.com>
 License: GPLv3
 Project-URL: homepage, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: documentation, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Project-URL: repository, https://github.com/MultimodalNeuroimagingLab/ERDetect
 Keywords: evoked response,detection,ieeg,n1,SPES,CCEP
@@ -46,20 +46,25 @@
 
 1. First install ERdetect, in the command-line run:
 ```
 pip install erdetect
 ```
 
 2. To run:
-- a) From the commandline:
+- a) With a graphical user interface:
+```
+python -m erdetect ~/bids_data ~/output/ --gui
+```
+
+- b) From the commandline:
 ```
 python -m erdetect ~/bids_data ~/output/ [--participant_label PARTICIPANT_LABEL [PARTICIPANT_LABEL ...]]
 ```
 
-- b) To process a subset directly in a python script:
+- c) To process a subset directly in a python script:
 ```
 import erdetect
 erdetect.process_subset('/bids_data_root/subj-01/ieeg/sub-01_run-06.edf', '/output_path/')
 ```
```

### Comparing `erdetect-2.1.0/erdetect.egg-info/SOURCES.txt` & `erdetect-2.2.0/erdetect.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,11 +18,8 @@
 erdetect/core/peak_finder.py
 erdetect/core/metrics/metric_cross_proj.py
 erdetect/core/metrics/metric_waveform.py
 erdetect/utils/__init__.py
 erdetect/utils/misc.py
 erdetect/views/__init__.py
 erdetect/views/gui.py
-erdetect/views/output_images.py
-tests/test_fileio.py
-tests/test_gui.py
-tests/test_process.py
+erdetect/views/output_images.py
```

### Comparing `erdetect-2.1.0/pyproject.toml` & `erdetect-2.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [project]
 name = "erdetect"
 description = "A package for the automatic detection of evoked responses in SPES/CCEP data"
 readme = "README.md"
 license = { text="GPLv3" }
 requires-python = ">=3.8"
 dependencies = [
-    "ieegprep >= 1.2.0",
+    "ieegprep >= 1.3.0",
     "numpy >= 1.22.3",
     "scipy >= 1.8.0",
     "matplotlib >= 3.5.1",
     "bids_validator >= 1.9.3",
 ]
 keywords = ["evoked response", "detection", "ieeg", "n1", "SPES", "CCEP"]
 authors = [{ name="Max van den Boom", email="m.a.vandenboom84@gmail.com" }]
@@ -37,8 +37,7 @@
 [tool.setuptools.dynamic]
 version = {attr = "erdetect.version.__version__"}
 
 [project.urls]
 homepage = "https://github.com/MultimodalNeuroimagingLab/ERDetect"
 documentation = "https://github.com/MultimodalNeuroimagingLab/ERDetect"
 repository = "https://github.com/MultimodalNeuroimagingLab/ERDetect"
-
```

