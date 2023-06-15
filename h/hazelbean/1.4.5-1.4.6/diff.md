# Comparing `tmp/hazelbean-1.4.5.tar.gz` & `tmp/hazelbean-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazelbean-1.4.5.tar", last modified: Thu Jun  8 15:02:20 2023, max compression
+gzip compressed data, was "hazelbean-1.4.6.tar", last modified: Thu Jun 15 11:52:07 2023, max compression
```

## Comparing `hazelbean-1.4.5.tar` & `hazelbean-1.4.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 15:02:20.126000 hazelbean-1.4.5/
--rw-rw-rw-   0        0        0    14763 2023-06-08 15:02:14.000000 hazelbean-1.4.5/LICENSE
--rw-rw-rw-   0        0        0      145 2023-06-08 15:02:14.000000 hazelbean-1.4.5/MANIFEST.in
--rw-rw-rw-   0        0        0      443 2023-06-08 15:02:20.063000 hazelbean-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     4863 2023-06-08 15:02:14.000000 hazelbean-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 15:02:18.028000 hazelbean-1.4.5/hazelbean/
--rw-rw-rw-   0        0        0     8196 2022-09-28 15:14:40.000000 hazelbean-1.4.5/hazelbean/__init__.py
--rw-rw-rw-   0        0        0    15645 2022-09-28 14:32:01.000000 hazelbean-1.4.5/hazelbean/arrayframe.py
--rw-rw-rw-   0        0        0     6865 2022-05-09 18:31:33.000000 hazelbean-1.4.5/hazelbean/arrayframe_functions.py
--rw-rw-rw-   0        0        0     5787 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/arrayframe_numpy_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:02:19.119000 hazelbean-1.4.5/hazelbean/calculation_core/
--rw-rw-rw-   0        0        0     2523 2022-09-27 18:48:13.000000 hazelbean-1.4.5/hazelbean/calculation_core/__init__.py
--rw-rw-rw-   0        0        0   364367 2023-01-30 15:25:17.000000 hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.c
--rw-rw-rw-   0        0        0    59392 2023-01-30 15:25:21.000000 hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0   370413 2023-06-06 15:16:35.000000 hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.cpp
--rw-rw-rw-   0        0        0     5843 2023-01-30 15:25:06.000000 hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.pyx
--rw-rw-rw-   0        0        0      746 2023-06-01 20:11:21.000000 hazelbean-1.4.5/hazelbean/calculation_core/compile_cython_functions.py
--rw-rw-rw-   0        0        0  3445406 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.c
--rw-rw-rw-   0        0        0   567808 2023-06-02 01:58:12.000000 hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0  3452047 2023-06-06 15:16:35.000000 hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.cpp
--rw-rw-rw-   0        0        0   150011 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.pyx
--rw-rw-rw-   0        0        0     4830 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/cat_ears.py
--rw-rw-rw-   0        0        0     7177 2023-06-01 20:54:47.000000 hazelbean-1.4.5/hazelbean/cloud_utils.py
--rw-rw-rw-   0        0        0    19206 2022-09-23 17:47:57.000000 hazelbean-1.4.5/hazelbean/config.py
--rw-rw-rw-   0        0        0     3471 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/conventions.py
--rw-rw-rw-   0        0        0     8594 2023-06-05 19:37:33.000000 hazelbean-1.4.5/hazelbean/core.py
--rw-rw-rw-   0        0        0    21132 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/data_structures.py
--rw-rw-rw-   0        0        0    30780 2023-02-16 18:33:50.000000 hazelbean-1.4.5/hazelbean/file_io.py
--rw-rw-rw-   0        0        0   115964 2022-09-23 21:13:00.000000 hazelbean-1.4.5/hazelbean/geoprocessing.py
--rw-rw-rw-   0        0        0    74113 2023-03-08 17:18:14.000000 hazelbean-1.4.5/hazelbean/geoprocessing_extension.py
--rw-rw-rw-   0        0        0    44554 2022-09-22 15:56:20.000000 hazelbean-1.4.5/hazelbean/globals.py
--rw-rw-rw-   0        0        0    43887 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/netcdf.py
--rw-rw-rw-   0        0        0    75326 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/os_utils.py
--rw-rw-rw-   0        0        0    20647 2023-01-28 21:04:04.000000 hazelbean-1.4.5/hazelbean/parallel.py
--rw-rw-rw-   0        0        0    52148 2023-05-08 17:19:48.000000 hazelbean-1.4.5/hazelbean/project_flow.py
--rw-rw-rw-   0        0        0   100770 2023-05-09 13:27:50.000000 hazelbean-1.4.5/hazelbean/pyramids.py
--rw-rw-rw-   0        0        0    52342 2022-06-15 17:44:31.000000 hazelbean-1.4.5/hazelbean/raster_vector_interface.py
--rw-rw-rw-   0        0        0      290 2022-09-22 18:26:12.000000 hazelbean-1.4.5/hazelbean/slow_config.py
--rw-rw-rw-   0        0        0    38359 2022-09-28 14:32:01.000000 hazelbean-1.4.5/hazelbean/spatial_projection.py
--rw-rw-rw-   0        0        0   237426 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/spatial_utils.py
--rw-rw-rw-   0        0        0    90574 2023-01-12 21:05:30.000000 hazelbean-1.4.5/hazelbean/stats.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:02:20.040000 hazelbean-1.4.5/hazelbean/ui/
--rw-rw-rw-   0        0        0        0 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/__init__.py
--rw-rw-rw-   0        0        0     5376 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/auto_ui.py
--rw-rw-rw-   0        0        0     6353 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/auto_ui_tg.py
--rw-rw-rw-   0        0        0    23376 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/cli.py
--rw-rw-rw-   0        0        0    24868 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/datastack.py
--rw-rw-rw-   0        0        0     2621 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/execution.py
--rw-rw-rw-   0        0        0   102272 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/inputs.py
--rw-rw-rw-   0        0        0     2565 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/launcher.py
--rw-rw-rw-   0        0        0   112823 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/model.py
--rw-rw-rw-   0        0        0    10862 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/usage.py
--rw-rw-rw-   0        0        0     3750 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/usage_logger.py
--rw-rw-rw-   0        0        0    18766 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/utils.py
--rw-rw-rw-   0        0        0     5941 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/validation.py
--rw-rw-rw-   0        0        0    31953 2023-06-07 19:23:27.000000 hazelbean-1.4.5/hazelbean/utils.py
--rw-rw-rw-   0        0        0    82552 2023-03-03 14:42:11.000000 hazelbean-1.4.5/hazelbean/visualization.py
--rw-rw-rw-   0        0        0     8838 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/watershed_processing.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:02:18.299000 hazelbean-1.4.5/hazelbean.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-08 15:02:15.000000 hazelbean-1.4.5/hazelbean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1857 2023-06-08 15:02:15.000000 hazelbean-1.4.5/hazelbean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 15:02:15.000000 hazelbean-1.4.5/hazelbean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-08 15:02:15.000000 hazelbean-1.4.5/hazelbean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-08 15:02:20.120000 hazelbean-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1708 2023-06-08 15:02:14.000000 hazelbean-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:52:07.476000 hazelbean-1.4.6/
+-rw-rw-rw-   0        0        0    14763 2023-06-15 11:51:56.000000 hazelbean-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0      145 2023-06-15 11:51:56.000000 hazelbean-1.4.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      443 2023-06-15 11:52:07.441000 hazelbean-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4863 2023-06-15 11:51:57.000000 hazelbean-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 11:52:04.692000 hazelbean-1.4.6/hazelbean/
+-rw-rw-rw-   0        0        0     8196 2022-09-28 15:14:40.000000 hazelbean-1.4.6/hazelbean/__init__.py
+-rw-rw-rw-   0        0        0    15645 2022-09-28 14:32:01.000000 hazelbean-1.4.6/hazelbean/arrayframe.py
+-rw-rw-rw-   0        0        0     6865 2022-05-09 18:31:33.000000 hazelbean-1.4.6/hazelbean/arrayframe_functions.py
+-rw-rw-rw-   0        0        0     5787 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/arrayframe_numpy_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:52:06.542000 hazelbean-1.4.6/hazelbean/calculation_core/
+-rw-rw-rw-   0        0        0     2523 2022-09-27 18:48:13.000000 hazelbean-1.4.6/hazelbean/calculation_core/__init__.py
+-rw-rw-rw-   0        0        0   364367 2023-01-30 15:25:17.000000 hazelbean-1.4.6/hazelbean/calculation_core/aspect_ratio_array_functions.c
+-rw-rw-rw-   0        0        0    59392 2023-01-30 15:25:21.000000 hazelbean-1.4.6/hazelbean/calculation_core/aspect_ratio_array_functions.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0   370413 2023-06-06 15:16:35.000000 hazelbean-1.4.6/hazelbean/calculation_core/aspect_ratio_array_functions.cpp
+-rw-rw-rw-   0        0        0     5843 2023-01-30 15:25:06.000000 hazelbean-1.4.6/hazelbean/calculation_core/aspect_ratio_array_functions.pyx
+-rw-rw-rw-   0        0        0      746 2023-06-01 20:11:21.000000 hazelbean-1.4.6/hazelbean/calculation_core/compile_cython_functions.py
+-rw-rw-rw-   0        0        0  3445406 2023-06-01 20:11:20.000000 hazelbean-1.4.6/hazelbean/calculation_core/cython_functions.c
+-rw-rw-rw-   0        0        0   567808 2023-06-02 01:58:12.000000 hazelbean-1.4.6/hazelbean/calculation_core/cython_functions.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0  3452047 2023-06-06 15:16:35.000000 hazelbean-1.4.6/hazelbean/calculation_core/cython_functions.cpp
+-rw-rw-rw-   0        0        0   150011 2023-06-01 20:11:20.000000 hazelbean-1.4.6/hazelbean/calculation_core/cython_functions.pyx
+-rw-rw-rw-   0        0        0     4830 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/cat_ears.py
+-rw-rw-rw-   0        0        0     7588 2023-06-12 16:50:12.000000 hazelbean-1.4.6/hazelbean/cloud_utils.py
+-rw-rw-rw-   0        0        0    19206 2022-09-23 17:47:57.000000 hazelbean-1.4.6/hazelbean/config.py
+-rw-rw-rw-   0        0        0     3471 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/conventions.py
+-rw-rw-rw-   0        0        0     8594 2023-06-05 19:37:33.000000 hazelbean-1.4.6/hazelbean/core.py
+-rw-rw-rw-   0        0        0    21132 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/data_structures.py
+-rw-rw-rw-   0        0        0    30780 2023-02-16 18:33:50.000000 hazelbean-1.4.6/hazelbean/file_io.py
+-rw-rw-rw-   0        0        0   115964 2022-09-23 21:13:00.000000 hazelbean-1.4.6/hazelbean/geoprocessing.py
+-rw-rw-rw-   0        0        0    74113 2023-03-08 17:18:14.000000 hazelbean-1.4.6/hazelbean/geoprocessing_extension.py
+-rw-rw-rw-   0        0        0    44554 2022-09-22 15:56:20.000000 hazelbean-1.4.6/hazelbean/globals.py
+-rw-rw-rw-   0        0        0    43887 2023-06-01 20:11:20.000000 hazelbean-1.4.6/hazelbean/netcdf.py
+-rw-rw-rw-   0        0        0    75326 2023-06-01 20:11:20.000000 hazelbean-1.4.6/hazelbean/os_utils.py
+-rw-rw-rw-   0        0        0    20647 2023-01-28 21:04:04.000000 hazelbean-1.4.6/hazelbean/parallel.py
+-rw-rw-rw-   0        0        0    52148 2023-05-08 17:19:48.000000 hazelbean-1.4.6/hazelbean/project_flow.py
+-rw-rw-rw-   0        0        0   100770 2023-05-09 13:27:50.000000 hazelbean-1.4.6/hazelbean/pyramids.py
+-rw-rw-rw-   0        0        0    52342 2022-06-15 17:44:31.000000 hazelbean-1.4.6/hazelbean/raster_vector_interface.py
+-rw-rw-rw-   0        0        0      290 2022-09-22 18:26:12.000000 hazelbean-1.4.6/hazelbean/slow_config.py
+-rw-rw-rw-   0        0        0    38359 2022-09-28 14:32:01.000000 hazelbean-1.4.6/hazelbean/spatial_projection.py
+-rw-rw-rw-   0        0        0   237426 2023-06-01 20:11:20.000000 hazelbean-1.4.6/hazelbean/spatial_utils.py
+-rw-rw-rw-   0        0        0    90574 2023-01-12 21:05:30.000000 hazelbean-1.4.6/hazelbean/stats.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:52:07.410000 hazelbean-1.4.6/hazelbean/ui/
+-rw-rw-rw-   0        0        0        0 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/__init__.py
+-rw-rw-rw-   0        0        0     5376 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/auto_ui.py
+-rw-rw-rw-   0        0        0     6353 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/auto_ui_tg.py
+-rw-rw-rw-   0        0        0    23376 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/cli.py
+-rw-rw-rw-   0        0        0    24868 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/datastack.py
+-rw-rw-rw-   0        0        0     2621 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/execution.py
+-rw-rw-rw-   0        0        0   102272 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/inputs.py
+-rw-rw-rw-   0        0        0     2565 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/launcher.py
+-rw-rw-rw-   0        0        0   112823 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/model.py
+-rw-rw-rw-   0        0        0    10862 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/usage.py
+-rw-rw-rw-   0        0        0     3750 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/usage_logger.py
+-rw-rw-rw-   0        0        0    18766 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/utils.py
+-rw-rw-rw-   0        0        0     5941 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/ui/validation.py
+-rw-rw-rw-   0        0        0    32547 2023-06-12 22:59:07.000000 hazelbean-1.4.6/hazelbean/utils.py
+-rw-rw-rw-   0        0        0    82552 2023-03-03 14:42:11.000000 hazelbean-1.4.6/hazelbean/visualization.py
+-rw-rw-rw-   0        0        0     8838 2022-03-21 14:48:42.000000 hazelbean-1.4.6/hazelbean/watershed_processing.py
+drwxrwxrwx   0        0        0        0 2023-06-15 11:52:04.949000 hazelbean-1.4.6/hazelbean.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-06-15 11:52:00.000000 hazelbean-1.4.6/hazelbean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1857 2023-06-15 11:52:01.000000 hazelbean-1.4.6/hazelbean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 11:52:00.000000 hazelbean-1.4.6/hazelbean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-15 11:52:00.000000 hazelbean-1.4.6/hazelbean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-15 11:52:07.471000 hazelbean-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1708 2023-06-15 11:51:57.000000 hazelbean-1.4.6/setup.py
```

### Comparing `hazelbean-1.4.5/LICENSE` & `hazelbean-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/README.md` & `hazelbean-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/__init__.py` & `hazelbean-1.4.6/hazelbean/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/arrayframe.py` & `hazelbean-1.4.6/hazelbean/arrayframe.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/arrayframe_functions.py` & `hazelbean-1.4.6/hazelbean/arrayframe_functions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/arrayframe_numpy_functions.py` & `hazelbean-1.4.6/hazelbean/arrayframe_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/calculation_core/__init__.py` & `hazelbean-1.4.6/hazelbean/calculation_core/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.c` & `hazelbean-1.4.6/hazelbean/calculation_core/aspect_ratio_array_functions.c`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.cpp` & `hazelbean-1.4.6/hazelbean/calculation_core/aspect_ratio_array_functions.cpp`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.pyx` & `hazelbean-1.4.6/hazelbean/calculation_core/aspect_ratio_array_functions.pyx`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/calculation_core/compile_cython_functions.py` & `hazelbean-1.4.6/hazelbean/calculation_core/compile_cython_functions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.c` & `hazelbean-1.4.6/hazelbean/calculation_core/cython_functions.c`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.cpp` & `hazelbean-1.4.6/hazelbean/calculation_core/cython_functions.cpp`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.pyx` & `hazelbean-1.4.6/hazelbean/calculation_core/cython_functions.pyx`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/cat_ears.py` & `hazelbean-1.4.6/hazelbean/cat_ears.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/cloud_utils.py` & `hazelbean-1.4.6/hazelbean/cloud_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,19 +109,20 @@
 
     task_graph.close()
     task_graph.join()
 
 
 
 def download_google_cloud_blob(bucket_name, source_blob_name, credentials_path, destination_file_name, chunk_size=262144*5,):
