# Comparing `tmp/McStasScript-0.0.8.tar.gz` & `tmp/McStasScript-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/McStasScript-0.0.8.tar", last modified: Mon Jul 29 08:41:08 2019, max compression
+gzip compressed data, was "dist/McStasScript-0.0.9.tar", last modified: Mon Aug 12 12:41:46 2019, max compression
```

## Comparing `McStasScript-0.0.8.tar` & `McStasScript-0.0.9.tar`

### file list

```diff
@@ -1,69 +1,78 @@
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    35149 2019-03-05 11:50:14.000000 McStasScript-0.0.8/LICENSE
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      205 2019-07-26 08:59:03.000000 McStasScript-0.0.8/MANIFEST.in
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/McStasScript.egg-info/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6125 2019-07-29 08:41:07.000000 McStasScript-0.0.8/McStasScript.egg-info/PKG-INFO
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2068 2019-07-29 08:41:07.000000 McStasScript-0.0.8/McStasScript.egg-info/SOURCES.txt
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        1 2019-07-29 08:41:07.000000 McStasScript-0.0.8/McStasScript.egg-info/dependency_links.txt
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)       17 2019-07-29 08:41:07.000000 McStasScript-0.0.8/McStasScript.egg-info/requires.txt
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)       13 2019-07-29 08:41:07.000000 McStasScript-0.0.8/McStasScript.egg-info/top_level.txt
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)   162306 2019-07-29 08:38:22.000000 McStasScript-0.0.8/McStasScript_documentation.pdf
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6125 2019-07-29 08:41:08.000000 McStasScript-0.0.8/PKG-INFO
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4864 2019-07-29 08:39:26.000000 McStasScript-0.0.8/README.md
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     8796 2019-07-25 12:07:08.000000 McStasScript-0.0.8/log.txt
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 12:43:38.000000 McStasScript-0.0.8/mcstasscript/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      193 2019-07-26 08:31:41.000000 McStasScript-0.0.8/mcstasscript/configuration.yaml
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/data/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 12:43:39.000000 McStasScript-0.0.8/mcstasscript/data/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     9413 2019-06-11 12:36:30.000000 McStasScript-0.0.8/mcstasscript/data/data.py
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/helper/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 12:43:39.000000 McStasScript-0.0.8/mcstasscript/helper/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    13940 2019-06-04 12:50:11.000000 McStasScript-0.0.8/mcstasscript/helper/component_reader.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      947 2019-06-04 12:51:27.000000 McStasScript-0.0.8/mcstasscript/helper/formatting.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     8909 2019-06-13 12:16:48.000000 McStasScript-0.0.8/mcstasscript/helper/managed_mcrun.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    28000 2019-06-17 12:56:39.000000 McStasScript-0.0.8/mcstasscript/helper/mcstas_objects.py
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/integration_tests/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-25 14:10:23.000000 McStasScript-0.0.8/mcstasscript/integration_tests/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6351 2019-06-17 12:46:59.000000 McStasScript-0.0.8/mcstasscript/integration_tests/test_complex_instrument.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     5293 2019-06-13 13:36:42.000000 McStasScript-0.0.8/mcstasscript/integration_tests/test_simple_instrument.py
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/interface/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 12:43:38.000000 McStasScript-0.0.8/mcstasscript/interface/__init__.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     3978 2019-07-26 08:02:50.000000 McStasScript-0.0.8/mcstasscript/interface/configurator.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6795 2019-07-26 08:21:51.000000 McStasScript-0.0.8/mcstasscript/interface/functions.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    46932 2019-07-25 13:50:09.000000 McStasScript-0.0.8/mcstasscript/interface/instr.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    22779 2019-07-25 14:58:52.000000 McStasScript-0.0.8/mcstasscript/interface/plotter.py
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/tests/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 15:00:48.000000 McStasScript-0.0.8/mcstasscript/tests/__init__.py
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/contrib/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:19:23.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/contrib/test_for_empty.txt
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/misc/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:18:26.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/misc/test_for_ignore.com
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:18:38.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/misc/test_for_ignore_weird.comp.backup
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     5760 2019-05-14 13:39:38.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/misc/test_for_reading.comp
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:18:13.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/misc/test_for_structure.comp
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/sources/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:19:06.000000 McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/sources/test_for_structure2.comp
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    17303 2019-06-04 06:49:14.000000 McStasScript-0.0.8/mcstasscript/tests/test_ComponentReader.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4704 2019-07-26 08:22:07.000000 McStasScript-0.0.8/mcstasscript/tests/test_Configurator.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    53833 2019-07-26 08:30:22.000000 McStasScript-0.0.8/mcstasscript/tests/test_Instr.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    14458 2019-06-13 13:34:36.000000 McStasScript-0.0.8/mcstasscript/tests/test_ManagedMcrun.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4349 2019-05-20 07:24:01.000000 McStasScript-0.0.8/mcstasscript/tests/test_McStasData.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4395 2019-05-20 07:34:02.000000 McStasScript-0.0.8/mcstasscript/tests/test_McStasMetaData.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2171 2019-05-20 07:35:27.000000 McStasScript-0.0.8/mcstasscript/tests/test_McStasPlotOptions.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    22873 2019-06-17 12:57:00.000000 McStasScript-0.0.8/mcstasscript/tests/test_component.py
-drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-29 08:41:08.000000 McStasScript-0.0.8/mcstasscript/tests/test_data_set/
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4249 2019-05-15 09:49:59.000000 McStasScript-0.0.8/mcstasscript/tests/test_data_set/L_mon.dat
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)  1087701 2019-05-15 09:49:59.000000 McStasScript-0.0.8/mcstasscript/tests/test_data_set/PSD.dat
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)  3066044 2019-05-15 09:49:59.000000 McStasScript-0.0.8/mcstasscript/tests/test_data_set/PSD_4PI.dat
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2199 2019-05-15 09:49:59.000000 McStasScript-0.0.8/mcstasscript/tests/test_data_set/jupyter_demo.instr
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2256 2019-05-15 09:49:59.000000 McStasScript-0.0.8/mcstasscript/tests/test_data_set/mccode.sim
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6432 2019-05-20 07:55:08.000000 McStasScript-0.0.8/mcstasscript/tests/test_declare_variable.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     5654 2019-05-14 14:21:54.000000 McStasScript-0.0.8/mcstasscript/tests/test_for_reading.comp
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2041 2019-05-21 11:17:24.000000 McStasScript-0.0.8/mcstasscript/tests/test_formatting.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     7751 2019-07-24 07:39:15.000000 McStasScript-0.0.8/mcstasscript/tests/test_functions.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6507 2019-05-20 07:59:45.000000 McStasScript-0.0.8/mcstasscript/tests/test_parameter_variable.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      387 2019-06-04 07:55:35.000000 McStasScript-0.0.8/mcstasscript/tests/utilities.py
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)       38 2019-07-29 08:41:08.000000 McStasScript-0.0.8/setup.cfg
--rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      755 2019-07-29 08:40:57.000000 McStasScript-0.0.8/setup.py
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    35149 2019-03-05 11:50:14.000000 McStasScript-0.0.9/LICENSE
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      205 2019-07-26 08:59:03.000000 McStasScript-0.0.9/MANIFEST.in
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/McStasScript.egg-info/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     7171 2019-08-12 12:41:45.000000 McStasScript-0.0.9/McStasScript.egg-info/PKG-INFO
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2417 2019-08-12 12:41:45.000000 McStasScript-0.0.9/McStasScript.egg-info/SOURCES.txt
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        1 2019-08-12 12:41:45.000000 McStasScript-0.0.9/McStasScript.egg-info/dependency_links.txt
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)       17 2019-08-12 12:41:45.000000 McStasScript-0.0.9/McStasScript.egg-info/requires.txt
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)       13 2019-08-12 12:41:45.000000 McStasScript-0.0.9/McStasScript.egg-info/top_level.txt
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)   167419 2019-08-12 12:07:30.000000 McStasScript-0.0.9/McStasScript_documentation.pdf
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     7171 2019-08-12 12:41:46.000000 McStasScript-0.0.9/PKG-INFO
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     5798 2019-08-12 12:40:20.000000 McStasScript-0.0.9/README.md
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 12:43:38.000000 McStasScript-0.0.9/mcstasscript/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      193 2019-07-26 08:31:41.000000 McStasScript-0.0.9/mcstasscript/configuration.yaml
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/data/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 12:43:39.000000 McStasScript-0.0.9/mcstasscript/data/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     9633 2019-08-07 06:13:13.000000 McStasScript-0.0.9/mcstasscript/data/data.py
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/helper/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 12:43:39.000000 McStasScript-0.0.9/mcstasscript/helper/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    14898 2019-08-09 08:39:21.000000 McStasScript-0.0.9/mcstasscript/helper/component_reader.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      947 2019-06-04 12:51:27.000000 McStasScript-0.0.9/mcstasscript/helper/formatting.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     8963 2019-08-07 06:13:49.000000 McStasScript-0.0.9/mcstasscript/helper/managed_mcrun.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    30671 2019-08-09 12:52:41.000000 McStasScript-0.0.9/mcstasscript/helper/mcstas_objects.py
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/instr_reader/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-01 12:35:09.000000 McStasScript-0.0.9/mcstasscript/instr_reader/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     8205 2019-08-12 05:37:41.000000 McStasScript-0.0.9/mcstasscript/instr_reader/control.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    11034 2019-08-12 07:15:56.000000 McStasScript-0.0.9/mcstasscript/instr_reader/read_declare.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     5401 2019-08-12 07:05:50.000000 McStasScript-0.0.9/mcstasscript/instr_reader/read_definition.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     1865 2019-08-07 09:49:31.000000 McStasScript-0.0.9/mcstasscript/instr_reader/read_finally.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2304 2019-08-12 05:51:49.000000 McStasScript-0.0.9/mcstasscript/instr_reader/read_initialize.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    23720 2019-08-12 07:15:32.000000 McStasScript-0.0.9/mcstasscript/instr_reader/read_trace.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4345 2019-08-12 05:40:38.000000 McStasScript-0.0.9/mcstasscript/instr_reader/util.py
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/integration_tests/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-07-25 14:10:23.000000 McStasScript-0.0.9/mcstasscript/integration_tests/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6351 2019-06-17 12:46:59.000000 McStasScript-0.0.9/mcstasscript/integration_tests/test_complex_instrument.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     5293 2019-06-13 13:36:42.000000 McStasScript-0.0.9/mcstasscript/integration_tests/test_simple_instrument.py
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/interface/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 12:43:38.000000 McStasScript-0.0.9/mcstasscript/interface/__init__.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6795 2019-07-26 08:21:51.000000 McStasScript-0.0.9/mcstasscript/interface/functions.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    54446 2019-08-12 09:02:40.000000 McStasScript-0.0.9/mcstasscript/interface/instr.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    22779 2019-07-25 14:58:52.000000 McStasScript-0.0.9/mcstasscript/interface/plotter.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2330 2019-08-12 07:52:25.000000 McStasScript-0.0.9/mcstasscript/interface/reader.py
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/tests/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-13 15:00:48.000000 McStasScript-0.0.9/mcstasscript/tests/__init__.py
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:45.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/contrib/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:19:23.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/contrib/test_for_empty.txt
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/misc/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:18:26.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/misc/test_for_ignore.com
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:18:38.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/misc/test_for_ignore_weird.comp.backup
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     5760 2019-05-14 13:39:38.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/misc/test_for_reading.comp
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:18:13.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/misc/test_for_structure.comp
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/sources/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-05-14 09:19:06.000000 McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/sources/test_for_structure2.comp
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    17303 2019-06-04 06:49:14.000000 McStasScript-0.0.9/mcstasscript/tests/test_ComponentReader.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4704 2019-07-26 08:22:07.000000 McStasScript-0.0.9/mcstasscript/tests/test_Configurator.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    58435 2019-08-12 11:44:05.000000 McStasScript-0.0.9/mcstasscript/tests/test_Instr.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    12418 2019-08-12 11:21:07.000000 McStasScript-0.0.9/mcstasscript/tests/test_Instr_reader.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    14458 2019-06-13 13:34:36.000000 McStasScript-0.0.9/mcstasscript/tests/test_ManagedMcrun.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4349 2019-05-20 07:24:01.000000 McStasScript-0.0.9/mcstasscript/tests/test_McStasData.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4395 2019-05-20 07:34:02.000000 McStasScript-0.0.9/mcstasscript/tests/test_McStasMetaData.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2171 2019-05-20 07:35:27.000000 McStasScript-0.0.9/mcstasscript/tests/test_McStasPlotOptions.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)    24439 2019-08-09 12:52:24.000000 McStasScript-0.0.9/mcstasscript/tests/test_component.py
+drwxr-xr-x   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)        0 2019-08-12 12:41:46.000000 McStasScript-0.0.9/mcstasscript/tests/test_data_set/
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     4249 2019-05-15 09:49:59.000000 McStasScript-0.0.9/mcstasscript/tests/test_data_set/L_mon.dat
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)  1087701 2019-05-15 09:49:59.000000 McStasScript-0.0.9/mcstasscript/tests/test_data_set/PSD.dat
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)  3066044 2019-05-15 09:49:59.000000 McStasScript-0.0.9/mcstasscript/tests/test_data_set/PSD_4PI.dat
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2199 2019-05-15 09:49:59.000000 McStasScript-0.0.9/mcstasscript/tests/test_data_set/jupyter_demo.instr
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2256 2019-05-15 09:49:59.000000 McStasScript-0.0.9/mcstasscript/tests/test_data_set/mccode.sim
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6432 2019-05-20 07:55:08.000000 McStasScript-0.0.9/mcstasscript/tests/test_declare_variable.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     5654 2019-05-14 14:21:54.000000 McStasScript-0.0.9/mcstasscript/tests/test_for_reading.comp
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     2041 2019-05-21 11:17:24.000000 McStasScript-0.0.9/mcstasscript/tests/test_formatting.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     7751 2019-07-24 07:39:15.000000 McStasScript-0.0.9/mcstasscript/tests/test_functions.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)     6507 2019-05-20 07:59:45.000000 McStasScript-0.0.9/mcstasscript/tests/test_parameter_variable.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      388 2019-08-12 11:58:33.000000 McStasScript-0.0.9/mcstasscript/tests/utilities.py
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)       38 2019-08-12 12:41:46.000000 McStasScript-0.0.9/setup.cfg
+-rw-r--r--   0 madsbertelsen (1083417152) ESSS\Domain Users (14964212)      755 2019-08-12 12:41:13.000000 McStasScript-0.0.9/setup.py
```

### Comparing `McStasScript-0.0.8/LICENSE` & `McStasScript-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/McStasScript.egg-info/PKG-INFO` & `McStasScript-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-Metadata-Version: 2.1
-Name: McStasScript
-Version: 0.0.8
-Summary: A python scripting interface for McStas
-Home-page: https://github.com/PaNOSC-ViNYL/McStasScript
-Author: Mads Bertelsen
-Author-email: Mads.Bertelsen@esss.se
-License: UNKNOWN
-Description: # McStasScript
-        McStas API for creating and running McStas instruments from python scripting
-        
-        Prototype for an API that allow interaction with McStas through an interface like Jupyter Notebooks created under WP5 of PaNOSC.
-        
-        ## Installation
-        The package can be installed using pip
-        
-            python3 -m pip install McStasScript --upgrade
-        
-        It is necessary to configure the package so the McStas installation can be found, here we show how the appropriate code for an Ubuntu system. The configuration is saved permanently, and only needs to be updated when McStas is updated.
-        
-            from mcstasscript.interface import functions
-            my_configurator = functions.Configurator()
-            my_configurator.set_mcrun_path("/usr/bin/")
-            my_configurator.set_mcstas_path("/usr/share/mcstas/2.5/")
-        
-        
-        ## Instructions for basic use:
-        Import the interface 
-        
-            from mcstasscript.interface import instr, plotter, functions
-        
-        Now the package can be used. Start with creating a new instrument, just needs a name
-        
-            my_instrument = instr.McStas_instr("my_instrument_file")
-        
-        Then McStas components can be added, here we add a source
-        
-            my_source = my_instrument.add_component("source", "Source_simple")
-            my_source.show_parameters() # Can be used to show available parameters for Source simple
-        
-        The parameters of the source can be adjusted directly as attributes of the python object
-        
-            my_source.xwidth = 0.12
-            my_source.yheight = 0.12
-            my_source.lambda0 = 3
-            my_source.dlambda = 2.2
-            my_source.focus_xw = 0.05
-            my_source.focus_yh = 0.05
-            
-        A monitor is added as well to get data out of the simulation
-        
-            PSD = Instr.add_component("PSD", "PSD_monitor", AT=[0,0,1], RELATIVE="source") 
-            PSD.xwidth = 0.1
-            PSD.yheight = 0.1
-            PSD.nx = 200
-            PSD.ny = 200
-            PSD.filename = "\"PSD.dat\""
-        
-        This simple simulation can be executed from the 
-        
-            data = my_instrument.run_full_instrument(foldername="first_run", increment_folder_name=True)
-        
-        Results from the monitors would be stored as a list of McStasData objects in the returned data. The counts are stored as numpy arrays. We can read and change the intensity directly and manipulate the data before plotting.
-        
-            data[0].Intensity
-            
-        Plotting is usually done in a subplot of all monitors recorded.    
-        
-            plot = plotter.make_sub_plot(data)
-        
-        
-        ## Method overview
-        Here is a quick overview of the available methods of the main classes in the project. Most have more options from keyword arguments that are explained in the manual, but also in python help, for example help(instr.McStas_instr.show_components).
-        
-            instr
-            └── McStas_instr(str instr_name) # Returns McStas instrument object on initialize
-                ├── show_components(str category_name) # Show available components in given category
-                ├── component_help(str component_name) # Prints component parameters for given component name   
-                ├── add_component(str name, str component_name) # Adds component to instrument and returns object
-                ├── add_parameter(str name) # Adds instrument parameter with name
-                ├── add_declare_var(str type, str name) # Adds declared variable with type and name
-                ├── append_initialize(str string) # Appends a line to initialize (c syntax)
-                ├── print_components() # Prints list of components and their location
-                ├── write_full_instrument() # Writes instrument to disk with given name + ".instr"
-                └── run_full_instrument() # Runs simulation. Options in keyword arguments. Returns list of McStasData
-                
-            component # returned by add_component
-            ├── set_AT(list at_list) # Sets component position (list of x,y,z positions in [m])
-            ├── set_ROTATED(list rotated_list) # Sets component rotation (list of x,y,z rotations in [deg])
-            ├── set_RELATIVE(str component_name) # Sets relative to other component name
-            ├── set_parameters(dict input) # Set parameters using dict input
-            ├── set_comment(str string) # Set comment explaining something about the component
-            └── print_long() # Prints currently contained information on component
-            
-            functions
-            ├── name_search(str name, list McStasData) # Returns data set with given name from McStasData list
-            ├── name_plot_options(str name, list McStasData, kwargs) # Sends kwargs to dataset with given name
-            ├── load_data(str foldername) # Loads data from folder with McStas data as McStasData list
-            └── Configurator()
-                ├── set_mcrun_path(str path) # sets mcrun path
-                ├── set_mcstas_path(str path) # sets mcstas path
-                └── set_line_length(int length) # sets maximum line length
-            
-            plotter
-            ├── make_plot(list McStasData) # Plots each data set individually
-            └── make_sub_plot(list McStasData) # Plots data as subplot
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# McStasScript
+McStas API for creating and running McStas instruments from python scripting
+
+Prototype for an API that allow interaction with McStas through an interface like Jupyter Notebooks created under WP5 of PaNOSC.
+
+## Installation
+The package can be installed using pip
+
+    python3 -m pip install McStasScript --upgrade
+
+It is necessary to configure the package so the McStas installation can be found, here we show how the appropriate code for an Ubuntu system. The configuration is saved permanently, and only needs to be updated when McStas is updated.
+
+    from mcstasscript.interface import functions
+    my_configurator = functions.Configurator()
+    my_configurator.set_mcrun_path("/usr/bin/")
+    my_configurator.set_mcstas_path("/usr/share/mcstas/2.5/")
+
+
+## Instructions for basic use:
+Import the interface 
+
+    from mcstasscript.interface import instr, plotter, functions, reader
+
+Now the package can be used. Start with creating a new instrument, just needs a name
+
+    my_instrument = instr.McStas_instr("my_instrument_file")
+
+Then McStas components can be added, here we add a source
+
+    my_source = my_instrument.add_component("source", "Source_simple")
+    my_source.show_parameters() # Can be used to show available parameters for Source simple
+
+The parameters of the source can be adjusted directly as attributes of the python object
+
+    my_source.xwidth = 0.12
+    my_source.yheight = 0.12
+    my_source.lambda0 = 3
+    my_source.dlambda = 2.2
+    my_source.focus_xw = 0.05
+    my_source.focus_yh = 0.05
+    
+A monitor is added as well to get data out of the simulation
+
+    PSD = my_instrument.add_component("PSD", "PSD_monitor", AT=[0,0,1], RELATIVE="source") 
+    PSD.xwidth = 0.1
+    PSD.yheight = 0.1
+    PSD.nx = 200
+    PSD.ny = 200
+    PSD.filename = "\"PSD.dat\""
+
+This simple simulation can be executed from the 
+
+    data = my_instrument.run_full_instrument(foldername="first_run", increment_folder_name=True)
+
+Results from the monitors would be stored as a list of McStasData objects in the returned data. The counts are stored as numpy arrays. We can read and change the intensity directly and manipulate the data before plotting.
+
+    data[0].Intensity
+    
+Plotting is usually done in a subplot of all monitors recorded.    
+
+    plot = plotter.make_sub_plot(data)
+
+## Use in existing project
+If one wish to work on existing projects using McStasScript, there is a reader included that will read a McStas Instrument file and write the corresponding McStasScript python instrument to disk. Here is an example where the PSI_DMC.instr example is converted:
+
+    Reader = reader.McStas_file("PSI_DMC.instr")
+    reader.write_python_file("PSI_DMC_generated.py")
+
+It is highly advised to run a check between the output of the generated file and the original to ensure the process was sucessful.
+
+## Method overview
+Here is a quick overview of the available methods of the main classes in the project. Most have more options from keyword arguments that are explained in the manual, but also in python help, for example help(instr.McStas_instr.show_components).
+
+    instr
+    └── McStas_instr(str instr_name) # Returns McStas instrument object on initialize
+        ├── show_components(str category_name) # Show available components in given category
+        ├── component_help(str component_name) # Prints component parameters for given component name   
+        ├── add_component(str name, str component_name) # Adds component to instrument and returns object
+        ├── add_parameter(str name) # Adds instrument parameter with name
+        ├── add_declare_var(str type, str name) # Adds declared variable with type and name
+        ├── append_initialize(str string) # Appends a line to initialize (c syntax)
+        ├── print_components() # Prints list of components and their location
+        ├── write_full_instrument() # Writes instrument to disk with given name + ".instr"
+        └── run_full_instrument() # Runs simulation. Options in keyword arguments. Returns list of McStasData
+        
+    component # returned by add_component
+    ├── set_AT(list at_list) # Sets component position (list of x,y,z positions in [m])
+    ├── set_ROTATED(list rotated_list) # Sets component rotation (list of x,y,z rotations in [deg])
+    ├── set_RELATIVE(str component_name) # Sets relative to other component name
+    ├── set_parameters(dict input) # Set parameters using dict input
+    ├── set_comment(str string) # Set comment explaining something about the component
+    └── print_long() # Prints currently contained information on component
+    
+    functions
+    ├── name_search(str name, list McStasData) # Returns data set with given name from McStasData list
+    ├── name_plot_options(str name, list McStasData, kwargs) # Sends kwargs to dataset with given name
+    ├── load_data(str foldername) # Loads data from folder with McStas data as McStasData list
+    └── Configurator()
+        ├── set_mcrun_path(str path) # sets mcrun path
+        ├── set_mcstas_path(str path) # sets mcstas path
+        └── set_line_length(int length) # sets maximum line length
+    
+    plotter
+    ├── make_plot(list McStasData) # Plots each data set individually
+    └── make_sub_plot(list McStasData) # Plots data as subplot
+    
+    reader
+    └──  McStas_file(str filename) # Returns a reader that can extract information from given instr file
+
+    InstrumentReader # returned by McStas_file
+    ├── generate_python_file(str filename) # Writes python file with information contaiend in isntrument
+    └── add_to_instr(McStas_instr Instr) # Adds information from instrument to McStasScirpt instrument
```

### Comparing `McStasScript-0.0.8/McStasScript.egg-info/SOURCES.txt` & `McStasScript-0.0.9/McStasScript.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 McStasScript_documentation.pdf
 README.md
