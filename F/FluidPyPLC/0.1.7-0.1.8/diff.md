# Comparing `tmp/FluidPyPLC-0.1.7.tar.gz` & `tmp/FluidPyPLC-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidPyPLC-0.1.7.tar", last modified: Wed Jun 14 20:30:21 2023, max compression
+gzip compressed data, was "FluidPyPLC-0.1.8.tar", last modified: Thu Jun 15 08:39:18 2023, max compression
```

## Comparing `FluidPyPLC-0.1.7.tar` & `FluidPyPLC-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 20:30:21.984471 FluidPyPLC-0.1.7/
-drwxrwxrwx   0        0        0        0 2023-06-14 20:30:21.954060 FluidPyPLC-0.1.7/FluidPyPLC/
--rw-rw-rw-   0        0        0     7297 2023-06-14 20:24:29.000000 FluidPyPLC-0.1.7/FluidPyPLC/GUI.py
--rw-rw-rw-   0        0        0        0 2023-06-14 20:16:54.000000 FluidPyPLC-0.1.7/FluidPyPLC/__init__.py
--rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.7/FluidPyPLC/data.py
--rw-rw-rw-   0        0        0     3734 2023-06-14 20:26:13.000000 FluidPyPLC-0.1.7/FluidPyPLC/diagrams.py
--rw-rw-rw-   0        0        0     2478 2023-06-14 20:25:40.000000 FluidPyPLC-0.1.7/FluidPyPLC/f.py
--rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.7/FluidPyPLC/get_sequence.py
--rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.7/FluidPyPLC/plc.bak.py
--rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.7/FluidPyPLC/plc.bak2.py
--rw-rw-rw-   0        0        0    14521 2023-06-14 20:24:49.000000 FluidPyPLC-0.1.7/FluidPyPLC/plc.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:30:21.983480 FluidPyPLC-0.1.7/FluidPyPLC/resources/
--rw-rw-rw-   0        0        0       59 2023-06-14 19:54:48.000000 FluidPyPLC-0.1.7/FluidPyPLC/resources/config.json
--rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.7/FluidPyPLC/set_groups.py
--rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.7/FluidPyPLC/set_switches.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:30:21.982477 FluidPyPLC-0.1.7/FluidPyPLC.egg-info/
--rw-rw-rw-   0        0        0     1413 2023-06-14 20:30:21.000000 FluidPyPLC-0.1.7/FluidPyPLC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-06-14 20:30:21.000000 FluidPyPLC-0.1.7/FluidPyPLC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 20:30:21.000000 FluidPyPLC-0.1.7/FluidPyPLC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-14 20:30:21.000000 FluidPyPLC-0.1.7/FluidPyPLC.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       33 2023-06-14 20:30:21.000000 FluidPyPLC-0.1.7/FluidPyPLC.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-14 20:30:21.000000 FluidPyPLC-0.1.7/FluidPyPLC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1413 2023-06-14 20:30:21.984471 FluidPyPLC-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4905 2023-06-14 20:04:09.000000 FluidPyPLC-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 20:30:21.985473 FluidPyPLC-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1378 2023-06-14 20:29:00.000000 FluidPyPLC-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:39:18.397968 FluidPyPLC-0.1.8/
+drwxrwxrwx   0        0        0        0 2023-06-15 08:39:18.359681 FluidPyPLC-0.1.8/FluidPyPLC/
+-rw-rw-rw-   0        0        0     7297 2023-06-14 20:24:29.000000 FluidPyPLC-0.1.8/FluidPyPLC/GUI.py
+-rw-rw-rw-   0        0        0        0 2023-06-14 20:16:54.000000 FluidPyPLC-0.1.8/FluidPyPLC/__init__.py
+-rw-rw-rw-   0        0        0     2770 2023-06-14 09:49:52.000000 FluidPyPLC-0.1.8/FluidPyPLC/data.py
+-rw-rw-rw-   0        0        0     3734 2023-06-14 20:26:13.000000 FluidPyPLC-0.1.8/FluidPyPLC/diagrams.py
+-rw-rw-rw-   0        0        0     2763 2023-06-15 08:38:30.000000 FluidPyPLC-0.1.8/FluidPyPLC/f.py
+-rw-rw-rw-   0        0        0     2342 2023-06-02 12:32:53.000000 FluidPyPLC-0.1.8/FluidPyPLC/get_sequence.py
+-rw-rw-rw-   0        0        0    13777 2023-06-02 21:04:22.000000 FluidPyPLC-0.1.8/FluidPyPLC/plc.bak.py
+-rw-rw-rw-   0        0        0     9617 2023-06-08 07:50:29.000000 FluidPyPLC-0.1.8/FluidPyPLC/plc.bak2.py
+-rw-rw-rw-   0        0        0    14521 2023-06-14 20:24:49.000000 FluidPyPLC-0.1.8/FluidPyPLC/plc.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:39:18.394972 FluidPyPLC-0.1.8/FluidPyPLC/resources/
+-rw-rw-rw-   0        0        0       59 2023-06-14 19:54:48.000000 FluidPyPLC-0.1.8/FluidPyPLC/resources/config.json
+-rw-rw-rw-   0        0        0      889 2023-06-03 13:58:59.000000 FluidPyPLC-0.1.8/FluidPyPLC/set_groups.py
+-rw-rw-rw-   0        0        0     1120 2023-06-03 13:58:52.000000 FluidPyPLC-0.1.8/FluidPyPLC/set_switches.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:39:18.394097 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/
+-rw-rw-rw-   0        0        0     1413 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       33 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 08:39:18.000000 FluidPyPLC-0.1.8/FluidPyPLC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-05-29 12:32:57.000000 FluidPyPLC-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1413 2023-06-15 08:39:18.396965 FluidPyPLC-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5225 2023-06-14 21:04:11.000000 FluidPyPLC-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 08:39:18.397968 FluidPyPLC-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1378 2023-06-15 08:39:03.000000 FluidPyPLC-0.1.8/setup.py
```

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/GUI.py` & `FluidPyPLC-0.1.8/FluidPyPLC/GUI.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/data.py` & `FluidPyPLC-0.1.8/FluidPyPLC/data.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/diagrams.py` & `FluidPyPLC-0.1.8/FluidPyPLC/diagrams.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/f.py` & `FluidPyPLC-0.1.8/FluidPyPLC/f.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,38 +13,49 @@
 import os
 import pkg_resources
 import subprocess
 import textwrap
 
 
 config_file_path = pkg_resources.resource_filename('FluidPyPLC', 'resources/config.json')
-with open(config_file_path) as f:
-    config = json.load(f)
-    path = config["folder_path"]
+try:
+    with open(config_file_path) as f:
+        config = json.load(f)
+        path = config["folder_path"]
+except Exception as e:
+    print(e)
+
 
 def create_folders(folder_path):
     plots_folder = os.path.join(folder_path, 'Plots')
     plc_folder = os.path.join(folder_path, 'plc')
 
     # Create the Plots and plc folders
     os.makedirs(plots_folder, exist_ok=True)
     os.makedirs(plc_folder, exist_ok=True)
 
     print(f"Created 'Plots' and 'plc' folders inside '{folder_path}'.")
 
+    # Set this path to the config.json file
+    with open(config_file_path) as f:
+        config = json.load(f)
+    config["folder_path"] = folder_path
+
+    with open(config_file_path, 'w') as f:
+        json.dump(config, f, indent=4)
+
 # function to start the terminal version
 def terminal():
     sequence = Sequence()
     s = sequence.s
     diagrams(s)
     Plc(s)
 
 # args management
 def main():
-    global path
     parser = argparse.ArgumentParser(
         description='FluidPyPLC',
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog=textwrap.dedent('''Example:
         f.py --gui # to use the user interface mode
         f.py -t # to use the terminal version
         f.py --plc # to display the plc ST code
```

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/get_sequence.py` & `FluidPyPLC-0.1.8/FluidPyPLC/get_sequence.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/plc.bak.py` & `FluidPyPLC-0.1.8/FluidPyPLC/plc.bak.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/plc.bak2.py` & `FluidPyPLC-0.1.8/FluidPyPLC/plc.bak2.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/plc.py` & `FluidPyPLC-0.1.8/FluidPyPLC/plc.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/set_groups.py` & `FluidPyPLC-0.1.8/FluidPyPLC/set_groups.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC/set_switches.py` & `FluidPyPLC-0.1.8/FluidPyPLC/set_switches.py`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/FluidPyPLC.egg-info/PKG-INFO` & `FluidPyPLC-0.1.8/FluidPyPLC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.7
+Version: 0.1.8
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Home-page: https://github.com/MrLostInTheInternet/FluidPyPLC
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
```