-    """Downloads a blob from the bucket."""
-    if hb.path_exists(credentials_path):
+    """REPLACED IN SEALS BY SEALS VERSION. Downloads a blob from the bucket."""
+    require_database = True
+    if hb.path_exists(credentials_path) and require_database:
         client = storage.Client.from_service_account_json(credentials_path)
     else:
-        raise L.critical('Unable to find database license. Your code currently is stating it should be found at ' + str(credentials_path))
+        raise NameError('Unable to find database license. Your code currently is stating it should be found at ' + str(credentials_path) + ' relative to where the run script was launched. If you would like to generate your own database, disable this check (set require_database to False). Otherwise, feel free to reach out to the developer of SEALS to acquire the license key. It is only limited because the data are huge and expensive to host (600+ Gigabytes).')
 
     try:
         bucket = client.get_bucket(bucket_name)
     except Exception as e:
         L.critical('Unable to get bucket ' + str(bucket_name) + ' with exception ' + str(e))
 
     try:
```

### Comparing `hazelbean-1.4.5/hazelbean/config.py` & `hazelbean-1.4.6/hazelbean/config.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/conventions.py` & `hazelbean-1.4.6/hazelbean/conventions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/core.py` & `hazelbean-1.4.6/hazelbean/core.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/data_structures.py` & `hazelbean-1.4.6/hazelbean/data_structures.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/file_io.py` & `hazelbean-1.4.6/hazelbean/file_io.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/geoprocessing.py` & `hazelbean-1.4.6/hazelbean/geoprocessing.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/geoprocessing_extension.py` & `hazelbean-1.4.6/hazelbean/geoprocessing_extension.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/globals.py` & `hazelbean-1.4.6/hazelbean/globals.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/netcdf.py` & `hazelbean-1.4.6/hazelbean/netcdf.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/os_utils.py` & `hazelbean-1.4.6/hazelbean/os_utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/parallel.py` & `hazelbean-1.4.6/hazelbean/parallel.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/project_flow.py` & `hazelbean-1.4.6/hazelbean/project_flow.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/pyramids.py` & `hazelbean-1.4.6/hazelbean/pyramids.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/raster_vector_interface.py` & `hazelbean-1.4.6/hazelbean/raster_vector_interface.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/spatial_projection.py` & `hazelbean-1.4.6/hazelbean/spatial_projection.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/spatial_utils.py` & `hazelbean-1.4.6/hazelbean/spatial_utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/stats.py` & `hazelbean-1.4.6/hazelbean/stats.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/auto_ui.py` & `hazelbean-1.4.6/hazelbean/ui/auto_ui.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/auto_ui_tg.py` & `hazelbean-1.4.6/hazelbean/ui/auto_ui_tg.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/cli.py` & `hazelbean-1.4.6/hazelbean/ui/cli.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/datastack.py` & `hazelbean-1.4.6/hazelbean/ui/datastack.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/execution.py` & `hazelbean-1.4.6/hazelbean/ui/execution.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/inputs.py` & `hazelbean-1.4.6/hazelbean/ui/inputs.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/launcher.py` & `hazelbean-1.4.6/hazelbean/ui/launcher.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/model.py` & `hazelbean-1.4.6/hazelbean/ui/model.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/usage.py` & `hazelbean-1.4.6/hazelbean/ui/usage.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/usage_logger.py` & `hazelbean-1.4.6/hazelbean/ui/usage_logger.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/utils.py` & `hazelbean-1.4.6/hazelbean/ui/utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/ui/validation.py` & `hazelbean-1.4.6/hazelbean/ui/validation.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/utils.py` & `hazelbean-1.4.6/hazelbean/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 
 import hazelbean as hb
 import math
 from osgeo import gdal
 import contextlib
 import logging