-log.txt
 setup.py
 McStasScript.egg-info/PKG-INFO
 McStasScript.egg-info/SOURCES.txt
 McStasScript.egg-info/dependency_links.txt
 McStasScript.egg-info/requires.txt
 McStasScript.egg-info/top_level.txt
 mcstasscript/__init__.py
@@ -14,26 +13,35 @@
 mcstasscript/data/__init__.py
 mcstasscript/data/data.py
 mcstasscript/helper/__init__.py
 mcstasscript/helper/component_reader.py
 mcstasscript/helper/formatting.py
 mcstasscript/helper/managed_mcrun.py
 mcstasscript/helper/mcstas_objects.py
+mcstasscript/instr_reader/__init__.py
+mcstasscript/instr_reader/control.py
+mcstasscript/instr_reader/read_declare.py
+mcstasscript/instr_reader/read_definition.py
+mcstasscript/instr_reader/read_finally.py
+mcstasscript/instr_reader/read_initialize.py
+mcstasscript/instr_reader/read_trace.py
+mcstasscript/instr_reader/util.py
 mcstasscript/integration_tests/__init__.py
 mcstasscript/integration_tests/test_complex_instrument.py
 mcstasscript/integration_tests/test_simple_instrument.py
 mcstasscript/interface/__init__.py
