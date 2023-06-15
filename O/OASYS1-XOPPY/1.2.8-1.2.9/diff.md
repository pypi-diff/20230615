# Comparing `tmp/OASYS1-XOPPY-1.2.8.tar.gz` & `tmp/OASYS1-XOPPY-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OASYS1-XOPPY-1.2.8.tar", last modified: Mon Dec 12 14:19:14 2022, max compression
+gzip compressed data, was "dist/OASYS1-XOPPY-1.2.9.tar", last modified: Tue Dec 13 11:01:36 2022, max compression
```

## Comparing `OASYS1-XOPPY-1.2.8.tar` & `OASYS1-XOPPY-1.2.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/
--rw-r--r--   0 srio      (4230) soft      (3401)     1304 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/LICENSE
--rw-r--r--   0 srio      (4230) soft      (3401)      585 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/MANIFEST.in
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/
--rw-r--r--   0 srio      (4230) soft      (3401)      771 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)     4504 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/SOURCES.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        1 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/dependency_links.txt
--rw-r--r--   0 srio      (4230) soft      (3401)      162 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/entry_points.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       62 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/namespace_packages.txt
--rw-r--r--   0 srio      (4230) soft      (3401)        1 2022-05-10 15:11:00.000000 OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/not-zip-safe
--rw-r--r--   0 srio      (4230) soft      (3401)       68 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/requires.txt
--rw-r--r--   0 srio      (4230) soft      (3401)       14 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/top_level.txt
--rw-r--r--   0 srio      (4230) soft      (3401)      771 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/PKG-INFO
--rw-r--r--   0 srio      (4230) soft      (3401)       63 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/README.txt
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/
--rw-r--r--   0 srio      (4230) soft      (3401)       81 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/
--rw-r--r--   0 srio      (4230) soft      (3401)       82 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/menu/
--rwxr-xr-x   0 srio      (4230) soft      (3401)       42 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/menu/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1601 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/menu/xoppy_tools_menu.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/
--rw-r--r--   0 srio      (4230) soft      (3401)       81 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     8261 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/python_script.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/__init__.py
--rwxr-xr-x   0 srio      (4230) soft      (3401)    15318 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/itemmodels.py
--rw-r--r--   0 srio      (4230) soft      (3401)    10921 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/python_script.py
--rwxr-xr-x   0 srio      (4230) soft      (3401)     4432 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/value.py
--rwxr-xr-x   0 srio      (4230) soft      (3401)    18576 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/variable.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1084 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/xoppy_pymca_tools.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/
--rw-r--r--   0 srio      (4230) soft      (3401)       80 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/
--rw-r--r--   0 srio      (4230) soft      (3401)        0 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)    14408 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/image_view_with_fwhm.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1142 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/messages.py
--rw-r--r--   0 srio      (4230) soft      (3401)    22982 2022-10-05 08:10:13.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/ow_xoppy_widget.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1236 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/text_window.py
--rw-r--r--   0 srio      (4230) soft      (3401)     1659 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/xoppy_util.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/
--rw-r--r--   0 srio      (4230) soft      (3401)      383 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/
--rw-r--r--   0 srio      (4230) soft      (3401)   137447 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/obsolete_power3d.png
--rw-r--r--   0 srio      (4230) soft      (3401)    70456 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/srcalc.png
--rw-r--r--   0 srio      (4230) soft      (3401)    14594 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_2.png
--rw-r--r--   0 srio      (4230) soft      (3401)    79168 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_mare.png
--rw-r--r--   0 srio      (4230) soft      (3401)     5811 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_mlayer.png
--rw-r--r--   0 srio      (4230) soft      (3401)    30807 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_power3d.png
--rw-r--r--   0 srio      (4230) soft      (3401)     1613 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xcrosssec.png
--rw-r--r--   0 srio      (4230) soft      (3401)    10376 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xcrystal.png
--rw-r--r--   0 srio      (4230) soft      (3401)     1172 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xf0.png
--rw-r--r--   0 srio      (4230) soft      (3401)    13959 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xf1f2.png
--rw-r--r--   0 srio      (4230) soft      (3401)     1273 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xfh.png
--rw-r--r--   0 srio      (4230) soft      (3401)     3903 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xinpro.png
--rw-r--r--   0 srio      (4230) soft      (3401)     7802 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xpowder_fml.png
--rw-r--r--   0 srio      (4230) soft      (3401)    18851 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xpower.png
--rw-r--r--   0 srio      (4230) soft      (3401)     2858 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xxcom.png
--rw-r--r--   0 srio      (4230) soft      (3401)     7980 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xraylib.png
--rw-r--r--   0 srio      (4230) soft      (3401)    11280 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/mare.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/misc/
--rw-r--r--   0 srio      (4230) soft      (3401)    15357 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/misc/xraylib.jpg
--rw-r--r--   0 srio      (4230) soft      (3401)    24303 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/multilayer.py
--rw-r--r--   0 srio      (4230) soft      (3401)    45173 2022-11-24 15:53:34.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/power3Dcomponent.py
--rw-r--r--   0 srio      (4230) soft      (3401)    83050 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/srcalc_idpower.py
--rw-r--r--   0 srio      (4230) soft      (3401)    14838 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xcrosssec.py
--rw-r--r--   0 srio      (4230) soft      (3401)    35550 2022-05-16 08:17:47.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xcrystal.py
--rw-r--r--   0 srio      (4230) soft      (3401)    10041 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xf0.py
--rw-r--r--   0 srio      (4230) soft      (3401)    21384 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xf1f2.py
--rw-r--r--   0 srio      (4230) soft      (3401)    16534 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xfh.py
--rw-r--r--   0 srio      (4230) soft      (3401)    13771 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xinpro.py
--rw-r--r--   0 srio      (4230) soft      (3401)    10029 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xpowder_fml.py
--rw-r--r--   0 srio      (4230) soft      (3401)    45837 2022-11-24 15:53:34.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xpower.py
--rw-r--r--   0 srio      (4230) soft      (3401)    21147 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xraylib_widget.py
--rw-r--r--   0 srio      (4230) soft      (3401)    10114 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xxcom.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/
--rw-r--r--   0 srio      (4230) soft      (3401)      349 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/__init__.py
--rw-r--r--   0 srio      (4230) soft      (3401)     6134 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/black_body.py
--rw-r--r--   0 srio      (4230) soft      (3401)    22317 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/bm.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/
--rw-r--r--   0 srio      (4230) soft      (3401)    14594 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_2.png
--rw-r--r--   0 srio      (4230) soft      (3401)    28309 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_black_body.png
--rwxr-xr-x   0 srio      (4230) soft      (3401)    18339 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_bm.png
--rw-r--r--   0 srio      (4230) soft      (3401)    17867 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_power_density.png
--rw-r--r--   0 srio      (4230) soft      (3401)   171020 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_radiation.png
--rw-r--r--   0 srio      (4230) soft      (3401)    17867 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_spectrum.png
--rw-r--r--   0 srio      (4230) soft      (3401)    60152 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_wiggler_radiation.png
--rw-r--r--   0 srio      (4230) soft      (3401)    16070 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_ws.png
--rw-r--r--   0 srio      (4230) soft      (3401)    12481 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_xtc.png
--rw-r--r--   0 srio      (4230) soft      (3401)    15045 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_xtube_w.png
--rw-r--r--   0 srio      (4230) soft      (3401)    20580 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_xtubes.png
--rw-r--r--   0 srio      (4230) soft      (3401)    16070 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_xwiggler.png
--rw-r--r--   0 srio      (4230) soft      (3401)    24693 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/tc_slit.py
--rw-r--r--   0 srio      (4230) soft      (3401)    28017 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/undulator_power_density.py
--rw-r--r--   0 srio      (4230) soft      (3401)    36501 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/undulator_radiation.py
--rw-r--r--   0 srio      (4230) soft      (3401)    21817 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/undulator_spectrum.py
--rw-r--r--   0 srio      (4230) soft      (3401)    37717 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/wiggler_radiation.py
--rw-r--r--   0 srio      (4230) soft      (3401)    14150 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/ws.py
--rw-r--r--   0 srio      (4230) soft      (3401)    25564 2022-12-12 14:17:39.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xtc.py
--rw-r--r--   0 srio      (4230) soft      (3401)    26022 2022-12-12 14:16:31.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xtcap.py
--rw-r--r--   0 srio      (4230) soft      (3401)     5283 2022-05-17 14:56:54.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xtube_w.py
--rw-r--r--   0 srio      (4230) soft      (3401)     4733 2022-05-17 14:56:54.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xtubes.py
--rw-r--r--   0 srio      (4230) soft      (3401)    15955 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xwiggler.py
--rw-r--r--   0 srio      (4230) soft      (3401)    47390 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/yaup.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/tools/
--rw-r--r--   0 srio      (4230) soft      (3401)      278 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/tools/__init__.py
-drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/tools/icons/
--rwxr-xr-x   0 srio      (4230) soft      (3401)      514 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/tools/icons/histogram.png
--rw-r--r--   0 srio      (4230) soft      (3401)    14594 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/tools/icons/xoppy_2.png
--rw-r--r--   0 srio      (4230) soft      (3401)     5307 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/tools/plot_simple_exchange.py
--rw-r--r--   0 srio      (4230) soft      (3401)       38 2022-12-12 14:19:14.000000 OASYS1-XOPPY-1.2.8/setup.cfg
--rw-r--r--   0 srio      (4230) soft      (3401)     2961 2022-12-12 14:18:27.000000 OASYS1-XOPPY-1.2.8/setup.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/
+-rw-r--r--   0 srio      (4230) soft      (3401)     1304 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/LICENSE
+-rw-r--r--   0 srio      (4230) soft      (3401)      585 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/MANIFEST.in
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/
+-rw-r--r--   0 srio      (4230) soft      (3401)      771 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)     4504 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/SOURCES.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        1 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/dependency_links.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)      162 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/entry_points.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       62 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/namespace_packages.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)        1 2022-05-10 15:11:00.000000 OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/not-zip-safe
+-rw-r--r--   0 srio      (4230) soft      (3401)       68 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/requires.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)       14 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/top_level.txt
+-rw-r--r--   0 srio      (4230) soft      (3401)      771 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/PKG-INFO
+-rw-r--r--   0 srio      (4230) soft      (3401)       63 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/README.txt
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/
+-rw-r--r--   0 srio      (4230) soft      (3401)       81 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/
+-rw-r--r--   0 srio      (4230) soft      (3401)       82 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/menu/
+-rwxr-xr-x   0 srio      (4230) soft      (3401)       42 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/menu/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1601 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/menu/xoppy_tools_menu.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/
+-rw-r--r--   0 srio      (4230) soft      (3401)       81 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     8261 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/python_script.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/__init__.py
+-rwxr-xr-x   0 srio      (4230) soft      (3401)    15318 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/itemmodels.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    10921 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/python_script.py
+-rwxr-xr-x   0 srio      (4230) soft      (3401)     4432 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/value.py
+-rwxr-xr-x   0 srio      (4230) soft      (3401)    18576 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/variable.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1084 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/xoppy_pymca_tools.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/
+-rw-r--r--   0 srio      (4230) soft      (3401)       80 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/
+-rw-r--r--   0 srio      (4230) soft      (3401)        0 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    14408 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/image_view_with_fwhm.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1142 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/messages.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    22982 2022-10-05 08:10:13.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/ow_xoppy_widget.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1236 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/text_window.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     1659 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/xoppy_util.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/
+-rw-r--r--   0 srio      (4230) soft      (3401)      383 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/
+-rw-r--r--   0 srio      (4230) soft      (3401)   137447 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/obsolete_power3d.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    70456 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/srcalc.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    14594 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_2.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    79168 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_mare.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     5811 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_mlayer.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    30807 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_power3d.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     1613 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xcrosssec.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    10376 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xcrystal.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     1172 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xf0.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    13959 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xf1f2.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     1273 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xfh.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     3903 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xinpro.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     7802 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xpowder_fml.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    18851 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xpower.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     2858 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xxcom.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     7980 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xraylib.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    11280 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/mare.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/misc/
+-rw-r--r--   0 srio      (4230) soft      (3401)    15357 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/misc/xraylib.jpg
+-rw-r--r--   0 srio      (4230) soft      (3401)    24303 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/multilayer.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    45173 2022-11-24 15:53:34.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/power3Dcomponent.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    83050 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/srcalc_idpower.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    14838 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xcrosssec.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    35550 2022-05-16 08:17:47.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xcrystal.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    10041 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xf0.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    21384 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xf1f2.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    16534 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xfh.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    13771 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xinpro.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    10029 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xpowder_fml.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    45837 2022-11-24 15:53:34.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xpower.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    21147 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xraylib_widget.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    10114 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xxcom.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/
+-rw-r--r--   0 srio      (4230) soft      (3401)      349 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/__init__.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     6134 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/black_body.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    22317 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/bm.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/
+-rw-r--r--   0 srio      (4230) soft      (3401)    14594 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_2.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    28309 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_black_body.png
+-rwxr-xr-x   0 srio      (4230) soft      (3401)    18339 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_bm.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    17867 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_power_density.png
+-rw-r--r--   0 srio      (4230) soft      (3401)   171020 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_radiation.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    17867 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_spectrum.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    60152 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_wiggler_radiation.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    16070 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_ws.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    12481 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_xtc.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    15045 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_xtube_w.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    20580 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_xtubes.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    16070 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_xwiggler.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    24693 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/tc_slit.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    28017 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/undulator_power_density.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    36501 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/undulator_radiation.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    21817 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/undulator_spectrum.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    37717 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/wiggler_radiation.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    14150 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/ws.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    25564 2022-12-12 14:17:39.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xtc.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    26022 2022-12-12 14:16:31.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xtcap.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     5283 2022-05-17 14:56:54.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xtube_w.py
+-rw-r--r--   0 srio      (4230) soft      (3401)     4733 2022-05-17 14:56:54.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xtubes.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    15955 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xwiggler.py
+-rw-r--r--   0 srio      (4230) soft      (3401)    47390 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/yaup.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/tools/
+-rw-r--r--   0 srio      (4230) soft      (3401)      278 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/tools/__init__.py
+drwxr-xr-x   0 srio      (4230) soft      (3401)        0 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/tools/icons/
+-rwxr-xr-x   0 srio      (4230) soft      (3401)      514 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/tools/icons/histogram.png
+-rw-r--r--   0 srio      (4230) soft      (3401)    14594 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/tools/icons/xoppy_2.png
+-rw-r--r--   0 srio      (4230) soft      (3401)     5307 2022-05-10 14:36:30.000000 OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/tools/plot_simple_exchange.py
+-rw-r--r--   0 srio      (4230) soft      (3401)       38 2022-12-13 11:01:36.000000 OASYS1-XOPPY-1.2.9/setup.cfg
+-rw-r--r--   0 srio      (4230) soft      (3401)     2961 2022-12-13 11:00:06.000000 OASYS1-XOPPY-1.2.9/setup.py
```

### Comparing `OASYS1-XOPPY-1.2.8/LICENSE` & `OASYS1-XOPPY-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/MANIFEST.in` & `OASYS1-XOPPY-1.2.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/PKG-INFO` & `OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OASYS1-XOPPY
-Version: 1.2.8
+Version: 1.2.9
 Summary: XOPPY: XOP (X-ray oriented programs) in Python
 Home-page: https://github.com/oasys-kit/XOPPY
 Author: Manuel Sanchez del Rio, Luca Rebuffi, and Bioinformatics Laboratory, FRI UL
 Author-email: srio@esrf.eu, lrebuffi@anl.gov
 License: GPLv3
 Download-URL: https://github.com/oasys-kit/XOPPY
 Keywords: X-ray optics,simulator,oasys1
