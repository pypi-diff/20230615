# Comparing `tmp/cf-plot-3.2.6.tar.gz` & `tmp/cf-plot-3.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf-plot-3.2.6.tar", last modified: Thu Mar 30 14:33:58 2023, max compression
+gzip compressed data, was "cf-plot-3.2.7.tar", last modified: Thu Mar 30 16:15:44 2023, max compression
```

## Comparing `cf-plot-3.2.6.tar` & `cf-plot-3.2.7.tar`

### file list

```diff
@@ -1,225 +1,225 @@
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-30 14:33:58.071957 cf-plot-3.2.6/
--rw-r--r--   0 andy      (1000) andy      (1000)     1065 2016-01-26 13:42:08.000000 cf-plot-3.2.6/LICENSE.txt
--rw-r--r--   0 andy      (1000) andy      (1000)      123 2015-11-27 16:55:33.000000 cf-plot-3.2.6/MANIFEST.in
--rw-rw-r--   0 andy      (1000) andy      (1000)      569 2023-03-30 14:33:58.071957 cf-plot-3.2.6/PKG-INFO
--rw-r--r--   0 andy      (1000) andy      (1000)      251 2016-02-04 11:30:15.000000 cf-plot-3.2.6/README.md
--rw-r--r--   0 andy      (1000) andy      (1000)      253 2019-05-13 16:06:32.000000 cf-plot-3.2.6/README.txt
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-30 14:33:58.035958 cf-plot-3.2.6/cf_plot.egg-info/
--rw-rw-r--   0 andy      (1000) andy      (1000)      569 2023-03-30 14:33:57.000000 cf-plot-3.2.6/cf_plot.egg-info/PKG-INFO
--rw-rw-r--   0 andy      (1000) andy      (1000)     6757 2023-03-30 14:33:57.000000 cf-plot-3.2.6/cf_plot.egg-info/SOURCES.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-03-30 14:33:57.000000 cf-plot-3.2.6/cf_plot.egg-info/dependency_links.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)       64 2023-03-30 14:33:57.000000 cf-plot-3.2.6/cf_plot.egg-info/requires.txt
--rw-rw-r--   0 andy      (1000) andy      (1000)        7 2023-03-30 14:33:57.000000 cf-plot-3.2.6/cf_plot.egg-info/top_level.txt
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-30 14:33:58.035958 cf-plot-3.2.6/cfplot/
--rw-r--r--   0 andy      (1000) andy      (1000)      368 2023-03-30 14:30:05.000000 cf-plot-3.2.6/cfplot/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)   354464 2023-03-30 14:19:54.000000 cf-plot-3.2.6/cfplot/cfplot.py
-drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-30 14:33:58.071957 cf-plot-3.2.6/cfplot/colourmaps/
--rw-r--r--   0 andy      (1000) andy      (1000)     2708 2013-08-06 14:42:16.000000 cf-plot-3.2.6/cfplot/colourmaps/3gauss.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2746 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/3saw.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:57:38.000000 cf-plot-3.2.6/cfplot/colourmaps/BkBlAqGrYeOrReViWh200.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:57:48.000000 cf-plot-3.2.6/cfplot/colourmaps/BlAqGrYeOrRe.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:59:26.000000 cf-plot-3.2.6/cfplot/colourmaps/BlAqGrYeOrReVi200.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:59:34.000000 cf-plot-3.2.6/cfplot/colourmaps/BlGrYeOrReVi200.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1248 2013-08-06 14:59:56.000000 cf-plot-3.2.6/cfplot/colourmaps/BlRe.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:59:42.000000 cf-plot-3.2.6/cfplot/colourmaps/BlWhRe.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      414 2013-08-06 15:00:06.000000 cf-plot-3.2.6/cfplot/colourmaps/BlueDarkOrange18.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      414 2013-08-06 15:00:18.000000 cf-plot-3.2.6/cfplot/colourmaps/BlueDarkRed18.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      322 2013-08-06 15:00:28.000000 cf-plot-3.2.6/cfplot/colourmaps/BlueGreen14.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     4991 2013-08-06 14:59:48.000000 cf-plot-3.2.6/cfplot/colourmaps/BlueRed.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5010 2013-08-06 14:57:56.000000 cf-plot-3.2.6/cfplot/colourmaps/BlueRedGray.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5129 2013-08-06 15:00:38.000000 cf-plot-3.2.6/cfplot/colourmaps/BlueWhiteOrangeRed.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5272 2013-08-06 15:00:46.000000 cf-plot-3.2.6/cfplot/colourmaps/BlueYellowRed.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1390 2017-01-23 17:36:40.000000 cf-plot-3.2.6/cfplot/colourmaps/BrBG.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      276 2013-08-06 14:59:18.000000 cf-plot-3.2.6/cfplot/colourmaps/BrownBlue12.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      276 2013-08-06 15:01:00.000000 cf-plot-3.2.6/cfplot/colourmaps/Cat12.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1554 2013-08-06 15:01:08.000000 cf-plot-3.2.6/cfplot/colourmaps/GHRSST_anomaly.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5098 2013-08-06 14:59:08.000000 cf-plot-3.2.6/cfplot/colourmaps/GrayWhiteGray.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      368 2013-08-06 14:59:00.000000 cf-plot-3.2.6/cfplot/colourmaps/GreenMagenta16.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     4976 2013-08-06 14:58:02.000000 cf-plot-3.2.6/cfplot/colourmaps/GreenYellow.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5213 2013-08-06 14:58:40.000000 cf-plot-3.2.6/cfplot/colourmaps/OceanLakeLandSnow.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      525 2013-08-06 14:58:28.000000 cf-plot-3.2.6/cfplot/colourmaps/StepSeq25.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:42:30.000000 cf-plot-3.2.6/cfplot/colourmaps/ViBlGrWhYeOrRe.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:58:14.000000 cf-plot-3.2.6/cfplot/colourmaps/WhBlGrYeRe.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:57:28.000000 cf-plot-3.2.6/cfplot/colourmaps/WhBlReWh.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:57:00.000000 cf-plot-3.2.6/cfplot/colourmaps/WhViBlGrYeOrRe.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:56:48.000000 cf-plot-3.2.6/cfplot/colourmaps/WhViBlGrYeOrReWh.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5104 2013-08-06 14:56:38.000000 cf-plot-3.2.6/cfplot/colourmaps/WhiteBlue.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5126 2013-08-06 14:56:30.000000 cf-plot-3.2.6/cfplot/colourmaps/WhiteBlueGreenYellowRed.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5100 2013-08-06 14:56:16.000000 cf-plot-3.2.6/cfplot/colourmaps/WhiteGreen.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5105 2013-08-06 14:55:48.000000 cf-plot-3.2.6/cfplot/colourmaps/WhiteYellowOrangeRed.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)        0 2015-11-27 13:32:06.000000 cf-plot-3.2.6/cfplot/colourmaps/__init__.py
--rw-r--r--   0 andy      (1000) andy      (1000)      183 2013-08-06 14:56:08.000000 cf-plot-3.2.6/cfplot/colourmaps/amwg.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     4064 2013-09-12 13:37:22.000000 cf-plot-3.2.6/cfplot/colourmaps/amwg256.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-09-12 13:37:46.000000 cf-plot-3.2.6/cfplot/colourmaps/amwg_blueyellowred.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1415 2016-01-11 15:29:50.000000 cf-plot-3.2.6/cfplot/colourmaps/arctic.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      715 2013-08-06 14:55:40.000000 cf-plot-3.2.6/cfplot/colourmaps/cmp_b2r.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      238 2013-08-06 14:55:30.000000 cf-plot-3.2.6/cfplot/colourmaps/cmp_flux.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      733 2013-08-06 14:42:04.000000 cf-plot-3.2.6/cfplot/colourmaps/cmp_haxby.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      337 2016-01-11 10:38:42.000000 cf-plot-3.2.6/cfplot/colourmaps/colombia.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)    14626 2013-08-06 14:10:26.000000 cf-plot-3.2.6/cfplot/colourmaps/colournames.txt
--rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-06 14:56:00.000000 cf-plot-3.2.6/cfplot/colourmaps/cosam.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:55:20.000000 cf-plot-3.2.6/cfplot/colourmaps/cosam12.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      589 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/default.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2709 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/detail.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2810 2014-03-11 11:51:02.000000 cf-plot-3.2.6/cfplot/colourmaps/extrema.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1371 2015-10-16 10:27:40.000000 cf-plot-3.2.6/cfplot/colourmaps/gray.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      270 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/gui_default.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2315 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/helix.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2228 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/helix1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      589 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/hlu_default.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      247 2013-08-06 14:55:14.000000 cf-plot-3.2.6/cfplot/colourmaps/hotcold_18lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-06 14:55:04.000000 cf-plot-3.2.6/cfplot/colourmaps/hotcolr_19lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2350 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/hotres.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:06.000000 cf-plot-3.2.6/cfplot/colourmaps/idl0.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:14.000000 cf-plot-3.2.6/cfplot/colourmaps/idl1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:10.000000 cf-plot-3.2.6/cfplot/colourmaps/idl10.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:16.000000 cf-plot-3.2.6/cfplot/colourmaps/idl11.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:22.000000 cf-plot-3.2.6/cfplot/colourmaps/idl12.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:32.000000 cf-plot-3.2.6/cfplot/colourmaps/idl13.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:38.000000 cf-plot-3.2.6/cfplot/colourmaps/idl14.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:44.000000 cf-plot-3.2.6/cfplot/colourmaps/idl15.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:48.000000 cf-plot-3.2.6/cfplot/colourmaps/idl16.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:54.000000 cf-plot-3.2.6/cfplot/colourmaps/idl17.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:59:00.000000 cf-plot-3.2.6/cfplot/colourmaps/idl18.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:04.000000 cf-plot-3.2.6/cfplot/colourmaps/idl19.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:20.000000 cf-plot-3.2.6/cfplot/colourmaps/idl2.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:10.000000 cf-plot-3.2.6/cfplot/colourmaps/idl20.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:16.000000 cf-plot-3.2.6/cfplot/colourmaps/idl21.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:22.000000 cf-plot-3.2.6/cfplot/colourmaps/idl22.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:26.000000 cf-plot-3.2.6/cfplot/colourmaps/idl23.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:32.000000 cf-plot-3.2.6/cfplot/colourmaps/idl24.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:38.000000 cf-plot-3.2.6/cfplot/colourmaps/idl25.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:42.000000 cf-plot-3.2.6/cfplot/colourmaps/idl26.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:50.000000 cf-plot-3.2.6/cfplot/colourmaps/idl27.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:54.000000 cf-plot-3.2.6/cfplot/colourmaps/idl28.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:00.000000 cf-plot-3.2.6/cfplot/colourmaps/idl29.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:26.000000 cf-plot-3.2.6/cfplot/colourmaps/idl3.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:14.000000 cf-plot-3.2.6/cfplot/colourmaps/idl30.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:20.000000 cf-plot-3.2.6/cfplot/colourmaps/idl31.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:24.000000 cf-plot-3.2.6/cfplot/colourmaps/idl32.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:34.000000 cf-plot-3.2.6/cfplot/colourmaps/idl33.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:38.000000 cf-plot-3.2.6/cfplot/colourmaps/idl34.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:44.000000 cf-plot-3.2.6/cfplot/colourmaps/idl35.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:50.000000 cf-plot-3.2.6/cfplot/colourmaps/idl36.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:56.000000 cf-plot-3.2.6/cfplot/colourmaps/idl37.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:05:04.000000 cf-plot-3.2.6/cfplot/colourmaps/idl38.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:05:10.000000 cf-plot-3.2.6/cfplot/colourmaps/idl39.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:30.000000 cf-plot-3.2.6/cfplot/colourmaps/idl4.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:38.000000 cf-plot-3.2.6/cfplot/colourmaps/idl5.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:44.000000 cf-plot-3.2.6/cfplot/colourmaps/idl6.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:50.000000 cf-plot-3.2.6/cfplot/colourmaps/idl7.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:56.000000 cf-plot-3.2.6/cfplot/colourmaps/idl8.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:02.000000 cf-plot-3.2.6/cfplot/colourmaps/idl9.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2588 2015-10-20 15:11:08.000000 cf-plot-3.2.6/cfplot/colourmaps/inferno.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2700 2015-10-16 09:51:04.000000 cf-plot-3.2.6/cfplot/colourmaps/magma.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      768 2013-08-06 14:54:38.000000 cf-plot-3.2.6/cfplot/colourmaps/matlab_hot.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      768 2013-08-06 14:54:20.000000 cf-plot-3.2.6/cfplot/colourmaps/matlab_hsv.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      768 2013-08-06 14:54:12.000000 cf-plot-3.2.6/cfplot/colourmaps/matlab_jet.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      768 2013-08-06 14:54:06.000000 cf-plot-3.2.6/cfplot/colourmaps/matlab_lines.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-08-06 14:53:56.000000 cf-plot-3.2.6/cfplot/colourmaps/mch_default.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3810 2013-09-12 13:37:56.000000 cf-plot-3.2.6/cfplot/colourmaps/ncl_default.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2544 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/ncview_default.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      252 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/nrl_sirkes.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      228 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/nrl_sirkes_nowhite.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      133 2016-01-11 10:38:42.000000 cf-plot-3.2.6/cfplot/colourmaps/nrwc.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      168 2016-01-11 15:30:18.000000 cf-plot-3.2.6/cfplot/colourmaps/os250kmetres.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2723 2015-10-16 11:07:50.000000 cf-plot-3.2.6/cfplot/colourmaps/parula.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-06 14:53:20.000000 cf-plot-3.2.6/cfplot/colourmaps/perc2_9lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:53:10.000000 cf-plot-3.2.6/cfplot/colourmaps/percent_11lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2693 2015-10-20 15:11:20.000000 cf-plot-3.2.6/cfplot/colourmaps/plasma.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-06 14:53:00.000000 cf-plot-3.2.6/cfplot/colourmaps/posneg_1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      229 2013-08-06 14:52:50.000000 cf-plot-3.2.6/cfplot/colourmaps/posneg_2.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      221 2013-08-06 14:51:46.000000 cf-plot-3.2.6/cfplot/colourmaps/prcp_1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:51:38.000000 cf-plot-3.2.6/cfplot/colourmaps/prcp_2.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      284 2013-08-06 14:51:28.000000 cf-plot-3.2.6/cfplot/colourmaps/prcp_3.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-06 14:52:42.000000 cf-plot-3.2.6/cfplot/colourmaps/precip2_15lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-06 14:52:32.000000 cf-plot-3.2.6/cfplot/colourmaps/precip2_17lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      221 2013-08-06 14:52:22.000000 cf-plot-3.2.6/cfplot/colourmaps/precip3_16lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:53:46.000000 cf-plot-3.2.6/cfplot/colourmaps/precip4_11lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-06 14:53:36.000000 cf-plot-3.2.6/cfplot/colourmaps/precip4_diff_19lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:52:10.000000 cf-plot-3.2.6/cfplot/colourmaps/precip_11lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      169 2013-08-06 14:50:54.000000 cf-plot-3.2.6/cfplot/colourmaps/precip_diff_12lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)       26 2013-08-06 14:50:38.000000 cf-plot-3.2.6/cfplot/colourmaps/precip_diff_1lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      423 2013-08-06 14:51:18.000000 cf-plot-3.2.6/cfplot/colourmaps/radar.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      312 2013-08-06 14:45:04.000000 cf-plot-3.2.6/cfplot/colourmaps/radar_1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2444 2013-08-06 14:48:50.000000 cf-plot-3.2.6/cfplot/colourmaps/rainbow.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3081 2013-08-06 14:50:22.000000 cf-plot-3.2.6/cfplot/colourmaps/rainbow_gray.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3081 2013-08-06 14:49:28.000000 cf-plot-3.2.6/cfplot/colourmaps/rainbow_white.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     3094 2013-08-06 14:49:54.000000 cf-plot-3.2.6/cfplot/colourmaps/rainbow_white_gray.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-06 14:47:42.000000 cf-plot-3.2.6/cfplot/colourmaps/rh_19lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-06 16:42:42.000000 cf-plot-3.2.6/cfplot/colourmaps/scale1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-07 11:11:52.000000 cf-plot-3.2.6/cfplot/colourmaps/scale10.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:12:22.000000 cf-plot-3.2.6/cfplot/colourmaps/scale11.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-07 11:13:32.000000 cf-plot-3.2.6/cfplot/colourmaps/scale12.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:14:00.000000 cf-plot-3.2.6/cfplot/colourmaps/scale13.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-07 11:14:34.000000 cf-plot-3.2.6/cfplot/colourmaps/scale14.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      182 2013-08-07 11:15:04.000000 cf-plot-3.2.6/cfplot/colourmaps/scale15.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-07 11:15:36.000000 cf-plot-3.2.6/cfplot/colourmaps/scale16.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:16:06.000000 cf-plot-3.2.6/cfplot/colourmaps/scale17.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:16:38.000000 cf-plot-3.2.6/cfplot/colourmaps/scale18.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:17:10.000000 cf-plot-3.2.6/cfplot/colourmaps/scale19.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-07 11:06:16.000000 cf-plot-3.2.6/cfplot/colourmaps/scale2.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-07 11:17:42.000000 cf-plot-3.2.6/cfplot/colourmaps/scale20.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:18:12.000000 cf-plot-3.2.6/cfplot/colourmaps/scale21.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      182 2013-08-07 11:18:40.000000 cf-plot-3.2.6/cfplot/colourmaps/scale22.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      143 2013-08-07 11:19:10.000000 cf-plot-3.2.6/cfplot/colourmaps/scale23.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-07 11:19:40.000000 cf-plot-3.2.6/cfplot/colourmaps/scale24.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)       91 2013-08-07 11:20:08.000000 cf-plot-3.2.6/cfplot/colourmaps/scale25.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      364 2013-08-07 11:20:42.000000 cf-plot-3.2.6/cfplot/colourmaps/scale26.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      455 2013-08-07 11:21:22.000000 cf-plot-3.2.6/cfplot/colourmaps/scale27.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      117 2013-08-07 11:21:54.000000 cf-plot-3.2.6/cfplot/colourmaps/scale28.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-08-07 11:22:22.000000 cf-plot-3.2.6/cfplot/colourmaps/scale29.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-08-07 11:06:44.000000 cf-plot-3.2.6/cfplot/colourmaps/scale3.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      299 2013-08-07 11:22:56.000000 cf-plot-3.2.6/cfplot/colourmaps/scale30.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      252 2013-08-07 11:23:18.000000 cf-plot-3.2.6/cfplot/colourmaps/scale31.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      169 2013-08-07 11:23:28.000000 cf-plot-3.2.6/cfplot/colourmaps/scale32.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:23:36.000000 cf-plot-3.2.6/cfplot/colourmaps/scale33.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      221 2013-08-07 11:23:42.000000 cf-plot-3.2.6/cfplot/colourmaps/scale34.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      183 2013-08-07 11:23:46.000000 cf-plot-3.2.6/cfplot/colourmaps/scale35.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-08-07 11:23:52.000000 cf-plot-3.2.6/cfplot/colourmaps/scale36.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      245 2013-08-07 11:24:16.000000 cf-plot-3.2.6/cfplot/colourmaps/scale37.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      286 2013-08-07 11:24:34.000000 cf-plot-3.2.6/cfplot/colourmaps/scale38.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      311 2013-08-07 11:25:20.000000 cf-plot-3.2.6/cfplot/colourmaps/scale39.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:07:22.000000 cf-plot-3.2.6/cfplot/colourmaps/scale4.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      252 2013-08-07 11:25:42.000000 cf-plot-3.2.6/cfplot/colourmaps/scale40.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-07 11:26:00.000000 cf-plot-3.2.6/cfplot/colourmaps/scale41.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      209 2013-08-07 11:26:10.000000 cf-plot-3.2.6/cfplot/colourmaps/scale42.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:26:20.000000 cf-plot-3.2.6/cfplot/colourmaps/scale43.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      276 2013-08-07 11:26:30.000000 cf-plot-3.2.6/cfplot/colourmaps/scale44.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:08:00.000000 cf-plot-3.2.6/cfplot/colourmaps/scale5.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)       39 2013-08-07 11:08:46.000000 cf-plot-3.2.6/cfplot/colourmaps/scale6.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:10:16.000000 cf-plot-3.2.6/cfplot/colourmaps/scale7.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:10:54.000000 cf-plot-3.2.6/cfplot/colourmaps/scale8.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)       39 2013-08-07 11:11:24.000000 cf-plot-3.2.6/cfplot/colourmaps/scale9.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      217 2013-08-06 14:44:56.000000 cf-plot-3.2.6/cfplot/colourmaps/seaice_1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      168 2013-08-06 14:47:08.000000 cf-plot-3.2.6/cfplot/colourmaps/seaice_2.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      273 2013-08-06 14:45:54.000000 cf-plot-3.2.6/cfplot/colourmaps/so4_21.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      299 2013-08-06 14:46:06.000000 cf-plot-3.2.6/cfplot/colourmaps/so4_23.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-06 14:48:20.000000 cf-plot-3.2.6/cfplot/colourmaps/spread_15lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-06 14:47:16.000000 cf-plot-3.2.6/cfplot/colourmaps/sunshine_9lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      169 2013-08-06 14:47:34.000000 cf-plot-3.2.6/cfplot/colourmaps/sunshine_diff_12lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      390 2013-08-06 14:46:38.000000 cf-plot-3.2.6/cfplot/colourmaps/t2m_29lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:46:50.000000 cf-plot-3.2.6/cfplot/colourmaps/tbrAvg1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:46:26.000000 cf-plot-3.2.6/cfplot/colourmaps/tbrStd1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:45:42.000000 cf-plot-3.2.6/cfplot/colourmaps/tbrVar1.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:46:18.000000 cf-plot-3.2.6/cfplot/colourmaps/tbr_240_300.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:45:32.000000 cf-plot-3.2.6/cfplot/colourmaps/tbr_stdev_0_30.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:44:46.000000 cf-plot-3.2.6/cfplot/colourmaps/tbr_var_0_500.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-06 14:45:22.000000 cf-plot-3.2.6/cfplot/colourmaps/temp_19lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      247 2013-08-06 14:44:32.000000 cf-plot-3.2.6/cfplot/colourmaps/temp_diff_18lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)       26 2013-08-06 14:43:58.000000 cf-plot-3.2.6/cfplot/colourmaps/temp_diff_1lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1993 2012-08-01 16:32:20.000000 cf-plot-3.2.6/cfplot/colourmaps/testcmap.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2303 2014-03-11 11:54:08.000000 cf-plot-3.2.6/cfplot/colourmaps/thelix.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-06 14:43:42.000000 cf-plot-3.2.6/cfplot/colourmaps/topo_15lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     5851 2013-08-28 16:15:22.000000 cf-plot-3.2.6/cfplot/colourmaps/vcs.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2711 2015-10-16 09:05:58.000000 cf-plot-3.2.6/cfplot/colourmaps/viridis.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      169 2013-08-06 14:44:20.000000 cf-plot-3.2.6/cfplot/colourmaps/wgne15.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     2587 2013-08-06 14:43:24.000000 cf-plot-3.2.6/cfplot/colourmaps/wh_bl_gr_ye_re.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      480 2016-01-11 15:30:29.000000 cf-plot-3.2.6/cfplot/colourmaps/wiki_1_0_2.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      672 2016-01-11 15:30:34.000000 cf-plot-3.2.6/cfplot/colourmaps/wiki_1_0_3.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      696 2016-01-11 15:30:46.000000 cf-plot-3.2.6/cfplot/colourmaps/wiki_2_0.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      372 2016-01-11 15:30:45.000000 cf-plot-3.2.6/cfplot/colourmaps/wiki_2_0_reduced.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-06 14:43:06.000000 cf-plot-3.2.6/cfplot/colourmaps/wind_17lev.rgb
--rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:42:42.000000 cf-plot-3.2.6/cfplot/colourmaps/wxpEnIR.rgb
--rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-03-30 14:33:58.071957 cf-plot-3.2.6/setup.cfg
--rw-r--r--   0 andy      (1000) andy      (1000)     1183 2023-03-30 14:30:33.000000 cf-plot-3.2.6/setup.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-30 16:15:44.629943 cf-plot-3.2.7/
+-rw-r--r--   0 andy      (1000) andy      (1000)     1065 2016-01-26 13:42:08.000000 cf-plot-3.2.7/LICENSE.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)      123 2015-11-27 16:55:33.000000 cf-plot-3.2.7/MANIFEST.in
+-rw-rw-r--   0 andy      (1000) andy      (1000)      569 2023-03-30 16:15:44.629943 cf-plot-3.2.7/PKG-INFO
+-rw-r--r--   0 andy      (1000) andy      (1000)      251 2016-02-04 11:30:15.000000 cf-plot-3.2.7/README.md
+-rw-r--r--   0 andy      (1000) andy      (1000)      253 2019-05-13 16:06:32.000000 cf-plot-3.2.7/README.txt
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-30 16:15:44.609943 cf-plot-3.2.7/cf_plot.egg-info/
+-rw-rw-r--   0 andy      (1000) andy      (1000)      569 2023-03-30 16:15:44.000000 cf-plot-3.2.7/cf_plot.egg-info/PKG-INFO
+-rw-rw-r--   0 andy      (1000) andy      (1000)     6757 2023-03-30 16:15:44.000000 cf-plot-3.2.7/cf_plot.egg-info/SOURCES.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)        1 2023-03-30 16:15:44.000000 cf-plot-3.2.7/cf_plot.egg-info/dependency_links.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)       64 2023-03-30 16:15:44.000000 cf-plot-3.2.7/cf_plot.egg-info/requires.txt
+-rw-rw-r--   0 andy      (1000) andy      (1000)        7 2023-03-30 16:15:44.000000 cf-plot-3.2.7/cf_plot.egg-info/top_level.txt
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-30 16:15:44.609943 cf-plot-3.2.7/cfplot/
+-rw-r--r--   0 andy      (1000) andy      (1000)      368 2023-03-30 16:11:58.000000 cf-plot-3.2.7/cfplot/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)   355039 2023-03-30 16:12:21.000000 cf-plot-3.2.7/cfplot/cfplot.py
+drwxrwxr-x   0 andy      (1000) andy      (1000)        0 2023-03-30 16:15:44.629943 cf-plot-3.2.7/cfplot/colourmaps/
+-rw-r--r--   0 andy      (1000) andy      (1000)     2708 2013-08-06 14:42:16.000000 cf-plot-3.2.7/cfplot/colourmaps/3gauss.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2746 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/3saw.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:57:38.000000 cf-plot-3.2.7/cfplot/colourmaps/BkBlAqGrYeOrReViWh200.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:57:48.000000 cf-plot-3.2.7/cfplot/colourmaps/BlAqGrYeOrRe.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:59:26.000000 cf-plot-3.2.7/cfplot/colourmaps/BlAqGrYeOrReVi200.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:59:34.000000 cf-plot-3.2.7/cfplot/colourmaps/BlGrYeOrReVi200.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1248 2013-08-06 14:59:56.000000 cf-plot-3.2.7/cfplot/colourmaps/BlRe.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:59:42.000000 cf-plot-3.2.7/cfplot/colourmaps/BlWhRe.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      414 2013-08-06 15:00:06.000000 cf-plot-3.2.7/cfplot/colourmaps/BlueDarkOrange18.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      414 2013-08-06 15:00:18.000000 cf-plot-3.2.7/cfplot/colourmaps/BlueDarkRed18.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      322 2013-08-06 15:00:28.000000 cf-plot-3.2.7/cfplot/colourmaps/BlueGreen14.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     4991 2013-08-06 14:59:48.000000 cf-plot-3.2.7/cfplot/colourmaps/BlueRed.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5010 2013-08-06 14:57:56.000000 cf-plot-3.2.7/cfplot/colourmaps/BlueRedGray.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5129 2013-08-06 15:00:38.000000 cf-plot-3.2.7/cfplot/colourmaps/BlueWhiteOrangeRed.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5272 2013-08-06 15:00:46.000000 cf-plot-3.2.7/cfplot/colourmaps/BlueYellowRed.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1390 2017-01-23 17:36:40.000000 cf-plot-3.2.7/cfplot/colourmaps/BrBG.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      276 2013-08-06 14:59:18.000000 cf-plot-3.2.7/cfplot/colourmaps/BrownBlue12.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      276 2013-08-06 15:01:00.000000 cf-plot-3.2.7/cfplot/colourmaps/Cat12.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1554 2013-08-06 15:01:08.000000 cf-plot-3.2.7/cfplot/colourmaps/GHRSST_anomaly.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5098 2013-08-06 14:59:08.000000 cf-plot-3.2.7/cfplot/colourmaps/GrayWhiteGray.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      368 2013-08-06 14:59:00.000000 cf-plot-3.2.7/cfplot/colourmaps/GreenMagenta16.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     4976 2013-08-06 14:58:02.000000 cf-plot-3.2.7/cfplot/colourmaps/GreenYellow.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5213 2013-08-06 14:58:40.000000 cf-plot-3.2.7/cfplot/colourmaps/OceanLakeLandSnow.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      525 2013-08-06 14:58:28.000000 cf-plot-3.2.7/cfplot/colourmaps/StepSeq25.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:42:30.000000 cf-plot-3.2.7/cfplot/colourmaps/ViBlGrWhYeOrRe.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:58:14.000000 cf-plot-3.2.7/cfplot/colourmaps/WhBlGrYeRe.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:57:28.000000 cf-plot-3.2.7/cfplot/colourmaps/WhBlReWh.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:57:00.000000 cf-plot-3.2.7/cfplot/colourmaps/WhViBlGrYeOrRe.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:56:48.000000 cf-plot-3.2.7/cfplot/colourmaps/WhViBlGrYeOrReWh.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5104 2013-08-06 14:56:38.000000 cf-plot-3.2.7/cfplot/colourmaps/WhiteBlue.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5126 2013-08-06 14:56:30.000000 cf-plot-3.2.7/cfplot/colourmaps/WhiteBlueGreenYellowRed.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5100 2013-08-06 14:56:16.000000 cf-plot-3.2.7/cfplot/colourmaps/WhiteGreen.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5105 2013-08-06 14:55:48.000000 cf-plot-3.2.7/cfplot/colourmaps/WhiteYellowOrangeRed.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)        0 2015-11-27 13:32:06.000000 cf-plot-3.2.7/cfplot/colourmaps/__init__.py
+-rw-r--r--   0 andy      (1000) andy      (1000)      183 2013-08-06 14:56:08.000000 cf-plot-3.2.7/cfplot/colourmaps/amwg.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     4064 2013-09-12 13:37:22.000000 cf-plot-3.2.7/cfplot/colourmaps/amwg256.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-09-12 13:37:46.000000 cf-plot-3.2.7/cfplot/colourmaps/amwg_blueyellowred.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1415 2016-01-11 15:29:50.000000 cf-plot-3.2.7/cfplot/colourmaps/arctic.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      715 2013-08-06 14:55:40.000000 cf-plot-3.2.7/cfplot/colourmaps/cmp_b2r.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      238 2013-08-06 14:55:30.000000 cf-plot-3.2.7/cfplot/colourmaps/cmp_flux.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      733 2013-08-06 14:42:04.000000 cf-plot-3.2.7/cfplot/colourmaps/cmp_haxby.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      337 2016-01-11 10:38:42.000000 cf-plot-3.2.7/cfplot/colourmaps/colombia.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)    14626 2013-08-06 14:10:26.000000 cf-plot-3.2.7/cfplot/colourmaps/colournames.txt
+-rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-06 14:56:00.000000 cf-plot-3.2.7/cfplot/colourmaps/cosam.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:55:20.000000 cf-plot-3.2.7/cfplot/colourmaps/cosam12.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      589 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/default.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2709 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/detail.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2810 2014-03-11 11:51:02.000000 cf-plot-3.2.7/cfplot/colourmaps/extrema.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1371 2015-10-16 10:27:40.000000 cf-plot-3.2.7/cfplot/colourmaps/gray.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      270 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/gui_default.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2315 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/helix.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2228 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/helix1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      589 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/hlu_default.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      247 2013-08-06 14:55:14.000000 cf-plot-3.2.7/cfplot/colourmaps/hotcold_18lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-06 14:55:04.000000 cf-plot-3.2.7/cfplot/colourmaps/hotcolr_19lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2350 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/hotres.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:06.000000 cf-plot-3.2.7/cfplot/colourmaps/idl0.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:14.000000 cf-plot-3.2.7/cfplot/colourmaps/idl1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:10.000000 cf-plot-3.2.7/cfplot/colourmaps/idl10.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:16.000000 cf-plot-3.2.7/cfplot/colourmaps/idl11.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:22.000000 cf-plot-3.2.7/cfplot/colourmaps/idl12.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:32.000000 cf-plot-3.2.7/cfplot/colourmaps/idl13.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:38.000000 cf-plot-3.2.7/cfplot/colourmaps/idl14.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:44.000000 cf-plot-3.2.7/cfplot/colourmaps/idl15.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:48.000000 cf-plot-3.2.7/cfplot/colourmaps/idl16.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:54.000000 cf-plot-3.2.7/cfplot/colourmaps/idl17.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:59:00.000000 cf-plot-3.2.7/cfplot/colourmaps/idl18.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:04.000000 cf-plot-3.2.7/cfplot/colourmaps/idl19.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:20.000000 cf-plot-3.2.7/cfplot/colourmaps/idl2.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:10.000000 cf-plot-3.2.7/cfplot/colourmaps/idl20.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:16.000000 cf-plot-3.2.7/cfplot/colourmaps/idl21.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:22.000000 cf-plot-3.2.7/cfplot/colourmaps/idl22.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:26.000000 cf-plot-3.2.7/cfplot/colourmaps/idl23.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:32.000000 cf-plot-3.2.7/cfplot/colourmaps/idl24.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:38.000000 cf-plot-3.2.7/cfplot/colourmaps/idl25.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:42.000000 cf-plot-3.2.7/cfplot/colourmaps/idl26.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:50.000000 cf-plot-3.2.7/cfplot/colourmaps/idl27.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:03:54.000000 cf-plot-3.2.7/cfplot/colourmaps/idl28.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:00.000000 cf-plot-3.2.7/cfplot/colourmaps/idl29.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:26.000000 cf-plot-3.2.7/cfplot/colourmaps/idl3.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:14.000000 cf-plot-3.2.7/cfplot/colourmaps/idl30.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:20.000000 cf-plot-3.2.7/cfplot/colourmaps/idl31.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:24.000000 cf-plot-3.2.7/cfplot/colourmaps/idl32.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:34.000000 cf-plot-3.2.7/cfplot/colourmaps/idl33.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:38.000000 cf-plot-3.2.7/cfplot/colourmaps/idl34.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:44.000000 cf-plot-3.2.7/cfplot/colourmaps/idl35.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:50.000000 cf-plot-3.2.7/cfplot/colourmaps/idl36.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:04:56.000000 cf-plot-3.2.7/cfplot/colourmaps/idl37.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:05:04.000000 cf-plot-3.2.7/cfplot/colourmaps/idl38.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 15:05:10.000000 cf-plot-3.2.7/cfplot/colourmaps/idl39.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:30.000000 cf-plot-3.2.7/cfplot/colourmaps/idl4.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:38.000000 cf-plot-3.2.7/cfplot/colourmaps/idl5.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:44.000000 cf-plot-3.2.7/cfplot/colourmaps/idl6.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:50.000000 cf-plot-3.2.7/cfplot/colourmaps/idl7.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:57:56.000000 cf-plot-3.2.7/cfplot/colourmaps/idl8.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3302 2013-08-07 14:58:02.000000 cf-plot-3.2.7/cfplot/colourmaps/idl9.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2588 2015-10-20 15:11:08.000000 cf-plot-3.2.7/cfplot/colourmaps/inferno.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2700 2015-10-16 09:51:04.000000 cf-plot-3.2.7/cfplot/colourmaps/magma.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      768 2013-08-06 14:54:38.000000 cf-plot-3.2.7/cfplot/colourmaps/matlab_hot.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      768 2013-08-06 14:54:20.000000 cf-plot-3.2.7/cfplot/colourmaps/matlab_hsv.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      768 2013-08-06 14:54:12.000000 cf-plot-3.2.7/cfplot/colourmaps/matlab_jet.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      768 2013-08-06 14:54:06.000000 cf-plot-3.2.7/cfplot/colourmaps/matlab_lines.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-08-06 14:53:56.000000 cf-plot-3.2.7/cfplot/colourmaps/mch_default.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3810 2013-09-12 13:37:56.000000 cf-plot-3.2.7/cfplot/colourmaps/ncl_default.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2544 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/ncview_default.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      252 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/nrl_sirkes.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      228 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/nrl_sirkes_nowhite.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      133 2016-01-11 10:38:42.000000 cf-plot-3.2.7/cfplot/colourmaps/nrwc.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      168 2016-01-11 15:30:18.000000 cf-plot-3.2.7/cfplot/colourmaps/os250kmetres.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2723 2015-10-16 11:07:50.000000 cf-plot-3.2.7/cfplot/colourmaps/parula.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-06 14:53:20.000000 cf-plot-3.2.7/cfplot/colourmaps/perc2_9lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:53:10.000000 cf-plot-3.2.7/cfplot/colourmaps/percent_11lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2693 2015-10-20 15:11:20.000000 cf-plot-3.2.7/cfplot/colourmaps/plasma.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-06 14:53:00.000000 cf-plot-3.2.7/cfplot/colourmaps/posneg_1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      229 2013-08-06 14:52:50.000000 cf-plot-3.2.7/cfplot/colourmaps/posneg_2.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      221 2013-08-06 14:51:46.000000 cf-plot-3.2.7/cfplot/colourmaps/prcp_1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:51:38.000000 cf-plot-3.2.7/cfplot/colourmaps/prcp_2.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      284 2013-08-06 14:51:28.000000 cf-plot-3.2.7/cfplot/colourmaps/prcp_3.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-06 14:52:42.000000 cf-plot-3.2.7/cfplot/colourmaps/precip2_15lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-06 14:52:32.000000 cf-plot-3.2.7/cfplot/colourmaps/precip2_17lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      221 2013-08-06 14:52:22.000000 cf-plot-3.2.7/cfplot/colourmaps/precip3_16lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:53:46.000000 cf-plot-3.2.7/cfplot/colourmaps/precip4_11lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-06 14:53:36.000000 cf-plot-3.2.7/cfplot/colourmaps/precip4_diff_19lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-06 14:52:10.000000 cf-plot-3.2.7/cfplot/colourmaps/precip_11lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      169 2013-08-06 14:50:54.000000 cf-plot-3.2.7/cfplot/colourmaps/precip_diff_12lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)       26 2013-08-06 14:50:38.000000 cf-plot-3.2.7/cfplot/colourmaps/precip_diff_1lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      423 2013-08-06 14:51:18.000000 cf-plot-3.2.7/cfplot/colourmaps/radar.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      312 2013-08-06 14:45:04.000000 cf-plot-3.2.7/cfplot/colourmaps/radar_1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2444 2013-08-06 14:48:50.000000 cf-plot-3.2.7/cfplot/colourmaps/rainbow.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3081 2013-08-06 14:50:22.000000 cf-plot-3.2.7/cfplot/colourmaps/rainbow_gray.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3081 2013-08-06 14:49:28.000000 cf-plot-3.2.7/cfplot/colourmaps/rainbow_white.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     3094 2013-08-06 14:49:54.000000 cf-plot-3.2.7/cfplot/colourmaps/rainbow_white_gray.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-06 14:47:42.000000 cf-plot-3.2.7/cfplot/colourmaps/rh_19lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-06 16:42:42.000000 cf-plot-3.2.7/cfplot/colourmaps/scale1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-07 11:11:52.000000 cf-plot-3.2.7/cfplot/colourmaps/scale10.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:12:22.000000 cf-plot-3.2.7/cfplot/colourmaps/scale11.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-07 11:13:32.000000 cf-plot-3.2.7/cfplot/colourmaps/scale12.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:14:00.000000 cf-plot-3.2.7/cfplot/colourmaps/scale13.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-07 11:14:34.000000 cf-plot-3.2.7/cfplot/colourmaps/scale14.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      182 2013-08-07 11:15:04.000000 cf-plot-3.2.7/cfplot/colourmaps/scale15.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-07 11:15:36.000000 cf-plot-3.2.7/cfplot/colourmaps/scale16.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:16:06.000000 cf-plot-3.2.7/cfplot/colourmaps/scale17.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:16:38.000000 cf-plot-3.2.7/cfplot/colourmaps/scale18.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:17:10.000000 cf-plot-3.2.7/cfplot/colourmaps/scale19.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-07 11:06:16.000000 cf-plot-3.2.7/cfplot/colourmaps/scale2.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-07 11:17:42.000000 cf-plot-3.2.7/cfplot/colourmaps/scale20.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:18:12.000000 cf-plot-3.2.7/cfplot/colourmaps/scale21.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      182 2013-08-07 11:18:40.000000 cf-plot-3.2.7/cfplot/colourmaps/scale22.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      143 2013-08-07 11:19:10.000000 cf-plot-3.2.7/cfplot/colourmaps/scale23.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-07 11:19:40.000000 cf-plot-3.2.7/cfplot/colourmaps/scale24.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)       91 2013-08-07 11:20:08.000000 cf-plot-3.2.7/cfplot/colourmaps/scale25.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      364 2013-08-07 11:20:42.000000 cf-plot-3.2.7/cfplot/colourmaps/scale26.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      455 2013-08-07 11:21:22.000000 cf-plot-3.2.7/cfplot/colourmaps/scale27.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      117 2013-08-07 11:21:54.000000 cf-plot-3.2.7/cfplot/colourmaps/scale28.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-08-07 11:22:22.000000 cf-plot-3.2.7/cfplot/colourmaps/scale29.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-08-07 11:06:44.000000 cf-plot-3.2.7/cfplot/colourmaps/scale3.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      299 2013-08-07 11:22:56.000000 cf-plot-3.2.7/cfplot/colourmaps/scale30.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      252 2013-08-07 11:23:18.000000 cf-plot-3.2.7/cfplot/colourmaps/scale31.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      169 2013-08-07 11:23:28.000000 cf-plot-3.2.7/cfplot/colourmaps/scale32.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:23:36.000000 cf-plot-3.2.7/cfplot/colourmaps/scale33.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      221 2013-08-07 11:23:42.000000 cf-plot-3.2.7/cfplot/colourmaps/scale34.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      183 2013-08-07 11:23:46.000000 cf-plot-3.2.7/cfplot/colourmaps/scale35.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      195 2013-08-07 11:23:52.000000 cf-plot-3.2.7/cfplot/colourmaps/scale36.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      245 2013-08-07 11:24:16.000000 cf-plot-3.2.7/cfplot/colourmaps/scale37.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      286 2013-08-07 11:24:34.000000 cf-plot-3.2.7/cfplot/colourmaps/scale38.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      311 2013-08-07 11:25:20.000000 cf-plot-3.2.7/cfplot/colourmaps/scale39.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:07:22.000000 cf-plot-3.2.7/cfplot/colourmaps/scale4.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      252 2013-08-07 11:25:42.000000 cf-plot-3.2.7/cfplot/colourmaps/scale40.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-07 11:26:00.000000 cf-plot-3.2.7/cfplot/colourmaps/scale41.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      209 2013-08-07 11:26:10.000000 cf-plot-3.2.7/cfplot/colourmaps/scale42.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      156 2013-08-07 11:26:20.000000 cf-plot-3.2.7/cfplot/colourmaps/scale43.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      276 2013-08-07 11:26:30.000000 cf-plot-3.2.7/cfplot/colourmaps/scale44.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:08:00.000000 cf-plot-3.2.7/cfplot/colourmaps/scale5.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)       39 2013-08-07 11:08:46.000000 cf-plot-3.2.7/cfplot/colourmaps/scale6.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:10:16.000000 cf-plot-3.2.7/cfplot/colourmaps/scale7.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      104 2013-08-07 11:10:54.000000 cf-plot-3.2.7/cfplot/colourmaps/scale8.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)       39 2013-08-07 11:11:24.000000 cf-plot-3.2.7/cfplot/colourmaps/scale9.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      217 2013-08-06 14:44:56.000000 cf-plot-3.2.7/cfplot/colourmaps/seaice_1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      168 2013-08-06 14:47:08.000000 cf-plot-3.2.7/cfplot/colourmaps/seaice_2.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      273 2013-08-06 14:45:54.000000 cf-plot-3.2.7/cfplot/colourmaps/so4_21.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      299 2013-08-06 14:46:06.000000 cf-plot-3.2.7/cfplot/colourmaps/so4_23.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-06 14:48:20.000000 cf-plot-3.2.7/cfplot/colourmaps/spread_15lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      130 2013-08-06 14:47:16.000000 cf-plot-3.2.7/cfplot/colourmaps/sunshine_9lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      169 2013-08-06 14:47:34.000000 cf-plot-3.2.7/cfplot/colourmaps/sunshine_diff_12lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      390 2013-08-06 14:46:38.000000 cf-plot-3.2.7/cfplot/colourmaps/t2m_29lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:46:50.000000 cf-plot-3.2.7/cfplot/colourmaps/tbrAvg1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:46:26.000000 cf-plot-3.2.7/cfplot/colourmaps/tbrStd1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1313 2013-08-06 14:45:42.000000 cf-plot-3.2.7/cfplot/colourmaps/tbrVar1.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:46:18.000000 cf-plot-3.2.7/cfplot/colourmaps/tbr_240_300.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:45:32.000000 cf-plot-3.2.7/cfplot/colourmaps/tbr_stdev_0_30.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2600 2013-08-06 14:44:46.000000 cf-plot-3.2.7/cfplot/colourmaps/tbr_var_0_500.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      260 2013-08-06 14:45:22.000000 cf-plot-3.2.7/cfplot/colourmaps/temp_19lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      247 2013-08-06 14:44:32.000000 cf-plot-3.2.7/cfplot/colourmaps/temp_diff_18lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)       26 2013-08-06 14:43:58.000000 cf-plot-3.2.7/cfplot/colourmaps/temp_diff_1lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1993 2012-08-01 16:32:20.000000 cf-plot-3.2.7/cfplot/colourmaps/testcmap.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2303 2014-03-11 11:54:08.000000 cf-plot-3.2.7/cfplot/colourmaps/thelix.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      208 2013-08-06 14:43:42.000000 cf-plot-3.2.7/cfplot/colourmaps/topo_15lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     5851 2013-08-28 16:15:22.000000 cf-plot-3.2.7/cfplot/colourmaps/vcs.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2711 2015-10-16 09:05:58.000000 cf-plot-3.2.7/cfplot/colourmaps/viridis.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      169 2013-08-06 14:44:20.000000 cf-plot-3.2.7/cfplot/colourmaps/wgne15.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     2587 2013-08-06 14:43:24.000000 cf-plot-3.2.7/cfplot/colourmaps/wh_bl_gr_ye_re.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      480 2016-01-11 15:30:29.000000 cf-plot-3.2.7/cfplot/colourmaps/wiki_1_0_2.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      672 2016-01-11 15:30:34.000000 cf-plot-3.2.7/cfplot/colourmaps/wiki_1_0_3.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      696 2016-01-11 15:30:46.000000 cf-plot-3.2.7/cfplot/colourmaps/wiki_2_0.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      372 2016-01-11 15:30:45.000000 cf-plot-3.2.7/cfplot/colourmaps/wiki_2_0_reduced.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)      234 2013-08-06 14:43:06.000000 cf-plot-3.2.7/cfplot/colourmaps/wind_17lev.rgb
+-rw-r--r--   0 andy      (1000) andy      (1000)     1300 2013-08-06 14:42:42.000000 cf-plot-3.2.7/cfplot/colourmaps/wxpEnIR.rgb
+-rw-rw-r--   0 andy      (1000) andy      (1000)       38 2023-03-30 16:15:44.629943 cf-plot-3.2.7/setup.cfg
+-rw-r--r--   0 andy      (1000) andy      (1000)     1183 2023-03-30 16:11:42.000000 cf-plot-3.2.7/setup.py
```

### Comparing `cf-plot-3.2.6/LICENSE.txt` & `cf-plot-3.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/PKG-INFO` & `cf-plot-3.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-plot
-Version: 3.2.6
+Version: 3.2.7
 Summary: Climate contour, vector and line plots in Python
 Home-page: http://ajheaps.github.io/cf-plot
 Author: Andy Heaps
 Author-email: andy.heaps@ncas.ac.uk
 License: LICENSE.txt
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `cf-plot-3.2.6/cf_plot.egg-info/PKG-INFO` & `cf-plot-3.2.7/cf_plot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-plot
-Version: 3.2.6
+Version: 3.2.7
 Summary: Climate contour, vector and line plots in Python
 Home-page: http://ajheaps.github.io/cf-plot
 Author: Andy Heaps
 Author-email: andy.heaps@ncas.ac.uk
 License: LICENSE.txt
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `cf-plot-3.2.6/cf_plot.egg-info/SOURCES.txt` & `cf-plot-3.2.7/cf_plot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/cfplot.py` & `cf-plot-3.2.7/cfplot/cfplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -4529,15 +4529,16 @@
         # Cylindrical projection
         # Add cyclic information if missing.
         lonrange = np.nanmax(xpts) - np.nanmin(xpts)
         if lonrange < 360:
             # field, xpts = cartopy_util.add_cyclic_point(field, xpts)
             field, xpts = add_cyclic(field, xpts)
 