-mcstasscript/interface/configurator.py
 mcstasscript/interface/functions.py
 mcstasscript/interface/instr.py
 mcstasscript/interface/plotter.py
+mcstasscript/interface/reader.py
 mcstasscript/tests/__init__.py
 mcstasscript/tests/test_ComponentReader.py
 mcstasscript/tests/test_Configurator.py
 mcstasscript/tests/test_Instr.py
+mcstasscript/tests/test_Instr_reader.py
 mcstasscript/tests/test_ManagedMcrun.py
 mcstasscript/tests/test_McStasData.py
 mcstasscript/tests/test_McStasMetaData.py
 mcstasscript/tests/test_McStasPlotOptions.py
 mcstasscript/tests/test_component.py
 mcstasscript/tests/test_declare_variable.py
 mcstasscript/tests/test_for_reading.comp
```

### Comparing `McStasScript-0.0.8/PKG-INFO` & `McStasScript-0.0.9/McStasScript.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: McStasScript
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python scripting interface for McStas
 Home-page: https://github.com/PaNOSC-ViNYL/McStasScript
 Author: Mads Bertelsen
 Author-email: Mads.Bertelsen@esss.se
 License: UNKNOWN
 Description: # McStasScript
         McStas API for creating and running McStas instruments from python scripting
@@ -23,15 +23,15 @@
             my_configurator.set_mcrun_path("/usr/bin/")
             my_configurator.set_mcstas_path("/usr/share/mcstas/2.5/")
         
         
         ## Instructions for basic use:
         Import the interface 
         
-            from mcstasscript.interface import instr, plotter, functions
+            from mcstasscript.interface import instr, plotter, functions, reader
         
         Now the package can be used. Start with creating a new instrument, just needs a name
         
             my_instrument = instr.McStas_instr("my_instrument_file")
         
         Then McStas components can be added, here we add a source
         
@@ -45,15 +45,15 @@
             my_source.lambda0 = 3
             my_source.dlambda = 2.2
             my_source.focus_xw = 0.05
             my_source.focus_yh = 0.05
             
         A monitor is added as well to get data out of the simulation
         