```

### Comparing `OASYS1-XOPPY-1.2.8/OASYS1_XOPPY.egg-info/SOURCES.txt` & `OASYS1-XOPPY-1.2.9/OASYS1_XOPPY.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/PKG-INFO` & `OASYS1-XOPPY-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OASYS1-XOPPY
-Version: 1.2.8
+Version: 1.2.9
 Summary: XOPPY: XOP (X-ray oriented programs) in Python
 Home-page: https://github.com/oasys-kit/XOPPY
 Author: Manuel Sanchez del Rio, Luca Rebuffi, and Bioinformatics Laboratory, FRI UL
 Author-email: srio@esrf.eu, lrebuffi@anl.gov
 License: GPLv3
 Download-URL: https://github.com/oasys-kit/XOPPY
 Keywords: X-ray optics,simulator,oasys1
```

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/menu/xoppy_tools_menu.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/menu/xoppy_tools_menu.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/python_script.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/python_script.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/itemmodels.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/itemmodels.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/python_script.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/python_script.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/value.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/value.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/script/variable.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/script/variable.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/util/xoppy_pymca_tools.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/util/xoppy_pymca_tools.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/image_view_with_fwhm.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/image_view_with_fwhm.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/messages.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/messages.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/ow_xoppy_widget.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/ow_xoppy_widget.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/text_window.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/text_window.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/gui/xoppy_util.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/gui/xoppy_util.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/obsolete_power3d.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/obsolete_power3d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/srcalc.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/srcalc.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_2.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_mare.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_mare.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_mlayer.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_mlayer.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_power3d.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_power3d.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xcrosssec.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xcrosssec.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xcrystal.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xcrystal.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xf0.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xf0.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xf1f2.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xf1f2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xfh.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xfh.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xinpro.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xinpro.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xpowder_fml.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xpowder_fml.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xpower.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xpower.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xoppy_xxcom.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xoppy_xxcom.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/icons/xraylib.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/icons/xraylib.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/mare.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/mare.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/misc/xraylib.jpg` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/misc/xraylib.jpg`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/multilayer.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/multilayer.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/power3Dcomponent.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/power3Dcomponent.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/srcalc_idpower.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/srcalc_idpower.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xcrosssec.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xcrosssec.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xcrystal.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xcrystal.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xf0.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xf0.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xf1f2.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xf1f2.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xfh.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xfh.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xinpro.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xinpro.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xpowder_fml.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xpowder_fml.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xpower.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xpower.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xraylib_widget.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xraylib_widget.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/optics/xxcom.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/optics/xxcom.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/black_body.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/black_body.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/bm.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/bm.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_2.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_black_body.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_black_body.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_bm.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_bm.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_power_density.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_power_density.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_radiation.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_radiation.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_spectrum.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_undulator_spectrum.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_wiggler_radiation.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_wiggler_radiation.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_ws.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_ws.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_xtc.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_xtc.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_xtube_w.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_xtube_w.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_xtubes.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_xtubes.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/icons/xoppy_xwiggler.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/icons/xoppy_xwiggler.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/tc_slit.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/tc_slit.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/undulator_power_density.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/undulator_power_density.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/undulator_radiation.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/undulator_radiation.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/undulator_spectrum.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/undulator_spectrum.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/wiggler_radiation.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/wiggler_radiation.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/ws.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/ws.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xtc.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xtc.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xtcap.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xtcap.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xtube_w.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xtube_w.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xtubes.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xtubes.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/xwiggler.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/xwiggler.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/source/yaup.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/source/yaup.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/tools/icons/histogram.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/tools/icons/histogram.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/tools/icons/xoppy_2.png` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/tools/icons/xoppy_2.png`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/orangecontrib/xoppy/widgets/tools/plot_simple_exchange.py` & `OASYS1-XOPPY-1.2.9/orangecontrib/xoppy/widgets/tools/plot_simple_exchange.py`

 * *Files identical despite different names*

