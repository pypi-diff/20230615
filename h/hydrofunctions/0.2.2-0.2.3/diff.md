# Comparing `tmp/hydrofunctions-0.2.2.tar.gz` & `tmp/hydrofunctions-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrofunctions-0.2.2.tar", last modified: Mon Nov  8 03:43:36 2021, max compression
+gzip compressed data, was "hydrofunctions-0.2.3.tar", last modified: Mon Apr 18 23:41:49 2022, max compression
```

## Comparing `hydrofunctions-0.2.2.tar` & `hydrofunctions-0.2.3.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 03:43:36.000458 hydrofunctions-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6396 2021-11-08 03:43:36.000458 hydrofunctions-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5598 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 03:43:35.972458 hydrofunctions-0.2.2/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     8223 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/_static/HerringHydrograph.png
--rw-r--r--   0 runner    (1001) docker     (121)    40866 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/_static/HydroCloudTable.png
--rw-r--r--   0 runner    (1001) docker     (121)   134651 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/_static/draw_map.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     8720 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 03:43:35.976458 hydrofunctions-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6794 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 03:43:35.976458 hydrofunctions-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     8223 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/_static/HerringHydrograph.png
--rw-r--r--   0 runner    (1001) docker     (121)      351 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)    69337 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/_static/cycleplot_annual-week.png
--rw-r--r--   0 runner    (1001) docker     (121)    52918 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/_static/cycleplot_dirunal_compare-month.png
--rw-r--r--   0 runner    (1001) docker     (121)    54196 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/_static/cycleplot_diurnal_compare-month.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    11609 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/_static/flow_duration_linear.png
--rw-r--r--   0 runner    (1001) docker     (121)    13582 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/_static/flow_duration_logit.png
--rw-r--r--   0 runner    (1001) docker     (121)    15371 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/_static/hf-logo-sm.svg
--rw-r--r--   0 runner    (1001) docker     (121)    14579 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/_static/hf-logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11433 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8476 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6116 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/graphing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4576 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/hydrofunctions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      973 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3990 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5385 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6585 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 03:43:35.988458 hydrofunctions-0.2.2/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)    55952 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Comparing_Urban_and_Rural_Streams.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   136086 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/DailyMean_vs_Instant.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    41937 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Data_Catalog.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2377 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/DeadRun_Daily.parquet
--rw-r--r--   0 runner    (1001) docker     (121)    86854 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/DeadRun_Instant.parquet
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Draw_Map_Demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   261560 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Graphing.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    48733 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Hydrofunctions_Comparing_Stream_Environments.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   234728 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Hydrofunctions_Tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    53817 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Hydrofunctions_nested_watersheds.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   300020 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Hysteresis.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    32416 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/PG.parquet
--rw-r--r--   0 runner    (1001) docker     (121)    52284 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Peak_Discharge.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     5214 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Saving_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   135233 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Selecting_Sites.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    11910 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Site_File.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   136458 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/USGS_Statistics_Service.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    19747 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Urban_Rural.parquet
--rw-r--r--   0 runner    (1001) docker     (121)    21602 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/Writing_Valid_Requests_for_NWIS.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 03:43:35.992458 hydrofunctions-0.2.2/docs/notebooks/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     8223 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/_static/HerringHydrograph.png
--rw-r--r--   0 runner    (1001) docker     (121)    40866 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/_static/HydroCloudTable.png
--rw-r--r--   0 runner    (1001) docker     (121)    99126 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/_static/draw_map.jpg
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/create_df.parquet
--rw-r--r--   0 runner    (1001) docker     (121)    66934 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/graphing-1.parquet
--rw-r--r--   0 runner    (1001) docker     (121)  3674054 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/graphing-2.parquet
--rw-r--r--   0 runner    (1001) docker     (121)    30516 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/groundwater.parquet
--rw-r--r--   0 runner    (1001) docker     (121)     2538 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/herring_july.parquet
--rw-r--r--   0 runner    (1001) docker     (121)   188744 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/mult.parquet
--rw-r--r--   0 runner    (1001) docker     (121)     6589 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/parquet_example.parquet
--rw-r--r--   0 runner    (1001) docker     (121)     6589 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/parquet_example2.parquet
--rw-r--r--   0 runner    (1001) docker     (121)     3501 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/save_example.json.gz
--rw-r--r--   0 runner    (1001) docker     (121)     7764 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/save_example.parquet
--rw-r--r--   0 runner    (1001) docker     (121)   142197 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/view-example.parquet
--rw-r--r--   0 runner    (1001) docker     (121)    67436 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/viewing.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   537750 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/docs/notebooks/virginia.parquet
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 03:43:35.992458 hydrofunctions-0.2.2/hydrofunctions/
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16170 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/charts.py
--rw-r--r--   0 runner    (1001) docker     (121)     4021 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    29793 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/hydrofunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4829 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    14287 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/station.py
--rw-r--r--   0 runner    (1001) docker     (121)    24650 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/usgs_rdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     6272 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/validate.py
--rw-r--r--   0 runner    (1001) docker     (121)     4651 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/hydrofunctions/waterwatch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 03:43:35.992458 hydrofunctions-0.2.2/hydrofunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6396 2021-11-08 03:43:35.000000 hydrofunctions-0.2.2/hydrofunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2021-11-08 03:43:35.000000 hydrofunctions-0.2.2/hydrofunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-08 03:43:35.000000 hydrofunctions-0.2.2/hydrofunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-08 03:43:35.000000 hydrofunctions-0.2.2/hydrofunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-11-08 03:43:35.000000 hydrofunctions-0.2.2/hydrofunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-11-08 03:43:35.000000 hydrofunctions-0.2.2/hydrofunctions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5091 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/pypi_readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      478 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-08 03:43:36.000458 hydrofunctions-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-08 03:43:36.000458 hydrofunctions-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)   624836 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/Test Data Prep.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)    16839 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/fixtures_daily_dupe.py
--rw-r--r--   0 runner    (1001) docker     (121)   574431 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/fixtures_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    22907 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/fixtures_multiple_methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     9483 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/fixtures_recent_only.py
--rw-r--r--   0 runner    (1001) docker     (121)   543542 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/fixtures_tzfail.py
--rw-r--r--   0 runner    (1001) docker     (121)    14393 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/fixtures_usgs_rdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     8447 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_charts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    27066 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_hydrofunctions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_online_resources.py
--rw-r--r--   0 runner    (1001) docker     (121)    51305 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_station.py
--rw-r--r--   0 runner    (1001) docker     (121)    17340 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_usgs_rdb.py
--rw-r--r--   0 runner    (1001) docker     (121)     6329 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2021-11-08 03:43:26.000000 hydrofunctions-0.2.2/tests/test_waterwatch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.985617 hydrofunctions-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7119 2022-04-18 23:41:49.985617 hydrofunctions-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5717 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.957617 hydrofunctions-0.2.3/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     8223 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/_static/HerringHydrograph.png
+-rw-r--r--   0 runner    (1001) docker     (121)    40866 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/_static/HydroCloudTable.png
+-rw-r--r--   0 runner    (1001) docker     (121)   134651 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/_static/draw_map.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)     8720 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.961617 hydrofunctions-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     6794 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.961617 hydrofunctions-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     8223 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/_static/HerringHydrograph.png
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (121)    69337 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/_static/cycleplot_annual-week.png
+-rw-r--r--   0 runner    (1001) docker     (121)    52918 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/_static/cycleplot_dirunal_compare-month.png
+-rw-r--r--   0 runner    (1001) docker     (121)    54196 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/_static/cycleplot_diurnal_compare-month.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)    11609 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/_static/flow_duration_linear.png
+-rw-r--r--   0 runner    (1001) docker     (121)    13582 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/_static/flow_duration_logit.png
+-rw-r--r--   0 runner    (1001) docker     (121)    15371 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/_static/hf-logo-sm.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    14579 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/_static/hf-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11435 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8654 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6116 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/graphing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4879 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/hydrofunctions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5385 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6585 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.973617 hydrofunctions-0.2.3/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (121)    55952 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Comparing_Urban_and_Rural_Streams.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   136086 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/DailyMean_vs_Instant.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    41937 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Data_Catalog.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/DeadRun_Daily.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)    86854 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/DeadRun_Instant.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Draw_Map_Demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   261560 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Graphing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    48733 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Hydrofunctions_Comparing_Stream_Environments.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   234728 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Hydrofunctions_Tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    53817 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Hydrofunctions_nested_watersheds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   300020 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Hysteresis.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    32416 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/PG.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)    52284 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Peak_Discharge.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     5214 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Saving_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   135233 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Selecting_Sites.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    11910 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Site_File.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   136458 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/USGS_Statistics_Service.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)    19747 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Urban_Rural.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)    21602 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/Writing_Valid_Requests_for_NWIS.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.977617 hydrofunctions-0.2.3/docs/notebooks/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     8223 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/_static/HerringHydrograph.png
+-rw-r--r--   0 runner    (1001) docker     (121)    40866 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/_static/HydroCloudTable.png
+-rw-r--r--   0 runner    (1001) docker     (121)    99126 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/_static/draw_map.jpg
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/create_df.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)    66934 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/graphing-1.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)  3674054 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/graphing-2.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)    30516 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/groundwater.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)     2538 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/herring_july.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)   188744 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/mult.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)     6589 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/parquet_example.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)     6589 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/parquet_example2.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)     3501 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/save_example.json.gz
+-rw-r--r--   0 runner    (1001) docker     (121)     7764 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/save_example.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)   142197 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/view-example.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)    67436 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/viewing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)   537750 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/docs/notebooks/virginia.parquet
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1976 2022-04-18 23:41:49.985617 hydrofunctions-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.957617 hydrofunctions-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.977617 hydrofunctions-0.2.3/src/hydrofunctions/
+-rw-r--r--   0 runner    (1001) docker     (121)     3061 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16170 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/charts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29901 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/hydrofunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4829 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14446 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/station.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24645 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/usgs_rdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6272 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/validate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/src/hydrofunctions/waterwatch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.981617 hydrofunctions-0.2.3/src/hydrofunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7119 2022-04-18 23:41:49.000000 hydrofunctions-0.2.3/src/hydrofunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3074 2022-04-18 23:41:49.000000 hydrofunctions-0.2.3/src/hydrofunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-18 23:41:49.000000 hydrofunctions-0.2.3/src/hydrofunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-18 23:41:47.000000 hydrofunctions-0.2.3/src/hydrofunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-04-18 23:41:49.000000 hydrofunctions-0.2.3/src/hydrofunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-18 23:41:49.000000 hydrofunctions-0.2.3/src/hydrofunctions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-18 23:41:49.985617 hydrofunctions-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)   624836 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/Test Data Prep.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16839 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/fixtures_daily_dupe.py
+-rw-r--r--   0 runner    (1001) docker     (121)   574431 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/fixtures_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22907 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/fixtures_multiple_methods.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9483 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/fixtures_recent_only.py
+-rw-r--r--   0 runner    (1001) docker     (121)   543542 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/fixtures_tzfail.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14393 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/fixtures_usgs_rdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8447 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_charts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27066 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_hydrofunctions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_online_resources.py
+-rw-r--r--   0 runner    (1001) docker     (121)    51324 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_station.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17340 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_usgs_rdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6329 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-04-18 23:41:36.000000 hydrofunctions-0.2.3/tests/test_waterwatch.py
```

### Comparing `hydrofunctions-0.2.2/LICENSE` & `hydrofunctions-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/PKG-INFO` & `hydrofunctions-0.2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: hydrofunctions
-Version: 0.2.2
-Summary: A suite of convenience functions for exploring water data in a Jupyter Notebook.
+Version: 0.2.3
+Summary: A suite of convenience functions for exploring water data in a Jupyter Notebook
 Home-page: https://github.com/mroberge/hydrofunctions
 Author: Martin Roberge
 Author-email: mroberge@towson.edu
 License: MIT license
 Project-URL: Documentation, https://hydrofunctions.readthedocs.io
 Project-URL: Source, https://github.com/mroberge/hydrofunctions
 Project-URL: Latest, https://github.com/mroberge/hydrofunctions/tree/develop