-        if plotvars.proj == 'cyl':
+        #if plotvars.proj == 'cyl':
+        if plotvars.proj in ['cyl', 'robin', 'merc', 'ortho', 'moll']:        
             # Calculate interpolation points
             xnew, ynew = stipple_points(xmin=np.nanmin(xpts),
                                         xmax=np.nanmax(xpts),
                                         ymin=np.nanmin(ypts),
                                         ymax=np.nanmax(ypts),
                                         pts=pts, stype=2)
 
@@ -8147,24 +8148,25 @@
 
         if plotvars.plot_type == 6 and (plotvars.proj == 'rotated' or plotvars.proj == 'UKCP'):
             this_plot = plotvars.plot     
 
         l, b, w, h = this_plot.get_position().bounds
 
         if orientation == 'horizontal':
-            if plotvars.plot_type > 1 or plotvars.plot == 0 or plotvars.proj != 'cyl':
+            if plotvars.plot_type > 1 or plotvars.plot == 0 or plotvars.proj not in ['cyl', 'lcc', 'moll', 'merc', 'ortho', 'robin']:
                 this_plot.set_position([l, b + fraction, w, h - fraction])
 
-            if plotvars.plot_type == 1 and plotvars.proj == 'cyl':
-
+            #if plotvars.plot_type == 1 and plotvars.proj == 'cyl':
+            if plotvars.plot_type == 1 and plotvars.proj in ['cyl', 'lcc', 'moll', 'merc', 'ortho', 'robin']:
                 # Move plot up if aspect ratio is < 1.5
                 lonrange = plotvars.lonmax - plotvars.lonmin
                 latrange = plotvars.latmax - plotvars.latmin
                 
                 if (lonrange / latrange) <= 1.5:
+                    print('moving plot up')
                     this_plot.set_position([l, b + 0.08, w, h - 0.12])
                     l, b, w, h = this_plot.get_position().bounds
 
                 ax1 = plotvars.master_plot.add_axes([l + w * (1.0 - shrink)/2.0,
                                                      b - fraction * (1.0 - anchor),
                                                      w * shrink,
                                                      thick])
@@ -8372,25 +8374,29 @@
     lon_0 = plotvars.lon_0
     lonmin = plotvars.lonmin
     lonmax = plotvars.lonmax
     latmin = plotvars.latmin
     latmax = plotvars.latmax
     polar_range = 90-abs(boundinglat)
 
-    if plotvars.proj == 'cyl':
+    myprojs = ['cyl', 'robin', 'moll', 'merc']
+    if plotvars.proj in myprojs:    
         lon_mid = lonmin + (lonmax - lonmin) / 2.0
         mylon = lon_mid
         if dims:
             mylon = lonmin
-        proj = ccrs.PlateCarree(central_longitude=lon_mid)
+        projs = [ccrs.PlateCarree, ccrs.Robinson, ccrs.Mollweide, ccrs.Mercator]
+        myind = myprojs.index(plotvars.proj)
+        #if plotvars.proj == 'cyl':
+        #    proj = ccrs.PlateCarree(central_longitude=lon_mid)
+        proj = projs[myind](central_longitude=lon_mid)
         mylat = latmax
         xpt, ypt = proj.transform_point(mylon, mylat, ccrs.PlateCarree())
