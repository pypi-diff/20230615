# Comparing `tmp/EXtra-data-1.9.0.tar.gz` & `tmp/EXtra-data-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EXtra-data-1.9.0.tar", last modified: Thu Nov 25 13:34:24 2021, max compression
+gzip compressed data, was "EXtra-data-1.9.1.tar", last modified: Tue Nov 30 12:54:47 2021, max compression
```

## Comparing `EXtra-data-1.9.0.tar` & `EXtra-data-1.9.1.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.846306 EXtra-data-1.9.0/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       55 2020-06-02 12:57:21.000000 EXtra-data-1.9.0/.coveragerc
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.783298 EXtra-data-1.9.0/.github/
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.784298 EXtra-data-1.9.0/.github/dependabot/
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      266 2021-11-25 12:54:59.000000 EXtra-data-1.9.0/.github/dependabot/constraints.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      125 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/.github/dependabot.yml
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.784298 EXtra-data-1.9.0/.github/workflows/
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1055 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/.github/workflows/tests.yml
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      134 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/.gitignore
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      244 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/Dockerfile
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.785298 EXtra-data-1.9.0/EXtra_data.egg-info/
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1882 2021-11-25 13:34:24.000000 EXtra-data-1.9.0/EXtra_data.egg-info/PKG-INFO
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3025 2021-11-25 13:34:24.000000 EXtra-data-1.9.0/EXtra_data.egg-info/SOURCES.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)        1 2021-11-25 13:34:24.000000 EXtra-data-1.9.0/EXtra_data.egg-info/dependency_links.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      274 2021-11-25 13:34:24.000000 EXtra-data-1.9.0/EXtra_data.egg-info/entry_points.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      218 2021-11-25 13:34:24.000000 EXtra-data-1.9.0/EXtra_data.egg-info/requires.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       11 2021-11-25 13:34:24.000000 EXtra-data-1.9.0/EXtra_data.egg-info/top_level.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1548 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/LICENSE
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       73 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/MANIFEST.in
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      666 2020-05-27 14:35:09.000000 EXtra-data-1.9.0/Makefile
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1882 2021-11-25 13:34:24.846306 EXtra-data-1.9.0/PKG-INFO
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      978 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/README.md
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       13 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/codecov.yml
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.794299 EXtra-data-1.9.0/docs/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7740 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/Makefile
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.802300 EXtra-data-1.9.0/docs/_static/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/_static/.keep
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    57574 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/_static/agipd_layout.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)   108114 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/_static/agipd_layout.svg
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    46000 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/_static/dssc_hexes.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    31042 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/_static/dssc_hexes.svg
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    46070 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/_static/dssc_layout.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    75907 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/_static/dssc_layout.svg
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    54105 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/_static/lpd_layout.png
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    82299 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/_static/lpd_layout.svg
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1585 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/docs/agipd_lpd_data.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    29319 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/docs/aligning_trains.ipynb
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2760 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/docs/architecture.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    14659 2021-11-25 13:32:37.000000 EXtra-data-1.9.0/docs/changelog.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4218 2021-11-25 13:32:37.000000 EXtra-data-1.9.0/docs/cli.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9809 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/conf.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    23242 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/docs/dask_averaging.ipynb
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5105 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/data_format.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2577 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/design.org
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2392 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/docs/index.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8368 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/docs/inspection.ipynb
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8911 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/iterate_trains.ipynb
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10037 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/docs/lpd_data.ipynb
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7291 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/make.bat
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    13501 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/docs/parallel_example.ipynb
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2385 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/docs/performance.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    14095 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/docs/reading_files.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1418 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/docs/streaming.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1231 2021-11-25 13:32:37.000000 EXtra-data-1.9.0/docs/validation.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)   163973 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/docs/xpd_examples.ipynb
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)   250879 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/docs/xpd_examples2.ipynb
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.816302 EXtra-data-1.9.0/extra_data/
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2067 2021-11-25 13:32:13.000000 EXtra-data-1.9.0/extra_data/__init__.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.817302 EXtra-data-1.9.0/extra_data/cli/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       41 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/cli/__init__.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4304 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/cli/make_virtual_cxi.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1923 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/cli/serve_files.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    56023 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/components.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1515 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/exceptions.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     5841 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/export.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16067 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/file_access.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16354 2021-11-25 12:54:09.000000 EXtra-data-1.9.0/extra_data/keydata.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4020 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/extra_data/locality.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6172 2021-08-06 13:02:36.000000 EXtra-data-1.9.0/extra_data/lsxfel.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8259 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/read_machinery.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    57516 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/reader.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     7637 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/extra_data/run_files_map.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3063 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/sourcedata.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8803 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/stacking.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.830304 EXtra-data-1.9.0/extra_data/tests/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/__init__.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.830304 EXtra-data-1.9.0/extra_data/tests/cli/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/cli/__init__.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      814 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/tests/cli/test_make_virtual_cxi.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3772 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/tests/conftest.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16400 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/tests/make_examples.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.844306 EXtra-data-1.9.0/extra_data/tests/mockdata/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       31 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2005 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/adc.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8133 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/base.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1576 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/basler_camera.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      814 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/control_common.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1881 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/dctrl.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6120 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/detectors.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1049 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/gauge.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2092 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/gec_camera.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4120 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/imgfel.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2554 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/jungfrau.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      778 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/mkfile.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4952 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/motor.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4662 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/mpod.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1046 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/sidemic_camera.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1062 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/tsens.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      645 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/uvlamp.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2009 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/mockdata/xgm.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10822 2021-08-06 13:02:36.000000 EXtra-data-1.9.0/extra_data/tests/test_bad_trains.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    19157 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/tests/test_components.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8097 2021-11-25 12:54:09.000000 EXtra-data-1.9.0/extra_data/tests/test_keydata.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      399 2021-08-06 13:02:36.000000 EXtra-data-1.9.0/extra_data/tests/test_lsxfel.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1924 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/test_open_file_limiter.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      430 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/test_read_machinery.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    31355 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/tests/test_reader_mockdata.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2677 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/extra_data/tests/test_run_files_map.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      511 2020-10-15 10:17:11.000000 EXtra-data-1.9.0/extra_data/tests/test_slice_objs.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1230 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/tests/test_sourcedata.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6148 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/extra_data/tests/test_stacking.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3044 2021-06-14 13:42:12.000000 EXtra-data-1.9.0/extra_data/tests/test_streamer.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      517 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/tests/test_utils.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6763 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/tests/test_validation.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1987 2021-08-06 13:02:36.000000 EXtra-data-1.9.0/extra_data/tests/test_writer.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3368 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/utils.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    12133 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/extra_data/validation.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16726 2021-11-02 17:59:24.000000 EXtra-data-1.9.0/extra_data/write_cxi.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8111 2021-08-06 13:02:36.000000 EXtra-data-1.9.0/extra_data/writer.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      260 2021-11-24 09:44:06.000000 EXtra-data-1.9.0/pytest.ini
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       82 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/readthedocs.yml
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       38 2021-11-25 13:34:24.846306 EXtra-data-1.9.0/setup.cfg
--rwxrwxr-x   0 takluyver  (1000) takluyver  (1000)     2759 2021-11-25 13:32:37.000000 EXtra-data-1.9.0/setup.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-25 13:34:24.845306 EXtra-data-1.9.0/timing/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      506 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/timing/dataframe.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1406 2020-03-22 13:20:16.000000 EXtra-data-1.9.0/timing/iteration.py
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.891432 EXtra-data-1.9.1/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       55 2020-06-02 12:57:21.000000 EXtra-data-1.9.1/.coveragerc
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.852431 EXtra-data-1.9.1/.github/
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.852431 EXtra-data-1.9.1/.github/dependabot/
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      282 2021-11-30 10:03:31.000000 EXtra-data-1.9.1/.github/dependabot/constraints.txt
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      125 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/.github/dependabot.yml
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.852431 EXtra-data-1.9.1/.github/workflows/
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1055 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/.github/workflows/tests.yml
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      134 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/.gitignore
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      244 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/Dockerfile
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.853431 EXtra-data-1.9.1/EXtra_data.egg-info/
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1882 2021-11-30 12:54:47.000000 EXtra-data-1.9.1/EXtra_data.egg-info/PKG-INFO
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3025 2021-11-30 12:54:47.000000 EXtra-data-1.9.1/EXtra_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)        1 2021-11-30 12:54:47.000000 EXtra-data-1.9.1/EXtra_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      274 2021-11-30 12:54:47.000000 EXtra-data-1.9.1/EXtra_data.egg-info/entry_points.txt
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      218 2021-11-30 12:54:47.000000 EXtra-data-1.9.1/EXtra_data.egg-info/requires.txt
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       11 2021-11-30 12:54:47.000000 EXtra-data-1.9.1/EXtra_data.egg-info/top_level.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1548 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/LICENSE
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       73 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/MANIFEST.in
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      666 2020-05-27 14:35:09.000000 EXtra-data-1.9.1/Makefile
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1882 2021-11-30 12:54:47.890432 EXtra-data-1.9.1/PKG-INFO
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      978 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/README.md
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       13 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/codecov.yml
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.861431 EXtra-data-1.9.1/docs/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7740 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/Makefile
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.868431 EXtra-data-1.9.1/docs/_static/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/_static/.keep
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    57574 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/_static/agipd_layout.png
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)   108114 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/_static/agipd_layout.svg
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    46000 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/_static/dssc_hexes.png
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    31042 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/_static/dssc_hexes.svg
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    46070 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/_static/dssc_layout.png
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    75907 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/_static/dssc_layout.svg
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    54105 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/_static/lpd_layout.png
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    82299 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/_static/lpd_layout.svg
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1585 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/docs/agipd_lpd_data.rst
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    29319 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/docs/aligning_trains.ipynb
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2760 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/docs/architecture.rst
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    14835 2021-11-30 12:49:26.000000 EXtra-data-1.9.1/docs/changelog.rst
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4218 2021-11-25 13:32:37.000000 EXtra-data-1.9.1/docs/cli.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9809 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/conf.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    23242 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/docs/dask_averaging.ipynb
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5105 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/data_format.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2577 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/design.org
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2392 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/docs/index.rst
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8368 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/docs/inspection.ipynb
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8911 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/iterate_trains.ipynb
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10037 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/docs/lpd_data.ipynb
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7291 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/make.bat
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    13501 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/docs/parallel_example.ipynb
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2385 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/docs/performance.rst
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    14095 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/docs/reading_files.rst
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1418 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/docs/streaming.rst
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1231 2021-11-25 13:32:37.000000 EXtra-data-1.9.1/docs/validation.rst
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)   163973 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/docs/xpd_examples.ipynb
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)   250879 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/docs/xpd_examples2.ipynb
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.877431 EXtra-data-1.9.1/extra_data/
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2067 2021-11-30 12:51:56.000000 EXtra-data-1.9.1/extra_data/__init__.py
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.878432 EXtra-data-1.9.1/extra_data/cli/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       41 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/cli/__init__.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4304 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/cli/make_virtual_cxi.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1923 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/cli/serve_files.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    56023 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/components.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1515 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/exceptions.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     5841 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/export.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16067 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/file_access.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16500 2021-11-30 10:03:31.000000 EXtra-data-1.9.1/extra_data/keydata.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4020 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/extra_data/locality.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6172 2021-08-06 13:02:36.000000 EXtra-data-1.9.1/extra_data/lsxfel.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8259 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/read_machinery.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    57516 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/reader.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     7637 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/extra_data/run_files_map.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3063 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/sourcedata.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8803 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/stacking.py
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.884432 EXtra-data-1.9.1/extra_data/tests/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/__init__.py
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.884432 EXtra-data-1.9.1/extra_data/tests/cli/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/cli/__init__.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      814 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/tests/cli/test_make_virtual_cxi.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3772 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/tests/conftest.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16400 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/tests/make_examples.py
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.889432 EXtra-data-1.9.1/extra_data/tests/mockdata/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       31 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2005 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/adc.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8133 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/base.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1576 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/basler_camera.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      814 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/control_common.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1881 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/dctrl.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6120 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/detectors.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1049 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/gauge.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2092 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/gec_camera.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4120 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/imgfel.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2554 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/jungfrau.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      778 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/mkfile.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4952 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/motor.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4662 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/mpod.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1046 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/sidemic_camera.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1062 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/tsens.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      645 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/uvlamp.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2009 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/mockdata/xgm.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10822 2021-08-06 13:02:36.000000 EXtra-data-1.9.1/extra_data/tests/test_bad_trains.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    19157 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/tests/test_components.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     9415 2021-11-30 10:03:31.000000 EXtra-data-1.9.1/extra_data/tests/test_keydata.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      399 2021-08-06 13:02:36.000000 EXtra-data-1.9.1/extra_data/tests/test_lsxfel.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1924 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/test_open_file_limiter.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      430 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/test_read_machinery.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    31355 2021-11-30 12:49:18.000000 EXtra-data-1.9.1/extra_data/tests/test_reader_mockdata.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2677 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/extra_data/tests/test_run_files_map.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      511 2020-10-15 10:17:11.000000 EXtra-data-1.9.1/extra_data/tests/test_slice_objs.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1230 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/tests/test_sourcedata.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6148 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/extra_data/tests/test_stacking.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3044 2021-06-14 13:42:12.000000 EXtra-data-1.9.1/extra_data/tests/test_streamer.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      517 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/tests/test_utils.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6763 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/tests/test_validation.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1987 2021-08-06 13:02:36.000000 EXtra-data-1.9.1/extra_data/tests/test_writer.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3368 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/utils.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    12133 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/extra_data/validation.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16726 2021-11-02 17:59:24.000000 EXtra-data-1.9.1/extra_data/write_cxi.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8111 2021-08-06 13:02:36.000000 EXtra-data-1.9.1/extra_data/writer.py
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      260 2021-11-24 09:44:06.000000 EXtra-data-1.9.1/pytest.ini
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       82 2021-11-29 15:34:16.000000 EXtra-data-1.9.1/readthedocs.yml
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       38 2021-11-30 12:54:47.891432 EXtra-data-1.9.1/setup.cfg
+-rwxrwxr-x   0 takluyver  (1000) takluyver  (1000)     2759 2021-11-25 13:32:37.000000 EXtra-data-1.9.1/setup.py
+drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2021-11-30 12:54:47.890432 EXtra-data-1.9.1/timing/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      506 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/timing/dataframe.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1406 2020-03-22 13:20:16.000000 EXtra-data-1.9.1/timing/iteration.py
```

### Comparing `EXtra-data-1.9.0/.github/workflows/tests.yml` & `EXtra-data-1.9.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/EXtra_data.egg-info/PKG-INFO` & `EXtra-data-1.9.1/EXtra_data.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EXtra-data
-Version: 1.9.0
+Version: 1.9.1
 Summary: Tools to read and analyse data from European XFEL 
 Home-page: https://github.com/European-XFEL/EXtra-data
 Author: European XFEL GmbH
 Author-email: da-support@xfel.eu
 Maintainer: Thomas Michelat
 License: BSD-3-Clause
 Platform: UNKNOWN
