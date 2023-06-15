# Comparing `tmp/datajudge-1.7.0.tar.gz` & `tmp/datajudge-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datajudge-1.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "datajudge-1.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `datajudge-1.7.0.tar` & `datajudge-1.8.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      378 2023-06-02 14:28:48.383106 datajudge-1.7.0/.flake8
--rw-r--r--   0        0        0      238 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/.pull_request_template.md
--rw-r--r--   0        0        0      823 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/actions/pytest/action.yml
--rw-r--r--   0        0        0      154 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1275 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/workflows/build_and_publish.yaml
--rw-r--r--   0        0        0    11535 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     2962 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/workflows/codeql.yml
--rw-r--r--   0        0        0     1369 2023-06-02 14:28:48.383106 datajudge-1.7.0/.github/workflows/pre-commit-autoupdate.yml
--rw-r--r--   0        0        0     1311 2023-06-02 14:28:48.383106 datajudge-1.7.0/.gitignore
--rw-r--r--   0        0        0      958 2023-06-02 14:28:48.383106 datajudge-1.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      268 2023-06-02 14:28:48.383106 datajudge-1.7.0/.readthedocs.yml
--rw-r--r--   0        0        0     3355 2023-06-02 14:28:48.383106 datajudge-1.7.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1515 2023-06-02 14:28:48.383106 datajudge-1.7.0/LICENSE
--rw-r--r--   0        0        0     1600 2023-06-02 14:28:48.383106 datajudge-1.7.0/README.md
--rw-r--r--   0        0        0       32 2023-06-02 14:28:48.383106 datajudge-1.7.0/_typos.toml
--rw-r--r--   0        0        0       84 2023-06-02 14:28:48.383106 datajudge-1.7.0/codecov.yml
--rw-r--r--   0        0        0     1241 2023-06-02 14:28:48.383106 datajudge-1.7.0/docker-compose.yaml
--rw-r--r--   0        0        0      638 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/Makefile
--rw-r--r--   0        0        0      764 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/make.bat
--rw-r--r--   0        0        0      905 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/conf.py
--rw-r--r--   0        0        0     1168 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/development.rst
--rw-r--r--   0        0        0     5146 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/example.rst
--rw-r--r--   0        0        0     6419 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/example_dates.rst
--rw-r--r--   0        0        0     8642 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/example_exploration.rst
--rw-r--r--   0        0        0    12556 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/example_twitch.rst
--rw-r--r--   0        0        0      194 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/examples.rst
--rw-r--r--   0        0        0     1381 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_process.py
--rw-r--r--   0        0        0    17481 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_report.html
--rw-r--r--   0        0        0     2663 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_specification.py
--rw-r--r--   0        0        0      573 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_upload.py
--rw-r--r--   0        0        0    70396 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_version1.csv
--rw-r--r--   0        0        0    82951 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitch_version2.csv
--rw-r--r--   0        0        0    78962 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/examples/twitchdata.csv
--rw-r--r--   0        0        0     8452 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/getting_started.rst
--rw-r--r--   0        0        0      543 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/index.rst
--rw-r--r--   0        0        0      155 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/installation.rst
--rw-r--r--   0        0        0     1527 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/motivation.rst
--rw-r--r--   0        0        0    51601 2023-06-02 14:28:48.383106 datajudge-1.7.0/docs/source/report_failing_query1.png
--rw-r--r--   0        0        0   163420 2023-06-02 14:28:48.387106 datajudge-1.7.0/docs/source/report_failing_query2.png
--rw-r--r--   0        0        0    11178 2023-06-02 14:28:48.387106 datajudge-1.7.0/docs/source/testing.rst
--rw-r--r--   0        0        0      329 2023-06-02 14:28:48.387106 datajudge-1.7.0/environment.yml
--rw-r--r--   0        0        0     1168 2023-06-02 14:28:48.387106 datajudge-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      510 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/__init__.py
--rw-r--r--   0        0        0     8560 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/base.py
--rw-r--r--   0        0        0     4636 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/column.py
--rw-r--r--   0        0        0     8603 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/date.py
--rw-r--r--   0        0        0     1788 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/groupby.py
--rw-r--r--   0        0        0     4202 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/interval.py
--rw-r--r--   0        0        0     6427 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/miscs.py
--rw-r--r--   0        0        0     6075 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/nrows.py
--rw-r--r--   0        0        0    10449 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/numeric.py
--rw-r--r--   0        0        0     7220 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/row.py
--rw-r--r--   0        0        0     4532 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/stats.py
--rw-r--r--   0        0        0    15216 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/uniques.py
--rw-r--r--   0        0        0     7384 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/constraints/varchar.py
--rw-r--r--   0        0        0    43806 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/db_access.py
--rw-r--r--   0        0        0     1019 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/pytest_integration.py
--rw-r--r--   0        0        0    71257 2023-06-02 14:28:48.387106 datajudge-1.7.0/src/datajudge/requirements.py
--rwxr-xr-x   0        0        0      173 2023-06-02 14:28:48.387106 datajudge-1.7.0/start_db2.sh
--rwxr-xr-x   0        0        0      522 2023-06-02 14:28:48.387106 datajudge-1.7.0/start_mssql.sh
--rwxr-xr-x   0        0        0      140 2023-06-02 14:28:48.387106 datajudge-1.7.0/start_postgres.sh
--rw-r--r--   0        0        0        0 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/__init__.py
--rw-r--r--   0        0        0    32592 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     2848 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/test_column_capitalization.py
--rw-r--r--   0        0        0     6795 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/test_data_source.py
--rw-r--r--   0        0        0    76755 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/test_integration.py
--rw-r--r--   0        0        0     2520 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/integration/test_stats.py
--rw-r--r--   0        0        0     2216 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_condition.py
--rw-r--r--   0        0        0      726 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_db_access.py
--rw-r--r--   0        0        0      856 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_percentiles.py
--rw-r--r--   0        0        0     2208 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_pytest.py
--rw-r--r--   0        0        0     1763 2023-06-02 14:28:48.387106 datajudge-1.7.0/tests/unit/test_set_functions.py
--rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 datajudge-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      378 2023-06-15 11:38:57.236727 datajudge-1.8.0/.flake8
+-rw-r--r--   0        0        0      238 2023-06-15 11:38:57.236727 datajudge-1.8.0/.github/.pull_request_template.md
+-rw-r--r--   0        0        0      823 2023-06-15 11:38:57.236727 datajudge-1.8.0/.github/actions/pytest/action.yml
+-rw-r--r--   0        0        0      154 2023-06-15 11:38:57.236727 datajudge-1.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1275 2023-06-15 11:38:57.236727 datajudge-1.8.0/.github/workflows/build_and_publish.yaml
+-rw-r--r--   0        0        0    11745 2023-06-15 11:38:57.236727 datajudge-1.8.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     2962 2023-06-15 11:38:57.236727 datajudge-1.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0     1369 2023-06-15 11:38:57.236727 datajudge-1.8.0/.github/workflows/pre-commit-autoupdate.yml
+-rw-r--r--   0        0        0     1311 2023-06-15 11:38:57.236727 datajudge-1.8.0/.gitignore
+-rw-r--r--   0        0        0      958 2023-06-15 11:38:57.236727 datajudge-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      268 2023-06-15 11:38:57.236727 datajudge-1.8.0/.readthedocs.yml
+-rw-r--r--   0        0        0     3665 2023-06-15 11:38:57.236727 datajudge-1.8.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1515 2023-06-15 11:38:57.236727 datajudge-1.8.0/LICENSE
+-rw-r--r--   0        0        0     1600 2023-06-15 11:38:57.240728 datajudge-1.8.0/README.md
+-rw-r--r--   0        0        0       32 2023-06-15 11:38:57.240728 datajudge-1.8.0/_typos.toml
+-rw-r--r--   0        0        0       84 2023-06-15 11:38:57.240728 datajudge-1.8.0/codecov.yml
+-rw-r--r--   0        0        0     1241 2023-06-15 11:38:57.240728 datajudge-1.8.0/docker-compose.yaml
+-rw-r--r--   0        0        0      638 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/Makefile
+-rw-r--r--   0        0        0      764 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/make.bat
+-rw-r--r--   0        0        0      905 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/conf.py
+-rw-r--r--   0        0        0     1168 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/development.rst
+-rw-r--r--   0        0        0     5146 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/example.rst
+-rw-r--r--   0        0        0     6419 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/example_dates.rst
+-rw-r--r--   0        0        0     8642 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/example_exploration.rst
+-rw-r--r--   0        0        0    12556 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/example_twitch.rst
+-rw-r--r--   0        0        0      194 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/examples.rst
+-rw-r--r--   0        0        0     1381 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/twitch_process.py
+-rw-r--r--   0        0        0    17481 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/twitch_report.html
+-rw-r--r--   0        0        0     2663 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/twitch_specification.py
+-rw-r--r--   0        0        0      573 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/twitch_upload.py
+-rw-r--r--   0        0        0    70396 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/twitch_version1.csv
+-rw-r--r--   0        0        0    82951 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/twitch_version2.csv
+-rw-r--r--   0        0        0    78962 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/examples/twitchdata.csv
+-rw-r--r--   0        0        0     8452 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/getting_started.rst
+-rw-r--r--   0        0        0      543 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/index.rst
+-rw-r--r--   0        0        0      155 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/installation.rst
+-rw-r--r--   0        0        0     1527 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/motivation.rst
+-rw-r--r--   0        0        0    51601 2023-06-15 11:38:57.240728 datajudge-1.8.0/docs/source/report_failing_query1.png
+-rw-r--r--   0        0        0   163420 2023-06-15 11:38:57.244727 datajudge-1.8.0/docs/source/report_failing_query2.png
+-rw-r--r--   0        0        0    11178 2023-06-15 11:38:57.244727 datajudge-1.8.0/docs/source/testing.rst
+-rw-r--r--   0        0        0      329 2023-06-15 11:38:57.244727 datajudge-1.8.0/environment.yml
+-rw-r--r--   0        0        0     1168 2023-06-15 11:38:57.244727 datajudge-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      510 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/__init__.py
+-rw-r--r--   0        0        0     8560 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/base.py
+-rw-r--r--   0        0        0     4636 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/column.py
+-rw-r--r--   0        0        0     8603 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/date.py
+-rw-r--r--   0        0        0     1788 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/groupby.py
+-rw-r--r--   0        0        0     4202 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/interval.py
+-rw-r--r--   0        0        0     7160 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/miscs.py
+-rw-r--r--   0        0        0     6075 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/nrows.py
+-rw-r--r--   0        0        0    10449 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/numeric.py
+-rw-r--r--   0        0        0     7220 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/row.py
+-rw-r--r--   0        0        0     4532 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/stats.py
+-rw-r--r--   0        0        0    15216 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/uniques.py
+-rw-r--r--   0        0        0     7384 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/constraints/varchar.py
+-rw-r--r--   0        0        0    44765 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/db_access.py
+-rw-r--r--   0        0        0     1019 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/pytest_integration.py
+-rw-r--r--   0        0        0    72668 2023-06-15 11:38:57.244727 datajudge-1.8.0/src/datajudge/requirements.py
+-rwxr-xr-x   0        0        0      173 2023-06-15 11:38:57.244727 datajudge-1.8.0/start_db2.sh
+-rwxr-xr-x   0        0        0      522 2023-06-15 11:38:57.244727 datajudge-1.8.0/start_mssql.sh
+-rwxr-xr-x   0        0        0      140 2023-06-15 11:38:57.244727 datajudge-1.8.0/start_postgres.sh
+-rw-r--r--   0        0        0        0 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0    34106 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2848 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/integration/test_column_capitalization.py
+-rw-r--r--   0        0        0     6795 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/integration/test_data_source.py
+-rw-r--r--   0        0        0    77833 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/integration/test_integration.py
+-rw-r--r--   0        0        0     2520 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/integration/test_stats.py
+-rw-r--r--   0        0        0     2216 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/unit/test_condition.py
+-rw-r--r--   0        0        0      726 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/unit/test_db_access.py
+-rw-r--r--   0        0        0      856 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/unit/test_percentiles.py
+-rw-r--r--   0        0        0     2212 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/unit/test_pytest.py
+-rw-r--r--   0        0        0     1763 2023-06-15 11:38:57.244727 datajudge-1.8.0/tests/unit/test_set_functions.py
+-rw-r--r--   0        0        0     2360 1970-01-01 00:00:00.000000 datajudge-1.8.0/PKG-INFO
```

### Comparing `datajudge-1.7.0/.github/actions/pytest/action.yml` & `datajudge-1.8.0/.github/actions/pytest/action.yml`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/.github/workflows/build_and_publish.yaml` & `datajudge-1.8.0/.github/workflows/build_and_publish.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     strategy:
       fail-fast: true
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
-      - uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
+      - uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
         with:
           environment-file: environment.yml
 
       - name: Build
         shell: bash -l {0}
         # It seems as though flit publish expects a .pypirc file as compared to
         # only a token passed as an argument.
```

