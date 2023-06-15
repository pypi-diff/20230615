# Comparing `tmp/steam-pysigma-2023.6.7.tar.gz` & `tmp/steam-pysigma-2023.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-pysigma-2023.6.7.tar", last modified: Wed Jun 14 14:29:22 2023, max compression
+gzip compressed data, was "dist\steam-pysigma-2023.6.8.tar", last modified: Thu Jun 15 08:30:24 2023, max compression
```

## Comparing `steam-pysigma-2023.6.7.tar` & `steam-pysigma-2023.6.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.528104 steam-pysigma-2023.6.7/
--rw-rw-rw-   0        0        0     1030 2023-06-14 14:29:22.527103 steam-pysigma-2023.6.7/PKG-INFO
--rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 14:29:22.528104 steam-pysigma-2023.6.7/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-06-14 14:28:54.000000 steam-pysigma-2023.6.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.486103 steam-pysigma-2023.6.7/steam_pysigma/
--rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.7/steam_pysigma/MainSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.7/steam_pysigma/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.500103 steam-pysigma-2023.6.7/steam_pysigma/comsol/
--rw-rw-rw-   0        0        0    17446 2023-06-14 06:46:01.000000 steam-pysigma-2023.6.7/steam_pysigma/comsol/BuildComsolModel.py
--rw-rw-rw-   0        0        0    15172 2023-06-14 14:28:30.000000 steam-pysigma-2023.6.7/steam_pysigma/comsol/BuildGlobalVariables.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/comsol/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.506105 steam-pysigma-2023.6.7/steam_pysigma/data/
--rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.7/steam_pysigma/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.7/steam_pysigma/data/DataSIGMA.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.509103 steam-pysigma-2023.6.7/steam_pysigma/domain_generator/
--rw-rw-rw-   0        0        0    17309 2023-06-14 13:36:18.000000 steam-pysigma-2023.6.7/steam_pysigma/domain_generator/GeometryMultipole.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/domain_generator/__init__.py
--rw-rw-rw-   0        0        0    12500 2023-04-21 07:21:40.000000 steam-pysigma-2023.6.7/steam_pysigma/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.512104 steam-pysigma-2023.6.7/steam_pysigma/parsers/
--rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.7/steam_pysigma/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.517104 steam-pysigma-2023.6.7/steam_pysigma/plotters/
--rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.7/steam_pysigma/plotters/PlotterPysigma.py
--rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.7/steam_pysigma/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.520103 steam-pysigma-2023.6.7/steam_pysigma/postprocessing/
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.7/steam_pysigma/postprocessing/postprocessing.py
--rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.7/steam_pysigma/pysigma.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.525103 steam-pysigma-2023.6.7/steam_pysigma/utils/
--rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.7/steam_pysigma/utils/Util.py
--rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.7/steam_pysigma/utils/__init__.py
--rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.7/steam_pysigma/utils/make_folder_if_not_existing.py
-drwxrwxrwx   0        0        0        0 2023-06-14 14:29:22.496102 steam-pysigma-2023.6.7/steam_pysigma.egg-info/
--rw-rw-rw-   0        0        0     1030 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1005 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-14 14:29:18.000000 steam-pysigma-2023.6.7/steam_pysigma.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.912745 steam-pysigma-2023.6.8/
+-rw-rw-rw-   0        0        0     1030 2023-06-15 08:30:24.905743 steam-pysigma-2023.6.8/PKG-INFO
+-rw-rw-rw-   0        0        0      616 2023-02-22 13:16:40.000000 steam-pysigma-2023.6.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-15 08:30:24.912745 steam-pysigma-2023.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      897 2023-06-15 08:29:50.000000 steam-pysigma-2023.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.809744 steam-pysigma-2023.6.8/steam_pysigma/
+-rw-rw-rw-   0        0        0     2861 2023-05-23 07:10:27.000000 steam-pysigma-2023.6.8/steam_pysigma/MainSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-02-02 13:16:25.000000 steam-pysigma-2023.6.8/steam_pysigma/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.849743 steam-pysigma-2023.6.8/steam_pysigma/comsol/
+-rw-rw-rw-   0        0        0    17523 2023-06-15 08:24:04.000000 steam-pysigma-2023.6.8/steam_pysigma/comsol/BuildComsolModel.py
+-rw-rw-rw-   0        0        0    15418 2023-06-15 07:02:59.000000 steam-pysigma-2023.6.8/steam_pysigma/comsol/BuildGlobalVariables.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/comsol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.862743 steam-pysigma-2023.6.8/steam_pysigma/data/
+-rw-rw-rw-   0        0        0     8068 2023-05-25 12:15:47.000000 steam-pysigma-2023.6.8/steam_pysigma/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     7220 2023-06-01 09:48:39.000000 steam-pysigma-2023.6.8/steam_pysigma/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.867745 steam-pysigma-2023.6.8/steam_pysigma/domain_generator/
+-rw-rw-rw-   0        0        0    17309 2023-06-14 13:36:18.000000 steam-pysigma-2023.6.8/steam_pysigma/domain_generator/GeometryMultipole.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/domain_generator/__init__.py
+-rw-rw-rw-   0        0        0    12590 2023-06-15 08:15:06.000000 steam-pysigma-2023.6.8/steam_pysigma/helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.870742 steam-pysigma-2023.6.8/steam_pysigma/parsers/
+-rw-rw-rw-   0        0        0     1975 2023-05-25 12:04:31.000000 steam-pysigma-2023.6.8/steam_pysigma/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.876743 steam-pysigma-2023.6.8/steam_pysigma/plotters/
+-rw-rw-rw-   0        0        0    17437 2023-05-08 12:35:29.000000 steam-pysigma-2023.6.8/steam_pysigma/plotters/PlotterPysigma.py
+-rw-rw-rw-   0        0        0     8879 2023-05-22 07:52:03.000000 steam-pysigma-2023.6.8/steam_pysigma/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.879743 steam-pysigma-2023.6.8/steam_pysigma/postprocessing/
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     3077 2023-05-08 12:18:35.000000 steam-pysigma-2023.6.8/steam_pysigma/postprocessing/postprocessing.py
+-rw-rw-rw-   0        0        0    10147 2023-04-27 07:07:05.000000 steam-pysigma-2023.6.8/steam_pysigma/pysigma.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.901743 steam-pysigma-2023.6.8/steam_pysigma/utils/
+-rw-rw-rw-   0        0        0     1945 2023-05-08 12:45:36.000000 steam-pysigma-2023.6.8/steam_pysigma/utils/Util.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 13:08:12.000000 steam-pysigma-2023.6.8/steam_pysigma/utils/__init__.py
+-rw-rw-rw-   0        0        0      299 2022-11-02 10:29:42.000000 steam-pysigma-2023.6.8/steam_pysigma/utils/make_folder_if_not_existing.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:30:24.831743 steam-pysigma-2023.6.8/steam_pysigma.egg-info/
+-rw-rw-rw-   0        0        0     1030 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1005 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-15 08:30:19.000000 steam-pysigma-2023.6.8/steam_pysigma.egg-info/top_level.txt
```

### Comparing `steam-pysigma-2023.6.7/PKG-INFO` & `steam-pysigma-2023.6.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.7
+Version: 2023.6.8
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,STEAM,SIGMA
+Keywords: CERN,SIGMA,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.7/README.md` & `steam-pysigma-2023.6.8/README.md`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/setup.py` & `steam-pysigma-2023.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-pysigma',
-    version="2023.6.7",
+    version="2023.6.8",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="This is python wrapper of STEAM SIGMA code",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_pysigma",
     keywords={'STEAM', 'SIGMA', 'CERN'},
```

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/MainSIGMA.py` & `steam-pysigma-2023.6.8/steam_pysigma/MainSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/comsol/BuildComsolModel.py` & `steam-pysigma-2023.6.8/steam_pysigma/comsol/BuildComsolModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,25 +250,29 @@
         Function writes a .bat file which has to be run to create a COMSOL model.
         :return: None
         """
         print("Excecuting bat file")
         script_lines = []
         class_paths = ''
         for file in self.split_java_file_path:
-            script_lines += [f'"{self.COMSOL_compile_path}" -jdkroot "{self.java_jdk_path}" "{file}.java"',
-                             f'"{self.java_jdk_path}\\bin\\jar.exe" cf "{file}.jar" "{file}.class"']
+            script_lines += [
+                f'"{self.COMSOL_compile_path}" -jdkroot "{self.java_jdk_path}" -XX:+DisableExplicitGC "{file}.java"',
+                f'"{self.java_jdk_path}\\bin\\jar.exe" cf "{file}.jar" "{file}.class"'
+            ]
             class_paths += f'-classpathadd "{file}.jar" '
 
         script_lines += [
-            f'"{self.COMSOL_compile_path}" -jdkroot "{self.java_jdk_path}" {class_paths}"{self.model_java_file_path}"',
+            f'"{self.COMSOL_compile_path}" -jdkroot "{self.java_jdk_path}" {class_paths}"{self.model_java_file_path}" -XX:+DisableExplicitGC',
             f'"{self.COMSOL_batch_path}" -inputfile "{self.model_class_file_path}" '
-            f'-outputfile "{os.path.join(self.output_path, self.model_data.general_parameters.magnet_name)}.mph"']
+            f'-outputfile "{os.path.join(self.output_path, self.model_data.general_parameters.magnet_name)}.mph"'
+        ]
 
         with open(self.compile_batch_file_path, "w") as outfile:
             outfile.write("\n".join(str(line) for line in script_lines))
+
         print(f'BuilderSIGMA successfully saved: {self.compile_batch_file_path}')
         os.chdir(self.output_path)
 
     def plot_magnet(self):
         """
         Plot blocks and halfturns for the roxie model data
         :return: None