-Project-URL: Tracker, https://github.com/mroberge/hydrofunctions/issues
+Project-URL: Issue Tracker, https://github.com/mroberge/hydrofunctions/issues
 Keywords: hydrofunctions hydrology USGS stream gauge water NWIS
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE
 
 ===============================
 HydroFunctions
 ===============================
 
 .. image:: https://img.shields.io/pypi/v/hydrofunctions.svg
@@ -47,15 +50,15 @@
         :target: https://hydrofunctions.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://img.shields.io/github/license/mashape/apistatus.svg
         :target: https://github.com/mroberge/hydrofunctions/blob/master/LICENSE
         :alt: MIT license
 
-a suite of convenience functions for exploring water data in Python.
+A suite of convenience functions for exploring water data in Python.
 
 Features
 --------
 
 * Retrieves stream data from the USGS NWIS service
 * Select data using multiple site numbers, by state, county codes, or a boundary box
 * Preserves NWIS metadata, including NoData values
@@ -66,65 +69,69 @@
    * flow duration charts
    * cycle plots to illustrate annual or diurnal cycles
    * Interactive map for finding stream gauge ID numbers
 * Plotting and manipulation through Pandas dataframes
 * Retrieve USGS rating curves, peak discharges, field notes, and site files for gauging stations
 * Retrieve USGS daily, monthly, and annual statistics for gauging stations
 * Saves data in compact, easy-to-use parquet files instead of requesting the same dataset repeatedly