### Comparing `datajudge-1.7.0/.github/workflows/ci.yaml` & `datajudge-1.8.0/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -41,30 +41,30 @@
         SA_VERSION: ['<2.0', '>=2.0']
     steps:
       - name: Checkout branch
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
       - name: Set up micromamba
-        uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
+        uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
         with:
           environment-file: environment.yml
           cache-downloads: true
           cache-environment: true
           cache-environment-key: ${{ runner.os }}-${{ hashFiles('environment.yml') }}-${{ matrix.PYTHON_VERSION }}-${{ matrix.SA_VERSION }}
           create-args: >-
             python=${{ matrix.PYTHON_VERSION }}
             sqlalchemy${{ matrix.SA_VERSION }}
       - name: Run tests
         uses: ./.github/actions/pytest
         with:
           args: "tests/unit"
 
   mssql:
-    if: ${{ contains(github.event.pull_request.labels.*.name, 'sqlserver') || contains(github.event.pull_request.labels.*.name, 'ready') }}
+    if: ${{ contains(github.event.pull_request.labels.*.name, 'sqlserver') || contains(github.event.pull_request.labels.*.name, 'ready') || github.ref == 'refs/heads/main' }}
     name: "mssql - Python ${{ matrix.PYTHON_VERSION }} - SA ${{ matrix.SA_VERSION }}"
     runs-on: ubuntu-20.04
     env:
       CI: True
     strategy:
       fail-fast: false
       matrix:
@@ -81,15 +81,15 @@
     steps:
       - name: Checkout branch
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
           fetch-depth: 0
       - name: Set up micromamba
-        uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
+        uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
         with:
           environment-file: environment.yml
           cache-downloads: true
           cache-environment: true
           cache-environment-key: ${{ runner.os }}-${{ hashFiles('environment.yml') }}-${{ matrix.PYTHON_VERSION }}-${{ matrix.SA_VERSION }}
           create-args: >-
             python=${{ matrix.PYTHON_VERSION }}
@@ -107,15 +107,15 @@
       - name: Run tests
         uses: ./.github/actions/pytest
         with:
           backend: mssql
           args: tests/integration
 
   postgres:
-    if: ${{ contains(github.event.pull_request.labels.*.name, 'postgres') || contains(github.event.pull_request.labels.*.name, 'ready') }}
+    if: ${{ contains(github.event.pull_request.labels.*.name, 'postgres') || contains(github.event.pull_request.labels.*.name, 'ready') || github.ref == 'refs/heads/main' }}
     name: "PostgreSQL ${{ matrix.POSTGRES_VERSION }} - Python ${{ matrix.PYTHON_VERSION }} - SA ${{ matrix.SA_VERSION }}"
     runs-on: ubuntu-20.04
     env:
       CI: True
     strategy:
       fail-fast: false
       matrix:
@@ -134,15 +134,15 @@
     steps:
       - name: Checkout branch
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
           fetch-depth: 0       
       - name: Set up micromamba
-        uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
+        uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
         with:
           environment-file: environment.yml
           cache-downloads: true
           cache-environment: true
           cache-environment-key: ${{ runner.os }}-${{ hashFiles('environment.yml') }}-${{ matrix.PYTHON_VERSION }}-${{ matrix.SA_VERSION }}
           create-args: >-
             python=${{ matrix.PYTHON_VERSION }}
@@ -152,15 +152,15 @@
         uses: ./.github/actions/pytest
         with:
           backend: postgres
           args: tests/integration
       
 
   db2:
-    if: ${{ contains(github.event.pull_request.labels.*.name, 'db2') || contains(github.event.pull_request.labels.*.name, 'ready') }}
+    if: ${{ contains(github.event.pull_request.labels.*.name, 'db2') || contains(github.event.pull_request.labels.*.name, 'ready') || github.ref == 'refs/heads/main' }}
     name: "DB2 - Python ${{ matrix.PYTHON_VERSION }} - SA ${{ matrix.SA_VERSION }}"
     runs-on: ubuntu-20.04
     env:
       CI: True
     strategy:
       fail-fast: false
       matrix:
@@ -182,15 +182,15 @@
     steps:
       - name: Checkout branch
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
           fetch-depth: 0
       - name: Set up micromamba
-        uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
+        uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
         with:
           environment-file: environment.yml
           cache-downloads: true
           cache-environment: true
           cache-environment-key: ${{ runner.os }}-${{ hashFiles('environment.yml') }}-${{ matrix.PYTHON_VERSION }}-${{ matrix.SA_VERSION }}
           create-args: >-
             python=${{ matrix.PYTHON_VERSION }}
@@ -205,15 +205,15 @@
         with:
           backend: db2
           args: tests/integration
       
 
 
   snowflake:
-    if: ${{ contains(github.event.pull_request.labels.*.name, 'snowflake') || contains(github.event.pull_request.labels.*.name, 'ready') }}
+    if: ${{ contains(github.event.pull_request.labels.*.name, 'snowflake') || contains(github.event.pull_request.labels.*.name, 'ready') || github.ref == 'refs/heads/main' }}
     name: "Snowflake - Python ${{ matrix.PYTHON_VERSION }} - SA ${{ matrix.SA_VERSION }}"
     runs-on: ubuntu-latest
     env:
       SNOWFLAKE_USER: DATAJUDGE
       SNOWFLAKE_PASSWORD: ${{ secrets.SNOWFLAKE_PASSWORD }}
       SNOWFLAKE_ACCOUNT: ${{ secrets.SNOWFLAKE_ACCOUNT }}
     strategy:
@@ -224,15 +224,15 @@
     steps:
       - name: Checkout branch
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
           fetch-depth: 0
       - name: Set up micromamba
-        uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
+        uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
         with:
           environment-file: environment.yml
           cache-downloads: true
           cache-environment: true
           cache-environment-key: ${{ runner.os }}-${{ hashFiles('environment.yml') }}-${{ matrix.PYTHON_VERSION }}-${{ matrix.SA_VERSION }}
           create-args: >-
             python=${{ matrix.PYTHON_VERSION }}
@@ -241,30 +241,30 @@
       - name: Run tests
         uses: ./.github/actions/pytest
         with:
           backend: snowflake
           args: tests/integration
 
   bigquery:
-    if: ${{ contains(github.event.pull_request.labels.*.name, 'bigquery') || contains(github.event.pull_request.labels.*.name, 'ready') }}
+    if: ${{ contains(github.event.pull_request.labels.*.name, 'bigquery') || contains(github.event.pull_request.labels.*.name, 'ready') || github.ref == 'refs/heads/main' }}
     name: "BigQuery - Python ${{ matrix.PYTHON_VERSION }} - SA ${{ matrix.SA_VERSION }}"
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
       matrix:
         PYTHON_VERSION: [ '3.8' ]
         SA_VERSION: ["<2.0"]
     steps:
       - name: Checkout branch
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
           fetch-depth: 0
       - name: Set up micromamba