```

### Comparing `EXtra-data-1.9.0/EXtra_data.egg-info/SOURCES.txt` & `EXtra-data-1.9.1/EXtra_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/LICENSE` & `EXtra-data-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/Makefile` & `EXtra-data-1.9.1/Makefile`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/PKG-INFO` & `EXtra-data-1.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EXtra-data
-Version: 1.9.0
+Version: 1.9.1
 Summary: Tools to read and analyse data from European XFEL 
 Home-page: https://github.com/European-XFEL/EXtra-data
 Author: European XFEL GmbH
 Author-email: da-support@xfel.eu
 Maintainer: Thomas Michelat
 License: BSD-3-Clause
 Platform: UNKNOWN
```

### Comparing `EXtra-data-1.9.0/README.md` & `EXtra-data-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/Makefile` & `EXtra-data-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/_static/agipd_layout.png` & `EXtra-data-1.9.1/docs/_static/agipd_layout.png`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/_static/agipd_layout.svg` & `EXtra-data-1.9.1/docs/_static/agipd_layout.svg`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/_static/dssc_hexes.png` & `EXtra-data-1.9.1/docs/_static/dssc_hexes.png`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/_static/dssc_hexes.svg` & `EXtra-data-1.9.1/docs/_static/dssc_hexes.svg`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/_static/dssc_layout.png` & `EXtra-data-1.9.1/docs/_static/dssc_layout.png`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/_static/dssc_layout.svg` & `EXtra-data-1.9.1/docs/_static/dssc_layout.svg`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/_static/lpd_layout.png` & `EXtra-data-1.9.1/docs/_static/lpd_layout.png`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/_static/lpd_layout.svg` & `EXtra-data-1.9.1/docs/_static/lpd_layout.svg`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/agipd_lpd_data.rst` & `EXtra-data-1.9.1/docs/agipd_lpd_data.rst`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/aligning_trains.ipynb` & `EXtra-data-1.9.1/docs/aligning_trains.ipynb`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/architecture.rst` & `EXtra-data-1.9.1/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/changelog.rst` & `EXtra-data-1.9.1/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Release Notes
 =============
 
