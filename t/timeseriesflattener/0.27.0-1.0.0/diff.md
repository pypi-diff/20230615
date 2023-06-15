# Comparing `tmp/timeseriesflattener-0.27.0.tar.gz` & `tmp/timeseriesflattener-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-0.27.0.tar", last modified: Fri May 19 14:48:01 2023, max compression
+gzip compressed data, was "timeseriesflattener-1.0.0.tar", last modified: Thu Jun 15 09:31:15 2023, max compression
```

## Comparing `timeseriesflattener-0.27.0.tar` & `timeseriesflattener-1.0.0.tar`

### file list

```diff
@@ -1,130 +1,133 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.771905 timeseriesflattener-0.27.0/
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.cruft.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.731904 timeseriesflattener-0.27.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.719903 timeseriesflattener-0.27.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.731904 timeseriesflattener-0.27.0/.github/actions/test/
--rw-r--r--   0 root         (0) root         (0)      896 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/actions/test/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.731904 timeseriesflattener-0.27.0/.github/actions/test_tutorials/
--rw-r--r--   0 root         (0) root         (0)      994 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 root         (0) root         (0)      529 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/dependabot.yml
--rw-r--r--   0 root         (0) root         (0)      252 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/pull_request_template.md
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/recommended_repo_setup.md
--rw-r--r--   0 root         (0) root         (0)      465 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/setup_ci.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.735904 timeseriesflattener-0.27.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 root         (0) root         (0)     2083 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/cruft.yml
--rw-r--r--   0 root         (0) root         (0)      849 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 root         (0) root         (0)      877 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/documentation.yml
--rw-r--r--   0 root         (0) root         (0)      727 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 root         (0) root         (0)     2446 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 root         (0) root         (0)     2891 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 root         (0) root         (0)     1132 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/stalebot.yml
--rw-r--r--   0 root         (0) root         (0)     3056 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.github/workflows/static_type_checks.yml
--rw-r--r--   0 root         (0) root         (0)     2871 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      644 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1286 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/.zenodo.json
--rw-r--r--   0 root         (0) root         (0)    54804 2023-05-19 14:47:50.000000 timeseriesflattener-0.27.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     5238 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     4474 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1087 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    11584 2023-05-19 14:48:01.771905 timeseriesflattener-0.27.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9185 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/README.md
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/citation.cff
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.739904 timeseriesflattener-0.27.0/docs/
--rw-r--r--   0 root         (0) root         (0)      633 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.739904 timeseriesflattener-0.27.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)    15406 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/_static/favicon.ico
--rw-r--r--   0 root         (0) root         (0)    49714 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/_static/icon.png
--rw-r--r--   0 root         (0) root         (0)    49714 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/_static/icon_dark.png
--rw-r--r--   0 root         (0) root         (0)   811066 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/_static/terminology_figure.png
--rw-r--r--   0 root         (0) root         (0)     4211 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     2097 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)      320 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/feature_specifications.rst
--rw-r--r--   0 root         (0) root         (0)     5280 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      299 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/timeseriesflattener.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.739904 timeseriesflattener-0.27.0/docs/tutorials/
--rw-r--r--   0 root         (0) root         (0)   130849 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 root         (0) root         (0)    68308 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 root         (0) root         (0)    77800 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.743904 timeseriesflattener-0.27.0/docs/tutorials/img/
--rw-r--r--   0 root         (0) root         (0)    78953 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/img/term_a.png
--rw-r--r--   0 root         (0) root         (0)   109486 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/img/term_b.png
--rw-r--r--   0 root         (0) root         (0)   107613 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/img/term_c.png
--rw-r--r--   0 root         (0) root         (0)   250306 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials/img/term_d.png
--rw-r--r--   0 root         (0) root         (0)      370 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/docs/tutorials.rst
--rw-r--r--   0 root         (0) root         (0)    49714 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.743904 timeseriesflattener-0.27.0/paper/
--rw-r--r--   0 root         (0) root         (0)    14392 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/paper/paper.bib
--rw-r--r--   0 root         (0) root         (0)     9344 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/paper/paper.md
--rw-r--r--   0 root         (0) root         (0)     4318 2023-05-19 14:47:50.000000 timeseriesflattener-0.27.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-19 14:48:01.771905 timeseriesflattener-0.27.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.719903 timeseriesflattener-0.27.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.743904 timeseriesflattener-0.27.0/src/timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)      226 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1971 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 root         (0) root         (0)     6145 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
--rw-r--r--   0 root         (0) root         (0)    44130 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/feature_spec_objects.py
--rw-r--r--   0 root         (0) root         (0)    36771 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 root         (0) root         (0)     2234 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/logger.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/resolve_multiple_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/src/timeseriesflattener/testing/
--rw-r--r--   0 root         (0) root         (0)     3168 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/testing/load_synth_data.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     5271 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/testing/utils_for_testing.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/text_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/src/timeseriesflattener/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11584 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3857 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      723 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-19 14:48:01.000000 timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     9179 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.723904 timeseriesflattener-0.27.0/tests/test_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.723904 timeseriesflattener-0.27.0/tests/test_data/flattened/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.747904 timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 root         (0) root         (0)     1477 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 root         (0) root         (0)   864795 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.751904 timeseriesflattener-0.27.0/tests/test_data/models/
--rw-r--r--   0 root         (0) root         (0)     1869 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 root         (0) root         (0)    25543 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 root         (0) root         (0)     1015 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.767905 timeseriesflattener-0.27.0/tests/test_data/raw/
--rw-r--r--   0 root         (0) root         (0)      779 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 root         (0) root         (0)     1003 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_sex.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 root         (0) root         (0)   248865 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 root         (0) root         (0)   268962 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 root         (0) root         (0)   268904 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 root         (0) root         (0)  4316151 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 root         (0) root         (0)  4315816 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 root         (0) root         (0)    68900 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_sex.csv
--rw-r--r--   0 root         (0) root         (0)    84570 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_data/raw/synth_text_data.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.767905 timeseriesflattener-0.27.0/tests/test_feature_cache/
--rw-r--r--   0 root         (0) root         (0)     3490 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.767905 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 root         (0) root         (0)     9272 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 14:48:01.771905 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18335 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 root         (0) root         (0)     2456 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 root         (0) root         (0)     2327 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 root         (0) root         (0)     7995 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 root         (0) root         (0)     2390 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 root         (0) root         (0)    16795 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_resolve_multiple.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-05-19 14:47:49.000000 timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_utils.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.464397 timeseriesflattener-1.0.0/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      489 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.cookiecutter.json
+-rw-r--r--   0 au484925 (903520038) staff       (20)      738 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.cruft.json
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.410705 timeseriesflattener-1.0.0/.github/
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.403811 timeseriesflattener-1.0.0/.github/actions/
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.410959 timeseriesflattener-1.0.0/.github/actions/test/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      892 2023-06-14 14:06:50.000000 timeseriesflattener-1.0.0/.github/actions/test/action.yml
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.411219 timeseriesflattener-1.0.0/.github/actions/test_tutorials/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      948 2023-06-15 08:56:38.000000 timeseriesflattener-1.0.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      529 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/dependabot.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      252 2023-03-01 09:46:41.000000 timeseriesflattener-1.0.0/.github/pull_request_template.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1689 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)      465 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/.github/setup_ci.md
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.413184 timeseriesflattener-1.0.0/.github/workflows/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      720 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2083 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/workflows/cruft.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      849 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      868 2023-06-07 11:02:56.000000 timeseriesflattener-1.0.0/.github/workflows/documentation.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      727 2023-03-23 07:54:31.000000 timeseriesflattener-1.0.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2446 2023-03-23 07:59:10.000000 timeseriesflattener-1.0.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2891 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1132 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     3056 2023-06-14 14:23:53.000000 timeseriesflattener-1.0.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2871 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.gitignore
+-rw-r--r--   0 au484925 (903520038) staff       (20)      644 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1286 2023-03-31 09:12:14.000000 timeseriesflattener-1.0.0/.zenodo.json
+-rw-r--r--   0 au484925 (903520038) staff       (20)    55767 2023-06-15 09:31:08.000000 timeseriesflattener-1.0.0/CHANGELOG.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     5238 2023-03-01 10:46:04.000000 timeseriesflattener-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4474 2023-03-01 11:40:47.000000 timeseriesflattener-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1087 2022-12-06 14:15:36.000000 timeseriesflattener-1.0.0/LICENSE
+-rw-r--r--   0 au484925 (903520038) staff       (20)      262 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/Makefile
+-rw-r--r--   0 au484925 (903520038) staff       (20)    11520 2023-06-15 09:31:15.463864 timeseriesflattener-1.0.0/PKG-INFO
+-rw-r--r--   0 au484925 (903520038) staff       (20)     9122 2023-06-15 08:47:22.000000 timeseriesflattener-1.0.0/README.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)      658 2022-12-06 09:57:22.000000 timeseriesflattener-1.0.0/citation.cff
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.415040 timeseriesflattener-1.0.0/docs/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      633 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/docs/Makefile
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.416482 timeseriesflattener-1.0.0/docs/_static/
+-rw-r--r--   0 au484925 (903520038) staff       (20)    15406 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/_static/favicon.ico
+-rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/_static/icon.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/_static/icon_dark.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)   811066 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4211 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/conf.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2097 2023-04-19 11:55:26.000000 timeseriesflattener-1.0.0/docs/faq.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)      332 2023-06-14 14:10:35.000000 timeseriesflattener-1.0.0/docs/feature_specifications.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)     5280 2023-01-25 13:20:02.000000 timeseriesflattener-1.0.0/docs/index.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)      299 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/installation.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)      312 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/timeseriesflattener.rst
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.421322 timeseriesflattener-1.0.0/docs/tutorials/
+-rw-r--r--   0 au484925 (903520038) staff       (20)   118804 2023-06-15 08:47:23.000000 timeseriesflattener-1.0.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 au484925 (903520038) staff       (20)    50220 2023-06-15 08:47:22.000000 timeseriesflattener-1.0.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 au484925 (903520038) staff       (20)    72388 2023-06-15 08:34:08.000000 timeseriesflattener-1.0.0/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.424123 timeseriesflattener-1.0.0/docs/tutorials/img/
+-rw-r--r--   0 au484925 (903520038) staff       (20)    78953 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)   109486 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)   107613 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)   250306 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)      370 2023-02-23 15:25:24.000000 timeseriesflattener-1.0.0/docs/tutorials.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/icon.png
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.425267 timeseriesflattener-1.0.0/paper/
+-rw-r--r--   0 au484925 (903520038) staff       (20)    14392 2023-03-31 09:12:14.000000 timeseriesflattener-1.0.0/paper/paper.bib
+-rw-r--r--   0 au484925 (903520038) staff       (20)     9344 2023-03-31 09:12:14.000000 timeseriesflattener-1.0.0/paper/paper.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4327 2023-06-15 09:31:08.000000 timeseriesflattener-1.0.0/pyproject.toml
+-rw-r--r--   0 au484925 (903520038) staff       (20)       38 2023-06-15 09:31:15.464448 timeseriesflattener-1.0.0/setup.cfg
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.425526 timeseriesflattener-1.0.0/src/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1996 2023-06-14 14:28:54.000000 timeseriesflattener-1.0.0/src/conftest.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.427953 timeseriesflattener-1.0.0/src/timeseriesflattener/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      309 2023-06-14 08:57:30.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4834 2023-06-15 08:30:34.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/aggregation_fns.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     5559 2023-06-14 12:58:48.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/column_handler.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.429076 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-12-06 12:02:05.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1977 2023-06-14 09:34:12.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     6308 2023-06-15 08:28:24.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.429592 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     7344 2023-06-15 08:34:18.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_specs/group_specs.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     8428 2023-06-15 08:34:18.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_specs/single_specs.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)    36395 2023-06-15 08:30:40.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2271 2023-06-14 09:07:20.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2239 2023-06-14 09:07:20.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/logger.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     7704 2023-06-14 11:44:29.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/misc_utils.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.430337 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     3008 2023-06-14 12:20:04.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.405297 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.405021 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.430851 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1477 2023-03-20 10:36:42.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)   864795 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.433308 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1869 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)    25543 2023-02-23 15:25:24.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1015 2023-02-23 15:25:24.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.453628 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      784 2023-06-14 09:07:20.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1003 2023-03-20 10:36:42.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)      980 2023-06-14 09:07:20.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)      816 2023-03-20 10:36:42.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)   248865 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)   268962 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)   268904 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)  4316151 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)  4315816 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)    68900 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)    84570 2023-02-23 15:25:24.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1392 2023-06-14 12:15:52.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     5179 2023-06-14 13:28:04.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.454465 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/__init__.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.454563 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_feature_cache/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     3425 2023-06-15 08:34:08.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.455393 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)    16237 2023-06-15 08:34:01.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1452 2023-06-14 10:33:38.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2305 2023-06-15 08:34:09.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.462878 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2023-02-07 08:39:43.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)    18309 2023-06-15 08:34:09.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2688 2023-06-15 08:34:11.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2328 2023-06-14 10:33:38.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2319 2023-06-15 08:34:18.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     8190 2023-06-15 08:34:19.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2397 2023-06-14 11:20:11.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2342 2023-06-14 12:24:11.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/text_embedding_functions.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.463210 timeseriesflattener-1.0.0/src/timeseriesflattener/utils/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1065 2023-06-14 13:05:30.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/utils/pydantic_basemodel.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.428600 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 au484925 (903520038) staff       (20)    11520 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4668 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 au484925 (903520038) staff       (20)        1 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 au484925 (903520038) staff       (20)      739 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 au484925 (903520038) staff       (20)       29 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 au484925 (903520038) staff       (20)     9396 2023-06-15 08:57:16.000000 timeseriesflattener-1.0.0/tasks.py
```

### Comparing `timeseriesflattener-0.27.0/.cruft.json` & `timeseriesflattener-1.0.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/actions/test/action.yml` & `timeseriesflattener-1.0.0/.github/actions/test/action.yml`

 * *Files 2% similar despite different names*

```diff
@@ -27,8 +27,8 @@
       shell: bash
       run: |
         pip install invoke tox
 
     - name: Run tests
       shell: bash
       run: |
-        inv test --python-versions=${{ matrix.python-version }} --pytest-args "-n auto"  --pytest-args "--skiphuggingface" --pytest-args "--cov=src" --pytest-args "--cov-report term-missing" --pytest-args="--color=yes"
+        inv test --python-versions=${{ matrix.python-version }} --pytest-args "src/" --pytest-args "--skiphuggingface" --pytest-args "--cov=src" --pytest-args "--cov-report term-missing" --pytest-args="--color=yes"
```

### Comparing `timeseriesflattener-0.27.0/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-1.0.0/.github/actions/test_tutorials/action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     - name: Install jupyter
       shell: bash
       run: |
         pip install jupyter
     - name: Compile notebooks and check for errors
       shell: bash
       run: |