```

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/comsol/BuildGlobalVariables.py` & `steam-pysigma-2023.6.8/steam_pysigma/comsol/BuildGlobalVariables.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,16 +242,21 @@
         w_list = self.model_data.quench_protection.quench_heaters.w
         qh_to_bath_list = self.model_data.quench_protection.quench_heaters.s_ins_He
         qh_steel_strip = self.model_data.quench_protection.quench_heaters.h
         tau = [round(a * b, 4) for a, b in
                zip(self.model_data.quench_protection.quench_heaters.R_warm, self.model_data.quench_protection.quench_heaters.C)]
         num_qh_div = self.model_data.options_sigma.quench_initialization.num_qh_div
         u_init = self.model_data.quench_protection.quench_heaters.U0
-        i_init = [round(a / b, 3) for a, b in zip(self.model_data.quench_protection.quench_heaters.U0,
+
+        # In case R_warm = 0
+        try: i_init = [round(a / b, 3) for a, b in zip(self.model_data.quench_protection.quench_heaters.U0,
+                                                  self.model_data.quench_protection.quench_heaters.R_warm)]
+        except: i_init = [0 for a, b in zip(self.model_data.quench_protection.quench_heaters.U0,
                                                   self.model_data.quench_protection.quench_heaters.R_warm)]
+
         frac_heater = self.model_data.quench_protection.quench_heaters.f_cover
         trigger_time = self.model_data.quench_protection.quench_heaters.t_trigger
         ins_thick_to_coil = self.model_data.options_sigma.quench_heaters.th_coils
         lengths_qh = self.model_data.quench_protection.quench_heaters.l
 
         for i in range(self.model_data.quench_protection.quench_heaters.N_strips):
             if self.model_data.options_sigma.time_vector_solution.time_step[-1][-1] < trigger_time[i]:
```

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/data/DataRoxieParser.py` & `steam-pysigma-2023.6.8/steam_pysigma/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/data/DataSIGMA.py` & `steam-pysigma-2023.6.8/steam_pysigma/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/domain_generator/GeometryMultipole.py` & `steam-pysigma-2023.6.8/steam_pysigma/domain_generator/GeometryMultipole.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/helpers.py` & `steam-pysigma-2023.6.8/steam_pysigma/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,26 +59,27 @@
         content.insert(public_indexes[0] + 3 + ll, '\t}\n')
         java_file.writelines(content)
     print("Creating java files DONE.")
     print("Excecuting bat file")
     script_lines = []
     class_paths = ''
     for file in split_java_file_path:
-        script_lines += [f'"{COMSOL_compile_path}" -jdkroot "{java_jdk_path}" "{file}.java"',
+        script_lines += [f'"{COMSOL_compile_path}" -jdkroot "{java_jdk_path}" -XX:+DisableExplicitGC "{file}.java"',
                          f'"{java_jdk_path}\\bin\\jar.exe" cf "{file}.jar" "{file}.class"']
         class_paths += f'-classpathadd "{file}.jar" '
 
     script_lines += [
-        f'"{COMSOL_compile_path}" -jdkroot "{java_jdk_path}" {class_paths}"{model_java_file_path}"',
+        f'"{COMSOL_compile_path}" -jdkroot "{java_jdk_path}" {class_paths}"{model_java_file_path}" -XX:+DisableExplicitGC',
         f'"{COMSOL_batch_path}" -inputfile "{model_class_file_path}" '
         f'-outputfile "{os.path.join(output_path, magnet_name)}.mph" ']
 
     with open(compile_batch_file_path, "w") as outfile:
         outfile.write("\n".join(str(line) for line in script_lines))
 
+    # Excecute process without DriverSIGMA
     proc = subprocess.Popen([compile_batch_file_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE,
                             universal_newlines=True)
     (stdout, stderr) = proc.communicate()
 
     if proc.returncode != 0:
         print(stderr)
     else:
```

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/parsers/ParserRoxie.py` & `steam-pysigma-2023.6.8/steam_pysigma/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/plotters/PlotterPysigma.py` & `steam-pysigma-2023.6.8/steam_pysigma/plotters/PlotterPysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/plotters/PlotterRoxie.py` & `steam-pysigma-2023.6.8/steam_pysigma/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/postprocessing/postprocessing.py` & `steam-pysigma-2023.6.8/steam_pysigma/postprocessing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/pysigma.py` & `steam-pysigma-2023.6.8/steam_pysigma/pysigma.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma/utils/Util.py` & `steam-pysigma-2023.6.8/steam_pysigma/utils/Util.py`

 * *Files identical despite different names*

### Comparing `steam-pysigma-2023.6.7/steam_pysigma.egg-info/PKG-INFO` & `steam-pysigma-2023.6.8/steam_pysigma.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-pysigma
-Version: 2023.6.7
+Version: 2023.6.8
 Summary: This is python wrapper of STEAM SIGMA code
 Home-page: https://gitlab.cern.ch/steam/steam_pysigma
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: CERN,STEAM,SIGMA
+Keywords: CERN,SIGMA,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM PySIGMA
```

### Comparing `steam-pysigma-2023.6.7/steam_pysigma.egg-info/SOURCES.txt` & `steam-pysigma-2023.6.8/steam_pysigma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