### Comparing `FluidPyPLC-0.1.7/LICENSE` & `FluidPyPLC-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FluidPyPLC-0.1.7/PKG-INFO` & `FluidPyPLC-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FluidPyPLC
-Version: 0.1.7
+Version: 0.1.8
 Summary: FluidSim Circuits Analyzer & PLC ST Code Generator
 Home-page: https://github.com/MrLostInTheInternet/FluidPyPLC
 Author: MrLostInTheInternet (Eugen Iofciu Vasile)
 Author-email: <eugen.iofciuvasile@hotmail.com>
 License: GPLv3
 Keywords: python,plc,fluidsim,structured text,plc python,codesys,circuits,pneumatics,oleodynamics,plc programming
 Classifier: Development Status :: 1 - Planning
```

### Comparing `FluidPyPLC-0.1.7/README.md` & `FluidPyPLC-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -50,22 +50,31 @@
 ```bash
 config.json :
 {
   "folder_path": "full/path/to/the/folder/that/you/want"
 }
 ```
 
-P.S. I still have to manage the files that will be saved by FluidPyPLC and where to store them. For now, you have to create a dedicated folder to make it work. <br>
-I will manage to do that ASAP.
+Now you need to create the Plot and the plc folder. You can do it manually or you can use:
+```bash
+fluidpy --folder path/to/your/folder
+```
+And FluidPyPLC will create the two folders for you.
 
+[+] For Windows Users. If you want an icon to execute the GUI faster -> create a new shortcut and assign the Target:
+```bash
+Target: fluidpy.exe --gui
+```
+Windows will automatically locate the fluidpy.exe script in your Python/scripts folder and you can launch the app from your icon now.
 
+[Use my favicon if you want]
 ## 🎈 Usage <a name="usage"></a>
 You can invoke the command from anywhere on your terminal:
 ```bash
-FluidPyPLC
+fluidpy
 ```
 
 To view all the usage's methods use the tags ```--help``` or ```-h```.
  
 ## ⚙️ CODESYS configuration <a name="codesys_configuration"></a>
 [+] To test your PLC's sequence code you can use the plc.py and one of the CONFIGURATION pdfs in the fluidsim folder.
```

### Comparing `FluidPyPLC-0.1.7/setup.py` & `FluidPyPLC-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'FluidSim Circuits Analyzer & PLC ST Code Generator'
 
 with open("FluidPyPLC/README.md", "r") as f:
     long_description = f.read()
 
 # Setting up
 setup(
```