+1.9.1
+-----
+
+- Fix errors from :meth:`~.KeyData.data_counts` and
+  :meth:`~.KeyData.drop_empty_trains` when different train IDs exist for
+  different sources (:ghpull:`257`).
+
 1.9
 ---
 
 - New :meth:`.KeyData.as_single_value` method to check that a key remains
   constant (within a specified tolerance) through the data, and return it as
   a single value (:ghpull:`228`).
 - New :meth:`.KeyData.train_id_coordinates` method to get train IDs associated
```

### Comparing `EXtra-data-1.9.0/docs/cli.rst` & `EXtra-data-1.9.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/conf.py` & `EXtra-data-1.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/dask_averaging.ipynb` & `EXtra-data-1.9.1/docs/dask_averaging.ipynb`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/data_format.rst` & `EXtra-data-1.9.1/docs/data_format.rst`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/design.org` & `EXtra-data-1.9.1/docs/design.org`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/index.rst` & `EXtra-data-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/inspection.ipynb` & `EXtra-data-1.9.1/docs/inspection.ipynb`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/iterate_trains.ipynb` & `EXtra-data-1.9.1/docs/iterate_trains.ipynb`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/lpd_data.ipynb` & `EXtra-data-1.9.1/docs/lpd_data.ipynb`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/make.bat` & `EXtra-data-1.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/parallel_example.ipynb` & `EXtra-data-1.9.1/docs/parallel_example.ipynb`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/performance.rst` & `EXtra-data-1.9.1/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/reading_files.rst` & `EXtra-data-1.9.1/docs/reading_files.rst`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/streaming.rst` & `EXtra-data-1.9.1/docs/streaming.rst`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/validation.rst` & `EXtra-data-1.9.1/docs/validation.rst`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/xpd_examples.ipynb` & `EXtra-data-1.9.1/docs/xpd_examples.ipynb`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/docs/xpd_examples2.ipynb` & `EXtra-data-1.9.1/docs/xpd_examples2.ipynb`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/__init__.py` & `EXtra-data-1.9.1/extra_data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 You should have received a copy of the 3-Clause BSD License along with this
 program. If not, see <https://opensource.org/licenses/BSD-3-Clause>
 """
 
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 
 from .exceptions import (
     SourceNameError, PropertyNameError, TrainIDError, MultiRunError
 )
 from .keydata import KeyData
 from .reader import *
```

### Comparing `EXtra-data-1.9.0/extra_data/cli/make_virtual_cxi.py` & `EXtra-data-1.9.1/extra_data/cli/make_virtual_cxi.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/cli/serve_files.py` & `EXtra-data-1.9.1/extra_data/cli/serve_files.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/components.py` & `EXtra-data-1.9.1/extra_data/components.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/exceptions.py` & `EXtra-data-1.9.1/extra_data/exceptions.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/export.py` & `EXtra-data-1.9.1/extra_data/export.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/file_access.py` & `EXtra-data-1.9.1/extra_data/file_access.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/keydata.py` & `EXtra-data-1.9.1/extra_data/keydata.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,21 +160,24 @@
         else:
             train_ids = counts = np.zeros(0, dtype=np.uint64)
 
         if labelled:
             import pandas as pd
             return pd.Series(counts, index=train_ids)
         else:
-            # self.train_ids is always sorted. The train IDs from chunks
-            # should be in order, but sometimes trains are written out of order.
-            # Reorder the counts to match self.train_ids.
-            assert len(train_ids) == len(self.train_ids)
+            # We may be missing some train IDs, if they're not in any file
+            # for this source, and they're sometimes out of order within chunks
+            # (they shouldn't be, but we try not to fail too badly if they are).
             assert np.isin(train_ids, self.train_ids).all()
-            idxs = np.argsort(train_ids)
-            return counts[idxs]
+            tid_to_ix = {t: i for (i, t) in enumerate(self.train_ids)}
+            res = np.zeros(len(self.train_ids), dtype=np.uint64)
+            for tid, ct in zip(train_ids, counts):
+                res[tid_to_ix[tid]] = ct
+
+            return res
 
     def as_single_value(self, rtol=1e-5, atol=0.0, reduce_by='median'):
         """Retrieve a single reduced value if within tolerances.
 
         The relative and absolute tolerances *rtol* and *atol* work the
         same way as in ``numpy.allclose``. The default relative tolerance
         is 1e-5 with no absolute tolerance. The data for this key is compared