-        uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
+        uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
         with:
           environment-file: environment.yml
           cache-downloads: true
           cache-environment: true
           cache-environment-key: ${{ runner.os }}-${{ hashFiles('environment.yml') }}-${{ matrix.PYTHON_VERSION }}-${{ matrix.SA_VERSION }}
           create-args: >-
             python=${{ matrix.PYTHON_VERSION }}
@@ -278,15 +278,15 @@
       - name: Run tests
         uses: ./.github/actions/pytest
         with:
           backend: bigquery
           args: -n auto tests/integration
 
   impala-column:
-    if: ${{ contains(github.event.pull_request.labels.*.name, 'impala') || contains(github.event.pull_request.labels.*.name, 'ready') }}
+    if: ${{ contains(github.event.pull_request.labels.*.name, 'impala') || contains(github.event.pull_request.labels.*.name, 'ready') || github.ref == 'refs/heads/main' }}
     name: "Impala - Python ${{ matrix.PYTHON_VERSION }} - SA ${{ matrix.SA_VERSION }}"
     runs-on: ubuntu-20.04
     env:
       CI: True
     strategy:
       fail-fast: false
       matrix:
@@ -297,15 +297,15 @@
     steps:
       - name: Checkout branch
         uses: actions/checkout@v3
         with:
           ref: ${{ github.head_ref }}
           fetch-depth: 0
       - name: Set up micromamba
-        uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
+        uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
         with:
           environment-file: environment.yml
           cache-downloads: true
           cache-environment: true
           cache-environment-key: ${{ runner.os }}-${{ hashFiles('environment.yml') }}-${{ matrix.PYTHON_VERSION }}-${{ matrix.SA_VERSION }}
           create-args: >-
             python=${{ matrix.PYTHON_VERSION }}
```

### Comparing `datajudge-1.7.0/.github/workflows/codeql.yml` & `datajudge-1.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/.github/workflows/pre-commit-autoupdate.yml` & `datajudge-1.8.0/.github/workflows/pre-commit-autoupdate.yml`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     steps:
       - name: Checkout branch
         uses: actions/checkout@v3
         # We need to checkout with SSH here to have actions run on the PR.
         with:
           ssh-key: ${{ secrets.SSH_PRIVATE_KEY }}
       - name: Set up micromamba environment
-        uses: mamba-org/setup-micromamba@5d5dbebd87f7b9358c403c7a66651fa92b310105
+        uses: mamba-org/setup-micromamba@875557da4ee020f18df03b8910a42203fbf02da1
         with:
           environment-name: pre-commit
           create-args: >-
             pre-commit
             mamba
       - name: Update pre-commit hooks and run
         id: versions
```

### Comparing `datajudge-1.7.0/.gitignore` & `datajudge-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/.pre-commit-config.yaml` & `datajudge-1.8.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,20 @@
       - id: flake8-conda
   - repo: https://github.com/Quantco/pre-commit-mirrors-isort
     rev: 5.12.0
     hooks:
       - id: isort-conda
         additional_dependencies: [-c, conda-forge, toml=0.10.2]
   - repo: https://github.com/Quantco/pre-commit-mirrors-mypy
-    rev: "1.2.0"
+    rev: "1.3.0"
     hooks:
       - id: mypy-conda
         additional_dependencies: [-c, conda-forge, types-setuptools]
   - repo: https://github.com/Quantco/pre-commit-mirrors-pyupgrade
-    rev: 3.3.2
+    rev: 3.6.0
     hooks:
       - id: pyupgrade-conda
         args:
           - --py38-plus
   - repo: https://github.com/Quantco/pre-commit-mirrors-typos
     rev: 1.13.20
     hooks:
```

### Comparing `datajudge-1.7.0/CHANGELOG.rst` & `datajudge-1.8.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,31 @@
    * Update the major if you break the public API
    * Update the minor if you add new functionality
    * Update the patch if you fixed a bug
 
 Changelog
 =========
 
+1.8.0 - 2023.XX.XX
+------------------
+
+**New features**
+
+- Implement :meth:`datajudge.WithinRequirement.add_functional_dependency_constraint`.
+
+**Other changes**
+
+- Improve error message when a :class:`~datajudge.DataReference` is constructed with a single column name instead of specifying a list of columns.
+
 1.7.0 - 2023.05.11
 ------------------
 
 **New features**
 
-- Implement :meth:`datajudge.WithinRequirement.add_value_distribution_constraint`.
+- Implement :meth:`datajudge.WithinRequirement.add_categorical_bound_constraint`.
 - Extended :meth:`datajudge.WithinRequirement.add_column_type_constraint` to support column type specification using string format, backend-specific SQLAlchemy types, and SQLAlchemy's generic types.
 - Implement :meth:`datajudge.WithinRequirement.add_numeric_no_gap_constraint`, :meth:`datajudge.WithinRequirement.add_numeric_no_overlap_constraint`,
 
 1.6.0 - 2022.04.12
 ------------------
 
 **Other changes**
