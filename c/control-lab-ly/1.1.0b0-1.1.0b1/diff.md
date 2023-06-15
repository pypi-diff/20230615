# Comparing `tmp/control-lab-ly-1.1.0b0.tar.gz` & `tmp/control-lab-ly-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control-lab-ly-1.1.0b0.tar", last modified: Thu Jun 15 05:55:53 2023, max compression
+gzip compressed data, was "control-lab-ly-1.1.0b1.tar", last modified: Thu Jun 15 06:28:57 2023, max compression
```

## Comparing `control-lab-ly-1.1.0b0.tar` & `control-lab-ly-1.1.0b1.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.574456 control-lab-ly-1.1.0b0/
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0b0/LICENSE.md
--rw-rw-rw-   0        0        0       44 2023-06-15 05:55:28.000000 control-lab-ly-1.1.0b0/MANIFEST.in
--rw-rw-rw-   0        0        0    20718 2023-06-15 05:55:53.574456 control-lab-ly-1.1.0b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.242181 control-lab-ly-1.1.0b0/docs/
--rw-rw-rw-   0        0        0     6576 2023-06-15 05:47:20.000000 control-lab-ly-1.1.0b0/docs/CHANGELOG.md
--rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.0b0/docs/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/docs/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0b0/docs/LICENSE.md
--rw-rw-rw-   0        0        0    13024 2023-06-15 02:35:45.000000 control-lab-ly-1.1.0b0/docs/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.250795 control-lab-ly-1.1.0b0/docs/assets/
--rw-rw-rw-   0        0        0   203629 2023-06-15 02:22:15.000000 control-lab-ly-1.1.0b0/docs/assets/Documentation guide.png
--rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/pyproject.toml
--rw-rw-rw-   0        0        0     1500 2023-06-15 05:55:53.574456 control-lab-ly-1.1.0b0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.0b0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:51.925283 control-lab-ly-1.1.0b0/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.292330 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/
--rw-rw-rw-   0        0        0    20718 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7587 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 05:55:51.000000 control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.309630 control-lab-ly-1.1.0b0/src/controllably/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.326989 control-lab-ly-1.1.0b0/src/controllably/Compound/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.343958 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.361685 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/Opentrons/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
--rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/__init__.py
--rw-rw-rw-   0        0        0    17618 2023-06-07 08:08:37.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py
--rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/__init__.py
--rw-rw-rw-   0        0        0     8197 2023-06-07 15:06:53.000000 control-lab-ly-1.1.0b0/src/controllably/Compound/compound_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.378265 control-lab-ly-1.1.0b0/src/controllably/Control/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.419000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.472031 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/
--rw-rw-rw-   0        0        0      569 2023-06-07 07:31:49.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/__init__.py
--rw-rw-rw-   0        0        0     7129 2023-06-07 08:09:06.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/maker_panel.py
--rw-rw-rw-   0        0        0     7976 2023-06-09 02:26:55.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/measurer_panel.py
--rw-rw-rw-   0        0        0    16355 2023-06-09 02:26:45.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/mover_panel.py
--rw-rw-rw-   0        0        0     8767 2023-06-07 07:59:03.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
--rw-rw-rw-   0        0        0     3780 2023-06-07 08:09:39.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/viewer_panel.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.515458 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/
--rw-rw-rw-   0        0        0      406 2023-06-07 07:37:47.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/__init__.py
--rw-rw-rw-   0        0        0      888 2023-06-07 07:29:39.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/loader_panel.py
--rw-rw-rw-   0        0        0     8681 2023-06-07 15:28:23.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/pop_ups.py
--rw-rw-rw-   0        0        0     4573 2023-06-07 15:28:30.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/templates.py
--rw-rw-rw-   0        0        0      519 2023-06-07 15:50:08.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/__init__.py
--rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/_guibuilder.py
--rw-rw-rw-   0        0        0     5544 2023-06-07 08:08:44.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/compound_panel.py
--rw-rw-rw-   0        0        0    16264 2023-06-07 08:08:56.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/gui_utils.py
--rw-rw-rw-   0        0        0    14530 2023-06-15 02:18:22.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/guide_panel.py
--rw-rw-rw-   0        0        0     3481 2023-06-07 07:35:28.000000 control-lab-ly-1.1.0b0/src/controllably/Control/GUI/multichannel_panel.py
--rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.1.0b0/src/controllably/Control/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.546239 control-lab-ly-1.1.0b0/src/controllably/Make/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.577289 control-lab-ly-1.1.0b0/src/controllably/Make/Heat/
--rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Heat/__init__.py
--rw-rw-rw-   0        0        0    11244 2023-06-07 08:09:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Heat/peltier_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.626845 control-lab-ly-1.1.0b0/src/controllably/Make/Light/
--rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Light/__init__.py
--rw-rw-rw-   0        0        0     9882 2023-06-07 08:09:54.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Light/led_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.634274 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.648457 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/
--rw-rw-rw-   0        0        0      252 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/__init__.py
--rw-rw-rw-   0        0        0    27552 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.709617 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
--rw-rw-rw-   0        0        0      171 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
--rw-rw-rw-   0        0        0    37854 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
--rw-rw-rw-   0        0        0     4984 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.725629 control-lab-ly-1.1.0b0/src/controllably/Make/ThinFilm/
--rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/ThinFilm/__init__.py
--rw-rw-rw-   0        0        0    10777 2023-06-07 08:10:11.000000 control-lab-ly-1.1.0b0/src/controllably/Make/ThinFilm/spinner_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Make/__init__.py
--rw-rw-rw-   0        0        0     4220 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b0/src/controllably/Make/make_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.746436 control-lab-ly-1.1.0b0/src/controllably/Measure/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.760623 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.784503 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/
--rw-rw-rw-   0        0        0      314 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/__init__.py
--rw-rw-rw-   0        0        0    18010 2023-06-07 08:10:41.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py
--rw-rw-rw-   0        0        0     7484 2023-06-07 08:10:49.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
--rw-rw-rw-   0        0        0     1993 2023-06-07 08:10:55.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.807068 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/programs/
--rw-rw-rw-   0        0        0      287 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
--rw-rw-rw-   0        0        0    10637 2023-06-07 15:30:15.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/electrical_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.815712 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.881116 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/
--rw-rw-rw-   0        0        0      334 2023-05-18 08:27:22.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
--rw-rw-rw-   0        0        0    10341 2023-06-07 08:11:13.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
--rw-rw-rw-   0        0        0     3159 2023-06-07 08:11:18.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
--rw-rw-rw-   0        0        0     2012 2023-06-07 08:11:22.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.900436 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
--rw-rw-rw-   0        0        0      236 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
--rw-rw-rw-   0        0        0     3534 2023-06-07 08:11:26.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/__init__.py
--rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/mechanical_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.917099 control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/
--rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/__init__.py
--rw-rw-rw-   0        0        0     8358 2023-06-07 08:11:32.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/balance_utils.py
--rw-rw-rw-   0        0        0     8199 2023-06-07 08:11:37.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/force_sensor_utils.py
--rw-rw-rw-   0        0        0      535 2023-06-06 08:07:20.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/__init__.py
--rw-rw-rw-   0        0        0     5437 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/instrument_utils.py
--rw-rw-rw-   0        0        0    14062 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/measure_utils.py
--rw-rw-rw-   0        0        0     4180 2023-06-07 08:10:29.000000 control-lab-ly-1.1.0b0/src/controllably/Measure/program_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.927685 control-lab-ly-1.1.0b0/src/controllably/Move/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.945665 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/
--rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/__init__.py
--rw-rw-rw-   0        0        0     9077 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/cartesian_utils.py
--rw-rw-rw-   0        0        0     3450 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/ender_utils.py
--rw-rw-rw-   0        0        0     2852 2023-06-06 07:14:55.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/primitiv_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.962232 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:52.986737 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/
--rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.010543 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/
--rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
--rw-rw-rw-   0        0        0    24280 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
--rw-rw-rw-   0        0        0    15776 2023-06-07 08:12:14.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py
--rw-rw-rw-   0        0        0     7128 2023-06-15 03:26:52.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
--rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py
--rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/__init__.py
--rw-rw-rw-   0        0        0    10566 2023-06-07 08:12:11.000000 control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/jointed_utils.py
--rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Move/__init__.py
--rw-rw-rw-   0        0        0    32385 2023-06-05 18:48:48.000000 control-lab-ly-1.1.0b0/src/controllably/Move/move_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.028178 control-lab-ly-1.1.0b0/src/controllably/Transfer/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.052652 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.077054 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.109936 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/
--rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
--rw-rw-rw-   0        0        0     3440 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
--rw-rw-rw-   0        0        0    29858 2023-06-07 08:12:55.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
--rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/__init__.py
--rw-rw-rw-   0        0        0     7672 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
--rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.126250 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/
--rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/__init__.py
--rw-rw-rw-   0        0        0     2792 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
--rw-rw-rw-   0        0        0    31695 2023-06-07 15:33:06.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
--rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/__init__.py
--rw-rw-rw-   0        0        0    13230 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/liquid_utils.py
--rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/syringe_lib.py
--rw-rw-rw-   0        0        0    14600 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/syringe_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.134466 control-lab-ly-1.1.0b0/src/controllably/Transfer/Powder/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Powder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.152260 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.168316 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/Dobot/
--rw-rw-rw-   0        0        0      397 2023-06-07 02:20:21.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/Dobot/__init__.py
--rw-rw-rw-   0        0        0     8844 2023-06-07 08:13:13.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
--rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/substrate_utils.py
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/src/controllably/Transfer/transfer_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.184342 control-lab-ly-1.1.0b0/src/controllably/View/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.193029 control-lab-ly-1.1.0b0/src/controllably/View/Classifiers/
--rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/View/Classifiers/__init__.py
--rw-rw-rw-   0        0        0     2584 2023-06-08 02:41:36.000000 control-lab-ly-1.1.0b0/src/controllably/View/Classifiers/classifier_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.201058 control-lab-ly-1.1.0b0/src/controllably/View/Optical/
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/View/Optical/__init__.py
--rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/View/Optical/optical_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.209053 control-lab-ly-1.1.0b0/src/controllably/View/Optical/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b0/src/controllably/View/Optical/placeholders/__init__.py
--rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Optical/placeholders/optical_camera.png
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.225709 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.225709 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:04:15.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.260043 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/
--rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/__init__.py
--rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8.py
--rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
--rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
--rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
--rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.276352 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/placeholders/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/placeholders/__init__.py
--rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png
--rw-rw-rw-   0        0        0     2988 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/src/controllably/View/Thermal/thermal_utils.py
--rw-rw-rw-   0        0        0      304 2023-06-08 02:41:32.000000 control-lab-ly-1.1.0b0/src/controllably/View/__init__.py
--rw-rw-rw-   0        0        0    15703 2023-06-07 14:50:19.000000 control-lab-ly-1.1.0b0/src/controllably/View/image.py
--rw-rw-rw-   0        0        0    15898 2023-06-08 02:41:35.000000 control-lab-ly-1.1.0b0/src/controllably/View/view_utils.py
--rw-rw-rw-   0        0        0      131 2023-06-05 18:11:26.000000 control-lab-ly-1.1.0b0/src/controllably/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.334847 control-lab-ly-1.1.0b0/src/controllably/misc/
--rw-rw-rw-   0        0        0      627 2023-06-07 15:16:27.000000 control-lab-ly-1.1.0b0/src/controllably/misc/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/decorators.py
--rw-rw-rw-   0        0        0     9596 2023-06-09 02:42:47.000000 control-lab-ly-1.1.0b0/src/controllably/misc/factory.py
--rw-rw-rw-   0        0        0     7940 2023-06-13 09:57:18.000000 control-lab-ly-1.1.0b0/src/controllably/misc/helper.py
--rw-rw-rw-   0        0        0    17547 2023-06-07 14:53:56.000000 control-lab-ly-1.1.0b0/src/controllably/misc/layout.py
--rw-rw-rw-   0        0        0     2863 2023-06-07 08:11:52.000000 control-lab-ly-1.1.0b0/src/controllably/misc/logger.py
--rw-rw-rw-   0        0        0     4543 2023-06-14 09:42:31.000000 control-lab-ly-1.1.0b0/src/controllably/misc/misc_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.343783 control-lab-ly-1.1.0b0/src/controllably/misc/templates/
--rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.368664 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/
--rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.384661 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/plugins/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/plugins/plugin_template.py
--rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/registry.yaml
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.417857 control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/
--rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/config.yaml
--rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/layout.json
-drwxrwxrwx   0        0        0        0 2023-06-15 05:55:53.566458 control-lab-ly-1.1.0b0/tests/
--rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0b0/tests/test_camera_optical.py
--rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_camera_thermal.py
--rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_cartesian_ender.py
--rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_cartesian_primitiv.py
--rw-rw-rw-   0        0        0      629 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0b0/tests/test_compound_liquidmover.py
--rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_compound_spin_printer.py
--rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_dobot_m1pro.py
--rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_dobot_mg400.py
--rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_electrical_keithley.py
--rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_film_spin.py
--rw-rw-rw-   0        0        0      586 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/tests/test_heat_peltier.py
--rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_light_led_array.py
--rw-rw-rw-   0        0        0      390 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0b0/tests/test_liquid_sartorius.py
--rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_liquid_syringe_assembly.py
--rw-rw-rw-   0        0        0      538 2023-05-04 09:11:29.000000 control-lab-ly-1.1.0b0/tests/test_liquid_tricontinent.py
--rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_mechanical_piezorobotics.py
--rw-rw-rw-   0        0        0     1011 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b0/tests/test_mixture_shaker.py
--rw-rw-rw-   0        0        0     2365 2023-06-15 02:45:10.000000 control-lab-ly-1.1.0b0/tests/test_panels.py
--rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_physical_balance.py
--rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b0/tests/test_pump_peristaltic.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.315276 control-lab-ly-1.1.0b1/
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0b1/LICENSE.md
+-rw-rw-rw-   0        0        0       44 2023-06-15 05:55:28.000000 control-lab-ly-1.1.0b1/MANIFEST.in
+-rw-rw-rw-   0        0        0    20812 2023-06-15 06:28:57.315276 control-lab-ly-1.1.0b1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.633108 control-lab-ly-1.1.0b1/docs/
+-rw-rw-rw-   0        0        0     6576 2023-06-15 05:47:20.000000 control-lab-ly-1.1.0b1/docs/CHANGELOG.md
+-rw-rw-rw-   0        0        0     5356 2023-02-24 14:06:11.000000 control-lab-ly-1.1.0b1/docs/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/docs/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1093 2023-02-24 13:59:16.000000 control-lab-ly-1.1.0b1/docs/LICENSE.md
+-rw-rw-rw-   0        0        0    13118 2023-06-15 06:27:50.000000 control-lab-ly-1.1.0b1/docs/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.641155 control-lab-ly-1.1.0b1/docs/assets/
+-rw-rw-rw-   0        0        0   203629 2023-06-15 02:22:15.000000 control-lab-ly-1.1.0b1/docs/assets/Documentation guide.png
+-rw-rw-rw-   0        0        0      108 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/pyproject.toml
+-rw-rw-rw-   0        0        0     1500 2023-06-15 06:28:57.324760 control-lab-ly-1.1.0b1/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-03-10 02:02:34.000000 control-lab-ly-1.1.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.235800 control-lab-ly-1.1.0b1/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.676638 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/
+-rw-rw-rw-   0        0        0    20812 2023-06-15 06:28:54.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7587 2023-06-15 06:28:55.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 06:28:54.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-06-15 06:28:54.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 06:28:54.000000 control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.684653 control-lab-ly-1.1.0b1/src/controllably/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.710318 control-lab-ly-1.1.0b1/src/controllably/Compound/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.728730 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.781362 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/Opentrons/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/Opentrons/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/Opentrons/opentrons_utils.py
+-rw-rw-rw-   0        0        0      259 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/__init__.py
+-rw-rw-rw-   0        0        0    17618 2023-06-07 08:08:37.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/liquidmover_utils.py
+-rw-rw-rw-   0        0        0      241 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/__init__.py
+-rw-rw-rw-   0        0        0     8197 2023-06-07 15:06:53.000000 control-lab-ly-1.1.0b1/src/controllably/Compound/compound_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.799953 control-lab-ly-1.1.0b1/src/controllably/Control/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.903515 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:55.963518 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/
+-rw-rw-rw-   0        0        0      569 2023-06-07 07:31:49.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/__init__.py
+-rw-rw-rw-   0        0        0     7129 2023-06-07 08:09:06.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/maker_panel.py
+-rw-rw-rw-   0        0        0     7976 2023-06-09 02:26:55.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/measurer_panel.py
+-rw-rw-rw-   0        0        0    16355 2023-06-09 02:26:45.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/mover_panel.py
+-rw-rw-rw-   0        0        0     8767 2023-06-07 07:59:03.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py
+-rw-rw-rw-   0        0        0     3780 2023-06-07 08:09:39.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/viewer_panel.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.009365 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/
+-rw-rw-rw-   0        0        0      406 2023-06-07 07:37:47.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/__init__.py
+-rw-rw-rw-   0        0        0      888 2023-06-07 07:29:39.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/loader_panel.py
+-rw-rw-rw-   0        0        0     8681 2023-06-07 15:28:23.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/pop_ups.py
+-rw-rw-rw-   0        0        0     4573 2023-06-07 15:28:30.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/templates.py
+-rw-rw-rw-   0        0        0      519 2023-06-07 15:50:08.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/__init__.py
+-rw-rw-rw-   0        0        0    20954 2023-04-24 02:45:08.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/_guibuilder.py
+-rw-rw-rw-   0        0        0     5544 2023-06-07 08:08:44.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/compound_panel.py
+-rw-rw-rw-   0        0        0    16264 2023-06-07 08:08:56.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/gui_utils.py
+-rw-rw-rw-   0        0        0    14530 2023-06-15 02:18:22.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/guide_panel.py
+-rw-rw-rw-   0        0        0     3481 2023-06-07 07:35:28.000000 control-lab-ly-1.1.0b1/src/controllably/Control/GUI/multichannel_panel.py
+-rw-rw-rw-   0        0        0        0 2023-06-05 18:40:54.000000 control-lab-ly-1.1.0b1/src/controllably/Control/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.025413 control-lab-ly-1.1.0b1/src/controllably/Make/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.077219 control-lab-ly-1.1.0b1/src/controllably/Make/Heat/
+-rw-rw-rw-   0        0        0      225 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Heat/__init__.py
+-rw-rw-rw-   0        0        0    11244 2023-06-07 08:09:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Heat/peltier_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.100685 control-lab-ly-1.1.0b1/src/controllably/Make/Light/
+-rw-rw-rw-   0        0        0      218 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Light/__init__.py
+-rw-rw-rw-   0        0        0     9882 2023-06-07 08:09:54.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Light/led_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.108732 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.134458 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/
+-rw-rw-rw-   0        0        0      252 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/__init__.py
+-rw-rw-rw-   0        0        0    27552 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.166902 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/
+-rw-rw-rw-   0        0        0      171 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/__init__.py
+-rw-rw-rw-   0        0        0    37854 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py
+-rw-rw-rw-   0        0        0     4984 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.188087 control-lab-ly-1.1.0b1/src/controllably/Make/ThinFilm/
+-rw-rw-rw-   0        0        0      268 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/ThinFilm/__init__.py
+-rw-rw-rw-   0        0        0    10777 2023-06-07 08:10:11.000000 control-lab-ly-1.1.0b1/src/controllably/Make/ThinFilm/spinner_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Make/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-06-05 10:20:45.000000 control-lab-ly-1.1.0b1/src/controllably/Make/make_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.232611 control-lab-ly-1.1.0b1/src/controllably/Measure/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.248032 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.312523 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/
+-rw-rw-rw-   0        0        0      314 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/__init__.py
+-rw-rw-rw-   0        0        0    18010 2023-06-07 08:10:41.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_device.py
+-rw-rw-rw-   0        0        0     7484 2023-06-07 08:10:49.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py
+-rw-rw-rw-   0        0        0     1993 2023-06-07 08:10:55.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.337117 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/programs/
+-rw-rw-rw-   0        0        0      287 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/programs/__init__.py
+-rw-rw-rw-   0        0        0    10637 2023-06-07 15:30:15.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/electrical_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.354994 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.394443 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/
+-rw-rw-rw-   0        0        0      334 2023-05-18 08:27:22.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/__init__.py
+-rw-rw-rw-   0        0        0    10341 2023-06-07 08:11:13.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py
+-rw-rw-rw-   0        0        0     3159 2023-06-07 08:11:18.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py
+-rw-rw-rw-   0        0        0     2012 2023-06-07 08:11:22.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.410444 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/
+-rw-rw-rw-   0        0        0      236 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/__init__.py
+-rw-rw-rw-   0        0        0     3534 2023-06-07 08:11:26.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/__init__.py
+-rw-rw-rw-   0        0        0      298 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/mechanical_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.451924 control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/
+-rw-rw-rw-   0        0        0      249 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/__init__.py
+-rw-rw-rw-   0        0        0     8358 2023-06-07 08:11:32.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/balance_utils.py
+-rw-rw-rw-   0        0        0     8199 2023-06-07 08:11:37.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/force_sensor_utils.py
+-rw-rw-rw-   0        0        0      535 2023-06-06 08:07:20.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/__init__.py
+-rw-rw-rw-   0        0        0     5437 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/instrument_utils.py
+-rw-rw-rw-   0        0        0    14062 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/measure_utils.py
+-rw-rw-rw-   0        0        0     4180 2023-06-07 08:10:29.000000 control-lab-ly-1.1.0b1/src/controllably/Measure/program_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.478387 control-lab-ly-1.1.0b1/src/controllably/Move/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.530473 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/
+-rw-rw-rw-   0        0        0      346 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/__init__.py
+-rw-rw-rw-   0        0        0     9077 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/cartesian_utils.py
+-rw-rw-rw-   0        0        0     3450 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/ender_utils.py
+-rw-rw-rw-   0        0        0     2852 2023-06-06 07:14:55.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/primitiv_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.550498 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.576440 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/
+-rw-rw-rw-   0        0        0      336 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.592649 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/
+-rw-rw-rw-   0        0        0       62 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/__init__.py
+-rw-rw-rw-   0        0        0    24280 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py
+-rw-rw-rw-   0        0        0    15776 2023-06-07 08:12:14.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_utils.py
+-rw-rw-rw-   0        0        0     7128 2023-06-15 03:26:52.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py
+-rw-rw-rw-   0        0        0     4325 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/mg400_utils.py
+-rw-rw-rw-   0        0        0      233 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/__init__.py
+-rw-rw-rw-   0        0        0    10566 2023-06-07 08:12:11.000000 control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/jointed_utils.py
+-rw-rw-rw-   0        0        0      217 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Move/__init__.py
+-rw-rw-rw-   0        0        0    32385 2023-06-05 18:48:48.000000 control-lab-ly-1.1.0b1/src/controllably/Move/move_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.613438 control-lab-ly-1.1.0b1/src/controllably/Transfer/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.674765 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.714528 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.762359 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/
+-rw-rw-rw-   0        0        0      255 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/__init__.py
+-rw-rw-rw-   0        0        0     3440 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py
+-rw-rw-rw-   0        0        0    29858 2023-06-07 08:12:55.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py
+-rw-rw-rw-   0        0        0      332 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/__init__.py
+-rw-rw-rw-   0        0        0     7672 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py
+-rw-rw-rw-   0        0        0     3097 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.782331 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/
+-rw-rw-rw-   0        0        0      252 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/__init__.py
+-rw-rw-rw-   0        0        0     2792 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py
+-rw-rw-rw-   0        0        0    31695 2023-06-07 15:33:06.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py
+-rw-rw-rw-   0        0        0      364 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/__init__.py
+-rw-rw-rw-   0        0        0    13230 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/liquid_utils.py
+-rw-rw-rw-   0        0        0     3451 2023-04-21 08:27:57.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/syringe_lib.py
+-rw-rw-rw-   0        0        0    14600 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/syringe_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.795317 control-lab-ly-1.1.0b1/src/controllably/Transfer/Powder/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Powder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.809214 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.826776 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/Dobot/
+-rw-rw-rw-   0        0        0      397 2023-06-07 02:20:21.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/Dobot/__init__.py
+-rw-rw-rw-   0        0        0     8844 2023-06-07 08:13:13.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py
+-rw-rw-rw-   0        0        0      238 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/substrate_utils.py
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/src/controllably/Transfer/transfer_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.904830 control-lab-ly-1.1.0b1/src/controllably/View/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.926575 control-lab-ly-1.1.0b1/src/controllably/View/Classifiers/
+-rw-rw-rw-   0        0        0      333 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/View/Classifiers/__init__.py
+-rw-rw-rw-   0        0        0     2584 2023-06-08 02:41:36.000000 control-lab-ly-1.1.0b1/src/controllably/View/Classifiers/classifier_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.957284 control-lab-ly-1.1.0b1/src/controllably/View/Optical/
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/View/Optical/__init__.py
+-rw-rw-rw-   0        0        0     3163 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/View/Optical/optical_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.974305 control-lab-ly-1.1.0b1/src/controllably/View/Optical/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:51.000000 control-lab-ly-1.1.0b1/src/controllably/View/Optical/placeholders/__init__.py
+-rw-rw-rw-   0        0        0    15567 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Optical/placeholders/optical_camera.png
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.982357 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:56.992333 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:04:15.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.030189 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/
+-rw-rw-rw-   0        0        0       33 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/__init__.py
+-rw-rw-rw-   0        0        0    10147 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8.py
+-rw-rw-rw-   0        0        0     3821 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py
+-rw-rw-rw-   0        0        0      636 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py
+-rw-rw-rw-   0        0        0      819 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py
+-rw-rw-rw-   0        0        0      219 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.047742 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/placeholders/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/placeholders/__init__.py
+-rw-rw-rw-   0        0        0   148660 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/placeholders/infrared_camera.png
+-rw-rw-rw-   0        0        0     2988 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/src/controllably/View/Thermal/thermal_utils.py
+-rw-rw-rw-   0        0        0      304 2023-06-08 02:41:32.000000 control-lab-ly-1.1.0b1/src/controllably/View/__init__.py
+-rw-rw-rw-   0        0        0    15703 2023-06-07 14:50:19.000000 control-lab-ly-1.1.0b1/src/controllably/View/image.py
+-rw-rw-rw-   0        0        0    15898 2023-06-08 02:41:35.000000 control-lab-ly-1.1.0b1/src/controllably/View/view_utils.py
+-rw-rw-rw-   0        0        0      131 2023-06-05 18:11:26.000000 control-lab-ly-1.1.0b1/src/controllably/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.106130 control-lab-ly-1.1.0b1/src/controllably/misc/
+-rw-rw-rw-   0        0        0      627 2023-06-07 15:16:27.000000 control-lab-ly-1.1.0b1/src/controllably/misc/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/decorators.py
+-rw-rw-rw-   0        0        0     9596 2023-06-09 02:42:47.000000 control-lab-ly-1.1.0b1/src/controllably/misc/factory.py
+-rw-rw-rw-   0        0        0     7940 2023-06-13 09:57:18.000000 control-lab-ly-1.1.0b1/src/controllably/misc/helper.py
+-rw-rw-rw-   0        0        0    17547 2023-06-07 14:53:56.000000 control-lab-ly-1.1.0b1/src/controllably/misc/layout.py
+-rw-rw-rw-   0        0        0     2863 2023-06-07 08:11:52.000000 control-lab-ly-1.1.0b1/src/controllably/misc/logger.py
+-rw-rw-rw-   0        0        0     4543 2023-06-14 09:42:31.000000 control-lab-ly-1.1.0b1/src/controllably/misc/misc_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.110310 control-lab-ly-1.1.0b1/src/controllably/misc/templates/
+-rw-rw-rw-   0        0        0        0 2023-02-23 06:19:52.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.133215 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/
+-rw-rw-rw-   0        0        0        0 2023-02-23 14:08:10.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.149724 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/plugins/
+-rw-rw-rw-   0        0        0        0 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/plugins/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/plugins/plugin_template.py
+-rw-rw-rw-   0        0        0      439 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/registry.yaml
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.178290 control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/
+-rw-rw-rw-   0        0        0      772 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/config.yaml
+-rw-rw-rw-   0        0        0      987 2023-04-12 15:51:49.000000 control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/layout.json
+drwxrwxrwx   0        0        0        0 2023-06-15 06:28:57.312029 control-lab-ly-1.1.0b1/tests/
+-rw-rw-rw-   0        0        0      197 2023-04-21 15:18:23.000000 control-lab-ly-1.1.0b1/tests/test_camera_optical.py
+-rw-rw-rw-   0        0        0      230 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_camera_thermal.py
+-rw-rw-rw-   0        0        0      509 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_cartesian_ender.py
+-rw-rw-rw-   0        0        0      429 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_cartesian_primitiv.py
+-rw-rw-rw-   0        0        0      629 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0b1/tests/test_compound_liquidmover.py
+-rw-rw-rw-   0        0        0      801 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_compound_spin_printer.py
+-rw-rw-rw-   0        0        0      616 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_dobot_m1pro.py
+-rw-rw-rw-   0        0        0      651 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_dobot_mg400.py
+-rw-rw-rw-   0        0        0      324 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_electrical_keithley.py
+-rw-rw-rw-   0        0        0      392 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_film_spin.py
+-rw-rw-rw-   0        0        0      586 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/tests/test_heat_peltier.py
+-rw-rw-rw-   0        0        0      349 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_light_led_array.py
+-rw-rw-rw-   0        0        0      390 2023-05-04 14:05:17.000000 control-lab-ly-1.1.0b1/tests/test_liquid_sartorius.py
+-rw-rw-rw-   0        0        0      412 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_liquid_syringe_assembly.py
+-rw-rw-rw-   0        0        0      538 2023-05-04 09:11:29.000000 control-lab-ly-1.1.0b1/tests/test_liquid_tricontinent.py
+-rw-rw-rw-   0        0        0      239 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_mechanical_piezorobotics.py
+-rw-rw-rw-   0        0        0     1011 2023-05-25 07:11:07.000000 control-lab-ly-1.1.0b1/tests/test_mixture_shaker.py
+-rw-rw-rw-   0        0        0     2365 2023-06-15 02:45:10.000000 control-lab-ly-1.1.0b1/tests/test_panels.py
+-rw-rw-rw-   0        0        0      273 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_physical_balance.py
+-rw-rw-rw-   0        0        0      337 2023-04-11 09:18:51.000000 control-lab-ly-1.1.0b1/tests/test_pump_peristaltic.py
```

### Comparing `control-lab-ly-1.1.0b0/LICENSE.md` & `control-lab-ly-1.1.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/PKG-INFO` & `control-lab-ly-1.1.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.0b0
+Version: 1.1.0b1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -81,15 +81,15 @@
 
 ### View documentation
 Use the built-in guide to read the documentation for the package.
 ```python
 from controllably import guide_me
 guide_me()
 ```