-* **Massive Users Guide that makes Hydrology AND Data Science easy!**
+* **Massive** `Users Guide`_ **that makes Hydrology AND Data Science easy!**
 
 Still in active development! Let me know what features you want!
 
-Read the `Users Guide <https://hydrofunctions.readthedocs.io/en/master>`_ for more details.
+Read the `Users Guide`_ for more details.
 
 
 Basic Usage
 -----------
 
-First, import hydrofunctions into your project and enable automatic chart
-display:
+First, import hydrofunctions into your project. If you plan to work with Jupyter
+notebooks, then go ahead and enable automatic chart display:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> import hydrofunctions as hf
-    >>> %matplotlib inline
-..
+    In  [1]: import hydrofunctions as hf
+             %matplotlib inline
 
-Create NWIS data object to hold our request and the data we will retrieve.
-We will request the daily values ('dv') for site '0158520' for the past
-55 days:
+Create an NWIS data object to hold our request and the data we will retrieve.
+We will request the instantaneous values ('iv') for site '01585200' for the
+past 55 days:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> herring = hf.NWIS('01585200', 'dv', period='P55D')
+    In  [2]: herring = hf.NWIS('01585200', 'iv', period='P55D')
     Requested data from https://waterservices.usgs.gov/nwis/iv/?format=json%2C1.1&sites=01585200&period=P55D
-..
+
+You can check that the request went smoothly:
+
+.. code-block:: ipython
+
+    In  [3]: herring.ok
+    Out [3]: True
 
 Find out what data we received:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> herring
-    USGS:01585200: WEST BRANCH HERRING RUN AT IDLEWYLDE, MD
-        00060: <5 * Minutes>  Discharge, cubic feet per second
-        00065: <5 * Minutes>  Gage height, feet
-    Start: 2019-05-25 01:05:00+00:00
-    End:   2019-07-19 19:05:00+00:00
-..
+    In  [4]: herring
+    Out [4]: USGS:01585200: WEST BRANCH HERRING RUN AT IDLEWYLDE, MD
+                 00060: <5 * Minutes>  Discharge, cubic feet per second
+                 00065: <5 * Minutes>  Gage height, feet
+             Start: 2019-05-25 01:05:00+00:00
+             End:   2019-07-19 19:05:00+00:00
 
-This tells us the name of our site, and gives a list of the parameters that we
+This tells us the name of our site and gives a list of the parameters that we
 have. For each parameter it lists how frequently the data were collected, and
-it show the common name of the parameter and its units.
+it shows the common name of the parameter and its units.
 
-Create a dataframe from our data, and list the first five items:
+Create a dataframe using only our discharge data, and list the first five items:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> herring.df().head()
-..
+    In  [5]: herring.df('discharge').head()
+    Out [5]:
 
 *--a table with our data appears--*
 
     +------------------------------+---------------------------+
     |          datetimeUTC         | USGS:01585200:00060:00000 |
     +------------------------------+---------------------------+
     |   2019-05-25 01:05:00+00:00  |                1.57       |
@@ -134,37 +141,48 @@
     |   2019-05-25 01:15:00+00:00  |                1.51       |
     +------------------------------+---------------------------+
     |   2019-05-25 01:20:00+00:00  |                1.57       |
     +------------------------------+---------------------------+
     |   2019-05-25 01:25:00+00:00  |                1.57       |
     +------------------------------+---------------------------+
 
-Plot the data using built-in methods from Pandas and mathplotlib:
+If we're using Jupyter Lab, we can plot a graph of the data using built-in methods from Pandas and mathplotlib:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> herring.df().plot()
-..
+    In  [6]: herring.df('q').plot()
+    Out [6]:
 
 *--a stream hydrograph appears--*
 
 .. image:: https://raw.githubusercontent.com/mroberge/hydrofunctions/master/_static/HerringHydrograph.png
-        :alt: a stream hydrograph for Herring Run
+   :alt: a stream hydrograph for Herring Run
+
+Learn more:  
+
+* `Users Guide`_
+
 
 Easy Installation
 -----------------
 
 The easiest way to install Hydrofunctions is by typing this from your
 command line:
 
 .. code-block:: console
 
     $ pip install hydrofunctions
-..
+
 
 Hydrofunctions depends upon Pandas and numerous other scientific packages
-for Python. `Anaconda <https://docs.anaconda.com/anaconda/install/>`_
+for Python. `Anaconda <https://www.anaconda.com/products/individual>`_
 is an easy, safe, open-source method for downloading everything and avoiding
 conflicts with other versions of Python that might be running on your
 computer.
 
+Visit the `Installation Page <https://hydrofunctions.readthedocs.io/en/master/installation.html>`_
+in the Users Guide to learn how to install
+Anaconda, or if you have problems using the Easy Installation method above.
+
+
+.. _`Users Guide`:  https://hydrofunctions.readthedocs.io/en/latest
```

### Comparing `hydrofunctions-0.2.2/README.rst` & `hydrofunctions-0.2.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 past 55 days:
 
 .. code-block:: ipython
 
     In  [2]: herring = hf.NWIS('01585200', 'iv', period='P55D')
     Requested data from https://waterservices.usgs.gov/nwis/iv/?format=json%2C1.1&sites=01585200&period=P55D
 
-Check that the request went smoothly:
+You can check that the request went smoothly:
 
 .. code-block:: ipython
 
     In  [3]: herring.ok
     Out [3]: True
 
 Find out what data we received:
@@ -82,17 +82,17 @@
     In  [4]: herring
     Out [4]: USGS:01585200: WEST BRANCH HERRING RUN AT IDLEWYLDE, MD
                  00060: <5 * Minutes>  Discharge, cubic feet per second
                  00065: <5 * Minutes>  Gage height, feet
              Start: 2019-05-25 01:05:00+00:00
              End:   2019-07-19 19:05:00+00:00
 
-This tells us the name of our site, and gives a list of the parameters that we
+This tells us the name of our site and gives a list of the parameters that we
 have. For each parameter it lists how frequently the data were collected, and
-it show the common name of the parameter and its units.
+it shows the common name of the parameter and its units.
 
 Create a dataframe using only our discharge data, and list the first five items:
 
 .. code-block:: ipython
 
     In  [5]: herring.df('discharge').head()
     Out [5]:
@@ -109,24 +109,24 @@
     |   2019-05-25 01:15:00+00:00  |                1.51       |
     +------------------------------+---------------------------+
     |   2019-05-25 01:20:00+00:00  |                1.57       |
     +------------------------------+---------------------------+
     |   2019-05-25 01:25:00+00:00  |                1.57       |
     +------------------------------+---------------------------+
 
-Plot the data using built-in methods from Pandas and mathplotlib:
+If we're using Jupyter Lab, we can plot a graph of the data using built-in methods from Pandas and mathplotlib:
 
 .. code-block:: ipython
 
     In  [6]: herring.df('q').plot()
     Out [6]:
 
 *--a stream hydrograph appears--*
 