+from google.cloud import storage
 
 import pandas as pd
 
 L = hb.get_logger('hazelbean utils')
 
 def hprint(*args, **kwargs):
     return hb_pprint(*args, **kwargs)
@@ -757,21 +758,34 @@
         return True
     else:
         return False
     
 def get_first_extant_path(relative_path, possible_dirs):
     # Searches for a file in a list of possible directories and returns the first one it finds.
     # If it doesn't find any, it returns the first one it tried.
+    # If it was given None, just return None
+
+    if hb.path_exists(relative_path):
+        return relative_path
+
+    # Check if it's relative
+    if relative_path is not None:
+        if relative_path[1] == ':':
+            raise NameError('The path given to hb.get_first_extant_path() does not appear to be relative (nor does it exist at the unmodified path): ' + str(relative_path) + ', ' + str(possible_dirs))
+
     for possible_dir in possible_dirs:
-        path = os.path.join(possible_dir, relative_path)
-        if hb.path_exists(path):
-            return path
+        if relative_path is not None:
+            path = os.path.join(possible_dir, relative_path)
+            if hb.path_exists(path):
+                return path
+        else:
+            return None
+    
+    # If it was neither found nor None, THEN return the path constructed from the first element in possible_dirs
     path = os.path.join(possible_dirs[0], relative_path)