-        ypt = ypt + (latmax - latmin) / 40.0
-
-
+        ypt = ypt + (latmax - latmin) / 40.0        
+        
     if plotvars.proj == 'npstere':
         mylon = lon_0 + 180
         mylat = boundinglat-polar_range/15.0
         proj = ccrs.NorthPolarStereo(central_longitude=lon_0)
         xpt, ypt = proj.transform_point(mylon, mylat, ccrs.PlateCarree())
         if dims:
             mylon = lon_0 + 180
@@ -8472,15 +8478,15 @@
     | title3=None - additional title     
     |
     |
     |
     |
     |
     """
-
+    
     # Logic for the supplied titles
     # if just title is supplied:
     #     title - contour or line title
     #
     # if both title and title2 are supplied:
     #     title u component of title
     #     title2 v component of the title
```

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/3gauss.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/3gauss.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/3saw.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/3saw.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BkBlAqGrYeOrReViWh200.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BkBlAqGrYeOrReViWh200.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BlAqGrYeOrRe.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BlAqGrYeOrRe.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BlAqGrYeOrReVi200.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BlAqGrYeOrReVi200.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BlGrYeOrReVi200.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BlGrYeOrReVi200.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BlRe.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BlRe.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BlWhRe.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BlWhRe.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BlueRed.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BlueRed.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BlueRedGray.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BlueRedGray.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BlueWhiteOrangeRed.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BlueWhiteOrangeRed.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BlueYellowRed.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BlueYellowRed.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/BrBG.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/BrBG.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/GHRSST_anomaly.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/GHRSST_anomaly.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/GrayWhiteGray.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/GrayWhiteGray.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/GreenYellow.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/GreenYellow.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/OceanLakeLandSnow.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/OceanLakeLandSnow.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/StepSeq25.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/StepSeq25.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/ViBlGrWhYeOrRe.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/ViBlGrWhYeOrRe.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/WhBlGrYeRe.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/WhBlGrYeRe.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/WhBlReWh.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/WhBlReWh.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/WhViBlGrYeOrRe.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/WhViBlGrYeOrRe.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/WhViBlGrYeOrReWh.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/WhViBlGrYeOrReWh.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/WhiteBlue.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/WhiteBlue.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/WhiteBlueGreenYellowRed.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/WhiteBlueGreenYellowRed.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/WhiteGreen.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/WhiteGreen.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/WhiteYellowOrangeRed.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/WhiteYellowOrangeRed.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/amwg256.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/amwg256.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/arctic.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/arctic.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/cmp_b2r.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/cmp_b2r.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/cmp_haxby.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/cmp_haxby.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/colournames.txt` & `cf-plot-3.2.7/cfplot/colourmaps/colournames.txt`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/default.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/default.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/detail.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/detail.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/extrema.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/extrema.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/gray.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/gray.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/helix.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/helix.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/helix1.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/helix1.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/hlu_default.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/hlu_default.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/hotres.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/hotres.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl0.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl0.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl1.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl1.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl10.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl10.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl11.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl11.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl12.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl12.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl13.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl13.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl14.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl14.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl15.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl15.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl16.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl16.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl17.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl17.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl18.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl18.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl19.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl19.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl2.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl2.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl20.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl20.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl21.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl21.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl22.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl22.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl23.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl23.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl24.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl24.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl25.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl25.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl26.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl26.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl27.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl27.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl28.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl28.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl29.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl29.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl3.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl3.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl30.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl30.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl31.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl31.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl32.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl32.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl33.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl33.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl34.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl34.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl35.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl35.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl36.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl36.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl37.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl37.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl38.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl38.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl39.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl39.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl4.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl4.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl5.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl5.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl6.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl6.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl7.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl7.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl8.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl8.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/idl9.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/idl9.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/inferno.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/inferno.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/magma.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/magma.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/matlab_hot.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/matlab_hot.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/matlab_hsv.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/matlab_hsv.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/matlab_jet.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/matlab_jet.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/matlab_lines.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/matlab_lines.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/ncl_default.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/ncl_default.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/ncview_default.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/ncview_default.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/parula.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/parula.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/plasma.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/plasma.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/rainbow.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/rainbow.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/rainbow_gray.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/rainbow_gray.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/rainbow_white.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/rainbow_white.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/rainbow_white_gray.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/rainbow_white_gray.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/tbrAvg1.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/tbrAvg1.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/tbrStd1.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/tbrStd1.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/tbrVar1.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/tbrVar1.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/tbr_240_300.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/tbr_240_300.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/tbr_stdev_0_30.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/tbr_stdev_0_30.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/tbr_var_0_500.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/tbr_var_0_500.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/testcmap.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/testcmap.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/thelix.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/thelix.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/vcs.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/vcs.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/viridis.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/viridis.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/wh_bl_gr_ye_re.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/wh_bl_gr_ye_re.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/wiki_1_0_3.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/wiki_1_0_3.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/wiki_2_0.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/wiki_2_0.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/cfplot/colourmaps/wxpEnIR.rgb` & `cf-plot-3.2.7/cfplot/colourmaps/wxpEnIR.rgb`

 * *Files identical despite different names*

### Comparing `cf-plot-3.2.6/setup.py` & `cf-plot-3.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 package_data = [f for f in find_package_data_files('cfplot/colourmaps')]
 
 
 setup(
     name = "cf-plot",
-    version = "3.2.6",
+    version = "3.2.7",
     author = "Andy Heaps",
     author_email = "andy.heaps@ncas.ac.uk",
     packages = ["cfplot"],
     package_dir = {"cfplot":"cfplot"},
     package_data = {"cfplot": package_data},
     include_package_data = True,
     install_requires = ["matplotlib >=3.1.0",
```