-            PSD = Instr.add_component("PSD", "PSD_monitor", AT=[0,0,1], RELATIVE="source") 
+            PSD = my_instrument.add_component("PSD", "PSD_monitor", AT=[0,0,1], RELATIVE="source") 
             PSD.xwidth = 0.1
             PSD.yheight = 0.1
             PSD.nx = 200
             PSD.ny = 200
             PSD.filename = "\"PSD.dat\""
         
         This simple simulation can be executed from the 
@@ -64,14 +64,21 @@
         
             data[0].Intensity
             
         Plotting is usually done in a subplot of all monitors recorded.    
         
             plot = plotter.make_sub_plot(data)
         
+        ## Use in existing project
+        If one wish to work on existing projects using McStasScript, there is a reader included that will read a McStas Instrument file and write the corresponding McStasScript python instrument to disk. Here is an example where the PSI_DMC.instr example is converted:
+        
+            Reader = reader.McStas_file("PSI_DMC.instr")
+            reader.write_python_file("PSI_DMC_generated.py")
+        
+        It is highly advised to run a check between the output of the generated file and the original to ensure the process was sucessful.
         
         ## Method overview
         Here is a quick overview of the available methods of the main classes in the project. Most have more options from keyword arguments that are explained in the manual, but also in python help, for example help(instr.McStas_instr.show_components).
         
             instr
             └── McStas_instr(str instr_name) # Returns McStas instrument object on initialize
                 ├── show_components(str category_name) # Show available components in given category
@@ -100,13 +107,20 @@
                 ├── set_mcrun_path(str path) # sets mcrun path
                 ├── set_mcstas_path(str path) # sets mcstas path
                 └── set_line_length(int length) # sets maximum line length
             
             plotter
             ├── make_plot(list McStasData) # Plots each data set individually
             └── make_sub_plot(list McStasData) # Plots data as subplot
+            
+            reader
+            └──  McStas_file(str filename) # Returns a reader that can extract information from given instr file
+        
+            InstrumentReader # returned by McStas_file
+            ├── generate_python_file(str filename) # Writes python file with information contaiend in isntrument
+            └── add_to_instr(McStas_instr Instr) # Adds information from instrument to McStasScirpt instrument
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `McStasScript-0.0.8/mcstasscript/data/data.py` & `McStasScript-0.0.9/mcstasscript/data/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,20 @@
         if "component" in self.info:
             self.component_name = self.info["component"].rstrip()
 
         # Extract filename
         if "filename" in self.info:
             self.filename = self.info["filename"].rstrip()
         else:
-            raise NameError(
-                "No filename found in mccode data section!")
+            # Monitors without output files does exist
+            #raise NameError(
+            #    "No filename found in mccode data section!")
+            print("The component named \"" + self.component_name
+                  + "\" had no data file and will not be loaded.")
+            self.filename = ""
 
         # Extract limits
         self.limits = []
         if "xylimits" in self.info:
             # find the four numbers
             temp_str = self.info["xylimits"]
             limits_string = temp_str.split()
```

### Comparing `McStasScript-0.0.8/mcstasscript/helper/component_reader.py` & `McStasScript-0.0.9/mcstasscript/helper/component_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -274,14 +274,16 @@
             # find definition parameters and their values
             if (self.line_starts_with(line.strip(), "DEFINITION PARAMETERS")
                     or self.line_starts_with(line.strip(),
                                              "SETTING PARAMETERS")):
 
                 parts = line.split("(")
                 parameter_parts = parts[1].split(",")
+                
+                parameter_parts = self.correct_for_brackets(parameter_parts)
 
                 parameter_parts = list(filter(("\n").__ne__, parameter_parts))
 
                 break_now = False
                 while True:
                     # Read all definition parameters
 
@@ -343,14 +345,15 @@
                             result.parameter_defaults[par_name] = par_value
                             result.parameter_types[par_name] = temp_par_type
 
                     if break_now:
                         break
 
                     parameter_parts = fo.readline().split(",")
+                    parameter_parts = self.correct_for_brackets(parameter_parts)
 
             if self.line_starts_with(line, "DECLARE"):
                 break
 
             if self.line_starts_with(line, "TRACE"):
                 break
 
@@ -365,14 +368,39 @@
 
         """
         To lower memory use one could remove all comments and units that
         does not correspond to a found parameter name.
         """
 
         return result
+    
+    def correct_for_brackets(self, parameter_parts):
+        corrected_parts = []
+        current_part = ""
+        index = 0
+        while True:
+            
+            current_part = parameter_parts[index]
+            inner_index = 0
+            while True: 
+                if (current_part.count("{") == current_part.count("}")):
+                    corrected_parts.append(current_part)
+                    index += inner_index
+                    break                          
+                else:
+                    inner_index +=1
+                    current_part += "," + parameter_parts[index+inner_index]
+
+            index += 1
+            
+            if index >= len(parameter_parts):
+                break
+            
+        return corrected_parts
+        
 
     def line_starts_with(self, line, string):
         """
         Helper method that checks if a string is the start of a line
 
         """
         if len(line) < len(string):
```

### Comparing `McStasScript-0.0.8/mcstasscript/helper/formatting.py` & `McStasScript-0.0.9/mcstasscript/helper/formatting.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/helper/managed_mcrun.py` & `McStasScript-0.0.9/mcstasscript/helper/managed_mcrun.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,15 +202,16 @@
             # Could read other details about run
 
             if lines == "end data\n":
                 # No more data for this metadata object
                 # Extract the information
                 current_object.extract_info()
                 # Add to metadata list
-                metadata_list.append(current_object)
+                if current_object.filename != "":
+                    metadata_list.append(current_object)
                 # Stop reading data
                 in_data = False
 
             if in_data:
                 # This line contains info to be added to metadata
                 colon_index = lines.index(":")
                 key = lines[2:colon_index]
```

### Comparing `McStasScript-0.0.8/mcstasscript/helper/mcstas_objects.py` & `McStasScript-0.0.9/mcstasscript/helper/mcstas_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,15 +120,16 @@
 
     Methods
     -------
     write_line(fo)
         Writes a line to text file fo declaring the parameter in c
     """
     def __init__(self, *args, **kwargs):
-        """Initializing mcstas parameter object
+        """
+        Initializing mcstas parameter object
 
         Parameters
         ----------
         Positional argument 1: type : str
             Type of the parameter, double, int or string
 
         Positional argument 2: name : str
@@ -144,15 +145,24 @@
 
             comment : str
                 sets comment displayed next to declaration
         """
         self.type = args[0]
         self.name = str(args[1])
 
-        if not is_legal_parameter(self.name):
+
+        par_name = self.name
+        if "*" in par_name[0]:
+            # Remove any number of prefixed *, indicating variable is a pointer
+            par_name = par_name.split("*")[-1]
+        elif "&" in par_name[0]:
+            # Remove the first & indicating the variable is an address
+            par_name = par_name[1:]
+            
+        if not is_legal_parameter(par_name):
             raise NameError("The given parameter name: \""
                             + self.name
                             + "\" is not a legal c variable name, "
                             + " and cannot be used in McStas.")
 
         self.value = ""
         if "value" in kwargs:
@@ -163,38 +173,52 @@
             self.vector = kwargs["array"]
 
         self.comment = ""
         if "comment" in kwargs:
             self.comment = " // " + kwargs["comment"]
 
     def write_line(self, fo):
-        """Writes line declaring variable to file fo
+        """
+        Writes line declaring variable to file fo
 
         Parameters
         ----------
         fo : file object
             File the line will be written to
         """
         if self.value is "" and self.vector == 0:
             fo.write("%s %s;%s" % (self.type, self.name, self.comment))
         if self.value is not "" and self.vector == 0:
             if self.type == "int":
                 fo.write("%s %s = %d;%s" % (self.type, self.name,
                                             self.value, self.comment))
             else:
-                fo.write("%s %s = %G;%s" % (self.type, self.name,
-                                            self.value, self.comment))
+                try:
+                    fo.write("%s %s = %G;%s" % (self.type, self.name,
+                                                self.value, self.comment))
+                except:
+                    fo.write("%s %s = %s;%s" % (self.type, self.name,
+                                                self.value, self.comment))
         if self.value is "" and self.vector != 0:
             fo.write("%s %s[%d];%s" % (self.type, self.name,
                                        self.vector, self.comment))
         if self.value is not "" and self.vector != 0:
-            fo.write("%s %s[%d] = {" % (self.type, self.name, self.vector))
-            for i in range(0, len(self.value) - 1):
-                fo.write("%G," % self.value[i])
-            fo.write("%G};%s" % (self.value[-1], self.comment))
+            if isinstance(self.value, str):
+                # value is a string
+                string = self.value
+                #string = string.replace('"',"\\\"")
+                fo.write("%s %s[%d] = %s;" % (self.type, self.name, self.vector, string))
+            else:
+                # list of values
+                fo.write("%s %s[%d] = {" % (self.type, self.name, self.vector))
+                for i in range(0, len(self.value) - 1):
+                    fo.write("%G," % self.value[i])
+                fo.write("%G};%s" % (self.value[-1], self.comment))
+                
+                
 
 
 class component:
     """
     A class describing a McStas component to be written to a instrument
 
     This class is used by the instrument class when setting up
@@ -351,77 +375,92 @@
 
         # Allow addition of attributes in init
         self._unfreeze()
 
         self.name = instance_name
         self.component_name = component_name
 