-.. image:: _static/HerringHydrograph.png
+.. image:: https://raw.githubusercontent.com/mroberge/hydrofunctions/master/_static/HerringHydrograph.png
    :alt: a stream hydrograph for Herring Run
 
 Learn more:  
 
 * `Users Guide`_
```

### Comparing `hydrofunctions-0.2.2/_static/HerringHydrograph.png` & `hydrofunctions-0.2.3/_static/HerringHydrograph.png`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/_static/HydroCloudTable.png` & `hydrofunctions-0.2.3/_static/HydroCloudTable.png`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/_static/draw_map.jpg` & `hydrofunctions-0.2.3/_static/draw_map.jpg`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/_static/favicon.ico` & `hydrofunctions-0.2.3/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/Makefile` & `hydrofunctions-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/_static/HerringHydrograph.png` & `hydrofunctions-0.2.3/docs/_static/HerringHydrograph.png`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/_static/cycleplot_annual-week.png` & `hydrofunctions-0.2.3/docs/_static/cycleplot_annual-week.png`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/_static/cycleplot_dirunal_compare-month.png` & `hydrofunctions-0.2.3/docs/_static/cycleplot_dirunal_compare-month.png`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/_static/cycleplot_diurnal_compare-month.jpg` & `hydrofunctions-0.2.3/docs/_static/cycleplot_diurnal_compare-month.jpg`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/_static/flow_duration_linear.png` & `hydrofunctions-0.2.3/docs/_static/flow_duration_linear.png`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/_static/flow_duration_logit.png` & `hydrofunctions-0.2.3/docs/_static/flow_duration_logit.png`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/_static/hf-logo-sm.svg` & `hydrofunctions-0.2.3/docs/_static/hf-logo-sm.svg`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/_static/hf-logo.svg` & `hydrofunctions-0.2.3/docs/_static/hf-logo.svg`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/conf.py` & `hydrofunctions-0.2.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 # Renames internal refs so that they include page #.
 # See http://www.sphinx-doc.org/en/stable/ext/autosectionlabel.html#confval-autosectionlabel_prefix_document
 autosectionlabel_prefix_document = True
 
 # General information about the project.
 project = "Hydrofunctions"
-copyright = "Copyright 2016-2021, Martin Roberge and Hydrofunctions contributors"
+copyright = "Copyright 2016-2022, Martin Roberge and Hydrofunctions contributors"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = hydrofunctions.__version__
@@ -336,15 +336,15 @@
 texinfo_documents = [
     (
         "index",
         "hydrofunctions",
         u"HydroFunctions User's Guide",
         u"Martin Roberge",
         "hydrofunctions",
-        "A set of convenience functions for exploring water data.",
+        "A suite of convenience functions for exploring water data.",
         "Miscellaneous",
     ),
 ]
 
 # Documents to append as an appendix to all manuals.
 # texinfo_appendices = []
```

### Comparing `hydrofunctions-0.2.2/docs/contributing.rst` & `hydrofunctions-0.2.3/docs/contributing.rst`

 * *Files 14% similar despite different names*

```diff
@@ -36,107 +36,107 @@
 - If you make a change, add your name to AUTHORS.rst
 - Note your change in HISTORY.rst and initial it.
 - Use docstrings, illustrate features in a notebook, add a section to docs/usage.rst
 - I use 'Black' for code formatting. Follow PEP8 standards!
 - Use `Google-style docstrings <https://google.github.io/styleguide/pyguide.html?showone=Comments#Comments>`_
   , described `here <https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html>`_.
 - Add tests! Lots of tests! Make sure you test your code!
-- Your code should work for Python 3.6, 3.7, 3.8, & 3.9. This gets tested by the `CI <https://github.com/mroberge/hydrofunctions/actions/workflows/test.yaml>`_
+- Your code should work for Python 3.6, 3.7, 3.8, 3.9, & 3.10. This gets tested by the `CI <https://github.com/mroberge/hydrofunctions/actions/workflows/test.yaml>`_
 
 
 A detailed guide to contributing new code
 -----------------------------------------
 
 .. highlight:: doscon
 
 Ready to contribute? Here's how to set up `hydrofunctions` for local development.
 
 #. Fork the `hydrofunctions repo <https://github.com/mroberge/hydrofunctions>`_ on GitHub by clicking the
    'Fork' button near the upper right corner.
 
+#. Open the GitHub page for your fork, and clone it to your local computer where you
+   will be doing your coding. To clone your fork, I like to use GitHub's Desktop tool, 
+   which does a great job of putting most of Git's best features into an easy-to-use GUI.
+
+   Download `GitHub Desktop <https://desktop.github.com>`_.
+
+   There are two ways to clone your files to your local computer:
+
+   - Starting from the GitHub page for your fork: Select the 'Code' button and select 'Open with GitHub Desktop'
+   - or, if you have GitHub Desktop open: File > clone repository...
+
+   These options will set up a local folder on your computer where you can use git while editing
+   your version of hydrofunctions.
+
 #. Install Anaconda 3 if you don't already have it on your system. This includes the
-   latest version of Python, and
-   a package manager, **conda**, which replaces pip and also manages virtual
-   environments, replacing venv, and virtualenv.:
+   latest version of Python, and a package manager, **conda**, which is an alternative to pip that
+   also manages virtual environments, replacing venv, and virtualenv.:
 
    Download Anaconda: https://www.continuum.io/downloads
 
 #. Much of the rest involves the command line. In the following examples I'll
    be using Windows, but this will only affect simple commands like making a new
    directory, or changing directory. The important commands are the same on
    different platforms.  Also, if you are using Windows, use **cmd.exe** as your
    command line instead of PowerShell, which seems to interfere
    with one of our tools, conda.
 
-#. Create a directory for your development work and change directories into
-   it (I call mine py-dev)::
-
-     > mkdir py-dev
-     > cd py-dev
+#. Create a new conda environment named `my39env`. Include everything we need:
+   python 3.9, git, and the anaconda set of scientific packages::
 
-#. Create a new conda environment named `my36env`. Include everything we need:
-   python 3.6, git, and the anaconda set of scientific packages::
-
-    > conda create -n my36env python=3.6 anaconda git
+    > conda create -n my36env python=3.9 anaconda git
 
 #. List all of your available environments and activate my36env. The active
    environment will have a star next to it::
 
     > conda info -e
-    > activate my36env
+    > activate my39env
 
 #. For kicks, check that you've got the right version of python running, and
    list all of the packages that you have available to you in this environment::
 
     > python --version
     > conda list
 