```

### Comparing `EXtra-data-1.9.0/extra_data/locality.py` & `EXtra-data-1.9.1/extra_data/locality.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/lsxfel.py` & `EXtra-data-1.9.1/extra_data/lsxfel.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/read_machinery.py` & `EXtra-data-1.9.1/extra_data/read_machinery.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/reader.py` & `EXtra-data-1.9.1/extra_data/reader.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/run_files_map.py` & `EXtra-data-1.9.1/extra_data/run_files_map.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/sourcedata.py` & `EXtra-data-1.9.1/extra_data/sourcedata.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/stacking.py` & `EXtra-data-1.9.1/extra_data/stacking.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/cli/test_make_virtual_cxi.py` & `EXtra-data-1.9.1/extra_data/tests/cli/test_make_virtual_cxi.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/conftest.py` & `EXtra-data-1.9.1/extra_data/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/make_examples.py` & `EXtra-data-1.9.1/extra_data/tests/make_examples.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/adc.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/adc.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/base.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/base.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/basler_camera.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/basler_camera.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/control_common.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/control_common.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/dctrl.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/dctrl.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/detectors.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/detectors.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/gauge.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/gauge.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/gec_camera.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/gec_camera.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/imgfel.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/imgfel.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/jungfrau.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/jungfrau.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/mkfile.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/mkfile.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/motor.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/motor.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/mpod.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/mpod.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/sidemic_camera.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/sidemic_camera.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/tsens.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/tsens.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/uvlamp.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/uvlamp.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/mockdata/xgm.py` & `EXtra-data-1.9.1/extra_data/tests/mockdata/xgm.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_bad_trains.py` & `EXtra-data-1.9.1/extra_data/tests/test_bad_trains.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_components.py` & `EXtra-data-1.9.1/extra_data/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_keydata.py` & `EXtra-data-1.9.1/extra_data/tests/test_keydata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import os
 import numpy as np
 import pytest
 