+        # initialize McStas information
+        self.AT_data = [0, 0, 0]
+        self.AT_relative = "ABSOLUTE"
+        self.ROTATED_specified = False
+        self.ROTATED_data = [0, 0, 0]
+        self.ROTATED_relative = "ABSOLUTE"
+        self.WHEN = ""
+        self.EXTEND = ""
+        self.GROUP = ""
+        self.JUMP = ""
+        self.SPLIT = 0
+        self.comment = ""
+        self.c_code_before = "" 
+        self.c_code_after = ""
+
+        # If any keywords are set in kwargs, update these
+        self.set_keyword_input(**kwargs)
+
+        """
+        Could store an option for whether this component should be
+        printed in instrument file or in a seperate file which would
+        then be included.
+        """
+
+        # Do not allow addition of attributes after init
+        self._freeze()
+    
+    def set_keyword_input(self, **kwargs):
+        # Allow addition of attributes in init
+        self._unfreeze()
+
         if "AT" in kwargs:
             self.AT_data = kwargs["AT"]
-        else:
-            self.AT_data = [0, 0, 0]
+        
         # Could check if AT_RELATIVE is a string
         if "AT_RELATIVE" in kwargs:
             self.AT_relative = "RELATIVE " + kwargs["AT_RELATIVE"]
-        else:
-            self.AT_relative = "ABSOLUTE"
 
+        self.ROTATED_specified = False
         if "ROTATED" in kwargs:
             self.ROTATED_data = kwargs["ROTATED"]
-        else:
-            self.ROTATED_data = [0, 0, 0]
+            self.ROTATED_specified = True
+
         # Could check if ROTATED_RELATIVE is a string
         if "ROTATED_RELATIVE" in kwargs:
             self.ROTATED_relative = "RELATIVE " + kwargs["ROTATED_RELATIVE"]
-        else:
-            self.ROTATED_relative = "ABSOLUTE"
+            self.ROTATED_specified = True
 
         # Could check if RELATIVE is a string
         if "RELATIVE" in kwargs:
             self.AT_relative = "RELATIVE " + kwargs["RELATIVE"]
             self.ROTATED_relative = "RELATIVE " + kwargs["RELATIVE"]
+            self.ROTATED_specified = True
 
         if "WHEN" in kwargs:
             self.WHEN = "WHEN (" + kwargs["WHEN"] + ")"
-        else:
-            self.WHEN = ""
 
         if "EXTEND" in kwargs:
             self.EXTEND = kwargs["EXTEND"] + "\n"
-        else:
-            self.EXTEND = ""
 
         if "GROUP" in kwargs:
             self.GROUP = kwargs["GROUP"]
-        else:
-            self.GROUP = ""
 
         if "JUMP" in kwargs:
             self.JUMP = kwargs["JUMP"]
-        else:
-            self.JUMP = ""
             
         if "SPLIT" in kwargs:
             self.SPLIT = kwargs["SPLIT"]
-        else:
-            self.SPLIT = 0
 
         if "comment" in kwargs:
             self.comment = kwargs["comment"]
-        else:
-            self.comment = ""
-
-        """
-        Could store an option for whether this component should be
-        printed in instrument file or in a seperate file which would
-        then be included.
-        """
-
-        # Do not allow addition of attributes after init
-        self._freeze()
+            
+        if "c_code_before" in kwargs:
+            self.c_code_before = kwargs["c_code_before"]
+        
+        if "c_code_after" in kwargs:
+            self.c_code_after = kwargs["c_code_after"]
+        
 
     def __setattr__(self, key, value):
         if self.__isfrozen and not hasattr(self, key):
             raise AttributeError("No parameter called '"
                                  + key
                                  + "' in component named "
                                  + self.name
@@ -445,14 +484,15 @@
                 self.AT_relative = relative_name
             else:
                 self.AT_relative = "RELATIVE " + relative_name
 
     def set_ROTATED(self, rotated_list, **kwargs):
         """Sets ROTATED data, List of 3 floats"""
         self.ROTATED_data = rotated_list
+        self.ROTATED_specified = True
         if "RELATIVE" in kwargs:
             relative_name = kwargs["RELATIVE"]
             if relative_name == "ABSOLUTE":
                 self.ROTATED_relative = relative_name
             else:
                 self.ROTATED_relative = "RELATIVE " + relative_name
 
@@ -505,27 +545,41 @@
     def append_EXTEND(self, string):
         """Appends a line of code to EXTEND block of component"""
         self.EXTEND = self.EXTEND + string + "\n"
 
     def set_comment(self, string):
         """Method that sets a comment to be written to instrument file"""
         self.comment = string
+        
+    def set_c_code_before(self, string):
+        """Method that sets c code to be written before the component"""
+        self.c_code_before = string
+        
+    def set_c_code_after(self, string):
+        """Method that sets c code to be written after the component"""
+        self.c_code_after = string
 
     def write_component(self, fo):
         """
         Method that writes component to file
 
         Relies on attributes added when McStas_Instr creates a subclass
         based on the component class.
 
         """
         parameters_per_line = 2
         # Could use character limit on lines instead
         parameters_written = 0  # internal parameter
 
+
+        if len(self.c_code_before) > 0:
+            explanation = "From component named " + self.name
+            fo.write("%s // %s\n" % (str(self.c_code_before), explanation))
+            fo.write("\n")
+
         # Write comment if present
         if len(self.comment) > 1:
             fo.write("// %s\n" % (str(self.comment)))
 
         if self.SPLIT is not 0:
             fo.write("SPLIT " + str(self.SPLIT) + " ") 
 
@@ -573,43 +627,52 @@
             fo.write("%s\n" % self.WHEN)
 
         # Write AT and ROTATED section
         fo.write("AT (%s,%s,%s)" % (str(self.AT_data[0]),
                                     str(self.AT_data[1]),
                                     str(self.AT_data[2])))
         fo.write(" %s\n" % self.AT_relative)
-        fo.write("ROTATED (%s,%s,%s)" % (str(self.ROTATED_data[0]),
-                                         str(self.ROTATED_data[1]),
-                                         str(self.ROTATED_data[2])))
-        fo.write(" %s\n" % self.ROTATED_relative)
+        
+        if self.ROTATED_specified:
+            fo.write("ROTATED (%s,%s,%s)" % (str(self.ROTATED_data[0]),
+                                             str(self.ROTATED_data[1]),
+                                             str(self.ROTATED_data[2])))
+            fo.write(" %s\n" % self.ROTATED_relative)
 
         if not self.GROUP == "":
             fo.write("GROUP %s\n" % self.GROUP)
 
         # Optional EXTEND section
         if not self.EXTEND == "":
             fo.write("EXTEND %{\n")
             fo.write("%s" % self.EXTEND)
             fo.write("%}\n")
 
         if not self.JUMP == "":
             fo.write("JUMP %s\n" % self.JUMP)
+            
+        if len(self.c_code_after) > 0:
+            fo.write("\n")
+            explanation = "From component named " + self.name
+            fo.write("%s // %s\n" % (str(self.c_code_after), explanation))
 
         # Leave a new line between components for readability
         fo.write("\n")
 
     def print_long(self):
         """
         Prints contained information to Python terminal
 
         Includes information on required parameters if they are not yet
         specified. Information on the components are added when the
         class is used as a superclass for classes describing each
         McStas component.
         """
+        if len(self.c_code_before) > 1:
+            print(self.c_code_before)
         if len(self.comment) > 1:
             print("// " + self.comment)
         if self.SPLIT is not 0:
             print("SPLIT " + str(self.SPLIT) + " ", end="")
         print("COMPONENT", str(self.name),
               "=", str(self.component_name))
         for key in self.parameter_names:
@@ -632,35 +695,43 @@
                           + bcolors.FAIL
                           + " : Required parameter not yet specified"
                           + bcolors.ENDC)
 
         if not self.WHEN == "":
             print(self.WHEN)
         print("AT", self.AT_data, self.AT_relative)
-        print("ROTATED", self.ROTATED_data, self.ROTATED_relative)
+        if self.ROTATED_specified:
+            print("ROTATED", self.ROTATED_data, self.ROTATED_relative)
         if not self.GROUP == "":
             print("GROUP " + self.GROUP)
         if not self.EXTEND == "":
             print("EXTEND %{")
             print(self.EXTEND + "%}")
         if not self.JUMP == "":
             print("JUMP " + self.JUMP)
+        if len(self.c_code_after) > 1:
+            print(self.c_code_after)
 
     def print_short(self, **kwargs):
         """Prints short description of component to list print"""