-#. Conda doesn't install packages located on github or pypi, so we'll use pip to install the source
-   files from the fork you created in your GitHub account. We use the -e flag to install packages
-   in development mode. This creates a src directory with
-   a subdirectory named in the `egg=` part of the url. Now you can edit the source
-   files and have the edits freshly interpreted again when you `import
-   hydrofunctions` during a python session. Additionally, git will create a `.git`
-   directory inside of the hydrofunctions directory. ::
-
-    > pip install -e git+https://github.com/your_github_name/hydrofunctions.git@develop#egg=hydrofunctions
-
-#. Move into the hydrofunctions directory::
-
-    > cd src/hydrofunctions
+#. Now we are going to install hydrofunctions using the file from **your** forked version, 
+   instead of the standard version from PyPI. To do this, first move into the directory
+   where you had GitHub Desktop put your clone::
+
+   > cd GitHub/hydrofunctions
+
+#. We'll use pip to install your files in 'develop' mode using the '-e' flag. 
+   Now you can edit the source files and have the edits freshly interpreted again when you
+   `import hydrofunctions` during a python session. The [dev] part tells pip to install all
+   of the extra requirements that you'll need as a developer::
+   
+   > pip install -e .[dev]
 
 #. Run the automatic tests to make sure everything is hunky-dory::
 
-    > python setup.py test
+    > pytest
 
-#. Start your own branch in git::
+#. Before you start improving hydrofunctions with all your fantastic changes, create a new branch.
+   Give it a simple name that explains what your change adds::
 
     > git checkout -b name-of-your-bugfix-or-feature
 
-   Alternatively, use GitHub's Desktop tool, which does a great job of putting most of
-   Git's best features into an easy-to-use GUI.
-
-   Download `GitHub Desktop <https://desktop.github.com>`_.
-   Add the repository we created in step 8:
+   Alternatively, use GitHub's Desktop tool:
 
-        - click on the + pull-down > 'Add';
-        - find the repository `py-dev/src/hydrofunctions`
-        - confirm with 'Add Repository'.
-        - Any changes you make in this directory will appear in this program.
+      - Branch > New branch...
 
-#. Go ahead and make changes to the files now. I like to use Spyder, which you
+#. Go ahead and make changes to the files now. I like to use VS Code or Spyder, which you
    installed already with anaconda::
 
     > spyder
 
 #. After you've made a small change, make sure you didn't break anything by
    running the tests again. I find it easiest to run the tests from the command
-   line::
+   line inside the hydrofunctions directory::
 
-    > python setup.py tests
+    > pytest
 
 #. Before you make too many changes, 'commit' what you've done. Ideally, each
    group of changes that you put into a commit will be logically related to each
    other, and the group of changes will be really small. Make sure that you
    explain your changes in the commit message. Use GitHub Desktop. If you use the
    command line, then type::
 
@@ -166,29 +166,29 @@
 
     $ git clone git@github.com:your_name_here/hydrofunctions.git
 
 3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
 
     $ mkvirtualenv hydrofunctions
     $ cd hydrofunctions/
-    $ python setup.py develop
+    $ pip install -e .[dev]
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
    Now you can make your changes locally.
 
 5. When you're done making changes, check that your changes pass flake8 and the tests, including
    testing other Python versions with tox::
 
        $ flake8 hydrofunctions tests
-       $ python setup.py test
+       $ pytest
 
-   or ``$ python -m unittest -v`` or  ``$ py.test`` or ``$ nose2``
+   or ``$ python -m unittest -v``
 
    then::
 
     $ tox
 
    To get flake8 and tox, just pip install them into your virtualenv.::
```

### Comparing `hydrofunctions-0.2.2/docs/graphing.rst` & `hydrofunctions-0.2.3/docs/graphing.rst`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/history.rst` & `hydrofunctions-0.2.3/docs/history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -110,7 +110,15 @@
 * Added verbose mode to USGS RDB functions
 * Bugfix: `hf.df('q')` returned non-discharge data; fixed & added tests & fixture (dgk)
 * Bugfix: renamed `typing.py` module to `validate.py` to prevent interference with typing
 * Bugfix: HF will raise HydroNoDataError when non-200 response comes back from USGS
 * Bugfix: logging off by default.
 * Added hf._start_logging() to create a log & start logging.
 * HydroExceptions will now create a log message when raised.
+
+0.2.3 (2022-04-18)
+--------------------
+
+* Moved package requirements & dev requirements to setup.cfg
+* Create new 'dev' extra_requirements. Install from inside hydrofunctions: `pip install -e .[dev]`
+* Changed default behavior of NWIS & extract_nwis_df to NOT fill missing values by interpolation.
+
```

### Comparing `hydrofunctions-0.2.2/docs/hydrofunctions.rst` & `hydrofunctions-0.2.3/docs/hydrofunctions.rst`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/index.rst` & `hydrofunctions-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/installation.rst` & `hydrofunctions-0.2.3/docs/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
 
 
 Why use Anaconda?
 =================
 
 Anaconda is a free, open-source Python distribution. It bundles important
-scientific software like Jupyter notebooks and the Spyder IDE all into one
+scientific software like Jupyter notebooks, VS Code, and the Spyder IDE all into one
 pre-configured, pre-compiled download, along with a huge number of scientific
 libraries (packages). It also includes a tool, `conda`, which manages and
 updates these packages. Conda also creates 'environments', which are isolated
 installations of Python, just in case your ArcGIS software (for example) uses a
 different version of Python than some other piece of software.
 
 If you want to install Jupyter notebooks at the same time that you install
@@ -66,29 +66,29 @@
 Safe Anaconda install for people having problems
 ================================================
 
 *For people who like to write their own code, or have Python already installed
 for something else, or who had difficulties.*
 
 1. From the command prompt, create a new environment called 'myenv' with
-packages for Python 3.7 and jupyter notebooks::
+packages for Python 3.9 and jupyter notebooks::
 
         > conda create -n myenv python=3.7 jupyternb nb_conda
 
 
 2. List all of the environments that you have
 available::
 
         > conda info -e
 
 
 3. The active environment will have a star next to it. To activate a
 different environment, such as the one you just created, type::
 
-        > conda activate name_of_environment
+        > activate name_of_environment
 
 
 4. To test that you have the correct version
 of python::
 
         > python --version
 
@@ -108,15 +108,15 @@
 and other bundled software directly. If you would rather just launch python
 directly from the command line, just open a command prompt and type the
 following:
 
       - for a command line interface: `python`
       - for an enhanced command line: `ipython`
       - to use the Spyder IDE: `spyder`
-      - or to use a Jupyter Notebook: `jupyter notebook`
+      - or to use Jupyter Notebook: `jupyter lab`
 
 To use hydrofunctions in your python code, make sure that one of your first
 lines says this::
 
          > import hydrofunctions as hf