```

### Comparing `datajudge-1.7.0/LICENSE` & `datajudge-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/README.md` & `datajudge-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docker-compose.yaml` & `datajudge-1.8.0/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/Makefile` & `datajudge-1.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/make.bat` & `datajudge-1.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/conf.py` & `datajudge-1.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/development.rst` & `datajudge-1.8.0/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/example.rst` & `datajudge-1.8.0/docs/source/examples/example.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/example_dates.rst` & `datajudge-1.8.0/docs/source/examples/example_dates.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/example_exploration.rst` & `datajudge-1.8.0/docs/source/examples/example_exploration.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/example_twitch.rst` & `datajudge-1.8.0/docs/source/examples/example_twitch.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/twitch_process.py` & `datajudge-1.8.0/docs/source/examples/twitch_process.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/twitch_report.html` & `datajudge-1.8.0/docs/source/examples/twitch_report.html`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/twitch_specification.py` & `datajudge-1.8.0/docs/source/examples/twitch_specification.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/twitch_upload.py` & `datajudge-1.8.0/docs/source/examples/twitch_upload.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/twitch_version1.csv` & `datajudge-1.8.0/docs/source/examples/twitch_version1.csv`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/twitch_version2.csv` & `datajudge-1.8.0/docs/source/examples/twitch_version2.csv`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/examples/twitchdata.csv` & `datajudge-1.8.0/docs/source/examples/twitchdata.csv`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/getting_started.rst` & `datajudge-1.8.0/docs/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/index.rst` & `datajudge-1.8.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/motivation.rst` & `datajudge-1.8.0/docs/source/motivation.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/report_failing_query1.png` & `datajudge-1.8.0/docs/source/report_failing_query1.png`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/report_failing_query2.png` & `datajudge-1.8.0/docs/source/report_failing_query2.png`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/docs/source/testing.rst` & `datajudge-1.8.0/docs/source/testing.rst`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/pyproject.toml` & `datajudge-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/base.py` & `datajudge-1.8.0/src/datajudge/constraints/base.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/column.py` & `datajudge-1.8.0/src/datajudge/constraints/column.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/date.py` & `datajudge-1.8.0/src/datajudge/constraints/date.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/groupby.py` & `datajudge-1.8.0/src/datajudge/constraints/groupby.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/interval.py` & `datajudge-1.8.0/src/datajudge/constraints/interval.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/miscs.py` & `datajudge-1.8.0/src/datajudge/constraints/miscs.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,14 +115,33 @@
             f"uniques. This surpasses the max_duplicate_fraction of "
             f"{self.ref_value}. An example tuple breaking the "
             f"uniqueness condition is: {sample_string}."
         )
         return TestResult.failure(assertion_text)
 
 
+class FunctionalDependency(Constraint):
+    def __init__(self, ref: DataReference, key_columns: List[str], **kwargs):
+        super().__init__(ref, ref_value=object(), **kwargs)
+        self.key_columns = key_columns
+
+    def test(self, engine: sa.engine.Engine) -> TestResult:
+        violations, _ = db_access.get_functional_dependency_violations(
+            engine, self.ref, self.key_columns
+        )
+        if not violations:
+            return TestResult.success()
+
+        assertion_text = (
+            f"{self.ref.get_string()} has violations of functional dependence, e.g.:\n"
+            + "\n".join([f"{tuple(violation)}" for violation in violations][:5])
+        )
+        return TestResult.failure(assertion_text)
+
+
 class MaxNullFraction(Constraint):
     def __init__(
         self,
         ref,
         *,
         ref2: DataReference = None,
         max_null_fraction: float = None,
```

### Comparing `datajudge-1.7.0/src/datajudge/constraints/nrows.py` & `datajudge-1.8.0/src/datajudge/constraints/nrows.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/numeric.py` & `datajudge-1.8.0/src/datajudge/constraints/numeric.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/row.py` & `datajudge-1.8.0/src/datajudge/constraints/row.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/stats.py` & `datajudge-1.8.0/src/datajudge/constraints/stats.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/uniques.py` & `datajudge-1.8.0/src/datajudge/constraints/uniques.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/constraints/varchar.py` & `datajudge-1.8.0/src/datajudge/constraints/varchar.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/db_access.py` & `datajudge-1.8.0/src/datajudge/db_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,17 +290,20 @@
         return self.clause
 
 
 class DataReference:
     def __init__(
         self,
         data_source: DataSource,
-        columns: list[str] = None,
-        condition: Condition = None,
+        columns: list[str] | None = None,
+        condition: Condition | None = None,
     ):
+        if columns is not None and not isinstance(columns, list):
+            raise TypeError(f"columns must be a list, not {type(columns)}")
+
         self.data_source = data_source
         self.columns = columns
         self.condition = condition
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(data_source={self.data_source!r}, columns={self.columns!r}, condition={self.condition!r})"
 
@@ -778,14 +781,42 @@
         start_column,
         end_column,
         legitimate_gap_size,
         _numeric_gap_condition,
     )
 
 