+        if self.ROTATED_specified:
+            print_rotate_rel = self.ROTATED_relative
+        else:
+            print_rotate_rel = self.AT_relative
+        
         if "longest_name" in kwargs:
             number_of_spaces = 3+kwargs["longest_name"]-len(self.name)
             print(str(self.name) + " "*number_of_spaces, end='')
             print(str(self.component_name),
                   "\tAT", self.AT_data, self.AT_relative,
-                  "ROTATED", self.ROTATED_data, self.ROTATED_relative)
+                  "ROTATED", self.ROTATED_data, print_rotate_rel)
         else:
             print(str(self.name), "=", str(self.component_name),
                   "\tAT", self.AT_data, self.AT_relative,
-                  "ROTATED", self.ROTATED_data, self.ROTATED_relative)
+                  "ROTATED", self.ROTATED_data, print_rotate_rel)
 
     def show_parameters(self, **kwargs):
         """
         Shows available parameters and their defaults for the component
 
         Any value specified is not reflected in this view. The
         additional attributes defined when McStas_Instr creates
```

### Comparing `McStasScript-0.0.8/mcstasscript/integration_tests/test_complex_instrument.py` & `McStasScript-0.0.9/mcstasscript/integration_tests/test_complex_instrument.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/integration_tests/test_simple_instrument.py` & `McStasScript-0.0.9/mcstasscript/integration_tests/test_simple_instrument.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/interface/functions.py` & `McStasScript-0.0.9/mcstasscript/interface/functions.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/interface/instr.py` & `McStasScript-0.0.9/mcstasscript/interface/instr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import print_function
 
 import os
 import datetime
 import yaml
 import subprocess
+import copy
 
 from mcstasscript.data.data import McStasData
 from mcstasscript.helper.mcstas_objects import declare_variable
 from mcstasscript.helper.mcstas_objects import parameter_variable
 from mcstasscript.helper.mcstas_objects import component
 from mcstasscript.helper.component_reader import ComponentReader
 from mcstasscript.helper.managed_mcrun import ManagedMcrun
@@ -57,15 +58,15 @@
         list of components in the instrument
 
     component_name_list : list of strings
         list of names of the components in the instrument
 
     Methods
     -------
-    add_parameter(*args,**kwargs)
+    add_parameter(*args, **kwargs)
         Adds input parameter to the define section
 
     add_declare_var()
         Adds declared variable ot the declare section
 
     append_initialize(string)
         Appends a string to the initialize section, then adds new line
@@ -81,51 +82,57 @@
 
     append_trace(string)
         Obsolete method, add components instead (used in write_c_files)
 
     show_components(string)
         Shows available components in given category
 
-    add_component(instance_name,component_name,**kwargs)
+    add_component(instance_name, component_name, **kwargs)
         Add a component to the instrument file
 
     get_component(instance_name)
         Returns component instance with name instance_name
 
     get_last_component()
         Returns component instance of last component
 
-    set_component_parameter(instance_name,dict)
+    set_component_parameter(instance_name, dict)
         Adds parameters as dict to component with instance_name
 
-    set_component_AT(instance_name,AT_data,**kwargs)
+    set_component_AT(instance_name, AT_data, **kwargs)
         Sets position of component named instance_name
 
-    set_component_ROTATED(instance_name,ROTATED_data,**kwargs)
+    set_component_ROTATED(instance_name, ROTATED_data, **kwargs)
         Sets rotation of component named instance_name
 
-    set_component_RELATIVE(instane_name,string)
+    set_component_RELATIVE(instane_name, string)
         Sets position and rotation reference for named component
 
-    set_component_WHEN(instance_name,string)
+    set_component_WHEN(instance_name, string)
         Sets WHEN condition of named component, is logical c expression
 
-    set_component_GROUP(instance_name,string)
+    set_component_GROUP(instance_name, string)
         Sets GROUP name of component named instance_name
 
-    append_component_EXTEND(instance_name,string)
+    append_component_EXTEND(instance_name, string)
         Appends a line to EXTEND section of named component
 
-    set_component_JUMP(instance_name,string)
+    set_component_JUMP(instance_name, string)
         Sets JUMP code for named component
 
-    set_component_SPLIT(instance_name,string)
+    set_component_SPLIT(instance_name, string)
         Sets SPLIT value for named component
-
-    set_component_comment(instance_name,string)
+        
+    set_component_c_code_before(instance_name, string)
+        Sets c code before the component
+        
+    set_component_c_code_after(instance_name, string)
+        Sets c code after the component
+        
+    set_component_comment(instance_name, string)
         Sets comment to be written before named component
 
     print_component(instance_name)
         Prints an overview of current state of named component
 
     print_component_short(instance_name)
         Prints short overview of current state of named component
@@ -209,14 +216,15 @@
             raise NameError("At this stage of development "
                             + "McStasScript need the absolute path "
                             + "for the McStas installation as keyword "
                             + "named mcstas_path or in configuration.yaml")
 
         self.parameter_list = []
         self.declare_list = []
+        #self.declare_section = ""
         self.initialize_section = ("// Start of initialize for generated "
                                    + name + "\n")
         self.trace_section = ("// Start of trace section for generated "
                               + name + "\n")
         self.finally_section = ("// Start of finally for generated "
                                 + name + "\n")
         # Handle components
@@ -357,28 +365,47 @@
 
             comment : str
                 Comment displayed next to declaration of parameter
 
         """
         # declare_variable class documented independently
         self.declare_list.append(declare_variable(*args, **kwargs))
+        
+    def append_declare(self, string):
+        """
+        Method for appending code to the declare section directly
+        
+        This method is not meant for declaring simple variables which
+        should be done using add_declare_var. This method can be used
+        to declare functions, structures and unions directly.
+        
+        Parameters
+        ----------
+        string : str
+            code to be added to declare section
+        """
+        
+        #self.declare_section = self.declare_section + string + "\n"
+        self.declare_list.append(string)
+        
 
     def append_initialize(self, string):
         """
         Method for appending code to the intialize section
 
         The intialize section consists of c code and will be compiled,
         thus any syntax errors will crash the simulation. Code is added
         on a new line for each call to this method.
 
         Parameters
         ----------
         string : str
             code to be added to initialize section
         """
+        
         self.initialize_section = self.initialize_section + string + "\n"
 
     def append_initialize_no_new_line(self, string):
         """
         Method for appending code to the intialize section, no new line
 
         The intialize section consists of c code and will be compiled,
@@ -645,14 +672,150 @@
         # If after or before keywords absent, place component at the end
         else:
             new_component = self._create_component_instance(*args, **kwargs)
             self.component_list.append(new_component)
             self.component_name_list.append(args[0])
 
         return new_component
+    
+    def copy_component(self, *args, **kwargs):
+        """
+        Method for adding a copy of a component instance to the instrument
+
+        Creates a copy of component instance in the instrument.  This
+        requires a unique instance name of the component to be used for
+        future reference and the name of the McStas component to be
+        used.  The component is placed at the end of the instrument file
+        unless otherwise specified with the after and before keywords.
+        The component may be initialized using other keyword arguments,
+        but all attributes can be set with approrpiate methods.
+
+        Parameters
+        ----------
+        First positional argument : str
+            Unique name of component instance
+
+        Second positional argument : str
+            Name of component instance to create copy of
+
+        Keyword arguments:
+            after : str
+                Place this component after component with given name
+
+            before : str
+                Place this component before component with given name
+
+            AT : List of 3 floats
+                Sets AT_data, position relative to reference
+
+            AT_RELATIVE : str
+                Sets reference component for postion
+
+            ROTATED : List of 3 floats
+                Sets ROTATED_data, rotation relative to reference
+
+            ROTATED_RELATIVE : str
+                Sets reference component for rotation
+
+            RELATIVE : str
+                Sets reference component for both position and rotation
+
+            WHEN : str
+                Sets when condition which must be a logical c expression
+
+            EXTEND : str
+                Initialize the extend section with a line of c code
+
+            GROUP : str
+                Name of the group this component should belong to
+
+            JUMP : str
+                Set code for McStas JUMP statement
+
+            comment : str
+                Comment that will be displayed before the component
+        """
+
+        # could also allow input of a component object        
+        
+        instance_name = args[0]
+        """
+        If the name starts with COPY, use unique naming as described in the
+        McStas manual.
+        """
+        if instance_name.startswith("COPY("):
+            target_name = instance_name.split("(", 1)[1]
+            target_name = target_name.split(")", 1)[0]
+            instance_name = target_name
+
+            label = 0
+            instance_name = target_name + "_" + str(label)
+            while instance_name in self.component_name_list:
+                instance_name = target_name + "_" + str(label)
+                label += 1
+
+        if instance_name in self.component_name_list:
+            raise NameError(("Component name \"" + str(args[0])
+                             + "\" used twice, McStas does not allow this."
+                             + " Rename or remove one instance of this"
+                             + " name."))
+        
+        if not args[1] in self.component_name_list:
+            raise NameError("Component name \"" + str(args[1])
+                            + "\" was not found in the McStas instrument."
+                            + " and thus can not be copied.")
+        else:
+            component_to_copy = self.get_component(args[1])
+        
+        # Insert component after component with this name
+        if "after" in kwargs:
+            if kwargs["after"] not in self.component_name_list:
+                raise NameError("Trying to add a component after a component"
+                                + " named \"" + str(kwargs["after"])
+                                + "\", but a component with that name was"
+                                + " not found.")
+
+            new_index = self.component_name_list.index(kwargs["after"])
+
+            new_component = copy.deepcopy(component_to_copy)
+            new_component.name = instance_name
+            self.component_list.insert(new_index+1, new_component)
+
+            self.component_name_list.insert(new_index+1, instance_name)
+
+        # Insert component after component with this name
+        elif "before" in kwargs:
+            if kwargs["before"] not in self.component_name_list:
+                raise NameError(("Trying to add a component before a "
+                                 + "component named \""
+                                 + str(kwargs["before"])
+                                 + "\", but a component with that "
+                                 + "name was not found."))
+
+            new_index = self.component_name_list.index(kwargs["before"])
+
+            new_component = copy.deepcopy(component_to_copy)
+            new_component.name = instance_name
+            self.component_list.insert(new_index, new_component)
+
+            self.component_name_list.insert(new_index, instance_name)
+
+        # If after or before keywords absent, place component at the end
+        else:
+            new_component = copy.deepcopy(component_to_copy)
+            new_component.name = instance_name
+            self.component_list.append(new_component)
+            self.component_name_list.append(instance_name)
+        
+        # Set the new name of the instance
+        new_component.name = instance_name
+        # Run set_keyword_input again for keyword arguments to take effect
+        new_component.set_keyword_input(**kwargs)
+
+        return new_component
 
     def get_component(self, name):
         """
         Get the component instance of component with specified name
 
         This method is used to get direct access to any component
         instance in the instrument.  The component instance can be