-        jupyter nbconvert --to notebook --execute docs/tutorials/*.ipynb
+        inv test-tutorials
         for notebook in tutorials/*.ipynb; do
           if grep -q "\"cell_type\": \"error\"" $notebook; then
             echo "Error cell found in $notebook"
             exit 1
           fi
         done
```

### Comparing `timeseriesflattener-0.27.0/.github/dependabot.yml` & `timeseriesflattener-1.0.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/recommended_repo_setup.md` & `timeseriesflattener-1.0.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/workflows/check_for_rej.yml` & `timeseriesflattener-1.0.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/workflows/cruft.yml` & `timeseriesflattener-1.0.0/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-1.0.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/workflows/documentation.yml` & `timeseriesflattener-1.0.0/.github/workflows/documentation.yml`

 * *Files 15% similar despite different names*

```diff
@@ -28,9 +28,9 @@
         with:
           documentation_path: docs
 
       - name: Push changes
         if: ${{ github.event_name == 'push' }}
         uses: ad-m/github-push-action@v0.6.0
         with:
-          github_token: ${{ secrets.GITHUB_TOKEN }}
+          github_token: ${{ secrets.PAT }}
           branch: gh-pages
```

### Comparing `timeseriesflattener-0.27.0/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-1.0.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-1.0.0/.github/workflows/main_test_and_release.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/workflows/pre-commit.yml` & `timeseriesflattener-1.0.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/workflows/stalebot.yml` & `timeseriesflattener-1.0.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.github/workflows/static_type_checks.yml` & `timeseriesflattener-1.0.0/.github/workflows/static_type_checks.yml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             .tox
           key: ${{ runner.os }}-${{ matrix.python-version }}
 
       - name: Set up Python
         uses: actions/setup-python@v4
         id: setup_python
         with:
-          python-version: "3.8"
+          python-version: "3.9"
 
       - name: Install dependencies
         shell: bash
         run: |
           pip install invoke tox
 
       - name: Run static type checker
```

### Comparing `timeseriesflattener-0.27.0/.gitignore` & `timeseriesflattener-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.pre-commit-config.yaml` & `timeseriesflattener-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/.zenodo.json` & `timeseriesflattener-1.0.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/CHANGELOG.md` & `timeseriesflattener-1.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,39 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.0 (2023-06-15)
+
+### Feature
+
+* Specs should be pydantic basemodels ([`04781f6`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/04781f6ace79d8abbddaa92ac57a4877be5f9398))
+
+### Fix
+
+* Incorrect type coercion in pydantic ([`e37eefb`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/e37eefb830d77ce46db4e6e18b904556b19ee9df))
+* Types ([`3ed4b59`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/3ed4b59f6b00e062ffeb203fedbdfaac52caf33f))
+* Remove unnecessary feature_name from group specs ([`f29d017`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f29d017938b5a54e336352c043aad14bd9ede61f))
+
+### Documentation
+
+* Update tutorials ([`175de3b`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/175de3b359c411d2acdb71d63226e7d9fd1aad37))
+* Use PAT for docs ([`3500cdf`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/3500cdfdd2878e36c883f49f6ffed63dc9381701))
+
 ## v0.27.0 (2023-05-19)
 ### Feature
 * Add feature_name arg to group specs and make non-optional for non group specs ([`34df7a3`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/34df7a3561206d952cb17474f8c1efa097146e6f))
 
 ## v0.26.0 (2023-05-04)
 ### Feature
 * Add group spec for text predictor spec ([`75a0112`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/75a0112f7c2717d16e1996d5087d993ba7f75cc4))
 
 ### Fix
 * Update type hints ([`887bc06`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/887bc062bf970690077fea105b5ca77018049e6d))
-* Incorrect naming of resolve_multiple_fn ([`0a4607e`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/0a4607ee48e9dd6227205bca09ab123b6d30504a))
+* Incorrect naming of aggregation_fn ([`0a4607e`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/0a4607ee48e9dd6227205bca09ab123b6d30504a))
 
 ## v0.25.1 (2023-05-02)
 ### Fix
 * Bump version to generate new release ([`2316b38`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/2316b388aa71573aceeeba3f899037a93c71cb4f))
 
 ## v0.25.0 (2023-04-26)
 ### Feature
@@ -110,15 +127,15 @@
 * Add sklearn embedding function ([`6c10d3f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/6c10d3f62ae3d57c7302f74dfcbc740aace15131))
 * Add optional loader_kwargs to group specs ([`14b872c`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/14b872cfebd0d5c7917310706f56af0e40ff34f3))
 * Add loader_kwargs to group specs ([`a1e5a14`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/a1e5a14e8a618fece255eb1b5544c1ac1634faf4))
 * Add `embedding_fn_kwargs` to `TextPredictorSpec` ([`7aa48a5`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/7aa48a5285c4ffbb00c36b312f4affa338c11566))
 * Example text embedding functions ([`f4ce9a2`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f4ce9a2e08dfaf93b5cf1fa30e28cdffb2dc1867))
 * Handle text features and features with multiple columns ([`a3cafe9`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/a3cafe9ce1a9aae3db1ae6f7f2b9c394323409d5))
 * TextSpec and option for additional feature name .get_col_str ([`2986203`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/2986203e3d595c5bb387db8feee34bb1fa6a5ddf))
-* Added "concatenate" resolve_multiple_fn ([`5dc8c9f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/5dc8c9f7025099bf0186881af5ecc158af0aadda))
+* Added concatenate aggregation_fn ([`5dc8c9f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/5dc8c9f7025099bf0186881af5ecc158af0aadda))
 
 ### Fix
 * Fix semantic release ([`7e993e3`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/7e993e34c2b670a3239a452703213cd368261d18))
 * Move `embed_text_values` to use timeseriesflattener without text dependencies installed ([`487daec`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/487daec180e1d2d94ba2dcc06b31f35b16ed7e12))
 * Proper guard against neither `df` nor `output_spec` specified in `get_value_col_str_name` ([`aeef039`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/aeef039796bb28eaf6fc35958c12f60f224e82e4))
 * Correct col str name generation for text specs when column names are ints (e.g. HF embeddings) ([`c10565d`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/c10565d1c3589f9b59da270fdd1272661852123a))
 
@@ -235,22 +252,22 @@
 ### Documentation
 * Doc change to run hooks ([`3e4ee58`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/3e4ee58a84af4ae1e74c94878c323bdcfdc0fa51))
 * Adding description ([`dde5111`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/dde5111de21928161af37d5cbd16cd7f7983837a))
 
 ## v0.17.0 (2022-12-08)
 ### Feature
 * More appropriate logging level ([`7122e79`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/7122e79606ec2d2fd5802361ecda8ebde318de12))
-* Infer resolve_multiple_fn str rep for groups ([`8058d65`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/8058d65fdf6e65c534adab87861dcaaeafdd03b8))
-* Infer resolve_multiple_fn str repr from __name__ ([`55be07d`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/55be07df7947b5a7baafafcae7955c4b426a45d0))
+* Infer aggregation_fn str rep for groups ([`8058d65`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/8058d65fdf6e65c534adab87861dcaaeafdd03b8))
+* Infer aggregation_fn str repr from __name__ ([`55be07d`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/55be07df7947b5a7baafafcae7955c4b426a45d0))
 * Add lookahead and lookbehind days to feature group specs ([`318591b`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/318591b7edda233897e11af0a79fdd97a5f12716))
 
 ### Fix
 * Guard against incident attribute not existing ([`3b1329b`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/3b1329b35c11477d09555287a904a9f895e99964))
-* Re-add resolve_multiple str resolution ([`18983a7`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/18983a7988473352f2e994f1ef18ab7e1c8caa80))
-* Only infer resolve_multiple_str if not specified manually ([`f2648f8`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f2648f8afc692812f490e019db0bbb44391d96e2))
+* Re-add aggregation str resolution ([`18983a7`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/18983a7988473352f2e994f1ef18ab7e1c8caa80))
+* Only infer aggregation_str if not specified manually ([`f2648f8`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f2648f8afc692812f490e019db0bbb44391d96e2))
 * Create dir for diskcache if it doesn't exist ([`0e32436`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/0e32436a0c9ee2d59b916158e7f46f0081661fa2))
 * Create dir if it doesn't exist ([`c32f3c7`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/c32f3c702c0d473b59c506cd2e855def65764b24))
 
 ### Documentation
 * Update output ([`a4fa6f7`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/a4fa6f7bf5d9f05d3b6c423f596a5bf102f06e49))
 * Update tutorial based on feedback ([`92c3d3b`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/92c3d3bf5db019a2a3e5bd4ae3182f22cc4bcd38))
 * Add figures to basic tutorial ([`5eb069f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/5eb069f28bde3a4bb951b6d81f86ae80ed9b455f))
@@ -295,15 +312,15 @@
 * Allow either interval_days or lookahead/lookbehind days ([`a270801`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/a2708014eaad78622a5447cf6958f544ad095945))
 
 ### Fix
 * Failing imports after merge ([`dd17771`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/dd177711c8aff74619d962845ab7dd32df00a91b))
 * Unify file naming in cache module ([`f155217`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f155217edc860cbde68e60f6d102dc1fc2191347))
 * Use correct suffix ([`6e737b8`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/6e737b8010c06f62ef320c868fc3821d524ec117))
 * Remove seconds from diskcache to avoid ([`f9ac05c`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f9ac05c46ca13649c248588470f000aa70ec6650))
-* Key_for_resolve_multiple should be optional ([`c569b74`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/c569b749e9c47a60d0e66eae8c0633519ed0e0de))
+* Key_for_aggregation should be optional ([`c569b74`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/c569b749e9c47a60d0e66eae8c0633519ed0e0de))
 
 ### Documentation
 * Add basic tutorial ([`8136a1b`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/8136a1b3db20f30df7898363dfa68e584a6cfe8d))
 
 ## v0.14.0 (2022-12-06)
 ### Feature
 * Add colored logging ([`d230213`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/d230213b0fde3a26329e3c5bab6737ef3391fa09))
@@ -385,15 +402,15 @@
 
 ### Documentation
 * Improve docs ([`9aad0af`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/9aad0af6205af2e3deffb573676af5a20401bae1))
 
 ## v0.7.0 (2022-11-16)
 ### Feature
 * Full run ([`142212f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/142212fc63a59662048b6569dc874def92dfe62f))
-* Rename resolve_multiple registry keys to their previous one ([`3fd3f35`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/3fd3f3566a8a9312ef9a8326a700b162ed9815c3))
+* Rename aggregation registry keys to their previous one ([`3fd3f35`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/3fd3f3566a8a9312ef9a8326a700b162ed9815c3))
 * Reimplement ([`c99585f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/c99585fdf9f9f407a69e0ead05f935d34ed86a63))
 * Use lru cache decorator for values_df loading ([`4006818`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/40068187da20854fcca980872bc42b8a3a096cc9))
 * Add support for loader kwargs ([`127f821`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/127f8215c35b792390595b890210baa0e8cf3591))
 * Move values_df resolution to anyspec object ([`714e83f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/714e83fd3722b298cdd256b06915659ca7a34259))
 * Make date of birth output prefix a param ([`0ed1198`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/0ed11982ba1b239e5650d23dbfab707100e38137))
 * Ensure that dfs are sorted and of same length before concat ([`84a4d65`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/84a4d65b731a6822d0a8f6313d01b7de9c574afe))
 * Use pandas with set_index for concat ([`b93290a`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/b93290ae733857855abe8197291dd047cf6c6fa8))
@@ -412,30 +429,30 @@
 * Coerce by default ([`60adb99`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/60adb999c83b6d93d97f1c6537f20c012721561e))
 * Output_col_name_override applied at loading, not flattening ([`95a96ce`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/95a96ce64a186c01f4e4e09d8787a97e42388df8))
 * Typo ([`01240ed`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/01240ed7b06843011593bcb3c3c71283918c90b2))
 * Incorrect attribute addressing ([`a6e82b5`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/a6e82b59ca353413066346e089f1557dc831d145))
 * Correctly resolve values_df ([`def67cd`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/def67cd954440df76f1570acf7e48f68ae636d6c))
 * MinGroupSpec should take a sequence of name to permute over ([`f0c8140`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/f0c814017b6f355d5916ba15fe26d9f3350a3a7b))
 * Typo ([`61c7241`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/61c7241d11f7bff3bad11e98cfea38600e239167))
-* Remove resolve_multiple_fn_name ([`617d386`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/617d386095139bc3445a5f4d14ffebce1e5ffa24))
+* Remove aggregation_fn_name ([`617d386`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/617d386095139bc3445a5f4d14ffebce1e5ffa24))
 * Old concat resulted in wrong ordering of rrows. ([`3759f71`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/3759f719070175c8be4184a0bdc5fc07db2c492c))
 * Set hba1c as eval ([`89fe6d2`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/89fe6d209b93d345d9a0d8cd562e90ec395dfa8d))
 * Typos ([`6eac440`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/6eac4408d8f0a58bb4cc66ac948bae5519a2c8cd))
 * Correct col name inference for static predictors ([`dfe5dc7`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/dfe5dc72d5d22332ce3d496fb1d3bcca3c9328c7))
 * Misc. fixes ([`45f8348`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/45f83488bef809ae059825caea9bf6937a5264d9))
 * Generate the correct amount of combinations when creating specs ([`c472b3c`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/c472b3c69e0dfc64b433546e538298ddd2d44a5f))
 * Typo resulted in cache breaking ([`fdd47d7`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/fdd47d705f166fcc3dc54612dc0387761d0489a9))
 * Correct col naming ([`bc74ae3`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/bc74ae3089a7bbfc99ee31d82902e1c98e30f18e))
 * Do not infer feature name from values_df ([`150569f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/150569fde483f6c427f1efe5688038340dfceb92))
 * Misc. errors found from tests ([`3a1b5db`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/3a1b5db493566592b349d317f7641d7564a662ad))
 * Revert falttened dataset to use specs ([`e4fada7`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/e4fada7a9fb98d1ebccd6c41568619aa7e059d79))
 * Misc. errors after introducing feature specs ([`0308eca`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/0308ecae8032ff309725b0917fd3901fadf102f9))
 * Correctly merge dataframes ([`a907885`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/a907885f592ba345cdf68ce5299699aacdc97b49))
 * Cache error because of loss off UUID ([`89d7f6f`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/89d7f6f0ce557c7c3126116864ba75d0ddb0037e))
-* New bugs in resolve_multiple ([`5714a39`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/5714a39c9e84081f6429dd0b8119873a9610e804))
+* New bugs in aggregation ([`5714a39`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/5714a39c9e84081f6429dd0b8119873a9610e804))
 * Rename outcomespec appropriately ([`41fa220`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/41fa22069453ac6df7dae824d49944775cf12ecc))
 * Lookbehind_days must be iterable ([`cc879e9`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/cc879e9d6b0f806a2a604ff71cb3febbd625c2aa))
 
 ### Documentation
 * Document feature spec objects ([`c7f1074`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/c7f10749d49b14a4614436097de2478f3e7fc879))
 * Typo ([`6bc7140`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/6bc71405a318de4811f259b2823c91f1951ebb95))
```

### Comparing `timeseriesflattener-0.27.0/CODE_OF_CONDUCT.md` & `timeseriesflattener-1.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/CONTRIBUTING.md` & `timeseriesflattener-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/LICENSE` & `timeseriesflattener-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/PKG-INFO` & `timeseriesflattener-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 0.27.0
+Version: 1.0.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -97,32 +97,30 @@
             "value": [1, 2, 3, 4],
         },
     )
     # Load a dataframe specifying when the outcome occurs
     outcome_df = pd.DataFrame({"id": [1], "date": ["2020-03-01"], "value": [1]})
 
     # Specify how to aggregate the predictors and define the outcome
-    from timeseriesflattener.feature_spec_objects import OutcomeSpec, PredictorSpec
-    from timeseriesflattener.resolve_multiple_functions import maximum, mean
+    from timeseriesflattener.feature_specs.single_specs import OutcomeSpec, PredictorSpec
+    from timeseriesflattener.aggregation_fns import maximum, mean
 
     predictor_spec = PredictorSpec(
-        values_df=predictor_df,
+        timeseries_df=predictor_df,
         lookbehind_days=30,
         fallback=np.nan,
-        entity_id_col_name="id",
-        resolve_multiple_fn=mean,
-        feature_name="test_feature",
+        aggregation_fn=mean,
+        feature_base_name="test_feature",
     )
     outcome_spec = OutcomeSpec(
-        values_df=outcome_df,
+        timeseries_df=outcome_df,
         lookahead_days=31,
         fallback=0,
-        entity_id_col_name="id",
-        resolve_multiple_fn=maximum,
-        feature_name="test_outcome",
+        aggregation_fn=maximum,
+        feature_base_name="test_outcome",
         incident=False,
     )
 
     # Instantiate TimeseriesFlattener and add the specifications
     from timeseriesflattener import TimeseriesFlattener
 
     ts_flattener = TimeseriesFlattener(
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.27.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.0.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
@@ -61,23 +61,22 @@
 pd.DataFrame( { "id": [1, 1, 2], "date": ["2020-01-01", "2020-02-01", "2020-02-
 01"], }, ) # Load a dataframe with raw values you wish to aggregate as
 predictors predictor_df = pd.DataFrame( { "id": [1, 1, 1, 2], "date": [ "2020-
 01-15", "2019-12-10", "2019-12-15", "2020-01-02", ], "value": [1, 2, 3, 4], },
 ) # Load a dataframe specifying when the outcome occurs outcome_df =
 pd.DataFrame({"id": [1], "date": ["2020-03-01"], "value": [1]}) # Specify how
 to aggregate the predictors and define the outcome from
-timeseriesflattener.feature_spec_objects import OutcomeSpec, PredictorSpec from
-timeseriesflattener.resolve_multiple_functions import maximum, mean
-predictor_spec = PredictorSpec( values_df=predictor_df, lookbehind_days=30,
-fallback=np.nan, entity_id_col_name="id", resolve_multiple_fn=mean,
-feature_name="test_feature", ) outcome_spec = OutcomeSpec
-( values_df=outcome_df, lookahead_days=31, fallback=0, entity_id_col_name="id",
-resolve_multiple_fn=maximum, feature_name="test_outcome", incident=False, ) #
-Instantiate TimeseriesFlattener and add the specifications from
-timeseriesflattener import TimeseriesFlattener ts_flattener =
+timeseriesflattener.feature_specs.single_specs import OutcomeSpec,
+PredictorSpec from timeseriesflattener.aggregation_fns import maximum, mean
+predictor_spec = PredictorSpec( timeseries_df=predictor_df, lookbehind_days=30,
+fallback=np.nan, aggregation_fn=mean, feature_base_name="test_feature", )
+outcome_spec = OutcomeSpec( timeseries_df=outcome_df, lookahead_days=31,
+fallback=0, aggregation_fn=maximum, feature_base_name="test_outcome",
+incident=False, ) # Instantiate TimeseriesFlattener and add the specifications
+from timeseriesflattener import TimeseriesFlattener ts_flattener =
 TimeseriesFlattener( prediction_times_df=prediction_times_df,
 entity_id_col_name="id", timestamp_col_name="date", n_workers=1,
 drop_pred_times_with_insufficient_look_distance=False, ) ts_flattener.add_spec(
 [predictor_spec, outcome_spec]) df = ts_flattener.get_df() df ``` Output: | |
 id | date | prediction_time_uuid |
 pred_test_feature_within_30_days_mean_fallback_nan |
 outc_test_outcome_within_31_days_maximum_fallback_0_dichotomous | | ---: | ---:
```

### Comparing `timeseriesflattener-0.27.0/README.md` & `timeseriesflattener-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,32 +51,30 @@
             "value": [1, 2, 3, 4],
         },
     )
     # Load a dataframe specifying when the outcome occurs
     outcome_df = pd.DataFrame({"id": [1], "date": ["2020-03-01"], "value": [1]})
 
     # Specify how to aggregate the predictors and define the outcome
-    from timeseriesflattener.feature_spec_objects import OutcomeSpec, PredictorSpec
-    from timeseriesflattener.resolve_multiple_functions import maximum, mean
+    from timeseriesflattener.feature_specs.single_specs import OutcomeSpec, PredictorSpec
+    from timeseriesflattener.aggregation_fns import maximum, mean
 
     predictor_spec = PredictorSpec(
-        values_df=predictor_df,
+        timeseries_df=predictor_df,
         lookbehind_days=30,
         fallback=np.nan,
-        entity_id_col_name="id",
-        resolve_multiple_fn=mean,
-        feature_name="test_feature",
+        aggregation_fn=mean,
+        feature_base_name="test_feature",
     )
     outcome_spec = OutcomeSpec(
-        values_df=outcome_df,
+        timeseries_df=outcome_df,
         lookahead_days=31,
         fallback=0,
-        entity_id_col_name="id",
-        resolve_multiple_fn=maximum,
-        feature_name="test_outcome",
+        aggregation_fn=maximum,
+        feature_base_name="test_outcome",
         incident=False,
     )
 
     # Instantiate TimeseriesFlattener and add the specifications
     from timeseriesflattener import TimeseriesFlattener
 
     ts_flattener = TimeseriesFlattener(
```

### Comparing `timeseriesflattener-0.27.0/citation.cff` & `timeseriesflattener-1.0.0/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/Makefile` & `timeseriesflattener-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/_static/favicon.ico` & `timeseriesflattener-1.0.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/_static/icon.png` & `timeseriesflattener-1.0.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/_static/icon_dark.png` & `timeseriesflattener-1.0.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/_static/terminology_figure.png` & `timeseriesflattener-1.0.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/conf.py` & `timeseriesflattener-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/faq.rst` & `timeseriesflattener-1.0.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/index.rst` & `timeseriesflattener-1.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-1.0.0/docs/tutorials/01_basic.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9678197846890939%*

 * *Differences: {"'cells'": "{7: {'execution_count': 2, 'outputs': {1: {'data': {'text/html': {insert: [(25, "*

 * *            "'      <th>95792</th>\\n'), (26, '      <td>0</td>\\n'), (27, '      <td>1969-10-19 "*

 * *            "10:29:00</td>\\n'), (28, '      <td>0.799246</td>\\n'), (31, '      "*

 * *            "<th>82592</th>\\n'), (32, '      <td>0</td>\\n'), (33, '      <td>1965-05-03 "*

 * *            "05:23:00</td>\\n'), (34, '      <td>6.630007</td>\\n'), (37, '      "*

 * *            "<th>1377</th>\\n'), (38, '      <td>0</td>\\n') […]*

```diff
@@ -238,15 +238,15 @@
             "source": [
                 "### Loading a temporal predictor\n",
                 "Then, we'll load the values for our temporal predictor. Temporal predictors are predictors that can have a different value at different timepoints."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\">\u256d\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 skimpy summary \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u256e\n",
                             "\u2502 <span style=\"font-style: italic\">         Data Summary         </span> <span style=\"font-style: italic\">      Data Types       </span>                                                          \u2502\n",
@@ -326,103 +326,104 @@
                             "      <th>entity_id</th>\n",
                             "      <th>timestamp</th>\n",
                             "      <th>value</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>9476</td>\n",
-                            "      <td>1969-03-05 08:08:00</td>\n",
-                            "      <td>0.816995</td>\n",
+                            "      <th>95792</th>\n",
+                            "      <td>0</td>\n",
+                            "      <td>1969-10-19 10:29:00</td>\n",
+                            "      <td>0.799246</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>4631</td>\n",
-                            "      <td>1967-04-10 22:48:00</td>\n",
-                            "      <td>4.818074</td>\n",
+                            "      <th>82592</th>\n",
+                            "      <td>0</td>\n",
+                            "      <td>1965-05-03 05:23:00</td>\n",
+                            "      <td>6.630007</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>3890</td>\n",
-                            "      <td>1969-12-15 14:07:00</td>\n",
-                            "      <td>2.503789</td>\n",
+                            "      <th>1377</th>\n",
+                            "      <td>0</td>\n",
+                            "      <td>1967-06-12 14:06:00</td>\n",
+                            "      <td>0.174793</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>1098</td>\n",
-                            "      <td>1965-11-19 03:53:00</td>\n",
-                            "      <td>3.515041</td>\n",
+                            "      <th>28579</th>\n",
+                            "      <td>0</td>\n",
+                            "      <td>1967-11-26 01:59:00</td>\n",
+                            "      <td>2.981185</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>1626</td>\n",
-                            "      <td>1966-05-03 14:07:00</td>\n",
-                            "      <td>4.353115</td>\n",
+                            "      <th>81247</th>\n",
+                            "      <td>0</td>\n",
+                            "      <td>1967-05-12 12:44:00</td>\n",
+                            "      <td>0.970382</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>...</th>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "      <td>...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>99995</th>\n",
-                            "      <td>4542</td>\n",
-                            "      <td>1968-06-01 17:09:00</td>\n",
-                            "      <td>9.616722</td>\n",
+                            "      <th>10277</th>\n",
+                            "      <td>9999</td>\n",
+                            "      <td>1967-06-20 00:12:00</td>\n",
+                            "      <td>4.304568</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>99996</th>\n",
-                            "      <td>4839</td>\n",
-                            "      <td>1966-11-24 01:13:00</td>\n",
-                            "      <td>0.235124</td>\n",
+                            "      <th>74701</th>\n",
+                            "      <td>9999</td>\n",
+                            "      <td>1968-08-19 10:15:00</td>\n",
+                            "      <td>0.671907</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>99997</th>\n",
-                            "      <td>8168</td>\n",
-                            "      <td>1969-07-30 01:45:00</td>\n",
-                            "      <td>0.929738</td>\n",
+                            "      <th>69566</th>\n",
+                            "      <td>9999</td>\n",
+                            "      <td>1968-01-08 02:41:00</td>\n",
+                            "      <td>3.250538</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>99998</th>\n",
-                            "      <td>9328</td>\n",
-                            "      <td>1965-12-22 10:53:00</td>\n",
-                            "      <td>5.124424</td>\n",
+                            "      <th>40901</th>\n",
+                            "      <td>9999</td>\n",
+                            "      <td>1966-04-23 02:37:00</td>\n",
+                            "      <td>8.924175</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
-                            "      <th>99999</th>\n",
-                            "      <td>6582</td>\n",
-                            "      <td>1965-02-10 09:52:00</td>\n",
-                            "      <td>7.414466</td>\n",
+                            "      <th>96881</th>\n",
+                            "      <td>9999</td>\n",
+                            "      <td>1969-06-24 07:19:00</td>\n",
+                            "      <td>4.501553</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "<p>100000 rows \u00d7 3 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "       entity_id           timestamp     value\n",
-                            "0           9476 1969-03-05 08:08:00  0.816995\n",
-                            "1           4631 1967-04-10 22:48:00  4.818074\n",
-                            "2           3890 1969-12-15 14:07:00  2.503789\n",
-                            "3           1098 1965-11-19 03:53:00  3.515041\n",
-                            "4           1626 1966-05-03 14:07:00  4.353115\n",
+                            "95792          0 1969-10-19 10:29:00  0.799246\n",
+                            "82592          0 1965-05-03 05:23:00  6.630007\n",
+                            "1377           0 1967-06-12 14:06:00  0.174793\n",
+                            "28579          0 1967-11-26 01:59:00  2.981185\n",
+                            "81247          0 1967-05-12 12:44:00  0.970382\n",
                             "...          ...                 ...       ...\n",
-                            "99995       4542 1968-06-01 17:09:00  9.616722\n",
-                            "99996       4839 1966-11-24 01:13:00  0.235124\n",
-                            "99997       8168 1969-07-30 01:45:00  0.929738\n",
-                            "99998       9328 1965-12-22 10:53:00  5.124424\n",
-                            "99999       6582 1965-02-10 09:52:00  7.414466\n",
+                            "10277       9999 1967-06-20 00:12:00  4.304568\n",
+                            "74701       9999 1968-08-19 10:15:00  0.671907\n",
+                            "69566       9999 1968-01-08 02:41:00  3.250538\n",
+                            "40901       9999 1966-04-23 02:37:00  8.924175\n",
+                            "96881       9999 1969-06-24 07:19:00  4.501553\n",
                             "\n",
                             "[100000 rows x 3 columns]"
                         ]
                     },
+                    "execution_count": 2,
                     "metadata": {},
-                    "output_type": "display_data"
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from timeseriesflattener.testing.load_synth_data import load_synth_predictor_float\n",
                 "\n",
                 "df_synth_predictors = load_synth_predictor_float()\n",
                 "\n",
@@ -635,15 +636,15 @@
             "metadata": {},
             "source": [
                 "And, lastly, our outcome values. We've chosen a binary outcome and only stored values for the timestamps that experience the outcome. From these, we can infer patients that do not experience the outcome, since they do not have a timestamp. We handle this by setting a fallback of 0 - more on that in the following section."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\">\u256d\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 skimpy summary \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u256e\n",
                             "\u2502 <span style=\"font-style: italic\">         Data Summary         </span> <span style=\"font-style: italic\">      Data Types       </span>                                                          \u2502\n",
@@ -808,16 +809,17 @@
                             "6256       9968 1968-09-06 13:15:00      1\n",
                             "6257       9970 1967-01-24 08:52:00      1\n",
                             "6269       9992 1966-12-10 14:53:00      1\n",
                             "\n",
                             "[3103 rows x 3 columns]"
                         ]
                     },
+                    "execution_count": 4,
                     "metadata": {},
-                    "output_type": "display_data"
+                    "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from timeseriesflattener.testing.load_synth_data import load_synth_outcome\n",
                 "\n",
                 "df_synth_outcome = load_synth_outcome()\n",
                 "\n",
@@ -871,42 +873,42 @@
                 "![](img/term_b.png)\n",
                 "\n",
                 "We want labels for prediction times to be 0 if the outcome never occurs, or if the outcome happens outside the lookahead window. Labels should only be 1 if the outcome occurs inside the lookahead window. Let's specify this in code."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from timeseriesflattener.feature_spec_objects import OutcomeSpec\n",
-                "from timeseriesflattener.resolve_multiple_functions import maximum\n",
+                "from timeseriesflattener.feature_specs.single_specs import OutcomeSpec\n",
+                "from timeseriesflattener.aggregation_fns import maximum\n",
                 "import pandas as pd\n",
                 "\n",
                 "test_df = pd.DataFrame()\n",
                 "\n",
                 "outcome_spec = OutcomeSpec(\n",
-                "    values_df=df_synth_outcome,\n",
+                "    timeseries_df=df_synth_outcome,\n",
                 "    lookahead_days=365,\n",
                 "    fallback=0,\n",
-                "    resolve_multiple_fn=maximum,\n",
+                "    aggregation_fn=maximum,\n",
                 "    incident=False,\n",
-                "    feature_name=\"outcome_name\",\n",
+                "    feature_base_name=\"outcome_name\",\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Since our outcome is binary, we want each prediction time to be labeled with 0 for the outcome if none is present within lookahead days. To do this, we use the fallback argument, which specifies the default value to use if none are found in `values_df` within `lookahead`. In this case, we set it to 0.\n",
                 "\n",
-                "Your use case determines how you want to handle multiple outcome values within lookahead days. In this case, we decide that any prediction time with at least one outcome (a timestamp in the loaded outcome data with a corresponding value of 1) within the specified lookahead days is \"positive\". I.e., if there is both a 0 and a 1 within lookahead days, the prediction time should be labeled with a 1. We set `resolve_multiple_fn = maximum` to accomplish this.\n",
+                "Your use case determines how you want to handle multiple outcome values within lookahead days. In this case, we decide that any prediction time with at least one outcome (a timestamp in the loaded outcome data with a corresponding value of 1) within the specified lookahead days is \"positive\". I.e., if there is both a 0 and a 1 within lookahead days, the prediction time should be labeled with a 1. We set `aggregation_fn = maximum` to accomplish this.\n",
                 "\n",
                 "We also specify that the outcome is not incident. This means that patient ID (dw_ek_borger) can experience the outcome more than once. If the outcome was marked as incident, all prediction times after the patient experiences the outcome are dropped. This is useful for cases where an event is permanent - for example, whether a patient has type 1 diabetes or not.\n",
                 "\n",
                 "Lastly, we specify a name of the outcome which'll be used when generating its column."
             ]
         },
         {
@@ -927,50 +929,50 @@
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from timeseriesflattener.feature_spec_objects import PredictorSpec, StaticSpec\n",
-                "from timeseriesflattener.resolve_multiple_functions import mean\n",
+                "from timeseriesflattener.feature_specs.single_specs import PredictorSpec, StaticSpec\n",
+                "from timeseriesflattener.aggregation_fns import mean\n",
                 "import numpy as np\n",
                 "\n",
                 "temporal_predictor_spec = PredictorSpec(\n",
-                "    values_df=df_synth_predictors,\n",
+                "    timeseries_df=df_synth_predictors,\n",
                 "    lookbehind_days=730,\n",
                 "    fallback=np.nan,\n",
-                "    resolve_multiple_fn=mean,\n",
-                "    feature_name=\"predictor_name\",\n",
+                "    aggregation_fn=mean,\n",
+                "    feature_base_name=\"predictor_name\",\n",
                 ")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "![](img/term_c.png)\n",
                 "\n",
-                "Values within the *lookbehind* window are aggregated using `resolve_multiple_fn`, for example the mean as shown in this example, or max/min etc. "
+                "Values within the *lookbehind* window are aggregated using `aggregation_fn`, for example the mean as shown in this example, or max/min etc. "
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Static predictor specification\n",
                 "Static features should be specified using `StaticSpec` as they are handled slightly differently. As in the previous specifications, we provide a `values_df` containing the values and we set the feature name. However, now we also add a prefix. By default, `PredictorSpec` prefixes columns with \u201cpred\u201d and `OutcomeSpec` prefixes columns with \u201coutc\u201d to make filtering easy. \n",
                 "As `StaticSpec` can be used for both generating predictors and outcomes, we manually set the prefix to be \u201cpred\u201d, as sex is used as predictor in this case."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1068,38 +1070,39 @@
                             "9996       9997       1\n",
                             "9997       9998       1\n",
                             "9998       9999       0\n",
                             "\n",
                             "[9999 rows x 2 columns]"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "sex_predictor_spec = StaticSpec(\n",
-                "    values_df=df_synth_sex,\n",
-                "    feature_name=\"female\",\n",
+                "    timeseries_df=df_synth_sex,\n",
+                "    feature_base_name=\"female\",\n",
                 "    prefix=\"pred\",\n",
-                "    input_col_name_override=\"female\",\n",
                 ")\n",
                 "\n",
                 "df_synth_sex"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Note that we also specify the \"input_col_name_override\", because the df_synth_sex df has its values in the \"female\" column. By default, tsflattener looks for a column names \"value\"."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we're ready to flatten our dataset!"
             ]
         },
         {
@@ -1109,15 +1112,15 @@
             "source": [
                 "## Flattening\n",
                 "Flattening is as easy as instantiating the `TimeseriesFlattener` class with the prediction times df along with dataset specific metadata and calling the `add_*` functions. `n_workers` can be set to parallelize operations across multiple cores. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from timeseriesflattener import TimeseriesFlattener\n",
                 "\n",
                 "ts_flattener = TimeseriesFlattener(\n",
                 "    prediction_times_df=df_prediction_times,\n",
@@ -1139,27 +1142,41 @@
                 "\n",
                 "\n",
                 "For most applications, this should be true - you do not want features to say they're looking a year into the future, if you only have a month of data. This would compromise generalisability. However, there are some edge cases where you might want this to be false - see the advanced tutorial for a brief discussion on this."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ts_flattener.add_spec([sex_predictor_spec, temporal_predictor_spec, outcome_spec])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "2023-06-14 16:11:40 [INFO] There were unprocessed specs, computing...\n",
+                        "2023-06-14 16:11:40 [INFO] _drop_pred_time_if_insufficient_look_distance: Dropped 5999 (59.99%) rows\n",
+                        "2023-06-14 16:11:40 [INFO] Processing 2 temporal features in parallel with 1 workers. Chunksize is 2. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\n",
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 2/2 [00:00<00:00,  2.14it/s]\n",
+                        "2023-06-14 16:11:41 [INFO] Checking alignment of dataframes - this might take a little while (~2 minutes for 1.000 dataframes with 2.000.000 rows).\n",
+                        "2023-06-14 16:11:41 [INFO] Starting concatenation. Will take some time on performant systems, e.g. 30s for 100 features and 2_000_000 prediction times. This is normal.\n",
+                        "2023-06-14 16:11:41 [INFO] Concatenation took 0.003 seconds\n",
+                        "2023-06-14 16:11:41 [INFO] Merging with original df\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "<pre style=\"white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace\">\u256d\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500 skimpy summary \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u256e\n",
                             "\u2502 <span style=\"font-style: italic\">         Data Summary         </span> <span style=\"font-style: italic\">      Data Types       </span>                                                          \u2502\n",
                             "\u2502 \u250f\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2513 \u250f\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2513                                                          \u2502\n",
                             "\u2502 \u2503<span style=\"color: #008080; text-decoration-color: #008080; font-weight: bold\"> dataframe         </span>\u2503<span style=\"color: #008080; text-decoration-color: #008080; font-weight: bold\"> Values </span>\u2503 \u2503<span style=\"color: #008080; text-decoration-color: #008080; font-weight: bold\"> Column Type </span>\u2503<span style=\"color: #008080; text-decoration-color: #008080; font-weight: bold\"> Count </span>\u2503                                                          \u2502\n",
                             "\u2502 \u2521\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2529 \u2521\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2529                                                          \u2502\n",
@@ -1169,16 +1186,16 @@
                             "\u2502                                \u2502 string      \u2502 1     \u2502                                                          \u2502\n",
                             "\u2502                                \u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518                                                          \u2502\n",
                             "\u2502 <span style=\"font-style: italic\">                                                    number                                                    </span>  \u2502\n",
                             "\u2502 \u250f\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2513  \u2502\n",
                             "\u2502 \u2503<span style=\"font-weight: bold\"> column_name                </span>\u2503<span style=\"font-weight: bold\"> NA  </span>\u2503<span style=\"font-weight: bold\"> NA %   </span>\u2503<span style=\"font-weight: bold\"> mean    </span>\u2503<span style=\"font-weight: bold\"> sd     </span>\u2503<span style=\"font-weight: bold\"> p0      </span>\u2503<span style=\"font-weight: bold\"> p25    </span>\u2503<span style=\"font-weight: bold\"> p75   </span>\u2503<span style=\"font-weight: bold\"> p100   </span>\u2503<span style=\"font-weight: bold\"> hist    </span>\u2503  \u2502\n",
                             "\u2502 \u2521\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2529  \u2502\n",
                             "\u2502 \u2502 <span style=\"color: #af87ff; text-decoration-color: #af87ff\">entity_id                 </span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">   5000</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  2900</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">      3</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  2600</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\"> 7500</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\"> 10000</span> \u2502 <span style=\"color: #008000; text-decoration-color: #008000\">\u2588\u2588\u2588\u2588\u2588\u2587 </span> \u2502  \u2502\n",
-                            "\u2502 \u2502 <span style=\"color: #af87ff; text-decoration-color: #af87ff\">outc_outcome_name_wi      </span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  0.064</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  0.25</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">      0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">    0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     1</span> \u2502 <span style=\"color: #008000; text-decoration-color: #008000\">\u2588    \u2581 </span> \u2502  \u2502\n",
                             "\u2502 \u2502 <span style=\"color: #af87ff; text-decoration-color: #af87ff\">pred_predictor_name_      </span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\"> 72</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">   1.8</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">      5</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">   1.6</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  0.097</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">   3.9</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">    6</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">   9.9</span> \u2502 <span style=\"color: #008000; text-decoration-color: #008000\">\u2581\u2583\u2588\u2588\u2583\u2581 </span> \u2502  \u2502\n",
+                            "\u2502 \u2502 <span style=\"color: #af87ff; text-decoration-color: #af87ff\">outc_outcome_name_wi      </span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  0.064</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  0.25</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">      0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">    0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     1</span> \u2502 <span style=\"color: #008000; text-decoration-color: #008000\">\u2588    \u2581 </span> \u2502  \u2502\n",
                             "\u2502 \u2502 <span style=\"color: #af87ff; text-decoration-color: #af87ff\">pred_female               </span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">  0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">   0.49</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">   0.5</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">      0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">    1</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">     1</span> \u2502 <span style=\"color: #008000; text-decoration-color: #008000\">\u2588    \u2588 </span> \u2502  \u2502\n",
                             "\u2502 \u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518  \u2502\n",
                             "\u2502 <span style=\"font-style: italic\">                                                   datetime                                                   </span>  \u2502\n",
                             "\u2502 \u250f\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2513  \u2502\n",
                             "\u2502 \u2503<span style=\"font-weight: bold\"> column_name      </span>\u2503<span style=\"font-weight: bold\"> NA   </span>\u2503<span style=\"font-weight: bold\"> NA %    </span>\u2503<span style=\"font-weight: bold\"> first                      </span>\u2503<span style=\"font-weight: bold\"> last                       </span>\u2503<span style=\"font-weight: bold\"> frequency    </span>\u2503  \u2502\n",
                             "\u2502 \u2521\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2529  \u2502\n",
                             "\u2502 \u2502 <span style=\"color: #af87ff; text-decoration-color: #af87ff\">timestamp       </span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">   0</span> \u2502 <span style=\"color: #008080; text-decoration-color: #008080\">      0</span> \u2502 <span style=\"color: #800000; text-decoration-color: #800000\">   1967-01-02 01:16:00    </span> \u2502 <span style=\"color: #800000; text-decoration-color: #800000\">   1968-12-31 04:39:00    </span> \u2502 <span style=\"color: #af87ff; text-decoration-color: #af87ff\">None        </span> \u2502  \u2502\n",
@@ -1204,16 +1221,16 @@
                             "\u2502                                \u2502 string      \u2502 1     \u2502                                                          \u2502\n",
                             "\u2502                                \u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518                                                          \u2502\n",
                             "\u2502 \u001b[3m                                                    number                                                    \u001b[0m  \u2502\n",
                             "\u2502 \u250f\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2513  \u2502\n",
                             "\u2502 \u2503\u001b[1m \u001b[0m\u001b[1mcolumn_name               \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mNA \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mNA %  \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mmean   \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1msd    \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mp0     \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mp25   \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mp75  \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mp100  \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mhist   \u001b[0m\u001b[1m \u001b[0m\u2503  \u2502\n",
                             "\u2502 \u2521\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2529  \u2502\n",
                             "\u2502 \u2502 \u001b[38;5;141mentity_id                 \u001b[0m \u2502 \u001b[36m  0\u001b[0m \u2502 \u001b[36m     0\u001b[0m \u2502 \u001b[36m   5000\u001b[0m \u2502 \u001b[36m  2900\u001b[0m \u2502 \u001b[36m      3\u001b[0m \u2502 \u001b[36m  2600\u001b[0m \u2502 \u001b[36m 7500\u001b[0m \u2502 \u001b[36m 10000\u001b[0m \u2502 \u001b[32m\u2588\u2588\u2588\u2588\u2588\u2587 \u001b[0m \u2502  \u2502\n",
-                            "\u2502 \u2502 \u001b[38;5;141moutc_outcome_name_wi      \u001b[0m \u2502 \u001b[36m  0\u001b[0m \u2502 \u001b[36m     0\u001b[0m \u2502 \u001b[36m  0.064\u001b[0m \u2502 \u001b[36m  0.25\u001b[0m \u2502 \u001b[36m      0\u001b[0m \u2502 \u001b[36m     0\u001b[0m \u2502 \u001b[36m    0\u001b[0m \u2502 \u001b[36m     1\u001b[0m \u2502 \u001b[32m\u2588    \u2581 \u001b[0m \u2502  \u2502\n",
                             "\u2502 \u2502 \u001b[38;5;141mpred_predictor_name_      \u001b[0m \u2502 \u001b[36m 72\u001b[0m \u2502 \u001b[36m   1.8\u001b[0m \u2502 \u001b[36m      5\u001b[0m \u2502 \u001b[36m   1.6\u001b[0m \u2502 \u001b[36m  0.097\u001b[0m \u2502 \u001b[36m   3.9\u001b[0m \u2502 \u001b[36m    6\u001b[0m \u2502 \u001b[36m   9.9\u001b[0m \u2502 \u001b[32m\u2581\u2583\u2588\u2588\u2583\u2581 \u001b[0m \u2502  \u2502\n",
+                            "\u2502 \u2502 \u001b[38;5;141moutc_outcome_name_wi      \u001b[0m \u2502 \u001b[36m  0\u001b[0m \u2502 \u001b[36m     0\u001b[0m \u2502 \u001b[36m  0.064\u001b[0m \u2502 \u001b[36m  0.25\u001b[0m \u2502 \u001b[36m      0\u001b[0m \u2502 \u001b[36m     0\u001b[0m \u2502 \u001b[36m    0\u001b[0m \u2502 \u001b[36m     1\u001b[0m \u2502 \u001b[32m\u2588    \u2581 \u001b[0m \u2502  \u2502\n",
                             "\u2502 \u2502 \u001b[38;5;141mpred_female               \u001b[0m \u2502 \u001b[36m  0\u001b[0m \u2502 \u001b[36m     0\u001b[0m \u2502 \u001b[36m   0.49\u001b[0m \u2502 \u001b[36m   0.5\u001b[0m \u2502 \u001b[36m      0\u001b[0m \u2502 \u001b[36m     0\u001b[0m \u2502 \u001b[36m    1\u001b[0m \u2502 \u001b[36m     1\u001b[0m \u2502 \u001b[32m\u2588    \u2588 \u001b[0m \u2502  \u2502\n",
                             "\u2502 \u2514\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2534\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2518  \u2502\n",
                             "\u2502 \u001b[3m                                                   datetime                                                   \u001b[0m  \u2502\n",
                             "\u2502 \u250f\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2533\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2513  \u2502\n",
                             "\u2502 \u2503\u001b[1m \u001b[0m\u001b[1mcolumn_name     \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mNA  \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mNA %   \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mfirst                     \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mlast                      \u001b[0m\u001b[1m \u001b[0m\u2503\u001b[1m \u001b[0m\u001b[1mfrequency   \u001b[0m\u001b[1m \u001b[0m\u2503  \u2502\n",
                             "\u2502 \u2521\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2547\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2501\u2529  \u2502\n",
                             "\u2502 \u2502 \u001b[38;5;141mtimestamp       \u001b[0m \u2502 \u001b[36m   0\u001b[0m \u2502 \u001b[36m      0\u001b[0m \u2502 \u001b[31m   1967-01-02 01:16:00    \u001b[0m \u2502 \u001b[31m   1968-12-31 04:39:00    \u001b[0m \u2502 \u001b[38;5;141mNone        \u001b[0m \u2502  \u2502\n",
@@ -1232,20 +1249,20 @@
                 },
                 {
                     "data": {
                         "text/plain": [
                             "['entity_id',\n",
                             " 'timestamp',\n",
                             " 'prediction_time_uuid',\n",
-                            " 'outc_outcome_name_within_365_days_maximum_fallback_0_dichotomous',\n",
                             " 'pred_predictor_name_within_730_days_mean_fallback_nan',\n",
+                            " 'outc_outcome_name_within_365_days_maximum_fallback_0_dichotomous',\n",
                             " 'pred_female']"
                         ]
                     },
-                    "execution_count": 16,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "df = ts_flattener.get_df()\n",
                 "\n",
@@ -1260,122 +1277,122 @@
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<style type=\"text/css\">\n",
                             "</style>\n",
-                            "<table id=\"T_4f6bc\" style=\"font-size: 10px\">\n",
+                            "<table id=\"T_003c4\" style=\"font-size: 14px\">\n",
                             "  <thead>\n",
                             "    <tr>\n",
                             "      <th class=\"blank level0\" >&nbsp;</th>\n",
-                            "      <th id=\"T_4f6bc_level0_col0\" class=\"col_heading level0 col0\" >entity_id</th>\n",
-                            "      <th id=\"T_4f6bc_level0_col1\" class=\"col_heading level0 col1\" >timestamp</th>\n",
-                            "      <th id=\"T_4f6bc_level0_col2\" class=\"col_heading level0 col2\" >prediction_time_uuid</th>\n",
-                            "      <th id=\"T_4f6bc_level0_col3\" class=\"col_heading level0 col3\" >outc_Y</th>\n",
-                            "      <th id=\"T_4f6bc_level0_col4\" class=\"col_heading level0 col4\" >pred_X</th>\n",
-                            "      <th id=\"T_4f6bc_level0_col5\" class=\"col_heading level0 col5\" >pred_female</th>\n",
+                            "      <th id=\"T_003c4_level0_col0\" class=\"col_heading level0 col0\" >entity_id</th>\n",
+                            "      <th id=\"T_003c4_level0_col1\" class=\"col_heading level0 col1\" >timestamp</th>\n",
+                            "      <th id=\"T_003c4_level0_col2\" class=\"col_heading level0 col2\" >prediction_time_uuid</th>\n",
+                            "      <th id=\"T_003c4_level0_col3\" class=\"col_heading level0 col3\" >pred_X</th>\n",
+                            "      <th id=\"T_003c4_level0_col4\" class=\"col_heading level0 col4\" >outc_Y</th>\n",
+                            "      <th id=\"T_003c4_level0_col5\" class=\"col_heading level0 col5\" >pred_female</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row0\" class=\"row_heading level0 row0\" >0</th>\n",
-                            "      <td id=\"T_4f6bc_row0_col0\" class=\"data row0 col0\" >9903</td>\n",
-                            "      <td id=\"T_4f6bc_row0_col1\" class=\"data row0 col1\" >1968-05-09 21:24:00</td>\n",
-                            "      <td id=\"T_4f6bc_row0_col2\" class=\"data row0 col2\" >9903-1968-05-09-21-24-00</td>\n",
-                            "      <td id=\"T_4f6bc_row0_col3\" class=\"data row0 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row0_col4\" class=\"data row0 col4\" >0.990763</td>\n",
-                            "      <td id=\"T_4f6bc_row0_col5\" class=\"data row0 col5\" >0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row1\" class=\"row_heading level0 row1\" >1</th>\n",
-                            "      <td id=\"T_4f6bc_row1_col0\" class=\"data row1 col0\" >6447</td>\n",
-                            "      <td id=\"T_4f6bc_row1_col1\" class=\"data row1 col1\" >1967-09-25 18:08:00</td>\n",
-                            "      <td id=\"T_4f6bc_row1_col2\" class=\"data row1 col2\" >6447-1967-09-25-18-08-00</td>\n",
-                            "      <td id=\"T_4f6bc_row1_col3\" class=\"data row1 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row1_col4\" class=\"data row1 col4\" >5.582745</td>\n",
-                            "      <td id=\"T_4f6bc_row1_col5\" class=\"data row1 col5\" >1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row2\" class=\"row_heading level0 row2\" >2</th>\n",
-                            "      <td id=\"T_4f6bc_row2_col0\" class=\"data row2 col0\" >4927</td>\n",
-                            "      <td id=\"T_4f6bc_row2_col1\" class=\"data row2 col1\" >1968-06-30 12:13:00</td>\n",
-                            "      <td id=\"T_4f6bc_row2_col2\" class=\"data row2 col2\" >4927-1968-06-30-12-13-00</td>\n",
-                            "      <td id=\"T_4f6bc_row2_col3\" class=\"data row2 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row2_col4\" class=\"data row2 col4\" >4.957251</td>\n",
-                            "      <td id=\"T_4f6bc_row2_col5\" class=\"data row2 col5\" >0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row3\" class=\"row_heading level0 row3\" >3</th>\n",
-                            "      <td id=\"T_4f6bc_row3_col0\" class=\"data row3 col0\" >5475</td>\n",
-                            "      <td id=\"T_4f6bc_row3_col1\" class=\"data row3 col1\" >1967-01-09 03:09:00</td>\n",
-                            "      <td id=\"T_4f6bc_row3_col2\" class=\"data row3 col2\" >5475-1967-01-09-03-09-00</td>\n",
-                            "      <td id=\"T_4f6bc_row3_col3\" class=\"data row3 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row3_col4\" class=\"data row3 col4\" >5.999336</td>\n",
-                            "      <td id=\"T_4f6bc_row3_col5\" class=\"data row3 col5\" >0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row4\" class=\"row_heading level0 row4\" >4</th>\n",
-                            "      <td id=\"T_4f6bc_row4_col0\" class=\"data row4 col0\" >9793</td>\n",
-                            "      <td id=\"T_4f6bc_row4_col1\" class=\"data row4 col1\" >1968-12-15 12:59:00</td>\n",
-                            "      <td id=\"T_4f6bc_row4_col2\" class=\"data row4 col2\" >9793-1968-12-15-12-59-00</td>\n",
-                            "      <td id=\"T_4f6bc_row4_col3\" class=\"data row4 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row4_col4\" class=\"data row4 col4\" >7.294038</td>\n",
-                            "      <td id=\"T_4f6bc_row4_col5\" class=\"data row4 col5\" >0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row5\" class=\"row_heading level0 row5\" >5</th>\n",
-                            "      <td id=\"T_4f6bc_row5_col0\" class=\"data row5 col0\" >9768</td>\n",
-                            "      <td id=\"T_4f6bc_row5_col1\" class=\"data row5 col1\" >1967-07-04 23:09:00</td>\n",
-                            "      <td id=\"T_4f6bc_row5_col2\" class=\"data row5 col2\" >9768-1967-07-04-23-09-00</td>\n",
-                            "      <td id=\"T_4f6bc_row5_col3\" class=\"data row5 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row5_col4\" class=\"data row5 col4\" >4.326286</td>\n",
-                            "      <td id=\"T_4f6bc_row5_col5\" class=\"data row5 col5\" >1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row6\" class=\"row_heading level0 row6\" >6</th>\n",
-                            "      <td id=\"T_4f6bc_row6_col0\" class=\"data row6 col0\" >7916</td>\n",
-                            "      <td id=\"T_4f6bc_row6_col1\" class=\"data row6 col1\" >1968-12-20 03:38:00</td>\n",
-                            "      <td id=\"T_4f6bc_row6_col2\" class=\"data row6 col2\" >7916-1968-12-20-03-38-00</td>\n",
-                            "      <td id=\"T_4f6bc_row6_col3\" class=\"data row6 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row6_col4\" class=\"data row6 col4\" >4.629502</td>\n",
-                            "      <td id=\"T_4f6bc_row6_col5\" class=\"data row6 col5\" >0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row7\" class=\"row_heading level0 row7\" >7</th>\n",
-                            "      <td id=\"T_4f6bc_row7_col0\" class=\"data row7 col0\" >33</td>\n",
-                            "      <td id=\"T_4f6bc_row7_col1\" class=\"data row7 col1\" >1967-07-28 03:16:00</td>\n",
-                            "      <td id=\"T_4f6bc_row7_col2\" class=\"data row7 col2\" >33-1967-07-28-03-16-00</td>\n",
-                            "      <td id=\"T_4f6bc_row7_col3\" class=\"data row7 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row7_col4\" class=\"data row7 col4\" >4.628500</td>\n",
-                            "      <td id=\"T_4f6bc_row7_col5\" class=\"data row7 col5\" >0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row8\" class=\"row_heading level0 row8\" >8</th>\n",
-                            "      <td id=\"T_4f6bc_row8_col0\" class=\"data row8 col0\" >2883</td>\n",
-                            "      <td id=\"T_4f6bc_row8_col1\" class=\"data row8 col1\" >1968-01-28 21:50:00</td>\n",
-                            "      <td id=\"T_4f6bc_row8_col2\" class=\"data row8 col2\" >2883-1968-01-28-21-50-00</td>\n",
-                            "      <td id=\"T_4f6bc_row8_col3\" class=\"data row8 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row8_col4\" class=\"data row8 col4\" >8.257742</td>\n",
-                            "      <td id=\"T_4f6bc_row8_col5\" class=\"data row8 col5\" >1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th id=\"T_4f6bc_level0_row9\" class=\"row_heading level0 row9\" >9</th>\n",
-                            "      <td id=\"T_4f6bc_row9_col0\" class=\"data row9 col0\" >1515</td>\n",
-                            "      <td id=\"T_4f6bc_row9_col1\" class=\"data row9 col1\" >1968-07-18 08:28:00</td>\n",
-                            "      <td id=\"T_4f6bc_row9_col2\" class=\"data row9 col2\" >1515-1968-07-18-08-28-00</td>\n",
-                            "      <td id=\"T_4f6bc_row9_col3\" class=\"data row9 col3\" >0.000000</td>\n",
-                            "      <td id=\"T_4f6bc_row9_col4\" class=\"data row9 col4\" >2.973084</td>\n",
-                            "      <td id=\"T_4f6bc_row9_col5\" class=\"data row9 col5\" >0</td>\n",
+                            "      <th id=\"T_003c4_level0_row0\" class=\"row_heading level0 row0\" >0</th>\n",
+                            "      <td id=\"T_003c4_row0_col0\" class=\"data row0 col0\" >9903</td>\n",
+                            "      <td id=\"T_003c4_row0_col1\" class=\"data row0 col1\" >1968-05-09 21:24:00</td>\n",
+                            "      <td id=\"T_003c4_row0_col2\" class=\"data row0 col2\" >9903-1968-05-09-21-24-00</td>\n",
+                            "      <td id=\"T_003c4_row0_col3\" class=\"data row0 col3\" >0.990763</td>\n",
+                            "      <td id=\"T_003c4_row0_col4\" class=\"data row0 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row0_col5\" class=\"data row0 col5\" >0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_003c4_level0_row1\" class=\"row_heading level0 row1\" >1</th>\n",
+                            "      <td id=\"T_003c4_row1_col0\" class=\"data row1 col0\" >6447</td>\n",
+                            "      <td id=\"T_003c4_row1_col1\" class=\"data row1 col1\" >1967-09-25 18:08:00</td>\n",
+                            "      <td id=\"T_003c4_row1_col2\" class=\"data row1 col2\" >6447-1967-09-25-18-08-00</td>\n",
+                            "      <td id=\"T_003c4_row1_col3\" class=\"data row1 col3\" >5.582745</td>\n",
+                            "      <td id=\"T_003c4_row1_col4\" class=\"data row1 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row1_col5\" class=\"data row1 col5\" >1</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_003c4_level0_row2\" class=\"row_heading level0 row2\" >2</th>\n",
+                            "      <td id=\"T_003c4_row2_col0\" class=\"data row2 col0\" >4927</td>\n",
+                            "      <td id=\"T_003c4_row2_col1\" class=\"data row2 col1\" >1968-06-30 12:13:00</td>\n",
+                            "      <td id=\"T_003c4_row2_col2\" class=\"data row2 col2\" >4927-1968-06-30-12-13-00</td>\n",
+                            "      <td id=\"T_003c4_row2_col3\" class=\"data row2 col3\" >4.957251</td>\n",
+                            "      <td id=\"T_003c4_row2_col4\" class=\"data row2 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row2_col5\" class=\"data row2 col5\" >0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_003c4_level0_row3\" class=\"row_heading level0 row3\" >3</th>\n",
+                            "      <td id=\"T_003c4_row3_col0\" class=\"data row3 col0\" >5475</td>\n",
+                            "      <td id=\"T_003c4_row3_col1\" class=\"data row3 col1\" >1967-01-09 03:09:00</td>\n",
+                            "      <td id=\"T_003c4_row3_col2\" class=\"data row3 col2\" >5475-1967-01-09-03-09-00</td>\n",
+                            "      <td id=\"T_003c4_row3_col3\" class=\"data row3 col3\" >5.999336</td>\n",
+                            "      <td id=\"T_003c4_row3_col4\" class=\"data row3 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row3_col5\" class=\"data row3 col5\" >0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_003c4_level0_row4\" class=\"row_heading level0 row4\" >4</th>\n",
+                            "      <td id=\"T_003c4_row4_col0\" class=\"data row4 col0\" >9793</td>\n",
+                            "      <td id=\"T_003c4_row4_col1\" class=\"data row4 col1\" >1968-12-15 12:59:00</td>\n",
+                            "      <td id=\"T_003c4_row4_col2\" class=\"data row4 col2\" >9793-1968-12-15-12-59-00</td>\n",
+                            "      <td id=\"T_003c4_row4_col3\" class=\"data row4 col3\" >7.294038</td>\n",
+                            "      <td id=\"T_003c4_row4_col4\" class=\"data row4 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row4_col5\" class=\"data row4 col5\" >0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_003c4_level0_row5\" class=\"row_heading level0 row5\" >5</th>\n",
+                            "      <td id=\"T_003c4_row5_col0\" class=\"data row5 col0\" >9768</td>\n",
+                            "      <td id=\"T_003c4_row5_col1\" class=\"data row5 col1\" >1967-07-04 23:09:00</td>\n",
+                            "      <td id=\"T_003c4_row5_col2\" class=\"data row5 col2\" >9768-1967-07-04-23-09-00</td>\n",
+                            "      <td id=\"T_003c4_row5_col3\" class=\"data row5 col3\" >4.326286</td>\n",
+                            "      <td id=\"T_003c4_row5_col4\" class=\"data row5 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row5_col5\" class=\"data row5 col5\" >1</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_003c4_level0_row6\" class=\"row_heading level0 row6\" >6</th>\n",
+                            "      <td id=\"T_003c4_row6_col0\" class=\"data row6 col0\" >7916</td>\n",
+                            "      <td id=\"T_003c4_row6_col1\" class=\"data row6 col1\" >1968-12-20 03:38:00</td>\n",
+                            "      <td id=\"T_003c4_row6_col2\" class=\"data row6 col2\" >7916-1968-12-20-03-38-00</td>\n",
+                            "      <td id=\"T_003c4_row6_col3\" class=\"data row6 col3\" >4.629502</td>\n",
+                            "      <td id=\"T_003c4_row6_col4\" class=\"data row6 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row6_col5\" class=\"data row6 col5\" >0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_003c4_level0_row7\" class=\"row_heading level0 row7\" >7</th>\n",
+                            "      <td id=\"T_003c4_row7_col0\" class=\"data row7 col0\" >33</td>\n",
+                            "      <td id=\"T_003c4_row7_col1\" class=\"data row7 col1\" >1967-07-28 03:16:00</td>\n",
+                            "      <td id=\"T_003c4_row7_col2\" class=\"data row7 col2\" >33-1967-07-28-03-16-00</td>\n",
+                            "      <td id=\"T_003c4_row7_col3\" class=\"data row7 col3\" >4.628500</td>\n",
+                            "      <td id=\"T_003c4_row7_col4\" class=\"data row7 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row7_col5\" class=\"data row7 col5\" >0</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_003c4_level0_row8\" class=\"row_heading level0 row8\" >8</th>\n",
+                            "      <td id=\"T_003c4_row8_col0\" class=\"data row8 col0\" >2883</td>\n",
+                            "      <td id=\"T_003c4_row8_col1\" class=\"data row8 col1\" >1968-01-28 21:50:00</td>\n",
+                            "      <td id=\"T_003c4_row8_col2\" class=\"data row8 col2\" >2883-1968-01-28-21-50-00</td>\n",
+                            "      <td id=\"T_003c4_row8_col3\" class=\"data row8 col3\" >8.257742</td>\n",
+                            "      <td id=\"T_003c4_row8_col4\" class=\"data row8 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row8_col5\" class=\"data row8 col5\" >1</td>\n",
+                            "    </tr>\n",
+                            "    <tr>\n",
+                            "      <th id=\"T_003c4_level0_row9\" class=\"row_heading level0 row9\" >9</th>\n",
+                            "      <td id=\"T_003c4_row9_col0\" class=\"data row9 col0\" >1515</td>\n",
+                            "      <td id=\"T_003c4_row9_col1\" class=\"data row9 col1\" >1968-07-18 08:28:00</td>\n",
+                            "      <td id=\"T_003c4_row9_col2\" class=\"data row9 col2\" >1515-1968-07-18-08-28-00</td>\n",
+                            "      <td id=\"T_003c4_row9_col3\" class=\"data row9 col3\" >2.973084</td>\n",
+                            "      <td id=\"T_003c4_row9_col4\" class=\"data row9 col4\" >0.000000</td>\n",
+                            "      <td id=\"T_003c4_row9_col5\" class=\"data row9 col5\" >0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n"
                         ],
                         "text/plain": [
-                            "<pandas.io.formats.style.Styler at 0x1477d2380>"
+                            "<pandas.io.formats.style.Styler at 0x107535f70>"
                         ]
                     },
                     "execution_count": 14,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
@@ -1392,412 +1409,25 @@
                 "    axis=1,\n",
                 ")\n",
                 "\n",
                 "df[0:10].style.set_table_attributes('style=\"font-size: 14px\"')"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "And there we go! A dataframe ready for classification, containing:\n",
                 "1. The citizen IDs\n",
                 "2. Timestamps for each prediction time\n",
                 "3. A unique identifier for each prediciton-time\n",
                 "4. Our predictor columns, prefixed with `pred_` and\n",
                 "5. Our outcome columns, prefixed with `outc_`"
             ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Handling data frames shaped as long with multiple value types"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Often, you may wish to create predictors or outcomes from a long data frame which contains values for multiple different value types, e.g. values from different types of blood value measurements. Below you can view an example of such a data frame."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from timeseriesflattener.testing.utils_for_testing import load_long_df_with_multiple_values\n",
-                "from timeseriesflattener.utils import split_df_and_register_to_dict"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>dw_ek_borger</th>\n",
-                            "      <th>timestamp</th>\n",
-                            "      <th>value_names</th>\n",
-                            "      <th>value</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>3824</td>\n",
-                            "      <td>1968-10-30 00:01:00</td>\n",
-                            "      <td>value_name_1</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>3986</td>\n",
-                            "      <td>1967-04-08 04:15:00</td>\n",
-                            "      <td>value_name_1</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>3703</td>\n",
-                            "      <td>1968-09-06 09:43:00</td>\n",
-                            "      <td>value_name_1</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>3596</td>\n",
-                            "      <td>1967-12-30 10:24:00</td>\n",
-                            "      <td>value_name_1</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>4678</td>\n",
-                            "      <td>1967-10-29 09:21:00</td>\n",
-                            "      <td>value_name_1</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>...</th>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>19995</th>\n",
-                            "      <td>2149</td>\n",
-                            "      <td>1966-09-19 09:51:00</td>\n",
-                            "      <td>value_name_2</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>19996</th>\n",
-                            "      <td>571</td>\n",
-                            "      <td>1966-03-15 19:20:00</td>\n",
-                            "      <td>value_name_2</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>19997</th>\n",
-                            "      <td>4028</td>\n",
-                            "      <td>1967-08-03 00:44:00</td>\n",
-                            "      <td>value_name_2</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>19998</th>\n",
-                            "      <td>4454</td>\n",
-                            "      <td>1965-11-29 06:18:00</td>\n",
-                            "      <td>value_name_2</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>19999</th>\n",
-                            "      <td>910</td>\n",
-                            "      <td>1967-03-30 23:39:00</td>\n",
-                            "      <td>value_name_2</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "<p>20000 rows \u00d7 4 columns</p>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "       dw_ek_borger           timestamp   value_names  value\n",
-                            "0              3824 1968-10-30 00:01:00  value_name_1      1\n",
-                            "1              3986 1967-04-08 04:15:00  value_name_1      0\n",
-                            "2              3703 1968-09-06 09:43:00  value_name_1      0\n",
-                            "3              3596 1967-12-30 10:24:00  value_name_1      0\n",
-                            "4              4678 1967-10-29 09:21:00  value_name_1      1\n",
-                            "...             ...                 ...           ...    ...\n",
-                            "19995          2149 1966-09-19 09:51:00  value_name_2      0\n",
-                            "19996           571 1966-03-15 19:20:00  value_name_2      1\n",
-                            "19997          4028 1967-08-03 00:44:00  value_name_2      1\n",
-                            "19998          4454 1965-11-29 06:18:00  value_name_2      0\n",
-                            "19999           910 1967-03-30 23:39:00  value_name_2      1\n",
-                            "\n",
-                            "[20000 rows x 4 columns]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
-            "source": [
-                "long_df = load_long_df_with_multiple_values()\n",
-                "long_df"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "To parrallelise the generation of features, timeseriesflattener needs a dataframe for each type of raw data. Instead of having to manually split the long data frame into separate data frames, the package allows users to automatically split a long data frame.\n",
-                "\n",
-                "Specifically, when loading split_df_and_register_to_dict, a variable with an empty dict is added to your namespace. When calling split_df_and_register_to_dict, it splits the dataframe and assigns this split dataframes to this variable. Let\u2019s see an example:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/plain": [
-                            "{'value_name_1':       dw_ek_borger           timestamp  value\n",
-                            " 0             3824 1968-10-30 00:01:00      1\n",
-                            " 1             3986 1967-04-08 04:15:00      0\n",
-                            " 2             3703 1968-09-06 09:43:00      0\n",
-                            " 3             3596 1967-12-30 10:24:00      0\n",
-                            " 4             4678 1967-10-29 09:21:00      1\n",
-                            " ...            ...                 ...    ...\n",
-                            " 9995          2149 1966-09-19 09:51:00      0\n",
-                            " 9996           571 1966-03-15 19:20:00      1\n",
-                            " 9997          4028 1967-08-03 00:44:00      1\n",
-                            " 9998          4454 1965-11-29 06:18:00      0\n",
-                            " 9999           910 1967-03-30 23:39:00      1\n",
-                            " \n",
-                            " [10000 rows x 3 columns],\n",
-                            " 'value_name_2':        dw_ek_borger           timestamp  value\n",
-                            " 10000          3824 1968-10-30 00:01:00      1\n",
-                            " 10001          3986 1967-04-08 04:15:00      0\n",
-                            " 10002          3703 1968-09-06 09:43:00      0\n",
-                            " 10003          3596 1967-12-30 10:24:00      0\n",
-                            " 10004          4678 1967-10-29 09:21:00      1\n",
-                            " ...             ...                 ...    ...\n",
-                            " 19995          2149 1966-09-19 09:51:00      0\n",
-                            " 19996           571 1966-03-15 19:20:00      1\n",
-                            " 19997          4028 1967-08-03 00:44:00      1\n",
-                            " 19998          4454 1965-11-29 06:18:00      0\n",
-                            " 19999           910 1967-03-30 23:39:00      1\n",
-                            " \n",
-                            " [10000 rows x 3 columns]}"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
-            "source": [
-                "split_df_and_register_to_dict(df=long_df)\n",
-                "\n",
-                "# This import is only needed to show the registered dfs in the docs\n",
-                "# You don't need to import it to use the function\n",
-                "from timeseriesflattener.feature_spec_objects import split_dfs\n",
-                "\n",
-                "split_dfs"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Once the variable has been populated, the separate data frames can be fetched when specifying features. You simply pass the value_name to the `values_name` keyword argument. When the specification is initialized, it searches through the keys in the dictionary and extracts the corresponding data frame:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "pred_spec = PredictorSpec(\n",
-                "    values_name=\"value_name_1\",\n",
-                "    lookbehind_days=365,\n",
-                "    fallback=np.nan,\n",
-                "    resolve_multiple_fn=mean,\n",
-                "    feature_name=\"value\",\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "text/html": [
-                            "<div>\n",
-                            "<style scoped>\n",
-                            "    .dataframe tbody tr th:only-of-type {\n",
-                            "        vertical-align: middle;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe tbody tr th {\n",
-                            "        vertical-align: top;\n",
-                            "    }\n",
-                            "\n",
-                            "    .dataframe thead th {\n",
-                            "        text-align: right;\n",
-                            "    }\n",
-                            "</style>\n",
-                            "<table border=\"1\" class=\"dataframe\">\n",
-                            "  <thead>\n",
-                            "    <tr style=\"text-align: right;\">\n",
-                            "      <th></th>\n",
-                            "      <th>dw_ek_borger</th>\n",
-                            "      <th>timestamp</th>\n",
-                            "      <th>value</th>\n",
-                            "    </tr>\n",
-                            "  </thead>\n",
-                            "  <tbody>\n",
-                            "    <tr>\n",
-                            "      <th>0</th>\n",
-                            "      <td>3824</td>\n",
-                            "      <td>1968-10-30 00:01:00</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>1</th>\n",
-                            "      <td>3986</td>\n",
-                            "      <td>1967-04-08 04:15:00</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>2</th>\n",
-                            "      <td>3703</td>\n",
-                            "      <td>1968-09-06 09:43:00</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>3</th>\n",
-                            "      <td>3596</td>\n",
-                            "      <td>1967-12-30 10:24:00</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>4</th>\n",
-                            "      <td>4678</td>\n",
-                            "      <td>1967-10-29 09:21:00</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>...</th>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "      <td>...</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>9995</th>\n",
-                            "      <td>2149</td>\n",
-                            "      <td>1966-09-19 09:51:00</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>9996</th>\n",
-                            "      <td>571</td>\n",
-                            "      <td>1966-03-15 19:20:00</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>9997</th>\n",
-                            "      <td>4028</td>\n",
-                            "      <td>1967-08-03 00:44:00</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>9998</th>\n",
-                            "      <td>4454</td>\n",
-                            "      <td>1965-11-29 06:18:00</td>\n",
-                            "      <td>0</td>\n",
-                            "    </tr>\n",
-                            "    <tr>\n",
-                            "      <th>9999</th>\n",
-                            "      <td>910</td>\n",
-                            "      <td>1967-03-30 23:39:00</td>\n",
-                            "      <td>1</td>\n",
-                            "    </tr>\n",
-                            "  </tbody>\n",
-                            "</table>\n",
-                            "<p>10000 rows \u00d7 3 columns</p>\n",
-                            "</div>"
-                        ],
-                        "text/plain": [
-                            "      dw_ek_borger           timestamp  value\n",
-                            "0             3824 1968-10-30 00:01:00      1\n",
-                            "1             3986 1967-04-08 04:15:00      0\n",
-                            "2             3703 1968-09-06 09:43:00      0\n",
-                            "3             3596 1967-12-30 10:24:00      0\n",
-                            "4             4678 1967-10-29 09:21:00      1\n",
-                            "...            ...                 ...    ...\n",
-                            "9995          2149 1966-09-19 09:51:00      0\n",
-                            "9996           571 1966-03-15 19:20:00      1\n",
-                            "9997          4028 1967-08-03 00:44:00      1\n",
-                            "9998          4454 1965-11-29 06:18:00      0\n",
-                            "9999           910 1967-03-30 23:39:00      1\n",
-                            "\n",
-                            "[10000 rows x 3 columns]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                }
-            ],
-            "source": [
-                "pred_spec.values_df"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Now we know how to use data loader functions and how to handle a long data frame with multiple different value types to more efficiently handle the data from which we want to create features. We also know how to create a bunch of feature specifications quickly! But with more features comes more computation. Let's look at caching next, so we can iterate on our datasets more quickly."
-            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": ".venv",
             "language": "python",
             "name": "python3"
@@ -1808,15 +1438,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.9.17"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "d2b49c0af2d95979144de75823f7cfbb268839811992fdd0cb17fc1bb54ce815"
             }
         }
```

### Comparing `timeseriesflattener-0.27.0/docs/tutorials/03_text.ipynb` & `timeseriesflattener-1.0.0/docs/tutorials/03_text.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9718737876096428%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 2: "*

 * *            "{'execution_count': 8, 'source': ['from timeseriesflattener.testing.load_synth_data "*

 * *            "import load_synth_text\\n']}, 3: {'execution_count': 9, 'outputs': {0: {'data': "*

 * *            "{'text/html': {insert: [(21, '      <th>value</th>\\n'), (29, '      <td>The patient "*

 * *            "went into a medically induced coma...</td>\\n'), (36, '      <td>The patient is taken "*

 * *            "to the emergenc […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Adding text features\n",
                 "\n",
                 "So far, the tutorials have dealt with _tabular_ data only. This tutorial will show you to make predictors out of text features, such as clinical notes, within `timeseriesflattener`.\n",
                 "\n",
@@ -20,34 +21,35 @@
                 "or by installing `timeseriesflattener` with the text dependencies.\n",
                 "```\n",
                 "pip install timeseriesflattener\"[text]\"\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## The dataset\n",
                 "\n",
                 "To start out, let's load a synthetic dataset containing text. As with all other features, each row in the dataset needs an ID, a timestamp, and the feature value. "
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from timeseriesflattener.testing.load_synth_data import load_synth_text"
+                "from timeseriesflattener.testing.load_synth_data import load_synth_text\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 9,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -66,198 +68,218 @@
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>entity_id</th>\n",
                             "      <th>timestamp</th>\n",
                             "      <th>text</th>\n",
+                            "      <th>value</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>0</th>\n",
                             "      <td>4647</td>\n",
                             "      <td>1967-07-19 00:22:00</td>\n",
                             "      <td>The patient went into a medically induced coma...</td>\n",
+                            "      <td>The patient went into a medically induced coma...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1</th>\n",
                             "      <td>2007</td>\n",
                             "      <td>1966-11-25 02:02:00</td>\n",
                             "      <td>The patient is taken to the emergency departme...</td>\n",
+                            "      <td>The patient is taken to the emergency departme...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>2</th>\n",
                             "      <td>5799</td>\n",
                             "      <td>1967-09-19 12:31:00</td>\n",
                             "      <td>The patient, described as a 7-month old son wh...</td>\n",
+                            "      <td>The patient, described as a 7-month old son wh...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>3</th>\n",
                             "      <td>1319</td>\n",
                             "      <td>1969-07-21 23:16:00</td>\n",
                             "      <td>The patient had been left on a bed for 20 minu...</td>\n",
+                            "      <td>The patient had been left on a bed for 20 minu...</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>4</th>\n",
                             "      <td>4234</td>\n",
                             "      <td>1966-04-14 22:04:00</td>\n",
                             "      <td>The patient had had some severe allergies but ...</td>\n",
+                            "      <td>The patient had had some severe allergies but ...</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "   entity_id           timestamp  \\\n",
                             "0       4647 1967-07-19 00:22:00   \n",
                             "1       2007 1966-11-25 02:02:00   \n",
                             "2       5799 1967-09-19 12:31:00   \n",
                             "3       1319 1969-07-21 23:16:00   \n",
                             "4       4234 1966-04-14 22:04:00   \n",
                             "\n",
-                            "                                                text  \n",
+                            "                                                text  \\\n",
+                            "0  The patient went into a medically induced coma...   \n",
+                            "1  The patient is taken to the emergency departme...   \n",
+                            "2  The patient, described as a 7-month old son wh...   \n",
+                            "3  The patient had been left on a bed for 20 minu...   \n",
+                            "4  The patient had had some severe allergies but ...   \n",
+                            "\n",
+                            "                                               value  \n",
                             "0  The patient went into a medically induced coma...  \n",
                             "1  The patient is taken to the emergency departme...  \n",
                             "2  The patient, described as a 7-month old son wh...  \n",
                             "3  The patient had been left on a bed for 20 minu...  \n",
                             "4  The patient had had some severe allergies but ...  "
                         ]
                     },
-                    "execution_count": 2,
+                    "execution_count": 9,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "load_synth_text().head()"
+                "load_synth_text().head()\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## TextPredictorSpec\n",
                 "\n",
                 "The main difference when specifying text predictors compared to tabular predictors is the `Spec` you define. For text, we need to specify a `TextPredictorSpec` which is entirely similar to the `PredictorSpec` except for two additional attributes: `embedding_fn` and `embedding_fn_kwargs`.\n",
                 "\n",
                 "`embedding_fn` should be a callable that takes a pandas Series containing text and converts it to a pandas DataFrame with a column for each feature. `embedding_fn_kwargs` are simply optional keyword arguments that will be passed to the embedding function, such as a Huggingface model name.\n",
                 "\n",
                 "Not all `resolve_multiple_fn` are meaningful for text, as we can't do numerical operations on text. Instead, `TextPredictorSpec` defaults to the \"concatenate\" option, which simply concatenates all texts within the lookbehind within. Other options that work for text are \"latest\" and \"earliest\". \n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Featurization using sentence-transformers\n",
                 "Let's specify a `TextPredictorSpec` using a [sentence-transformers](https://www.sbert.net/) model. `timeseriesflattener` includes functions that make it easy to featurize text using either sentence-transformers or any text model from the [Huggingface Hub](https://huggingface.co/). \n",
                 "\n",
                 "The `sentence_transformers_embedding` function is recommended for sentence-transformers. If you want to another type of model from the Huggingface Hub we recommend using the `huggingface_embedding` function which has the same interface as `sentence_transformers_embedding`.\n",
                 "\n",
                 "Notice, both `huggingface_embedding` and `sentence_transformers_embedding` will truncate the input to the maximum sequence length allowed by the model. If you want to use Huggingface embeddings for larger blocks of text, either use the `sklearn_embedding` function or write your own embedding function (see below)."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 10,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from timeseriesflattener.text_embedding_functions import (\n",
-                "        sentence_transformers_embedding, huggingface_embedding\n",
-                "        )\n",
+                "    sentence_transformers_embedding,\n",
+                "    huggingface_embedding,\n",
+                ")\n",
                 "from timeseriesflattener import TextPredictorSpec\n",
+                "from timeseriesflattener.aggregation_fns import concatenate\n",
                 "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 11,
             "metadata": {},
             "outputs": [],
             "source": [
                 "text_spec = TextPredictorSpec(\n",
-                "    values_loader=load_synth_text,\n",
+                "    timeseries_df=load_synth_text(),\n",
                 "    lookbehind_days=730,\n",
                 "    fallback=np.nan,\n",
-                "    resolve_multiple_fn=\"concatenate\",\n",
-                "    feature_name=\"text-st\",\n",
-                "    input_col_name_override=\"text\",\n",
+                "    aggregation_fn=concatenate,\n",
+                "    feature_base_name=\"text-st\",\n",
                 "    embedding_fn=sentence_transformers_embedding,\n",
-                "    embedding_fn_kwargs={\"model_name\": \"sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2\"},\n",
+                "    embedding_fn_kwargs={\n",
+                "        \"model_name\": \"sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2\"\n",
+                "    },\n",
                 ")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "That's it. Let's make our features in the usual way."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 12,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from timeseriesflattener import TimeseriesFlattener\n",
-                "from timeseriesflattener.testing.load_synth_data import load_synth_prediction_times"
+                "from timeseriesflattener.testing.load_synth_data import load_synth_prediction_times\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 13,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ts_flattener = TimeseriesFlattener(\n",
                 "    prediction_times_df=load_synth_prediction_times(),\n",
                 "    entity_id_col_name=\"entity_id\",\n",
                 "    timestamp_col_name=\"timestamp\",\n",
                 "    n_workers=1,\n",
                 "    drop_pred_times_with_insufficient_look_distance=False,\n",
                 ")\n",
-                "ts_flattener.add_spec(text_spec)"
+                "ts_flattener.add_spec(text_spec)\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "2023-02-07 11:08:40 [INFO] There were unprocessed specs, computing...\n",
-                        "2023-02-07 11:08:40 [INFO] Processing 1 temporal features in parallel with 1 workers. Chunksize is 1. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\n",
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:07<00:00,  7.37s/it]\n",
-                        "2023-02-07 11:08:47 [INFO] Checking alignment of dataframes - this might take a little while (~2 minutes for 1.000 dataframes with 2.000.000 rows).\n",
-                        "2023-02-07 11:08:47 [INFO] Starting concatenation. Will take some time on performant systems, e.g. 30s for 100 features and 2_000_000 prediction times. This is normal.\n",
-                        "2023-02-07 11:08:47 [INFO] Concatenation took 0.021 seconds\n",
-                        "2023-02-07 11:08:47 [INFO] Merging with original df\n"
+                        "2023-06-14 16:20:20 [INFO] There were unprocessed specs, computing...\n",
+                        "2023-06-14 16:20:20 [INFO] Processing 1 temporal features in parallel with 1 workers. Chunksize is 1. If this is above 1, it may take some time for the progress bar to move, as processing is batched. However, this makes for much faster total performance.\n",
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:05<00:00,  5.27s/it]\n",
+                        "2023-06-14 16:20:25 [INFO] Checking alignment of dataframes - this might take a little while (~2 minutes for 1.000 dataframes with 2.000.000 rows).\n",
+                        "2023-06-14 16:20:25 [INFO] Starting concatenation. Will take some time on performant systems, e.g. 30s for 100 features and 2_000_000 prediction times. This is normal.\n",
+                        "2023-06-14 16:20:25 [INFO] Concatenation took 0.006 seconds\n",
+                        "2023-06-14 16:20:25 [INFO] Merging with original df\n"
                     ]
                 }
             ],
             "source": [
-                "df = ts_flattener.get_df()"
+                "df = ts_flattener.get_df()\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's check the features."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 15,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -276,15 +298,15 @@
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>entity_id</th>\n",
                             "      <th>timestamp</th>\n",
                             "      <th>prediction_time_uuid</th>\n",
-                            "      <th>pred_text-st_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-0_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-1_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-2_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-3_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-4_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-5_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-6_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>...</th>\n",
@@ -430,20 +452,20 @@
                             "   entity_id           timestamp      prediction_time_uuid  \\\n",
                             "0       9903 1968-05-09 21:24:00  9903-1968-05-09-21-24-00   \n",
                             "1       7465 1966-05-24 01:23:00  7465-1966-05-24-01-23-00   \n",
                             "2       6447 1967-09-25 18:08:00  6447-1967-09-25-18-08-00   \n",
                             "3       2121 1966-05-05 20:52:00  2121-1966-05-05-20-52-00   \n",
                             "4       4927 1968-06-30 12:13:00  4927-1968-06-30-12-13-00   \n",
                             "\n",
-                            "   pred_text-st_within_730_days_concatenate_fallback_nan  \\\n",
-                            "0                                                NaN       \n",
-                            "1                                                NaN       \n",
-                            "2                                                NaN       \n",
-                            "3                                                NaN       \n",
-                            "4                                                NaN       \n",
+                            "   pred_text-st-0_within_730_days_concatenate_fallback_nan  \\\n",
+                            "0                                                NaN         \n",
+                            "1                                                NaN         \n",
+                            "2                                                NaN         \n",
+                            "3                                                NaN         \n",
+                            "4                                                NaN         \n",
                             "\n",
                             "   pred_text-st-1_within_730_days_concatenate_fallback_nan  \\\n",
                             "0                                                NaN         \n",
                             "1                                                NaN         \n",
                             "2                                                NaN         \n",
                             "3                                                NaN         \n",
                             "4                                                NaN         \n",
@@ -552,33 +574,34 @@
                             "2                                                NaN          \n",
                             "3                                                NaN          \n",
                             "4                                                NaN          \n",
                             "\n",
                             "[5 rows x 387 columns]"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df.head()"
+                "df.head()\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Because the synthetic text data is much smaller than the prediction times data, there are a lot of NaNs. Let's subset to only see the prediction times that actually include text."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 9,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -597,15 +620,15 @@
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>entity_id</th>\n",
                             "      <th>timestamp</th>\n",
                             "      <th>prediction_time_uuid</th>\n",
-                            "      <th>pred_text-st_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-0_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-1_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-2_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-3_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-4_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-5_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-6_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>...</th>\n",
@@ -633,17 +656,17 @@
                             "      <td>-0.240372</td>\n",
                             "      <td>0.105265</td>\n",
                             "      <td>0.004314</td>\n",
                             "      <td>-0.151738</td>\n",
                             "      <td>...</td>\n",
                             "      <td>0.121190</td>\n",
                             "      <td>0.381909</td>\n",
-                            "      <td>0.144212</td>\n",
+                            "      <td>0.144211</td>\n",
                             "      <td>-0.038955</td>\n",
-                            "      <td>-0.000123</td>\n",
+                            "      <td>-0.000124</td>\n",
                             "      <td>0.156520</td>\n",
                             "      <td>-0.196082</td>\n",
                             "      <td>0.080771</td>\n",
                             "      <td>0.025773</td>\n",
                             "      <td>0.193602</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
@@ -657,15 +680,15 @@
                             "      <td>0.033173</td>\n",
                             "      <td>-0.044742</td>\n",
                             "      <td>0.193883</td>\n",
                             "      <td>-0.165403</td>\n",
                             "      <td>...</td>\n",
                             "      <td>-0.236144</td>\n",
                             "      <td>0.051994</td>\n",
-                            "      <td>-0.029249</td>\n",
+                            "      <td>-0.029250</td>\n",
                             "      <td>-0.080070</td>\n",
                             "      <td>-0.105516</td>\n",
                             "      <td>0.141162</td>\n",
                             "      <td>0.008052</td>\n",
                             "      <td>-0.315303</td>\n",
                             "      <td>0.049577</td>\n",
                             "      <td>-0.070045</td>\n",
@@ -675,23 +698,23 @@
                             "      <td>2007</td>\n",
                             "      <td>1968-10-15 14:12:00</td>\n",
                             "      <td>2007-1968-10-15-14-12-00</td>\n",
                             "      <td>0.048036</td>\n",
                             "      <td>-0.050683</td>\n",
                             "      <td>0.039954</td>\n",
                             "      <td>0.038270</td>\n",
-                            "      <td>-0.208976</td>\n",
+                            "      <td>-0.208975</td>\n",
                             "      <td>-0.262620</td>\n",
                             "      <td>0.084824</td>\n",
                             "      <td>...</td>\n",
                             "      <td>-0.064676</td>\n",
                             "      <td>0.065383</td>\n",
                             "      <td>-0.030430</td>\n",
                             "      <td>-0.047385</td>\n",
-                            "      <td>-0.037472</td>\n",
+                            "      <td>-0.037471</td>\n",
                             "      <td>0.031160</td>\n",
                             "      <td>-0.191298</td>\n",
                             "      <td>0.291992</td>\n",
                             "      <td>-0.154983</td>\n",
                             "      <td>-0.043705</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
@@ -751,20 +774,20 @@
                             "      entity_id           timestamp      prediction_time_uuid  \\\n",
                             "244        7337 1966-06-28 10:34:00  7337-1966-06-28-10-34-00   \n",
                             "755        8951 1969-12-22 16:32:00  8951-1969-12-22-16-32-00   \n",
                             "896        2007 1968-10-15 14:12:00  2007-1968-10-15-14-12-00   \n",
                             "1517       1728 1968-05-29 12:27:00  1728-1968-05-29-12-27-00   \n",
                             "1917       4977 1968-11-28 16:05:00  4977-1968-11-28-16-05-00   \n",
                             "\n",
-                            "      pred_text-st_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.020497       \n",
-                            "755                                            0.069950       \n",
-                            "896                                            0.048036       \n",
-                            "1517                                           0.042505       \n",
-                            "1917                                           0.135539       \n",
+                            "      pred_text-st-0_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                           -0.020497         \n",
+                            "755                                            0.069950         \n",
+                            "896                                            0.048036         \n",
+                            "1517                                           0.042505         \n",
+                            "1917                                           0.135539         \n",
                             "\n",
                             "      pred_text-st-1_within_730_days_concatenate_fallback_nan  \\\n",
                             "244                                            0.201255         \n",
                             "755                                            0.099192         \n",
                             "896                                           -0.050683         \n",
                             "1517                                          -0.009908         \n",
                             "1917                                           0.035848         \n",
@@ -782,15 +805,15 @@
                             "896                                            0.038270         \n",
                             "1517                                          -0.005621         \n",
                             "1917                                           0.098358         \n",
                             "\n",
                             "      pred_text-st-4_within_730_days_concatenate_fallback_nan  \\\n",
                             "244                                            0.105265         \n",
                             "755                                           -0.044742         \n",
-                            "896                                           -0.208976         \n",
+                            "896                                           -0.208975         \n",
                             "1517                                          -0.085136         \n",
                             "1917                                          -0.066512         \n",
                             "\n",
                             "      pred_text-st-5_within_730_days_concatenate_fallback_nan  \\\n",
                             "244                                            0.004314         \n",
                             "755                                            0.193883         \n",
                             "896                                           -0.262620         \n",
@@ -815,31 +838,31 @@
                             "244                                            0.381909           \n",
                             "755                                            0.051994           \n",
                             "896                                            0.065383           \n",
                             "1517                                           0.319632           \n",
                             "1917                                           0.246103           \n",
                             "\n",
                             "      pred_text-st-376_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                            0.144212           \n",
-                            "755                                           -0.029249           \n",
+                            "244                                            0.144211           \n",
+                            "755                                           -0.029250           \n",
                             "896                                           -0.030430           \n",
                             "1517                                          -0.044289           \n",
                             "1917                                           0.102282           \n",
                             "\n",
                             "      pred_text-st-377_within_730_days_concatenate_fallback_nan  \\\n",
                             "244                                           -0.038955           \n",
                             "755                                           -0.080070           \n",
                             "896                                           -0.047385           \n",
                             "1517                                          -0.042798           \n",
                             "1917                                           0.031486           \n",
                             "\n",
                             "      pred_text-st-378_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.000123           \n",
+                            "244                                           -0.000124           \n",
                             "755                                           -0.105516           \n",
-                            "896                                           -0.037472           \n",
+                            "896                                           -0.037471           \n",
                             "1517                                          -0.136277           \n",
                             "1917                                          -0.336561           \n",
                             "\n",
                             "      pred_text-st-379_within_730_days_concatenate_fallback_nan  \\\n",
                             "244                                            0.156520           \n",
                             "755                                            0.141162           \n",
                             "896                                            0.031160           \n",
@@ -873,100 +896,104 @@
                             "896                                           -0.043705          \n",
                             "1517                                           0.103499          \n",
                             "1917                                          -0.023900          \n",
                             "\n",
                             "[5 rows x 387 columns]"
                         ]
                     },
-                    "execution_count": 9,
+                    "execution_count": 16,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df_pred_times_with_text = df[~df[\"pred_text-st-1_within_730_days_concatenate_fallback_nan\"].isna()]\n",
+                "df_pred_times_with_text = df[\n",
+                "    ~df[\"pred_text-st-1_within_730_days_concatenate_fallback_nan\"].isna()\n",
+                "]\n",
                 "df_pred_times_with_text.head()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Featurization using sklearn models\n",
                 "\n",
                 "If you want to embed your model using an sklearn model using e.g. TF-IDF, this can also be easily accomplished. First, you should train the sklearn model (e.g. `TfidfVectorizer`) on your dataset (using the `.fit` method). \n",
                 "\n",
                 "Now, to use your trained model in `timeseriesflattener`, simply use the `sklearn_embedding` function and supply the model as an embedding function keyword argument. \n",
                 "\n",
                 "In the following example we will use a simple CountVectorizer model, which has been pretrained on the synthetic data, to create the predictors."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "/Users/au484925/Desktop/Git/timeseriesflattener/.venv39/lib/python3.9/site-packages/sklearn/base.py:318: UserWarning: Trying to unpickle estimator CountVectorizer from version 1.1.2 when using version 1.2.2. This might lead to breaking code or invalid results. Use at your own risk. For more info please refer to:\n",
+                        "https://scikit-learn.org/stable/model_persistence.html#security-maintainability-limitations\n",
+                        "  warnings.warn(\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/html": [
                             "<style>#sk-container-id-1 {color: black;background-color: white;}#sk-container-id-1 pre{padding: 0;}#sk-container-id-1 div.sk-toggleable {background-color: white;}#sk-container-id-1 label.sk-toggleable__label {cursor: pointer;display: block;width: 100%;margin-bottom: 0;padding: 0.3em;box-sizing: border-box;text-align: center;}#sk-container-id-1 label.sk-toggleable__label-arrow:before {content: \"\u25b8\";float: left;margin-right: 0.25em;color: #696969;}#sk-container-id-1 label.sk-toggleable__label-arrow:hover:before {color: black;}#sk-container-id-1 div.sk-estimator:hover label.sk-toggleable__label-arrow:before {color: black;}#sk-container-id-1 div.sk-toggleable__content {max-height: 0;max-width: 0;overflow: hidden;text-align: left;background-color: #f0f8ff;}#sk-container-id-1 div.sk-toggleable__content pre {margin: 0.2em;color: black;border-radius: 0.25em;background-color: #f0f8ff;}#sk-container-id-1 input.sk-toggleable__control:checked~div.sk-toggleable__content {max-height: 200px;max-width: 100%;overflow: auto;}#sk-container-id-1 input.sk-toggleable__control:checked~label.sk-toggleable__label-arrow:before {content: \"\u25be\";}#sk-container-id-1 div.sk-estimator input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-label input.sk-toggleable__control:checked~label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 input.sk-hidden--visually {border: 0;clip: rect(1px 1px 1px 1px);clip: rect(1px, 1px, 1px, 1px);height: 1px;margin: -1px;overflow: hidden;padding: 0;position: absolute;width: 1px;}#sk-container-id-1 div.sk-estimator {font-family: monospace;background-color: #f0f8ff;border: 1px dotted black;border-radius: 0.25em;box-sizing: border-box;margin-bottom: 0.5em;}#sk-container-id-1 div.sk-estimator:hover {background-color: #d4ebff;}#sk-container-id-1 div.sk-parallel-item::after {content: \"\";width: 100%;border-bottom: 1px solid gray;flex-grow: 1;}#sk-container-id-1 div.sk-label:hover label.sk-toggleable__label {background-color: #d4ebff;}#sk-container-id-1 div.sk-serial::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: 0;}#sk-container-id-1 div.sk-serial {display: flex;flex-direction: column;align-items: center;background-color: white;padding-right: 0.2em;padding-left: 0.2em;position: relative;}#sk-container-id-1 div.sk-item {position: relative;z-index: 1;}#sk-container-id-1 div.sk-parallel {display: flex;align-items: stretch;justify-content: center;background-color: white;position: relative;}#sk-container-id-1 div.sk-item::before, #sk-container-id-1 div.sk-parallel-item::before {content: \"\";position: absolute;border-left: 1px solid gray;box-sizing: border-box;top: 0;bottom: 0;left: 50%;z-index: -1;}#sk-container-id-1 div.sk-parallel-item {display: flex;flex-direction: column;z-index: 1;position: relative;background-color: white;}#sk-container-id-1 div.sk-parallel-item:first-child::after {align-self: flex-end;width: 50%;}#sk-container-id-1 div.sk-parallel-item:last-child::after {align-self: flex-start;width: 50%;}#sk-container-id-1 div.sk-parallel-item:only-child::after {width: 0;}#sk-container-id-1 div.sk-dashed-wrapped {border: 1px dashed gray;margin: 0 0.4em 0.5em 0.4em;box-sizing: border-box;padding-bottom: 0.4em;background-color: white;}#sk-container-id-1 div.sk-label label {font-family: monospace;font-weight: bold;display: inline-block;line-height: 1.2em;}#sk-container-id-1 div.sk-label-container {text-align: center;}#sk-container-id-1 div.sk-container {/* jupyter's `normalize.less` sets `[hidden] { display: none; }` but bootstrap.min.css set `[hidden] { display: none !important; }` so we also need the `!important` here to be able to override the default hidden behavior on the sphinx rendered scikit-learn.org. See: https://github.com/scikit-learn/scikit-learn/issues/21755 */display: inline-block !important;position: relative;}#sk-container-id-1 div.sk-text-repr-fallback {display: none;}</style><div id=\"sk-container-id-1\" class=\"sk-top-container\"><div class=\"sk-text-repr-fallback\"><pre>CountVectorizer(max_features=10)</pre><b>In a Jupyter environment, please rerun this cell to show the HTML representation or trust the notebook. <br />On GitHub, the HTML representation is unable to render, please try loading this page with nbviewer.org.</b></div><div class=\"sk-container\" hidden><div class=\"sk-item\"><div class=\"sk-estimator sk-toggleable\"><input class=\"sk-toggleable__control sk-hidden--visually\" id=\"sk-estimator-id-1\" type=\"checkbox\" checked><label for=\"sk-estimator-id-1\" class=\"sk-toggleable__label sk-toggleable__label-arrow\">CountVectorizer</label><div class=\"sk-toggleable__content\"><pre>CountVectorizer(max_features=10)</pre></div></div></div></div></div>"
                         ],
                         "text/plain": [
                             "CountVectorizer(max_features=10)"
                         ]
                     },