### Comparing `OASYS1-XOPPY-1.2.8/setup.py` & `OASYS1-XOPPY-1.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'OASYS1-XOPPY'
-VERSION = '1.2.8'
+VERSION = '1.2.9'
 ISRELEASED = False
 
 DESCRIPTION = 'XOPPY: XOP (X-ray oriented programs) in Python'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.txt')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Manuel Sanchez del Rio, Luca Rebuffi, and Bioinformatics Laboratory, FRI UL'
 AUTHOR_EMAIL = 'srio@esrf.eu, lrebuffi@anl.gov'
@@ -39,16 +39,16 @@
     'setuptools',
 )
 
 INSTALL_REQUIRES = (
     'oasys1>=1.2.62',
     'oasys-srwpy',
     'pySRU',
-    'srxraylib>=1.0.30',  # remove when oasys1 requires at least this version
-    'xoppylib>=1.0.16',
+    'srxraylib>=1.0.39',  # remove when oasys1 requires at least this version
+    'xoppylib>=1.0.17',
 )
 
 PACKAGES = find_packages(exclude=('*.tests', '*.tests.*', 'tests.*', 'tests'))
 
 PACKAGE_DATA = {
     "orangecontrib.xoppy.widgets.source":["icons/*.png", "icons/*.jpg"],
     "orangecontrib.xoppy.widgets.optics":["icons/*.png", "icons/*.jpg", "misc/*.*"],
```