@@ -834,14 +997,46 @@
 
         SPLIT : int
             Sets SPLIT value for named McStas component
         """
 
         component = self.get_component(name)
         component.set_SPLIT(SPLIT)
+        
+    def set_component_c_code_before(self, name, code):
+        """
+        Method for setting c code before component
+
+        Parameters
+        ----------
+        name : str
+            Unique name of component to modify
+            
+        code : str
+            Code to be pasted before component
+        """
+
+        component = self.get_component(name)
+        component.set_c_code_before(code)
+        
+    def set_component_c_code_after(self, name, code):
+        """
+        Method for setting c code before component
+
+        Parameters
+        ----------
+        name : str
+            Unique name of component to modify
+        
+        code : str
+            Code to be pasted after component
+        """
+
+        component = self.get_component(name)
+        component.set_c_code_after(code)        
 
     def set_component_comment(self, name, string):
         """
         Sets a comment displayed before the component in written files
 
         Parameters
         ----------
@@ -1077,16 +1272,21 @@
             except OSError:
                 print("Creation of the directory %s failed" % path)
 
         fo = open("./generated_includes/" + self.name + "_declare.c", "w")
         fo.write("// declare section for %s \n" % self.name)
         fo.close()
         fo = open("./generated_includes/" + self.name + "_declare.c", "a")
+        #fo.write(self.declare_section)
         for dec_line in self.declare_list:
-            dec_line.write_line(fo)
+            if isinstance(dec_line, str):
+                # append declare section parts written here
+                fo.write(dec_line)
+            else:
+                dec_line.write_line(fo)
             fo.write("\n")
         fo.close()
 
         fo = open("./generated_includes/" + self.name + "_initialize.c", "w")
         fo.write(self.initialize_section)
         fo.close()
 
@@ -1150,16 +1350,21 @@
         if len(self.parameter_list) > 0:
             self.parameter_list[-1].write_parameter(fo, " ")
         fo.write(")\n")
         fo.write("\n")
 
         # Write declare
         fo.write("DECLARE \n%{\n")
+        #fo.write(self.declare_section)
         for dec_line in self.declare_list:
-            dec_line.write_line(fo)
+            if isinstance(dec_line, str):
+                # append declare section parts written here
+                fo.write(dec_line)
+            else:
+                dec_line.write_line(fo)
             fo.write("\n")
         fo.write("%}\n\n")
 
         # Write initialize
         fo.write("INITIALIZE \n%{\n")
         fo.write(self.initialize_section)
         # Alternatively hide everything in include
