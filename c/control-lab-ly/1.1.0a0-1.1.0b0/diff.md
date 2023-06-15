# Comparing `tmp/control-lab-ly-1.1.0a0.tar.gz` & `tmp/control-lab-ly-1.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.1.0a0.tar", last modified: Mon May 15 14:04:14 2023, max compression
+gzip compressed data, was "control-lab-ly-1.1.0b0.tar", last modified: Thu Jun 15 05:55:53 2023, max compression
```

## Comparing `control-lab-ly-1.1.0a0.tar` & `control-lab-ly-1.1.0b0.tar`

### file list

```diff
@@ -1,228 +1,221 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.378557 control-lab-ly-1.1.0a0/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0a0/LICENSE.md
--rw-rw-rw-   0        0        0       17 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/MANIFEST.in
--rw-rw-rw-   0        0        0    18871 2023-05-15 14:04:14.380947 control-lab-ly-1.1.0a0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.151796 control-lab-ly-1.1.0a0/docs/
--rw-rw-rw-   0        0        0     5644 2023-05-15 13:59:45.000000 control-lab-ly-1.1.0a0/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.0a0/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0a0/docs/LICENSE.md
--rw-rw-rw-   0        0        0    12109 2023-04-21 06:54:10.000000 control-lab-ly-1.1.0a0/docs/README.md
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/pyproject.toml
--rw-rw-rw-   0        0        0     1559 2023-05-15 14:04:14.401059 control-lab-ly-1.1.0a0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.0a0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:11.791488 control-lab-ly-1.1.0a0/src/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.205931 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    18871 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7781 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-15 14:04:11.000000 control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.221443 control-lab-ly-1.1.0a0/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.225133 control-lab-ly-1.1.0a0/src/controllably/Analyse/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.233432 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.260868 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Database/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Database/__init__.py
--rw-rw-rw-   0        0        0     3029 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Database/database_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.297495 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/
--rw-rw-rw-   0        0        0      277 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/__init__.py
--rw-rw-rw-   0        0        0     6448 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/circuit_datatype.py
--rw-rw-rw-   0        0        0    26583 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/eis_datatype.py
--rw-rw-rw-   0        0        0      956 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
--rw-rw-rw-   0        0        0     1585 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/Types/eis_tests.json
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.319968 control-lab-ly-1.1.0a0/src/controllably/Analyse/Visualisation/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Visualisation/__init__.py
--rw-rw-rw-   0        0        0      830 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/Visualisation/visualisation_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Analyse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.366749 control-lab-ly-1.1.0a0/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.389946 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.409910 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    17622 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8151 2023-04-21 07:30:47.000000 control-lab-ly-1.1.0a0/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.419711 control-lab-ly-1.1.0a0/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.511823 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/
--rw-rw-rw-   0        0        0      658 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0     5544 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/compound_panel.py
--rw-rw-rw-   0        0        0    17966 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0     8757 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/liquid_panel.py
--rw-rw-rw-   0        0        0      886 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/loader_panel.py
--rw-rw-rw-   0        0        0     7373 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/measurer_panel.py
--rw-rw-rw-   0        0        0    15419 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/mover_panel.py
--rw-rw-rw-   0        0        0     3775 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Control/GUI/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.527946 control-lab-ly-1.1.0a0/src/controllably/Control/Schedule/
--rw-rw-rw-   0        0        0      147 2023-04-11 14:01:57.000000 control-lab-ly-1.1.0a0/src/controllably/Control/Schedule/__init__.py
--rw-rw-rw-   0        0        0     1868 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Control/Schedule/schedule_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.583054 control-lab-ly-1.1.0a0/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.590031 control-lab-ly-1.1.0a0/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    10712 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.602987 control-lab-ly-1.1.0a0/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9118 2023-05-12 05:43:18.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.612265 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.641242 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/
--rw-rw-rw-   0        0        0      252 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/__init__.py
--rw-rw-rw-   0        0        0    23118 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.730314 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
--rw-rw-rw-   0        0        0      171 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
--rw-rw-rw-   0        0        0    37208 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
--rw-rw-rw-   0        0        0     4984 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.767908 control-lab-ly-1.1.0a0/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0     9684 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     3989 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.902347 control-lab-ly-1.1.0a0/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.924529 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:12.976210 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      314 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18014 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7492 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     2102 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.005819 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      401 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10256 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.023228 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.059844 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      334 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10345 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2093 2023-05-12 05:43:18.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.071087 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      350 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3973 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.084284 control-lab-ly-1.1.0a0/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     8427 2023-05-05 09:28:56.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0      535 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5398 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    13804 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4176 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.118283 control-lab-ly-1.1.0a0/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.167233 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9049 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3450 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     2853 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.187296 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.234375 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.262286 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24280 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15883 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7030 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10507 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32152 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.317381 control-lab-ly-1.1.0a0/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.357489 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.385737 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.425074 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3440 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29862 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     9064 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.467891 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     3210 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    31585 2023-05-15 13:59:45.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13191 2023-05-04 14:14:48.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14619 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.485042 control-lab-ly-1.1.0a0/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.509326 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.562012 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      348 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     9316 2023-05-15 13:59:45.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.635650 control-lab-ly-1.1.0a0/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.691292 control-lab-ly-1.1.0a0/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.707631 control-lab-ly-1.1.0a0/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.749564 control-lab-ly-1.1.0a0/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0a0/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.814548 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.825322 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.890281 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:13.915566 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2983 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      310 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0a0/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15591 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0a0/src/controllably/View/image_utils.py
--rw-rw-rw-   0        0        0    15865 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0a0/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0       98 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.000324 control-lab-ly-1.1.0a0/src/controllably/misc/
--rw-rw-rw-   0        0        0      586 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0    10014 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     6559 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17440 2023-04-21 07:30:47.000000 control-lab-ly-1.1.0a0/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2867 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4576 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.017274 control-lab-ly-1.1.0a0/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.034992 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.063944 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.094843 control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-05-15 14:04:14.372578 control-lab-ly-1.1.0a0/tests/
--rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0a0/tests/test_camera_optical.py
--rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_camera_thermal.py
--rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_cartesian_ender.py
--rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_cartesian_primitiv.py
--rw-rw-rw-   0        0        0      629 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/tests/test_compound_liquidmover.py
--rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_compound_spin_printer.py
--rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_dobot_m1pro.py
--rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_dobot_mg400.py
--rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_electrical_keithley.py
--rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_film_spin.py
--rw-rw-rw-   0        0        0      586 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/tests/test_heat_peltier.py
--rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_light_led_array.py
--rw-rw-rw-   0        0        0      390 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0a0/tests/test_liquid_sartorius.py
--rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_liquid_syringe_assembly.py
--rw-rw-rw-   0        0        0      538 2023-05-04 09:11:29.000000 control-lab-ly-1.1.0a0/tests/test_liquid_tricontinent.py
--rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_mechanical_piezorobotics.py
--rw-rw-rw-   0        0        0     1011 2023-05-15 13:59:31.000000 control-lab-ly-1.1.0a0/tests/test_mixture_shaker.py
--rw-rw-rw-   0        0        0     1020 2023-05-09 08:54:35.000000 control-lab-ly-1.1.0a0/tests/test_panels.py
--rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_physical_balance.py
--rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0a0/tests/test_pump_peristaltic.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.574456 control-lab-ly-1.1.0b0/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0b0/LICENSE.md
+-rw-rw-rw-   0        0        0       44 2023-06-15 05:55:28.000000 control-lab-ly-1.1.0b0/MANIFEST.in
+-rw-rw-rw-   0        0        0    20718 2023-06-15 05:55:53.574456 control-lab-ly-1.1.0b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.242181 control-lab-ly-1.1.0b0/docs/
+-rw-rw-rw-   0        0        0     6576 2023-06-15 05:47:20.000000 control-lab-ly-1.1.0b0/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.0b0/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0b0/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    13024 2023-06-15 02:35:45.000000 control-lab-ly-1.1.0b0/docs/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.250795 control-lab-ly-1.1.0b0/docs/assets/
+-rw-rw-rw-   0        0        0   203629 2023-06-15 02:22:15.000000 control-lab-ly-1.1.0b0/docs/assets/Documentation guide.png
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/pyproject.toml
+-rw-rw-rw-   0        0        0     1500 2023-06-15 05:55:53.574456 control-lab-ly-1.1.0b0/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:51.925283 control-lab-ly-1.1.0b0/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.292330 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    20718 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7587 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.309630 control-lab-ly-1.1.0b0/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.326989 control-lab-ly-1.1.0b0/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.343958 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.361685 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    17618 2023-06-07 08:08:37.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8197 2023-06-07 15:06:53.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.378265 control-lab-ly-1.1.0b0/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.419000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.472031 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/
+-rw-rw-rw-   0        0        0      569 2023-06-07 07:31:49.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/__init__.py
+-rw-rw-rw-   0        0        0     7129 2023-06-07 08:09:06.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/maker_panel.py
+-rw-rw-rw-   0        0        0     7976 2023-06-09 02:26:55.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/measurer_panel.py
+-rw-rw-rw-   0        0        0    16355 2023-06-09 02:26:45.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/mover_panel.py
+-rw-rw-rw-   0        0        0     8767 2023-06-07 07:59:03.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
+-rw-rw-rw-   0        0        0     3780 2023-06-07 08:09:39.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.515458 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/
+-rw-rw-rw-   0        0        0      406 2023-06-07 07:37:47.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/__init__.py
+-rw-rw-rw-   0        0        0      888 2023-06-07 07:29:39.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/loader_panel.py
+-rw-rw-rw-   0        0        0     8681 2023-06-07 15:28:23.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/pop_ups.py
+-rw-rw-rw-   0        0        0     4573 2023-06-07 15:28:30.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/templates.py
+-rw-rw-rw-   0        0        0      519 2023-06-07 15:50:08.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0     5544 2023-06-07 08:08:44.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/compound_panel.py
+-rw-rw-rw-   0        0        0    16264 2023-06-07 08:08:56.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0    14530 2023-06-15 02:18:22.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/guide_panel.py
+-rw-rw-rw-   0        0        0     3481 2023-06-07 07:35:28.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/multichannel_panel.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.1.0b0/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.546239 control-lab-ly-1.1.0b0/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.577289 control-lab-ly-1.1.0b0/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    11244 2023-06-07 08:09:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.626845 control-lab-ly-1.1.0b0/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9882 2023-06-07 08:09:54.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.634274 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.648457 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/
+-rw-rw-rw-   0        0        0      252 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/__init__.py
+-rw-rw-rw-   0        0        0    27552 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.709617 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
+-rw-rw-rw-   0        0        0      171 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
+-rw-rw-rw-   0        0        0    37854 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
+-rw-rw-rw-   0        0        0     4984 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.725629 control-lab-ly-1.1.0b0/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0    10777 2023-06-07 08:10:11.000000 control-lab-ly-1.1.0b0/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b0/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.746436 control-lab-ly-1.1.0b0/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.760623 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.784503 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      314 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18010 2023-06-07 08:10:41.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7484 2023-06-07 08:10:49.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     1993 2023-06-07 08:10:55.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.807068 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      287 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10637 2023-06-07 15:30:15.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.815712 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.881116 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      334 2023-05-18 08:27:22.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10341 2023-06-07 08:11:13.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3159 2023-06-07 08:11:18.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2012 2023-06-07 08:11:22.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.900436 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      236 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3534 2023-06-07 08:11:26.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.917099 control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     8358 2023-06-07 08:11:32.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0     8199 2023-06-07 08:11:37.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/force_sensor_utils.py
+-rw-rw-rw-   0        0        0      535 2023-06-06 08:07:20.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5437 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    14062 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4180 2023-06-07 08:10:29.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.927685 control-lab-ly-1.1.0b0/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.945665 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9077 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3450 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     2852 2023-06-06 07:14:55.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.962232 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.986737 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.010543 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24280 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15776 2023-06-07 08:12:14.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7128 2023-06-15 03:26:52.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10566 2023-06-07 08:12:11.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32385 2023-06-05 18:48:48.000000 control-lab-ly-1.1.0b0/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.028178 control-lab-ly-1.1.0b0/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.052652 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.077054 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.109936 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3440 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29858 2023-06-07 08:12:55.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     7672 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.126250 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    31695 2023-06-07 15:33:06.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13230 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14600 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.134466 control-lab-ly-1.1.0b0/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.152260 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.168316 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      397 2023-06-07 02:20:21.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8844 2023-06-07 08:13:13.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.184342 control-lab-ly-1.1.0b0/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.193029 control-lab-ly-1.1.0b0/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-06-08 02:41:36.000000 control-lab-ly-1.1.0b0/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.201058 control-lab-ly-1.1.0b0/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.209053 control-lab-ly-1.1.0b0/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.225709 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.225709 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:04:15.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.260043 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.276352 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2988 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      304 2023-06-08 02:41:32.000000 control-lab-ly-1.1.0b0/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15703 2023-06-07 14:50:19.000000 control-lab-ly-1.1.0b0/src/controllably/View/image.py
+-rw-rw-rw-   0        0        0    15898 2023-06-08 02:41:35.000000 control-lab-ly-1.1.0b0/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0      131 2023-06-05 18:11:26.000000 control-lab-ly-1.1.0b0/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.334847 control-lab-ly-1.1.0b0/src/controllably/misc/
+-rw-rw-rw-   0        0        0      627 2023-06-07 15:16:27.000000 control-lab-ly-1.1.0b0/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0     9596 2023-06-09 02:42:47.000000 control-lab-ly-1.1.0b0/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     7940 2023-06-13 09:57:18.000000 control-lab-ly-1.1.0b0/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17547 2023-06-07 14:53:56.000000 control-lab-ly-1.1.0b0/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2863 2023-06-07 08:11:52.000000 control-lab-ly-1.1.0b0/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4543 2023-06-14 09:42:31.000000 control-lab-ly-1.1.0b0/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.343783 control-lab-ly-1.1.0b0/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.368664 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.384661 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.417857 control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.566458 control-lab-ly-1.1.0b0/tests/
+-rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0b0/tests/test_camera_optical.py
+-rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_camera_thermal.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_cartesian_ender.py
+-rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_cartesian_primitiv.py
+-rw-rw-rw-   0        0        0      629 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0b0/tests/test_compound_liquidmover.py
+-rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_compound_spin_printer.py
+-rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_dobot_m1pro.py
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_dobot_mg400.py
+-rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_electrical_keithley.py
+-rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_film_spin.py
+-rw-rw-rw-   0        0        0      586 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/tests/test_heat_peltier.py
+-rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_light_led_array.py
+-rw-rw-rw-   0        0        0      390 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0b0/tests/test_liquid_sartorius.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_liquid_syringe_assembly.py
+-rw-rw-rw-   0        0        0      538 2023-05-04 09:11:29.000000 control-lab-ly-1.1.0b0/tests/test_liquid_tricontinent.py
+-rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_mechanical_piezorobotics.py
+-rw-rw-rw-   0        0        0     1011 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/tests/test_mixture_shaker.py
+-rw-rw-rw-   0        0        0     2365 2023-06-15 02:45:10.000000 control-lab-ly-1.1.0b0/tests/test_panels.py
+-rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_physical_balance.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-1.1.0a0/LICENSE.md` & `control-lab-ly-1.1.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/PKG-INFO` & `control-lab-ly-1.1.0b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.0a0
+Version: 1.1.0b0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -26,31 +26,32 @@
 # Control.lab.ly
 Lab Equipment Automation Package
 
 ## Description
 User-friendly package that enables flexible automation an reconfigurable setups for high-throughput experimentation and machine learning.
 
 ## Package Structure
-1. Analyse
-2. Compound
-3. Control
-4. Make
-5. Measure
-6. Move
-7. Transfer
-8. View
+1. Compound
+2. Control
+3. Make
+4. Measure
+5. Move
+6. Transfer
+7. View
 
 ## Device support
 - Make
+  - (QInstruments) Bioshake Orbital Shaker
   - Multi-channel LED array \[Arduino\]
   - Multi-channel spin-coater \[Arduino\]
   - Peltier device \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
+  - (Sentron) SI series pH meters - *full functionality in development*
   - Precision mass balance \[Arduino\]
 - Move
   - (Creality) Ender-3
   - (Dobot) M1 Pro
   - (Dobot) MG400
   - Primitiv \[Arduino\]
 - Transfer
@@ -59,276 +60,289 @@
   - (TriContinent) C Series syringe pumps
   - Peristaltic pump and syringe system \[Arduino\]
 - View
   - (FLIR) AX8 thermal imaging camera - *full functionality in development*
   - Web cameras \[General\]
 
 ## Installation
-Control.lab.ly can be found on PyPI and can be installed easily with `pip install`.
+Control.lab.ly can be found on PyPI and can be easily installed with `pip install`.
 ```shell
 $ pip install control-lab-ly
 ```
 
 ## Basic Usage
 Simple start-up guide for basic usage of the package.
 
 ### Import desired class
 ```python
 from controllably.Move.Cartesian import Ender
 mover = Ender(...)
 mover.safeMoveTo((x,y,z))
 ```
 
-More details for each class / module / package can be explored by using the `help` function.
+### View documentation
+Use the built-in guide to read the documentation for the package.
 ```python
-help(controllably.Move)   # help on package
-help(Ender)               # help on class
-help(mover)               # help on instance/object
+from controllably import guide_me
+guide_me()
 ```
+![Screenshot of the documentation guide](./assets/Documentation%20guide.png)
 
-Alternatively, you can use the native `pydoc` documentation generator.
-```shell
-$ python -m pydoc controllably.Move
-```
-
->Tip: when using Interactive Python (IPython) (e.g. Jupyter notebooks), add a exclamation mark (`!`) in front of the shell command
+Alternatively, details for each class / module / package can be explored by using the `help` function.
 ```python
->>> !python -m pydoc controllably.Move
->>> !python -m pydoc -b   # Generates a static HTML site to browse package documentation
+help(Ender)
 ```
-For basic usage, this is all you need to know. Check the documentation for more details on each respective class.
+
+For basic usage, this is all you need to know. Check the documentation for more details on each class and function.
 
 ---
 
 ## Advanced Usage
-For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation.
+For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation. This includes setting up configuration files and adding plugin drivers.
 
-### 0. Import package
-The convention is to import Control-lab-ly as `lab`.
+### Import package
 ```python
 import controllably as lab
 ```
 
-### Contents
-1. Projects
-2. Setups
-3. Decks
-4. Safety measures
-5. Plugins
-
-### 1. Creating a new project
-Create a `/configs` folder in the base folder of your project repository to store all configuration related files from which the package will read from.\
-This only has to be done once when you first set up the project folder.
-```python
-lab.create_configs()
-```
-
-A different address may be used by different machines for the same device. To manage the different addresses used by different machines, you first need your machine's unique identifier.
+Optionally, you can set the safety policy for the session. This feature allows the user to prevent collisions before each movement is made. The safety policy has to be assigned before importing any of the `Mover` objects.
 ```python
-# Get your machine's ID
-print(lab.Helper.get_node())
-```
+lab.set_safety('high')  # Notifies; Pauses for input before every move action
+lab.set_safety('low')   # Notifies; Waits for countdown before every move action
+lab.set_safety(None)    # Movement actions carry out without delay
 
-A template of `registry.yaml` has also been added to the folder to hold the machine-specific addresses of your connected devices (i.e. COM ports).\
-Populate the YAML file in the format shown below.
-```yaml
-### registry.yaml ###
-'012345678901234':          # insert your machine's 15-digit ID here (from the above step)
-    cam_index:              # camera index of the connected imaging devices
-      __cam_01__: 1         # keep the leading and trailing double underscores
-      __cam_02__: 0
-    port:                   # addresses of serial COM ports
-      __device_01__: COM3   # keep the leading and trailing double underscores
-      __device_02__: COM16
+# Import control-lab-ly classes only after setting the safety policy
 ```
 
-To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use:
-```python
-lab.Helper.get_ports()
-```
+### Contents
+1. [Setups](#1-creating-a-new-setup)
+2. [Decks](#2-managing-a-deck)
+3. [Addresses](#3-managing-project-addresses)
+4. [Plugins](#4-using-plugins)
 
-### 2. Creating a new setup
-Create a new folder for the configuration files of your new setup. If you had skipped the previous step of creating a project, calling `lab.create_setup()` will also generate the required file structure. However, be sure to populate your machine ID and device addresses in the `registry.yaml` file.
 
+### 1. Creating a new setup
+Create a `/configs/MySetup` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
 ```python
-lab.create_setup(setup_name = "_Setup01_")
-# replace "_Setup01_" with the desired name for your setup
+lab.create_setup(setup_name = "MySetup")
 ```
-This creates a `/_Setup01_` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
 
-#### 2.1 `config.yaml`
-Configuration and calibration values for your devices is stored in `config.yaml`.\
-Each configuration starts with the `name` of your device, then its `module`, `class`, and `settings`.
+#### 1.1 `config.yaml`
+This file stores the configuration and calibration values for your devices.
 ```yaml
-_Device01_:                                     # name of simple device (user-defined)
-  module: _module_name_01_                      # device module
-  class: _submodule_1A_._class_1A_              # device class
+MyDevice:                                       # device name
+  module: Move                                  # top-level category
+  class: Cartesian.Ender                        # device class
   settings:
-    port: __device_01__                         # port addresses defined in registry.yaml
-    _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
-    _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
-```
+    port: COM1                                  # serial port address
+    setting_A: {'tuple': [300,0,200]}           # use keys to define the type of iterable
+    setting_B: {'array': [[0,1,0],[-1,0,0]]}    # only tuple and np.array supported
+```
+> Each device configuration starts with the device name, then the following parameters:\
+> `module`: top-level category (such as Make, Measure, Move,Transfer, View)\
+> `class`: point to specific subclass using dot notation\
+> `settings`: various initialisation settings\
+> *See the* [**guide**](#view-documentation) *for more details on these parameters*
 
-`Compound` devices are similarly configured. The configuration values for its component devices are defined under the `component_config` setting. The structure of the configuration values for the component devices are similar to that shown above, except indented to fall under the indentation of the `component_config` setting.
+Compound devices are similarly configured. 
 ```yaml
-_Device02_:                                 # name of 'Compound' device (user-defined)
-  module: Compound                            
-  class: _submodule_2A_._class_2A_
-  settings:
-    _setting_C_: 1                          # other settings for your 'Compound' device
-    component_config:                       # nest component configuration settings here
-      _Component01_:                        # name of component
-        module: _module_name_03_
-        class: _submodule_3A_._class_3A_
-        settings:
-          ip_address: '192.0.0.1'           # IP addresses do not vary between machines
-      _Component02_: 
-        module: _module_name_04_
-        class: _submodule_4A_._class_4A_
-        settings:
-          _setting_D_: 2                    # settings for your component device
+MyCompoundDevice:                         # compound device name
+  module: Compound
+  class: LiquidMover.LiquidMoverSetup
+  settings:                               # settings for your compound device
+    setting_C: True
+    component_config:                     # nest component configuration settings here
+      MyFirstDevice:                      # component device name
+        module: Transfer
+        class: Liquid.SyringeAssembly
+        settings:                         # settings for your component device
+          port: COM22
+          setting_D: 2                    
+      MySecondDevice:                     # component device name
+        module: Mover
+        class: Jointed.Dobot.M1Pro
+        settings:                         # settings for your compound device
+          ip_address: '192.0.0.1'
 ```
+> The configuration values for the component devices are nested under the `component_config` setting of the compound device.
 
-Lastly, you can define shortcuts to quickly access components of `Compound` devices.
+Lastly, you can define shortcuts (or nicknames) to quickly access the components of compound devices.
 ```yaml
 SHORTCUTS:
-  _Nickname1_: '_Device02_._Component01_'
-  _Nickname2_: '_Device02_._Component02_'
+  First: 'MyCompoundDevice.MyFirstDevice'
+  Second: 'MyCompoundDevice.MySecondDevice'
 ```
+> A different serial port address or camera index may be used by different machines for the same device.\
+*See* [**Section 3**](#3-creating-a-new-project) *to find out how to manage the different addresses used by different machines.*
+
+
+#### 1.2 `layout.json`
+This file stores the layout configuration of your physical workspace, also known as a `Deck`.\
+*See* [**Section 2**](#2-managing-a-deck) *on how to load this information into the setup.*
+
+*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a layout configuration may not be required*
+> This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block / object.
 
-#### 2.2 `layout.json`
-Layout configuration of your physical workspace (`Deck`) will be stored in `layout.json`. This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block/object.
 
-*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a layout configuration may not be required.*
 ```json
 {
   "reference_points":{
-    "1": ["_x01_","_y01_","_z01_"],
-    "2": ["_x02_","_y02_","_z02_"]
+    "1": [11.1,22.2,33.3],
+    "2": [44.4,55.5,66.6],
+    "3": [77.7,88.8,99.9]
   },
   "slots":{
     "1": {
-      "name": "_Labware01_",
+      "name": "MyLabware01",
       "exclusion_height": -1,
-      "filepath": "_repo_/.../_Labware01_.json"
+      "filepath": "MyREPO/.../MyLabware01.json"
     },
     "2": {
-      "name": "_Labware02_",
+      "name": "MyLabware02",
       "exclusion_height": 0,
-      "filepath": "_repo_/.../_Labware02_.json"
+      "filepath": "MyREPO/.../MyLabware02.json"
     },
     "3": {
-      "name": "_Labware03_",
+      "name": "MyLabware03",
       "exclusion_height": 10,
-      "filepath": "_repo_/.../_Labware03_.json"
+      "filepath": "MyREPO/.../MyLabware03.json"
     }
   }
 }
 ```
-In `reference_points`, the bottom-left coordinates of each slot in the workspace are defined. Slots are positions where Labware blocks may be placed.
+> In `reference_points`, the bottom-left coordinates of each slot on the deck are defined. Slots are positions where Labware blocks may be placed.
 
-In `slots`, the name of each slot and the file reference for Labware block that occupies that slot are defined. The filepath starts with the repository's base folder name.
+> In `slots`, the `name` of the Labware and the `filepath` to the JSON file containing Labware details are defined. The filepath starts with the name of the repository's base folder.\
+>\
+> The `exclusion_height` is the height (in mm) above the dimensions of the Labware block to steer clear from when performing movement actions. Values less than 0 means the Labware is not avoided.\
+>\
+> *(Note: Labware avoidance only applies to final coordinates (i.e. destination). Does not guarantee collision avoidance when using point-to-point move actions. Use* `safeMoveTo()` *instead.)*
 
-The `exclusion_height` is the height (in mm) above the dimensions of the Labware block to steer clear from when performing move actions. Defaults to -1 (i.e. do not avoid).\
-*(Note: only applies to final coordinates (i.e. destination). Does not guarantee collision avoidance when using point-to-point move actions. Use* `safeMoveTo()` *instead.)*
-
-#### 2.3 Load setup
-The initialisation of the setup occurs during the import `setup` from within `configs/_Setup01_`.
+#### 1.3 Load setup
+The initialisation of the setup occurs when importing `setup` from `configs.MySetup`. With `setup`, you can access all the devices that you have defined in [**Section 1.1**](#11-configyaml).
 
 ```python
+### main.py ###
 # Add repository folder to sys.path
 from pathlib import Path
 import sys
-REPO = '_repo_' 
-# replace "_repo_" with your base directory for the project
+REPO = 'MyREPO'
 ROOT = str(Path().absolute()).split(REPO)[0]
 sys.path.append(f'{ROOT}{REPO}')
 
 # Import the initialised setup
-from configs._Setup01_ import setup
-this = setup
-this._Device01_
-this._Nickname2_
-```
-With `this`, you can access all the devices that you have defined in `configs.yaml`.
-
-### 3. Managing a deck
-*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a* `Deck` *may not be required.*
-
-#### 3.1 Loading a deck
-To load the `Deck` from the layout file, use the `loadDeck()` function.
-```python
-from configs._Setup01_ import LAYOUT_FILE
-this._Device02_.loadDeck(LAYOUT_FILE)
-deck = this._Device02.deck
+from configs.MySetup import setup
+setup.MyDevice
+setup.First
+```
+
+
+### 2. Managing a deck
+*Optional: if your setup does not involve moving items around in a pre-defined workspace,  a* `Deck` *may not be required*
+
+#### 2.1 Loading a deck
+To load a `Deck` from the layout file, use the `loadDeck()` function of a `Mover` object (or its subclasses).
+```python
+from configs.MySetup import setup, LAYOUT_FILE
+setup.Mover.loadDeck(LAYOUT_FILE)
 ``` 
+> `LAYOUT_FILE` contains the details that has been defined in `layout.json` (see [**Section 1.2**](#12-layoutjson))
 
-#### 3.2 Loading a Labware
-To load the `Labware` into the `Deck`, use the `load_labware()` method.
+#### 2.2 Loading a Labware
+To load a `Labware` onto the deck, use the `load_labware()` method of the `Deck` object.
 ```python
-deck.load_labware(...)
+setup.Mover.deck.load_labware(...)
 ``` 
+> This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block / object.
+
+
+### 3. Managing project addresses
+A `/configs` folder will have been created in the base folder of your project repository to store all configuration related files from which the package will read from, in [**Section 1**](#1-creating-a-new-setup). A template of `registry.yaml` has also been added to the `/configs` folder to manage the machine-specific addresses of your connected devices (e.g. serial port and camera index).
+```yaml
+### registry.yaml ###
+'012345678901234':              # insert your machine's 15-digit ID here
+    cam_index:                  # camera index of the connected imaging devices
+      __cam_01__: 1             # keep the leading and trailing double underscores
+      __cam_02__: 0
+    port:                       # addresses of serial ports
+      __MyDevice__: COM1        # keep the leading and trailing double underscores
+      __MyFirstDevice__: COM22
+```
+
+> Use the `Helper.get_node()` function to get the 15-digit unique identifier of your machine\
+> Use the `Helper.get_port()` function to get the serial port addresses of your connect devices
 
-### 4. Setting up safety measures
-You can optionally set the safety policy for session. This has to be done before importing any of the classes.
 ```python
-lab.set_safety('high')  # Pauses for input before every move action
-lab.set_safety('low')   # Waits for countdown before every move action
-# Import other classes from control-lab-ly only after setting the safety policy
+lab.Helper.get_node()           # Get your machine's ID (15-digit)
+lab.Helper.get_ports()          # Get the port addresses of connected devices
 ```
 
-### 5. Using plugins
-User-defined plugins can be integrated into Control.lab.ly without making additions or modifications to the package itself. All classes and functions can be found in `lab.modules`.
+Afterwards, change the value for the serial port address in the `config.yaml` file to match the registry.
+```yaml
+### config.yaml ###
+MyDevice:
+  module: Move
+  class: Cartesian.Ender
+  settings:
+    port: __MyDevice__          # serial port address
+```
+
+### 4. Using plugins
+*Optional: if drivers for your hardware components are already included, plugins may not be required*
+
+User-defined plugins can be easily written and integrated into Control.lab.ly. All available classes and functions can be found in `lab.modules`.
 ```python
-print(lab.modules)  
-# view the entire package (only those that have been imported during the session)
-lab.modules.Make.Something.Good.myClass
-# this expression returns the registered class
+lab.guide_me()                              # Use guide to view imported objects
+lab.modules.at.Make.Something.Good.MyClass  # Access the the class 
 ```
 
-#### 5.1 Directly registering a Class or Function
+#### 4.1 Registering a Class or Function
 You can import the class and register the object using the `Factory.register()` function.
 ```python
-from my_module import myClass
-lab.Factory.register(myClass, "Make.Something.Good")
+from my_module import MyClass
+lab.Factory.register(MyClass, "Make.Something.Good")
 ```
 
-#### 5.2 Registering a Python module
-Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.\
-Declare a `__where__` global variable to indicate where to register the module.
+#### 4.2 Registering a Python module
+Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.
+> 1. Declare a `__where__` global variable to indicate where to register the module
+> 2. At the end of the .py file, import and call  the `include_this_module()` function
 ```python
 ### my_module.py ###
-__where__ = "Make.Something.Good"                 # Where to register this module to
-# ==========
-def myClass:                                      # Main body of code goes here
+__where__ = "Make.Something.Good"               # Where to register this module to
+
+def MyClass:                                    # Main body of code goes here
+  ...
+
+def my_function:
   ...
-# ==========
-from controllably import include_this_module      # Registers only the Classes and Functions
-include_this_module()                             # defined above in this .py file
+
+from controllably import include_this_module    # Registers only the Classes and Functions
+include_this_module()                           # defined above in this .py file
 ```
-At the end of the .py file, import and call  the `include_this_module()` function.
 
+The Classes and Functions in the module will be registered when you import the module.
+```python
+### main.py ###
+from my_module import MyClass, my_function
+```
 ---
 
 ## Dependencies
-- Dash (>=2.7.1)
-- Impedance (>=1.4.1)
-- Imutils (>=0.5.4)
-- Matplotlib (>=3.3.4)
-- Nest-asyncio (>=1.5.1)
-- Numpy (>=1.19.5)
-- Opencv-python (>=4.5.4.58)
-- Pandas (>=1.2.4)
-- Plotly (>=5.3.1)
-- PyModbusTCP (>=0.2.0)
-- Pyserial (>=3.5)
-- PySimpleGUI (>=4.60.4)
+- imutils (>=0.5.4)
+- Markdown (>=3.3.4)
+- numpy (>=1.19.5)
+- opencv-python (>=4.5.4.58)
+- pandas (>=1.2.4)
+- pyModbusTCP (>=0.2.0)
+- pyserial (>=3.5)
+- PySimpleGUI (>=4.60.5)
 - PyVISA (>=1.12.0)
 - PyYAML (>=6.0)
-- Scipy (>=1.6.2)
+- tkhtmlview (>=0.2.0)
 
 ## Contributors
 [@kylejeanlewis](https://github.com/kylejeanlewis)\
 [@mat-fox](https://github.com/mat-fox)\
 [@Quijanove](https://github.com/Quijanove)\
 [@AniketChitre](https://github.com/AniketChitre)
 
@@ -340,18 +354,46 @@
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
 ---
 # Change Log
 
 ## Unreleased
 *Items under development*
-### 1.1.0
-- Integration for orbital shaker \[QInstruments\]
-- Integration for pH meter probe \[Sentron\]
-- Integration for force sensor
+### 1.2.0
+- Integration for mass balance from Sartorius
+
+## Version 1.1.0
+Bug fixes and feature enhancements. First released 15 Jun 2023.
+### Added
+- `ForceSensor` - DIY force sensor (#55)
+- `BioShake` - orbital shaker from QInstruments (#56)
+- `SentronProbe` - pH meter probe from Sentron (#75)
+- `Maker`
+  - added `execute()` abstract method and implemented in subclasses
+- GUI
+  - `Guide` - documentation guide
+  - `MakerPanel` - daptive GUI controls for `Maker` objects (#87)
+### Changed
+- `M1Pro`
+  - fix issue with changing handedness (#86)
+- `Peltier`
+  - rename `getTemperatures()` to `getTemperature()`
+  - rename `isReady()` to `isAtTemperature()`
+  - rename `set_point` to `set_temperature`
+- `Ender`
+  - rename `set_point` to `set_temperature`
+- `TriContinent`
+  - rename `step_limit` to `limits`
+- Refactor and reorganize `GUI` code
+- Refactor code in `helper` and `factory`
+- Updated documentation
+### Removed
+- `Analyse` sub-package removed
+- `Control.Schedule` sub-package removed
+- Unnecessary commented-out blocks of code
 
 
 ## Version 1.0.1
 Bug fixes and minor feature enhancements. First released 08 May 2023.
 ### Added
 - `LiquidMover`
   - Added `LiquidMover.touchTip()` method to touch the pipette tip against the walls of the vessel to remove excess liquid on the outside of the tip (#62)
```

### Comparing `control-lab-ly-1.1.0a0/docs/CHANGELOG.md` & `control-lab-ly-1.1.0b0/docs/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,43 @@
 # Change Log
 
 ## Unreleased
 *Items under development*
-### 1.1.0
-- Integration for orbital shaker \[QInstruments\]
-- Integration for pH meter probe \[Sentron\]
-- Integration for force sensor
+### 1.2.0
+- Integration for mass balance from Sartorius
+
+## Version 1.1.0
+Bug fixes and feature enhancements. First released 15 Jun 2023.
+### Added
+- `ForceSensor` - DIY force sensor (#55)
+- `BioShake` - orbital shaker from QInstruments (#56)
+- `SentronProbe` - pH meter probe from Sentron (#75)
+- `Maker`
+  - added `execute()` abstract method and implemented in subclasses
+- GUI
+  - `Guide` - documentation guide
+  - `MakerPanel` - daptive GUI controls for `Maker` objects (#87)
+### Changed
+- `M1Pro`
+  - fix issue with changing handedness (#86)
+- `Peltier`
+  - rename `getTemperatures()` to `getTemperature()`
+  - rename `isReady()` to `isAtTemperature()`
+  - rename `set_point` to `set_temperature`
+- `Ender`
+  - rename `set_point` to `set_temperature`
+- `TriContinent`
+  - rename `step_limit` to `limits`
+- Refactor and reorganize `GUI` code
+- Refactor code in `helper` and `factory`
+- Updated documentation
+### Removed
+- `Analyse` sub-package removed
+- `Control.Schedule` sub-package removed
+- Unnecessary commented-out blocks of code
 
 
 ## Version 1.0.1
 Bug fixes and minor feature enhancements. First released 08 May 2023.
 ### Added
 - `LiquidMover`
   - Added `LiquidMover.touchTip()` method to touch the pipette tip against the walls of the vessel to remove excess liquid on the outside of the tip (#62)
```

### Comparing `control-lab-ly-1.1.0a0/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.1.0b0/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/docs/LICENSE.md` & `control-lab-ly-1.1.0b0/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/docs/README.md` & `control-lab-ly-1.1.0b0/docs/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # Control.lab.ly
 Lab Equipment Automation Package
 
 ## Description
 User-friendly package that enables flexible automation an reconfigurable setups for high-throughput experimentation and machine learning.
 
 ## Package Structure
-1. Analyse
-2. Compound
-3. Control
-4. Make
-5. Measure
-6. Move
-7. Transfer
-8. View
+1. Compound
+2. Control
+3. Make
+4. Measure
+5. Move
+6. Transfer
+7. View
 
 ## Device support
 - Make
+  - (QInstruments) Bioshake Orbital Shaker
   - Multi-channel LED array \[Arduino\]
   - Multi-channel spin-coater \[Arduino\]
   - Peltier device \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
+  - (Sentron) SI series pH meters - *full functionality in development*
   - Precision mass balance \[Arduino\]
 - Move
   - (Creality) Ender-3
   - (Dobot) M1 Pro
   - (Dobot) MG400
   - Primitiv \[Arduino\]
 - Transfer
@@ -34,276 +35,289 @@
   - (TriContinent) C Series syringe pumps
   - Peristaltic pump and syringe system \[Arduino\]
 - View
   - (FLIR) AX8 thermal imaging camera - *full functionality in development*
   - Web cameras \[General\]
 
 ## Installation
-Control.lab.ly can be found on PyPI and can be installed easily with `pip install`.
+Control.lab.ly can be found on PyPI and can be easily installed with `pip install`.
 ```shell
 $ pip install control-lab-ly
 ```
 
 ## Basic Usage
 Simple start-up guide for basic usage of the package.
 
 ### Import desired class
 ```python
 from controllably.Move.Cartesian import Ender
 mover = Ender(...)
 mover.safeMoveTo((x,y,z))
 ```
 
-More details for each class / module / package can be explored by using the `help` function.
+### View documentation
+Use the built-in guide to read the documentation for the package.
 ```python
-help(controllably.Move)   # help on package
-help(Ender)               # help on class
-help(mover)               # help on instance/object
+from controllably import guide_me
+guide_me()
 ```
+![Screenshot of the documentation guide](./assets/Documentation%20guide.png)
 
-Alternatively, you can use the native `pydoc` documentation generator.
-```shell
-$ python -m pydoc controllably.Move
-```
-
->Tip: when using Interactive Python (IPython) (e.g. Jupyter notebooks), add a exclamation mark (`!`) in front of the shell command
+Alternatively, details for each class / module / package can be explored by using the `help` function.
 ```python
->>> !python -m pydoc controllably.Move
->>> !python -m pydoc -b   # Generates a static HTML site to browse package documentation
+help(Ender)
 ```
-For basic usage, this is all you need to know. Check the documentation for more details on each respective class.
+
+For basic usage, this is all you need to know. Check the documentation for more details on each class and function.
 
 ---
 
 ## Advanced Usage
-For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation.
+For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation. This includes setting up configuration files and adding plugin drivers.
 
-### 0. Import package
-The convention is to import Control-lab-ly as `lab`.
+### Import package
 ```python
 import controllably as lab
 ```
 
-### Contents
-1. Projects
-2. Setups
-3. Decks
-4. Safety measures
-5. Plugins
-
-### 1. Creating a new project
-Create a `/configs` folder in the base folder of your project repository to store all configuration related files from which the package will read from.\
-This only has to be done once when you first set up the project folder.
+Optionally, you can set the safety policy for the session. This feature allows the user to prevent collisions before each movement is made. The safety policy has to be assigned before importing any of the `Mover` objects.
 ```python
-lab.create_configs()
-```
+lab.set_safety('high')  # Notifies; Pauses for input before every move action
+lab.set_safety('low')   # Notifies; Waits for countdown before every move action
+lab.set_safety(None)    # Movement actions carry out without delay
 
-A different address may be used by different machines for the same device. To manage the different addresses used by different machines, you first need your machine's unique identifier.
-```python
-# Get your machine's ID
-print(lab.Helper.get_node())
+# Import control-lab-ly classes only after setting the safety policy
 ```
 
-A template of `registry.yaml` has also been added to the folder to hold the machine-specific addresses of your connected devices (i.e. COM ports).\
-Populate the YAML file in the format shown below.
-```yaml
-### registry.yaml ###
-'012345678901234':          # insert your machine's 15-digit ID here (from the above step)
-    cam_index:              # camera index of the connected imaging devices
-      __cam_01__: 1         # keep the leading and trailing double underscores
-      __cam_02__: 0
-    port:                   # addresses of serial COM ports
-      __device_01__: COM3   # keep the leading and trailing double underscores
-      __device_02__: COM16
-```
-
-To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use:
-```python
-lab.Helper.get_ports()
-```
+### Contents
+1. [Setups](#1-creating-a-new-setup)
+2. [Decks](#2-managing-a-deck)
+3. [Addresses](#3-managing-project-addresses)
+4. [Plugins](#4-using-plugins)
 
-### 2. Creating a new setup
-Create a new folder for the configuration files of your new setup. If you had skipped the previous step of creating a project, calling `lab.create_setup()` will also generate the required file structure. However, be sure to populate your machine ID and device addresses in the `registry.yaml` file.
 
+### 1. Creating a new setup
+Create a `/configs/MySetup` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
 ```python
-lab.create_setup(setup_name = "_Setup01_")
-# replace "_Setup01_" with the desired name for your setup
+lab.create_setup(setup_name = "MySetup")
 ```
-This creates a `/_Setup01_` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
 
-#### 2.1 `config.yaml`
-Configuration and calibration values for your devices is stored in `config.yaml`.\
-Each configuration starts with the `name` of your device, then its `module`, `class`, and `settings`.
+#### 1.1 `config.yaml`
+This file stores the configuration and calibration values for your devices.
 ```yaml
-_Device01_:                                     # name of simple device (user-defined)
-  module: _module_name_01_                      # device module
-  class: _submodule_1A_._class_1A_              # device class
+MyDevice:                                       # device name
+  module: Move                                  # top-level category
+  class: Cartesian.Ender                        # device class
   settings:
-    port: __device_01__                         # port addresses defined in registry.yaml
-    _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
-    _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
-```
+    port: COM1                                  # serial port address
+    setting_A: {'tuple': [300,0,200]}           # use keys to define the type of iterable
+    setting_B: {'array': [[0,1,0],[-1,0,0]]}    # only tuple and np.array supported
+```
+> Each device configuration starts with the device name, then the following parameters:\
+> `module`: top-level category (such as Make, Measure, Move,Transfer, View)\
+> `class`: point to specific subclass using dot notation\
+> `settings`: various initialisation settings\
+> *See the* [**guide**](#view-documentation) *for more details on these parameters*
 
-`Compound` devices are similarly configured. The configuration values for its component devices are defined under the `component_config` setting. The structure of the configuration values for the component devices are similar to that shown above, except indented to fall under the indentation of the `component_config` setting.
+Compound devices are similarly configured. 
 ```yaml
-_Device02_:                                 # name of 'Compound' device (user-defined)
-  module: Compound                            
-  class: _submodule_2A_._class_2A_
-  settings:
-    _setting_C_: 1                          # other settings for your 'Compound' device
-    component_config:                       # nest component configuration settings here
-      _Component01_:                        # name of component
-        module: _module_name_03_
-        class: _submodule_3A_._class_3A_
-        settings:
-          ip_address: '192.0.0.1'           # IP addresses do not vary between machines
-      _Component02_: 
-        module: _module_name_04_
-        class: _submodule_4A_._class_4A_
-        settings:
-          _setting_D_: 2                    # settings for your component device
+MyCompoundDevice:                         # compound device name
+  module: Compound
+  class: LiquidMover.LiquidMoverSetup
+  settings:                               # settings for your compound device
+    setting_C: True
+    component_config:                     # nest component configuration settings here
+      MyFirstDevice:                      # component device name
+        module: Transfer
+        class: Liquid.SyringeAssembly
+        settings:                         # settings for your component device
+          port: COM22
+          setting_D: 2                    
+      MySecondDevice:                     # component device name
+        module: Mover
+        class: Jointed.Dobot.M1Pro
+        settings:                         # settings for your compound device
+          ip_address: '192.0.0.1'
 ```
+> The configuration values for the component devices are nested under the `component_config` setting of the compound device.
 
-Lastly, you can define shortcuts to quickly access components of `Compound` devices.
+Lastly, you can define shortcuts (or nicknames) to quickly access the components of compound devices.
 ```yaml
 SHORTCUTS:
-  _Nickname1_: '_Device02_._Component01_'
-  _Nickname2_: '_Device02_._Component02_'
+  First: 'MyCompoundDevice.MyFirstDevice'
+  Second: 'MyCompoundDevice.MySecondDevice'
 ```
+> A different serial port address or camera index may be used by different machines for the same device.\
+*See* [**Section 3**](#3-creating-a-new-project) *to find out how to manage the different addresses used by different machines.*
+
+
+#### 1.2 `layout.json`
+This file stores the layout configuration of your physical workspace, also known as a `Deck`.\
+*See* [**Section 2**](#2-managing-a-deck) *on how to load this information into the setup.*
+
+*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a layout configuration may not be required*
+> This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block / object.
 
-#### 2.2 `layout.json`
-Layout configuration of your physical workspace (`Deck`) will be stored in `layout.json`. This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block/object.
 
-*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a layout configuration may not be required.*
 ```json
 {
   "reference_points":{
-    "1": ["_x01_","_y01_","_z01_"],
-    "2": ["_x02_","_y02_","_z02_"]
+    "1": [11.1,22.2,33.3],
+    "2": [44.4,55.5,66.6],
+    "3": [77.7,88.8,99.9]
   },
   "slots":{
     "1": {
-      "name": "_Labware01_",
+      "name": "MyLabware01",
       "exclusion_height": -1,
-      "filepath": "_repo_/.../_Labware01_.json"
+      "filepath": "MyREPO/.../MyLabware01.json"
     },
     "2": {
-      "name": "_Labware02_",
+      "name": "MyLabware02",
       "exclusion_height": 0,
-      "filepath": "_repo_/.../_Labware02_.json"
+      "filepath": "MyREPO/.../MyLabware02.json"
     },
     "3": {
-      "name": "_Labware03_",
+      "name": "MyLabware03",
       "exclusion_height": 10,
-      "filepath": "_repo_/.../_Labware03_.json"
+      "filepath": "MyREPO/.../MyLabware03.json"
     }
   }
 }
 ```
-In `reference_points`, the bottom-left coordinates of each slot in the workspace are defined. Slots are positions where Labware blocks may be placed.
+> In `reference_points`, the bottom-left coordinates of each slot on the deck are defined. Slots are positions where Labware blocks may be placed.
 
-In `slots`, the name of each slot and the file reference for Labware block that occupies that slot are defined. The filepath starts with the repository's base folder name.
+> In `slots`, the `name` of the Labware and the `filepath` to the JSON file containing Labware details are defined. The filepath starts with the name of the repository's base folder.\
+>\
+> The `exclusion_height` is the height (in mm) above the dimensions of the Labware block to steer clear from when performing movement actions. Values less than 0 means the Labware is not avoided.\
+>\
+> *(Note: Labware avoidance only applies to final coordinates (i.e. destination). Does not guarantee collision avoidance when using point-to-point move actions. Use* `safeMoveTo()` *instead.)*
 
-The `exclusion_height` is the height (in mm) above the dimensions of the Labware block to steer clear from when performing move actions. Defaults to -1 (i.e. do not avoid).\
-*(Note: only applies to final coordinates (i.e. destination). Does not guarantee collision avoidance when using point-to-point move actions. Use* `safeMoveTo()` *instead.)*
-
-#### 2.3 Load setup
-The initialisation of the setup occurs during the import `setup` from within `configs/_Setup01_`.
+#### 1.3 Load setup
+The initialisation of the setup occurs when importing `setup` from `configs.MySetup`. With `setup`, you can access all the devices that you have defined in [**Section 1.1**](#11-configyaml).
 
 ```python
+### main.py ###
 # Add repository folder to sys.path
 from pathlib import Path
 import sys
-REPO = '_repo_' 
-# replace "_repo_" with your base directory for the project
+REPO = 'MyREPO'
 ROOT = str(Path().absolute()).split(REPO)[0]
 sys.path.append(f'{ROOT}{REPO}')
 
 # Import the initialised setup
-from configs._Setup01_ import setup
-this = setup
-this._Device01_
-this._Nickname2_
-```
-With `this`, you can access all the devices that you have defined in `configs.yaml`.
-
-### 3. Managing a deck
-*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a* `Deck` *may not be required.*
-
-#### 3.1 Loading a deck
-To load the `Deck` from the layout file, use the `loadDeck()` function.
-```python
-from configs._Setup01_ import LAYOUT_FILE
-this._Device02_.loadDeck(LAYOUT_FILE)
-deck = this._Device02.deck
+from configs.MySetup import setup
+setup.MyDevice
+setup.First
+```
+
+
+### 2. Managing a deck
+*Optional: if your setup does not involve moving items around in a pre-defined workspace,  a* `Deck` *may not be required*
+
+#### 2.1 Loading a deck
+To load a `Deck` from the layout file, use the `loadDeck()` function of a `Mover` object (or its subclasses).
+```python
+from configs.MySetup import setup, LAYOUT_FILE
+setup.Mover.loadDeck(LAYOUT_FILE)
 ``` 
+> `LAYOUT_FILE` contains the details that has been defined in `layout.json` (see [**Section 1.2**](#12-layoutjson))
 
-#### 3.2 Loading a Labware
-To load the `Labware` into the `Deck`, use the `load_labware()` method.
+#### 2.2 Loading a Labware
+To load a `Labware` onto the deck, use the `load_labware()` method of the `Deck` object.
 ```python
-deck.load_labware(...)
+setup.Mover.deck.load_labware(...)
 ``` 
+> This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block / object.
+
+
+### 3. Managing project addresses
+A `/configs` folder will have been created in the base folder of your project repository to store all configuration related files from which the package will read from, in [**Section 1**](#1-creating-a-new-setup). A template of `registry.yaml` has also been added to the `/configs` folder to manage the machine-specific addresses of your connected devices (e.g. serial port and camera index).
+```yaml
+### registry.yaml ###
+'012345678901234':              # insert your machine's 15-digit ID here
+    cam_index:                  # camera index of the connected imaging devices
+      __cam_01__: 1             # keep the leading and trailing double underscores
+      __cam_02__: 0
+    port:                       # addresses of serial ports
+      __MyDevice__: COM1        # keep the leading and trailing double underscores
+      __MyFirstDevice__: COM22
+```
+
+> Use the `Helper.get_node()` function to get the 15-digit unique identifier of your machine\
+> Use the `Helper.get_port()` function to get the serial port addresses of your connect devices
 
-### 4. Setting up safety measures
-You can optionally set the safety policy for session. This has to be done before importing any of the classes.
 ```python
-lab.set_safety('high')  # Pauses for input before every move action
-lab.set_safety('low')   # Waits for countdown before every move action
-# Import other classes from control-lab-ly only after setting the safety policy
+lab.Helper.get_node()           # Get your machine's ID (15-digit)
+lab.Helper.get_ports()          # Get the port addresses of connected devices
 ```
 
-### 5. Using plugins
-User-defined plugins can be integrated into Control.lab.ly without making additions or modifications to the package itself. All classes and functions can be found in `lab.modules`.
+Afterwards, change the value for the serial port address in the `config.yaml` file to match the registry.
+```yaml
+### config.yaml ###
+MyDevice:
+  module: Move
+  class: Cartesian.Ender
+  settings:
+    port: __MyDevice__          # serial port address
+```
+
+### 4. Using plugins
+*Optional: if drivers for your hardware components are already included, plugins may not be required*
+
+User-defined plugins can be easily written and integrated into Control.lab.ly. All available classes and functions can be found in `lab.modules`.
 ```python
-print(lab.modules)  
-# view the entire package (only those that have been imported during the session)
-lab.modules.Make.Something.Good.myClass
-# this expression returns the registered class
+lab.guide_me()                              # Use guide to view imported objects
+lab.modules.at.Make.Something.Good.MyClass  # Access the the class 
 ```
 
-#### 5.1 Directly registering a Class or Function
+#### 4.1 Registering a Class or Function
 You can import the class and register the object using the `Factory.register()` function.
 ```python
-from my_module import myClass
-lab.Factory.register(myClass, "Make.Something.Good")
+from my_module import MyClass
+lab.Factory.register(MyClass, "Make.Something.Good")
 ```
 
-#### 5.2 Registering a Python module
-Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.\
-Declare a `__where__` global variable to indicate where to register the module.
+#### 4.2 Registering a Python module
+Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.
+> 1. Declare a `__where__` global variable to indicate where to register the module
+> 2. At the end of the .py file, import and call  the `include_this_module()` function
 ```python
 ### my_module.py ###
-__where__ = "Make.Something.Good"                 # Where to register this module to
-# ==========
-def myClass:                                      # Main body of code goes here
+__where__ = "Make.Something.Good"               # Where to register this module to
+
+def MyClass:                                    # Main body of code goes here
   ...
-# ==========
-from controllably import include_this_module      # Registers only the Classes and Functions
-include_this_module()                             # defined above in this .py file
+
+def my_function:
+  ...
+
+from controllably import include_this_module    # Registers only the Classes and Functions
+include_this_module()                           # defined above in this .py file
 ```
-At the end of the .py file, import and call  the `include_this_module()` function.
 
+The Classes and Functions in the module will be registered when you import the module.
+```python
+### main.py ###
+from my_module import MyClass, my_function
+```
 ---
 
 ## Dependencies
-- Dash (>=2.7.1)
-- Impedance (>=1.4.1)
-- Imutils (>=0.5.4)
-- Matplotlib (>=3.3.4)
-- Nest-asyncio (>=1.5.1)
-- Numpy (>=1.19.5)
-- Opencv-python (>=4.5.4.58)
-- Pandas (>=1.2.4)
-- Plotly (>=5.3.1)
-- PyModbusTCP (>=0.2.0)
-- Pyserial (>=3.5)
-- PySimpleGUI (>=4.60.4)
+- imutils (>=0.5.4)
+- Markdown (>=3.3.4)
+- numpy (>=1.19.5)
+- opencv-python (>=4.5.4.58)
+- pandas (>=1.2.4)
+- pyModbusTCP (>=0.2.0)
+- pyserial (>=3.5)
+- PySimpleGUI (>=4.60.5)
 - PyVISA (>=1.12.0)
 - PyYAML (>=6.0)
-- Scipy (>=1.6.2)
+- tkhtmlview (>=0.2.0)
 
 ## Contributors
 [@kylejeanlewis](https://github.com/kylejeanlewis)\
 [@mat-fox](https://github.com/mat-fox)\
 [@Quijanove](https://github.com/Quijanove)\
 [@AniketChitre](https://github.com/AniketChitre)
```

### Comparing `control-lab-ly-1.1.0a0/setup.cfg` & `control-lab-ly-1.1.0b0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,94 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e31  y..version = 1.1
-00000030: 2e30 2d61 0d0a 6465 7363 7269 7074 696f  .0-a..descriptio
-00000040: 6e20 3d20 4c61 6220 4571 7569 706d 656e  n = Lab Equipmen
-00000050: 7420 4175 746f 6d61 7469 6f6e 2050 6163  t Automation Pac
-00000060: 6b61 6765 0d0a 6c6f 6e67 5f64 6573 6372  kage..long_descr
-00000070: 6970 7469 6f6e 203d 2066 696c 653a 2064  iption = file: d
-00000080: 6f63 732f 5245 4144 4d45 2e6d 642c 2064  ocs/README.md, d
-00000090: 6f63 732f 4348 414e 4745 4c4f 472e 6d64  ocs/CHANGELOG.md
-000000a0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
-000000b0: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
-000000c0: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0d  = text/markdown.
-000000d0: 0a61 7574 686f 7220 3d20 4368 616e 6720  .author = Chang 
-000000e0: 4a69 6520 4c65 6f6e 670d 0a61 7574 686f  Jie Leong..autho
-000000f0: 725f 656d 6169 6c20 3d20 6368 616e 676a  r_email = changj
-00000100: 6965 2e6c 656f 6e67 406f 7574 6c6f 6f6b  ie.leong@outlook
-00000110: 2e63 6f6d 0d0a 7572 6c20 3d20 6874 7470  .com..url = http
-00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6b  s://github.com/k
-00000130: 796c 656a 6561 6e6c 6577 6973 2f63 6f6e  ylejeanlewis/con
-00000140: 7472 6f6c 2d6c 6162 2d6c 650d 0a70 726f  trol-lab-le..pro
-00000150: 6a65 6374 5f75 726c 7320 3d20 0d0a 0947  ject_urls = ...G
-00000160: 6974 4875 6220 3d20 6874 7470 733a 2f2f  itHub = https://
-00000170: 6769 7468 7562 2e63 6f6d 2f6b 796c 656a  github.com/kylej
-00000180: 6561 6e6c 6577 6973 2f63 6f6e 7472 6f6c  eanlewis/control
-00000190: 2d6c 6162 2d6c 650d 0a09 446f 6375 6d65  -lab-le...Docume
-000001a0: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
-000001b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
-000001c0: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
-000001d0: 6f6c 2d6c 6162 2d6c 652f 626c 6f62 2f6d  ol-lab-le/blob/m
-000001e0: 6169 6e2f 646f 6373 2f52 4541 444d 452e  ain/docs/README.
-000001f0: 6d64 0d0a 0943 6861 6e67 656c 6f67 203d  md...Changelog =
-00000200: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000210: 636f 6d2f 6b79 6c65 6a65 616e 6c65 7769  com/kylejeanlewi
-00000220: 732f 636f 6e74 726f 6c2d 6c61 622d 6c65  s/control-lab-le
-00000230: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
-00000240: 4348 414e 4745 4c4f 472e 6d64 0d0a 0954  CHANGELOG.md...T
-00000250: 7261 636b 6572 203d 2068 7474 7073 3a2f  racker = https:/
-00000260: 2f67 6974 6875 622e 636f 6d2f 6b79 6c65  /github.com/kyle
-00000270: 6a65 616e 6c65 7769 732f 636f 6e74 726f  jeanlewis/contro
-00000280: 6c2d 6c61 622d 6c65 2f69 7373 7565 730d  l-lab-le/issues.
-00000290: 0a6c 6963 656e 7365 203d 204d 4954 0d0a  .license = MIT..
-000002a0: 6b65 7977 6f72 6473 203d 200d 0a09 7079  keywords = ...py
-000002b0: 7468 6f6e 0d0a 096c 6162 2061 7574 6f6d  thon...lab autom
-000002c0: 6174 696f 6e0d 0a63 6c61 7373 6966 6965  ation..classifie
-000002d0: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
-000002e0: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
-000002f0: 2d20 416c 7068 610d 0a09 496e 7465 6e64  - Alpha...Intend
-00000300: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-00000310: 6576 656c 6f70 6572 730d 0a09 496e 7465  evelopers...Inte
-00000320: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000330: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
-00000340: 680d 0a09 4c69 6365 6e73 6520 3a3a 204f  h...License :: O
-00000350: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
-00000360: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
-00000370: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
-00000380: 204d 6963 726f 736f 6674 203a 3a20 5769   Microsoft :: Wi
-00000390: 6e64 6f77 730d 0a09 5072 6f67 7261 6d6d  ndows...Programm
-000003a0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000003b0: 5079 7468 6f6e 203a 3a20 330d 0a09 5072  Python :: 3...Pr
-000003c0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000003d0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000003e0: 332e 380d 0a09 546f 7069 6320 3a3a 2053  3.8...Topic :: S
-000003f0: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-00000400: 6572 696e 670d 0a0d 0a5b 6f70 7469 6f6e  ering....[option
-00000410: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-00000420: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
-00000430: 6167 6573 203d 2066 696e 643a 0d0a 696e  ages = find:..in
-00000440: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-00000450: 7461 203d 2054 7275 650d 0a70 7974 686f  ta = True..pytho
-00000460: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000470: 2e38 0d0a 696e 7374 616c 6c5f 7265 7175  .8..install_requ
-00000480: 6972 6573 203d 200d 0a09 6461 7368 3e3d  ires = ...dash>=
-00000490: 322e 370d 0a09 696d 7065 6461 6e63 653e  2.7...impedance>
-000004a0: 3d31 2e34 0d0a 0969 6d75 7469 6c73 3e3d  =1.4...imutils>=
-000004b0: 302e 350d 0a09 6d61 7470 6c6f 746c 6962  0.5...matplotlib
-000004c0: 3e3d 332e 330d 0a09 6e65 7374 5f61 7379  >=3.3...nest_asy
-000004d0: 6e63 696f 3e3d 312e 350d 0a09 6e75 6d70  ncio>=1.5...nump
-000004e0: 793e 3d31 2e31 390d 0a09 6f70 656e 6376  y>=1.19...opencv
-000004f0: 5f70 7974 686f 6e3e 3d34 2e35 2e30 0d0a  _python>=4.5.0..
-00000500: 0970 616e 6461 733e 3d31 2e32 0d0a 0970  .pandas>=1.2...p
-00000510: 6c6f 746c 793e 3d35 2e33 0d0a 0970 794d  lotly>=5.3...pyM
-00000520: 6f64 6275 7354 4350 3e3d 302e 320d 0a09  odbusTCP>=0.2...
-00000530: 7079 7365 7269 616c 3e3d 332e 350d 0a09  pyserial>=3.5...
-00000540: 5079 5369 6d70 6c65 4755 493e 3d34 2e36  PySimpleGUI>=4.6
-00000550: 300d 0a09 5079 5649 5341 3e3d 312e 3132  0...PyVISA>=1.12
-00000560: 0d0a 0950 7959 414d 4c3e 3d36 2e30 0d0a  ...PyYAML>=6.0..
-00000570: 0973 6369 7079 3e3d 312e 360d 0a0d 0a5b  .scipy>=1.6....[
-00000580: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
-00000590: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-000005a0: 7372 630d 0a65 7863 6c75 6465 203d 2074  src..exclude = t
-000005b0: 6573 7473 0d0a 0d0a 5b6f 7074 696f 6e73  ests....[options
-000005c0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
-000005d0: 2a20 3d20 2a2e 6a73 6f6e 2c20 2a2e 7961  * = *.json, *.ya
-000005e0: 6d6c 2c20 2a2e 706e 670d 0a0d 0a5b 6567  ml, *.png....[eg
-000005f0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000600: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000610: 3d20 300d 0a0d 0a                        = 0....
+00000030: 2e30 2d62 300d 0a64 6573 6372 6970 7469  .0-b0..descripti
+00000040: 6f6e 203d 204c 6162 2045 7175 6970 6d65  on = Lab Equipme
+00000050: 6e74 2041 7574 6f6d 6174 696f 6e20 5061  nt Automation Pa
+00000060: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
+00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
+00000080: 646f 6373 2f52 4541 444d 452e 6d64 2c20  docs/README.md, 
+00000090: 646f 6373 2f43 4841 4e47 454c 4f47 2e6d  docs/CHANGELOG.m
+000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
+000000b0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+000000c0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+000000d0: 0d0a 6175 7468 6f72 203d 2043 6861 6e67  ..author = Chang
+000000e0: 204a 6965 204c 656f 6e67 0d0a 6175 7468   Jie Leong..auth
+000000f0: 6f72 5f65 6d61 696c 203d 2063 6861 6e67  or_email = chang
+00000100: 6a69 652e 6c65 6f6e 6740 6f75 746c 6f6f  jie.leong@outloo
+00000110: 6b2e 636f 6d0d 0a75 726c 203d 2068 7474  k.com..url = htt
+00000120: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000130: 6b79 6c65 6a65 616e 6c65 7769 732f 636f  kylejeanlewis/co
+00000140: 6e74 726f 6c2d 6c61 622d 6c65 0d0a 7072  ntrol-lab-le..pr
+00000150: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
+00000160: 4769 7448 7562 203d 2068 7474 7073 3a2f  GitHub = https:/
+00000170: 2f67 6974 6875 622e 636f 6d2f 6b79 6c65  /github.com/kyle
+00000180: 6a65 616e 6c65 7769 732f 636f 6e74 726f  jeanlewis/contro
+00000190: 6c2d 6c61 622d 6c65 0d0a 0944 6f63 756d  l-lab-le...Docum
+000001a0: 656e 7461 7469 6f6e 203d 2068 7474 7073  entation = https
+000001b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b79  ://github.com/ky
+000001c0: 6c65 6a65 616e 6c65 7769 732f 636f 6e74  lejeanlewis/cont
+000001d0: 726f 6c2d 6c61 622d 6c65 2f62 6c6f 622f  rol-lab-le/blob/
+000001e0: 6d61 696e 2f64 6f63 732f 5245 4144 4d45  main/docs/README
+000001f0: 2e6d 640d 0a09 4368 616e 6765 6c6f 6720  .md...Changelog 
+00000200: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000210: 2e63 6f6d 2f6b 796c 656a 6561 6e6c 6577  .com/kylejeanlew
+00000220: 6973 2f63 6f6e 7472 6f6c 2d6c 6162 2d6c  is/control-lab-l
+00000230: 652f 626c 6f62 2f6d 6169 6e2f 646f 6373  e/blob/main/docs
+00000240: 2f43 4841 4e47 454c 4f47 2e6d 640d 0a09  /CHANGELOG.md...
+00000250: 5472 6163 6b65 7220 3d20 6874 7470 733a  Tracker = https:
+00000260: 2f2f 6769 7468 7562 2e63 6f6d 2f6b 796c  //github.com/kyl
+00000270: 656a 6561 6e6c 6577 6973 2f63 6f6e 7472  ejeanlewis/contr
+00000280: 6f6c 2d6c 6162 2d6c 652f 6973 7375 6573  ol-lab-le/issues
+00000290: 0d0a 6c69 6365 6e73 6520 3d20 4d49 540d  ..license = MIT.
+000002a0: 0a6b 6579 776f 7264 7320 3d20 0d0a 0970  .keywords = ...p
+000002b0: 7974 686f 6e0d 0a09 6c61 6220 6175 746f  ython...lab auto
+000002c0: 6d61 7469 6f6e 0d0a 636c 6173 7369 6669  mation..classifi
+000002d0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
+000002e0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
+000002f0: 202d 2041 6c70 6861 0d0a 0949 6e74 656e   - Alpha...Inten
+00000300: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
+00000310: 4465 7665 6c6f 7065 7273 0d0a 0949 6e74  Developers...Int
+00000320: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+00000330: 3a20 5363 6965 6e63 652f 5265 7365 6172  : Science/Resear
+00000340: 6368 0d0a 094c 6963 656e 7365 203a 3a20  ch...License :: 
+00000350: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000360: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
+00000370: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000380: 3a20 4d69 6372 6f73 6f66 7420 3a3a 2057  : Microsoft :: W
+00000390: 696e 646f 7773 0d0a 0950 726f 6772 616d  indows...Program
+000003a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000003b0: 2050 7974 686f 6e20 3a3a 2033 0d0a 0950   Python :: 3...P
+000003c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000003d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000003e0: 2033 2e38 0d0a 0954 6f70 6963 203a 3a20   3.8...Topic :: 
+000003f0: 5363 6965 6e74 6966 6963 2f45 6e67 696e  Scientific/Engin
+00000400: 6565 7269 6e67 0d0a 0d0a 5b6f 7074 696f  eering....[optio
+00000410: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+00000420: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
+00000430: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a69  kages = find:..i
+00000440: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000450: 6174 6120 3d20 5472 7565 0d0a 7079 7468  ata = True..pyth
+00000460: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000470: 332e 380d 0a69 6e73 7461 6c6c 5f72 6571  3.8..install_req
+00000480: 7569 7265 7320 3d20 0d0a 0969 6d75 7469  uires = ...imuti
+00000490: 6c73 3e3d 302e 350d 0a09 4d61 726b 646f  ls>=0.5...Markdo
+000004a0: 776e 3e3d 332e 330d 0a09 6e75 6d70 793e  wn>=3.3...numpy>
+000004b0: 3d31 2e31 390d 0a09 6f70 656e 6376 5f70  =1.19...opencv_p
+000004c0: 7974 686f 6e3e 3d34 2e35 2e30 0d0a 0970  ython>=4.5.0...p
+000004d0: 616e 6461 733e 3d31 2e32 0d0a 0970 794d  andas>=1.2...pyM
+000004e0: 6f64 6275 7354 4350 3e3d 302e 320d 0a09  odbusTCP>=0.2...
+000004f0: 7079 7365 7269 616c 3e3d 332e 350d 0a09  pyserial>=3.5...
+00000500: 5079 5369 6d70 6c65 4755 493e 3d34 2e36  PySimpleGUI>=4.6
+00000510: 300d 0a09 5079 5649 5341 3e3d 312e 3132  0...PyVISA>=1.12
+00000520: 0d0a 0950 7959 414d 4c3e 3d36 2e30 0d0a  ...PyYAML>=6.0..
+00000530: 0974 6b68 746d 6c76 6965 773e 3d30 2e32  .tkhtmlview>=0.2
+00000540: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+00000550: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
+00000560: 7265 203d 2073 7263 0d0a 6578 636c 7564  re = src..exclud
+00000570: 6520 3d20 7465 7374 730d 0a0d 0a5b 6f70  e = tests....[op
+00000580: 7469 6f6e 732e 7061 636b 6167 655f 6461  tions.package_da
+00000590: 7461 5d0d 0a2a 203d 202a 2e6a 736f 6e2c  ta]..* = *.json,
+000005a0: 202a 2e79 616d 6c2c 202a 2e70 6e67 0d0a   *.yaml, *.png..
+000005b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000005c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000005d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.0a0
+Version: 1.1.0b0
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -26,31 +26,32 @@
 # Control.lab.ly
 Lab Equipment Automation Package
 
 ## Description
 User-friendly package that enables flexible automation an reconfigurable setups for high-throughput experimentation and machine learning.
 
 ## Package Structure
-1. Analyse
-2. Compound
-3. Control
-4. Make
-5. Measure
-6. Move
-7. Transfer
-8. View
+1. Compound
+2. Control
+3. Make
+4. Measure
+5. Move
+6. Transfer
+7. View
 
 ## Device support
 - Make
+  - (QInstruments) Bioshake Orbital Shaker
   - Multi-channel LED array \[Arduino\]
   - Multi-channel spin-coater \[Arduino\]
   - Peltier device \[Arduino\]
 - Measure
   - (Keithley) 2450 Source Measure Unit (SMU) Instrument
   - (PiezoRobotics) Dynamic Mechanical Analyser (DMA)
+  - (Sentron) SI series pH meters - *full functionality in development*
   - Precision mass balance \[Arduino\]
 - Move
   - (Creality) Ender-3
   - (Dobot) M1 Pro
   - (Dobot) MG400
   - Primitiv \[Arduino\]
 - Transfer
@@ -59,276 +60,289 @@
   - (TriContinent) C Series syringe pumps
   - Peristaltic pump and syringe system \[Arduino\]
 - View
   - (FLIR) AX8 thermal imaging camera - *full functionality in development*
   - Web cameras \[General\]
 
 ## Installation
-Control.lab.ly can be found on PyPI and can be installed easily with `pip install`.
+Control.lab.ly can be found on PyPI and can be easily installed with `pip install`.
 ```shell
 $ pip install control-lab-ly
 ```
 
 ## Basic Usage
 Simple start-up guide for basic usage of the package.
 
 ### Import desired class
 ```python
 from controllably.Move.Cartesian import Ender
 mover = Ender(...)
 mover.safeMoveTo((x,y,z))
 ```
 
-More details for each class / module / package can be explored by using the `help` function.
+### View documentation
+Use the built-in guide to read the documentation for the package.
 ```python
-help(controllably.Move)   # help on package
-help(Ender)               # help on class
-help(mover)               # help on instance/object
+from controllably import guide_me
+guide_me()
 ```
+![Screenshot of the documentation guide](./assets/Documentation%20guide.png)
 
-Alternatively, you can use the native `pydoc` documentation generator.
-```shell
-$ python -m pydoc controllably.Move
-```
-
->Tip: when using Interactive Python (IPython) (e.g. Jupyter notebooks), add a exclamation mark (`!`) in front of the shell command
+Alternatively, details for each class / module / package can be explored by using the `help` function.
 ```python
->>> !python -m pydoc controllably.Move
->>> !python -m pydoc -b   # Generates a static HTML site to browse package documentation
+help(Ender)
 ```
-For basic usage, this is all you need to know. Check the documentation for more details on each respective class.
+
+For basic usage, this is all you need to know. Check the documentation for more details on each class and function.
 
 ---
 
 ## Advanced Usage
-For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation.
+For more advanced uses, Control.lab.ly provides a host of tools to streamline the development of lab equipment automation. This includes setting up configuration files and adding plugin drivers.
 
-### 0. Import package
-The convention is to import Control-lab-ly as `lab`.
+### Import package
 ```python
 import controllably as lab
 ```
 
-### Contents
-1. Projects
-2. Setups
-3. Decks
-4. Safety measures
-5. Plugins
-
-### 1. Creating a new project
-Create a `/configs` folder in the base folder of your project repository to store all configuration related files from which the package will read from.\
-This only has to be done once when you first set up the project folder.
-```python
-lab.create_configs()
-```
-
-A different address may be used by different machines for the same device. To manage the different addresses used by different machines, you first need your machine's unique identifier.
+Optionally, you can set the safety policy for the session. This feature allows the user to prevent collisions before each movement is made. The safety policy has to be assigned before importing any of the `Mover` objects.
 ```python
-# Get your machine's ID
-print(lab.Helper.get_node())
-```
+lab.set_safety('high')  # Notifies; Pauses for input before every move action
+lab.set_safety('low')   # Notifies; Waits for countdown before every move action
+lab.set_safety(None)    # Movement actions carry out without delay
 
-A template of `registry.yaml` has also been added to the folder to hold the machine-specific addresses of your connected devices (i.e. COM ports).\
-Populate the YAML file in the format shown below.
-```yaml
-### registry.yaml ###
-'012345678901234':          # insert your machine's 15-digit ID here (from the above step)
-    cam_index:              # camera index of the connected imaging devices
-      __cam_01__: 1         # keep the leading and trailing double underscores
-      __cam_02__: 0
-    port:                   # addresses of serial COM ports
-      __device_01__: COM3   # keep the leading and trailing double underscores
-      __device_02__: COM16
+# Import control-lab-ly classes only after setting the safety policy
 ```
 
-To find the COM port address(es) of the device(s) that is/are currently connected to your machine, use:
-```python
-lab.Helper.get_ports()
-```
+### Contents
+1. [Setups](#1-creating-a-new-setup)
+2. [Decks](#2-managing-a-deck)
+3. [Addresses](#3-managing-project-addresses)
+4. [Plugins](#4-using-plugins)
 
-### 2. Creating a new setup
-Create a new folder for the configuration files of your new setup. If you had skipped the previous step of creating a project, calling `lab.create_setup()` will also generate the required file structure. However, be sure to populate your machine ID and device addresses in the `registry.yaml` file.
 
+### 1. Creating a new setup
+Create a `/configs/MySetup` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
 ```python
-lab.create_setup(setup_name = "_Setup01_")
-# replace "_Setup01_" with the desired name for your setup
+lab.create_setup(setup_name = "MySetup")
 ```
-This creates a `/_Setup01_` folder that holds the configuration files for the setup, which includes `config.yaml` and `layout.json`.
 
-#### 2.1 `config.yaml`
-Configuration and calibration values for your devices is stored in `config.yaml`.\
-Each configuration starts with the `name` of your device, then its `module`, `class`, and `settings`.
+#### 1.1 `config.yaml`
+This file stores the configuration and calibration values for your devices.
 ```yaml
-_Device01_:                                     # name of simple device (user-defined)
-  module: _module_name_01_                      # device module
-  class: _submodule_1A_._class_1A_              # device class
+MyDevice:                                       # device name
+  module: Move                                  # top-level category
+  class: Cartesian.Ender                        # device class
   settings:
-    port: __device_01__                         # port addresses defined in registry.yaml
-    _setting_A_: {'tuple': [300,0,200]}         # use keys to define the type of iterable
-    _setting_B_: {'array': [[0,1,0],[-1,0,0]]}  # only tuple and np.array supported
-```
+    port: COM1                                  # serial port address
+    setting_A: {'tuple': [300,0,200]}           # use keys to define the type of iterable
+    setting_B: {'array': [[0,1,0],[-1,0,0]]}    # only tuple and np.array supported
+```
+> Each device configuration starts with the device name, then the following parameters:\
+> `module`: top-level category (such as Make, Measure, Move,Transfer, View)\
+> `class`: point to specific subclass using dot notation\
+> `settings`: various initialisation settings\
+> *See the* [**guide**](#view-documentation) *for more details on these parameters*
 
-`Compound` devices are similarly configured. The configuration values for its component devices are defined under the `component_config` setting. The structure of the configuration values for the component devices are similar to that shown above, except indented to fall under the indentation of the `component_config` setting.
+Compound devices are similarly configured. 
 ```yaml
-_Device02_:                                 # name of 'Compound' device (user-defined)
-  module: Compound                            
-  class: _submodule_2A_._class_2A_
-  settings:
-    _setting_C_: 1                          # other settings for your 'Compound' device
-    component_config:                       # nest component configuration settings here
-      _Component01_:                        # name of component
-        module: _module_name_03_
-        class: _submodule_3A_._class_3A_
-        settings:
-          ip_address: '192.0.0.1'           # IP addresses do not vary between machines
-      _Component02_: 
-        module: _module_name_04_
-        class: _submodule_4A_._class_4A_
-        settings:
-          _setting_D_: 2                    # settings for your component device
+MyCompoundDevice:                         # compound device name
+  module: Compound
+  class: LiquidMover.LiquidMoverSetup
+  settings:                               # settings for your compound device
+    setting_C: True
+    component_config:                     # nest component configuration settings here
+      MyFirstDevice:                      # component device name
+        module: Transfer
+        class: Liquid.SyringeAssembly
+        settings:                         # settings for your component device
+          port: COM22
+          setting_D: 2                    
+      MySecondDevice:                     # component device name
+        module: Mover
+        class: Jointed.Dobot.M1Pro
+        settings:                         # settings for your compound device
+          ip_address: '192.0.0.1'
 ```
+> The configuration values for the component devices are nested under the `component_config` setting of the compound device.
 
-Lastly, you can define shortcuts to quickly access components of `Compound` devices.
+Lastly, you can define shortcuts (or nicknames) to quickly access the components of compound devices.
 ```yaml
 SHORTCUTS:
-  _Nickname1_: '_Device02_._Component01_'
-  _Nickname2_: '_Device02_._Component02_'
+  First: 'MyCompoundDevice.MyFirstDevice'
+  Second: 'MyCompoundDevice.MySecondDevice'
 ```
+> A different serial port address or camera index may be used by different machines for the same device.\
+*See* [**Section 3**](#3-creating-a-new-project) *to find out how to manage the different addresses used by different machines.*
+
+
+#### 1.2 `layout.json`
+This file stores the layout configuration of your physical workspace, also known as a `Deck`.\
+*See* [**Section 2**](#2-managing-a-deck) *on how to load this information into the setup.*
+
+*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a layout configuration may not be required*
+> This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block / object.
 
-#### 2.2 `layout.json`
-Layout configuration of your physical workspace (`Deck`) will be stored in `layout.json`. This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block/object.
 
-*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a layout configuration may not be required.*
 ```json
 {
   "reference_points":{
-    "1": ["_x01_","_y01_","_z01_"],
-    "2": ["_x02_","_y02_","_z02_"]
+    "1": [11.1,22.2,33.3],
+    "2": [44.4,55.5,66.6],
+    "3": [77.7,88.8,99.9]
   },
   "slots":{
     "1": {
-      "name": "_Labware01_",
+      "name": "MyLabware01",
       "exclusion_height": -1,
-      "filepath": "_repo_/.../_Labware01_.json"
+      "filepath": "MyREPO/.../MyLabware01.json"
     },
     "2": {
-      "name": "_Labware02_",
+      "name": "MyLabware02",
       "exclusion_height": 0,
-      "filepath": "_repo_/.../_Labware02_.json"
+      "filepath": "MyREPO/.../MyLabware02.json"
     },
     "3": {
-      "name": "_Labware03_",
+      "name": "MyLabware03",
       "exclusion_height": 10,
-      "filepath": "_repo_/.../_Labware03_.json"
+      "filepath": "MyREPO/.../MyLabware03.json"
     }
   }
 }
 ```
-In `reference_points`, the bottom-left coordinates of each slot in the workspace are defined. Slots are positions where Labware blocks may be placed.
+> In `reference_points`, the bottom-left coordinates of each slot on the deck are defined. Slots are positions where Labware blocks may be placed.
 
-In `slots`, the name of each slot and the file reference for Labware block that occupies that slot are defined. The filepath starts with the repository's base folder name.
+> In `slots`, the `name` of the Labware and the `filepath` to the JSON file containing Labware details are defined. The filepath starts with the name of the repository's base folder.\
+>\
+> The `exclusion_height` is the height (in mm) above the dimensions of the Labware block to steer clear from when performing movement actions. Values less than 0 means the Labware is not avoided.\
+>\
+> *(Note: Labware avoidance only applies to final coordinates (i.e. destination). Does not guarantee collision avoidance when using point-to-point move actions. Use* `safeMoveTo()` *instead.)*
 
-The `exclusion_height` is the height (in mm) above the dimensions of the Labware block to steer clear from when performing move actions. Defaults to -1 (i.e. do not avoid).\
-*(Note: only applies to final coordinates (i.e. destination). Does not guarantee collision avoidance when using point-to-point move actions. Use* `safeMoveTo()` *instead.)*
-
-#### 2.3 Load setup
-The initialisation of the setup occurs during the import `setup` from within `configs/_Setup01_`.
+#### 1.3 Load setup
+The initialisation of the setup occurs when importing `setup` from `configs.MySetup`. With `setup`, you can access all the devices that you have defined in [**Section 1.1**](#11-configyaml).
 
 ```python
+### main.py ###
 # Add repository folder to sys.path
 from pathlib import Path
 import sys
-REPO = '_repo_' 
-# replace "_repo_" with your base directory for the project
+REPO = 'MyREPO'
 ROOT = str(Path().absolute()).split(REPO)[0]
 sys.path.append(f'{ROOT}{REPO}')
 
 # Import the initialised setup
-from configs._Setup01_ import setup
-this = setup
-this._Device01_
-this._Nickname2_
-```
-With `this`, you can access all the devices that you have defined in `configs.yaml`.
-
-### 3. Managing a deck
-*Optional: if your setup does not involve moving objects around in a pre-defined workspace,  a* `Deck` *may not be required.*
-
-#### 3.1 Loading a deck
-To load the `Deck` from the layout file, use the `loadDeck()` function.
-```python
-from configs._Setup01_ import LAYOUT_FILE
-this._Device02_.loadDeck(LAYOUT_FILE)
-deck = this._Device02.deck
+from configs.MySetup import setup
+setup.MyDevice
+setup.First
+```
+
+
+### 2. Managing a deck
+*Optional: if your setup does not involve moving items around in a pre-defined workspace,  a* `Deck` *may not be required*
+
+#### 2.1 Loading a deck
+To load a `Deck` from the layout file, use the `loadDeck()` function of a `Mover` object (or its subclasses).
+```python
+from configs.MySetup import setup, LAYOUT_FILE
+setup.Mover.loadDeck(LAYOUT_FILE)
 ``` 
+> `LAYOUT_FILE` contains the details that has been defined in `layout.json` (see [**Section 1.2**](#12-layoutjson))
 
-#### 3.2 Loading a Labware
-To load the `Labware` into the `Deck`, use the `load_labware()` method.
+#### 2.2 Loading a Labware
+To load a `Labware` onto the deck, use the `load_labware()` method of the `Deck` object.
 ```python
-deck.load_labware(...)
+setup.Mover.deck.load_labware(...)
 ``` 
+> This package uses the same Labware files as those provided by [Opentrons](https://opentrons.com/), which can be found [here](https://labware.opentrons.com/), and custom Labware files can be created [here](https://labware.opentrons.com/create/). Labware files are JSON files that specifies the external and internal dimensions of a Labware block / object.
+
+
+### 3. Managing project addresses
+A `/configs` folder will have been created in the base folder of your project repository to store all configuration related files from which the package will read from, in [**Section 1**](#1-creating-a-new-setup). A template of `registry.yaml` has also been added to the `/configs` folder to manage the machine-specific addresses of your connected devices (e.g. serial port and camera index).
+```yaml
+### registry.yaml ###
+'012345678901234':              # insert your machine's 15-digit ID here
+    cam_index:                  # camera index of the connected imaging devices
+      __cam_01__: 1             # keep the leading and trailing double underscores
+      __cam_02__: 0
+    port:                       # addresses of serial ports
+      __MyDevice__: COM1        # keep the leading and trailing double underscores
+      __MyFirstDevice__: COM22
+```
+
+> Use the `Helper.get_node()` function to get the 15-digit unique identifier of your machine\
+> Use the `Helper.get_port()` function to get the serial port addresses of your connect devices
 
-### 4. Setting up safety measures
-You can optionally set the safety policy for session. This has to be done before importing any of the classes.
 ```python
-lab.set_safety('high')  # Pauses for input before every move action
-lab.set_safety('low')   # Waits for countdown before every move action
-# Import other classes from control-lab-ly only after setting the safety policy
+lab.Helper.get_node()           # Get your machine's ID (15-digit)
+lab.Helper.get_ports()          # Get the port addresses of connected devices
 ```
 
-### 5. Using plugins
-User-defined plugins can be integrated into Control.lab.ly without making additions or modifications to the package itself. All classes and functions can be found in `lab.modules`.
+Afterwards, change the value for the serial port address in the `config.yaml` file to match the registry.
+```yaml
+### config.yaml ###
+MyDevice:
+  module: Move
+  class: Cartesian.Ender
+  settings:
+    port: __MyDevice__          # serial port address
+```
+
+### 4. Using plugins
+*Optional: if drivers for your hardware components are already included, plugins may not be required*
+
+User-defined plugins can be easily written and integrated into Control.lab.ly. All available classes and functions can be found in `lab.modules`.
 ```python
-print(lab.modules)  
-# view the entire package (only those that have been imported during the session)
-lab.modules.Make.Something.Good.myClass
-# this expression returns the registered class
+lab.guide_me()                              # Use guide to view imported objects
+lab.modules.at.Make.Something.Good.MyClass  # Access the the class 
 ```
 
-#### 5.1 Directly registering a Class or Function
+#### 4.1 Registering a Class or Function
 You can import the class and register the object using the `Factory.register()` function.
 ```python
-from my_module import myClass
-lab.Factory.register(myClass, "Make.Something.Good")
+from my_module import MyClass
+lab.Factory.register(MyClass, "Make.Something.Good")
 ```
 
-#### 5.2 Registering a Python module
-Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.\
-Declare a `__where__` global variable to indicate where to register the module.
+#### 4.2 Registering a Python module
+Alternatively, you can automatically register all Classes and Functions in a Python module just by importing it.
+> 1. Declare a `__where__` global variable to indicate where to register the module
+> 2. At the end of the .py file, import and call  the `include_this_module()` function
 ```python
 ### my_module.py ###
-__where__ = "Make.Something.Good"                 # Where to register this module to
-# ==========
-def myClass:                                      # Main body of code goes here
+__where__ = "Make.Something.Good"               # Where to register this module to
+
+def MyClass:                                    # Main body of code goes here
+  ...
+
+def my_function:
   ...
-# ==========
-from controllably import include_this_module      # Registers only the Classes and Functions
-include_this_module()                             # defined above in this .py file
+
+from controllably import include_this_module    # Registers only the Classes and Functions
+include_this_module()                           # defined above in this .py file
 ```
-At the end of the .py file, import and call  the `include_this_module()` function.
 
+The Classes and Functions in the module will be registered when you import the module.
+```python
+### main.py ###
+from my_module import MyClass, my_function
+```
 ---
 
 ## Dependencies
-- Dash (>=2.7.1)
-- Impedance (>=1.4.1)
-- Imutils (>=0.5.4)
-- Matplotlib (>=3.3.4)
-- Nest-asyncio (>=1.5.1)
-- Numpy (>=1.19.5)
-- Opencv-python (>=4.5.4.58)
-- Pandas (>=1.2.4)
-- Plotly (>=5.3.1)
-- PyModbusTCP (>=0.2.0)
-- Pyserial (>=3.5)
-- PySimpleGUI (>=4.60.4)
+- imutils (>=0.5.4)
+- Markdown (>=3.3.4)
+- numpy (>=1.19.5)
+- opencv-python (>=4.5.4.58)
+- pandas (>=1.2.4)
+- pyModbusTCP (>=0.2.0)
+- pyserial (>=3.5)
+- PySimpleGUI (>=4.60.5)
 - PyVISA (>=1.12.0)
 - PyYAML (>=6.0)
-- Scipy (>=1.6.2)
+- tkhtmlview (>=0.2.0)
 
 ## Contributors
 [@kylejeanlewis](https://github.com/kylejeanlewis)\
 [@mat-fox](https://github.com/mat-fox)\
 [@Quijanove](https://github.com/Quijanove)\
 [@AniketChitre](https://github.com/AniketChitre)
 
@@ -340,18 +354,46 @@
 This project is distributed under the [MIT License](https://github.com/kylejeanlewis/control-lab-le/blob/main/LICENSE).
 
 ---
 # Change Log
 
 ## Unreleased
 *Items under development*
-### 1.1.0
-- Integration for orbital shaker \[QInstruments\]
-- Integration for pH meter probe \[Sentron\]
-- Integration for force sensor
+### 1.2.0
+- Integration for mass balance from Sartorius
+
+## Version 1.1.0
+Bug fixes and feature enhancements. First released 15 Jun 2023.
+### Added
+- `ForceSensor` - DIY force sensor (#55)
+- `BioShake` - orbital shaker from QInstruments (#56)
+- `SentronProbe` - pH meter probe from Sentron (#75)
+- `Maker`
+  - added `execute()` abstract method and implemented in subclasses
+- GUI
+  - `Guide` - documentation guide
+  - `MakerPanel` - daptive GUI controls for `Maker` objects (#87)
+### Changed
+- `M1Pro`
+  - fix issue with changing handedness (#86)
+- `Peltier`
+  - rename `getTemperatures()` to `getTemperature()`
+  - rename `isReady()` to `isAtTemperature()`
+  - rename `set_point` to `set_temperature`
+- `Ender`
+  - rename `set_point` to `set_temperature`
+- `TriContinent`
+  - rename `step_limit` to `limits`
+- Refactor and reorganize `GUI` code
+- Refactor code in `helper` and `factory`
+- Updated documentation
+### Removed
+- `Analyse` sub-package removed
+- `Control.Schedule` sub-package removed
+- Unnecessary commented-out blocks of code
 
 
 ## Version 1.0.1
 Bug fixes and minor feature enhancements. First released 08 May 2023.
 ### Added
 - `LiquidMover`
   - Added `LiquidMover.touchTip()` method to touch the pipette tip against the walls of the vessel to remove excess liquid on the outside of the tip (#62)
```

### Comparing `control-lab-ly-1.1.0a0/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,49 +4,44 @@
 setup.cfg
 setup.py
 docs/CHANGELOG.md
 docs/CODE_OF_CONDUCT.md
 docs/CONTRIBUTING.md
 docs/LICENSE.md
 docs/README.md
+docs/assets/Documentation guide.png
 src/control_lab_ly.egg-info/PKG-INFO
 src/control_lab_ly.egg-info/SOURCES.txt
 src/control_lab_ly.egg-info/dependency_links.txt
 src/control_lab_ly.egg-info/requires.txt
 src/control_lab_ly.egg-info/top_level.txt
 src/controllably/__init__.py
-src/controllably/Analyse/__init__.py
-src/controllably/Analyse/Data/__init__.py
-src/controllably/Analyse/Data/Database/__init__.py
-src/controllably/Analyse/Data/Database/database_utils.py
-src/controllably/Analyse/Data/Types/__init__.py
-src/controllably/Analyse/Data/Types/circuit_datatype.py
-src/controllably/Analyse/Data/Types/eis_datatype.py
-src/controllably/Analyse/Data/Types/eis_test_circuits.yaml
-src/controllably/Analyse/Data/Types/eis_tests.json
-src/controllably/Analyse/Visualisation/__init__.py
-src/controllably/Analyse/Visualisation/visualisation_utils.py
 src/controllably/Compound/__init__.py
 src/controllably/Compound/compound_utils.py
 src/controllably/Compound/LiquidMover/__init__.py
 src/controllably/Compound/LiquidMover/liquidmover_utils.py
 src/controllably/Compound/LiquidMover/Opentrons/__init__.py
 src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
 src/controllably/Control/__init__.py
 src/controllably/Control/GUI/__init__.py
 src/controllably/Control/GUI/_guibuilder.py
 src/controllably/Control/GUI/compound_panel.py
 src/controllably/Control/GUI/gui_utils.py
-src/controllably/Control/GUI/liquid_panel.py
-src/controllably/Control/GUI/loader_panel.py
-src/controllably/Control/GUI/measurer_panel.py
-src/controllably/Control/GUI/mover_panel.py
-src/controllably/Control/GUI/viewer_panel.py
-src/controllably/Control/Schedule/__init__.py
-src/controllably/Control/Schedule/schedule_utils.py
+src/controllably/Control/GUI/guide_panel.py
+src/controllably/Control/GUI/multichannel_panel.py
+src/controllably/Control/GUI/Basic/__init__.py
+src/controllably/Control/GUI/Basic/maker_panel.py
+src/controllably/Control/GUI/Basic/measurer_panel.py
+src/controllably/Control/GUI/Basic/mover_panel.py
+src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
+src/controllably/Control/GUI/Basic/viewer_panel.py
+src/controllably/Control/GUI/Elements/__init__.py
+src/controllably/Control/GUI/Elements/loader_panel.py
+src/controllably/Control/GUI/Elements/pop_ups.py
+src/controllably/Control/GUI/Elements/templates.py
 src/controllably/Make/__init__.py
 src/controllably/Make/make_utils.py
 src/controllably/Make/Heat/__init__.py
 src/controllably/Make/Heat/peltier_utils.py
 src/controllably/Make/Light/__init__.py
 src/controllably/Make/Light/led_utils.py
 src/controllably/Make/Mixture/__init__.py
@@ -75,14 +70,15 @@
 src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
 src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
 src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
 src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
 src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
 src/controllably/Measure/Physical/__init__.py
 src/controllably/Measure/Physical/balance_utils.py
+src/controllably/Measure/Physical/force_sensor_utils.py
 src/controllably/Move/__init__.py
 src/controllably/Move/move_utils.py
 src/controllably/Move/Cartesian/__init__.py
 src/controllably/Move/Cartesian/cartesian_utils.py
 src/controllably/Move/Cartesian/ender_utils.py
 src/controllably/Move/Cartesian/primitiv_utils.py
 src/controllably/Move/Jointed/__init__.py
@@ -110,15 +106,15 @@
 src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
 src/controllably/Transfer/Powder/__init__.py
 src/controllably/Transfer/Substrate/__init__.py
 src/controllably/Transfer/Substrate/substrate_utils.py
 src/controllably/Transfer/Substrate/Dobot/__init__.py
 src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
 src/controllably/View/__init__.py
-src/controllably/View/image_utils.py
+src/controllably/View/image.py
 src/controllably/View/view_utils.py
 src/controllably/View/Classifiers/__init__.py
 src/controllably/View/Classifiers/classifier_utils.py
 src/controllably/View/Optical/__init__.py
 src/controllably/View/Optical/optical_utils.py
 src/controllably/View/Optical/placeholders/__init__.py
 src/controllably/View/Optical/placeholders/optical_camera.png
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     Args:
         `config` (Optional[str], optional): filename of config .yaml file. Defaults to None.
         `layout` (Optional[str], optional): filename of layout .json file. Defaults to None.
         `component_config` (Optional[dict], optional): configuration dictionary of component settings. Defaults to None.
         `layout_dict` (Optional[dict], optional): dictionary of layout. Defaults to None.
         `components` (Optional[dict], optional): dictionary of components. Defaults to None.
         `tip_approach_height` (float, optional): height in mm from which to approach tip rack during pick up. Defaults to 20.
-        
+    
     ### Attributes
     - `tip_approach_height` (float): height in mm from which to approach tip rack during tip pickup
     
     ### Properties
     - `liquid` (Liquid): liquid transfer tool
     - `mover` (Mover): movement / translation robot
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Compound/compound_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 # Standard library imports
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from typing import Optional
 
 # Local application imports
-from ..misc import Factory, Layout
+from ..misc import Factory, Helper, Layout
 print(f"Import: OK <{__name__}>")
 
 class CompoundSetup(ABC):
     """
     Abstract Base Class (ABC) for CompoundSetup objects (i.e. compound tools that combine multiple basic tools).
     ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
     
@@ -73,15 +73,15 @@
             verbose (bool, optional): verbosity of class. Defaults to False.
         """
         self.components = {} if components is None else components
         self.deck = Layout.Deck()
         self.flags = self._default_flags.copy()
         self.positions = {}
         self.verbose = verbose
-        self._config = Factory.get_plans(config) if config is not None else component_config
+        self._config = Helper.get_plans(config) if config is not None else component_config
 
         self._connect(diagnostic=diagnostic)
         self.loadDeck(layout_file=layout, layout_dict=layout_dict)
         pass
     
     @abstractmethod
     def reset(self, *args, **kwargs):
@@ -140,16 +140,17 @@
         Set flags by using keyword arguments
 
         Kwargs:
             key, value: (flag name, boolean) pairs
         """
         if not all([type(v)==bool for v in kwargs.values()]):
             raise ValueError("Ensure all assigned flag values are boolean.")
-        for key, value in kwargs.items():
-            self.flags[key] = value
+        self.flags.update(kwargs)
+        # for key, value in kwargs.items():
+        #     self.flags[key] = value
         return
     
     def setPosition(self, overwrite:bool = False, **kwargs):
         """
         Set predefined positions using keyword arguments
 
         Args:
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """
-This sub-package imports the base class for control panels as well as basic panels
-for measurers, movers, and viewers.
+This sub-package imports the basic panels for makers, measurers, movers, liquid transfers, and viewers.
 
 Classes:
-    Panel (ABC)
-    CompoundPanel (Panel)
-    LiquidPanel (Panel)
+    LiquidPanel (MultiChannelPanel)
+    MakerPanel (MultiChannelPanel)
     MeasurerPanel (Panel)
     MoverPanel (Panel)
-    MultiChannelPanel (Panel)
     ViewerPanel (Panel)
 """
-from .gui_utils import Panel, MultiChannelPanel
-from .compound_panel import CompoundPanel
-from .liquid_panel import LiquidPanel
+from .maker_panel import MakerPanel
 from .measurer_panel import MeasurerPanel
 from .mover_panel import MoverPanel
+from .transfer_liquid_panel import LiquidPanel
 from .viewer_panel import ViewerPanel
 
 from controllably import include_this_module
 include_this_module(get_local_only=False)
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/compound_panel.py` & `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/compound_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # %% -*- coding: utf-8 -*-
 """
-This module holds the base class compound panels.
+This module holds the base class for compound panels.
 
 Classes:
     CompoundPanel (Panel)
 """
 # Standard library imports
 from __future__ import annotations
 from collections import OrderedDict
@@ -22,15 +22,15 @@
     CompoundPanel provides methods to form a multi-tool control panel
 
     ### Constructor
     Args:
         `ensemble` (dict[str, Panel]): dictionary of individual sub-panels
         `name` (str, optional): name of panel. Defaults to ''.
         `group` (Optional[str], optional): name of group. Defaults to None.
-        
+    
     ### Attributes
     - `panels` (dict[str, Panel]): dictionary of individual sub-panels
     
     ### Methods
     - `close`: exit the application
     - `getLayout`: build `sg.Column` object
     - `listenEvents`: listen to events and act on values
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/gui_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # %% -*- coding: utf-8 -*-
 """
-This module holds the base class for control panels as well as multichannel panels.
+This module holds the base class for control panels.
 
 Classes:
     Panel (ABC)
-    MultiChannelPanel (Panel)
-    
+
 Other constants and variables:
     HEIGHT (int): height of screen size in number of pixels
     WIDTH (int): width of screen size in number of pixels
 """
 # Standard library imports
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from collections import OrderedDict
 from typing import Optional, Union
 
 # Third party imports
-import PySimpleGUI as sg # pip install PySimpleGUI
+import PySimpleGUI as sg                                            # pip install PySimpleGUI
 from PySimpleGUI import WIN_CLOSED, WINDOW_CLOSE_ATTEMPTED_EVENT
 
 # Local application imports
 print(f"Import: OK <{__name__}>")
 
 WIDTH, HEIGHT = sg.Window.get_screen_size()
 
@@ -33,15 +31,15 @@
     ### Constructor
     Args:
         `name` (str, optional): name of panel. Defaults to ''.
         `group` (Optional[str], optional): name of group. Defaults to None.
         `font_sizes` (tuple[int], optional): list of font sizes. Defaults to (14,12,10,8,6).
         `theme` (str, optional): name of theme. Defaults to 'LightGreen'.
         `typeface` (str, optional): name of typeface. Defaults to "Helvetica".
-
+    
     ### Attributes
     #### Class
     - `font_sizes` (tuple[int]): list of font sizes
     - `theme` (str): name of theme
     - `typeface` (str): name of typeface
     #### Instance
     - `flags` (dict[str, bool]): keywords paired with boolean flags
@@ -261,41 +259,57 @@
                     kw[k] = v
             label = texts[i] if i<len(texts) else label
             tooltip = tooltips[i] if i<len(tooltips) else None
             buttons.append(sg.Button(label, size=size, key=key, font=font, tooltip=tooltip, **kw))
         return buttons
     
     @staticmethod
-    def getInputs(fields:list[str], key_prefix: str) -> list[sg.Column]:
+    def getInputs(
+            fields: list[str], 
+            key_prefix: str, 
+            initial_visibility: bool = True, 
+            label_map: Optional[dict] = None,
+            defaults: Optional[dict] = None,
+            tooltips: Optional[dict] = None,
+            **kwargs
+        ) -> list[sg.Column]:
         """
         Get the layout for the input section
         
         Args:
             fields (list[str]): list of field names
             key_prefix (str): prefix of button key
+            initial_visibility (bool, optional): whether the field is initially visible. Defaults to True.
+            label_map (Optional[dict], optional): text label for each field. Defaults to None.
+            defaults (Optional[dict], optional): default value for each field. Defaults to None.
+            tooltips (Optional[dict], optional): tooltip for each field. Defaults to None.
 
         Returns:
             list[sg.Column]: list of columns
         """
         # template for procedurally adding input fields
         labels = []
         inputs = []
         for input_field in fields:
             key_label = f'-{key_prefix}-{input_field.upper()}-LABEL-'
             key_input = f'-{key_prefix}-{input_field.upper()}-VALUE-'
+            label = label_map.get(input_field, input_field.title()) if type(label_map) is dict else input_field.title()
+            default = defaults.get(input_field, '') if type(defaults) is dict else ''
+            tooltip = tooltips.get(input_field, None) if type(tooltips) is dict else None
+            
             _label = sg.pin(
                 sg.Column(
-                    [[sg.Text(input_field.title(), key=key_label, visible=True)]],
-                    key=f'{key_label}BOX-', visible=True
+                    [[sg.Text(label, key=key_label, visible=True, tooltip=tooltip)]],
+                    key=f'{key_label}BOX-', visible=initial_visibility
                 )
             )
             _input = sg.pin(
                 sg.Column(
-                    [[sg.Input(size=(5,2), key=key_input, visible=True, tooltip='')]],
-                    key=f'{key_input}BOX-', visible=True
+                    [[sg.Input(default, size=(5,2), key=key_input, visible=True, tooltip=tooltip)]],
+                    key=f'{key_input}BOX-', visible=initial_visibility
                 )
             )
             labels.append([_label])
             inputs.append([_input])
         labels_column = sg.Column(labels, justification='right', pad=10, visible=True)
         inputs_column = sg.Column(inputs, justification='left', pad=10, visible=True)
         labels_inputs = [labels_column, inputs_column]
@@ -327,44 +341,54 @@
         ele = sg.Text('', size=(1,1))
         try:
             ele = sg.Push()
         except Exception as e:
             print(e)
         return ele
     
-    @staticmethod
-    def parseInput(text:str) -> list[Union[float, str]]:
+    @classmethod
+    def parseInput(cls, text:str) -> Union[list, bool, float, str, None]:
         """
         Parse inputs from GUI
 
         Args:
             text (str): input text read from GUI window
 
         Returns:
-            list[Union[float, str]]: variable output including floats, strings, and tuples
+            Union[list, bool, float, str, None]: variable output including floats, strings, and tuples
         """
+        text = text.strip()
+        if len(text) == 0:
+            return None
+        
+        array = []
         if ',' in text:
-            strings = text.split(',')
+            array = text.split(',')
         elif ';' in text:
-            strings = text.split(';')
-        else:
-            try:
-                text = float(text)
-                return text
-            finally:
-                # return text
-                pass
-        output = []
-        for text in strings:
-            try:
-                output.append(float(text))
-            except ValueError:
-                # output.append(text)
-                pass
-        return output
+            array = text.split(';')
+        if len(array):
+            new_array = []
+            for value in array:
+                new_array.append(cls.parseInput(value))
+            return new_array
+        
+        if text.replace('.','',1).replace('-','',1).isdigit():
+            if '.' in text:
+                return float(text)
+            else:
+                return int(text)
+        
+        if text.title() == "True":
+            return True
+        if text.title() == "False":
+            return False
+        
+        if text[0] in ("'", '"') and text[-1] in ("'", '"'):
+            return text[1:-1]
+        return text
     
     def runGUI(self, title:str = 'Application', maximize:bool = False):
         """
         Run the GUI loop
 
         Args:
             title (str, optional): title of window. Defaults to 'Application'.
@@ -387,16 +411,17 @@
         Set flags by using keyword arguments
 
         Kwargs:
             key, value: (flag name, boolean) pairs
         """
         if not all([type(v)==bool for v in kwargs.values()]):
             raise ValueError("Ensure all assigned flag values are boolean.")
-        for key, value in kwargs.items():
-            self.flags[key] = value
+        self.flags.update(kwargs)
+        # for key, value in kwargs.items():
+        #     self.flags[key] = value
         return
 
     # Protected method(s)
     def _loop_gui(self):
         """Loop GUI process"""
         if type(self.window) == type(None):
             return
@@ -420,93 +445,7 @@
         Args:
             text (str): text to be mangled
 
         Returns:
             str: mangled text
         """
         return f'-{self.name}{text}'
-    
-
-class MultiChannelPanel(Panel):
-    """
-    Abstract Base Class (ABC) for Multi-Channel Panel objects (i.e. GUI panels for tools with multiple channels).
-    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
-
-    ### Constructor
-    Args:
-        `name` (str, optional): name of panel. Defaults to ''.
-        `group` (Optional[str], optional): name of group. Defaults to None.
-    
-    ### Methods
-    #### Abstract
-    - `getChannelPanel`: get the panel layout for a single channel
-    - `listenEvents`: listen to events and act on values
-    #### Public
-    - `getLayout`: build `sg.Column` object
-    """
-    
-    def __init__(self, name:str = '', group:Optional[str] = None):
-        """
-        Instantiate the class
-
-        Args:
-            name (str, optional): name of panel. Defaults to ''.
-            group (Optional[str], optional): name of group. Defaults to None.
-        """
-        super().__init__(name=name, group=group)
-        return
-    
-    @abstractmethod
-    def getChannelPanel(self, channel_id:int, tool:object, **kwargs) -> sg.Column:
-        """
-        Get the panel layout for a single channel
-
-        Args:
-            channel_id (int): channel index
-            tool (object): tool object
-
-        Returns:
-            sg.Column: Column object
-        """
-        
-    def getLayout(self, title:str = 'Tool Control', title_font_level:int = 1, **kwargs) -> sg.Column:
-        """
-        Build `sg.Column` object
-
-        Args:
-            title (str, optional): title of layout. Defaults to 'Tool Control'.
-            title_font_level (int, optional): index of font size from levels in `font_sizes`. Defaults to 1.
-
-        Returns:
-            sg.Column: Column object
-        """
-        font = (self.typeface, self.font_sizes[title_font_level])
-        layout = super().getLayout(title, justification='center', font=font)
-        channels = {}
-        if 'channels' in dir(self.tool):
-            channels = self.tool.channels
-        else:
-            channels = {self.tool.channel: self.tool}
-        if len(channels) == 0:
-            return layout
-        
-        channel_panels = []
-        for channel_id, tool in channels.items():
-            _layout = self.getChannelPanel(channel_id, tool)
-            channel_panels.append((channel_id, _layout))
-        if len(channel_panels) == 1:
-            panel = channel_panels[0][1]
-        else:
-            tabs = [sg.Tab(key, [[_layout]], expand_x=True) for key,_layout in channel_panels]
-            panel = sg.TabGroup(
-                [tabs], tab_location='topleft', key=f'-{self.name}-TABS-', 
-                expand_x=True, expand_y=True
-            )
-        
-        suite = sg.Column([[panel]], vertical_alignment='top')
-        layout = [
-            [layout],
-            [sg.Push()],
-            [suite]
-        ]
-        layout = sg.Column(layout, vertical_alignment='top')
-        return layout
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/liquid_panel.py` & `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from threading import Thread
 from typing import Callable, Protocol
 
 # Third party imports
 import PySimpleGUI as sg    # pip install PySimpleGUI
 
 # Local application imports
-from .gui_utils import MultiChannelPanel
+from ..multichannel_panel import MultiChannelPanel
 print(f"Import: OK <{__name__}>")
 
 class Liquid(Protocol):
     capacity: float
     channel: int
     reagent: str
     volume: float
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/loader_panel.py` & `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/loader_panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import time
 from typing import Protocol, Callable
 
 # Third party imports
 import PySimpleGUI as sg # pip install PySimpleGUI
 
 # Local application imports
-from ...misc import Helper
-from .gui_utils import Panel
+from ....misc import Helper
+from ..gui_utils import Panel
 print(f"Import: OK <{__name__}>")
 
 class LoaderPanel(Panel):
     """
     Loader Panel class
 
     Args:
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/measurer_panel.py` & `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/measurer_panel.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from dataclasses import dataclass, field
 from typing import Protocol, Callable, Any
 
 # Third party imports
 import PySimpleGUI as sg # pip install PySimpleGUI
 
 # Local application imports
-from .gui_utils import Panel
+from .... import modules
+from ..gui_utils import Panel
 print(f"Import: OK <{__name__}>")
 
 @dataclass
 class ProgramDetails:
     """
     ProgramDetails dataclass represents the set of inputs, default values, truncated docstring and tooltip of a program class.
     <from `controllably.Measure.program_utils`>
@@ -34,16 +35,15 @@
     
     inputs: list[str] = field(default_factory=lambda: [])
     defaults: dict[str, Any] = field(default_factory=lambda: {})
     short_doc: str = ''
     tooltip: str = ''
 
 class Measurer(Protocol):
-    available_programs: tuple[str]      # FIXME
-    possible_inputs: tuple[str]         # FIXME
+    _place: str
     program_details: ProgramDetails
     program_type: Callable
     def loadProgram(self, *args, **kwargs):
         ...
     def measure(self, *args, **kwargs):
         ...
     def reset(self, *args, **kwargs):
@@ -54,26 +54,28 @@
     Measurer Panel class
 
     ### Constructor
     Args:
         `measurer` (Measurer): Measurer object
         `name` (str, optional): name of panel. Defaults to 'MEASURE'.
         `group` (str, optional): name of group. Defaults to 'measurer'.
-        
+    
     ### Attributes
     - `current_program` (str): currently active program
+    - `input_map` (dict[int, Optional[str]]): enumerated map of program inputs
     
     ### Properties
     - `measurer` (Measurer): alias for `tool`
     
     ### Methods
     - `getLayout`: build `sg.Column` object
     - `listenEvents`: listen to events and act on values
     """
     
+    _default_input_map: dict = {f"INPUT-{i:02}": None for i in range(20)}
     def __init__(self, 
         measurer: Measurer, 
         name: str = 'MEASURE', 
         group: str = 'measurer', 
         **kwargs
     ):
         """
@@ -83,44 +85,46 @@
             measurer (Measurer): Measurer object
             name (str, optional): name of panel. Defaults to 'MEASURE'.
             group (str, optional): name of group. Defaults to 'measurer'.
         """
         super().__init__(name=name, group=group, **kwargs)
         self.tool = measurer
         self.current_program = ''
+        self.input_map = self._default_input_map
         return
     
     # Properties
     @property
     def measurer(self) -> Measurer:
         return self.tool
     
     def getLayout(self, title_font_level:int = 0, **kwargs) -> sg.Column:
         """
         Build `sg.Column` object
 
         Args:
-            title (str, optional): title of layout. Defaults to 'Panel'.
             title_font_level (int, optional): index of font size from levels in font_sizes. Defaults to 0.
 
         Returns:
             sg.Column: Column object
         """
         font = (self.typeface, self.font_sizes[title_font_level])
         layout = super().getLayout(f'{self.name.title()} Control', justification='center', font=font)
         
         font = (self.typeface, self.font_sizes[title_font_level+1])
         # add dropdown for program list
+        programs = eval(f"modules.at.{self.measurer._place}.programs")
+        program_names = [p for p in programs if p != "_doc_"]
         dropdown = sg.Combo(
-            values=self.measurer.available_programs, size=(20, 1), 
+            values=program_names, size=(20, 1), 
             key=self._mangle('-PROGRAMS-'), enable_events=True, readonly=True
         )
         
         # add template for procedurally adding input fields
-        labels_inputs = self.getInputs(fields=self.measurer.possible_inputs, key_prefix=self.name)
+        labels_inputs = self.getInputs(fields=[i for i in self.input_map], key_prefix=self.name, initial_visibility=False)
         
         # add run, clear, reset buttons
         layout = [
             [layout],
             [self.pad()],
             [sg.Column([[dropdown]], justification='center')],
             [self.pad()],
@@ -144,29 +148,30 @@
             dict: dictionary of updates
         """
         updates = {}
         # 1. Select program
         if event == self._mangle('-PROGRAMS-'):
             selected_program = values[self._mangle('-PROGRAMS-')]       # COMBO
             if selected_program != self.current_program:
-                self.measurer.loadProgram(selected_program)
+                self.measurer.loadProgram(eval(f"modules.at.{self.measurer._place}.programs.{selected_program}"))
                 update_part = self._show_inputs(self.measurer.program_details)
                 updates.update(update_part)
             self.current_program = selected_program
         
         # 2. Start measure
         if event == self._mangle('-Run-'):
             if self.measurer.program_type is not None:
                 print('Start measure')
                 parameters = {}
-                for input_field in self.measurer.program_details.inputs:
-                    key = self._mangle(f'-{input_field}-VALUE-')
-                    if key in values.keys():
-                        value = self.parseInput(values[key])
-                        parameters[input_field] = value
+                for key, input_field in self.input_map.items():
+                    if input_field is None:
+                        break
+                    key_input = self._mangle(f'-{key}-VALUE-')
+                    value = self.parseInput(values[key_input])
+                    parameters[input_field] = value
                 print(parameters)
                 self.measurer.measure(parameters=parameters)
             else:
                 print('Please select a program first.')
         
         # 3. Reset measurer
         if event == self._mangle('-Reset-'):
@@ -187,19 +192,26 @@
         Args:
             program_details (ProgramDetails): details of loaded program
 
         Returns:
             dict: dictionary of updates
         """
         updates = {}
-        for input_field in self.measurer.possible_inputs:
-            key_label = self._mangle(f'-{input_field}-LABEL-')
-            key_input = self._mangle(f'-{input_field}-VALUE-')
+        self.input_map = self._default_input_map
+        for key_id, input_field in enumerate(program_details.inputs):
+            self.input_map[f"INPUT-{key_id:02}"] = input_field
+        
+        for key, input_field in self.input_map.items():
+            key_label = self._mangle(f'-{key}-LABEL-')
+            key_input = self._mangle(f'-{key}-VALUE-')
             updates[f'{key_label}BOX-'] = dict(visible=False)
             updates[f'{key_input}BOX-'] = dict(visible=False)
+            if input_field is None:
+                continue
             if input_field in program_details.inputs:
-                updates[key_label] = dict(tooltip=program_details.tooltip)
+                updates[key_label] = dict(tooltip=program_details.tooltip,
+                                          value=input_field.title())
                 updates[key_input] = dict(tooltip=program_details.tooltip, 
-                                          value=program_details.get(input_field,''))
+                                          value=program_details.defaults.get(input_field,''))
                 updates[f'{key_label}BOX-'] = dict(visible=True)
                 updates[f'{key_input}BOX-'] = dict(visible=True)
         return updates
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/mover_panel.py` & `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/mover_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,64 +3,63 @@
 This module holds the class for mover control panels.
 
 Classes:
     MoverPanel (Panel)
 """
 # Standard library imports
 from __future__ import annotations
+import inspect
 import numpy as np
-from typing import Callable, Optional, Protocol, Union
+from typing import Optional, Protocol, Union
 
 # Third party imports
 import PySimpleGUI as sg # pip install PySimpleGUI
 
 # Local application imports
-from ...misc import Factory, Helper
-from .gui_utils import Panel
+from ....misc import Helper, modules
+from ..gui_utils import Panel
 print(f"Import: OK <{__name__}>")
 
+MAX_FUNCTION_BUTTONS = 7
+
 class Mover(Protocol):
-    # attachment: Callable
+    _place: str
     heights: dict
     home_coordinates: tuple
-    max_actions: int
-    possible_attachments: list
     tool_position: tuple(np.ndarray, np.ndarray)
     def home(self, *args, **kwargs):
         ...
     def move(self, *args, **kwargs):
         ...
     def moveTo(self, *args, **kwargs):
         ...
     def reset(self, *args, **kwargs):
         ...
     def rotateTo(self, *args, **kwargs):
         ...
-    # def toggleAttachment(self, *args, **kwargs):
-    #     ...
     def _transform_out(self, *args, **kwargs):
         ...
         
 class MoverPanel(Panel):
     """
     MoverPanel provides methods to create a control panel for a mover
 
     ### Constructor
     Args:
         `mover` (Mover): Mover object
         `name` (str, optional): name of panel. Defaults to 'MOVE'.
         `group` (str, optional): name of group. Defaults to 'mover'.
         `axes` (Union[list, str], optional): available axes of motion. Defaults to 'XYZabc'.
-        
+    
     ### Attributes
     - `attachment_methods` (list[str]): list of methods available to attachment
     - `axes` (list[str]): list of available axes of motion
     - `buttons` (dict[str, tuple[str, float]]) : dictionary of {button id, (axes, value)}
     - `current_attachment` (str): name of current attachment
-    - `methods_fn_key_map` (dict[str, str]): dictionary of {button id, button label} 
+    - `method_map` (dict[str, str]): dictionary of {button id, button label} 
     
     ### Properties
     - `mover` (Mover): alias for `tool`
     
     ### Methods
     - `getLayout`: build `sg.Column` object
     - `listenEvents`: listen to events and act on values
@@ -85,15 +84,15 @@
         super().__init__(name=name, group=group, **kwargs)
         self.tool = mover
         
         self.axes = [*axes]
         self.buttons = {}
         self.current_attachment = ''
         self.attachment_methods = []
-        self.methods_fn_key_map = {}
+        self.method_map = {}
         
         self.flags['update_position'] = True
         return
     
     # Properties
     @property
     def mover(self) -> Mover:
@@ -247,34 +246,46 @@
         
         # 6. Reset mover
         if event == self._mangle(f'-Reset-'):
             self.mover.reset()
             tool_position = cache_position
             
         # 7. Function buttons for attachment
-        if event in self.methods_fn_key_map:
-            fn_name = self.methods_fn_key_map[event].lower()
+        if event in self.method_map:
+            fn_name = self.method_map[event].lower()
             print(fn_name)
             action = getattr(self.mover.attachment, fn_name, None)
             if callable(action):
                 action()
                 
         # 8. Select attachment
         if event == self._mangle('-ATTACH-'):
-            selected_attachment = values[self._mangle('-ATTACH-')]         # COMBO
-            if selected_attachment != self.current_attachment:
-                if selected_attachment == 'None':
+            selected_attachment = values[self._mangle('-ATTACH-')]                                      # Drop-down list
+            if selected_attachment != self.current_attachment:                                          # Only when there is a change
+                if selected_attachment == 'None':                                                       # If None selected, remove attachment
                     selected_attachment = ''
                     self.mover.toggleAttachment(False)
                     self.attachment_methods = []
                     update_part = self._toggle_buttons(False)
-                else:
-                    selected_attachment_class = Factory.get_class(f"Transfer.Substrate.Dobot.{selected_attachment}")     ### FIXME: hard-coded
+                else:                                                                                   # Find and attach selected attachment
+                    selected_attachment_class = eval(
+                        f"modules.at.{self.mover._place}.attachments.{selected_attachment}"
+                    )
                     self.mover.toggleAttachment(True, selected_attachment_class)
-                    self.attachment_methods = [method for method in Helper.get_method_names(self.mover.attachment) if not method.startswith('_')]
+                    methods = []
+                    for method in Helper.get_method_names(self.mover.attachment):                       # Find methods to surface as function buttons
+                        if method.startswith('_'):
+                            continue
+                        signature = inspect.signature(getattr(self.mover.attachment, method))
+                        parameters = dict(signature.parameters)
+                        parameters.pop('self', None)
+                        if any([(p.default == inspect.Parameter.empty) for p in list(parameters.values())]):
+                            continue
+                        methods.append(method)
+                    self.attachment_methods = methods
                     fn_buttons = [l.title() for l in self.attachment_methods]
                     update_part = self._toggle_buttons(True, fn_buttons)
                 updates.update(update_part)
             self.current_attachment = selected_attachment
         
         # 9. Update position
         if self.flags['update_position']:
@@ -296,64 +307,67 @@
         Returns:
             sg.Column: column of labelled buttons if there is an attachment, else placeholder buttons
         """
         show_section = False
         show_buttons = False
         alt_texts = []
         fn_layout = []
-        button_labels = [f'FN{i+1}' for i in range(max(self.mover.max_actions,5))]  # Placeholder buttons
+        button_labels = [f'FN{i+1}' for i in range(MAX_FUNCTION_BUTTONS)]  # Placeholder buttons
         if 'attachment' in dir(self.mover):
+            attachments = eval(f"modules.at.{self.mover._place}.attachments")
+            attachment_names = [a for a in attachments if a != "_doc_"]
+            
             show_section = True
             default_value = self.mover.attachment.__class__.__name__ if self.mover.attachment is not None else 'None'
             dropdown = sg.Combo(
-                values=self.mover.possible_attachments+['None'], default_value=default_value,
+                values=['None']+attachment_names, default_value=default_value,
                 size=(20, 1), key=self._mangle('-ATTACH-'), enable_events=True, readonly=True
             )
             dropdown_column = sg.Column([[dropdown]], justification='center')
             fn_layout.append([dropdown_column])
             fn_layout.append([self.pad()])
             if self.mover.attachment is not None:
                 show_buttons = True
                 self.current_attachment = self.mover.attachment.__class__.__name__
                 self.attachment_methods = [method for method in Helper.get_method_names(self.mover.attachment) if not method.startswith('_')]
                 alt_texts = [l.title() for l in self.attachment_methods]
-                self.methods_fn_key_map = {f'-{self.name}-{k}-':v for k,v in zip(button_labels, alt_texts)}
+                self.method_map = {f'-{self.name}-{k}-':v for k,v in zip(button_labels, alt_texts)}
         buttons = self.getButtons(button_labels, (5,2), self.name, font, texts=alt_texts)
         buttons = [sg.pin(button) for button in buttons]
         buttons_column = sg.Column([buttons], justification='center', visible=show_buttons, key=self._mangle('-FN-BUTTONS-'))
         fn_layout.append([buttons_column])
         
         column = sg.Column(fn_layout, justification='center', visible=show_section)
         return column
      
     def _toggle_buttons(self, on:bool, active_buttons:Optional[list[str]] = None) -> dict[str, dict]:
         """
-        Toggle between shown the function buttons for attachment
+        Toggle between showing the function buttons for attachment
 
         Args:
             on (bool): whether to show buttons
             active_buttons (Optional[list[str]], optional): list of method names. Defaults to None.
 
         Returns:
             dict: dictionary of updates
         """
         updates = {}
-        self.methods_fn_key_map = {}
+        self.method_map = {}
         # Hide all buttons
         if not on:
             updates[self._mangle('-FN-BUTTONS-')] = dict(visible=False)
             return updates
         if active_buttons is None:
             return updates
         
         # Show buttons and change labels
         updates[self._mangle('-FN-BUTTONS-')] = dict(visible=True)
         for i,method in enumerate(active_buttons):
             key_button = self._mangle(f'-FN{i+1}-')
             updates[key_button] = dict(visible=True, text=method)
-            self.methods_fn_key_map[key_button] = method
+            self.method_map[key_button] = method
         
         # Hide remaining buttons
-        for j in range(i+1, max(self.mover.max_actions,5)):
+        for j in range(len(active_buttons), MAX_FUNCTION_BUTTONS):
             key_button = self._mangle(f'-FN{j+1}-')
             updates[key_button] = dict(visible=False, text=f'FN{j+1}')
         return updates
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Control/GUI/viewer_panel.py` & `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/viewer_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from typing import Protocol
 
 # Third party imports
 import cv2              # pip install opencv-python
 import PySimpleGUI as sg # pip install PySimpleGUI
 
 # Local application imports
-from .gui_utils import Panel
+from ..gui_utils import Panel
 print(f"Import: OK <{__name__}>")
 
 class Viewer(Protocol):
     def getImage(self, *args, **kwargs):
         ...
     def shutdown(self, *args, **kwargs):
         ...
@@ -29,15 +29,15 @@
     ViewerPanel provides methods to create a control panel for a viewer
     
     ### Constructor
     Args:
         `viewer` (Viewer): Viewer object
         `name` (str, optional): name of panel. Defaults to 'VIEW'.
         `group` (str, optional): name of group. Defaults to 'viewer'.
-
+    
     ### Attributes
     - `display_box` (str): element id
     
     ### Properties
     - `viewer` (Viewer): alias for `tool`
     
     ### Methods
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Make/Heat/peltier_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,27 +31,29 @@
 
     ### Constructor
     Args:
         `port` (str): COM port of device
         `power_threshold` (float, optional): minimum threshold under which temperature can be considered stable. Defaults to 20.
         `stabilize_buffer_time` (float, optional): buffer time over which temperature can be considered stable. Defaults to 10.
         `tolerance` (float, optional): tolerance above and below target temperature. Defaults to 1.5.
-            
+    
     ### Attributes
+    - `buffer_df` (pd.DataFrame): buffer dataframe to store collected data
     - `power_threshold` (float): minimum threshold under which temperature can be considered stable
     - `set_temperature` (float): temperature set point
     - `stabilize_buffer_time` (float): buffer time over which temperature can be considered stable
     - `temperature` (float): temperature at sample site
     - `tolerance` (float): tolerance above and below target temperature
     
     ### Properties
     - `port`: COM port of device
     
     ### Methods
     - `clearCache`: clears and remove data in buffer
+    - `execute`: alias for `holdTemperature()`
     - `getTemperature`: retrieve temperatures from device
     - `holdTemperature`: hold target temperature for desired duration
     - `isAtTemperature`: checks and returns whether target temperature has been reached
     - `reset`: reset the device
     - `setTemperature`: set a target temperature
     - `shutdown`: shutdown procedure for tool
     - `toggleFeedbackLoop`: start or stop feedback loop
@@ -110,14 +112,26 @@
         """Clears and remove data in buffer"""
         self.setFlag(pause_feedback=True)
         time.sleep(0.1)
         self.buffer_df = pd.DataFrame(columns=self._columns)
         self.setFlag(pause_feedback=False)
         return
     
+    def execute(self, temperature:float, time_s:float, *args, **kwargs):
+        """
+        Alias for `holdTemperature()`
+        
+        Hold target temperature for desired duration
+
+        Args:
+            temperature (float): temperature in degree Celsius
+            time_s (float): duration in seconds
+        """
+        return self.holdTemperature(temperature=temperature, time_s=time_s)
+    
     def getTemperature(self) -> Union[tuple, str]:
         """
         Retrieve temperatures from device 
         Including the set temperature, hot temperature, cold temperature, and the power level
         
         Returns:
             Union[tuple, str]: response from device
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Make/Light/led_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class LED:
     """
     LED dataclass represents a single LED unit
 
     ### Constructor
     Args:
         `channel` (int): channel id
-        
+    
     ### Attributes
     - `channel` (int): channel id
     - `update_power` (bool): whether to update the LED's power
     
     ### Properties
     - `power` (int): power level of LED (0~255)
     
@@ -85,14 +85,15 @@
     ### Attributes
     - `channels` (dict[int, LED]): dictionary of {channel id, `LED` objects}
     
     ### Properties
     - `port` (str): COM port address
     
     ### Methods
+    - `execute`: alias for `setPower()`
     - `getPower`: get power level(s) of channel(s)
     - `getTimedChannels`: get channels that are still timed
     - `isBusy`: checks and returns whether the LED array is still busy
     - `setPower`: set the power value(s) for channel(s)
     - `shutdown`: shutdown procedure for tool
     - `startTiming`: start counting down time left with LEDs on
     - `turnOff`: turn of specified LED channels
@@ -102,26 +103,46 @@
         'busy': False,
         'connected': False,
         'execute_now': False,
         'timing_loop': False
     }
     
     def __init__(self, port:str, channels:list[int] = [0], **kwargs):
+        """
+        Instantiate the class
+
+        Args:
+            port (str): COM port addressed
+            channels (list[int], optional): list of channels. Defaults to [0].
+        """
         super().__init__(**kwargs)
         self.channels = {chn: LED(chn) for chn in channels}
         self._threads = {}
         self._timed_channels = []
         self._connect(port)
         return
     
     # Properties
     @property
     def port(self) -> str:
         return self.connection_details.get('port', '')
     
+    def execute(self, value:int, time_s:int = 0, channel:Optional[int] = None, *args, **kwargs):
+        """
+        Alias for `setPower()`
+        
+        Set the power value(s) for channel(s)
+
+        Args:
+            value (int): 8-bit integer for LED power (i.e. 0~255)
+            time_s (int, optional): duration in seconds. Defaults to 0.
+            channel (Optional[int], optional): channel id. Defaults to None.
+        """
+        return self.setPower(value=value, time_s=time_s, channel=channel)
+    
     def getPower(self, channel:Optional[int] = None) -> list[int]:
         """
         Get power level(s) of channel(s)
 
         Args:
             channel (Optional[int], optional): channel index. Defaults to None.
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 This module holds the class for shakers from QInstruments.
 
 Classes:
     BioShake (Maker)
 """
 # Standard library imports
 from __future__ import annotations
+from datetime import datetime
+import pandas as pd
 from threading import Thread
 import time
 from typing import Optional, Union
 
 # Local application imports
 from ...make_utils import Maker
 from .qinstruments_api import QInstruments
 print(f"Import: OK <{__name__}>")
 
 ACCELERATION_LIMIT = (1,30)
+COLUMNS = ('Time', 'Set', 'Actual')
+"""Headers for output data from BioShake device"""
 
 class BioShake(Maker):
     """
     BioShake provides methods to control
     
     ### Constructor
     Args:
         `port` (str): COM port address
     
     ### Attributes
+    - `buffer_df` (pd.DataFrame): buffer dataframe to store collected data
     - `device` (Callable): device object that communicates with physical tool
     - `limits` (dict[str, tuple]): hardware limits for device
     - `model` (str): device model description
     - `ranges` (dict[str, tuple]): user-defined ranges for controls
     - `set_speed` (float): target speed
     - `set_temperature` (float): target temperature
     - `shake_time_left` (float): remaining time left on shaker
@@ -40,14 +45,16 @@
     
     ### Properties
     - `acceleration` (float): acceleration / deceleration of the shaker in seconds
     - `port` (str): COM port address
     - `verbose` (bool): verbosity of class
     
     ### Methods
+    - `clearCache`: clears and remove data in buffer
+    - `execute`: alias for `holdTemperature()` and `shake()`
     - `getAcceleration`: returns the acceleration/deceleration value
     - `getErrors`: returns a list with errors and warnings which can occur during processing
     - `getShakeTimeLeft`: returns the remaining shake time in seconds if device was started with the a defined duration
     - `getSpeed`: returns the set speed and current mixing speed in rpm
     - `getStatus`: retrieve the status of the device's ELM, shaker, and temperature control
     - `getTemperature`: returns the set temperature and current temperature in °C
     - `getUserLimits`: retrieve the user defined limits for speed and temperature
@@ -62,56 +69,64 @@
     - `setCounterClockwise`: sets the mixing direction to counter clockwise
     - `setSpeed`: set the target mixing speed
     - `setTemperature`: sets target temperature between TempMin and TempMax in 1/10°C increments
     - `shake`: shake the plate at target speed, for specified duration
     - `shutdown`: shutdown procedure for tool
     - `stop`: stop the shaker immediately at an undefined position, ignoring the defined deceleration time if in an emergency
     - `toggleECO`: toggle the economical mode to save energy and decrease abrasion 
+    - `toggleFeedbackLoop`: start or stop feedback loop
     - `toggleGrip`: grip or release the object
+    - `toggleRecord`: start or stop data recording
     - `toggleShake`: starts/stops shaking with defined speed with defined acceleration/deceleration time
     - `toggleTemperature`: switches on/off the temperature control feature and starts/stops heating/cooling
     """
     
     _default_acceleration: int = 5
     _default_speed: int = 500
+    _default_temperature: float = 25
     _default_flags = {
         'busy': False,
         'connected': False,
         'elm_locked': True,
+        'get_feedback': False,
+        'pause_feedback': False,
+        'record': False,
         'shake_counterclockwise': True,
         'speed_reached': False,
         'temperature_reached': False
     }
     def __init__(self, port: str, **kwargs):
         """
         Instantiate the class
 
         Args:
             port (str): COM port address
         """
         super().__init__(**kwargs)
+        self.buffer_df = pd.DataFrame(columns=list(COLUMNS))
         self.device: QInstruments = None
         self.model = ''
-        self.set_speed = None
-        self.set_temperature = None
+        self.set_speed = self._default_speed
+        self.set_temperature = self._default_temperature
         self.shake_time_left = None
         self.speed = self._default_speed
-        self.temperature = None
-        self.tolerance = 0.01
+        self.temperature = self._default_temperature
+        self.tolerance = 0.05
         
         self.limits = {
-            'acceleration': (0,0),
-            'speed': (0,0),
-            'temperature': (0,0)
+            'acceleration': (0,9999),
+            'speed': (0,9999),
+            'temperature': (0,9999)
         }
         self.ranges = {
-            'speed': (0,0),
-            'temperature': (0,0)
+            'speed': (0,9999),
+            'temperature': (0,9999)
         }
         self._acceleration = self._default_acceleration
+        self._columns = list(COLUMNS)
         self._threads = {}
         self._connect(port)
         self.verbose = kwargs.get('verbose', False)
         return
     
     # Properties
     @property
@@ -138,14 +153,16 @@
         del self._verbose
         return
     
     def __defaults__(self):
         """Retrieve the default and starting configuration of the device upon start up"""
         self.isCounterClockwise()
         self.isLocked()
+        if not self.isConnected():
+            return
         self.limits['acceleration'] = ( self.device.getShakeAccelerationMin(), self.device.getShakeAccelerationMax() )
         self.limits['speed'] = ( self.device.getShakeMinRpm(), self.device.getShakeMaxRpm() )
         self.limits['temperature'] = ( self.device.getTempMin(), self.device.getTempMax() )
         return
     
     def __info__(self):
         """Prints the boot screen text"""
@@ -178,14 +195,58 @@
         Retrieve the software version on the device
 
         Returns:
             str: device version
         """
         return self.device.getVersion()
     
+    def clearCache(self):
+        """Clears and remove data in buffer"""
+        self.setFlag(pause_feedback=True)
+        time.sleep(0.1)
+        self.buffer_df = pd.DataFrame(columns=self._columns)
+        self.setFlag(pause_feedback=False)
+        return
+    
+    def execute(self, 
+            shake: bool,
+            temperature: Optional[float] = None, 
+            speed: Optional[int] = None, 
+            duration: Optional[int] = None, 
+            acceleration: Optional[int] = None, 
+            *args, **kwargs
+        ):
+        """
+        Alias for `holdTemperature()` and `shake()`
+        
+        Set target temperature, then shake the plate at target speed and hold target temperature for desired duration
+
+        Args:
+            shake (bool): whether to shake
+            temperature (Optional[float], optional): temperature in degree °C. Defaults to None.
+            speed (Optional[int], optional): shaking speed. Defaults to None.
+            duration (Optional[int], optional): duration of shake. Defaults to None.
+            acceleration (Optional[int], optional): acceleration value. Defaults to None.
+        """
+        # setTemperature
+        if temperature is not None:
+            self.setTemperature(temperature)
+        
+        # shake
+        if shake:
+            self.shake(speed=speed, duration=duration, acceleration=acceleration)
+        
+        # holdTemperature
+        if temperature is not None and duration:
+            print(f"Holding at {self.set_temperature}°C for {duration} seconds")
+            time.sleep(duration)
+            print(f"End of temperature hold")
+            # self.setTemperature(25, False)
+        return
+    
     def getAcceleration(self) -> float:
         """
         Returns the acceleration/deceleration value
 
         Returns:
             float: acceleration/deceleration value
         """
@@ -247,45 +308,55 @@
     def getTemperature(self) -> tuple[float]:
         """
         Returns the set temperature and current temperature in °C
 
         Returns:
             tuple[float]: set temperature, current temperature
         """
+        now = datetime.now()
         response = self.device.getTempTarget()
         self.set_temperature = response if response is not None else self.set_temperature
         response = self.device.getTempActual()
         self.temperature = response if response is not None else self.temperature
         
         flag = (abs(self.temperature - self.set_temperature) <= self.tolerance*self.set_temperature) if self.set_temperature else False
         self.setFlag(temperature_reached=flag)
+        
+        if self.flags['record']:
+            values = [now, self.set_temperature, self.temperature]
+            row = {k:v for k,v in zip(self._columns, values)}
+            # self.buffer_df = self.buffer_df.append(row, ignore_index=True)
+            new_row_df = pd.DataFrame(row)
+            self.buffer_df = pd.concat([self.buffer_df, new_row_df])
         return self.set_temperature, self.temperature
     
     def getUserLimits(self):
         """Retrieve the user defined limits for speed and temperature"""
+        if not self.isConnected():
+            return
         try:
             self.ranges['temperature'] = ( self.device.getTempLimiterMin(), self.device.getTempLimiterMax() )
             self.ranges['speed'] = ( self.device.getShakeSpeedLimitMin(), self.device.getShakeSpeedLimitMax() )
         except AttributeError:
-            self.ranges['temperature'] = self.limits.get('temperature', (0,0))
-            self.ranges['speed'] = self.limits.get('speed', (0,0))
+            self.ranges['temperature'] = self.limits.get('temperature', (0,9999))
+            self.ranges['speed'] = self.limits.get('speed', (0,9999))
         return
 
     def holdTemperature(self, temperature:float, time_s:float):
         """
         Hold target temperature for desired duration
 
         Args:
             temperature (float): temperature in degree °C
             time_s (float): duration in seconds
         """
         self.setTemperature(temperature)
         print(f"Holding at {self.set_temperature}°C for {time_s} seconds")
         time.sleep(time_s)
-        print(f"End of temperature hold")
+        print(f"End of temperature hold ({time_s}s)")
         return
     
     def home(self, timeout:int = 5):
         """
         Move shaker to the home position and locks in place
         
         Note: Minimum response time is less than 4 sec (internal failure timeout)
@@ -343,14 +414,16 @@
         Restarts the controller
         
         Note: This takes about 30 seconds for BS units and 5 for the Q1, CP models
         
         Args:
             timeout (int, optional): number of seconds to wait before aborting. Defaults to 30.
         """
+        self.toggleRecord(False)
+        self.clearCache()
         self.device.resetDevice(timeout=timeout)
         return
 
     def setAcceleration(self, acceleration:int, default:bool = False):
         """
         Sets the acceleration/deceleration value in seconds
 
@@ -373,15 +446,15 @@
         Sets the mixing direction to counter clockwise
 
         Args:
             counterclockwise (bool): whether to set mixing direction to counter clockwise
         """
         self.device.setShakeDirection(counterclockwise=counterclockwise)
         response = self.device.getShakeDirection()
-        response = response if response is not None else self.flags['shake_counterclockwise']
+        response = response if response is not None else counterclockwise
         self.setFlag(shake_counterclockwise=response)
         return 
     
     def setSpeed(self, speed:int, default:bool = False):
         """
         Set the target mixing speed
         
@@ -412,20 +485,20 @@
             temperature (float): target temperature (between TempMin and TempMax)
             blocking (bool, optional): whether to wait for temperature to reach set point. Defaults to True.
         """
         self.toggleTemperature(on=True)
         limits = self.ranges.get('temperature', (0,99))
         lower_limit, upper_limit = limits
         if lower_limit <= temperature <= upper_limit:
-            self.set_temperature = temperature
+            self.set_temperature = float(temperature)
             self.device.setTempTarget(temperature=temperature)
         else:
             raise ValueError(f"Temperature out of range {limits}: {temperature}")
         
-        while self.set_temperature != self.device.getTempTarget():
+        while self.set_temperature != float(temperature):
             self.getTemperature()
         print(f"New set temperature at {self.set_temperature}°C")
         self.setFlag(temperature_reached=False)
         
         if blocking:
             print(f"Waiting for temperature to reach {self.set_temperature}°C")
         while not self.isAtTemperature():
@@ -463,14 +536,15 @@
             while not self.isAtSpeed():
                 shake_time = time.perf_counter() - start_time
                 if shake_time > self.acceleration:
                     break
                 time.sleep(1)
             if duration:
                 time.sleep(abs(duration - shake_time))
+                print(f"End of shake ({duration}s)")
             return self.isAtSpeed()
         thread = Thread(target=checkSpeed)
         thread.start()
         self._threads['check_speed'] = thread
         return
         
     def shutdown(self):
@@ -502,28 +576,57 @@
             timeout (int, optional): number of seconds to wait before aborting. Defaults to 5.
         """
         if on:
             self.device.setEcoMode(timeout=timeout)
         else:
             self.device.leaveEcoMode(timeout=timeout)
         return
+    
+    def toggleFeedbackLoop(self, on:bool):
+        """
+        Start or stop feedback loop
+
+        Args:
+            on (bool): whether to start loop to continuously read from device
+        """
+        self.setFlag(get_feedback=on)
+        if on:
+            if 'feedback_loop' in self._threads:
+                self._threads['feedback_loop'].join()
+            thread = Thread(target=self._loop_feedback)
+            thread.start()
+            self._threads['feedback_loop'] = thread
+        else:
+            self._threads['feedback_loop'].join()
+        return
      
     def toggleGrip(self, on:bool):
         """
         Grip or release the object
 
         Args:
             on (bool): whether to grip the object
         """
         if on:
             self.device.setElmLockPos()
         else:
             self.device.setElmUnlockPos()
         return
     
+    def toggleRecord(self, on:bool):
+        """
+        Start or stop data recording
+
+        Args:
+            on (bool): whether to start recording temperature
+        """
+        self.setFlag(record=on, get_feedback=on, pause_feedback=False)
+        self.toggleFeedbackLoop(on=on)
+        return
+    
     def toggleShake(self, on:bool, duration:Optional[int] = None, home:bool = True):
         """
         Starts/stops shaking with defined speed with defined acceleration/deceleration time.
         Shake runtime can be specified, as well as whether to return to home position after stopping.
 
         Args:
             on (bool): whether to start shaking
@@ -578,17 +681,29 @@
             device = QInstruments(port, baudrate, timeout=timeout)
             self.device = device
         except Exception as e:
             if self.verbose:
                 print(e)
         else:
             self.model = device.model
-            self.setFlag(connected=True)
-            self.__defaults__()
-            self.getUserLimits()
+            self.setFlag(connected=self.device.flags.get('connected', False))
+            if self.isConnected():
+                self.__defaults__()
+                self.getUserLimits()
+        return
+    
+    def _loop_feedback(self):
+        """Loop to constantly read from device"""
+        print('Listening...')
+        while self.flags['get_feedback']:
+            if self.flags['pause_feedback']:
+                continue
+            self.getTemperature()
+            time.sleep(0.1)
+        print('Stop listening...')
         return
     
     def _query(self, 
             command: str, 
             numeric: bool = False, 
             slow: bool = False, 
             timeout_s: float = 0.3
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py` & `control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         `timeout` (int, optional): timeout in seconds. Defaults to 1.
         `verbose` (bool, optional): verbosity of class. Defaults to False.
     
     ### Attributes
     - `connection_details` (dict): dictionary of connection details (e.g. COM port / IP address)
     - `device` (Callable): device object that communicates with physical tool
     - `flags` (dict[str, bool]): keywords paired with boolean flags
+    - `model` (str): device model
     - `verbose` (bool): verbosity of class
     
     ### Methods
     #### Initialization
     - `disableBootScreen`: permanent deactivation of the boot screen startup text
     - `disableCLED`: permanent deactivation of the LED indication lights
     - `enableBootScreen`: permanent activation of the boot screen startup text
@@ -110,17 +111,19 @@
     - `setElmStartupPosition`: permanently set whether the ELM is unlocked after device startup
     - `setElmUnlockPos`: open the ELM
     #### General
     - `connect`: reconnect to device using existing connection details
     - `disconnect`: disconnect from device
     - `query`: write command to and read response from device
     - `read`: read response from device
+    - `setFlag`: set flags by using keyword arguments
     - `write`: write command to device
     """
     
+    _default_flags: dict[str, bool] = {'busy': False, 'connected': False}
     def __init__(self, 
         port: str, 
         baudrate:int = 9600, 
         timeout:int = 1, 
         verbose:bool = False, 
         **kwargs
     ):
@@ -131,14 +134,15 @@
             port (str): COM port address
             baudrate (int, optional): baudrate. Defaults to 9600.
             timeout (int, optional): timeout in seconds. Defaults to 1.
             verbose (bool, optional): verbosity of class. Defaults to False.
         """
         self.connection_details = {}
         self.device = None
+        self.flags = self._default_flags.copy()
         self.model = ''
         self.verbose = verbose
         self._connect(port=port, baudrate=baudrate, timeout=timeout)
         return
         
     # Initialization methods
     def disableBootScreen(self):
@@ -690,15 +694,14 @@
         Returns:
             bool: whether temperature control is enabled
         """
         response = self.query("getTempState", numeric=True)
         if response is np.nan:
             return None
         state = bool(int(response)%2)
-        # TODO: add flags
         return state
     
     def getTempTarget(self) -> Optional[float]:
         """
         Returns the target temperature
 
         Returns:
@@ -965,14 +968,28 @@
                 print(e)
         else:
             response = response.decode('utf-8').strip()
             if self.verbose and len(response):
                 print(response)
         return response
     
+    def setFlag(self, **kwargs):
+        """
+        Set flags by using keyword arguments
+
+        Kwargs:
+            key, value: (flag name, boolean) pairs
+        """
+        if not all([type(v)==bool for v in kwargs.values()]):
+            raise ValueError("Ensure all assigned flag values are boolean.")
+        self.flags.update(kwargs)
+        # for key, value in kwargs.items():
+        #     self.flags[key] = value
+        return
+    
     def write(self, command:str) -> bool:
         """
         Write command to device
 
         Args:
             command (str): <command code><value>
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py` & `control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     - `speed` (int): spin speed in rpm
     
     ### Properties
     - `port` (str): COM port address
     - `position` (np.ndarray): x,y,z position of spinner
     
     ### Methods
+    - `execute`: alias for `run()`
     - `run`: executes the soak and spin steps
     - `shutdown`: shutdown procedure for tool
     - `soak`: executes a soak step
     - `spin`: execute a spin step
     """
     
     _default_flags = {
@@ -76,14 +77,27 @@
     def port(self) -> str:
         return self.connection_details.get('port', '')
     
     @property
     def position(self) -> np.ndarray:
         return np.array(self._position)
     
+    def execute(self, soak_time:int = 0, spin_speed:int = 2000, spin_time:int = 1, *args, **kwargs):
+        """
+        Alias for `run()`
+        
+        Execute the soak and spin steps
+
+        Args:
+            soak_time (int, optional): soak time. Defaults to 0.
+            spin_speed (int, optional): spin speed. Defaults to 2000.
+            spin_time (int, optional): spin time. Defaults to 1.
+        """
+        return self.run(soak_time=soak_time, spin_speed=spin_speed, spin_time=spin_time)
+    
     def run(self, soak_time:int = 0, spin_speed:int = 2000, spin_time:int = 1, **kwargs):
         """
         Execute the soak and spin steps
 
         Args:
             soak_time (int, optional): soak time. Defaults to 0.
             spin_speed (int, optional): spin speed. Defaults to 2000.
@@ -192,20 +206,21 @@
     SpinnerAssembly provides methods to control multiple spin coater controller units
     
     ### Constructor
     Args:
         `ports` (list[str]): COM port addresses
         `channels` (list[int]): channel ids
         `positions` (list[tuple[float]]): x,y,z positions of spinners
-
+    
     ### Attributes
     - `channels` (dict[int, Spinner]): dictionary of {channel id, `Spinner` objects}
     
     ### Methods
     - `disconnect`: disconnect from device
+    - `execute`: alias for `run()`
     - `isBusy`: checks and returns whether any of the spinners are still busy
     - `isConnected`: checks and returns whether all spinners are connected
     - `run`: executes the soak and spin steps
     - `shutdown`: shutdown procedure for tool
     - `soak`: executes a soak step
     - `spin`: execute a spin step
     """
@@ -237,14 +252,28 @@
         return
 
     def disconnect(self):
         """Disconnect from device"""
         for channel in self.channels.values():
             channel.disconnect()
         return super().disconnect() 
+    
+    def execute(self, soak_time:int, spin_speed:int, spin_time:int, channel:int, *args, **kwargs):
+        """
+        Alias for `run()`
+        
+        Execute the soak and spin steps
+
+        Args:
+            soak_time (int): soak time
+            spin_speed (int): spin speed
+            spin_time (int): spin time
+            channel (int): channel id
+        """
+        return self.run(soak_time=soak_time, spin_speed=spin_speed, spin_time=spin_time, channel=channel)
         
     def isBusy(self) -> bool:
         """
         Checks and returns whether any of the spinners are still busy
 
         Returns:
             bool: whether any of the spinners are still busy
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Make/make_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Make/make_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,21 +16,23 @@
     ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
     
     ### Constructor
     Args:
         `verbose` (bool, optional): verbosity of class. Defaults to False.
     
     ### Attributes
+    - `channel` (int): channel id
     - `connection_details` (dict): dictionary of connection details (e.g. COM port / IP address)
     - `device` (Callable): device object that communicates with physical tool
     - `flags` (dict[str, bool]): keywords paired with boolean flags
     - `verbose` (bool): verbosity of class
     
     ### Methods
     #### Abstract
+    - `execute`: execute task
     - `shutdown`: shutdown procedure for tool
     - `_connect`: connection procedure for tool
     #### Public
     - `connect`: establish connection with device
     - `disconnect`: disconnect from device
     - `isBusy`: checks and returns whether the device is busy
     - `isConnected`: checks and returns whether the device is connected
@@ -42,24 +44,29 @@
     def __init__(self, verbose:bool = False, **kwargs):
         """
         Instantiate the class
 
         Args:
             verbose (bool, optional): verbosity of class. Defaults to False.
         """
+        self.channel = 0
         self.connection_details = {}
         self.device = None
         self.flags = self._default_flags.copy()
         self.verbose = verbose
         return
     
     def __del__(self):
         self.shutdown()
         
     @abstractmethod
+    def execute(self, *args, **kwargs):
+        """Execute task"""
+        
+    @abstractmethod
     def shutdown(self):
         """Shutdown procedure for tool"""
         self.disconnect()
         self.resetFlags()
         return
         
     @abstractmethod
@@ -114,11 +121,12 @@
         Set flags by using keyword arguments
 
         Kwargs:
             key, value: (flag name, boolean) pairs
         """
         if not all([type(v)==bool for v in kwargs.values()]):
             raise ValueError("Ensure all assigned flag values are boolean.")
-        for key, value in kwargs.items():
-            self.flags[key] = value
+        self.flags.update(kwargs)
+        # for key, value in kwargs.items():
+        #     self.flags[key] = value
         return
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
     KeithleyDevice provides methods to interface with the potentiometer from Keithley
     
     ### Constructor
     Args:
         `ip_address` (str): IP address of device
         `name` (str, optional): name of device. Defaults to 'def'.
-        
+    
     ### Attributes
     - `active_buffer` (str): name of active buffer in Keithley
     - `name` (str): name of device
     - `sense` (SenseDetails): parameters for Keithley's sense terminal
     - `source` (SourceDetails): parameters for Keithley's source terminal
     
     ### Properties
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     ### Constructor
     Args:
         `function_type` (Optional[str]): name of function, choice from current, resistance, and voltage. Defaults to None.
         `range_limit` (Union[str, float, None]): sensing range. Defaults to 'DEFault'.
         `four_point` (bool): whether to use four-point probe measurement. Defaults to True.
         `count` (int): number of readings to measure for each condition. Defaults to 1.
-        
+    
     ### Attributes
     - `count` (int): number of readings to measure for each condition
     - `four_point` (bool): whether to use four-point probe measurement
     - `function_type` (Optional[str]): name of function
     - `range_limit` (Union[str, float, None]): sensing range
     
     ### Properties
@@ -158,15 +158,15 @@
     SourceDetails represents a set of parameters for Keithley's source terminal
 
     ### Constructor
     Args:
         `function_type` (Optional[str]): name of function, choice from current and voltage. Defaults to None.
         `range_limit` (Union[str, float, None]): sourcing range. Defaults to None.
         `measure_limit` (Union[str, float, None]): limit imposed on the measurement range. Defaults to 'DEFault'.
-        
+    
     ### Attributes
     - `function_type` (Optional[str]): name of function
     - `measure_limit` (Union[str, float, None]): limit imposed on the measurement range
     - `range_limit` (Union[str, float, None]): sourcing range
     
     ### Properties
     - `measure_type` (str): type of measurement limit
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # %% -*- coding: utf-8 -*-
 """
 This module holds the class for tools from Keithley.
 
 Classes:
     Keithley (Programmable)
 """
-# Local application imports
+# Standard library imports
 from __future__ import annotations
+
+# Local application imports
 from ...measure_utils import Programmable
 from .keithley_device import KeithleyDevice
 from . import programs
 print(f"Import: OK <{__name__}>")
 
 class Keithley(Programmable):
     """
     Keithley provides methods to control potentiometers from Keithley
     
     ### Constructor
     Args:
         `ip_address` (str): IP address of device. Defaults to '192.168.1.125'.
         `name` (str): name of device. Defaults to 'def'.
-        
+    
     ### Properties
     - `ip_address` (str): IP address of device
     
     ### Methods
     - `disconnect`: disconnect from device
     """
-    model = 'keithley_'
-    available_programs: tuple[str] = tuple(programs.PROGRAM_NAMES)      # FIXME
-    possible_inputs: tuple[str] = tuple(programs.INPUTS_SET)            # FIXME
+    
+    _place: str = '.'.join(__name__.split('.')[1:-1])
+    model: str = 'keithley_'
     def __init__(self, ip_address:str = '192.168.1.125', name:str = 'def', **kwargs):
         """
         Instantiate the class
         
         Args:
             ip_address (str): IP address of device. Defaults to '192.168.1.125'.
             name (str): name of device. Defaults to 'def'.
@@ -60,10 +62,9 @@
             ip_address (str): IP address of device
             name (str): name of device
         """
         self.connection_details = {
             'ip_address': ip_address,
             'name': name
         }
-        self._ip_address = ip_address
         self.device = KeithleyDevice(ip_address=ip_address, name=name)
         return
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 # %% -*- coding: utf-8 -*-
 """
-This module holds the program class for tools from PiezoRobotics.
+This module holds the program class for tools from Keithley.
 
 Classes:
     IV_Scan (Program)
     LSV (Program)
     OCV (Program)
-
-Other constants and variables:
-    INPUTS_SET (list)
-    PROGRAM_NAMES (list)
 """
 # Standard library imports
 import pandas as pd
 import time
 from typing import Optional, Protocol
 
 # Local application imports
-from ....program_utils import Program, get_program_details
+from ....program_utils import Program
 from ..keithley_lib import SenseDetails, SourceDetails
 print(f"Import: OK <{__name__}>")
 
 class Device(Protocol):
     sense: SenseDetails
     source: SourceDetails
     def beep(self, *args, **kwargs):
@@ -75,14 +71,22 @@
     
     def __init__(self, 
         device: Device, 
         parameters: Optional[dict] = None,
         verbose: bool = False, 
         **kwargs
     ):
+        """
+        Instantiate the class
+
+        Args:
+            device (Device): device object
+            parameters (Optional[dict], optional): dictionary of kwargs. Defaults to None.
+            verbose (bool, optional): verbosity of class. Defaults to False.
+        """
         super().__init__(device=device, parameters=parameters, verbose=verbose, **kwargs)
         return
     
     def run(self):
         """Run the measurement program"""
         device = self.device
         count = self.parameters.get('count', 1)
@@ -96,15 +100,15 @@
         
         for current in self.parameters.get('currents', (0,)):
             device.setSource(value=current)
             device.toggleOutput(on=True)
             device.run()
             time.sleep(0.1*count)
         time.sleep(1)
-        self.data_df = device.read(bulk=True)
+        self.data_df = device.readAll()
         device.beep()
         device.getErrors()
         return
 
 
 class OCV(Program):
     """
@@ -133,14 +137,22 @@
     
     def __init__(self, 
         device: Device, 
         parameters: Optional[dict] = None,
         verbose: bool = False, 
         **kwargs
     ):
+        """
+        Instantiate the class
+
+        Args:
+            device (Device): device object
+            parameters (Optional[dict], optional): dictionary of kwargs. Defaults to None.
+            verbose (bool, optional): verbosity of class. Defaults to False.
+        """
         super().__init__(device=device, parameters=parameters, verbose=verbose, **kwargs)
         return
     
     def run(self):
         """Run the measurement program"""
         device = self.device
         count = self.parameters.get('count', 1)
@@ -152,30 +164,30 @@
         device.makeBuffer()
         device.beep()
         
         device.setSource(value=0)
         device.toggleOutput(on=True)
         device.run()
         time.sleep(0.1*count)
-        self.data_df = device.read(bulk=True)
+        self.data_df = device.readAll()
         device.beep()
         device.getErrors()
         return
 
 
 class LSV(Program):
     """
-    I-V Scan program
+    Linear Sweep Voltammetry Scan program
 
     ### Constructor
     Args:
         `device` (Device): device object
         `parameters` (Optional[dict], optional): dictionary of kwargs. Defaults to None.
         `verbose` (bool, optional): verbosity of class. Defaults to False.
-
+    
     ### Attributes
     - `data_df` (pd.DataFrame): data collected from device when running the program
     - `device` (Device): device object
     - `parameters` (dict[str, ...]): parameters
     - `verbose` (bool): verbosity of class
     
     ### Methods
@@ -196,14 +208,22 @@
     
     def __init__(self, 
         device: Device, 
         parameters: Optional[dict] = None,
         verbose: bool = False, 
         **kwargs
     ):
+        """
+        Instantiate the class
+
+        Args:
+            device (Device): device object
+            parameters (Optional[dict], optional): dictionary of kwargs. Defaults to None.
+            verbose (bool, optional): verbosity of class. Defaults to False.
+        """
         super().__init__(device=device, parameters=parameters, verbose=verbose, **kwargs)
         return
     
     def run(self):
         """Run the measurement program"""
         device= self.device
         # Get OCV
@@ -291,17 +311,8 @@
         parameters = [voltages, str(dwell_time), str(repeat), 'AUTO', 'OFF', bidirectional]
         device.sendCommands(
             [f'SOURce:SWEep:{device.source.function_type}:{mode} {",".join(parameters)}']
         )
         device.start(sequential_commands=False)
         return
 
-
-# FIXME: Do away with these objects below
-PROGRAMS = [IV_Scan, OCV, LSV]
-INPUTS = [item for item in [[key for key in get_program_details(prog).inputs] for prog in PROGRAMS]]
-PROGRAM_NAMES = [prog.__name__ for prog in PROGRAMS]
-"""List of program names"""
-INPUTS_SET = sorted( list(set([item for sublist in INPUTS for item in sublist])) )
-"""Sorted list of input parameters"""
-
 # %%
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     PiezoRoboticsDevice provides methods to interface with the characterisation device from PiezoRobotics
 
     ### Constructor
     Args:
         `port` (str): COM port address
         `channel` (int, optional): channel id. Defaults to 1.
-        
+    
     ### Attributes
     - `channel` (int): channel id
     
     ### Properties
     - `frequency` (Frequency): lower and upper frequency range limit
     
     ### Methods
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     """
     Frequency dataclass represents a low and high frequency range limit
 
     ### Constructor
     Args:
         `low` (float): frequency lower bound. Defaults to FrequencyCode.FREQ_01
         `high` (float): frequency upper bound. Defaults to FrequencyCode.FREQ_54
-        
+    
     ### Attributes
     - `low` (float): frequency lower bound. Defaults to FrequencyCode.FREQ_01
     - `high` (float): frequency upper bound. Defaults to FrequencyCode.FREQ_54
     
     ### Properties
     - `code` (tuple[str]): tuple of (lower frequency code, upper frequency code)
     """
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # %% -*- coding: utf-8 -*-
 """
 This module holds the class for tools from PiezoRobotics.
 
 Classes:
     PiezoRobotics (Programmable)
 """
-# Local application imports
+# Standard library imports
 from __future__ import annotations
+
+# Local application imports
 from ...measure_utils import Programmable
 from .piezorobotics_device import PiezoRoboticsDevice
 from . import programs
 print(f"Import: OK <{__name__}>")
         
 class PiezoRobotics(Programmable):
     """
     PiezoRobotics provides methods to control the characterisation device from PiezoRobotics
 
     ### Constructor
     Args:
         `port` (str): COM port address
         `channel` (int, optional): channel id. Defaults to 1.
-        
+    
     ### Properties
     - `port` (str): COM port address
     
     ### Methods
     - `disconnect`: disconnect from device
     """
     
     _default_program = programs.DMA
+    _place: str = '.'.join(__name__.split('.')[1:-1])
     model = 'piezorobotics_'
-    available_programs: tuple[str] = tuple(programs.PROGRAM_NAMES)      # FIXME
-    possible_inputs: tuple[str] = tuple(programs.INPUTS_SET)            # FIXME
     def __init__(self, port:str, channel=1, **kwargs):
         """
         Instantiate the class
 
         Args:
             port (str): COM port address
             channel (int, optional): channel id. Defaults to 1.
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 This module holds the program class for tools from PiezoRobotics.
 
 Classes:
     DMA (Program)
 
 Other constants and variables:
     FREQUENCIES (tuple)
-    INPUTS_SET (list)
-    PROGRAM_NAMES (list)
 """
 # Standard library imports
 from datetime import datetime
 import pandas as pd
 import time
 from typing import Optional, Protocol
 
 # Local application imports
-from ....program_utils import Program, get_program_details
+from ....program_utils import Program
 from ..piezorobotics_lib import FrequencyCode
 print(f"Import: OK <{__name__}>")
 
 FREQUENCIES = tuple([frequency.value for frequency in FrequencyCode])
 """Collection of all available frequency values"""
 
 class Device(Protocol):
@@ -39,15 +37,15 @@
     Dynamic Mechanical Analysis
 
     ### Constructor
     Args:
         `device` (Device): device object
         `parameters` (Optional[dict], optional): dictionary of kwargs. Defaults to None.
         `verbose` (bool, optional): verbosity of class. Defaults to False.
-
+    
     ### Attributes
     - `data_df` (pd.DataFrame): data collected from device when running the program
     - `device` (Device): device object
     - `parameters` (dict[str, ...]): parameters
     - `verbose` (bool): verbosity of class
     
     ### Methods
@@ -102,16 +100,7 @@
             df['run'] = i+1
             if i == 0:
                 self.data_df = df
             else:
                 self.data_df = pd.concat([self.data_df, df], ignore_index=True)
         device.toggleClamp(False)
         return
-
-
-# FIXME: Do away with these objects below
-PROGRAMS = [DMA]
-INPUTS = [item for item in [[key for key in get_program_details(prog).inputs] for prog in PROGRAMS]]
-PROGRAM_NAMES = [prog.__name__ for prog in PROGRAMS]
-"""List of program names"""
-INPUTS_SET = sorted( list(set([item for sublist in INPUTS for item in sublist])) )
-"""Sorted list of input parameters"""
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/balance_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,22 +31,23 @@
     """
     MassBalance provides methods to read out values from a precision mass balance
 
     ### Constructor
     Args:
         `port` (str): COM port address
         `calibration_factor` (float, optional): calibration factor of device readout to mg. Defaults to CALIBRATION_FACTOR.
-        
+    
     ### Attributes
     - `baseline` (float): baseline readout at which zero mass is set
     - `calibration_factor` (float): calibration factor of device readout to mg
     - `precision` (int): number of decimal places to print mass value
     
     ### Properties
     - `mass` (float): mass of sample
+    - `port` (str): COM port address
     
     ### Methods
     - `clearCache`: clear most recent data and configurations
     - `disconnect`: disconnect from device
     - `getMass`: get the mass of the sample by measuring the force response
     - `reset`: reset the device
     - `shutdown`: shutdown procedure for tool
@@ -82,14 +83,18 @@
         self._connect(port)
         return
     
     # Properties
     @property
     def mass(self) -> float:
         return round(self._mass, self.precision)
+    
+    @property
+    def port(self) -> str:
+        return self.connection_details.get('port', '')
    
     def clearCache(self):
         """Clear most recent data and configurations"""
         self.setFlag(pause_feedback=True)
         time.sleep(0.1)
         self.buffer_df = pd.DataFrame(columns=COLUMNS)
         self.setFlag(pause_feedback=False)
@@ -125,17 +130,14 @@
                     now, 
                     value, 
                     self.calibration_factor, 
                     self.baseline, 
                     self._mass
                 ]
                 row = {k:v for k,v in zip(COLUMNS, values)}
-                # self.buffer_df = self.buffer_df.append(row, ignore_index=True)
-                # new_row_df = pd.DataFrame(row)
-                # self.buffer_df = pd.concat([self.buffer_df, new_row_df])
                 new_row_df = pd.DataFrame(row, index=[0])
                 self.buffer_df = pd.concat([self.buffer_df, new_row_df], ignore_index=True)
         return response
   
     def reset(self):
         """Reset the device"""
         super().reset()
@@ -170,15 +172,15 @@
         return
     
     def toggleRecord(self, on:bool):
         """
         Start or stop data recording
 
         Args:
-            on (bool): whether to start recording temperature
+            on (bool): whether to start recording data
         """
         self.setFlag(record=on, get_feedback=on, pause_feedback=False)
         self.toggleFeedbackLoop(on=on)
         return
 
     def zero(self, wait:int = 5):
         """
@@ -241,15 +243,15 @@
         while self.flags['get_feedback']:
             if self.flags['pause_feedback']:
                 continue
             self.getMass()
         print('Stop listening...')
         return
 
-    def _read(self):
+    def _read(self) -> str:
         """
         Read response from device
 
         Returns:
             str: response string
         """
         response = ''
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/__init__.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 Classes:
     Instrument (ABC)
     Measurer (ABC)
     Program (ABC)
     Programmable (Measurer)
     ProgramDetails (dataclass)
-    
+
 Functions:
     get_program_details
 """
 from .instrument_utils import Instrument
 from .measure_utils import Measurer, Programmable
 from .program_utils import Program, ProgramDetails, get_program_details
 
-from controllably import include_this_module
-include_this_module(get_local_only=False)
+# from controllably import include_this_module
+# include_this_module(get_local_only=False)
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/instrument_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,16 +146,17 @@
         Set flags by using keyword arguments
 
         Kwargs:
             key, value: (flag name, boolean) pairs
         """
         if not all([type(v)==bool for v in kwargs.values()]):
             raise ValueError("Ensure all assigned flag values are boolean.")
-        for key, value in kwargs.items():
-            self.flags[key] = value
+        self.flags.update(kwargs)
+        # for key, value in kwargs.items():
+        #     self.flags[key] = value
         return
   
     def shutdown(self):
         """Shutdown procedure for tool"""
         self.reset()
         self.disconnect()
         return
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/measure_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     - `buffer_df` (pd.DataFrame): buffer dataframe to store collected data
     - `connection_details` (dict): dictionary of connection details (e.g. COM port / IP address)
     - `device` (Callable): device object that communicates with physical tool
     - `flags` (dict[str, bool]): keywords paired with boolean flags
     - `verbose` (bool): verbosity of class
     
     ### Properties
-    - `instrument`: Alias for `device`
+    - `instrument` (Callable): Alias for `device`
     
     ### Methods
     #### Abstract
     - `clearCache`: clear most recent data and configurations
     - `disconnect`: disconnect from device
     - `_connect`: connection procedure for tool
     #### Public
@@ -161,16 +161,17 @@
         Set flags by using keyword arguments
 
         Kwargs:
             key, value: (flag name, boolean) pairs
         """
         if not all([type(v)==bool for v in kwargs.values()]):
             raise ValueError("Ensure all assigned flag values are boolean.")
-        for key, value in kwargs.items():
-            self.flags[key] = value
+        self.flags.update(kwargs)
+        # for key, value in kwargs.items():
+        #     self.flags[key] = value
         return
     
     def shutdown(self):
         """Shutdown procedure for tool"""
         self.reset()
         self.disconnect()
         return
@@ -189,20 +190,20 @@
     #### Class
     - `model` (str): model name of class
     #### Instance
     - `data` (Data): instantiated Data class with data in buffer
     - `datatype` (Data): Data class
     - `program` (Program): instantiated Program class with parameters provided
     - `program_details` (ProgramDetails): program details such as inputs, defaults, and docstring
-    - `program_parser` (function): function to get the program details from the program class docstring
     - `program_type` (Program): Program class
     - `recent_parameters` (list[dict[str, ...]]): list of previously used parameters
     
     ### Properties
-    - `instrument`: alias for `device`
+    - `instrument` (Callable): alias for `device`
+    - `program_parser` (Callable): function to get the program details from the program class docstring
     
     ### Methods
     #### Abstract
     - `disconnect`: disconnect from device
     - `_connect`: connection procedure for tool
     #### Public
     - `clearCache`: clear most recent data and configurations
@@ -221,30 +222,38 @@
     _default_flags = {
         'busy': False,
         'connected': False,
         'measured': False,
         'read': False,
         'stop_measure': False
     }
-    model = ''
-    available_programs: tuple[str] = ('',)      # FIXME
-    possible_inputs: tuple[str] = ('',)         # FIXME
+    _place: str = '.'.join(__name__.split('.')[1:-1])
+    model: str = ''
     def __init__(self, **kwargs):
         """Instantiate the class"""
         super().__init__(**kwargs)
         self.data: Optional[Data] = None
         self.datatype: Optional[Data] = self._default_datatype
         self.program: Optional[Program] = None
-        self.program_parser = self._default_program_parser
+        self._program_parser = self._default_program_parser
         self.program_type: Optional[Program] = self._default_program
         
         self.program_details = ProgramDetails()
         self.recent_parameters = []
         self._measure_method_docstring = self.measure.__doc__
         return
+    
+    # Properties
+    @property
+    def program_parser(self) -> Callable:
+        return self._program_parser.get('parser', lambda x:x)
+    @program_parser.setter
+    def program_parser(self, func: Callable):
+        self._program_parser['parser'] = func
+        return 
           
     def clearCache(self):
         """Clear most recent data and configurations """
         self.buffer_df = pd.DataFrame()
         self.data = None
         self.program = None
         self.setFlag(measured=False, read=False, stop_measure=False)
@@ -295,15 +304,15 @@
     def loadProgramInterpreter(self, program_parser: Optional[function] = None):
         """
         Load a program interpreter to get the program details from the program class docstring
 
         Args:
             program_parser (Optional[function], optional): function that interprets the program class docstring. Defaults to None.
         """
-        self.program_parser = self._default_program_parser if program_parser is None else {"parser": program_parser}
+        self._program_parser = self._default_program_parser if program_parser is None else {"parser": program_parser}
         return
     
     def measure(self, parameters: Optional[dict] = None, channel:Union[int, tuple[int]] = 0, **kwargs):
         """
         Perform measurement using loaded Program and parameters provided.
         Use `help()` to find out about program parameters.
 
@@ -385,12 +394,11 @@
             Exception: Load a program first
             
         Returns:
             ProgramDetails: details of program class
         """
         if self.program_type is None:
             raise Exception('Load a program first.')
-        parser = self.program_parser["parser"]
-        details = parser(program_class=self.program_type, verbose=self.verbose)
+        details = self.program_parser(program_class=self.program_type, verbose=self.verbose)
         self.program_details: ProgramDetails = details
         return details
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Measure/program_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Base Program template
 
     ### Constructor
     Args:
         `device` (Device): device object
         `parameters` (Optional[dict], optional): dictionary of kwargs. Defaults to None.
         `verbose` (bool, optional): verbosity of class. Defaults to False.
-
+    
     ### Attributes
     - `data_df` (pd.DataFrame): data collected from device when running the program
     - `device` (Device): device object
     - `parameters` (dict[str, ...]): parameters
     - `verbose` (bool): verbosity of class
     
     ### Methods
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     - `moveBy`: move the robot by target direction
     - `moveTo`: move the robot to target position
     - `reset`: reset the robot
     - `setSpeed`: set the speed of the robot
     - `shutdown`: shutdown procedure for tool
     """
     
+    _place: str = '.'.join(__name__.split('.')[1:-1])
     def __init__(self, 
         port: str, 
         limits: tuple[tuple[float]] = ((0, 0, 0), (0, 0, 0)), 
         safe_height: Optional[float] = None, 
         max_speed: float = 250, # [mm/s] (i.e. 15,000 mm/min)
         **kwargs
     ):
@@ -176,15 +177,15 @@
     
     def reset(self):
         """Reset the robot"""
         self.disconnect()
         self.connect()
         return super().reset()
     
-    def setSpeed(self, speed: int): # NOTE: waiting for PR #48
+    def setSpeed(self, speed: int):
         """
         Set the speed of the robot
 
         Args:
             speed (int): speed in mm/s
         """
         print(f'Speed: {speed} mm/s')
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ### Constructor
     Args:
         `port` (str): COM port address
         `limits` (tuple[tuple[float]], optional): lower and upper limits of gantry. Defaults to ((-410,-290,-120), (0,0,0)).
         `safe_height` (float, optional): height at which obstacles can be avoided. Defaults to -80.
         `max_speed` (float, optional): maximum travel speed. Defaults to 250.
     
-    ### Methods:
+    ### Methods
     - `home`: make the robot go home
     """
     def __init__(self, 
         port: str, 
         limits: tuple[tuple[float]] = ((-410,-290,-120), (0,0,0)), 
         safe_height: float = -80, 
         max_speed: float = 250, # [mm/s] (i.e. 15,000 mm/min)
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     Abstract Base Class (ABC) for Dobot objects. Dobot provides controls for articulated robots from Dobot.
     ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
     
     ### Constructor
     Args:
         `ip_address` (str): IP address of Dobot
         `attachment_name` (str, optional): name of attachment. Defaults to None.
-
+    
     ### Attributes
     - `attachment` (DobotAttachment): attached Dobot tool
     
     ### Properties
     - `dashboard` (dobot_api_dashboard): connection to status and signal control
     - `feedback` (dobot_api_feedback): connection to movement controls
     - `ip_address` (str): IP address of Dobot
@@ -66,16 +66,15 @@
     - `reset`: reset the robot
     - `setSpeed`: set the speed of the robot
     - `shutdown`: shutdown procedure for tool
     - `toggleAttachment`: couple or remove Dobot attachment that interfaces with Dobot's digital output
     - `toggleCalibration`: enter or exit calibration mode, with a sharp point implement for alignment
     """
     
-    possible_attachments = ['TwoJawGrip', 'VacuumGrip']     ### FIXME: hard-coded
-    max_actions = 5                                         ### FIXME: hard-coded
+    _place: str = '.'.join(__name__.split('.')[1:-1])
     def __init__(self, ip_address:str, attachment_name:str = None, **kwargs):
         """
         Instantiate the class
 
         Args:
             ip_address (str): IP address of Dobot
             attachment_name (str, optional): name of attachment. Defaults to None.
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     ### Constructor
     Args:
         `ip_address` (str): IP address of Dobot
         `right_handed` (bool, optional): whether the robot is in right-handed mode (i.e elbow bends to the right). Defaults to True.
         `safe_height` (float, optional): height at which obstacles can be avoided. Defaults to 100.
         `home_coordinates` (tuple[float], optional): home coordinates for the robot. Defaults to (0,300,100).
     
-    ## Methods
+    ### Methods
     - `home`: make the robot go home
     - `isFeasible`: checks and returns whether the target coordinate is feasible
     - `moveCoordBy`: relative Cartesian movement and tool orientation, using robot coordinates
     - `retractArm`: tuck in arm, rotate about base, then extend again (NOTE: not implemented)
     - `setHandedness`: set the handedness of the robot
     - `stretchArm`: extend the arm to full reach
     """
@@ -60,15 +60,15 @@
         super().__init__(
             ip_address=ip_address, 
             safe_height=safe_height,
             home_coordinates=home_coordinates, 
             **kwargs
         )
         self._speed_angular_max = 180
-        self.setHandedness(right_hand=right_handed, stretch=False)
+        self.setHandedness(right_hand=right_handed, stretch=True)
         self.home()
         return
     
     def home(self, safe:bool = True, tool_offset:bool = False) -> bool:
         """
         Make the robot go home
 
@@ -118,15 +118,16 @@
         # Space constraints
         # if x > 344: # front edge
         #     return False
         # if x < 76 and abs(y) < 150: # elevated structure
         #     return False
         
         grad = abs(y/(x+1E-6))
-        if grad > 0.75 or x < 0:
+        gradient_threshold = 0.1
+        if grad > gradient_threshold or x < 0:
             right_hand = (y>0)
             self.setHandedness(right_hand=right_hand, stretch=True) 
         return not self.deck.is_excluded(self._transform_out(coordinates, tool_offset=True))
     
     def moveCoordBy(self, 
         vector: tuple[float] = (0,0,0), 
         angles: tuple[float] = (0,0,0)
@@ -160,39 +161,39 @@
         Args:
             right_hand (bool): whether to select right-handedness
             stretch (bool, optional): whether to stretch the arm. Defaults to False.
 
         Returns:
             bool: whether movement is successful
         """
-        set_value = None
-        if not right_hand and self.flags['right_handed'] != False:  # Set to left-handed: 0
-            set_value = 0
-        elif right_hand and self.flags['right_handed'] != True:     # Set to right-handed: 1
-            set_value = 1
-        else:
+        if right_hand == self.flags['right_handed']:
             return False
         
         try:
-            self.dashboard.SetArmOrientation(set_value,1,1,1)
+            self.dashboard.SetArmOrientation(int(right_hand),1,1,1)
         except (AttributeError, OSError):
             if self.verbose:
                 print("Not connected to arm!")
         else:
             time.sleep(2)
             if stretch:
                 self.stretchArm()
                 time.sleep(1)
-        self.setFlag(right_handed=bool(set_value))
+        self.setFlag(right_handed=right_hand)
         return True
             
     def stretchArm(self) -> bool:
         """
         Extend the arm to full reach
         
         Returns:
             bool: whether movement is successful
         """
-        _,y,z = self.coordinates
-        y = 240 * math.copysign(1, y)
-        return self.moveCoordTo(coordinates=(320,y,z))
-   
+        x,y,z = self.coordinates
+        y_stretch = math.copysign(240, y)
+        z_home = self.home_coordinates[2]
+        ret1 = self.moveCoordTo(coordinates=(x,y,z_home))
+        ret2 = self.moveCoordTo(coordinates=(320,y_stretch,z_home))
+        ret3 = self.moveCoordTo(coordinates=(x,y,z_home))
+        ret4 = self.moveCoordTo(coordinates=(x,y,z))
+        return all([ret1,ret2,ret3,ret4])
+
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Abstract Base Class (ABC) for Robot Arm objects. RobotArm provides controls for jointed robots with articulated arms.
     ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
     
     ### Constructor
     Args:
         `safe_height` (Optional[float], optional): height at which obstacles can be avoided. Defaults to None.
         `retract` (bool, optional): whether to retract arm before movement. Defaults to False.
-
+    
     ### Properties
     - `speed_angular` (float): angular speed of the robot
 
     ### Methods
     #### Abstract
     - `disconnect`: disconnect from device
     - `isFeasible`: checks and returns whether the target coordinate is feasible
@@ -50,14 +50,15 @@
     """
     
     _default_flags = {
         'busy': False,
         'connected': False,
         'retract': False
     }
+    _place: str = '.'.join(__name__.split('.')[1:-1])
     def __init__(self, safe_height:Optional[float] = None, retract:bool = False, **kwargs):
         """
         Instantiate the class
 
         Args:
             safe_height (Optional[float], optional): height at which obstacles can be avoided. Defaults to None.
             retract (bool, optional): whether to retract arm before movement. Defaults to False.
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Move/move_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Move/move_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,16 +84,15 @@
     - `setHeight`: set predefined heights using keyword arguments
     - `setImplementOffset`: set offset of attached implement, then home if desired
     - `updatePosition`: update attributes to current position
     """
     
     _default_flags: dict[str, bool] = {'busy': False, 'connected': False}
     _default_heights: dict[str, float] = {}
-    possible_attachments = ()                               ### FIXME: hard-coded
-    max_actions = 5                                         ### FIXME: hard-coded
+    _place: str = '.'.join(__name__.split('.')[1:-1])
     def __init__(self, 
         coordinates: tuple[float] = (0,0,0),
         deck: Layout.Deck = Layout.Deck(),
         home_coordinates: tuple[float] = (0,0,0),
         home_orientation: tuple[float] = (0,0,0),
         implement_offset: tuple[float] = (0,0,0),
         orientate_matrix: np.ndarray = np.identity(3),
@@ -578,16 +577,17 @@
         Set flags by using keyword arguments
 
         Kwargs:
             key, value: (flag name, boolean) pairs
         """
         if not all([type(v)==bool for v in kwargs.values()]):
             raise ValueError("Ensure all assigned flag values are boolean.")
-        for key, value in kwargs.items():
-            self.flags[key] = value
+        self.flags.update(kwargs)
+        # for key, value in kwargs.items():
+        #     self.flags[key] = value
         return
     
     def setHeight(self, overwrite:bool = False, **kwargs):
         """
         Set predefined heights using keyword arguments
 
         Args:
@@ -731,42 +731,50 @@
 
 
     ### NOTE: DEPRECATE
     def getPosition(self):
         """
         Get robot coordinates and orientation.
         
+        TO BE DEPRECATED: Use `position` attribute instead.
+        
         Returns:
             tuple, tuple: x,y,z coordinates; a,b,c angles
         """
         print("`getPosition()` to be deprecated. Use `position` attribute instead.")
         return self.position
     
     def getToolPosition(self):
         """
         Retrieve coordinates of tool tip/end of implement.
+        
+        TO BE DEPRECATED: Use `tool_position` attribute instead.
 
         Returns:
             tuple, tuple: x,y,z coordinates; a,b,c angles
         """
         print("`getToolPosition()` to be deprecated. Use `tool_position` attribute instead.")
         return self.tool_position
     
     def getUserPosition(self):
         """
         Retrieve user-defined workspace coordinates.
+        
+        TO BE DEPRECATED: Use `user_position` attribute instead.
 
         Returns:
             tuple, tuple: x,y,z coordinates; a,b,c angles
         """
         print("`getUserPosition()` to be deprecated. Use `user_position` attribute instead.")
         return self.user_position
     
     def getWorkspacePosition(self):
         """
-        Alias for getUserPosition
+        Alias for getUserPosition.
+        
+        TO BE DEPRECATED: Use `workspace_position` attribute instead.
 
         Returns:
             tuple, tuple: x,y,z coordinates; a,b,c angles
         """
         print("`getWorkspacePosition()` to be deprecated. Use `workspace_position` attribute instead.")
         return self.workspace_position
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Args:
         `port` (str): COM port address
         `channel` (Union[int, tuple[int]]): channel id(s)
         `model` (Union[str, tuple[str]]): model name(s)
         `capacity` (Union[int, tuple[int]]): capacity (capacities)
         `output_right` (Union[bool, tuple[bool]]): whether liquid is pumped out to the right for channel(s)
         `name` (Union[str, tuple[str]], optional): name of the pump(s). Defaults to ''.
-        
+    
     ### Attributes
     - `channels` (dict[int, TriContinentPump]): dictionary of {channel id, TriContinentPump object}
     - `current_channel` (TriContinentPump): currently active pump
     - `name` (str): name of current pump
     - `capacity` (int): syringe capacity of current pump
     - `resolution` (float): volume resolution of current pump (i.e. uL per step)
     - `limits` (int): maximum allowable position of current pump
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,276 +1,266 @@
 # %% -*- coding: utf-8 -*-
 """
-This module holds the class for peristaltic pumps.
+This module holds the classes for substrate gripper tools from Dobot.
 
 Classes:
-    Peristaltic (Pump)
+    DobotGripper (Gripper)
+    TwoJawGrip (DobotGripper)
+    VacuumGrip (DobotGripper)
 """
 # Standard library imports
 from __future__ import annotations
+import numpy as np
 import time
-from typing import Optional, Union
+from typing import Callable, Optional
 
 # Local application imports
-from .pump_utils import Pump
+from ....misc import Helper
+from ..substrate_utils import Gripper
 print(f"Import: OK <{__name__}>")
 
-class Peristaltic(Pump):
+class DobotGripper(Gripper):
     """
-    Peristaltic provides methods to control a generic peristaltic pump
+    Abstract Base Class (ABC) for Dobot Gripper objects.
+    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
 
     ### Constructor
     Args:
-        `port` (str): COM port address
-        `output_clockwise` (bool, optional): whether liquid is pumped out when turned clockwise. Defaults to False.
+        `dashboard` (Optional[Callable], optional): connection to status and signal control. Defaults to None.
+        `channel_map` (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
+    
+    ### Attributes
+    - `dashboard` (Callable): connection to status and signal control
+    
+    ### Properties
+    - `channel_map` (dict): mapping of digital I/O channel(s)
+    - `implement_offset` (np.ndarray): offset from attachment site to tooltip
     
     ### Methods
-    - `aspirate`: aspirate desired volume of reagent
-    - `blowout`: blowout liquid from tip (NOTE: not implemented)
-    - `dispense`: dispense desired volume of reagent
-    - `pull`: pull liquid in, away from outlet
-    - `pullback`: pullback liquid from tip
-    - `push`: push liquid out, towards the outlet
-    - `setCurrentChannel`: set the current active channel
-    - `setValve`: open or close the valve for a specified channel
-    - `stop`: stop the pump
-    - `turnAntiClockwise`: spin the pump anti-clockwise at a specified speed
-    - `turnClockwise`: spin the pump clockwise at a specified speed
+    #### Abstract
+    - `drop`: releases an object
+    - `grab`: picks up an object
+    #### Public
+    - `setDashboard`: set the dashboard object
     """
     
-    _default_flags = {
-        'busy': False, 
-        'connected': False,
-        'output_clockwise': False
-    }
-    def __init__(self, port:str, output_clockwise:bool = False, **kwargs):
+    _implement_offset: tuple[float] = (0,0,0)
+    def __init__(self, dashboard:Optional[Callable] = None, channel_map:Optional[dict] = None):
         """
         Instantiate the class
 
         Args:
-            port (str): COM port address
-            output_clockwise (bool, optional): whether liquid is pumped out when turned clockwise. Defaults to False.
+            dashboard (Optional[Callable], optional): connection to status and signal control. Defaults to None.
+            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
         """
-        super().__init__(port=port, **kwargs)
-        self.setFlag(output_clockwise=output_clockwise)
+        self.dashboard = None
+        self._channel_map = {}
+        self.setDashboard(dashboard=dashboard, channel_map=channel_map)
+        return
+    
+    # Properties
+    @property
+    def channel_map(self) -> dict:
+        return self._channel_map
+    @channel_map.setter
+    def channel_map(self, value:dict):
+        if value is None:
+            self._channel_map = {}
+            return
+        if all([(1<= v <=24) for v in value.values()]):
+            self._channel_map = value
+        else:
+            raise ValueError("Please provide valid channel ids from 1 to 24.")
         return
     
-    def aspirate(self, speed:int, pump_time:int, channel:Optional[int] = None, **kwargs) -> bool:
+    @property
+    def implement_offset(self) -> np.ndarray:
+        return np.array(self._implement_offset)
+    
+    def setDashboard(self, dashboard:Callable, channel_map:Optional[dict] = None):
         """
-        Aspirate desired volume of reagent
+        Set the dashboard object
 
         Args:
-            speed (int): speed of pump rotation
-            pump_time (int): duration to run pump for
-            channel (Optional[int], optional): channel id. Defaults to None.
-
-        Returns:
-            bool: whether the action is successful
+            dashboard (Callable): connection to status and signal control
+            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
         """
-        self.setFlag(busy=True)
-        self.setValve(open=True, channel=channel)
-        
-        if self.pull(speed=speed):
-            time.sleep(pump_time)
-        self.stop()
-        
-        self.setValve(open=False, channel=channel)
-        self.setFlag(busy=False)
-        return True
+        self.dashboard = dashboard
+        self.channel_map = channel_map
+        return
     
-    def blowout(self, channel: Optional[Union[int, tuple[int]]] = None, **kwargs) -> bool: # NOTE: no implementation
-        return False
     
-    def dispense(self, speed:int, pump_time:int, channel:Optional[int] = None, **kwargs) -> bool:
+class TwoJawGrip(DobotGripper):
+    """
+    TwoJawGrip provides methods to operate the Dobot jaw gripper.
+    Channel map labels: `grab`
+    
+    ### Constructor
+    Args:
+        `dashboard` (Optional[Callable], optional): connection to status and signal control. Defaults to None.
+        `channel_map` (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
+    
+    ### Methods
+    - `drop`: releases an object by opening the gripper
+    - `grab`: picks up an object by closing the gripper
+    """
+    
+    _implement_offset = (0,0,-95)
+    def __init__(self, dashboard:Optional[Callable] = None, channel_map:Optional[dict] = None):
         """
-        Dispense desired volume of reagent
+        Instantiate the class
 
         Args:
-            speed (int): speed of pump rotation
-            pump_time (int): duration to run pump for
-            channel (Optional[int], optional): channel id. Defaults to None.
+            dashboard (Optional[Callable], optional): connection to status and signal control. Defaults to None.
+            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
+        """
+        super().__init__(dashboard=dashboard, channel_map=channel_map)
+        return
 
-        Returns:
-            bool: whether the action is successful
+    def drop(self) -> bool:
         """
-        self.setFlag(busy=True)
-        self.setValve(open=True, channel=channel)
-        
-        if self.push(speed=speed):
-            time.sleep(pump_time)
-        self.stop()
+        Releases an object by opening the gripper
         
-        self.setValve(open=False, channel=channel)
-        self.setFlag(busy=False)
+        Returns:
+            bool: whether action is successful
+        """
+        channel = self.channel_map.get("grab", 1)
+        try:
+            self.dashboard.DOExecute(channel, 1)
+        except (AttributeError, OSError):
+            print('Tried to drop...')
+            print("Not connected to arm.")
+            return False
         return True
     
-    def pull(self, speed:int) -> bool:
-        """
-        Pull liquid in, away from outlet
-
-        Args:
-            speed (int): speed of pump rotation
-
-        Returns:
-            bool: whether the action is successful
+    def grab(self) -> bool:
         """
-        pull_func = self.turnAntiClockwise if self.flags['output_clockwise'] else self.turnClockwise
-        return pull_func(speed=speed)
+        Picks up an object by closing the gripper
         
-    def pullback(self, speed:int, pump_time:int, channel:Optional[int] = None, **kwargs) -> bool:
-        """
-        Pullback liquid from tip
-
-        Args:
-            speed (int): speed of pump rotation
-            pump_time (int): duration to run pump for
-            channel (Optional[int], optional): channel id. Defaults to None.
-
         Returns:
-            bool: whether the action is successful
+            bool: whether action is successful
         """
-        self.setFlag(busy=True)
-        self.setValve(open=True, channel=channel)
-        
-        if self.pull(speed=speed):
-            time.sleep(pump_time)
-        self.stop()
-        
-        self.setValve(open=False, channel=channel)
-        self.setFlag(busy=False)
+        channel = self.channel_map.get("grab", 1)
+        try:
+            self.dashboard.DOExecute(channel, 0)
+        except (AttributeError, OSError):
+            print('Tried to grab...')
+            print("Not connected to arm.")
+            return False
         return True
-    
-    def push(self, speed:int) -> bool:
-        """
-        Push liquid out, towards the outlet
 
-        Args:
-            speed (int): speed of pump rotation
 
-        Returns:
-            bool: whether the action is successful
-        """
-        push_func = self.turnClockwise if self.flags['output_clockwise'] else self.turnAntiClockwise
-        return push_func(speed=speed)
+class VacuumGrip(DobotGripper):
+    """
+    VacuumGrip provides methods to operate the Dobot vacuum grip.
+    Channel map labels: `pull`, `push`
+    
+    ### Constructor
+    Args:
+        `dashboard` (Optional[Callable], optional): connection to status and signal control. Defaults to None.
+        `channel_map` (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
     
-    def setCurrentChannel(self, channel:Optional[int] = None) -> bool:
+    ### Methods
+    - `drop`: releases an object by pushing out air
+    - `grab`: picks up an object by pulling in air
+    - `pull`: activate pump to suck in air
+    - `push`: activate pump to blow out air
+    - `stop`: stop airflow
+    """
+    
+    _implement_offset = (0,0,-60)
+    def __init__(self, dashboard:Optional[Callable] = None, channel_map:Optional[dict] = None):
         """
-        Set the current active channel
+        Instantiate the class
 
         Args:
-            channel (Optional[int], optional): channel id. Defaults to None.
+            dashboard (Optional[Callable], optional): connection to status and signal control. Defaults to None.
+            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
+        """
+        super().__init__(dashboard=dashboard, channel_map=channel_map)
+        return
 
+    def drop(self) -> bool:
+        """
+        Releases an object by pushing out air
+        
         Returns:
-            bool: whether the action is successful
+            bool: whether action is successful
         """
-        self.setValve(False)
-        return self.setValve(open=True, channel=channel)
+        print('Tried to drop...')
+        return self.push(0.5)
     
-    def setValve(self, open:bool = False, channel:Optional[int] = None) -> bool:
+    def grab(self) -> bool:
         """
-        Open or close the valve for a specified channel.
-        Closes all valves if no input is given.
-
-        Args:
-            open (bool, optional): whether to open or close the valve. Defaults to False.
-            channel (Optional[int], optional): channel id. Defaults to None.
-
-        Raises:
-            ValueError: Please select a channel from 1-8
-
+        Picks up an object by pulling in air
+        
         Returns:
-            bool: whether the action is successful
+            bool: whether action is successful
         """
-        state = 0
-        if channel is None:
-            state = 9
-        elif type(channel) is int and (1<= channel <=8):
-            state = -channel if open else channel
-        if state == 0:
-            raise ValueError("Please select a channel from 1-8.")
-        return self._write(f"{state}\n")
-    
-    def stop(self) -> bool:
-        """Stop the pump"""
-        return self._write("10\n")
+        print('Tried to grab...')
+        return self.pull(3)
     
-    def turnAntiClockwise(self, speed:int) -> bool:
+    def pull(self, duration:Optional[int] = None) -> bool:
         """
-        Spin the pump anti-clockwise at a specified speed
+        Activate pump to suck in air
         
         Args:
-            speed (int): speed of pump rotation
+            duration (Optional[int], optional): number of seconds to pull air. Defaults to None.
+        
+        Returns:
+            bool: whether action is successful
         """
-        return self._turn_pump(abs(speed))
+        channel = self.channel_map.get("pull", 1)
+        try:
+            self.dashboard.DOExecute(channel, 1)
+        except (AttributeError, OSError):
+            print('Tried to pull...')
+            print("Not connected to arm.")
+            return False
+        else:
+            if duration is not None:
+                time.sleep(duration)
+                self.dashboard.DOExecute(channel, 0)
+                time.sleep(1)
+        return True
     
-    def turnClockwise(self, speed:int) -> bool:
+    def push(self, duration:Optional[int] = None) -> bool:
         """
-        Spin the pump clockwise at a specified speed
+        Activate pump to blow out air
         
         Args:
-            speed (int): speed of pump rotation
-        """
-        return self._turn_pump(-abs(speed))
-     
-    # Protected method(s)
-    def _connect(self, port: str, baudrate: int = 9600, timeout: int = 1):
-        """
-        Connection procedure for tool
-
-        Args:
-            port (str): COM port address
-            baudrate (int, optional): baudrate. Defaults to 9600.
-            timeout (int, optional): timeout in seconds. Defaults to 1.
+            duration (Optional[int], optional): number of seconds to push air. Defaults to None.
+            
+        Returns:
+            bool: whether action is successful
         """
-        super()._connect(port, baudrate, timeout)
-        self.setValve(False)
-        return
+        channel = self.channel_map.get("push", 2)
+        try:
+            self.dashboard.DOExecute(channel, 1)
+        except (AttributeError, OSError):
+            print('Tried to push...')
+            print("Not connected to arm.")
+            return False
+        else:
+            if duration is not None:
+                time.sleep(duration)
+                self.dashboard.DOExecute(channel, 0)
+                time.sleep(1)
+        return True
     
-    def _turn_pump(self, speed:int) -> bool:
+    def stop(self) -> bool:
         """
-        Relay instructions to pump
+        Stop airflow
         
-        Args:
-            speed (int): speed of pump rotation
+        Returns:
+            bool: whether action is successful
         """
-        return self._write(f"{speed}\n")
-
-
-    ### NOTE: DEPRECATE
-    # def _push(self, speed:int, push_time:int, pullback_time:int, channel:int):
-    #     """
-    #     Dispense (aspirate) liquid from (into) syringe
-        
-    #     Args:
-    #         speed (int): speed of pump of rotation (<0 aspirate; >0 dispense)
-    #         push_time (int, or float): time to achieve desired volume
-    #         pullback_time (int, or float): time to pullback the peristaltic pump
-    #         channel (int): valve channel
-    #     """
-    #     run_time = pullback_time + push_time
-    #     interval = 0.1
-        
-    #     start_time = time.time()
-    #     self.setValve(open=True, channel=channel)
-    #     self._turn_pump(speed)
-        
-    #     while(True):
-    #         time.sleep(0.001)
-    #         if (interval <= time.time() - start_time):
-    #             interval += 0.1
-    #         if (run_time <= time.time() - start_time):
-    #             break
-        
-    #     start_time = time.time()
-    #     self.setValve(open=True, channel=channel)
-    #     self._turn_pump(-abs(speed))
-
-    #     while(True):
-    #         time.sleep(0.001)
-    #         if (interval <= time.time() - start_time):
-    #             interval += 0.1
-    #         if (pullback_time <= time.time() - start_time):
-    #             self._turn_pump(10)
-    #             self.setValve(open=False, channel=channel)
-    #             break
-    #     return
-    
+        channels = [v for v in self.channel_map.values()] if len(self.channel_map) else [1,2]
+        try:
+            for channel in channels:
+                self.dashboard.DOExecute(channel, 0)
+            time.sleep(1)
+        except (AttributeError, OSError):
+            print('Tried to stop...')
+            print("Not connected to arm.")
+            return False
+        return True
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,14 @@
     StatusCode (Enum)
     StatusQueryCode (Enum)
     Model (dataclass)
 
 Other types:
     PresetSpeeds (namedtuple)
     SpeedParameters (namedtuple)
-
-Other constants and variables:
-    QUERIES (list)  
-    STATIC_QUERIES (list)
-    STATUS_QUERIES (list)
 """
 # Standard library imports
 from collections import namedtuple
 from dataclasses import dataclass
 from enum import Enum
 print(f"Import: OK <{__name__}>")
 
@@ -69,27 +64,21 @@
 class StatusCode(Enum):
     Normal          = 0
     Braking         = 1
     Running         = 2
     Drive_Busy      = 4
     Running_Busy    = 6
     General_Error   = 8
-
+    
 class StaticQueryCode(Enum):
-    Version         = 'DV'
-    Model           = 'DM'
-    Cycles          = 'DX'
-    Speed_In        = 'DI'
-    Speed_Out       = 'DO'
-    Resolution      = 'DR'
+    DV  = 'Version'
+    DM  = 'Model'
+    DX  = 'Cycles'
+    DI  = 'Speed In'
+    DO  = 'Speed_Out'
+    DR  = 'Resolution'
     
 class StatusQueryCode(Enum):
-    Status          = 'DS'
-    Errors          = 'DE'
-    Position        = 'DP'
-    Liquid_Sensor   = 'DN'
-
-
-# FIXME: Do away with these objects below
-STATIC_QUERIES  = [static_query.value for static_query in StaticQueryCode]
-STATUS_QUERIES  = [status_query.value for status_query in StatusQueryCode]
-QUERIES         = STATUS_QUERIES + STATIC_QUERIES
+    DS  = 'Status'
+    DE  = 'Errors'
+    DP  = 'Position'
+    DN  = 'Liquid Sensor'
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,1950 +26,1956 @@
 00000190: 7365 7269 616c 2023 2070 6970 2069 6e73  serial # pip ins
 000001a0: 7461 6c6c 2070 7973 6572 6961 6c0d 0a0d  tall pyserial...
 000001b0: 0a23 204c 6f63 616c 2061 7070 6c69 6361  .# Local applica
 000001c0: 7469 6f6e 2069 6d70 6f72 7473 0d0a 6672  tion imports..fr
 000001d0: 6f6d 202e 2e6c 6971 7569 645f 7574 696c  om ..liquid_util
 000001e0: 7320 696d 706f 7274 204c 6971 7569 6448  s import LiquidH
 000001f0: 616e 646c 6572 2c20 5370 6565 640d 0a66  andler, Speed..f
-00000200: 726f 6d20 2e73 6172 746f 7269 7573 5f6c  rom .sartorius_l
-00000210: 6962 2069 6d70 6f72 7420 4572 726f 7243  ib import ErrorC
-00000220: 6f64 652c 204d 6f64 656c 496e 666f 2c20  ode, ModelInfo, 
-00000230: 5374 6174 7573 436f 6465 2c20 5370 6565  StatusCode, Spee
-00000240: 6450 6172 616d 6574 6572 732c 204d 6f64  dParameters, Mod
-00000250: 656c 0d0a 6672 6f6d 202e 7361 7274 6f72  el..from .sartor
-00000260: 6975 735f 6c69 6220 696d 706f 7274 2053  ius_lib import S
-00000270: 5441 5455 535f 5155 4552 4945 532c 2051  TATUS_QUERIES, Q
-00000280: 5545 5249 4553 0d0a 7072 696e 7428 6622  UERIES..print(f"
-00000290: 496d 706f 7274 3a20 4f4b 203c 7b5f 5f6e  Import: OK <{__n
-000002a0: 616d 655f 5f7d 3e22 290d 0a0d 0a53 5445  ame__}>")....STE
-000002b0: 505f 5245 534f 4c55 5449 4f4e 203d 2031  P_RESOLUTION = 1
-000002c0: 300d 0a22 2222 4d69 6e69 6d75 6d20 6e75  0.."""Minimum nu
-000002d0: 6d62 6572 206f 6620 7374 6570 7320 746f  mber of steps to
-000002e0: 2068 6176 6520 746f 6c65 7261 626c 6520   have tolerable 
-000002f0: 6572 726f 7273 2069 6e20 766f 6c75 6d65  errors in volume
-00000300: 2222 220d 0a0d 0a63 6c61 7373 2053 6172  """....class Sar
-00000310: 746f 7269 7573 284c 6971 7569 6448 616e  torius(LiquidHan
-00000320: 646c 6572 293a 0d0a 2020 2020 2222 220d  dler):..    """.
-00000330: 0a20 2020 2053 6172 746f 7269 7573 206f  .    Sartorius o
-00000340: 626a 6563 740d 0a0d 0a20 2020 2023 2323  bject....    ###
-00000350: 2043 6f6e 7374 7275 6374 6f72 0d0a 2020   Constructor..  
-00000360: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-00000370: 2060 706f 7274 6020 2873 7472 293a 2043   `port` (str): C
-00000380: 4f4d 2070 6f72 7420 6164 6472 6573 730d  OM port address.
-00000390: 0a20 2020 2020 2020 2060 6368 616e 6e65  .        `channe
-000003a0: 6c60 2028 696e 742c 206f 7074 696f 6e61  l` (int, optiona
-000003b0: 6c29 3a20 6368 616e 6e65 6c20 6964 2e20  l): channel id. 
-000003c0: 4465 6661 756c 7473 2074 6f20 312e 0d0a  Defaults to 1...
-000003d0: 2020 2020 2020 2020 606f 6666 7365 7460          `offset`
-000003e0: 2028 7475 706c 655b 666c 6f61 745d 2c20   (tuple[float], 
-000003f0: 6f70 7469 6f6e 616c 293a 2078 2c79 2c7a  optional): x,y,z
-00000400: 206f 6666 7365 7420 6f66 2074 6970 2e20   offset of tip. 
-00000410: 4465 6661 756c 7473 2074 6f20 2830 2c30  Defaults to (0,0
-00000420: 2c30 292e 0d0a 2020 2020 2020 2020 6072  ,0)...        `r
-00000430: 6573 706f 6e73 655f 7469 6d65 6020 2866  esponse_time` (f
-00000440: 6c6f 6174 2c20 6f70 7469 6f6e 616c 293a  loat, optional):
-00000450: 2064 656c 6179 2062 6574 7765 656e 2073   delay between s
-00000460: 656e 6469 6e67 2061 2063 6f6d 6d61 6e64  ending a command
-00000470: 2061 6e64 2072 6563 6569 7669 6e67 2061   and receiving a
-00000480: 2072 6573 706f 6e73 652c 2069 6e20 7365   response, in se
-00000490: 636f 6e64 732e 2044 6566 6175 6c74 7320  conds. Defaults 
-000004a0: 746f 2031 2e30 332e 0d0a 2020 2020 2020  to 1.03...      
-000004b0: 2020 6074 6970 5f74 6872 6573 686f 6c64    `tip_threshold
-000004c0: 6020 2869 6e74 2c20 6f70 7469 6f6e 616c  ` (int, optional
-000004d0: 293a 2074 6872 6573 686f 6c64 2061 626f  ): threshold abo
-000004e0: 7665 2077 6869 6368 2061 2063 6f6e 6475  ve which a condu
-000004f0: 6374 6976 6520 7069 7065 7474 6520 7469  ctive pipette ti
-00000500: 7020 6973 2063 6f6e 7369 6465 7265 6420  p is considered 
-00000510: 746f 2062 6520 6174 7461 6368 6564 2e20  to be attached. 
-00000520: 4465 6661 756c 7473 2074 6f20 3237 362e  Defaults to 276.
-00000530: 0d0a 2020 2020 0d0a 2020 2020 2323 2320  ..    ..    ### 
-00000540: 4174 7472 6962 7574 6573 0d0a 2020 2020  Attributes..    
-00000550: 2d20 6063 6861 6e6e 656c 6020 2869 6e74  - `channel` (int
-00000560: 293a 2063 6861 6e6e 656c 2069 640d 0a20  ): channel id.. 
-00000570: 2020 202d 2060 6c69 6d69 7473 6020 2874     - `limits` (t
-00000580: 7570 6c65 5b69 6e74 5d29 3a20 6c6f 7765  uple[int]): lowe
-00000590: 7220 616e 6420 7570 7065 7220 7374 6570  r and upper step
-000005a0: 206c 696d 6974 730d 0a20 2020 202d 2060   limits..    - `
-000005b0: 6d6f 6465 6c5f 696e 666f 6020 2853 6172  model_info` (Sar
-000005c0: 746f 7269 7573 5069 7065 7474 654d 6f64  toriusPipetteMod
-000005d0: 656c 293a 2053 6172 746f 7269 7573 206d  el): Sartorius m
-000005e0: 6f64 656c 2069 6e66 6f0d 0a20 2020 202d  odel info..    -
-000005f0: 2060 6f66 6673 6574 6020 2874 7570 6c65   `offset` (tuple
-00000600: 5b66 6c6f 6174 5d29 3a20 782c 792c 7a20  [float]): x,y,z 
-00000610: 6f66 6673 6574 206f 6620 7469 700d 0a20  offset of tip.. 
-00000620: 2020 202d 2060 706f 7369 7469 6f6e 6020     - `position` 
-00000630: 2869 6e74 293a 2070 6f73 6974 696f 6e20  (int): position 
-00000640: 6f66 2070 6c75 6e67 6572 0d0a 2020 2020  of plunger..    
-00000650: 2d20 6072 6573 706f 6e73 655f 7469 6d65  - `response_time
-00000660: 6020 2866 6c6f 6174 293a 2064 656c 6179  ` (float): delay
-00000670: 2062 6574 7765 656e 2073 656e 6469 6e67   between sending
-00000680: 2061 2063 6f6d 6d61 6e64 2061 6e64 2072   a command and r
-00000690: 6563 6569 7669 6e67 2061 2072 6573 706f  eceiving a respo
-000006a0: 6e73 652c 2069 6e20 7365 636f 6e64 730d  nse, in seconds.
-000006b0: 0a20 2020 202d 2060 7370 6565 645f 636f  .    - `speed_co
-000006c0: 6465 6020 2853 7065 6564 293a 2063 6f64  de` (Speed): cod
-000006d0: 6573 2066 6f72 2061 7370 6972 6174 6520  es for aspirate 
-000006e0: 616e 6420 6469 7370 656e 7365 2073 7065  and dispense spe
-000006f0: 6564 730d 0a20 2020 202d 2060 7370 6565  eds..    - `spee
-00000700: 645f 7072 6573 6574 7360 2028 5072 6573  d_presets` (Pres
-00000710: 6574 5370 6565 6473 293a 2070 7265 7365  etSpeeds): prese
-00000720: 7420 7370 6565 6473 2061 7661 696c 6162  t speeds availab
-00000730: 6c65 0d0a 2020 2020 2d20 6074 6970 5f6c  le..    - `tip_l
-00000740: 656e 6774 6860 2028 666c 6f61 7429 3a20  ength` (float): 
-00000750: 6c65 6e67 7468 206f 6620 7069 7065 7474  length of pipett
-00000760: 6520 7469 700d 0a20 2020 202d 2060 7469  e tip..    - `ti
-00000770: 705f 7468 7265 7368 6f6c 6460 2028 696e  p_threshold` (in
-00000780: 7429 3a20 7468 7265 7368 6f6c 6420 6162  t): threshold ab
-00000790: 6f76 6520 7768 6963 6820 6120 636f 6e64  ove which a cond
-000007a0: 7563 7469 7665 2070 6970 6574 7465 2074  uctive pipette t
-000007b0: 6970 2069 7320 636f 6e73 6964 6572 6564  ip is considered
-000007c0: 2074 6f20 6265 2061 7474 6163 6865 640d   to be attached.
-000007d0: 0a20 2020 200d 0a20 2020 2023 2320 5072  .    ..    ## Pr
-000007e0: 6f70 6572 7469 6573 0d0a 2020 2020 2d20  operties..    - 
-000007f0: 6063 6170 6163 6974 616e 6365 6020 2869  `capacitance` (i
-00000800: 6e74 293a 2063 6170 6163 6974 616e 6365  nt): capacitance
-00000810: 2061 7320 6d65 6173 7572 6564 2061 7420   as measured at 
-00000820: 7468 6520 656e 6420 6f66 2074 6865 2070  the end of the p
-00000830: 6970 6574 7465 0d0a 2020 2020 2d20 6068  ipette..    - `h
-00000840: 6f6d 655f 706f 7369 7469 6f6e 6020 2869  ome_position` (i
-00000850: 6e74 293a 2068 6f6d 6520 706f 7369 7469  nt): home positi
-00000860: 6f6e 206f 6620 7069 7065 7474 650d 0a20  on of pipette.. 
-00000870: 2020 202d 2060 706f 7274 6020 2873 7472     - `port` (str
-00000880: 293a 2043 4f4d 2070 6f72 7420 6164 6472  ): COM port addr
-00000890: 6573 730d 0a20 2020 202d 2060 7265 736f  ess..    - `reso
-000008a0: 6c75 7469 6f6e 6020 2866 6c6f 6174 293a  lution` (float):
-000008b0: 2076 6f6c 756d 6520 7265 736f 6c75 7469   volume resoluti
-000008c0: 6f6e 206f 6620 7069 7065 7474 6520 2869  on of pipette (i
-000008d0: 2e65 2e20 754c 2070 6572 2073 7465 7029  .e. uL per step)
-000008e0: 0d0a 2020 2020 2d20 6073 7461 7475 7360  ..    - `status`
-000008f0: 2028 7374 7229 3a20 7069 7065 7474 6520   (str): pipette 
-00000900: 7374 6174 7573 0d0a 2020 2020 0d0a 2020  status..    ..  
-00000910: 2020 2323 2320 4d65 7468 6f64 730d 0a20    ### Methods.. 
-00000920: 2020 202d 2060 6164 6441 6972 4761 7060     - `addAirGap`
-00000930: 3a20 6372 6561 7465 2061 6e20 6169 7220  : create an air 
-00000940: 6761 7020 6265 7477 6565 6e20 7477 6f20  gap between two 
-00000950: 766f 6c75 6d65 7320 6f66 206c 6971 7569  volumes of liqui
-00000960: 6420 696e 2070 6970 6574 7465 0d0a 2020  d in pipette..  
-00000970: 2020 2d20 6061 7370 6972 6174 6560 3a20    - `aspirate`: 
-00000980: 6173 7069 7261 7465 2064 6573 6972 6564  aspirate desired
-00000990: 2076 6f6c 756d 6520 6f66 2072 6561 6765   volume of reage
-000009a0: 6e74 2069 6e74 6f20 7069 7065 7474 650d  nt into pipette.
-000009b0: 0a20 2020 202d 2060 626c 6f77 6f75 7460  .    - `blowout`
-000009c0: 3a20 626c 6f77 6f75 7420 6c69 7175 6964  : blowout liquid
-000009d0: 2066 726f 6d20 7469 700d 0a20 2020 202d   from tip..    -
-000009e0: 2060 6469 7370 656e 7365 603a 2064 6973   `dispense`: dis
-000009f0: 7065 6e73 6520 6465 7369 7265 6420 766f  pense desired vo
-00000a00: 6c75 6d65 206f 6620 7265 6167 656e 740d  lume of reagent.
-00000a10: 0a20 2020 202d 2060 656a 6563 7460 3a20  .    - `eject`: 
-00000a20: 656a 6563 7420 7468 6520 7069 7065 7474  eject the pipett
-00000a30: 6520 7469 700d 0a20 2020 202d 2060 656d  e tip..    - `em
-00000a40: 7074 7960 3a20 656d 7074 7920 7468 6520  pty`: empty the 
-00000a50: 7069 7065 7474 650d 0a20 2020 202d 2060  pipette..    - `
-00000a60: 6765 7443 6170 6163 6974 616e 6365 603a  getCapacitance`:
-00000a70: 2067 6574 2074 6865 2063 6170 6163 6974   get the capacit
-00000a80: 616e 6365 2061 7320 6d65 6173 7572 6564  ance as measured
-00000a90: 2061 7420 7468 6520 656e 6420 6f66 2074   at the end of t
-00000aa0: 6865 2070 6970 6574 7465 0d0a 2020 2020  he pipette..    
-00000ab0: 2d20 6067 6574 4572 726f 7273 603a 2067  - `getErrors`: g
-00000ac0: 6574 2065 7272 6f72 7320 6672 6f6d 2074  et errors from t
-00000ad0: 6865 2064 6576 6963 650d 0a20 2020 202d  he device..    -
-00000ae0: 2060 6765 7449 6e66 6f60 3a20 6765 7420   `getInfo`: get 
-00000af0: 6465 7461 696c 7320 6f66 2074 6865 2053  details of the S
-00000b00: 6172 746f 7269 7573 2070 6970 6574 7465  artorius pipette
-00000b10: 206d 6f64 656c 0d0a 2020 2020 2d20 6067   model..    - `g
-00000b20: 6574 506f 7369 7469 6f6e 603a 2067 6574  etPosition`: get
-00000b30: 2074 6865 2063 7572 7265 6e74 2070 6f73   the current pos
-00000b40: 6974 696f 6e20 6f66 2074 6865 2070 6970  ition of the pip
-00000b50: 6574 7465 0d0a 2020 2020 2d20 6067 6574  ette..    - `get
-00000b60: 5374 6174 7573 603a 2067 6574 2074 6865  Status`: get the
-00000b70: 2073 7461 7475 7320 6f66 2074 6865 2070   status of the p
-00000b80: 6970 6574 7465 0d0a 2020 2020 2d20 6068  ipette..    - `h
-00000b90: 6f6d 6560 3a20 7265 7475 726e 2070 6c75  ome`: return plu
-00000ba0: 6e67 6572 2074 6f20 686f 6d65 2070 6f73  nger to home pos
-00000bb0: 6974 696f 6e0d 0a20 2020 202d 2060 6973  ition..    - `is
-00000bc0: 4665 6173 6962 6c65 603a 2063 6865 636b  Feasible`: check
-00000bd0: 7320 616e 6420 7265 7475 726e 7320 7768  s and returns wh
-00000be0: 6574 6865 7220 7468 6520 706c 756e 6765  ether the plunge
-00000bf0: 7220 706f 7369 7469 6f6e 2069 7320 6665  r position is fe
-00000c00: 6173 6962 6c65 0d0a 2020 2020 2d20 6069  asible..    - `i
-00000c10: 7354 6970 4f6e 603a 2063 6865 636b 7320  sTipOn`: checks 
-00000c20: 616e 6420 7265 7475 726e 7320 7768 6574  and returns whet
-00000c30: 6865 7220 6120 7069 7065 7474 6520 7469  her a pipette ti
-00000c40: 7020 6973 2061 7474 6163 6865 640d 0a20  p is attached.. 
-00000c50: 2020 202d 2060 6d6f 7665 603a 206d 6f76     - `move`: mov
-00000c60: 6520 7468 6520 706c 756e 6765 7220 6569  e the plunger ei
-00000c70: 7468 6572 2075 7020 6f72 2064 6f77 6e20  ther up or down 
-00000c80: 6279 2061 2073 7065 6369 6669 6564 206e  by a specified n
-00000c90: 756d 6265 7220 6f66 2073 7465 7073 0d0a  umber of steps..
-00000ca0: 2020 2020 2d20 606d 6f76 6542 7960 3a20      - `moveBy`: 
-00000cb0: 6d6f 7665 2074 6865 2070 6c75 6e67 6572  move the plunger
-00000cc0: 2062 7920 6120 7370 6563 6966 6965 6420   by a specified 
-00000cd0: 6e75 6d62 6572 206f 6620 7374 6570 730d  number of steps.
-00000ce0: 0a20 2020 202d 2060 6d6f 7665 546f 603a  .    - `moveTo`:
-00000cf0: 206d 6f76 6520 7468 6520 706c 756e 6765   move the plunge
-00000d00: 7220 746f 2061 2073 7065 6369 6669 6564  r to a specified
-00000d10: 2070 6f73 6974 696f 6e0d 0a20 2020 202d   position..    -
-00000d20: 2060 7075 6c6c 6261 636b 603a 2070 756c   `pullback`: pul
-00000d30: 6c62 6163 6b20 6c69 7175 6964 2066 726f  lback liquid fro
-00000d40: 6d20 7469 700d 0a20 2020 202d 2060 7265  m tip..    - `re
-00000d50: 7365 7460 3a20 7265 7365 7420 7468 6520  set`: reset the 
-00000d60: 7069 7065 7474 650d 0a20 2020 202d 2060  pipette..    - `
-00000d70: 7365 7453 7065 6564 603a 2073 6574 2074  setSpeed`: set t
-00000d80: 6865 2073 7065 6564 206f 6620 7468 6520  he speed of the 
-00000d90: 706c 756e 6765 720d 0a20 2020 202d 2060  plunger..    - `
-00000da0: 7368 7574 646f 776e 603a 2073 6875 7464  shutdown`: shutd
-00000db0: 6f77 6e20 7072 6f63 6564 7572 6520 666f  own procedure fo
-00000dc0: 7220 746f 6f6c 0d0a 2020 2020 2d20 6074  r tool..    - `t
-00000dd0: 6f67 676c 6546 6565 6462 6163 6b4c 6f6f  oggleFeedbackLoo
-00000de0: 7060 3a20 7374 6172 7420 6f72 2073 746f  p`: start or sto
-00000df0: 7020 6665 6564 6261 636b 206c 6f6f 700d  p feedback loop.
-00000e00: 0a20 2020 202d 2060 7a65 726f 603a 207a  .    - `zero`: z
-00000e10: 6572 6f20 7468 6520 706c 756e 6765 7220  ero the plunger 
-00000e20: 706f 7369 7469 6f6e 0d0a 2020 2020 2222  position..    ""
-00000e30: 220d 0a20 2020 200d 0a20 2020 205f 6465  "..    ..    _de
-00000e40: 6661 756c 745f 666c 6167 7320 3d20 7b0d  fault_flags = {.
-00000e50: 0a20 2020 2020 2020 2027 6275 7379 273a  .        'busy':
-00000e60: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00000e70: 2027 636f 6e64 7563 7469 7665 5f74 6970   'conductive_tip
-00000e80: 7327 3a20 4661 6c73 652c 0d0a 2020 2020  s': False,..    
-00000e90: 2020 2020 2763 6f6e 6e65 6374 6564 273a      'connected':
-00000ea0: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00000eb0: 2027 6765 745f 6665 6564 6261 636b 273a   'get_feedback':
-00000ec0: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00000ed0: 2027 6f63 6375 7069 6564 273a 2046 616c   'occupied': Fal
-00000ee0: 7365 2c0d 0a20 2020 2020 2020 2027 7061  se,..        'pa
-00000ef0: 7573 655f 6665 6564 6261 636b 273a 4661  use_feedback':Fa
-00000f00: 6c73 652c 0d0a 2020 2020 2020 2020 2774  lse,..        't
-00000f10: 6970 5f6f 6e27 3a20 4661 6c73 650d 0a20  ip_on': False.. 
-00000f20: 2020 207d 0d0a 2020 2020 696d 706c 656d     }..    implem
-00000f30: 656e 745f 6f66 6673 6574 203d 2028 302c  ent_offset = (0,
-00000f40: 302c 2d32 3530 290d 0a20 2020 2074 6970  0,-250)..    tip
-00000f50: 5f69 6e73 6574 5f6d 6d20 3d20 3132 0d0a  _inset_mm = 12..
-00000f60: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-00000f70: 2873 656c 662c 200d 0a20 2020 2020 2020  (self, ..       
-00000f80: 2070 6f72 743a 7374 722c 200d 0a20 2020   port:str, ..   
-00000f90: 2020 2020 2063 6861 6e6e 656c 3a20 696e       channel: in
-00000fa0: 7420 3d20 312c 200d 0a20 2020 2020 2020  t = 1, ..       
-00000fb0: 206f 6666 7365 743a 2074 7570 6c65 5b66   offset: tuple[f
-00000fc0: 6c6f 6174 5d20 3d20 2830 2c30 2c30 292c  loat] = (0,0,0),
-00000fd0: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-00000fe0: 7365 5f74 696d 653a 2066 6c6f 6174 203d  se_time: float =
-00000ff0: 2031 2e30 332c 0d0a 2020 2020 2020 2020   1.03,..        
-00001000: 7469 705f 7468 7265 7368 6f6c 643a 2069  tip_threshold: i
-00001010: 6e74 203d 2032 3736 2c0d 0a20 2020 2020  nt = 276,..     
-00001020: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
-00001030: 2029 3a0d 0a20 2020 2020 2020 2022 2222   ):..        """
-00001040: 0d0a 2020 2020 2020 2020 496e 7374 616e  ..        Instan
-00001050: 7469 6174 6520 7468 6520 636c 6173 730d  tiate the class.
-00001060: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00001070: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-00001080: 7274 2028 7374 7229 3a20 434f 4d20 706f  rt (str): COM po
-00001090: 7274 2061 6464 7265 7373 0d0a 2020 2020  rt address..    
-000010a0: 2020 2020 2020 2020 6368 616e 6e65 6c20          channel 
-000010b0: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
-000010c0: 2063 6861 6e6e 656c 2069 642e 2044 6566   channel id. Def
-000010d0: 6175 6c74 7320 746f 2031 2e0d 0a20 2020  aults to 1...   
-000010e0: 2020 2020 2020 2020 206f 6666 7365 7420           offset 
-000010f0: 2874 7570 6c65 5b66 6c6f 6174 5d2c 206f  (tuple[float], o
-00001100: 7074 696f 6e61 6c29 3a20 782c 792c 7a20  ptional): x,y,z 
-00001110: 6f66 6673 6574 206f 6620 7469 702e 2044  offset of tip. D
-00001120: 6566 6175 6c74 7320 746f 2028 302c 302c  efaults to (0,0,
-00001130: 3029 2e0d 0a20 2020 2020 2020 2020 2020  0)...           
-00001140: 2072 6573 706f 6e73 655f 7469 6d65 2028   response_time (
-00001150: 666c 6f61 742c 206f 7074 696f 6e61 6c29  float, optional)
-00001160: 3a20 6465 6c61 7920 6265 7477 6565 6e20  : delay between 
-00001170: 7365 6e64 696e 6720 6120 636f 6d6d 616e  sending a comman
-00001180: 6420 616e 6420 7265 6365 6976 696e 6720  d and receiving 
-00001190: 6120 7265 7370 6f6e 7365 2c20 696e 2073  a response, in s
-000011a0: 6563 6f6e 6473 2e20 4465 6661 756c 7473  econds. Defaults
-000011b0: 2074 6f20 312e 3033 2e0d 0a20 2020 2020   to 1.03...     
-000011c0: 2020 2020 2020 2074 6970 5f74 6872 6573         tip_thres
-000011d0: 686f 6c64 2028 696e 742c 206f 7074 696f  hold (int, optio
-000011e0: 6e61 6c29 3a20 7468 7265 7368 6f6c 6420  nal): threshold 
-000011f0: 6162 6f76 6520 7768 6963 6820 6120 636f  above which a co
-00001200: 6e64 7563 7469 7665 2070 6970 6574 7465  nductive pipette
-00001210: 2074 6970 2069 7320 636f 6e73 6964 6572   tip is consider
-00001220: 6564 2074 6f20 6265 2061 7474 6163 6865  ed to be attache
-00001230: 642e 2044 6566 6175 6c74 7320 746f 2032  d. Defaults to 2
-00001240: 3736 2e0d 0a20 2020 2020 2020 2022 2222  76...        """
-00001250: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-00001260: 292e 5f5f 696e 6974 5f5f 282a 2a6b 7761  ).__init__(**kwa
-00001270: 7267 7329 0d0a 2020 2020 2020 2020 7365  rgs)..        se
-00001280: 6c66 2e63 6861 6e6e 656c 203d 2063 6861  lf.channel = cha
-00001290: 6e6e 656c 0d0a 2020 2020 2020 2020 7365  nnel..        se
-000012a0: 6c66 2e6f 6666 7365 7420 3d20 6f66 6673  lf.offset = offs
-000012b0: 6574 0d0a 2020 2020 2020 2020 7365 6c66  et..        self
-000012c0: 2e72 6573 706f 6e73 655f 7469 6d65 203d  .response_time =
-000012d0: 2072 6573 706f 6e73 655f 7469 6d65 0d0a   response_time..
-000012e0: 2020 2020 2020 2020 7365 6c66 2e74 6970          self.tip
-000012f0: 5f74 6872 6573 686f 6c64 203d 2074 6970  _threshold = tip
-00001300: 5f74 6872 6573 686f 6c64 0d0a 2020 2020  _threshold..    
-00001310: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
-00001320: 6c66 2e6d 6f64 656c 5f69 6e66 6f3a 204d  lf.model_info: M
-00001330: 6f64 656c 203d 204e 6f6e 650d 0a20 2020  odel = None..   
-00001340: 2020 2020 2073 656c 662e 6c69 6d69 7473       self.limits
-00001350: 203d 2028 302c 3029 0d0a 2020 2020 2020   = (0,0)..      
-00001360: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
-00001370: 3d20 300d 0a20 2020 2020 2020 2073 656c  = 0..        sel
-00001380: 662e 7370 6565 645f 636f 6465 203d 2053  f.speed_code = S
-00001390: 7065 6564 2833 2c33 290d 0a20 2020 2020  peed(3,3)..     
-000013a0: 2020 2073 656c 662e 7370 6565 645f 7072     self.speed_pr
-000013b0: 6573 6574 7320 3d20 4e6f 6e65 0d0a 2020  esets = None..  
-000013c0: 2020 2020 2020 7365 6c66 2e74 6970 5f6c        self.tip_l
-000013d0: 656e 6774 6820 3d20 300d 0a20 2020 2020  ength = 0..     
-000013e0: 2020 200d 0a20 2020 2020 2020 2073 656c     ..        sel
-000013f0: 662e 5f63 6170 6163 6974 616e 6365 203d  f._capacitance =
-00001400: 2030 0d0a 2020 2020 2020 2020 7365 6c66   0..        self
-00001410: 2e5f 7374 6174 7573 5f63 6f64 6520 3d20  ._status_code = 
-00001420: 2727 0d0a 2020 2020 2020 2020 7365 6c66  ''..        self
-00001430: 2e5f 7468 7265 6164 7320 3d20 7b7d 0d0a  ._threads = {}..
-00001440: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00001450: 2020 7072 696e 7428 2241 6e79 2061 7474    print("Any att
-00001460: 6163 6865 6420 7069 7065 7474 6520 7469  ached pipette ti
-00001470: 7020 6d61 7920 6472 6f70 2064 7572 696e  p may drop durin
-00001480: 6720 696e 6974 6961 6c69 7361 7469 6f6e  g initialisation
-00001490: 2e22 290d 0a20 2020 2020 2020 2073 656c  .")..        sel
-000014a0: 662e 5f63 6f6e 6e65 6374 2870 6f72 7429  f._connect(port)
-000014b0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000014c0: 0d0a 2020 2020 0d0a 2020 2020 2320 5072  ..    ..    # Pr
-000014d0: 6f70 6572 7469 6573 0d0a 2020 2020 4070  operties..    @p
-000014e0: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
-000014f0: 2063 6170 6163 6974 616e 6365 2873 656c   capacitance(sel
-00001500: 6629 202d 3e20 696e 743a 0d0a 2020 2020  f) -> int:..    
-00001510: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00001520: 5f63 6170 6163 6974 616e 6365 0d0a 2020  _capacitance..  
-00001530: 2020 2020 2020 0d0a 2020 2020 4070 726f        ..    @pro
-00001540: 7065 7274 790d 0a20 2020 2064 6566 2068  perty..    def h
-00001550: 6f6d 655f 706f 7369 7469 6f6e 2873 656c  ome_position(sel
-00001560: 6629 202d 3e20 696e 743a 0d0a 2020 2020  f) -> int:..    
-00001570: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00001580: 6d6f 6465 6c5f 696e 666f 2e68 6f6d 655f  model_info.home_
-00001590: 706f 7369 7469 6f6e 0d0a 2020 2020 0d0a  position..    ..
-000015a0: 2020 2020 4070 726f 7065 7274 790d 0a20      @property.. 
-000015b0: 2020 2064 6566 2070 6f72 7428 7365 6c66     def port(self
-000015c0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-000015d0: 2020 2072 6574 7572 6e20 7365 6c66 2e63     return self.c
-000015e0: 6f6e 6e65 6374 696f 6e5f 6465 7461 696c  onnection_detail
-000015f0: 732e 6765 7428 2770 6f72 7427 2c20 2727  s.get('port', ''
-00001600: 290d 0a20 2020 200d 0a20 2020 2040 7072  )..    ..    @pr
-00001610: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-00001620: 7265 736f 6c75 7469 6f6e 2873 656c 6629  resolution(self)
-00001630: 202d 3e20 666c 6f61 743a 0d0a 2020 2020   -> float:..    
-00001640: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00001650: 6d6f 6465 6c5f 696e 666f 2e72 6573 6f6c  model_info.resol
-00001660: 7574 696f 6e0d 0a20 2020 200d 0a20 2020  ution..    ..   
-00001670: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00001680: 6465 6620 7374 6174 7573 2873 656c 6629  def status(self)
-00001690: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
-000016a0: 2020 7265 7475 726e 2073 656c 662e 6765    return self.ge
-000016b0: 7453 7461 7475 7328 290d 0a20 2020 200d  tStatus()..    .
-000016c0: 0a20 2020 2064 6566 205f 5f63 7963 6c65  .    def __cycle
-000016d0: 735f 5f28 7365 6c66 2920 2d3e 2055 6e69  s__(self) -> Uni
-000016e0: 6f6e 5b69 6e74 2c20 7374 725d 3a0d 0a20  on[int, str]:.. 
-000016f0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00001700: 2020 2020 5265 7472 6965 7665 2074 6f74      Retrieve tot
-00001710: 616c 2063 7963 6c65 206c 6966 6574 696d  al cycle lifetim
-00001720: 650d 0a0d 0a20 2020 2020 2020 2052 6574  e....        Ret
-00001730: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-00001740: 2020 2055 6e69 6f6e 5b69 6e74 2c20 7374     Union[int, st
-00001750: 725d 3a20 6e75 6d62 6572 206f 6620 6c69  r]: number of li
-00001760: 6665 7469 6d65 2063 7963 6c65 732c 206f  fetime cycles, o
-00001770: 7220 7265 7370 6f6e 7365 2073 7472 696e  r response strin
-00001780: 670d 0a20 2020 2020 2020 2022 2222 0d0a  g..        """..
-00001790: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-000017a0: 203d 2073 656c 662e 5f71 7565 7279 2827   = self._query('
-000017b0: 4458 2729 0d0a 2020 2020 2020 2020 7472  DX')..        tr
-000017c0: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
-000017d0: 6379 636c 6573 203d 2069 6e74 2872 6573  cycles = int(res
-000017e0: 706f 6e73 6529 0d0a 2020 2020 2020 2020  ponse)..        
-000017f0: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-00001800: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00001810: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
-00001820: 0a20 2020 2020 2020 2070 7269 6e74 2866  .        print(f
-00001830: 2754 6f74 616c 2063 7963 6c65 733a 207b  'Total cycles: {
-00001840: 6379 636c 6573 7d27 290d 0a20 2020 2020  cycles}')..     
-00001850: 2020 2072 6574 7572 6e20 6379 636c 6573     return cycles
-00001860: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00001870: 5f5f 6d6f 6465 6c5f 5f28 7365 6c66 2920  __model__(self) 
-00001880: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
-00001890: 2022 2222 0d0a 2020 2020 2020 2020 5265   """..        Re
-000018a0: 7472 6965 7665 2074 6865 206d 6f64 656c  trieve the model
-000018b0: 206f 6620 7468 6520 6465 7669 6365 0d0a   of the device..
-000018c0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000018d0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000018e0: 7374 723a 206d 6f64 656c 206e 616d 650d  str: model name.
-000018f0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00001900: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00001910: 2073 656c 662e 5f71 7565 7279 2827 444d   self._query('DM
-00001920: 2729 0d0a 2020 2020 2020 2020 7072 696e  ')..        prin
-00001930: 7428 6627 4d6f 6465 6c3a 207b 7265 7370  t(f'Model: {resp
-00001940: 6f6e 7365 7d27 290d 0a20 2020 2020 2020  onse}')..       
-00001950: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00001960: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00001970: 5f5f 7265 736f 6c75 7469 6f6e 5f5f 2873  __resolution__(s
-00001980: 656c 6629 202d 3e20 556e 696f 6e5b 696e  elf) -> Union[in
-00001990: 742c 2073 7472 5d3a 0d0a 2020 2020 2020  t, str]:..      
-000019a0: 2020 2222 220d 0a20 2020 2020 2020 2052    """..        R
-000019b0: 6574 7269 6576 6520 7468 6520 7265 736f  etrieve the reso
-000019c0: 6c75 7469 6f6e 206f 6620 7468 6520 6465  lution of the de
-000019d0: 7669 6365 0d0a 0d0a 2020 2020 2020 2020  vice....        
-000019e0: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
-000019f0: 2020 2020 2020 556e 696f 6e5b 696e 742c        Union[int,
-00001a00: 2073 7472 5d3a 2076 6f6c 756d 6520 7265   str]: volume re
-00001a10: 736f 6c75 7469 6f6e 206f 6620 6465 7669  solution of devi
-00001a20: 6365 2069 6e20 6e4c 2c20 6f72 2072 6573  ce in nL, or res
-00001a30: 706f 6e73 6520 7374 7269 6e67 0d0a 2020  ponse string..  
-00001a40: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00001a50: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-00001a60: 6c66 2e5f 7175 6572 7928 2744 5227 290d  lf._query('DR').
-00001a70: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00001a80: 2020 2020 2020 2020 2020 2072 6573 6f6c             resol
-00001a90: 7574 696f 6e20 3d20 696e 7428 7265 7370  ution = int(resp
-00001aa0: 6f6e 7365 290d 0a20 2020 2020 2020 2065  onse)..        e
-00001ab0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-00001ac0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
-00001ad0: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00001ae0: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00001af0: 7b72 6573 6f6c 7574 696f 6e2f 3130 3030  {resolution/1000
-00001b00: 7d20 754c 202f 2073 7465 7027 290d 0a20  } uL / step').. 
-00001b10: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00001b20: 736f 6c75 7469 6f6e 0d0a 2020 2020 0d0a  solution..    ..
-00001b30: 2020 2020 6465 6620 5f5f 7665 7273 696f      def __versio
-00001b40: 6e5f 5f28 7365 6c66 2920 2d3e 2073 7472  n__(self) -> str
-00001b50: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00001b60: 2020 2020 2020 2020 5265 7472 6965 7665          Retrieve
-00001b70: 2074 6865 2073 6f66 7477 6172 6520 7665   the software ve
-00001b80: 7273 696f 6e20 6f6e 2074 6865 2064 6576  rsion on the dev
-00001b90: 6963 650d 0a0d 0a20 2020 2020 2020 2052  ice....        R
-00001ba0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00001bb0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-00001bc0: 2076 6572 7369 6f6e 0d0a 2020 2020 2020   version..      
-00001bd0: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
-00001be0: 6574 7572 6e20 7365 6c66 2e5f 7175 6572  eturn self._quer
-00001bf0: 7928 2744 5627 290d 0a0d 0a20 2020 2064  y('DV')....    d
-00001c00: 6566 2061 6464 4169 7247 6170 2873 656c  ef addAirGap(sel
-00001c10: 662c 2073 7465 7073 3a69 6e74 203d 2031  f, steps:int = 1
-00001c20: 3029 202d 3e20 7374 723a 0d0a 2020 2020  0) -> str:..    
-00001c30: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00001c40: 2043 7265 6174 6520 616e 2061 6972 2067   Create an air g
-00001c50: 6170 2062 6574 7765 656e 2074 776f 2076  ap between two v
-00001c60: 6f6c 756d 6573 206f 6620 6c69 7175 6964  olumes of liquid
-00001c70: 2069 6e20 7069 7065 7474 650d 0a20 2020   in pipette..   
-00001c80: 2020 2020 200d 0a20 2020 2020 2020 2041       ..        A
-00001c90: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-00001ca0: 2020 7374 6570 7320 2869 6e74 2c20 6f70    steps (int, op
-00001cb0: 7469 6f6e 616c 293a 206e 756d 6265 7220  tional): number 
-00001cc0: 6f66 2073 7465 7073 2066 6f72 2061 6972  of steps for air
-00001cd0: 2067 6170 2e20 4465 6661 756c 7473 2074   gap. Defaults t
-00001ce0: 6f20 4445 4641 554c 545f 4149 5247 4150  o DEFAULT_AIRGAP
-00001cf0: 2e0d 0a20 2020 2020 2020 2020 2020 2063  ...            c
-00001d00: 6861 6e6e 656c 2028 696e 742c 206f 7074  hannel (int, opt
-00001d10: 696f 6e61 6c29 3a20 6368 616e 6e65 6c20  ional): channel 
-00001d20: 746f 2061 6464 2061 6972 2067 6170 2e20  to add air gap. 
-00001d30: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-00001d40: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
-00001d50: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-00001d60: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
-00001d70: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
-00001d80: 2022 2222 0d0a 2020 2020 2020 2020 7265   """..        re
-00001d90: 7370 6f6e 7365 203d 2073 656c 662e 5f71  sponse = self._q
-00001da0: 7565 7279 2866 2752 497b 7374 6570 737d  uery(f'RI{steps}
-00001db0: 2729 0d0a 2020 2020 2020 2020 7469 6d65  ')..        time
-00001dc0: 2e73 6c65 6570 2831 290d 0a20 2020 2020  .sleep(1)..     
-00001dd0: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
-00001de0: 7365 0d0a 2020 2020 2020 2020 0d0a 2020  se..        ..  
-00001df0: 2020 6465 6620 6173 7069 7261 7465 2873    def aspirate(s
-00001e00: 656c 662c 200d 0a20 2020 2020 2020 2076  elf, ..        v
-00001e10: 6f6c 756d 653a 2066 6c6f 6174 2c20 0d0a  olume: float, ..
-00001e20: 2020 2020 2020 2020 7370 6565 643a 204f          speed: O
-00001e30: 7074 696f 6e61 6c5b 666c 6f61 745d 203d  ptional[float] =
-00001e40: 204e 6f6e 652c 200d 0a20 2020 2020 2020   None, ..       
-00001e50: 2077 6169 743a 2069 6e74 203d 2030 2c20   wait: int = 0, 
-00001e60: 0d0a 2020 2020 2020 2020 7061 7573 653a  ..        pause:
-00001e70: 2062 6f6f 6c20 3d20 4661 6c73 652c 200d   bool = False, .
-00001e80: 0a20 2020 2020 2020 2072 6561 6765 6e74  .        reagent
-00001e90: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00001ea0: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-00001eb0: 202a 2a6b 7761 7267 730d 0a20 2020 2029   **kwargs..    )
-00001ec0: 202d 3e20 7374 723a 0d0a 2020 2020 2020   -> str:..      
-00001ed0: 2020 2222 220d 0a20 2020 2020 2020 2041    """..        A
-00001ee0: 7370 6972 6174 6520 6465 7369 7265 6420  spirate desired 
-00001ef0: 766f 6c75 6d65 206f 6620 7265 6167 656e  volume of reagen
-00001f00: 740d 0a0d 0a20 2020 2020 2020 2041 7267  t....        Arg
-00001f10: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00001f20: 766f 6c75 6d65 2028 666c 6f61 7429 3a20  volume (float): 
-00001f30: 7461 7267 6574 2076 6f6c 756d 650d 0a20  target volume.. 
-00001f40: 2020 2020 2020 2020 2020 2073 7065 6564             speed
-00001f50: 2028 4f70 7469 6f6e 616c 5b66 6c6f 6174   (Optional[float
-00001f60: 5d2c 206f 7074 696f 6e61 6c29 3a20 7370  ], optional): sp
-00001f70: 6565 6420 746f 2061 7370 6972 6174 6520  eed to aspirate 
-00001f80: 6174 2e20 4465 6661 756c 7473 2074 6f20  at. Defaults to 
-00001f90: 4e6f 6e65 2e0d 0a20 2020 2020 2020 2020  None...         
-00001fa0: 2020 2077 6169 7420 2869 6e74 2c20 6f70     wait (int, op
-00001fb0: 7469 6f6e 616c 293a 2074 696d 6520 6465  tional): time de
-00001fc0: 6c61 7920 6166 7465 7220 6173 7069 7261  lay after aspira
-00001fd0: 7465 2e20 4465 6661 756c 7473 2074 6f20  te. Defaults to 
-00001fe0: 302e 0d0a 2020 2020 2020 2020 2020 2020  0...            
-00001ff0: 7061 7573 6520 2862 6f6f 6c2c 206f 7074  pause (bool, opt
-00002000: 696f 6e61 6c29 3a20 7768 6574 6865 7220  ional): whether 
-00002010: 746f 2070 6175 7365 2066 6f72 2075 7365  to pause for use
-00002020: 7220 696e 7465 7276 656e 7469 6f6e 2e20  r intervention. 
-00002030: 4465 6661 756c 7473 2074 6f20 4661 6c73  Defaults to Fals
-00002040: 652e 0d0a 2020 2020 2020 2020 2020 2020  e...            
-00002050: 7265 6167 656e 7420 284f 7074 696f 6e61  reagent (Optiona
-00002060: 6c5b 7374 725d 2c20 6f70 7469 6f6e 616c  l[str], optional
-00002070: 293a 206e 616d 6520 6f66 2072 6561 6765  ): name of reage
-00002080: 6e74 2e20 4465 6661 756c 7473 2074 6f20  nt. Defaults to 
-00002090: 4e6f 6e65 2e0d 0a20 2020 2020 2020 2020  None...         
-000020a0: 2020 200d 0a20 2020 2020 2020 2052 6574     ..        Ret
-000020b0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-000020c0: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
-000020d0: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
-000020e0: 2022 2222 200d 0a20 2020 2020 2020 2073   """ ..        s
-000020f0: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
-00002100: 655f 6665 6564 6261 636b 3d54 7275 652c  e_feedback=True,
-00002110: 206f 6363 7570 6965 643d 5472 7565 290d   occupied=True).
-00002120: 0a20 2020 2020 2020 2076 6f6c 756d 6520  .        volume 
-00002130: 3d20 6d69 6e28 766f 6c75 6d65 2c20 7365  = min(volume, se
-00002140: 6c66 2e63 6170 6163 6974 7920 2d20 7365  lf.capacity - se
-00002150: 6c66 2e76 6f6c 756d 6529 0d0a 2020 2020  lf.volume)..    
-00002160: 2020 2020 7374 6570 7320 3d20 696e 7428      steps = int(
-00002170: 766f 6c75 6d65 202f 2073 656c 662e 7265  volume / self.re
-00002180: 736f 6c75 7469 6f6e 290d 0a20 2020 2020  solution)..     
-00002190: 2020 2076 6f6c 756d 6520 3d20 7374 6570     volume = step
-000021a0: 7320 2a20 7365 6c66 2e72 6573 6f6c 7574  s * self.resolut
-000021b0: 696f 6e0d 0a20 2020 2020 2020 2069 6620  ion..        if 
-000021c0: 766f 6c75 6d65 203d 3d20 303a 0d0a 2020  volume == 0:..  
-000021d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000021e0: 2027 270d 0a20 2020 2020 2020 2070 7269   ''..        pri
-000021f0: 6e74 2866 2741 7370 6972 6174 696e 6720  nt(f'Aspirating 
-00002200: 7b76 6f6c 756d 657d 2075 4c2e 2e2e 2729  {volume} uL...')
-00002210: 0d0a 2020 2020 2020 2020 7374 6172 745f  ..        start_
-00002220: 6173 7069 7261 7465 203d 2074 696d 652e  aspirate = time.
-00002230: 7065 7266 5f63 6f75 6e74 6572 2829 0d0a  perf_counter()..
-00002240: 2020 2020 2020 2020 7370 6565 6420 3d20          speed = 
-00002250: 7365 6c66 2e73 7065 6564 2e75 7020 6966  self.speed.up if
-00002260: 2073 7065 6564 2069 7320 4e6f 6e65 2065   speed is None e
-00002270: 6c73 6520 7370 6565 640d 0a20 2020 2020  lse speed..     
-00002280: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-00002290: 7370 6565 6420 696e 2073 656c 662e 7370  speed in self.sp
-000022a0: 6565 645f 7072 6573 6574 733a 0d0a 2020  eed_presets:..  
-000022b0: 2020 2020 2020 2020 2020 6966 2073 7065            if spe
-000022c0: 6564 2021 3d20 7365 6c66 2e73 7065 6564  ed != self.speed
-000022d0: 2e75 703a 0d0a 2020 2020 2020 2020 2020  .up:..          
-000022e0: 2020 2020 2020 7365 6c66 2e73 6574 5370        self.setSp
-000022f0: 6565 6428 7370 6565 643d 7370 6565 642c  eed(speed=speed,
-00002300: 2075 703d 5472 7565 2c20 6465 6661 756c   up=True, defaul
-00002310: 743d 4661 6c73 6529 0d0a 2020 2020 2020  t=False)..      
-00002320: 2020 2020 2020 7374 6172 745f 6173 7069        start_aspi
-00002330: 7261 7465 203d 2074 696d 652e 7065 7266  rate = time.perf
-00002340: 5f63 6f75 6e74 6572 2829 0d0a 2020 2020  _counter()..    
-00002350: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00002360: 203d 2073 656c 662e 5f71 7565 7279 2866   = self._query(f
-00002370: 2752 497b 7374 6570 737d 2729 0d0a 2020  'RI{steps}')..  
-00002380: 2020 2020 2020 2020 2020 6d6f 7665 5f74            move_t
-00002390: 696d 6520 3d20 7374 6570 732a 7365 6c66  ime = steps*self
-000023a0: 2e72 6573 6f6c 7574 696f 6e20 2f20 7370  .resolution / sp
-000023b0: 6565 640d 0a20 2020 2020 2020 2020 2020  eed..           
-000023c0: 2064 7572 6174 696f 6e20 3d20 7469 6d65   duration = time
-000023d0: 2e70 6572 665f 636f 756e 7465 7228 2920  .perf_counter() 
-000023e0: 2d20 7374 6172 745f 6173 7069 7261 7465  - start_aspirate
-000023f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00002400: 2064 7572 6174 696f 6e20 3c20 286d 6f76   duration < (mov
-00002410: 655f 7469 6d65 293a 0d0a 2020 2020 2020  e_time):..      
-00002420: 2020 2020 2020 2020 2020 7469 6d65 2e73            time.s
-00002430: 6c65 6570 286d 6f76 655f 7469 6d65 2d64  leep(move_time-d
-00002440: 7572 6174 696f 6e29 0d0a 2020 2020 2020  uration)..      
-00002450: 2020 2020 2020 2320 6966 2072 6573 706f        # if respo
-00002460: 6e73 6520 213d 2027 6f6b 273a 0d0a 2020  nse != 'ok':..  
-00002470: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00002480: 7265 7475 726e 2072 6573 706f 6e73 650d  return response.
-00002490: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-000024a0: 2020 2020 2020 2065 6c69 6620 7370 6565         elif spee
-000024b0: 6420 6e6f 7420 696e 2073 656c 662e 7370  d not in self.sp
-000024c0: 6565 645f 7072 6573 6574 733a 0d0a 2020  eed_presets:..  
-000024d0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-000024e0: 6622 5461 7267 6574 3a20 7b76 6f6c 756d  f"Target: {volum
-000024f0: 657d 2075 4c20 6174 207b 7370 6565 647d  e} uL at {speed}
-00002500: 2075 4c2f 732e 2e2e 2229 0d0a 2020 2020   uL/s...")..    
-00002510: 2020 2020 2020 2020 7370 6565 645f 7061          speed_pa
-00002520: 7261 6d65 7465 7273 203d 2073 656c 662e  rameters = self.
-00002530: 5f63 616c 6375 6c61 7465 5f73 7065 6564  _calculate_speed
-00002540: 5f70 6172 616d 6574 6572 7328 766f 6c75  _parameters(volu
-00002550: 6d65 3d76 6f6c 756d 652c 2073 7065 6564  me=volume, speed
-00002560: 3d73 7065 6564 290d 0a20 2020 2020 2020  =speed)..       
-00002570: 2020 2020 2070 7269 6e74 2873 7065 6564       print(speed
-00002580: 5f70 6172 616d 6574 6572 7329 0d0a 2020  _parameters)..  
-00002590: 2020 2020 2020 2020 2020 7072 6573 6574            preset
-000025a0: 203d 2073 7065 6564 5f70 6172 616d 6574   = speed_paramet
-000025b0: 6572 732e 7072 6573 6574 0d0a 2020 2020  ers.preset..    
-000025c0: 2020 2020 2020 2020 6966 2070 7265 7365          if prese
-000025d0: 7420 6973 204e 6f6e 653a 0d0a 2020 2020  t is None:..    
-000025e0: 2020 2020 2020 2020 2020 2020 2320 7261              # ra
-000025f0: 6973 6520 5275 6e74 696d 6545 7272 6f72  ise RuntimeError
-00002600: 2827 5461 7267 6574 2073 7065 6564 206e  ('Target speed n
-00002610: 6f74 2070 6f73 7369 626c 652e 2729 0d0a  ot possible.')..
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 7072 696e 7428 2754 6172 6765 7420 7370  print('Target sp
-00002640: 6565 6420 6e6f 7420 706f 7373 6962 6c65  eed not possible
-00002650: 2e27 290d 0a20 2020 2020 2020 2020 2020  .')..           
-00002660: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-00002670: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-00002680: 7453 7065 6564 2873 7065 6564 3d70 7265  tSpeed(speed=pre
-00002690: 7365 742c 2075 703d 5472 7565 2c20 6465  set, up=True, de
-000026a0: 6661 756c 743d 4661 6c73 6529 0d0a 2020  fault=False)..  
-000026b0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-000026c0: 2020 2020 2020 2020 7374 6570 735f 6c65          steps_le
-000026d0: 6674 203d 2073 7465 7073 0d0a 2020 2020  ft = steps..    
-000026e0: 2020 2020 2020 2020 6465 6c61 7920 3d20          delay = 
-000026f0: 7370 6565 645f 7061 7261 6d65 7465 7273  speed_parameters
-00002700: 2e64 656c 6179 0d0a 2020 2020 2020 2020  .delay..        
-00002710: 2020 2020 7374 6570 5f73 697a 6520 3d20      step_size = 
-00002720: 7370 6565 645f 7061 7261 6d65 7465 7273  speed_parameters
-00002730: 2e73 7465 705f 7369 7a65 0d0a 2020 2020  .step_size..    
-00002740: 2020 2020 2020 2020 696e 7465 7276 616c          interval
-00002750: 7320 3d20 7370 6565 645f 7061 7261 6d65  s = speed_parame
-00002760: 7465 7273 2e69 6e74 6572 7661 6c73 0d0a  ters.intervals..
-00002770: 2020 2020 2020 2020 2020 2020 7374 6172              star
-00002780: 745f 6173 7069 7261 7465 203d 2074 696d  t_aspirate = tim
-00002790: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
-000027a0: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-000027b0: 7220 6920 696e 2072 616e 6765 2869 6e74  r i in range(int
-000027c0: 6572 7661 6c73 293a 0d0a 2020 2020 2020  ervals):..      
-000027d0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-000027e0: 7469 6d65 203d 2074 696d 652e 7065 7266  time = time.perf
-000027f0: 5f63 6f75 6e74 6572 2829 0d0a 2020 2020  _counter()..    
-00002800: 2020 2020 2020 2020 2020 2020 7374 6570              step
-00002810: 203d 2073 7465 705f 7369 7a65 2069 6620   = step_size if 
-00002820: 2869 2b31 2021 3d20 696e 7465 7276 616c  (i+1 != interval
-00002830: 7329 2065 6c73 6520 7374 6570 735f 6c65  s) else steps_le
-00002840: 6674 0d0a 2020 2020 2020 2020 2020 2020  ft..            
-00002850: 2020 2020 6d6f 7665 5f74 696d 6520 3d20      move_time = 
-00002860: 7374 6570 2a73 656c 662e 7265 736f 6c75  step*self.resolu
-00002870: 7469 6f6e 202f 2070 7265 7365 740d 0a20  tion / preset.. 
-00002880: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002890: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-000028a0: 7175 6572 7928 6627 5249 7b73 7465 707d  query(f'RI{step}
-000028b0: 272c 2072 6573 756d 655f 6665 6564 6261  ', resume_feedba
-000028c0: 636b 3d46 616c 7365 2c20 6765 745f 706f  ck=False, get_po
-000028d0: 7369 7469 6f6e 3d46 616c 7365 290d 0a20  sition=False).. 
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000028f0: 2069 6620 7265 7370 6f6e 7365 2021 3d20   if response != 
-00002900: 276f 6b27 3a0d 0a20 2020 2020 2020 2020  'ok':..         
-00002910: 2020 2020 2020 2023 2020 2020 2070 7269         #     pri
-00002920: 6e74 2822 4173 7069 7261 7469 6f6e 2066  nt("Aspiration f
-00002930: 6169 6c65 6422 290d 0a20 2020 2020 2020  ailed")..       
-00002940: 2020 2020 2020 2020 2023 2020 2020 2072           #     r
-00002950: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002970: 7374 6570 735f 6c65 6674 202d 3d20 7374  steps_left -= st
-00002980: 6570 0d0a 2020 2020 2020 2020 2020 2020  ep..            
-00002990: 2020 2020 6475 7261 7469 6f6e 203d 2074      duration = t
-000029a0: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
-000029b0: 2829 202d 2073 7461 7274 5f74 696d 650d  () - start_time.
-000029c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000029d0: 2069 6620 6475 7261 7469 6f6e 203c 2028   if duration < (
-000029e0: 6465 6c61 792b 6d6f 7665 5f74 696d 6529  delay+move_time)
-000029f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00002a00: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-00002a10: 7028 6465 6c61 792b 6d6f 7665 5f74 696d  p(delay+move_tim
-00002a20: 652d 6475 7261 7469 6f6e 290d 0a20 2020  e-duration)..   
-00002a30: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-00002a40: 2055 7064 6174 6520 7661 6c75 6573 0d0a   Update values..
-00002a50: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
-00002a60: 4173 7069 7261 7469 6f6e 2074 696d 653a  Aspiration time:
-00002a70: 207b 7469 6d65 2e70 6572 665f 636f 756e   {time.perf_coun
-00002a80: 7465 7228 292d 7374 6172 745f 6173 7069  ter()-start_aspi
-00002a90: 7261 7465 7d73 2729 0d0a 2020 2020 2020  rate}s')..      
-00002aa0: 2020 7469 6d65 2e73 6c65 6570 2877 6169    time.sleep(wai
-00002ab0: 7429 0d0a 2020 2020 2020 2020 7365 6c66  t)..        self
-00002ac0: 2e73 6574 466c 6167 286f 6363 7570 6965  .setFlag(occupie
-00002ad0: 643d 4661 6c73 652c 2070 6175 7365 5f66  d=False, pause_f
-00002ae0: 6565 6462 6163 6b3d 4661 6c73 6529 0d0a  eedback=False)..
-00002af0: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-00002b00: 506f 7369 7469 6f6e 2829 0d0a 2020 2020  Position()..    
-00002b10: 2020 2020 7365 6c66 2e76 6f6c 756d 6520      self.volume 
-00002b20: 2b3d 2076 6f6c 756d 650d 0a20 2020 2020  += volume..     
-00002b30: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
-00002b40: 202b 3d20 7374 6570 730d 0a20 2020 2020   += steps..     
-00002b50: 2020 2069 6620 7265 6167 656e 7420 6973     if reagent is
-00002b60: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
-00002b70: 2020 2020 2020 2020 7365 6c66 2e72 6561          self.rea
-00002b80: 6765 6e74 203d 2072 6561 6765 6e74 0d0a  gent = reagent..
-00002b90: 2020 2020 2020 2020 6966 2070 6175 7365          if pause
-00002ba0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00002bb0: 6e70 7574 2822 5072 6573 7320 2745 6e74  nput("Press 'Ent
-00002bc0: 6572 2720 746f 2070 726f 6365 6564 2e22  er' to proceed."
-00002bd0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00002be0: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
-00002bf0: 0d0a 2020 2020 6465 6620 626c 6f77 6f75  ..    def blowou
-00002c00: 7428 7365 6c66 2c20 686f 6d65 3a62 6f6f  t(self, home:boo
-00002c10: 6c20 3d20 5472 7565 2c20 2a2a 6b77 6172  l = True, **kwar
-00002c20: 6773 2920 2d3e 2073 7472 3a0d 0a20 2020  gs) -> str:..   
-00002c30: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00002c40: 2020 426c 6f77 6f75 7420 6c69 7175 6964    Blowout liquid
-00002c50: 2066 726f 6d20 7469 700d 0a0d 0a20 2020   from tip....   
-00002c60: 2020 2020 2041 7267 733a 0d0a 2020 2020       Args:..    
-00002c70: 2020 2020 2020 2020 686f 6d65 2028 626f          home (bo
-00002c80: 6f6c 2c20 6f70 7469 6f6e 616c 293a 2077  ol, optional): w
-00002c90: 6865 7468 6572 2074 6f20 7265 7475 726e  hether to return
-00002ca0: 2070 6c75 6e67 6572 2074 6f20 686f 6d65   plunger to home
-00002cb0: 2070 6f73 6974 696f 6e2e 2044 6566 6175   position. Defau
-00002cc0: 6c74 7320 746f 2054 7275 652e 0d0a 0d0a  lts to True.....
-00002cd0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00002ce0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00002cf0: 723a 2064 6576 6963 6520 7265 7370 6f6e  r: device respon
-00002d00: 7365 0d0a 2020 2020 2020 2020 2222 220d  se..        """.
-00002d10: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-00002d20: 203d 2066 2752 427b 7365 6c66 2e68 6f6d   = f'RB{self.hom
-00002d30: 655f 706f 7369 7469 6f6e 7d27 2069 6620  e_position}' if 
-00002d40: 686f 6d65 2065 6c73 6520 2752 4227 0d0a  home else 'RB'..
-00002d50: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00002d60: 203d 2073 656c 662e 5f71 7565 7279 2863   = self._query(c
-00002d70: 6f6d 6d61 6e64 290d 0a20 2020 2020 2020  ommand)..       
-00002d80: 2073 656c 662e 706f 7369 7469 6f6e 203d   self.position =
-00002d90: 2073 656c 662e 686f 6d65 5f70 6f73 6974   self.home_posit
-00002da0: 696f 6e0d 0a20 2020 2020 2020 2074 696d  ion..        tim
-00002db0: 652e 736c 6565 7028 3129 0d0a 2020 2020  e.sleep(1)..    
-00002dc0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00002dd0: 6e73 650d 0a20 2020 200d 0a20 2020 2064  nse..    ..    d
-00002de0: 6566 2064 6973 7065 6e73 6528 7365 6c66  ef dispense(self
-00002df0: 2c20 0d0a 2020 2020 2020 2020 766f 6c75  , ..        volu
-00002e00: 6d65 3a20 666c 6f61 742c 200d 0a20 2020  me: float, ..   
-00002e10: 2020 2020 2073 7065 6564 3a20 4f70 7469       speed: Opti
-00002e20: 6f6e 616c 5b66 6c6f 6174 5d20 3d20 4e6f  onal[float] = No
-00002e30: 6e65 2c20 0d0a 2020 2020 2020 2020 7761  ne, ..        wa
-00002e40: 6974 3a20 696e 7420 3d20 302c 200d 0a20  it: int = 0, .. 
-00002e50: 2020 2020 2020 2070 6175 7365 3a20 626f         pause: bo
-00002e60: 6f6c 203d 2046 616c 7365 2c20 0d0a 2020  ol = False, ..  
-00002e70: 2020 2020 2020 626c 6f77 6f75 743a 2062        blowout: b
-00002e80: 6f6f 6c20 3d20 4661 6c73 652c 0d0a 2020  ool = False,..  
-00002e90: 2020 2020 2020 626c 6f77 6f75 745f 686f        blowout_ho
-00002ea0: 6d65 3a20 626f 6f6c 203d 2054 7275 652c  me: bool = True,
-00002eb0: 0d0a 2020 2020 2020 2020 666f 7263 655f  ..        force_
-00002ec0: 6469 7370 656e 7365 3a20 626f 6f6c 203d  dispense: bool =
-00002ed0: 2046 616c 7365 2c20 0d0a 2020 2020 2020   False, ..      
-00002ee0: 2020 2a2a 6b77 6172 6773 0d0a 2020 2020    **kwargs..    
-00002ef0: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-00002f00: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00002f10: 4469 7370 656e 7365 2064 6573 6972 6564  Dispense desired
-00002f20: 2076 6f6c 756d 6520 6f66 2072 6561 6765   volume of reage
-00002f30: 6e74 0d0a 0d0a 2020 2020 2020 2020 4172  nt....        Ar
-00002f40: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
-00002f50: 2076 6f6c 756d 6520 2866 6c6f 6174 293a   volume (float):
-00002f60: 2074 6172 6765 7420 766f 6c75 6d65 0d0a   target volume..
-00002f70: 2020 2020 2020 2020 2020 2020 7370 6565              spee
-00002f80: 6420 284f 7074 696f 6e61 6c5b 666c 6f61  d (Optional[floa
-00002f90: 745d 2c20 6f70 7469 6f6e 616c 293a 2073  t], optional): s
-00002fa0: 7065 6564 2074 6f20 6469 7370 656e 7365  peed to dispense
-00002fb0: 2061 742e 2044 6566 6175 6c74 7320 746f   at. Defaults to
-00002fc0: 204e 6f6e 652e 0d0a 2020 2020 2020 2020   None...        
-00002fd0: 2020 2020 7761 6974 2028 696e 742c 206f      wait (int, o
-00002fe0: 7074 696f 6e61 6c29 3a20 7469 6d65 2064  ptional): time d
-00002ff0: 656c 6179 2061 6674 6572 2064 6973 7065  elay after dispe
-00003000: 6e73 652e 2044 6566 6175 6c74 7320 746f  nse. Defaults to
-00003010: 2030 2e0d 0a20 2020 2020 2020 2020 2020   0...           
-00003020: 2070 6175 7365 2028 626f 6f6c 2c20 6f70   pause (bool, op
-00003030: 7469 6f6e 616c 293a 2077 6865 7468 6572  tional): whether
-00003040: 2074 6f20 7061 7573 6520 666f 7220 7573   to pause for us
-00003050: 6572 2069 6e74 6572 7665 6e74 696f 6e2e  er intervention.
-00003060: 2044 6566 6175 6c74 7320 746f 2046 616c   Defaults to Fal
-00003070: 7365 2e0d 0a20 2020 2020 2020 2020 2020  se...           
-00003080: 2062 6c6f 776f 7574 2028 626f 6f6c 2c20   blowout (bool, 
-00003090: 6f70 7469 6f6e 616c 293a 2077 6865 7468  optional): wheth
-000030a0: 6572 2070 6572 666f 726d 2062 6c6f 776f  er perform blowo
-000030b0: 7574 2e20 4465 6661 756c 7473 2074 6f20  ut. Defaults to 
-000030c0: 4661 6c73 652e 0d0a 2020 2020 2020 2020  False...        
-000030d0: 2020 2020 626c 6f77 6f75 745f 686f 6d65      blowout_home
-000030e0: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
-000030f0: 293a 2077 6865 7468 6572 2074 6f20 7265  ): whether to re
-00003100: 7475 726e 2074 6865 2070 6c75 6e67 6572  turn the plunger
-00003110: 2068 6f6d 6520 6166 7465 7220 626c 6f77   home after blow
-00003120: 6f75 742e 2044 6566 6175 6c74 7320 746f  out. Defaults to
-00003130: 2054 7275 652e 0d0a 2020 2020 2020 2020   True...        
-00003140: 2020 2020 666f 7263 655f 6469 7370 656e      force_dispen
-00003150: 7365 2028 626f 6f6c 2c20 6f70 7469 6f6e  se (bool, option
-00003160: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
-00003170: 6469 7370 656e 7365 2072 6561 6765 6e74  dispense reagent
-00003180: 2072 6567 6172 646c 6573 732e 2044 6566   regardless. Def
-00003190: 6175 6c74 7320 746f 2046 616c 7365 2e0d  aults to False..
-000031a0: 0a0d 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-000031b0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-000031c0: 5661 6c75 6545 7272 6f72 3a20 5265 7175  ValueError: Requ
-000031d0: 6972 6564 2064 6973 7065 6e73 6520 766f  ired dispense vo
-000031e0: 6c75 6d65 2069 7320 6772 6561 7465 7220  lume is greater 
-000031f0: 7468 616e 2076 6f6c 756d 6520 696e 2074  than volume in t
-00003200: 6970 0d0a 0d0a 2020 2020 2020 2020 5265  ip....        Re
-00003210: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-00003220: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
-00003230: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
-00003240: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
-00003250: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
-00003260: 655f 6665 6564 6261 636b 3d54 7275 652c  e_feedback=True,
-00003270: 206f 6363 7570 6965 643d 5472 7565 290d   occupied=True).
-00003280: 0a20 2020 2020 2020 2069 6620 666f 7263  .        if forc
-00003290: 655f 6469 7370 656e 7365 3a0d 0a20 2020  e_dispense:..   
-000032a0: 2020 2020 2020 2020 2076 6f6c 756d 6520           volume 
-000032b0: 3d20 6d69 6e28 766f 6c75 6d65 2c20 7365  = min(volume, se
-000032c0: 6c66 2e76 6f6c 756d 6529 0d0a 2020 2020  lf.volume)..    
-000032d0: 2020 2020 656c 6966 2076 6f6c 756d 6520      elif volume 
-000032e0: 3e20 7365 6c66 2e76 6f6c 756d 653a 0d0a  > self.volume:..
-000032f0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00003300: 6520 5661 6c75 6545 7272 6f72 2827 5265  e ValueError('Re
-00003310: 7175 6972 6564 2064 6973 7065 6e73 6520  quired dispense 
-00003320: 766f 6c75 6d65 2069 7320 6772 6561 7465  volume is greate
-00003330: 7220 7468 616e 2076 6f6c 756d 6520 696e  r than volume in
-00003340: 2074 6970 2e27 290d 0a20 2020 2020 2020   tip.')..       
-00003350: 2073 7465 7073 203d 2069 6e74 2876 6f6c   steps = int(vol
-00003360: 756d 6520 2f20 7365 6c66 2e72 6573 6f6c  ume / self.resol
-00003370: 7574 696f 6e29 0d0a 2020 2020 2020 2020  ution)..        
-00003380: 766f 6c75 6d65 203d 2073 7465 7073 202a  volume = steps *
-00003390: 2073 656c 662e 7265 736f 6c75 7469 6f6e   self.resolution
-000033a0: 0d0a 2020 2020 2020 2020 6966 2076 6f6c  ..        if vol
-000033b0: 756d 6520 3d3d 2030 3a0d 0a20 2020 2020  ume == 0:..     
-000033c0: 2020 2020 2020 2072 6574 7572 6e20 2727         return ''
-000033d0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-000033e0: 6627 4469 7370 656e 7369 6e67 207b 766f  f'Dispensing {vo
-000033f0: 6c75 6d65 7d20 754c 2e2e 2e27 290d 0a20  lume} uL...').. 
-00003400: 2020 2020 2020 2073 7461 7274 5f64 6973         start_dis
-00003410: 7065 6e73 6520 3d20 7469 6d65 2e70 6572  pense = time.per
-00003420: 665f 636f 756e 7465 7228 290d 0a20 2020  f_counter()..   
-00003430: 2020 2020 2073 7065 6564 203d 2073 656c       speed = sel
-00003440: 662e 7370 6565 642e 646f 776e 2069 6620  f.speed.down if 
-00003450: 7370 6565 6420 6973 204e 6f6e 6520 656c  speed is None el
-00003460: 7365 2073 7065 6564 0d0a 0d0a 2020 2020  se speed....    
-00003470: 2020 2020 6966 2073 7065 6564 2069 6e20      if speed in 
-00003480: 7365 6c66 2e73 7065 6564 5f70 7265 7365  self.speed_prese
-00003490: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
-000034a0: 2069 6620 7370 6565 6420 213d 2073 656c   if speed != sel
-000034b0: 662e 7370 6565 642e 646f 776e 3a0d 0a20  f.speed.down:.. 
-000034c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000034d0: 656c 662e 7365 7453 7065 6564 2873 7065  elf.setSpeed(spe
-000034e0: 6564 3d73 7065 6564 2c20 7570 3d46 616c  ed=speed, up=Fal
-000034f0: 7365 2c20 6465 6661 756c 743d 4661 6c73  se, default=Fals
-00003500: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
-00003510: 7374 6172 745f 6469 7370 656e 7365 203d  start_dispense =
-00003520: 2074 696d 652e 7065 7266 5f63 6f75 6e74   time.perf_count
-00003530: 6572 2829 0d0a 2020 2020 2020 2020 2020  er()..          
-00003540: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-00003550: 662e 5f71 7565 7279 2866 2752 4f7b 7374  f._query(f'RO{st
-00003560: 6570 737d 2729 0d0a 2020 2020 2020 2020  eps}')..        
-00003570: 2020 2020 6d6f 7665 5f74 696d 6520 3d20      move_time = 
-00003580: 7374 6570 732a 7365 6c66 2e72 6573 6f6c  steps*self.resol
-00003590: 7574 696f 6e20 2f20 7370 6565 640d 0a20  ution / speed.. 
-000035a0: 2020 2020 2020 2020 2020 2064 7572 6174             durat
-000035b0: 696f 6e20 3d20 7469 6d65 2e70 6572 665f  ion = time.perf_
-000035c0: 636f 756e 7465 7228 2920 2d20 7374 6172  counter() - star
-000035d0: 745f 6469 7370 656e 7365 0d0a 2020 2020  t_dispense..    
-000035e0: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
-000035f0: 696f 6e20 3c20 286d 6f76 655f 7469 6d65  ion < (move_time
-00003600: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00003610: 2020 2020 7469 6d65 2e73 6c65 6570 286d      time.sleep(m
-00003620: 6f76 655f 7469 6d65 2d64 7572 6174 696f  ove_time-duratio
-00003630: 6e29 0d0a 2020 2020 2020 2020 2020 2020  n)..            
-00003640: 2320 6966 2072 6573 706f 6e73 6520 213d  # if response !=
-00003650: 2027 6f6b 273a 0d0a 2020 2020 2020 2020   'ok':..        
-00003660: 2020 2020 2320 2020 2020 7265 7475 726e      #     return
-00003670: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-00003680: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00003690: 2065 6c69 6620 7370 6565 6420 6e6f 7420   elif speed not 
-000036a0: 696e 2073 656c 662e 7370 6565 645f 7072  in self.speed_pr
-000036b0: 6573 6574 733a 0d0a 2020 2020 2020 2020  esets:..        
-000036c0: 2020 2020 7072 696e 7428 6622 5461 7267      print(f"Targ
-000036d0: 6574 3a20 7b76 6f6c 756d 657d 2075 4c20  et: {volume} uL 
-000036e0: 6174 207b 7370 6565 647d 2075 4c2f 732e  at {speed} uL/s.
-000036f0: 2e2e 2229 0d0a 2020 2020 2020 2020 2020  ..")..          
-00003700: 2020 7370 6565 645f 7061 7261 6d65 7465    speed_paramete
-00003710: 7273 203d 2073 656c 662e 5f63 616c 6375  rs = self._calcu
-00003720: 6c61 7465 5f73 7065 6564 5f70 6172 616d  late_speed_param
-00003730: 6574 6572 7328 766f 6c75 6d65 3d76 6f6c  eters(volume=vol
-00003740: 756d 652c 2073 7065 6564 3d73 7065 6564  ume, speed=speed
-00003750: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00003760: 7269 6e74 2873 7065 6564 5f70 6172 616d  rint(speed_param
-00003770: 6574 6572 7329 0d0a 2020 2020 2020 2020  eters)..        
-00003780: 2020 2020 7072 6573 6574 203d 2073 7065      preset = spe
-00003790: 6564 5f70 6172 616d 6574 6572 732e 7072  ed_parameters.pr
-000037a0: 6573 6574 0d0a 2020 2020 2020 2020 2020  eset..          
-000037b0: 2020 6966 2070 7265 7365 7420 6973 204e    if preset is N
-000037c0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000037d0: 2020 2020 2020 2320 7261 6973 6520 5275        # raise Ru
-000037e0: 6e74 696d 6545 7272 6f72 2827 5461 7267  ntimeError('Targ
-000037f0: 6574 2073 7065 6564 206e 6f74 2070 6f73  et speed not pos
-00003800: 7369 626c 652e 2729 0d0a 2020 2020 2020  sible.')..      
-00003810: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00003820: 2754 6172 6765 7420 7370 6565 6420 6e6f  'Target speed no
-00003830: 7420 706f 7373 6962 6c65 2e27 290d 0a20  t possible.').. 
-00003840: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003850: 6574 7572 6e0d 0a20 2020 2020 2020 2020  eturn..         
-00003860: 2020 2073 656c 662e 7365 7453 7065 6564     self.setSpeed
-00003870: 2873 7065 6564 3d70 7265 7365 742c 2075  (speed=preset, u
-00003880: 703d 4661 6c73 652c 2064 6566 6175 6c74  p=False, default
-00003890: 3d46 616c 7365 290d 0a20 2020 2020 2020  =False)..       
-000038a0: 200d 0a20 2020 2020 2020 2020 2020 2073   ..            s
-000038b0: 7465 7073 5f6c 6566 7420 3d20 7374 6570  teps_left = step
-000038c0: 730d 0a20 2020 2020 2020 2020 2020 2064  s..            d
-000038d0: 656c 6179 203d 2073 7065 6564 5f70 6172  elay = speed_par
-000038e0: 616d 6574 6572 732e 6465 6c61 790d 0a20  ameters.delay.. 
-000038f0: 2020 2020 2020 2020 2020 2073 7465 705f             step_
-00003900: 7369 7a65 203d 2073 7065 6564 5f70 6172  size = speed_par
-00003910: 616d 6574 6572 732e 7374 6570 5f73 697a  ameters.step_siz
-00003920: 650d 0a20 2020 2020 2020 2020 2020 2069  e..            i
-00003930: 6e74 6572 7661 6c73 203d 2073 7065 6564  ntervals = speed
-00003940: 5f70 6172 616d 6574 6572 732e 696e 7465  _parameters.inte
-00003950: 7276 616c 730d 0a20 2020 2020 2020 2020  rvals..         
-00003960: 2020 2073 7461 7274 5f64 6973 7065 6e73     start_dispens
-00003970: 6520 3d20 7469 6d65 2e70 6572 665f 636f  e = time.perf_co
-00003980: 756e 7465 7228 290d 0a20 2020 2020 2020  unter()..       
-00003990: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-000039a0: 6e67 6528 696e 7465 7276 616c 7329 3a0d  nge(intervals):.
-000039b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000039c0: 2073 7461 7274 5f74 696d 6520 3d20 7469   start_time = ti
-000039d0: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
-000039e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-000039f0: 2020 2073 7465 7020 3d20 7374 6570 5f73     step = step_s
-00003a00: 697a 6520 6966 2028 692b 3120 213d 2069  ize if (i+1 != i
-00003a10: 6e74 6572 7661 6c73 2920 656c 7365 2073  ntervals) else s
-00003a20: 7465 7073 5f6c 6566 740d 0a20 2020 2020  teps_left..     
-00003a30: 2020 2020 2020 2020 2020 206d 6f76 655f             move_
-00003a40: 7469 6d65 203d 2073 7465 702a 7365 6c66  time = step*self
-00003a50: 2e72 6573 6f6c 7574 696f 6e20 2f20 7072  .resolution / pr
-00003a60: 6573 6574 0d0a 2020 2020 2020 2020 2020  eset..          
-00003a70: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00003a80: 2073 656c 662e 5f71 7565 7279 2866 2752   self._query(f'R
-00003a90: 4f7b 7374 6570 7d27 2c20 7265 7375 6d65  O{step}', resume
-00003aa0: 5f66 6565 6462 6163 6b3d 4661 6c73 652c  _feedback=False,
-00003ab0: 2067 6574 5f70 6f73 6974 696f 6e3d 4661   get_position=Fa
-00003ac0: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
-00003ad0: 2020 2020 2020 2320 6966 2072 6573 706f        # if respo
-00003ae0: 6e73 6520 213d 2027 6f6b 273a 0d0a 2020  nse != 'ok':..  
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00003b00: 2020 2020 7072 696e 7428 2244 6973 7065      print("Dispe
-00003b10: 6e73 6520 6661 696c 6564 2229 0d0a 2020  nse failed")..  
-00003b20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00003b30: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
-00003b40: 6e73 650d 0a20 2020 2020 2020 2020 2020  nse..           
-00003b50: 2020 2020 2073 7465 7073 5f6c 6566 7420       steps_left 
-00003b60: 2d3d 2073 7465 700d 0a20 2020 2020 2020  -= step..       
-00003b70: 2020 2020 2020 2020 2064 7572 6174 696f           duratio
-00003b80: 6e20 3d20 7469 6d65 2e70 6572 665f 636f  n = time.perf_co
-00003b90: 756e 7465 7228 2920 2d20 7374 6172 745f  unter() - start_
-00003ba0: 7469 6d65 0d0a 2020 2020 2020 2020 2020  time..          
-00003bb0: 2020 2020 2020 6966 2064 7572 6174 696f        if duratio
-00003bc0: 6e20 3c20 2864 656c 6179 2b6d 6f76 655f  n < (delay+move_
-00003bd0: 7469 6d65 293a 0d0a 2020 2020 2020 2020  time):..        
-00003be0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00003bf0: 2e73 6c65 6570 2864 656c 6179 2b6d 6f76  .sleep(delay+mov
-00003c00: 655f 7469 6d65 2d64 7572 6174 696f 6e29  e_time-duration)
-00003c10: 0d0a 0d0a 2020 2020 2020 2020 2320 5570  ....        # Up
-00003c20: 6461 7465 2076 616c 7565 730d 0a20 2020  date values..   
-00003c30: 2020 2020 2070 7269 6e74 2866 2744 6973       print(f'Dis
-00003c40: 7065 6e73 6520 7469 6d65 3a20 7b74 696d  pense time: {tim
-00003c50: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
-00003c60: 2d73 7461 7274 5f64 6973 7065 6e73 657d  -start_dispense}
-00003c70: 7327 290d 0a20 2020 2020 2020 2074 696d  s')..        tim
-00003c80: 652e 736c 6565 7028 7761 6974 290d 0a20  e.sleep(wait).. 
-00003c90: 2020 2020 2020 2073 656c 662e 7365 7446         self.setF
-00003ca0: 6c61 6728 6f63 6375 7069 6564 3d46 616c  lag(occupied=Fal
-00003cb0: 7365 2c20 7061 7573 655f 6665 6564 6261  se, pause_feedba
-00003cc0: 636b 3d46 616c 7365 290d 0a20 2020 2020  ck=False)..     
-00003cd0: 2020 2073 656c 662e 6765 7450 6f73 6974     self.getPosit
-00003ce0: 696f 6e28 290d 0a20 2020 2020 2020 2073  ion()..        s
-00003cf0: 656c 662e 766f 6c75 6d65 203d 206d 6178  elf.volume = max
-00003d00: 2873 656c 662e 766f 6c75 6d65 202d 2076  (self.volume - v
-00003d10: 6f6c 756d 652c 2030 290d 0a20 2020 2020  olume, 0)..     
-00003d20: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
-00003d30: 202d 3d20 7374 6570 730d 0a20 2020 2020   -= steps..     
-00003d40: 2020 2069 6620 7365 6c66 2e76 6f6c 756d     if self.volum
-00003d50: 6520 3d3d 2030 2061 6e64 2062 6c6f 776f  e == 0 and blowo
-00003d60: 7574 3a0d 0a20 2020 2020 2020 2020 2020  ut:..           
-00003d70: 2073 656c 662e 626c 6f77 6f75 7428 686f   self.blowout(ho
-00003d80: 6d65 3d62 6c6f 776f 7574 5f68 6f6d 6529  me=blowout_home)
-00003d90: 0d0a 2020 2020 2020 2020 6966 2070 6175  ..        if pau
-00003da0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00003db0: 2069 6e70 7574 2822 5072 6573 7320 2745   input("Press 'E
-00003dc0: 6e74 6572 2720 746f 2070 726f 6365 6564  nter' to proceed
-00003dd0: 2e22 290d 0a20 2020 2020 2020 2072 6574  .")..        ret
-00003de0: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
-00003df0: 2020 0d0a 2020 2020 6465 6620 656a 6563    ..    def ejec
-00003e00: 7428 7365 6c66 2c20 686f 6d65 3a62 6f6f  t(self, home:boo
-00003e10: 6c20 3d20 5472 7565 2920 2d3e 2073 7472  l = True) -> str
-00003e20: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
-00003e30: 2020 2020 2020 2020 456a 6563 7420 7468          Eject th
-00003e40: 6520 7069 7065 7474 6520 7469 700d 0a0d  e pipette tip...
-00003e50: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-00003e60: 2020 2020 2020 2020 2020 2020 686f 6d65              home
-00003e70: 2028 626f 6f6c 2c20 6f70 7469 6f6e 616c   (bool, optional
-00003e80: 293a 2077 6865 7468 6572 2074 6f20 7265  ): whether to re
-00003e90: 7475 726e 2070 6c75 6e67 6572 2074 6f20  turn plunger to 
-00003ea0: 686f 6d65 2070 6f73 6974 696f 6e2e 2044  home position. D
-00003eb0: 6566 6175 6c74 7320 746f 2054 7275 652e  efaults to True.
-00003ec0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-00003ed0: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
-00003ee0: 2020 7374 723a 2064 6576 6963 6520 7265    str: device re
-00003ef0: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
-00003f00: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-00003f10: 662e 7265 6167 656e 7420 3d20 2727 0d0a  f.reagent = ''..
-00003f20: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
-00003f30: 3d20 6627 5245 7b73 656c 662e 686f 6d65  = f'RE{self.home
-00003f40: 5f70 6f73 6974 696f 6e7d 2720 6966 2068  _position}' if h
-00003f50: 6f6d 6520 656c 7365 2027 5245 270d 0a20  ome else 'RE'.. 
-00003f60: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00003f70: 3d20 7365 6c66 2e5f 7175 6572 7928 636f  = self._query(co
-00003f80: 6d6d 616e 6429 0d0a 2020 2020 2020 2020  mmand)..        
-00003f90: 7365 6c66 2e70 6f73 6974 696f 6e20 3d20  self.position = 
-00003fa0: 7365 6c66 2e68 6f6d 655f 706f 7369 7469  self.home_positi
-00003fb0: 6f6e 2069 6620 686f 6d65 2065 6c73 6520  on if home else 
-00003fc0: 300d 0a20 2020 2020 2020 2074 696d 652e  0..        time.
-00003fd0: 736c 6565 7028 3129 0d0a 2020 2020 2020  sleep(1)..      
-00003fe0: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-00003ff0: 650d 0a20 2020 200d 0a20 2020 2064 6566  e..    ..    def
-00004000: 2067 6574 4361 7061 6369 7461 6e63 6528   getCapacitance(
-00004010: 7365 6c66 2920 2d3e 2055 6e69 6f6e 5b69  self) -> Union[i
-00004020: 6e74 2c20 7374 725d 3a0d 0a20 2020 2020  nt, str]:..     
-00004030: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00004040: 4765 7420 7468 6520 6361 7061 6369 7461  Get the capacita
-00004050: 6e63 6520 6173 206d 6561 7375 7265 6420  nce as measured 
-00004060: 6174 2074 6865 2065 6e64 206f 6620 7468  at the end of th
-00004070: 6520 7069 7065 7474 650d 0a20 2020 2020  e pipette..     
-00004080: 2020 200d 0a20 2020 2020 2020 2052 6574     ..        Ret
-00004090: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-000040a0: 2020 2055 6e69 6f6e 5b69 6e74 2c20 7374     Union[int, st
-000040b0: 725d 3a20 6361 7061 6369 7461 6e63 6520  r]: capacitance 
-000040c0: 7661 6c75 652c 206f 7220 6465 7669 6365  value, or device
-000040d0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-000040e0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000040f0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-00004100: 5f71 7565 7279 2827 444e 2729 0d0a 2020  _query('DN')..  
-00004110: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-00004120: 2020 2020 2020 2020 6361 7061 6369 7461          capacita
-00004130: 6e63 6520 3d20 696e 7428 7265 7370 6f6e  nce = int(respon
-00004140: 7365 290d 0a20 2020 2020 2020 2065 7863  se)..        exc
-00004150: 6570 7420 5661 6c75 6545 7272 6f72 3a0d  ept ValueError:.
-00004160: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00004170: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
-00004180: 2020 2020 2020 7365 6c66 2e5f 6361 7061        self._capa
-00004190: 6369 7461 6e63 6520 3d20 6361 7061 6369  citance = capaci
-000041a0: 7461 6e63 650d 0a20 2020 2020 2020 2072  tance..        r
-000041b0: 6574 7572 6e20 6361 7061 6369 7461 6e63  eturn capacitanc
-000041c0: 650d 0a20 0d0a 2020 2020 6465 6620 6765  e.. ..    def ge
-000041d0: 7445 7272 6f72 7328 7365 6c66 2920 2d3e  tErrors(self) ->
-000041e0: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
-000041f0: 2222 0d0a 2020 2020 2020 2020 4765 7420  ""..        Get 
-00004200: 6572 726f 7273 2066 726f 6d20 7468 6520  errors from the 
-00004210: 6465 7669 6365 0d0a 0d0a 2020 2020 2020  device....      
-00004220: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00004230: 2020 2020 2020 2020 7374 723a 2064 6576          str: dev
-00004240: 6963 6520 7265 7370 6f6e 7365 0d0a 2020  ice response..  
-00004250: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00004260: 2020 2072 6574 7572 6e20 7365 6c66 2e5f     return self._
-00004270: 7175 6572 7928 2744 4527 290d 0a20 2020  query('DE')..   
-00004280: 200d 0a20 2020 2064 6566 2067 6574 496e   ..    def getIn
-00004290: 666f 2873 656c 662c 206d 6f64 656c 3a20  fo(self, model: 
-000042a0: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-000042b0: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
-000042c0: 2222 2247 6574 2064 6574 6169 6c73 206f  """Get details o
-000042d0: 6620 7468 6520 5361 7274 6f72 6975 7320  f the Sartorius 
-000042e0: 7069 7065 7474 6520 6d6f 6465 6c22 2222  pipette model"""
-000042f0: 0d0a 2020 2020 2020 2020 6d6f 6465 6c20  ..        model 
-00004300: 3d20 7365 6c66 2e5f 5f6d 6f64 656c 5f5f  = self.__model__
-00004310: 2829 2e73 706c 6974 2827 2d27 295b 305d  ().split('-')[0]
-00004320: 2069 6620 6d6f 6465 6c20 6973 204e 6f6e   if model is Non
-00004330: 6520 656c 7365 206d 6f64 656c 0d0a 2020  e else model..  
-00004340: 2020 2020 2020 6966 206d 6f64 656c 206e        if model n
-00004350: 6f74 2069 6e20 4d6f 6465 6c49 6e66 6f2e  ot in ModelInfo.
-00004360: 5f6d 656d 6265 725f 6e61 6d65 735f 3a0d  _member_names_:.
-00004370: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00004380: 6e74 2866 2752 6563 6569 7665 643a 207b  nt(f'Received: {
-00004390: 6d6f 6465 6c7d 2729 0d0a 2020 2020 2020  model}')..      
-000043a0: 2020 2020 2020 6d6f 6465 6c20 3d20 2742        model = 'B
-000043b0: 524c 3027 0d0a 2020 2020 2020 2020 2020  RL0'..          
-000043c0: 2020 7072 696e 7428 6622 4465 6661 756c    print(f"Defaul
-000043d0: 7469 6e67 2074 6f3a 207b 2742 524c 3027  ting to: {'BRL0'
-000043e0: 7d22 290d 0a20 2020 2020 2020 2020 2020  }")..           
-000043f0: 2070 7269 6e74 2866 2256 616c 6964 206d   print(f"Valid m
-00004400: 6f64 656c 7320 6172 653a 207b 272c 2027  odels are: {', '
-00004410: 2e6a 6f69 6e28 4d6f 6465 6c49 6e66 6f2e  .join(ModelInfo.
-00004420: 5f6d 656d 6265 725f 6e61 6d65 735f 297d  _member_names_)}
-00004430: 2229 0d0a 2020 2020 2020 2020 696e 666f  ")..        info
-00004440: 3a20 4d6f 6465 6c20 3d20 4d6f 6465 6c49  : Model = ModelI
-00004450: 6e66 6f5b 6d6f 6465 6c5d 2e76 616c 7565  nfo[model].value
-00004460: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00004470: 696e 666f 290d 0a20 2020 2020 2020 2073  info)..        s
-00004480: 656c 662e 6d6f 6465 6c5f 696e 666f 203d  elf.model_info =
-00004490: 2069 6e66 6f0d 0a20 2020 2020 2020 2073   info..        s
-000044a0: 656c 662e 6361 7061 6369 7479 203d 2069  elf.capacity = i
-000044b0: 6e66 6f2e 6361 7061 6369 7479 0d0a 2020  nfo.capacity..  
-000044c0: 2020 2020 2020 7365 6c66 2e6c 696d 6974        self.limit
-000044d0: 7320 3d20 2869 6e66 6f2e 7469 705f 656a  s = (info.tip_ej
-000044e0: 6563 745f 706f 7369 7469 6f6e 2c20 696e  ect_position, in
-000044f0: 666f 2e6d 6178 5f70 6f73 6974 696f 6e29  fo.max_position)
-00004500: 0d0a 2020 2020 2020 2020 7365 6c66 2e73  ..        self.s
-00004510: 7065 6564 5f70 7265 7365 7473 203d 2069  peed_presets = i
-00004520: 6e66 6f2e 7072 6573 6574 5f73 7065 6564  nfo.preset_speed
-00004530: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-00004540: 7370 6565 642e 7570 203d 2073 656c 662e  speed.up = self.
-00004550: 7370 6565 645f 7072 6573 6574 735b 7365  speed_presets[se
-00004560: 6c66 2e73 7065 6564 5f63 6f64 652e 7570  lf.speed_code.up
-00004570: 2d31 5d0d 0a20 2020 2020 2020 2073 656c  -1]..        sel
-00004580: 662e 7370 6565 642e 646f 776e 203d 2073  f.speed.down = s
-00004590: 656c 662e 7370 6565 645f 7072 6573 6574  elf.speed_preset
-000045a0: 735b 7365 6c66 2e73 7065 6564 5f63 6f64  s[self.speed_cod
-000045b0: 652e 646f 776e 2d31 5d0d 0a20 2020 2020  e.down-1]..     
-000045c0: 2020 2072 6574 7572 6e0d 0a20 2020 200d     return..    .
-000045d0: 0a20 2020 2064 6566 2067 6574 506f 7369  .    def getPosi
-000045e0: 7469 6f6e 2873 656c 662c 202a 2a6b 7761  tion(self, **kwa
-000045f0: 7267 7329 202d 3e20 696e 743a 0d0a 2020  rgs) -> int:..  
-00004600: 2020 2020 2020 2222 2247 6574 2074 6865        """Get the
-00004610: 2063 7572 7265 6e74 2070 6f73 6974 696f   current positio
-00004620: 6e20 6f66 2074 6865 2070 6970 6574 7465  n of the pipette
-00004630: 2222 220d 0a20 2020 2020 2020 2072 6573  """..        res
-00004640: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
-00004650: 6572 7928 2744 5027 290d 0a20 2020 2020  ery('DP')..     
-00004660: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00004670: 2020 2020 2070 6f73 6974 696f 6e20 3d20       position = 
-00004680: 696e 7428 7265 7370 6f6e 7365 290d 0a20  int(response).. 
-00004690: 2020 2020 2020 2065 7863 6570 7420 5661         except Va
-000046a0: 6c75 6545 7272 6f72 3a0d 0a20 2020 2020  lueError:..     
-000046b0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-000046c0: 7370 6f6e 7365 0d0a 2020 2020 2020 2020  sponse..        
-000046d0: 7365 6c66 2e70 6f73 6974 696f 6e20 3d20  self.position = 
-000046e0: 706f 7369 7469 6f6e 0d0a 2020 2020 2020  position..      
-000046f0: 2020 7265 7475 726e 2073 656c 662e 706f    return self.po
-00004700: 7369 7469 6f6e 0d0a 2020 2020 2020 0d0a  sition..      ..
-00004710: 2020 2020 6465 6620 6765 7453 7461 7475      def getStatu
-00004720: 7328 7365 6c66 2c20 2a2a 6b77 6172 6773  s(self, **kwargs
-00004730: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-00004740: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00004750: 4765 7420 7468 6520 7374 6174 7573 206f  Get the status o
-00004760: 6620 7468 6520 7069 7065 7474 650d 0a0d  f the pipette...
-00004770: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00004780: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00004790: 7472 3a20 6465 7669 6365 2072 6573 706f  tr: device respo
-000047a0: 6e73 650d 0a20 2020 2020 2020 2022 2222  nse..        """
-000047b0: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
-000047c0: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
-000047d0: 2827 4453 2729 0d0a 2020 2020 2020 2020  ('DS')..        
-000047e0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-000047f0: 2020 7374 6174 7573 203d 2069 6e74 2872    status = int(r
-00004800: 6573 706f 6e73 6529 0d0a 2020 2020 2020  esponse)..      
-00004810: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
-00004820: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
-00004830: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
-00004840: 650d 0a20 2020 2020 2020 2069 6620 7265  e..        if re
-00004850: 7370 6f6e 7365 206e 6f74 2069 6e20 5b5f  sponse not in [_
-00004860: 7374 6174 7573 2e76 616c 7565 2066 6f72  status.value for
-00004870: 205f 7374 6174 7573 2069 6e20 5374 6174   _status in Stat
-00004880: 7573 436f 6465 5d3a 0d0a 2020 2020 2020  usCode]:..      
-00004890: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-000048a0: 706f 6e73 650d 0a20 2020 2020 2020 200d  ponse..        .
-000048b0: 0a20 2020 2020 2020 2073 656c 662e 5f73  .        self._s
-000048c0: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-000048d0: 7475 730d 0a20 2020 2020 2020 2069 6620  tus..        if 
-000048e0: 7374 6174 7573 2069 6e20 5b34 2c36 2c38  status in [4,6,8
-000048f0: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
-00004900: 7365 6c66 2e73 6574 466c 6167 2862 7573  self.setFlag(bus
-00004910: 793d 5472 7565 290d 0a20 2020 2020 2020  y=True)..       
-00004920: 2020 2020 2069 6620 7365 6c66 2e76 6572       if self.ver
-00004930: 626f 7365 3a0d 0a20 2020 2020 2020 2020  bose:..         
-00004940: 2020 2020 2020 2070 7269 6e74 2853 7461         print(Sta
-00004950: 7475 7343 6f64 6528 7374 6174 7573 292e  tusCode(status).
-00004960: 6e61 6d65 290d 0a20 2020 2020 2020 2065  name)..        e
-00004970: 6c69 6620 7374 6174 7573 203d 3d20 303a  lif status == 0:
-00004980: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00004990: 6c66 2e73 6574 466c 6167 2862 7573 793d  lf.setFlag(busy=
-000049a0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
-000049b0: 7265 7475 726e 2053 7461 7475 7343 6f64  return StatusCod
-000049c0: 6528 7365 6c66 2e5f 7374 6174 7573 5f63  e(self._status_c
-000049d0: 6f64 6529 2e6e 616d 650d 0a20 2020 200d  ode).name..    .
-000049e0: 0a20 2020 2064 6566 2068 6f6d 6528 7365  .    def home(se
-000049f0: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
-00004a00: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00004a10: 2020 5265 7475 726e 2070 6c75 6e67 6572    Return plunger
-00004a20: 2074 6f20 686f 6d65 2070 6f73 6974 696f   to home positio
-00004a30: 6e0d 0a20 2020 2020 2020 200d 0a20 2020  n..        ..   
-00004a40: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
-00004a50: 2020 2020 2020 2020 2020 2073 7472 3a20             str: 
-00004a60: 6465 7669 6365 2072 6573 706f 6e73 650d  device response.
-00004a70: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00004a80: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
-00004a90: 2073 656c 662e 5f71 7565 7279 2866 2752   self._query(f'R
-00004aa0: 507b 7365 6c66 2e68 6f6d 655f 706f 7369  P{self.home_posi
-00004ab0: 7469 6f6e 7d27 290d 0a20 2020 2020 2020  tion}')..       
-00004ac0: 2073 656c 662e 766f 6c75 6d65 203d 2030   self.volume = 0
-00004ad0: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
-00004ae0: 6f73 6974 696f 6e20 3d20 7365 6c66 2e68  osition = self.h
-00004af0: 6f6d 655f 706f 7369 7469 6f6e 0d0a 2020  ome_position..  
-00004b00: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
-00004b10: 2831 290d 0a20 2020 2020 2020 2072 6574  (1)..        ret
-00004b20: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
-00004b30: 2020 0d0a 2020 2020 6465 6620 6973 4665    ..    def isFe
-00004b40: 6173 6962 6c65 2873 656c 662c 2070 6f73  asible(self, pos
-00004b50: 6974 696f 6e3a 696e 7429 202d 3e20 626f  ition:int) -> bo
-00004b60: 6f6c 3a0d 0a20 2020 2020 2020 2022 2222  ol:..        """
-00004b70: 0d0a 2020 2020 2020 2020 4368 6563 6b73  ..        Checks
-00004b80: 2061 6e64 2072 6574 7572 6e73 2077 6865   and returns whe
-00004b90: 7468 6572 2074 6865 2070 6c75 6e67 6572  ther the plunger
-00004ba0: 2070 6f73 6974 696f 6e20 6973 2066 6561   position is fea
-00004bb0: 7369 626c 650d 0a0d 0a20 2020 2020 2020  sible....       
-00004bc0: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
-00004bd0: 2020 2020 706f 7369 7469 6f6e 2028 696e      position (in
-00004be0: 7429 3a20 706c 756e 6765 7220 706f 7369  t): plunger posi
-00004bf0: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
-00004c00: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
-00004c10: 2020 2020 2020 626f 6f6c 3a20 7768 6574        bool: whet
-00004c20: 6865 7220 706c 756e 6765 7220 706f 7369  her plunger posi
-00004c30: 7469 6f6e 2069 7320 6665 6173 6962 6c65  tion is feasible
-00004c40: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00004c50: 2020 2020 2020 2069 6620 2873 656c 662e         if (self.
-00004c60: 6c69 6d69 7473 5b30 5d20 3c3d 2070 6f73  limits[0] <= pos
-00004c70: 6974 696f 6e20 3c3d 2073 656c 662e 6c69  ition <= self.li
-00004c80: 6d69 7473 5b31 5d29 3a0d 0a20 2020 2020  mits[1]):..     
-00004c90: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00004ca0: 7565 0d0a 2020 2020 2020 2020 7072 696e  ue..        prin
-00004cb0: 7428 6622 5261 6e67 6520 6c69 6d69 7473  t(f"Range limits
-00004cc0: 2072 6561 6368 6564 2120 7b73 656c 662e   reached! {self.
-00004cd0: 6c69 6d69 7473 7d22 290d 0a20 2020 2020  limits}")..     
-00004ce0: 2020 2072 6574 7572 6e20 4661 6c73 650d     return False.
-00004cf0: 0a20 2020 200d 0a20 2020 2064 6566 2069  .    ..    def i
-00004d00: 7354 6970 4f6e 2873 656c 6629 202d 3e20  sTipOn(self) -> 
-00004d10: 626f 6f6c 3a0d 0a20 2020 2020 2020 2022  bool:..        "
-00004d20: 2222 0d0a 2020 2020 2020 2020 4368 6563  ""..        Chec
-00004d30: 6b73 2061 6e64 2072 6574 7572 6e73 2077  ks and returns w
-00004d40: 6865 7468 6572 2061 2070 6970 6574 7465  hether a pipette
-00004d50: 2074 6970 2069 7320 6174 7461 6368 6564   tip is attached
-00004d60: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00004d70: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
-00004d80: 2020 2020 2020 2020 2020 626f 6f6c 3a20            bool: 
-00004d90: 7768 6574 6865 7220 6120 7069 7065 7474  whether a pipett
-00004da0: 6520 7469 7020 696e 2061 7474 6163 6865  e tip in attache
-00004db0: 640d 0a20 2020 2020 2020 2022 2222 0d0a  d..        """..
-00004dc0: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-00004dd0: 4361 7061 6369 7461 6e63 6528 290d 0a20  Capacitance().. 
-00004de0: 2020 2020 2020 2070 7269 6e74 2866 2754         print(f'T
-00004df0: 6970 2063 6170 6163 6974 616e 6365 3a20  ip capacitance: 
-00004e00: 7b73 656c 662e 6361 7061 6369 7461 6e63  {self.capacitanc
-00004e10: 657d 2729 0d0a 2020 2020 2020 2020 6966  e}')..        if
-00004e20: 2073 656c 662e 666c 6167 735b 2763 6f6e   self.flags['con
-00004e30: 6475 6374 6976 655f 7469 7073 275d 3a0d  ductive_tips']:.
-00004e40: 0a20 2020 2020 2020 2020 2020 2074 6970  .            tip
-00004e50: 5f6f 6e20 3d20 2873 656c 662e 6361 7061  _on = (self.capa
-00004e60: 6369 7461 6e63 6520 3e20 7365 6c66 2e74  citance > self.t
-00004e70: 6970 5f74 6872 6573 686f 6c64 290d 0a20  ip_threshold).. 
-00004e80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00004e90: 7365 7446 6c61 6728 7469 705f 6f6e 3d74  setFlag(tip_on=t
-00004ea0: 6970 5f6f 6e29 0d0a 2020 2020 2020 2020  ip_on)..        
-00004eb0: 7469 705f 6f6e 203d 2073 656c 662e 666c  tip_on = self.fl
-00004ec0: 6167 735b 2774 6970 5f6f 6e27 5d0d 0a20  ags['tip_on'].. 
-00004ed0: 2020 2020 2020 2072 6574 7572 6e20 7469         return ti
-00004ee0: 705f 6f6e 0d0a 2020 2020 0d0a 2020 2020  p_on..    ..    
-00004ef0: 6465 6620 6d6f 7665 2873 656c 662c 2073  def move(self, s
-00004f00: 7465 7073 3a69 6e74 2c20 7570 3a62 6f6f  teps:int, up:boo
-00004f10: 6c2c 202a 2a6b 7761 7267 7329 202d 3e20  l, **kwargs) -> 
-00004f20: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
-00004f30: 220d 0a20 2020 2020 2020 204d 6f76 6520  "..        Move 
-00004f40: 7468 6520 706c 756e 6765 7220 6569 7468  the plunger eith
-00004f50: 6572 2075 7020 6f72 2064 6f77 6e20 6279  er up or down by
-00004f60: 2061 2073 7065 6369 6669 6564 206e 756d   a specified num
-00004f70: 6265 7220 6f66 2073 7465 7073 0d0a 0d0a  ber of steps....
-00004f80: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
-00004f90: 2020 2020 2020 2020 2020 2073 7465 7073             steps
-00004fa0: 2028 696e 7429 3a20 6e75 6d62 6572 206f   (int): number o
-00004fb0: 6620 7374 6570 7320 746f 206d 6f76 6520  f steps to move 
-00004fc0: 706c 756e 6765 7220 6279 0d0a 2020 2020  plunger by..    
-00004fd0: 2020 2020 2020 2020 7570 2028 626f 6f6c          up (bool
-00004fe0: 293a 2077 6865 7468 6572 2074 6f20 6d6f  ): whether to mo
-00004ff0: 7665 2074 6865 2070 6c75 6e67 6572 2075  ve the plunger u
-00005000: 700d 0a0d 0a20 2020 2020 2020 2052 6574  p....        Ret
-00005010: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-00005020: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
-00005030: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
-00005040: 2022 2222 0d0a 2020 2020 2020 2020 7374   """..        st
-00005050: 6570 7320 3d20 6162 7328 7374 6570 7329  eps = abs(steps)
-00005060: 2069 6620 7570 2065 6c73 6520 2d61 6273   if up else -abs
-00005070: 2873 7465 7073 290d 0a20 2020 2020 2020  (steps)..       
-00005080: 2072 6574 7572 6e20 7365 6c66 2e6d 6f76   return self.mov
-00005090: 6542 7928 7374 6570 7329 0d0a 2020 2020  eBy(steps)..    
-000050a0: 0d0a 2020 2020 6465 6620 6d6f 7665 4279  ..    def moveBy
-000050b0: 2873 656c 662c 2073 7465 7073 3a69 6e74  (self, steps:int
-000050c0: 2c20 2a2a 6b77 6172 6773 2920 2d3e 2073  , **kwargs) -> s
-000050d0: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
-000050e0: 0d0a 2020 2020 2020 2020 4d6f 7665 2074  ..        Move t
-000050f0: 6865 2070 6c75 6e67 6572 2062 7920 7370  he plunger by sp
-00005100: 6563 6966 6965 6420 6e75 6d62 6572 206f  ecified number o
-00005110: 6620 7374 6570 730d 0a0d 0a20 2020 2020  f steps....     
-00005120: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
-00005130: 2020 2020 2020 7374 6570 7320 2869 6e74        steps (int
-00005140: 293a 206e 756d 6265 7220 6f66 2073 7465  ): number of ste
-00005150: 7073 2074 6f20 6d6f 7665 2070 6c75 6e67  ps to move plung
-00005160: 6572 2062 7920 283c 303a 206d 6f76 6520  er by (<0: move 
-00005170: 646f 776e 2f64 6973 7065 6e73 653b 203e  down/dispense; >
-00005180: 3020 6d6f 7665 2075 702f 6173 7069 7261  0 move up/aspira
-00005190: 7465 290d 0a0d 0a20 2020 2020 2020 2052  te)....        R
-000051a0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-000051b0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
-000051c0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
-000051d0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000051e0: 636f 6d6d 616e 6420 3d20 6627 5249 7b73  command = f'RI{s
-000051f0: 7465 7073 7d27 2069 6620 7374 6570 7320  teps}' if steps 
-00005200: 3e20 3020 656c 7365 2066 2752 4f7b 2d73  > 0 else f'RO{-s
-00005210: 7465 7073 7d27 0d0a 2020 2020 2020 2020  teps}'..        
-00005220: 7365 6c66 2e70 6f73 6974 696f 6e20 2b3d  self.position +=
-00005230: 2073 7465 7073 0d0a 2020 2020 2020 2020   steps..        
-00005240: 7265 7475 726e 2073 656c 662e 5f71 7565  return self._que
-00005250: 7279 2863 6f6d 6d61 6e64 290d 0a20 2020  ry(command)..   
-00005260: 200d 0a20 2020 2064 6566 206d 6f76 6554   ..    def moveT
-00005270: 6f28 7365 6c66 2c20 706f 7369 7469 6f6e  o(self, position
-00005280: 3a69 6e74 2c20 2a2a 6b77 6172 6773 2920  :int, **kwargs) 
-00005290: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
-000052a0: 2022 2222 0d0a 2020 2020 2020 2020 4d6f   """..        Mo
-000052b0: 7665 2074 6865 2070 6c75 6e67 6572 2074  ve the plunger t
-000052c0: 6f20 6120 7370 6563 6966 6965 6420 706f  o a specified po
-000052d0: 7369 7469 6f6e 0d0a 0d0a 2020 2020 2020  sition....      
-000052e0: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
-000052f0: 2020 2020 2070 6f73 6974 696f 6e20 2869       position (i
-00005300: 6e74 293a 2074 6172 6765 7420 706c 756e  nt): target plun
-00005310: 6765 7220 706f 7369 7469 6f6e 0d0a 0d0a  ger position....
-00005320: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00005330: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00005340: 723a 2064 6576 6963 6520 7265 7370 6f6e  r: device respon
-00005350: 7365 0d0a 2020 2020 2020 2020 2222 220d  se..        """.
-00005360: 0a20 2020 2020 2020 2073 656c 662e 706f  .        self.po
-00005370: 7369 7469 6f6e 203d 2070 6f73 6974 696f  sition = positio
-00005380: 6e0d 0a20 2020 2020 2020 2072 6574 7572  n..        retur
-00005390: 6e20 7365 6c66 2e5f 7175 6572 7928 6627  n self._query(f'
-000053a0: 5250 7b70 6f73 6974 696f 6e7d 2729 0d0a  RP{position}')..
-000053b0: 2020 2020 0d0a 2020 2020 6465 6620 7075      ..    def pu
-000053c0: 6c6c 6261 636b 2873 656c 662c 2073 7465  llback(self, ste
-000053d0: 7073 3a69 6e74 203d 2035 2c20 2a2a 6b77  ps:int = 5, **kw
-000053e0: 6172 6773 2920 2d3e 2073 7472 3a0d 0a20  args) -> str:.. 
-000053f0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00005400: 2020 2020 5075 6c6c 6261 636b 206c 6971      Pullback liq
-00005410: 7569 6420 6672 6f6d 2074 6970 0d0a 2020  uid from tip..  
-00005420: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00005430: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
-00005440: 2020 2073 7465 7073 2028 696e 742c 206f     steps (int, o
-00005450: 7074 696f 6e61 6c29 3a20 6e75 6d62 6572  ptional): number
-00005460: 206f 6620 7374 6570 7320 746f 2070 756c   of steps to pul
-00005470: 6c62 6163 6b2e 2044 6566 6175 6c74 7320  lback. Defaults 
-00005480: 746f 2035 2e0d 0a0d 0a20 2020 2020 2020  to 5.....       
-00005490: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
-000054a0: 2020 2020 2020 2073 7472 3a20 6465 7669         str: devi
-000054b0: 6365 2072 6573 706f 6e73 650d 0a20 2020  ce response..   
-000054c0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-000054d0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
-000054e0: 662e 5f71 7565 7279 2866 2752 497b 7374  f._query(f'RI{st
-000054f0: 6570 737d 2729 0d0a 2020 2020 2020 2020  eps}')..        
-00005500: 7365 6c66 2e70 6f73 6974 696f 6e20 2b3d  self.position +=
-00005510: 2073 7465 7073 0d0a 2020 2020 2020 2020   steps..        
-00005520: 7469 6d65 2e73 6c65 6570 2831 290d 0a20  time.sleep(1).. 
-00005530: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00005540: 7370 6f6e 7365 0d0a 2020 2020 0d0a 2020  sponse..    ..  
-00005550: 2020 6465 6620 7265 7365 7428 7365 6c66    def reset(self
-00005560: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
-00005570: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00005580: 5265 7365 7420 7468 6520 7069 7065 7474  Reset the pipett
-00005590: 650d 0a0d 0a20 2020 2020 2020 2052 6574  e....        Ret
-000055a0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
-000055b0: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
-000055c0: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
-000055d0: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
-000055e0: 6c66 2e7a 6572 6f28 290d 0a20 2020 2020  lf.zero()..     
-000055f0: 2020 2072 6574 7572 6e20 7365 6c66 2e68     return self.h
-00005600: 6f6d 6528 290d 0a20 2020 200d 0a20 2020  ome()..    ..   
-00005610: 2064 6566 2073 6574 5370 6565 6428 7365   def setSpeed(se
-00005620: 6c66 2c20 7370 6565 643a 696e 742c 2075  lf, speed:int, u
-00005630: 703a 626f 6f6c 2c20 6465 6661 756c 743a  p:bool, default:
-00005640: 626f 6f6c 203d 2046 616c 7365 2c20 2a2a  bool = False, **
-00005650: 6b77 6172 6773 2920 2d3e 2073 7472 3a0d  kwargs) -> str:.
-00005660: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00005670: 2020 2020 2020 5365 7420 7468 6520 7370        Set the sp
-00005680: 6565 6420 6f66 2074 6865 2070 6c75 6e67  eed of the plung
-00005690: 6572 0d0a 0d0a 2020 2020 2020 2020 4172  er....        Ar
-000056a0: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
-000056b0: 2073 7065 6564 2028 696e 7429 3a20 7370   speed (int): sp
-000056c0: 6565 6420 6f66 2070 6c75 6e67 6572 0d0a  eed of plunger..
-000056d0: 2020 2020 2020 2020 2020 2020 7570 2028              up (
-000056e0: 626f 6f6c 293a 2064 6972 6563 7469 6f6e  bool): direction
-000056f0: 206f 6620 7472 6176 656c 0d0a 2020 2020   of travel..    
-00005700: 2020 2020 2020 2020 6465 6661 756c 7420          default 
-00005710: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
-00005720: 3a20 7768 6574 6865 7220 746f 2073 6574  : whether to set
-00005730: 2073 7065 6564 2061 7320 6120 6465 6661   speed as a defa
-00005740: 756c 742e 2044 6566 6175 6c74 7320 746f  ult. Defaults to
-00005750: 2046 616c 7365 2e0d 0a0d 0a20 2020 2020   False.....     
-00005760: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00005770: 2020 2020 2020 2020 2073 7472 3a20 6465           str: de
-00005780: 7669 6365 2072 6573 706f 6e73 650d 0a20  vice response.. 
-00005790: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000057a0: 2020 2020 7370 6565 645f 636f 6465 203d      speed_code =
-000057b0: 2031 202b 205b 7820 666f 7220 782c 7661   1 + [x for x,va
-000057c0: 6c20 696e 2065 6e75 6d65 7261 7465 286e  l in enumerate(n
-000057d0: 702e 6172 7261 7928 7365 6c66 2e73 7065  p.array(self.spe
-000057e0: 6564 5f70 7265 7365 7473 292d 7370 6565  ed_presets)-spee
-000057f0: 6429 2069 6620 7661 6c20 3e3d 2030 5d5b  d) if val >= 0][
-00005800: 305d 0d0a 2020 2020 2020 2020 7072 696e  0]..        prin
-00005810: 7428 6627 5370 6565 6420 7b73 7065 6564  t(f'Speed {speed
-00005820: 5f63 6f64 657d 3a20 7b73 656c 662e 7370  _code}: {self.sp
-00005830: 6565 645f 7072 6573 6574 735b 7370 6565  eed_presets[spee
-00005840: 645f 636f 6465 2d31 5d7d 2075 4c2f 7327  d_code-1]} uL/s'
-00005850: 290d 0a20 2020 2020 2020 2064 6972 6563  )..        direc
-00005860: 7469 6f6e 203d 2027 4927 2069 6620 7570  tion = 'I' if up
-00005870: 2065 6c73 6520 274f 270d 0a20 2020 2020   else 'O'..     
-00005880: 2020 2073 656c 662e 5f71 7565 7279 2866     self._query(f
-00005890: 2753 7b64 6972 6563 7469 6f6e 7d7b 7370  'S{direction}{sp
-000058a0: 6565 645f 636f 6465 7d27 290d 0a20 2020  eed_code}')..   
-000058b0: 2020 2020 2069 6620 6e6f 7420 6465 6661       if not defa
-000058c0: 756c 743a 0d0a 2020 2020 2020 2020 2020  ult:..          
-000058d0: 2020 7265 7475 726e 2073 656c 662e 5f71    return self._q
-000058e0: 7565 7279 2866 2744 7b64 6972 6563 7469  uery(f'D{directi
-000058f0: 6f6e 7d27 290d 0a20 2020 2020 2020 2069  on}')..        i
-00005900: 6620 7570 3a0d 0a20 2020 2020 2020 2020  f up:..         
-00005910: 2020 2073 656c 662e 7370 6565 645f 636f     self.speed_co
-00005920: 6465 2e75 7020 3d20 7370 6565 645f 636f  de.up = speed_co
-00005930: 6465 0d0a 2020 2020 2020 2020 2020 2020  de..            
-00005940: 7365 6c66 2e73 7065 6564 2e75 7020 3d20  self.speed.up = 
-00005950: 7365 6c66 2e73 7065 6564 5f70 7265 7365  self.speed_prese
-00005960: 7473 5b73 7065 6564 5f63 6f64 652d 315d  ts[speed_code-1]
-00005970: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00005980: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00005990: 662e 7370 6565 645f 636f 6465 2e64 6f77  f.speed_code.dow
-000059a0: 6e20 3d20 7370 6565 645f 636f 6465 0d0a  n = speed_code..
-000059b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000059c0: 2e73 7065 6564 2e64 6f77 6e20 3d20 7365  .speed.down = se
-000059d0: 6c66 2e73 7065 6564 5f70 7265 7365 7473  lf.speed_presets
-000059e0: 5b73 7065 6564 5f63 6f64 652d 315d 0d0a  [speed_code-1]..
-000059f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00005a00: 656c 662e 5f71 7565 7279 2866 2744 7b64  elf._query(f'D{d
-00005a10: 6972 6563 7469 6f6e 7d27 290d 0a20 2020  irection}')..   
-00005a20: 200d 0a20 2020 2064 6566 2073 6875 7464   ..    def shutd
-00005a30: 6f77 6e28 7365 6c66 293a 0d0a 2020 2020  own(self):..    
-00005a40: 2020 2020 2222 2253 6875 7464 6f77 6e20      """Shutdown 
-00005a50: 7072 6f63 6564 7572 6520 666f 7220 746f  procedure for to
-00005a60: 6f6c 2222 220d 0a20 2020 2020 2020 2073  ol"""..        s
-00005a70: 656c 662e 746f 6767 6c65 4665 6564 6261  elf.toggleFeedba
-00005a80: 636b 4c6f 6f70 286f 6e3d 4661 6c73 6529  ckLoop(on=False)
-00005a90: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00005aa0: 2073 7570 6572 2829 2e73 6875 7464 6f77   super().shutdow
-00005ab0: 6e28 290d 0a20 2020 200d 0a20 2020 2064  n()..    ..    d
-00005ac0: 6566 2074 6f67 676c 6546 6565 6462 6163  ef toggleFeedbac
-00005ad0: 6b4c 6f6f 7028 7365 6c66 2c20 6f6e 3a62  kLoop(self, on:b
-00005ae0: 6f6f 6c29 3a0d 0a20 2020 2020 2020 2022  ool):..        "
-00005af0: 2222 0d0a 2020 2020 2020 2020 5374 6172  ""..        Star
-00005b00: 7420 6f72 2073 746f 7020 6665 6564 6261  t or stop feedba
-00005b10: 636b 206c 6f6f 700d 0a20 2020 2020 2020  ck loop..       
-00005b20: 200d 0a20 2020 2020 2020 2041 7267 733a   ..        Args:
-00005b30: 0d0a 2020 2020 2020 2020 2020 2020 6f6e  ..            on
-00005b40: 2028 626f 6f6c 293a 2077 6865 7468 6572   (bool): whether
-00005b50: 2074 6f20 7374 6172 7420 6665 6564 6261   to start feedba
-00005b60: 636b 206c 6f6f 700d 0a20 2020 2020 2020  ck loop..       
-00005b70: 2022 2222 0d0a 2020 2020 2020 2020 7365   """..        se
-00005b80: 6c66 2e73 6574 466c 6167 2867 6574 5f66  lf.setFlag(get_f
-00005b90: 6565 6462 6163 6b3d 6f6e 290d 0a20 2020  eedback=on)..   
-00005ba0: 2020 2020 2069 6620 6f6e 3a0d 0a20 2020       if on:..   
-00005bb0: 2020 2020 2020 2020 2069 6620 2766 6565           if 'fee
-00005bc0: 6462 6163 6b5f 6c6f 6f70 2720 696e 2073  dback_loop' in s
-00005bd0: 656c 662e 5f74 6872 6561 6473 3a0d 0a20  elf._threads:.. 
-00005be0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00005bf0: 656c 662e 5f74 6872 6561 6473 5b27 6665  elf._threads['fe
-00005c00: 6564 6261 636b 5f6c 6f6f 7027 5d2e 6a6f  edback_loop'].jo
-00005c10: 696e 2829 0d0a 2020 2020 2020 2020 2020  in()..          
-00005c20: 2020 7468 7265 6164 203d 2054 6872 6561    thread = Threa
-00005c30: 6428 7461 7267 6574 3d73 656c 662e 5f6c  d(target=self._l
-00005c40: 6f6f 705f 6665 6564 6261 636b 290d 0a20  oop_feedback).. 
-00005c50: 2020 2020 2020 2020 2020 2074 6872 6561             threa
-00005c60: 642e 7374 6172 7428 290d 0a20 2020 2020  d.start()..     
-00005c70: 2020 2020 2020 2073 656c 662e 5f74 6872         self._thr
-00005c80: 6561 6473 5b27 6665 6564 6261 636b 5f6c  eads['feedback_l
-00005c90: 6f6f 7027 5d20 3d20 7468 7265 6164 0d0a  oop'] = thread..
-00005ca0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00005cb0: 2020 2020 2020 2020 2020 2069 6620 2766             if 'f
-00005cc0: 6565 6462 6163 6b5f 6c6f 6f70 2720 696e  eedback_loop' in
-00005cd0: 2073 656c 662e 5f74 6872 6561 6473 3a0d   self._threads:.
-00005ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005cf0: 2073 656c 662e 5f74 6872 6561 6473 5b27   self._threads['
-00005d00: 6665 6564 6261 636b 5f6c 6f6f 7027 5d2e  feedback_loop'].
-00005d10: 6a6f 696e 2829 0d0a 2020 2020 2020 2020  join()..        
-00005d20: 7265 7475 726e 0d0a 0d0a 2020 2020 6465  return....    de
-00005d30: 6620 7a65 726f 2873 656c 6629 202d 3e20  f zero(self) -> 
-00005d40: 7374 723a 0d0a 2020 2020 2020 2020 2222  str:..        ""
-00005d50: 220d 0a20 2020 2020 2020 205a 6572 6f20  "..        Zero 
-00005d60: 7468 6520 706c 756e 6765 7220 706f 7369  the plunger posi
-00005d70: 7469 6f6e 0d0a 2020 2020 2020 2020 0d0a  tion..        ..
-00005d80: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00005d90: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00005da0: 723a 2064 6576 6963 6520 7265 7370 6f6e  r: device respon
-00005db0: 7365 0d0a 2020 2020 2020 2020 2222 220d  se..        """.
-00005dc0: 0a20 2020 2020 2020 2073 656c 662e 656a  .        self.ej
-00005dd0: 6563 7428 290d 0a20 2020 2020 2020 2072  ect()..        r
-00005de0: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
-00005df0: 7175 6572 7928 2752 5a27 290d 0a20 2020  query('RZ')..   
-00005e00: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
-00005e10: 6f6e 203d 2030 0d0a 2020 2020 2020 2020  on = 0..        
-00005e20: 7469 6d65 2e73 6c65 6570 2832 290d 0a20  time.sleep(2).. 
-00005e30: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-00005e40: 7370 6f6e 7365 0d0a 0d0a 2020 2020 2320  sponse....    # 
-00005e50: 5072 6f74 6563 7465 6420 6d65 7468 6f64  Protected method
-00005e60: 2873 290d 0a20 2020 2064 6566 205f 6361  (s)..    def _ca
-00005e70: 6c63 756c 6174 655f 7370 6565 645f 7061  lculate_speed_pa
-00005e80: 7261 6d65 7465 7273 2873 656c 662c 2076  rameters(self, v
-00005e90: 6f6c 756d 653a 696e 742c 2073 7065 6564  olume:int, speed
-00005ea0: 3a69 6e74 2920 2d3e 2053 7065 6564 5061  :int) -> SpeedPa
-00005eb0: 7261 6d65 7465 7273 3a0d 0a20 2020 2020  rameters:..     
-00005ec0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00005ed0: 4361 6c63 756c 6174 6573 2074 6865 2062  Calculates the b
-00005ee0: 6573 7420 7061 7261 6d65 7465 7273 2066  est parameters f
-00005ef0: 6f72 2076 6f6c 756d 6520 616e 6420 7370  or volume and sp
-00005f00: 6565 640d 0a0d 0a20 2020 2020 2020 2041  eed....        A
-00005f10: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-00005f20: 2020 766f 6c75 6d65 2028 696e 7429 3a20    volume (int): 
-00005f30: 766f 6c75 6d65 2074 6f20 6265 2074 7261  volume to be tra
-00005f40: 6e73 6665 7272 6564 0d0a 2020 2020 2020  nsferred..      
-00005f50: 2020 2020 2020 7370 6565 6420 2869 6e74        speed (int
-00005f60: 293a 2073 7065 6564 2061 7420 7768 6963  ): speed at whic
-00005f70: 6820 6c69 7175 6964 2069 7320 7472 616e  h liquid is tran
-00005f80: 7366 6572 7265 640d 0a0d 0a20 2020 2020  sferred....     
-00005f90: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
-00005fa0: 2020 2020 2020 2020 2064 6963 743a 2064           dict: d
-00005fb0: 6963 7469 6f6e 6172 7920 6f66 2062 6573  ictionary of bes
-00005fc0: 7420 7061 7261 6d65 7465 7273 0d0a 2020  t parameters..  
-00005fd0: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00005fe0: 2020 206f 7574 636f 6d65 7320 3d20 7b7d     outcomes = {}
-00005ff0: 0d0a 2020 2020 2020 2020 7374 6570 5f69  ..        step_i
-00006000: 6e74 6572 7661 6c5f 6c69 6d69 7420 3d20  nterval_limit = 
-00006010: 696e 7428 766f 6c75 6d65 2f73 656c 662e  int(volume/self.
-00006020: 7265 736f 6c75 7469 6f6e 2f53 5445 505f  resolution/STEP_
-00006030: 5245 534f 4c55 5449 4f4e 290d 0a20 2020  RESOLUTION)..   
-00006040: 2020 2020 2066 6f72 2070 7265 7365 7420       for preset 
-00006050: 696e 2073 656c 662e 7370 6565 645f 7072  in self.speed_pr
-00006060: 6573 6574 733a 0d0a 2020 2020 2020 2020  esets:..        
-00006070: 2020 2020 6966 2070 7265 7365 7420 3c20      if preset < 
-00006080: 7370 6565 643a 0d0a 2020 2020 2020 2020  speed:..        
-00006090: 2020 2020 2020 2020 2320 7072 6573 6574          # preset
-000060a0: 2069 7320 736c 6f77 6572 2074 6861 6e20   is slower than 
-000060b0: 7461 7267 6574 2073 7065 6564 2c20 6974  target speed, it
-000060c0: 2077 696c 6c20 6e65 7665 7220 6869 7420   will never hit 
-000060d0: 7461 7267 6574 2073 7065 6564 0d0a 2020  target speed..  
-000060e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000060f0: 6e74 696e 7565 0d0a 2020 2020 2020 2020  ntinue..        
-00006100: 2020 2020 7469 6d65 5f69 6e74 6572 7661      time_interva
-00006110: 6c5f 6c69 6d69 7420 3d20 696e 7428 766f  l_limit = int(vo
-00006120: 6c75 6d65 2a28 312f 7370 6565 6420 2d20  lume*(1/speed - 
-00006130: 312f 7072 6573 6574 292f 7365 6c66 2e72  1/preset)/self.r
-00006140: 6573 706f 6e73 655f 7469 6d65 290d 0a20  esponse_time).. 
-00006150: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00006160: 7420 7374 6570 5f69 6e74 6572 7661 6c5f  t step_interval_
-00006170: 6c69 6d69 7420 6f72 206e 6f74 2074 696d  limit or not tim
-00006180: 655f 696e 7465 7276 616c 5f6c 696d 6974  e_interval_limit
-00006190: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000061a0: 2020 2063 6f6e 7469 6e75 650d 0a20 2020     continue..   
-000061b0: 2020 2020 2020 2020 2069 6e74 6572 7661           interva
-000061c0: 6c73 203d 206d 6178 286d 696e 2873 7465  ls = max(min(ste
-000061d0: 705f 696e 7465 7276 616c 5f6c 696d 6974  p_interval_limit
-000061e0: 2c20 7469 6d65 5f69 6e74 6572 7661 6c5f  , time_interval_
-000061f0: 6c69 6d69 7429 2c20 3129 0d0a 2020 2020  limit), 1)..    
-00006200: 2020 2020 2020 2020 6561 6368 5f73 7465          each_ste
-00006210: 7073 203d 2076 6f6c 756d 652f 7365 6c66  ps = volume/self
-00006220: 2e72 6573 6f6c 7574 696f 6e2f 696e 7465  .resolution/inte
-00006230: 7276 616c 730d 0a20 2020 2020 2020 2020  rvals..         
-00006240: 2020 2065 6163 685f 6465 6c61 7920 3d20     each_delay = 
-00006250: 766f 6c75 6d65 2a28 312f 7370 6565 6420  volume*(1/speed 
-00006260: 2d20 312f 7072 6573 6574 292f 696e 7465  - 1/preset)/inte
-00006270: 7276 616c 730d 0a20 2020 2020 2020 2020  rvals..         
-00006280: 2020 2061 7265 6120 3d20 302e 3520 2a20     area = 0.5 * 
-00006290: 2876 6f6c 756d 652a 2a32 2920 2a20 2831  (volume**2) * (1
-000062a0: 2f73 656c 662e 7265 736f 6c75 7469 6f6e  /self.resolution
-000062b0: 2920 2a20 2831 2f69 6e74 6572 7661 6c73  ) * (1/intervals
-000062c0: 2920 2a20 2831 2f73 7065 6564 202d 2031  ) * (1/speed - 1
-000062d0: 2f70 7265 7365 7429 0d0a 2020 2020 2020  /preset)..      
-000062e0: 2020 2020 2020 6f75 7463 6f6d 6573 5b61        outcomes[a
-000062f0: 7265 615d 203d 2053 7065 6564 5061 7261  rea] = SpeedPara
-00006300: 6d65 7465 7273 2870 7265 7365 742c 2069  meters(preset, i
-00006310: 6e74 6572 7661 6c73 2c20 696e 7428 6561  ntervals, int(ea
-00006320: 6368 5f73 7465 7073 292c 2065 6163 685f  ch_steps), each_
-00006330: 6465 6c61 7929 0d0a 2020 2020 2020 2020  delay)..        
-00006340: 6966 206c 656e 286f 7574 636f 6d65 7329  if len(outcomes)
-00006350: 203d 3d20 303a 0d0a 2020 2020 2020 2020   == 0:..        
-00006360: 2020 2020 7072 696e 7428 224e 6f20 6665      print("No fe
-00006370: 6173 6962 6c65 2073 7065 6564 2070 6172  asible speed par
-00006380: 616d 6574 6572 732e 2229 0d0a 2020 2020  ameters.")..    
-00006390: 2020 2020 2020 2020 7265 7475 726e 2053          return S
-000063a0: 7065 6564 5061 7261 6d65 7465 7273 284e  peedParameters(N
-000063b0: 6f6e 652c 2053 5445 505f 5245 534f 4c55  one, STEP_RESOLU
-000063c0: 5449 4f4e 2c20 5354 4550 5f52 4553 4f4c  TION, STEP_RESOL
-000063d0: 5554 494f 4e2c 2073 656c 662e 7265 7370  UTION, self.resp
-000063e0: 6f6e 7365 5f74 696d 6529 0d0a 2020 2020  onse_time)..    
-000063f0: 2020 2020 7072 696e 7428 6627 4265 7374      print(f'Best
-00006400: 2070 6172 616d 6574 6572 733a 207b 6f75   parameters: {ou
-00006410: 7463 6f6d 6573 5b6d 696e 286f 7574 636f  tcomes[min(outco
-00006420: 6d65 7329 5d7d 2729 0d0a 2020 2020 2020  mes)]}')..      
-00006430: 2020 7265 7475 726e 206f 7574 636f 6d65    return outcome
-00006440: 735b 6d69 6e28 6f75 7463 6f6d 6573 295d  s[min(outcomes)]
-00006450: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00006460: 5f63 6f6e 6e65 6374 2873 656c 662c 2070  _connect(self, p
-00006470: 6f72 743a 7374 722c 2062 6175 6472 6174  ort:str, baudrat
-00006480: 653a 696e 7420 3d20 3936 3030 2c20 7469  e:int = 9600, ti
-00006490: 6d65 6f75 743a 696e 7420 3d20 3129 3a0d  meout:int = 1):.
-000064a0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-000064b0: 2020 2020 2020 436f 6e6e 6563 7469 6f6e        Connection
-000064c0: 2070 726f 6365 6475 7265 2066 6f72 2074   procedure for t
-000064d0: 6f6f 6c0d 0a0d 0a20 2020 2020 2020 2041  ool....        A
-000064e0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
-000064f0: 2020 706f 7274 2028 7374 7229 3a20 434f    port (str): CO
-00006500: 4d20 706f 7274 2061 6464 7265 7373 0d0a  M port address..
-00006510: 2020 2020 2020 2020 2020 2020 6261 7564              baud
-00006520: 7261 7465 2028 696e 742c 206f 7074 696f  rate (int, optio
-00006530: 6e61 6c29 3a20 6261 7564 7261 7465 2e20  nal): baudrate. 
-00006540: 4465 6661 756c 7473 2074 6f20 3936 3030  Defaults to 9600
-00006550: 2e0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
-00006560: 696d 656f 7574 2028 696e 742c 206f 7074  imeout (int, opt
-00006570: 696f 6e61 6c29 3a20 7469 6d65 6f75 7420  ional): timeout 
-00006580: 696e 2073 6563 6f6e 6473 2e20 4465 6661  in seconds. Defa
-00006590: 756c 7473 2074 6f20 312e 0d0a 2020 2020  ults to 1...    
-000065a0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000065b0: 2073 656c 662e 636f 6e6e 6563 7469 6f6e   self.connection
-000065c0: 5f64 6574 6169 6c73 203d 207b 0d0a 2020  _details = {..  
-000065d0: 2020 2020 2020 2020 2020 2770 6f72 7427            'port'
-000065e0: 3a20 706f 7274 2c0d 0a20 2020 2020 2020  : port,..       
-000065f0: 2020 2020 2027 6261 7564 7261 7465 273a       'baudrate':
-00006600: 2062 6175 6472 6174 652c 0d0a 2020 2020   baudrate,..    
-00006610: 2020 2020 2020 2020 2774 696d 656f 7574          'timeout
-00006620: 273a 2074 696d 656f 7574 0d0a 2020 2020  ': timeout..    
-00006630: 2020 2020 7d0d 0a20 2020 2020 2020 2064      }..        d
-00006640: 6576 6963 6520 3d20 4e6f 6e65 0d0a 2020  evice = None..  
-00006650: 2020 2020 2020 7472 793a 0d0a 2020 2020        try:..    
-00006660: 2020 2020 2020 2020 6465 7669 6365 203d          device =
-00006670: 2073 6572 6961 6c2e 5365 7269 616c 2870   serial.Serial(p
-00006680: 6f72 742c 2062 6175 6472 6174 652c 2074  ort, baudrate, t
-00006690: 696d 656f 7574 3d74 696d 656f 7574 290d  imeout=timeout).
-000066a0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-000066b0: 4578 6365 7074 696f 6e20 6173 2065 3a0d  Exception as e:.
-000066c0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-000066d0: 6e74 2866 2243 6f75 6c64 206e 6f74 2063  nt(f"Could not c
-000066e0: 6f6e 6e65 6374 2074 6f20 7b70 6f72 747d  onnect to {port}
-000066f0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00006700: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
-00006710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006720: 2020 7072 696e 7428 6529 0d0a 2020 2020    print(e)..    
-00006730: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00006740: 2020 2020 2020 2074 696d 652e 736c 6565         time.slee
-00006750: 7028 3229 2020 2023 2057 6169 7420 666f  p(2)   # Wait fo
-00006760: 7220 6772 626c 2074 6f20 696e 6974 6961  r grbl to initia
-00006770: 6c69 7a65 0d0a 2020 2020 2020 2020 2020  lize..          
-00006780: 2020 6465 7669 6365 2e66 6c75 7368 496e    device.flushIn
-00006790: 7075 7428 290d 0a20 2020 2020 2020 2020  put()..         
-000067a0: 2020 2070 7269 6e74 2866 2243 6f6e 6e65     print(f"Conne
-000067b0: 6374 696f 6e20 6f70 656e 6564 2074 6f20  ction opened to 
-000067c0: 7b70 6f72 747d 2229 0d0a 2020 2020 2020  {port}")..      
-000067d0: 2020 2020 2020 7365 6c66 2e73 6574 466c        self.setFl
-000067e0: 6167 2863 6f6e 6e65 6374 6564 3d54 7275  ag(connected=Tru
-000067f0: 6529 0d0a 2020 2020 2020 2020 7365 6c66  e)..        self
-00006800: 2e64 6576 6963 6520 3d20 6465 7669 6365  .device = device
-00006810: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
-00006820: 6574 496e 666f 2829 0d0a 2020 2020 2020  etInfo()..      
-00006830: 2020 7365 6c66 2e72 6573 6574 2829 0d0a    self.reset()..
-00006840: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-00006850: 2020 2020 0d0a 2020 2020 6465 6620 5f69      ..    def _i
-00006860: 735f 6578 7065 6374 6564 5f72 6570 6c79  s_expected_reply
-00006870: 2873 656c 662c 2072 6573 706f 6e73 653a  (self, response:
-00006880: 7374 722c 2063 6f6d 6d61 6e64 5f63 6f64  str, command_cod
-00006890: 653a 7374 722c 202a 2a6b 7761 7267 7329  e:str, **kwargs)
-000068a0: 202d 3e20 626f 6f6c 3a0d 0a20 2020 2020   -> bool:..     
-000068b0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-000068c0: 4368 6563 6b73 2061 6e64 2072 6574 7572  Checks and retur
-000068d0: 6e73 2077 6865 7468 6572 2074 6865 2072  ns whether the r
-000068e0: 6573 706f 6e73 6520 6973 2061 6e20 6578  esponse is an ex
-000068f0: 7065 6374 6564 2072 6570 6c79 0d0a 0d0a  pected reply....
-00006900: 2020 2020 2020 2020 4172 6773 3a0d 0a20          Args:.. 
-00006910: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-00006920: 6e73 6520 2873 7472 293a 2072 6573 706f  nse (str): respo
-00006930: 6e73 6520 7374 7269 6e67 2066 726f 6d20  nse string from 
-00006940: 6465 7669 6365 0d0a 2020 2020 2020 2020  device..        
-00006950: 2020 2020 636f 6d6d 616e 645f 636f 6465      command_code
-00006960: 2028 7374 7229 3a20 7477 6f2d 6368 6172   (str): two-char
-00006970: 6163 7465 7220 636f 6d6d 616e 6420 636f  acter command co
-00006980: 6465 0d0a 0d0a 2020 2020 2020 2020 5265  de....        Re
-00006990: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
-000069a0: 2020 2020 626f 6f6c 3a20 7768 6574 6865      bool: whethe
-000069b0: 7220 7468 6520 7265 7370 6f6e 7365 2069  r the response i
-000069c0: 7320 616e 2065 7870 6563 7465 6420 7265  s an expected re
-000069d0: 706c 790d 0a20 2020 2020 2020 2022 2222  ply..        """
-000069e0: 0d0a 2020 2020 2020 2020 6966 2072 6573  ..        if res
-000069f0: 706f 6e73 6520 696e 2045 7272 6f72 436f  ponse in ErrorCo
-00006a00: 6465 2e5f 6d65 6d62 6572 5f6e 616d 6573  de._member_names
-00006a10: 5f3a 0d0a 2020 2020 2020 2020 2020 2020  _:..            
-00006a20: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
-00006a30: 2020 2020 2069 6620 636f 6d6d 616e 645f       if command_
-00006a40: 636f 6465 206e 6f74 2069 6e20 5155 4552  code not in QUER
-00006a50: 4945 5320 616e 6420 7265 7370 6f6e 7365  IES and response
-00006a60: 203d 3d20 276f 6b27 3a0d 0a20 2020 2020   == 'ok':..     
-00006a70: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-00006a80: 7565 0d0a 2020 2020 2020 2020 6966 2063  ue..        if c
-00006a90: 6f6d 6d61 6e64 5f63 6f64 6520 696e 2051  ommand_code in Q
-00006aa0: 5545 5249 4553 2061 6e64 2072 6573 706f  UERIES and respo
-00006ab0: 6e73 655b 3a32 5d20 3d3d 2063 6f6d 6d61  nse[:2] == comma
-00006ac0: 6e64 5f63 6f64 652e 6c6f 7765 7228 293a  nd_code.lower():
-00006ad0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00006ae0: 706c 795f 636f 6465 2c20 6461 7461 203d  ply_code, data =
-00006af0: 2072 6573 706f 6e73 655b 3a32 5d2c 2072   response[:2], r
-00006b00: 6573 706f 6e73 655b 323a 5d0d 0a20 2020  esponse[2:]..   
-00006b10: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00006b20: 2e76 6572 626f 7365 3a0d 0a20 2020 2020  .verbose:..     
-00006b30: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00006b40: 2866 275b 7b72 6570 6c79 5f63 6f64 657d  (f'[{reply_code}
-00006b50: 5d20 7b64 6174 617d 2729 0d0a 2020 2020  ] {data}')..    
-00006b60: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00006b70: 7275 650d 0a20 2020 2020 2020 2072 6574  rue..        ret
-00006b80: 7572 6e20 4661 6c73 650d 0a0d 0a20 2020  urn False....   
-00006b90: 2064 6566 205f 6c6f 6f70 5f66 6565 6462   def _loop_feedb
-00006ba0: 6163 6b28 7365 6c66 293a 0d0a 2020 2020  ack(self):..    
-00006bb0: 2020 2020 2222 224c 6f6f 7020 746f 2063      """Loop to c
-00006bc0: 6f6e 7374 616e 746c 7920 7265 6164 2066  onstantly read f
-00006bd0: 726f 6d20 6465 7669 6365 2222 220d 0a20  rom device""".. 
-00006be0: 2020 2020 2020 2070 7269 6e74 2827 4c69         print('Li
-00006bf0: 7374 656e 696e 672e 2e2e 2729 0d0a 2020  stening...')..  
-00006c00: 2020 2020 2020 7768 696c 6520 7365 6c66        while self
-00006c10: 2e66 6c61 6773 5b27 6765 745f 6665 6564  .flags['get_feed
-00006c20: 6261 636b 275d 3a0d 0a20 2020 2020 2020  back']:..       
-00006c30: 2020 2020 2069 6620 7365 6c66 2e66 6c61       if self.fla
-00006c40: 6773 5b27 7061 7573 655f 6665 6564 6261  gs['pause_feedba
-00006c50: 636b 275d 3a0d 0a20 2020 2020 2020 2020  ck']:..         
-00006c60: 2020 2020 2020 2063 6f6e 7469 6e75 650d         continue.
-00006c70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006c80: 662e 6765 7453 7461 7475 7328 290d 0a20  f.getStatus().. 
-00006c90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006ca0: 6765 7443 6170 6163 6974 616e 6365 2829  getCapacitance()
-00006cb0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00006cc0: 2753 746f 7020 6c69 7374 656e 696e 672e  'Stop listening.
-00006cd0: 2e2e 2729 0d0a 2020 2020 2020 2020 7265  ..')..        re
-00006ce0: 7475 726e 0d0a 2020 2020 0d0a 2020 2020  turn..    ..    
-00006cf0: 6465 6620 5f71 7565 7279 2873 656c 662c  def _query(self,
-00006d00: 200d 0a20 2020 2020 2020 2063 6f6d 6d61   ..        comma
-00006d10: 6e64 3a20 7374 722c 200d 0a20 2020 2020  nd: str, ..     
-00006d20: 2020 2074 696d 656f 7574 5f73 3a20 666c     timeout_s: fl
-00006d30: 6f61 7420 3d20 302e 332c 200d 0a20 2020  oat = 0.3, ..   
-00006d40: 2020 2020 2072 6573 756d 655f 6665 6564       resume_feed
-00006d50: 6261 636b 3a20 626f 6f6c 203d 2046 616c  back: bool = Fal
-00006d60: 7365 2c0d 0a20 2020 2020 2020 2067 6574  se,..        get
-00006d70: 5f70 6f73 6974 696f 6e3a 2062 6f6f 6c20  _position: bool 
-00006d80: 3d20 5472 7565 0d0a 2020 2020 2920 2d3e  = True..    ) ->
-00006d90: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
-00006da0: 2222 0d0a 2020 2020 2020 2020 5772 6974  ""..        Writ
-00006db0: 6520 636f 6d6d 616e 6420 746f 2061 6e64  e command to and
-00006dc0: 2072 6561 6420 7265 7370 6f6e 7365 2066   read response f
-00006dd0: 726f 6d20 6465 7669 6365 0d0a 0d0a 2020  rom device....  
-00006de0: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
-00006df0: 2020 2020 2020 2020 2063 6f6d 6d61 6e64           command
-00006e00: 2028 7374 7229 3a20 636f 6d6d 616e 6420   (str): command 
-00006e10: 7374 7269 6e67 0d0a 2020 2020 2020 2020  string..        
-00006e20: 2020 2020 7469 6d65 6f75 745f 7320 2866      timeout_s (f
-00006e30: 6c6f 6174 2c20 6f70 7469 6f6e 616c 293a  loat, optional):
-00006e40: 2064 7572 6174 696f 6e20 746f 2077 6169   duration to wai
-00006e50: 7420 6265 666f 7265 2074 696d 656f 7574  t before timeout
-00006e60: 2e20 4465 6661 756c 7473 2074 6f20 302e  . Defaults to 0.
-00006e70: 332e 0d0a 2020 2020 2020 2020 2020 2020  3...            
-00006e80: 7265 7375 6d65 5f66 6565 6462 6163 6b20  resume_feedback 
-00006e90: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
-00006ea0: 3a20 7768 6574 6865 7220 746f 2072 6573  : whether to res
-00006eb0: 756d 6520 7265 6164 696e 6720 6672 6f6d  ume reading from
-00006ec0: 2064 6576 6963 652e 2044 6566 6175 6c74   device. Default
-00006ed0: 7320 746f 2046 616c 7365 2e0d 0a20 2020  s to False...   
-00006ee0: 2020 2020 2020 2020 2067 6574 5f70 6f73           get_pos
-00006ef0: 6974 696f 6e20 2862 6f6f 6c2c 206f 7074  ition (bool, opt
-00006f00: 696f 6e61 6c29 3a20 7768 6574 6865 7220  ional): whether 
-00006f10: 746f 2067 6574 2074 6865 2070 6f73 6974  to get the posit
-00006f20: 696f 6e20 6f66 2074 6865 2070 6c75 6e67  ion of the plung
-00006f30: 6572 2e20 4465 6661 756c 7473 2074 6f20  er. Defaults to 
-00006f40: 5472 7565 2e0d 0a20 2020 2020 2020 2052  True...        R
-00006f50: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
-00006f60: 2020 2020 2073 7472 3a20 7265 7370 6f6e       str: respon
-00006f70: 7365 2073 7472 696e 670d 0a20 2020 2020  se string..     
-00006f80: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00006f90: 636f 6d6d 616e 645f 636f 6465 203d 2063  command_code = c
-00006fa0: 6f6d 6d61 6e64 5b3a 325d 0d0a 2020 2020  ommand[:2]..    
-00006fb0: 2020 2020 6966 2063 6f6d 6d61 6e64 5f63      if command_c
-00006fc0: 6f64 6520 6e6f 7420 696e 2053 5441 5455  ode not in STATU
-00006fd0: 535f 5155 4552 4945 533a 0d0a 2020 2020  S_QUERIES:..    
-00006fe0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00006ff0: 666c 6167 735b 2767 6574 5f66 6565 6462  flags['get_feedb
-00007000: 6163 6b27 5d20 616e 6420 6e6f 7420 7365  ack'] and not se
-00007010: 6c66 2e66 6c61 6773 5b27 7061 7573 655f  lf.flags['pause_
-00007020: 6665 6564 6261 636b 275d 3a0d 0a20 2020  feedback']:..   
-00007030: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007040: 662e 7365 7446 6c61 6728 7061 7573 655f  f.setFlag(pause_
-00007050: 6665 6564 6261 636b 3d54 7275 6529 0d0a  feedback=True)..
-00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007070: 7469 6d65 2e73 6c65 6570 2874 696d 656f  time.sleep(timeo
-00007080: 7574 5f73 290d 0a20 2020 2020 2020 2020  ut_s)..         
-00007090: 2020 2023 2073 656c 662e 6765 7453 7461     # self.getSta
-000070a0: 7475 7328 290d 0a20 2020 2020 2020 2020  tus()..         
-000070b0: 2020 2023 2077 6869 6c65 2073 656c 662e     # while self.
-000070c0: 6973 4275 7379 2829 3a0d 0a20 2020 2020  isBusy():..     
-000070d0: 2020 2020 2020 2023 2020 2020 2073 656c         #     sel
-000070e0: 662e 6765 7453 7461 7475 7328 290d 0a20  f.getStatus().. 
-000070f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00007100: 6c66 2e69 7342 7573 7928 293a 0d0a 2020  lf.isBusy():..  
-00007110: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00007120: 6d65 2e73 6c65 6570 2874 696d 656f 7574  me.sleep(timeout
-00007130: 5f73 290d 0a20 2020 2020 2020 200d 0a20  _s)..        .. 
-00007140: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
-00007150: 6520 3d20 7469 6d65 2e70 6572 665f 636f  e = time.perf_co
-00007160: 756e 7465 7228 290d 0a20 2020 2020 2020  unter()..       
-00007170: 2073 656c 662e 5f77 7269 7465 2863 6f6d   self._write(com
-00007180: 6d61 6e64 290d 0a20 2020 2020 2020 2072  mand)..        r
-00007190: 6573 706f 6e73 6520 3d20 2727 0d0a 2020  esponse = ''..  
-000071a0: 2020 2020 2020 7768 696c 6520 6e6f 7420        while not 
-000071b0: 7365 6c66 2e5f 6973 5f65 7870 6563 7465  self._is_expecte
-000071c0: 645f 7265 706c 7928 7265 7370 6f6e 7365  d_reply(response
-000071d0: 2c20 636f 6d6d 616e 645f 636f 6465 293a  , command_code):
-000071e0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000071f0: 2074 696d 652e 7065 7266 5f63 6f75 6e74   time.perf_count
-00007200: 6572 2829 202d 2073 7461 7274 5f74 696d  er() - start_tim
-00007210: 6520 3e20 7469 6d65 6f75 745f 733a 0d0a  e > timeout_s:..
-00007220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007230: 6272 6561 6b0d 0a20 2020 2020 2020 2020  break..         
-00007240: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-00007250: 6c66 2e5f 7265 6164 2829 0d0a 2020 2020  lf._read()..    
-00007260: 2020 2020 2320 7072 696e 7428 7469 6d65      # print(time
-00007270: 2e70 6572 665f 636f 756e 7465 7228 2920  .perf_counter() 
-00007280: 2d20 7374 6172 745f 7469 6d65 290d 0a20  - start_time).. 
-00007290: 2020 2020 2020 2069 6620 636f 6d6d 616e         if comman
-000072a0: 645f 636f 6465 2069 6e20 5155 4552 4945  d_code in QUERIE
-000072b0: 533a 0d0a 2020 2020 2020 2020 2020 2020  S:..            
-000072c0: 7265 7370 6f6e 7365 203d 2072 6573 706f  response = respo
-000072d0: 6e73 655b 323a 5d0d 0a20 2020 2020 2020  nse[2:]..       
-000072e0: 2069 6620 636f 6d6d 616e 645f 636f 6465   if command_code
-000072f0: 206e 6f74 2069 6e20 5354 4154 5553 5f51   not in STATUS_Q
-00007300: 5545 5249 4553 3a0d 0a20 2020 2020 2020  UERIES:..       
-00007310: 2020 2020 2069 6620 6765 745f 706f 7369       if get_posi
-00007320: 7469 6f6e 3a0d 0a20 2020 2020 2020 2020  tion:..         
-00007330: 2020 2020 2020 2073 656c 662e 6765 7450         self.getP
-00007340: 6f73 6974 696f 6e28 290d 0a20 2020 2020  osition()..     
-00007350: 2020 2020 2020 2069 6620 7265 7375 6d65         if resume
-00007360: 5f66 6565 6462 6163 6b3a 0d0a 2020 2020  _feedback:..    
-00007370: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00007380: 2e73 6574 466c 6167 2870 6175 7365 5f66  .setFlag(pause_f
-00007390: 6565 6462 6163 6b3d 4661 6c73 6529 0d0a  eedback=False)..
-000073a0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000073b0: 6573 706f 6e73 650d 0a0d 0a20 2020 2064  esponse....    d
-000073c0: 6566 205f 7265 6164 2873 656c 6629 202d  ef _read(self) -
-000073d0: 3e20 7374 723a 0d0a 2020 2020 2020 2020  > str:..        
-000073e0: 2222 220d 0a20 2020 2020 2020 2052 6561  """..        Rea
-000073f0: 6420 7265 7370 6f6e 7365 2066 726f 6d20  d response from 
-00007400: 6465 7669 6365 0d0a 0d0a 2020 2020 2020  device....      
-00007410: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
-00007420: 2020 2020 2020 2020 7374 723a 2072 6573          str: res
-00007430: 706f 6e73 6520 7374 7269 6e67 0d0a 2020  ponse string..  
+00000200: 726f 6d20 2e20 696d 706f 7274 2073 6172  rom . import sar
+00000210: 746f 7269 7573 5f6c 6962 2061 7320 6c69  torius_lib as li
+00000220: 620d 0a70 7269 6e74 2866 2249 6d70 6f72  b..print(f"Impor
+00000230: 743a 204f 4b20 3c7b 5f5f 6e61 6d65 5f5f  t: OK <{__name__
+00000240: 7d3e 2229 0d0a 0d0a 5155 4552 4945 5320  }>")....QUERIES 
+00000250: 3d20 6c69 622e 5374 6174 7573 5175 6572  = lib.StatusQuer
+00000260: 7943 6f64 652e 5f6d 656d 6265 725f 6e61  yCode._member_na
+00000270: 6d65 735f 202b 206c 6962 2e53 7461 7469  mes_ + lib.Stati
+00000280: 6351 7565 7279 436f 6465 2e5f 6d65 6d62  cQueryCode._memb
+00000290: 6572 5f6e 616d 6573 5f0d 0a22 2222 4c69  er_names_.."""Li
+000002a0: 7374 206f 6620 616c 6c20 7175 6572 7920  st of all query 
+000002b0: 636f 6465 7322 2222 0d0a 5354 4550 5f52  codes"""..STEP_R
+000002c0: 4553 4f4c 5554 494f 4e20 3d20 3130 0d0a  ESOLUTION = 10..
+000002d0: 2222 224d 696e 696d 756d 206e 756d 6265  """Minimum numbe
+000002e0: 7220 6f66 2073 7465 7073 2074 6f20 6861  r of steps to ha
+000002f0: 7665 2074 6f6c 6572 6162 6c65 2065 7272  ve tolerable err
+00000300: 6f72 7320 696e 2076 6f6c 756d 6522 2222  ors in volume"""
+00000310: 0d0a 0d0a 636c 6173 7320 5361 7274 6f72  ....class Sartor
+00000320: 6975 7328 4c69 7175 6964 4861 6e64 6c65  ius(LiquidHandle
+00000330: 7229 3a0d 0a20 2020 2022 2222 0d0a 2020  r):..    """..  
+00000340: 2020 5361 7274 6f72 6975 7320 6f62 6a65    Sartorius obje
+00000350: 6374 0d0a 0d0a 2020 2020 2323 2320 436f  ct....    ### Co
+00000360: 6e73 7472 7563 746f 720d 0a20 2020 2041  nstructor..    A
+00000370: 7267 733a 0d0a 2020 2020 2020 2020 6070  rgs:..        `p
+00000380: 6f72 7460 2028 7374 7229 3a20 434f 4d20  ort` (str): COM 
+00000390: 706f 7274 2061 6464 7265 7373 0d0a 2020  port address..  
+000003a0: 2020 2020 2020 6063 6861 6e6e 656c 6020        `channel` 
+000003b0: 2869 6e74 2c20 6f70 7469 6f6e 616c 293a  (int, optional):
+000003c0: 2063 6861 6e6e 656c 2069 642e 2044 6566   channel id. Def
+000003d0: 6175 6c74 7320 746f 2031 2e0d 0a20 2020  aults to 1...   
+000003e0: 2020 2020 2060 6f66 6673 6574 6020 2874       `offset` (t
+000003f0: 7570 6c65 5b66 6c6f 6174 5d2c 206f 7074  uple[float], opt
+00000400: 696f 6e61 6c29 3a20 782c 792c 7a20 6f66  ional): x,y,z of
+00000410: 6673 6574 206f 6620 7469 702e 2044 6566  fset of tip. Def
+00000420: 6175 6c74 7320 746f 2028 302c 302c 3029  aults to (0,0,0)
+00000430: 2e0d 0a20 2020 2020 2020 2060 7265 7370  ...        `resp
+00000440: 6f6e 7365 5f74 696d 6560 2028 666c 6f61  onse_time` (floa
+00000450: 742c 206f 7074 696f 6e61 6c29 3a20 6465  t, optional): de
+00000460: 6c61 7920 6265 7477 6565 6e20 7365 6e64  lay between send
+00000470: 696e 6720 6120 636f 6d6d 616e 6420 616e  ing a command an
+00000480: 6420 7265 6365 6976 696e 6720 6120 7265  d receiving a re
+00000490: 7370 6f6e 7365 2c20 696e 2073 6563 6f6e  sponse, in secon
+000004a0: 6473 2e20 4465 6661 756c 7473 2074 6f20  ds. Defaults to 
+000004b0: 312e 3033 2e0d 0a20 2020 2020 2020 2060  1.03...        `
+000004c0: 7469 705f 7468 7265 7368 6f6c 6460 2028  tip_threshold` (
+000004d0: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
+000004e0: 7468 7265 7368 6f6c 6420 6162 6f76 6520  threshold above 
+000004f0: 7768 6963 6820 6120 636f 6e64 7563 7469  which a conducti
+00000500: 7665 2070 6970 6574 7465 2074 6970 2069  ve pipette tip i
+00000510: 7320 636f 6e73 6964 6572 6564 2074 6f20  s considered to 
+00000520: 6265 2061 7474 6163 6865 642e 2044 6566  be attached. Def
+00000530: 6175 6c74 7320 746f 2032 3736 2e0d 0a20  aults to 276... 
+00000540: 2020 200d 0a20 2020 2023 2323 2041 7474     ..    ### Att
+00000550: 7269 6275 7465 730d 0a20 2020 202d 2060  ributes..    - `
+00000560: 6368 616e 6e65 6c60 2028 696e 7429 3a20  channel` (int): 
+00000570: 6368 616e 6e65 6c20 6964 0d0a 2020 2020  channel id..    
+00000580: 2d20 606c 696d 6974 7360 2028 7475 706c  - `limits` (tupl
+00000590: 655b 696e 745d 293a 206c 6f77 6572 2061  e[int]): lower a
+000005a0: 6e64 2075 7070 6572 2073 7465 7020 6c69  nd upper step li
+000005b0: 6d69 7473 0d0a 2020 2020 2d20 606d 6f64  mits..    - `mod
+000005c0: 656c 5f69 6e66 6f60 2028 5361 7274 6f72  el_info` (Sartor
+000005d0: 6975 7350 6970 6574 7465 4d6f 6465 6c29  iusPipetteModel)
+000005e0: 3a20 5361 7274 6f72 6975 7320 6d6f 6465  : Sartorius mode
+000005f0: 6c20 696e 666f 0d0a 2020 2020 2d20 606f  l info..    - `o
+00000600: 6666 7365 7460 2028 7475 706c 655b 666c  ffset` (tuple[fl
+00000610: 6f61 745d 293a 2078 2c79 2c7a 206f 6666  oat]): x,y,z off
+00000620: 7365 7420 6f66 2074 6970 0d0a 2020 2020  set of tip..    
+00000630: 2d20 6070 6f73 6974 696f 6e60 2028 696e  - `position` (in
+00000640: 7429 3a20 706f 7369 7469 6f6e 206f 6620  t): position of 
+00000650: 706c 756e 6765 720d 0a20 2020 202d 2060  plunger..    - `
+00000660: 7265 7370 6f6e 7365 5f74 696d 6560 2028  response_time` (
+00000670: 666c 6f61 7429 3a20 6465 6c61 7920 6265  float): delay be
+00000680: 7477 6565 6e20 7365 6e64 696e 6720 6120  tween sending a 
+00000690: 636f 6d6d 616e 6420 616e 6420 7265 6365  command and rece
+000006a0: 6976 696e 6720 6120 7265 7370 6f6e 7365  iving a response
+000006b0: 2c20 696e 2073 6563 6f6e 6473 0d0a 2020  , in seconds..  
+000006c0: 2020 2d20 6073 7065 6564 5f63 6f64 6560    - `speed_code`
+000006d0: 2028 5370 6565 6429 3a20 636f 6465 7320   (Speed): codes 
+000006e0: 666f 7220 6173 7069 7261 7465 2061 6e64  for aspirate and
+000006f0: 2064 6973 7065 6e73 6520 7370 6565 6473   dispense speeds
+00000700: 0d0a 2020 2020 2d20 6073 7065 6564 5f70  ..    - `speed_p
+00000710: 7265 7365 7473 6020 2850 7265 7365 7453  resets` (PresetS
+00000720: 7065 6564 7329 3a20 7072 6573 6574 2073  peeds): preset s
+00000730: 7065 6564 7320 6176 6169 6c61 626c 650d  peeds available.
+00000740: 0a20 2020 202d 2060 7469 705f 6c65 6e67  .    - `tip_leng
+00000750: 7468 6020 2866 6c6f 6174 293a 206c 656e  th` (float): len
+00000760: 6774 6820 6f66 2070 6970 6574 7465 2074  gth of pipette t
+00000770: 6970 0d0a 2020 2020 2d20 6074 6970 5f74  ip..    - `tip_t
+00000780: 6872 6573 686f 6c64 6020 2869 6e74 293a  hreshold` (int):
+00000790: 2074 6872 6573 686f 6c64 2061 626f 7665   threshold above
+000007a0: 2077 6869 6368 2061 2063 6f6e 6475 6374   which a conduct
+000007b0: 6976 6520 7069 7065 7474 6520 7469 7020  ive pipette tip 
+000007c0: 6973 2063 6f6e 7369 6465 7265 6420 746f  is considered to
+000007d0: 2062 6520 6174 7461 6368 6564 0d0a 2020   be attached..  
+000007e0: 2020 0d0a 2020 2020 2323 2320 5072 6f70    ..    ### Prop
+000007f0: 6572 7469 6573 0d0a 2020 2020 2d20 6063  erties..    - `c
+00000800: 6170 6163 6974 616e 6365 6020 2869 6e74  apacitance` (int
+00000810: 293a 2063 6170 6163 6974 616e 6365 2061  ): capacitance a
+00000820: 7320 6d65 6173 7572 6564 2061 7420 7468  s measured at th
+00000830: 6520 656e 6420 6f66 2074 6865 2070 6970  e end of the pip
+00000840: 6574 7465 0d0a 2020 2020 2d20 6068 6f6d  ette..    - `hom
+00000850: 655f 706f 7369 7469 6f6e 6020 2869 6e74  e_position` (int
+00000860: 293a 2068 6f6d 6520 706f 7369 7469 6f6e  ): home position
+00000870: 206f 6620 7069 7065 7474 650d 0a20 2020   of pipette..   
+00000880: 202d 2060 706f 7274 6020 2873 7472 293a   - `port` (str):
+00000890: 2043 4f4d 2070 6f72 7420 6164 6472 6573   COM port addres
+000008a0: 730d 0a20 2020 202d 2060 7265 736f 6c75  s..    - `resolu
+000008b0: 7469 6f6e 6020 2866 6c6f 6174 293a 2076  tion` (float): v
+000008c0: 6f6c 756d 6520 7265 736f 6c75 7469 6f6e  olume resolution
+000008d0: 206f 6620 7069 7065 7474 6520 2869 2e65   of pipette (i.e
+000008e0: 2e20 754c 2070 6572 2073 7465 7029 0d0a  . uL per step)..
+000008f0: 2020 2020 2d20 6073 7461 7475 7360 2028      - `status` (
+00000900: 7374 7229 3a20 7069 7065 7474 6520 7374  str): pipette st
+00000910: 6174 7573 0d0a 2020 2020 0d0a 2020 2020  atus..    ..    
+00000920: 2323 2320 4d65 7468 6f64 730d 0a20 2020  ### Methods..   
+00000930: 202d 2060 6164 6441 6972 4761 7060 3a20   - `addAirGap`: 
+00000940: 6372 6561 7465 2061 6e20 6169 7220 6761  create an air ga
+00000950: 7020 6265 7477 6565 6e20 7477 6f20 766f  p between two vo
+00000960: 6c75 6d65 7320 6f66 206c 6971 7569 6420  lumes of liquid 
+00000970: 696e 2070 6970 6574 7465 0d0a 2020 2020  in pipette..    
+00000980: 2d20 6061 7370 6972 6174 6560 3a20 6173  - `aspirate`: as
+00000990: 7069 7261 7465 2064 6573 6972 6564 2076  pirate desired v
+000009a0: 6f6c 756d 6520 6f66 2072 6561 6765 6e74  olume of reagent
+000009b0: 2069 6e74 6f20 7069 7065 7474 650d 0a20   into pipette.. 
+000009c0: 2020 202d 2060 626c 6f77 6f75 7460 3a20     - `blowout`: 
+000009d0: 626c 6f77 6f75 7420 6c69 7175 6964 2066  blowout liquid f
+000009e0: 726f 6d20 7469 700d 0a20 2020 202d 2060  rom tip..    - `
+000009f0: 6469 7370 656e 7365 603a 2064 6973 7065  dispense`: dispe
+00000a00: 6e73 6520 6465 7369 7265 6420 766f 6c75  nse desired volu
+00000a10: 6d65 206f 6620 7265 6167 656e 740d 0a20  me of reagent.. 
+00000a20: 2020 202d 2060 656a 6563 7460 3a20 656a     - `eject`: ej
+00000a30: 6563 7420 7468 6520 7069 7065 7474 6520  ect the pipette 
+00000a40: 7469 700d 0a20 2020 202d 2060 656d 7074  tip..    - `empt
+00000a50: 7960 3a20 656d 7074 7920 7468 6520 7069  y`: empty the pi
+00000a60: 7065 7474 650d 0a20 2020 202d 2060 6765  pette..    - `ge
+00000a70: 7443 6170 6163 6974 616e 6365 603a 2067  tCapacitance`: g
+00000a80: 6574 2074 6865 2063 6170 6163 6974 616e  et the capacitan
+00000a90: 6365 2061 7320 6d65 6173 7572 6564 2061  ce as measured a
+00000aa0: 7420 7468 6520 656e 6420 6f66 2074 6865  t the end of the
+00000ab0: 2070 6970 6574 7465 0d0a 2020 2020 2d20   pipette..    - 
+00000ac0: 6067 6574 4572 726f 7273 603a 2067 6574  `getErrors`: get
+00000ad0: 2065 7272 6f72 7320 6672 6f6d 2074 6865   errors from the
+00000ae0: 2064 6576 6963 650d 0a20 2020 202d 2060   device..    - `
+00000af0: 6765 7449 6e66 6f60 3a20 6765 7420 6465  getInfo`: get de
+00000b00: 7461 696c 7320 6f66 2074 6865 2053 6172  tails of the Sar
+00000b10: 746f 7269 7573 2070 6970 6574 7465 206d  torius pipette m
+00000b20: 6f64 656c 0d0a 2020 2020 2d20 6067 6574  odel..    - `get
+00000b30: 506f 7369 7469 6f6e 603a 2067 6574 2074  Position`: get t
+00000b40: 6865 2063 7572 7265 6e74 2070 6f73 6974  he current posit
+00000b50: 696f 6e20 6f66 2074 6865 2070 6970 6574  ion of the pipet
+00000b60: 7465 0d0a 2020 2020 2d20 6067 6574 5374  te..    - `getSt
+00000b70: 6174 7573 603a 2067 6574 2074 6865 2073  atus`: get the s
+00000b80: 7461 7475 7320 6f66 2074 6865 2070 6970  tatus of the pip
+00000b90: 6574 7465 0d0a 2020 2020 2d20 6068 6f6d  ette..    - `hom
+00000ba0: 6560 3a20 7265 7475 726e 2070 6c75 6e67  e`: return plung
+00000bb0: 6572 2074 6f20 686f 6d65 2070 6f73 6974  er to home posit
+00000bc0: 696f 6e0d 0a20 2020 202d 2060 6973 4665  ion..    - `isFe
+00000bd0: 6173 6962 6c65 603a 2063 6865 636b 7320  asible`: checks 
+00000be0: 616e 6420 7265 7475 726e 7320 7768 6574  and returns whet
+00000bf0: 6865 7220 7468 6520 706c 756e 6765 7220  her the plunger 
+00000c00: 706f 7369 7469 6f6e 2069 7320 6665 6173  position is feas
+00000c10: 6962 6c65 0d0a 2020 2020 2d20 6069 7354  ible..    - `isT
+00000c20: 6970 4f6e 603a 2063 6865 636b 7320 616e  ipOn`: checks an
+00000c30: 6420 7265 7475 726e 7320 7768 6574 6865  d returns whethe
+00000c40: 7220 6120 7069 7065 7474 6520 7469 7020  r a pipette tip 
+00000c50: 6973 2061 7474 6163 6865 640d 0a20 2020  is attached..   
+00000c60: 202d 2060 6d6f 7665 603a 206d 6f76 6520   - `move`: move 
+00000c70: 7468 6520 706c 756e 6765 7220 6569 7468  the plunger eith
+00000c80: 6572 2075 7020 6f72 2064 6f77 6e20 6279  er up or down by
+00000c90: 2061 2073 7065 6369 6669 6564 206e 756d   a specified num
+00000ca0: 6265 7220 6f66 2073 7465 7073 0d0a 2020  ber of steps..  
+00000cb0: 2020 2d20 606d 6f76 6542 7960 3a20 6d6f    - `moveBy`: mo
+00000cc0: 7665 2074 6865 2070 6c75 6e67 6572 2062  ve the plunger b
+00000cd0: 7920 6120 7370 6563 6966 6965 6420 6e75  y a specified nu
+00000ce0: 6d62 6572 206f 6620 7374 6570 730d 0a20  mber of steps.. 
+00000cf0: 2020 202d 2060 6d6f 7665 546f 603a 206d     - `moveTo`: m
+00000d00: 6f76 6520 7468 6520 706c 756e 6765 7220  ove the plunger 
+00000d10: 746f 2061 2073 7065 6369 6669 6564 2070  to a specified p
+00000d20: 6f73 6974 696f 6e0d 0a20 2020 202d 2060  osition..    - `
+00000d30: 7075 6c6c 6261 636b 603a 2070 756c 6c62  pullback`: pullb
+00000d40: 6163 6b20 6c69 7175 6964 2066 726f 6d20  ack liquid from 
+00000d50: 7469 700d 0a20 2020 202d 2060 7265 7365  tip..    - `rese
+00000d60: 7460 3a20 7265 7365 7420 7468 6520 7069  t`: reset the pi
+00000d70: 7065 7474 650d 0a20 2020 202d 2060 7365  pette..    - `se
+00000d80: 7453 7065 6564 603a 2073 6574 2074 6865  tSpeed`: set the
+00000d90: 2073 7065 6564 206f 6620 7468 6520 706c   speed of the pl
+00000da0: 756e 6765 720d 0a20 2020 202d 2060 7368  unger..    - `sh
+00000db0: 7574 646f 776e 603a 2073 6875 7464 6f77  utdown`: shutdow
+00000dc0: 6e20 7072 6f63 6564 7572 6520 666f 7220  n procedure for 
+00000dd0: 746f 6f6c 0d0a 2020 2020 2d20 6074 6f67  tool..    - `tog
+00000de0: 676c 6546 6565 6462 6163 6b4c 6f6f 7060  gleFeedbackLoop`
+00000df0: 3a20 7374 6172 7420 6f72 2073 746f 7020  : start or stop 
+00000e00: 6665 6564 6261 636b 206c 6f6f 700d 0a20  feedback loop.. 
+00000e10: 2020 202d 2060 7a65 726f 603a 207a 6572     - `zero`: zer
+00000e20: 6f20 7468 6520 706c 756e 6765 7220 706f  o the plunger po
+00000e30: 7369 7469 6f6e 0d0a 2020 2020 2222 220d  sition..    """.
+00000e40: 0a20 2020 200d 0a20 2020 205f 6465 6661  .    ..    _defa
+00000e50: 756c 745f 666c 6167 7320 3d20 7b0d 0a20  ult_flags = {.. 
+00000e60: 2020 2020 2020 2027 6275 7379 273a 2046         'busy': F
+00000e70: 616c 7365 2c0d 0a20 2020 2020 2020 2027  alse,..        '
+00000e80: 636f 6e64 7563 7469 7665 5f74 6970 7327  conductive_tips'
+00000e90: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
+00000ea0: 2020 2763 6f6e 6e65 6374 6564 273a 2046    'connected': F
+00000eb0: 616c 7365 2c0d 0a20 2020 2020 2020 2027  alse,..        '
+00000ec0: 6765 745f 6665 6564 6261 636b 273a 2046  get_feedback': F
+00000ed0: 616c 7365 2c0d 0a20 2020 2020 2020 2027  alse,..        '
+00000ee0: 6f63 6375 7069 6564 273a 2046 616c 7365  occupied': False
+00000ef0: 2c0d 0a20 2020 2020 2020 2027 7061 7573  ,..        'paus
+00000f00: 655f 6665 6564 6261 636b 273a 4661 6c73  e_feedback':Fals
+00000f10: 652c 0d0a 2020 2020 2020 2020 2774 6970  e,..        'tip
+00000f20: 5f6f 6e27 3a20 4661 6c73 650d 0a20 2020  _on': False..   
+00000f30: 207d 0d0a 2020 2020 696d 706c 656d 656e   }..    implemen
+00000f40: 745f 6f66 6673 6574 203d 2028 302c 302c  t_offset = (0,0,
+00000f50: 2d32 3530 290d 0a20 2020 2074 6970 5f69  -250)..    tip_i
+00000f60: 6e73 6574 5f6d 6d20 3d20 3132 0d0a 2020  nset_mm = 12..  
+00000f70: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00000f80: 656c 662c 200d 0a20 2020 2020 2020 2070  elf, ..        p
+00000f90: 6f72 743a 7374 722c 200d 0a20 2020 2020  ort:str, ..     
+00000fa0: 2020 2063 6861 6e6e 656c 3a20 696e 7420     channel: int 
+00000fb0: 3d20 312c 200d 0a20 2020 2020 2020 206f  = 1, ..        o
+00000fc0: 6666 7365 743a 2074 7570 6c65 5b66 6c6f  ffset: tuple[flo
+00000fd0: 6174 5d20 3d20 2830 2c30 2c30 292c 0d0a  at] = (0,0,0),..
+00000fe0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00000ff0: 5f74 696d 653a 2066 6c6f 6174 203d 2031  _time: float = 1
+00001000: 2e30 332c 0d0a 2020 2020 2020 2020 7469  .03,..        ti
+00001010: 705f 7468 7265 7368 6f6c 643a 2069 6e74  p_threshold: int
+00001020: 203d 2032 3736 2c0d 0a20 2020 2020 2020   = 276,..       
+00001030: 202a 2a6b 7761 7267 730d 0a20 2020 2029   **kwargs..    )
+00001040: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00001050: 2020 2020 2020 2020 496e 7374 616e 7469          Instanti
+00001060: 6174 6520 7468 6520 636c 6173 730d 0a0d  ate the class...
+00001070: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+00001080: 2020 2020 2020 2020 2020 2020 706f 7274              port
+00001090: 2028 7374 7229 3a20 434f 4d20 706f 7274   (str): COM port
+000010a0: 2061 6464 7265 7373 0d0a 2020 2020 2020   address..      
+000010b0: 2020 2020 2020 6368 616e 6e65 6c20 2869        channel (i
+000010c0: 6e74 2c20 6f70 7469 6f6e 616c 293a 2063  nt, optional): c
+000010d0: 6861 6e6e 656c 2069 642e 2044 6566 6175  hannel id. Defau
+000010e0: 6c74 7320 746f 2031 2e0d 0a20 2020 2020  lts to 1...     
+000010f0: 2020 2020 2020 206f 6666 7365 7420 2874         offset (t
+00001100: 7570 6c65 5b66 6c6f 6174 5d2c 206f 7074  uple[float], opt
+00001110: 696f 6e61 6c29 3a20 782c 792c 7a20 6f66  ional): x,y,z of
+00001120: 6673 6574 206f 6620 7469 702e 2044 6566  fset of tip. Def
+00001130: 6175 6c74 7320 746f 2028 302c 302c 3029  aults to (0,0,0)
+00001140: 2e0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
+00001150: 6573 706f 6e73 655f 7469 6d65 2028 666c  esponse_time (fl
+00001160: 6f61 742c 206f 7074 696f 6e61 6c29 3a20  oat, optional): 
+00001170: 6465 6c61 7920 6265 7477 6565 6e20 7365  delay between se
+00001180: 6e64 696e 6720 6120 636f 6d6d 616e 6420  nding a command 
+00001190: 616e 6420 7265 6365 6976 696e 6720 6120  and receiving a 
+000011a0: 7265 7370 6f6e 7365 2c20 696e 2073 6563  response, in sec
+000011b0: 6f6e 6473 2e20 4465 6661 756c 7473 2074  onds. Defaults t
+000011c0: 6f20 312e 3033 2e0d 0a20 2020 2020 2020  o 1.03...       
+000011d0: 2020 2020 2074 6970 5f74 6872 6573 686f       tip_thresho
+000011e0: 6c64 2028 696e 742c 206f 7074 696f 6e61  ld (int, optiona
+000011f0: 6c29 3a20 7468 7265 7368 6f6c 6420 6162  l): threshold ab
+00001200: 6f76 6520 7768 6963 6820 6120 636f 6e64  ove which a cond
+00001210: 7563 7469 7665 2070 6970 6574 7465 2074  uctive pipette t
+00001220: 6970 2069 7320 636f 6e73 6964 6572 6564  ip is considered
+00001230: 2074 6f20 6265 2061 7474 6163 6865 642e   to be attached.
+00001240: 2044 6566 6175 6c74 7320 746f 2032 3736   Defaults to 276
+00001250: 2e0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00001260: 2020 2020 2020 2020 7375 7065 7228 292e          super().
+00001270: 5f5f 696e 6974 5f5f 282a 2a6b 7761 7267  __init__(**kwarg
+00001280: 7329 0d0a 2020 2020 2020 2020 7365 6c66  s)..        self
+00001290: 2e63 6861 6e6e 656c 203d 2063 6861 6e6e  .channel = chann
+000012a0: 656c 0d0a 2020 2020 2020 2020 7365 6c66  el..        self
+000012b0: 2e6f 6666 7365 7420 3d20 6f66 6673 6574  .offset = offset
+000012c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
+000012d0: 6573 706f 6e73 655f 7469 6d65 203d 2072  esponse_time = r
+000012e0: 6573 706f 6e73 655f 7469 6d65 0d0a 2020  esponse_time..  
+000012f0: 2020 2020 2020 7365 6c66 2e74 6970 5f74        self.tip_t
+00001300: 6872 6573 686f 6c64 203d 2074 6970 5f74  hreshold = tip_t
+00001310: 6872 6573 686f 6c64 0d0a 2020 2020 2020  hreshold..      
+00001320: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+00001330: 2e6d 6f64 656c 5f69 6e66 6f3a 206c 6962  .model_info: lib
+00001340: 2e4d 6f64 656c 203d 204e 6f6e 650d 0a20  .Model = None.. 
+00001350: 2020 2020 2020 2073 656c 662e 6c69 6d69         self.limi
+00001360: 7473 203d 2028 302c 3029 0d0a 2020 2020  ts = (0,0)..    
+00001370: 2020 2020 7365 6c66 2e70 6f73 6974 696f      self.positio
+00001380: 6e20 3d20 300d 0a20 2020 2020 2020 2073  n = 0..        s
+00001390: 656c 662e 7370 6565 645f 636f 6465 203d  elf.speed_code =
+000013a0: 2053 7065 6564 2833 2c33 290d 0a20 2020   Speed(3,3)..   
+000013b0: 2020 2020 2073 656c 662e 7370 6565 645f       self.speed_
+000013c0: 7072 6573 6574 7320 3d20 4e6f 6e65 0d0a  presets = None..
+000013d0: 2020 2020 2020 2020 7365 6c66 2e74 6970          self.tip
+000013e0: 5f6c 656e 6774 6820 3d20 300d 0a20 2020  _length = 0..   
+000013f0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+00001400: 656c 662e 5f63 6170 6163 6974 616e 6365  elf._capacitance
+00001410: 203d 2030 0d0a 2020 2020 2020 2020 7365   = 0..        se
+00001420: 6c66 2e5f 7374 6174 7573 5f63 6f64 6520  lf._status_code 
+00001430: 3d20 2727 0d0a 2020 2020 2020 2020 7365  = ''..        se
+00001440: 6c66 2e5f 7468 7265 6164 7320 3d20 7b7d  lf._threads = {}
+00001450: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00001460: 2020 2020 7072 696e 7428 2241 6e79 2061      print("Any a
+00001470: 7474 6163 6865 6420 7069 7065 7474 6520  ttached pipette 
+00001480: 7469 7020 6d61 7920 6472 6f70 2064 7572  tip may drop dur
+00001490: 696e 6720 696e 6974 6961 6c69 7361 7469  ing initialisati
+000014a0: 6f6e 2e22 290d 0a20 2020 2020 2020 2073  on.")..        s
+000014b0: 656c 662e 5f63 6f6e 6e65 6374 2870 6f72  elf._connect(por
+000014c0: 7429 0d0a 2020 2020 2020 2020 7265 7475  t)..        retu
+000014d0: 726e 0d0a 2020 2020 0d0a 2020 2020 2320  rn..    ..    # 
+000014e0: 5072 6f70 6572 7469 6573 0d0a 2020 2020  Properties..    
+000014f0: 4070 726f 7065 7274 790d 0a20 2020 2064  @property..    d
+00001500: 6566 2063 6170 6163 6974 616e 6365 2873  ef capacitance(s
+00001510: 656c 6629 202d 3e20 696e 743a 0d0a 2020  elf) -> int:..  
+00001520: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00001530: 662e 5f63 6170 6163 6974 616e 6365 0d0a  f._capacitance..
+00001540: 2020 2020 2020 2020 0d0a 2020 2020 4070          ..    @p
+00001550: 726f 7065 7274 790d 0a20 2020 2064 6566  roperty..    def
+00001560: 2068 6f6d 655f 706f 7369 7469 6f6e 2873   home_position(s
+00001570: 656c 6629 202d 3e20 696e 743a 0d0a 2020  elf) -> int:..  
+00001580: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00001590: 662e 6d6f 6465 6c5f 696e 666f 2e68 6f6d  f.model_info.hom
+000015a0: 655f 706f 7369 7469 6f6e 0d0a 2020 2020  e_position..    
+000015b0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+000015c0: 0a20 2020 2064 6566 2070 6f72 7428 7365  .    def port(se
+000015d0: 6c66 2920 2d3e 2073 7472 3a0d 0a20 2020  lf) -> str:..   
+000015e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+000015f0: 2e63 6f6e 6e65 6374 696f 6e5f 6465 7461  .connection_deta
+00001600: 696c 732e 6765 7428 2770 6f72 7427 2c20  ils.get('port', 
+00001610: 2727 290d 0a20 2020 200d 0a20 2020 2040  '')..    ..    @
+00001620: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00001630: 6620 7265 736f 6c75 7469 6f6e 2873 656c  f resolution(sel
+00001640: 6629 202d 3e20 666c 6f61 743a 0d0a 2020  f) -> float:..  
+00001650: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00001660: 662e 6d6f 6465 6c5f 696e 666f 2e72 6573  f.model_info.res
+00001670: 6f6c 7574 696f 6e0d 0a20 2020 200d 0a20  olution..    .. 
+00001680: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
+00001690: 2020 6465 6620 7374 6174 7573 2873 656c    def status(sel
+000016a0: 6629 202d 3e20 7374 723a 0d0a 2020 2020  f) -> str:..    
+000016b0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000016c0: 6765 7453 7461 7475 7328 290d 0a20 2020  getStatus()..   
+000016d0: 200d 0a20 2020 2064 6566 205f 5f63 7963   ..    def __cyc
+000016e0: 6c65 735f 5f28 7365 6c66 2920 2d3e 2055  les__(self) -> U
+000016f0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 3a0d  nion[int, str]:.
+00001700: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00001710: 2020 2020 2020 5265 7472 6965 7665 2074        Retrieve t
+00001720: 6f74 616c 2063 7963 6c65 206c 6966 6574  otal cycle lifet
+00001730: 696d 650d 0a0d 0a20 2020 2020 2020 2052  ime....        R
+00001740: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+00001750: 2020 2020 2055 6e69 6f6e 5b69 6e74 2c20       Union[int, 
+00001760: 7374 725d 3a20 6e75 6d62 6572 206f 6620  str]: number of 
+00001770: 6c69 6665 7469 6d65 2063 7963 6c65 732c  lifetime cycles,
+00001780: 206f 7220 7265 7370 6f6e 7365 2073 7472   or response str
+00001790: 696e 670d 0a20 2020 2020 2020 2022 2222  ing..        """
+000017a0: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
+000017b0: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
+000017c0: 2827 4458 2729 0d0a 2020 2020 2020 2020  ('DX')..        
+000017d0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000017e0: 2020 6379 636c 6573 203d 2069 6e74 2872    cycles = int(r
+000017f0: 6573 706f 6e73 6529 0d0a 2020 2020 2020  esponse)..      
+00001800: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
+00001810: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
+00001820: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+00001830: 650d 0a20 2020 2020 2020 2070 7269 6e74  e..        print
+00001840: 2866 2754 6f74 616c 2063 7963 6c65 733a  (f'Total cycles:
+00001850: 207b 6379 636c 6573 7d27 290d 0a20 2020   {cycles}')..   
+00001860: 2020 2020 2072 6574 7572 6e20 6379 636c       return cycl
+00001870: 6573 0d0a 2020 2020 0d0a 2020 2020 6465  es..    ..    de
+00001880: 6620 5f5f 6d6f 6465 6c5f 5f28 7365 6c66  f __model__(self
+00001890: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+000018a0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000018b0: 5265 7472 6965 7665 2074 6865 206d 6f64  Retrieve the mod
+000018c0: 656c 206f 6620 7468 6520 6465 7669 6365  el of the device
+000018d0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+000018e0: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
+000018f0: 2020 7374 723a 206d 6f64 656c 206e 616d    str: model nam
+00001900: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
+00001910: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00001920: 203d 2073 656c 662e 5f71 7565 7279 2827   = self._query('
+00001930: 444d 2729 0d0a 2020 2020 2020 2020 7072  DM')..        pr
+00001940: 696e 7428 6627 4d6f 6465 6c3a 207b 7265  int(f'Model: {re
+00001950: 7370 6f6e 7365 7d27 290d 0a20 2020 2020  sponse}')..     
+00001960: 2020 2072 6574 7572 6e20 7265 7370 6f6e     return respon
+00001970: 7365 0d0a 2020 2020 0d0a 2020 2020 6465  se..    ..    de
+00001980: 6620 5f5f 7265 736f 6c75 7469 6f6e 5f5f  f __resolution__
+00001990: 2873 656c 6629 202d 3e20 556e 696f 6e5b  (self) -> Union[
+000019a0: 696e 742c 2073 7472 5d3a 0d0a 2020 2020  int, str]:..    
+000019b0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000019c0: 2052 6574 7269 6576 6520 7468 6520 7265   Retrieve the re
+000019d0: 736f 6c75 7469 6f6e 206f 6620 7468 6520  solution of the 
+000019e0: 6465 7669 6365 0d0a 0d0a 2020 2020 2020  device....      
+000019f0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00001a00: 2020 2020 2020 2020 556e 696f 6e5b 696e          Union[in
+00001a10: 742c 2073 7472 5d3a 2076 6f6c 756d 6520  t, str]: volume 
+00001a20: 7265 736f 6c75 7469 6f6e 206f 6620 6465  resolution of de
+00001a30: 7669 6365 2069 6e20 6e4c 2c20 6f72 2072  vice in nL, or r
+00001a40: 6573 706f 6e73 6520 7374 7269 6e67 0d0a  esponse string..
+00001a50: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00001a60: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+00001a70: 7365 6c66 2e5f 7175 6572 7928 2744 5227  self._query('DR'
+00001a80: 290d 0a20 2020 2020 2020 2074 7279 3a0d  )..        try:.
+00001a90: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00001aa0: 6f6c 7574 696f 6e20 3d20 696e 7428 7265  olution = int(re
+00001ab0: 7370 6f6e 7365 290d 0a20 2020 2020 2020  sponse)..       
+00001ac0: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+00001ad0: 6f72 3a0d 0a20 2020 2020 2020 2020 2020  or:..           
+00001ae0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+00001af0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00001b00: 6627 7b72 6573 6f6c 7574 696f 6e2f 3130  f'{resolution/10
+00001b10: 3030 7d20 754c 202f 2073 7465 7027 290d  00} uL / step').
+00001b20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001b30: 7265 736f 6c75 7469 6f6e 0d0a 2020 2020  resolution..    
+00001b40: 0d0a 2020 2020 6465 6620 5f5f 7665 7273  ..    def __vers
+00001b50: 696f 6e5f 5f28 7365 6c66 2920 2d3e 2073  ion__(self) -> s
+00001b60: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
+00001b70: 0d0a 2020 2020 2020 2020 5265 7472 6965  ..        Retrie
+00001b80: 7665 2074 6865 2073 6f66 7477 6172 6520  ve the software 
+00001b90: 7665 7273 696f 6e20 6f6e 2074 6865 2064  version on the d
+00001ba0: 6576 6963 650d 0a0d 0a20 2020 2020 2020  evice....       
+00001bb0: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+00001bc0: 2020 2020 2020 2073 7472 3a20 6465 7669         str: devi
+00001bd0: 6365 2076 6572 7369 6f6e 0d0a 2020 2020  ce version..    
+00001be0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00001bf0: 2072 6574 7572 6e20 7365 6c66 2e5f 7175   return self._qu
+00001c00: 6572 7928 2744 5627 290d 0a0d 0a20 2020  ery('DV')....   
+00001c10: 2064 6566 2061 6464 4169 7247 6170 2873   def addAirGap(s
+00001c20: 656c 662c 2073 7465 7073 3a69 6e74 203d  elf, steps:int =
+00001c30: 2031 3029 202d 3e20 7374 723a 0d0a 2020   10) -> str:..  
+00001c40: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00001c50: 2020 2043 7265 6174 6520 616e 2061 6972     Create an air
+00001c60: 2067 6170 2062 6574 7765 656e 2074 776f   gap between two
+00001c70: 2076 6f6c 756d 6573 206f 6620 6c69 7175   volumes of liqu
+00001c80: 6964 2069 6e20 7069 7065 7474 650d 0a20  id in pipette.. 
+00001c90: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00001ca0: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00001cb0: 2020 2020 7374 6570 7320 2869 6e74 2c20      steps (int, 
+00001cc0: 6f70 7469 6f6e 616c 293a 206e 756d 6265  optional): numbe
+00001cd0: 7220 6f66 2073 7465 7073 2066 6f72 2061  r of steps for a
+00001ce0: 6972 2067 6170 2e20 4465 6661 756c 7473  ir gap. Defaults
+00001cf0: 2074 6f20 4445 4641 554c 545f 4149 5247   to DEFAULT_AIRG
+00001d00: 4150 2e0d 0a20 2020 2020 2020 2020 2020  AP...           
+00001d10: 2063 6861 6e6e 656c 2028 696e 742c 206f   channel (int, o
+00001d20: 7074 696f 6e61 6c29 3a20 6368 616e 6e65  ptional): channe
+00001d30: 6c20 746f 2061 6464 2061 6972 2067 6170  l to add air gap
+00001d40: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+00001d50: 6e65 2e0d 0a0d 0a20 2020 2020 2020 2052  ne.....        R
+00001d60: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+00001d70: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
+00001d80: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+00001d90: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00001da0: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00001db0: 5f71 7565 7279 2866 2752 497b 7374 6570  _query(f'RI{step
+00001dc0: 737d 2729 0d0a 2020 2020 2020 2020 7469  s}')..        ti
+00001dd0: 6d65 2e73 6c65 6570 2831 290d 0a20 2020  me.sleep(1)..   
+00001de0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+00001df0: 6f6e 7365 0d0a 2020 2020 2020 2020 0d0a  onse..        ..
+00001e00: 2020 2020 6465 6620 6173 7069 7261 7465      def aspirate
+00001e10: 2873 656c 662c 200d 0a20 2020 2020 2020  (self, ..       
+00001e20: 2076 6f6c 756d 653a 2066 6c6f 6174 2c20   volume: float, 
+00001e30: 0d0a 2020 2020 2020 2020 7370 6565 643a  ..        speed:
+00001e40: 204f 7074 696f 6e61 6c5b 666c 6f61 745d   Optional[float]
+00001e50: 203d 204e 6f6e 652c 200d 0a20 2020 2020   = None, ..     
+00001e60: 2020 2077 6169 743a 2069 6e74 203d 2030     wait: int = 0
+00001e70: 2c20 0d0a 2020 2020 2020 2020 7061 7573  , ..        paus
+00001e80: 653a 2062 6f6f 6c20 3d20 4661 6c73 652c  e: bool = False,
+00001e90: 200d 0a20 2020 2020 2020 2072 6561 6765   ..        reage
+00001ea0: 6e74 3a20 4f70 7469 6f6e 616c 5b73 7472  nt: Optional[str
+00001eb0: 5d20 3d20 4e6f 6e65 2c0d 0a20 2020 2020  ] = None,..     
+00001ec0: 2020 202a 2a6b 7761 7267 730d 0a20 2020     **kwargs..   
+00001ed0: 2029 202d 3e20 7374 723a 0d0a 2020 2020   ) -> str:..    
+00001ee0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00001ef0: 2041 7370 6972 6174 6520 6465 7369 7265   Aspirate desire
+00001f00: 6420 766f 6c75 6d65 206f 6620 7265 6167  d volume of reag
+00001f10: 656e 740d 0a0d 0a20 2020 2020 2020 2041  ent....        A
+00001f20: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+00001f30: 2020 766f 6c75 6d65 2028 666c 6f61 7429    volume (float)
+00001f40: 3a20 7461 7267 6574 2076 6f6c 756d 650d  : target volume.
+00001f50: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
+00001f60: 6564 2028 4f70 7469 6f6e 616c 5b66 6c6f  ed (Optional[flo
+00001f70: 6174 5d2c 206f 7074 696f 6e61 6c29 3a20  at], optional): 
+00001f80: 7370 6565 6420 746f 2061 7370 6972 6174  speed to aspirat
+00001f90: 6520 6174 2e20 4465 6661 756c 7473 2074  e at. Defaults t
+00001fa0: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
+00001fb0: 2020 2020 2077 6169 7420 2869 6e74 2c20       wait (int, 
+00001fc0: 6f70 7469 6f6e 616c 293a 2074 696d 6520  optional): time 
+00001fd0: 6465 6c61 7920 6166 7465 7220 6173 7069  delay after aspi
+00001fe0: 7261 7465 2e20 4465 6661 756c 7473 2074  rate. Defaults t
+00001ff0: 6f20 302e 0d0a 2020 2020 2020 2020 2020  o 0...          
+00002000: 2020 7061 7573 6520 2862 6f6f 6c2c 206f    pause (bool, o
+00002010: 7074 696f 6e61 6c29 3a20 7768 6574 6865  ptional): whethe
+00002020: 7220 746f 2070 6175 7365 2066 6f72 2075  r to pause for u
+00002030: 7365 7220 696e 7465 7276 656e 7469 6f6e  ser intervention
+00002040: 2e20 4465 6661 756c 7473 2074 6f20 4661  . Defaults to Fa
+00002050: 6c73 652e 0d0a 2020 2020 2020 2020 2020  lse...          
+00002060: 2020 7265 6167 656e 7420 284f 7074 696f    reagent (Optio
+00002070: 6e61 6c5b 7374 725d 2c20 6f70 7469 6f6e  nal[str], option
+00002080: 616c 293a 206e 616d 6520 6f66 2072 6561  al): name of rea
+00002090: 6765 6e74 2e20 4465 6661 756c 7473 2074  gent. Defaults t
+000020a0: 6f20 4e6f 6e65 2e0d 0a20 2020 2020 2020  o None...       
+000020b0: 2020 2020 200d 0a20 2020 2020 2020 2052       ..        R
+000020c0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+000020d0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
+000020e0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+000020f0: 2020 2022 2222 200d 0a20 2020 2020 2020     """ ..       
+00002100: 2073 656c 662e 7365 7446 6c61 6728 7061   self.setFlag(pa
+00002110: 7573 655f 6665 6564 6261 636b 3d54 7275  use_feedback=Tru
+00002120: 652c 206f 6363 7570 6965 643d 5472 7565  e, occupied=True
+00002130: 290d 0a20 2020 2020 2020 2076 6f6c 756d  )..        volum
+00002140: 6520 3d20 6d69 6e28 766f 6c75 6d65 2c20  e = min(volume, 
+00002150: 7365 6c66 2e63 6170 6163 6974 7920 2d20  self.capacity - 
+00002160: 7365 6c66 2e76 6f6c 756d 6529 0d0a 2020  self.volume)..  
+00002170: 2020 2020 2020 7374 6570 7320 3d20 696e        steps = in
+00002180: 7428 766f 6c75 6d65 202f 2073 656c 662e  t(volume / self.
+00002190: 7265 736f 6c75 7469 6f6e 290d 0a20 2020  resolution)..   
+000021a0: 2020 2020 2076 6f6c 756d 6520 3d20 7374       volume = st
+000021b0: 6570 7320 2a20 7365 6c66 2e72 6573 6f6c  eps * self.resol
+000021c0: 7574 696f 6e0d 0a20 2020 2020 2020 2069  ution..        i
+000021d0: 6620 766f 6c75 6d65 203d 3d20 303a 0d0a  f volume == 0:..
+000021e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000021f0: 726e 2027 270d 0a20 2020 2020 2020 2070  rn ''..        p
+00002200: 7269 6e74 2866 2741 7370 6972 6174 696e  rint(f'Aspiratin
+00002210: 6720 7b76 6f6c 756d 657d 2075 4c2e 2e2e  g {volume} uL...
+00002220: 2729 0d0a 2020 2020 2020 2020 7374 6172  ')..        star
+00002230: 745f 6173 7069 7261 7465 203d 2074 696d  t_aspirate = tim
+00002240: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
+00002250: 0d0a 2020 2020 2020 2020 7370 6565 6420  ..        speed 
+00002260: 3d20 7365 6c66 2e73 7065 6564 2e75 7020  = self.speed.up 
+00002270: 6966 2073 7065 6564 2069 7320 4e6f 6e65  if speed is None
+00002280: 2065 6c73 6520 7370 6565 640d 0a20 2020   else speed..   
+00002290: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+000022a0: 6620 7370 6565 6420 696e 2073 656c 662e  f speed in self.
+000022b0: 7370 6565 645f 7072 6573 6574 733a 0d0a  speed_presets:..
+000022c0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000022d0: 7065 6564 2021 3d20 7365 6c66 2e73 7065  peed != self.spe
+000022e0: 6564 2e75 703a 0d0a 2020 2020 2020 2020  ed.up:..        
+000022f0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+00002300: 5370 6565 6428 7370 6565 643d 7370 6565  Speed(speed=spee
+00002310: 642c 2075 703d 5472 7565 2c20 6465 6661  d, up=True, defa
+00002320: 756c 743d 4661 6c73 6529 0d0a 2020 2020  ult=False)..    
+00002330: 2020 2020 2020 2020 7374 6172 745f 6173          start_as
+00002340: 7069 7261 7465 203d 2074 696d 652e 7065  pirate = time.pe
+00002350: 7266 5f63 6f75 6e74 6572 2829 0d0a 2020  rf_counter()..  
+00002360: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+00002370: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
+00002380: 2866 2752 497b 7374 6570 737d 2729 0d0a  (f'RI{steps}')..
+00002390: 2020 2020 2020 2020 2020 2020 6d6f 7665              move
+000023a0: 5f74 696d 6520 3d20 7374 6570 732a 7365  _time = steps*se
+000023b0: 6c66 2e72 6573 6f6c 7574 696f 6e20 2f20  lf.resolution / 
+000023c0: 7370 6565 640d 0a20 2020 2020 2020 2020  speed..         
+000023d0: 2020 2064 7572 6174 696f 6e20 3d20 7469     duration = ti
+000023e0: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
+000023f0: 2920 2d20 7374 6172 745f 6173 7069 7261  ) - start_aspira
+00002400: 7465 0d0a 2020 2020 2020 2020 2020 2020  te..            
+00002410: 6966 2064 7572 6174 696f 6e20 3c20 286d  if duration < (m
+00002420: 6f76 655f 7469 6d65 293a 0d0a 2020 2020  ove_time):..    
+00002430: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00002440: 2e73 6c65 6570 286d 6f76 655f 7469 6d65  .sleep(move_time
+00002450: 2d64 7572 6174 696f 6e29 0d0a 2020 2020  -duration)..    
+00002460: 2020 2020 2020 2020 2320 6966 2072 6573          # if res
+00002470: 706f 6e73 6520 213d 2027 6f6b 273a 0d0a  ponse != 'ok':..
+00002480: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00002490: 2020 7265 7475 726e 2072 6573 706f 6e73    return respons
+000024a0: 650d 0a20 2020 2020 2020 2020 2020 200d  e..            .
+000024b0: 0a20 2020 2020 2020 2065 6c69 6620 7370  .        elif sp
+000024c0: 6565 6420 6e6f 7420 696e 2073 656c 662e  eed not in self.
+000024d0: 7370 6565 645f 7072 6573 6574 733a 0d0a  speed_presets:..
+000024e0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000024f0: 7428 6622 5461 7267 6574 3a20 7b76 6f6c  t(f"Target: {vol
+00002500: 756d 657d 2075 4c20 6174 207b 7370 6565  ume} uL at {spee
+00002510: 647d 2075 4c2f 732e 2e2e 2229 0d0a 2020  d} uL/s...")..  
+00002520: 2020 2020 2020 2020 2020 7370 6565 645f            speed_
+00002530: 7061 7261 6d65 7465 7273 203d 2073 656c  parameters = sel
+00002540: 662e 5f63 616c 6375 6c61 7465 5f73 7065  f._calculate_spe
+00002550: 6564 5f70 6172 616d 6574 6572 7328 766f  ed_parameters(vo
+00002560: 6c75 6d65 3d76 6f6c 756d 652c 2073 7065  lume=volume, spe
+00002570: 6564 3d73 7065 6564 290d 0a20 2020 2020  ed=speed)..     
+00002580: 2020 2020 2020 2070 7269 6e74 2873 7065         print(spe
+00002590: 6564 5f70 6172 616d 6574 6572 7329 0d0a  ed_parameters)..
+000025a0: 2020 2020 2020 2020 2020 2020 7072 6573              pres
+000025b0: 6574 203d 2073 7065 6564 5f70 6172 616d  et = speed_param
+000025c0: 6574 6572 732e 7072 6573 6574 0d0a 2020  eters.preset..  
+000025d0: 2020 2020 2020 2020 2020 6966 2070 7265            if pre
+000025e0: 7365 7420 6973 204e 6f6e 653a 0d0a 2020  set is None:..  
+000025f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00002600: 7261 6973 6520 5275 6e74 696d 6545 7272  raise RuntimeErr
+00002610: 6f72 2827 5461 7267 6574 2073 7065 6564  or('Target speed
+00002620: 206e 6f74 2070 6f73 7369 626c 652e 2729   not possible.')
+00002630: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002640: 2020 7072 696e 7428 2754 6172 6765 7420    print('Target 
+00002650: 7370 6565 6420 6e6f 7420 706f 7373 6962  speed not possib
+00002660: 6c65 2e27 290d 0a20 2020 2020 2020 2020  le.')..         
+00002670: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
+00002680: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002690: 7365 7453 7065 6564 2873 7065 6564 3d70  setSpeed(speed=p
+000026a0: 7265 7365 742c 2075 703d 5472 7565 2c20  reset, up=True, 
+000026b0: 6465 6661 756c 743d 4661 6c73 6529 0d0a  default=False)..
+000026c0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+000026d0: 2020 2020 2020 2020 2020 7374 6570 735f            steps_
+000026e0: 6c65 6674 203d 2073 7465 7073 0d0a 2020  left = steps..  
+000026f0: 2020 2020 2020 2020 2020 6465 6c61 7920            delay 
+00002700: 3d20 7370 6565 645f 7061 7261 6d65 7465  = speed_paramete
+00002710: 7273 2e64 656c 6179 0d0a 2020 2020 2020  rs.delay..      
+00002720: 2020 2020 2020 7374 6570 5f73 697a 6520        step_size 
+00002730: 3d20 7370 6565 645f 7061 7261 6d65 7465  = speed_paramete
+00002740: 7273 2e73 7465 705f 7369 7a65 0d0a 2020  rs.step_size..  
+00002750: 2020 2020 2020 2020 2020 696e 7465 7276            interv
+00002760: 616c 7320 3d20 7370 6565 645f 7061 7261  als = speed_para
+00002770: 6d65 7465 7273 2e69 6e74 6572 7661 6c73  meters.intervals
+00002780: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00002790: 6172 745f 6173 7069 7261 7465 203d 2074  art_aspirate = t
+000027a0: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
+000027b0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+000027c0: 666f 7220 6920 696e 2072 616e 6765 2869  for i in range(i
+000027d0: 6e74 6572 7661 6c73 293a 0d0a 2020 2020  ntervals):..    
+000027e0: 2020 2020 2020 2020 2020 2020 7374 6172              star
+000027f0: 745f 7469 6d65 203d 2074 696d 652e 7065  t_time = time.pe
+00002800: 7266 5f63 6f75 6e74 6572 2829 0d0a 2020  rf_counter()..  
+00002810: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00002820: 6570 203d 2073 7465 705f 7369 7a65 2069  ep = step_size i
+00002830: 6620 2869 2b31 2021 3d20 696e 7465 7276  f (i+1 != interv
+00002840: 616c 7329 2065 6c73 6520 7374 6570 735f  als) else steps_
+00002850: 6c65 6674 0d0a 2020 2020 2020 2020 2020  left..          
+00002860: 2020 2020 2020 6d6f 7665 5f74 696d 6520        move_time 
+00002870: 3d20 7374 6570 2a73 656c 662e 7265 736f  = step*self.reso
+00002880: 6c75 7469 6f6e 202f 2070 7265 7365 740d  lution / preset.
+00002890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000028a0: 2072 6573 706f 6e73 6520 3d20 7365 6c66   response = self
+000028b0: 2e5f 7175 6572 7928 6627 5249 7b73 7465  ._query(f'RI{ste
+000028c0: 707d 272c 2072 6573 756d 655f 6665 6564  p}', resume_feed
+000028d0: 6261 636b 3d46 616c 7365 2c20 6765 745f  back=False, get_
+000028e0: 706f 7369 7469 6f6e 3d46 616c 7365 290d  position=False).
+000028f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002900: 2023 2069 6620 7265 7370 6f6e 7365 2021   # if response !
+00002910: 3d20 276f 6b27 3a0d 0a20 2020 2020 2020  = 'ok':..       
+00002920: 2020 2020 2020 2020 2023 2020 2020 2070           #     p
+00002930: 7269 6e74 2822 4173 7069 7261 7469 6f6e  rint("Aspiration
+00002940: 2066 6169 6c65 6422 290d 0a20 2020 2020   failed")..     
+00002950: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00002960: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+00002970: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002980: 2020 7374 6570 735f 6c65 6674 202d 3d20    steps_left -= 
+00002990: 7374 6570 0d0a 2020 2020 2020 2020 2020  step..          
+000029a0: 2020 2020 2020 6475 7261 7469 6f6e 203d        duration =
+000029b0: 2074 696d 652e 7065 7266 5f63 6f75 6e74   time.perf_count
+000029c0: 6572 2829 202d 2073 7461 7274 5f74 696d  er() - start_tim
+000029d0: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+000029e0: 2020 2069 6620 6475 7261 7469 6f6e 203c     if duration <
+000029f0: 2028 6465 6c61 792b 6d6f 7665 5f74 696d   (delay+move_tim
+00002a00: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
+00002a10: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
+00002a20: 6565 7028 6465 6c61 792b 6d6f 7665 5f74  eep(delay+move_t
+00002a30: 696d 652d 6475 7261 7469 6f6e 290d 0a20  ime-duration).. 
+00002a40: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002a50: 2023 2055 7064 6174 6520 7661 6c75 6573   # Update values
+00002a60: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00002a70: 6627 4173 7069 7261 7469 6f6e 2074 696d  f'Aspiration tim
+00002a80: 653a 207b 7469 6d65 2e70 6572 665f 636f  e: {time.perf_co
+00002a90: 756e 7465 7228 292d 7374 6172 745f 6173  unter()-start_as
+00002aa0: 7069 7261 7465 7d73 2729 0d0a 2020 2020  pirate}s')..    
+00002ab0: 2020 2020 7469 6d65 2e73 6c65 6570 2877      time.sleep(w
+00002ac0: 6169 7429 0d0a 2020 2020 2020 2020 7365  ait)..        se
+00002ad0: 6c66 2e73 6574 466c 6167 286f 6363 7570  lf.setFlag(occup
+00002ae0: 6965 643d 4661 6c73 652c 2070 6175 7365  ied=False, pause
+00002af0: 5f66 6565 6462 6163 6b3d 4661 6c73 6529  _feedback=False)
+00002b00: 0d0a 2020 2020 2020 2020 7365 6c66 2e67  ..        self.g
+00002b10: 6574 506f 7369 7469 6f6e 2829 0d0a 2020  etPosition()..  
+00002b20: 2020 2020 2020 7365 6c66 2e76 6f6c 756d        self.volum
+00002b30: 6520 2b3d 2076 6f6c 756d 650d 0a20 2020  e += volume..   
+00002b40: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
+00002b50: 6f6e 202b 3d20 7374 6570 730d 0a20 2020  on += steps..   
+00002b60: 2020 2020 2069 6620 7265 6167 656e 7420       if reagent 
+00002b70: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
+00002b80: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00002b90: 6561 6765 6e74 203d 2072 6561 6765 6e74  eagent = reagent
+00002ba0: 0d0a 2020 2020 2020 2020 6966 2070 6175  ..        if pau
+00002bb0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00002bc0: 2069 6e70 7574 2822 5072 6573 7320 2745   input("Press 'E
+00002bd0: 6e74 6572 2720 746f 2070 726f 6365 6564  nter' to proceed
+00002be0: 2e22 290d 0a20 2020 2020 2020 2072 6574  .")..        ret
+00002bf0: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
+00002c00: 2020 0d0a 2020 2020 6465 6620 626c 6f77    ..    def blow
+00002c10: 6f75 7428 7365 6c66 2c20 686f 6d65 3a62  out(self, home:b
+00002c20: 6f6f 6c20 3d20 5472 7565 2c20 2a2a 6b77  ool = True, **kw
+00002c30: 6172 6773 2920 2d3e 2073 7472 3a0d 0a20  args) -> str:.. 
+00002c40: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00002c50: 2020 2020 426c 6f77 6f75 7420 6c69 7175      Blowout liqu
+00002c60: 6964 2066 726f 6d20 7469 700d 0a0d 0a20  id from tip.... 
+00002c70: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
+00002c80: 2020 2020 2020 2020 2020 686f 6d65 2028            home (
+00002c90: 626f 6f6c 2c20 6f70 7469 6f6e 616c 293a  bool, optional):
+00002ca0: 2077 6865 7468 6572 2074 6f20 7265 7475   whether to retu
+00002cb0: 726e 2070 6c75 6e67 6572 2074 6f20 686f  rn plunger to ho
+00002cc0: 6d65 2070 6f73 6974 696f 6e2e 2044 6566  me position. Def
+00002cd0: 6175 6c74 7320 746f 2054 7275 652e 0d0a  aults to True...
+00002ce0: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00002cf0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00002d00: 7374 723a 2064 6576 6963 6520 7265 7370  str: device resp
+00002d10: 6f6e 7365 0d0a 2020 2020 2020 2020 2222  onse..        ""
+00002d20: 220d 0a20 2020 2020 2020 2063 6f6d 6d61  "..        comma
+00002d30: 6e64 203d 2066 2752 427b 7365 6c66 2e68  nd = f'RB{self.h
+00002d40: 6f6d 655f 706f 7369 7469 6f6e 7d27 2069  ome_position}' i
+00002d50: 6620 686f 6d65 2065 6c73 6520 2752 4227  f home else 'RB'
+00002d60: 0d0a 2020 2020 2020 2020 7265 7370 6f6e  ..        respon
+00002d70: 7365 203d 2073 656c 662e 5f71 7565 7279  se = self._query
+00002d80: 2863 6f6d 6d61 6e64 290d 0a20 2020 2020  (command)..     
+00002d90: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
+00002da0: 203d 2073 656c 662e 686f 6d65 5f70 6f73   = self.home_pos
+00002db0: 6974 696f 6e0d 0a20 2020 2020 2020 2074  ition..        t
+00002dc0: 696d 652e 736c 6565 7028 3129 0d0a 2020  ime.sleep(1)..  
+00002dd0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00002de0: 706f 6e73 650d 0a20 2020 200d 0a20 2020  ponse..    ..   
+00002df0: 2064 6566 2064 6973 7065 6e73 6528 7365   def dispense(se
+00002e00: 6c66 2c20 0d0a 2020 2020 2020 2020 766f  lf, ..        vo
+00002e10: 6c75 6d65 3a20 666c 6f61 742c 200d 0a20  lume: float, .. 
+00002e20: 2020 2020 2020 2073 7065 6564 3a20 4f70         speed: Op
+00002e30: 7469 6f6e 616c 5b66 6c6f 6174 5d20 3d20  tional[float] = 
+00002e40: 4e6f 6e65 2c20 0d0a 2020 2020 2020 2020  None, ..        
+00002e50: 7761 6974 3a20 696e 7420 3d20 302c 200d  wait: int = 0, .
+00002e60: 0a20 2020 2020 2020 2070 6175 7365 3a20  .        pause: 
+00002e70: 626f 6f6c 203d 2046 616c 7365 2c20 0d0a  bool = False, ..
+00002e80: 2020 2020 2020 2020 626c 6f77 6f75 743a          blowout:
+00002e90: 2062 6f6f 6c20 3d20 4661 6c73 652c 0d0a   bool = False,..
+00002ea0: 2020 2020 2020 2020 626c 6f77 6f75 745f          blowout_
+00002eb0: 686f 6d65 3a20 626f 6f6c 203d 2054 7275  home: bool = Tru
+00002ec0: 652c 0d0a 2020 2020 2020 2020 666f 7263  e,..        forc
+00002ed0: 655f 6469 7370 656e 7365 3a20 626f 6f6c  e_dispense: bool
+00002ee0: 203d 2046 616c 7365 2c20 0d0a 2020 2020   = False, ..    
+00002ef0: 2020 2020 2a2a 6b77 6172 6773 0d0a 2020      **kwargs..  
+00002f00: 2020 2920 2d3e 2073 7472 3a0d 0a20 2020    ) -> str:..   
+00002f10: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00002f20: 2020 4469 7370 656e 7365 2064 6573 6972    Dispense desir
+00002f30: 6564 2076 6f6c 756d 6520 6f66 2072 6561  ed volume of rea
+00002f40: 6765 6e74 0d0a 0d0a 2020 2020 2020 2020  gent....        
+00002f50: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
+00002f60: 2020 2076 6f6c 756d 6520 2866 6c6f 6174     volume (float
+00002f70: 293a 2074 6172 6765 7420 766f 6c75 6d65  ): target volume
+00002f80: 0d0a 2020 2020 2020 2020 2020 2020 7370  ..            sp
+00002f90: 6565 6420 284f 7074 696f 6e61 6c5b 666c  eed (Optional[fl
+00002fa0: 6f61 745d 2c20 6f70 7469 6f6e 616c 293a  oat], optional):
+00002fb0: 2073 7065 6564 2074 6f20 6469 7370 656e   speed to dispen
+00002fc0: 7365 2061 742e 2044 6566 6175 6c74 7320  se at. Defaults 
+00002fd0: 746f 204e 6f6e 652e 0d0a 2020 2020 2020  to None...      
+00002fe0: 2020 2020 2020 7761 6974 2028 696e 742c        wait (int,
+00002ff0: 206f 7074 696f 6e61 6c29 3a20 7469 6d65   optional): time
+00003000: 2064 656c 6179 2061 6674 6572 2064 6973   delay after dis
+00003010: 7065 6e73 652e 2044 6566 6175 6c74 7320  pense. Defaults 
+00003020: 746f 2030 2e0d 0a20 2020 2020 2020 2020  to 0...         
+00003030: 2020 2070 6175 7365 2028 626f 6f6c 2c20     pause (bool, 
+00003040: 6f70 7469 6f6e 616c 293a 2077 6865 7468  optional): wheth
+00003050: 6572 2074 6f20 7061 7573 6520 666f 7220  er to pause for 
+00003060: 7573 6572 2069 6e74 6572 7665 6e74 696f  user interventio
+00003070: 6e2e 2044 6566 6175 6c74 7320 746f 2046  n. Defaults to F
+00003080: 616c 7365 2e0d 0a20 2020 2020 2020 2020  alse...         
+00003090: 2020 2062 6c6f 776f 7574 2028 626f 6f6c     blowout (bool
+000030a0: 2c20 6f70 7469 6f6e 616c 293a 2077 6865  , optional): whe
+000030b0: 7468 6572 2070 6572 666f 726d 2062 6c6f  ther perform blo
+000030c0: 776f 7574 2e20 4465 6661 756c 7473 2074  wout. Defaults t
+000030d0: 6f20 4661 6c73 652e 0d0a 2020 2020 2020  o False...      
+000030e0: 2020 2020 2020 626c 6f77 6f75 745f 686f        blowout_ho
+000030f0: 6d65 2028 626f 6f6c 2c20 6f70 7469 6f6e  me (bool, option
+00003100: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
+00003110: 7265 7475 726e 2074 6865 2070 6c75 6e67  return the plung
+00003120: 6572 2068 6f6d 6520 6166 7465 7220 626c  er home after bl
+00003130: 6f77 6f75 742e 2044 6566 6175 6c74 7320  owout. Defaults 
+00003140: 746f 2054 7275 652e 0d0a 2020 2020 2020  to True...      
+00003150: 2020 2020 2020 666f 7263 655f 6469 7370        force_disp
+00003160: 656e 7365 2028 626f 6f6c 2c20 6f70 7469  ense (bool, opti
+00003170: 6f6e 616c 293a 2077 6865 7468 6572 2074  onal): whether t
+00003180: 6f20 6469 7370 656e 7365 2072 6561 6765  o dispense reage
+00003190: 6e74 2072 6567 6172 646c 6573 732e 2044  nt regardless. D
+000031a0: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+000031b0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6169  .....        Rai
+000031c0: 7365 733a 0d0a 2020 2020 2020 2020 2020  ses:..          
+000031d0: 2020 5661 6c75 6545 7272 6f72 3a20 5265    ValueError: Re
+000031e0: 7175 6972 6564 2064 6973 7065 6e73 6520  quired dispense 
+000031f0: 766f 6c75 6d65 2069 7320 6772 6561 7465  volume is greate
+00003200: 7220 7468 616e 2076 6f6c 756d 6520 696e  r than volume in
+00003210: 2074 6970 0d0a 0d0a 2020 2020 2020 2020   tip....        
+00003220: 5265 7475 726e 733a 0d0a 2020 2020 2020  Returns:..      
+00003230: 2020 2020 2020 7374 723a 2064 6576 6963        str: devic
+00003240: 6520 7265 7370 6f6e 7365 0d0a 2020 2020  e response..    
+00003250: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+00003260: 2073 656c 662e 7365 7446 6c61 6728 7061   self.setFlag(pa
+00003270: 7573 655f 6665 6564 6261 636b 3d54 7275  use_feedback=Tru
+00003280: 652c 206f 6363 7570 6965 643d 5472 7565  e, occupied=True
+00003290: 290d 0a20 2020 2020 2020 2069 6620 666f  )..        if fo
+000032a0: 7263 655f 6469 7370 656e 7365 3a0d 0a20  rce_dispense:.. 
+000032b0: 2020 2020 2020 2020 2020 2076 6f6c 756d             volum
+000032c0: 6520 3d20 6d69 6e28 766f 6c75 6d65 2c20  e = min(volume, 
+000032d0: 7365 6c66 2e76 6f6c 756d 6529 0d0a 2020  self.volume)..  
+000032e0: 2020 2020 2020 656c 6966 2076 6f6c 756d        elif volum
+000032f0: 6520 3e20 7365 6c66 2e76 6f6c 756d 653a  e > self.volume:
+00003300: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00003310: 6973 6520 5661 6c75 6545 7272 6f72 2827  ise ValueError('
+00003320: 5265 7175 6972 6564 2064 6973 7065 6e73  Required dispens
+00003330: 6520 766f 6c75 6d65 2069 7320 6772 6561  e volume is grea
+00003340: 7465 7220 7468 616e 2076 6f6c 756d 6520  ter than volume 
+00003350: 696e 2074 6970 2e27 290d 0a20 2020 2020  in tip.')..     
+00003360: 2020 2073 7465 7073 203d 2069 6e74 2876     steps = int(v
+00003370: 6f6c 756d 6520 2f20 7365 6c66 2e72 6573  olume / self.res
+00003380: 6f6c 7574 696f 6e29 0d0a 2020 2020 2020  olution)..      
+00003390: 2020 766f 6c75 6d65 203d 2073 7465 7073    volume = steps
+000033a0: 202a 2073 656c 662e 7265 736f 6c75 7469   * self.resoluti
+000033b0: 6f6e 0d0a 2020 2020 2020 2020 6966 2076  on..        if v
+000033c0: 6f6c 756d 6520 3d3d 2030 3a0d 0a20 2020  olume == 0:..   
+000033d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000033e0: 2727 0d0a 2020 2020 2020 2020 7072 696e  ''..        prin
+000033f0: 7428 6627 4469 7370 656e 7369 6e67 207b  t(f'Dispensing {
+00003400: 766f 6c75 6d65 7d20 754c 2e2e 2e27 290d  volume} uL...').
+00003410: 0a20 2020 2020 2020 2073 7461 7274 5f64  .        start_d
+00003420: 6973 7065 6e73 6520 3d20 7469 6d65 2e70  ispense = time.p
+00003430: 6572 665f 636f 756e 7465 7228 290d 0a20  erf_counter().. 
+00003440: 2020 2020 2020 2073 7065 6564 203d 2073         speed = s
+00003450: 656c 662e 7370 6565 642e 646f 776e 2069  elf.speed.down i
+00003460: 6620 7370 6565 6420 6973 204e 6f6e 6520  f speed is None 
+00003470: 656c 7365 2073 7065 6564 0d0a 0d0a 2020  else speed....  
+00003480: 2020 2020 2020 6966 2073 7065 6564 2069        if speed i
+00003490: 6e20 7365 6c66 2e73 7065 6564 5f70 7265  n self.speed_pre
+000034a0: 7365 7473 3a0d 0a20 2020 2020 2020 2020  sets:..         
+000034b0: 2020 2069 6620 7370 6565 6420 213d 2073     if speed != s
+000034c0: 656c 662e 7370 6565 642e 646f 776e 3a0d  elf.speed.down:.
+000034d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034e0: 2073 656c 662e 7365 7453 7065 6564 2873   self.setSpeed(s
+000034f0: 7065 6564 3d73 7065 6564 2c20 7570 3d46  peed=speed, up=F
+00003500: 616c 7365 2c20 6465 6661 756c 743d 4661  alse, default=Fa
+00003510: 6c73 6529 0d0a 2020 2020 2020 2020 2020  lse)..          
+00003520: 2020 7374 6172 745f 6469 7370 656e 7365    start_dispense
+00003530: 203d 2074 696d 652e 7065 7266 5f63 6f75   = time.perf_cou
+00003540: 6e74 6572 2829 0d0a 2020 2020 2020 2020  nter()..        
+00003550: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+00003560: 656c 662e 5f71 7565 7279 2866 2752 4f7b  elf._query(f'RO{
+00003570: 7374 6570 737d 2729 0d0a 2020 2020 2020  steps}')..      
+00003580: 2020 2020 2020 6d6f 7665 5f74 696d 6520        move_time 
+00003590: 3d20 7374 6570 732a 7365 6c66 2e72 6573  = steps*self.res
+000035a0: 6f6c 7574 696f 6e20 2f20 7370 6565 640d  olution / speed.
+000035b0: 0a20 2020 2020 2020 2020 2020 2064 7572  .            dur
+000035c0: 6174 696f 6e20 3d20 7469 6d65 2e70 6572  ation = time.per
+000035d0: 665f 636f 756e 7465 7228 2920 2d20 7374  f_counter() - st
+000035e0: 6172 745f 6469 7370 656e 7365 0d0a 2020  art_dispense..  
+000035f0: 2020 2020 2020 2020 2020 6966 2064 7572            if dur
+00003600: 6174 696f 6e20 3c20 286d 6f76 655f 7469  ation < (move_ti
+00003610: 6d65 293a 0d0a 2020 2020 2020 2020 2020  me):..          
+00003620: 2020 2020 2020 7469 6d65 2e73 6c65 6570        time.sleep
+00003630: 286d 6f76 655f 7469 6d65 2d64 7572 6174  (move_time-durat
+00003640: 696f 6e29 0d0a 2020 2020 2020 2020 2020  ion)..          
+00003650: 2020 2320 6966 2072 6573 706f 6e73 6520    # if response 
+00003660: 213d 2027 6f6b 273a 0d0a 2020 2020 2020  != 'ok':..      
+00003670: 2020 2020 2020 2320 2020 2020 7265 7475        #     retu
+00003680: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
+00003690: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+000036a0: 2020 2065 6c69 6620 7370 6565 6420 6e6f     elif speed no
+000036b0: 7420 696e 2073 656c 662e 7370 6565 645f  t in self.speed_
+000036c0: 7072 6573 6574 733a 0d0a 2020 2020 2020  presets:..      
+000036d0: 2020 2020 2020 7072 696e 7428 6622 5461        print(f"Ta
+000036e0: 7267 6574 3a20 7b76 6f6c 756d 657d 2075  rget: {volume} u
+000036f0: 4c20 6174 207b 7370 6565 647d 2075 4c2f  L at {speed} uL/
+00003700: 732e 2e2e 2229 0d0a 2020 2020 2020 2020  s...")..        
+00003710: 2020 2020 7370 6565 645f 7061 7261 6d65      speed_parame
+00003720: 7465 7273 203d 2073 656c 662e 5f63 616c  ters = self._cal
+00003730: 6375 6c61 7465 5f73 7065 6564 5f70 6172  culate_speed_par
+00003740: 616d 6574 6572 7328 766f 6c75 6d65 3d76  ameters(volume=v
+00003750: 6f6c 756d 652c 2073 7065 6564 3d73 7065  olume, speed=spe
+00003760: 6564 290d 0a20 2020 2020 2020 2020 2020  ed)..           
+00003770: 2070 7269 6e74 2873 7065 6564 5f70 6172   print(speed_par
+00003780: 616d 6574 6572 7329 0d0a 2020 2020 2020  ameters)..      
+00003790: 2020 2020 2020 7072 6573 6574 203d 2073        preset = s
+000037a0: 7065 6564 5f70 6172 616d 6574 6572 732e  peed_parameters.
+000037b0: 7072 6573 6574 0d0a 2020 2020 2020 2020  preset..        
+000037c0: 2020 2020 6966 2070 7265 7365 7420 6973      if preset is
+000037d0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+000037e0: 2020 2020 2020 2020 2320 7261 6973 6520          # raise 
+000037f0: 5275 6e74 696d 6545 7272 6f72 2827 5461  RuntimeError('Ta
+00003800: 7267 6574 2073 7065 6564 206e 6f74 2070  rget speed not p
+00003810: 6f73 7369 626c 652e 2729 0d0a 2020 2020  ossible.')..    
+00003820: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00003830: 7428 2754 6172 6765 7420 7370 6565 6420  t('Target speed 
+00003840: 6e6f 7420 706f 7373 6962 6c65 2e27 290d  not possible.').
+00003850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003860: 2072 6574 7572 6e0d 0a20 2020 2020 2020   return..       
+00003870: 2020 2020 2073 656c 662e 7365 7453 7065       self.setSpe
+00003880: 6564 2873 7065 6564 3d70 7265 7365 742c  ed(speed=preset,
+00003890: 2075 703d 4661 6c73 652c 2064 6566 6175   up=False, defau
+000038a0: 6c74 3d46 616c 7365 290d 0a20 2020 2020  lt=False)..     
+000038b0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+000038c0: 2073 7465 7073 5f6c 6566 7420 3d20 7374   steps_left = st
+000038d0: 6570 730d 0a20 2020 2020 2020 2020 2020  eps..           
+000038e0: 2064 656c 6179 203d 2073 7065 6564 5f70   delay = speed_p
+000038f0: 6172 616d 6574 6572 732e 6465 6c61 790d  arameters.delay.
+00003900: 0a20 2020 2020 2020 2020 2020 2073 7465  .            ste
+00003910: 705f 7369 7a65 203d 2073 7065 6564 5f70  p_size = speed_p
+00003920: 6172 616d 6574 6572 732e 7374 6570 5f73  arameters.step_s
+00003930: 697a 650d 0a20 2020 2020 2020 2020 2020  ize..           
+00003940: 2069 6e74 6572 7661 6c73 203d 2073 7065   intervals = spe
+00003950: 6564 5f70 6172 616d 6574 6572 732e 696e  ed_parameters.in
+00003960: 7465 7276 616c 730d 0a20 2020 2020 2020  tervals..       
+00003970: 2020 2020 2073 7461 7274 5f64 6973 7065       start_dispe
+00003980: 6e73 6520 3d20 7469 6d65 2e70 6572 665f  nse = time.perf_
+00003990: 636f 756e 7465 7228 290d 0a20 2020 2020  counter()..     
+000039a0: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+000039b0: 7261 6e67 6528 696e 7465 7276 616c 7329  range(intervals)
+000039c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000039d0: 2020 2073 7461 7274 5f74 696d 6520 3d20     start_time = 
+000039e0: 7469 6d65 2e70 6572 665f 636f 756e 7465  time.perf_counte
+000039f0: 7228 290d 0a20 2020 2020 2020 2020 2020  r()..           
+00003a00: 2020 2020 2073 7465 7020 3d20 7374 6570       step = step
+00003a10: 5f73 697a 6520 6966 2028 692b 3120 213d  _size if (i+1 !=
+00003a20: 2069 6e74 6572 7661 6c73 2920 656c 7365   intervals) else
+00003a30: 2073 7465 7073 5f6c 6566 740d 0a20 2020   steps_left..   
+00003a40: 2020 2020 2020 2020 2020 2020 206d 6f76               mov
+00003a50: 655f 7469 6d65 203d 2073 7465 702a 7365  e_time = step*se
+00003a60: 6c66 2e72 6573 6f6c 7574 696f 6e20 2f20  lf.resolution / 
+00003a70: 7072 6573 6574 0d0a 2020 2020 2020 2020  preset..        
+00003a80: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00003a90: 203d 2073 656c 662e 5f71 7565 7279 2866   = self._query(f
+00003aa0: 2752 4f7b 7374 6570 7d27 2c20 7265 7375  'RO{step}', resu
+00003ab0: 6d65 5f66 6565 6462 6163 6b3d 4661 6c73  me_feedback=Fals
+00003ac0: 652c 2067 6574 5f70 6f73 6974 696f 6e3d  e, get_position=
+00003ad0: 4661 6c73 6529 0d0a 2020 2020 2020 2020  False)..        
+00003ae0: 2020 2020 2020 2020 2320 6966 2072 6573          # if res
+00003af0: 706f 6e73 6520 213d 2027 6f6b 273a 0d0a  ponse != 'ok':..
+00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b10: 2320 2020 2020 7072 696e 7428 2244 6973  #     print("Dis
+00003b20: 7065 6e73 6520 6661 696c 6564 2229 0d0a  pense failed")..
+00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b40: 2320 2020 2020 7265 7475 726e 2072 6573  #     return res
+00003b50: 706f 6e73 650d 0a20 2020 2020 2020 2020  ponse..         
+00003b60: 2020 2020 2020 2073 7465 7073 5f6c 6566         steps_lef
+00003b70: 7420 2d3d 2073 7465 700d 0a20 2020 2020  t -= step..     
+00003b80: 2020 2020 2020 2020 2020 2064 7572 6174             durat
+00003b90: 696f 6e20 3d20 7469 6d65 2e70 6572 665f  ion = time.perf_
+00003ba0: 636f 756e 7465 7228 2920 2d20 7374 6172  counter() - star
+00003bb0: 745f 7469 6d65 0d0a 2020 2020 2020 2020  t_time..        
+00003bc0: 2020 2020 2020 2020 6966 2064 7572 6174          if durat
+00003bd0: 696f 6e20 3c20 2864 656c 6179 2b6d 6f76  ion < (delay+mov
+00003be0: 655f 7469 6d65 293a 0d0a 2020 2020 2020  e_time):..      
+00003bf0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00003c00: 6d65 2e73 6c65 6570 2864 656c 6179 2b6d  me.sleep(delay+m
+00003c10: 6f76 655f 7469 6d65 2d64 7572 6174 696f  ove_time-duratio
+00003c20: 6e29 0d0a 0d0a 2020 2020 2020 2020 2320  n)....        # 
+00003c30: 5570 6461 7465 2076 616c 7565 730d 0a20  Update values.. 
+00003c40: 2020 2020 2020 2070 7269 6e74 2866 2744         print(f'D
+00003c50: 6973 7065 6e73 6520 7469 6d65 3a20 7b74  ispense time: {t
+00003c60: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
+00003c70: 2829 2d73 7461 7274 5f64 6973 7065 6e73  ()-start_dispens
+00003c80: 657d 7327 290d 0a20 2020 2020 2020 2074  e}s')..        t
+00003c90: 696d 652e 736c 6565 7028 7761 6974 290d  ime.sleep(wait).
+00003ca0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00003cb0: 7446 6c61 6728 6f63 6375 7069 6564 3d46  tFlag(occupied=F
+00003cc0: 616c 7365 2c20 7061 7573 655f 6665 6564  alse, pause_feed
+00003cd0: 6261 636b 3d46 616c 7365 290d 0a20 2020  back=False)..   
+00003ce0: 2020 2020 2073 656c 662e 6765 7450 6f73       self.getPos
+00003cf0: 6974 696f 6e28 290d 0a20 2020 2020 2020  ition()..       
+00003d00: 2073 656c 662e 766f 6c75 6d65 203d 206d   self.volume = m
+00003d10: 6178 2873 656c 662e 766f 6c75 6d65 202d  ax(self.volume -
+00003d20: 2076 6f6c 756d 652c 2030 290d 0a20 2020   volume, 0)..   
+00003d30: 2020 2020 2073 656c 662e 706f 7369 7469       self.positi
+00003d40: 6f6e 202d 3d20 7374 6570 730d 0a20 2020  on -= steps..   
+00003d50: 2020 2020 2069 6620 7365 6c66 2e76 6f6c       if self.vol
+00003d60: 756d 6520 3d3d 2030 2061 6e64 2062 6c6f  ume == 0 and blo
+00003d70: 776f 7574 3a0d 0a20 2020 2020 2020 2020  wout:..         
+00003d80: 2020 2073 656c 662e 626c 6f77 6f75 7428     self.blowout(
+00003d90: 686f 6d65 3d62 6c6f 776f 7574 5f68 6f6d  home=blowout_hom
+00003da0: 6529 0d0a 2020 2020 2020 2020 6966 2070  e)..        if p
+00003db0: 6175 7365 3a0d 0a20 2020 2020 2020 2020  ause:..         
+00003dc0: 2020 2069 6e70 7574 2822 5072 6573 7320     input("Press 
+00003dd0: 2745 6e74 6572 2720 746f 2070 726f 6365  'Enter' to proce
+00003de0: 6564 2e22 290d 0a20 2020 2020 2020 2072  ed.")..        r
+00003df0: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
+00003e00: 2020 2020 0d0a 2020 2020 6465 6620 656a      ..    def ej
+00003e10: 6563 7428 7365 6c66 2c20 686f 6d65 3a62  ect(self, home:b
+00003e20: 6f6f 6c20 3d20 5472 7565 2920 2d3e 2073  ool = True) -> s
+00003e30: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
+00003e40: 0d0a 2020 2020 2020 2020 456a 6563 7420  ..        Eject 
+00003e50: 7468 6520 7069 7065 7474 6520 7469 700d  the pipette tip.
+00003e60: 0a0d 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00003e70: 0d0a 2020 2020 2020 2020 2020 2020 686f  ..            ho
+00003e80: 6d65 2028 626f 6f6c 2c20 6f70 7469 6f6e  me (bool, option
+00003e90: 616c 293a 2077 6865 7468 6572 2074 6f20  al): whether to 
+00003ea0: 7265 7475 726e 2070 6c75 6e67 6572 2074  return plunger t
+00003eb0: 6f20 686f 6d65 2070 6f73 6974 696f 6e2e  o home position.
+00003ec0: 2044 6566 6175 6c74 7320 746f 2054 7275   Defaults to Tru
+00003ed0: 652e 0d0a 0d0a 2020 2020 2020 2020 5265  e.....        Re
+00003ee0: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+00003ef0: 2020 2020 7374 723a 2064 6576 6963 6520      str: device 
+00003f00: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+00003f10: 2020 2222 220d 0a20 2020 2020 2020 2073    """..        s
+00003f20: 656c 662e 7265 6167 656e 7420 3d20 2727  elf.reagent = ''
+00003f30: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
+00003f40: 6420 3d20 6627 5245 7b73 656c 662e 686f  d = f'RE{self.ho
+00003f50: 6d65 5f70 6f73 6974 696f 6e7d 2720 6966  me_position}' if
+00003f60: 2068 6f6d 6520 656c 7365 2027 5245 270d   home else 'RE'.
+00003f70: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00003f80: 6520 3d20 7365 6c66 2e5f 7175 6572 7928  e = self._query(
+00003f90: 636f 6d6d 616e 6429 0d0a 2020 2020 2020  command)..      
+00003fa0: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
+00003fb0: 3d20 7365 6c66 2e68 6f6d 655f 706f 7369  = self.home_posi
+00003fc0: 7469 6f6e 2069 6620 686f 6d65 2065 6c73  tion if home els
+00003fd0: 6520 300d 0a20 2020 2020 2020 2074 696d  e 0..        tim
+00003fe0: 652e 736c 6565 7028 3129 0d0a 2020 2020  e.sleep(1)..    
+00003ff0: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00004000: 6e73 650d 0a20 2020 200d 0a20 2020 2064  nse..    ..    d
+00004010: 6566 2067 6574 4361 7061 6369 7461 6e63  ef getCapacitanc
+00004020: 6528 7365 6c66 2920 2d3e 2055 6e69 6f6e  e(self) -> Union
+00004030: 5b69 6e74 2c20 7374 725d 3a0d 0a20 2020  [int, str]:..   
+00004040: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00004050: 2020 4765 7420 7468 6520 6361 7061 6369    Get the capaci
+00004060: 7461 6e63 6520 6173 206d 6561 7375 7265  tance as measure
+00004070: 6420 6174 2074 6865 2065 6e64 206f 6620  d at the end of 
+00004080: 7468 6520 7069 7065 7474 650d 0a20 2020  the pipette..   
+00004090: 2020 2020 200d 0a20 2020 2020 2020 2052       ..        R
+000040a0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+000040b0: 2020 2020 2055 6e69 6f6e 5b69 6e74 2c20       Union[int, 
+000040c0: 7374 725d 3a20 6361 7061 6369 7461 6e63  str]: capacitanc
+000040d0: 6520 7661 6c75 652c 206f 7220 6465 7669  e value, or devi
+000040e0: 6365 2072 6573 706f 6e73 650d 0a20 2020  ce response..   
+000040f0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00004100: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
+00004110: 662e 5f71 7565 7279 2827 444e 2729 0d0a  f._query('DN')..
+00004120: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+00004130: 2020 2020 2020 2020 2020 6361 7061 6369            capaci
+00004140: 7461 6e63 6520 3d20 696e 7428 7265 7370  tance = int(resp
+00004150: 6f6e 7365 290d 0a20 2020 2020 2020 2065  onse)..        e
+00004160: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
+00004170: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+00004180: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
+00004190: 2020 2020 2020 2020 7365 6c66 2e5f 6361          self._ca
+000041a0: 7061 6369 7461 6e63 6520 3d20 6361 7061  pacitance = capa
+000041b0: 6369 7461 6e63 650d 0a20 2020 2020 2020  citance..       
+000041c0: 2072 6574 7572 6e20 6361 7061 6369 7461   return capacita
+000041d0: 6e63 650d 0a20 0d0a 2020 2020 6465 6620  nce.. ..    def 
+000041e0: 6765 7445 7272 6f72 7328 7365 6c66 2920  getErrors(self) 
+000041f0: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
+00004200: 2022 2222 0d0a 2020 2020 2020 2020 4765   """..        Ge
+00004210: 7420 6572 726f 7273 2066 726f 6d20 7468  t errors from th
+00004220: 6520 6465 7669 6365 0d0a 0d0a 2020 2020  e device....    
+00004230: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+00004240: 2020 2020 2020 2020 2020 7374 723a 2064            str: d
+00004250: 6576 6963 6520 7265 7370 6f6e 7365 0d0a  evice response..
+00004260: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00004270: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00004280: 2e5f 7175 6572 7928 2744 4527 290d 0a20  ._query('DE').. 
+00004290: 2020 200d 0a20 2020 2064 6566 2067 6574     ..    def get
+000042a0: 496e 666f 2873 656c 662c 206d 6f64 656c  Info(self, model
+000042b0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+000042c0: 3d20 4e6f 6e65 293a 0d0a 2020 2020 2020  = None):..      
+000042d0: 2020 2222 2247 6574 2064 6574 6169 6c73    """Get details
+000042e0: 206f 6620 7468 6520 5361 7274 6f72 6975   of the Sartoriu
+000042f0: 7320 7069 7065 7474 6520 6d6f 6465 6c22  s pipette model"
+00004300: 2222 0d0a 2020 2020 2020 2020 6d6f 6465  ""..        mode
+00004310: 6c20 3d20 7365 6c66 2e5f 5f6d 6f64 656c  l = self.__model
+00004320: 5f5f 2829 2e73 706c 6974 2827 2d27 295b  __().split('-')[
+00004330: 305d 2069 6620 6d6f 6465 6c20 6973 204e  0] if model is N
+00004340: 6f6e 6520 656c 7365 206d 6f64 656c 0d0a  one else model..
+00004350: 2020 2020 2020 2020 6966 206d 6f64 656c          if model
+00004360: 206e 6f74 2069 6e20 6c69 622e 4d6f 6465   not in lib.Mode
+00004370: 6c49 6e66 6f2e 5f6d 656d 6265 725f 6e61  lInfo._member_na
+00004380: 6d65 735f 3a0d 0a20 2020 2020 2020 2020  mes_:..         
+00004390: 2020 2070 7269 6e74 2866 2752 6563 6569     print(f'Recei
+000043a0: 7665 643a 207b 6d6f 6465 6c7d 2729 0d0a  ved: {model}')..
+000043b0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+000043c0: 6c20 3d20 2742 524c 3027 0d0a 2020 2020  l = 'BRL0'..    
+000043d0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+000043e0: 4465 6661 756c 7469 6e67 2074 6f3a 207b  Defaulting to: {
+000043f0: 2742 524c 3027 7d22 290d 0a20 2020 2020  'BRL0'}")..     
+00004400: 2020 2020 2020 2070 7269 6e74 2866 2256         print(f"V
+00004410: 616c 6964 206d 6f64 656c 7320 6172 653a  alid models are:
+00004420: 207b 272c 2027 2e6a 6f69 6e28 6c69 622e   {', '.join(lib.
+00004430: 4d6f 6465 6c49 6e66 6f2e 5f6d 656d 6265  ModelInfo._membe
+00004440: 725f 6e61 6d65 735f 297d 2229 0d0a 2020  r_names_)}")..  
+00004450: 2020 2020 2020 696e 666f 3a20 6c69 622e        info: lib.
+00004460: 4d6f 6465 6c20 3d20 6c69 622e 4d6f 6465  Model = lib.Mode
+00004470: 6c49 6e66 6f5b 6d6f 6465 6c5d 2e76 616c  lInfo[model].val
+00004480: 7565 0d0a 2020 2020 2020 2020 7072 696e  ue..        prin
+00004490: 7428 696e 666f 290d 0a20 2020 2020 2020  t(info)..       
+000044a0: 2073 656c 662e 6d6f 6465 6c5f 696e 666f   self.model_info
+000044b0: 203d 2069 6e66 6f0d 0a20 2020 2020 2020   = info..       
+000044c0: 2073 656c 662e 6361 7061 6369 7479 203d   self.capacity =
+000044d0: 2069 6e66 6f2e 6361 7061 6369 7479 0d0a   info.capacity..
+000044e0: 2020 2020 2020 2020 7365 6c66 2e6c 696d          self.lim
+000044f0: 6974 7320 3d20 2869 6e66 6f2e 7469 705f  its = (info.tip_
+00004500: 656a 6563 745f 706f 7369 7469 6f6e 2c20  eject_position, 
+00004510: 696e 666f 2e6d 6178 5f70 6f73 6974 696f  info.max_positio
+00004520: 6e29 0d0a 2020 2020 2020 2020 7365 6c66  n)..        self
+00004530: 2e73 7065 6564 5f70 7265 7365 7473 203d  .speed_presets =
+00004540: 2069 6e66 6f2e 7072 6573 6574 5f73 7065   info.preset_spe
+00004550: 6564 730d 0a20 2020 2020 2020 2073 656c  eds..        sel
+00004560: 662e 7370 6565 642e 7570 203d 2073 656c  f.speed.up = sel
+00004570: 662e 7370 6565 645f 7072 6573 6574 735b  f.speed_presets[
+00004580: 7365 6c66 2e73 7065 6564 5f63 6f64 652e  self.speed_code.
+00004590: 7570 2d31 5d0d 0a20 2020 2020 2020 2073  up-1]..        s
+000045a0: 656c 662e 7370 6565 642e 646f 776e 203d  elf.speed.down =
+000045b0: 2073 656c 662e 7370 6565 645f 7072 6573   self.speed_pres
+000045c0: 6574 735b 7365 6c66 2e73 7065 6564 5f63  ets[self.speed_c
+000045d0: 6f64 652e 646f 776e 2d31 5d0d 0a20 2020  ode.down-1]..   
+000045e0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+000045f0: 200d 0a20 2020 2064 6566 2067 6574 506f   ..    def getPo
+00004600: 7369 7469 6f6e 2873 656c 662c 202a 2a6b  sition(self, **k
+00004610: 7761 7267 7329 202d 3e20 696e 743a 0d0a  wargs) -> int:..
+00004620: 2020 2020 2020 2020 2222 2247 6574 2074          """Get t
+00004630: 6865 2063 7572 7265 6e74 2070 6f73 6974  he current posit
+00004640: 696f 6e20 6f66 2074 6865 2070 6970 6574  ion of the pipet
+00004650: 7465 2222 220d 0a20 2020 2020 2020 2072  te"""..        r
+00004660: 6573 706f 6e73 6520 3d20 7365 6c66 2e5f  esponse = self._
+00004670: 7175 6572 7928 2744 5027 290d 0a20 2020  query('DP')..   
+00004680: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
+00004690: 2020 2020 2020 2070 6f73 6974 696f 6e20         position 
+000046a0: 3d20 696e 7428 7265 7370 6f6e 7365 290d  = int(response).
+000046b0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000046c0: 5661 6c75 6545 7272 6f72 3a0d 0a20 2020  ValueError:..   
+000046d0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000046e0: 7265 7370 6f6e 7365 0d0a 2020 2020 2020  response..      
+000046f0: 2020 7365 6c66 2e70 6f73 6974 696f 6e20    self.position 
+00004700: 3d20 706f 7369 7469 6f6e 0d0a 2020 2020  = position..    
+00004710: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00004720: 706f 7369 7469 6f6e 0d0a 2020 2020 2020  position..      
+00004730: 0d0a 2020 2020 6465 6620 6765 7453 7461  ..    def getSta
+00004740: 7475 7328 7365 6c66 2c20 2a2a 6b77 6172  tus(self, **kwar
+00004750: 6773 2920 2d3e 2073 7472 3a0d 0a20 2020  gs) -> str:..   
+00004760: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00004770: 2020 4765 7420 7468 6520 7374 6174 7573    Get the status
+00004780: 206f 6620 7468 6520 7069 7065 7474 650d   of the pipette.
+00004790: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000047a0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+000047b0: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
+000047c0: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
+000047d0: 2222 0d0a 2020 2020 2020 2020 7265 7370  ""..        resp
+000047e0: 6f6e 7365 203d 2073 656c 662e 5f71 7565  onse = self._que
+000047f0: 7279 2827 4453 2729 0d0a 2020 2020 2020  ry('DS')..      
+00004800: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
+00004810: 2020 2020 7374 6174 7573 203d 2069 6e74      status = int
+00004820: 2872 6573 706f 6e73 6529 0d0a 2020 2020  (response)..    
+00004830: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
+00004840: 4572 726f 723a 0d0a 2020 2020 2020 2020  Error:..        
+00004850: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00004860: 6e73 650d 0a20 2020 2020 2020 2069 6620  nse..        if 
+00004870: 7265 7370 6f6e 7365 206e 6f74 2069 6e20  response not in 
+00004880: 5b5f 7374 6174 7573 2e76 616c 7565 2066  [_status.value f
+00004890: 6f72 205f 7374 6174 7573 2069 6e20 6c69  or _status in li
+000048a0: 622e 5374 6174 7573 436f 6465 5d3a 0d0a  b.StatusCode]:..
+000048b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000048c0: 726e 2072 6573 706f 6e73 650d 0a20 2020  rn response..   
+000048d0: 2020 2020 200d 0a20 2020 2020 2020 2073       ..        s
+000048e0: 656c 662e 5f73 7461 7475 735f 636f 6465  elf._status_code
+000048f0: 203d 2073 7461 7475 730d 0a20 2020 2020   = status..     
+00004900: 2020 2069 6620 7374 6174 7573 2069 6e20     if status in 
+00004910: 5b34 2c36 2c38 5d3a 0d0a 2020 2020 2020  [4,6,8]:..      
+00004920: 2020 2020 2020 7365 6c66 2e73 6574 466c        self.setFl
+00004930: 6167 2862 7573 793d 5472 7565 290d 0a20  ag(busy=True).. 
+00004940: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00004950: 6c66 2e76 6572 626f 7365 3a0d 0a20 2020  lf.verbose:..   
+00004960: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00004970: 6e74 286c 6962 2e53 7461 7475 7343 6f64  nt(lib.StatusCod
+00004980: 6528 7374 6174 7573 292e 6e61 6d65 290d  e(status).name).
+00004990: 0a20 2020 2020 2020 2065 6c69 6620 7374  .        elif st
+000049a0: 6174 7573 203d 3d20 303a 0d0a 2020 2020  atus == 0:..    
+000049b0: 2020 2020 2020 2020 7365 6c66 2e73 6574          self.set
+000049c0: 466c 6167 2862 7573 793d 4661 6c73 6529  Flag(busy=False)
+000049d0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+000049e0: 206c 6962 2e53 7461 7475 7343 6f64 6528   lib.StatusCode(
+000049f0: 7365 6c66 2e5f 7374 6174 7573 5f63 6f64  self._status_cod
+00004a00: 6529 2e6e 616d 650d 0a20 2020 200d 0a20  e).name..    .. 
+00004a10: 2020 2064 6566 2068 6f6d 6528 7365 6c66     def home(self
+00004a20: 2920 2d3e 2073 7472 3a0d 0a20 2020 2020  ) -> str:..     
+00004a30: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00004a40: 5265 7475 726e 2070 6c75 6e67 6572 2074  Return plunger t
+00004a50: 6f20 686f 6d65 2070 6f73 6974 696f 6e0d  o home position.
+00004a60: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00004a70: 2020 2052 6574 7572 6e73 3a0d 0a20 2020     Returns:..   
+00004a80: 2020 2020 2020 2020 2073 7472 3a20 6465           str: de
+00004a90: 7669 6365 2072 6573 706f 6e73 650d 0a20  vice response.. 
+00004aa0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00004ab0: 2020 2020 7265 7370 6f6e 7365 203d 2073      response = s
+00004ac0: 656c 662e 5f71 7565 7279 2866 2752 507b  elf._query(f'RP{
+00004ad0: 7365 6c66 2e68 6f6d 655f 706f 7369 7469  self.home_positi
+00004ae0: 6f6e 7d27 290d 0a20 2020 2020 2020 2073  on}')..        s
+00004af0: 656c 662e 766f 6c75 6d65 203d 2030 0d0a  elf.volume = 0..
+00004b00: 2020 2020 2020 2020 7365 6c66 2e70 6f73          self.pos
+00004b10: 6974 696f 6e20 3d20 7365 6c66 2e68 6f6d  ition = self.hom
+00004b20: 655f 706f 7369 7469 6f6e 0d0a 2020 2020  e_position..    
+00004b30: 2020 2020 7469 6d65 2e73 6c65 6570 2831      time.sleep(1
+00004b40: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00004b50: 6e20 7265 7370 6f6e 7365 0d0a 2020 2020  n response..    
+00004b60: 0d0a 2020 2020 6465 6620 6973 4665 6173  ..    def isFeas
+00004b70: 6962 6c65 2873 656c 662c 2070 6f73 6974  ible(self, posit
+00004b80: 696f 6e3a 696e 7429 202d 3e20 626f 6f6c  ion:int) -> bool
+00004b90: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00004ba0: 2020 2020 2020 2020 4368 6563 6b73 2061          Checks a
+00004bb0: 6e64 2072 6574 7572 6e73 2077 6865 7468  nd returns wheth
+00004bc0: 6572 2074 6865 2070 6c75 6e67 6572 2070  er the plunger p
+00004bd0: 6f73 6974 696f 6e20 6973 2066 6561 7369  osition is feasi
+00004be0: 626c 650d 0a0d 0a20 2020 2020 2020 2041  ble....        A
+00004bf0: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+00004c00: 2020 706f 7369 7469 6f6e 2028 696e 7429    position (int)
+00004c10: 3a20 706c 756e 6765 7220 706f 7369 7469  : plunger positi
+00004c20: 6f6e 0d0a 0d0a 2020 2020 2020 2020 5265  on....        Re
+00004c30: 7475 726e 733a 0d0a 2020 2020 2020 2020  turns:..        
+00004c40: 2020 2020 626f 6f6c 3a20 7768 6574 6865      bool: whethe
+00004c50: 7220 706c 756e 6765 7220 706f 7369 7469  r plunger positi
+00004c60: 6f6e 2069 7320 6665 6173 6962 6c65 0d0a  on is feasible..
+00004c70: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00004c80: 2020 2020 2069 6620 2873 656c 662e 6c69       if (self.li
+00004c90: 6d69 7473 5b30 5d20 3c3d 2070 6f73 6974  mits[0] <= posit
+00004ca0: 696f 6e20 3c3d 2073 656c 662e 6c69 6d69  ion <= self.limi
+00004cb0: 7473 5b31 5d29 3a0d 0a20 2020 2020 2020  ts[1]):..       
+00004cc0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00004cd0: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00004ce0: 6622 5261 6e67 6520 6c69 6d69 7473 2072  f"Range limits r
+00004cf0: 6561 6368 6564 2120 7b73 656c 662e 6c69  eached! {self.li
+00004d00: 6d69 7473 7d22 290d 0a20 2020 2020 2020  mits}")..       
+00004d10: 2072 6574 7572 6e20 4661 6c73 650d 0a20   return False.. 
+00004d20: 2020 200d 0a20 2020 2064 6566 2069 7354     ..    def isT
+00004d30: 6970 4f6e 2873 656c 6629 202d 3e20 626f  ipOn(self) -> bo
+00004d40: 6f6c 3a0d 0a20 2020 2020 2020 2022 2222  ol:..        """
+00004d50: 0d0a 2020 2020 2020 2020 4368 6563 6b73  ..        Checks
+00004d60: 2061 6e64 2072 6574 7572 6e73 2077 6865   and returns whe
+00004d70: 7468 6572 2061 2070 6970 6574 7465 2074  ther a pipette t
+00004d80: 6970 2069 7320 6174 7461 6368 6564 0d0a  ip is attached..
+00004d90: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00004da0: 2020 5265 7475 726e 733a 0d0a 2020 2020    Returns:..    
+00004db0: 2020 2020 2020 2020 626f 6f6c 3a20 7768          bool: wh
+00004dc0: 6574 6865 7220 6120 7069 7065 7474 6520  ether a pipette 
+00004dd0: 7469 7020 696e 2061 7474 6163 6865 640d  tip in attached.
+00004de0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00004df0: 2020 2020 2020 7365 6c66 2e67 6574 4361        self.getCa
+00004e00: 7061 6369 7461 6e63 6528 290d 0a20 2020  pacitance()..   
+00004e10: 2020 2020 2070 7269 6e74 2866 2754 6970       print(f'Tip
+00004e20: 2063 6170 6163 6974 616e 6365 3a20 7b73   capacitance: {s
+00004e30: 656c 662e 6361 7061 6369 7461 6e63 657d  elf.capacitance}
+00004e40: 2729 0d0a 2020 2020 2020 2020 6966 2073  ')..        if s
+00004e50: 656c 662e 666c 6167 735b 2763 6f6e 6475  elf.flags['condu
+00004e60: 6374 6976 655f 7469 7073 275d 3a0d 0a20  ctive_tips']:.. 
+00004e70: 2020 2020 2020 2020 2020 2074 6970 5f6f             tip_o
+00004e80: 6e20 3d20 2873 656c 662e 6361 7061 6369  n = (self.capaci
+00004e90: 7461 6e63 6520 3e20 7365 6c66 2e74 6970  tance > self.tip
+00004ea0: 5f74 6872 6573 686f 6c64 290d 0a20 2020  _threshold)..   
+00004eb0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00004ec0: 7446 6c61 6728 7469 705f 6f6e 3d74 6970  tFlag(tip_on=tip
+00004ed0: 5f6f 6e29 0d0a 2020 2020 2020 2020 7469  _on)..        ti
+00004ee0: 705f 6f6e 203d 2073 656c 662e 666c 6167  p_on = self.flag
+00004ef0: 735b 2774 6970 5f6f 6e27 5d0d 0a20 2020  s['tip_on']..   
+00004f00: 2020 2020 2072 6574 7572 6e20 7469 705f       return tip_
+00004f10: 6f6e 0d0a 2020 2020 0d0a 2020 2020 6465  on..    ..    de
+00004f20: 6620 6d6f 7665 2873 656c 662c 2073 7465  f move(self, ste
+00004f30: 7073 3a69 6e74 2c20 7570 3a62 6f6f 6c2c  ps:int, up:bool,
+00004f40: 202a 2a6b 7761 7267 7329 202d 3e20 7374   **kwargs) -> st
+00004f50: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+00004f60: 0a20 2020 2020 2020 204d 6f76 6520 7468  .        Move th
+00004f70: 6520 706c 756e 6765 7220 6569 7468 6572  e plunger either
+00004f80: 2075 7020 6f72 2064 6f77 6e20 6279 2061   up or down by a
+00004f90: 2073 7065 6369 6669 6564 206e 756d 6265   specified numbe
+00004fa0: 7220 6f66 2073 7465 7073 0d0a 0d0a 2020  r of steps....  
+00004fb0: 2020 2020 2020 4172 6773 3a0d 0a20 2020        Args:..   
+00004fc0: 2020 2020 2020 2020 2073 7465 7073 2028           steps (
+00004fd0: 696e 7429 3a20 6e75 6d62 6572 206f 6620  int): number of 
+00004fe0: 7374 6570 7320 746f 206d 6f76 6520 706c  steps to move pl
+00004ff0: 756e 6765 7220 6279 0d0a 2020 2020 2020  unger by..      
+00005000: 2020 2020 2020 7570 2028 626f 6f6c 293a        up (bool):
+00005010: 2077 6865 7468 6572 2074 6f20 6d6f 7665   whether to move
+00005020: 2074 6865 2070 6c75 6e67 6572 2075 700d   the plunger up.
+00005030: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00005040: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+00005050: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
+00005060: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
+00005070: 2222 0d0a 2020 2020 2020 2020 7374 6570  ""..        step
+00005080: 7320 3d20 6162 7328 7374 6570 7329 2069  s = abs(steps) i
+00005090: 6620 7570 2065 6c73 6520 2d61 6273 2873  f up else -abs(s
+000050a0: 7465 7073 290d 0a20 2020 2020 2020 2072  teps)..        r
+000050b0: 6574 7572 6e20 7365 6c66 2e6d 6f76 6542  eturn self.moveB
+000050c0: 7928 7374 6570 7329 0d0a 2020 2020 0d0a  y(steps)..    ..
+000050d0: 2020 2020 6465 6620 6d6f 7665 4279 2873      def moveBy(s
+000050e0: 656c 662c 2073 7465 7073 3a69 6e74 2c20  elf, steps:int, 
+000050f0: 2a2a 6b77 6172 6773 2920 2d3e 2073 7472  **kwargs) -> str
+00005100: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00005110: 2020 2020 2020 2020 4d6f 7665 2074 6865          Move the
+00005120: 2070 6c75 6e67 6572 2062 7920 7370 6563   plunger by spec
+00005130: 6966 6965 6420 6e75 6d62 6572 206f 6620  ified number of 
+00005140: 7374 6570 730d 0a0d 0a20 2020 2020 2020  steps....       
+00005150: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00005160: 2020 2020 7374 6570 7320 2869 6e74 293a      steps (int):
+00005170: 206e 756d 6265 7220 6f66 2073 7465 7073   number of steps
+00005180: 2074 6f20 6d6f 7665 2070 6c75 6e67 6572   to move plunger
+00005190: 2062 7920 283c 303a 206d 6f76 6520 646f   by (<0: move do
+000051a0: 776e 2f64 6973 7065 6e73 653b 203e 3020  wn/dispense; >0 
+000051b0: 6d6f 7665 2075 702f 6173 7069 7261 7465  move up/aspirate
+000051c0: 290d 0a0d 0a20 2020 2020 2020 2052 6574  )....        Ret
+000051d0: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+000051e0: 2020 2073 7472 3a20 6465 7669 6365 2072     str: device r
+000051f0: 6573 706f 6e73 650d 0a20 2020 2020 2020  esponse..       
+00005200: 2022 2222 0d0a 2020 2020 2020 2020 636f   """..        co
+00005210: 6d6d 616e 6420 3d20 6627 5249 7b73 7465  mmand = f'RI{ste
+00005220: 7073 7d27 2069 6620 7374 6570 7320 3e20  ps}' if steps > 
+00005230: 3020 656c 7365 2066 2752 4f7b 2d73 7465  0 else f'RO{-ste
+00005240: 7073 7d27 0d0a 2020 2020 2020 2020 7365  ps}'..        se
+00005250: 6c66 2e70 6f73 6974 696f 6e20 2b3d 2073  lf.position += s
+00005260: 7465 7073 0d0a 2020 2020 2020 2020 7265  teps..        re
+00005270: 7475 726e 2073 656c 662e 5f71 7565 7279  turn self._query
+00005280: 2863 6f6d 6d61 6e64 290d 0a20 2020 200d  (command)..    .
+00005290: 0a20 2020 2064 6566 206d 6f76 6554 6f28  .    def moveTo(
+000052a0: 7365 6c66 2c20 706f 7369 7469 6f6e 3a69  self, position:i
+000052b0: 6e74 2c20 2a2a 6b77 6172 6773 2920 2d3e  nt, **kwargs) ->
+000052c0: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
+000052d0: 2222 0d0a 2020 2020 2020 2020 4d6f 7665  ""..        Move
+000052e0: 2074 6865 2070 6c75 6e67 6572 2074 6f20   the plunger to 
+000052f0: 6120 7370 6563 6966 6965 6420 706f 7369  a specified posi
+00005300: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
+00005310: 4172 6773 3a0d 0a20 2020 2020 2020 2020  Args:..         
+00005320: 2020 2070 6f73 6974 696f 6e20 2869 6e74     position (int
+00005330: 293a 2074 6172 6765 7420 706c 756e 6765  ): target plunge
+00005340: 7220 706f 7369 7469 6f6e 0d0a 0d0a 2020  r position....  
+00005350: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00005360: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00005370: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
+00005380: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005390: 2020 2020 2020 2073 656c 662e 706f 7369         self.posi
+000053a0: 7469 6f6e 203d 2070 6f73 6974 696f 6e0d  tion = position.
+000053b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000053c0: 7365 6c66 2e5f 7175 6572 7928 6627 5250  self._query(f'RP
+000053d0: 7b70 6f73 6974 696f 6e7d 2729 0d0a 2020  {position}')..  
+000053e0: 2020 0d0a 2020 2020 6465 6620 7075 6c6c    ..    def pull
+000053f0: 6261 636b 2873 656c 662c 2073 7465 7073  back(self, steps
+00005400: 3a69 6e74 203d 2035 2c20 2a2a 6b77 6172  :int = 5, **kwar
+00005410: 6773 2920 2d3e 2073 7472 3a0d 0a20 2020  gs) -> str:..   
+00005420: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00005430: 2020 5075 6c6c 6261 636b 206c 6971 7569    Pullback liqui
+00005440: 6420 6672 6f6d 2074 6970 0d0a 2020 2020  d from tip..    
+00005450: 2020 2020 0d0a 2020 2020 2020 2020 4172      ..        Ar
+00005460: 6773 3a0d 0a20 2020 2020 2020 2020 2020  gs:..           
+00005470: 2073 7465 7073 2028 696e 742c 206f 7074   steps (int, opt
+00005480: 696f 6e61 6c29 3a20 6e75 6d62 6572 206f  ional): number o
+00005490: 6620 7374 6570 7320 746f 2070 756c 6c62  f steps to pullb
+000054a0: 6163 6b2e 2044 6566 6175 6c74 7320 746f  ack. Defaults to
+000054b0: 2035 2e0d 0a0d 0a20 2020 2020 2020 2052   5.....        R
+000054c0: 6574 7572 6e73 3a0d 0a20 2020 2020 2020  eturns:..       
+000054d0: 2020 2020 2073 7472 3a20 6465 7669 6365       str: device
+000054e0: 2072 6573 706f 6e73 650d 0a20 2020 2020   response..     
+000054f0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00005500: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
+00005510: 5f71 7565 7279 2866 2752 497b 7374 6570  _query(f'RI{step
+00005520: 737d 2729 0d0a 2020 2020 2020 2020 7365  s}')..        se
+00005530: 6c66 2e70 6f73 6974 696f 6e20 2b3d 2073  lf.position += s
+00005540: 7465 7073 0d0a 2020 2020 2020 2020 7469  teps..        ti
+00005550: 6d65 2e73 6c65 6570 2831 290d 0a20 2020  me.sleep(1)..   
+00005560: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+00005570: 6f6e 7365 0d0a 2020 2020 0d0a 2020 2020  onse..    ..    
+00005580: 6465 6620 7265 7365 7428 7365 6c66 2920  def reset(self) 
+00005590: 2d3e 2073 7472 3a0d 0a20 2020 2020 2020  -> str:..       
+000055a0: 2022 2222 0d0a 2020 2020 2020 2020 5265   """..        Re
+000055b0: 7365 7420 7468 6520 7069 7065 7474 650d  set the pipette.
+000055c0: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000055d0: 6e73 3a0d 0a20 2020 2020 2020 2020 2020  ns:..           
+000055e0: 2073 7472 3a20 6465 7669 6365 2072 6573   str: device res
+000055f0: 706f 6e73 650d 0a20 2020 2020 2020 2022  ponse..        "
+00005600: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00005610: 2e7a 6572 6f28 290d 0a20 2020 2020 2020  .zero()..       
+00005620: 2072 6574 7572 6e20 7365 6c66 2e68 6f6d   return self.hom
+00005630: 6528 290d 0a20 2020 200d 0a20 2020 2064  e()..    ..    d
+00005640: 6566 2073 6574 5370 6565 6428 7365 6c66  ef setSpeed(self
+00005650: 2c20 7370 6565 643a 696e 742c 2075 703a  , speed:int, up:
+00005660: 626f 6f6c 2c20 6465 6661 756c 743a 626f  bool, default:bo
+00005670: 6f6c 203d 2046 616c 7365 2c20 2a2a 6b77  ol = False, **kw
+00005680: 6172 6773 2920 2d3e 2073 7472 3a0d 0a20  args) -> str:.. 
+00005690: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+000056a0: 2020 2020 5365 7420 7468 6520 7370 6565      Set the spee
+000056b0: 6420 6f66 2074 6865 2070 6c75 6e67 6572  d of the plunger
+000056c0: 0d0a 0d0a 2020 2020 2020 2020 4172 6773  ....        Args
+000056d0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000056e0: 7065 6564 2028 696e 7429 3a20 7370 6565  peed (int): spee
+000056f0: 6420 6f66 2070 6c75 6e67 6572 0d0a 2020  d of plunger..  
+00005700: 2020 2020 2020 2020 2020 7570 2028 626f            up (bo
+00005710: 6f6c 293a 2064 6972 6563 7469 6f6e 206f  ol): direction o
+00005720: 6620 7472 6176 656c 0d0a 2020 2020 2020  f travel..      
+00005730: 2020 2020 2020 6465 6661 756c 7420 2862        default (b
+00005740: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
+00005750: 7768 6574 6865 7220 746f 2073 6574 2073  whether to set s
+00005760: 7065 6564 2061 7320 6120 6465 6661 756c  peed as a defaul
+00005770: 742e 2044 6566 6175 6c74 7320 746f 2046  t. Defaults to F
+00005780: 616c 7365 2e0d 0a0d 0a20 2020 2020 2020  alse.....       
+00005790: 2052 6574 7572 6e73 3a0d 0a20 2020 2020   Returns:..     
+000057a0: 2020 2020 2020 2073 7472 3a20 6465 7669         str: devi
+000057b0: 6365 2072 6573 706f 6e73 650d 0a20 2020  ce response..   
+000057c0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000057d0: 2020 7370 6565 645f 636f 6465 203d 2031    speed_code = 1
+000057e0: 202b 205b 7820 666f 7220 782c 7661 6c20   + [x for x,val 
+000057f0: 696e 2065 6e75 6d65 7261 7465 286e 702e  in enumerate(np.
+00005800: 6172 7261 7928 7365 6c66 2e73 7065 6564  array(self.speed
+00005810: 5f70 7265 7365 7473 292d 7370 6565 6429  _presets)-speed)
+00005820: 2069 6620 7661 6c20 3e3d 2030 5d5b 305d   if val >= 0][0]
+00005830: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+00005840: 6627 5370 6565 6420 7b73 7065 6564 5f63  f'Speed {speed_c
+00005850: 6f64 657d 3a20 7b73 656c 662e 7370 6565  ode}: {self.spee
+00005860: 645f 7072 6573 6574 735b 7370 6565 645f  d_presets[speed_
+00005870: 636f 6465 2d31 5d7d 2075 4c2f 7327 290d  code-1]} uL/s').
+00005880: 0a20 2020 2020 2020 2064 6972 6563 7469  .        directi
+00005890: 6f6e 203d 2027 4927 2069 6620 7570 2065  on = 'I' if up e
+000058a0: 6c73 6520 274f 270d 0a20 2020 2020 2020  lse 'O'..       
+000058b0: 2073 656c 662e 5f71 7565 7279 2866 2753   self._query(f'S
+000058c0: 7b64 6972 6563 7469 6f6e 7d7b 7370 6565  {direction}{spee
+000058d0: 645f 636f 6465 7d27 290d 0a20 2020 2020  d_code}')..     
+000058e0: 2020 2069 6620 6e6f 7420 6465 6661 756c     if not defaul
+000058f0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+00005900: 7265 7475 726e 2073 656c 662e 5f71 7565  return self._que
+00005910: 7279 2866 2744 7b64 6972 6563 7469 6f6e  ry(f'D{direction
+00005920: 7d27 290d 0a20 2020 2020 2020 2069 6620  }')..        if 
+00005930: 7570 3a0d 0a20 2020 2020 2020 2020 2020  up:..           
+00005940: 2073 656c 662e 7370 6565 645f 636f 6465   self.speed_code
+00005950: 2e75 7020 3d20 7370 6565 645f 636f 6465  .up = speed_code
+00005960: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00005970: 6c66 2e73 7065 6564 2e75 7020 3d20 7365  lf.speed.up = se
+00005980: 6c66 2e73 7065 6564 5f70 7265 7365 7473  lf.speed_presets
+00005990: 5b73 7065 6564 5f63 6f64 652d 315d 0d0a  [speed_code-1]..
+000059a0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+000059b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000059c0: 7370 6565 645f 636f 6465 2e64 6f77 6e20  speed_code.down 
+000059d0: 3d20 7370 6565 645f 636f 6465 0d0a 2020  = speed_code..  
+000059e0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000059f0: 7065 6564 2e64 6f77 6e20 3d20 7365 6c66  peed.down = self
+00005a00: 2e73 7065 6564 5f70 7265 7365 7473 5b73  .speed_presets[s
+00005a10: 7065 6564 5f63 6f64 652d 315d 0d0a 2020  peed_code-1]..  
+00005a20: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00005a30: 662e 5f71 7565 7279 2866 2744 7b64 6972  f._query(f'D{dir
+00005a40: 6563 7469 6f6e 7d27 290d 0a20 2020 200d  ection}')..    .
+00005a50: 0a20 2020 2064 6566 2073 6875 7464 6f77  .    def shutdow
+00005a60: 6e28 7365 6c66 293a 0d0a 2020 2020 2020  n(self):..      
+00005a70: 2020 2222 2253 6875 7464 6f77 6e20 7072    """Shutdown pr
+00005a80: 6f63 6564 7572 6520 666f 7220 746f 6f6c  ocedure for tool
+00005a90: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
+00005aa0: 662e 746f 6767 6c65 4665 6564 6261 636b  f.toggleFeedback
+00005ab0: 4c6f 6f70 286f 6e3d 4661 6c73 6529 0d0a  Loop(on=False)..
+00005ac0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00005ad0: 7570 6572 2829 2e73 6875 7464 6f77 6e28  uper().shutdown(
+00005ae0: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
+00005af0: 2074 6f67 676c 6546 6565 6462 6163 6b4c   toggleFeedbackL
+00005b00: 6f6f 7028 7365 6c66 2c20 6f6e 3a62 6f6f  oop(self, on:boo
+00005b10: 6c29 3a0d 0a20 2020 2020 2020 2022 2222  l):..        """
+00005b20: 0d0a 2020 2020 2020 2020 5374 6172 7420  ..        Start 
+00005b30: 6f72 2073 746f 7020 6665 6564 6261 636b  or stop feedback
+00005b40: 206c 6f6f 700d 0a20 2020 2020 2020 200d   loop..        .
+00005b50: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+00005b60: 2020 2020 2020 2020 2020 2020 6f6e 2028              on (
+00005b70: 626f 6f6c 293a 2077 6865 7468 6572 2074  bool): whether t
+00005b80: 6f20 7374 6172 7420 6665 6564 6261 636b  o start feedback
+00005b90: 206c 6f6f 700d 0a20 2020 2020 2020 2022   loop..        "
+00005ba0: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00005bb0: 2e73 6574 466c 6167 2867 6574 5f66 6565  .setFlag(get_fee
+00005bc0: 6462 6163 6b3d 6f6e 290d 0a20 2020 2020  dback=on)..     
+00005bd0: 2020 2069 6620 6f6e 3a0d 0a20 2020 2020     if on:..     
+00005be0: 2020 2020 2020 2069 6620 2766 6565 6462         if 'feedb
+00005bf0: 6163 6b5f 6c6f 6f70 2720 696e 2073 656c  ack_loop' in sel
+00005c00: 662e 5f74 6872 6561 6473 3a0d 0a20 2020  f._threads:..   
+00005c10: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00005c20: 662e 5f74 6872 6561 6473 5b27 6665 6564  f._threads['feed
+00005c30: 6261 636b 5f6c 6f6f 7027 5d2e 6a6f 696e  back_loop'].join
+00005c40: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
+00005c50: 7468 7265 6164 203d 2054 6872 6561 6428  thread = Thread(
+00005c60: 7461 7267 6574 3d73 656c 662e 5f6c 6f6f  target=self._loo
+00005c70: 705f 6665 6564 6261 636b 290d 0a20 2020  p_feedback)..   
+00005c80: 2020 2020 2020 2020 2074 6872 6561 642e           thread.
+00005c90: 7374 6172 7428 290d 0a20 2020 2020 2020  start()..       
+00005ca0: 2020 2020 2073 656c 662e 5f74 6872 6561       self._threa
+00005cb0: 6473 5b27 6665 6564 6261 636b 5f6c 6f6f  ds['feedback_loo
+00005cc0: 7027 5d20 3d20 7468 7265 6164 0d0a 2020  p'] = thread..  
+00005cd0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00005ce0: 2020 2020 2020 2020 2069 6620 2766 6565           if 'fee
+00005cf0: 6462 6163 6b5f 6c6f 6f70 2720 696e 2073  dback_loop' in s
+00005d00: 656c 662e 5f74 6872 6561 6473 3a0d 0a20  elf._threads:.. 
+00005d10: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00005d20: 656c 662e 5f74 6872 6561 6473 5b27 6665  elf._threads['fe
+00005d30: 6564 6261 636b 5f6c 6f6f 7027 5d2e 6a6f  edback_loop'].jo
+00005d40: 696e 2829 0d0a 2020 2020 2020 2020 7265  in()..        re
+00005d50: 7475 726e 0d0a 0d0a 2020 2020 6465 6620  turn....    def 
+00005d60: 7a65 726f 2873 656c 6629 202d 3e20 7374  zero(self) -> st
+00005d70: 723a 0d0a 2020 2020 2020 2020 2222 220d  r:..        """.
+00005d80: 0a20 2020 2020 2020 205a 6572 6f20 7468  .        Zero th
+00005d90: 6520 706c 756e 6765 7220 706f 7369 7469  e plunger positi
+00005da0: 6f6e 0d0a 2020 2020 2020 2020 0d0a 2020  on..        ..  
+00005db0: 2020 2020 2020 5265 7475 726e 733a 0d0a        Returns:..
+00005dc0: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00005dd0: 2064 6576 6963 6520 7265 7370 6f6e 7365   device response
+00005de0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005df0: 2020 2020 2020 2073 656c 662e 656a 6563         self.ejec
+00005e00: 7428 290d 0a20 2020 2020 2020 2072 6573  t()..        res
+00005e10: 706f 6e73 6520 3d20 7365 6c66 2e5f 7175  ponse = self._qu
+00005e20: 6572 7928 2752 5a27 290d 0a20 2020 2020  ery('RZ')..     
+00005e30: 2020 2073 656c 662e 706f 7369 7469 6f6e     self.position
+00005e40: 203d 2030 0d0a 2020 2020 2020 2020 7469   = 0..        ti
+00005e50: 6d65 2e73 6c65 6570 2832 290d 0a20 2020  me.sleep(2)..   
+00005e60: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+00005e70: 6f6e 7365 0d0a 0d0a 2020 2020 2320 5072  onse....    # Pr
+00005e80: 6f74 6563 7465 6420 6d65 7468 6f64 2873  otected method(s
+00005e90: 290d 0a20 2020 2064 6566 205f 6361 6c63  )..    def _calc
+00005ea0: 756c 6174 655f 7370 6565 645f 7061 7261  ulate_speed_para
+00005eb0: 6d65 7465 7273 2873 656c 662c 2076 6f6c  meters(self, vol
+00005ec0: 756d 653a 696e 742c 2073 7065 6564 3a69  ume:int, speed:i
+00005ed0: 6e74 2920 2d3e 206c 6962 2e53 7065 6564  nt) -> lib.Speed
+00005ee0: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
+00005ef0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00005f00: 2020 4361 6c63 756c 6174 6573 2074 6865    Calculates the
+00005f10: 2062 6573 7420 7061 7261 6d65 7465 7273   best parameters
+00005f20: 2066 6f72 2076 6f6c 756d 6520 616e 6420   for volume and 
+00005f30: 7370 6565 640d 0a0d 0a20 2020 2020 2020  speed....       
+00005f40: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00005f50: 2020 2020 766f 6c75 6d65 2028 696e 7429      volume (int)
+00005f60: 3a20 766f 6c75 6d65 2074 6f20 6265 2074  : volume to be t
+00005f70: 7261 6e73 6665 7272 6564 0d0a 2020 2020  ransferred..    
+00005f80: 2020 2020 2020 2020 7370 6565 6420 2869          speed (i
+00005f90: 6e74 293a 2073 7065 6564 2061 7420 7768  nt): speed at wh
+00005fa0: 6963 6820 6c69 7175 6964 2069 7320 7472  ich liquid is tr
+00005fb0: 616e 7366 6572 7265 640d 0a0d 0a20 2020  ansferred....   
+00005fc0: 2020 2020 2052 6574 7572 6e73 3a0d 0a20       Returns:.. 
+00005fd0: 2020 2020 2020 2020 2020 2064 6963 743a             dict:
+00005fe0: 2064 6963 7469 6f6e 6172 7920 6f66 2062   dictionary of b
+00005ff0: 6573 7420 7061 7261 6d65 7465 7273 0d0a  est parameters..
+00006000: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00006010: 2020 2020 206f 7574 636f 6d65 7320 3d20       outcomes = 
+00006020: 7b7d 0d0a 2020 2020 2020 2020 7374 6570  {}..        step
+00006030: 5f69 6e74 6572 7661 6c5f 6c69 6d69 7420  _interval_limit 
+00006040: 3d20 696e 7428 766f 6c75 6d65 2f73 656c  = int(volume/sel
+00006050: 662e 7265 736f 6c75 7469 6f6e 2f53 5445  f.resolution/STE
+00006060: 505f 5245 534f 4c55 5449 4f4e 290d 0a20  P_RESOLUTION).. 
+00006070: 2020 2020 2020 2066 6f72 2070 7265 7365         for prese
+00006080: 7420 696e 2073 656c 662e 7370 6565 645f  t in self.speed_
+00006090: 7072 6573 6574 733a 0d0a 2020 2020 2020  presets:..      
+000060a0: 2020 2020 2020 6966 2070 7265 7365 7420        if preset 
+000060b0: 3c20 7370 6565 643a 0d0a 2020 2020 2020  < speed:..      
+000060c0: 2020 2020 2020 2020 2020 2320 7072 6573            # pres
+000060d0: 6574 2069 7320 736c 6f77 6572 2074 6861  et is slower tha
+000060e0: 6e20 7461 7267 6574 2073 7065 6564 2c20  n target speed, 
+000060f0: 6974 2077 696c 6c20 6e65 7665 7220 6869  it will never hi
+00006100: 7420 7461 7267 6574 2073 7065 6564 0d0a  t target speed..
+00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006120: 636f 6e74 696e 7565 0d0a 2020 2020 2020  continue..      
+00006130: 2020 2020 2020 7469 6d65 5f69 6e74 6572        time_inter
+00006140: 7661 6c5f 6c69 6d69 7420 3d20 696e 7428  val_limit = int(
+00006150: 766f 6c75 6d65 2a28 312f 7370 6565 6420  volume*(1/speed 
+00006160: 2d20 312f 7072 6573 6574 292f 7365 6c66  - 1/preset)/self
+00006170: 2e72 6573 706f 6e73 655f 7469 6d65 290d  .response_time).
+00006180: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00006190: 6e6f 7420 7374 6570 5f69 6e74 6572 7661  not step_interva
+000061a0: 6c5f 6c69 6d69 7420 6f72 206e 6f74 2074  l_limit or not t
+000061b0: 696d 655f 696e 7465 7276 616c 5f6c 696d  ime_interval_lim
+000061c0: 6974 3a0d 0a20 2020 2020 2020 2020 2020  it:..           
+000061d0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+000061e0: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
+000061f0: 7661 6c73 203d 206d 6178 286d 696e 2873  vals = max(min(s
+00006200: 7465 705f 696e 7465 7276 616c 5f6c 696d  tep_interval_lim
+00006210: 6974 2c20 7469 6d65 5f69 6e74 6572 7661  it, time_interva
+00006220: 6c5f 6c69 6d69 7429 2c20 3129 0d0a 2020  l_limit), 1)..  
+00006230: 2020 2020 2020 2020 2020 6561 6368 5f73            each_s
+00006240: 7465 7073 203d 2076 6f6c 756d 652f 7365  teps = volume/se
+00006250: 6c66 2e72 6573 6f6c 7574 696f 6e2f 696e  lf.resolution/in
+00006260: 7465 7276 616c 730d 0a20 2020 2020 2020  tervals..       
+00006270: 2020 2020 2065 6163 685f 6465 6c61 7920       each_delay 
+00006280: 3d20 766f 6c75 6d65 2a28 312f 7370 6565  = volume*(1/spee
+00006290: 6420 2d20 312f 7072 6573 6574 292f 696e  d - 1/preset)/in
+000062a0: 7465 7276 616c 730d 0a20 2020 2020 2020  tervals..       
+000062b0: 2020 2020 2061 7265 6120 3d20 302e 3520       area = 0.5 
+000062c0: 2a20 2876 6f6c 756d 652a 2a32 2920 2a20  * (volume**2) * 
+000062d0: 2831 2f73 656c 662e 7265 736f 6c75 7469  (1/self.resoluti
+000062e0: 6f6e 2920 2a20 2831 2f69 6e74 6572 7661  on) * (1/interva
+000062f0: 6c73 2920 2a20 2831 2f73 7065 6564 202d  ls) * (1/speed -
+00006300: 2031 2f70 7265 7365 7429 0d0a 2020 2020   1/preset)..    
+00006310: 2020 2020 2020 2020 6f75 7463 6f6d 6573          outcomes
+00006320: 5b61 7265 615d 203d 206c 6962 2e53 7065  [area] = lib.Spe
+00006330: 6564 5061 7261 6d65 7465 7273 2870 7265  edParameters(pre
+00006340: 7365 742c 2069 6e74 6572 7661 6c73 2c20  set, intervals, 
+00006350: 696e 7428 6561 6368 5f73 7465 7073 292c  int(each_steps),
+00006360: 2065 6163 685f 6465 6c61 7929 0d0a 2020   each_delay)..  
+00006370: 2020 2020 2020 6966 206c 656e 286f 7574        if len(out
+00006380: 636f 6d65 7329 203d 3d20 303a 0d0a 2020  comes) == 0:..  
+00006390: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000063a0: 224e 6f20 6665 6173 6962 6c65 2073 7065  "No feasible spe
+000063b0: 6564 2070 6172 616d 6574 6572 732e 2229  ed parameters.")
+000063c0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000063d0: 7475 726e 206c 6962 2e53 7065 6564 5061  turn lib.SpeedPa
+000063e0: 7261 6d65 7465 7273 284e 6f6e 652c 2053  rameters(None, S
+000063f0: 5445 505f 5245 534f 4c55 5449 4f4e 2c20  TEP_RESOLUTION, 
+00006400: 5354 4550 5f52 4553 4f4c 5554 494f 4e2c  STEP_RESOLUTION,
+00006410: 2073 656c 662e 7265 7370 6f6e 7365 5f74   self.response_t
+00006420: 696d 6529 0d0a 2020 2020 2020 2020 7072  ime)..        pr
+00006430: 696e 7428 6627 4265 7374 2070 6172 616d  int(f'Best param
+00006440: 6574 6572 733a 207b 6f75 7463 6f6d 6573  eters: {outcomes
+00006450: 5b6d 696e 286f 7574 636f 6d65 7329 5d7d  [min(outcomes)]}
+00006460: 2729 0d0a 2020 2020 2020 2020 7265 7475  ')..        retu
+00006470: 726e 206f 7574 636f 6d65 735b 6d69 6e28  rn outcomes[min(
+00006480: 6f75 7463 6f6d 6573 295d 0d0a 2020 2020  outcomes)]..    
+00006490: 0d0a 2020 2020 6465 6620 5f63 6f6e 6e65  ..    def _conne
+000064a0: 6374 2873 656c 662c 2070 6f72 743a 7374  ct(self, port:st
+000064b0: 722c 2062 6175 6472 6174 653a 696e 7420  r, baudrate:int 
+000064c0: 3d20 3936 3030 2c20 7469 6d65 6f75 743a  = 9600, timeout:
+000064d0: 696e 7420 3d20 3129 3a0d 0a20 2020 2020  int = 1):..     
+000064e0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+000064f0: 436f 6e6e 6563 7469 6f6e 2070 726f 6365  Connection proce
+00006500: 6475 7265 2066 6f72 2074 6f6f 6c0d 0a0d  dure for tool...
+00006510: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
+00006520: 2020 2020 2020 2020 2020 2020 706f 7274              port
+00006530: 2028 7374 7229 3a20 434f 4d20 706f 7274   (str): COM port
+00006540: 2061 6464 7265 7373 0d0a 2020 2020 2020   address..      
+00006550: 2020 2020 2020 6261 7564 7261 7465 2028        baudrate (
+00006560: 696e 742c 206f 7074 696f 6e61 6c29 3a20  int, optional): 
+00006570: 6261 7564 7261 7465 2e20 4465 6661 756c  baudrate. Defaul
+00006580: 7473 2074 6f20 3936 3030 2e0d 0a20 2020  ts to 9600...   
+00006590: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+000065a0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
+000065b0: 3a20 7469 6d65 6f75 7420 696e 2073 6563  : timeout in sec
+000065c0: 6f6e 6473 2e20 4465 6661 756c 7473 2074  onds. Defaults t
+000065d0: 6f20 312e 0d0a 2020 2020 2020 2020 2222  o 1...        ""
+000065e0: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+000065f0: 636f 6e6e 6563 7469 6f6e 5f64 6574 6169  connection_detai
+00006600: 6c73 203d 207b 0d0a 2020 2020 2020 2020  ls = {..        
+00006610: 2020 2020 2770 6f72 7427 3a20 706f 7274      'port': port
+00006620: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
+00006630: 6261 7564 7261 7465 273a 2062 6175 6472  baudrate': baudr
+00006640: 6174 652c 0d0a 2020 2020 2020 2020 2020  ate,..          
+00006650: 2020 2774 696d 656f 7574 273a 2074 696d    'timeout': tim
+00006660: 656f 7574 0d0a 2020 2020 2020 2020 7d0d  eout..        }.
+00006670: 0a20 2020 2020 2020 2064 6576 6963 6520  .        device 
+00006680: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
+00006690: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000066a0: 2020 6465 7669 6365 203d 2073 6572 6961    device = seria
+000066b0: 6c2e 5365 7269 616c 2870 6f72 742c 2062  l.Serial(port, b
+000066c0: 6175 6472 6174 652c 2074 696d 656f 7574  audrate, timeout
+000066d0: 3d74 696d 656f 7574 290d 0a20 2020 2020  =timeout)..     
+000066e0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+000066f0: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+00006700: 2020 2020 2020 2070 7269 6e74 2866 2243         print(f"C
+00006710: 6f75 6c64 206e 6f74 2063 6f6e 6e65 6374  ould not connect
+00006720: 2074 6f20 7b70 6f72 747d 2229 0d0a 2020   to {port}")..  
+00006730: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00006740: 662e 7665 7262 6f73 653a 0d0a 2020 2020  f.verbose:..    
+00006750: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00006760: 7428 6529 0d0a 2020 2020 2020 2020 656c  t(e)..        el
+00006770: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
+00006780: 2074 696d 652e 736c 6565 7028 3229 2020   time.sleep(2)  
+00006790: 2023 2057 6169 7420 666f 7220 6772 626c   # Wait for grbl
+000067a0: 2074 6f20 696e 6974 6961 6c69 7a65 0d0a   to initialize..
+000067b0: 2020 2020 2020 2020 2020 2020 6465 7669              devi
+000067c0: 6365 2e66 6c75 7368 496e 7075 7428 290d  ce.flushInput().
+000067d0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000067e0: 6e74 2866 2243 6f6e 6e65 6374 696f 6e20  nt(f"Connection 
+000067f0: 6f70 656e 6564 2074 6f20 7b70 6f72 747d  opened to {port}
+00006800: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00006810: 7365 6c66 2e73 6574 466c 6167 2863 6f6e  self.setFlag(con
+00006820: 6e65 6374 6564 3d54 7275 6529 0d0a 2020  nected=True)..  
+00006830: 2020 2020 2020 7365 6c66 2e64 6576 6963        self.devic
+00006840: 6520 3d20 6465 7669 6365 0d0a 2020 2020  e = device..    
+00006850: 2020 2020 7365 6c66 2e67 6574 496e 666f      self.getInfo
+00006860: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+00006870: 2e72 6573 6574 2829 0d0a 2020 2020 2020  .reset()..      
+00006880: 2020 7265 7475 726e 0d0a 2020 2020 0d0a    return..    ..
+00006890: 2020 2020 6465 6620 5f69 735f 6578 7065      def _is_expe
+000068a0: 6374 6564 5f72 6570 6c79 2873 656c 662c  cted_reply(self,
+000068b0: 2072 6573 706f 6e73 653a 7374 722c 2063   response:str, c
+000068c0: 6f6d 6d61 6e64 5f63 6f64 653a 7374 722c  ommand_code:str,
+000068d0: 202a 2a6b 7761 7267 7329 202d 3e20 626f   **kwargs) -> bo
+000068e0: 6f6c 3a0d 0a20 2020 2020 2020 2022 2222  ol:..        """
+000068f0: 0d0a 2020 2020 2020 2020 4368 6563 6b73  ..        Checks
+00006900: 2061 6e64 2072 6574 7572 6e73 2077 6865   and returns whe
+00006910: 7468 6572 2074 6865 2072 6573 706f 6e73  ther the respons
+00006920: 6520 6973 2061 6e20 6578 7065 6374 6564  e is an expected
+00006930: 2072 6570 6c79 0d0a 0d0a 2020 2020 2020   reply....      
+00006940: 2020 4172 6773 3a0d 0a20 2020 2020 2020    Args:..       
+00006950: 2020 2020 2072 6573 706f 6e73 6520 2873       response (s
+00006960: 7472 293a 2072 6573 706f 6e73 6520 7374  tr): response st
+00006970: 7269 6e67 2066 726f 6d20 6465 7669 6365  ring from device
+00006980: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00006990: 6d6d 616e 645f 636f 6465 2028 7374 7229  mmand_code (str)
+000069a0: 3a20 7477 6f2d 6368 6172 6163 7465 7220  : two-character 
+000069b0: 636f 6d6d 616e 6420 636f 6465 0d0a 0d0a  command code....
+000069c0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+000069d0: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
+000069e0: 6f6c 3a20 7768 6574 6865 7220 7468 6520  ol: whether the 
+000069f0: 7265 7370 6f6e 7365 2069 7320 616e 2065  response is an e
+00006a00: 7870 6563 7465 6420 7265 706c 790d 0a20  xpected reply.. 
+00006a10: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00006a20: 2020 2020 6966 2072 6573 706f 6e73 6520      if response 
+00006a30: 696e 206c 6962 2e45 7272 6f72 436f 6465  in lib.ErrorCode
+00006a40: 2e5f 6d65 6d62 6572 5f6e 616d 6573 5f3a  ._member_names_:
+00006a50: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00006a60: 7475 726e 2054 7275 650d 0a20 2020 2020  turn True..     
+00006a70: 2020 2069 6620 636f 6d6d 616e 645f 636f     if command_co
+00006a80: 6465 206e 6f74 2069 6e20 5155 4552 4945  de not in QUERIE
+00006a90: 5320 616e 6420 7265 7370 6f6e 7365 203d  S and response =
+00006aa0: 3d20 276f 6b27 3a0d 0a20 2020 2020 2020  = 'ok':..       
+00006ab0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00006ac0: 0d0a 2020 2020 2020 2020 6966 2063 6f6d  ..        if com
+00006ad0: 6d61 6e64 5f63 6f64 6520 696e 2051 5545  mand_code in QUE
+00006ae0: 5249 4553 2061 6e64 2072 6573 706f 6e73  RIES and respons
+00006af0: 655b 3a32 5d20 3d3d 2063 6f6d 6d61 6e64  e[:2] == command
+00006b00: 5f63 6f64 652e 6c6f 7765 7228 293a 0d0a  _code.lower():..
+00006b10: 2020 2020 2020 2020 2020 2020 7265 706c              repl
+00006b20: 795f 636f 6465 2c20 6461 7461 203d 2072  y_code, data = r
+00006b30: 6573 706f 6e73 655b 3a32 5d2c 2072 6573  esponse[:2], res
+00006b40: 706f 6e73 655b 323a 5d0d 0a20 2020 2020  ponse[2:]..     
+00006b50: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+00006b60: 6572 626f 7365 3a0d 0a20 2020 2020 2020  erbose:..       
+00006b70: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+00006b80: 275b 7b72 6570 6c79 5f63 6f64 657d 5d20  '[{reply_code}] 
+00006b90: 7b64 6174 617d 2729 0d0a 2020 2020 2020  {data}')..      
+00006ba0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00006bb0: 650d 0a20 2020 2020 2020 2072 6574 7572  e..        retur
+00006bc0: 6e20 4661 6c73 650d 0a0d 0a20 2020 2064  n False....    d
+00006bd0: 6566 205f 6c6f 6f70 5f66 6565 6462 6163  ef _loop_feedbac
+00006be0: 6b28 7365 6c66 293a 0d0a 2020 2020 2020  k(self):..      
+00006bf0: 2020 2222 224c 6f6f 7020 746f 2063 6f6e    """Loop to con
+00006c00: 7374 616e 746c 7920 7265 6164 2066 726f  stantly read fro
+00006c10: 6d20 6465 7669 6365 2222 220d 0a20 2020  m device"""..   
+00006c20: 2020 2020 2070 7269 6e74 2827 4c69 7374       print('List
+00006c30: 656e 696e 672e 2e2e 2729 0d0a 2020 2020  ening...')..    
+00006c40: 2020 2020 7768 696c 6520 7365 6c66 2e66      while self.f
+00006c50: 6c61 6773 5b27 6765 745f 6665 6564 6261  lags['get_feedba
+00006c60: 636b 275d 3a0d 0a20 2020 2020 2020 2020  ck']:..         
+00006c70: 2020 2069 6620 7365 6c66 2e66 6c61 6773     if self.flags
+00006c80: 5b27 7061 7573 655f 6665 6564 6261 636b  ['pause_feedback
+00006c90: 275d 3a0d 0a20 2020 2020 2020 2020 2020  ']:..           
+00006ca0: 2020 2020 2063 6f6e 7469 6e75 650d 0a20       continue.. 
+00006cb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006cc0: 6765 7453 7461 7475 7328 290d 0a20 2020  getStatus()..   
+00006cd0: 2020 2020 2020 2020 2073 656c 662e 6765           self.ge
+00006ce0: 7443 6170 6163 6974 616e 6365 2829 0d0a  tCapacitance()..
+00006cf0: 2020 2020 2020 2020 7072 696e 7428 2753          print('S
+00006d00: 746f 7020 6c69 7374 656e 696e 672e 2e2e  top listening...
+00006d10: 2729 0d0a 2020 2020 2020 2020 7265 7475  ')..        retu
+00006d20: 726e 0d0a 2020 2020 0d0a 2020 2020 6465  rn..    ..    de
+00006d30: 6620 5f71 7565 7279 2873 656c 662c 200d  f _query(self, .
+00006d40: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
+00006d50: 3a20 7374 722c 200d 0a20 2020 2020 2020  : str, ..       
+00006d60: 2074 696d 656f 7574 5f73 3a20 666c 6f61   timeout_s: floa
+00006d70: 7420 3d20 302e 332c 200d 0a20 2020 2020  t = 0.3, ..     
+00006d80: 2020 2072 6573 756d 655f 6665 6564 6261     resume_feedba
+00006d90: 636b 3a20 626f 6f6c 203d 2046 616c 7365  ck: bool = False
+00006da0: 2c0d 0a20 2020 2020 2020 2067 6574 5f70  ,..        get_p
+00006db0: 6f73 6974 696f 6e3a 2062 6f6f 6c20 3d20  osition: bool = 
+00006dc0: 5472 7565 0d0a 2020 2020 2920 2d3e 2073  True..    ) -> s
+00006dd0: 7472 3a0d 0a20 2020 2020 2020 2022 2222  tr:..        """
+00006de0: 0d0a 2020 2020 2020 2020 5772 6974 6520  ..        Write 
+00006df0: 636f 6d6d 616e 6420 746f 2061 6e64 2072  command to and r
+00006e00: 6561 6420 7265 7370 6f6e 7365 2066 726f  ead response fro
+00006e10: 6d20 6465 7669 6365 0d0a 0d0a 2020 2020  m device....    
+00006e20: 2020 2020 4172 6773 3a0d 0a20 2020 2020      Args:..     
+00006e30: 2020 2020 2020 2063 6f6d 6d61 6e64 2028         command (
+00006e40: 7374 7229 3a20 636f 6d6d 616e 6420 7374  str): command st
+00006e50: 7269 6e67 0d0a 2020 2020 2020 2020 2020  ring..          
+00006e60: 2020 7469 6d65 6f75 745f 7320 2866 6c6f    timeout_s (flo
+00006e70: 6174 2c20 6f70 7469 6f6e 616c 293a 2064  at, optional): d
+00006e80: 7572 6174 696f 6e20 746f 2077 6169 7420  uration to wait 
+00006e90: 6265 666f 7265 2074 696d 656f 7574 2e20  before timeout. 
+00006ea0: 4465 6661 756c 7473 2074 6f20 302e 332e  Defaults to 0.3.
+00006eb0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00006ec0: 7375 6d65 5f66 6565 6462 6163 6b20 2862  sume_feedback (b
+00006ed0: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
+00006ee0: 7768 6574 6865 7220 746f 2072 6573 756d  whether to resum
+00006ef0: 6520 7265 6164 696e 6720 6672 6f6d 2064  e reading from d
+00006f00: 6576 6963 652e 2044 6566 6175 6c74 7320  evice. Defaults 
+00006f10: 746f 2046 616c 7365 2e0d 0a20 2020 2020  to False...     
+00006f20: 2020 2020 2020 2067 6574 5f70 6f73 6974         get_posit
+00006f30: 696f 6e20 2862 6f6f 6c2c 206f 7074 696f  ion (bool, optio
+00006f40: 6e61 6c29 3a20 7768 6574 6865 7220 746f  nal): whether to
+00006f50: 2067 6574 2074 6865 2070 6f73 6974 696f   get the positio
+00006f60: 6e20 6f66 2074 6865 2070 6c75 6e67 6572  n of the plunger
+00006f70: 2e20 4465 6661 756c 7473 2074 6f20 5472  . Defaults to Tr
+00006f80: 7565 2e0d 0a20 2020 2020 2020 2052 6574  ue...        Ret
+00006f90: 7572 6e73 3a0d 0a20 2020 2020 2020 2020  urns:..         
+00006fa0: 2020 2073 7472 3a20 7265 7370 6f6e 7365     str: response
+00006fb0: 2073 7472 696e 670d 0a20 2020 2020 2020   string..       
+00006fc0: 2022 2222 0d0a 2020 2020 2020 2020 636f   """..        co
+00006fd0: 6d6d 616e 645f 636f 6465 203d 2063 6f6d  mmand_code = com
+00006fe0: 6d61 6e64 5b3a 325d 0d0a 2020 2020 2020  mand[:2]..      
+00006ff0: 2020 6966 2063 6f6d 6d61 6e64 5f63 6f64    if command_cod
+00007000: 6520 6e6f 7420 696e 206c 6962 2e53 7461  e not in lib.Sta
+00007010: 7475 7351 7565 7279 436f 6465 2e5f 6d65  tusQueryCode._me
+00007020: 6d62 6572 5f6e 616d 6573 5f3a 0d0a 2020  mber_names_:..  
+00007030: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00007040: 662e 666c 6167 735b 2767 6574 5f66 6565  f.flags['get_fee
+00007050: 6462 6163 6b27 5d20 616e 6420 6e6f 7420  dback'] and not 
+00007060: 7365 6c66 2e66 6c61 6773 5b27 7061 7573  self.flags['paus
+00007070: 655f 6665 6564 6261 636b 275d 3a0d 0a20  e_feedback']:.. 
+00007080: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007090: 656c 662e 7365 7446 6c61 6728 7061 7573  elf.setFlag(paus
+000070a0: 655f 6665 6564 6261 636b 3d54 7275 6529  e_feedback=True)
+000070b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000070c0: 2020 7469 6d65 2e73 6c65 6570 2874 696d    time.sleep(tim
+000070d0: 656f 7574 5f73 290d 0a20 2020 2020 2020  eout_s)..       
+000070e0: 2020 2020 2023 2073 656c 662e 6765 7453       # self.getS
+000070f0: 7461 7475 7328 290d 0a20 2020 2020 2020  tatus()..       
+00007100: 2020 2020 2023 2077 6869 6c65 2073 656c       # while sel
+00007110: 662e 6973 4275 7379 2829 3a0d 0a20 2020  f.isBusy():..   
+00007120: 2020 2020 2020 2020 2023 2020 2020 2073           #     s
+00007130: 656c 662e 6765 7453 7461 7475 7328 290d  elf.getStatus().
+00007140: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00007150: 7365 6c66 2e69 7342 7573 7928 293a 0d0a  self.isBusy():..
+00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007170: 7469 6d65 2e73 6c65 6570 2874 696d 656f  time.sleep(timeo
+00007180: 7574 5f73 290d 0a20 2020 2020 2020 200d  ut_s)..        .
+00007190: 0a20 2020 2020 2020 2073 7461 7274 5f74  .        start_t
+000071a0: 696d 6520 3d20 7469 6d65 2e70 6572 665f  ime = time.perf_
+000071b0: 636f 756e 7465 7228 290d 0a20 2020 2020  counter()..     
+000071c0: 2020 2073 656c 662e 5f77 7269 7465 2863     self._write(c
+000071d0: 6f6d 6d61 6e64 290d 0a20 2020 2020 2020  ommand)..       
+000071e0: 2072 6573 706f 6e73 6520 3d20 2727 0d0a   response = ''..
+000071f0: 2020 2020 2020 2020 7768 696c 6520 6e6f          while no
+00007200: 7420 7365 6c66 2e5f 6973 5f65 7870 6563  t self._is_expec
+00007210: 7465 645f 7265 706c 7928 7265 7370 6f6e  ted_reply(respon
+00007220: 7365 2c20 636f 6d6d 616e 645f 636f 6465  se, command_code
+00007230: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00007240: 6966 2074 696d 652e 7065 7266 5f63 6f75  if time.perf_cou
+00007250: 6e74 6572 2829 202d 2073 7461 7274 5f74  nter() - start_t
+00007260: 696d 6520 3e20 7469 6d65 6f75 745f 733a  ime > timeout_s:
+00007270: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007280: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
+00007290: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+000072a0: 7365 6c66 2e5f 7265 6164 2829 0d0a 2020  self._read()..  
+000072b0: 2020 2020 2020 2320 7072 696e 7428 7469        # print(ti
+000072c0: 6d65 2e70 6572 665f 636f 756e 7465 7228  me.perf_counter(
+000072d0: 2920 2d20 7374 6172 745f 7469 6d65 290d  ) - start_time).
+000072e0: 0a20 2020 2020 2020 2069 6620 636f 6d6d  .        if comm
+000072f0: 616e 645f 636f 6465 2069 6e20 5155 4552  and_code in QUER
+00007300: 4945 533a 0d0a 2020 2020 2020 2020 2020  IES:..          
+00007310: 2020 7265 7370 6f6e 7365 203d 2072 6573    response = res
+00007320: 706f 6e73 655b 323a 5d0d 0a20 2020 2020  ponse[2:]..     
+00007330: 2020 2069 6620 636f 6d6d 616e 645f 636f     if command_co
+00007340: 6465 206e 6f74 2069 6e20 6c69 622e 5374  de not in lib.St
+00007350: 6174 7573 5175 6572 7943 6f64 652e 5f6d  atusQueryCode._m
+00007360: 656d 6265 725f 6e61 6d65 735f 3a0d 0a20  ember_names_:.. 
+00007370: 2020 2020 2020 2020 2020 2069 6620 6765             if ge
+00007380: 745f 706f 7369 7469 6f6e 3a0d 0a20 2020  t_position:..   
+00007390: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000073a0: 662e 6765 7450 6f73 6974 696f 6e28 290d  f.getPosition().
+000073b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000073c0: 7265 7375 6d65 5f66 6565 6462 6163 6b3a  resume_feedback:
+000073d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000073e0: 2020 7365 6c66 2e73 6574 466c 6167 2870    self.setFlag(p
+000073f0: 6175 7365 5f66 6565 6462 6163 6b3d 4661  ause_feedback=Fa
+00007400: 6c73 6529 0d0a 2020 2020 2020 2020 7265  lse)..        re
+00007410: 7475 726e 2072 6573 706f 6e73 650d 0a0d  turn response...
+00007420: 0a20 2020 2064 6566 205f 7265 6164 2873  .    def _read(s
+00007430: 656c 6629 202d 3e20 7374 723a 0d0a 2020  elf) -> str:..  
 00007440: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00007450: 2020 2072 6573 706f 6e73 6520 3d20 2727     response = ''
-00007460: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
-00007470: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-00007480: 6f6e 7365 203d 2073 656c 662e 6465 7669  onse = self.devi
-00007490: 6365 2e72 6561 646c 696e 6528 290d 0a20  ce.readline().. 
-000074a0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-000074b0: 6e28 7265 7370 6f6e 7365 2920 3d3d 2030  n(response) == 0
-000074c0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000074d0: 2020 2072 6573 706f 6e73 6520 3d20 7365     response = se
-000074e0: 6c66 2e64 6576 6963 652e 7265 6164 6c69  lf.device.readli
-000074f0: 6e65 2829 0d0a 2020 2020 2020 2020 2020  ne()..          
-00007500: 2020 7265 7370 6f6e 7365 203d 2072 6573    response = res
-00007510: 706f 6e73 655b 323a 2d32 5d2e 6465 636f  ponse[2:-2].deco
-00007520: 6465 2827 7574 662d 3827 290d 0a20 2020  de('utf-8')..   
-00007530: 2020 2020 2065 7863 6570 7420 4174 7472       except Attr
-00007540: 6962 7574 6545 7272 6f72 3a0d 0a20 2020  ibuteError:..   
-00007550: 2020 2020 2020 2020 2070 6173 730d 0a20           pass.. 
-00007560: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00007570: 6365 7074 696f 6e20 6173 2065 3a0d 0a20  ception as e:.. 
-00007580: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00007590: 6c66 2e76 6572 626f 7365 3a0d 0a20 2020  lf.verbose:..   
-000075a0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000075b0: 6e74 2865 290d 0a20 2020 2020 2020 2069  nt(e)..        i
-000075c0: 6620 7265 7370 6f6e 7365 2069 6e20 4572  f response in Er
-000075d0: 726f 7243 6f64 652e 5f6d 656d 6265 725f  rorCode._member_
-000075e0: 6e61 6d65 735f 3a0d 0a20 2020 2020 2020  names_:..       
-000075f0: 2020 2020 2070 7269 6e74 2845 7272 6f72       print(Error
-00007600: 436f 6465 5b72 6573 706f 6e73 655d 2e76  Code[response].v
-00007610: 616c 7565 290d 0a20 2020 2020 2020 2072  alue)..        r
-00007620: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00007630: 2020 2020 0d0a 2020 2020 6465 6620 5f73      ..    def _s
-00007640: 6574 5f63 6861 6e6e 656c 5f69 6428 7365  et_channel_id(se
-00007650: 6c66 2c20 6e65 775f 6368 616e 6e65 6c5f  lf, new_channel_
-00007660: 6964 3a69 6e74 293a 0d0a 2020 2020 2020  id:int):..      
-00007670: 2020 2222 220d 0a20 2020 2020 2020 2053    """..        S
-00007680: 6574 2063 6861 6e6e 656c 2069 6420 6f66  et channel id of
-00007690: 2064 6576 6963 650d 0a0d 0a20 2020 2020   device....     
-000076a0: 2020 2041 7267 733a 0d0a 2020 2020 2020     Args:..      
-000076b0: 2020 2020 2020 6e65 775f 6368 616e 6e65        new_channe
-000076c0: 6c20 2869 6e74 293a 206e 6577 2063 6861  l (int): new cha
-000076d0: 6e6e 656c 2069 640d 0a0d 0a20 2020 2020  nnel id....     
-000076e0: 2020 2052 6169 7365 733a 0d0a 2020 2020     Raises:..    
-000076f0: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
-00007700: 6f72 3a20 506c 6561 7365 2073 656c 6563  or: Please selec
-00007710: 7420 6120 7661 6c69 6420 724c 696e 6520  t a valid rLine 
-00007720: 6164 6472 6573 7320 6672 6f6d 2031 2074  address from 1 t
-00007730: 6f20 390d 0a20 2020 2020 2020 2022 2222  o 9..        """
-00007740: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-00007750: 2028 3020 3c20 6e65 775f 6368 616e 6e65   (0 < new_channe
-00007760: 6c5f 6964 203c 2031 3029 3a0d 0a20 2020  l_id < 10):..   
-00007770: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-00007780: 616c 7565 4572 726f 7228 2750 6c65 6173  alueError('Pleas
-00007790: 6520 7365 6c65 6374 2061 2076 616c 6964  e select a valid
-000077a0: 2072 4c69 6e65 2061 6464 7265 7373 2066   rLine address f
-000077b0: 726f 6d20 3120 746f 2039 2e27 290d 0a20  rom 1 to 9.').. 
-000077c0: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-000077d0: 3d20 7365 6c66 2e5f 7175 6572 7928 6627  = self._query(f'
-000077e0: 2a41 7b6e 6577 5f63 6861 6e6e 656c 5f69  *A{new_channel_i
-000077f0: 647d 2729 0d0a 2020 2020 2020 2020 6966  d}')..        if
-00007800: 2072 6573 706f 6e73 6520 3d3d 2027 6f6b   response == 'ok
-00007810: 273a 0d0a 2020 2020 2020 2020 2020 2020  ':..            
-00007820: 7365 6c66 2e63 6861 6e6e 656c 203d 206e  self.channel = n
-00007830: 6577 5f63 6861 6e6e 656c 5f69 640d 0a20  ew_channel_id.. 
-00007840: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
-00007850: 2020 200d 0a20 2020 2064 6566 205f 7772     ..    def _wr
-00007860: 6974 6528 7365 6c66 2c20 636f 6d6d 616e  ite(self, comman
-00007870: 643a 7374 7229 202d 3e20 626f 6f6c 3a0d  d:str) -> bool:.
-00007880: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00007890: 2020 2020 2020 5772 6974 6520 636f 6d6d        Write comm
-000078a0: 616e 6420 746f 2064 6576 6963 650d 0a0d  and to device...
-000078b0: 0a20 2020 2020 2020 2041 7267 733a 0d0a  .        Args:..
-000078c0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
-000078d0: 616e 6420 2873 7472 293a 203c 636f 6d6d  and (str): <comm
-000078e0: 616e 6420 636f 6465 3e3c 7661 6c75 653e  and code><value>
-000078f0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-00007900: 726e 733a 0d0a 2020 2020 2020 2020 2020  rns:..          
-00007910: 2020 626f 6f6c 3a20 7768 6574 6865 7220    bool: whether 
-00007920: 636f 6d6d 616e 6420 7761 7320 7365 6e74  command was sent
-00007930: 2073 7563 6365 7373 6675 6c6c 790d 0a20   successfully.. 
-00007940: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00007950: 2020 2020 6966 2073 656c 662e 7665 7262      if self.verb
-00007960: 6f73 653a 0d0a 2020 2020 2020 2020 2020  ose:..          
-00007970: 2020 7072 696e 7428 636f 6d6d 616e 6429    print(command)
-00007980: 0d0a 2020 2020 2020 2020 6673 7472 696e  ..        fstrin
-00007990: 6720 3d20 6627 017b 7365 6c66 2e63 6861  g = f'.{self.cha
-000079a0: 6e6e 656c 7d7b 636f 6d6d 616e 647d c2ba  nnel}{command}..
-000079b0: 5c72 2720 2320 636f 6d6d 616e 6420 7465  \r' # command te
-000079c0: 6d70 6c61 7465 3a20 3c50 5245 3e3c 4144  mplate: <PRE><AD
-000079d0: 523e 3c43 4f44 453e 3c44 4154 413e 3c4c  R><CODE><DATA><L
-000079e0: 5243 3e3c 504f 5354 3e0d 0a20 2020 2020  RC><POST>..     
-000079f0: 2020 2023 2062 7374 7269 6e67 203d 2062     # bstring = b
-00007a00: 7974 6561 7272 6179 2e66 726f 6d68 6578  ytearray.fromhex
-00007a10: 2866 7374 7269 6e67 2e65 6e63 6f64 6528  (fstring.encode(
-00007a20: 2775 7466 2d38 2729 2e68 6578 2829 290d  'utf-8').hex()).
-00007a30: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
-00007a40: 2020 2020 2020 2020 2020 2023 2054 7970             # Typ
-00007a50: 6963 616c 2074 696d 656f 7574 2077 6169  ical timeout wai
-00007a60: 7420 6973 2034 3030 6d73 0d0a 2020 2020  t is 400ms..    
-00007a70: 2020 2020 2020 2020 7365 6c66 2e64 6576          self.dev
-00007a80: 6963 652e 7772 6974 6528 6673 7472 696e  ice.write(fstrin
-00007a90: 672e 656e 636f 6465 2827 7574 662d 3827  g.encode('utf-8'
-00007aa0: 2929 0d0a 2020 2020 2020 2020 6578 6365  ))..        exce
-00007ab0: 7074 2041 7474 7269 6275 7465 4572 726f  pt AttributeErro
-00007ac0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
-00007ad0: 7061 7373 0d0a 2020 2020 2020 2020 6578  pass..        ex
-00007ae0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-00007af0: 7320 653a 0d0a 2020 2020 2020 2020 2020  s e:..          
-00007b00: 2020 6966 2073 656c 662e 7665 7262 6f73    if self.verbos
-00007b10: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00007b20: 2020 2020 7072 696e 7428 6529 0d0a 2020      print(e)..  
-00007b30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007b40: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00007b50: 7265 7475 726e 2054 7275 650d 0a20 2020  return True..   
-00007b60: 20                                        
+00007450: 2020 2052 6561 6420 7265 7370 6f6e 7365     Read response
+00007460: 2066 726f 6d20 6465 7669 6365 0d0a 0d0a   from device....
+00007470: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00007480: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+00007490: 723a 2072 6573 706f 6e73 6520 7374 7269  r: response stri
+000074a0: 6e67 0d0a 2020 2020 2020 2020 2222 220d  ng..        """.
+000074b0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+000074c0: 6520 3d20 2727 0d0a 2020 2020 2020 2020  e = ''..        
+000074d0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000074e0: 2020 7265 7370 6f6e 7365 203d 2073 656c    response = sel
+000074f0: 662e 6465 7669 6365 2e72 6561 646c 696e  f.device.readlin
+00007500: 6528 290d 0a20 2020 2020 2020 2020 2020  e()..           
+00007510: 2069 6620 6c65 6e28 7265 7370 6f6e 7365   if len(response
+00007520: 2920 3d3d 2030 3a0d 0a20 2020 2020 2020  ) == 0:..       
+00007530: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+00007540: 6520 3d20 7365 6c66 2e64 6576 6963 652e  e = self.device.
+00007550: 7265 6164 6c69 6e65 2829 0d0a 2020 2020  readline()..    
+00007560: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00007570: 203d 2072 6573 706f 6e73 655b 323a 2d32   = response[2:-2
+00007580: 5d2e 6465 636f 6465 2827 7574 662d 3827  ].decode('utf-8'
+00007590: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+000075a0: 7420 4174 7472 6962 7574 6545 7272 6f72  t AttributeError
+000075b0: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+000075c0: 6173 730d 0a20 2020 2020 2020 2065 7863  ass..        exc
+000075d0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+000075e0: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
+000075f0: 2069 6620 7365 6c66 2e76 6572 626f 7365   if self.verbose
+00007600: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00007610: 2020 2070 7269 6e74 2865 290d 0a20 2020     print(e)..   
+00007620: 2020 2020 2069 6620 7265 7370 6f6e 7365       if response
+00007630: 2069 6e20 6c69 622e 4572 726f 7243 6f64   in lib.ErrorCod
+00007640: 652e 5f6d 656d 6265 725f 6e61 6d65 735f  e._member_names_
+00007650: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00007660: 7269 6e74 286c 6962 2e45 7272 6f72 436f  rint(lib.ErrorCo
+00007670: 6465 5b72 6573 706f 6e73 655d 2e76 616c  de[response].val
+00007680: 7565 290d 0a20 2020 2020 2020 2072 6574  ue)..        ret
+00007690: 7572 6e20 7265 7370 6f6e 7365 0d0a 2020  urn response..  
+000076a0: 2020 0d0a 2020 2020 6465 6620 5f73 6574    ..    def _set
+000076b0: 5f63 6861 6e6e 656c 5f69 6428 7365 6c66  _channel_id(self
+000076c0: 2c20 6e65 775f 6368 616e 6e65 6c5f 6964  , new_channel_id
+000076d0: 3a69 6e74 293a 0d0a 2020 2020 2020 2020  :int):..        
+000076e0: 2222 220d 0a20 2020 2020 2020 2053 6574  """..        Set
+000076f0: 2063 6861 6e6e 656c 2069 6420 6f66 2064   channel id of d
+00007700: 6576 6963 650d 0a0d 0a20 2020 2020 2020  evice....       
+00007710: 2041 7267 733a 0d0a 2020 2020 2020 2020   Args:..        
+00007720: 2020 2020 6e65 775f 6368 616e 6e65 6c20      new_channel 
+00007730: 2869 6e74 293a 206e 6577 2063 6861 6e6e  (int): new chann
+00007740: 656c 2069 640d 0a0d 0a20 2020 2020 2020  el id....       
+00007750: 2052 6169 7365 733a 0d0a 2020 2020 2020   Raises:..      
+00007760: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
+00007770: 3a20 506c 6561 7365 2073 656c 6563 7420  : Please select 
+00007780: 6120 7661 6c69 6420 724c 696e 6520 6164  a valid rLine ad
+00007790: 6472 6573 7320 6672 6f6d 2031 2074 6f20  dress from 1 to 
+000077a0: 390d 0a20 2020 2020 2020 2022 2222 0d0a  9..        """..
+000077b0: 2020 2020 2020 2020 6966 206e 6f74 2028          if not (
+000077c0: 3020 3c20 6e65 775f 6368 616e 6e65 6c5f  0 < new_channel_
+000077d0: 6964 203c 2031 3029 3a0d 0a20 2020 2020  id < 10):..     
+000077e0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+000077f0: 7565 4572 726f 7228 2750 6c65 6173 6520  ueError('Please 
+00007800: 7365 6c65 6374 2061 2076 616c 6964 2072  select a valid r
+00007810: 4c69 6e65 2061 6464 7265 7373 2066 726f  Line address fro
+00007820: 6d20 3120 746f 2039 2e27 290d 0a20 2020  m 1 to 9.')..   
+00007830: 2020 2020 2072 6573 706f 6e73 6520 3d20       response = 
+00007840: 7365 6c66 2e5f 7175 6572 7928 6627 2a41  self._query(f'*A
+00007850: 7b6e 6577 5f63 6861 6e6e 656c 5f69 647d  {new_channel_id}
+00007860: 2729 0d0a 2020 2020 2020 2020 6966 2072  ')..        if r
+00007870: 6573 706f 6e73 6520 3d3d 2027 6f6b 273a  esponse == 'ok':
+00007880: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00007890: 6c66 2e63 6861 6e6e 656c 203d 206e 6577  lf.channel = new
+000078a0: 5f63 6861 6e6e 656c 5f69 640d 0a20 2020  _channel_id..   
+000078b0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+000078c0: 200d 0a20 2020 2064 6566 205f 7772 6974   ..    def _writ
+000078d0: 6528 7365 6c66 2c20 636f 6d6d 616e 643a  e(self, command:
+000078e0: 7374 7229 202d 3e20 626f 6f6c 3a0d 0a20  str) -> bool:.. 
+000078f0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00007900: 2020 2020 5772 6974 6520 636f 6d6d 616e      Write comman
+00007910: 6420 746f 2064 6576 6963 650d 0a0d 0a20  d to device.... 
+00007920: 2020 2020 2020 2041 7267 733a 0d0a 2020         Args:..  
+00007930: 2020 2020 2020 2020 2020 636f 6d6d 616e            comman
+00007940: 6420 2873 7472 293a 203c 636f 6d6d 616e  d (str): <comman
+00007950: 6420 636f 6465 3e3c 7661 6c75 653e 0d0a  d code><value>..
+00007960: 0d0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00007970: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00007980: 626f 6f6c 3a20 7768 6574 6865 7220 636f  bool: whether co
+00007990: 6d6d 616e 6420 7761 7320 7365 6e74 2073  mmand was sent s
+000079a0: 7563 6365 7373 6675 6c6c 790d 0a20 2020  uccessfully..   
+000079b0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000079c0: 2020 6966 2073 656c 662e 7665 7262 6f73    if self.verbos
+000079d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000079e0: 7072 696e 7428 636f 6d6d 616e 6429 0d0a  print(command)..
+000079f0: 2020 2020 2020 2020 6673 7472 696e 6720          fstring 
+00007a00: 3d20 6627 017b 7365 6c66 2e63 6861 6e6e  = f'.{self.chann
+00007a10: 656c 7d7b 636f 6d6d 616e 647d c2ba 5c72  el}{command}..\r
+00007a20: 2720 2320 636f 6d6d 616e 6420 7465 6d70  ' # command temp
+00007a30: 6c61 7465 3a20 3c50 5245 3e3c 4144 523e  late: <PRE><ADR>
+00007a40: 3c43 4f44 453e 3c44 4154 413e 3c4c 5243  <CODE><DATA><LRC
+00007a50: 3e3c 504f 5354 3e0d 0a20 2020 2020 2020  ><POST>..       
+00007a60: 2023 2062 7374 7269 6e67 203d 2062 7974   # bstring = byt
+00007a70: 6561 7272 6179 2e66 726f 6d68 6578 2866  earray.fromhex(f
+00007a80: 7374 7269 6e67 2e65 6e63 6f64 6528 2775  string.encode('u
+00007a90: 7466 2d38 2729 2e68 6578 2829 290d 0a20  tf-8').hex()).. 
+00007aa0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00007ab0: 2020 2020 2020 2020 2023 2054 7970 6963           # Typic
+00007ac0: 616c 2074 696d 656f 7574 2077 6169 7420  al timeout wait 
+00007ad0: 6973 2034 3030 6d73 0d0a 2020 2020 2020  is 400ms..      
+00007ae0: 2020 2020 2020 7365 6c66 2e64 6576 6963        self.devic
+00007af0: 652e 7772 6974 6528 6673 7472 696e 672e  e.write(fstring.
+00007b00: 656e 636f 6465 2827 7574 662d 3827 2929  encode('utf-8'))
+00007b10: 0d0a 2020 2020 2020 2020 6578 6365 7074  ..        except
+00007b20: 2041 7474 7269 6275 7465 4572 726f 723a   AttributeError:
+00007b30: 0d0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
+00007b40: 7373 0d0a 2020 2020 2020 2020 6578 6365  ss..        exce
+00007b50: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00007b60: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00007b70: 6966 2073 656c 662e 7665 7262 6f73 653a  if self.verbose:
+00007b80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007b90: 2020 7072 696e 7428 6529 0d0a 2020 2020    print(e)..    
+00007ba0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00007bb0: 616c 7365 0d0a 2020 2020 2020 2020 7265  alse..        re
+00007bc0: 7475 726e 2054 7275 650d 0a20 2020 20    turn True..
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,16 +351,17 @@
         Set flags by using keyword arguments
 
         Kwargs:
             key, value: (flag name, boolean) pairs
         """
         if not all([type(v)==bool for v in kwargs.values()]):
             raise ValueError("Ensure all assigned flag values are boolean.")
-        for key, value in kwargs.items():
-            self.flags[key] = value
+        self.flags.update(kwargs)
+        # for key, value in kwargs.items():
+        #     self.flags[key] = value
         return
 
     def shutdown(self):
         """Shutdown procedure for tool"""
         self.disconnect()
         self.resetFlags()
         return
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,26 +339,26 @@
 
         Returns:
             bool: whether the device is connected
         """
         return self.pump.isConnected()
 
     @_multi_channel
-    def pullback(self, channel:Optional[Union[int, tuple[int]]] = None,): # FIXME
+    def pullback(self, channel:Optional[Union[int, tuple[int]]] = None,):
         """
         Pullback liquid from tip
 
         Args:
             channel (Optional[Union[int, tuple[int]]], optional): channel id. Defaults to None.
             
         Returns:
             bool: whether the action is successful
         """
         syringe = self.syringes[channel]
-        return self.pump.pullback(speed=300, pump_time=syringe.pullback_time, channel=channel)
+        return self.pump.pullback(pump_time=syringe.pullback_time, channel=channel)
     
     @_multi_channel
     def rinse(self, 
         speed: Optional[float] = None, 
         wait: int = 0, 
         cycles: int = 1, 
         channel: Optional[Union[int, tuple[int]]] = None,
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.1.0b0/src/controllably/misc/factory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,279 +1,301 @@
 # %% -*- coding: utf-8 -*-
 """
-This module holds the classes for substrate gripper tools from Dobot.
+This module holds the factory functions in Control.lab.ly.
 
 Classes:
-    DobotGripper (Gripper)
-    TwoJawGrip (DobotGripper)
-    VacuumGrip (DobotGripper)
+    DottableDict (dict)
+    ModuleDirectory (dataclass)
+
+Functions:
+    get_class
+    get_details
+    include_this_module
+    load_components
+    register
+    unregister
 
 Other constants and variables:
-    ATTACHMENT_NAMES (list)
-    METHODS_SET (list)
+    HOME_PACKAGES (list)
+    modules (ModuleDirectory)
 """
 # Standard library imports
-from __future__ import annotations
+from dataclasses import dataclass, field
+import importlib
+import inspect
 import numpy as np
-import time
+import pprint
+import sys
 from typing import Callable, Optional
 
+# Third party imports
+import yaml     # pip install pyyaml
+
 # Local application imports
-from ....misc import Helper
-from ..substrate_utils import Gripper
 print(f"Import: OK <{__name__}>")
 
-class DobotGripper(Gripper):
-    """
-    Abstract Base Class (ABC) for Dobot Gripper objects.
-    ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
+HOME_PACKAGES = ['controllably','lab']
+"""Names and aliases of base package"""
 
-    ### Constructor
-    Args:
-        `dashboard` (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-        `channel_map` (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
+class DottableDict(dict):
+    """DottableDict provides a way to use dot notation on dictionaries"""
     
-    ### Attributes
-    - `dashboard` (Callable): connection to status and signal control
+    def __init__(self, *args, **kwargs):
+        """Instantiate the class"""
+        dict.__init__(self, *args, **kwargs)
+        self.__dict__ = self
+        
+    def allow_dotting(self, state:bool = True):
+        """
+        Turn on or off the dot notation feature
+
+        Args:
+            state (bool, optional): whether to turn on dot notation feature. Defaults to True.
+        """
+        if state:
+            self.__dict__ = self
+        else:
+            self.__dict__ = dict()
+
+@dataclass
+class ModuleDirectory:
+    """
+    ModuleDirectory represents the entire collection of imported modules into `controllably`
     
     ### Properties
-    - `channel_map` (dict): mapping of digital I/O channel(s)
-    - `implement_offset` (np.ndarray): offset from attachment site to tooltip
+    - `at`: dictionary structure of imported Classes
     
     ### Methods
-    #### Abstract
-    - `drop`: releases an object
-    - `grab`: picks up an object
-    #### Public
-    - `setDashboard`: set the dashboard object
+    - `get_class`: get Class object from collection
+    - `get_parent`: get parent dictionary of target Class
     """
     
-    _implement_offset: tuple[float] = (0,0,0)
-    def __init__(self, dashboard:Optional[Callable] = None, channel_map:Optional[dict] = None):
-        """
-        Instantiate the class
-
-        Args:
-            dashboard (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
-        """
-        self.dashboard = None
-        self._channel_map = {}
-        self.setDashboard(dashboard=dashboard, channel_map=channel_map)
-        return
+    _modules: DottableDict = field(default_factory=DottableDict, init=False)
     
-    # Properties
-    @property
-    def channel_map(self) -> dict:
-        return self._channel_map
-    @channel_map.setter
-    def channel_map(self, value:dict):
-        if value is None:
-            self._channel_map = {}
-            return
-        if all([(1<= v <=24) for v in value.values()]):
-            self._channel_map = value
-        else:
-            raise ValueError("Please provide valid channel ids from 1 to 24.")
-        return
+    def __repr__(self) -> str:
+        printable_mod = self._modules.copy()
+        def remove_docs(d):
+            """
+            Purge empty dictionaries from nested dictionary
+
+            Args:
+                d (dict): dictionary to be purged
+            """
+            for k, v in list(d.items()):
+                if isinstance(v, dict):
+                    remove_docs(v)
+                if k == "_doc_":
+                    del d[k]
+        remove_docs(printable_mod)
+        return pprint.pformat(printable_mod)
     
     @property
-    def implement_offset(self) -> np.ndarray:
-        return np.array(self._implement_offset)
+    def at(self) -> DottableDict:
+        return self._modules
     
-    def setDashboard(self, dashboard:Callable, channel_map:Optional[dict] = None):
+    def get_class(self, dot_notation:str) -> Callable:
         """
-        Set the dashboard object
+        Get Class object from collection
 
         Args:
-            dashboard (Callable): connection to status and signal control
-            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
+            dot_notation (str): dot notation of target Class
+
+        Returns:
+            Callable: Class object
         """
-        self.dashboard = dashboard
-        self.channel_map = channel_map
-        return
-    
-    
-class TwoJawGrip(DobotGripper):
-    """
-    TwoJawGrip provides methods to operate the Dobot jaw gripper.
-    Channel map labels: `grab`
+        name = dot_notation.split('.')[-1]
+        temp = self.get_parent(dot_notation=dot_notation)
+        return temp.get(name)
     
-    ### Constructor
-    Args:
-        `dashboard` (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-        `channel_map` (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
-        
-    ### Methods
-    - `drop`: releases an object by opening the gripper
-    - `grab`: picks up an object by closing the gripper
-    """
-    
-    _implement_offset = (0,0,-95)
-    def __init__(self, dashboard:Optional[Callable] = None, channel_map:Optional[dict] = None):
+    def get_parent(self, dot_notation:str) -> DottableDict:
         """
-        Instantiate the class
+        Get parent dictionary of target Class
 
         Args:
-            dashboard (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
-        """
-        super().__init__(dashboard=dashboard, channel_map=channel_map)
-        return
+            dot_notation (str): dot notation of target Class
 
-    def drop(self) -> bool:
-        """
-        Releases an object by opening the gripper
-        
         Returns:
-            bool: whether action is successful
-        """
-        channel = self.channel_map.get("grab", 1)
-        try:
-            self.dashboard.DOExecute(channel, 1)
-        except (AttributeError, OSError):
-            print('Tried to drop...')
-            print("Not connected to arm.")
-            return False
-        return True
-    
-    def grab(self) -> bool:
+            DottableDict: parent dictionary of target Class
         """
-        Picks up an object by closing the gripper
+        keys = dot_notation.split('.')
+        keys = keys[:-1]
+        temp = self._modules
+        for key in keys:
+            if key in HOME_PACKAGES:
+                continue
+            temp = temp[key]
+        return temp
         
-        Returns:
-            bool: whether action is successful
-        """
-        channel = self.channel_map.get("grab", 1)
-        try:
-            self.dashboard.DOExecute(channel, 0)
-        except (AttributeError, OSError):
-            print('Tried to grab...')
-            print("Not connected to arm.")
-            return False
-        return True
+modules = ModuleDirectory()
+"""Holds all `controllably` and user-registered classes and functions"""
 
+def get_class(dot_notation:str) -> Callable:
+    """
+    Retrieve the relevant class from the sub-package
+
+    Args:
+        dot_notation (str): dot notation of Class object
 
-class VacuumGrip(DobotGripper):
+    Returns:
+        Callable: target Class
     """
-    VacuumGrip provides methods to operate the Dobot vacuum grip.
-    Channel map labels: `pull`, `push`
-    
-    ### Constructor
+    print('\n')
+    top_package = __name__.split('.')[0]
+    import_path = f'{top_package}.{dot_notation}'
+    package = importlib.import_module('.'.join(import_path.split('.')[:-1]))
+    _class = modules.get_class(dot_notation=dot_notation)
+    return _class
+
+def get_details(configs:dict, addresses:Optional[dict] = None) -> dict:
+    """
+    Decode dictionary of configuration details to get np.ndarrays and tuples
+
     Args:
-        `dashboard` (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-        `channel_map` (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
+        configs (dict): dictionary of configuration details
+        addresses (Optional[dict], optional): dictionary of registered addresses. Defaults to None.
+
+    Returns:
+        dict: dictionary of configuration details
+    """
+    addresses = {} if addresses is None else addresses
+    for name, details in configs.items():
+        settings = details.get('settings', {})
         
-    ### Methods
-    - `drop`: releases an object by pushing out air
-    - `grab`: picks up an object by pulling in air
-    - `pull`: activate pump to suck in air
-    - `push`: activate pump to blow out air
-    - `stop`: stop airflow
+        for key,value in settings.items():
+            if key == 'component_config':
+                value = get_details(value, addresses=addresses)
+            if type(value) == str:
+                if key in ['cam_index', 'port'] and value.startswith('__'):
+                    settings[key] = addresses.get(key, {}).get(settings[key], value)
+            if type(value) == dict:
+                if "tuple" in value:
+                    settings[key] = tuple(value['tuple'])
+                elif "array" in value:
+                    settings[key] = np.array(value['array'])
+
+        configs[name] = details
+    return configs
+
+def include_this_module(
+    where: Optional[str] = None, 
+    module_name: Optional[str] = None, 
+    get_local_only: bool = True
+):
     """
-    
-    _implement_offset = (0,0,-60)
-    def __init__(self, dashboard:Optional[Callable] = None, channel_map:Optional[dict] = None):
-        """
-        Instantiate the class
+    Include the module py file that this function is called from
 
-        Args:
-            dashboard (Optional[Callable], optional): connection to status and signal control. Defaults to None.
-            channel_map (Optional[dict], optional): mapping of digital I/O channel(s). Defaults to None.
-        """
-        super().__init__(dashboard=dashboard, channel_map=channel_map)
-        return
+    Args:
+        where (Optional[str], optional): location within structure to include module. Defaults to None.
+        module_name (Optional[str], optional): dot notation name of module. Defaults to None.
+        get_local_only (bool, optional): whether to only include objects defined in caller py file. Defaults to True.
+    """
+    module_doc = "< No documentation >"
+    frm = inspect.stack()[1]
+    current_mod = inspect.getmodule(frm[0])
+    doc = inspect.getdoc(current_mod)
+    module_doc = module_doc if doc is None else doc
+    if module_name is None:
+        module_name = current_mod.__name__
+    
+    objs = inspect.getmembers(sys.modules[module_name])
+    __where__ = [obj for name,obj in objs if name == "__where__"]
+    where = f"{__where__[0]}." if (len(__where__) and where is None) else where
+    classes = [(nm,obj) for nm,obj in objs if inspect.isclass(obj)]
+    functions = [(nm,obj) for nm,obj in objs if inspect.isfunction(obj)]
+    objs = classes + functions
+    if get_local_only:
+        objs = [obj for obj in objs if obj[1].__module__ == module_name]
+    
+    for name,obj in objs:
+        if name == inspect.stack()[0][3]:
+            continue
+        mod_name = obj.__module__ if where is None else where
+        register(obj, '.'.join(mod_name.split('.')[:-1]), module_docs=module_doc)
+    return
 
-    def drop(self) -> bool:
-        """
-        Releases an object by pushing out air
-        
-        Returns:
-            bool: whether action is successful
-        """
-        print('Tried to drop...')
-        return self.push(0.5)
-    
-    def grab(self) -> bool:
-        """
-        Picks up an object by pulling in air
-        
-        Returns:
-            bool: whether action is successful
-        """
-        print('Tried to grab...')
-        return self.pull(3)
-    
-    def pull(self, duration:Optional[int] = None) -> bool:
-        """
-        Activate pump to suck in air
-        
-        Args:
-            duration (Optional[int], optional): number of seconds to pull air. Defaults to None.
-        
-        Returns:
-            bool: whether action is successful
-        """
-        channel = self.channel_map.get("pull", 1)
-        try:
-            self.dashboard.DOExecute(channel, 1)
-        except (AttributeError, OSError):
-            print('Tried to pull...')
-            print("Not connected to arm.")
-            return False
-        else:
-            if duration is not None:
-                time.sleep(duration)
-                self.dashboard.DOExecute(channel, 0)
-                time.sleep(1)
-        return True
+def load_components(config:dict) -> dict:
+    """
+    Load components of compound tools
+
+    Args:
+        config (dict): dictionary of configuration parameters
+
+    Returns:
+        dict: dictionary of component tools
+    """
+    components = {}
+    for name, details in config.items():
+        _module = details.get('module')
+        if _module is None:
+            continue
+        dot_notation = [_module, details.get('class', '')]
+        _class = get_class('.'.join(dot_notation))
+        settings = details.get('settings', {})
+        components[name] = _class(**settings)
+    return components
+
+def register(new_object:Callable, where:str, module_docs:Optional[str] = None):
+    """
+    Register the object into target location within structure
+
+    Args:
+        new_object (Callable): new Callable object (Class or function) to be registered
+        where (str): location within structure to register the object in
+        module_docs (Optional[str], optional): module documentation. Defaults to None.
+    """
+    module_docs = "< No documentation >" if module_docs is None else module_docs
+    keys = where.split('.')
+    temp = modules._modules
+    for key in keys:
+        if key in HOME_PACKAGES:
+            continue
+        if key not in temp:
+            temp[key] = DottableDict()
+        temp = temp[key]
+    if "_doc_" not in temp:
+        temp["_doc_"] = module_docs
+    
+    name = new_object.__name__
+    if name in temp:
+        overwrite = input(f"An object with the same name ({name}) already exists, Overwrite? [y/n]")
+        if overwrite.lower()[0] == 'n':
+            print(f"Skipping {name}...")
+            return
+    temp[new_object.__name__] = new_object
+    return
+
+def unregister(dot_notation:str):
+    """
+    Unregister an object from structure, using its dot notation reference
+
+    Args:
+        dot_notation (str): dot notation reference to target object
+    """
+    keys = dot_notation.split('.')
+    keys, name = keys[:-1], keys[-1]
+    temp = modules._modules
+    for key in keys:
+        if key in HOME_PACKAGES:
+            continue
+        temp = temp[key]
+    temp.pop(name)
     
-    def push(self, duration:Optional[int] = None) -> bool:
+    # Clean up empty dictionaries
+    def remove_empty_dicts(d: dict):
         """
-        Activate pump to blow out air
-        
+        Purge empty dictionaries from nested dictionary
+
         Args:
-            duration (Optional[int], optional): number of seconds to push air. Defaults to None.
-            
-        Returns:
-            bool: whether action is successful
+            d (dict): dictionary to be purged
         """
-        channel = self.channel_map.get("push", 2)
-        try:
-            self.dashboard.DOExecute(channel, 1)
-        except (AttributeError, OSError):
-            print('Tried to push...')
-            print("Not connected to arm.")
-            return False
-        else:
-            if duration is not None:
-                time.sleep(duration)
-                self.dashboard.DOExecute(channel, 0)
-                time.sleep(1)
-        return True
-    
-    def stop(self) -> bool:
-        """
-        Stop airflow
-        
-        Returns:
-            bool: whether action is successful
-        """
-        channels = [v for v in self.channel_map.values()] if len(self.channel_map) else [1,2]
-        try:
-            for channel in channels:
-                self.dashboard.DOExecute(channel, 0)
-            time.sleep(1)
-        except (AttributeError, OSError):
-            print('Tried to stop...')
-            print("Not connected to arm.")
-            return False
-        return True
-
-
-# FIXME: Do away with these objects below
-ATTACHMENTS = [TwoJawGrip, VacuumGrip]
-METHODS = [Helper.get_method_names(attachment) for attachment in ATTACHMENTS]
-ATTACHMENT_NAMES = [att.__name__ for att in ATTACHMENTS]
-"""List of attachment names"""
-METHODS_SET = sorted( list(set([item for sublist in METHODS for item in sublist])) )
-"""Sorted list of method names"""
+        for k, v in list(d.items()):
+            if isinstance(v, dict):
+                remove_empty_dicts(v)
+            if not v:
+                del d[k]
+        if list(d.keys()) == ['_doc_']:
+            del d['_doc_']
+    remove_empty_dicts(modules._modules)
+    return
+
+__where__ = "misc.Factory"
+include_this_module(get_local_only=True)
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Standard library imports
 from abc import ABC, abstractmethod
 
 # Third party imports
 import cv2 # pip install opencv-python
 
 # Local application imports
-from ..image_utils import Image
+from .. import image as Image
 print(f"Import: OK <{__name__}>")
 
 class Classifier(ABC):
     """
     Abstract Base Class (ABC) for Classifier objects (i.e. models that can detect image targets).
     ABC cannot be instantiated, and must be subclassed with abstract methods implemented before use.
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.1.0b0/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/thermal_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # %% -*- coding: utf-8 -*-
 """
-This module holds the class for thermal cameras.
+WIP: This module holds the class for thermal cameras.
 
 Classes:
     Thermal (Camera)
 """
 # Standard library imports
 from __future__ import annotations
 import numpy as np
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/image_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/View/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,17 @@
         180: cv2.ROTATE_180,
         270: cv2.ROTATE_90_COUNTERCLOCKWISE
     }
     if angle != 0:
         frame = cv2.rotate(frame, rotateCodes.get(angle))
     return frame
 
-
+__where__ = "View.Image"
+from controllably import include_this_module
+include_this_module(get_local_only=True)
 
 # NOTE: DEPRECATED
 
 # class Image:
 #     """
 #     Image class with image manipulation methods
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/View/view_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/View/view_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import Optional, Protocol
 
 # Third party imports
 import cv2              # pip install opencv-python
 
 # Local application imports
 from ..misc import Helper
-from . import image_utils as Image
+from . import image as Image
 print(f"Import: OK <{__name__}>")
 
 DIMENSION_THRESHOLD = 36
 """Minimum width in pixels of target for detection"""
 ROW_DISTANCE = 30
 """Number of pixels between rows of detected targets"""
 
@@ -229,16 +229,17 @@
         Set flags by using keyword arguments
 
         Kwargs:
             key, value: (flag name, boolean) pairs
         """
         if not all([type(v)==bool for v in kwargs.values()]):
             raise ValueError("Ensure all assigned flag values are boolean.")
-        for key, value in kwargs.items():
-            self.flags[key] = value
+        self.flags.update(kwargs)
+        # for key, value in kwargs.items():
+        #     self.flags[key] = value
         return
     
     def shutdown(self):
         """Shutdown procedure for tool"""
         self.disconnect()
         cv2.destroyAllWindows()
         self.resetFlags()
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/__init__.py` & `control-lab-ly-1.1.0b0/src/controllably/misc/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Modules:
     Factory
     Helper
     Layout
 
 Classes:
     Logger
-    
+
 Functions:
     create_configs
     create_setup
     include_this_module
     load_deck
     load_setup
     set_safety (decorator)
@@ -22,8 +22,10 @@
     modules (ModuleDirectory)
 """
 from . import factory as Factory
 from . import helper as Helper
 from . import layout as Layout
 from .factory import include_this_module, modules
 from .logger import Logger, LOGGER
-from .misc_utils import *
+from .misc_utils import *
+
+include_this_module(get_local_only=False)
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/decorators.py` & `control-lab-ly-1.1.0b0/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/helper.py` & `control-lab-ly-1.1.0b0/src/controllably/misc/helper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # %% -*- coding: utf-8 -*-
 """
 This module holds the helper functions in Control.lab.ly.
 
 Functions:
     create_folder
+    get_machine_addresses
     get_method_names
     get_node
+    get_plans
     get_ports
     is_overrun
     pretty_print_duration
     read_json
     read_yaml
     safety_measures (decorator)
     zip_inputs
@@ -26,19 +28,20 @@
 import pandas as pd
 import pkgutil
 import time
 from typing import Callable, Optional
 import uuid
 
 # Third party imports
-import serial.tools.list_ports # pip install pyserial
-import yaml # pip install pyyaml
+import serial.tools.list_ports      # pip install pyserial
+import yaml                         # pip install pyyaml
 
 # Local application imports
 from . import decorators
+from . import factory
 print(f"Import: OK <{__name__}>")
 
 safety_countdown = 3
 """Safety countdown before executing move, in seconds"""
 safety_mode = None
 """Safety level (`'high'`, `'low'`, `None`)"""
 
@@ -56,14 +59,32 @@
     main_folder = datetime.now().strftime("%Y-%m-%d_%H%M")
     if parent_folder:
         main_folder = '/'.join([parent_folder, main_folder])
     folder = '/'.join([main_folder, child_folder]) if child_folder else main_folder
     if not os.path.exists(folder):
         os.makedirs(folder)
     return main_folder
+
+def get_machine_addresses(registry:dict) -> dict:
+    """
+    Get the appropriate addresses for current machine
+
+    Args:
+        registry (str): dictionary of yaml file with com port addresses and camera ids
+
+    Returns:
+        dict: dictionary of com port addresses and camera ids for current machine
+    """
+    node_id = get_node()
+    addresses = registry.get('machine_id',{}).get(node_id,{})
+    if len(addresses) == 0:
+        print("\nAppend machine id and camera ids/port addresses to registry file")
+        print(yaml.dump(registry))
+        raise Exception(f"Machine not yet registered. (Current machine id: {node_id})")
+    return addresses
     
 def get_method_names(obj:Callable) -> list[str]:
     """
     Get the names of the methods in Callable object (class/instance)
 
     Args:
         obj (Callable): object of interest
@@ -84,15 +105,35 @@
 def get_node() -> str:
     """
     Display the machine's unique identifier
 
     Returns:
         str: machine unique identifier
     """
-    return str(uuid.getnode())
+    node_id = str(uuid.getnode())
+    print(f"Current machine id: {node_id}")
+    return node_id
+
+def get_plans(config_file:str, registry_file:Optional[str] = None, package:Optional[str] = None) -> dict:
+    """
+    Read configuration file (yaml) and get details
+
+    Args:
+        config_file (str): filename of configuration file
+        registry_file (Optional[str], optional): filename of registry file. Defaults to None.
+        package (Optional[str], optional): name of package to look in. Defaults to None.
+
+    Returns:
+        dict: dictionary of configuration parameters
+    """
+    configs = read_yaml(config_file, package)
+    registry = read_yaml(registry_file, package)
+    addresses = get_machine_addresses(registry=registry)
+    configs = factory.get_details(configs, addresses=addresses)
+    return configs
 
 def get_ports() -> list[str]:
     """
     Get available ports
 
     Returns:
         list[str]: list of connected serial ports
@@ -183,18 +224,18 @@
         Callable: wrapped function
     """
     return decorators.safety_measures(mode=safety_mode, countdown=safety_countdown)(func=func)
 
 def zip_inputs(primary_keyword:str, **kwargs) -> dict:
     """
     Checks and zips multiple keyword arguments of lists into dictionary
-
+    
     Args:
         primary_keyword (str): primary keyword to be used as key
-        
+    
     Kwargs:
         key, list[...]: {keyword, list of values} pairs
 
     Raises:
         Exception: Ensure the lengths of inputs are the same
 
     Returns:
@@ -211,18 +252,9 @@
                 kwargs[key] = value * input_length
     if not all(len(kwargs[key]) == input_length for key in keys):
         raise Exception(f"Ensure the lengths of these inputs are the same: {', '.join(keys)}")
     kwargs_df = pd.DataFrame(kwargs)
     kwargs_df.set_index(primary_keyword, drop=False, inplace=True)
     return kwargs_df.to_dict('index')
 
-
-### NOTE: DEPRECATE
-def display_ports() -> list[str]:
-    """
-    Get available ports
-
-    Returns:
-        list: list of connected serial ports
-    """
-    print("'display_ports()' method to be deprecated. Use 'get_ports()' method instead.")
-    return get_ports()
+__where__ = "misc.Helper"
+factory.include_this_module(get_local_only=True)
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/layout.py` & `control-lab-ly-1.1.0b0/src/controllably/misc/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
     ### Constructor
     Args:
         `slot` (str): deck slot number
         `bottom_left_coordinates` (tuple[float]): coordinates of bottom left corner of Labware (i.e. reference point)
         `labware_file` (str): filepath of Labware JSON file
         `package` (Optional[str], optional): name of package to look in. Defaults to None.
-        
+    
     ### Attributes
     - `details` (dict): dictionary read from Labware file
     - `name` (str): name of Labware
     - `slot` (str): deck slot number
     
     ### Properties
     - `center` (np.ndarray): center of Labware
@@ -486,7 +486,11 @@
             index = self.names.get(name)
         elif index is not None and name is None:
             name = [k for k,v in self.names.items() if v==index][0]
         self.names.pop(name)
         self._slots.pop(str(index))
         self.exclusion_zones.pop(str(index))
         return
+
+__where__ = "misc.Layout"
+from .factory import include_this_module
+include_this_module(get_local_only=True)
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/logger.py` & `control-lab-ly-1.1.0b0/src/controllably/misc/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class Logger:
     """
     Logger class with miscellaneous methods
     
     ### Constructor
     Args:
         `name` (str): name of logger
-        
+    
     ### Attributes
     - `all_logs` (list[str]): list of all logs
     - `logs` (dict): logs by group
     - `name` (str): name of logger
     
     ### Methods
     - `log_now`: add log message with timestamp
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.1.0b0/src/controllably/misc/misc_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,15 @@
     """Create new configs folder"""
     cwd = os.getcwd().replace('\\', '/')
     src = f"{here}/templates/configs"
     dst = f"{cwd}/configs"
     if not os.path.exists(dst):
         print("Creating configs folder...\n")
         copytree(src=src, dst=dst)
-        node_id = helper.get_node()
-        print(f"Current machine id: {node_id}")
+        helper.get_node()
     return
 
 def create_setup(setup_name:Optional[str] = None):
     """
     Create new setup folder
 
     Args:
@@ -66,14 +65,15 @@
     cfg = f"{cwd}/configs"
     dst = f"{cfg}/{setup_name}"
     if not os.path.exists(cfg):
         create_configs()
     if not os.path.exists(dst):
         print(f"Creating setup folder ({setup_name})...\n")
         copytree(src=src, dst=dst)
+        helper.get_node()
     return
 
 def load_deck(device:Callable, layout_file:str, get_absolute_filepath:bool = True) -> Callable:
     """
     Load deck information from layout file
 
     Args:
@@ -105,15 +105,15 @@
     Args:
         config_file (str): config filename
         registry_file (Optional[str], optional): registry filename. Defaults to None.
 
     Returns:
         dict: dictionary of loaded devices
     """
-    config = factory.get_plans(config_file=config_file, registry_file=registry_file)
+    config = helper.get_plans(config_file=config_file, registry_file=registry_file)
     setup = factory.load_components(config=config)
     shortcuts = config.get('SHORTCUTS',{})
     
     for key,value in shortcuts.items():
         parent, child = value.split('.')
         tool = setup.get(parent)
         if tool is None:
```

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/tests/test_compound_liquidmover.py` & `control-lab-ly-1.1.0b0/tests/test_compound_liquidmover.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/tests/test_compound_spin_printer.py` & `control-lab-ly-1.1.0b0/tests/test_compound_spin_printer.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/tests/test_dobot_m1pro.py` & `control-lab-ly-1.1.0b0/tests/test_dobot_m1pro.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/tests/test_dobot_mg400.py` & `control-lab-ly-1.1.0b0/tests/test_dobot_mg400.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/tests/test_heat_peltier.py` & `control-lab-ly-1.1.0b0/tests/test_heat_peltier.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/tests/test_liquid_tricontinent.py` & `control-lab-ly-1.1.0b0/tests/test_liquid_tricontinent.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0a0/tests/test_mixture_shaker.py` & `control-lab-ly-1.1.0b0/tests/test_mixture_shaker.py`

 * *Files identical despite different names*