-![Screenshot of the documentation guide](./assets/Documentation%20guide.png)
+![Screenshot of the documentation guide](https://raw.githubusercontent.com/kylejeanlewis/repo-readme-assets/main/control-lab-le/v1-1-0/assets/Documentation%20guide.png)
 
 Alternatively, details for each class / module / package can be explored by using the `help` function.
 ```python
 help(Ender)
 ```
 
 For basic usage, this is all you need to know. Check the documentation for more details on each class and function.
@@ -104,15 +104,15 @@
 import controllably as lab
 ```
 
 Optionally, you can set the safety policy for the session. This feature allows the user to prevent collisions before each movement is made. The safety policy has to be assigned before importing any of the `Mover` objects.
 ```python
 lab.set_safety('high')  # Notifies; Pauses for input before every move action
 lab.set_safety('low')   # Notifies; Waits for countdown before every move action
-lab.set_safety(None)    # Movement actions carry out without delay
+lab.set_safety(None)    # Carries out movement actions without delay
 
 # Import control-lab-ly classes only after setting the safety policy
 ```
 
 ### Contents
 1. [Setups](#1-creating-a-new-setup)
 2. [Decks](#2-managing-a-deck)
```

### Comparing `control-lab-ly-1.1.0b0/docs/CHANGELOG.md` & `control-lab-ly-1.1.0b1/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/docs/CODE_OF_CONDUCT.md` & `control-lab-ly-1.1.0b1/docs/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/docs/LICENSE.md` & `control-lab-ly-1.1.0b1/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/docs/README.md` & `control-lab-ly-1.1.0b1/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 ### View documentation
 Use the built-in guide to read the documentation for the package.
 ```python
 from controllably import guide_me
 guide_me()
 ```
-![Screenshot of the documentation guide](./assets/Documentation%20guide.png)
+![Screenshot of the documentation guide](https://raw.githubusercontent.com/kylejeanlewis/repo-readme-assets/main/control-lab-le/v1-1-0/assets/Documentation%20guide.png)
 
 Alternatively, details for each class / module / package can be explored by using the `help` function.
 ```python
 help(Ender)
 ```
 
 For basic usage, this is all you need to know. Check the documentation for more details on each class and function.
@@ -79,15 +79,15 @@
 import controllably as lab
 ```
 
 Optionally, you can set the safety policy for the session. This feature allows the user to prevent collisions before each movement is made. The safety policy has to be assigned before importing any of the `Mover` objects.
 ```python
 lab.set_safety('high')  # Notifies; Pauses for input before every move action
 lab.set_safety('low')   # Notifies; Waits for countdown before every move action
-lab.set_safety(None)    # Movement actions carry out without delay
+lab.set_safety(None)    # Carries out movement actions without delay
 
 # Import control-lab-ly classes only after setting the safety policy
 ```
 
 ### Contents
 1. [Setups](#1-creating-a-new-setup)
 2. [Decks](#2-managing-a-deck)
```

### Comparing `control-lab-ly-1.1.0b0/docs/assets/Documentation guide.png` & `control-lab-ly-1.1.0b1/docs/assets/Documentation guide.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/setup.cfg` & `control-lab-ly-1.1.0b1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6e 7472 6f6c 2d6c 6162 2d6c   = control-lab-l
 00000020: 790d 0a76 6572 7369 6f6e 203d 2031 2e31  y..version = 1.1
-00000030: 2e30 2d62 300d 0a64 6573 6372 6970 7469  .0-b0..descripti
+00000030: 2e30 2d62 310d 0a64 6573 6372 6970 7469  .0-b1..descripti
 00000040: 6f6e 203d 204c 6162 2045 7175 6970 6d65  on = Lab Equipme
 00000050: 6e74 2041 7574 6f6d 6174 696f 6e20 5061  nt Automation Pa
 00000060: 636b 6167 650d 0a6c 6f6e 675f 6465 7363  ckage..long_desc
 00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000080: 646f 6373 2f52 4541 444d 452e 6d64 2c20  docs/README.md, 
 00000090: 646f 6373 2f43 4841 4e47 454c 4f47 2e6d  docs/CHANGELOG.m
 000000a0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
```

### Comparing `control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/PKG-INFO` & `control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: control-lab-ly
-Version: 1.1.0b0
+Version: 1.1.0b1
 Summary: Lab Equipment Automation Package
 Home-page: https://github.com/kylejeanlewis/control-lab-le
 Author: Chang Jie Leong
 Author-email: changjie.leong@outlook.com
 License: MIT
 Project-URL: GitHub, https://github.com/kylejeanlewis/control-lab-le
 Project-URL: Documentation, https://github.com/kylejeanlewis/control-lab-le/blob/main/docs/README.md
@@ -81,15 +81,15 @@
 
 ### View documentation
 Use the built-in guide to read the documentation for the package.
 ```python
 from controllably import guide_me
 guide_me()
 ```
-![Screenshot of the documentation guide](./assets/Documentation%20guide.png)
+![Screenshot of the documentation guide](https://raw.githubusercontent.com/kylejeanlewis/repo-readme-assets/main/control-lab-le/v1-1-0/assets/Documentation%20guide.png)
 
 Alternatively, details for each class / module / package can be explored by using the `help` function.
 ```python
 help(Ender)
 ```
 
 For basic usage, this is all you need to know. Check the documentation for more details on each class and function.
@@ -104,15 +104,15 @@
 import controllably as lab
 ```
 
 Optionally, you can set the safety policy for the session. This feature allows the user to prevent collisions before each movement is made. The safety policy has to be assigned before importing any of the `Mover` objects.
 ```python
 lab.set_safety('high')  # Notifies; Pauses for input before every move action
 lab.set_safety('low')   # Notifies; Waits for countdown before every move action
-lab.set_safety(None)    # Movement actions carry out without delay
+lab.set_safety(None)    # Carries out movement actions without delay
 
 # Import control-lab-ly classes only after setting the safety policy
 ```
 
 ### Contents
 1. [Setups](#1-creating-a-new-setup)
 2. [Decks](#2-managing-a-deck)
```

### Comparing `control-lab-ly-1.1.0b0/src/control_lab_ly.egg-info/SOURCES.txt` & `control-lab-ly-1.1.0b1/src/control_lab_ly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Compound/LiquidMover/liquidmover_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Compound/LiquidMover/liquidmover_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Compound/compound_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Compound/compound_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/__init__.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/maker_panel.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/maker_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/measurer_panel.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/measurer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/mover_panel.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/mover_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/transfer_liquid_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Basic/viewer_panel.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Basic/viewer_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/loader_panel.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/loader_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/pop_ups.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/pop_ups.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/Elements/templates.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/Elements/templates.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/__init__.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/_guibuilder.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/_guibuilder.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/compound_panel.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/compound_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/gui_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/gui_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/guide_panel.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/guide_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Control/GUI/multichannel_panel.py` & `control-lab-ly-1.1.0b1/src/controllably/Control/GUI/multichannel_panel.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Make/Heat/peltier_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Make/Heat/peltier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Make/Light/led_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Make/Light/led_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/orbital_shaker_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py` & `control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py` & `control-lab-ly-1.1.0b1/src/controllably/Make/Mixture/QInstruments/qinstruments_api/qinstruments_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Make/ThinFilm/spinner_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Make/ThinFilm/spinner_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Make/make_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Make/make_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_device.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_lib.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/keithley_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/keithley_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Electrical/Keithley/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_device.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/piezorobotics_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Mechanical/PiezoRobotics/programs/base_programs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/balance_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/balance_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/Physical/force_sensor_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/Physical/force_sensor_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/__init__.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/instrument_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/instrument_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/measure_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/measure_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Measure/program_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Measure/program_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/cartesian_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/cartesian_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/ender_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/ender_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Move/Cartesian/primitiv_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Move/Cartesian/primitiv_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py` & `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_api/dobot_api.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/dobot_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/dobot_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/m1pro_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/m1pro_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/Dobot/mg400_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/Dobot/mg400_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Move/Jointed/jointed_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Move/Jointed/jointed_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Move/move_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Move/move_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/TriContinent/tricontinent_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/peristaltic_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Pumps/pump_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Pumps/pump_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/Sartorius/sartorius_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/liquid_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/liquid_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/syringe_lib.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/syringe_lib.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Liquid/syringe_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Liquid/syringe_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/Dobot/dobot_attachments.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/Transfer/Substrate/substrate_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/Transfer/Substrate/substrate_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/Classifiers/classifier_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/View/Classifiers/classifier_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/Optical/optical_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/View/Optical/optical_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/Optical/placeholders/optical_camera.png` & `control-lab-ly-1.1.0b1/src/controllably/View/Optical/placeholders/optical_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8.py` & `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py` & `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_camera_feed.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py` & `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_regs.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/Flir/ax8/ax8_modbus_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/placeholders/infrared_camera.png` & `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/placeholders/infrared_camera.png`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/Thermal/thermal_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/View/Thermal/thermal_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/image.py` & `control-lab-ly-1.1.0b1/src/controllably/View/image.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/View/view_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/View/view_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/__init__.py` & `control-lab-ly-1.1.0b1/src/controllably/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/decorators.py` & `control-lab-ly-1.1.0b1/src/controllably/misc/decorators.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/factory.py` & `control-lab-ly-1.1.0b1/src/controllably/misc/factory.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/helper.py` & `control-lab-ly-1.1.0b1/src/controllably/misc/helper.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/layout.py` & `control-lab-ly-1.1.0b1/src/controllably/misc/layout.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/logger.py` & `control-lab-ly-1.1.0b1/src/controllably/misc/logger.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/misc_utils.py` & `control-lab-ly-1.1.0b1/src/controllably/misc/misc_utils.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/templates/configs/plugins/plugin_template.py` & `control-lab-ly-1.1.0b1/src/controllably/misc/templates/configs/plugins/plugin_template.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/__init__.py` & `control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/config.yaml` & `control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/config.yaml`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/src/controllably/misc/templates/setup/layout.json` & `control-lab-ly-1.1.0b1/src/controllably/misc/templates/setup/layout.json`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/tests/test_compound_liquidmover.py` & `control-lab-ly-1.1.0b1/tests/test_compound_liquidmover.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/tests/test_compound_spin_printer.py` & `control-lab-ly-1.1.0b1/tests/test_compound_spin_printer.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/tests/test_dobot_m1pro.py` & `control-lab-ly-1.1.0b1/tests/test_dobot_m1pro.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/tests/test_dobot_mg400.py` & `control-lab-ly-1.1.0b1/tests/test_dobot_mg400.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/tests/test_heat_peltier.py` & `control-lab-ly-1.1.0b1/tests/test_heat_peltier.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/tests/test_liquid_tricontinent.py` & `control-lab-ly-1.1.0b1/tests/test_liquid_tricontinent.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/tests/test_mixture_shaker.py` & `control-lab-ly-1.1.0b1/tests/test_mixture_shaker.py`

 * *Files identical despite different names*

### Comparing `control-lab-ly-1.1.0b0/tests/test_panels.py` & `control-lab-ly-1.1.0b1/tests/test_panels.py`

 * *Files identical despite different names*