```

### Comparing `hydrofunctions-0.2.2/docs/introduction.rst` & `hydrofunctions-0.2.3/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/make.bat` & `hydrofunctions-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Comparing_Urban_and_Rural_Streams.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Comparing_Urban_and_Rural_Streams.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/DailyMean_vs_Instant.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/DailyMean_vs_Instant.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Data_Catalog.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Data_Catalog.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/DeadRun_Daily.parquet` & `hydrofunctions-0.2.3/docs/notebooks/DeadRun_Daily.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/DeadRun_Instant.parquet` & `hydrofunctions-0.2.3/docs/notebooks/DeadRun_Instant.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Draw_Map_Demo.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Draw_Map_Demo.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Graphing.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Graphing.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Hydrofunctions_Comparing_Stream_Environments.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Hydrofunctions_Comparing_Stream_Environments.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Hydrofunctions_Tutorial.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Hydrofunctions_Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Hydrofunctions_nested_watersheds.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Hydrofunctions_nested_watersheds.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Hysteresis.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Hysteresis.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/PG.parquet` & `hydrofunctions-0.2.3/docs/notebooks/PG.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Peak_Discharge.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Peak_Discharge.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Saving_Data.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Saving_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Selecting_Sites.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Selecting_Sites.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Site_File.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Site_File.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/USGS_Statistics_Service.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/USGS_Statistics_Service.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Urban_Rural.parquet` & `hydrofunctions-0.2.3/docs/notebooks/Urban_Rural.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/Writing_Valid_Requests_for_NWIS.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/Writing_Valid_Requests_for_NWIS.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/_static/HerringHydrograph.png` & `hydrofunctions-0.2.3/docs/notebooks/_static/HerringHydrograph.png`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/_static/HydroCloudTable.png` & `hydrofunctions-0.2.3/docs/notebooks/_static/HydroCloudTable.png`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/_static/draw_map.jpg` & `hydrofunctions-0.2.3/docs/notebooks/_static/draw_map.jpg`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/create_df.parquet` & `hydrofunctions-0.2.3/docs/notebooks/create_df.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/graphing-1.parquet` & `hydrofunctions-0.2.3/docs/notebooks/graphing-1.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/graphing-2.parquet` & `hydrofunctions-0.2.3/docs/notebooks/graphing-2.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/groundwater.parquet` & `hydrofunctions-0.2.3/docs/notebooks/groundwater.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/herring_july.parquet` & `hydrofunctions-0.2.3/docs/notebooks/herring_july.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/mult.parquet` & `hydrofunctions-0.2.3/docs/notebooks/mult.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/parquet_example.parquet` & `hydrofunctions-0.2.3/docs/notebooks/parquet_example.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/parquet_example2.parquet` & `hydrofunctions-0.2.3/docs/notebooks/parquet_example2.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/save_example.json.gz` & `hydrofunctions-0.2.3/docs/notebooks/save_example.json.gz`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/save_example.parquet` & `hydrofunctions-0.2.3/docs/notebooks/save_example.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/view-example.parquet` & `hydrofunctions-0.2.3/docs/notebooks/view-example.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/viewing.ipynb` & `hydrofunctions-0.2.3/docs/notebooks/viewing.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/docs/notebooks/virginia.parquet` & `hydrofunctions-0.2.3/docs/notebooks/virginia.parquet`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/hydrofunctions/__init__.py` & `hydrofunctions-0.2.3/src/hydrofunctions/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,22 +52,23 @@
     >>> help(hf)
     >>> help(hf.NWIS)
 
 Read more about Hydrofunctions here: https://hydrofunctions.readthedocs.io/
 
 """
 from __future__ import absolute_import, print_function
+try:
+    from importlib.metadata import version
+except ImportError:
+    from importlib_metadata import version
 
-__title__ = "hydrofunctions"
-__version__ = "0.2.2"
+__version__ = version('hydrofunctions')
 __author__ = "Martin Roberge"
-__email__ = "mroberge@towson.edu"
-__license__ = "MIT"
-__copyright__ = "Copyright 2016 Martin Roberge and contributors"
-
+__author_email__ = "mroberge@towson.edu"
+__url__ = "https://github.com/mroberge/hydrofunctions"
 
 from .exceptions import (
     HydroNoDataError,
     HydroUserWarning,
 )
 from .hydrofunctions import (
     get_nwis,
```

### Comparing `hydrofunctions-0.2.2/hydrofunctions/charts.py` & `hydrofunctions-0.2.3/src/hydrofunctions/charts.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/hydrofunctions/exceptions.py` & `hydrofunctions-0.2.3/src/hydrofunctions/exceptions.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/hydrofunctions/helpers.py` & `hydrofunctions-0.2.3/src/hydrofunctions/helpers.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/hydrofunctions/hydrofunctions.py` & `hydrofunctions-0.2.3/src/hydrofunctions/hydrofunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,23 +408,26 @@
     # Why catch this? If we can't find the key, we already return the index.
     except:  # TODO: dangerous to use bare 'except'  clauses.
         msg = 'The selected key "{}" could not be found'.format(key)
         raise ValueError(msg)
     return vals
 
 
-def extract_nwis_df(nwis_dict, interpolate=True):
+def extract_nwis_df(nwis_dict, interpolate=False):
     """Returns a Pandas dataframe and a metadata dict from the NWIS response
     object or the json dict of the response.
 
     Args:
         nwis_dict (obj):
             the json from a response object as returned by get_nwis().json().
             Alternatively, you may supply the response object itself.
 
+        interpolate (bool):
+            fill missing data values with interpolated values. Default False.
+
     Returns:
         a pandas dataframe.
 
     Raises:
         HydroNoDataError
             when the request is valid, but NWIS has no data for
             the parameters provided in the request.
```

### Comparing `hydrofunctions-0.2.2/hydrofunctions/logging.py` & `hydrofunctions-0.2.3/src/hydrofunctions/logging.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/hydrofunctions/station.py` & `hydrofunctions-0.2.3/src/hydrofunctions/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,17 @@
 
         period (str):
             NWIS period code. Default is None.
                 * Format is "PxxD", where xx is the number of days before \
                 today, with a maximum of 999 days accepted.
                 * Either use start_date or period, but not both.
 
+        interpolate (bool):
+            Fill missing values through interpolation. Default False.
+        
         file (str):
             A filename for acting as a cache for the data request. Accepts file
             extensions of '*.json.gz' (default) and '*.parquet'. If this parameter is
             included, the NWIS object will first attempt to read its data from the file.
             If the file does not exist, it will use the other parameters to obtain the
             data and will then save to the provided filename.
 
@@ -110,14 +113,15 @@
         start_date=None,
         end_date=None,
         stateCd=None,
         countyCd=None,
         bBox=None,
         parameterCd="all",
         period=None,
+        interpolate=False,
         file=None,
         verbose=True,
     ):
 
         self.ok = False
         if file:
             if len(file.split(".")) == 1:
@@ -143,15 +147,15 @@
                 bBox=bBox,
                 parameterCd=parameterCd,
                 period=period,
                 verbose=verbose,
             )
             try:
                 self.json = self.response.json()
-                self._dataframe, self.meta = hf.extract_nwis_df(self.json)
+                self._dataframe, self.meta = hf.extract_nwis_df(self.json, interpolate=interpolate)
                 self.ok = self.response.ok
                 if file is not None:
                     self.save(file)
                     if verbose:
                         print("Saving data to", file)
             except json.JSONDecodeError as err:
                 self.ok = False
```

### Comparing `hydrofunctions-0.2.2/hydrofunctions/usgs_rdb.py` & `hydrofunctions-0.2.3/src/hydrofunctions/usgs_rdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 This module is for working with the various USGS dataservices that use the rdb
 text format. These include the statistics service, the field measurements
 service, the rating curve service, and the peak discharge service.
 """
 import pandas as pd
 import requests
 from io import StringIO