```

### Comparing `McStasScript-0.0.8/mcstasscript/interface/plotter.py` & `McStasScript-0.0.9/mcstasscript/interface/plotter.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/dummy_mcstas/misc/test_for_reading.comp` & `McStasScript-0.0.9/mcstasscript/tests/dummy_mcstas/misc/test_for_reading.comp`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_ComponentReader.py` & `McStasScript-0.0.9/mcstasscript/tests/test_ComponentReader.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_Configurator.py` & `McStasScript-0.0.9/mcstasscript/tests/test_Configurator.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_Instr.py` & `McStasScript-0.0.9/mcstasscript/tests/test_Instr.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,37 @@
 
     comp1 = instr.add_component("first_component", "test_for_reading")
     comp2 = instr.add_component("second_component", "test_for_reading")
     comp3 = instr.add_component("third_component", "test_for_reading")
 
     return instr
 
+def setup_populated_with_some_options_instr():
+    """
+    Sets up a instrument with some features used and two components
+    """
+    instr = setup_instr_root_path()
+
+    instr.add_parameter("double", "theta")
+    instr.add_parameter("double", "has_default", value=37)
+    instr.add_declare_var("double", "two_theta")
+    instr.append_initialize("two_theta = 2.0*theta;")
+
+    comp1 = instr.add_component("first_component", "test_for_reading")
+    comp1.set_AT([0,0,1])
+    comp1.set_GROUP("Starters")
+    comp2 = instr.add_component("second_component", "test_for_reading")
+    comp2.set_AT([0,0,2], RELATIVE="first_component")
+    comp2.set_ROTATED([0,30,0])
+    comp2.set_WHEN("1==1")
+    comp2.yheight=1.23
+    comp3 = instr.add_component("third_component", "test_for_reading")
+
+    return instr
+
 
 class TestMcStas_instr(unittest.TestCase):
     """
     Tests of the main class in McStasScript called McStas_instr.
     """
 
     def test_simple_initialize(self):
@@ -216,14 +239,50 @@
         """
         instr = setup_instr_root_path()
 
         instr.add_declare_var("double", "two_theta", comment="test par")
 
         self.assertEqual(instr.declare_list[0].name, "two_theta")
         self.assertEqual(instr.declare_list[0].comment, " // test par")
+        
+    def test_simple_append_declare(self):
+        """
+        The declare lines are held as a string. This method
+        appends that string.
+        """
+        instr = setup_instr_root_path()
+
+        instr.append_declare("First line of declare")
+        instr.append_declare("Second line of declare")
+        instr.append_declare("Third line of declare")
+
+        self.assertEqual(instr.declare_list[0],
+                         "First line of declare")
+        self.assertEqual(instr.declare_list[1], 
+                         "Second line of declare")
+        self.assertEqual(instr.declare_list[2], 
+                         "Third line of declare")
+        
+    def test_simple_append_declare_var_mix(self):
+        """
+        The declare lines are held as a string. This method
+        appends that string.
+        """
+        instr = setup_instr_root_path()
+
+        instr.append_declare("First line of declare")
+        instr.add_declare_var("double", "two_theta", comment="test par")
+        instr.append_declare("Third line of declare")
+
+        self.assertEqual(instr.declare_list[0],
+                         "First line of declare")
+        self.assertEqual(instr.declare_list[1].name, "two_theta")
+        self.assertEqual(instr.declare_list[1].comment, " // test par")
+        self.assertEqual(instr.declare_list[2], 
+                         "Third line of declare")        
 
     def test_simple_append_initialize(self):
         """
         The initialize section is held as a string. This method
         appends that string.
         """
         instr = setup_instr_root_path()
@@ -629,26 +688,69 @@
             comp = instr.add_component("test_component",
                                        "test_for_reading",
                                        before="non_exsistent_component")
 
     @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
     def test_add_component_simple_double_naming_error(self, mock_stdout):
         """
-        The add_component method adds a new component object to the
-        instrument and keeps track of its location within the
-        sequence of components.  Normally a new component is added to
-        the end of the sequence, but the before and after keywords can
-        be used to select another location. Here keyword passing is
-        tested.
+        This tests checks that an error occurs when giving the new
+        component a name which has already been used.
         """
 
         instr = setup_populated_instr()
 
         with self.assertRaises(NameError):
             comp = instr.add_component("first_component", "test_for_reading")
+            
+    @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
+    def test_copy_component_simple(self, mock_stdout):
+        """
+        Checks that a component can be copied
+        """
+
+        instr = setup_populated_with_some_options_instr()
+        
+        comp = instr.copy_component("copy_of_second_comp", "second_component")
+
+        self.assertEqual(comp.name, "copy_of_second_comp")
+        self.assertEqual(comp.yheight, 1.23)
+        self.assertEqual(comp.AT_data[0], 0)
+        self.assertEqual(comp.AT_data[1], 0)
+        self.assertEqual(comp.AT_data[2], 2)
+        
+    @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
+    def test_copy_component_keywords(self, mock_stdout):
+        """
+        Checks that a component can be copied and that keyword
+        arguments given under copy operation is sucessfully 
+        applied to the new component. A check is also made to 
+        ensure that the original component was not modified.
+        """
+
+        instr = setup_populated_with_some_options_instr()
+
+        comp = instr.copy_component("copy_of_second_comp", "second_component",
+                                    AT=[1,2,3], SPLIT=10)
+
+        self.assertEqual(comp.name, "copy_of_second_comp")
+        self.assertEqual(comp.yheight, 1.23)
+        self.assertEqual(comp.AT_data[0], 1)
+        self.assertEqual(comp.AT_data[1], 2)
+        self.assertEqual(comp.AT_data[2], 3)
+        self.assertEqual(comp.SPLIT, 10)
+        
+        # ensure original component was not changed
+        original = instr.get_component("second_component")
+        self.assertEqual(original.name, "second_component")
+        self.assertEqual(original.yheight, 1.23)
+        self.assertEqual(original.AT_data[0], 0)
+        self.assertEqual(original.AT_data[1], 0)
+        self.assertEqual(original.AT_data[2], 2)
+        self.assertEqual(original.SPLIT, 0)
+        
 
     @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
     def test_get_component_simple(self, mock_stdout):
         """
         get_component retrieves a component with a given name for
         easier manipulation.
         """
@@ -860,14 +962,44 @@
         instr = setup_populated_instr()
 
         instr.set_component_comment("second_component", "test comment")
 
         comp = instr.get_component("second_component")
 
         self.assertEqual(comp.comment, "test comment")
+        
+    @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
+    def test_set_c_code_before(self, mock_stdout):
+        """
+        set_component_c_code_before passes the argument to the similar
+        method in the component class.
+        """
+
+        instr = setup_populated_instr()
+
+        instr.set_component_c_code_before("second_component", "%include before.instr")
+
+        comp = instr.get_component("second_component")
+
+        self.assertEqual(comp.c_code_before, "%include before.instr")
+        
+    @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
+    def test_set_c_code_after(self, mock_stdout):
+        """
+        set_component_c_code_after passes the argument to the similar
+        method in the component class.
+        """
+
+        instr = setup_populated_instr()
+
+        instr.set_component_c_code_after("second_component", "%include after.instr")
+
+        comp = instr.get_component("second_component")
+
+        self.assertEqual(comp.c_code_after, "%include after.instr")
 
     @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
     def test_print_component(self, mock_stdout):
         """
         print_component calls the print_long method in the component
         class.
         """
@@ -897,15 +1029,16 @@
         par_name = bcolors.BOLD + "test_string" + bcolors.ENDC
         warning = (bcolors.FAIL
                    + " : Required parameter not yet specified"
                    + bcolors.ENDC)
         self.assertEqual(output[3], "  " + par_name + warning)
 
         self.assertEqual(output[4], "AT [0, 0, 0] ABSOLUTE")
-        self.assertEqual(output[5], "ROTATED [0, 0, 0] ABSOLUTE")
+        # Rotation not printed since it was never specified
+        #self.assertEqual(output[5], "ROTATED [0, 0, 0] ABSOLUTE")
 
     @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
     def test_print_component_short(self, mock_stdout):
         """
         print_component_short calls the print_short method in the
         component class.
         """
@@ -916,15 +1049,15 @@
 
         instr.print_component_short("second_component")
 
         output = mock_stdout.getvalue().split("\n")
 
         expected = ("second_component = test_for_reading "
                     + "\tAT [-1, 2, 3.4] RELATIVE home "
-                    + "ROTATED [0, 0, 0] ABSOLUTE")
+                    + "ROTATED [0, 0, 0] RELATIVE home")
 
         self.assertEqual(output[0], expected)
 
     @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
     def test_print_components_simple(self, mock_stdout):
         """
         print_components calls the print_short method in the component
@@ -1143,39 +1276,34 @@
         # right file. Can be improved by splitting the method into
         # several for easier testing. Acceptable since it is rarely
         # used.
         handle = mock_f()
         call = unittest.mock.call
         wrts = [
          call("// declare section for test_instrument \n"),
+         #call(""),
          call("double two_theta;"),
          call("\n"),
          call("// Start of initialize for generated test_instrument\n"
               + "two_theta = 2.0*theta;\n"),
          call("// Start of trace section for generated test_instrument\n"),
          call("COMPONENT first_component = test_for_reading("),
          call(")\n"),
          call("AT (0,0,0)"),
          call(" ABSOLUTE\n"),
-         call("ROTATED (0,0,0)"),
-         call(" ABSOLUTE\n"),
          call("\n"),
          call("COMPONENT second_component = test_for_reading("),
          call(")\n"),
          call("AT (0,0,0)"),
          call(" ABSOLUTE\n"),
-         call("ROTATED (0,0,0)"),
-         call(" ABSOLUTE\n"),
          call("\n"),
          call("COMPONENT third_component = test_for_reading("),
          call(")\n"),
          call("AT (0,0,0)"),
          call(" ABSOLUTE\n"),
-         call("ROTATED (0,0,0)"),
-         call(" ABSOLUTE\n"),
          call("\n")]
 
         handle.write.assert_has_calls(wrts, any_order=False)
 
     @unittest.mock.patch("sys.stdout", new_callable=io.StringIO)
     @unittest.mock.patch('__main__.__builtins__.open',
                          new_callable=unittest.mock.mock_open)
@@ -1234,42 +1362,37 @@
          my_call(" = 37"),
          my_call(" "),
          my_call(""),
          my_call("\n"),
          my_call(")\n"),
          my_call("\n"),
          my_call("DECLARE \n%{\n"),
+         #my_call(""),
          my_call("double two_theta;"),
          my_call("\n"),
          my_call("%}\n\n"),
          my_call("INITIALIZE \n%{\n"),
          my_call("// Start of initialize for generated test_instrument\n"
                  + "two_theta = 2.0*theta;\n"),
          my_call("%}\n\n"),
          my_call("TRACE \n"),
          my_call("COMPONENT first_component = test_for_reading("),
          my_call(")\n"),
          my_call("AT (0,0,0)"),
          my_call(" ABSOLUTE\n"),
-         my_call("ROTATED (0,0,0)"),
-         my_call(" ABSOLUTE\n"),
          my_call("\n"),
          my_call("COMPONENT second_component = test_for_reading("),
          my_call(")\n"),
          my_call("AT (0,0,0)"),
          my_call(" ABSOLUTE\n"),
-         my_call("ROTATED (0,0,0)"),
-         my_call(" ABSOLUTE\n"),
          my_call("\n"),
          my_call("COMPONENT third_component = test_for_reading("),
          my_call(")\n"),
          my_call("AT (0,0,0)"),
          my_call(" ABSOLUTE\n"),
-         my_call("ROTATED (0,0,0)"),
-         my_call(" ABSOLUTE\n"),
          my_call("\n"),
          my_call("FINALLY \n%{\n"),
          my_call("// Start of finally for generated test_instrument\n"),
          my_call("%}\n"),
          my_call("\nEND\n")]
 
         mock_f.assert_called_with("test_instrument.instr", "w")
```

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_ManagedMcrun.py` & `McStasScript-0.0.9/mcstasscript/tests/test_ManagedMcrun.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_McStasData.py` & `McStasScript-0.0.9/mcstasscript/tests/test_McStasData.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_McStasMetaData.py` & `McStasScript-0.0.9/mcstasscript/tests/test_McStasMetaData.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_McStasPlotOptions.py` & `McStasScript-0.0.9/mcstasscript/tests/test_McStasPlotOptions.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_component.py` & `McStasScript-0.0.9/mcstasscript/tests/test_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -349,23 +349,62 @@
         with mock_f('test.txt', 'w') as m_fo:
             comp.write_component(m_fo)
 
         my_call = unittest.mock.call
         expected_writes = [my_call("COMPONENT test_component = Arm("),
                            my_call(")\n"),
                            my_call("AT (0,0,0)"),
-                           my_call(" ABSOLUTE\n"),
-                           my_call("ROTATED (0,0,0)"),
                            my_call(" ABSOLUTE\n")]
 
         mock_f.assert_called_with('test.txt', 'w')
         handle = mock_f()
         handle.write.assert_has_calls(expected_writes, any_order=False)
 
     @unittest.mock.patch('__main__.__builtins__.open',
+                         new_callable=unittest.mock.mock_open)    
+    def test_component_write_to_file_include(self, mock_f):
+        """
+        Testing that a component can be written to file with the
+        expected output. Here with simple input.
+        """
+
+        comp = component("test_component", "Arm",
+                         c_code_before="%include \"test.instr\"")
+        
+        comp.set_c_code_after("%include \"after.instr\"")
+        
+        comp._unfreeze()
+        # Need to set up attribute parameters
+        # Also need to categorize them as when created
+        comp.parameter_names = []
+        comp.parameter_defaults = {}
+        comp.parameter_types = {}
+        comp._freeze()
+
+        with mock_f('test.txt', 'w') as m_fo:
+            comp.write_component(m_fo)
+
+        my_call = unittest.mock.call
+        expected_writes = [my_call("%include \"test.instr\" // From"
+                                   + " component named test_component\n"),
+                           my_call("\n"),
+                           my_call("COMPONENT test_component = Arm("),
+                           my_call(")\n"),
+                           my_call("AT (0,0,0)"),
+                           my_call(" ABSOLUTE\n"),
+                           my_call("\n"),
+                           my_call("%include \"after.instr\" // From"
+                                   + " component named test_component\n"),
+                           my_call("\n")]
+
+        mock_f.assert_called_with('test.txt', 'w')
+        handle = mock_f()
+        handle.write.assert_has_calls(expected_writes, any_order=False)
+
+    @unittest.mock.patch('__main__.__builtins__.open',
                          new_callable=unittest.mock.mock_open)
     def test_component_write_to_file_complex(self, mock_f):
         """
         Testing that a component can be written to file with the
         expected output. Here with complex input.
         """
```

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_data_set/L_mon.dat` & `McStasScript-0.0.9/mcstasscript/tests/test_data_set/L_mon.dat`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_data_set/PSD.dat` & `McStasScript-0.0.9/mcstasscript/tests/test_data_set/PSD.dat`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_data_set/PSD_4PI.dat` & `McStasScript-0.0.9/mcstasscript/tests/test_data_set/PSD_4PI.dat`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_data_set/jupyter_demo.instr` & `McStasScript-0.0.9/mcstasscript/tests/test_data_set/jupyter_demo.instr`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_data_set/mccode.sim` & `McStasScript-0.0.9/mcstasscript/tests/test_data_set/mccode.sim`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_declare_variable.py` & `McStasScript-0.0.9/mcstasscript/tests/test_declare_variable.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_for_reading.comp` & `McStasScript-0.0.9/mcstasscript/tests/test_for_reading.comp`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_formatting.py` & `McStasScript-0.0.9/mcstasscript/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_functions.py` & `McStasScript-0.0.9/mcstasscript/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/mcstasscript/tests/test_parameter_variable.py` & `McStasScript-0.0.9/mcstasscript/tests/test_parameter_variable.py`

 * *Files identical despite different names*

### Comparing `McStasScript-0.0.8/setup.py` & `McStasScript-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='McStasScript',
-     version='0.0.8',
+     version='0.0.9',
      author="Mads Bertelsen",
      author_email="Mads.Bertelsen@esss.se",
      description="A python scripting interface for McStas",
      include_package_data=True,
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/PaNOSC-ViNYL/McStasScript",
```