-                    "execution_count": 10,
+                    "execution_count": 17,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from timeseriesflattener.text_embedding_functions import sklearn_embedding\n",
                 "from timeseriesflattener.testing.text_embedding_functions import _load_bow_model\n",
                 "\n",
                 "tfidf_model = _load_bow_model()\n",
-                "tfidf_model"
+                "tfidf_model\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 11,
+            "execution_count": 20,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "2023-02-07 11:08:48 [INFO] text-cv: Loading values\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "count_vectorizer_text_spec = TextPredictorSpec(\n",
-                "    values_loader=load_synth_text,\n",
+                "    timeseries_df=load_synth_text(),\n",
                 "    lookbehind_days=730,\n",
                 "    fallback=np.nan,\n",
-                "    resolve_multiple_fn=\"concatenate\",\n",
-                "    feature_name=\"text-cv\",\n",
-                "    input_col_name_override=\"text\",\n",
+                "    aggregation_fn=concatenate,\n",
+                "    feature_base_name=\"text-cv\",\n",
                 "    embedding_fn=sklearn_embedding,\n",
                 "    embedding_fn_kwargs={\"model\": tfidf_model},\n",
-                ")"
+                ")\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's add the feature to the dataset:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": null,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
                         "2023-02-07 11:08:48 [INFO] There were unprocessed specs, computing...\n",
@@ -979,27 +1006,28 @@
                         "2023-02-07 11:08:51 [INFO] Concatenation took 0.004 seconds\n",
                         "2023-02-07 11:08:51 [INFO] Merging with original df\n"
                     ]
                 }
             ],
             "source": [
                 "ts_flattener.add_spec(count_vectorizer_text_spec)\n",
-                "df = ts_flattener.get_df()"
+                "df = ts_flattener.get_df()\n"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Let's subset to only see the prediction times that include text again."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 21,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1018,32 +1046,32 @@
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
                             "      <th>entity_id</th>\n",
                             "      <th>timestamp</th>\n",
                             "      <th>prediction_time_uuid</th>\n",
-                            "      <th>pred_text-st_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-0_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-1_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-2_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-3_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-4_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-5_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>pred_text-st-6_within_730_days_concatenate_fallback_nan</th>\n",
                             "      <th>...</th>\n",
-                            "      <th>pred_text-cv-and_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-for_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-in_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-of_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-or_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-patient_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-that_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-the_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-to_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-was_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-374_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-375_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-376_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-377_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-378_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-379_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-380_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-381_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-382_within_730_days_concatenate_fallback_nan</th>\n",
+                            "      <th>pred_text-st-383_within_730_days_concatenate_fallback_nan</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>244</th>\n",
                             "      <td>7337</td>\n",
                             "      <td>1966-06-28 10:34:00</td>\n",
@@ -1052,140 +1080,140 @@
                             "      <td>0.201255</td>\n",
                             "      <td>-0.187649</td>\n",
                             "      <td>-0.240372</td>\n",
                             "      <td>0.105265</td>\n",
                             "      <td>0.004314</td>\n",
                             "      <td>-0.151738</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>16.0</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>2.0</td>\n",
+                            "      <td>0.121190</td>\n",
+                            "      <td>0.381909</td>\n",
+                            "      <td>0.144211</td>\n",
+                            "      <td>-0.038955</td>\n",
+                            "      <td>-0.000124</td>\n",
+                            "      <td>0.156520</td>\n",
+                            "      <td>-0.196082</td>\n",
+                            "      <td>0.080771</td>\n",
+                            "      <td>0.025773</td>\n",
+                            "      <td>0.193602</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>755</th>\n",
                             "      <td>8951</td>\n",
                             "      <td>1969-12-22 16:32:00</td>\n",
                             "      <td>8951-1969-12-22-16-32-00</td>\n",
                             "      <td>0.069950</td>\n",
                             "      <td>0.099192</td>\n",
                             "      <td>-0.007804</td>\n",
                             "      <td>0.033173</td>\n",
                             "      <td>-0.044742</td>\n",
                             "      <td>0.193883</td>\n",
                             "      <td>-0.165403</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>8.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>-0.236144</td>\n",
+                            "      <td>0.051994</td>\n",
+                            "      <td>-0.029250</td>\n",
+                            "      <td>-0.080070</td>\n",
+                            "      <td>-0.105516</td>\n",
+                            "      <td>0.141162</td>\n",
+                            "      <td>0.008052</td>\n",
+                            "      <td>-0.315303</td>\n",
+                            "      <td>0.049577</td>\n",
+                            "      <td>-0.070045</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>896</th>\n",
                             "      <td>2007</td>\n",
                             "      <td>1968-10-15 14:12:00</td>\n",
                             "      <td>2007-1968-10-15-14-12-00</td>\n",
                             "      <td>0.048036</td>\n",
                             "      <td>-0.050683</td>\n",
                             "      <td>0.039954</td>\n",
                             "      <td>0.038270</td>\n",
-                            "      <td>-0.208976</td>\n",
+                            "      <td>-0.208975</td>\n",
                             "      <td>-0.262620</td>\n",
                             "      <td>0.084824</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>6.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>13.0</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>0.0</td>\n",
+                            "      <td>-0.064676</td>\n",
+                            "      <td>0.065383</td>\n",
+                            "      <td>-0.030430</td>\n",
+                            "      <td>-0.047385</td>\n",
+                            "      <td>-0.037471</td>\n",
+                            "      <td>0.031160</td>\n",
+                            "      <td>-0.191298</td>\n",
+                            "      <td>0.291992</td>\n",
+                            "      <td>-0.154983</td>\n",
+                            "      <td>-0.043705</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1517</th>\n",
                             "      <td>1728</td>\n",
                             "      <td>1968-05-29 12:27:00</td>\n",
                             "      <td>1728-1968-05-29-12-27-00</td>\n",
                             "      <td>0.042505</td>\n",
                             "      <td>-0.009908</td>\n",
                             "      <td>-0.091326</td>\n",
                             "      <td>-0.005621</td>\n",
                             "      <td>-0.085136</td>\n",
                             "      <td>0.168317</td>\n",
                             "      <td>0.037416</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>8.0</td>\n",
-                            "      <td>11.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>11.0</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>2.0</td>\n",
+                            "      <td>0.027059</td>\n",
+                            "      <td>0.319632</td>\n",
+                            "      <td>-0.044289</td>\n",
+                            "      <td>-0.042798</td>\n",
+                            "      <td>-0.136277</td>\n",
+                            "      <td>-0.118022</td>\n",
+                            "      <td>0.169292</td>\n",
+                            "      <td>-0.029509</td>\n",
+                            "      <td>0.262050</td>\n",
+                            "      <td>0.103499</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1917</th>\n",
                             "      <td>4977</td>\n",
                             "      <td>1968-11-28 16:05:00</td>\n",
                             "      <td>4977-1968-11-28-16-05-00</td>\n",
                             "      <td>0.135539</td>\n",
                             "      <td>0.035848</td>\n",
                             "      <td>0.089571</td>\n",
                             "      <td>0.098358</td>\n",
                             "      <td>-0.066512</td>\n",
                             "      <td>-0.051096</td>\n",
                             "      <td>0.027142</td>\n",
                             "      <td>...</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>6.0</td>\n",
-                            "      <td>7.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>8.0</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>1.0</td>\n",
+                            "      <td>-0.039122</td>\n",
+                            "      <td>0.246103</td>\n",
+                            "      <td>0.102282</td>\n",
+                            "      <td>0.031486</td>\n",
+                            "      <td>-0.336561</td>\n",
+                            "      <td>-0.110646</td>\n",
+                            "      <td>0.089151</td>\n",
+                            "      <td>0.233425</td>\n",
+                            "      <td>-0.021751</td>\n",
+                            "      <td>-0.023900</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
-                            "<p>5 rows \u00d7 397 columns</p>\n",
+                            "<p>5 rows \u00d7 387 columns</p>\n",
                             "</div>"
                         ],
                         "text/plain": [
                             "      entity_id           timestamp      prediction_time_uuid  \\\n",
                             "244        7337 1966-06-28 10:34:00  7337-1966-06-28-10-34-00   \n",
                             "755        8951 1969-12-22 16:32:00  8951-1969-12-22-16-32-00   \n",
                             "896        2007 1968-10-15 14:12:00  2007-1968-10-15-14-12-00   \n",
                             "1517       1728 1968-05-29 12:27:00  1728-1968-05-29-12-27-00   \n",
                             "1917       4977 1968-11-28 16:05:00  4977-1968-11-28-16-05-00   \n",
                             "\n",
-                            "      pred_text-st_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                           -0.020497       \n",
-                            "755                                            0.069950       \n",
-                            "896                                            0.048036       \n",
-                            "1517                                           0.042505       \n",
-                            "1917                                           0.135539       \n",
+                            "      pred_text-st-0_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                           -0.020497         \n",
+                            "755                                            0.069950         \n",
+                            "896                                            0.048036         \n",
+                            "1517                                           0.042505         \n",
+                            "1917                                           0.135539         \n",
                             "\n",
                             "      pred_text-st-1_within_730_days_concatenate_fallback_nan  \\\n",
                             "244                                            0.201255         \n",
                             "755                                            0.099192         \n",
                             "896                                           -0.050683         \n",
                             "1517                                          -0.009908         \n",
                             "1917                                           0.035848         \n",
@@ -1203,15 +1231,15 @@
                             "896                                            0.038270         \n",
                             "1517                                          -0.005621         \n",
                             "1917                                           0.098358         \n",
                             "\n",
                             "      pred_text-st-4_within_730_days_concatenate_fallback_nan  \\\n",
                             "244                                            0.105265         \n",
                             "755                                           -0.044742         \n",
-                            "896                                           -0.208976         \n",
+                            "896                                           -0.208975         \n",
                             "1517                                          -0.085136         \n",
                             "1917                                          -0.066512         \n",
                             "\n",
                             "      pred_text-st-5_within_730_days_concatenate_fallback_nan  \\\n",
                             "244                                            0.004314         \n",
                             "755                                            0.193883         \n",
                             "896                                           -0.262620         \n",
@@ -1221,107 +1249,110 @@
                             "      pred_text-st-6_within_730_days_concatenate_fallback_nan  ...  \\\n",
                             "244                                           -0.151738        ...   \n",
                             "755                                           -0.165403        ...   \n",
                             "896                                            0.084824        ...   \n",
                             "1517                                           0.037416        ...   \n",
                             "1917                                           0.027142        ...   \n",
                             "\n",
-                            "      pred_text-cv-and_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 4.0           \n",
-                            "755                                                 1.0           \n",
-                            "896                                                 4.0           \n",
-                            "1517                                                1.0           \n",
-                            "1917                                                2.0           \n",
-                            "\n",
-                            "      pred_text-cv-for_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 2.0           \n",
-                            "755                                                 5.0           \n",
-                            "896                                                 0.0           \n",
-                            "1517                                                1.0           \n",
-                            "1917                                                1.0           \n",
-                            "\n",
-                            "      pred_text-cv-in_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 2.0          \n",
-                            "755                                                 1.0          \n",
-                            "896                                                 2.0          \n",
-                            "1517                                                8.0          \n",
-                            "1917                                                6.0          \n",
-                            "\n",
-                            "      pred_text-cv-of_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 5.0          \n",
-                            "755                                                 1.0          \n",
-                            "896                                                 1.0          \n",
-                            "1517                                               11.0          \n",
-                            "1917                                                7.0          \n",
-                            "\n",
-                            "      pred_text-cv-or_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 0.0          \n",
-                            "755                                                 1.0          \n",
-                            "896                                                 5.0          \n",
-                            "1517                                                0.0          \n",
-                            "1917                                                2.0          \n",
-                            "\n",
-                            "      pred_text-cv-patient_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 3.0               \n",
-                            "755                                                 2.0               \n",
-                            "896                                                 6.0               \n",
-                            "1517                                                2.0               \n",
-                            "1917                                                2.0               \n",
-                            "\n",
-                            "      pred_text-cv-that_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 1.0            \n",
-                            "755                                                 2.0            \n",
-                            "896                                                 2.0            \n",
-                            "1517                                                1.0            \n",
-                            "1917                                                1.0            \n",
-                            "\n",
-                            "      pred_text-cv-the_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                16.0           \n",
-                            "755                                                 8.0           \n",
-                            "896                                                13.0           \n",
-                            "1517                                               11.0           \n",
-                            "1917                                                8.0           \n",
-                            "\n",
-                            "      pred_text-cv-to_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 4.0          \n",
-                            "755                                                 2.0          \n",
-                            "896                                                 3.0          \n",
-                            "1517                                                5.0          \n",
-                            "1917                                                4.0          \n",
-                            "\n",
-                            "      pred_text-cv-was_within_730_days_concatenate_fallback_nan  \n",
-                            "244                                                 2.0          \n",
-                            "755                                                 0.0          \n",
-                            "896                                                 0.0          \n",
-                            "1517                                                2.0          \n",
-                            "1917                                                1.0          \n",
+                            "      pred_text-st-374_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                            0.121190           \n",
+                            "755                                           -0.236144           \n",
+                            "896                                           -0.064676           \n",
+                            "1517                                           0.027059           \n",
+                            "1917                                          -0.039122           \n",
+                            "\n",
+                            "      pred_text-st-375_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                            0.381909           \n",
+                            "755                                            0.051994           \n",
+                            "896                                            0.065383           \n",
+                            "1517                                           0.319632           \n",
+                            "1917                                           0.246103           \n",
+                            "\n",
+                            "      pred_text-st-376_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                            0.144211           \n",
+                            "755                                           -0.029250           \n",
+                            "896                                           -0.030430           \n",
+                            "1517                                          -0.044289           \n",
+                            "1917                                           0.102282           \n",
                             "\n",
-                            "[5 rows x 397 columns]"
+                            "      pred_text-st-377_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                           -0.038955           \n",
+                            "755                                           -0.080070           \n",
+                            "896                                           -0.047385           \n",
+                            "1517                                          -0.042798           \n",
+                            "1917                                           0.031486           \n",
+                            "\n",
+                            "      pred_text-st-378_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                           -0.000124           \n",
+                            "755                                           -0.105516           \n",
+                            "896                                           -0.037471           \n",
+                            "1517                                          -0.136277           \n",
+                            "1917                                          -0.336561           \n",
+                            "\n",
+                            "      pred_text-st-379_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                            0.156520           \n",
+                            "755                                            0.141162           \n",
+                            "896                                            0.031160           \n",
+                            "1517                                          -0.118022           \n",
+                            "1917                                          -0.110646           \n",
+                            "\n",
+                            "      pred_text-st-380_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                           -0.196082           \n",
+                            "755                                            0.008052           \n",
+                            "896                                           -0.191298           \n",
+                            "1517                                           0.169292           \n",
+                            "1917                                           0.089151           \n",
+                            "\n",
+                            "      pred_text-st-381_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                            0.080771           \n",
+                            "755                                           -0.315303           \n",
+                            "896                                            0.291992           \n",
+                            "1517                                          -0.029509           \n",
+                            "1917                                           0.233425           \n",
+                            "\n",
+                            "      pred_text-st-382_within_730_days_concatenate_fallback_nan  \\\n",
+                            "244                                            0.025773           \n",
+                            "755                                            0.049577           \n",
+                            "896                                           -0.154983           \n",
+                            "1517                                           0.262050           \n",
+                            "1917                                          -0.021751           \n",
+                            "\n",
+                            "      pred_text-st-383_within_730_days_concatenate_fallback_nan  \n",
+                            "244                                            0.193602          \n",
+                            "755                                           -0.070045          \n",
+                            "896                                           -0.043705          \n",
+                            "1517                                           0.103499          \n",
+                            "1917                                          -0.023900          \n",
+                            "\n",
+                            "[5 rows x 387 columns]"
                         ]
                     },