-from IPython.core import display
+from IPython import display
 from . import exceptions
 
 
 class hydroRDB:
     """A class for holding the information from USGS rdb files.
 
     Args:
```

### Comparing `hydrofunctions-0.2.2/hydrofunctions/validate.py` & `hydrofunctions-0.2.3/src/hydrofunctions/validate.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/hydrofunctions/waterwatch.py` & `hydrofunctions-0.2.3/src/hydrofunctions/waterwatch.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/hydrofunctions.egg-info/PKG-INFO` & `hydrofunctions-0.2.3/src/hydrofunctions.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: hydrofunctions
-Version: 0.2.2
-Summary: A suite of convenience functions for exploring water data in a Jupyter Notebook.
+Version: 0.2.3
+Summary: A suite of convenience functions for exploring water data in a Jupyter Notebook
 Home-page: https://github.com/mroberge/hydrofunctions
 Author: Martin Roberge
 Author-email: mroberge@towson.edu
 License: MIT license
 Project-URL: Documentation, https://hydrofunctions.readthedocs.io
 Project-URL: Source, https://github.com/mroberge/hydrofunctions
 Project-URL: Latest, https://github.com/mroberge/hydrofunctions/tree/develop
-Project-URL: Tracker, https://github.com/mroberge/hydrofunctions/issues
+Project-URL: Issue Tracker, https://github.com/mroberge/hydrofunctions/issues
 Keywords: hydrofunctions hydrology USGS stream gauge water NWIS
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Hydrology
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: dev
 License-File: LICENSE
 
 ===============================
 HydroFunctions
 ===============================
 
 .. image:: https://img.shields.io/pypi/v/hydrofunctions.svg
@@ -47,15 +50,15 @@
         :target: https://hydrofunctions.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 .. image:: https://img.shields.io/github/license/mashape/apistatus.svg
         :target: https://github.com/mroberge/hydrofunctions/blob/master/LICENSE
         :alt: MIT license
 
-a suite of convenience functions for exploring water data in Python.
+A suite of convenience functions for exploring water data in Python.
 
 Features
 --------
 
 * Retrieves stream data from the USGS NWIS service
 * Select data using multiple site numbers, by state, county codes, or a boundary box
 * Preserves NWIS metadata, including NoData values
@@ -66,65 +69,69 @@
    * flow duration charts
    * cycle plots to illustrate annual or diurnal cycles
    * Interactive map for finding stream gauge ID numbers
 * Plotting and manipulation through Pandas dataframes
 * Retrieve USGS rating curves, peak discharges, field notes, and site files for gauging stations
 * Retrieve USGS daily, monthly, and annual statistics for gauging stations
 * Saves data in compact, easy-to-use parquet files instead of requesting the same dataset repeatedly
-* **Massive Users Guide that makes Hydrology AND Data Science easy!**
+* **Massive** `Users Guide`_ **that makes Hydrology AND Data Science easy!**
 
 Still in active development! Let me know what features you want!
 
-Read the `Users Guide <https://hydrofunctions.readthedocs.io/en/master>`_ for more details.
+Read the `Users Guide`_ for more details.
 
 
 Basic Usage
 -----------
 
-First, import hydrofunctions into your project and enable automatic chart
-display:
+First, import hydrofunctions into your project. If you plan to work with Jupyter
+notebooks, then go ahead and enable automatic chart display:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> import hydrofunctions as hf
-    >>> %matplotlib inline
-..
+    In  [1]: import hydrofunctions as hf
+             %matplotlib inline
 
-Create NWIS data object to hold our request and the data we will retrieve.
-We will request the daily values ('dv') for site '0158520' for the past
-55 days:
+Create an NWIS data object to hold our request and the data we will retrieve.
+We will request the instantaneous values ('iv') for site '01585200' for the
+past 55 days:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> herring = hf.NWIS('01585200', 'dv', period='P55D')
+    In  [2]: herring = hf.NWIS('01585200', 'iv', period='P55D')
     Requested data from https://waterservices.usgs.gov/nwis/iv/?format=json%2C1.1&sites=01585200&period=P55D
-..
+
+You can check that the request went smoothly:
+
+.. code-block:: ipython
+
+    In  [3]: herring.ok
+    Out [3]: True
 
 Find out what data we received:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> herring
-    USGS:01585200: WEST BRANCH HERRING RUN AT IDLEWYLDE, MD
-        00060: <5 * Minutes>  Discharge, cubic feet per second
-        00065: <5 * Minutes>  Gage height, feet
-    Start: 2019-05-25 01:05:00+00:00
-    End:   2019-07-19 19:05:00+00:00
-..
+    In  [4]: herring
+    Out [4]: USGS:01585200: WEST BRANCH HERRING RUN AT IDLEWYLDE, MD
+                 00060: <5 * Minutes>  Discharge, cubic feet per second
+                 00065: <5 * Minutes>  Gage height, feet
+             Start: 2019-05-25 01:05:00+00:00
+             End:   2019-07-19 19:05:00+00:00
 
-This tells us the name of our site, and gives a list of the parameters that we
+This tells us the name of our site and gives a list of the parameters that we
 have. For each parameter it lists how frequently the data were collected, and
-it show the common name of the parameter and its units.
+it shows the common name of the parameter and its units.
 
-Create a dataframe from our data, and list the first five items:
+Create a dataframe using only our discharge data, and list the first five items:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> herring.df().head()
-..
+    In  [5]: herring.df('discharge').head()
+    Out [5]:
 
 *--a table with our data appears--*
 
     +------------------------------+---------------------------+
     |          datetimeUTC         | USGS:01585200:00060:00000 |
     +------------------------------+---------------------------+
     |   2019-05-25 01:05:00+00:00  |                1.57       |
@@ -134,37 +141,48 @@
     |   2019-05-25 01:15:00+00:00  |                1.51       |
     +------------------------------+---------------------------+
     |   2019-05-25 01:20:00+00:00  |                1.57       |
     +------------------------------+---------------------------+
     |   2019-05-25 01:25:00+00:00  |                1.57       |
     +------------------------------+---------------------------+
 
-Plot the data using built-in methods from Pandas and mathplotlib:
+If we're using Jupyter Lab, we can plot a graph of the data using built-in methods from Pandas and mathplotlib:
 
-.. code-block:: python
+.. code-block:: ipython
 
-    >>> herring.df().plot()
-..
+    In  [6]: herring.df('q').plot()
+    Out [6]:
 
 *--a stream hydrograph appears--*
 
 .. image:: https://raw.githubusercontent.com/mroberge/hydrofunctions/master/_static/HerringHydrograph.png
-        :alt: a stream hydrograph for Herring Run
+   :alt: a stream hydrograph for Herring Run
+
+Learn more:  
+
+* `Users Guide`_
+
 
 Easy Installation
 -----------------
 
 The easiest way to install Hydrofunctions is by typing this from your
 command line:
 
 .. code-block:: console
 
     $ pip install hydrofunctions
-..
+
 
 Hydrofunctions depends upon Pandas and numerous other scientific packages
-for Python. `Anaconda <https://docs.anaconda.com/anaconda/install/>`_
+for Python. `Anaconda <https://www.anaconda.com/products/individual>`_
 is an easy, safe, open-source method for downloading everything and avoiding
 conflicts with other versions of Python that might be running on your
 computer.
 
+Visit the `Installation Page <https://hydrofunctions.readthedocs.io/en/master/installation.html>`_
+in the Users Guide to learn how to install
+Anaconda, or if you have problems using the Easy Installation method above.
+
+
+.. _`Users Guide`:  https://hydrofunctions.readthedocs.io/en/latest
```

### Comparing `hydrofunctions-0.2.2/hydrofunctions.egg-info/SOURCES.txt` & `hydrofunctions-0.2.3/src/hydrofunctions.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
-pypi_readme.rst
+VERSION.txt
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
 _static/HerringHydrograph.png
 _static/HydroCloudTable.png
 _static/draw_map.jpg
 _static/favicon.ico
 docs/Makefile
@@ -61,30 +60,30 @@
 docs/notebooks/save_example.parquet
 docs/notebooks/view-example.parquet
 docs/notebooks/viewing.ipynb
 docs/notebooks/virginia.parquet
 docs/notebooks/_static/HerringHydrograph.png
 docs/notebooks/_static/HydroCloudTable.png
 docs/notebooks/_static/draw_map.jpg
-hydrofunctions/__init__.py
-hydrofunctions/charts.py
-hydrofunctions/exceptions.py
-hydrofunctions/helpers.py
-hydrofunctions/hydrofunctions.py
-hydrofunctions/logging.py
-hydrofunctions/station.py
-hydrofunctions/usgs_rdb.py
-hydrofunctions/validate.py
-hydrofunctions/waterwatch.py
-hydrofunctions.egg-info/PKG-INFO
-hydrofunctions.egg-info/SOURCES.txt
-hydrofunctions.egg-info/dependency_links.txt
-hydrofunctions.egg-info/not-zip-safe
-hydrofunctions.egg-info/requires.txt
-hydrofunctions.egg-info/top_level.txt
+src/hydrofunctions/__init__.py
+src/hydrofunctions/charts.py
+src/hydrofunctions/exceptions.py
+src/hydrofunctions/helpers.py
+src/hydrofunctions/hydrofunctions.py
+src/hydrofunctions/logging.py
+src/hydrofunctions/station.py
+src/hydrofunctions/usgs_rdb.py
+src/hydrofunctions/validate.py
+src/hydrofunctions/waterwatch.py
+src/hydrofunctions.egg-info/PKG-INFO
+src/hydrofunctions.egg-info/SOURCES.txt
+src/hydrofunctions.egg-info/dependency_links.txt
+src/hydrofunctions.egg-info/not-zip-safe
+src/hydrofunctions.egg-info/requires.txt
+src/hydrofunctions.egg-info/top_level.txt
 tests/Test Data Prep.ipynb
 tests/__init__.py
 tests/fixtures.py
 tests/fixtures_daily_dupe.py
 tests/fixtures_data.py
 tests/fixtures_multiple_methods.py
 tests/fixtures_recent_only.py
```

### Comparing `hydrofunctions-0.2.2/tests/Test Data Prep.ipynb` & `hydrofunctions-0.2.3/tests/Test Data Prep.ipynb`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/fixtures.py` & `hydrofunctions-0.2.3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/fixtures_daily_dupe.py` & `hydrofunctions-0.2.3/tests/fixtures_daily_dupe.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/fixtures_data.py` & `hydrofunctions-0.2.3/tests/fixtures_data.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/fixtures_multiple_methods.py` & `hydrofunctions-0.2.3/tests/fixtures_multiple_methods.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/fixtures_recent_only.py` & `hydrofunctions-0.2.3/tests/fixtures_recent_only.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/fixtures_tzfail.py` & `hydrofunctions-0.2.3/tests/fixtures_tzfail.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/fixtures_usgs_rdb.py` & `hydrofunctions-0.2.3/tests/fixtures_usgs_rdb.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/test_charts.py` & `hydrofunctions-0.2.3/tests/test_charts.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/test_exceptions.py` & `hydrofunctions-0.2.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/test_helpers.py` & `hydrofunctions-0.2.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/test_hydrofunctions.py` & `hydrofunctions-0.2.3/tests/test_hydrofunctions.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/test_logging.py` & `hydrofunctions-0.2.3/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/test_online_resources.py` & `hydrofunctions-0.2.3/tests/test_online_resources.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/test_station.py` & `hydrofunctions-0.2.3/tests/test_station.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,15 @@
         mock_df = pd.DataFrame(
             np.random.randn(5, 1),
             columns=["A"],
             index=pd.date_range("20130101", periods=5, freq="T"),
         )
         mock_extract_nwis_df.return_value = (mock_df, "expected dict")
         actual = station.NWIS()
-        mock_extract_nwis_df.assert_called_once_with(expected_json)
+        mock_extract_nwis_df.assert_called_once_with(expected_json, interpolate=False)
 
     @mock.patch("hydrofunctions.hydrofunctions.read_parquet")
     def test_NWIS_init_filename_calls_read_parquet(self, mock_read):
         expected_filename = "expected_filename.parquet"
         expected_meta = "expected meta"
         expected_df = pd.DataFrame(
             np.random.randn(5, 1),
```

### Comparing `hydrofunctions-0.2.2/tests/test_usgs_rdb.py` & `hydrofunctions-0.2.3/tests/test_usgs_rdb.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/test_validate.py` & `hydrofunctions-0.2.3/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `hydrofunctions-0.2.2/tests/test_waterwatch.py` & `hydrofunctions-0.2.3/tests/test_waterwatch.py`

 * *Files identical despite different names*