+def get_functional_dependency_violations(
+    engine: sa.engine.Engine,
+    ref: DataReference,
+    key_columns: list[str],
+):
+    selection = ref.get_selection(engine)
+    uniques = selection.distinct().cte()
+
+    key_columns_sa = [uniques.c[key_column] for key_column in key_columns]
+    violations_stmt = (
+        sa.select(*key_columns_sa).group_by(*key_columns_sa).having(sa.func.count() > 1)
+    ).cte()
+
+    join_condition = sa.and_(
+        *[
+            uniques.c[key_column] == violations_stmt.c[key_column]
+            for key_column in key_columns
+        ]
+    )
+
+    violation_tuples = sa.select(uniques).select_from(
+        uniques.join(violations_stmt, join_condition)
+    )
+
+    result = engine.connect().execute(violation_tuples).fetchall()
+    return result, [violation_tuples]
+
+
 def get_row_count(engine, ref, row_limit: int = None):
     """Return the number of rows for a `DataReference`.
 
     If `row_limit` is given, the number of rows is capped at the limit.
     """
     subquery = ref.get_selection(engine)
     if row_limit:
```

### Comparing `datajudge-1.7.0/src/datajudge/pytest_integration.py` & `datajudge-1.8.0/src/datajudge/pytest_integration.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/src/datajudge/requirements.py` & `datajudge-1.8.0/src/datajudge/requirements.py`

 * *Files 0% similar despite different names*

```diff
@@ -802,14 +802,41 @@
                 end_columns=[end_column],
                 max_relative_n_violations=max_relative_n_violations,
                 legitimate_gap_size=1 if end_included else 0,
                 name=name,
             )
         )
 