-                    "execution_count": 13,
+                    "execution_count": 21,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df_pred_times_with_text = df[~df[\"pred_text-st-1_within_730_days_concatenate_fallback_nan\"].isna()]\n",
+                "df_pred_times_with_text = df[\n",
+                "    ~df[\"pred_text-st-1_within_730_days_concatenate_fallback_nan\"].isna()\n",
+                "]\n",
                 "df_pred_times_with_text.head()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We can subset further to only include the features we created with the count vectorizer by subsetting to only include columns starting with the feature name (\"text-cv\")."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 22,
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "text/html": [
                             "<div>\n",
                             "<style scoped>\n",
@@ -1337,208 +1368,86 @@
                             "        text-align: right;\n",
                             "    }\n",
                             "</style>\n",
                             "<table border=\"1\" class=\"dataframe\">\n",
                             "  <thead>\n",
                             "    <tr style=\"text-align: right;\">\n",
                             "      <th></th>\n",
-                            "      <th>pred_text-cv-and_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-for_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-in_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-of_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-or_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-patient_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-that_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-the_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-to_within_730_days_concatenate_fallback_nan</th>\n",
-                            "      <th>pred_text-cv-was_within_730_days_concatenate_fallback_nan</th>\n",
                             "    </tr>\n",
                             "  </thead>\n",
                             "  <tbody>\n",
                             "    <tr>\n",
                             "      <th>244</th>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>16.0</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>755</th>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>8.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>896</th>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>6.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>13.0</td>\n",
-                            "      <td>3.0</td>\n",
-                            "      <td>0.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1517</th>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>8.0</td>\n",
-                            "      <td>11.0</td>\n",
-                            "      <td>0.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>11.0</td>\n",
-                            "      <td>5.0</td>\n",
-                            "      <td>2.0</td>\n",
                             "    </tr>\n",
                             "    <tr>\n",
                             "      <th>1917</th>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>6.0</td>\n",
-                            "      <td>7.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>2.0</td>\n",
-                            "      <td>1.0</td>\n",
-                            "      <td>8.0</td>\n",
-                            "      <td>4.0</td>\n",
-                            "      <td>1.0</td>\n",
                             "    </tr>\n",
                             "  </tbody>\n",
                             "</table>\n",
                             "</div>"
                         ],
                         "text/plain": [
-                            "      pred_text-cv-and_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 4.0           \n",
-                            "755                                                 1.0           \n",
-                            "896                                                 4.0           \n",
-                            "1517                                                1.0           \n",
-                            "1917                                                2.0           \n",
-                            "\n",
-                            "      pred_text-cv-for_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 2.0           \n",
-                            "755                                                 5.0           \n",
-                            "896                                                 0.0           \n",
-                            "1517                                                1.0           \n",
-                            "1917                                                1.0           \n",
-                            "\n",
-                            "      pred_text-cv-in_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 2.0          \n",
-                            "755                                                 1.0          \n",
-                            "896                                                 2.0          \n",
-                            "1517                                                8.0          \n",
-                            "1917                                                6.0          \n",
-                            "\n",
-                            "      pred_text-cv-of_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 5.0          \n",
-                            "755                                                 1.0          \n",
-                            "896                                                 1.0          \n",
-                            "1517                                               11.0          \n",
-                            "1917                                                7.0          \n",
-                            "\n",
-                            "      pred_text-cv-or_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 0.0          \n",
-                            "755                                                 1.0          \n",
-                            "896                                                 5.0          \n",
-                            "1517                                                0.0          \n",
-                            "1917                                                2.0          \n",
-                            "\n",
-                            "      pred_text-cv-patient_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 3.0               \n",
-                            "755                                                 2.0               \n",
-                            "896                                                 6.0               \n",
-                            "1517                                                2.0               \n",
-                            "1917                                                2.0               \n",
-                            "\n",
-                            "      pred_text-cv-that_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 1.0            \n",
-                            "755                                                 2.0            \n",
-                            "896                                                 2.0            \n",
-                            "1517                                                1.0            \n",
-                            "1917                                                1.0            \n",
-                            "\n",
-                            "      pred_text-cv-the_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                16.0           \n",
-                            "755                                                 8.0           \n",
-                            "896                                                13.0           \n",
-                            "1517                                               11.0           \n",
-                            "1917                                                8.0           \n",
-                            "\n",
-                            "      pred_text-cv-to_within_730_days_concatenate_fallback_nan  \\\n",
-                            "244                                                 4.0          \n",
-                            "755                                                 2.0          \n",
-                            "896                                                 3.0          \n",
-                            "1517                                                5.0          \n",
-                            "1917                                                4.0          \n",
-                            "\n",
-                            "      pred_text-cv-was_within_730_days_concatenate_fallback_nan  \n",
-                            "244                                                 2.0          \n",
-                            "755                                                 0.0          \n",
-                            "896                                                 0.0          \n",
-                            "1517                                                2.0          \n",
-                            "1917                                                1.0          "
+                            "Empty DataFrame\n",
+                            "Columns: []\n",
+                            "Index: [244, 755, 896, 1517, 1917]"
                         ]
                     },
-                    "execution_count": 14,
+                    "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "df_cv_pred_times_with_text = df_pred_times_with_text.loc[:,df_pred_times_with_text.columns.str.startswith(\"pred_text-cv\")]\n",
+                "df_cv_pred_times_with_text = df_pred_times_with_text.loc[\n",
+                "    :, df_pred_times_with_text.columns.str.startswith(\"pred_text-cv\")\n",
+                "]\n",
                 "df_cv_pred_times_with_text.head()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Notice that the text column names are informative wrt. the word they count (e.g. and, for, in, etc.). This is because `sklearn_embedding` uses the `.get_feature_names` method of the sklearn model to set the column names."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Writing your own text embedding function\n",
                 "\n",
                 "If you want to write your own embedding function, you simply need to write a function that takes a pd.Series of text as the first input and any number of optional keyword arguments. Let's write a small function to embed long texts using a Huggingface model. Note that this implementation will likely be quite slow."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 23,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from transformers import AutoTokenizer, AutoModel\n",
                 "import pandas as pd\n",
-                "import torch"
+                "import torch\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 24,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def huggingface_long_text_embedding(\n",
                 "    text_series: pd.Series, model_name: str, chunk_length: int\n",
                 ") -> pd.DataFrame:\n",
                 "    \"\"\"\n",
@@ -1564,49 +1473,42 @@
                 "        tokenized = tokenizer(\n",
                 "            text_chunks, padding=True, truncation=True, return_tensors=\"pt\"\n",
                 "        )\n",
                 "        with torch.no_grad():\n",
                 "            output = model(**tokenized)\n",
                 "        # take mean of all tokens in each chunk, then mean of all chunks\n",
                 "        embeddings.append(output[0].mean(axis=1).mean(axis=0).cpu().numpy())\n",
-                "    return pd.DataFrame(embeddings)\n"
+                "    return pd.DataFrame(embeddings)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The function can now be used as an embedding function in a `TextPredictorSpec` and used in the same manner as usual."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 26,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "2023-02-07 11:08:52 [INFO] text-hf-long: Loading values\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
                 "huggingface_long_text_spec = TextPredictorSpec(\n",
-                "    values_loader=load_synth_text,\n",
+                "    timeseries_df=load_synth_text(),\n",
                 "    lookbehind_days=730,\n",
                 "    fallback=np.nan,\n",
-                "    resolve_multiple_fn=\"concatenate\",\n",
-                "    feature_name=\"text-hf-long\",\n",
-                "    input_col_name_override=\"text\",\n",
+                "    aggregation_fn=concatenate,\n",
+                "    feature_base_name=\"text-hf-long\",\n",
                 "    embedding_fn=huggingface_long_text_embedding,\n",
                 "    embedding_fn_kwargs={\n",
-                "        \"model_name\": \"sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2\", \n",
-                "        \"chunk_length\" : 256},\n",
+                "        \"model_name\": \"sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2\",\n",
+                "        \"chunk_length\": 256,\n",
+                "    },\n",
                 ")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3.10.9 ('.venv': poetry)",
@@ -1619,15 +1521,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.9.17"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "9e85d6a49b1f06126f30ca9ae16ded22dd7c17d2dbfabea9098dc6424f12e12a"
             }
         }
```

### Comparing `timeseriesflattener-0.27.0/docs/tutorials/img/term_a.png` & `timeseriesflattener-1.0.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/tutorials/img/term_b.png` & `timeseriesflattener-1.0.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/tutorials/img/term_c.png` & `timeseriesflattener-1.0.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/docs/tutorials/img/term_d.png` & `timeseriesflattener-1.0.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/icon.png` & `timeseriesflattener-1.0.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/paper/paper.bib` & `timeseriesflattener-1.0.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/paper/paper.md` & `timeseriesflattener-1.0.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/pyproject.toml` & `timeseriesflattener-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "0.27.0"
+version = "1.0.0"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
@@ -33,20 +33,20 @@
 
 [project.license]
 file = "LICENSE"
 name = "MIT"
 [project.optional-dependencies]
 dev = [
   "cruft",
-  "pyright",  
+  "pyright==1.1.305",  
   "pre-commit==2.20.0,<2.21.0",
-  "ruff==0.0.263", # important that these match the pre-commit hooks
+  "ruff==0.0.272", # important that these match the pre-commit hooks
   "black[jupyter]==22.8.0", # important that these match the pre-commit hooks
   "pandas-stubs", # type stubs for pandas
-  "invoke",
+  "invoke==2.1.1",
   "tox",
 ]
 test = [
   "pytest>=7.1.3,<7.3.0",
   "pytest-cov>=3.0.0,<3.1.0",
   "pytest-xdist>=3.0.0,<3.2.0",
   "pytest-sugar>=0.9.4,<0.10.0",
@@ -178,25 +178,25 @@
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py{38,311}
+envlist = py39
 
 [testenv]
 description: run unit tests
 extras = test, text
 use_develop = true
 commands =
   pytest -n auto {posargs:tests}
 
 [testenv:type]
 description: run static type checking
 extras = test, text, dev
-basepython = py38
+basepython = py39
 use_develop = true
 allowlist_externals = ls
 commands =
   pyright .
 """
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/column_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """This module contains functions for handling dataframes with multiindex columns."""
 from typing import Callable, List, Optional
 
 import pandas as pd
 
-from timeseriesflattener.feature_spec_objects import TemporalSpec
+from timeseriesflattener.feature_specs.single_specs import (
+    AnySpec,
+    TemporalSpec,
+    TextPredictorSpec,
+)
 
 
 class ColumnHandler:
     """Class for handling dataframes with multiindex columns."""
 
     @staticmethod
     def embed_text_column(
@@ -39,46 +43,54 @@
         # make multiindex with embedding as 'value'
         df = pd.concat([df, embedding], axis=1, keys=["df", "value"])
         return df
 
     @staticmethod
     def rename_value_column(
         df: pd.DataFrame,
-        output_spec: TemporalSpec,
+        output_spec: AnySpec,
     ) -> pd.DataFrame:
         """Renames the value column to the column name specified in the output_spec.
         Handles the case where the output_spec has a multiindex.
 
         Args:
             output_spec (TemporalSpec): Output specification
             df (pd.DataFrame): Dataframe with value column
         """
         if isinstance(df["value"], pd.DataFrame):
+            if not isinstance(output_spec, TextPredictorSpec):
+                raise ValueError(
+                    f"output_spec must be a TextPredictorSpec if the value column is a "
+                    f"multiindex. Got {type(output_spec)}.",
+                )
             df = ColumnHandler._rename_multi_index_dataframe(output_spec, df)
         else:
-            df = df.rename(columns={"value": output_spec.get_col_str()})
+            df = df.rename(columns={"value": output_spec.get_output_col_name()})
+
         return df
 
     @staticmethod
     def _rename_multi_index_dataframe(
-        output_spec: TemporalSpec,
+        output_spec: TextPredictorSpec,
         df: pd.DataFrame,
     ) -> pd.DataFrame:
         """Renames a multiindex dataframe to the column names specified in the
         output_spec.
 
         Args:
             output_spec (TemporalSpec): Output specification
             df (pd.DataFrame): Dataframe with value column as multiindex
         """
         feature_names = df["value"].columns
+
         col_names = [
-            output_spec.get_col_str(additional_feature_name=feature_name)
+            output_spec.get_output_col_name(additional_feature_name=feature_name)
             for feature_name in feature_names
         ]
+
         feature_col_name_mapping = dict(zip(feature_names, col_names))
         # level=1 means that the column names are in the second level of the multiindex
         df = df.rename(columns=feature_col_name_mapping, level=1)
         return df
 
     @staticmethod
     def replace_na_in_spec_col_with_fallback(
@@ -92,15 +104,17 @@
         Args:
             df (pd.DataFrame): Dataframe with value column
             output_spec (TemporalSpec): Output specification
         """
         if "value" in df.columns and isinstance(df["value"], pd.DataFrame):
             df["value"] = df["value"].fillna(output_spec.fallback)  # type: ignore
         else:
-            df[output_spec.get_col_str()] = df[output_spec.get_col_str()].fillna(
+            df[output_spec.get_output_col_name()] = df[
+                output_spec.get_output_col_name()
+            ].fillna(
                 output_spec.fallback,  # type: ignore
             )
         return df
 
     @staticmethod
     def flatten_multiindex(df: pd.DataFrame) -> pd.DataFrame:
         """Checks if dataframe has multiindex columns and flattens them if it does.
@@ -123,10 +137,10 @@
         Args:
             df (pd.DataFrame): Dataframe to get value column name from.
             output_spec (TemporalSpec): Output specification"""
         if df is not None or output_spec is not None:
             return (
                 df["value"].columns.tolist()  # type: ignore
                 if isinstance(df.columns, pd.MultiIndex)  # type: ignore
-                else [output_spec.get_col_str()]  # type: ignore
+                else [output_spec.get_output_col_name()]  # type: ignore
             )
         raise ValueError("Either df or output_spec must be provided.")
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Base method that defines a feature cache."""
 from abc import ABCMeta, abstractmethod
 from typing import Any
 
 import pandas as pd
 
-from timeseriesflattener.feature_spec_objects import TemporalSpec
+from timeseriesflattener.feature_specs.single_specs import TemporalSpec
 
 
 class FeatureCache(metaclass=ABCMeta):
     """Base class that defines a feature cache."""
 
     @abstractmethod
     def __init__(
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Cache module for writing features to disk."""
 import datetime as dt
 import os
 from pathlib import Path
 from typing import Optional
 
+import numpy as np
 import pandas as pd
 
 from timeseriesflattener.feature_cache.abstract_feature_cache import FeatureCache
-from timeseriesflattener.feature_spec_objects import TemporalSpec
-from timeseriesflattener.utils import load_dataset_from_file, write_df_to_file
+from timeseriesflattener.feature_specs.single_specs import TemporalSpec
+from timeseriesflattener.misc_utils import load_dataset_from_file, write_df_to_file
 
 
 class DiskCache(FeatureCache):
     """Cache module for writing features to disk."""
 
     def __init__(
         self,
@@ -83,17 +84,17 @@
 
         Args:
             feature_spec (AnySpec): Feature spec
 
         Returns:
             str: File name
         """
-        n_rows = feature_spec.values_df.shape[0]  # type: ignore
+        n_rows = feature_spec.timeseries_df.shape[0]  # type: ignore
 
-        return f"{feature_spec.get_col_str()}_{n_rows}_rows_in_values_df"
+        return f"{feature_spec.get_output_col_name()}_{n_rows}_rows_in_values_df"
 
     def _get_file_pattern(
         self,
         feature_spec: TemporalSpec,
     ) -> str:
         """Get file pattern for feature spec.
 
@@ -125,31 +126,35 @@
             left=self.prediction_times_df[self.pred_time_uuid_col_name],
             right=df,
             how="left",
             on=self.pred_time_uuid_col_name,
             validate="m:1",
         )
 
+        fallback = np.nan if feature_spec.fallback == "nan" else feature_spec.fallback
+
         # Replace NaNs with fallback
-        df[feature_spec.get_col_str()] = df[feature_spec.get_col_str()].fillna(
-            feature_spec.fallback,  # type: ignore
+        df[feature_spec.get_output_col_name()] = df[
+            feature_spec.get_output_col_name()
+        ].fillna(
+            fallback,  # type: ignore
         )
 
         return df
 
     def write_feature(
         self,
         feature_spec: TemporalSpec,
         df: pd.DataFrame,
     ):
         """Write feature to cache."""
         file_name = self._get_file_name(feature_spec=feature_spec)
 
         # Drop rows containing fallback, since it's non-informative
-        df = df[df[feature_spec.get_col_str()] != feature_spec.fallback].dropna()  # type: ignore
+        df = df[df[feature_spec.get_output_col_name()] != feature_spec.fallback].dropna()  # type: ignore
 
         # Drop entity and timestamp columns if they exists
         for col in [self.entity_entity_id_col_name, self.timestamp_col_name]:
             if col in df.columns:
                 df = df.drop(columns=col)
 
         # Write df to cache
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/flattened_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,45 +4,48 @@
 """
 import datetime as dt
 import logging
 import random
 import time
 from datetime import timedelta
 from multiprocessing import Pool
-from typing import Callable, List, Optional, Union
+from typing import Callable, List, Optional, Sequence, Union
 
 import coloredlogs
 import numpy as np
 import pandas as pd
 import tqdm
 from pandas import DataFrame
 from pydantic import BaseModel as PydanticBaseModel
 
 from timeseriesflattener.column_handler import ColumnHandler
 from timeseriesflattener.feature_cache.abstract_feature_cache import FeatureCache
-from timeseriesflattener.feature_spec_objects import (
+from timeseriesflattener.feature_specs.single_specs import (
+    AnySpec,
     OutcomeSpec,
     PredictorSpec,
     StaticSpec,
     TemporalSpec,
     TextPredictorSpec,
-    _AnySpec,
 )
 from timeseriesflattener.flattened_ds_validator import ValidateInitFlattenedDataset
-from timeseriesflattener.utils import print_df_dimensions_diff
+from timeseriesflattener.misc_utils import print_df_dimensions_diff
 
 log = logging.getLogger(__name__)
 
 
 class SpecCollection(PydanticBaseModel):
     """A collection of specs."""
 
     outcome_specs: List[OutcomeSpec] = []
-    predictor_specs: List[PredictorSpec] = []
-    static_specs: List[_AnySpec] = []
+    predictor_specs: List[Union[PredictorSpec, TextPredictorSpec]] = []
+    static_specs: List[AnySpec] = []
+
+    class Config:
+        arbitrary_types_allowed = True
 
     def __len__(self) -> int:
         """Return number of specs in collection."""
         return (
             len(self.outcome_specs) + len(self.predictor_specs) + len(self.static_specs)
         )
 
@@ -208,51 +211,51 @@
             df,
             how="left",
             on=pred_time_uuid_colname,
             suffixes=("", "_temp"),
         )
 
     @staticmethod
-    def _resolve_multiple_values_within_interval_days(
-        resolve_multiple: Callable,
+    def _aggregate_values_within_interval_days(
+        aggregation: Callable,
         df: DataFrame,
         pred_time_uuid_colname: str,
         val_timestamp_col_name: str,
     ) -> DataFrame:
-        """Apply the resolve_multiple function to prediction_times where there
+        """Apply the aggregation function to prediction_times where there
 
         are multiple values within the interval_days lookahead.
 
         Args:
-            resolve_multiple (Callable): Takes a grouped df and collapses each group to one record (e.g. sum, count etc.).
+            aggregation (Callable): Takes a grouped df and collapses each group to one record (e.g. sum, count etc.).
             df (DataFrame): Source dataframe with all prediction time x val combinations.
             pred_time_uuid_colname (str): Name of uuid column in df.
             val_timestamp_col_name (str): Name of timestamp column in df.
 
         Returns:
             DataFrame: DataFrame with one row pr. prediction time.
         """
-        # Convert timestamp val to numeric that can be used for resolve_multiple functions
+        # Convert timestamp val to numeric that can be used for aggregation functions
         # Numeric value amounts to days passed since 1/1/1970
         try:
             df[val_timestamp_col_name] = (
                 df[val_timestamp_col_name] - dt.datetime(1970, 1, 1)
             ).dt.total_seconds() / 86400
         except TypeError:
             log.info("All values are NaT, returning empty dataframe")
 
-        # Sort by timestamp_pred in case resolve_multiple needs dates
+        # Sort by timestamp_pred in case aggregation needs dates
         grouped_df = df.sort_values(by=val_timestamp_col_name).groupby(
             pred_time_uuid_colname,
         )
 
-        if callable(resolve_multiple):
-            df = resolve_multiple(grouped_df).reset_index()
+        if callable(aggregation):
+            df = aggregation(grouped_df).reset_index()
         else:
-            raise ValueError("resolve_multiple must be or resolve to a Callable")
+            raise ValueError("aggregation must be or resolve to a Callable")
 
         return df
 
     @staticmethod
     def _drop_records_outside_interval_days(
         df: DataFrame,
         direction: str,
@@ -331,66 +334,64 @@
         Returns:
             DataFrame
         """
         # Generate df with one row for each prediction time x event time combination
         # Drop id for faster merge
         df = pd.merge(
             left=prediction_times_with_uuid_df,
-            right=output_spec.values_df,
+            right=output_spec.timeseries_df,
             how="left",
             on=entity_id_col_name,
             suffixes=("_pred", "_val"),
             validate="m:m",
         ).drop(entity_id_col_name, axis=1)
 
         timestamp_val_col_name = f"{timestamp_col_name}_val"
         timestamp_pred_col_name = f"{timestamp_col_name}_pred"
-        df = TimeseriesFlattener.rename_input_col_to_value(
-            df=df,
-            output_spec=output_spec,
-        )
 
         # Drop prediction times without event times within interval days
         if isinstance(output_spec, OutcomeSpec):
             direction = "ahead"
-        elif isinstance(output_spec, PredictorSpec):
+            interval_days = output_spec.lookahead_days
+        elif isinstance(output_spec, (PredictorSpec, TextPredictorSpec)):
             direction = "behind"
+            interval_days = output_spec.lookbehind_days
         else:
             raise ValueError(f"Unknown output_spec type {type(output_spec)}")
 
         df = TimeseriesFlattener._drop_records_outside_interval_days(
             df,
             direction=direction,
-            interval_days=output_spec.interval_days,  # type: ignore
+            interval_days=interval_days,
             timestamp_pred_colname=timestamp_pred_col_name,
             timestamp_value_colname=timestamp_val_col_name,
         )
 
         df[timestamp_val_col_name].replace(
             {output_spec.fallback: pd.NaT},
             inplace=True,  # noqa
         )
 
-        df = TimeseriesFlattener._resolve_multiple_values_within_interval_days(
-            resolve_multiple=output_spec.resolve_multiple_fn,  # type: ignore
+        df = TimeseriesFlattener._aggregate_values_within_interval_days(
+            aggregation=output_spec.aggregation_fn,  # type: ignore
             df=df,
             pred_time_uuid_colname=pred_time_uuid_col_name,
             val_timestamp_col_name=timestamp_val_col_name,
         )
 
         # handle embedding and dimensionality reduction if text predictor
         if isinstance(output_spec, TextPredictorSpec):
             df = ColumnHandler.embed_text_column(
                 df=df,
                 text_col_name="value",
                 embedding_fn=output_spec.embedding_fn,
                 embedding_fn_kwargs=output_spec.embedding_fn_kwargs,
             )
 
-        # If resolve_multiple generates empty values,
+        # If aggregation generates empty values,
         # e.g. when there is only one prediction_time within look_ahead window for slope calculation,
         # replace with NaN
 
         # Rename column
         df = ColumnHandler.rename_value_column(df=df, output_spec=output_spec)
 
         # Find value_cols and add fallback to them
@@ -403,39 +404,28 @@
             output_spec=output_spec,
         )
 
         # check if multiindex and flatten
         df = ColumnHandler.flatten_multiindex(df)
         if verbose:
             log.info(
-                f"Returning {df.shape[0]} rows of flattened dataframe for {output_spec.get_col_str()}",
+                f"Returning {df.shape[0]} rows of flattened dataframe for {output_spec.get_output_col_name()}",
             )
 
         # Add back prediction times that don't have a value, and fill them with fallback
         df = TimeseriesFlattener._add_back_prediction_times_without_value(
             df=df,
             pred_times_with_uuid=prediction_times_with_uuid_df,
             pred_time_uuid_colname=pred_time_uuid_col_name,
         ).fillna(
             output_spec.fallback,  # type: ignore
         )
 
         return df[[*value_col_str_name, pred_time_uuid_col_name]]
 
-    @staticmethod
-    def rename_input_col_to_value(
-        df: pd.DataFrame,
-        output_spec: TemporalSpec,
-    ) -> pd.DataFrame:
-        """Checks whether 'value' is a column in df, and if not, renames the
-        input column"""
-        if "value" not in df.columns:
-            df = df.rename(columns={output_spec.input_col_name_override: "value"})
-        return df
-
     def _get_temporal_feature(
         self,
         feature_spec: TemporalSpec,
     ) -> pd.DataFrame:
         """Get feature. Either load from cache, or generate if necessary.
 
         Args:
@@ -443,19 +433,21 @@
 
         Returns:
             pd.DataFrame: Feature
         """
         if self.cache:
             if self.cache.feature_exists(feature_spec=feature_spec):
                 log.debug(
-                    f"Cache hit for {feature_spec.get_col_str()}, loading from cache",
+                    f"Cache hit for {feature_spec.get_output_col_name()}, loading from cache",
                 )
                 df = self.cache.read_feature(feature_spec=feature_spec)
                 return df.set_index(keys=self.pred_time_uuid_col_name).sort_index()
-            log.debug(f"Cache miss for {feature_spec.get_col_str()}, generating")
+            log.debug(
+                f"Cache miss for {feature_spec.get_output_col_name()}, generating",
+            )
         elif not self.cache:
             log.debug("No cache specified, not attempting load")
 
         df = self._flatten_temporal_values_to_df(
             prediction_times_with_uuid_df=self._df[
                 [
                     self.pred_time_uuid_col_name,
@@ -584,51 +576,48 @@
 
         self._concatenate_flattened_timeseries(
             flattened_predictor_dfs=flattened_predictor_dfs,
         )
 
     def _add_static_info(
         self,
-        static_spec: _AnySpec,
+        static_spec: AnySpec,
     ):
         """Add static info to each prediction time, e.g. age, sex etc.
 
         Args:
             static_spec (StaticSpec): Specification for the static info to add.
 
         Raises:
             ValueError: If input_col_name does not match a column in info_df.
         """
         # Try to infer value col name if not provided
-        if static_spec.input_col_name_override is None:
-            possible_value_cols = [
-                col
-                for col in static_spec.values_df.columns  # type: ignore
-                if col not in self.entity_id_col_name
-            ]
-
-            if len(possible_value_cols) == 1:
-                value_col_name = possible_value_cols[0]
-            elif len(possible_value_cols) > 1:
-                raise ValueError(
-                    f"Only one value column can be added to static info, found multiple: {possible_value_cols}",
-                )
-            elif len(possible_value_cols) == 0:
-                raise ValueError(
-                    "No value column found in spec.df, please check.",
-                )
-        else:
-            value_col_name = static_spec.input_col_name_override
+        possible_value_cols = [
+            col
+            for col in static_spec.timeseries_df.columns  # type: ignore
+            if col not in self.entity_id_col_name
+        ]
+
+        if len(possible_value_cols) == 1:
+            value_col_name = possible_value_cols[0]
+        elif len(possible_value_cols) > 1:
+            raise ValueError(
+                f"Only one value column can be added to static info, found multiple: {possible_value_cols}",
+            )
+        elif len(possible_value_cols) == 0:
+            raise ValueError(
+                "No value column found in spec.df, please check.",
+            )
 
-        output_col_name = static_spec.get_col_str()
+        output_col_name = static_spec.get_output_col_name()
 
         df = pd.DataFrame(
             {
-                self.entity_id_col_name: static_spec.values_df[self.entity_id_col_name],  # type: ignore
-                output_col_name: static_spec.values_df[value_col_name],  # type: ignore
+                self.entity_id_col_name: static_spec.timeseries_df[self.entity_id_col_name],  # type: ignore
+                output_col_name: static_spec.timeseries_df[value_col_name],  # type: ignore
             },
         )
 
         self._df = pd.merge(
             self._df,
             df,
             how="left",
@@ -655,15 +644,15 @@
         Can be done vectorized, hence the separate function.
         """
         prediction_timestamp_col_name = f"{self.timestamp_col_name}_prediction"
         outcome_timestamp_col_name = f"{self.timestamp_col_name}_outcome"
 
         df = pd.merge(
             self._df,
-            outcome_spec.values_df,
+            outcome_spec.timeseries_df,
             how="left",
             on=self.entity_id_col_name,
             suffixes=("_prediction", "_outcome"),
             validate="m:1",
         )
 
         df = df.drop(
@@ -671,19 +660,21 @@
                 df[outcome_timestamp_col_name] < df[prediction_timestamp_col_name]
             ].index,
         )
 
         if outcome_spec.is_dichotomous():
             outcome_is_within_lookahead = (
                 df[prediction_timestamp_col_name]  # type: ignore
-                + timedelta(days=outcome_spec.interval_days)  # type: ignore
+                + timedelta(days=outcome_spec.lookahead_days)
                 > df[outcome_timestamp_col_name]
             )
 
-            df[outcome_spec.get_col_str()] = outcome_is_within_lookahead.astype(int)
+            df[outcome_spec.get_output_col_name()] = outcome_is_within_lookahead.astype(
+                int,
+            )
 
         df = df.rename(
             {prediction_timestamp_col_name: "timestamp"},
             axis=1,
         )
         df = df.drop([outcome_timestamp_col_name], axis=1)
 
@@ -700,19 +691,19 @@
         there will necessarily be fewer outcomes - without that reflecting reality. This means our model won't generalise.
 
         Returns:
             pd.Timestamp: A cutoff date.
         """
 
         if isinstance(spec, PredictorSpec):
-            min_val_date = spec.values_df[self.timestamp_col_name].min()  # type: ignore
+            min_val_date = spec.timeseries_df[self.timestamp_col_name].min()  # type: ignore
             return min_val_date + pd.Timedelta(days=spec.lookbehind_days)
 
         if isinstance(spec, OutcomeSpec):
-            max_val_date = spec.values_df[self.timestamp_col_name].max()  # type: ignore
+            max_val_date = spec.timeseries_df[self.timestamp_col_name].max()  # type: ignore
             return max_val_date - pd.Timedelta(days=spec.lookahead_days)
 
         raise ValueError(f"Spec type {type(spec)} not recognised.")
 
     @print_df_dimensions_diff
     def _drop_pred_time_if_insufficient_look_distance(
         self,
@@ -787,94 +778,96 @@
         if len(temporal_batch) > 0:
             self._add_temporal_batch(temporal_batch=temporal_batch)
 
         # Remove the processed specs
         self.unprocessed_specs.outcome_specs = []
         self.unprocessed_specs.predictor_specs = []
 
-    def _check_that_spec_df_has_required_columns(self, spec: _AnySpec):
+    def _check_that_spec_df_has_required_columns(self, spec: AnySpec):
         """Check that df has required columns."""
         # Find all attributes in self that contain col_name
         required_columns = [self.entity_id_col_name]
 
         if not isinstance(spec, StaticSpec):
             required_columns += [self.timestamp_col_name]
 
         for col in required_columns:
-            if col not in spec.values_df.columns:  # type: ignore
-                raise ValueError(f"Missing required column: {col}")
+            if col not in spec.timeseries_df.columns:  # type: ignore
+                raise KeyError(f"Missing required column: {col}")
 
     def _check_that_spec_df_timestamp_col_is_correctly_formatted(
         self,
         spec: TemporalSpec,
     ):
         """Check that timestamp column is correctly formatted. Attempt to coerce if possible."""
-        timestamp_col_type = spec.values_df[self.timestamp_col_name].dtype  # type: ignore
+        timestamp_col_type = spec.timeseries_df[self.timestamp_col_name].dtype  # type: ignore
 
         if timestamp_col_type not in ("Timestamp", "datetime64[ns]"):
             # Convert column dtype to datetime64[ns] if it isn't already
             log.info(
-                f"{spec.feature_name}: Converting timestamp column to datetime64[ns]",
+                f"{spec.feature_base_name}: Converting timestamp column to datetime64[ns]",
             )
 
-            spec.values_df[self.timestamp_col_name] = pd.to_datetime(  # type: ignore
-                spec.values_df[self.timestamp_col_name],  # type: ignore
+            spec.timeseries_df[self.timestamp_col_name] = pd.to_datetime(  # type: ignore
+                spec.timeseries_df[self.timestamp_col_name],  # type: ignore
             )
 
-            min_timestamp = min(spec.values_df[self.timestamp_col_name])  # type: ignore
+            min_timestamp = min(spec.timeseries_df[self.timestamp_col_name])  # type: ignore
 
             if min_timestamp < pd.Timestamp("1971-01-01"):
                 log.warning(
-                    f"{spec.feature_name}: Minimum timestamp is {min_timestamp} - perhaps ints were coerced to timestamps?",
+                    f"{spec.feature_base_name}: Minimum timestamp is {min_timestamp} - perhaps ints were coerced to timestamps?",
                 )
 
     def add_spec(
         self,
-        spec: Union[List[_AnySpec], _AnySpec],
+        spec: Union[Sequence[AnySpec], AnySpec],
     ):
         """Add a specification to the flattened dataset.
 
         This adds it to a queue of unprocessed specs, which are not processed
         until you call the .compute() or .get_df() methods. This allows us to
         more effectiely parallelise the processing of the specs.
 
         Most of the complexity lies in the OutcomeSpec and PredictorSpec objects.
         For further documentation, see those objects and the tutorial.
         """
-        if isinstance(spec, _AnySpec):
-            specs_to_process: List[_AnySpec] = [spec]
-        else:
-            specs_to_process = spec
+        specs_to_process = [spec] if not isinstance(spec, Sequence) else spec
 
         for spec_i in specs_to_process:
-            allowed_spec_types = (OutcomeSpec, PredictorSpec, StaticSpec)
+            allowed_spec_types = (
+                OutcomeSpec,
+                PredictorSpec,
+                StaticSpec,
+                TextPredictorSpec,
+            )
 
             if not isinstance(spec_i, allowed_spec_types):
                 raise ValueError(
                     f"Input is not allowed. Must be one of: {allowed_spec_types}",
                 )
 
             self._check_that_spec_df_has_required_columns(spec=spec_i)
 
-            if isinstance(spec_i, TemporalSpec):
+            if isinstance(spec_i, (PredictorSpec, OutcomeSpec, TextPredictorSpec)):
                 self._check_that_spec_df_timestamp_col_is_correctly_formatted(
-                    spec=spec_i,
+                    spec=spec_i,  # type: ignore
                 )
 
             if isinstance(spec_i, OutcomeSpec):
                 self.unprocessed_specs.outcome_specs.append(spec_i)
-            elif isinstance(spec_i, PredictorSpec):
+            elif isinstance(spec_i, (PredictorSpec, TextPredictorSpec)):
                 self.unprocessed_specs.predictor_specs.append(spec_i)
             elif isinstance(spec_i, StaticSpec):
                 self.unprocessed_specs.static_specs.append(spec_i)
 
     def add_age(
         self,
         date_of_birth_df: DataFrame,
-        date_of_birth_col_name: Optional[str] = "date_of_birth",
+        date_of_birth_col_name: str = "date_of_birth",
         output_prefix: str = "pred",
     ):
         """Add age at prediction time as predictor.
 
         Has its own function because of its very frequent use.
 
         Args:
@@ -894,21 +887,20 @@
                     f"Conversion of {date_of_birth_col_name} to datetime failed, doesn't match format %Y-%m-%d. Recommend converting to datetime before adding.",
                 ) from e
 
         output_age_col_name = f"{output_prefix}_age_in_years"
 
         tmp_prefix = "tmp"
         self._add_static_info(
-            static_spec=_AnySpec(
-                values_df=date_of_birth_df,
-                input_col_name_override=date_of_birth_col_name,
+            static_spec=StaticSpec(
+                timeseries_df=date_of_birth_df,
                 prefix=tmp_prefix,
+                feature_base_name=date_of_birth_col_name,
                 # We typically don't want to use date of birth as a predictor,
                 # but might want to use transformations - e.g. "year of birth" or "age at prediction time".
-                feature_name=date_of_birth_col_name,
             ),
         )
 
         tmp_date_of_birth_col_name = f"{tmp_prefix}_{date_of_birth_col_name}"
 
         self._df[output_age_col_name] = (
             (
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Validator for a flattened dataset."""
 import pandas as pd
 
-from timeseriesflattener.utils import df_contains_duplicates
+from timeseriesflattener.misc_utils import df_contains_duplicates
 
 
 class ValidateInitFlattenedDataset:
     """Validator for a flattened dataset."""
 
     def __init__(
         self,
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/logger.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 from pathlib import Path
 from typing import Optional, Union
 
 import coloredlogs
 
-from timeseriesflattener.utils import PROJECT_ROOT
+from timeseriesflattener.misc_utils import PROJECT_ROOT
 
 
 def setup_logger(
     name: str,
     level: int = logging.DEBUG,
     log_file_path: Optional[Union[str, Path]] = None,
     fmt: str = "%(asctime)s [%(levelname)s] %(message)s",
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,83 +1,81 @@
 """Loaders for synth data."""
 
 import logging
 from typing import Optional
 
 import pandas as pd
-from timeseriesflattener.utils import PROJECT_ROOT, data_loaders
+from timeseriesflattener.misc_utils import PROJECT_ROOT
 
 log = logging.getLogger(__name__)
 
+TEST_DATA_PATH = PROJECT_ROOT / "src" / "timeseriesflattener" / "testing" / "test_data"
+
 
 def load_raw_test_csv(filename: str, n_rows: Optional[int] = None) -> pd.DataFrame:
     """Load raw csv.
 
     Args:
         filename (str): Name of the file to load.
         n_rows (int, optional): Number of rows to load. Defaults to None.
     """
     df = pd.read_csv(
-        PROJECT_ROOT / "tests" / "test_data" / "raw" / filename,
+        TEST_DATA_PATH / "raw" / filename,
         nrows=n_rows,
     )
 
     # Convert timestamp col to datetime
     if "timestamp" in df.columns:
         df["timestamp"] = pd.to_datetime(df["timestamp"])
 
     return df
 
 
-@data_loaders.register("synth_predictor_float")
 def load_synth_predictor_float(
     n_rows: Optional[int] = None,
 ) -> pd.DataFrame:
     """Load synth predictor data.".
 
     Args:
         n_rows: Number of rows to return. Defaults to None which returns entire coercion data view.
 
     Returns:
         pd.DataFrame
     """
     return load_raw_test_csv("synth_raw_float_1.csv", n_rows=n_rows)
 
 
-@data_loaders.register("synth_sex")
 def load_synth_sex(
     n_rows: Optional[int] = None,
 ) -> pd.DataFrame:
     """Load synth sex data.".
 
     Args:
         n_rows: Number of rows to return. Defaults to None which returns entire coercion data view.
 
     Returns:
         pd.DataFrame
     """
     return load_raw_test_csv("synth_sex.csv", n_rows=n_rows)
 
 
-@data_loaders.register("synth_predictor_binary")
 def synth_predictor_binary(
     n_rows: Optional[int] = None,
 ) -> pd.DataFrame:
     """Load synth predictor data.".
 
     Args:
         n_rows: Number of rows to return. Defaults to None which returns entire coercion data view.
 
     Returns:
         pd.DataFrame
     """
     return load_raw_test_csv("synth_raw_binary_1.csv", n_rows=n_rows)
 
 
-@data_loaders.register("synth_outcome")
 def load_synth_outcome(
     n_rows: Optional[int] = None,
 ) -> pd.DataFrame:
     """Load synth predictor data.".
 
     Args:
         n_rows: Number of rows to return. Defaults to None which returns entire coercion data view.
@@ -90,35 +88,35 @@
     df = df.groupby("entity_id").last().reset_index()
 
     # Drop all rows with a value equal to 1
     df = df[df["value"] == 1]
     return df
 
 
-@data_loaders.register("synth_prediction_times")
 def load_synth_prediction_times(
     n_rows: Optional[int] = None,
 ) -> pd.DataFrame:
     """Load synth predictor data.".
 
     Args:
         n_rows: Number of rows to return. Defaults to None which returns entire coercion data view.
 
     Returns:
         pd.DataFrame
     """
     return load_raw_test_csv("synth_prediction_times.csv", n_rows=n_rows)
 
 
-@data_loaders.register("synth_text")
 def load_synth_text(
     n_rows: Optional[int] = None,
 ) -> pd.DataFrame:
     """Load synth text data.".
 
     Args:
         n_rows: Number of rows to return. Defaults to None which returns entire coercion data view.
 
     Returns:
         pd.DataFrame
     """
-    return load_raw_test_csv("synth_text_data.csv", n_rows=n_rows)
+    df = load_raw_test_csv("synth_text_data.csv", n_rows=n_rows)
+    df["value"] = df["text"]
+    return df
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import pickle as pkl
 from pathlib import Path
 
 import pandas as pd
 from pandas import DataFrame, Series
 from sklearn.decomposition import PCA
 from sklearn.feature_extraction.text import CountVectorizer
-from timeseriesflattener.utils import PROJECT_ROOT
+from timeseriesflattener.testing.load_synth_data import TEST_DATA_PATH
 
 
 def _load_bow_model() -> CountVectorizer:
     """Loads the bag-of-words model from a pickle file"""
-    filename = PROJECT_ROOT / "tests" / "test_data" / "models" / "synth_bow_model.pkl"
+    filename = TEST_DATA_PATH / "models" / "synth_bow_model.pkl"
 
     with Path(filename).open("rb") as f:
         return pkl.load(f)
 
 
 def _load_pca_model() -> PCA:
     """Loads the PCA model from a pickle file"""
-    filename = PROJECT_ROOT / "tests" / "test_data" / "models" / "synth_pca_model.pkl"
+    filename = TEST_DATA_PATH / "models" / "synth_pca_model.pkl"
 
     with Path(filename).open("rb") as f:
         return pkl.load(f)
 
 
 def bow_test_embedding(text_series: Series) -> DataFrame:
     """Embeds the text data using a bag-of-words model"""
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from typing import Any, List, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
 from pandas.testing import assert_series_equal
 from timeseriesflattener import TimeseriesFlattener
-from timeseriesflattener.feature_spec_objects import _AnySpec
+from timeseriesflattener.feature_specs.single_specs import AnySpec
 from timeseriesflattener.testing.load_synth_data import (
     synth_predictor_binary,
 )
-from timeseriesflattener.utils import data_loaders
 
 
 def convert_cols_with_matching_colnames_to_datetime(
     df: DataFrame,
     colname_substr: str,
 ) -> DataFrame:
     """Convert columns that contain colname_substr in their name to datetimes.
@@ -69,29 +68,29 @@
 
     # Drop "Unnamed" cols
     return df.loc[:, ~df.columns.str.contains("^Unnamed")]
 
 
 def _get_value_cols_based_on_spec(
     df: pd.DataFrame,
-    spec: _AnySpec,
+    spec: AnySpec,
 ) -> Union[str, List[str]]:
     """Get value columns based on spec. Checks if multiple value columns are present."""
-    feature_name = spec.feature_name
+    feature_name = spec.feature_base_name
     value_cols = df.columns[df.columns.str.contains(feature_name)].tolist()
     # to avoid indexing issues
     if len(value_cols) == 1:
         return value_cols[0]
 
     return value_cols
 
 
 def assert_flattened_data_as_expected(
     prediction_times_df: Union[pd.DataFrame, str],
-    output_spec: _AnySpec,
+    output_spec: AnySpec,
     expected_df: Optional[pd.DataFrame] = None,
     expected_values: Optional[Sequence[Any]] = None,
 ):
     """Flatten spec and assert that flattened data is as expected."""
     if isinstance(prediction_times_df, str):
         prediction_times_df = str_to_df(prediction_times_df)
 
@@ -109,17 +108,17 @@
         for col in expected_df.columns:
             assert_series_equal(
                 left=flattened_ds.get_df()[col],
                 right=expected_df[col],
                 check_dtype=False,
             )
     elif expected_values:
-        output = flattened_ds.get_df()
-        value_cols = _get_value_cols_based_on_spec(output, output_spec)
-        output = flattened_ds.get_df()[value_cols].values.tolist()
+        output_df = flattened_ds.get_df()
+        value_cols = _get_value_cols_based_on_spec(output_df, output_spec)
+        output = output_df[value_cols].values.tolist()
         expected = list(expected_values)
 
         for i, expected_val in enumerate(expected):
             # NaN != NaN, hence specific handling
             if not isinstance(expected_val, (str, list)) and np.isnan(expected_val):
                 assert np.isnan(output[i])
             else:
@@ -141,15 +140,14 @@
         var_name="value_names",
         value_name="value",
     )
 
     return long_df
 
 
-@data_loaders.register("load_event_times")
 def load_event_times() -> DataFrame:
     """Load event times."""
     event_times_str = """entity_id,timestamp,value,
                     1,2021-12-30 00:00:01, 1
                     1,2021-12-29 00:00:02, 2
                     """
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener/utils.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 0.27.0
+Version: 1.0.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
         
@@ -97,32 +97,30 @@
             "value": [1, 2, 3, 4],
         },
     )
     # Load a dataframe specifying when the outcome occurs
     outcome_df = pd.DataFrame({"id": [1], "date": ["2020-03-01"], "value": [1]})
 
     # Specify how to aggregate the predictors and define the outcome
-    from timeseriesflattener.feature_spec_objects import OutcomeSpec, PredictorSpec
-    from timeseriesflattener.resolve_multiple_functions import maximum, mean
+    from timeseriesflattener.feature_specs.single_specs import OutcomeSpec, PredictorSpec
+    from timeseriesflattener.aggregation_fns import maximum, mean
 
     predictor_spec = PredictorSpec(
-        values_df=predictor_df,
+        timeseries_df=predictor_df,
         lookbehind_days=30,
         fallback=np.nan,
-        entity_id_col_name="id",
-        resolve_multiple_fn=mean,
-        feature_name="test_feature",
+        aggregation_fn=mean,
+        feature_base_name="test_feature",
     )
     outcome_spec = OutcomeSpec(
-        values_df=outcome_df,
+        timeseries_df=outcome_df,
         lookahead_days=31,
         fallback=0,
-        entity_id_col_name="id",
-        resolve_multiple_fn=maximum,
-        feature_name="test_outcome",
+        aggregation_fn=maximum,
+        feature_base_name="test_outcome",
         incident=False,
     )
 
     # Instantiate TimeseriesFlattener and add the specifications
     from timeseriesflattener import TimeseriesFlattener
 
     ts_flattener = TimeseriesFlattener(
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 0.27.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.0.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
@@ -61,23 +61,22 @@
 pd.DataFrame( { "id": [1, 1, 2], "date": ["2020-01-01", "2020-02-01", "2020-02-
 01"], }, ) # Load a dataframe with raw values you wish to aggregate as
 predictors predictor_df = pd.DataFrame( { "id": [1, 1, 1, 2], "date": [ "2020-
 01-15", "2019-12-10", "2019-12-15", "2020-01-02", ], "value": [1, 2, 3, 4], },
 ) # Load a dataframe specifying when the outcome occurs outcome_df =
 pd.DataFrame({"id": [1], "date": ["2020-03-01"], "value": [1]}) # Specify how
 to aggregate the predictors and define the outcome from
-timeseriesflattener.feature_spec_objects import OutcomeSpec, PredictorSpec from
-timeseriesflattener.resolve_multiple_functions import maximum, mean
-predictor_spec = PredictorSpec( values_df=predictor_df, lookbehind_days=30,
-fallback=np.nan, entity_id_col_name="id", resolve_multiple_fn=mean,
-feature_name="test_feature", ) outcome_spec = OutcomeSpec
-( values_df=outcome_df, lookahead_days=31, fallback=0, entity_id_col_name="id",
-resolve_multiple_fn=maximum, feature_name="test_outcome", incident=False, ) #
-Instantiate TimeseriesFlattener and add the specifications from
-timeseriesflattener import TimeseriesFlattener ts_flattener =
+timeseriesflattener.feature_specs.single_specs import OutcomeSpec,
+PredictorSpec from timeseriesflattener.aggregation_fns import maximum, mean
+predictor_spec = PredictorSpec( timeseries_df=predictor_df, lookbehind_days=30,
+fallback=np.nan, aggregation_fn=mean, feature_base_name="test_feature", )
+outcome_spec = OutcomeSpec( timeseries_df=outcome_df, lookahead_days=31,
+fallback=0, aggregation_fn=maximum, feature_base_name="test_outcome",
+incident=False, ) # Instantiate TimeseriesFlattener and add the specifications
+from timeseriesflattener import TimeseriesFlattener ts_flattener =
 TimeseriesFlattener( prediction_times_df=prediction_times_df,
 entity_id_col_name="id", timestamp_col_name="date", n_workers=1,
 drop_pred_times_with_insufficient_look_distance=False, ) ts_flattener.add_spec(
 [predictor_spec, outcome_spec]) df = ts_flattener.get_df() df ``` Output: | |
 id | date | prediction_time_uuid |
 pred_test_feature_within_30_days_mean_fallback_nan |
 outc_test_outcome_within_31_days_maximum_fallback_0_dichotomous | | ---: | ---:
```

### Comparing `timeseriesflattener-0.27.0/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 protobuf<=4.22.3
 frozendict>=2.3.4
 coloredlogs>14.0.0
 psycopmlutils>=0.5.0
 
 [dev]
 cruft
-pyright
+pyright==1.1.305
 pre-commit<2.21.0,==2.20.0
-ruff==0.0.263
+ruff==0.0.272
 black[jupyter]==22.8.0
 pandas-stubs
-invoke
+invoke==2.1.1
 tox
 
 [docs]
 sphinx<7.1.0,>=5.3.0
 furo==2023.3.27
 sphinx-copybutton<0.5.3,>=0.5.1
 sphinxext-opengraph<0.8.3,>=0.7.3
```

### Comparing `timeseriesflattener-0.27.0/tasks.py` & `timeseriesflattener-1.0.0/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,14 +243,15 @@
     pytest_args: List[str] = [],  # noqa
 ):
     """Run tests"""
     echo_header(f"{Emo.TEST} Running tests")
 
     if len(pytest_args) == 0:
         pytest_args = [
+            "src",
             "-n auto",
             "-rfE",
             "--failed-first",
             "-p no:cov",
             "--disable-warnings",
             "-q",
         ]
@@ -306,19 +307,27 @@
     """Lint the project using the pre-commit hooks and mypy."""
     test_for_rej()
     pre_commit(c=c, auto_fix=auto_fix)
     static_type_checks(c)
 
 
 @task
+def test_tutorials(c: Context):
+    c.run(
+        "find docs/tutorials -name '*.ipynb' | grep -v 'nbconvert' | xargs jupyter nbconvert --to notebook --execute",
+    )
+
+
+@task
 def pr(c: Context, auto_fix: bool = False):
     """Run all checks and update the PR."""
     add_and_commit(c)
     lint(c, auto_fix=auto_fix)
     test(c, python_versions="3.8,3.11")
+    test_tutorials(c)
     update_branch(c)
     update_pr(c)
 
 
 @task
 def docs(c: Context, view: bool = False, view_only: bool = False):
     """
```

### Comparing `timeseriesflattener-0.27.0/tests/conftest.py` & `timeseriesflattener-1.0.0/src/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 from pandas import DataFrame
+from timeseriesflattener.feature_specs.group_specs import NamedDataframe
 from timeseriesflattener.testing.load_synth_data import (
     load_synth_outcome,
     load_synth_prediction_times,
     load_synth_text,
 )
 from timeseriesflattener.testing.utils_for_testing import (
     load_long_df_with_multiple_values,
@@ -60,7 +61,18 @@
     return load_long_df_with_multiple_values()
 
 
 @pytest.fixture()
 def synth_text_data() -> DataFrame:
     """Load the synth text data."""
     return load_synth_text()
+
+
+@pytest.fixture()
+def empty_df() -> DataFrame:
+    """Create an empty dataframe."""
+    return DataFrame()
+
+
+@pytest.fixture()
+def empty_named_df() -> NamedDataframe:
+    return NamedDataframe(df=DataFrame(), name="empty")
```

### Comparing `timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Generate dataframe with prediction times."""
 
 from psycop_ml_utils.synth_data_generator.synth_col_generators import (
     generate_data_columns,
 )
-from timeseriesflattener.utils import PROJECT_ROOT
+from timeseriesflattener.misc_utils import PROJECT_ROOT
 
 if __name__ == "__main__":
     # Get project root directory
 
     column_specs = {
         "entity_id": {
             "column_type": "uniform_int",
```

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Generate raw float dataframe."""
 
 from psycop_ml_utils.synth_data_generator.synth_col_generators import (
     generate_data_columns,
 )
-from timeseriesflattener.utils import PROJECT_ROOT
+from timeseriesflattener.misc_utils import PROJECT_ROOT
 
 if __name__ == "__main__":
     # Get project root directory
 
     column_specs = [
         {
             "entity_id": {
```

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/create_synth_sex.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/synth_sex.csv` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_data/raw/synth_text_data.csv` & `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-0.27.0/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Testing of the DiskCache class."""
 
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from pandas.testing import assert_frame_equal
+from timeseriesflattener.aggregation_fns import latest
 from timeseriesflattener.feature_cache.cache_to_disk import DiskCache
-from timeseriesflattener.feature_spec_objects import PredictorSpec
-from timeseriesflattener.resolve_multiple_functions import latest
+from timeseriesflattener.feature_specs.single_specs import PredictorSpec
 
 
 def test_write_and_check_feature(
     tmp_path: Path,
 ):
     """Test that write_feature writes a feature to disk."""
 
@@ -31,28 +31,27 @@
             "pred_time_uuid": [1, 2, 3],
             "timestamp": [1, 2, 3],
             "value": [1, 2, 3],
         },
     )
 
     test_spec = PredictorSpec(
-        values_df=values_df,
+        feature_base_name="test_feature",
+        timeseries_df=values_df,
         lookbehind_days=5,
-        resolve_multiple_fn=latest,
-        key_for_resolve_multiple="latest",
+        aggregation_fn=latest,
         fallback=np.nan,
-        feature_name="test_feature",
     )
 
     generated_df = pd.DataFrame(
         {
             "entity_id": [1, 2, 3],
             "pred_time_uuid": [1, 2, 3],
             "timestamp": [1, 2, 3],
-            f"{test_spec.get_col_str()}": [1, 2, 3],
+            f"{test_spec.get_output_col_name()}": [1, 2, 3],
         },
     )
 
     assert cache.feature_exists(feature_spec=test_spec) is False
 
     cache.write_feature(feature_spec=test_spec, df=generated_df)
 
@@ -86,32 +85,31 @@
             "entity_id": [1, 2, 3, 4, 5],
             "timestamp": [1, 2, 3, 4, 5],
             "value": [1, 2, 3, 4, 5],
         },
     )
 
     test_spec = PredictorSpec(
-        values_df=values_df,
-        interval_days=5,
-        resolve_multiple_fn=latest,
-        key_for_resolve_multiple="latest",
-        fallback=np.nan,
-        feature_name="test_feature",
+        timeseries_df=values_df,
+        lookbehind_days=5,
+        aggregation_fn=latest,
+        fallback=np.NaN,
+        feature_base_name="test_feature",
     )
 
     generated_df = pd.DataFrame(
         {
             "entity_id": [
                 1,
                 2,
                 3,
             ],
             "pred_time_uuid": [1, 2, 3],
             "timestamp": [1, 2, 3],
-            f"{test_spec.get_col_str()}": [1, 2, np.nan],
+            f"{test_spec.get_output_col_name()}": [1, 2, np.nan],
         },
     )
 
     cache.write_feature(feature_spec=test_spec, df=generated_df)
 
     df = cache.read_feature(feature_spec=test_spec)
```

### Comparing `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tests for the text embedding functions"""
 import pandas as pd
 import pytest
+
 from timeseriesflattener.testing.text_embedding_functions import bow_test_embedding
 from timeseriesflattener.text_embedding_functions import (
     huggingface_embedding,
     sentence_transformers_embedding,
 )
```

### Comparing `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Tests for adding values to a flattened dataset."""
 
 
 import numpy as np
 import pandas as pd
 import pytest
+
 from timeseriesflattener import TimeseriesFlattener
-from timeseriesflattener.feature_spec_objects import (
+from timeseriesflattener.aggregation_fns import concatenate, maximum, minimum
+from timeseriesflattener.feature_specs.single_specs import (
     OutcomeSpec,
     PredictorSpec,
     StaticSpec,
     TextPredictorSpec,
 )
 from timeseriesflattener.testing.text_embedding_functions import bow_test_embedding
 from timeseriesflattener.testing.utils_for_testing import (
@@ -30,19 +32,19 @@
     1,2022-01-01 00:00:01, 1.0
     """,
     )
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_df,
         output_spec=PredictorSpec(
-            values_df=predictor_df,
+            timeseries_df=predictor_df,
             lookbehind_days=2,
-            resolve_multiple_fn="max",
+            aggregation_fn=maximum,
             fallback=np.NaN,
-            feature_name="value",
+            feature_base_name="value",
         ),
         expected_values=[np.NaN],
     )
 
 
 def test_predictor_before_prediction():
     prediction_times_df = """entity_id,timestamp,
@@ -51,19 +53,19 @@
     predictor_df_str = """entity_id,timestamp,value,
                         1,2021-12-30 22:59:59, 1
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_df,
         output_spec=PredictorSpec(
-            values_df=str_to_df(predictor_df_str),
+            timeseries_df=str_to_df(predictor_df_str),
             lookbehind_days=2,
-            resolve_multiple_fn="max",
+            aggregation_fn=maximum,
             fallback=np.NaN,
-            feature_name="value",
+            feature_base_name="value",
         ),
         expected_values=[1],
     )
 
 
 def test_text_predictor():
     prediction_times_df = """entity_id,timestamp,
@@ -72,20 +74,20 @@
     predictor_df_str = """entity_id,timestamp,value,
                         1,2021-12-30 22:59:59, "hello world"
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_df,
         output_spec=TextPredictorSpec(
-            values_df=str_to_df(predictor_df_str),
+            timeseries_df=str_to_df(predictor_df_str),
             embedding_fn=bow_test_embedding,
             lookbehind_days=1,
-            resolve_multiple_fn="concatenate",
+            aggregation_fn=concatenate,
             fallback=np.NaN,
-            feature_name="text_value",
+            feature_base_name="text_value",
         ),
         expected_values=[[0] * 10],
     )
 
 
 def test_multiple_citizens_predictor():
     prediction_times_df_str = """entity_id,timestamp,
@@ -102,19 +104,19 @@
                         5,2022-01-04 00:00:01, 2
                         7,2022-01-05 00:00:00, 5
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_df_str,
         output_spec=PredictorSpec(
-            values_df=str_to_df(predictor_df_str),
-            interval_days=2,
+            timeseries_df=str_to_df(predictor_df_str),
+            lookbehind_days=2,
             fallback=np.NaN,
-            feature_name="value",
-            resolve_multiple_fn="max",
+            feature_base_name="value",
+            aggregation_fn=maximum,
         ),
         expected_values=[0, 1, 0, 2, np.NaN],
     )
 
 
 # Outcomes
 def test_event_after_prediction_time():
@@ -124,20 +126,20 @@
     outcome_df_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:01, 1
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_df_str,
         output_spec=OutcomeSpec(
-            values_df=str_to_df(outcome_df_str),
+            timeseries_df=str_to_df(outcome_df_str),
             lookahead_days=2,
-            resolve_multiple_fn="max",
+            aggregation_fn=maximum,
             incident=True,
             fallback=np.NaN,
-            feature_name="value",
+            feature_base_name="value",
         ),
         expected_values=[1],
     )
 
 
 def test_event_before_prediction():
     prediction_times_df_str = """entity_id,timestamp,
@@ -146,20 +148,20 @@
     outcome_df_str = """entity_id,timestamp,value,
                         1,2021-12-30 23:59:59, 1.0
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_df_str,
         output_spec=OutcomeSpec(
-            values_df=str_to_df(outcome_df_str),
+            timeseries_df=str_to_df(outcome_df_str),
             lookahead_days=2,
-            resolve_multiple_fn="max",
+            aggregation_fn=maximum,
             incident=False,
             fallback=np.NaN,
-            feature_name="value",
+            feature_base_name="value",
         ),
         expected_values=[np.NaN],
     )
 
 
 def test_multiple_citizens_outcome():
     prediction_times_df_str = """entity_id,timestamp,
@@ -174,20 +176,20 @@
                         5,2025-01-03 00:00:00, 1.0
                         5,2022-01-05 00:00:01, 1.0
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_df_str,
         output_spec=OutcomeSpec(
-            values_df=str_to_df(outcome_df_str),
+            timeseries_df=str_to_df(outcome_df_str),
             lookahead_days=2,
-            resolve_multiple_fn="max",
+            aggregation_fn=maximum,
             incident=False,
             fallback=np.NaN,
-            feature_name="value",
+            feature_base_name="value",
         ),
         expected_values=[1, np.NaN, 1, np.NaN],
     )
 
 
 def test_citizen_without_outcome():
     prediction_times_df_str = """entity_id,timestamp,
@@ -196,20 +198,20 @@
     outcome_df_str = """entity_id,timestamp,value,
                         0,2021-12-31 00:00:01, 1.0
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_df_str,
         output_spec=OutcomeSpec(
-            values_df=str_to_df(outcome_df_str),
+            timeseries_df=str_to_df(outcome_df_str),
             lookahead_days=2,
-            resolve_multiple_fn="max",
+            aggregation_fn=maximum,
             incident=False,
             fallback=np.NaN,
-            feature_name="value",
+            feature_base_name="value",
         ),
         expected_values=[np.NaN],
     )
 
 
 def test_static_predictor():
     prefix = "meta"
@@ -228,18 +230,17 @@
     dataset = TimeseriesFlattener(
         prediction_times_df=str_to_df(prediction_times_df),
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     dataset.add_spec(
         StaticSpec(  # type: ignore
-            values_df=str_to_df(static_predictor),
-            feature_name=feature_name,
+            timeseries_df=str_to_df(static_predictor),
+            feature_base_name=feature_name,
             prefix=prefix,
-            input_col_name_override=feature_name,
         ),
     )
 
     expected_values = pd.DataFrame(
         {
             output_col_name: [
                 "1994-12-31 00:00:01",
@@ -328,15 +329,15 @@
                             """
 
     event_times_str = """entity_id,timestamp,value,
                         1,2021-12-31 00:00:01, 1
                         2,2021-12-31 00:00:01, 1
                         """
 
-    expected_df_str = """entity_id,timestamp,outc_value_within_2_days_max_fallback_nan_dichotomous,
+    expected_df_str = """entity_id,timestamp,outc_value_within_2_days_maximum_fallback_nan_dichotomous,
                         1,2021-12-31 00:00:00, 1.0
                         2,2021-12-31 00:00:00, 1.0
                         3,2023-12-31 00:00:00, 0.0
                         """
 
     prediction_times_df = str_to_df(prediction_times_str)
     event_times_df = str_to_df(event_times_str)
@@ -348,20 +349,20 @@
         entity_id_col_name="entity_id",
         n_workers=4,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     flattened_dataset.add_spec(
         spec=OutcomeSpec(
-            values_df=event_times_df,
-            interval_days=2,
+            timeseries_df=event_times_df,
+            lookahead_days=2,
             incident=True,
             fallback=np.NaN,
-            feature_name="value",
-            resolve_multiple_fn="max",
+            feature_base_name="value",
+            aggregation_fn=maximum,
         ),
     )
 
     outcome_df = flattened_dataset.get_df().reset_index(drop=True)
 
     for col in expected_df.columns:
         pd.testing.assert_series_equal(
@@ -381,15 +382,15 @@
                             """
 
     event_times_str = """entity_id,timestamp,value,
                         1,2021-12-31 00:00:01, 1
                         2,2021-12-31 00:00:01, 1
                         """
 
-    expected_df_str = """entity_id,timestamp,outc_value_within_2_days_max_fallback_0_dichotomous,pred_age_in_years,pred_male_overridden
+    expected_df_str = """entity_id,timestamp,outc_value_within_2_days_maximum_fallback_0_dichotomous,pred_age_in_years,pred_male
                         1,2021-12-31 00:00:00, 1.0,22.00,1
                         2,2021-12-31 00:00:00, 1.0,22.00,0
                         3,2023-12-31 00:00:00, 0.0,23.99,1
                         """
 
     birthdates_df_str = """entity_id,date_of_birth,
     1,2000-01-01,
@@ -412,48 +413,46 @@
         timestamp_col_name="timestamp",
         entity_id_col_name="entity_id",
         n_workers=4,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     output_spec = OutcomeSpec(
-        values_df=event_times_df,
-        interval_days=2,
-        resolve_multiple_fn="max",
+        timeseries_df=event_times_df,
+        lookahead_days=2,
+        aggregation_fn=maximum,
         fallback=0,
         incident=True,
-        feature_name="value",
+        feature_base_name="value",
     )
 
     flattened_dataset.add_spec(
         spec=[
             output_spec,
             StaticSpec(  # type: ignore
-                values_df=male_df,
-                feature_name="male",
+                timeseries_df=male_df,
+                feature_base_name="male",
                 prefix="pred",
-                input_col_name_override="male",
-                output_col_name_override="pred_male_overridden",
             ),
         ],
     )
 
     flattened_dataset.add_age(
         date_of_birth_col_name="date_of_birth",
         date_of_birth_df=birthdates_df,
     )
 
     outcome_df = flattened_dataset.get_df()
 
     for col in (
         "entity_id",
         "timestamp",
-        "outc_value_within_2_days_max_fallback_0_dichotomous",
+        "outc_value_within_2_days_maximum_fallback_0_dichotomous",
         "pred_age_in_years",
-        "pred_male_overridden",
+        "pred_male",
     ):
         pd.testing.assert_series_equal(
             outcome_df[col].reset_index(drop=True),
             expected_df[col].reset_index(drop=True),
             check_dtype=False,
         )
 
@@ -492,28 +491,27 @@
         n_workers=4,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     flattened_dataset.add_spec(
         spec=[
             PredictorSpec(
-                values_df=predictors_df,
-                interval_days=365,
-                resolve_multiple_fn="min",
+                timeseries_df=predictors_df,
+                lookbehind_days=365,
+                aggregation_fn=minimum,
                 fallback=np.nan,
-                allowed_nan_value_prop=0,
-                feature_name="value",
+                feature_base_name="value",
             ),
             OutcomeSpec(
-                values_df=event_times_df,
-                interval_days=2,
-                resolve_multiple_fn="max",
+                timeseries_df=event_times_df,
+                lookahead_days=2,
+                aggregation_fn=maximum,
                 fallback=0,
                 incident=True,
-                feature_name="value",
+                feature_base_name="value",
             ),
         ],
     )
 
     outcome_df = flattened_dataset.get_df().set_index("entity_id").sort_index()
     expected_df = expected_df.set_index("entity_id").sort_index()
 
@@ -533,15 +531,15 @@
                             1,2023-11-05 00:00:00
                             """
 
     event_times_str = """entity_id,timestamp,value,
                         1,2021-11-06 00:00:01, 1
                         """
 
-    expected_df_str = """outc_value_within_2_days_max_fallback_nan_dichotomous,
+    expected_df_str = """outc_value_within_2_days_maximum_fallback_nan_dichotomous,
     1
     0"""
 
     prediction_times_df = str_to_df(prediction_times_str)
     event_times_df = str_to_df(event_times_str)
     expected_df = str_to_df(expected_df_str)
 
@@ -551,20 +549,20 @@
         entity_id_col_name="entity_id",
         n_workers=4,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     flattened_dataset.add_spec(
         spec=OutcomeSpec(
-            values_df=event_times_df,
-            interval_days=2,
+            timeseries_df=event_times_df,
+            lookahead_days=2,
             incident=True,
             fallback=np.NaN,
-            feature_name="value",
-            resolve_multiple_fn="max",
+            feature_base_name="value",
+            aggregation_fn=maximum,
         ),
     )
 
     outcome_df = flattened_dataset.get_df()
 
     for col in [c for c in expected_df.columns if "outc" in c]:
         for df in (outcome_df, expected_df):
```

### Comparing `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,41 +3,48 @@
 
 from pathlib import Path
 from typing import List
 
 import numpy as np
 import pandas as pd
 import pytest
+
+from timeseriesflattener.aggregation_fns import maximum, mean
 from timeseriesflattener.feature_cache.cache_to_disk import DiskCache
-from timeseriesflattener.feature_spec_objects import PredictorGroupSpec, PredictorSpec
+from timeseriesflattener.feature_specs.group_specs import (
+    NamedDataframe,
+    PredictorGroupSpec,
+)
+from timeseriesflattener.feature_specs.single_specs import PredictorSpec
 from timeseriesflattener.testing.load_synth_data import (
     load_synth_prediction_times,
+    load_synth_predictor_float,
+    synth_predictor_binary,
 )
-
-from tests.test_timeseriesflattener.test_flattened_dataset.utils import (
+from timeseriesflattener.tests.test_timeseriesflattener.test_flattened_dataset.utils import (
     check_dfs_have_same_contents_by_column,
     create_flattened_df,
 )
 
 base_float_predictor_combinations = PredictorGroupSpec(
-    values_loader=["synth_predictor_float"],
+    named_dataframes=[
+        NamedDataframe(df=load_synth_predictor_float(), name="synth_predictor_float"),
+    ],
     lookbehind_days=[365, 730],
-    resolve_multiple_fn=["mean"],
+    aggregation_fns=[mean],
     fallback=[np.NaN],
-    allowed_nan_value_prop=[0.0],
-    feature_name="test_feature",
 ).create_combinations()
 
 base_binary_predictor_combinations = PredictorGroupSpec(
-    values_loader=["synth_predictor_binary"],
+    named_dataframes=[
+        NamedDataframe(df=synth_predictor_binary(), name="synth_predictor_binary"),
+    ],
     lookbehind_days=[365, 730],
-    resolve_multiple_fn=["max"],
+    aggregation_fns=[maximum],
     fallback=[np.NaN],
-    allowed_nan_value_prop=[0.0],
-    feature_name="test_feature",
 ).create_combinations()
 
 
 @pytest.mark.parametrize(
     "predictor_specs",
     [base_float_predictor_combinations, base_binary_predictor_combinations],
 )
```

### Comparing `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 import uuid
 from typing import Any, Callable, List
 
 import pandas as pd
 import pytest
 from pandas import DataFrame
+
 from timeseriesflattener.flattened_dataset import TimeseriesFlattener
 
 
 def benchmark(func: Callable, *args: Any, **kwargs: Any) -> float:
     """Benchmark a function."""
     start = time.perf_counter()
     func(*args, **kwargs)
@@ -51,15 +52,15 @@
     # 0.033 seconds for 9 dfs when sampling 100_000 rows
     # 7.622 seconds for 100 dfs when sampling 2_000_000 rows
     compute_seconds = benchmark(
         TimeseriesFlattener._check_dfs_are_ready_for_concat,
         dfs,
     )
 
-    assert compute_seconds < 2
+    assert compute_seconds < 4
 
 
 def test_error_raised_with_unaligend_rows():
     """Test that an error is raised when the rows are not aligned"""
     n_rows = 2_000_000
     uuids = [uuid.uuid4().hex[:16] for _ in range(n_rows)]
     random_ints = [1 for _ in range(n_rows)]
```

### Comparing `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Tests for errors raised from flattened dataset class."""
 
 import pytest
-from timeseriesflattener.feature_spec_objects import PredictorSpec
+
+from timeseriesflattener.aggregation_fns import maximum
+from timeseriesflattener.feature_specs.single_specs import PredictorSpec
 from timeseriesflattener.flattened_dataset import TimeseriesFlattener
 from timeseriesflattener.testing.utils_for_testing import (
     str_to_df,
 )
 
 
 def test_col_does_not_exist_in_prediction_times():
@@ -43,19 +45,19 @@
         entity_id_col_name="entity_id",
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     with pytest.raises(KeyError):
         flattened_df.add_spec(
             spec=PredictorSpec(
-                values_df=event_times_df,
-                interval_days=2,
-                resolve_multiple_fn="max",
+                timeseries_df=event_times_df,
+                lookbehind_days=2,
+                aggregation_fn=maximum,
                 fallback=2,
-                feature_name="value",
+                feature_base_name="value",
             ),
         )
 
 
 def test_duplicate_prediction_times():
     with pytest.raises(ValueError, match=r".*Duplicate.*"):  # noqa
         prediction_times_df_str = """entity_id,timestamp,
```

### Comparing `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """Larger tests for the `flattened_dataset.py` module."""
 import numpy as np
 import pandas as pd
 import pytest
-from timeseriesflattener.feature_spec_objects import (
+
+from timeseriesflattener.aggregation_fns import concatenate, latest, mean
+from timeseriesflattener.feature_specs.group_specs import (
+    NamedDataframe,
+    TextPredictorGroupSpec,
+)
+from timeseriesflattener.feature_specs.single_specs import (
     OutcomeSpec,
     PredictorSpec,
     StaticSpec,
-    TextPredictorGroupSpec,
     TextPredictorSpec,
 )
 from timeseriesflattener.flattened_dataset import TimeseriesFlattener
-from timeseriesflattener.resolve_multiple_functions import latest, mean
+from timeseriesflattener.testing.load_synth_data import load_synth_text
 from timeseriesflattener.testing.text_embedding_functions import (
     _load_bow_model,
 )
 from timeseriesflattener.text_embedding_functions import (
     sentence_transformers_embedding,
     sklearn_embedding,
 )
@@ -25,31 +30,31 @@
     dataset = TimeseriesFlattener(
         prediction_times_df=synth_prediction_times,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     # Create sample specs
     outcome_spec = OutcomeSpec(
-        values_df=synth_outcome,
-        feature_name="outcome",
+        timeseries_df=synth_outcome,
+        feature_base_name="outcome",
         lookahead_days=1,
-        resolve_multiple_fn=mean,
+        aggregation_fn=mean,
         fallback=0,
         incident=False,
     )
     predictor_spec = PredictorSpec(
-        values_df=synth_outcome,
-        feature_name="predictor",
+        timeseries_df=synth_outcome,
+        feature_base_name="predictor",
         lookbehind_days=1,
-        resolve_multiple_fn=mean,
+        aggregation_fn=mean,
         fallback=np.nan,
     )
     static_spec = StaticSpec(
-        values_df=synth_outcome,
-        feature_name="static",
+        timeseries_df=synth_outcome,
+        feature_base_name="static",
         prefix="pred",
     )
 
     # Test adding a single spec
     dataset.add_spec(outcome_spec)
     assert dataset.unprocessed_specs.outcome_specs == [outcome_spec]
 
@@ -71,41 +76,42 @@
 ):
     # Create an instance of the class that contains the `add_spec` method
     dataset = TimeseriesFlattener(
         prediction_times_df=synth_prediction_times,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
+    synth_text_data["value"] = synth_text_data["text"]
+
     # Create sample specs
     outcome_spec = OutcomeSpec(
-        values_df=synth_outcome,
-        feature_name="outcome",
+        timeseries_df=synth_outcome,
+        feature_base_name="outcome",
         lookahead_days=1,
-        resolve_multiple_fn=mean,
+        aggregation_fn=mean,
         fallback=0,
         incident=False,
     )
     predictor_spec = PredictorSpec(
-        values_df=synth_outcome,
-        feature_name="predictor",
+        timeseries_df=synth_outcome,
+        feature_base_name="predictor",
         lookbehind_days=1,
-        resolve_multiple_fn=mean,
+        aggregation_fn=mean,
         fallback=np.nan,
     )
     static_spec = StaticSpec(
-        values_df=synth_outcome[["value", "entity_id"]],
-        feature_name="static",
+        timeseries_df=synth_outcome[["value", "entity_id"]],
+        feature_base_name="static",
         prefix="pred",
     )
     text_spec = TextPredictorSpec(  # type: ignore
-        values_df=synth_text_data,
-        feature_name="text",
+        timeseries_df=synth_text_data,
+        feature_base_name="text",
         lookbehind_days=750,
-        input_col_name_override="text",
-        resolve_multiple_fn="concatenate",
+        aggregation_fn=concatenate,
         fallback=np.nan,
         embedding_fn=sentence_transformers_embedding,
         embedding_fn_kwargs={
             "model_name": "sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2",
         },
     )
 
@@ -139,35 +145,35 @@
             "datetime": ["2022-01-01"],
             "value": [1],
         },
     )
 
     # Create a sample set of specs
     predictor_spec = PredictorSpec(
-        values_df=pred_val_df,
+        timeseries_df=pred_val_df,
         lookbehind_days=1,
-        resolve_multiple_fn=latest,
+        aggregation_fn=latest,
         fallback=np.nan,
-        feature_name="test_feature",
+        feature_base_name="test_feature",
     )
 
     out_val_df = pd.DataFrame(
         {
             "entity_id": [1],
             "datetime": ["2022-01-05"],
             "value": [4],
         },
     )
 
     outcome_spec = OutcomeSpec(
-        values_df=out_val_df,
+        timeseries_df=out_val_df,
         lookahead_days=2,
-        resolve_multiple_fn=latest,
+        aggregation_fn=latest,
         fallback=np.nan,
-        feature_name="test_feature",
+        feature_base_name="test_feature",
         incident=False,
     )
 
     ts_flattener.add_spec(spec=[predictor_spec, outcome_spec])
 
     out_df = ts_flattener.get_df()
 
@@ -200,20 +206,19 @@
                 "2020-03-16",
             ],
             "value": [1, 2, 3, 4, 4, 5, 6],
         },
     )
 
     predictor_spec = PredictorSpec(
-        values_df=predictor_df,
+        timeseries_df=predictor_df,
         lookbehind_days=15,
         fallback=np.nan,
-        entity_id_col_name="entity_id",
-        resolve_multiple_fn=mean,
-        feature_name="test_feature",
+        aggregation_fn=mean,
+        feature_base_name="test_feature",
     )
 
     ts_flattener = TimeseriesFlattener(
         prediction_times_df=prediction_times_df,
         entity_id_col_name="entity_id",
         timestamp_col_name="date",
         n_workers=1,
@@ -234,34 +239,33 @@
     dataset = TimeseriesFlattener(
         prediction_times_df=synth_prediction_times,
         drop_pred_times_with_insufficient_look_distance=False,
     )
 
     # Create sample specs
     outcome_spec = OutcomeSpec(
-        values_df=synth_outcome,
-        feature_name="outcome",
+        timeseries_df=synth_outcome,
+        feature_base_name="outcome",
         lookahead_days=1,
-        resolve_multiple_fn=mean,
+        aggregation_fn=mean,
         fallback=0,
         incident=False,
     )
 
     bow_model = _load_bow_model()
 
     predictor_spec = TextPredictorGroupSpec(
-        values_loader=("synth_text",),
+        named_dataframes=[NamedDataframe(df=load_synth_text(), name="synth_text")],
         prefix="test",
-        resolve_multiple_fn=["concatenate"],
+        aggregation_fns=[concatenate],
         fallback=[np.nan],
         lookbehind_days=[100],
-        feature_name="bow",
+        embedding_fn_name="bow",
         embedding_fn=[sklearn_embedding],
         embedding_fn_kwargs=[{"model": bow_model}],
-        input_col_name_override="text",
     ).create_combinations()
 
     dataset.add_spec(outcome_spec)
     dataset.add_spec(predictor_spec)  # type: ignore
 
     df = dataset.get_df()
```

### Comparing `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Integration test for the flattened dataset generation."""
 
 
 from typing import List, Optional
 
 import numpy as np
 import pandas as pd
+
 from timeseriesflattener.feature_cache.abstract_feature_cache import FeatureCache
-from timeseriesflattener.feature_spec_objects import PredictorSpec
+from timeseriesflattener.feature_specs.single_specs import PredictorSpec
 from timeseriesflattener.flattened_dataset import TimeseriesFlattener
 
 
 def check_dfs_have_same_contents_by_column(df1: pd.DataFrame, df2: pd.DataFrame):
     """Check that two dataframes have the same contents by column.
 
     Makes debugging much easier, as it generates a diff df which is easy to read.
```

### Comparing `timeseriesflattener-0.27.0/tests/test_timeseriesflattener/test_resolve_multiple.py` & `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,111 +1,106 @@
-"""Tests of resolve_multiple strategies."""
+"""Tests of aggregation strategies."""
 
 
 import numpy as np
-from timeseriesflattener.feature_spec_objects import OutcomeSpec, PredictorSpec
+
+from timeseriesflattener.aggregation_fns import (
+    boolean,
+    change_per_day,
+    concatenate,
+    count,
+    earliest,
+    latest,
+    maximum,
+    mean,
+    mean_number_of_characters,
+    minimum,
+    summed,
+    type_token_ratio,
+    variance,
+)
+from timeseriesflattener.feature_specs.single_specs import (
+    OutcomeSpec,
+    PredictorSpec,
+)
 from timeseriesflattener.testing.utils_for_testing import (
     assert_flattened_data_as_expected,
     str_to_df,
 )
 
 
-def test_resolve_multiple_catalogue():
-    """Test that resolve_multiple functions can be retrieved from catalogue."""
-    prediction_times_str = """entity_id,timestamp,
-                            1,2021-12-31 00:00:00
-                            """
-    event_times_str = """entity_id,timestamp,value,
-                        1,2022-01-01 00:00:01, 1
-                        1,2022-01-01 00:00:02, 2
-                        """
-
-    assert_flattened_data_as_expected(
-        prediction_times_df=prediction_times_str,
-        output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="min",
-            interval_days=2,
-            fallback=0,
-            incident=False,
-        ),
-        expected_values=[1],
-    )
-
-
-def test_resolve_multiple_max():
+def test_aggregation_max():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:01, 1
                         1,2022-01-01 00:00:02, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="max",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=maximum,
+            lookahead_days=2,
             fallback=0,
             incident=False,
         ),
         expected_values=[2],
     )
 
 
-def test_resolve_multiple_min():
+def test_aggregation_min():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:01, 1
                         1,2022-01-01 00:00:02, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="min",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=minimum,
+            lookahead_days=2,
             fallback=0,
             incident=False,
         ),
         expected_values=[1],
     )
 
 
-def test_resolve_multiple_avg():
+def test_aggregation_avg():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 08:00:00
                             """
     predictor_df_str = """entity_id,timestamp,value,
                         1,2021-12-30 00:00:01, 1
                         1,2021-12-30 00:00:02, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=PredictorSpec(
-            feature_name="value",
-            values_df=str_to_df(predictor_df_str),
-            resolve_multiple_fn="mean",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(predictor_df_str),
+            aggregation_fn=mean,
+            lookbehind_days=2,
             fallback=0,
         ),
         expected_values=[1.5],
     )
 
 
-def test_resolve_multiple_latest():
+def test_aggregation_latest():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:01, 1
                         1,2022-01-01 00:00:03, 3
@@ -114,72 +109,72 @@
                         2,2022-01-01 00:00:03, 9
                         2,2022-01-01 00:00:02, 6
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="latest",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=latest,
+            lookahead_days=2,
             fallback=0,
             incident=False,
         ),
         expected_values=[3, 9],
     )
 
 
-def test_resolve_multiple_latest_no_values():
+def test_aggregation_latest_no_values():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:01, 1
                         1,2022-01-01 00:00:02, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="latest",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=latest,
+            lookahead_days=2,
             fallback=np.nan,
             incident=False,
         ),
         expected_values=[2, np.nan],
     )
 
 
-def test_resolve_multiple_latest_one_vlaue():
+def test_aggregation_latest_one_vlaue():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:01, 1
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="latest",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=latest,
+            lookahead_days=2,
             fallback=0,
             incident=False,
         ),
         expected_values=[1],
     )
 
 
-def test_resolve_multiple_earliest():
+def test_aggregation_earliest():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:03, 3
                         1,2022-01-01 00:00:01, 1
@@ -188,312 +183,312 @@
                         2,2022-01-01 00:00:01, 1
                         2,2022-01-01 00:00:02, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="earliest",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=earliest,
+            lookahead_days=2,
             fallback=0,
             incident=False,
         ),
         expected_values=[1, 1],
     )
 
 
-def test_resolve_multiple_sum():
+def test_aggregation_sum():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             """
     predictor_df_str = """entity_id,timestamp,value,
                         1,2021-12-30 00:00:01, 1
                         1,2021-12-30 00:00:02, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=PredictorSpec(
-            feature_name="value",
-            values_df=str_to_df(predictor_df_str),
-            resolve_multiple_fn="sum",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(predictor_df_str),
+            aggregation_fn=summed,
+            lookbehind_days=2,
             fallback=0,
         ),
         expected_values=[3],
     )
 
 
-def test_resolve_multiple_count():
+def test_aggregation_count():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:01, 1
                         1,2022-01-01 00:00:02, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="count",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=count,
+            lookahead_days=2,
             fallback=0,
             incident=False,
         ),
         expected_values=[2],
     )
 
 
-def test_resolve_multiple_bool():
+def test_aggregation_bool():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:01, 1
                         1,2022-01-01 00:00:02, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="bool",
-            interval_days=2,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=boolean,
+            lookahead_days=2,
             fallback=0,
             incident=False,
         ),
         expected_values=[1, 0],
     )
 
 
-def test_resolve_multiple_change_per_day():
+def test_aggregation_change_per_day():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:00, 1
                         1,2022-01-02 00:00:00, 2
                         2,2022-01-01 00:00:00, 1
                         2,2023-01-08 00:00:00, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="change_per_day",
-            interval_days=4,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=change_per_day,
+            lookahead_days=4,
             fallback=np.NaN,
             incident=False,
         ),
         expected_values=[1, np.NaN],
     )
 
 
-def test_resolve_multiple_change_per_day_unordered():
+def test_aggregation_change_per_day_unordered():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-02 00:00:00, 2
                         1,2022-01-01 00:00:00, 1
                         2,2022-01-02 00:00:00, 2
                         2,2022-01-01 00:00:00, 1
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="change_per_day",
-            interval_days=4,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=change_per_day,
+            lookahead_days=4,
             fallback=np.NaN,
             incident=False,
         ),
         expected_values=[1, 1],
     )
 
 
-def test_resolve_multiple_change_per_day_negative():
+def test_aggregation_change_per_day_negative():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-02 00:00:00, 2
                         1,2022-01-01 00:00:00, 1
                         2,2022-01-02 00:00:00, 1
                         2,2022-01-01 00:00:00, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="change_per_day",
-            interval_days=4,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=change_per_day,
+            lookahead_days=4,
             fallback=np.NaN,
             incident=False,
         ),
         expected_values=[1, -1],
     )
 
 
-def test_resolve_multiple_change_per_day_too_few_datapoints():
+def test_aggregation_change_per_day_too_few_datapoints():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:00, 1
                         1,2022-01-02 00:00:00, 2
                         2,2022-01-01 00:00:00, 1
                         2,2022-01-08 00:00:00, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="change_per_day",
-            interval_days=4,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=change_per_day,
+            lookahead_days=4,
             fallback=99999,
             incident=False,
         ),
         expected_values=[1, 99999],
     )
 
 
-def test_resolve_multiple_change_per_day_only_one_observation():
+def test_aggregation_change_per_day_only_one_observation():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:00, 1
                         1,2022-01-02 00:00:00, 2
                         2,2022-01-01 00:00:00, 1
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="change_per_day",
-            interval_days=4,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=change_per_day,
+            lookahead_days=4,
             fallback=0,
             incident=False,
         ),
         expected_values=[1, 0],
     )
 
 
-def test_resolve_multiple_variance():
+def test_aggregation_variance():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:00, 1
                         1,2022-01-02 00:00:00, 2
                         2,2022-01-01 00:00:00, 1
                         2,2022-01-08 00:00:00, 2
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="variance",
-            interval_days=4,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=variance,
+            lookahead_days=4,
             fallback=np.NaN,
             incident=False,
         ),
         expected_values=[0.5, np.NaN],
     )
 
 
-def test_resolve_multiple_concatenate():
+def test_aggregation_concatenate():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:00,the patient
                         1,2022-01-02 00:00:00,is feeling ill
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="concatenate",
-            interval_days=4,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=concatenate,
+            lookahead_days=4,
             fallback=np.NaN,
             incident=False,
         ),
         expected_values=["the patient is feeling ill"],
     )
 
 
-def test_resolve_multiple_mean_len():
+def test_aggregation_mean_len():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:00,the patient
                         1,2022-01-02 00:00:00,is feeling ill
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="mean_number_of_characters",
-            interval_days=4,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=mean_number_of_characters,
+            lookahead_days=4,
             fallback=np.NaN,
             incident=False,
         ),
         expected_values=[12.5],
     )
 
 
-def test_resolve_multiple_type_token_ratio():
+def test_aggregation_type_token_ratio():
     prediction_times_str = """entity_id,timestamp,
                             1,2021-12-31 00:00:00
                             2,2021-12-31 00:00:00
                             """
     event_times_str = """entity_id,timestamp,value,
                         1,2022-01-01 00:00:00,The patient feels very tired!
                         1,2022-01-02 00:00:00,The patient is tired tired.
                         2,2022-01-01 00:00:00,The patient feels very happy!
                         2,2022-01-02 00:00:00,The patient is feeling tired.
                         """
 
     assert_flattened_data_as_expected(
         prediction_times_df=prediction_times_str,
         output_spec=OutcomeSpec(
-            feature_name="value",
-            values_df=str_to_df(event_times_str),
-            resolve_multiple_fn="type_token_ratio",
-            interval_days=4,
+            feature_base_name="value",
+            timeseries_df=str_to_df(event_times_str),
+            aggregation_fn=type_token_ratio,
+            lookahead_days=4,
             fallback=np.NaN,
             incident=False,
         ),
         expected_values=[0.6, 0.8],
     )
```

