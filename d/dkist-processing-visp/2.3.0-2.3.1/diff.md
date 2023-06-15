# Comparing `tmp/dkist_processing_visp-2.3.0.tar.gz` & `tmp/dkist_processing_visp-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.3.0.tar", last modified: Wed May 17 21:48:06 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.3.1.tar", last modified: Thu Jun 15 16:50:48 2023, max compression
```

## Comparing `dkist_processing_visp-2.3.0.tar` & `dkist_processing_visp-2.3.1.tar`

### file list

```diff
@@ -1,110 +1,109 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.659523 dkist_processing_visp-2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    20545 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-05-17 21:48:06.659523 dkist_processing_visp-2.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3428 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.651523 dkist_processing_visp-2.3.0/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.651523 dkist_processing_visp-2.3.0/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.651523 dkist_processing_visp-2.3.0/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.651523 dkist_processing_visp-2.3.0/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    11585 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.655523 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.655523 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    14365 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    40378 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    20011 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5343 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.655523 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5656 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/downsample.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10422 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4604 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28173 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    27922 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6846 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.659523 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16389 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6595 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/e2e_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    17553 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/e2e_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    18443 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_downsample.py
--rw-rw-rw-   0 root         (0) root         (0)    14009 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    12613 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5651 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11818 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    16234 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5097 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.659523 dkist_processing_visp-2.3.0/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/dkist_processing_visp/workflows/single_task_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.651523 dkist_processing_visp-2.3.0/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-05-17 21:48:06.000000 dkist_processing_visp-2.3.0/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3620 2023-05-17 21:48:06.000000 dkist_processing_visp-2.3.0/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-17 21:48:06.000000 dkist_processing_visp-2.3.0/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-05-17 21:48:06.000000 dkist_processing_visp-2.3.0/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-17 21:48:06.000000 dkist_processing_visp-2.3.0/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.659523 dkist_processing_visp-2.3.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6427 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/gain_correction.rst
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/polarization_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/science_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/docs/scientific_changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     5761 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/init_guess.dat
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-17 21:48:06.659523 dkist_processing_visp-2.3.0/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1705 2023-05-17 21:48:06.663523 dkist_processing_visp-2.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-05-17 21:47:59.000000 dkist_processing_visp-2.3.0/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    20825 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.501040 dkist_processing_visp-2.3.1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.501040 dkist_processing_visp-2.3.1/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.501040 dkist_processing_visp-2.3.1/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.505040 dkist_processing_visp-2.3.1/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    11306 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.505040 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.505040 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14365 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    40623 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    20011 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5343 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.505040 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5656 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10422 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4604 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28173 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    27922 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6846 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.509040 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16332 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6595 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/e2e_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    17553 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/e2e_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    18443 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    14009 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    12613 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11818 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    16234 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9883 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5097 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.509040 dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/single_task_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.501040 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-15 16:50:48.000000 dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1705 2023-06-15 16:50:48.513040 dkist_processing_visp-2.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-06-15 16:50:42.000000 dkist_processing_visp-2.3.1/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.3.0/.gitignore` & `dkist_processing_visp-2.3.1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 
 # Pyre type checker
 .pyre/
 
 
 # other
 *.fits
+*.dat
 .tox
 .*.sw[op]
 *~
 
 # Ignore .c files by default to avoid including generated code. If you want to
 # add a non-generated .c extension, use `git add -f filename.c`.
 *.c
```

### Comparing `dkist_processing_visp-2.3.0/.pre-commit-config.yaml` & `dkist_processing_visp-2.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/CHANGELOG.rst` & `dkist_processing_visp-2.3.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.3.1 (2023-06-15)
+===================
+
+Bugfixes
+--------
+
+- Fix failure in Geometric task that happened when some modstates had a a different number of identified hairline regions than others. (`#118 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/118>`__)
+
+
 v2.3.0 (2023-05-17)
 ===================
 
 Misc
 ----
 
 - Bumping common to 2.7.0: ParseL0InputData --> ParseL0InputDataBase, constant_flowers --> constant_buds (`#115 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/115>`__)
```

### Comparing `dkist_processing_visp-2.3.0/PKG-INFO` & `dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dkist_processing_visp
-Version: 2.3.0
+Name: dkist-processing-visp
+Version: 2.3.1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.3.0/README.rst` & `dkist_processing_visp-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/SCIENCE_CHANGELOG.rst` & `dkist_processing_visp-2.3.1/SCIENCE_CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/bitbucket-pipelines.yml` & `dkist_processing_visp-2.3.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/check_changelog_updated.sh` & `dkist_processing_visp-2.3.1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.3.1/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/models/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,19 +115,14 @@
         """Plus/minus number of standard deviations away from the median used to clip bad hairline center fits.
 
         Clipping deviant values can greatly improve the fit to the slope and thus the beam angle.
         """
         return self._find_most_recent_past_value("visp_geo_hairline_angle_fit_sig_clip")
 
     @property