+    def add_functional_dependency_constraint(
+        self,
+        key_columns: List[str],
+        value_columns: List[str],
+        condition: Condition = None,
+        name: str = None,
+    ):
+        """
+        Expresses a functional dependency, a constraint where the `value_columns` are uniquely determined by the `key_columns`.
+        This means that for each unique combination of values in the `key_columns`, there is exactly one corresponding combination of values in the `value_columns`.
+
+        The ``add_unique_constraint`` constraint is a special case of this constraint, where the `key_columns` are a primary key,
+        and all other columns are included `value_columns`.
+        This constraint allows for a more general definition of functional dependencies, where the `key_columns` are not necessarily a primary key.
+
+        For more information on functional dependencies, see https://en.wikipedia.org/wiki/Functional_dependency.
+        """
+        relevant_columns = key_columns + value_columns
+        ref = DataReference(self.data_source, relevant_columns, condition)
+        self._constraints.append(
+            miscs_constraints.FunctionalDependency(
+                ref,
+                key_columns=key_columns,
+                name=name,
+            )
+        )
+
     def add_numeric_no_gap_constraint(
         self,
         start_column: str,
         end_column: str,
         key_columns: Optional[List[str]] = None,
         legitimate_gap_size: float = 0,
         max_relative_n_violations: float = 0,
@@ -1776,16 +1803,20 @@
         ``RowMatchingEquality`` considers only rows in both tables having values
         in ``matching_columns`` present in both tables. At most ``max_missing_fraction``
         of such rows can be missing in the intersection.
 
         Alternatively, this can be thought of as counting mismatches in
         ``comparison_columns`` after performing an inner join on ``matching_columns``.
         """
-        ref = DataReference(self.data_source, None, condition1)
-        ref2 = DataReference(self.data_source2, None, condition2)
+        ref = DataReference(
+            self.data_source, matching_columns1 + comparison_columns1, condition1
+        )
+        ref2 = DataReference(
+            self.data_source2, matching_columns2 + comparison_columns2, condition2
+        )
         self._constraints.append(
             row_constraints.RowMatchingEquality(
                 ref,
                 ref2,
                 matching_columns1,
                 matching_columns2,
                 comparison_columns1,
```

### Comparing `datajudge-1.7.0/start_mssql.sh` & `datajudge-1.8.0/start_mssql.sh`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/tests/integration/conftest.py` & `datajudge-1.8.0/tests/integration/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -724,14 +724,66 @@
         {"nested_varchar": "GHI#3,JKL#4,"},
     ]
     _handle_table(engine, metadata, table_name, columns, data)
     return TEST_DB_NAME, SCHEMA, table_name
 
 
 @pytest.fixture(scope="module")
+def functional_dependency_table(engine, metadata):
+    table_name = "functional_dependency_table"
+
+    # a -> b
+    # c -> b
+    # a -/-> c
+    columns = [
+        sa.Column("a", sa.Integer()),
+        sa.Column("b", sa.Integer()),
+        sa.Column("c", sa.Integer()),
+    ]
+    data = [
+        {"a": 1, "b": 2, "c": 3},
+        {"a": 1, "b": 2, "c": 4},
+        {"a": 2, "b": 3, "c": 5},
+        {"a": 2, "b": 3, "c": 6},
+        {"a": 3, "b": 4, "c": 1},
+        {"a": 3, "b": 4, "c": 2},
+    ]
+
+    _handle_table(engine, metadata, table_name, columns, data)
+    return TEST_DB_NAME, SCHEMA, table_name
+
+
+@pytest.fixture(scope="module")
+def functional_dependency_table_multi_key(engine, metadata):
+    table_name = "functional_dependency_table_multi_key"
+
+    # ab -> c
+    # ab -/-> d
+    columns = [
+        sa.Column("a", sa.Integer()),
+        sa.Column("b", sa.Integer()),
+        sa.Column("c", sa.Integer()),
+        sa.Column("d", sa.Integer()),
+    ]
+    data = [
+        {"a": 1, "b": 1, "c": 2, "d": 3},
+        {"a": 1, "b": 1, "c": 2, "d": 4},
+        {"a": 1, "b": 2, "c": 3, "d": 5},
+        {"a": 1, "b": 2, "c": 3, "d": 6},
+        {"a": 2, "b": 1, "c": 4, "d": 7},
+        {"a": 2, "b": 1, "c": 4, "d": 8},
+        {"a": 2, "b": 2, "c": 5, "d": 9},
+        {"a": 2, "b": 2, "c": 5, "d": 10},
+    ]
+
+    _handle_table(engine, metadata, table_name, columns, data)
+    return TEST_DB_NAME, SCHEMA, table_name
+
+
+@pytest.fixture(scope="module")
 def varchar_table1(engine, metadata):
     table_name = "varchar_table1"
     columns = [
         sa.Column("col_varchar", _string_column(engine)),
     ]
     data = [{"col_varchar": "qq" * i} for i in range(1, 10)]
     data.append({"col_varchar": None})
```

### Comparing `datajudge-1.7.0/tests/integration/test_column_capitalization.py` & `datajudge-1.8.0/tests/integration/test_column_capitalization.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/tests/integration/test_data_source.py` & `datajudge-1.8.0/tests/integration/test_data_source.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/tests/integration/test_integration.py` & `datajudge-1.8.0/tests/integration/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,14 +580,55 @@
         condition1=condition1,
         condition2=condition2,
     )
     test_result = req[0].test(engine)
     assert operation(test_result.outcome), test_result.failure_message
 
 
+@pytest.mark.parametrize(
+    "data",
+    [
+        (identity, ["a"], ["b"]),
+        (identity, ["c"], ["b"]),
+        (negation, ["a"], ["c"]),
+    ],
+)
+def test_functional_dependency_within(engine, functional_dependency_table, data):
+    (
+        operation,
+        key_columns,
+        value_columns,
+    ) = data
+    req = requirements.WithinRequirement.from_table(*functional_dependency_table)
+    req.add_functional_dependency_constraint(key_columns, value_columns)
+    assert operation(req[0].test(engine).outcome)
+
+
+@pytest.mark.parametrize(
+    "data",
+    [
+        (identity, ["a", "b"], ["c"]),
+        (negation, ["a", "b"], ["d"]),
+    ],
+)
+def test_functional_dependency_within_multi_key(
+    engine, functional_dependency_table_multi_key, data
+):
+    (
+        operation,
+        key_columns,
+        value_columns,
+    ) = data
+    req = requirements.WithinRequirement.from_table(
+        *functional_dependency_table_multi_key
+    )
+    req.add_functional_dependency_constraint(key_columns, value_columns)
+    assert operation(req[0].test(engine).outcome)
+
+
 def _flatten_and_filter(data):
     # Flattening one level
     res = []
     for d in data:
         res.extend(d)
 
     # returning an Iterable (set to get rid of duplicates in this case) without the empty string
```

### Comparing `datajudge-1.7.0/tests/integration/test_stats.py` & `datajudge-1.8.0/tests/integration/test_stats.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/tests/unit/test_condition.py` & `datajudge-1.8.0/tests/unit/test_condition.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/tests/unit/test_db_access.py` & `datajudge-1.8.0/tests/unit/test_db_access.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/tests/unit/test_percentiles.py` & `datajudge-1.8.0/tests/unit/test_percentiles.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/tests/unit/test_pytest.py` & `datajudge-1.8.0/tests/unit/test_pytest.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 @pytest.mark.parametrize(
     "method_name,arguments",
     [
         ("add_date_min_constraint", ["column", "column"]),
         ("add_varchar_min_length_constraint", ["column", "column"]),
         ("add_ks_2sample_constraint", ["column", "column"]),
         ("add_numeric_mean_constraint", ["column", "column", 0.1]),
-        ("add_row_superset_constraint", ["column", "column", 0]),
+        ("add_row_superset_constraint", [["column"], ["column"], 0]),
     ],
 )
 def test_test_name_between(method_name, arguments):
     req = BetweenRequirement.from_raw_queries(
         "select * from example",
         "example_table",
         "select * from example",
```

### Comparing `datajudge-1.7.0/tests/unit/test_set_functions.py` & `datajudge-1.8.0/tests/unit/test_set_functions.py`

 * *Files identical despite different names*

### Comparing `datajudge-1.7.0/PKG-INFO` & `datajudge-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datajudge
-Version: 1.7.0
+Version: 1.8.0
 Summary: datajudge allows to assess  whether data from database complies with reference
 Keywords: test,databases,validation
 Author-email: "QuantCo, Inc." <noreply@quantco.com>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

