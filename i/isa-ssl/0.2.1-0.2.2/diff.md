# Comparing `tmp/isa-ssl-0.2.1.tar.gz` & `tmp/isa-ssl-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isa-ssl-0.2.1.tar", last modified: Thu May 11 21:26:52 2023, max compression
+gzip compressed data, was "isa-ssl-0.2.2.tar", last modified: Thu Jun 15 11:17:06 2023, max compression
```

## Comparing `isa-ssl-0.2.1.tar` & `isa-ssl-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-02-13 21:31:07.000000 isa-ssl-0.2.1/LICENSE
--rw-rw-r--   0 magland   (1000) magland   (1000)      522 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)     1778 2023-04-21 18:25:46.000000 isa-ssl-0.2.1/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/isa/
--rw-rw-r--   0 magland   (1000) magland   (1000)     1165 2023-04-26 12:02:24.000000 isa-ssl-0.2.1/isa/RtcsharePlugin.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      148 2023-04-21 18:04:05.000000 isa-ssl-0.2.1/isa/__init__.py
--rw-rw-r--   0 magland   (1000) magland   (1000)      690 2023-05-10 16:00:58.000000 isa-ssl-0.2.1/isa/_find_singular_file_in_dir.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1913 2023-04-21 11:50:18.000000 isa-ssl-0.2.1/isa/_project_config.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     1089 2023-04-21 16:24:09.000000 isa-ssl-0.2.1/isa/add.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     4044 2023-05-10 20:42:52.000000 isa-ssl-0.2.1/isa/auto_detect_vocalizations.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2003 2023-04-21 16:24:09.000000 isa-ssl-0.2.1/isa/cli.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     5842 2023-05-10 19:11:58.000000 isa-ssl-0.2.1/isa/create_spectrograms.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     4438 2023-04-21 16:24:09.000000 isa-ssl-0.2.1/isa/init.py
--rw-rw-r--   0 magland   (1000) magland   (1000)     2773 2023-05-10 20:40:36.000000 isa-ssl-0.2.1/isa/update.py
--rw-rw-r--   0 magland   (1000) magland   (1000)       97 2023-05-11 21:26:37.000000 isa-ssl-0.2.1/isa/version.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/isa_ssl.egg-info/
--rw-rw-r--   0 magland   (1000) magland   (1000)      522 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)      442 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/SOURCES.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        1 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/dependency_links.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       36 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/entry_points.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       41 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/requires.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)        4 2023-05-11 21:26:52.000000 isa-ssl-0.2.1/isa_ssl.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)      547 2023-05-11 21:26:52.960310 isa-ssl-0.2.1/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      352 2023-05-11 21:26:10.000000 isa-ssl-0.2.1/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-06-15 11:17:06.067356 isa-ssl-0.2.2/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-02-13 21:31:07.000000 isa-ssl-0.2.2/LICENSE
+-rw-rw-r--   0 magland   (1000) magland   (1000)      522 2023-06-15 11:17:06.067356 isa-ssl-0.2.2/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2127 2023-05-11 22:03:43.000000 isa-ssl-0.2.2/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-06-15 11:17:06.067356 isa-ssl-0.2.2/isa/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1165 2023-06-01 12:20:46.000000 isa-ssl-0.2.2/isa/RtcsharePlugin.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      148 2023-04-21 18:04:05.000000 isa-ssl-0.2.2/isa/__init__.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)      690 2023-05-10 16:00:58.000000 isa-ssl-0.2.2/isa/_find_singular_file_in_dir.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1913 2023-04-21 11:50:18.000000 isa-ssl-0.2.2/isa/_project_config.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     1089 2023-04-21 16:24:09.000000 isa-ssl-0.2.2/isa/add.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     4044 2023-05-10 20:42:52.000000 isa-ssl-0.2.2/isa/auto_detect_vocalizations.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2003 2023-04-21 16:24:09.000000 isa-ssl-0.2.2/isa/cli.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     5830 2023-06-15 11:15:56.000000 isa-ssl-0.2.2/isa/create_spectrograms.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     4438 2023-04-21 16:24:09.000000 isa-ssl-0.2.2/isa/init.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2773 2023-05-10 20:40:36.000000 isa-ssl-0.2.2/isa/update.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)       97 2023-06-15 11:16:50.000000 isa-ssl-0.2.2/isa/version.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-06-15 11:17:06.067356 isa-ssl-0.2.2/isa_ssl.egg-info/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      522 2023-06-15 11:17:06.000000 isa-ssl-0.2.2/isa_ssl.egg-info/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)      442 2023-06-15 11:17:06.000000 isa-ssl-0.2.2/isa_ssl.egg-info/SOURCES.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        1 2023-06-15 11:17:06.000000 isa-ssl-0.2.2/isa_ssl.egg-info/dependency_links.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       36 2023-06-15 11:17:06.000000 isa-ssl-0.2.2/isa_ssl.egg-info/entry_points.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       41 2023-06-15 11:17:06.000000 isa-ssl-0.2.2/isa_ssl.egg-info/requires.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)        4 2023-06-15 11:17:06.000000 isa-ssl-0.2.2/isa_ssl.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)      547 2023-06-15 11:17:06.067356 isa-ssl-0.2.2/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      352 2023-05-11 21:26:10.000000 isa-ssl-0.2.2/setup.py
```

### Comparing `isa-ssl-0.2.1/LICENSE` & `isa-ssl-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.1/PKG-INFO` & `isa-ssl-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isa-ssl
-Version: 0.2.1
+Version: 0.2.2
 Summary: Isa (Ee-suh) is a visualization and annotation tool for sound source location.
 Home-page: https://github.com/scratchrealm/isa
 Author: Jeremy Magland and Ralph Peterson
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/scratchrealm/isa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `isa-ssl-0.2.1/README.md` & `isa-ssl-0.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 
 Install isa-ssl from PyPI:
 
 ```bash
 pip install isa-ssl
 ```
 
-Install rtcshare
-
-Todo: provide instructions for rtcshare
+Install [rtcshare](https://github.com/scratchrealm/rtcshare)
 
 ## Create a project
 
 Use the following directory structure for your project
 
 ```bash
 my-project/ # replace with the name of your project