+import h5py
+
 from extra_data import RunDirectory, H5File
 from extra_data.exceptions import TrainIDError, NoDataError
+from . import make_examples
 from .mockdata import write_file
 from .mockdata.xgm import XGM
 
 def test_get_keydata(mock_spb_raw_run):
     run = RunDirectory(mock_spb_raw_run)
     print(run.instrument_sources)
     am0 = run['SPB_DET_AGIPD1M-1/DET/0CH0:xtdf', 'image.data']
@@ -142,14 +145,54 @@
 
     count_none_ser = cam_nodata.drop_empty_trains().data_counts(labelled=True)
     assert len(count_none_ser) == 0
 
     count_none_arr = cam_nodata.drop_empty_trains().data_counts(labelled=False)
     assert len(count_none_arr) == 0
 
+
+@pytest.fixture()
+def fxe_run_module_offset(tmp_path):
+    run_dir = tmp_path / 'fxe-run-mod-offset'
+    run_dir.mkdir()
+    make_examples.make_fxe_run(run_dir, format_version='1.0')
+
+    # Shift the train IDs for a module by 1, so it has data for a different set
+    # of train IDs to other sources.
+    with h5py.File(run_dir / 'RAW-R0450-LPD08-S00000.h5', 'r+') as f:
+        tids_dset = f['INDEX/trainId']
+        tids_dset[:] = tids_dset[:] + 1
+
+    return run_dir
+
+
+def test_data_counts_missing_train(fxe_run_module_offset):
+    run = RunDirectory(fxe_run_module_offset)
+    assert len(run.train_ids) == 481
+    lpd_m8 = run['FXE_DET_LPD1M-1/DET/8CH0:xtdf', 'image.cellId']
+
+    ser = lpd_m8.data_counts(labelled=True)
+    assert len(ser) == 480
+    np.testing.assert_array_equal(ser.index, run.train_ids[1:])
+
+    arr = lpd_m8.data_counts(labelled=False)
+    assert len(arr) == 481
+    assert arr[0] == 0
+    np.testing.assert_array_equal(arr[1:], 128)
+
+    lpd_m8_w_data = lpd_m8.drop_empty_trains()
+    ser = lpd_m8_w_data.data_counts(labelled=True)
+    assert len(ser) == 480
+    np.testing.assert_array_equal(ser.index, run.train_ids[1:])
+
+    arr = lpd_m8_w_data.data_counts(labelled=False)
+    assert len(arr) == 480
+    np.testing.assert_array_equal(arr, 128)
+
+
 def test_select_by(mock_spb_raw_run):
     run = RunDirectory(mock_spb_raw_run)
     am0 = run['SPB_DET_AGIPD1M-1/DET/0CH0:xtdf', 'image.data']
 
     subrun = run.select(am0)
     assert subrun.all_sources == {am0.source}
     assert subrun.keys_for_source(am0.source) == {am0.key}