-
-    # START HERE: Got confused on logic because of double-nesting the filename
     return path
 
 
 
 def path_to_url(input_path, local_path_to_strip, url_start=''):
     splitted_path = hb.split_assume_two(input_path.replace('\\', '/'), local_path_to_strip.replace('\\', '/')) 
     right_path = splitted_path[1]
@@ -804,8 +818,10 @@
   seen = set()
   new_lst = []
   for item in lst:
     if item not in seen:
       seen.add(item)
       new_lst.append(item)
 
-  return new_lst
+  return new_lst
+
+
```

### Comparing `hazelbean-1.4.5/hazelbean/visualization.py` & `hazelbean-1.4.6/hazelbean/visualization.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean/watershed_processing.py` & `hazelbean-1.4.6/hazelbean/watershed_processing.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/hazelbean.egg-info/SOURCES.txt` & `hazelbean-1.4.6/hazelbean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.5/setup.py` & `hazelbean-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 packages=find_packages()
 include_package_data=True
 
 setup(
   name = 'hazelbean',
   packages = packages,
-  version = '1.4.5',
+  version = '1.4.6',
   description = 'Geospatial research tools',
   long_description = 'Geospatial research tools for economics and sustainability science.',
   author = 'Justin Andrew Johnson',
   url = 'https://github.com/jandrewjohnson/hazelbean',
   download_url = 'https://github.com/jandrewjohnson/hazelbean',
   keywords = ['geospatial', 'raster', 'shapefile', 'sustainability science'],
   classifiers = ["Programming Language :: Python :: 3"],
```