@@ -85,7 +83,18 @@
 
 ```bash
 isa init
 
 # replace SESSION_ID with the session ID
 isa update --session SESSION_ID
 ```
+
+## Viewing the project
+
+To view the project, you must have a running instance of rtcshare
+
+```bash
+cd my-project
+rtcshare start --dir . --plugins isa
+```
+
+Then open the rtcshare URL in a browser. You will see a file browser in the left panel. Navigate to the session you want to view and click on the view.yaml file. Then click "open in figurl".
```

### Comparing `isa-ssl-0.2.1/isa/RtcsharePlugin.py` & `isa-ssl-0.2.2/isa/RtcsharePlugin.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.1/isa/_find_singular_file_in_dir.py` & `isa-ssl-0.2.2/isa/_find_singular_file_in_dir.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.1/isa/_project_config.py` & `isa-ssl-0.2.2/isa/_project_config.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.1/isa/add.py` & `isa-ssl-0.2.2/isa/add.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.1/isa/auto_detect_vocalizations.py` & `isa-ssl-0.2.2/isa/auto_detect_vocalizations.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.1/isa/cli.py` & `isa-ssl-0.2.2/isa/cli.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.1/isa/create_spectrograms.py` & `isa-ssl-0.2.2/isa/create_spectrograms.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     audio_fname = _find_singular_file_in_dir(dirname, ['.h5', '.wav'])
     if audio_fname is None:
         raise Exception(f'No .h5 or .wav file found in directory: {dirname}')
     print(f'USING AUDIO: {audio_fname}')
     audio_path = f'{dirname}/{audio_fname}'
 
     print('Extracting audio signals')
-    if audio_path.endswith('.h5') is not None:
+    if audio_path.endswith('.h5'):
         with h5py.File(audio_path, 'r') as f:
             ch1 = np.array(f['ai_channels/ai0'])
             ch2 = np.array(f['ai_channels/ai1'])
             ch3 = np.array(f['ai_channels/ai2'])
             ch4 = np.array(f['ai_channels/ai3'])
             X = np.stack([ch1, ch2, ch3, ch4]).T
```

### Comparing `isa-ssl-0.2.1/isa/init.py` & `isa-ssl-0.2.2/isa/init.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.1/isa/update.py` & `isa-ssl-0.2.2/isa/update.py`

 * *Files identical despite different names*

### Comparing `isa-ssl-0.2.1/isa_ssl.egg-info/PKG-INFO` & `isa-ssl-0.2.2/isa_ssl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isa-ssl
-Version: 0.2.1
+Version: 0.2.2
 Summary: Isa (Ee-suh) is a visualization and annotation tool for sound source location.
 Home-page: https://github.com/scratchrealm/isa
 Author: Jeremy Magland and Ralph Peterson
 Author-email: jmagland@flatironinstitute.org
 Project-URL: Bug Tracker, https://github.com/scratchrealm/isa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `isa-ssl-0.2.1/setup.cfg` & `isa-ssl-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = isa-ssl
-version = 0.2.1
+version = 0.2.2
 author = Jeremy Magland and Ralph Peterson
 author_email = jmagland@flatironinstitute.org
 description = Isa (Ee-suh) is a visualization and annotation tool for sound source location.
 url = https://github.com/scratchrealm/isa
 include_package_data = True
 project_urls = 
 	Bug Tracker = https://github.com/scratchrealm/isa/issues
```