```

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_open_file_limiter.py` & `EXtra-data-1.9.1/extra_data/tests/test_open_file_limiter.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_reader_mockdata.py` & `EXtra-data-1.9.1/extra_data/tests/test_reader_mockdata.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_run_files_map.py` & `EXtra-data-1.9.1/extra_data/tests/test_run_files_map.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_sourcedata.py` & `EXtra-data-1.9.1/extra_data/tests/test_sourcedata.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_stacking.py` & `EXtra-data-1.9.1/extra_data/tests/test_stacking.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_streamer.py` & `EXtra-data-1.9.1/extra_data/tests/test_streamer.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_utils.py` & `EXtra-data-1.9.1/extra_data/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_validation.py` & `EXtra-data-1.9.1/extra_data/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/tests/test_writer.py` & `EXtra-data-1.9.1/extra_data/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/utils.py` & `EXtra-data-1.9.1/extra_data/utils.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/validation.py` & `EXtra-data-1.9.1/extra_data/validation.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/write_cxi.py` & `EXtra-data-1.9.1/extra_data/write_cxi.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/extra_data/writer.py` & `EXtra-data-1.9.1/extra_data/writer.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/setup.py` & `EXtra-data-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `EXtra-data-1.9.0/timing/iteration.py` & `EXtra-data-1.9.1/timing/iteration.py`

 * *Files identical despite different names*