-    def geo_hairline_angle_fit_min_samples(self) -> float:
-        """Return fractional number of samples required for the RANSAC regressor used to fit hairline angles."""
-        return self._find_most_recent_past_value("visp_geo_hairline_angle_fit_min_samples")
-
-    @property
     def geo_max_beam_2_angle_refinement(self) -> float:
         """Maximum allowable refinement to the beam 2 spectral tilt angle, in radians."""
         return self._find_most_recent_past_value("visp_geo_max_beam_2_angle_refinement")
 
     @property
     def geo_upsample_factor(self):
         """Pixel precision (1/upsample_factor) to use during phase matching of beam/modulator images."""
```

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/time.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/geometric.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,19 @@
         angle_list = []
         for modstate in range(1, self.constants.num_modstates + 1):
             data = self.basic_corrected_lamp_data(beam=beam, modstate=modstate)
             angle = self._compute_single_modstate_angles(data)
             logger.info(f"Angles for {beam = } and {modstate = } = {np.rad2deg(angle)} deg")
             angle_list.append(angle)
 
-        theta = float(np.nanmedian(angle_list))
+        # Flatten the list just in case we got different numbers of hairline regions for the different modstates
+        # (which can happen in data with strong higher-order hairline leaks).
+        flat_angle_list = np.hstack(angle_list)
+
+        theta = float(np.nanmedian(flat_angle_list))
         logger.info(f"Beam angle for {beam = }: {np.rad2deg(theta):0.4f} deg")
         return theta
 
     def _identify_hairlines_and_bad_pixels(
         self, input_array: np.ndarray
     ) -> tuple[np.ndarray, np.ndarray]:
         """
```

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/downsample.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,15 +375,14 @@
     visp_hairline_fraction: float = 0.11
     visp_hairline_mask_spatial_smoothing_width_px: float = 1.0
     visp_hairline_mask_gaussian_peak_cutoff_fraction: float = 0.02
     visp_geo_binary_opening_diameter: int = 21
     visp_geo_hairline_flat_id_threshold: float = 0.9
     visp_geo_hairline_fit_width_px: int = 10
     visp_geo_hairline_angle_fit_sig_clip: float = 3.0
-    visp_geo_hairline_angle_fit_min_samples: float = 0.9
     visp_geo_max_beam_2_angle_refinement: float = np.deg2rad(0.1)
     visp_geo_upsample_factor: float = 10.0
     visp_geo_max_shift: float = 40.0
     visp_geo_poly_fit_order: int = 3
     visp_solar_spectral_avg_window: WavelengthParameter = WavelengthParameter(
         values=(800, 800, 800, 800)
     )
```

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/e2e_helpers.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/e2e_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/e2e_test.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/e2e_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_downsample.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.3.1/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dkist-processing-visp
-Version: 2.3.0
+Name: dkist_processing_visp
+Version: 2.3.1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .pre-commit-config.yaml
 .readthedocs.yml
 CHANGELOG.rst
 README.rst
 SCIENCE_CHANGELOG.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
-init_guess.dat
 pyproject.toml
 science_towncrier.sh
 setup.cfg
 setup.py
 towncrier_science.toml
 changelog/.gitempty
 dkist_processing_visp/__init__.py
```

### Comparing `dkist_processing_visp-2.3.0/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.3.1/dkist_processing_visp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/docs/Makefile` & `dkist_processing_visp-2.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/docs/background_light.rst` & `dkist_processing_visp-2.3.1/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/docs/conf.py` & `dkist_processing_visp-2.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/docs/gain_correction.rst` & `dkist_processing_visp-2.3.1/docs/gain_correction.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.3.1/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/docs/make.bat` & `dkist_processing_visp-2.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/docs/polarization_calibration.rst` & `dkist_processing_visp-2.3.1/docs/polarization_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/docs/science_calibration.rst` & `dkist_processing_visp-2.3.1/docs/science_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/licenses/LICENSE.rst` & `dkist_processing_visp-2.3.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/pyproject.toml` & `dkist_processing_visp-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.3.0/setup.cfg` & `dkist_processing_visp-2.3.1/setup.cfg`

 * *Files identical despite different names*

