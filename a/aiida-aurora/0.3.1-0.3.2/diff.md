# Comparing `tmp/aiida_aurora-0.3.1.tar.gz` & `tmp/aiida_aurora-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_aurora-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_aurora-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_aurora-0.3.1.tar` & `aiida_aurora-0.3.2.tar`

### file list

```diff
@@ -1,61 +1,69 @@
--rw-r--r--   0        0        0       26 2023-06-08 14:37:01.364612 aiida_aurora-0.3.1/.coveragerc
--rwxr-xr-x   0        0        0      195 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.github/install_aiida_github.sh
--rw-r--r--   0        0        0     2157 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      753 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.github/workflows/publish-on-pypi.yml
--rw-r--r--   0        0        0      142 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.gitignore
--rw-r--r--   0        0        0      942 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      119 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.readthedocs.yml
--rw-r--r--   0        0        0      232 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/.style.yapf
--rw-r--r--   0        0        0     1070 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/LICENSE
--rw-r--r--   0        0        0       35 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/MANIFEST.in
--rw-r--r--   0        0        0     6365 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/README.md
--rw-r--r--   0        0        0       83 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/__init__.py
--rw-r--r--   0        0        0      211 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/calculations/__init__.py
--rw-r--r--   0        0        0     7147 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/calculations/cycler.py
--rw-r--r--   0        0        0     3396 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/calculations/fake.py
--rw-r--r--   0        0        0     1592 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/cli.py
--rw-r--r--   0        0        0      246 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/data/__init__.py
--rw-r--r--   0        0        0     4117 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/data/battery.py
--rw-r--r--   0        0        0     2362 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/data/control.py
--rw-r--r--   0        0        0     2322 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/data/experiment.py
--rw-r--r--   0        0        0     2696 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/helpers.py
--rw-r--r--   0        0        0     6271 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/parsers.py
--rw-r--r--   0        0        0    15913 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/scheduler.py
--rw-r--r--   0        0        0       49 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/utils/__init__.py
--rw-r--r--   0        0        0     9221 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/utils/cycling_analysis.py
--rw-r--r--   0        0        0     1263 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/utils/plot.py
--rw-r--r--   0        0        0      172 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/workflows/__init__.py
--rw-r--r--   0        0        0    12454 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/workflows/stress_test.py
--rw-r--r--   0        0        0    32366 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/aiida_aurora/workflows/stress_test_defaults.json
--rw-r--r--   0        0        0        7 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/docs/.gitignore
--rwxr-xr-x   0        0        0     1541 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/docs/Makefile
--rwxr-xr-x   0        0        0    11606 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/docs/source/conf.py
--rw-r--r--   0        0        0     2814 2023-06-08 14:37:01.368612 aiida_aurora-0.3.1/docs/source/developer_guide/index.rst
--rw-r--r--   0        0        0    76300 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/images/AiiDA_transparent_logo.png
--rwxr-xr-x   0        0        0     1274 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/index.rst
--rw-r--r--   0        0        0     1263 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/user_guide/get_started.rst
--rw-r--r--   0        0        0       94 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/user_guide/index.rst
--rw-r--r--   0        0        0      243 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/docs/source/user_guide/tutorial.rst
--rw-r--r--   0        0        0      275 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/code_ketchup-0.2rc2.yml
--rw-r--r--   0        0        0      292 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/code_monitor.yml
--rw-r--r--   0        0        0      280 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_ddm07162.yml
--rw-r--r--   0        0        0      329 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_ddm07162_config.yaml
--rw-r--r--   0        0        0      336 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_localhost-verdi.yml
--rw-r--r--   0        0        0       41 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_localhost-verdi_config.yaml
--rw-r--r--   0        0        0      276 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_localhost.yml
--rw-r--r--   0        0        0       41 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/computer_localhost_config.yaml
--rwxr-xr-x   0        0        0      517 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/config_files/setup.sh
--rw-r--r--   0        0        0     2761 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/stress_test/batteries.json
--rw-r--r--   0        0        0     4683 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/examples/stress_test/submit_test.py
--rw-r--r--   0        0        0      139 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/fake_aurora_server/batt.json
--rw-r--r--   0        0        0      147 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/fake_aurora_server/exp.json
--rwxr-xr-x   0        0        0     3001 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/fake_aurora_server/server.py
--rw-r--r--   0        0        0     3676 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      215 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0      485 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/input_files/__init__.py
--rw-r--r--   0        0        0       27 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/input_files/file1.txt
--rw-r--r--   0        0        0       27 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/input_files/file2.txt
--rw-r--r--   0        0        0     1107 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/test_calculations.py
--rw-r--r--   0        0        0     1151 2023-06-08 14:37:01.372612 aiida_aurora-0.3.1/tests/test_cli.py
--rw-r--r--   0        0        0     7677 1970-01-01 00:00:00.000000 aiida_aurora-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/.coveragerc
+-rwxr-xr-x   0        0        0      195 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/.github/install_aiida_github.sh
+-rw-r--r--   0        0        0     2157 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      753 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/.github/workflows/publish-on-pypi.yml
+-rw-r--r--   0        0        0      142 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1494 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      119 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/.readthedocs.yml
+-rw-r--r--   0        0        0      232 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/.style.yapf
+-rw-r--r--   0        0        0     1070 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/LICENSE
+-rw-r--r--   0        0        0       35 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/MANIFEST.in
+-rw-r--r--   0        0        0     6389 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/README.md
+-rw-r--r--   0        0        0       83 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/__init__.py
+-rw-r--r--   0        0        0      286 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/calculations/__init__.py
+-rw-r--r--   0        0        0     7190 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/calculations/cycler.py
+-rw-r--r--   0        0        0     3441 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/calculations/fake.py
+-rw-r--r--   0        0        0     1592 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/cli.py
+-rw-r--r--   0        0        0      360 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/data/__init__.py
+-rw-r--r--   0        0        0     4130 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/data/battery.py
+-rw-r--r--   0        0        0     2361 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/data/control.py
+-rw-r--r--   0        0        0     2329 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/data/experiment.py
+-rw-r--r--   0        0        0     2696 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/helpers.py
+-rw-r--r--   0        0        0     6277 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/parsers.py
+-rw-r--r--   0        0        0    15934 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/scheduler.py
+-rw-r--r--   0        0        0      118 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/schemas/__init__.py
+-rw-r--r--   0        0        0     3401 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/schemas/battery.py
+-rw-r--r--   0        0        0    20941 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/schemas/cycling.py
+-rw-r--r--   0        0        0     1277 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/schemas/dgbowl/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/schemas/dgbowl/converters/__init__.py
+-rw-r--r--   0        0        0      962 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/schemas/dgbowl/converters/method.py
+-rw-r--r--   0        0        0      813 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/schemas/dgbowl/converters/sample.py
+-rw-r--r--   0        0        0     3311 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/schemas/utils/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/utils/__init__.py
+-rw-r--r--   0        0        0     9392 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/utils/cycling_analysis.py
+-rw-r--r--   0        0        0     1203 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/utils/plot.py
+-rw-r--r--   0        0        0      214 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/workflows/__init__.py
+-rw-r--r--   0        0        0    12346 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/workflows/stress_test.py
+-rw-r--r--   0        0        0    32363 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/aiida_aurora/workflows/stress_test_defaults.json
+-rw-r--r--   0        0        0        7 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/docs/.gitignore
+-rwxr-xr-x   0        0        0     1541 2023-06-15 09:57:42.110115 aiida_aurora-0.3.2/docs/Makefile
+-rwxr-xr-x   0        0        0    11799 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/docs/source/conf.py
+-rw-r--r--   0        0        0     2814 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/docs/source/developer_guide/index.rst
+-rw-r--r--   0        0        0    76300 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/docs/source/images/AiiDA_transparent_logo.png
+-rwxr-xr-x   0        0        0     1400 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/docs/source/index.rst
+-rw-r--r--   0        0        0      604 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/docs/source/nitpick-exceptions
+-rw-r--r--   0        0        0     1271 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/docs/source/user_guide/get_started.rst
+-rw-r--r--   0        0        0       94 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/docs/source/user_guide/index.rst
+-rw-r--r--   0        0        0      243 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/docs/source/user_guide/tutorial.rst
+-rw-r--r--   0        0        0      275 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/config_files/code_ketchup-0.2rc2.yml
+-rw-r--r--   0        0        0      292 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/config_files/code_monitor.yml
+-rw-r--r--   0        0        0      280 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/config_files/computer_ddm07162.yml
+-rw-r--r--   0        0        0      329 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/config_files/computer_ddm07162_config.yaml
+-rw-r--r--   0        0        0      336 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/config_files/computer_localhost-verdi.yml
+-rw-r--r--   0        0        0       41 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/config_files/computer_localhost-verdi_config.yaml
+-rw-r--r--   0        0        0      276 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/config_files/computer_localhost.yml
+-rw-r--r--   0        0        0       41 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/config_files/computer_localhost_config.yaml
+-rwxr-xr-x   0        0        0      517 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/config_files/setup.sh
+-rw-r--r--   0        0        0     2762 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/stress_test/batteries.json
+-rw-r--r--   0        0        0     4859 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/examples/stress_test/submit_test.py
+-rw-r--r--   0        0        0      139 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/fake_aurora_server/batt.json
+-rw-r--r--   0        0        0      147 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/fake_aurora_server/exp.json
+-rwxr-xr-x   0        0        0     3001 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/fake_aurora_server/server.py
+-rw-r--r--   0        0        0     4004 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0      485 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/tests/input_files/__init__.py
+-rw-r--r--   0        0        0       27 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/tests/input_files/file1.txt
+-rw-r--r--   0        0        0       27 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/tests/input_files/file2.txt
+-rw-r--r--   0        0        0      404 2023-06-15 09:57:42.114115 aiida_aurora-0.3.2/tests/test_entry_points.py
+-rw-r--r--   0        0        0     7947 1970-01-01 00:00:00.000000 aiida_aurora-0.3.2/PKG-INFO
```

### Comparing `aiida_aurora-0.3.1/.github/workflows/ci.yml` & `aiida_aurora-0.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/.github/workflows/publish-on-pypi.yml` & `aiida_aurora-0.3.2/.github/workflows/publish-on-pypi.yml`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/LICENSE` & `aiida_aurora-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/README.md` & `aiida_aurora-0.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,100 +6,102 @@
 # aiida-aurora
 
 AiiDA plugin for the Aurora project (autonomous robotic battery innovation platform).
 A collaboration between EPFL & Empa, within the BIG-MAP Stakeholder Initiative Call 2021.
 
 ## Repository contents
 
-* [`.github/`](.github/): [Github Actions](https://github.com/features/actions) configuration
-  * [`ci.yml`](.github/workflows/ci.yml): runs tests, checks test coverage and builds documentation at every new commit
-  * [`publish-on-pypi.yml`](.github/workflows/publish-on-pypi.yml): automatically deploy git tags to PyPI - just generate a [PyPI API token](https://pypi.org/help/#apitoken) for your PyPI account and add it to the `pypi_token` secret of your github repository
-* [`aiida_aurora/`](aiida_aurora/): The main source code of the plugin package
-  * [`data/`](aiida_aurora/data/): A new `DiffParameters` data class, used as input to the `DiffCalculation` `CalcJob` class
-  * [`calculations.py`](aiida_aurora/calculations.py): A new `DiffCalculation` `CalcJob` class
-  * [`cli.py`](aiida_aurora/cli.py): Extensions of the `verdi data` command line interface for the `DiffParameters` class
-  * [`helpers.py`](aiida_aurora/helpers.py): Helpers for setting up an AiiDA code for `diff` automatically
-  * [`parsers.py`](aiida_aurora/parsers.py): A new `Parser` for the `DiffCalculation`
-* [`docs/`](docs/): A documentation template ready for publication on [Read the Docs](http://aiida-diff.readthedocs.io/en/latest/)
-* [`examples/`](examples/): An example of how to submit a calculation using this plugin
-* [`tests/`](tests/): Basic regression tests using the [pytest](https://docs.pytest.org/en/latest/) framework (submitting a calculation, ...). Install `pip install -e .[testing]` and run `pytest`.
-* [`.coveragerc`](.coveragerc): Configuration of [coverage.py](https://coverage.readthedocs.io/en/latest) tool reporting which lines of your plugin are covered by tests
-* [`.gitignore`](.gitignore): Telling git which files to ignore
-* [`.pre-commit-config.yaml`](.pre-commit-config.yaml): Configuration of [pre-commit hooks](https://pre-commit.com/) that sanitize coding style and check for syntax errors. Enable via `pip install -e .[pre-commit] && pre-commit install`
-* [`.readthedocs.yml`](.readthedocs.yml): Configuration of documentation build for [Read the Docs](https://readthedocs.org/)
-* [`LICENSE`](LICENSE): License for your plugin
-* [`MANIFEST.in`](MANIFEST.in): Configure non-Python files to be included for publication on [PyPI](https://pypi.org/)
-* [`README.md`](README.md): This file
-* [`conftest.py`](conftest.py): Configuration of fixtures for [pytest](https://docs.pytest.org/en/latest/)
-* [`pytest.ini`](pytest.ini): Configuration of [pytest](https://docs.pytest.org/en/latest/) test discovery
-* [`setup.json`](setup.json): Plugin metadata for registration on [PyPI](https://pypi.org/) and the [AiiDA plugin registry](https://aiidateam.github.io/aiida-registry/) (including entry points)
-* [`setup.py`](setup.py): Installation script for pip / [PyPI](https://pypi.org/)
-
+- [`.github/`](.github/): [Github Actions](https://github.com/features/actions) configuration
+  - [`ci.yml`](.github/workflows/ci.yml): runs tests, checks test coverage and builds documentation at every new commit
+  - [`publish-on-pypi.yml`](.github/workflows/publish-on-pypi.yml): automatically deploy git tags to PyPI - just generate a [PyPI API token](https://pypi.org/help/#apitoken) for your PyPI account and add it to the `pypi_token` secret of your github repository
+- [`aiida_aurora/`](aiida_aurora/): The main source code of the plugin package
+  - [`data/`](aiida_aurora/data/): A new `DiffParameters` data class, used as input to the `DiffCalculation` `CalcJob` class
+  - [`calculations.py`](aiida_aurora/calculations.py): A new `DiffCalculation` `CalcJob` class
+  - [`cli.py`](aiida_aurora/cli.py): Extensions of the `verdi data` command line interface for the `DiffParameters` class
+  - [`helpers.py`](aiida_aurora/helpers.py): Helpers for setting up an AiiDA code for `diff` automatically
+  - [`parsers.py`](aiida_aurora/parsers.py): A new `Parser` for the `DiffCalculation`
+- [`docs/`](docs/): A documentation template ready for publication on [Read the Docs](http://aiida-diff.readthedocs.io/en/latest/)
+- [`examples/`](examples/): An example of how to submit a calculation using this plugin
+- [`tests/`](tests/): Basic regression tests using the [pytest](https://docs.pytest.org/en/latest/) framework (submitting a calculation, ...). Install `pip install -e .[testing]` and run `pytest`.
+- [`.coveragerc`](.coveragerc): Configuration of [coverage.py](https://coverage.readthedocs.io/en/latest) tool reporting which lines of your plugin are covered by tests
+- [`.gitignore`](.gitignore): Telling git which files to ignore
+- [`.pre-commit-config.yaml`](.pre-commit-config.yaml): Configuration of [pre-commit hooks](https://pre-commit.com/) that sanitize coding style and check for syntax errors. Enable via `pip install -e .[pre-commit] && pre-commit install`
+- [`.readthedocs.yml`](.readthedocs.yml): Configuration of documentation build for [Read the Docs](https://readthedocs.org/)
+- [`LICENSE`](LICENSE): License for your plugin
+- [`MANIFEST.in`](MANIFEST.in): Configure non-Python files to be included for publication on [PyPI](https://pypi.org/)
+- [`README.md`](README.md): This file
+- [`conftest.py`](conftest.py): Configuration of fixtures for [pytest](https://docs.pytest.org/en/latest/)
+- [`pytest.ini`](pytest.ini): Configuration of [pytest](https://docs.pytest.org/en/latest/) test discovery
+- [`setup.json`](setup.json): Plugin metadata for registration on [PyPI](https://pypi.org/) and the [AiiDA plugin registry](https://aiidateam.github.io/aiida-registry/) (including entry points)
+- [`setup.py`](setup.py): Installation script for pip / [PyPI](https://pypi.org/)
 
 See also the following video sequences from the 2019-05 AiiDA tutorial:
 
- * [aiida-diff setup.json](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=240s)
- * [run aiida-diff example calculation](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=403s)
- * [aiida-diff CalcJob plugin](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=685s)
- * [aiida-diff Parser plugin](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=936s)
- * [aiida-diff computer/code helpers](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1238s)
- * [aiida-diff input data (with validation)](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1353s)
- * [aiida-diff cli](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1621s)
- * [aiida-diff tests](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1931s)
- * [Adding your plugin to the registry](https://www.youtube.com/watch?v=760O2lDB-TM&t=112s)
- * [pre-commit hooks](https://www.youtube.com/watch?v=760O2lDB-TM&t=333s)
+- [aiida-diff setup.json](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=240s)
+- [run aiida-diff example calculation](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=403s)
+- [aiida-diff CalcJob plugin](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=685s)
+- [aiida-diff Parser plugin](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=936s)
+- [aiida-diff computer/code helpers](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1238s)
+- [aiida-diff input data (with validation)](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1353s)
+- [aiida-diff cli](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1621s)
+- [aiida-diff tests](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1931s)
+- [Adding your plugin to the registry](https://www.youtube.com/watch?v=760O2lDB-TM&t=112s)
+- [pre-commit hooks](https://www.youtube.com/watch?v=760O2lDB-TM&t=333s)
 
 For more information, see the [developer guide](https://aiida-diff.readthedocs.io/en/latest/developer_guide) of your plugin.
 
-
 ## Features
 
- * Add input files using `SinglefileData`:
-   ```python
-   SinglefileData = DataFactory('singlefile')
-   inputs['file1'] = SinglefileData(file='/path/to/file1')
-   inputs['file2'] = SinglefileData(file='/path/to/file2')
-   ```
-
- * Specify command line options via a python dictionary and `DiffParameters`:
-   ```python
-   d = { 'ignore-case': True }
-   DiffParameters = DataFactory('aurora')
-   inputs['parameters'] = DiffParameters(dict=d)
-   ```
-
- * `DiffParameters` dictionaries are validated using [voluptuous](https://github.com/alecthomas/voluptuous).
-   Find out about supported options:
-   ```python
-   DiffParameters = DataFactory('aurora')
-   print(DiffParameters.schema.schema)
-   ```
+- Add input files using `SinglefileData`:
+
+  ```python
+  SinglefileData = DataFactory('singlefile')
+  inputs['file1'] = SinglefileData(file='/path/to/file1')
+  inputs['file2'] = SinglefileData(file='/path/to/file2')
+  ```
+
+- Specify command line options via a python dictionary and `DiffParameters`:
+
+  ```python
+  d = { 'ignore-case': True }
+  DiffParameters = DataFactory('aurora')
+  inputs['parameters'] = DiffParameters(dict=d)
+  ```
+
+- `DiffParameters` dictionaries are validated using [voluptuous](https://github.com/alecthomas/voluptuous).
+  Find out about supported options:
+
+  ```python
+  DiffParameters = DataFactory('aurora')
+  print(DiffParameters.schema.schema)
+  ```
 
 ## Installation
 
 ```shell
 pip install aiida-aurora
 verdi quicksetup  # better to set up a new profile
 verdi plugin list aiida.calculations  # should now show your calclulation plugins
 ```
 
-
 ## Usage
 
 Here goes a complete example of how to submit a test calculation using this plugin.
 
 A quick demo of how to submit a calculation:
+
 ```shell
 verdi daemon start     # make sure the daemon is running
 cd examples
 ./example_01.py        # run test calculation
 verdi process list -a  # check record of calculation
 ```
 
 The plugin also includes verdi commands to inspect its data types:
+
 ```shell
 verdi data aurora list
 verdi data aurora export <PK>
 ```
 
 ## Development
 
@@ -112,10 +114,13 @@
 ```
 
 See the [developer guide](http://aiida-aurora.readthedocs.io/en/latest/developer_guide/index.html) for more information.
 
 ## License
 
 MIT
+
 ## Contact
 
-loris.ercole@epfl.ch
+francisco.ramirez@epfl.ch
+edan.bainglass@psi.ch
+giovanni.pizzi@psi.ch
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/calculations/cycler.py` & `aiida_aurora-0.3.2/aiida_aurora/calculations/cycler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Battery cycling experiment CalcJobs.
 """
 from typing import Optional
 
-from aurora.schemas.dgbowl_schemas import conversion_map, payload_models
 import yaml
 
 from aiida.common import datastructures
 from aiida.engine import CalcJob
 from aiida.engine.processes.exit_code import ExitCode
 from aiida.orm import ArrayData, Node, SinglefileData
 
-from aiida_aurora.data.battery import BatterySampleData, BatteryStateData
+from aiida_aurora.data.battery import BatterySampleData
+# TODO: from aiida_aurora.data.battery import BatteryStateData
 from aiida_aurora.data.control import TomatoSettingsData
 from aiida_aurora.data.experiment import CyclingSpecsData
+from aiida_aurora.schemas.dgbowl import conversion_map, payload_models
 
 
 class BatteryCyclerExperiment(CalcJob):
     """
     AiiDA calculation plugin for the tomato instrument automation package.
     https://github.com/dgbowl/tomato
     """
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/calculations/fake.py` & `aiida_aurora-0.3.2/aiida_aurora/calculations/fake.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 Dummy CalcJobs to simulate a battery experiment.
 """
 from aiida.common import datastructures
 from aiida.engine import CalcJob
 # from aiida.orm import SinglefileData
 from aiida.orm import Dict
 
-from aiida_aurora.data.battery import BatterySampleData, BatteryStateData
+from aiida_aurora.data.battery import BatterySampleData
+# TODO: from aiida_aurora.data.battery import BatteryStateData
 from aiida_aurora.data.experiment import CyclingSpecsData
 
 
 class BatteryFakeExperiment(CalcJob):
     """
     AiiDA calculation plugin for the fake_aurora_server script.
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/cli.py` & `aiida_aurora-0.3.2/aiida_aurora/cli.py`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/aiida_aurora/data/battery.py` & `aiida_aurora-0.3.2/aiida_aurora/data/battery.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 Data types provided by plugin
 
 Register data types via the "aiida.data" entry point in setup.json.
 """
 
 import json
 
-from aurora.schemas.battery import BatterySample as BatterySampleSchema
-from aurora.schemas.battery import BatteryState as BatteryStateSchema
 import yaml
 
 from aiida.orm import Dict
 
+from aiida_aurora.schemas.battery import BatterySample as BatterySampleSchema
+from aiida_aurora.schemas.battery import BatteryState as BatteryStateSchema
+
 
 class BatterySampleData(Dict):  # pylint: disable=too-many-ancestors
     """
     A battery sample data object.
 
     This class represents a battery sample.
     """
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/data/control.py` & `aiida_aurora-0.3.2/aiida_aurora/data/control.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 A dummy experiment specifications class.
 """
 import json
 
-from aurora.schemas.dgbowl_schemas import conversion_map
 import yaml
 
 from aiida.orm import Dict
 
+from aiida_aurora.schemas.dgbowl import conversion_map
+
 TOMATO_PAYLOAD_VERSION = "0.2"
 TomatoSchema = conversion_map[TOMATO_PAYLOAD_VERSION]["tomato"]
 
 
 class TomatoSettingsData(Dict):  # pylint: disable=too-many-ancestors
     """
     An experiment specification object.
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/data/experiment.py` & `aiida_aurora-0.3.2/aiida_aurora/data/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 A dummy experiment specifications class.
 """
 
 import json
 
-from aurora.schemas.cycling import ElectroChemSequence as ElectroChemSequenceSchema
 import yaml
 
 from aiida.orm import Dict
 
+from aiida_aurora.schemas.cycling import ElectroChemSequence as ElectroChemSequenceSchema
+
 
 class CyclingSpecsData(Dict):  # pylint: disable=too-many-ancestors
     """
     An experiment specification object.
 
     This class represents the specifications used in an experiment.
     """
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/helpers.py` & `aiida_aurora-0.3.2/aiida_aurora/helpers.py`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/aiida_aurora/parsers.py` & `aiida_aurora-0.3.2/aiida_aurora/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,19 @@
 
 BatteryCyclerExperiment = CalculationFactory("aurora.cycler")
 
 
 class TomatoParser(Parser):
     """
     Parser class for parsing the output of a BatteryCyclerExperiment generated by tomato.
+
     Two files should be found in the working directory:
+
       - a ZIP file, containing the raw data
+
       - a JSON file, containing the data pre-processed by tomato & yadg
 
     Priority is to retrieve the parsed JSON file.
     The raw data ZIP file is also retained if found.
     """
 
     def __init__(self, node):
@@ -65,15 +68,15 @@
                 self.logger.warning(f"The raw data zip file '{output_zip_filename}' could not be read.")
                 output_raw_data_node_created = False
         else:
             self.logger.warning(f"The raw data zip file '{output_zip_filename}' is missing.")
             output_raw_data_node_created = False
 
         # Check that json file is present
-        if not output_json_filename in files_retrieved:
+        if output_json_filename not in files_retrieved:
             self.logger.error(f"The output json file '{output_json_filename}' is missing.")
             if output_raw_data_node_created:
                 # only json file is missing
                 return self.exit_codes.ERROR_OUTPUT_JSON_MISSING
             # both files are missing
             return self.exit_codes.ERROR_OUTPUT_FILES_MISSING
 
@@ -106,17 +109,20 @@
 
     @staticmethod
     def parse_tomato_results(data_dic, logger=None):
         """
         Parse results.json file.
 
         :returns: a :class:`aiida.orm.ArrayData` in this way:
+
           - `metadata` is stored as attribute
+
           - `data` is split in steps, physical quantity name, and n/s/u identifier (nominal value, std error, units)
             The name of each array is:  `'step{step_number}_{raw_quantity_name}_{identifier}'`
+
         """
         array_dic = {}
         for imstep, mstep in enumerate(data_dic["steps"]):  # method step
             raw_qty_names = list(mstep["data"][0]["raw"].keys())
             if logger:
                 logger.debug(f"parse_tomato_results: step {imstep}: {list(raw_qty_names)}")
             for raw_qty_name in raw_qty_names:
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/scheduler.py` & `aiida_aurora-0.3.2/aiida_aurora/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 from aiida.common.extendeddicts import AttributeDict
 from aiida.schedulers import Scheduler, SchedulerError
 from aiida.schedulers.datastructures import JobInfo, JobResource, JobState
 
 # There is no "job owner" in tomato.
 
 # Mapping of Tomato states to AiiDA `JobState`s
-## The following statuses are defined in tomato:
-## q  job is queued. Jobs shouldn't stay in q too long as that indicates there
-##      is no pipeline that can process the payload.
-## qw job is queued and a matching pipeline has been found, but it is either busy,
-##      not ready, or without the correct sample
-## r  job is running
-## c  job has completed successfully
-## ce job has completed with an error - output data not guaranteed, might be present in the job folder.
-## cd job has been cancelled - output data should be available as specified in the yamlfile
+#
+# The following statuses are defined in tomato:
+#  - q   job is queued. Jobs shouldn't stay in q too long as that indicates there
+#        is no pipeline that can process the payload.
+#  - qw  job is queued and a matching pipeline has been found, but it is either busy,
+#        not ready, or without the correct sample
+#  - r   job is running
+#  - c   job has completed successfully
+#  - ce  job has completed with an error - output data not guaranteed, might be present in the job folder.
+#  - cd  job has been cancelled - output data should be available as specified in the yamlfile
 
 _MAP_STATUS_TOMATO = {
     "q": JobState.QUEUED,  # JobState.QUEUED_HELD ?
     "qw": JobState.QUEUED,
     "r": JobState.RUNNING,
     "c": JobState.DONE,
     "ce": JobState.DONE,
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/utils/cycling_analysis.py` & `aiida_aurora-0.3.2/aiida_aurora/utils/cycling_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import itertools
 import json
+
 import numpy as np
-from aiida.orm import ArrayData, RemoteData, CalcJobNode, QueryBuilder
+
+from aiida.common.exceptions import AiidaException
+from aiida.orm import ArrayData, CalcJobNode, QueryBuilder, RemoteData
+
 
 def get_data_from_raw(jsdata):
     "Extract raw data from json file."
     if not isinstance(jsdata, dict):
         raise TypeError('jsdata should be a dictionary')
     if len(jsdata["steps"]) > 1:
         raise NotImplementedError('Analysis of multiple steps is not implemented.')
@@ -20,15 +24,15 @@
 
     # find indices of sign changes in I
     idx = np.where(np.diff(np.sign(I)) != 0)[0]
 
     # integrate and store charge and discharge currents
     Qc, Qd = [], []
     for ii in range(len(idx) - 1):
-        i0, ie = idx[ii], idx[ii+1]
+        i0, ie = idx[ii], idx[ii + 1]
         q = np.trapz(I[i0:ie], t[i0:ie])
         if q > 0:
             Qc.append(q)
         else:
             Qd.append(abs(q))
     data = {
         'time': t,
@@ -37,14 +41,15 @@
         'cn': cn,
         'time-cycles': t[idx[2::2]],
         'Qd': np.array(Qd),
         'Qc': np.array(Qc)
     }
     return data
 
+
 def get_data_from_results(array_node):
     "Extract data from parsed ArrayData node."
     if not isinstance(array_node, ArrayData):
         raise TypeError('array_node should be an ArrayData')
 
     # collect data
     t = array_node.get_array('step0_uts')
@@ -55,15 +60,15 @@
 
     # find indices of sign changes in I
     idx = np.where(np.diff(np.sign(I)) != 0)[0]
 
     # integrate and store charge and discharge currents
     Qc, Qd = [], []
     for ii in range(len(idx) - 1):
-        i0, ie = idx[ii], idx[ii+1]
+        i0, ie = idx[ii], idx[ii + 1]
         q = np.trapz(I[i0:ie], t[i0:ie])
         if q > 0:
             Qc.append(q)
         else:
             Qd.append(abs(q))
     data = {
         'time': t,
@@ -72,20 +77,22 @@
         'cn': cn,
         'time-cycles': t[idx[2::2]],
         'Qd': np.array(Qd),
         'Qc': np.array(Qc)
     }
     return data
 
+
 def get_capacities(data_dic, discharge=True):
     if discharge:
         return data_dic['Qd']
     else:
         return data_dic['Qc']
 
+
 def analyze_cycling_results(data, consecutive_cycles, threshold, discharge):
     """Analyse cycling results.
     `data` should be a dictionary generated by `get_data_from_*`.
     """
     Qs = get_capacities(data, discharge=discharge)
     print(f"  capacities:          {Qs}")
     print(f"  relative capacities: {Qs / Qs[0]}")
@@ -95,30 +102,37 @@
         below_thresh = Qs < threshold * Qs[0]
         below_groups = [sum(1 for _ in g) for k, g in itertools.groupby(below_thresh) if k]
         for g in below_groups:
             if g > consecutive_cycles:
                 print(f'Below threshold for {g} cycles!')
     return data
 
+
 def cycling_analysis(calcjob_node, retrieve_monitor_params=False, consecutive_cycles=2, threshold=0.8, discharge=True):
     """Perform the cycling analysis. You can provide either the cycler or the monitor calcjob.
     First, it will try to find and analyse any output of the cycler calcjob.
     If this does not succeed, the monitor calcjob outputs will be analysed (the results or the last snapshot).
 
       retrieve_monitor_params :  if True, try to load the monitor parameters from the inputs
     """
-    
+
     monitor_calcjob = None
     if calcjob_node.process_type == 'aiida.calculations:aurora.cycler':
         calcjob = calcjob_node
         if calcjob.get_extra('monitored', False):
             # find last monitor, if existing
             qb = QueryBuilder()
             qb.append(RemoteData, filters={'uuid': calcjob.outputs.remote_folder.uuid}, tag='rf')
-            qb.append(CalcJobNode, with_incoming='rf', edge_filters={'label': 'monitor_folder'}, project=['*', 'id'], tag='mon')
+            qb.append(
+                CalcJobNode,
+                with_incoming='rf',
+                edge_filters={'label': 'monitor_folder'},
+                project=['*', 'id'],
+                tag='mon'
+            )
             qb.order_by({'mon': {'id': 'desc'}})
             monitor_calcjob = qb.first()[0] if qb.count() else None
     elif calcjob_node.process_type == 'aiida.calculations:calcmonitor.calcjob_monitor':
         monitor_calcjob = calcjob_node
         calcjob = monitor_calcjob.inputs.monitor_folder.get_incoming().get_node_by_label('remote_folder')
     else:
         raise TypeError('calcjob_node should be a BatteryCyclerExperiment or a CalcjobMonitor')
@@ -134,15 +148,15 @@
 
     if monitor_calcjob:
         try:
             options = monitor_calcjob.inputs.monitor_protocols['monitor1'].get_attribute('options')
             threshold = options['threshold']
             discharge = (options['check_type'] == 'discharge_capacity')
             consecutive_cycles = options['consecutive_cycles']
-        except aiida.common.exceptions.AiidaException:
+        except AiidaException:
             # use default values
             pass
     print(f"Analysis options:")
     print(f"  check type:        ", "discharge capacity" if discharge else "charge capacity")
     print(f"  threshold:          {threshold}")
     print(f"  consecutive cycles: {consecutive_cycles}")
 
@@ -166,26 +180,29 @@
 
     def analyse_monitor_calcjob():
         output_labels = monitor_calcjob.get_outgoing().all_link_labels()
         if 'redirected_outputs__results' in output_labels:
             print('Analysing redirected output results')
             res = monitor_calcjob.outputs.redirected_outputs.results
             return analyze_cycling_results(get_data_from_results(res), consecutive_cycles, threshold, discharge)
-        elif 'redirected_outputs__raw_data' in output_labels and 'results.json' in monitor_calcjob.outputs.redirected_outputs.raw_data.list_object_names():
+        elif 'redirected_outputs__raw_data' in output_labels and 'results.json' in monitor_calcjob.outputs.redirected_outputs.raw_data.list_object_names(
+        ):
             print('Analysing redirected output raw_data')
             jsdata = json.loads(monitor_calcjob.outputs.redirected_outputs.get_object_content('results.json'))
             return analyze_cycling_results(get_data_from_raw(jsdata), consecutive_cycles, threshold, discharge)
         elif 'retrieved' in output_labels and 'results.json' in monitor_calcjob.outputs.retrieved.list_object_names():
             print('Analysing retrieved results.json file')
             jsdata = json.loads(monitor_calcjob.outputs.retrieved.get_object_content('results.json'))
             return analyze_cycling_results(get_data_from_raw(jsdata), consecutive_cycles, threshold, discharge)
         elif 'remote_folder' in output_labels:
             try:
                 print('Analysing last snapshot.json file')
-                with open(f"{monitor_calcjob.outputs.remote_folder.get_attribute('remote_path')}/snapshot.json", 'r') as fileobj:
+                with open(
+                    f"{monitor_calcjob.outputs.remote_folder.get_attribute('remote_path')}/snapshot.json"
+                ) as fileobj:
                     jsdata = json.load(fileobj)
                 return analyze_cycling_results(get_data_from_raw(jsdata), consecutive_cycles, threshold, discharge)
             except FileNotFoundError:
                 print('ERROR! Monitor CalcJob: no output found.')
                 return None
         else:
             return None
@@ -202,8 +219,8 @@
             data = analyse_calcjob()
         except Exception as err:
             print(err)
             data = analyse_monitor_calcjob()
         else:
             if data is None:
                 data = analyse_monitor_calcjob()
-    return data
+    return data
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/utils/plot.py` & `aiida_aurora-0.3.2/aiida_aurora/utils/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-import numpy as np
 import matplotlib.pyplot as plt
-from matplotlib.ticker import MultipleLocator
+
 
 def create_figure(title=None):
     fig, axx = plt.subplots(1, figsize=(9, 4))
     plt.subplots_adjust(left=0.1, right=0.95, bottom=0.15, top=0.9)
     if title:
         fig.suptitle(title)
     return fig, axx
 
+
 def plot_Ewe(data):
     fig, axx = create_figure()
     axx.plot(data["time"] / 3600., data["Ewe"], label='Ewe')
     axx.set_xlabel('t [h]')
     axx.set_ylabel('Ewe [V]')
 
+
 def plot_I(data):
     fig, axx = create_figure()
     axx.plot(data["time"] / 3600., data["I"] * 1000., label='I')
     axx.set_xlabel('t [h]')
     axx.set_ylabel('I [mA]')
     return fig
 
+
 def plot_Ewe_I(data):
     fig, axx = create_figure()
     axx.plot(data["time"] / 3600., data["Ewe"], label='Ewe')
     axx.set_xlabel('t [h]')
     axx.set_ylabel('Ewe [V]', c='b')
 
     ax2 = axx.twinx()
     ax2.plot(data["time"] / 3600, data["I"] * 1000., 'r--', label='I')
     ax2.set_ylabel('I [mA]', c='r')
 
+
 def plot_Qd(data, ytick=0.05):
     fig, axx = create_figure()
     axx.plot(range(1, len(data['Qd']) + 1), data['Qd'] / 3.6, '.-', label='Qd')
     axx.set_xlabel('cycle')
     axx.set_ylabel('Qd [mAh]')
     axx.axhline(data['Qd'][0] * 0.8 / 3.6, ls='--', c='r')
     axx.set_xlim([0, None])
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/workflows/stress_test.py` & `aiida_aurora-0.3.2/aiida_aurora/workflows/stress_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-# -*- coding: utf-8 -*-
 """Description
 """
 import json
 import pathlib
 
 from pydantic.utils import deep_update
 
 from aiida import orm
 from aiida.common import AttributeDict
 from aiida.engine import ToContext, WorkChain
-from aiida.plugins import CalculationFactory, DataFactory
+from aiida.plugins import CalculationFactory, DataFactory, WorkflowFactory
 
 TomatoCalcjob = CalculationFactory('aurora.cycler')
-CyclingSpecsData = aiida.plugins.DataFactory('aurora.cyclingspecs')
-BatterySampleData = aiida.plugins.DataFactory('aurora.batterysample')
-TomatoSettingsData = aiida.plugins.DataFactory('aurora.tomatosettings')
+CyclingSpecsData = DataFactory('aurora.cyclingspecs')
+BatterySampleData = DataFactory('aurora.batterysample')
+TomatoSettingsData = DataFactory('aurora.tomatosettings')
 
 CalcjobMonitor = WorkflowFactory('calcmonitor.monitor_wrapper')
-TomatoMonitorData = aiida.plugins.DataFactory('calcmonitor.monitor.tomatobiologic')
+TomatoMonitorData = DataFactory('calcmonitor.monitor.tomatobiologic')
 
 BASEPATH = pathlib.Path(__file__).parent.resolve()
-with open(f'{BASEPATH}/stress_test_defaults.json', 'r') as fileobj:
+with open(f'{BASEPATH}/stress_test_defaults.json') as fileobj:
     ALL_DEFAULTS = json.load(fileobj)
 
 DEFAULT_TOMATO_SETTINGS = ALL_DEFAULTS['DEFAULT_TOMATO_SETTINGS']
 DEFAULT_MONITOR_PROTOCOL = ALL_DEFAULTS['DEFAULT_MONITOR_PROTOCOL']
 DEFAULT_PROTECTION_METHOD = ALL_DEFAULTS['DEFAULT_PROTECTION_METHOD']
 DEFAULT_FORMATION_METHOD = ALL_DEFAULTS['DEFAULT_FORMATION_METHOD']
 DEFAULT_LONGTERM_METHOD = ALL_DEFAULTS['DEFAULT_LONGTERM_METHOD']
@@ -51,35 +50,36 @@
             cls.run_protection_precycle,
             cls.run_formation_cycle,
             cls.run_longterm_cycling,
             cls.run_discharge_procedure,
             cls.gather_results,
         )
 
-        spec.output("results_protection", valid_type=ArrayData, help="Results of the protection step.")
-        spec.output("results_formation", valid_type=ArrayData, help="Results of the formation step.")
-        spec.output("results_cycling", valid_type=ArrayData, help="Results of the main cycling experiment.")
-        spec.output("results_discharge", valid_type=ArrayData, help="Results of the final discharge.")
+        spec.output("results_protection", valid_type=orm.ArrayData, help="Results of the protection step.")
+        spec.output("results_formation", valid_type=orm.ArrayData, help="Results of the formation step.")
+        spec.output("results_cycling", valid_type=orm.ArrayData, help="Results of the main cycling experiment.")
+        spec.output("results_discharge", valid_type=orm.ArrayData, help="Results of the final discharge.")
 
         spec.exit_code(
             501,
             "WARNING_CHARGED_SAMPLE",
             message="The battery sample was not correctly discharged after the procedure."
         )
 
         # yapf: enable
 
     @classmethod
-    def get_builder_from_protocol(cls,
-        ketchup_code = None,
-        monitor_code = None,
-        battery_sample = None,
-        tomato_overrides = None,
-        cycler_overrides = None,
-        monitor_overrides = None,
+    def get_builder_from_protocol(
+        cls,
+        ketchup_code=None,
+        monitor_code=None,
+        battery_sample=None,
+        tomato_overrides=None,
+        cycler_overrides=None,
+        monitor_overrides=None,
         protocol=None,
         overrides=None,
         **kwargs
     ):
         """
         Return a builder prepopulated with inputs selected according to the chosen protocol.
         """
@@ -98,15 +98,15 @@
             tomato_settings_dict = deep_update(tomato_settings_dict, tomato_overrides_dict)
 
         cycler_method_dict = DEFAULT_PROTECTION_METHOD
         if 'protection_cycle' in cycler_overrides:
             cycler_overrides_dict = cycler_overrides['protection_cycle']
             cycler_method_dict = mydeep_update(cycler_method_dict, cycler_overrides_dict)
 
-        builder = BatteryCyclerExperiment.get_builder()
+        builder = TomatoCalcjob.get_builder()
         builder.code = ketchup_code
         builder.technique = CyclingSpecsData(cycler_method_dict)
         builder.control_settings = TomatoSettingsData(tomato_settings_dict)
         workchain_builder.protection_cycle = builder
 
         # formation_cycle
         tomato_settings_dict = DEFAULT_TOMATO_SETTINGS
@@ -115,15 +115,15 @@
             tomato_settings_dict = deep_update(tomato_settings_dict, tomato_overrides_dict)
 
         cycler_method_dict = DEFAULT_FORMATION_METHOD
         if 'formation_cycle' in cycler_overrides:
             cycler_overrides_dict = cycler_overrides['formation_cycle']
             cycler_method_dict = mydeep_update(cycler_method_dict, cycler_overrides_dict)
 
-        builder = BatteryCyclerExperiment.get_builder()
+        builder = TomatoCalcjob.get_builder()
         builder.code = ketchup_code
         builder.technique = CyclingSpecsData(cycler_method_dict)
         builder.control_settings = TomatoSettingsData(tomato_settings_dict)
         workchain_builder.formation_cycle = builder
 
         # longterm_cycle (monitor)
         tomato_settings_dict = DEFAULT_TOMATO_SETTINGS
@@ -132,25 +132,25 @@
             tomato_settings_dict = deep_update(tomato_settings_dict, tomato_overrides_dict)
 
         cycler_method_dict = DEFAULT_LONGTERM_METHOD
         if 'longterm_cycle' in cycler_overrides:
             cycler_overrides_dict = cycler_overrides['longterm_cycle']
             cycler_method_dict = mydeep_update(cycler_method_dict, cycler_overrides_dict)
 
-        builder = BatteryCyclerExperiment.get_builder()
+        builder = TomatoCalcjob.get_builder()
         builder.code = ketchup_code
         builder.technique = CyclingSpecsData(cycler_method_dict)
         builder.control_settings = TomatoSettingsData(tomato_settings_dict)
         workchain_builder.longterm_cycle = builder
 
         monitor_protocol_dict = DEFAULT_MONITOR_PROTOCOL
         if monitor_overrides is not None:
             monitor_protocol_dict = deep_update(monitor_protocol_dict, monitor_overrides)
 
-        monitor_builder = TomatoMonitorCalcjob.get_builder()
+        monitor_builder = CalcjobMonitor.get_builder()
         monitor_builder.code = monitor_code
         monitor_builder.metadata.options.parser_name = "calcmonitor.cycler"
         monitor_protocol = TomatoMonitorData(dict=monitor_protocol_dict)
         monitor_builder.monitor_protocols = {'monitor1': monitor_protocol}
         workchain_builder.monitor = monitor_builder
 
         # discharge_cycle
@@ -161,23 +161,22 @@
             tomato_settings_dict = deep_update(tomato_settings_dict, tomato_overrides_dict)
 
         cycler_method_dict = DEFAULT_DISCHARGE_METHOD
         if 'discharge_cycle' in cycler_overrides:
             cycler_overrides_dict = cycler_overrides['discharge_cycle']
             cycler_method_dict = mydeep_update(cycler_method_dict, cycler_overrides_dict)
 
-        builder = BatteryCyclerExperiment.get_builder()
+        builder = TomatoCalcjob.get_builder()
         builder.code = ketchup_code
         builder.technique = CyclingSpecsData(cycler_method_dict)
         builder.control_settings = TomatoSettingsData(tomato_settings_dict)
         workchain_builder.discharge_cycle = builder
 
         return workchain_builder
 
-
     def run_protection_precycle(self):
         """TODO."""
         calcjob_dictin = self.exposed_inputs(TomatoCalcjob, namespace='protection_cycle')
         calcjob_inputs = AttributeDict(calcjob_dictin)
         battery_sample = self.inputs.battery_sample
         battery_name = battery_sample.attributes['metadata']['name']
         calcjob_inputs.sample = battery_sample
@@ -232,15 +231,15 @@
         formation_cycle_calcjob = self.ctx.formation_cycle_calcjob
         longterm_cycle_calcjob = self.ctx.longterm_cycle_calcjob
         monitor_workflow = self.ctx.monitor_workflow
         discharge_cycle_calcjob = self.ctx.discharge_cycle_calcjob
 
         if protection_cycle_calcjob.is_finished_ok:
             self.out('results_protection', protection_cycle_calcjob.outputs.results)
-        
+
         if formation_cycle_calcjob.is_finished_ok:
             self.out('results_formation', formation_cycle_calcjob.outputs.results)
 
         if longterm_cycle_calcjob.is_finished_ok:
             self.out('results_cycling', longterm_cycle_calcjob.outputs.results)
         elif longterm_cycle_calcjob.is_killed and monitor_workflow.calcjob.is_finished_ok:
             self.out('results_cycling', monitor_workflow.calcjob.outputs.results)
@@ -259,15 +258,15 @@
 
     steps0 = len(method_basis)
     steps = len(method_overrides)
     if steps0 != steps:
         raise ValueError(f"One of the overrides must have {steps0} steps instead of {steps} (leave steps empty).")
 
     new_method = []
-    for step_basis, step_override in zip(method_basis,method_overrides):
+    for step_basis, step_override in zip(method_basis, method_overrides):
         new_step = deep_update(step_basis, step_override)
         new_method.append(new_step)
 
     return {'method': new_method}
 
 
-####################################################################################################
+####################################################################################################
```

### Comparing `aiida_aurora-0.3.1/aiida_aurora/workflows/stress_test_defaults.json` & `aiida_aurora-0.3.2/aiida_aurora/workflows/stress_test_defaults.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -5,2019 +5,2019 @@
 00000040: 6c6c 2c20 2270 7265 6669 7822 3a20 6e75  ll, "prefix": nu
 00000050: 6c6c 7d2c 0a20 2020 2020 2020 2022 736e  ll},.        "sn
 00000060: 6170 7368 6f74 223a 206e 756c 6c2c 0a20  apshot": null,. 
 00000070: 2020 2020 2020 2022 7665 7262 6f73 6974         "verbosit
 00000080: 7922 3a20 2249 4e46 4f22 2c0a 2020 2020  y": "INFO",.    
 00000090: 2020 2020 2275 6e6c 6f63 6b5f 7768 656e      "unlock_when
 000000a0: 5f64 6f6e 6522 3a20 7472 7565 0a20 2020  _done": true.   
-000000b0: 207d 2c20 2020 200a 2020 2020 2244 4546   },    .    "DEF
-000000c0: 4155 4c54 5f4d 4f4e 4954 4f52 5f50 524f  AULT_MONITOR_PRO
-000000d0: 544f 434f 4c22 3a20 7b0a 2020 2020 2020  TOCOL": {.      
-000000e0: 2020 2273 6f75 7263 6573 223a 207b 0a20    "sources": {. 
-000000f0: 2020 2020 2020 2020 2020 2022 6f75 7470             "outp
-00000100: 7574 223a 207b 0a20 2020 2020 2020 2020  ut": {.         
-00000110: 2020 2020 2020 2022 6669 6c65 7061 7468         "filepath
-00000120: 223a 2022 736e 6170 7368 6f74 2e6a 736f  ": "snapshot.jso
-00000130: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-00000140: 2020 2020 2272 6566 7265 7368 5f72 6174      "refresh_rat
-00000150: 6522 3a20 3630 300a 2020 2020 2020 2020  e": 600.        
-00000160: 2020 2020 7d0a 2020 2020 2020 2020 7d2c      }.        },
-00000170: 0a20 2020 2020 2020 2022 6f70 7469 6f6e  .        "option
-00000180: 7322 3a20 7b0a 2020 2020 2020 2020 2020  s": {.          
-00000190: 2020 2263 6865 636b 5f74 7970 6522 3a20    "check_type": 
-000001a0: 2264 6973 6368 6172 6765 5f63 6170 6163  "discharge_capac
-000001b0: 6974 7922 2c0a 2020 2020 2020 2020 2020  ity",.          
-000001c0: 2020 2263 6f6e 7365 6375 7469 7665 5f63    "consecutive_c
-000001d0: 7963 6c65 7322 3a20 322c 0a20 2020 2020  ycles": 2,.     
-000001e0: 2020 2020 2020 2022 7468 7265 7368 6f6c         "threshol
-000001f0: 6422 3a20 302e 380a 2020 2020 2020 2020  d": 0.8.        
-00000200: 7d2c 0a20 2020 2020 2020 2022 7265 7472  },.        "retr
-00000210: 6965 7665 223a 205b 2272 6573 756c 7473  ieve": ["results
-00000220: 2e6a 736f 6e22 5d2c 0a20 2020 2020 2020  .json"],.       
-00000230: 2022 7265 7472 6965 7665 5f74 656d 706f   "retrieve_tempo
-00000240: 7261 7279 223a 205b 2272 6573 756c 7473  rary": ["results
-00000250: 2e7a 6970 225d 0a20 2020 207d 2c0a 2020  .zip"].    },.  
-00000260: 2020 2244 4546 4155 4c54 5f44 4953 4348    "DEFAULT_DISCH
-00000270: 4152 4745 5f4d 4554 484f 4422 3a20 7b0a  ARGE_METHOD": {.
-00000280: 2020 2020 2020 226d 6574 686f 6422 3a20        "method": 
-00000290: 5b0a 2020 2020 2020 2020 7b0a 2020 2020  [.        {.    
-000002a0: 2020 2020 2020 226e 616d 6522 3a20 2243        "name": "C
-000002b0: 435f 3122 2c0a 2020 2020 2020 2020 2020  C_1",.          
-000002c0: 2264 6576 6963 6522 3a20 224d 5047 3222  "device": "MPG2"
-000002d0: 2c0a 2020 2020 2020 2020 2020 2274 6563  ,.          "tec
-000002e0: 686e 6971 7565 223a 2022 636f 6e73 7461  hnique": "consta
-000002f0: 6e74 5f63 7572 7265 6e74 222c 0a20 2020  nt_current",.   
-00000300: 2020 2020 2020 2022 7061 7261 6d65 7465         "paramete
-00000310: 7273 223a 207b 0a20 2020 2020 2020 2020  rs": {.         
-00000320: 2020 2022 7469 6d65 223a 207b 0a20 2020     "time": {.   
-00000330: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
-00000340: 6c22 3a20 2254 696d 653a 222c 0a20 2020  l": "Time:",.   
-00000350: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
-00000360: 7322 3a20 2273 222c 0a20 2020 2020 2020  s": "s",.       
-00000370: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00000380: 3336 3030 302e 302c 0a20 2020 2020 2020  36000.0,.       
-00000390: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-000003a0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-000003b0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-000003c0: 696f 6e22 3a20 224d 6178 696d 756d 2064  ion": "Maximum d
-000003d0: 7572 6174 696f 6e20 6f66 2074 6865 2043  uration of the C
-000003e0: 4320 7374 6570 222c 0a20 2020 2020 2020  C step",.       
-000003f0: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
-00000400: 7661 6c75 6522 3a20 302e 300a 2020 2020  value": 0.0.    
-00000410: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000420: 2020 2020 2020 2022 455f 7261 6e67 6522         "E_range"
-00000430: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00000440: 2020 226c 6162 656c 223a 2022 4520 7261    "label": "E ra
-00000450: 6e67 6522 2c0a 2020 2020 2020 2020 2020  nge",.          
-00000460: 2020 2020 2275 6e69 7473 223a 2022 222c      "units": "",
-00000470: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00000480: 7661 6c75 6522 3a20 222b 2d35 2e30 2056  value": "+-5.0 V
-00000490: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000004a0: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
-000004b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000004c0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000004d0: 2253 656c 6563 7420 7468 6520 766f 6c74  "Select the volt
-000004e0: 6167 6520 7261 6e67 6520 6f66 2074 6865  age range of the
-000004f0: 2070 6f74 656e 7469 6f73 7461 7422 2c0a   potentiostat",.
-00000500: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00000510: 6566 6175 6c74 5f76 616c 7565 223a 2022  efault_value": "
-00000520: 6175 746f 220a 2020 2020 2020 2020 2020  auto".          
-00000530: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00000540: 2022 495f 7261 6e67 6522 3a20 7b0a 2020   "I_range": {.  
-00000550: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
-00000560: 656c 223a 2022 4920 7261 6e67 6522 2c0a  el": "I range",.
-00000570: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00000580: 6e69 7473 223a 2022 222c 0a20 2020 2020  nits": "",.     
-00000590: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-000005a0: 3a20 2231 3020 6d41 222c 0a20 2020 2020  : "10 mA",.     
-000005b0: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
-000005c0: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
-000005d0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-000005e0: 7074 696f 6e22 3a20 2253 656c 6563 7420  ption": "Select 
-000005f0: 7468 6520 6375 7272 656e 7420 7261 6e67  the current rang
-00000600: 6520 6f66 2074 6865 2070 6f74 656e 7469  e of the potenti
-00000610: 6f73 7461 7422 2c0a 2020 2020 2020 2020  ostat",.        
-00000620: 2020 2020 2020 2264 6566 6175 6c74 5f76        "default_v
-00000630: 616c 7565 223a 2022 6b65 6570 220a 2020  alue": "keep".  
-00000640: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00000650: 2020 2020 2020 2020 2022 6375 7272 656e           "curren
-00000660: 7422 3a20 7b0a 2020 2020 2020 2020 2020  t": {.          
-00000670: 2020 2020 226c 6162 656c 223a 2022 5374      "label": "St
-00000680: 6570 2063 7572 7265 6e74 3a22 2c0a 2020  ep current:",.  
-00000690: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
-000006a0: 7473 223a 2022 4922 2c0a 2020 2020 2020  ts": "I",.      
-000006b0: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
-000006c0: 2022 442f 3130 222c 0a20 2020 2020 2020   "D/10",.       
-000006d0: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-000006e0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-000006f0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00000700: 696f 6e22 3a20 2243 7572 7265 6e74 2064  ion": "Current d
-00000710: 7572 696e 6720 7468 6520 6375 7272 656e  uring the curren
-00000720: 7420 7374 6570 222c 0a20 2020 2020 2020  t step",.       
-00000730: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
-00000740: 7661 6c75 6522 3a20 302e 300a 2020 2020  value": 0.0.    
-00000750: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000760: 2020 2020 2020 2022 6973 5f64 656c 7461         "is_delta
-00000770: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000780: 2020 2022 6c61 6265 6c22 3a20 225c 7530     "label": "\u0
-00000790: 3339 3424 4924 3a22 2c0a 2020 2020 2020  394$I$:",.      
-000007a0: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-000007b0: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
-000007c0: 2020 2022 7661 6c75 6522 3a20 6661 6c73     "value": fals
-000007d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000007e0: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
-000007f0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00000800: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00000810: 2249 7320 7468 6520 7374 6570 2063 7572  "Is the step cur
-00000820: 7265 6e74 2061 2024 5c5c 4465 6c74 6124  rent a $\\Delta$
-00000830: 2066 726f 6d20 7072 6576 696f 7573 2073   from previous s
-00000840: 7465 703f 222c 0a20 2020 2020 2020 2020  tep?",.         
-00000850: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
-00000860: 6c75 6522 3a20 6661 6c73 650a 2020 2020  lue": false.    
-00000870: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000880: 2020 2020 2020 2022 6e5f 6379 636c 6573         "n_cycles
-00000890: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000008a0: 2020 2022 6c61 6265 6c22 3a20 224e 756d     "label": "Num
-000008b0: 6265 7220 6f66 2063 7963 6c65 733a 222c  ber of cycles:",
-000008c0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000008d0: 756e 6974 7322 3a20 2222 2c0a 2020 2020  units": "",.    
-000008e0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-000008f0: 223a 2030 2c0a 2020 2020 2020 2020 2020  ": 0,.          
-00000900: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
-00000910: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
-00000920: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00000930: 223a 2022 4379 636c 6520 7468 726f 7567  ": "Cycle throug
-00000940: 6820 7468 6520 6375 7272 656e 7420 7465  h the current te
-00000950: 6368 6e69 7175 6520 4e20 7469 6d65 732e  chnique N times.
-00000960: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000970: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
-00000980: 3a20 300a 2020 2020 2020 2020 2020 2020  : 0.            
-00000990: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-000009a0: 6578 6974 5f6f 6e5f 6c69 6d69 7422 3a20  exit_on_limit": 
-000009b0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000009c0: 226c 6162 656c 223a 2022 4578 6974 2077  "label": "Exit w
-000009d0: 6865 6e20 6c69 6d69 7473 2072 6561 6368  hen limits reach
-000009e0: 6564 3f22 2c0a 2020 2020 2020 2020 2020  ed?",.          
-000009f0: 2020 2020 2275 6e69 7473 223a 2022 222c      "units": "",
-00000a00: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00000a10: 7661 6c75 6522 3a20 6661 6c73 652c 0a20  value": false,. 
-00000a20: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00000a30: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
-00000a40: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00000a50: 7363 7269 7074 696f 6e22 3a20 2253 746f  scription": "Sto
-00000a60: 7020 7468 6520 7768 6f6c 6520 6578 7065  p the whole expe
-00000a70: 7269 6d65 6e74 2077 6865 6e20 6c69 6d69  riment when limi
-00000a80: 7420 6973 2072 6561 6368 6564 3f22 2c0a  t is reached?",.
-00000a90: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00000aa0: 6566 6175 6c74 5f76 616c 7565 223a 2066  efault_value": f
-00000ab0: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00000ac0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00000ad0: 2272 6563 6f72 645f 6576 6572 795f 6445  "record_every_dE
-00000ae0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000af0: 2020 2022 6c61 6265 6c22 3a20 2252 6563     "label": "Rec
-00000b00: 6f72 6420 6576 6572 7920 2464 4524 3a22  ord every $dE$:"
-00000b10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000b20: 2275 6e69 7473 223a 2022 5622 2c0a 2020  "units": "V",.  
-00000b30: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00000b40: 7565 223a 2030 2e31 2c0a 2020 2020 2020  ue": 0.1,.      
-00000b50: 2020 2020 2020 2020 2272 6571 7569 7265          "require
-00000b60: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
-00000b70: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00000b80: 7469 6f6e 223a 2022 5265 636f 7264 2061  tion": "Record a
-00000b90: 2064 6174 6170 6f69 6e74 2061 7420 7072   datapoint at pr
-00000ba0: 6573 6372 6962 6564 2076 6f6c 7461 6765  escribed voltage
-00000bb0: 2073 7061 6369 6e67 222c 0a20 2020 2020   spacing",.     
-00000bc0: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
-00000bd0: 745f 7661 6c75 6522 3a20 302e 3030 350a  t_value": 0.005.
-00000be0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00000bf0: 2020 2020 2020 2020 2020 2022 7265 636f             "reco
-00000c00: 7264 5f65 7665 7279 5f64 7422 3a20 7b0a  rd_every_dt": {.
-00000c10: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00000c20: 6162 656c 223a 2022 5265 636f 7264 2065  abel": "Record e
-00000c30: 7665 7279 2024 6474 243a 222c 0a20 2020  very $dt$:",.   
-00000c40: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
-00000c50: 7322 3a20 2273 222c 0a20 2020 2020 2020  s": "s",.       
-00000c60: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00000c70: 3630 2e30 2c0a 2020 2020 2020 2020 2020  60.0,.          
-00000c80: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
-00000c90: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
-00000ca0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00000cb0: 223a 2022 5265 636f 7264 2061 2064 6174  ": "Record a dat
-00000cc0: 6170 6f69 6e74 2061 7420 7072 6573 6372  apoint at prescr
-00000cd0: 6962 6564 2074 696d 6520 7370 6163 696e  ibed time spacin
-00000ce0: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
-00000cf0: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-00000d00: 223a 2033 302e 300a 2020 2020 2020 2020  ": 30.0.        
-00000d10: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00000d20: 2020 2022 6c69 6d69 745f 6375 7272 656e     "limit_curren
-00000d30: 745f 6d61 7822 3a20 7b0a 2020 2020 2020  t_max": {.      
-00000d40: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-00000d50: 2022 4d61 7869 6d75 6d20 6375 7272 656e   "Maximum curren
-00000d60: 743a 222c 0a20 2020 2020 2020 2020 2020  t:",.           
-00000d70: 2020 2022 756e 6974 7322 3a20 2249 222c     "units": "I",
-00000d80: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00000d90: 7661 6c75 6522 3a20 6e75 6c6c 2c0a 2020  value": null,.  
-00000da0: 2020 2020 2020 2020 2020 2020 2272 6571              "req
-00000db0: 7569 7265 6422 3a20 6661 6c73 652c 0a20  uired": false,. 
-00000dc0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00000dd0: 7363 7269 7074 696f 6e22 3a20 2244 6566  scription": "Def
-00000de0: 696e 6520 7468 6520 7570 7065 7220 6c69  ine the upper li
-00000df0: 6d69 7420 6f66 2063 7572 7265 6e74 2066  mit of current f
-00000e00: 6f72 2074 6869 7320 7374 6570 222c 0a20  or this step",. 
-00000e10: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00000e20: 6661 756c 745f 7661 6c75 6522 3a20 6e75  fault_value": nu
-00000e30: 6c6c 0a20 2020 2020 2020 2020 2020 207d  ll.            }
-00000e40: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-00000e50: 696d 6974 5f63 7572 7265 6e74 5f6d 696e  imit_current_min
-00000e60: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00000e70: 2020 2022 6c61 6265 6c22 3a20 224d 696e     "label": "Min
-00000e80: 696d 756d 2063 7572 7265 6e74 3a22 2c0a  imum current:",.
-00000e90: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00000ea0: 6e69 7473 223a 2022 4922 2c0a 2020 2020  nits": "I",.    
-00000eb0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-00000ec0: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
-00000ed0: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-00000ee0: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
-00000ef0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00000f00: 7469 6f6e 223a 2022 4465 6669 6e65 2074  tion": "Define t
-00000f10: 6865 206c 6f77 6572 206c 696d 6974 206f  he lower limit o
-00000f20: 6620 6375 7272 656e 7420 666f 7220 7468  f current for th
-00000f30: 6973 2073 7465 7022 2c0a 2020 2020 2020  is step",.      
-00000f40: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-00000f50: 5f76 616c 7565 223a 206e 756c 6c0a 2020  _value": null.  
-00000f60: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00000f70: 2020 2020 2020 2020 2022 6c69 6d69 745f           "limit_
-00000f80: 766f 6c74 6167 655f 6d61 7822 3a20 7b0a  voltage_max": {.
-00000f90: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00000fa0: 6162 656c 223a 2022 4d61 7869 6d75 6d20  abel": "Maximum 
-00000fb0: 766f 6c74 6167 653a 222c 0a20 2020 2020  voltage:",.     
-00000fc0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
-00000fd0: 3a20 2256 222c 0a20 2020 2020 2020 2020  : "V",.         
-00000fe0: 2020 2020 2022 7661 6c75 6522 3a20 322e       "value": 2.
-00000ff0: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-00001000: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
-00001010: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00001020: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00001030: 2022 4465 6669 6e65 2074 6865 2075 7070   "Define the upp
-00001040: 6572 206c 696d 6974 206f 6620 766f 6c74  er limit of volt
-00001050: 6167 6520 666f 7220 7468 6973 2073 7465  age for this ste
-00001060: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-00001070: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-00001080: 223a 206e 756c 6c0a 2020 2020 2020 2020  ": null.        
-00001090: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000010a0: 2020 2022 6c69 6d69 745f 766f 6c74 6167     "limit_voltag
-000010b0: 655f 6d69 6e22 3a20 7b0a 2020 2020 2020  e_min": {.      
-000010c0: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-000010d0: 2022 4d69 6e69 6d75 6d20 766f 6c74 6167   "Minimum voltag
-000010e0: 653a 222c 0a20 2020 2020 2020 2020 2020  e:",.           
-000010f0: 2020 2022 756e 6974 7322 3a20 2256 222c     "units": "V",
-00001100: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00001110: 7661 6c75 6522 3a20 312e 352c 0a20 2020  value": 1.5,.   
-00001120: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
-00001130: 6972 6564 223a 2066 616c 7365 2c0a 2020  ired": false,.  
-00001140: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00001150: 6372 6970 7469 6f6e 223a 2022 4465 6669  cription": "Defi
-00001160: 6e65 2074 6865 206c 6f77 6572 206c 696d  ne the lower lim
-00001170: 6974 206f 6620 766f 6c74 6167 6520 666f  it of voltage fo
-00001180: 7220 7468 6973 2073 7465 7022 2c0a 2020  r this step",.  
-00001190: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-000011a0: 6175 6c74 5f76 616c 7565 223a 206e 756c  ault_value": nul
-000011b0: 6c0a 2020 2020 2020 2020 2020 2020 7d0a  l.            }.
-000011c0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-000011d0: 2020 2020 2020 2022 7368 6f72 745f 6e61         "short_na
-000011e0: 6d65 223a 2022 4343 222c 0a20 2020 2020  me": "CC",.     
-000011f0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00001200: 6e22 3a20 2243 6f6e 7472 6f6c 6c65 6420  n": "Controlled 
-00001210: 6375 7272 656e 7420 7465 6368 6e69 7175  current techniqu
-00001220: 652c 2077 6974 6820 6f70 7469 6f6e 616c  e, with optional
-00001230: 2076 6f6c 7461 6765 2061 6e64 2063 7572   voltage and cur
-00001240: 7265 6e74 206c 696d 6974 7322 0a20 2020  rent limits".   
-00001250: 2020 2020 207d 0a20 2020 2020 205d 0a20       }.      ]. 
-00001260: 2020 207d 2c0a 2020 2020 2244 4546 4155     },.    "DEFAU
-00001270: 4c54 5f4c 4f4e 4754 4552 4d5f 4d45 5448  LT_LONGTERM_METH
-00001280: 4f44 223a 207b 0a20 2020 2020 2022 6d65  OD": {.      "me
-00001290: 7468 6f64 223a 205b 0a20 2020 2020 2020  thod": [.       
-000012a0: 207b 0a20 2020 2020 2020 2020 2022 6e61   {.          "na
-000012b0: 6d65 223a 2022 4343 5f31 222c 0a20 2020  me": "CC_1",.   
-000012c0: 2020 2020 2020 2022 6465 7669 6365 223a         "device":
-000012d0: 2022 4d50 4732 222c 0a20 2020 2020 2020   "MPG2",.       
-000012e0: 2020 2022 7465 6368 6e69 7175 6522 3a20     "technique": 
-000012f0: 2263 6f6e 7374 616e 745f 6375 7272 656e  "constant_curren
-00001300: 7422 2c0a 2020 2020 2020 2020 2020 2270  t",.          "p
-00001310: 6172 616d 6574 6572 7322 3a20 7b0a 2020  arameters": {.  
-00001320: 2020 2020 2020 2020 2020 2274 696d 6522            "time"
-00001330: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00001340: 2020 226c 6162 656c 223a 2022 5469 6d65    "label": "Time
-00001350: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
-00001360: 2020 2275 6e69 7473 223a 2022 7322 2c0a    "units": "s",.
-00001370: 2020 2020 2020 2020 2020 2020 2020 2276                "v
-00001380: 616c 7565 223a 2031 3038 3030 2e30 2c0a  alue": 10800.0,.
-00001390: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-000013a0: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000013c0: 6573 6372 6970 7469 6f6e 223a 2022 4d61  escription": "Ma
-000013d0: 7869 6d75 6d20 6475 7261 7469 6f6e 206f  ximum duration o
-000013e0: 6620 7468 6520 4343 2073 7465 7022 2c0a  f the CC step",.
-000013f0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00001400: 6566 6175 6c74 5f76 616c 7565 223a 2030  efault_value": 0
-00001410: 2e30 0a20 2020 2020 2020 2020 2020 207d  .0.            }
-00001420: 2c0a 2020 2020 2020 2020 2020 2020 2245  ,.            "E
-00001430: 5f72 616e 6765 223a 207b 0a20 2020 2020  _range": {.     
-00001440: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00001450: 3a20 2245 2072 616e 6765 222c 0a20 2020  : "E range",.   
-00001460: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
-00001470: 7322 3a20 2222 2c0a 2020 2020 2020 2020  s": "",.        
-00001480: 2020 2020 2020 2276 616c 7565 223a 2022        "value": "
-00001490: 2b2d 352e 3020 5622 2c0a 2020 2020 2020  +-5.0 V",.      
-000014a0: 2020 2020 2020 2020 2272 6571 7569 7265          "require
-000014b0: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
-000014c0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-000014d0: 7469 6f6e 223a 2022 5365 6c65 6374 2074  tion": "Select t
-000014e0: 6865 2076 6f6c 7461 6765 2072 616e 6765  he voltage range
-000014f0: 206f 6620 7468 6520 706f 7465 6e74 696f   of the potentio
-00001500: 7374 6174 222c 0a20 2020 2020 2020 2020  stat",.         
-00001510: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
-00001520: 6c75 6522 3a20 2261 7574 6f22 0a20 2020  lue": "auto".   
-00001530: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00001540: 2020 2020 2020 2020 2249 5f72 616e 6765          "I_range
-00001550: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00001560: 2020 2022 6c61 6265 6c22 3a20 2249 2072     "label": "I r
-00001570: 616e 6765 222c 0a20 2020 2020 2020 2020  ange",.         
-00001580: 2020 2020 2022 756e 6974 7322 3a20 2222       "units": ""
-00001590: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000015a0: 2276 616c 7565 223a 2022 3130 206d 4122  "value": "10 mA"
-000015b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000015c0: 2272 6571 7569 7265 6422 3a20 7472 7565  "required": true
-000015d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000015e0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-000015f0: 5365 6c65 6374 2074 6865 2063 7572 7265  Select the curre
-00001600: 6e74 2072 616e 6765 206f 6620 7468 6520  nt range of the 
-00001610: 706f 7465 6e74 696f 7374 6174 222c 0a20  potentiostat",. 
-00001620: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00001630: 6661 756c 745f 7661 6c75 6522 3a20 226b  fault_value": "k
-00001640: 6565 7022 0a20 2020 2020 2020 2020 2020  eep".           
-00001650: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00001660: 2263 7572 7265 6e74 223a 207b 0a20 2020  "current": {.   
-00001670: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
-00001680: 6c22 3a20 2253 7465 7020 6375 7272 656e  l": "Step curren
-00001690: 743a 222c 0a20 2020 2020 2020 2020 2020  t:",.           
-000016a0: 2020 2022 756e 6974 7322 3a20 2249 222c     "units": "I",
-000016b0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000016c0: 7661 6c75 6522 3a20 2243 2f33 222c 0a20  value": "C/3",. 
-000016d0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-000016e0: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
-000016f0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00001700: 7363 7269 7074 696f 6e22 3a20 2243 7572  scription": "Cur
-00001710: 7265 6e74 2064 7572 696e 6720 7468 6520  rent during the 
-00001720: 6375 7272 656e 7420 7374 6570 222c 0a20  current step",. 
-00001730: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00001740: 6661 756c 745f 7661 6c75 6522 3a20 302e  fault_value": 0.
-00001750: 300a 2020 2020 2020 2020 2020 2020 7d2c  0.            },
-00001760: 0a20 2020 2020 2020 2020 2020 2022 6973  .            "is
-00001770: 5f64 656c 7461 223a 207b 0a20 2020 2020  _delta": {.     
-00001780: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00001790: 3a20 225c 7530 3339 3424 4924 3a22 2c0a  : "\u0394$I$:",.
-000017a0: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-000017b0: 6e69 7473 223a 2022 222c 0a20 2020 2020  nits": "",.     
-000017c0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-000017d0: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-000017e0: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-000017f0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-00001800: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00001810: 696f 6e22 3a20 2249 7320 7468 6520 7374  ion": "Is the st
-00001820: 6570 2063 7572 7265 6e74 2061 2024 5c5c  ep current a $\\
-00001830: 4465 6c74 6124 2066 726f 6d20 7072 6576  Delta$ from prev
-00001840: 696f 7573 2073 7465 703f 222c 0a20 2020  ious step?",.   
-00001850: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
-00001860: 756c 745f 7661 6c75 6522 3a20 6661 6c73  ult_value": fals
-00001870: 650a 2020 2020 2020 2020 2020 2020 7d2c  e.            },
-00001880: 0a20 2020 2020 2020 2020 2020 2022 6e5f  .            "n_
-00001890: 6379 636c 6573 223a 207b 0a20 2020 2020  cycles": {.     
-000018a0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-000018b0: 3a20 224e 756d 6265 7220 6f66 2063 7963  : "Number of cyc
-000018c0: 6c65 733a 222c 0a20 2020 2020 2020 2020  les:",.         
-000018d0: 2020 2020 2022 756e 6974 7322 3a20 2222       "units": ""
-000018e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000018f0: 2276 616c 7565 223a 2030 2c0a 2020 2020  "value": 0,.    
-00001900: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
-00001910: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
-00001920: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00001930: 6970 7469 6f6e 223a 2022 4379 636c 6520  iption": "Cycle 
-00001940: 7468 726f 7567 6820 7468 6520 6375 7272  through the curr
-00001950: 656e 7420 7465 6368 6e69 7175 6520 4e20  ent technique N 
-00001960: 7469 6d65 732e 222c 0a20 2020 2020 2020  times.",.       
-00001970: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
-00001980: 7661 6c75 6522 3a20 300a 2020 2020 2020  value": 0.      
-00001990: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000019a0: 2020 2020 2022 6578 6974 5f6f 6e5f 6c69       "exit_on_li
-000019b0: 6d69 7422 3a20 7b0a 2020 2020 2020 2020  mit": {.        
-000019c0: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
-000019d0: 4578 6974 2077 6865 6e20 6c69 6d69 7473  Exit when limits
-000019e0: 2072 6561 6368 6564 3f22 2c0a 2020 2020   reached?",.    
-000019f0: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
-00001a00: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
-00001a10: 2020 2020 2022 7661 6c75 6522 3a20 6661       "value": fa
-00001a20: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00001a30: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
-00001a40: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00001a50: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00001a60: 3a20 2253 746f 7020 7468 6520 7768 6f6c  : "Stop the whol
-00001a70: 6520 6578 7065 7269 6d65 6e74 2077 6865  e experiment whe
-00001a80: 6e20 6c69 6d69 7420 6973 2072 6561 6368  n limit is reach
-00001a90: 6564 3f22 2c0a 2020 2020 2020 2020 2020  ed?",.          
-00001aa0: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
-00001ab0: 7565 223a 2066 616c 7365 0a20 2020 2020  ue": false.     
-00001ac0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00001ad0: 2020 2020 2020 2272 6563 6f72 645f 6576        "record_ev
-00001ae0: 6572 795f 6445 223a 207b 0a20 2020 2020  ery_dE": {.     
-00001af0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00001b00: 3a20 2252 6563 6f72 6420 6576 6572 7920  : "Record every 
-00001b10: 2464 4524 3a22 2c0a 2020 2020 2020 2020  $dE$:",.        
-00001b20: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
-00001b30: 5622 2c0a 2020 2020 2020 2020 2020 2020  V",.            
-00001b40: 2020 2276 616c 7565 223a 2030 2e31 2c0a    "value": 0.1,.
-00001b50: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00001b60: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00001b80: 6573 6372 6970 7469 6f6e 223a 2022 5265  escription": "Re
-00001b90: 636f 7264 2061 2064 6174 6170 6f69 6e74  cord a datapoint
-00001ba0: 2061 7420 7072 6573 6372 6962 6564 2076   at prescribed v
-00001bb0: 6f6c 7461 6765 2073 7061 6369 6e67 222c  oltage spacing",
-00001bc0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00001bd0: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
-00001be0: 302e 3030 350a 2020 2020 2020 2020 2020  0.005.          
-00001bf0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00001c00: 2022 7265 636f 7264 5f65 7665 7279 5f64   "record_every_d
-00001c10: 7422 3a20 7b0a 2020 2020 2020 2020 2020  t": {.          
-00001c20: 2020 2020 226c 6162 656c 223a 2022 5265      "label": "Re
-00001c30: 636f 7264 2065 7665 7279 2024 6474 243a  cord every $dt$:
-00001c40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00001c50: 2022 756e 6974 7322 3a20 2273 222c 0a20   "units": "s",. 
-00001c60: 2020 2020 2020 2020 2020 2020 2022 7661               "va
-00001c70: 6c75 6522 3a20 3630 2e30 2c0a 2020 2020  lue": 60.0,.    
-00001c80: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
-00001c90: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
-00001ca0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00001cb0: 6970 7469 6f6e 223a 2022 5265 636f 7264  iption": "Record
-00001cc0: 2061 2064 6174 6170 6f69 6e74 2061 7420   a datapoint at 
-00001cd0: 7072 6573 6372 6962 6564 2074 696d 6520  prescribed time 
-00001ce0: 7370 6163 696e 6722 2c0a 2020 2020 2020  spacing",.      
-00001cf0: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-00001d00: 5f76 616c 7565 223a 2033 302e 300a 2020  _value": 30.0.  
-00001d10: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00001d20: 2020 2020 2020 2020 2022 6c69 6d69 745f           "limit_
-00001d30: 6375 7272 656e 745f 6d61 7822 3a20 7b0a  current_max": {.
-00001d40: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00001d50: 6162 656c 223a 2022 4d61 7869 6d75 6d20  abel": "Maximum 
-00001d60: 6375 7272 656e 743a 222c 0a20 2020 2020  current:",.     
-00001d70: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
-00001d80: 3a20 2249 222c 0a20 2020 2020 2020 2020  : "I",.         
-00001d90: 2020 2020 2022 7661 6c75 6522 3a20 6e75       "value": nu
-00001da0: 6c6c 2c0a 2020 2020 2020 2020 2020 2020  ll,.            
-00001db0: 2020 2272 6571 7569 7265 6422 3a20 6661    "required": fa
-00001dc0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00001dd0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00001de0: 3a20 2244 6566 696e 6520 7468 6520 7570  : "Define the up
-00001df0: 7065 7220 6c69 6d69 7420 6f66 2063 7572  per limit of cur
-00001e00: 7265 6e74 2066 6f72 2074 6869 7320 7374  rent for this st
-00001e10: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
-00001e20: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
-00001e30: 6522 3a20 6e75 6c6c 0a20 2020 2020 2020  e": null.       
-00001e40: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00001e50: 2020 2020 226c 696d 6974 5f63 7572 7265      "limit_curre
-00001e60: 6e74 5f6d 696e 223a 207b 0a20 2020 2020  nt_min": {.     
-00001e70: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00001e80: 3a20 224d 696e 696d 756d 2063 7572 7265  : "Minimum curre
-00001e90: 6e74 3a22 2c0a 2020 2020 2020 2020 2020  nt:",.          
-00001ea0: 2020 2020 2275 6e69 7473 223a 2022 4922      "units": "I"
-00001eb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001ec0: 2276 616c 7565 223a 206e 756c 6c2c 0a20  "value": null,. 
-00001ed0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00001ee0: 7175 6972 6564 223a 2066 616c 7365 2c0a  quired": false,.
-00001ef0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00001f00: 6573 6372 6970 7469 6f6e 223a 2022 4465  escription": "De
-00001f10: 6669 6e65 2074 6865 206c 6f77 6572 206c  fine the lower l
-00001f20: 696d 6974 206f 6620 6375 7272 656e 7420  imit of current 
-00001f30: 666f 7220 7468 6973 2073 7465 7022 2c0a  for this step",.
-00001f40: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00001f50: 6566 6175 6c74 5f76 616c 7565 223a 206e  efault_value": n
-00001f60: 756c 6c0a 2020 2020 2020 2020 2020 2020  ull.            
-00001f70: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00001f80: 6c69 6d69 745f 766f 6c74 6167 655f 6d61  limit_voltage_ma
-00001f90: 7822 3a20 7b0a 2020 2020 2020 2020 2020  x": {.          
-00001fa0: 2020 2020 226c 6162 656c 223a 2022 4d61      "label": "Ma
-00001fb0: 7869 6d75 6d20 766f 6c74 6167 653a 222c  ximum voltage:",
-00001fc0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00001fd0: 756e 6974 7322 3a20 2256 222c 0a20 2020  units": "V",.   
-00001fe0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-00001ff0: 6522 3a20 322e 352c 0a20 2020 2020 2020  e": 2.5,.       
-00002000: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-00002010: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
-00002020: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00002030: 7469 6f6e 223a 2022 4465 6669 6e65 2074  tion": "Define t
-00002040: 6865 2075 7070 6572 206c 696d 6974 206f  he upper limit o
-00002050: 6620 766f 6c74 6167 6520 666f 7220 7468  f voltage for th
-00002060: 6973 2073 7465 7022 2c0a 2020 2020 2020  is step",.      
-00002070: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-00002080: 5f76 616c 7565 223a 206e 756c 6c0a 2020  _value": null.  
-00002090: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-000020a0: 2020 2020 2020 2020 2022 6c69 6d69 745f           "limit_
-000020b0: 766f 6c74 6167 655f 6d69 6e22 3a20 7b0a  voltage_min": {.
-000020c0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-000020d0: 6162 656c 223a 2022 4d69 6e69 6d75 6d20  abel": "Minimum 
-000020e0: 766f 6c74 6167 653a 222c 0a20 2020 2020  voltage:",.     
-000020f0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
-00002100: 3a20 2256 222c 0a20 2020 2020 2020 2020  : "V",.         
-00002110: 2020 2020 2022 7661 6c75 6522 3a20 312e       "value": 1.
-00002120: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00002130: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
-00002140: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00002150: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00002160: 2022 4465 6669 6e65 2074 6865 206c 6f77   "Define the low
-00002170: 6572 206c 696d 6974 206f 6620 766f 6c74  er limit of volt
-00002180: 6167 6520 666f 7220 7468 6973 2073 7465  age for this ste
-00002190: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-000021a0: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-000021b0: 223a 206e 756c 6c0a 2020 2020 2020 2020  ": null.        
-000021c0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-000021d0: 7d2c 0a20 2020 2020 2020 2020 2022 7368  },.          "sh
-000021e0: 6f72 745f 6e61 6d65 223a 2022 4343 222c  ort_name": "CC",
-000021f0: 0a20 2020 2020 2020 2020 2022 6465 7363  .          "desc
-00002200: 7269 7074 696f 6e22 3a20 2243 6f6e 7472  ription": "Contr
-00002210: 6f6c 6c65 6420 6375 7272 656e 7420 7465  olled current te
-00002220: 6368 6e69 7175 652c 2077 6974 6820 6f70  chnique, with op
-00002230: 7469 6f6e 616c 2076 6f6c 7461 6765 2061  tional voltage a
-00002240: 6e64 2063 7572 7265 6e74 206c 696d 6974  nd current limit
-00002250: 7322 0a20 2020 2020 2020 207d 2c0a 2020  s".        },.  
-00002260: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00002270: 2020 226e 616d 6522 3a20 2243 435f 3222    "name": "CC_2"
-00002280: 2c0a 2020 2020 2020 2020 2020 2264 6576  ,.          "dev
-00002290: 6963 6522 3a20 224d 5047 3222 2c0a 2020  ice": "MPG2",.  
-000022a0: 2020 2020 2020 2020 2274 6563 686e 6971          "techniq
-000022b0: 7565 223a 2022 636f 6e73 7461 6e74 5f63  ue": "constant_c
-000022c0: 7572 7265 6e74 222c 0a20 2020 2020 2020  urrent",.       
-000022d0: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-000022e0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-000022f0: 7469 6d65 223a 207b 0a20 2020 2020 2020  time": {.       
-00002300: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
-00002310: 2254 696d 653a 222c 0a20 2020 2020 2020  "Time:",.       
-00002320: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
-00002330: 2273 222c 0a20 2020 2020 2020 2020 2020  "s",.           
-00002340: 2020 2022 7661 6c75 6522 3a20 3130 3830     "value": 1080
-00002350: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
-00002360: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
-00002370: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00002380: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00002390: 3a20 224d 6178 696d 756d 2064 7572 6174  : "Maximum durat
-000023a0: 696f 6e20 6f66 2074 6865 2043 4320 7374  ion of the CC st
-000023b0: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
-000023c0: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
-000023d0: 6522 3a20 302e 300a 2020 2020 2020 2020  e": 0.0.        
-000023e0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000023f0: 2020 2022 455f 7261 6e67 6522 3a20 7b0a     "E_range": {.
-00002400: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00002410: 6162 656c 223a 2022 4520 7261 6e67 6522  abel": "E range"
-00002420: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002430: 2275 6e69 7473 223a 2022 222c 0a20 2020  "units": "",.   
-00002440: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-00002450: 6522 3a20 222b 2d35 2e30 2056 222c 0a20  e": "+-5.0 V",. 
-00002460: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00002470: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
-00002480: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00002490: 7363 7269 7074 696f 6e22 3a20 2253 656c  scription": "Sel
-000024a0: 6563 7420 7468 6520 766f 6c74 6167 6520  ect the voltage 
-000024b0: 7261 6e67 6520 6f66 2074 6865 2070 6f74  range of the pot
-000024c0: 656e 7469 6f73 7461 7422 2c0a 2020 2020  entiostat",.    
-000024d0: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
-000024e0: 6c74 5f76 616c 7565 223a 2022 6175 746f  lt_value": "auto
-000024f0: 220a 2020 2020 2020 2020 2020 2020 7d2c  ".            },
-00002500: 0a20 2020 2020 2020 2020 2020 2022 495f  .            "I_
-00002510: 7261 6e67 6522 3a20 7b0a 2020 2020 2020  range": {.      
-00002520: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-00002530: 2022 4920 7261 6e67 6522 2c0a 2020 2020   "I range",.    
-00002540: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
-00002550: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
-00002560: 2020 2020 2022 7661 6c75 6522 3a20 2231       "value": "1
-00002570: 3020 6d41 222c 0a20 2020 2020 2020 2020  0 mA",.         
-00002580: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
-00002590: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
-000025a0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-000025b0: 6e22 3a20 2253 656c 6563 7420 7468 6520  n": "Select the 
-000025c0: 6375 7272 656e 7420 7261 6e67 6520 6f66  current range of
-000025d0: 2074 6865 2070 6f74 656e 7469 6f73 7461   the potentiosta
-000025e0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-000025f0: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-00002600: 223a 2022 6b65 6570 220a 2020 2020 2020  ": "keep".      
-00002610: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00002620: 2020 2020 2022 6375 7272 656e 7422 3a20       "current": 
-00002630: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00002640: 226c 6162 656c 223a 2022 5374 6570 2063  "label": "Step c
-00002650: 7572 7265 6e74 3a22 2c0a 2020 2020 2020  urrent:",.      
-00002660: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-00002670: 2022 4922 2c0a 2020 2020 2020 2020 2020   "I",.          
-00002680: 2020 2020 2276 616c 7565 223a 2022 442f      "value": "D/
-00002690: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-000026a0: 2020 2272 6571 7569 7265 6422 3a20 7472    "required": tr
-000026b0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-000026c0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000026d0: 2022 4375 7272 656e 7420 6475 7269 6e67   "Current during
-000026e0: 2074 6865 2063 7572 7265 6e74 2073 7465   the current ste
-000026f0: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-00002700: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-00002710: 223a 2030 2e30 0a20 2020 2020 2020 2020  ": 0.0.         
-00002720: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00002730: 2020 2269 735f 6465 6c74 6122 3a20 7b0a    "is_delta": {.
-00002740: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00002750: 6162 656c 223a 2022 5c75 3033 3934 2449  abel": "\u0394$I
-00002760: 243a 222c 0a20 2020 2020 2020 2020 2020  $:",.           
-00002770: 2020 2022 756e 6974 7322 3a20 2222 2c0a     "units": "",.
-00002780: 2020 2020 2020 2020 2020 2020 2020 2276                "v
-00002790: 616c 7565 223a 2066 616c 7365 2c0a 2020  alue": false,.  
-000027a0: 2020 2020 2020 2020 2020 2020 2272 6571              "req
-000027b0: 7569 7265 6422 3a20 7472 7565 2c0a 2020  uired": true,.  
-000027c0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-000027d0: 6372 6970 7469 6f6e 223a 2022 4973 2074  cription": "Is t
-000027e0: 6865 2073 7465 7020 6375 7272 656e 7420  he step current 
-000027f0: 6120 245c 5c44 656c 7461 2420 6672 6f6d  a $\\Delta$ from
-00002800: 2070 7265 7669 6f75 7320 7374 6570 3f22   previous step?"
-00002810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002820: 2264 6566 6175 6c74 5f76 616c 7565 223a  "default_value":
-00002830: 2066 616c 7365 0a20 2020 2020 2020 2020   false.         
-00002840: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00002850: 2020 226e 5f63 7963 6c65 7322 3a20 7b0a    "n_cycles": {.
-00002860: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00002870: 6162 656c 223a 2022 4e75 6d62 6572 206f  abel": "Number o
-00002880: 6620 6379 636c 6573 3a22 2c0a 2020 2020  f cycles:",.    
-00002890: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
-000028a0: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
-000028b0: 2020 2020 2022 7661 6c75 6522 3a20 302c       "value": 0,
-000028c0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000028d0: 7265 7175 6972 6564 223a 2074 7275 652c  required": true,
-000028e0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000028f0: 6465 7363 7269 7074 696f 6e22 3a20 2243  description": "C
-00002900: 7963 6c65 2074 6872 6f75 6768 2074 6865  ycle through the
-00002910: 2063 7572 7265 6e74 2074 6563 686e 6971   current techniq
-00002920: 7565 204e 2074 696d 6573 2e22 2c0a 2020  ue N times.",.  
-00002930: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-00002940: 6175 6c74 5f76 616c 7565 223a 2030 0a20  ault_value": 0. 
-00002950: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00002960: 2020 2020 2020 2020 2020 2265 7869 745f            "exit_
-00002970: 6f6e 5f6c 696d 6974 223a 207b 0a20 2020  on_limit": {.   
-00002980: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
-00002990: 6c22 3a20 2245 7869 7420 7768 656e 206c  l": "Exit when l
-000029a0: 696d 6974 7320 7265 6163 6865 643f 222c  imits reached?",
-000029b0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000029c0: 756e 6974 7322 3a20 2222 2c0a 2020 2020  units": "",.    
-000029d0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-000029e0: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
-000029f0: 2020 2020 2020 2020 2272 6571 7569 7265          "require
-00002a00: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
-00002a10: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00002a20: 7469 6f6e 223a 2022 5374 6f70 2074 6865  tion": "Stop the
-00002a30: 2077 686f 6c65 2065 7870 6572 696d 656e   whole experimen
-00002a40: 7420 7768 656e 206c 696d 6974 2069 7320  t when limit is 
-00002a50: 7265 6163 6865 643f 222c 0a20 2020 2020  reached?",.     
-00002a60: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
-00002a70: 745f 7661 6c75 6522 3a20 6661 6c73 650a  t_value": false.
-00002a80: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00002a90: 2020 2020 2020 2020 2020 2022 7265 636f             "reco
-00002aa0: 7264 5f65 7665 7279 5f64 4522 3a20 7b0a  rd_every_dE": {.
-00002ab0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00002ac0: 6162 656c 223a 2022 5265 636f 7264 2065  abel": "Record e
-00002ad0: 7665 7279 2024 6445 243a 222c 0a20 2020  very $dE$:",.   
-00002ae0: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
-00002af0: 7322 3a20 2256 222c 0a20 2020 2020 2020  s": "V",.       
-00002b00: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00002b10: 302e 312c 0a20 2020 2020 2020 2020 2020  0.1,.           
-00002b20: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
-00002b30: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00002b40: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00002b50: 3a20 2252 6563 6f72 6420 6120 6461 7461  : "Record a data
-00002b60: 706f 696e 7420 6174 2070 7265 7363 7269  point at prescri
-00002b70: 6265 6420 766f 6c74 6167 6520 7370 6163  bed voltage spac
-00002b80: 696e 6722 2c0a 2020 2020 2020 2020 2020  ing",.          
-00002b90: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
-00002ba0: 7565 223a 2030 2e30 3035 0a20 2020 2020  ue": 0.005.     
-00002bb0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00002bc0: 2020 2020 2020 2272 6563 6f72 645f 6576        "record_ev
-00002bd0: 6572 795f 6474 223a 207b 0a20 2020 2020  ery_dt": {.     
-00002be0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00002bf0: 3a20 2252 6563 6f72 6420 6576 6572 7920  : "Record every 
-00002c00: 2464 7424 3a22 2c0a 2020 2020 2020 2020  $dt$:",.        
-00002c10: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
-00002c20: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00002c30: 2020 2276 616c 7565 223a 2036 302e 302c    "value": 60.0,
-00002c40: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00002c50: 7265 7175 6972 6564 223a 2074 7275 652c  required": true,
-00002c60: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00002c70: 6465 7363 7269 7074 696f 6e22 3a20 2252  description": "R
-00002c80: 6563 6f72 6420 6120 6461 7461 706f 696e  ecord a datapoin
-00002c90: 7420 6174 2070 7265 7363 7269 6265 6420  t at prescribed 
-00002ca0: 7469 6d65 2073 7061 6369 6e67 222c 0a20  time spacing",. 
-00002cb0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00002cc0: 6661 756c 745f 7661 6c75 6522 3a20 3330  fault_value": 30
-00002cd0: 2e30 0a20 2020 2020 2020 2020 2020 207d  .0.            }
-00002ce0: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-00002cf0: 696d 6974 5f63 7572 7265 6e74 5f6d 6178  imit_current_max
-00002d00: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00002d10: 2020 2022 6c61 6265 6c22 3a20 224d 6178     "label": "Max
-00002d20: 696d 756d 2063 7572 7265 6e74 3a22 2c0a  imum current:",.
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00002d40: 6e69 7473 223a 2022 4922 2c0a 2020 2020  nits": "I",.    
-00002d50: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-00002d60: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
-00002d70: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-00002d80: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
-00002d90: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00002da0: 7469 6f6e 223a 2022 4465 6669 6e65 2074  tion": "Define t
-00002db0: 6865 2075 7070 6572 206c 696d 6974 206f  he upper limit o
-00002dc0: 6620 6375 7272 656e 7420 666f 7220 7468  f current for th
-00002dd0: 6973 2073 7465 7022 2c0a 2020 2020 2020  is step",.      
-00002de0: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-00002df0: 5f76 616c 7565 223a 206e 756c 6c0a 2020  _value": null.  
-00002e00: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00002e10: 2020 2020 2020 2020 2022 6c69 6d69 745f           "limit_
-00002e20: 6375 7272 656e 745f 6d69 6e22 3a20 7b0a  current_min": {.
-00002e30: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00002e40: 6162 656c 223a 2022 4d69 6e69 6d75 6d20  abel": "Minimum 
-00002e50: 6375 7272 656e 743a 222c 0a20 2020 2020  current:",.     
-00002e60: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
-00002e70: 3a20 2249 222c 0a20 2020 2020 2020 2020  : "I",.         
-00002e80: 2020 2020 2022 7661 6c75 6522 3a20 6e75       "value": nu
-00002e90: 6c6c 2c0a 2020 2020 2020 2020 2020 2020  ll,.            
-00002ea0: 2020 2272 6571 7569 7265 6422 3a20 6661    "required": fa
-00002eb0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00002ec0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00002ed0: 3a20 2244 6566 696e 6520 7468 6520 6c6f  : "Define the lo
-00002ee0: 7765 7220 6c69 6d69 7420 6f66 2063 7572  wer limit of cur
-00002ef0: 7265 6e74 2066 6f72 2074 6869 7320 7374  rent for this st
-00002f00: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
-00002f10: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
-00002f20: 6522 3a20 6e75 6c6c 0a20 2020 2020 2020  e": null.       
-00002f30: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00002f40: 2020 2020 226c 696d 6974 5f76 6f6c 7461      "limit_volta
-00002f50: 6765 5f6d 6178 223a 207b 0a20 2020 2020  ge_max": {.     
-00002f60: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
-00002f70: 3a20 224d 6178 696d 756d 2076 6f6c 7461  : "Maximum volta
-00002f80: 6765 3a22 2c0a 2020 2020 2020 2020 2020  ge:",.          
-00002f90: 2020 2020 2275 6e69 7473 223a 2022 5622      "units": "V"
-00002fa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002fb0: 2276 616c 7565 223a 2032 2e35 2c0a 2020  "value": 2.5,.  
-00002fc0: 2020 2020 2020 2020 2020 2020 2272 6571              "req
-00002fd0: 7569 7265 6422 3a20 6661 6c73 652c 0a20  uired": false,. 
-00002fe0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00002ff0: 7363 7269 7074 696f 6e22 3a20 2244 6566  scription": "Def
-00003000: 696e 6520 7468 6520 7570 7065 7220 6c69  ine the upper li
-00003010: 6d69 7420 6f66 2076 6f6c 7461 6765 2066  mit of voltage f
-00003020: 6f72 2074 6869 7320 7374 6570 222c 0a20  or this step",. 
-00003030: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00003040: 6661 756c 745f 7661 6c75 6522 3a20 6e75  fault_value": nu
-00003050: 6c6c 0a20 2020 2020 2020 2020 2020 207d  ll.            }
-00003060: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-00003070: 696d 6974 5f76 6f6c 7461 6765 5f6d 696e  imit_voltage_min
-00003080: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00003090: 2020 2022 6c61 6265 6c22 3a20 224d 696e     "label": "Min
-000030a0: 696d 756d 2076 6f6c 7461 6765 3a22 2c0a  imum voltage:",.
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-000030c0: 6e69 7473 223a 2022 5622 2c0a 2020 2020  nits": "V",.    
-000030d0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-000030e0: 223a 2031 2e35 2c0a 2020 2020 2020 2020  ": 1.5,.        
-000030f0: 2020 2020 2020 2272 6571 7569 7265 6422        "required"
-00003100: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-00003110: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00003120: 696f 6e22 3a20 2244 6566 696e 6520 7468  ion": "Define th
-00003130: 6520 6c6f 7765 7220 6c69 6d69 7420 6f66  e lower limit of
-00003140: 2076 6f6c 7461 6765 2066 6f72 2074 6869   voltage for thi
-00003150: 7320 7374 6570 222c 0a20 2020 2020 2020  s step",.       
-00003160: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
-00003170: 7661 6c75 6522 3a20 6e75 6c6c 0a20 2020  value": null.   
-00003180: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00003190: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000031a0: 2020 2273 686f 7274 5f6e 616d 6522 3a20    "short_name": 
-000031b0: 2243 4322 2c0a 2020 2020 2020 2020 2020  "CC",.          
-000031c0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
-000031d0: 436f 6e74 726f 6c6c 6564 2063 7572 7265  Controlled curre
-000031e0: 6e74 2074 6563 686e 6971 7565 2c20 7769  nt technique, wi
-000031f0: 7468 206f 7074 696f 6e61 6c20 766f 6c74  th optional volt
-00003200: 6167 6520 616e 6420 6375 7272 656e 7420  age and current 
-00003210: 6c69 6d69 7473 220a 2020 2020 2020 2020  limits".        
-00003220: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
-00003230: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
-00003240: 4c4f 4f50 5f31 222c 0a20 2020 2020 2020  LOOP_1",.       
-00003250: 2020 2022 6465 7669 6365 223a 2022 4d50     "device": "MP
-00003260: 4732 222c 0a20 2020 2020 2020 2020 2022  G2",.          "
-00003270: 7465 6368 6e69 7175 6522 3a20 226c 6f6f  technique": "loo
-00003280: 7022 2c0a 2020 2020 2020 2020 2020 2270  p",.          "p
-00003290: 6172 616d 6574 6572 7322 3a20 7b0a 2020  arameters": {.  
-000032a0: 2020 2020 2020 2020 2020 2267 6f74 6f22            "goto"
-000032b0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000032c0: 2020 226c 6162 656c 223a 2022 476f 2074    "label": "Go t
-000032d0: 6f3a 222c 0a20 2020 2020 2020 2020 2020  o:",.           
-000032e0: 2020 2022 756e 6974 7322 3a20 2222 2c0a     "units": "",.
-000032f0: 2020 2020 2020 2020 2020 2020 2020 2276                "v
-00003300: 616c 7565 223a 2031 2c0a 2020 2020 2020  alue": 1,.      
-00003310: 2020 2020 2020 2020 2272 6571 7569 7265          "require
-00003320: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
-00003330: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00003340: 7469 6f6e 223a 2022 496e 6465 7820 6f66  tion": "Index of
-00003350: 2074 6865 2074 6563 686e 6971 7565 2074   the technique t
-00003360: 6f20 676f 2062 6163 6b20 746f 222c 0a20  o go back to",. 
-00003370: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00003380: 6661 756c 745f 7661 6c75 6522 3a20 310a  fault_value": 1.
-00003390: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-000033a0: 2020 2020 2020 2020 2020 2022 6e5f 676f             "n_go
-000033b0: 746f 7322 3a20 7b0a 2020 2020 2020 2020  tos": {.        
-000033c0: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
-000033d0: 5265 7065 6174 7322 2c0a 2020 2020 2020  Repeats",.      
-000033e0: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-000033f0: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
-00003400: 2020 2022 7661 6c75 6522 3a20 3130 302c     "value": 100,
-00003410: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00003420: 7265 7175 6972 6564 223a 2074 7275 652c  required": true,
-00003430: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00003440: 6465 7363 7269 7074 696f 6e22 3a20 224e  description": "N
-00003450: 756d 6265 7220 6f66 2074 696d 6573 2074  umber of times t
-00003460: 6865 2074 6563 686e 6971 7565 2077 696c  he technique wil
-00003470: 6c20 6a75 6d70 3b20 7365 7420 746f 202d  l jump; set to -
-00003480: 3120 666f 7220 756e 6c69 6d69 7465 6422  1 for unlimited"
-00003490: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000034a0: 2264 6566 6175 6c74 5f76 616c 7565 223a  "default_value":
-000034b0: 202d 310a 2020 2020 2020 2020 2020 2020   -1.            
-000034c0: 7d0a 2020 2020 2020 2020 2020 7d2c 0a20  }.          },. 
-000034d0: 2020 2020 2020 2020 2022 7368 6f72 745f           "short_
-000034e0: 6e61 6d65 223a 2022 4c4f 4f50 222c 0a20  name": "LOOP",. 
-000034f0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00003500: 7074 696f 6e22 3a20 224c 6f6f 7020 7465  ption": "Loop te
-00003510: 6368 6e69 7175 652c 2061 6c6c 6f77 696e  chnique, allowin
-00003520: 6720 746f 2072 6570 6561 7420 6120 7365  g to repeat a se
-00003530: 7420 6f66 2070 7265 6365 6469 6e67 2074  t of preceding t
-00003540: 6563 686e 6971 7565 7320 696e 2061 2074  echniques in a t
-00003550: 6563 686e 6971 7565 2061 7272 6179 220a  echnique array".
-00003560: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00003570: 5d0a 2020 2020 7d2c 0a20 2020 2022 4445  ].    },.    "DE
-00003580: 4641 554c 545f 5052 4f54 4543 5449 4f4e  FAULT_PROTECTION
-00003590: 5f4d 4554 484f 4422 3a20 7b0a 2020 2020  _METHOD": {.    
-000035a0: 2020 226d 6574 686f 6422 3a20 5b0a 2020    "method": [.  
-000035b0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000035c0: 2020 226e 616d 6522 3a20 2243 435f 3122    "name": "CC_1"
-000035d0: 2c0a 2020 2020 2020 2020 2020 2264 6576  ,.          "dev
-000035e0: 6963 6522 3a20 224d 5047 3222 2c0a 2020  ice": "MPG2",.  
-000035f0: 2020 2020 2020 2020 2274 6563 686e 6971          "techniq
-00003600: 7565 223a 2022 636f 6e73 7461 6e74 5f63  ue": "constant_c
-00003610: 7572 7265 6e74 222c 0a20 2020 2020 2020  urrent",.       
-00003620: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-00003630: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00003640: 7469 6d65 223a 207b 0a20 2020 2020 2020  time": {.       
-00003650: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
-00003660: 2254 696d 653a 222c 0a20 2020 2020 2020  "Time:",.       
-00003670: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
-00003680: 2273 222c 0a20 2020 2020 2020 2020 2020  "s",.           
-00003690: 2020 2022 7661 6c75 6522 3a20 3336 3030     "value": 3600
-000036a0: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
-000036b0: 2020 2272 6571 7569 7265 6422 3a20 7472    "required": tr
-000036c0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-000036d0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000036e0: 2022 4d61 7869 6d75 6d20 6475 7261 7469   "Maximum durati
-000036f0: 6f6e 206f 6620 7468 6520 4343 2073 7465  on of the CC ste
-00003700: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-00003710: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-00003720: 223a 2030 2e30 0a20 2020 2020 2020 2020  ": 0.0.         
-00003730: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00003740: 2020 2245 5f72 616e 6765 223a 207b 0a20    "E_range": {. 
-00003750: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-00003760: 6265 6c22 3a20 2245 2072 616e 6765 222c  bel": "E range",
-00003770: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00003780: 756e 6974 7322 3a20 2222 2c0a 2020 2020  units": "",.    
-00003790: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-000037a0: 223a 2022 2b2d 352e 3020 5622 2c0a 2020  ": "+-5.0 V",.  
-000037b0: 2020 2020 2020 2020 2020 2020 2272 6571              "req
-000037c0: 7569 7265 6422 3a20 7472 7565 2c0a 2020  uired": true,.  
-000037d0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-000037e0: 6372 6970 7469 6f6e 223a 2022 5365 6c65  cription": "Sele
-000037f0: 6374 2074 6865 2076 6f6c 7461 6765 2072  ct the voltage r
-00003800: 616e 6765 206f 6620 7468 6520 706f 7465  ange of the pote
-00003810: 6e74 696f 7374 6174 222c 0a20 2020 2020  ntiostat",.     
-00003820: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
-00003830: 745f 7661 6c75 6522 3a20 2261 7574 6f22  t_value": "auto"
-00003840: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00003850: 2020 2020 2020 2020 2020 2020 2249 5f72              "I_r
-00003860: 616e 6765 223a 207b 0a20 2020 2020 2020  ange": {.       
-00003870: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
-00003880: 2249 2072 616e 6765 222c 0a20 2020 2020  "I range",.     
-00003890: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
-000038a0: 3a20 2222 2c0a 2020 2020 2020 2020 2020  : "",.          
-000038b0: 2020 2020 2276 616c 7565 223a 2022 3130      "value": "10
-000038c0: 206d 4122 2c0a 2020 2020 2020 2020 2020   mA",.          
-000038d0: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
-000038e0: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
-000038f0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00003900: 223a 2022 5365 6c65 6374 2074 6865 2063  ": "Select the c
-00003910: 7572 7265 6e74 2072 616e 6765 206f 6620  urrent range of 
-00003920: 7468 6520 706f 7465 6e74 696f 7374 6174  the potentiostat
-00003930: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003940: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
-00003950: 3a20 226b 6565 7022 0a20 2020 2020 2020  : "keep".       
-00003960: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00003970: 2020 2020 2263 7572 7265 6e74 223a 207b      "current": {
-00003980: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00003990: 6c61 6265 6c22 3a20 2253 7465 7020 6375  label": "Step cu
-000039a0: 7272 656e 743a 222c 0a20 2020 2020 2020  rrent:",.       
-000039b0: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
-000039c0: 2249 222c 0a20 2020 2020 2020 2020 2020  "I",.           
-000039d0: 2020 2022 7661 6c75 6522 3a20 2243 2f33     "value": "C/3
-000039e0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000039f0: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
-00003a00: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00003a10: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00003a20: 2243 7572 7265 6e74 2064 7572 696e 6720  "Current during 
-00003a30: 7468 6520 6375 7272 656e 7420 7374 6570  the current step
-00003a40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003a50: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
-00003a60: 3a20 302e 300a 2020 2020 2020 2020 2020  : 0.0.          
-00003a70: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00003a80: 2022 6973 5f64 656c 7461 223a 207b 0a20   "is_delta": {. 
-00003a90: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-00003aa0: 6265 6c22 3a20 225c 7530 3339 3424 4924  bel": "\u0394$I$
-00003ab0: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
-00003ac0: 2020 2275 6e69 7473 223a 2022 222c 0a20    "units": "",. 
-00003ad0: 2020 2020 2020 2020 2020 2020 2022 7661               "va
-00003ae0: 6c75 6522 3a20 6661 6c73 652c 0a20 2020  lue": false,.   
-00003af0: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
-00003b00: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
-00003b10: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00003b20: 7269 7074 696f 6e22 3a20 2249 7320 7468  ription": "Is th
-00003b30: 6520 7374 6570 2063 7572 7265 6e74 2061  e step current a
-00003b40: 2024 5c5c 4465 6c74 6124 2066 726f 6d20   $\\Delta$ from 
-00003b50: 7072 6576 696f 7573 2073 7465 703f 222c  previous step?",
-00003b60: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00003b70: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
-00003b80: 6661 6c73 650a 2020 2020 2020 2020 2020  false.          
-00003b90: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00003ba0: 2022 6e5f 6379 636c 6573 223a 207b 0a20   "n_cycles": {. 
-00003bb0: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-00003bc0: 6265 6c22 3a20 224e 756d 6265 7220 6f66  bel": "Number of
-00003bd0: 2063 7963 6c65 733a 222c 0a20 2020 2020   cycles:",.     
-00003be0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
-00003bf0: 3a20 2222 2c0a 2020 2020 2020 2020 2020  : "",.          
-00003c00: 2020 2020 2276 616c 7565 223a 2030 2c0a      "value": 0,.
-00003c10: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00003c20: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
-00003c30: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00003c40: 6573 6372 6970 7469 6f6e 223a 2022 4379  escription": "Cy
-00003c50: 636c 6520 7468 726f 7567 6820 7468 6520  cle through the 
-00003c60: 6375 7272 656e 7420 7465 6368 6e69 7175  current techniqu
-00003c70: 6520 4e20 7469 6d65 732e 222c 0a20 2020  e N times.",.   
-00003c80: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
-00003c90: 756c 745f 7661 6c75 6522 3a20 300a 2020  ult_value": 0.  
-00003ca0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00003cb0: 2020 2020 2020 2020 2022 6578 6974 5f6f           "exit_o
-00003cc0: 6e5f 6c69 6d69 7422 3a20 7b0a 2020 2020  n_limit": {.    
-00003cd0: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-00003ce0: 223a 2022 4578 6974 2077 6865 6e20 6c69  ": "Exit when li
-00003cf0: 6d69 7473 2072 6561 6368 6564 3f22 2c0a  mits reached?",.
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00003d10: 6e69 7473 223a 2022 222c 0a20 2020 2020  nits": "",.     
-00003d20: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00003d30: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-00003d40: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-00003d50: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-00003d60: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00003d70: 696f 6e22 3a20 2253 746f 7020 7468 6520  ion": "Stop the 
-00003d80: 7768 6f6c 6520 6578 7065 7269 6d65 6e74  whole experiment
-00003d90: 2077 6865 6e20 6c69 6d69 7420 6973 2072   when limit is r
-00003da0: 6561 6368 6564 3f22 2c0a 2020 2020 2020  eached?",.      
-00003db0: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-00003dc0: 5f76 616c 7565 223a 2066 616c 7365 0a20  _value": false. 
-00003dd0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00003de0: 2020 2020 2020 2020 2020 2272 6563 6f72            "recor
-00003df0: 645f 6576 6572 795f 6445 223a 207b 0a20  d_every_dE": {. 
-00003e00: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-00003e10: 6265 6c22 3a20 2252 6563 6f72 6420 6576  bel": "Record ev
-00003e20: 6572 7920 2464 4524 3a22 2c0a 2020 2020  ery $dE$:",.    
-00003e30: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
-00003e40: 223a 2022 5622 2c0a 2020 2020 2020 2020  ": "V",.        
-00003e50: 2020 2020 2020 2276 616c 7565 223a 2030        "value": 0
-00003e60: 2e31 2c0a 2020 2020 2020 2020 2020 2020  .1,.            
-00003e70: 2020 2272 6571 7569 7265 6422 3a20 7472    "required": tr
-00003e80: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00003e90: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00003ea0: 2022 5265 636f 7264 2061 2064 6174 6170   "Record a datap
-00003eb0: 6f69 6e74 2061 7420 7072 6573 6372 6962  oint at prescrib
-00003ec0: 6564 2076 6f6c 7461 6765 2073 7061 6369  ed voltage spaci
-00003ed0: 6e67 222c 0a20 2020 2020 2020 2020 2020  ng",.           
-00003ee0: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
-00003ef0: 6522 3a20 302e 3030 350a 2020 2020 2020  e": 0.005.      
-00003f00: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00003f10: 2020 2020 2022 7265 636f 7264 5f65 7665       "record_eve
-00003f20: 7279 5f64 7422 3a20 7b0a 2020 2020 2020  ry_dt": {.      
-00003f30: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-00003f40: 2022 5265 636f 7264 2065 7665 7279 2024   "Record every $
-00003f50: 6474 243a 222c 0a20 2020 2020 2020 2020  dt$:",.         
-00003f60: 2020 2020 2022 756e 6974 7322 3a20 2273       "units": "s
-00003f70: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003f80: 2022 7661 6c75 6522 3a20 3330 2e30 2c0a   "value": 30.0,.
-00003f90: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00003fa0: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
-00003fb0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00003fc0: 6573 6372 6970 7469 6f6e 223a 2022 5265  escription": "Re
-00003fd0: 636f 7264 2061 2064 6174 6170 6f69 6e74  cord a datapoint
-00003fe0: 2061 7420 7072 6573 6372 6962 6564 2074   at prescribed t
-00003ff0: 696d 6520 7370 6163 696e 6722 2c0a 2020  ime spacing",.  
-00004000: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-00004010: 6175 6c74 5f76 616c 7565 223a 2033 302e  ault_value": 30.
-00004020: 300a 2020 2020 2020 2020 2020 2020 7d2c  0.            },
-00004030: 0a20 2020 2020 2020 2020 2020 2022 6c69  .            "li
-00004040: 6d69 745f 6375 7272 656e 745f 6d61 7822  mit_current_max"
-00004050: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00004060: 2020 226c 6162 656c 223a 2022 4d61 7869    "label": "Maxi
-00004070: 6d75 6d20 6375 7272 656e 743a 222c 0a20  mum current:",. 
-00004080: 2020 2020 2020 2020 2020 2020 2022 756e               "un
-00004090: 6974 7322 3a20 2249 222c 0a20 2020 2020  its": "I",.     
-000040a0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-000040b0: 3a20 6e75 6c6c 2c0a 2020 2020 2020 2020  : null,.        
-000040c0: 2020 2020 2020 2272 6571 7569 7265 6422        "required"
-000040d0: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-000040e0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-000040f0: 696f 6e22 3a20 2244 6566 696e 6520 7468  ion": "Define th
-00004100: 6520 7570 7065 7220 6c69 6d69 7420 6f66  e upper limit of
-00004110: 2063 7572 7265 6e74 2066 6f72 2074 6869   current for thi
-00004120: 7320 7374 6570 222c 0a20 2020 2020 2020  s step",.       
-00004130: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
-00004140: 7661 6c75 6522 3a20 6e75 6c6c 0a20 2020  value": null.   
-00004150: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00004160: 2020 2020 2020 2020 226c 696d 6974 5f63          "limit_c
-00004170: 7572 7265 6e74 5f6d 696e 223a 207b 0a20  urrent_min": {. 
-00004180: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-00004190: 6265 6c22 3a20 224d 696e 696d 756d 2063  bel": "Minimum c
-000041a0: 7572 7265 6e74 3a22 2c0a 2020 2020 2020  urrent:",.      
-000041b0: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-000041c0: 2022 4922 2c0a 2020 2020 2020 2020 2020   "I",.          
-000041d0: 2020 2020 2276 616c 7565 223a 206e 756c      "value": nul
-000041e0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-000041f0: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
-00004200: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00004210: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00004220: 2022 4465 6669 6e65 2074 6865 206c 6f77   "Define the low
-00004230: 6572 206c 696d 6974 206f 6620 6375 7272  er limit of curr
-00004240: 656e 7420 666f 7220 7468 6973 2073 7465  ent for this ste
-00004250: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-00004260: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-00004270: 223a 206e 756c 6c0a 2020 2020 2020 2020  ": null.        
-00004280: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00004290: 2020 2022 6c69 6d69 745f 766f 6c74 6167     "limit_voltag
-000042a0: 655f 6d61 7822 3a20 7b0a 2020 2020 2020  e_max": {.      
-000042b0: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-000042c0: 2022 4d61 7869 6d75 6d20 766f 6c74 6167   "Maximum voltag
-000042d0: 653a 222c 0a20 2020 2020 2020 2020 2020  e:",.           
-000042e0: 2020 2022 756e 6974 7322 3a20 2256 222c     "units": "V",
-000042f0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00004300: 7661 6c75 6522 3a20 312e 352c 0a20 2020  value": 1.5,.   
-00004310: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
-00004320: 6972 6564 223a 2066 616c 7365 2c0a 2020  ired": false,.  
-00004330: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00004340: 6372 6970 7469 6f6e 223a 2022 4465 6669  cription": "Defi
-00004350: 6e65 2074 6865 2075 7070 6572 206c 696d  ne the upper lim
-00004360: 6974 206f 6620 766f 6c74 6167 6520 666f  it of voltage fo
-00004370: 7220 7468 6973 2073 7465 7022 2c0a 2020  r this step",.  
-00004380: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-00004390: 6175 6c74 5f76 616c 7565 223a 206e 756c  ault_value": nul
-000043a0: 6c0a 2020 2020 2020 2020 2020 2020 7d2c  l.            },
-000043b0: 0a20 2020 2020 2020 2020 2020 2022 6c69  .            "li
-000043c0: 6d69 745f 766f 6c74 6167 655f 6d69 6e22  mit_voltage_min"
-000043d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000043e0: 2020 226c 6162 656c 223a 2022 4d69 6e69    "label": "Mini
-000043f0: 6d75 6d20 766f 6c74 6167 653a 222c 0a20  mum voltage:",. 
-00004400: 2020 2020 2020 2020 2020 2020 2022 756e               "un
-00004410: 6974 7322 3a20 2256 222c 0a20 2020 2020  its": "V",.     
-00004420: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00004430: 3a20 302e 302c 0a20 2020 2020 2020 2020  : 0.0,.         
-00004440: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
-00004450: 2066 616c 7365 2c0a 2020 2020 2020 2020   false,.        
-00004460: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00004470: 6f6e 223a 2022 4465 6669 6e65 2074 6865  on": "Define the
-00004480: 206c 6f77 6572 206c 696d 6974 206f 6620   lower limit of 
-00004490: 766f 6c74 6167 6520 666f 7220 7468 6973  voltage for this
-000044a0: 2073 7465 7022 2c0a 2020 2020 2020 2020   step",.        
-000044b0: 2020 2020 2020 2264 6566 6175 6c74 5f76        "default_v
-000044c0: 616c 7565 223a 206e 756c 6c0a 2020 2020  alue": null.    
-000044d0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000044e0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000044f0: 2022 7368 6f72 745f 6e61 6d65 223a 2022   "short_name": "
-00004500: 4343 222c 0a20 2020 2020 2020 2020 2022  CC",.          "
-00004510: 6465 7363 7269 7074 696f 6e22 3a20 2243  description": "C
-00004520: 6f6e 7472 6f6c 6c65 6420 6375 7272 656e  ontrolled curren
-00004530: 7420 7465 6368 6e69 7175 652c 2077 6974  t technique, wit
-00004540: 6820 6f70 7469 6f6e 616c 2076 6f6c 7461  h optional volta
-00004550: 6765 2061 6e64 2063 7572 7265 6e74 206c  ge and current l
-00004560: 696d 6974 7322 0a20 2020 2020 2020 207d  imits".        }
-00004570: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
-00004580: 2020 2020 2020 226e 616d 6522 3a20 2243        "name": "C
-00004590: 565f 3122 2c0a 2020 2020 2020 2020 2020  V_1",.          
-000045a0: 2264 6576 6963 6522 3a20 224d 5047 3222  "device": "MPG2"
-000045b0: 2c0a 2020 2020 2020 2020 2020 2274 6563  ,.          "tec
-000045c0: 686e 6971 7565 223a 2022 636f 6e73 7461  hnique": "consta
-000045d0: 6e74 5f76 6f6c 7461 6765 222c 0a20 2020  nt_voltage",.   
-000045e0: 2020 2020 2020 2022 7061 7261 6d65 7465         "paramete
-000045f0: 7273 223a 207b 0a20 2020 2020 2020 2020  rs": {.         
-00004600: 2020 2022 7469 6d65 223a 207b 0a20 2020     "time": {.   
-00004610: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
-00004620: 6c22 3a20 2254 696d 653a 222c 0a20 2020  l": "Time:",.   
-00004630: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
-00004640: 7322 3a20 2273 222c 0a20 2020 2020 2020  s": "s",.       
-00004650: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00004660: 3930 302e 302c 0a20 2020 2020 2020 2020  900.0,.         
-00004670: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
-00004680: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
-00004690: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-000046a0: 6e22 3a20 224d 6178 696d 756d 2064 7572  n": "Maximum dur
-000046b0: 6174 696f 6e20 6f66 2074 6865 2043 5620  ation of the CV 
-000046c0: 7374 6570 222c 0a20 2020 2020 2020 2020  step",.         
-000046d0: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
-000046e0: 6c75 6522 3a20 302e 300a 2020 2020 2020  lue": 0.0.      
-000046f0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00004700: 2020 2020 2022 455f 7261 6e67 6522 3a20       "E_range": 
-00004710: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00004720: 226c 6162 656c 223a 2022 4520 7261 6e67  "label": "E rang
-00004730: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00004740: 2020 2275 6e69 7473 223a 2022 222c 0a20    "units": "",. 
-00004750: 2020 2020 2020 2020 2020 2020 2022 7661               "va
-00004760: 6c75 6522 3a20 222b 2d35 2e30 2056 222c  lue": "+-5.0 V",
-00004770: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00004780: 7265 7175 6972 6564 223a 2074 7275 652c  required": true,
-00004790: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000047a0: 6465 7363 7269 7074 696f 6e22 3a20 2253  description": "S
-000047b0: 656c 6563 7420 7468 6520 766f 6c74 6167  elect the voltag
-000047c0: 6520 7261 6e67 6520 6f66 2074 6865 2070  e range of the p
-000047d0: 6f74 656e 7469 6f73 7461 7422 2c0a 2020  otentiostat",.  
-000047e0: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-000047f0: 6175 6c74 5f76 616c 7565 223a 2022 6175  ault_value": "au
-00004800: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
-00004810: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00004820: 495f 7261 6e67 6522 3a20 7b0a 2020 2020  I_range": {.    
-00004830: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-00004840: 223a 2022 4920 7261 6e67 6522 2c0a 2020  ": "I range",.  
-00004850: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
-00004860: 7473 223a 2022 222c 0a20 2020 2020 2020  ts": "",.       
-00004870: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00004880: 2231 3020 6d41 222c 0a20 2020 2020 2020  "10 mA",.       
-00004890: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-000048a0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-000048b0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-000048c0: 696f 6e22 3a20 2253 656c 6563 7420 7468  ion": "Select th
-000048d0: 6520 6375 7272 656e 7420 7261 6e67 6520  e current range 
-000048e0: 6f66 2074 6865 2070 6f74 656e 7469 6f73  of the potentios
-000048f0: 7461 7422 2c0a 2020 2020 2020 2020 2020  tat",.          
-00004900: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
-00004910: 7565 223a 2022 6b65 6570 220a 2020 2020  ue": "keep".    
-00004920: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00004930: 2020 2020 2020 2022 766f 6c74 6167 6522         "voltage"
-00004940: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00004950: 2020 226c 6162 656c 223a 2022 5374 6570    "label": "Step
-00004960: 2076 6f6c 7461 6765 3a22 2c0a 2020 2020   voltage:",.    
-00004970: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
-00004980: 223a 2022 5622 2c0a 2020 2020 2020 2020  ": "V",.        
-00004990: 2020 2020 2020 2276 616c 7565 223a 2031        "value": 1
-000049a0: 2e35 2c0a 2020 2020 2020 2020 2020 2020  .5,.            
-000049b0: 2020 2272 6571 7569 7265 6422 3a20 7472    "required": tr
-000049c0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-000049d0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000049e0: 2022 566f 6c74 6167 6520 6f66 2074 6865   "Voltage of the
-000049f0: 2063 7572 7265 6e74 2073 7465 7022 2c0a   current step",.
-00004a00: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00004a10: 6566 6175 6c74 5f76 616c 7565 223a 2030  efault_value": 0
-00004a20: 2e30 0a20 2020 2020 2020 2020 2020 207d  .0.            }
-00004a30: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
-00004a40: 735f 6465 6c74 6122 3a20 7b0a 2020 2020  s_delta": {.    
-00004a50: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-00004a60: 223a 2022 5c75 3033 3934 2456 243a 222c  ": "\u0394$V$:",
-00004a70: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00004a80: 756e 6974 7322 3a20 2222 2c0a 2020 2020  units": "",.    
-00004a90: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-00004aa0: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
-00004ab0: 2020 2020 2020 2020 2272 6571 7569 7265          "require
-00004ac0: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
-00004ad0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00004ae0: 7469 6f6e 223a 2022 4973 2074 6865 2073  tion": "Is the s
-00004af0: 7465 7020 766f 6c74 6167 6520 6120 245c  tep voltage a $\
-00004b00: 5c44 656c 7461 2420 6672 6f6d 2070 7265  \Delta$ from pre
-00004b10: 7669 6f75 7320 7374 6570 3f22 2c0a 2020  vious step?",.  
-00004b20: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-00004b30: 6175 6c74 5f76 616c 7565 223a 2066 616c  ault_value": fal
-00004b40: 7365 0a20 2020 2020 2020 2020 2020 207d  se.            }
-00004b50: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
-00004b60: 5f63 7963 6c65 7322 3a20 7b0a 2020 2020  _cycles": {.    
-00004b70: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-00004b80: 223a 2022 4e75 6d62 6572 206f 6620 6379  ": "Number of cy
-00004b90: 636c 6573 3a22 2c0a 2020 2020 2020 2020  cles:",.        
-00004ba0: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
-00004bb0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00004bc0: 2022 7661 6c75 6522 3a20 302c 0a20 2020   "value": 0,.   
-00004bd0: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
-00004be0: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
-00004bf0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00004c00: 7269 7074 696f 6e22 3a20 2243 7963 6c65  ription": "Cycle
-00004c10: 2074 6872 6f75 6768 2074 6865 2063 7572   through the cur
-00004c20: 7265 6e74 2074 6563 686e 6971 7565 204e  rent technique N
-00004c30: 2074 696d 6573 2e22 2c0a 2020 2020 2020   times.",.      
-00004c40: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-00004c50: 5f76 616c 7565 223a 2030 0a20 2020 2020  _value": 0.     
-00004c60: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00004c70: 2020 2020 2020 2265 7869 745f 6f6e 5f6c        "exit_on_l
-00004c80: 696d 6974 223a 207b 0a20 2020 2020 2020  imit": {.       
-00004c90: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
-00004ca0: 2245 7869 7420 7768 656e 206c 696d 6974  "Exit when limit
-00004cb0: 7320 7265 6163 6865 643f 222c 0a20 2020  s reached?",.   
-00004cc0: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
-00004cd0: 7322 3a20 2222 2c0a 2020 2020 2020 2020  s": "",.        
-00004ce0: 2020 2020 2020 2276 616c 7565 223a 2066        "value": f
-00004cf0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00004d00: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
-00004d10: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
-00004d20: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00004d30: 223a 2022 5374 6f70 2074 6865 2077 686f  ": "Stop the who
-00004d40: 6c65 2065 7870 6572 696d 656e 7420 7768  le experiment wh
-00004d50: 656e 206c 696d 6974 2069 7320 7265 6163  en limit is reac
-00004d60: 6865 643f 222c 0a20 2020 2020 2020 2020  hed?",.         
-00004d70: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
-00004d80: 6c75 6522 3a20 6661 6c73 650a 2020 2020  lue": false.    
-00004d90: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00004da0: 2020 2020 2020 2022 7265 636f 7264 5f65         "record_e
-00004db0: 7665 7279 5f64 4922 3a20 7b0a 2020 2020  very_dI": {.    
-00004dc0: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-00004dd0: 223a 2022 5265 636f 7264 2065 7665 7279  ": "Record every
-00004de0: 2024 6449 243a 222c 0a20 2020 2020 2020   $dI$:",.       
-00004df0: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
-00004e00: 2249 222c 0a20 2020 2020 2020 2020 2020  "I",.           
-00004e10: 2020 2022 7661 6c75 6522 3a20 302e 312c     "value": 0.1,
-00004e20: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00004e30: 7265 7175 6972 6564 223a 2074 7275 652c  required": true,
-00004e40: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00004e50: 6465 7363 7269 7074 696f 6e22 3a20 2252  description": "R
-00004e60: 6563 6f72 6420 6120 6461 7461 706f 696e  ecord a datapoin
-00004e70: 7420 6174 2070 7265 7363 7269 6265 6420  t at prescribed 
-00004e80: 6375 7272 656e 7420 7370 6163 696e 6722  current spacing"
-00004e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00004ea0: 2264 6566 6175 6c74 5f76 616c 7565 223a  "default_value":
-00004eb0: 2030 2e30 3031 0a20 2020 2020 2020 2020   0.001.         
-00004ec0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00004ed0: 2020 2272 6563 6f72 645f 6576 6572 795f    "record_every_
-00004ee0: 6474 223a 207b 0a20 2020 2020 2020 2020  dt": {.         
-00004ef0: 2020 2020 2022 6c61 6265 6c22 3a20 2252       "label": "R
-00004f00: 6563 6f72 6420 6576 6572 7920 2464 7424  ecord every $dt$
-00004f10: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
-00004f20: 2020 2275 6e69 7473 223a 2022 7322 2c0a    "units": "s",.
-00004f30: 2020 2020 2020 2020 2020 2020 2020 2276                "v
-00004f40: 616c 7565 223a 2033 302e 302c 0a20 2020  alue": 30.0,.   
-00004f50: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
-00004f60: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
-00004f70: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00004f80: 7269 7074 696f 6e22 3a20 2252 6563 6f72  ription": "Recor
-00004f90: 6420 6120 6461 7461 706f 696e 7420 6174  d a datapoint at
-00004fa0: 2070 7265 7363 7269 6265 6420 7469 6d65   prescribed time
-00004fb0: 2073 7061 6369 6e67 222c 0a20 2020 2020   spacing",.     
-00004fc0: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
-00004fd0: 745f 7661 6c75 6522 3a20 3330 2e30 0a20  t_value": 30.0. 
-00004fe0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00004ff0: 2020 2020 2020 2020 2020 226c 696d 6974            "limit
-00005000: 5f63 7572 7265 6e74 5f6d 6178 223a 207b  _current_max": {
-00005010: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00005020: 6c61 6265 6c22 3a20 224d 6178 696d 756d  label": "Maximum
-00005030: 2063 7572 7265 6e74 3a22 2c0a 2020 2020   current:",.    
-00005040: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
-00005050: 223a 2022 4922 2c0a 2020 2020 2020 2020  ": "I",.        
-00005060: 2020 2020 2020 2276 616c 7565 223a 206e        "value": n
-00005070: 756c 6c2c 0a20 2020 2020 2020 2020 2020  ull,.           
-00005080: 2020 2022 7265 7175 6972 6564 223a 2066     "required": f
-00005090: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-000050a0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-000050b0: 223a 2022 4465 6669 6e65 2074 6865 2075  ": "Define the u
-000050c0: 7070 6572 206c 696d 6974 206f 6620 6375  pper limit of cu
-000050d0: 7272 656e 7420 666f 7220 7468 6973 2073  rrent for this s
-000050e0: 7465 7022 2c0a 2020 2020 2020 2020 2020  tep",.          
-000050f0: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
-00005100: 7565 223a 206e 756c 6c0a 2020 2020 2020  ue": null.      
-00005110: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00005120: 2020 2020 2022 6c69 6d69 745f 6375 7272       "limit_curr
-00005130: 656e 745f 6d69 6e22 3a20 7b0a 2020 2020  ent_min": {.    
-00005140: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-00005150: 223a 2022 4d69 6e69 6d75 6d20 6375 7272  ": "Minimum curr
-00005160: 656e 743a 222c 0a20 2020 2020 2020 2020  ent:",.         
-00005170: 2020 2020 2022 756e 6974 7322 3a20 2249       "units": "I
-00005180: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005190: 2022 7661 6c75 6522 3a20 6e75 6c6c 2c0a   "value": null,.
-000051a0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-000051b0: 6571 7569 7265 6422 3a20 6661 6c73 652c  equired": false,
-000051c0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000051d0: 6465 7363 7269 7074 696f 6e22 3a20 2244  description": "D
-000051e0: 6566 696e 6520 7468 6520 6c6f 7765 7220  efine the lower 
-000051f0: 6c69 6d69 7420 6f66 2063 7572 7265 6e74  limit of current
-00005200: 2066 6f72 2074 6869 7320 7374 6570 222c   for this step",
-00005210: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00005220: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
-00005230: 6e75 6c6c 0a20 2020 2020 2020 2020 2020  null.           
-00005240: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00005250: 226c 696d 6974 5f76 6f6c 7461 6765 5f6d  "limit_voltage_m
-00005260: 6178 223a 207b 0a20 2020 2020 2020 2020  ax": {.         
-00005270: 2020 2020 2022 6c61 6265 6c22 3a20 224d       "label": "M
-00005280: 6178 696d 756d 2076 6f6c 7461 6765 3a22  aximum voltage:"
-00005290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000052a0: 2275 6e69 7473 223a 2022 5622 2c0a 2020  "units": "V",.  
-000052b0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-000052c0: 7565 223a 2031 2e35 2c0a 2020 2020 2020  ue": 1.5,.      
-000052d0: 2020 2020 2020 2020 2272 6571 7569 7265          "require
-000052e0: 6422 3a20 6661 6c73 652c 0a20 2020 2020  d": false,.     
-000052f0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00005300: 7074 696f 6e22 3a20 2244 6566 696e 6520  ption": "Define 
-00005310: 7468 6520 7570 7065 7220 6c69 6d69 7420  the upper limit 
-00005320: 6f66 2076 6f6c 7461 6765 2066 6f72 2074  of voltage for t
-00005330: 6869 7320 7374 6570 222c 0a20 2020 2020  his step",.     
-00005340: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
-00005350: 745f 7661 6c75 6522 3a20 6e75 6c6c 0a20  t_value": null. 
-00005360: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00005370: 2020 2020 2020 2020 2020 226c 696d 6974            "limit
-00005380: 5f76 6f6c 7461 6765 5f6d 696e 223a 207b  _voltage_min": {
-00005390: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000053a0: 6c61 6265 6c22 3a20 224d 696e 696d 756d  label": "Minimum
-000053b0: 2076 6f6c 7461 6765 3a22 2c0a 2020 2020   voltage:",.    
-000053c0: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
-000053d0: 223a 2022 5622 2c0a 2020 2020 2020 2020  ": "V",.        
-000053e0: 2020 2020 2020 2276 616c 7565 223a 2030        "value": 0
-000053f0: 2e30 2c0a 2020 2020 2020 2020 2020 2020  .0,.            
-00005400: 2020 2272 6571 7569 7265 6422 3a20 6661    "required": fa
-00005410: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00005420: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00005430: 3a20 2244 6566 696e 6520 7468 6520 6c6f  : "Define the lo
-00005440: 7765 7220 6c69 6d69 7420 6f66 2076 6f6c  wer limit of vol
-00005450: 7461 6765 2066 6f72 2074 6869 7320 7374  tage for this st
-00005460: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
-00005470: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
-00005480: 6522 3a20 6e75 6c6c 0a20 2020 2020 2020  e": null.       
-00005490: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-000054a0: 207d 2c0a 2020 2020 2020 2020 2020 2273   },.          "s
-000054b0: 686f 7274 5f6e 616d 6522 3a20 2243 5622  hort_name": "CV"
-000054c0: 2c0a 2020 2020 2020 2020 2020 2264 6573  ,.          "des
-000054d0: 6372 6970 7469 6f6e 223a 2022 436f 6e74  cription": "Cont
-000054e0: 726f 6c6c 6564 2076 6f6c 7461 6765 2074  rolled voltage t
-000054f0: 6563 686e 6971 7565 2c20 7769 7468 206f  echnique, with o
-00005500: 7074 696f 6e61 6c20 6375 7272 656e 7420  ptional current 
-00005510: 616e 6420 766f 6c74 6167 6520 6c69 6d69  and voltage limi
-00005520: 7473 220a 2020 2020 2020 2020 7d2c 0a20  ts".        },. 
-00005530: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00005540: 2020 2022 6e61 6d65 223a 2022 4f43 565f     "name": "OCV_
-00005550: 3122 2c0a 2020 2020 2020 2020 2020 2264  1",.          "d
-00005560: 6576 6963 6522 3a20 224d 5047 3222 2c0a  evice": "MPG2",.
-00005570: 2020 2020 2020 2020 2020 2274 6563 686e            "techn
-00005580: 6971 7565 223a 2022 6f70 656e 5f63 6972  ique": "open_cir
-00005590: 6375 6974 5f76 6f6c 7461 6765 222c 0a20  cuit_voltage",. 
-000055a0: 2020 2020 2020 2020 2022 7061 7261 6d65           "parame
-000055b0: 7465 7273 223a 207b 0a20 2020 2020 2020  ters": {.       
-000055c0: 2020 2020 2022 7469 6d65 223a 207b 0a20       "time": {. 
-000055d0: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-000055e0: 6265 6c22 3a20 2254 696d 653a 222c 0a20  bel": "Time:",. 
-000055f0: 2020 2020 2020 2020 2020 2020 2022 756e               "un
-00005600: 6974 7322 3a20 2273 222c 0a20 2020 2020  its": "s",.     
-00005610: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00005620: 3a20 3231 3630 302e 302c 0a20 2020 2020  : 21600.0,.     
-00005630: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
-00005640: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
-00005650: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00005660: 7074 696f 6e22 3a20 2254 6865 206c 656e  ption": "The len
-00005670: 6774 6820 6f66 2074 6865 204f 4356 2073  gth of the OCV s
-00005680: 7465 7022 2c0a 2020 2020 2020 2020 2020  tep",.          
-00005690: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
-000056a0: 7565 223a 2030 2e30 0a20 2020 2020 2020  ue": 0.0.       
-000056b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-000056c0: 2020 2020 2245 5f72 616e 6765 223a 207b      "E_range": {
-000056d0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000056e0: 6c61 6265 6c22 3a20 2245 2072 616e 6765  label": "E range
-000056f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005700: 2022 756e 6974 7322 3a20 2222 2c0a 2020   "units": "",.  
-00005710: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00005720: 7565 223a 2022 2b2d 352e 3020 5622 2c0a  ue": "+-5.0 V",.
-00005730: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00005740: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
-00005750: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00005760: 6573 6372 6970 7469 6f6e 223a 2022 222c  escription": "",
-00005770: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00005780: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
-00005790: 2261 7574 6f22 0a20 2020 2020 2020 2020  "auto".         
-000057a0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-000057b0: 2020 2249 5f72 616e 6765 223a 207b 0a20    "I_range": {. 
-000057c0: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-000057d0: 6265 6c22 3a20 2249 2072 616e 6765 222c  bel": "I range",
-000057e0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000057f0: 756e 6974 7322 3a20 2222 2c0a 2020 2020  units": "",.    
-00005800: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-00005810: 223a 2022 3130 206d 4122 2c0a 2020 2020  ": "10 mA",.    
-00005820: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
-00005830: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
-00005840: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
-00005850: 6970 7469 6f6e 223a 2022 222c 0a20 2020  iption": "",.   
-00005860: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
-00005870: 756c 745f 7661 6c75 6522 3a20 2231 2041  ult_value": "1 A
-00005880: 220a 2020 2020 2020 2020 2020 2020 7d2c  ".            },
-00005890: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
-000058a0: 636f 7264 5f65 7665 7279 5f64 4522 3a20  cord_every_dE": 
-000058b0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000058c0: 226c 6162 656c 223a 2022 5265 636f 7264  "label": "Record
-000058d0: 2065 7665 7279 2024 6445 243a 222c 0a20   every $dE$:",. 
-000058e0: 2020 2020 2020 2020 2020 2020 2022 756e               "un
-000058f0: 6974 7322 3a20 2256 222c 0a20 2020 2020  its": "V",.     
-00005900: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00005910: 3a20 302e 312c 0a20 2020 2020 2020 2020  : 0.1,.         
-00005920: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
-00005930: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
-00005940: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00005950: 6e22 3a20 2252 6563 6f72 6420 6120 6461  n": "Record a da
-00005960: 7461 706f 696e 7420 6174 2070 7265 7363  tapoint at presc
-00005970: 7269 6265 6420 766f 6c74 6167 6520 7370  ribed voltage sp
-00005980: 6163 696e 6722 2c0a 2020 2020 2020 2020  acing",.        
-00005990: 2020 2020 2020 2264 6566 6175 6c74 5f76        "default_v
-000059a0: 616c 7565 223a 2030 2e30 3035 0a20 2020  alue": 0.005.   
-000059b0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000059c0: 2020 2020 2020 2020 2272 6563 6f72 645f          "record_
-000059d0: 6576 6572 795f 6474 223a 207b 0a20 2020  every_dt": {.   
-000059e0: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
-000059f0: 6c22 3a20 2252 6563 6f72 6420 6576 6572  l": "Record ever
-00005a00: 7920 2464 7424 3a22 2c0a 2020 2020 2020  y $dt$:",.      
-00005a10: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-00005a20: 2022 7322 2c0a 2020 2020 2020 2020 2020   "s",.          
-00005a30: 2020 2020 2276 616c 7565 223a 2033 302e      "value": 30.
-00005a40: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00005a50: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
-00005a60: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00005a70: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00005a80: 2252 6563 6f72 6420 6120 6461 7461 706f  "Record a datapo
-00005a90: 696e 7420 6174 2070 7265 7363 7269 6265  int at prescribe
-00005aa0: 6420 7469 6d65 2073 7061 6369 6e67 222c  d time spacing",
-00005ab0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00005ac0: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
-00005ad0: 3330 2e30 0a20 2020 2020 2020 2020 2020  30.0.           
-00005ae0: 207d 0a20 2020 2020 2020 2020 207d 2c0a   }.          },.
-00005af0: 2020 2020 2020 2020 2020 2273 686f 7274            "short
-00005b00: 5f6e 616d 6522 3a20 224f 4356 222c 0a20  _name": "OCV",. 
-00005b10: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00005b20: 7074 696f 6e22 3a20 224f 7065 6e20 6369  ption": "Open ci
-00005b30: 7263 7569 7420 766f 6c74 6167 6522 0a20  rcuit voltage". 
-00005b40: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
-00005b50: 0a20 2020 207d 2c0a 2020 2020 2244 4546  .    },.    "DEF
-00005b60: 4155 4c54 5f46 4f52 4d41 5449 4f4e 5f4d  AULT_FORMATION_M
-00005b70: 4554 484f 4422 3a20 7b0a 2020 2020 2020  ETHOD": {.      
-00005b80: 226d 6574 686f 6422 3a20 5b0a 2020 2020  "method": [.    
-00005b90: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00005ba0: 226e 616d 6522 3a20 2243 435f 3122 2c0a  "name": "CC_1",.
-00005bb0: 2020 2020 2020 2020 2020 2264 6576 6963            "devic
-00005bc0: 6522 3a20 224d 5047 3222 2c0a 2020 2020  e": "MPG2",.    
-00005bd0: 2020 2020 2020 2274 6563 686e 6971 7565        "technique
-00005be0: 223a 2022 636f 6e73 7461 6e74 5f63 7572  ": "constant_cur
-00005bf0: 7265 6e74 222c 0a20 2020 2020 2020 2020  rent",.         
-00005c00: 2022 7061 7261 6d65 7465 7273 223a 207b   "parameters": {
-00005c10: 0a20 2020 2020 2020 2020 2020 2022 7469  .            "ti
-00005c20: 6d65 223a 207b 0a20 2020 2020 2020 2020  me": {.         
-00005c30: 2020 2020 2022 6c61 6265 6c22 3a20 2254       "label": "T
-00005c40: 696d 653a 222c 0a20 2020 2020 2020 2020  ime:",.         
-00005c50: 2020 2020 2022 756e 6974 7322 3a20 2273       "units": "s
-00005c60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005c70: 2022 7661 6c75 6522 3a20 3336 3030 302e   "value": 36000.
-00005c80: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00005c90: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
-00005ca0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00005cb0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00005cc0: 224d 6178 696d 756d 2064 7572 6174 696f  "Maximum duratio
-00005cd0: 6e20 6f66 2074 6865 2043 4320 7374 6570  n of the CC step
-00005ce0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005cf0: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
-00005d00: 3a20 302e 300a 2020 2020 2020 2020 2020  : 0.0.          
-00005d10: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00005d20: 2022 455f 7261 6e67 6522 3a20 7b0a 2020   "E_range": {.  
-00005d30: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
-00005d40: 656c 223a 2022 4520 7261 6e67 6522 2c0a  el": "E range",.
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00005d60: 6e69 7473 223a 2022 222c 0a20 2020 2020  nits": "",.     
-00005d70: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00005d80: 3a20 222b 2d35 2e30 2056 222c 0a20 2020  : "+-5.0 V",.   
-00005d90: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
-00005da0: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
-00005db0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00005dc0: 7269 7074 696f 6e22 3a20 2253 656c 6563  ription": "Selec
-00005dd0: 7420 7468 6520 766f 6c74 6167 6520 7261  t the voltage ra
-00005de0: 6e67 6520 6f66 2074 6865 2070 6f74 656e  nge of the poten
-00005df0: 7469 6f73 7461 7422 2c0a 2020 2020 2020  tiostat",.      
-00005e00: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-00005e10: 5f76 616c 7565 223a 2022 6175 746f 220a  _value": "auto".
-00005e20: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00005e30: 2020 2020 2020 2020 2020 2022 495f 7261             "I_ra
-00005e40: 6e67 6522 3a20 7b0a 2020 2020 2020 2020  nge": {.        
-00005e50: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
-00005e60: 4920 7261 6e67 6522 2c0a 2020 2020 2020  I range",.      
-00005e70: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-00005e80: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
-00005e90: 2020 2022 7661 6c75 6522 3a20 2231 3020     "value": "10 
-00005ea0: 6d41 222c 0a20 2020 2020 2020 2020 2020  mA",.           
-00005eb0: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
-00005ec0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00005ed0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00005ee0: 3a20 2253 656c 6563 7420 7468 6520 6375  : "Select the cu
-00005ef0: 7272 656e 7420 7261 6e67 6520 6f66 2074  rrent range of t
-00005f00: 6865 2070 6f74 656e 7469 6f73 7461 7422  he potentiostat"
-00005f10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005f20: 2264 6566 6175 6c74 5f76 616c 7565 223a  "default_value":
-00005f30: 2022 6b65 6570 220a 2020 2020 2020 2020   "keep".        
-00005f40: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00005f50: 2020 2022 6375 7272 656e 7422 3a20 7b0a     "current": {.
-00005f60: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00005f70: 6162 656c 223a 2022 5374 6570 2063 7572  abel": "Step cur
-00005f80: 7265 6e74 3a22 2c0a 2020 2020 2020 2020  rent:",.        
-00005f90: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
-00005fa0: 4922 2c0a 2020 2020 2020 2020 2020 2020  I",.            
-00005fb0: 2020 2276 616c 7565 223a 2022 432f 3130    "value": "C/10
-00005fc0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005fd0: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
-00005fe0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00005ff0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00006000: 2243 7572 7265 6e74 2064 7572 696e 6720  "Current during 
-00006010: 7468 6520 6375 7272 656e 7420 7374 6570  the current step
-00006020: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00006030: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
-00006040: 3a20 302e 300a 2020 2020 2020 2020 2020  : 0.0.          
-00006050: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00006060: 2022 6973 5f64 656c 7461 223a 207b 0a20   "is_delta": {. 
-00006070: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-00006080: 6265 6c22 3a20 225c 7530 3339 3424 4924  bel": "\u0394$I$
-00006090: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
-000060a0: 2020 2275 6e69 7473 223a 2022 222c 0a20    "units": "",. 
-000060b0: 2020 2020 2020 2020 2020 2020 2022 7661               "va
-000060c0: 6c75 6522 3a20 6661 6c73 652c 0a20 2020  lue": false,.   
-000060d0: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
-000060e0: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
-000060f0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
-00006100: 7269 7074 696f 6e22 3a20 2249 7320 7468  ription": "Is th
-00006110: 6520 7374 6570 2063 7572 7265 6e74 2061  e step current a
-00006120: 2024 5c5c 4465 6c74 6124 2066 726f 6d20   $\\Delta$ from 
-00006130: 7072 6576 696f 7573 2073 7465 703f 222c  previous step?",
-00006140: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00006150: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
-00006160: 6661 6c73 650a 2020 2020 2020 2020 2020  false.          
-00006170: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00006180: 2022 6e5f 6379 636c 6573 223a 207b 0a20   "n_cycles": {. 
-00006190: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-000061a0: 6265 6c22 3a20 224e 756d 6265 7220 6f66  bel": "Number of
-000061b0: 2063 7963 6c65 733a 222c 0a20 2020 2020   cycles:",.     
-000061c0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
-000061d0: 3a20 2222 2c0a 2020 2020 2020 2020 2020  : "",.          
-000061e0: 2020 2020 2276 616c 7565 223a 2030 2c0a      "value": 0,.
-000061f0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00006200: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
-00006210: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00006220: 6573 6372 6970 7469 6f6e 223a 2022 4379  escription": "Cy
-00006230: 636c 6520 7468 726f 7567 6820 7468 6520  cle through the 
-00006240: 6375 7272 656e 7420 7465 6368 6e69 7175  current techniqu
-00006250: 6520 4e20 7469 6d65 732e 222c 0a20 2020  e N times.",.   
-00006260: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
-00006270: 756c 745f 7661 6c75 6522 3a20 300a 2020  ult_value": 0.  
-00006280: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00006290: 2020 2020 2020 2020 2022 6578 6974 5f6f           "exit_o
-000062a0: 6e5f 6c69 6d69 7422 3a20 7b0a 2020 2020  n_limit": {.    
-000062b0: 2020 2020 2020 2020 2020 226c 6162 656c            "label
-000062c0: 223a 2022 4578 6974 2077 6865 6e20 6c69  ": "Exit when li
-000062d0: 6d69 7473 2072 6561 6368 6564 3f22 2c0a  mits reached?",.
-000062e0: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-000062f0: 6e69 7473 223a 2022 222c 0a20 2020 2020  nits": "",.     
-00006300: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00006310: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-00006320: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-00006330: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-00006340: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00006350: 696f 6e22 3a20 2253 746f 7020 7468 6520  ion": "Stop the 
-00006360: 7768 6f6c 6520 6578 7065 7269 6d65 6e74  whole experiment
-00006370: 2077 6865 6e20 6c69 6d69 7420 6973 2072   when limit is r
-00006380: 6561 6368 6564 3f22 2c0a 2020 2020 2020  eached?",.      
-00006390: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-000063a0: 5f76 616c 7565 223a 2066 616c 7365 0a20  _value": false. 
-000063b0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-000063c0: 2020 2020 2020 2020 2020 2272 6563 6f72            "recor
-000063d0: 645f 6576 6572 795f 6445 223a 207b 0a20  d_every_dE": {. 
-000063e0: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-000063f0: 6265 6c22 3a20 2252 6563 6f72 6420 6576  bel": "Record ev
-00006400: 6572 7920 2464 4524 3a22 2c0a 2020 2020  ery $dE$:",.    
-00006410: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
-00006420: 223a 2022 5622 2c0a 2020 2020 2020 2020  ": "V",.        
-00006430: 2020 2020 2020 2276 616c 7565 223a 2030        "value": 0
-00006440: 2e31 2c0a 2020 2020 2020 2020 2020 2020  .1,.            
-00006450: 2020 2272 6571 7569 7265 6422 3a20 7472    "required": tr
-00006460: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00006470: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00006480: 2022 5265 636f 7264 2061 2064 6174 6170   "Record a datap
-00006490: 6f69 6e74 2061 7420 7072 6573 6372 6962  oint at prescrib
-000064a0: 6564 2076 6f6c 7461 6765 2073 7061 6369  ed voltage spaci
-000064b0: 6e67 222c 0a20 2020 2020 2020 2020 2020  ng",.           
-000064c0: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
-000064d0: 6522 3a20 302e 3030 350a 2020 2020 2020  e": 0.005.      
-000064e0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000064f0: 2020 2020 2022 7265 636f 7264 5f65 7665       "record_eve
-00006500: 7279 5f64 7422 3a20 7b0a 2020 2020 2020  ry_dt": {.      
-00006510: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-00006520: 2022 5265 636f 7264 2065 7665 7279 2024   "Record every $
-00006530: 6474 243a 222c 0a20 2020 2020 2020 2020  dt$:",.         
-00006540: 2020 2020 2022 756e 6974 7322 3a20 2273       "units": "s
-00006550: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00006560: 2022 7661 6c75 6522 3a20 3630 2e30 2c0a   "value": 60.0,.
-00006570: 2020 2020 2020 2020 2020 2020 2020 2272                "r
-00006580: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
-00006590: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-000065a0: 6573 6372 6970 7469 6f6e 223a 2022 5265  escription": "Re
-000065b0: 636f 7264 2061 2064 6174 6170 6f69 6e74  cord a datapoint
-000065c0: 2061 7420 7072 6573 6372 6962 6564 2074   at prescribed t
-000065d0: 696d 6520 7370 6163 696e 6722 2c0a 2020  ime spacing",.  
-000065e0: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-000065f0: 6175 6c74 5f76 616c 7565 223a 2033 302e  ault_value": 30.
-00006600: 300a 2020 2020 2020 2020 2020 2020 7d2c  0.            },
-00006610: 0a20 2020 2020 2020 2020 2020 2022 6c69  .            "li
-00006620: 6d69 745f 6375 7272 656e 745f 6d61 7822  mit_current_max"
-00006630: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00006640: 2020 226c 6162 656c 223a 2022 4d61 7869    "label": "Maxi
-00006650: 6d75 6d20 6375 7272 656e 743a 222c 0a20  mum current:",. 
-00006660: 2020 2020 2020 2020 2020 2020 2022 756e               "un
-00006670: 6974 7322 3a20 2249 222c 0a20 2020 2020  its": "I",.     
-00006680: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00006690: 3a20 6e75 6c6c 2c0a 2020 2020 2020 2020  : null,.        
-000066a0: 2020 2020 2020 2272 6571 7569 7265 6422        "required"
-000066b0: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-000066c0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-000066d0: 696f 6e22 3a20 2244 6566 696e 6520 7468  ion": "Define th
-000066e0: 6520 7570 7065 7220 6c69 6d69 7420 6f66  e upper limit of
-000066f0: 2063 7572 7265 6e74 2066 6f72 2074 6869   current for thi
-00006700: 7320 7374 6570 222c 0a20 2020 2020 2020  s step",.       
-00006710: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
-00006720: 7661 6c75 6522 3a20 6e75 6c6c 0a20 2020  value": null.   
-00006730: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00006740: 2020 2020 2020 2020 226c 696d 6974 5f63          "limit_c
-00006750: 7572 7265 6e74 5f6d 696e 223a 207b 0a20  urrent_min": {. 
-00006760: 2020 2020 2020 2020 2020 2020 2022 6c61               "la
-00006770: 6265 6c22 3a20 224d 696e 696d 756d 2063  bel": "Minimum c
-00006780: 7572 7265 6e74 3a22 2c0a 2020 2020 2020  urrent:",.      
-00006790: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-000067a0: 2022 4922 2c0a 2020 2020 2020 2020 2020   "I",.          
-000067b0: 2020 2020 2276 616c 7565 223a 206e 756c      "value": nul
-000067c0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-000067d0: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
-000067e0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-000067f0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00006800: 2022 4465 6669 6e65 2074 6865 206c 6f77   "Define the low
-00006810: 6572 206c 696d 6974 206f 6620 6375 7272  er limit of curr
-00006820: 656e 7420 666f 7220 7468 6973 2073 7465  ent for this ste
-00006830: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-00006840: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-00006850: 223a 206e 756c 6c0a 2020 2020 2020 2020  ": null.        
-00006860: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00006870: 2020 2022 6c69 6d69 745f 766f 6c74 6167     "limit_voltag
-00006880: 655f 6d61 7822 3a20 7b0a 2020 2020 2020  e_max": {.      
-00006890: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-000068a0: 2022 4d61 7869 6d75 6d20 766f 6c74 6167   "Maximum voltag
-000068b0: 653a 222c 0a20 2020 2020 2020 2020 2020  e:",.           
-000068c0: 2020 2022 756e 6974 7322 3a20 2256 222c     "units": "V",
-000068d0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000068e0: 7661 6c75 6522 3a20 322e 352c 0a20 2020  value": 2.5,.   
-000068f0: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
-00006900: 6972 6564 223a 2066 616c 7365 2c0a 2020  ired": false,.  
-00006910: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00006920: 6372 6970 7469 6f6e 223a 2022 4465 6669  cription": "Defi
-00006930: 6e65 2074 6865 2075 7070 6572 206c 696d  ne the upper lim
-00006940: 6974 206f 6620 766f 6c74 6167 6520 666f  it of voltage fo
-00006950: 7220 7468 6973 2073 7465 7022 2c0a 2020  r this step",.  
-00006960: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-00006970: 6175 6c74 5f76 616c 7565 223a 206e 756c  ault_value": nul
-00006980: 6c0a 2020 2020 2020 2020 2020 2020 7d2c  l.            },
-00006990: 0a20 2020 2020 2020 2020 2020 2022 6c69  .            "li
-000069a0: 6d69 745f 766f 6c74 6167 655f 6d69 6e22  mit_voltage_min"
-000069b0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000069c0: 2020 226c 6162 656c 223a 2022 4d69 6e69    "label": "Mini
-000069d0: 6d75 6d20 766f 6c74 6167 653a 222c 0a20  mum voltage:",. 
-000069e0: 2020 2020 2020 2020 2020 2020 2022 756e               "un
-000069f0: 6974 7322 3a20 2256 222c 0a20 2020 2020  its": "V",.     
-00006a00: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00006a10: 3a20 312e 302c 0a20 2020 2020 2020 2020  : 1.0,.         
-00006a20: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
-00006a30: 2066 616c 7365 2c0a 2020 2020 2020 2020   false,.        
-00006a40: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
-00006a50: 6f6e 223a 2022 4465 6669 6e65 2074 6865  on": "Define the
-00006a60: 206c 6f77 6572 206c 696d 6974 206f 6620   lower limit of 
-00006a70: 766f 6c74 6167 6520 666f 7220 7468 6973  voltage for this
-00006a80: 2073 7465 7022 2c0a 2020 2020 2020 2020   step",.        
-00006a90: 2020 2020 2020 2264 6566 6175 6c74 5f76        "default_v
-00006aa0: 616c 7565 223a 206e 756c 6c0a 2020 2020  alue": null.    
-00006ab0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00006ac0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00006ad0: 2022 7368 6f72 745f 6e61 6d65 223a 2022   "short_name": "
-00006ae0: 4343 222c 0a20 2020 2020 2020 2020 2022  CC",.          "
-00006af0: 6465 7363 7269 7074 696f 6e22 3a20 2243  description": "C
-00006b00: 6f6e 7472 6f6c 6c65 6420 6375 7272 656e  ontrolled curren
-00006b10: 7420 7465 6368 6e69 7175 652c 2077 6974  t technique, wit
-00006b20: 6820 6f70 7469 6f6e 616c 2076 6f6c 7461  h optional volta
-00006b30: 6765 2061 6e64 2063 7572 7265 6e74 206c  ge and current l
-00006b40: 696d 6974 7322 0a20 2020 2020 2020 207d  imits".        }
-00006b50: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
-00006b60: 2020 2020 2020 226e 616d 6522 3a20 2243        "name": "C
-00006b70: 435f 3222 2c0a 2020 2020 2020 2020 2020  C_2",.          
-00006b80: 2264 6576 6963 6522 3a20 224d 5047 3222  "device": "MPG2"
-00006b90: 2c0a 2020 2020 2020 2020 2020 2274 6563  ,.          "tec
-00006ba0: 686e 6971 7565 223a 2022 636f 6e73 7461  hnique": "consta
-00006bb0: 6e74 5f63 7572 7265 6e74 222c 0a20 2020  nt_current",.   
-00006bc0: 2020 2020 2020 2022 7061 7261 6d65 7465         "paramete
-00006bd0: 7273 223a 207b 0a20 2020 2020 2020 2020  rs": {.         
-00006be0: 2020 2022 7469 6d65 223a 207b 0a20 2020     "time": {.   
-00006bf0: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
-00006c00: 6c22 3a20 2254 696d 653a 222c 0a20 2020  l": "Time:",.   
-00006c10: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
-00006c20: 7322 3a20 2273 222c 0a20 2020 2020 2020  s": "s",.       
-00006c30: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00006c40: 3336 3030 302e 302c 0a20 2020 2020 2020  36000.0,.       
-00006c50: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-00006c60: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-00006c70: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00006c80: 696f 6e22 3a20 224d 6178 696d 756d 2064  ion": "Maximum d
-00006c90: 7572 6174 696f 6e20 6f66 2074 6865 2043  uration of the C
-00006ca0: 4320 7374 6570 222c 0a20 2020 2020 2020  C step",.       
-00006cb0: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
-00006cc0: 7661 6c75 6522 3a20 302e 300a 2020 2020  value": 0.0.    
-00006cd0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00006ce0: 2020 2020 2020 2022 455f 7261 6e67 6522         "E_range"
-00006cf0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00006d00: 2020 226c 6162 656c 223a 2022 4520 7261    "label": "E ra
-00006d10: 6e67 6522 2c0a 2020 2020 2020 2020 2020  nge",.          
-00006d20: 2020 2020 2275 6e69 7473 223a 2022 222c      "units": "",
-00006d30: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00006d40: 7661 6c75 6522 3a20 222b 2d35 2e30 2056  value": "+-5.0 V
-00006d50: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00006d60: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
-00006d70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00006d80: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00006d90: 2253 656c 6563 7420 7468 6520 766f 6c74  "Select the volt
-00006da0: 6167 6520 7261 6e67 6520 6f66 2074 6865  age range of the
-00006db0: 2070 6f74 656e 7469 6f73 7461 7422 2c0a   potentiostat",.
-00006dc0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00006dd0: 6566 6175 6c74 5f76 616c 7565 223a 2022  efault_value": "
-00006de0: 6175 746f 220a 2020 2020 2020 2020 2020  auto".          
-00006df0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-00006e00: 2022 495f 7261 6e67 6522 3a20 7b0a 2020   "I_range": {.  
-00006e10: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
-00006e20: 656c 223a 2022 4920 7261 6e67 6522 2c0a  el": "I range",.
-00006e30: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00006e40: 6e69 7473 223a 2022 222c 0a20 2020 2020  nits": "",.     
-00006e50: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
-00006e60: 3a20 2231 3020 6d41 222c 0a20 2020 2020  : "10 mA",.     
-00006e70: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
-00006e80: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
-00006e90: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
-00006ea0: 7074 696f 6e22 3a20 2253 656c 6563 7420  ption": "Select 
-00006eb0: 7468 6520 6375 7272 656e 7420 7261 6e67  the current rang
-00006ec0: 6520 6f66 2074 6865 2070 6f74 656e 7469  e of the potenti
-00006ed0: 6f73 7461 7422 2c0a 2020 2020 2020 2020  ostat",.        
-00006ee0: 2020 2020 2020 2264 6566 6175 6c74 5f76        "default_v
-00006ef0: 616c 7565 223a 2022 6b65 6570 220a 2020  alue": "keep".  
-00006f00: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00006f10: 2020 2020 2020 2020 2022 6375 7272 656e           "curren
-00006f20: 7422 3a20 7b0a 2020 2020 2020 2020 2020  t": {.          
-00006f30: 2020 2020 226c 6162 656c 223a 2022 5374      "label": "St
-00006f40: 6570 2063 7572 7265 6e74 3a22 2c0a 2020  ep current:",.  
-00006f50: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
-00006f60: 7473 223a 2022 4922 2c0a 2020 2020 2020  ts": "I",.      
-00006f70: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
-00006f80: 2022 442f 3130 222c 0a20 2020 2020 2020   "D/10",.       
-00006f90: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-00006fa0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
-00006fb0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00006fc0: 696f 6e22 3a20 2243 7572 7265 6e74 2064  ion": "Current d
-00006fd0: 7572 696e 6720 7468 6520 6375 7272 656e  uring the curren
-00006fe0: 7420 7374 6570 222c 0a20 2020 2020 2020  t step",.       
-00006ff0: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
-00007000: 7661 6c75 6522 3a20 302e 300a 2020 2020  value": 0.0.    
-00007010: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00007020: 2020 2020 2020 2022 6973 5f64 656c 7461         "is_delta
-00007030: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00007040: 2020 2022 6c61 6265 6c22 3a20 225c 7530     "label": "\u0
-00007050: 3339 3424 4924 3a22 2c0a 2020 2020 2020  394$I$:",.      
-00007060: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-00007070: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
-00007080: 2020 2022 7661 6c75 6522 3a20 6661 6c73     "value": fals
-00007090: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000070a0: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
-000070b0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000070c0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-000070d0: 2249 7320 7468 6520 7374 6570 2063 7572  "Is the step cur
-000070e0: 7265 6e74 2061 2024 5c5c 4465 6c74 6124  rent a $\\Delta$
-000070f0: 2066 726f 6d20 7072 6576 696f 7573 2073   from previous s
-00007100: 7465 703f 222c 0a20 2020 2020 2020 2020  tep?",.         
-00007110: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
-00007120: 6c75 6522 3a20 6661 6c73 650a 2020 2020  lue": false.    
-00007130: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00007140: 2020 2020 2020 2022 6e5f 6379 636c 6573         "n_cycles
-00007150: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00007160: 2020 2022 6c61 6265 6c22 3a20 224e 756d     "label": "Num
-00007170: 6265 7220 6f66 2063 7963 6c65 733a 222c  ber of cycles:",
-00007180: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00007190: 756e 6974 7322 3a20 2222 2c0a 2020 2020  units": "",.    
-000071a0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-000071b0: 223a 2030 2c0a 2020 2020 2020 2020 2020  ": 0,.          
-000071c0: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
-000071d0: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
-000071e0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-000071f0: 223a 2022 4379 636c 6520 7468 726f 7567  ": "Cycle throug
-00007200: 6820 7468 6520 6375 7272 656e 7420 7465  h the current te
-00007210: 6368 6e69 7175 6520 4e20 7469 6d65 732e  chnique N times.
-00007220: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00007230: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
-00007240: 3a20 300a 2020 2020 2020 2020 2020 2020  : 0.            
-00007250: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
-00007260: 6578 6974 5f6f 6e5f 6c69 6d69 7422 3a20  exit_on_limit": 
-00007270: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00007280: 226c 6162 656c 223a 2022 4578 6974 2077  "label": "Exit w
-00007290: 6865 6e20 6c69 6d69 7473 2072 6561 6368  hen limits reach
-000072a0: 6564 3f22 2c0a 2020 2020 2020 2020 2020  ed?",.          
-000072b0: 2020 2020 2275 6e69 7473 223a 2022 222c      "units": "",
-000072c0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000072d0: 7661 6c75 6522 3a20 6661 6c73 652c 0a20  value": false,. 
-000072e0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-000072f0: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
-00007300: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00007310: 7363 7269 7074 696f 6e22 3a20 2253 746f  scription": "Sto
-00007320: 7020 7468 6520 7768 6f6c 6520 6578 7065  p the whole expe
-00007330: 7269 6d65 6e74 2077 6865 6e20 6c69 6d69  riment when limi
-00007340: 7420 6973 2072 6561 6368 6564 3f22 2c0a  t is reached?",.
-00007350: 2020 2020 2020 2020 2020 2020 2020 2264                "d
-00007360: 6566 6175 6c74 5f76 616c 7565 223a 2066  efault_value": f
-00007370: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-00007380: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00007390: 2272 6563 6f72 645f 6576 6572 795f 6445  "record_every_dE
-000073a0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-000073b0: 2020 2022 6c61 6265 6c22 3a20 2252 6563     "label": "Rec
-000073c0: 6f72 6420 6576 6572 7920 2464 4524 3a22  ord every $dE$:"
-000073d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000073e0: 2275 6e69 7473 223a 2022 5622 2c0a 2020  "units": "V",.  
-000073f0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
-00007400: 7565 223a 2030 2e31 2c0a 2020 2020 2020  ue": 0.1,.      
-00007410: 2020 2020 2020 2020 2272 6571 7569 7265          "require
-00007420: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
-00007430: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00007440: 7469 6f6e 223a 2022 5265 636f 7264 2061  tion": "Record a
-00007450: 2064 6174 6170 6f69 6e74 2061 7420 7072   datapoint at pr
-00007460: 6573 6372 6962 6564 2076 6f6c 7461 6765  escribed voltage
-00007470: 2073 7061 6369 6e67 222c 0a20 2020 2020   spacing",.     
-00007480: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
-00007490: 745f 7661 6c75 6522 3a20 302e 3030 350a  t_value": 0.005.
-000074a0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-000074b0: 2020 2020 2020 2020 2020 2022 7265 636f             "reco
-000074c0: 7264 5f65 7665 7279 5f64 7422 3a20 7b0a  rd_every_dt": {.
-000074d0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-000074e0: 6162 656c 223a 2022 5265 636f 7264 2065  abel": "Record e
-000074f0: 7665 7279 2024 6474 243a 222c 0a20 2020  very $dt$:",.   
-00007500: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
-00007510: 7322 3a20 2273 222c 0a20 2020 2020 2020  s": "s",.       
-00007520: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
-00007530: 3630 2e30 2c0a 2020 2020 2020 2020 2020  60.0,.          
-00007540: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
-00007550: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
-00007560: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00007570: 223a 2022 5265 636f 7264 2061 2064 6174  ": "Record a dat
-00007580: 6170 6f69 6e74 2061 7420 7072 6573 6372  apoint at prescr
-00007590: 6962 6564 2074 696d 6520 7370 6163 696e  ibed time spacin
-000075a0: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
-000075b0: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-000075c0: 223a 2033 302e 300a 2020 2020 2020 2020  ": 30.0.        
-000075d0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000075e0: 2020 2022 6c69 6d69 745f 6375 7272 656e     "limit_curren
-000075f0: 745f 6d61 7822 3a20 7b0a 2020 2020 2020  t_max": {.      
-00007600: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-00007610: 2022 4d61 7869 6d75 6d20 6375 7272 656e   "Maximum curren
-00007620: 743a 222c 0a20 2020 2020 2020 2020 2020  t:",.           
-00007630: 2020 2022 756e 6974 7322 3a20 2249 222c     "units": "I",
-00007640: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-00007650: 7661 6c75 6522 3a20 6e75 6c6c 2c0a 2020  value": null,.  
-00007660: 2020 2020 2020 2020 2020 2020 2272 6571              "req
-00007670: 7569 7265 6422 3a20 6661 6c73 652c 0a20  uired": false,. 
-00007680: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00007690: 7363 7269 7074 696f 6e22 3a20 2244 6566  scription": "Def
-000076a0: 696e 6520 7468 6520 7570 7065 7220 6c69  ine the upper li
-000076b0: 6d69 7420 6f66 2063 7572 7265 6e74 2066  mit of current f
-000076c0: 6f72 2074 6869 7320 7374 6570 222c 0a20  or this step",. 
-000076d0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-000076e0: 6661 756c 745f 7661 6c75 6522 3a20 6e75  fault_value": nu
-000076f0: 6c6c 0a20 2020 2020 2020 2020 2020 207d  ll.            }
-00007700: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-00007710: 696d 6974 5f63 7572 7265 6e74 5f6d 696e  imit_current_min
-00007720: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00007730: 2020 2022 6c61 6265 6c22 3a20 224d 696e     "label": "Min
-00007740: 696d 756d 2063 7572 7265 6e74 3a22 2c0a  imum current:",.
-00007750: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00007760: 6e69 7473 223a 2022 4922 2c0a 2020 2020  nits": "I",.    
-00007770: 2020 2020 2020 2020 2020 2276 616c 7565            "value
-00007780: 223a 206e 756c 6c2c 0a20 2020 2020 2020  ": null,.       
-00007790: 2020 2020 2020 2022 7265 7175 6972 6564         "required
-000077a0: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
-000077b0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-000077c0: 7469 6f6e 223a 2022 4465 6669 6e65 2074  tion": "Define t
-000077d0: 6865 206c 6f77 6572 206c 696d 6974 206f  he lower limit o
-000077e0: 6620 6375 7272 656e 7420 666f 7220 7468  f current for th
-000077f0: 6973 2073 7465 7022 2c0a 2020 2020 2020  is step",.      
-00007800: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
-00007810: 5f76 616c 7565 223a 206e 756c 6c0a 2020  _value": null.  
-00007820: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00007830: 2020 2020 2020 2020 2022 6c69 6d69 745f           "limit_
-00007840: 766f 6c74 6167 655f 6d61 7822 3a20 7b0a  voltage_max": {.
-00007850: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00007860: 6162 656c 223a 2022 4d61 7869 6d75 6d20  abel": "Maximum 
-00007870: 766f 6c74 6167 653a 222c 0a20 2020 2020  voltage:",.     
-00007880: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
-00007890: 3a20 2256 222c 0a20 2020 2020 2020 2020  : "V",.         
-000078a0: 2020 2020 2022 7661 6c75 6522 3a20 322e       "value": 2.
-000078b0: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-000078c0: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
-000078d0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-000078e0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000078f0: 2022 4465 6669 6e65 2074 6865 2075 7070   "Define the upp
-00007900: 6572 206c 696d 6974 206f 6620 766f 6c74  er limit of volt
-00007910: 6167 6520 666f 7220 7468 6973 2073 7465  age for this ste
-00007920: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-00007930: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-00007940: 223a 206e 756c 6c0a 2020 2020 2020 2020  ": null.        
-00007950: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00007960: 2020 2022 6c69 6d69 745f 766f 6c74 6167     "limit_voltag
-00007970: 655f 6d69 6e22 3a20 7b0a 2020 2020 2020  e_min": {.      
-00007980: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
-00007990: 2022 4d69 6e69 6d75 6d20 766f 6c74 6167   "Minimum voltag
-000079a0: 653a 222c 0a20 2020 2020 2020 2020 2020  e:",.           
-000079b0: 2020 2022 756e 6974 7322 3a20 2256 222c     "units": "V",
-000079c0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
-000079d0: 7661 6c75 6522 3a20 312e 352c 0a20 2020  value": 1.5,.   
-000079e0: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
-000079f0: 6972 6564 223a 2066 616c 7365 2c0a 2020  ired": false,.  
-00007a00: 2020 2020 2020 2020 2020 2020 2264 6573              "des
-00007a10: 6372 6970 7469 6f6e 223a 2022 4465 6669  cription": "Defi
-00007a20: 6e65 2074 6865 206c 6f77 6572 206c 696d  ne the lower lim
-00007a30: 6974 206f 6620 766f 6c74 6167 6520 666f  it of voltage fo
-00007a40: 7220 7468 6973 2073 7465 7022 2c0a 2020  r this step",.  
-00007a50: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-00007a60: 6175 6c74 5f76 616c 7565 223a 206e 756c  ault_value": nul
-00007a70: 6c0a 2020 2020 2020 2020 2020 2020 7d0a  l.            }.
-00007a80: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00007a90: 2020 2020 2020 2022 7368 6f72 745f 6e61         "short_na
-00007aa0: 6d65 223a 2022 4343 222c 0a20 2020 2020  me": "CC",.     
-00007ab0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
-00007ac0: 6e22 3a20 2243 6f6e 7472 6f6c 6c65 6420  n": "Controlled 
-00007ad0: 6375 7272 656e 7420 7465 6368 6e69 7175  current techniqu
-00007ae0: 652c 2077 6974 6820 6f70 7469 6f6e 616c  e, with optional
-00007af0: 2076 6f6c 7461 6765 2061 6e64 2063 7572   voltage and cur
-00007b00: 7265 6e74 206c 696d 6974 7322 0a20 2020  rent limits".   
-00007b10: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00007b20: 7b0a 2020 2020 2020 2020 2020 226e 616d  {.          "nam
-00007b30: 6522 3a20 224c 4f4f 505f 3122 2c0a 2020  e": "LOOP_1",.  
-00007b40: 2020 2020 2020 2020 2264 6576 6963 6522          "device"
-00007b50: 3a20 224d 5047 3222 2c0a 2020 2020 2020  : "MPG2",.      
-00007b60: 2020 2020 2274 6563 686e 6971 7565 223a      "technique":
-00007b70: 2022 6c6f 6f70 222c 0a20 2020 2020 2020   "loop",.       
-00007b80: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
-00007b90: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00007ba0: 676f 746f 223a 207b 0a20 2020 2020 2020  goto": {.       
-00007bb0: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
-00007bc0: 2247 6f20 746f 3a22 2c0a 2020 2020 2020  "Go to:",.      
-00007bd0: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
-00007be0: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
-00007bf0: 2020 2022 7661 6c75 6522 3a20 312c 0a20     "value": 1,. 
-00007c00: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00007c10: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
-00007c20: 2020 2020 2020 2020 2020 2020 2022 6465               "de
-00007c30: 7363 7269 7074 696f 6e22 3a20 2249 6e64  scription": "Ind
-00007c40: 6578 206f 6620 7468 6520 7465 6368 6e69  ex of the techni
-00007c50: 7175 6520 746f 2067 6f20 6261 636b 2074  que to go back t
-00007c60: 6f22 2c0a 2020 2020 2020 2020 2020 2020  o",.            
-00007c70: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
-00007c80: 223a 2031 0a20 2020 2020 2020 2020 2020  ": 1.           
-00007c90: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00007ca0: 226e 5f67 6f74 6f73 223a 207b 0a20 2020  "n_gotos": {.   
-00007cb0: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
-00007cc0: 6c22 3a20 2252 6570 6561 7473 222c 0a20  l": "Repeats",. 
-00007cd0: 2020 2020 2020 2020 2020 2020 2022 756e               "un
-00007ce0: 6974 7322 3a20 2222 2c0a 2020 2020 2020  its": "",.      
-00007cf0: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
-00007d00: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
-00007d10: 2020 2272 6571 7569 7265 6422 3a20 7472    "required": tr
-00007d20: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00007d30: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-00007d40: 2022 4e75 6d62 6572 206f 6620 7469 6d65   "Number of time
-00007d50: 7320 7468 6520 7465 6368 6e69 7175 6520  s the technique 
-00007d60: 7769 6c6c 206a 756d 703b 2073 6574 2074  will jump; set t
-00007d70: 6f20 2d31 2066 6f72 2075 6e6c 696d 6974  o -1 for unlimit
-00007d80: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
-00007d90: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
-00007da0: 6522 3a20 2d31 0a20 2020 2020 2020 2020  e": -1.         
-00007db0: 2020 207d 0a20 2020 2020 2020 2020 207d     }.          }
-00007dc0: 2c0a 2020 2020 2020 2020 2020 2273 686f  ,.          "sho
-00007dd0: 7274 5f6e 616d 6522 3a20 224c 4f4f 5022  rt_name": "LOOP"
-00007de0: 2c0a 2020 2020 2020 2020 2020 2264 6573  ,.          "des
-00007df0: 6372 6970 7469 6f6e 223a 2022 4c6f 6f70  cription": "Loop
-00007e00: 2074 6563 686e 6971 7565 2c20 616c 6c6f   technique, allo
-00007e10: 7769 6e67 2074 6f20 7265 7065 6174 2061  wing to repeat a
-00007e20: 2073 6574 206f 6620 7072 6563 6564 696e   set of precedin
-00007e30: 6720 7465 6368 6e69 7175 6573 2069 6e20  g techniques in 
-00007e40: 6120 7465 6368 6e69 7175 6520 6172 7261  a technique arra
-00007e50: 7922 0a20 2020 2020 2020 207d 0a20 2020  y".        }.   
-00007e60: 2020 205d 0a20 2020 207d 0a20 207d          ].    }.  }
+000000b0: 207d 2c0a 2020 2020 2244 4546 4155 4c54   },.    "DEFAULT
+000000c0: 5f4d 4f4e 4954 4f52 5f50 524f 544f 434f  _MONITOR_PROTOCO
+000000d0: 4c22 3a20 7b0a 2020 2020 2020 2020 2273  L": {.        "s
+000000e0: 6f75 7263 6573 223a 207b 0a20 2020 2020  ources": {.     
+000000f0: 2020 2020 2020 2022 6f75 7470 7574 223a         "output":
+00000100: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00000110: 2020 2022 6669 6c65 7061 7468 223a 2022     "filepath": "
+00000120: 736e 6170 7368 6f74 2e6a 736f 6e22 2c0a  snapshot.json",.
+00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000140: 2272 6566 7265 7368 5f72 6174 6522 3a20  "refresh_rate": 
+00000150: 3630 300a 2020 2020 2020 2020 2020 2020  600.            
+00000160: 7d0a 2020 2020 2020 2020 7d2c 0a20 2020  }.        },.   
+00000170: 2020 2020 2022 6f70 7469 6f6e 7322 3a20       "options": 
+00000180: 7b0a 2020 2020 2020 2020 2020 2020 2263  {.            "c
+00000190: 6865 636b 5f74 7970 6522 3a20 2264 6973  heck_type": "dis
+000001a0: 6368 6172 6765 5f63 6170 6163 6974 7922  charge_capacity"
+000001b0: 2c0a 2020 2020 2020 2020 2020 2020 2263  ,.            "c
+000001c0: 6f6e 7365 6375 7469 7665 5f63 7963 6c65  onsecutive_cycle
+000001d0: 7322 3a20 322c 0a20 2020 2020 2020 2020  s": 2,.         
+000001e0: 2020 2022 7468 7265 7368 6f6c 6422 3a20     "threshold": 
+000001f0: 302e 380a 2020 2020 2020 2020 7d2c 0a20  0.8.        },. 
+00000200: 2020 2020 2020 2022 7265 7472 6965 7665         "retrieve
+00000210: 223a 205b 2272 6573 756c 7473 2e6a 736f  ": ["results.jso
+00000220: 6e22 5d2c 0a20 2020 2020 2020 2022 7265  n"],.        "re
+00000230: 7472 6965 7665 5f74 656d 706f 7261 7279  trieve_temporary
+00000240: 223a 205b 2272 6573 756c 7473 2e7a 6970  ": ["results.zip
+00000250: 225d 0a20 2020 207d 2c0a 2020 2020 2244  "].    },.    "D
+00000260: 4546 4155 4c54 5f44 4953 4348 4152 4745  EFAULT_DISCHARGE
+00000270: 5f4d 4554 484f 4422 3a20 7b0a 2020 2020  _METHOD": {.    
+00000280: 2020 226d 6574 686f 6422 3a20 5b0a 2020    "method": [.  
+00000290: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000002a0: 2020 226e 616d 6522 3a20 2243 435f 3122    "name": "CC_1"
+000002b0: 2c0a 2020 2020 2020 2020 2020 2264 6576  ,.          "dev
+000002c0: 6963 6522 3a20 224d 5047 3222 2c0a 2020  ice": "MPG2",.  
+000002d0: 2020 2020 2020 2020 2274 6563 686e 6971          "techniq
+000002e0: 7565 223a 2022 636f 6e73 7461 6e74 5f63  ue": "constant_c
+000002f0: 7572 7265 6e74 222c 0a20 2020 2020 2020  urrent",.       
+00000300: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
+00000310: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00000320: 7469 6d65 223a 207b 0a20 2020 2020 2020  time": {.       
+00000330: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00000340: 2254 696d 653a 222c 0a20 2020 2020 2020  "Time:",.       
+00000350: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00000360: 2273 222c 0a20 2020 2020 2020 2020 2020  "s",.           
+00000370: 2020 2022 7661 6c75 6522 3a20 3336 3030     "value": 3600
+00000380: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
+00000390: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
+000003a0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+000003b0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+000003c0: 3a20 224d 6178 696d 756d 2064 7572 6174  : "Maximum durat
+000003d0: 696f 6e20 6f66 2074 6865 2043 4320 7374  ion of the CC st
+000003e0: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
+000003f0: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
+00000400: 6522 3a20 302e 300a 2020 2020 2020 2020  e": 0.0.        
+00000410: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00000420: 2020 2022 455f 7261 6e67 6522 3a20 7b0a     "E_range": {.
+00000430: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00000440: 6162 656c 223a 2022 4520 7261 6e67 6522  abel": "E range"
+00000450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000460: 2275 6e69 7473 223a 2022 222c 0a20 2020  "units": "",.   
+00000470: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00000480: 6522 3a20 222b 2d35 2e30 2056 222c 0a20  e": "+-5.0 V",. 
+00000490: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+000004a0: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
+000004b0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+000004c0: 7363 7269 7074 696f 6e22 3a20 2253 656c  scription": "Sel
+000004d0: 6563 7420 7468 6520 766f 6c74 6167 6520  ect the voltage 
+000004e0: 7261 6e67 6520 6f66 2074 6865 2070 6f74  range of the pot
+000004f0: 656e 7469 6f73 7461 7422 2c0a 2020 2020  entiostat",.    
+00000500: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
+00000510: 6c74 5f76 616c 7565 223a 2022 6175 746f  lt_value": "auto
+00000520: 220a 2020 2020 2020 2020 2020 2020 7d2c  ".            },
+00000530: 0a20 2020 2020 2020 2020 2020 2022 495f  .            "I_
+00000540: 7261 6e67 6522 3a20 7b0a 2020 2020 2020  range": {.      
+00000550: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
+00000560: 2022 4920 7261 6e67 6522 2c0a 2020 2020   "I range",.    
+00000570: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+00000580: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
+00000590: 2020 2020 2022 7661 6c75 6522 3a20 2231       "value": "1
+000005a0: 3020 6d41 222c 0a20 2020 2020 2020 2020  0 mA",.         
+000005b0: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
+000005c0: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
+000005d0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+000005e0: 6e22 3a20 2253 656c 6563 7420 7468 6520  n": "Select the 
+000005f0: 6375 7272 656e 7420 7261 6e67 6520 6f66  current range of
+00000600: 2074 6865 2070 6f74 656e 7469 6f73 7461   the potentiosta
+00000610: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00000620: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
+00000630: 223a 2022 6b65 6570 220a 2020 2020 2020  ": "keep".      
+00000640: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000650: 2020 2020 2022 6375 7272 656e 7422 3a20       "current": 
+00000660: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000670: 226c 6162 656c 223a 2022 5374 6570 2063  "label": "Step c
+00000680: 7572 7265 6e74 3a22 2c0a 2020 2020 2020  urrent:",.      
+00000690: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
+000006a0: 2022 4922 2c0a 2020 2020 2020 2020 2020   "I",.          
+000006b0: 2020 2020 2276 616c 7565 223a 2022 442f      "value": "D/
+000006c0: 3130 222c 0a20 2020 2020 2020 2020 2020  10",.           
+000006d0: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
+000006e0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+000006f0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00000700: 3a20 2243 7572 7265 6e74 2064 7572 696e  : "Current durin
+00000710: 6720 7468 6520 6375 7272 656e 7420 7374  g the current st
+00000720: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
+00000730: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
+00000740: 6522 3a20 302e 300a 2020 2020 2020 2020  e": 0.0.        
+00000750: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00000760: 2020 2022 6973 5f64 656c 7461 223a 207b     "is_delta": {
+00000770: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00000780: 6c61 6265 6c22 3a20 225c 7530 3339 3424  label": "\u0394$
+00000790: 4924 3a22 2c0a 2020 2020 2020 2020 2020  I$:",.          
+000007a0: 2020 2020 2275 6e69 7473 223a 2022 222c      "units": "",
+000007b0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000007c0: 7661 6c75 6522 3a20 6661 6c73 652c 0a20  value": false,. 
+000007d0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+000007e0: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
+000007f0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00000800: 7363 7269 7074 696f 6e22 3a20 2249 7320  scription": "Is 
+00000810: 7468 6520 7374 6570 2063 7572 7265 6e74  the step current
+00000820: 2061 2024 5c5c 4465 6c74 6124 2066 726f   a $\\Delta$ fro
+00000830: 6d20 7072 6576 696f 7573 2073 7465 703f  m previous step?
+00000840: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000850: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
+00000860: 3a20 6661 6c73 650a 2020 2020 2020 2020  : false.        
+00000870: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00000880: 2020 2022 6e5f 6379 636c 6573 223a 207b     "n_cycles": {
+00000890: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000008a0: 6c61 6265 6c22 3a20 224e 756d 6265 7220  label": "Number 
+000008b0: 6f66 2063 7963 6c65 733a 222c 0a20 2020  of cycles:",.   
+000008c0: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
+000008d0: 7322 3a20 2222 2c0a 2020 2020 2020 2020  s": "",.        
+000008e0: 2020 2020 2020 2276 616c 7565 223a 2030        "value": 0
+000008f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000900: 2272 6571 7569 7265 6422 3a20 7472 7565  "required": true
+00000910: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000920: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00000930: 4379 636c 6520 7468 726f 7567 6820 7468  Cycle through th
+00000940: 6520 6375 7272 656e 7420 7465 6368 6e69  e current techni
+00000950: 7175 6520 4e20 7469 6d65 732e 222c 0a20  que N times.",. 
+00000960: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00000970: 6661 756c 745f 7661 6c75 6522 3a20 300a  fault_value": 0.
+00000980: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00000990: 2020 2020 2020 2020 2020 2022 6578 6974             "exit
+000009a0: 5f6f 6e5f 6c69 6d69 7422 3a20 7b0a 2020  _on_limit": {.  
+000009b0: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
+000009c0: 656c 223a 2022 4578 6974 2077 6865 6e20  el": "Exit when 
+000009d0: 6c69 6d69 7473 2072 6561 6368 6564 3f22  limits reached?"
+000009e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000009f0: 2275 6e69 7473 223a 2022 222c 0a20 2020  "units": "",.   
+00000a00: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00000a10: 6522 3a20 6661 6c73 652c 0a20 2020 2020  e": false,.     
+00000a20: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
+00000a30: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+00000a40: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00000a50: 7074 696f 6e22 3a20 2253 746f 7020 7468  ption": "Stop th
+00000a60: 6520 7768 6f6c 6520 6578 7065 7269 6d65  e whole experime
+00000a70: 6e74 2077 6865 6e20 6c69 6d69 7420 6973  nt when limit is
+00000a80: 2072 6561 6368 6564 3f22 2c0a 2020 2020   reached?",.    
+00000a90: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
+00000aa0: 6c74 5f76 616c 7565 223a 2066 616c 7365  lt_value": false
+00000ab0: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00000ac0: 2020 2020 2020 2020 2020 2020 2272 6563              "rec
+00000ad0: 6f72 645f 6576 6572 795f 6445 223a 207b  ord_every_dE": {
+00000ae0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00000af0: 6c61 6265 6c22 3a20 2252 6563 6f72 6420  label": "Record 
+00000b00: 6576 6572 7920 2464 4524 3a22 2c0a 2020  every $dE$:",.  
+00000b10: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
+00000b20: 7473 223a 2022 5622 2c0a 2020 2020 2020  ts": "V",.      
+00000b30: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
+00000b40: 2030 2e31 2c0a 2020 2020 2020 2020 2020   0.1,.          
+00000b50: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
+00000b60: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+00000b70: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00000b80: 223a 2022 5265 636f 7264 2061 2064 6174  ": "Record a dat
+00000b90: 6170 6f69 6e74 2061 7420 7072 6573 6372  apoint at prescr
+00000ba0: 6962 6564 2076 6f6c 7461 6765 2073 7061  ibed voltage spa
+00000bb0: 6369 6e67 222c 0a20 2020 2020 2020 2020  cing",.         
+00000bc0: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
+00000bd0: 6c75 6522 3a20 302e 3030 350a 2020 2020  lue": 0.005.    
+00000be0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000bf0: 2020 2020 2020 2022 7265 636f 7264 5f65         "record_e
+00000c00: 7665 7279 5f64 7422 3a20 7b0a 2020 2020  very_dt": {.    
+00000c10: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00000c20: 223a 2022 5265 636f 7264 2065 7665 7279  ": "Record every
+00000c30: 2024 6474 243a 222c 0a20 2020 2020 2020   $dt$:",.       
+00000c40: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00000c50: 2273 222c 0a20 2020 2020 2020 2020 2020  "s",.           
+00000c60: 2020 2022 7661 6c75 6522 3a20 3630 2e30     "value": 60.0
+00000c70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000c80: 2272 6571 7569 7265 6422 3a20 7472 7565  "required": true
+00000c90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000ca0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00000cb0: 5265 636f 7264 2061 2064 6174 6170 6f69  Record a datapoi
+00000cc0: 6e74 2061 7420 7072 6573 6372 6962 6564  nt at prescribed
+00000cd0: 2074 696d 6520 7370 6163 696e 6722 2c0a   time spacing",.
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00000cf0: 6566 6175 6c74 5f76 616c 7565 223a 2033  efault_value": 3
+00000d00: 302e 300a 2020 2020 2020 2020 2020 2020  0.0.            
+00000d10: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+00000d20: 6c69 6d69 745f 6375 7272 656e 745f 6d61  limit_current_ma
+00000d30: 7822 3a20 7b0a 2020 2020 2020 2020 2020  x": {.          
+00000d40: 2020 2020 226c 6162 656c 223a 2022 4d61      "label": "Ma
+00000d50: 7869 6d75 6d20 6375 7272 656e 743a 222c  ximum current:",
+00000d60: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00000d70: 756e 6974 7322 3a20 2249 222c 0a20 2020  units": "I",.   
+00000d80: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00000d90: 6522 3a20 6e75 6c6c 2c0a 2020 2020 2020  e": null,.      
+00000da0: 2020 2020 2020 2020 2272 6571 7569 7265          "require
+00000db0: 6422 3a20 6661 6c73 652c 0a20 2020 2020  d": false,.     
+00000dc0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00000dd0: 7074 696f 6e22 3a20 2244 6566 696e 6520  ption": "Define 
+00000de0: 7468 6520 7570 7065 7220 6c69 6d69 7420  the upper limit 
+00000df0: 6f66 2063 7572 7265 6e74 2066 6f72 2074  of current for t
+00000e00: 6869 7320 7374 6570 222c 0a20 2020 2020  his step",.     
+00000e10: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
+00000e20: 745f 7661 6c75 6522 3a20 6e75 6c6c 0a20  t_value": null. 
+00000e30: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00000e40: 2020 2020 2020 2020 2020 226c 696d 6974            "limit
+00000e50: 5f63 7572 7265 6e74 5f6d 696e 223a 207b  _current_min": {
+00000e60: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00000e70: 6c61 6265 6c22 3a20 224d 696e 696d 756d  label": "Minimum
+00000e80: 2063 7572 7265 6e74 3a22 2c0a 2020 2020   current:",.    
+00000e90: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+00000ea0: 223a 2022 4922 2c0a 2020 2020 2020 2020  ": "I",.        
+00000eb0: 2020 2020 2020 2276 616c 7565 223a 206e        "value": n
+00000ec0: 756c 6c2c 0a20 2020 2020 2020 2020 2020  ull,.           
+00000ed0: 2020 2022 7265 7175 6972 6564 223a 2066     "required": f
+00000ee0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00000ef0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00000f00: 223a 2022 4465 6669 6e65 2074 6865 206c  ": "Define the l
+00000f10: 6f77 6572 206c 696d 6974 206f 6620 6375  ower limit of cu
+00000f20: 7272 656e 7420 666f 7220 7468 6973 2073  rrent for this s
+00000f30: 7465 7022 2c0a 2020 2020 2020 2020 2020  tep",.          
+00000f40: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
+00000f50: 7565 223a 206e 756c 6c0a 2020 2020 2020  ue": null.      
+00000f60: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000f70: 2020 2020 2022 6c69 6d69 745f 766f 6c74       "limit_volt
+00000f80: 6167 655f 6d61 7822 3a20 7b0a 2020 2020  age_max": {.    
+00000f90: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00000fa0: 223a 2022 4d61 7869 6d75 6d20 766f 6c74  ": "Maximum volt
+00000fb0: 6167 653a 222c 0a20 2020 2020 2020 2020  age:",.         
+00000fc0: 2020 2020 2022 756e 6974 7322 3a20 2256       "units": "V
+00000fd0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00000fe0: 2022 7661 6c75 6522 3a20 322e 352c 0a20   "value": 2.5,. 
+00000ff0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00001000: 7175 6972 6564 223a 2066 616c 7365 2c0a  quired": false,.
+00001010: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00001020: 6573 6372 6970 7469 6f6e 223a 2022 4465  escription": "De
+00001030: 6669 6e65 2074 6865 2075 7070 6572 206c  fine the upper l
+00001040: 696d 6974 206f 6620 766f 6c74 6167 6520  imit of voltage 
+00001050: 666f 7220 7468 6973 2073 7465 7022 2c0a  for this step",.
+00001060: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00001070: 6566 6175 6c74 5f76 616c 7565 223a 206e  efault_value": n
+00001080: 756c 6c0a 2020 2020 2020 2020 2020 2020  ull.            
+00001090: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+000010a0: 6c69 6d69 745f 766f 6c74 6167 655f 6d69  limit_voltage_mi
+000010b0: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
+000010c0: 2020 2020 226c 6162 656c 223a 2022 4d69      "label": "Mi
+000010d0: 6e69 6d75 6d20 766f 6c74 6167 653a 222c  nimum voltage:",
+000010e0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000010f0: 756e 6974 7322 3a20 2256 222c 0a20 2020  units": "V",.   
+00001100: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00001110: 6522 3a20 312e 352c 0a20 2020 2020 2020  e": 1.5,.       
+00001120: 2020 2020 2020 2022 7265 7175 6972 6564         "required
+00001130: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
+00001140: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00001150: 7469 6f6e 223a 2022 4465 6669 6e65 2074  tion": "Define t
+00001160: 6865 206c 6f77 6572 206c 696d 6974 206f  he lower limit o
+00001170: 6620 766f 6c74 6167 6520 666f 7220 7468  f voltage for th
+00001180: 6973 2073 7465 7022 2c0a 2020 2020 2020  is step",.      
+00001190: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+000011a0: 5f76 616c 7565 223a 206e 756c 6c0a 2020  _value": null.  
+000011b0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000011c0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000011d0: 2020 2022 7368 6f72 745f 6e61 6d65 223a     "short_name":
+000011e0: 2022 4343 222c 0a20 2020 2020 2020 2020   "CC",.         
+000011f0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00001200: 2243 6f6e 7472 6f6c 6c65 6420 6375 7272  "Controlled curr
+00001210: 656e 7420 7465 6368 6e69 7175 652c 2077  ent technique, w
+00001220: 6974 6820 6f70 7469 6f6e 616c 2076 6f6c  ith optional vol
+00001230: 7461 6765 2061 6e64 2063 7572 7265 6e74  tage and current
+00001240: 206c 696d 6974 7322 0a20 2020 2020 2020   limits".       
+00001250: 207d 0a20 2020 2020 205d 0a20 2020 207d   }.      ].    }
+00001260: 2c0a 2020 2020 2244 4546 4155 4c54 5f4c  ,.    "DEFAULT_L
+00001270: 4f4e 4754 4552 4d5f 4d45 5448 4f44 223a  ONGTERM_METHOD":
+00001280: 207b 0a20 2020 2020 2022 6d65 7468 6f64   {.      "method
+00001290: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+000012a0: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
+000012b0: 2022 4343 5f31 222c 0a20 2020 2020 2020   "CC_1",.       
+000012c0: 2020 2022 6465 7669 6365 223a 2022 4d50     "device": "MP
+000012d0: 4732 222c 0a20 2020 2020 2020 2020 2022  G2",.          "
+000012e0: 7465 6368 6e69 7175 6522 3a20 2263 6f6e  technique": "con
+000012f0: 7374 616e 745f 6375 7272 656e 7422 2c0a  stant_current",.
+00001300: 2020 2020 2020 2020 2020 2270 6172 616d            "param
+00001310: 6574 6572 7322 3a20 7b0a 2020 2020 2020  eters": {.      
+00001320: 2020 2020 2020 2274 696d 6522 3a20 7b0a        "time": {.
+00001330: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00001340: 6162 656c 223a 2022 5469 6d65 3a22 2c0a  abel": "Time:",.
+00001350: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+00001360: 6e69 7473 223a 2022 7322 2c0a 2020 2020  nits": "s",.    
+00001370: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+00001380: 223a 2031 3038 3030 2e30 2c0a 2020 2020  ": 10800.0,.    
+00001390: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
+000013a0: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
+000013b0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+000013c0: 6970 7469 6f6e 223a 2022 4d61 7869 6d75  iption": "Maximu
+000013d0: 6d20 6475 7261 7469 6f6e 206f 6620 7468  m duration of th
+000013e0: 6520 4343 2073 7465 7022 2c0a 2020 2020  e CC step",.    
+000013f0: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
+00001400: 6c74 5f76 616c 7565 223a 2030 2e30 0a20  lt_value": 0.0. 
+00001410: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00001420: 2020 2020 2020 2020 2020 2245 5f72 616e            "E_ran
+00001430: 6765 223a 207b 0a20 2020 2020 2020 2020  ge": {.         
+00001440: 2020 2020 2022 6c61 6265 6c22 3a20 2245       "label": "E
+00001450: 2072 616e 6765 222c 0a20 2020 2020 2020   range",.       
+00001460: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00001470: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+00001480: 2020 2276 616c 7565 223a 2022 2b2d 352e    "value": "+-5.
+00001490: 3020 5622 2c0a 2020 2020 2020 2020 2020  0 V",.          
+000014a0: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
+000014b0: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+000014c0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+000014d0: 223a 2022 5365 6c65 6374 2074 6865 2076  ": "Select the v
+000014e0: 6f6c 7461 6765 2072 616e 6765 206f 6620  oltage range of 
+000014f0: 7468 6520 706f 7465 6e74 696f 7374 6174  the potentiostat
+00001500: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001510: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
+00001520: 3a20 2261 7574 6f22 0a20 2020 2020 2020  : "auto".       
+00001530: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00001540: 2020 2020 2249 5f72 616e 6765 223a 207b      "I_range": {
+00001550: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00001560: 6c61 6265 6c22 3a20 2249 2072 616e 6765  label": "I range
+00001570: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001580: 2022 756e 6974 7322 3a20 2222 2c0a 2020   "units": "",.  
+00001590: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+000015a0: 7565 223a 2022 3130 206d 4122 2c0a 2020  ue": "10 mA",.  
+000015b0: 2020 2020 2020 2020 2020 2020 2272 6571              "req
+000015c0: 7569 7265 6422 3a20 7472 7565 2c0a 2020  uired": true,.  
+000015d0: 2020 2020 2020 2020 2020 2020 2264 6573              "des
+000015e0: 6372 6970 7469 6f6e 223a 2022 5365 6c65  cription": "Sele
+000015f0: 6374 2074 6865 2063 7572 7265 6e74 2072  ct the current r
+00001600: 616e 6765 206f 6620 7468 6520 706f 7465  ange of the pote
+00001610: 6e74 696f 7374 6174 222c 0a20 2020 2020  ntiostat",.     
+00001620: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
+00001630: 745f 7661 6c75 6522 3a20 226b 6565 7022  t_value": "keep"
+00001640: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00001650: 2020 2020 2020 2020 2020 2020 2263 7572              "cur
+00001660: 7265 6e74 223a 207b 0a20 2020 2020 2020  rent": {.       
+00001670: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00001680: 2253 7465 7020 6375 7272 656e 743a 222c  "Step current:",
+00001690: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000016a0: 756e 6974 7322 3a20 2249 222c 0a20 2020  units": "I",.   
+000016b0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+000016c0: 6522 3a20 2243 2f33 222c 0a20 2020 2020  e": "C/3",.     
+000016d0: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
+000016e0: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+000016f0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00001700: 7074 696f 6e22 3a20 2243 7572 7265 6e74  ption": "Current
+00001710: 2064 7572 696e 6720 7468 6520 6375 7272   during the curr
+00001720: 656e 7420 7374 6570 222c 0a20 2020 2020  ent step",.     
+00001730: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
+00001740: 745f 7661 6c75 6522 3a20 302e 300a 2020  t_value": 0.0.  
+00001750: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00001760: 2020 2020 2020 2020 2022 6973 5f64 656c           "is_del
+00001770: 7461 223a 207b 0a20 2020 2020 2020 2020  ta": {.         
+00001780: 2020 2020 2022 6c61 6265 6c22 3a20 225c       "label": "\
+00001790: 7530 3339 3424 4924 3a22 2c0a 2020 2020  u0394$I$:",.    
+000017a0: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+000017b0: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
+000017c0: 2020 2020 2022 7661 6c75 6522 3a20 6661       "value": fa
+000017d0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+000017e0: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
+000017f0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00001800: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00001810: 3a20 2249 7320 7468 6520 7374 6570 2063  : "Is the step c
+00001820: 7572 7265 6e74 2061 2024 5c5c 4465 6c74  urrent a $\\Delt
+00001830: 6124 2066 726f 6d20 7072 6576 696f 7573  a$ from previous
+00001840: 2073 7465 703f 222c 0a20 2020 2020 2020   step?",.       
+00001850: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
+00001860: 7661 6c75 6522 3a20 6661 6c73 650a 2020  value": false.  
+00001870: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00001880: 2020 2020 2020 2020 2022 6e5f 6379 636c           "n_cycl
+00001890: 6573 223a 207b 0a20 2020 2020 2020 2020  es": {.         
+000018a0: 2020 2020 2022 6c61 6265 6c22 3a20 224e       "label": "N
+000018b0: 756d 6265 7220 6f66 2063 7963 6c65 733a  umber of cycles:
+000018c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000018d0: 2022 756e 6974 7322 3a20 2222 2c0a 2020   "units": "",.  
+000018e0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+000018f0: 7565 223a 2030 2c0a 2020 2020 2020 2020  ue": 0,.        
+00001900: 2020 2020 2020 2272 6571 7569 7265 6422        "required"
+00001910: 3a20 7472 7565 2c0a 2020 2020 2020 2020  : true,.        
+00001920: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00001930: 6f6e 223a 2022 4379 636c 6520 7468 726f  on": "Cycle thro
+00001940: 7567 6820 7468 6520 6375 7272 656e 7420  ugh the current 
+00001950: 7465 6368 6e69 7175 6520 4e20 7469 6d65  technique N time
+00001960: 732e 222c 0a20 2020 2020 2020 2020 2020  s.",.           
+00001970: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
+00001980: 6522 3a20 300a 2020 2020 2020 2020 2020  e": 0.          
+00001990: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+000019a0: 2022 6578 6974 5f6f 6e5f 6c69 6d69 7422   "exit_on_limit"
+000019b0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000019c0: 2020 226c 6162 656c 223a 2022 4578 6974    "label": "Exit
+000019d0: 2077 6865 6e20 6c69 6d69 7473 2072 6561   when limits rea
+000019e0: 6368 6564 3f22 2c0a 2020 2020 2020 2020  ched?",.        
+000019f0: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
+00001a00: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001a10: 2022 7661 6c75 6522 3a20 6661 6c73 652c   "value": false,
+00001a20: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00001a30: 7265 7175 6972 6564 223a 2074 7275 652c  required": true,
+00001a40: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00001a50: 6465 7363 7269 7074 696f 6e22 3a20 2253  description": "S
+00001a60: 746f 7020 7468 6520 7768 6f6c 6520 6578  top the whole ex
+00001a70: 7065 7269 6d65 6e74 2077 6865 6e20 6c69  periment when li
+00001a80: 6d69 7420 6973 2072 6561 6368 6564 3f22  mit is reached?"
+00001a90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001aa0: 2264 6566 6175 6c74 5f76 616c 7565 223a  "default_value":
+00001ab0: 2066 616c 7365 0a20 2020 2020 2020 2020   false.         
+00001ac0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00001ad0: 2020 2272 6563 6f72 645f 6576 6572 795f    "record_every_
+00001ae0: 6445 223a 207b 0a20 2020 2020 2020 2020  dE": {.         
+00001af0: 2020 2020 2022 6c61 6265 6c22 3a20 2252       "label": "R
+00001b00: 6563 6f72 6420 6576 6572 7920 2464 4524  ecord every $dE$
+00001b10: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
+00001b20: 2020 2275 6e69 7473 223a 2022 5622 2c0a    "units": "V",.
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00001b40: 616c 7565 223a 2030 2e31 2c0a 2020 2020  alue": 0.1,.    
+00001b50: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
+00001b60: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
+00001b70: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00001b80: 6970 7469 6f6e 223a 2022 5265 636f 7264  iption": "Record
+00001b90: 2061 2064 6174 6170 6f69 6e74 2061 7420   a datapoint at 
+00001ba0: 7072 6573 6372 6962 6564 2076 6f6c 7461  prescribed volta
+00001bb0: 6765 2073 7061 6369 6e67 222c 0a20 2020  ge spacing",.   
+00001bc0: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
+00001bd0: 756c 745f 7661 6c75 6522 3a20 302e 3030  ult_value": 0.00
+00001be0: 350a 2020 2020 2020 2020 2020 2020 7d2c  5.            },
+00001bf0: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+00001c00: 636f 7264 5f65 7665 7279 5f64 7422 3a20  cord_every_dt": 
+00001c10: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001c20: 226c 6162 656c 223a 2022 5265 636f 7264  "label": "Record
+00001c30: 2065 7665 7279 2024 6474 243a 222c 0a20   every $dt$:",. 
+00001c40: 2020 2020 2020 2020 2020 2020 2022 756e               "un
+00001c50: 6974 7322 3a20 2273 222c 0a20 2020 2020  its": "s",.     
+00001c60: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+00001c70: 3a20 3630 2e30 2c0a 2020 2020 2020 2020  : 60.0,.        
+00001c80: 2020 2020 2020 2272 6571 7569 7265 6422        "required"
+00001c90: 3a20 7472 7565 2c0a 2020 2020 2020 2020  : true,.        
+00001ca0: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00001cb0: 6f6e 223a 2022 5265 636f 7264 2061 2064  on": "Record a d
+00001cc0: 6174 6170 6f69 6e74 2061 7420 7072 6573  atapoint at pres
+00001cd0: 6372 6962 6564 2074 696d 6520 7370 6163  cribed time spac
+00001ce0: 696e 6722 2c0a 2020 2020 2020 2020 2020  ing",.          
+00001cf0: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
+00001d00: 7565 223a 2033 302e 300a 2020 2020 2020  ue": 30.0.      
+00001d10: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001d20: 2020 2020 2022 6c69 6d69 745f 6375 7272       "limit_curr
+00001d30: 656e 745f 6d61 7822 3a20 7b0a 2020 2020  ent_max": {.    
+00001d40: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00001d50: 223a 2022 4d61 7869 6d75 6d20 6375 7272  ": "Maximum curr
+00001d60: 656e 743a 222c 0a20 2020 2020 2020 2020  ent:",.         
+00001d70: 2020 2020 2022 756e 6974 7322 3a20 2249       "units": "I
+00001d80: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001d90: 2022 7661 6c75 6522 3a20 6e75 6c6c 2c0a   "value": null,.
+00001da0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00001db0: 6571 7569 7265 6422 3a20 6661 6c73 652c  equired": false,
+00001dc0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00001dd0: 6465 7363 7269 7074 696f 6e22 3a20 2244  description": "D
+00001de0: 6566 696e 6520 7468 6520 7570 7065 7220  efine the upper 
+00001df0: 6c69 6d69 7420 6f66 2063 7572 7265 6e74  limit of current
+00001e00: 2066 6f72 2074 6869 7320 7374 6570 222c   for this step",
+00001e10: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00001e20: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
+00001e30: 6e75 6c6c 0a20 2020 2020 2020 2020 2020  null.           
+00001e40: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00001e50: 226c 696d 6974 5f63 7572 7265 6e74 5f6d  "limit_current_m
+00001e60: 696e 223a 207b 0a20 2020 2020 2020 2020  in": {.         
+00001e70: 2020 2020 2022 6c61 6265 6c22 3a20 224d       "label": "M
+00001e80: 696e 696d 756d 2063 7572 7265 6e74 3a22  inimum current:"
+00001e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001ea0: 2275 6e69 7473 223a 2022 4922 2c0a 2020  "units": "I",.  
+00001eb0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+00001ec0: 7565 223a 206e 756c 6c2c 0a20 2020 2020  ue": null,.     
+00001ed0: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
+00001ee0: 6564 223a 2066 616c 7365 2c0a 2020 2020  ed": false,.    
+00001ef0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00001f00: 6970 7469 6f6e 223a 2022 4465 6669 6e65  iption": "Define
+00001f10: 2074 6865 206c 6f77 6572 206c 696d 6974   the lower limit
+00001f20: 206f 6620 6375 7272 656e 7420 666f 7220   of current for 
+00001f30: 7468 6973 2073 7465 7022 2c0a 2020 2020  this step",.    
+00001f40: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
+00001f50: 6c74 5f76 616c 7565 223a 206e 756c 6c0a  lt_value": null.
+00001f60: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00001f70: 2020 2020 2020 2020 2020 2022 6c69 6d69             "limi
+00001f80: 745f 766f 6c74 6167 655f 6d61 7822 3a20  t_voltage_max": 
+00001f90: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001fa0: 226c 6162 656c 223a 2022 4d61 7869 6d75  "label": "Maximu
+00001fb0: 6d20 766f 6c74 6167 653a 222c 0a20 2020  m voltage:",.   
+00001fc0: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
+00001fd0: 7322 3a20 2256 222c 0a20 2020 2020 2020  s": "V",.       
+00001fe0: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00001ff0: 322e 352c 0a20 2020 2020 2020 2020 2020  2.5,.           
+00002000: 2020 2022 7265 7175 6972 6564 223a 2066     "required": f
+00002010: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00002020: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00002030: 223a 2022 4465 6669 6e65 2074 6865 2075  ": "Define the u
+00002040: 7070 6572 206c 696d 6974 206f 6620 766f  pper limit of vo
+00002050: 6c74 6167 6520 666f 7220 7468 6973 2073  ltage for this s
+00002060: 7465 7022 2c0a 2020 2020 2020 2020 2020  tep",.          
+00002070: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
+00002080: 7565 223a 206e 756c 6c0a 2020 2020 2020  ue": null.      
+00002090: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+000020a0: 2020 2020 2022 6c69 6d69 745f 766f 6c74       "limit_volt
+000020b0: 6167 655f 6d69 6e22 3a20 7b0a 2020 2020  age_min": {.    
+000020c0: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+000020d0: 223a 2022 4d69 6e69 6d75 6d20 766f 6c74  ": "Minimum volt
+000020e0: 6167 653a 222c 0a20 2020 2020 2020 2020  age:",.         
+000020f0: 2020 2020 2022 756e 6974 7322 3a20 2256       "units": "V
+00002100: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002110: 2022 7661 6c75 6522 3a20 312e 302c 0a20   "value": 1.0,. 
+00002120: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00002130: 7175 6972 6564 223a 2066 616c 7365 2c0a  quired": false,.
+00002140: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00002150: 6573 6372 6970 7469 6f6e 223a 2022 4465  escription": "De
+00002160: 6669 6e65 2074 6865 206c 6f77 6572 206c  fine the lower l
+00002170: 696d 6974 206f 6620 766f 6c74 6167 6520  imit of voltage 
+00002180: 666f 7220 7468 6973 2073 7465 7022 2c0a  for this step",.
+00002190: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000021a0: 6566 6175 6c74 5f76 616c 7565 223a 206e  efault_value": n
+000021b0: 756c 6c0a 2020 2020 2020 2020 2020 2020  ull.            
+000021c0: 7d0a 2020 2020 2020 2020 2020 7d2c 0a20  }.          },. 
+000021d0: 2020 2020 2020 2020 2022 7368 6f72 745f           "short_
+000021e0: 6e61 6d65 223a 2022 4343 222c 0a20 2020  name": "CC",.   
+000021f0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00002200: 696f 6e22 3a20 2243 6f6e 7472 6f6c 6c65  ion": "Controlle
+00002210: 6420 6375 7272 656e 7420 7465 6368 6e69  d current techni
+00002220: 7175 652c 2077 6974 6820 6f70 7469 6f6e  que, with option
+00002230: 616c 2076 6f6c 7461 6765 2061 6e64 2063  al voltage and c
+00002240: 7572 7265 6e74 206c 696d 6974 7322 0a20  urrent limits". 
+00002250: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002260: 2020 7b0a 2020 2020 2020 2020 2020 226e    {.          "n
+00002270: 616d 6522 3a20 2243 435f 3222 2c0a 2020  ame": "CC_2",.  
+00002280: 2020 2020 2020 2020 2264 6576 6963 6522          "device"
+00002290: 3a20 224d 5047 3222 2c0a 2020 2020 2020  : "MPG2",.      
+000022a0: 2020 2020 2274 6563 686e 6971 7565 223a      "technique":
+000022b0: 2022 636f 6e73 7461 6e74 5f63 7572 7265   "constant_curre
+000022c0: 6e74 222c 0a20 2020 2020 2020 2020 2022  nt",.          "
+000022d0: 7061 7261 6d65 7465 7273 223a 207b 0a20  parameters": {. 
+000022e0: 2020 2020 2020 2020 2020 2022 7469 6d65             "time
+000022f0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00002300: 2020 2022 6c61 6265 6c22 3a20 2254 696d     "label": "Tim
+00002310: 653a 222c 0a20 2020 2020 2020 2020 2020  e:",.           
+00002320: 2020 2022 756e 6974 7322 3a20 2273 222c     "units": "s",
+00002330: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00002340: 7661 6c75 6522 3a20 3130 3830 302e 302c  value": 10800.0,
+00002350: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00002360: 7265 7175 6972 6564 223a 2074 7275 652c  required": true,
+00002370: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00002380: 6465 7363 7269 7074 696f 6e22 3a20 224d  description": "M
+00002390: 6178 696d 756d 2064 7572 6174 696f 6e20  aximum duration 
+000023a0: 6f66 2074 6865 2043 4320 7374 6570 222c  of the CC step",
+000023b0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000023c0: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
+000023d0: 302e 300a 2020 2020 2020 2020 2020 2020  0.0.            
+000023e0: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+000023f0: 455f 7261 6e67 6522 3a20 7b0a 2020 2020  E_range": {.    
+00002400: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00002410: 223a 2022 4520 7261 6e67 6522 2c0a 2020  ": "E range",.  
+00002420: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
+00002430: 7473 223a 2022 222c 0a20 2020 2020 2020  ts": "",.       
+00002440: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00002450: 222b 2d35 2e30 2056 222c 0a20 2020 2020  "+-5.0 V",.     
+00002460: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
+00002470: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+00002480: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00002490: 7074 696f 6e22 3a20 2253 656c 6563 7420  ption": "Select 
+000024a0: 7468 6520 766f 6c74 6167 6520 7261 6e67  the voltage rang
+000024b0: 6520 6f66 2074 6865 2070 6f74 656e 7469  e of the potenti
+000024c0: 6f73 7461 7422 2c0a 2020 2020 2020 2020  ostat",.        
+000024d0: 2020 2020 2020 2264 6566 6175 6c74 5f76        "default_v
+000024e0: 616c 7565 223a 2022 6175 746f 220a 2020  alue": "auto".  
+000024f0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00002500: 2020 2020 2020 2020 2022 495f 7261 6e67           "I_rang
+00002510: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
+00002520: 2020 2020 226c 6162 656c 223a 2022 4920      "label": "I 
+00002530: 7261 6e67 6522 2c0a 2020 2020 2020 2020  range",.        
+00002540: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
+00002550: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002560: 2022 7661 6c75 6522 3a20 2231 3020 6d41   "value": "10 mA
+00002570: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002580: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
+00002590: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000025a0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000025b0: 2253 656c 6563 7420 7468 6520 6375 7272  "Select the curr
+000025c0: 656e 7420 7261 6e67 6520 6f66 2074 6865  ent range of the
+000025d0: 2070 6f74 656e 7469 6f73 7461 7422 2c0a   potentiostat",.
+000025e0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000025f0: 6566 6175 6c74 5f76 616c 7565 223a 2022  efault_value": "
+00002600: 6b65 6570 220a 2020 2020 2020 2020 2020  keep".          
+00002610: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00002620: 2022 6375 7272 656e 7422 3a20 7b0a 2020   "current": {.  
+00002630: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
+00002640: 656c 223a 2022 5374 6570 2063 7572 7265  el": "Step curre
+00002650: 6e74 3a22 2c0a 2020 2020 2020 2020 2020  nt:",.          
+00002660: 2020 2020 2275 6e69 7473 223a 2022 4922      "units": "I"
+00002670: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002680: 2276 616c 7565 223a 2022 442f 3322 2c0a  "value": "D/3",.
+00002690: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+000026a0: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000026c0: 6573 6372 6970 7469 6f6e 223a 2022 4375  escription": "Cu
+000026d0: 7272 656e 7420 6475 7269 6e67 2074 6865  rrent during the
+000026e0: 2063 7572 7265 6e74 2073 7465 7022 2c0a   current step",.
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00002700: 6566 6175 6c74 5f76 616c 7565 223a 2030  efault_value": 0
+00002710: 2e30 0a20 2020 2020 2020 2020 2020 207d  .0.            }
+00002720: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
+00002730: 735f 6465 6c74 6122 3a20 7b0a 2020 2020  s_delta": {.    
+00002740: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00002750: 223a 2022 5c75 3033 3934 2449 243a 222c  ": "\u0394$I$:",
+00002760: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00002770: 756e 6974 7322 3a20 2222 2c0a 2020 2020  units": "",.    
+00002780: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+00002790: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
+000027a0: 2020 2020 2020 2020 2272 6571 7569 7265          "require
+000027b0: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
+000027c0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+000027d0: 7469 6f6e 223a 2022 4973 2074 6865 2073  tion": "Is the s
+000027e0: 7465 7020 6375 7272 656e 7420 6120 245c  tep current a $\
+000027f0: 5c44 656c 7461 2420 6672 6f6d 2070 7265  \Delta$ from pre
+00002800: 7669 6f75 7320 7374 6570 3f22 2c0a 2020  vious step?",.  
+00002810: 2020 2020 2020 2020 2020 2020 2264 6566              "def
+00002820: 6175 6c74 5f76 616c 7565 223a 2066 616c  ault_value": fal
+00002830: 7365 0a20 2020 2020 2020 2020 2020 207d  se.            }
+00002840: 2c0a 2020 2020 2020 2020 2020 2020 226e  ,.            "n
+00002850: 5f63 7963 6c65 7322 3a20 7b0a 2020 2020  _cycles": {.    
+00002860: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00002870: 223a 2022 4e75 6d62 6572 206f 6620 6379  ": "Number of cy
+00002880: 636c 6573 3a22 2c0a 2020 2020 2020 2020  cles:",.        
+00002890: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
+000028a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000028b0: 2022 7661 6c75 6522 3a20 302c 0a20 2020   "value": 0,.   
+000028c0: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
+000028d0: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
+000028e0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000028f0: 7269 7074 696f 6e22 3a20 2243 7963 6c65  ription": "Cycle
+00002900: 2074 6872 6f75 6768 2074 6865 2063 7572   through the cur
+00002910: 7265 6e74 2074 6563 686e 6971 7565 204e  rent technique N
+00002920: 2074 696d 6573 2e22 2c0a 2020 2020 2020   times.",.      
+00002930: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+00002940: 5f76 616c 7565 223a 2030 0a20 2020 2020  _value": 0.     
+00002950: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002960: 2020 2020 2020 2265 7869 745f 6f6e 5f6c        "exit_on_l
+00002970: 696d 6974 223a 207b 0a20 2020 2020 2020  imit": {.       
+00002980: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00002990: 2245 7869 7420 7768 656e 206c 696d 6974  "Exit when limit
+000029a0: 7320 7265 6163 6865 643f 222c 0a20 2020  s reached?",.   
+000029b0: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
+000029c0: 7322 3a20 2222 2c0a 2020 2020 2020 2020  s": "",.        
+000029d0: 2020 2020 2020 2276 616c 7565 223a 2066        "value": f
+000029e0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+000029f0: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
+00002a00: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+00002a10: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00002a20: 223a 2022 5374 6f70 2074 6865 2077 686f  ": "Stop the who
+00002a30: 6c65 2065 7870 6572 696d 656e 7420 7768  le experiment wh
+00002a40: 656e 206c 696d 6974 2069 7320 7265 6163  en limit is reac
+00002a50: 6865 643f 222c 0a20 2020 2020 2020 2020  hed?",.         
+00002a60: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
+00002a70: 6c75 6522 3a20 6661 6c73 650a 2020 2020  lue": false.    
+00002a80: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00002a90: 2020 2020 2020 2022 7265 636f 7264 5f65         "record_e
+00002aa0: 7665 7279 5f64 4522 3a20 7b0a 2020 2020  very_dE": {.    
+00002ab0: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00002ac0: 223a 2022 5265 636f 7264 2065 7665 7279  ": "Record every
+00002ad0: 2024 6445 243a 222c 0a20 2020 2020 2020   $dE$:",.       
+00002ae0: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00002af0: 2256 222c 0a20 2020 2020 2020 2020 2020  "V",.           
+00002b00: 2020 2022 7661 6c75 6522 3a20 302e 312c     "value": 0.1,
+00002b10: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00002b20: 7265 7175 6972 6564 223a 2074 7275 652c  required": true,
+00002b30: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00002b40: 6465 7363 7269 7074 696f 6e22 3a20 2252  description": "R
+00002b50: 6563 6f72 6420 6120 6461 7461 706f 696e  ecord a datapoin
+00002b60: 7420 6174 2070 7265 7363 7269 6265 6420  t at prescribed 
+00002b70: 766f 6c74 6167 6520 7370 6163 696e 6722  voltage spacing"
+00002b80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002b90: 2264 6566 6175 6c74 5f76 616c 7565 223a  "default_value":
+00002ba0: 2030 2e30 3035 0a20 2020 2020 2020 2020   0.005.         
+00002bb0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00002bc0: 2020 2272 6563 6f72 645f 6576 6572 795f    "record_every_
+00002bd0: 6474 223a 207b 0a20 2020 2020 2020 2020  dt": {.         
+00002be0: 2020 2020 2022 6c61 6265 6c22 3a20 2252       "label": "R
+00002bf0: 6563 6f72 6420 6576 6572 7920 2464 7424  ecord every $dt$
+00002c00: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
+00002c10: 2020 2275 6e69 7473 223a 2022 7322 2c0a    "units": "s",.
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00002c30: 616c 7565 223a 2036 302e 302c 0a20 2020  alue": 60.0,.   
+00002c40: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
+00002c50: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
+00002c60: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00002c70: 7269 7074 696f 6e22 3a20 2252 6563 6f72  ription": "Recor
+00002c80: 6420 6120 6461 7461 706f 696e 7420 6174  d a datapoint at
+00002c90: 2070 7265 7363 7269 6265 6420 7469 6d65   prescribed time
+00002ca0: 2073 7061 6369 6e67 222c 0a20 2020 2020   spacing",.     
+00002cb0: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
+00002cc0: 745f 7661 6c75 6522 3a20 3330 2e30 0a20  t_value": 30.0. 
+00002cd0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00002ce0: 2020 2020 2020 2020 2020 226c 696d 6974            "limit
+00002cf0: 5f63 7572 7265 6e74 5f6d 6178 223a 207b  _current_max": {
+00002d00: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00002d10: 6c61 6265 6c22 3a20 224d 6178 696d 756d  label": "Maximum
+00002d20: 2063 7572 7265 6e74 3a22 2c0a 2020 2020   current:",.    
+00002d30: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+00002d40: 223a 2022 4922 2c0a 2020 2020 2020 2020  ": "I",.        
+00002d50: 2020 2020 2020 2276 616c 7565 223a 206e        "value": n
+00002d60: 756c 6c2c 0a20 2020 2020 2020 2020 2020  ull,.           
+00002d70: 2020 2022 7265 7175 6972 6564 223a 2066     "required": f
+00002d80: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00002d90: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00002da0: 223a 2022 4465 6669 6e65 2074 6865 2075  ": "Define the u
+00002db0: 7070 6572 206c 696d 6974 206f 6620 6375  pper limit of cu
+00002dc0: 7272 656e 7420 666f 7220 7468 6973 2073  rrent for this s
+00002dd0: 7465 7022 2c0a 2020 2020 2020 2020 2020  tep",.          
+00002de0: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
+00002df0: 7565 223a 206e 756c 6c0a 2020 2020 2020  ue": null.      
+00002e00: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00002e10: 2020 2020 2022 6c69 6d69 745f 6375 7272       "limit_curr
+00002e20: 656e 745f 6d69 6e22 3a20 7b0a 2020 2020  ent_min": {.    
+00002e30: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00002e40: 223a 2022 4d69 6e69 6d75 6d20 6375 7272  ": "Minimum curr
+00002e50: 656e 743a 222c 0a20 2020 2020 2020 2020  ent:",.         
+00002e60: 2020 2020 2022 756e 6974 7322 3a20 2249       "units": "I
+00002e70: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00002e80: 2022 7661 6c75 6522 3a20 6e75 6c6c 2c0a   "value": null,.
+00002e90: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00002ea0: 6571 7569 7265 6422 3a20 6661 6c73 652c  equired": false,
+00002eb0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00002ec0: 6465 7363 7269 7074 696f 6e22 3a20 2244  description": "D
+00002ed0: 6566 696e 6520 7468 6520 6c6f 7765 7220  efine the lower 
+00002ee0: 6c69 6d69 7420 6f66 2063 7572 7265 6e74  limit of current
+00002ef0: 2066 6f72 2074 6869 7320 7374 6570 222c   for this step",
+00002f00: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00002f10: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
+00002f20: 6e75 6c6c 0a20 2020 2020 2020 2020 2020  null.           
+00002f30: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00002f40: 226c 696d 6974 5f76 6f6c 7461 6765 5f6d  "limit_voltage_m
+00002f50: 6178 223a 207b 0a20 2020 2020 2020 2020  ax": {.         
+00002f60: 2020 2020 2022 6c61 6265 6c22 3a20 224d       "label": "M
+00002f70: 6178 696d 756d 2076 6f6c 7461 6765 3a22  aximum voltage:"
+00002f80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002f90: 2275 6e69 7473 223a 2022 5622 2c0a 2020  "units": "V",.  
+00002fa0: 2020 2020 2020 2020 2020 2020 2276 616c              "val
+00002fb0: 7565 223a 2032 2e35 2c0a 2020 2020 2020  ue": 2.5,.      
+00002fc0: 2020 2020 2020 2020 2272 6571 7569 7265          "require
+00002fd0: 6422 3a20 6661 6c73 652c 0a20 2020 2020  d": false,.     
+00002fe0: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00002ff0: 7074 696f 6e22 3a20 2244 6566 696e 6520  ption": "Define 
+00003000: 7468 6520 7570 7065 7220 6c69 6d69 7420  the upper limit 
+00003010: 6f66 2076 6f6c 7461 6765 2066 6f72 2074  of voltage for t
+00003020: 6869 7320 7374 6570 222c 0a20 2020 2020  his step",.     
+00003030: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
+00003040: 745f 7661 6c75 6522 3a20 6e75 6c6c 0a20  t_value": null. 
+00003050: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00003060: 2020 2020 2020 2020 2020 226c 696d 6974            "limit
+00003070: 5f76 6f6c 7461 6765 5f6d 696e 223a 207b  _voltage_min": {
+00003080: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00003090: 6c61 6265 6c22 3a20 224d 696e 696d 756d  label": "Minimum
+000030a0: 2076 6f6c 7461 6765 3a22 2c0a 2020 2020   voltage:",.    
+000030b0: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+000030c0: 223a 2022 5622 2c0a 2020 2020 2020 2020  ": "V",.        
+000030d0: 2020 2020 2020 2276 616c 7565 223a 2031        "value": 1
+000030e0: 2e35 2c0a 2020 2020 2020 2020 2020 2020  .5,.            
+000030f0: 2020 2272 6571 7569 7265 6422 3a20 6661    "required": fa
+00003100: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00003110: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00003120: 3a20 2244 6566 696e 6520 7468 6520 6c6f  : "Define the lo
+00003130: 7765 7220 6c69 6d69 7420 6f66 2076 6f6c  wer limit of vol
+00003140: 7461 6765 2066 6f72 2074 6869 7320 7374  tage for this st
+00003150: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
+00003160: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
+00003170: 6522 3a20 6e75 6c6c 0a20 2020 2020 2020  e": null.       
+00003180: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00003190: 207d 2c0a 2020 2020 2020 2020 2020 2273   },.          "s
+000031a0: 686f 7274 5f6e 616d 6522 3a20 2243 4322  hort_name": "CC"
+000031b0: 2c0a 2020 2020 2020 2020 2020 2264 6573  ,.          "des
+000031c0: 6372 6970 7469 6f6e 223a 2022 436f 6e74  cription": "Cont
+000031d0: 726f 6c6c 6564 2063 7572 7265 6e74 2074  rolled current t
+000031e0: 6563 686e 6971 7565 2c20 7769 7468 206f  echnique, with o
+000031f0: 7074 696f 6e61 6c20 766f 6c74 6167 6520  ptional voltage 
+00003200: 616e 6420 6375 7272 656e 7420 6c69 6d69  and current limi
+00003210: 7473 220a 2020 2020 2020 2020 7d2c 0a20  ts".        },. 
+00003220: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00003230: 2020 2022 6e61 6d65 223a 2022 4c4f 4f50     "name": "LOOP
+00003240: 5f31 222c 0a20 2020 2020 2020 2020 2022  _1",.          "
+00003250: 6465 7669 6365 223a 2022 4d50 4732 222c  device": "MPG2",
+00003260: 0a20 2020 2020 2020 2020 2022 7465 6368  .          "tech
+00003270: 6e69 7175 6522 3a20 226c 6f6f 7022 2c0a  nique": "loop",.
+00003280: 2020 2020 2020 2020 2020 2270 6172 616d            "param
+00003290: 6574 6572 7322 3a20 7b0a 2020 2020 2020  eters": {.      
+000032a0: 2020 2020 2020 2267 6f74 6f22 3a20 7b0a        "goto": {.
+000032b0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+000032c0: 6162 656c 223a 2022 476f 2074 6f3a 222c  abel": "Go to:",
+000032d0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000032e0: 756e 6974 7322 3a20 2222 2c0a 2020 2020  units": "",.    
+000032f0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+00003300: 223a 2031 2c0a 2020 2020 2020 2020 2020  ": 1,.          
+00003310: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
+00003320: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+00003330: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00003340: 223a 2022 496e 6465 7820 6f66 2074 6865  ": "Index of the
+00003350: 2074 6563 686e 6971 7565 2074 6f20 676f   technique to go
+00003360: 2062 6163 6b20 746f 222c 0a20 2020 2020   back to",.     
+00003370: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
+00003380: 745f 7661 6c75 6522 3a20 310a 2020 2020  t_value": 1.    
+00003390: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000033a0: 2020 2020 2020 2022 6e5f 676f 746f 7322         "n_gotos"
+000033b0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000033c0: 2020 226c 6162 656c 223a 2022 5265 7065    "label": "Repe
+000033d0: 6174 7322 2c0a 2020 2020 2020 2020 2020  ats",.          
+000033e0: 2020 2020 2275 6e69 7473 223a 2022 222c      "units": "",
+000033f0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00003400: 7661 6c75 6522 3a20 3130 302c 0a20 2020  value": 100,.   
+00003410: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
+00003420: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
+00003430: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00003440: 7269 7074 696f 6e22 3a20 224e 756d 6265  ription": "Numbe
+00003450: 7220 6f66 2074 696d 6573 2074 6865 2074  r of times the t
+00003460: 6563 686e 6971 7565 2077 696c 6c20 6a75  echnique will ju
+00003470: 6d70 3b20 7365 7420 746f 202d 3120 666f  mp; set to -1 fo
+00003480: 7220 756e 6c69 6d69 7465 6422 2c0a 2020  r unlimited",.  
+00003490: 2020 2020 2020 2020 2020 2020 2264 6566              "def
+000034a0: 6175 6c74 5f76 616c 7565 223a 202d 310a  ault_value": -1.
+000034b0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+000034c0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000034d0: 2020 2020 2022 7368 6f72 745f 6e61 6d65       "short_name
+000034e0: 223a 2022 4c4f 4f50 222c 0a20 2020 2020  ": "LOOP",.     
+000034f0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00003500: 6e22 3a20 224c 6f6f 7020 7465 6368 6e69  n": "Loop techni
+00003510: 7175 652c 2061 6c6c 6f77 696e 6720 746f  que, allowing to
+00003520: 2072 6570 6561 7420 6120 7365 7420 6f66   repeat a set of
+00003530: 2070 7265 6365 6469 6e67 2074 6563 686e   preceding techn
+00003540: 6971 7565 7320 696e 2061 2074 6563 686e  iques in a techn
+00003550: 6971 7565 2061 7272 6179 220a 2020 2020  ique array".    
+00003560: 2020 2020 7d0a 2020 2020 2020 5d0a 2020      }.      ].  
+00003570: 2020 7d2c 0a20 2020 2022 4445 4641 554c    },.    "DEFAUL
+00003580: 545f 5052 4f54 4543 5449 4f4e 5f4d 4554  T_PROTECTION_MET
+00003590: 484f 4422 3a20 7b0a 2020 2020 2020 226d  HOD": {.      "m
+000035a0: 6574 686f 6422 3a20 5b0a 2020 2020 2020  ethod": [.      
+000035b0: 2020 7b0a 2020 2020 2020 2020 2020 226e    {.          "n
+000035c0: 616d 6522 3a20 2243 435f 3122 2c0a 2020  ame": "CC_1",.  
+000035d0: 2020 2020 2020 2020 2264 6576 6963 6522          "device"
+000035e0: 3a20 224d 5047 3222 2c0a 2020 2020 2020  : "MPG2",.      
+000035f0: 2020 2020 2274 6563 686e 6971 7565 223a      "technique":
+00003600: 2022 636f 6e73 7461 6e74 5f63 7572 7265   "constant_curre
+00003610: 6e74 222c 0a20 2020 2020 2020 2020 2022  nt",.          "
+00003620: 7061 7261 6d65 7465 7273 223a 207b 0a20  parameters": {. 
+00003630: 2020 2020 2020 2020 2020 2022 7469 6d65             "time
+00003640: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00003650: 2020 2022 6c61 6265 6c22 3a20 2254 696d     "label": "Tim
+00003660: 653a 222c 0a20 2020 2020 2020 2020 2020  e:",.           
+00003670: 2020 2022 756e 6974 7322 3a20 2273 222c     "units": "s",
+00003680: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00003690: 7661 6c75 6522 3a20 3336 3030 2e30 2c0a  value": 3600.0,.
+000036a0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+000036b0: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
+000036c0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000036d0: 6573 6372 6970 7469 6f6e 223a 2022 4d61  escription": "Ma
+000036e0: 7869 6d75 6d20 6475 7261 7469 6f6e 206f  ximum duration o
+000036f0: 6620 7468 6520 4343 2073 7465 7022 2c0a  f the CC step",.
+00003700: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00003710: 6566 6175 6c74 5f76 616c 7565 223a 2030  efault_value": 0
+00003720: 2e30 0a20 2020 2020 2020 2020 2020 207d  .0.            }
+00003730: 2c0a 2020 2020 2020 2020 2020 2020 2245  ,.            "E
+00003740: 5f72 616e 6765 223a 207b 0a20 2020 2020  _range": {.     
+00003750: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00003760: 3a20 2245 2072 616e 6765 222c 0a20 2020  : "E range",.   
+00003770: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
+00003780: 7322 3a20 2222 2c0a 2020 2020 2020 2020  s": "",.        
+00003790: 2020 2020 2020 2276 616c 7565 223a 2022        "value": "
+000037a0: 2b2d 352e 3020 5622 2c0a 2020 2020 2020  +-5.0 V",.      
+000037b0: 2020 2020 2020 2020 2272 6571 7569 7265          "require
+000037c0: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
+000037d0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+000037e0: 7469 6f6e 223a 2022 5365 6c65 6374 2074  tion": "Select t
+000037f0: 6865 2076 6f6c 7461 6765 2072 616e 6765  he voltage range
+00003800: 206f 6620 7468 6520 706f 7465 6e74 696f   of the potentio
+00003810: 7374 6174 222c 0a20 2020 2020 2020 2020  stat",.         
+00003820: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
+00003830: 6c75 6522 3a20 2261 7574 6f22 0a20 2020  lue": "auto".   
+00003840: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00003850: 2020 2020 2020 2020 2249 5f72 616e 6765          "I_range
+00003860: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00003870: 2020 2022 6c61 6265 6c22 3a20 2249 2072     "label": "I r
+00003880: 616e 6765 222c 0a20 2020 2020 2020 2020  ange",.         
+00003890: 2020 2020 2022 756e 6974 7322 3a20 2222       "units": ""
+000038a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000038b0: 2276 616c 7565 223a 2022 3130 206d 4122  "value": "10 mA"
+000038c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000038d0: 2272 6571 7569 7265 6422 3a20 7472 7565  "required": true
+000038e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000038f0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00003900: 5365 6c65 6374 2074 6865 2063 7572 7265  Select the curre
+00003910: 6e74 2072 616e 6765 206f 6620 7468 6520  nt range of the 
+00003920: 706f 7465 6e74 696f 7374 6174 222c 0a20  potentiostat",. 
+00003930: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00003940: 6661 756c 745f 7661 6c75 6522 3a20 226b  fault_value": "k
+00003950: 6565 7022 0a20 2020 2020 2020 2020 2020  eep".           
+00003960: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00003970: 2263 7572 7265 6e74 223a 207b 0a20 2020  "current": {.   
+00003980: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
+00003990: 6c22 3a20 2253 7465 7020 6375 7272 656e  l": "Step curren
+000039a0: 743a 222c 0a20 2020 2020 2020 2020 2020  t:",.           
+000039b0: 2020 2022 756e 6974 7322 3a20 2249 222c     "units": "I",
+000039c0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000039d0: 7661 6c75 6522 3a20 2243 2f33 222c 0a20  value": "C/3",. 
+000039e0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+000039f0: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
+00003a00: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00003a10: 7363 7269 7074 696f 6e22 3a20 2243 7572  scription": "Cur
+00003a20: 7265 6e74 2064 7572 696e 6720 7468 6520  rent during the 
+00003a30: 6375 7272 656e 7420 7374 6570 222c 0a20  current step",. 
+00003a40: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00003a50: 6661 756c 745f 7661 6c75 6522 3a20 302e  fault_value": 0.
+00003a60: 300a 2020 2020 2020 2020 2020 2020 7d2c  0.            },
+00003a70: 0a20 2020 2020 2020 2020 2020 2022 6973  .            "is
+00003a80: 5f64 656c 7461 223a 207b 0a20 2020 2020  _delta": {.     
+00003a90: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00003aa0: 3a20 225c 7530 3339 3424 4924 3a22 2c0a  : "\u0394$I$:",.
+00003ab0: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+00003ac0: 6e69 7473 223a 2022 222c 0a20 2020 2020  nits": "",.     
+00003ad0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+00003ae0: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
+00003af0: 2020 2020 2020 2022 7265 7175 6972 6564         "required
+00003b00: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00003b10: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00003b20: 696f 6e22 3a20 2249 7320 7468 6520 7374  ion": "Is the st
+00003b30: 6570 2063 7572 7265 6e74 2061 2024 5c5c  ep current a $\\
+00003b40: 4465 6c74 6124 2066 726f 6d20 7072 6576  Delta$ from prev
+00003b50: 696f 7573 2073 7465 703f 222c 0a20 2020  ious step?",.   
+00003b60: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
+00003b70: 756c 745f 7661 6c75 6522 3a20 6661 6c73  ult_value": fals
+00003b80: 650a 2020 2020 2020 2020 2020 2020 7d2c  e.            },
+00003b90: 0a20 2020 2020 2020 2020 2020 2022 6e5f  .            "n_
+00003ba0: 6379 636c 6573 223a 207b 0a20 2020 2020  cycles": {.     
+00003bb0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00003bc0: 3a20 224e 756d 6265 7220 6f66 2063 7963  : "Number of cyc
+00003bd0: 6c65 733a 222c 0a20 2020 2020 2020 2020  les:",.         
+00003be0: 2020 2020 2022 756e 6974 7322 3a20 2222       "units": ""
+00003bf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003c00: 2276 616c 7565 223a 2030 2c0a 2020 2020  "value": 0,.    
+00003c10: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
+00003c20: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
+00003c30: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00003c40: 6970 7469 6f6e 223a 2022 4379 636c 6520  iption": "Cycle 
+00003c50: 7468 726f 7567 6820 7468 6520 6375 7272  through the curr
+00003c60: 656e 7420 7465 6368 6e69 7175 6520 4e20  ent technique N 
+00003c70: 7469 6d65 732e 222c 0a20 2020 2020 2020  times.",.       
+00003c80: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
+00003c90: 7661 6c75 6522 3a20 300a 2020 2020 2020  value": 0.      
+00003ca0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00003cb0: 2020 2020 2022 6578 6974 5f6f 6e5f 6c69       "exit_on_li
+00003cc0: 6d69 7422 3a20 7b0a 2020 2020 2020 2020  mit": {.        
+00003cd0: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00003ce0: 4578 6974 2077 6865 6e20 6c69 6d69 7473  Exit when limits
+00003cf0: 2072 6561 6368 6564 3f22 2c0a 2020 2020   reached?",.    
+00003d00: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+00003d10: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
+00003d20: 2020 2020 2022 7661 6c75 6522 3a20 6661       "value": fa
+00003d30: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00003d40: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
+00003d50: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00003d60: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00003d70: 3a20 2253 746f 7020 7468 6520 7768 6f6c  : "Stop the whol
+00003d80: 6520 6578 7065 7269 6d65 6e74 2077 6865  e experiment whe
+00003d90: 6e20 6c69 6d69 7420 6973 2072 6561 6368  n limit is reach
+00003da0: 6564 3f22 2c0a 2020 2020 2020 2020 2020  ed?",.          
+00003db0: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
+00003dc0: 7565 223a 2066 616c 7365 0a20 2020 2020  ue": false.     
+00003dd0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00003de0: 2020 2020 2020 2272 6563 6f72 645f 6576        "record_ev
+00003df0: 6572 795f 6445 223a 207b 0a20 2020 2020  ery_dE": {.     
+00003e00: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00003e10: 3a20 2252 6563 6f72 6420 6576 6572 7920  : "Record every 
+00003e20: 2464 4524 3a22 2c0a 2020 2020 2020 2020  $dE$:",.        
+00003e30: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
+00003e40: 5622 2c0a 2020 2020 2020 2020 2020 2020  V",.            
+00003e50: 2020 2276 616c 7565 223a 2030 2e31 2c0a    "value": 0.1,.
+00003e60: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00003e70: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
+00003e80: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00003e90: 6573 6372 6970 7469 6f6e 223a 2022 5265  escription": "Re
+00003ea0: 636f 7264 2061 2064 6174 6170 6f69 6e74  cord a datapoint
+00003eb0: 2061 7420 7072 6573 6372 6962 6564 2076   at prescribed v
+00003ec0: 6f6c 7461 6765 2073 7061 6369 6e67 222c  oltage spacing",
+00003ed0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00003ee0: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
+00003ef0: 302e 3030 350a 2020 2020 2020 2020 2020  0.005.          
+00003f00: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00003f10: 2022 7265 636f 7264 5f65 7665 7279 5f64   "record_every_d
+00003f20: 7422 3a20 7b0a 2020 2020 2020 2020 2020  t": {.          
+00003f30: 2020 2020 226c 6162 656c 223a 2022 5265      "label": "Re
+00003f40: 636f 7264 2065 7665 7279 2024 6474 243a  cord every $dt$:
+00003f50: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003f60: 2022 756e 6974 7322 3a20 2273 222c 0a20   "units": "s",. 
+00003f70: 2020 2020 2020 2020 2020 2020 2022 7661               "va
+00003f80: 6c75 6522 3a20 3330 2e30 2c0a 2020 2020  lue": 30.0,.    
+00003f90: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
+00003fa0: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
+00003fb0: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00003fc0: 6970 7469 6f6e 223a 2022 5265 636f 7264  iption": "Record
+00003fd0: 2061 2064 6174 6170 6f69 6e74 2061 7420   a datapoint at 
+00003fe0: 7072 6573 6372 6962 6564 2074 696d 6520  prescribed time 
+00003ff0: 7370 6163 696e 6722 2c0a 2020 2020 2020  spacing",.      
+00004000: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+00004010: 5f76 616c 7565 223a 2033 302e 300a 2020  _value": 30.0.  
+00004020: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00004030: 2020 2020 2020 2020 2022 6c69 6d69 745f           "limit_
+00004040: 6375 7272 656e 745f 6d61 7822 3a20 7b0a  current_max": {.
+00004050: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00004060: 6162 656c 223a 2022 4d61 7869 6d75 6d20  abel": "Maximum 
+00004070: 6375 7272 656e 743a 222c 0a20 2020 2020  current:",.     
+00004080: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+00004090: 3a20 2249 222c 0a20 2020 2020 2020 2020  : "I",.         
+000040a0: 2020 2020 2022 7661 6c75 6522 3a20 6e75       "value": nu
+000040b0: 6c6c 2c0a 2020 2020 2020 2020 2020 2020  ll,.            
+000040c0: 2020 2272 6571 7569 7265 6422 3a20 6661    "required": fa
+000040d0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+000040e0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+000040f0: 3a20 2244 6566 696e 6520 7468 6520 7570  : "Define the up
+00004100: 7065 7220 6c69 6d69 7420 6f66 2063 7572  per limit of cur
+00004110: 7265 6e74 2066 6f72 2074 6869 7320 7374  rent for this st
+00004120: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
+00004130: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
+00004140: 6522 3a20 6e75 6c6c 0a20 2020 2020 2020  e": null.       
+00004150: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00004160: 2020 2020 226c 696d 6974 5f63 7572 7265      "limit_curre
+00004170: 6e74 5f6d 696e 223a 207b 0a20 2020 2020  nt_min": {.     
+00004180: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00004190: 3a20 224d 696e 696d 756d 2063 7572 7265  : "Minimum curre
+000041a0: 6e74 3a22 2c0a 2020 2020 2020 2020 2020  nt:",.          
+000041b0: 2020 2020 2275 6e69 7473 223a 2022 4922      "units": "I"
+000041c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000041d0: 2276 616c 7565 223a 206e 756c 6c2c 0a20  "value": null,. 
+000041e0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+000041f0: 7175 6972 6564 223a 2066 616c 7365 2c0a  quired": false,.
+00004200: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00004210: 6573 6372 6970 7469 6f6e 223a 2022 4465  escription": "De
+00004220: 6669 6e65 2074 6865 206c 6f77 6572 206c  fine the lower l
+00004230: 696d 6974 206f 6620 6375 7272 656e 7420  imit of current 
+00004240: 666f 7220 7468 6973 2073 7465 7022 2c0a  for this step",.
+00004250: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00004260: 6566 6175 6c74 5f76 616c 7565 223a 206e  efault_value": n
+00004270: 756c 6c0a 2020 2020 2020 2020 2020 2020  ull.            
+00004280: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+00004290: 6c69 6d69 745f 766f 6c74 6167 655f 6d61  limit_voltage_ma
+000042a0: 7822 3a20 7b0a 2020 2020 2020 2020 2020  x": {.          
+000042b0: 2020 2020 226c 6162 656c 223a 2022 4d61      "label": "Ma
+000042c0: 7869 6d75 6d20 766f 6c74 6167 653a 222c  ximum voltage:",
+000042d0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000042e0: 756e 6974 7322 3a20 2256 222c 0a20 2020  units": "V",.   
+000042f0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00004300: 6522 3a20 312e 352c 0a20 2020 2020 2020  e": 1.5,.       
+00004310: 2020 2020 2020 2022 7265 7175 6972 6564         "required
+00004320: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
+00004330: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00004340: 7469 6f6e 223a 2022 4465 6669 6e65 2074  tion": "Define t
+00004350: 6865 2075 7070 6572 206c 696d 6974 206f  he upper limit o
+00004360: 6620 766f 6c74 6167 6520 666f 7220 7468  f voltage for th
+00004370: 6973 2073 7465 7022 2c0a 2020 2020 2020  is step",.      
+00004380: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+00004390: 5f76 616c 7565 223a 206e 756c 6c0a 2020  _value": null.  
+000043a0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+000043b0: 2020 2020 2020 2020 2022 6c69 6d69 745f           "limit_
+000043c0: 766f 6c74 6167 655f 6d69 6e22 3a20 7b0a  voltage_min": {.
+000043d0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+000043e0: 6162 656c 223a 2022 4d69 6e69 6d75 6d20  abel": "Minimum 
+000043f0: 766f 6c74 6167 653a 222c 0a20 2020 2020  voltage:",.     
+00004400: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+00004410: 3a20 2256 222c 0a20 2020 2020 2020 2020  : "V",.         
+00004420: 2020 2020 2022 7661 6c75 6522 3a20 302e       "value": 0.
+00004430: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00004440: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
+00004450: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00004460: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00004470: 2022 4465 6669 6e65 2074 6865 206c 6f77   "Define the low
+00004480: 6572 206c 696d 6974 206f 6620 766f 6c74  er limit of volt
+00004490: 6167 6520 666f 7220 7468 6973 2073 7465  age for this ste
+000044a0: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
+000044b0: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
+000044c0: 223a 206e 756c 6c0a 2020 2020 2020 2020  ": null.        
+000044d0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+000044e0: 7d2c 0a20 2020 2020 2020 2020 2022 7368  },.          "sh
+000044f0: 6f72 745f 6e61 6d65 223a 2022 4343 222c  ort_name": "CC",
+00004500: 0a20 2020 2020 2020 2020 2022 6465 7363  .          "desc
+00004510: 7269 7074 696f 6e22 3a20 2243 6f6e 7472  ription": "Contr
+00004520: 6f6c 6c65 6420 6375 7272 656e 7420 7465  olled current te
+00004530: 6368 6e69 7175 652c 2077 6974 6820 6f70  chnique, with op
+00004540: 7469 6f6e 616c 2076 6f6c 7461 6765 2061  tional voltage a
+00004550: 6e64 2063 7572 7265 6e74 206c 696d 6974  nd current limit
+00004560: 7322 0a20 2020 2020 2020 207d 2c0a 2020  s".        },.  
+00004570: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00004580: 2020 226e 616d 6522 3a20 2243 565f 3122    "name": "CV_1"
+00004590: 2c0a 2020 2020 2020 2020 2020 2264 6576  ,.          "dev
+000045a0: 6963 6522 3a20 224d 5047 3222 2c0a 2020  ice": "MPG2",.  
+000045b0: 2020 2020 2020 2020 2274 6563 686e 6971          "techniq
+000045c0: 7565 223a 2022 636f 6e73 7461 6e74 5f76  ue": "constant_v
+000045d0: 6f6c 7461 6765 222c 0a20 2020 2020 2020  oltage",.       
+000045e0: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
+000045f0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00004600: 7469 6d65 223a 207b 0a20 2020 2020 2020  time": {.       
+00004610: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00004620: 2254 696d 653a 222c 0a20 2020 2020 2020  "Time:",.       
+00004630: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00004640: 2273 222c 0a20 2020 2020 2020 2020 2020  "s",.           
+00004650: 2020 2022 7661 6c75 6522 3a20 3930 302e     "value": 900.
+00004660: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00004670: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
+00004680: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00004690: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+000046a0: 224d 6178 696d 756d 2064 7572 6174 696f  "Maximum duratio
+000046b0: 6e20 6f66 2074 6865 2043 5620 7374 6570  n of the CV step
+000046c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000046d0: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
+000046e0: 3a20 302e 300a 2020 2020 2020 2020 2020  : 0.0.          
+000046f0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00004700: 2022 455f 7261 6e67 6522 3a20 7b0a 2020   "E_range": {.  
+00004710: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
+00004720: 656c 223a 2022 4520 7261 6e67 6522 2c0a  el": "E range",.
+00004730: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+00004740: 6e69 7473 223a 2022 222c 0a20 2020 2020  nits": "",.     
+00004750: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+00004760: 3a20 222b 2d35 2e30 2056 222c 0a20 2020  : "+-5.0 V",.   
+00004770: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
+00004780: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
+00004790: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000047a0: 7269 7074 696f 6e22 3a20 2253 656c 6563  ription": "Selec
+000047b0: 7420 7468 6520 766f 6c74 6167 6520 7261  t the voltage ra
+000047c0: 6e67 6520 6f66 2074 6865 2070 6f74 656e  nge of the poten
+000047d0: 7469 6f73 7461 7422 2c0a 2020 2020 2020  tiostat",.      
+000047e0: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+000047f0: 5f76 616c 7565 223a 2022 6175 746f 220a  _value": "auto".
+00004800: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00004810: 2020 2020 2020 2020 2020 2022 495f 7261             "I_ra
+00004820: 6e67 6522 3a20 7b0a 2020 2020 2020 2020  nge": {.        
+00004830: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00004840: 4920 7261 6e67 6522 2c0a 2020 2020 2020  I range",.      
+00004850: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
+00004860: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
+00004870: 2020 2022 7661 6c75 6522 3a20 2231 3020     "value": "10 
+00004880: 6d41 222c 0a20 2020 2020 2020 2020 2020  mA",.           
+00004890: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
+000048a0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+000048b0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+000048c0: 3a20 2253 656c 6563 7420 7468 6520 6375  : "Select the cu
+000048d0: 7272 656e 7420 7261 6e67 6520 6f66 2074  rrent range of t
+000048e0: 6865 2070 6f74 656e 7469 6f73 7461 7422  he potentiostat"
+000048f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004900: 2264 6566 6175 6c74 5f76 616c 7565 223a  "default_value":
+00004910: 2022 6b65 6570 220a 2020 2020 2020 2020   "keep".        
+00004920: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00004930: 2020 2022 766f 6c74 6167 6522 3a20 7b0a     "voltage": {.
+00004940: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00004950: 6162 656c 223a 2022 5374 6570 2076 6f6c  abel": "Step vol
+00004960: 7461 6765 3a22 2c0a 2020 2020 2020 2020  tage:",.        
+00004970: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
+00004980: 5622 2c0a 2020 2020 2020 2020 2020 2020  V",.            
+00004990: 2020 2276 616c 7565 223a 2031 2e35 2c0a    "value": 1.5,.
+000049a0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+000049b0: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
+000049c0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000049d0: 6573 6372 6970 7469 6f6e 223a 2022 566f  escription": "Vo
+000049e0: 6c74 6167 6520 6f66 2074 6865 2063 7572  ltage of the cur
+000049f0: 7265 6e74 2073 7465 7022 2c0a 2020 2020  rent step",.    
+00004a00: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
+00004a10: 6c74 5f76 616c 7565 223a 2030 2e30 0a20  lt_value": 0.0. 
+00004a20: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00004a30: 2020 2020 2020 2020 2020 2269 735f 6465            "is_de
+00004a40: 6c74 6122 3a20 7b0a 2020 2020 2020 2020  lta": {.        
+00004a50: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00004a60: 5c75 3033 3934 2456 243a 222c 0a20 2020  \u0394$V$:",.   
+00004a70: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
+00004a80: 7322 3a20 2222 2c0a 2020 2020 2020 2020  s": "",.        
+00004a90: 2020 2020 2020 2276 616c 7565 223a 2066        "value": f
+00004aa0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00004ab0: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
+00004ac0: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+00004ad0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00004ae0: 223a 2022 4973 2074 6865 2073 7465 7020  ": "Is the step 
+00004af0: 766f 6c74 6167 6520 6120 245c 5c44 656c  voltage a $\\Del
+00004b00: 7461 2420 6672 6f6d 2070 7265 7669 6f75  ta$ from previou
+00004b10: 7320 7374 6570 3f22 2c0a 2020 2020 2020  s step?",.      
+00004b20: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+00004b30: 5f76 616c 7565 223a 2066 616c 7365 0a20  _value": false. 
+00004b40: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00004b50: 2020 2020 2020 2020 2020 226e 5f63 7963            "n_cyc
+00004b60: 6c65 7322 3a20 7b0a 2020 2020 2020 2020  les": {.        
+00004b70: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00004b80: 4e75 6d62 6572 206f 6620 6379 636c 6573  Number of cycles
+00004b90: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
+00004ba0: 2020 2275 6e69 7473 223a 2022 222c 0a20    "units": "",. 
+00004bb0: 2020 2020 2020 2020 2020 2020 2022 7661               "va
+00004bc0: 6c75 6522 3a20 302c 0a20 2020 2020 2020  lue": 0,.       
+00004bd0: 2020 2020 2020 2022 7265 7175 6972 6564         "required
+00004be0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00004bf0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00004c00: 696f 6e22 3a20 2243 7963 6c65 2074 6872  ion": "Cycle thr
+00004c10: 6f75 6768 2074 6865 2063 7572 7265 6e74  ough the current
+00004c20: 2074 6563 686e 6971 7565 204e 2074 696d   technique N tim
+00004c30: 6573 2e22 2c0a 2020 2020 2020 2020 2020  es.",.          
+00004c40: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
+00004c50: 7565 223a 2030 0a20 2020 2020 2020 2020  ue": 0.         
+00004c60: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00004c70: 2020 2265 7869 745f 6f6e 5f6c 696d 6974    "exit_on_limit
+00004c80: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00004c90: 2020 2022 6c61 6265 6c22 3a20 2245 7869     "label": "Exi
+00004ca0: 7420 7768 656e 206c 696d 6974 7320 7265  t when limits re
+00004cb0: 6163 6865 643f 222c 0a20 2020 2020 2020  ached?",.       
+00004cc0: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00004cd0: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+00004ce0: 2020 2276 616c 7565 223a 2066 616c 7365    "value": false
+00004cf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004d00: 2272 6571 7569 7265 6422 3a20 7472 7565  "required": true
+00004d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004d20: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00004d30: 5374 6f70 2074 6865 2077 686f 6c65 2065  Stop the whole e
+00004d40: 7870 6572 696d 656e 7420 7768 656e 206c  xperiment when l
+00004d50: 696d 6974 2069 7320 7265 6163 6865 643f  imit is reached?
+00004d60: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00004d70: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
+00004d80: 3a20 6661 6c73 650a 2020 2020 2020 2020  : false.        
+00004d90: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00004da0: 2020 2022 7265 636f 7264 5f65 7665 7279     "record_every
+00004db0: 5f64 4922 3a20 7b0a 2020 2020 2020 2020  _dI": {.        
+00004dc0: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00004dd0: 5265 636f 7264 2065 7665 7279 2024 6449  Record every $dI
+00004de0: 243a 222c 0a20 2020 2020 2020 2020 2020  $:",.           
+00004df0: 2020 2022 756e 6974 7322 3a20 2249 222c     "units": "I",
+00004e00: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00004e10: 7661 6c75 6522 3a20 302e 312c 0a20 2020  value": 0.1,.   
+00004e20: 2020 2020 2020 2020 2020 2022 7265 7175             "requ
+00004e30: 6972 6564 223a 2074 7275 652c 0a20 2020  ired": true,.   
+00004e40: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+00004e50: 7269 7074 696f 6e22 3a20 2252 6563 6f72  ription": "Recor
+00004e60: 6420 6120 6461 7461 706f 696e 7420 6174  d a datapoint at
+00004e70: 2070 7265 7363 7269 6265 6420 6375 7272   prescribed curr
+00004e80: 656e 7420 7370 6163 696e 6722 2c0a 2020  ent spacing",.  
+00004e90: 2020 2020 2020 2020 2020 2020 2264 6566              "def
+00004ea0: 6175 6c74 5f76 616c 7565 223a 2030 2e30  ault_value": 0.0
+00004eb0: 3031 0a20 2020 2020 2020 2020 2020 207d  01.            }
+00004ec0: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
+00004ed0: 6563 6f72 645f 6576 6572 795f 6474 223a  ecord_every_dt":
+00004ee0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00004ef0: 2022 6c61 6265 6c22 3a20 2252 6563 6f72   "label": "Recor
+00004f00: 6420 6576 6572 7920 2464 7424 3a22 2c0a  d every $dt$:",.
+00004f10: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+00004f20: 6e69 7473 223a 2022 7322 2c0a 2020 2020  nits": "s",.    
+00004f30: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+00004f40: 223a 2033 302e 302c 0a20 2020 2020 2020  ": 30.0,.       
+00004f50: 2020 2020 2020 2022 7265 7175 6972 6564         "required
+00004f60: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00004f70: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00004f80: 696f 6e22 3a20 2252 6563 6f72 6420 6120  ion": "Record a 
+00004f90: 6461 7461 706f 696e 7420 6174 2070 7265  datapoint at pre
+00004fa0: 7363 7269 6265 6420 7469 6d65 2073 7061  scribed time spa
+00004fb0: 6369 6e67 222c 0a20 2020 2020 2020 2020  cing",.         
+00004fc0: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
+00004fd0: 6c75 6522 3a20 3330 2e30 0a20 2020 2020  lue": 30.0.     
+00004fe0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00004ff0: 2020 2020 2020 226c 696d 6974 5f63 7572        "limit_cur
+00005000: 7265 6e74 5f6d 6178 223a 207b 0a20 2020  rent_max": {.   
+00005010: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
+00005020: 6c22 3a20 224d 6178 696d 756d 2063 7572  l": "Maximum cur
+00005030: 7265 6e74 3a22 2c0a 2020 2020 2020 2020  rent:",.        
+00005040: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
+00005050: 4922 2c0a 2020 2020 2020 2020 2020 2020  I",.            
+00005060: 2020 2276 616c 7565 223a 206e 756c 6c2c    "value": null,
+00005070: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00005080: 7265 7175 6972 6564 223a 2066 616c 7365  required": false
+00005090: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000050a0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+000050b0: 4465 6669 6e65 2074 6865 2075 7070 6572  Define the upper
+000050c0: 206c 696d 6974 206f 6620 6375 7272 656e   limit of curren
+000050d0: 7420 666f 7220 7468 6973 2073 7465 7022  t for this step"
+000050e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000050f0: 2264 6566 6175 6c74 5f76 616c 7565 223a  "default_value":
+00005100: 206e 756c 6c0a 2020 2020 2020 2020 2020   null.          
+00005110: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00005120: 2022 6c69 6d69 745f 6375 7272 656e 745f   "limit_current_
+00005130: 6d69 6e22 3a20 7b0a 2020 2020 2020 2020  min": {.        
+00005140: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+00005150: 4d69 6e69 6d75 6d20 6375 7272 656e 743a  Minimum current:
+00005160: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00005170: 2022 756e 6974 7322 3a20 2249 222c 0a20   "units": "I",. 
+00005180: 2020 2020 2020 2020 2020 2020 2022 7661               "va
+00005190: 6c75 6522 3a20 6e75 6c6c 2c0a 2020 2020  lue": null,.    
+000051a0: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
+000051b0: 7265 6422 3a20 6661 6c73 652c 0a20 2020  red": false,.   
+000051c0: 2020 2020 2020 2020 2020 2022 6465 7363             "desc
+000051d0: 7269 7074 696f 6e22 3a20 2244 6566 696e  ription": "Defin
+000051e0: 6520 7468 6520 6c6f 7765 7220 6c69 6d69  e the lower limi
+000051f0: 7420 6f66 2063 7572 7265 6e74 2066 6f72  t of current for
+00005200: 2074 6869 7320 7374 6570 222c 0a20 2020   this step",.   
+00005210: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
+00005220: 756c 745f 7661 6c75 6522 3a20 6e75 6c6c  ult_value": null
+00005230: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00005240: 2020 2020 2020 2020 2020 2020 226c 696d              "lim
+00005250: 6974 5f76 6f6c 7461 6765 5f6d 6178 223a  it_voltage_max":
+00005260: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00005270: 2022 6c61 6265 6c22 3a20 224d 6178 696d   "label": "Maxim
+00005280: 756d 2076 6f6c 7461 6765 3a22 2c0a 2020  um voltage:",.  
+00005290: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
+000052a0: 7473 223a 2022 5622 2c0a 2020 2020 2020  ts": "V",.      
+000052b0: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
+000052c0: 2031 2e35 2c0a 2020 2020 2020 2020 2020   1.5,.          
+000052d0: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
+000052e0: 6661 6c73 652c 0a20 2020 2020 2020 2020  false,.         
+000052f0: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00005300: 6e22 3a20 2244 6566 696e 6520 7468 6520  n": "Define the 
+00005310: 7570 7065 7220 6c69 6d69 7420 6f66 2076  upper limit of v
+00005320: 6f6c 7461 6765 2066 6f72 2074 6869 7320  oltage for this 
+00005330: 7374 6570 222c 0a20 2020 2020 2020 2020  step",.         
+00005340: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
+00005350: 6c75 6522 3a20 6e75 6c6c 0a20 2020 2020  lue": null.     
+00005360: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00005370: 2020 2020 2020 226c 696d 6974 5f76 6f6c        "limit_vol
+00005380: 7461 6765 5f6d 696e 223a 207b 0a20 2020  tage_min": {.   
+00005390: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
+000053a0: 6c22 3a20 224d 696e 696d 756d 2076 6f6c  l": "Minimum vol
+000053b0: 7461 6765 3a22 2c0a 2020 2020 2020 2020  tage:",.        
+000053c0: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
+000053d0: 5622 2c0a 2020 2020 2020 2020 2020 2020  V",.            
+000053e0: 2020 2276 616c 7565 223a 2030 2e30 2c0a    "value": 0.0,.
+000053f0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00005400: 6571 7569 7265 6422 3a20 6661 6c73 652c  equired": false,
+00005410: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00005420: 6465 7363 7269 7074 696f 6e22 3a20 2244  description": "D
+00005430: 6566 696e 6520 7468 6520 6c6f 7765 7220  efine the lower 
+00005440: 6c69 6d69 7420 6f66 2076 6f6c 7461 6765  limit of voltage
+00005450: 2066 6f72 2074 6869 7320 7374 6570 222c   for this step",
+00005460: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00005470: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
+00005480: 6e75 6c6c 0a20 2020 2020 2020 2020 2020  null.           
+00005490: 207d 0a20 2020 2020 2020 2020 207d 2c0a   }.          },.
+000054a0: 2020 2020 2020 2020 2020 2273 686f 7274            "short
+000054b0: 5f6e 616d 6522 3a20 2243 5622 2c0a 2020  _name": "CV",.  
+000054c0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+000054d0: 7469 6f6e 223a 2022 436f 6e74 726f 6c6c  tion": "Controll
+000054e0: 6564 2076 6f6c 7461 6765 2074 6563 686e  ed voltage techn
+000054f0: 6971 7565 2c20 7769 7468 206f 7074 696f  ique, with optio
+00005500: 6e61 6c20 6375 7272 656e 7420 616e 6420  nal current and 
+00005510: 766f 6c74 6167 6520 6c69 6d69 7473 220a  voltage limits".
+00005520: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00005530: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00005540: 6e61 6d65 223a 2022 4f43 565f 3122 2c0a  name": "OCV_1",.
+00005550: 2020 2020 2020 2020 2020 2264 6576 6963            "devic
+00005560: 6522 3a20 224d 5047 3222 2c0a 2020 2020  e": "MPG2",.    
+00005570: 2020 2020 2020 2274 6563 686e 6971 7565        "technique
+00005580: 223a 2022 6f70 656e 5f63 6972 6375 6974  ": "open_circuit
+00005590: 5f76 6f6c 7461 6765 222c 0a20 2020 2020  _voltage",.     
+000055a0: 2020 2020 2022 7061 7261 6d65 7465 7273       "parameters
+000055b0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+000055c0: 2022 7469 6d65 223a 207b 0a20 2020 2020   "time": {.     
+000055d0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+000055e0: 3a20 2254 696d 653a 222c 0a20 2020 2020  : "Time:",.     
+000055f0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+00005600: 3a20 2273 222c 0a20 2020 2020 2020 2020  : "s",.         
+00005610: 2020 2020 2022 7661 6c75 6522 3a20 3231       "value": 21
+00005620: 3630 302e 302c 0a20 2020 2020 2020 2020  600.0,.         
+00005630: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
+00005640: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
+00005650: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00005660: 6e22 3a20 2254 6865 206c 656e 6774 6820  n": "The length 
+00005670: 6f66 2074 6865 204f 4356 2073 7465 7022  of the OCV step"
+00005680: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005690: 2264 6566 6175 6c74 5f76 616c 7565 223a  "default_value":
+000056a0: 2030 2e30 0a20 2020 2020 2020 2020 2020   0.0.           
+000056b0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+000056c0: 2245 5f72 616e 6765 223a 207b 0a20 2020  "E_range": {.   
+000056d0: 2020 2020 2020 2020 2020 2022 6c61 6265             "labe
+000056e0: 6c22 3a20 2245 2072 616e 6765 222c 0a20  l": "E range",. 
+000056f0: 2020 2020 2020 2020 2020 2020 2022 756e               "un
+00005700: 6974 7322 3a20 2222 2c0a 2020 2020 2020  its": "",.      
+00005710: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
+00005720: 2022 2b2d 352e 3020 5622 2c0a 2020 2020   "+-5.0 V",.    
+00005730: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
+00005740: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
+00005750: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00005760: 6970 7469 6f6e 223a 2022 222c 0a20 2020  iption": "",.   
+00005770: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
+00005780: 756c 745f 7661 6c75 6522 3a20 2261 7574  ult_value": "aut
+00005790: 6f22 0a20 2020 2020 2020 2020 2020 207d  o".            }
+000057a0: 2c0a 2020 2020 2020 2020 2020 2020 2249  ,.            "I
+000057b0: 5f72 616e 6765 223a 207b 0a20 2020 2020  _range": {.     
+000057c0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+000057d0: 3a20 2249 2072 616e 6765 222c 0a20 2020  : "I range",.   
+000057e0: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
+000057f0: 7322 3a20 2222 2c0a 2020 2020 2020 2020  s": "",.        
+00005800: 2020 2020 2020 2276 616c 7565 223a 2022        "value": "
+00005810: 3130 206d 4122 2c0a 2020 2020 2020 2020  10 mA",.        
+00005820: 2020 2020 2020 2272 6571 7569 7265 6422        "required"
+00005830: 3a20 7472 7565 2c0a 2020 2020 2020 2020  : true,.        
+00005840: 2020 2020 2020 2264 6573 6372 6970 7469        "descripti
+00005850: 6f6e 223a 2022 222c 0a20 2020 2020 2020  on": "",.       
+00005860: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
+00005870: 7661 6c75 6522 3a20 2231 2041 220a 2020  value": "1 A".  
+00005880: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00005890: 2020 2020 2020 2020 2022 7265 636f 7264           "record
+000058a0: 5f65 7665 7279 5f64 4522 3a20 7b0a 2020  _every_dE": {.  
+000058b0: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
+000058c0: 656c 223a 2022 5265 636f 7264 2065 7665  el": "Record eve
+000058d0: 7279 2024 6445 243a 222c 0a20 2020 2020  ry $dE$:",.     
+000058e0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+000058f0: 3a20 2256 222c 0a20 2020 2020 2020 2020  : "V",.         
+00005900: 2020 2020 2022 7661 6c75 6522 3a20 302e       "value": 0.
+00005910: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+00005920: 2022 7265 7175 6972 6564 223a 2074 7275   "required": tru
+00005930: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00005940: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00005950: 2252 6563 6f72 6420 6120 6461 7461 706f  "Record a datapo
+00005960: 696e 7420 6174 2070 7265 7363 7269 6265  int at prescribe
+00005970: 6420 766f 6c74 6167 6520 7370 6163 696e  d voltage spacin
+00005980: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
+00005990: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
+000059a0: 223a 2030 2e30 3035 0a20 2020 2020 2020  ": 0.005.       
+000059b0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000059c0: 2020 2020 2272 6563 6f72 645f 6576 6572      "record_ever
+000059d0: 795f 6474 223a 207b 0a20 2020 2020 2020  y_dt": {.       
+000059e0: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+000059f0: 2252 6563 6f72 6420 6576 6572 7920 2464  "Record every $d
+00005a00: 7424 3a22 2c0a 2020 2020 2020 2020 2020  t$:",.          
+00005a10: 2020 2020 2275 6e69 7473 223a 2022 7322      "units": "s"
+00005a20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005a30: 2276 616c 7565 223a 2033 302e 302c 0a20  "value": 30.0,. 
+00005a40: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00005a50: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
+00005a60: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00005a70: 7363 7269 7074 696f 6e22 3a20 2252 6563  scription": "Rec
+00005a80: 6f72 6420 6120 6461 7461 706f 696e 7420  ord a datapoint 
+00005a90: 6174 2070 7265 7363 7269 6265 6420 7469  at prescribed ti
+00005aa0: 6d65 2073 7061 6369 6e67 222c 0a20 2020  me spacing",.   
+00005ab0: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
+00005ac0: 756c 745f 7661 6c75 6522 3a20 3330 2e30  ult_value": 30.0
+00005ad0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+00005ae0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00005af0: 2020 2020 2020 2273 686f 7274 5f6e 616d        "short_nam
+00005b00: 6522 3a20 224f 4356 222c 0a20 2020 2020  e": "OCV",.     
+00005b10: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00005b20: 6e22 3a20 224f 7065 6e20 6369 7263 7569  n": "Open circui
+00005b30: 7420 766f 6c74 6167 6522 0a20 2020 2020  t voltage".     
+00005b40: 2020 207d 0a20 2020 2020 205d 0a20 2020     }.      ].   
+00005b50: 207d 2c0a 2020 2020 2244 4546 4155 4c54   },.    "DEFAULT
+00005b60: 5f46 4f52 4d41 5449 4f4e 5f4d 4554 484f  _FORMATION_METHO
+00005b70: 4422 3a20 7b0a 2020 2020 2020 226d 6574  D": {.      "met
+00005b80: 686f 6422 3a20 5b0a 2020 2020 2020 2020  hod": [.        
+00005b90: 7b0a 2020 2020 2020 2020 2020 226e 616d  {.          "nam
+00005ba0: 6522 3a20 2243 435f 3122 2c0a 2020 2020  e": "CC_1",.    
+00005bb0: 2020 2020 2020 2264 6576 6963 6522 3a20        "device": 
+00005bc0: 224d 5047 3222 2c0a 2020 2020 2020 2020  "MPG2",.        
+00005bd0: 2020 2274 6563 686e 6971 7565 223a 2022    "technique": "
+00005be0: 636f 6e73 7461 6e74 5f63 7572 7265 6e74  constant_current
+00005bf0: 222c 0a20 2020 2020 2020 2020 2022 7061  ",.          "pa
+00005c00: 7261 6d65 7465 7273 223a 207b 0a20 2020  rameters": {.   
+00005c10: 2020 2020 2020 2020 2022 7469 6d65 223a           "time":
+00005c20: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00005c30: 2022 6c61 6265 6c22 3a20 2254 696d 653a   "label": "Time:
+00005c40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00005c50: 2022 756e 6974 7322 3a20 2273 222c 0a20   "units": "s",. 
+00005c60: 2020 2020 2020 2020 2020 2020 2022 7661               "va
+00005c70: 6c75 6522 3a20 3336 3030 302e 302c 0a20  lue": 36000.0,. 
+00005c80: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00005c90: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
+00005ca0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00005cb0: 7363 7269 7074 696f 6e22 3a20 224d 6178  scription": "Max
+00005cc0: 696d 756d 2064 7572 6174 696f 6e20 6f66  imum duration of
+00005cd0: 2074 6865 2043 4320 7374 6570 222c 0a20   the CC step",. 
+00005ce0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00005cf0: 6661 756c 745f 7661 6c75 6522 3a20 302e  fault_value": 0.
+00005d00: 300a 2020 2020 2020 2020 2020 2020 7d2c  0.            },
+00005d10: 0a20 2020 2020 2020 2020 2020 2022 455f  .            "E_
+00005d20: 7261 6e67 6522 3a20 7b0a 2020 2020 2020  range": {.      
+00005d30: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
+00005d40: 2022 4520 7261 6e67 6522 2c0a 2020 2020   "E range",.    
+00005d50: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+00005d60: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
+00005d70: 2020 2020 2022 7661 6c75 6522 3a20 222b       "value": "+
+00005d80: 2d35 2e30 2056 222c 0a20 2020 2020 2020  -5.0 V",.       
+00005d90: 2020 2020 2020 2022 7265 7175 6972 6564         "required
+00005da0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+00005db0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00005dc0: 696f 6e22 3a20 2253 656c 6563 7420 7468  ion": "Select th
+00005dd0: 6520 766f 6c74 6167 6520 7261 6e67 6520  e voltage range 
+00005de0: 6f66 2074 6865 2070 6f74 656e 7469 6f73  of the potentios
+00005df0: 7461 7422 2c0a 2020 2020 2020 2020 2020  tat",.          
+00005e00: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
+00005e10: 7565 223a 2022 6175 746f 220a 2020 2020  ue": "auto".    
+00005e20: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00005e30: 2020 2020 2020 2022 495f 7261 6e67 6522         "I_range"
+00005e40: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00005e50: 2020 226c 6162 656c 223a 2022 4920 7261    "label": "I ra
+00005e60: 6e67 6522 2c0a 2020 2020 2020 2020 2020  nge",.          
+00005e70: 2020 2020 2275 6e69 7473 223a 2022 222c      "units": "",
+00005e80: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00005e90: 7661 6c75 6522 3a20 2231 3020 6d41 222c  value": "10 mA",
+00005ea0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00005eb0: 7265 7175 6972 6564 223a 2074 7275 652c  required": true,
+00005ec0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00005ed0: 6465 7363 7269 7074 696f 6e22 3a20 2253  description": "S
+00005ee0: 656c 6563 7420 7468 6520 6375 7272 656e  elect the curren
+00005ef0: 7420 7261 6e67 6520 6f66 2074 6865 2070  t range of the p
+00005f00: 6f74 656e 7469 6f73 7461 7422 2c0a 2020  otentiostat",.  
+00005f10: 2020 2020 2020 2020 2020 2020 2264 6566              "def
+00005f20: 6175 6c74 5f76 616c 7565 223a 2022 6b65  ault_value": "ke
+00005f30: 6570 220a 2020 2020 2020 2020 2020 2020  ep".            
+00005f40: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+00005f50: 6375 7272 656e 7422 3a20 7b0a 2020 2020  current": {.    
+00005f60: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00005f70: 223a 2022 5374 6570 2063 7572 7265 6e74  ": "Step current
+00005f80: 3a22 2c0a 2020 2020 2020 2020 2020 2020  :",.            
+00005f90: 2020 2275 6e69 7473 223a 2022 4922 2c0a    "units": "I",.
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00005fb0: 616c 7565 223a 2022 432f 3130 222c 0a20  alue": "C/10",. 
+00005fc0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00005fd0: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
+00005fe0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00005ff0: 7363 7269 7074 696f 6e22 3a20 2243 7572  scription": "Cur
+00006000: 7265 6e74 2064 7572 696e 6720 7468 6520  rent during the 
+00006010: 6375 7272 656e 7420 7374 6570 222c 0a20  current step",. 
+00006020: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00006030: 6661 756c 745f 7661 6c75 6522 3a20 302e  fault_value": 0.
+00006040: 300a 2020 2020 2020 2020 2020 2020 7d2c  0.            },
+00006050: 0a20 2020 2020 2020 2020 2020 2022 6973  .            "is
+00006060: 5f64 656c 7461 223a 207b 0a20 2020 2020  _delta": {.     
+00006070: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00006080: 3a20 225c 7530 3339 3424 4924 3a22 2c0a  : "\u0394$I$:",.
+00006090: 2020 2020 2020 2020 2020 2020 2020 2275                "u
+000060a0: 6e69 7473 223a 2022 222c 0a20 2020 2020  nits": "",.     
+000060b0: 2020 2020 2020 2020 2022 7661 6c75 6522           "value"
+000060c0: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
+000060d0: 2020 2020 2020 2022 7265 7175 6972 6564         "required
+000060e0: 223a 2074 7275 652c 0a20 2020 2020 2020  ": true,.       
+000060f0: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
+00006100: 696f 6e22 3a20 2249 7320 7468 6520 7374  ion": "Is the st
+00006110: 6570 2063 7572 7265 6e74 2061 2024 5c5c  ep current a $\\
+00006120: 4465 6c74 6124 2066 726f 6d20 7072 6576  Delta$ from prev
+00006130: 696f 7573 2073 7465 703f 222c 0a20 2020  ious step?",.   
+00006140: 2020 2020 2020 2020 2020 2022 6465 6661             "defa
+00006150: 756c 745f 7661 6c75 6522 3a20 6661 6c73  ult_value": fals
+00006160: 650a 2020 2020 2020 2020 2020 2020 7d2c  e.            },
+00006170: 0a20 2020 2020 2020 2020 2020 2022 6e5f  .            "n_
+00006180: 6379 636c 6573 223a 207b 0a20 2020 2020  cycles": {.     
+00006190: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+000061a0: 3a20 224e 756d 6265 7220 6f66 2063 7963  : "Number of cyc
+000061b0: 6c65 733a 222c 0a20 2020 2020 2020 2020  les:",.         
+000061c0: 2020 2020 2022 756e 6974 7322 3a20 2222       "units": ""
+000061d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000061e0: 2276 616c 7565 223a 2030 2c0a 2020 2020  "value": 0,.    
+000061f0: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
+00006200: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
+00006210: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+00006220: 6970 7469 6f6e 223a 2022 4379 636c 6520  iption": "Cycle 
+00006230: 7468 726f 7567 6820 7468 6520 6375 7272  through the curr
+00006240: 656e 7420 7465 6368 6e69 7175 6520 4e20  ent technique N 
+00006250: 7469 6d65 732e 222c 0a20 2020 2020 2020  times.",.       
+00006260: 2020 2020 2020 2022 6465 6661 756c 745f         "default_
+00006270: 7661 6c75 6522 3a20 300a 2020 2020 2020  value": 0.      
+00006280: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00006290: 2020 2020 2022 6578 6974 5f6f 6e5f 6c69       "exit_on_li
+000062a0: 6d69 7422 3a20 7b0a 2020 2020 2020 2020  mit": {.        
+000062b0: 2020 2020 2020 226c 6162 656c 223a 2022        "label": "
+000062c0: 4578 6974 2077 6865 6e20 6c69 6d69 7473  Exit when limits
+000062d0: 2072 6561 6368 6564 3f22 2c0a 2020 2020   reached?",.    
+000062e0: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+000062f0: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
+00006300: 2020 2020 2022 7661 6c75 6522 3a20 6661       "value": fa
+00006310: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00006320: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
+00006330: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00006340: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00006350: 3a20 2253 746f 7020 7468 6520 7768 6f6c  : "Stop the whol
+00006360: 6520 6578 7065 7269 6d65 6e74 2077 6865  e experiment whe
+00006370: 6e20 6c69 6d69 7420 6973 2072 6561 6368  n limit is reach
+00006380: 6564 3f22 2c0a 2020 2020 2020 2020 2020  ed?",.          
+00006390: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
+000063a0: 7565 223a 2066 616c 7365 0a20 2020 2020  ue": false.     
+000063b0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000063c0: 2020 2020 2020 2272 6563 6f72 645f 6576        "record_ev
+000063d0: 6572 795f 6445 223a 207b 0a20 2020 2020  ery_dE": {.     
+000063e0: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+000063f0: 3a20 2252 6563 6f72 6420 6576 6572 7920  : "Record every 
+00006400: 2464 4524 3a22 2c0a 2020 2020 2020 2020  $dE$:",.        
+00006410: 2020 2020 2020 2275 6e69 7473 223a 2022        "units": "
+00006420: 5622 2c0a 2020 2020 2020 2020 2020 2020  V",.            
+00006430: 2020 2276 616c 7565 223a 2030 2e31 2c0a    "value": 0.1,.
+00006440: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00006450: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
+00006460: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00006470: 6573 6372 6970 7469 6f6e 223a 2022 5265  escription": "Re
+00006480: 636f 7264 2061 2064 6174 6170 6f69 6e74  cord a datapoint
+00006490: 2061 7420 7072 6573 6372 6962 6564 2076   at prescribed v
+000064a0: 6f6c 7461 6765 2073 7061 6369 6e67 222c  oltage spacing",
+000064b0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000064c0: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
+000064d0: 302e 3030 350a 2020 2020 2020 2020 2020  0.005.          
+000064e0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+000064f0: 2022 7265 636f 7264 5f65 7665 7279 5f64   "record_every_d
+00006500: 7422 3a20 7b0a 2020 2020 2020 2020 2020  t": {.          
+00006510: 2020 2020 226c 6162 656c 223a 2022 5265      "label": "Re
+00006520: 636f 7264 2065 7665 7279 2024 6474 243a  cord every $dt$:
+00006530: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006540: 2022 756e 6974 7322 3a20 2273 222c 0a20   "units": "s",. 
+00006550: 2020 2020 2020 2020 2020 2020 2022 7661               "va
+00006560: 6c75 6522 3a20 3630 2e30 2c0a 2020 2020  lue": 60.0,.    
+00006570: 2020 2020 2020 2020 2020 2272 6571 7569            "requi
+00006580: 7265 6422 3a20 7472 7565 2c0a 2020 2020  red": true,.    
+00006590: 2020 2020 2020 2020 2020 2264 6573 6372            "descr
+000065a0: 6970 7469 6f6e 223a 2022 5265 636f 7264  iption": "Record
+000065b0: 2061 2064 6174 6170 6f69 6e74 2061 7420   a datapoint at 
+000065c0: 7072 6573 6372 6962 6564 2074 696d 6520  prescribed time 
+000065d0: 7370 6163 696e 6722 2c0a 2020 2020 2020  spacing",.      
+000065e0: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+000065f0: 5f76 616c 7565 223a 2033 302e 300a 2020  _value": 30.0.  
+00006600: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00006610: 2020 2020 2020 2020 2022 6c69 6d69 745f           "limit_
+00006620: 6375 7272 656e 745f 6d61 7822 3a20 7b0a  current_max": {.
+00006630: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00006640: 6162 656c 223a 2022 4d61 7869 6d75 6d20  abel": "Maximum 
+00006650: 6375 7272 656e 743a 222c 0a20 2020 2020  current:",.     
+00006660: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+00006670: 3a20 2249 222c 0a20 2020 2020 2020 2020  : "I",.         
+00006680: 2020 2020 2022 7661 6c75 6522 3a20 6e75       "value": nu
+00006690: 6c6c 2c0a 2020 2020 2020 2020 2020 2020  ll,.            
+000066a0: 2020 2272 6571 7569 7265 6422 3a20 6661    "required": fa
+000066b0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+000066c0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+000066d0: 3a20 2244 6566 696e 6520 7468 6520 7570  : "Define the up
+000066e0: 7065 7220 6c69 6d69 7420 6f66 2063 7572  per limit of cur
+000066f0: 7265 6e74 2066 6f72 2074 6869 7320 7374  rent for this st
+00006700: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
+00006710: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
+00006720: 6522 3a20 6e75 6c6c 0a20 2020 2020 2020  e": null.       
+00006730: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00006740: 2020 2020 226c 696d 6974 5f63 7572 7265      "limit_curre
+00006750: 6e74 5f6d 696e 223a 207b 0a20 2020 2020  nt_min": {.     
+00006760: 2020 2020 2020 2020 2022 6c61 6265 6c22           "label"
+00006770: 3a20 224d 696e 696d 756d 2063 7572 7265  : "Minimum curre
+00006780: 6e74 3a22 2c0a 2020 2020 2020 2020 2020  nt:",.          
+00006790: 2020 2020 2275 6e69 7473 223a 2022 4922      "units": "I"
+000067a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000067b0: 2276 616c 7565 223a 206e 756c 6c2c 0a20  "value": null,. 
+000067c0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+000067d0: 7175 6972 6564 223a 2066 616c 7365 2c0a  quired": false,.
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000067f0: 6573 6372 6970 7469 6f6e 223a 2022 4465  escription": "De
+00006800: 6669 6e65 2074 6865 206c 6f77 6572 206c  fine the lower l
+00006810: 696d 6974 206f 6620 6375 7272 656e 7420  imit of current 
+00006820: 666f 7220 7468 6973 2073 7465 7022 2c0a  for this step",.
+00006830: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00006840: 6566 6175 6c74 5f76 616c 7565 223a 206e  efault_value": n
+00006850: 756c 6c0a 2020 2020 2020 2020 2020 2020  ull.            
+00006860: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+00006870: 6c69 6d69 745f 766f 6c74 6167 655f 6d61  limit_voltage_ma
+00006880: 7822 3a20 7b0a 2020 2020 2020 2020 2020  x": {.          
+00006890: 2020 2020 226c 6162 656c 223a 2022 4d61      "label": "Ma
+000068a0: 7869 6d75 6d20 766f 6c74 6167 653a 222c  ximum voltage:",
+000068b0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000068c0: 756e 6974 7322 3a20 2256 222c 0a20 2020  units": "V",.   
+000068d0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+000068e0: 6522 3a20 322e 352c 0a20 2020 2020 2020  e": 2.5,.       
+000068f0: 2020 2020 2020 2022 7265 7175 6972 6564         "required
+00006900: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
+00006910: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00006920: 7469 6f6e 223a 2022 4465 6669 6e65 2074  tion": "Define t
+00006930: 6865 2075 7070 6572 206c 696d 6974 206f  he upper limit o
+00006940: 6620 766f 6c74 6167 6520 666f 7220 7468  f voltage for th
+00006950: 6973 2073 7465 7022 2c0a 2020 2020 2020  is step",.      
+00006960: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+00006970: 5f76 616c 7565 223a 206e 756c 6c0a 2020  _value": null.  
+00006980: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00006990: 2020 2020 2020 2020 2022 6c69 6d69 745f           "limit_
+000069a0: 766f 6c74 6167 655f 6d69 6e22 3a20 7b0a  voltage_min": {.
+000069b0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+000069c0: 6162 656c 223a 2022 4d69 6e69 6d75 6d20  abel": "Minimum 
+000069d0: 766f 6c74 6167 653a 222c 0a20 2020 2020  voltage:",.     
+000069e0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+000069f0: 3a20 2256 222c 0a20 2020 2020 2020 2020  : "V",.         
+00006a00: 2020 2020 2022 7661 6c75 6522 3a20 312e       "value": 1.
+00006a10: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00006a20: 2022 7265 7175 6972 6564 223a 2066 616c   "required": fal
+00006a30: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00006a40: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
+00006a50: 2022 4465 6669 6e65 2074 6865 206c 6f77   "Define the low
+00006a60: 6572 206c 696d 6974 206f 6620 766f 6c74  er limit of volt
+00006a70: 6167 6520 666f 7220 7468 6973 2073 7465  age for this ste
+00006a80: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
+00006a90: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
+00006aa0: 223a 206e 756c 6c0a 2020 2020 2020 2020  ": null.        
+00006ab0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00006ac0: 7d2c 0a20 2020 2020 2020 2020 2022 7368  },.          "sh
+00006ad0: 6f72 745f 6e61 6d65 223a 2022 4343 222c  ort_name": "CC",
+00006ae0: 0a20 2020 2020 2020 2020 2022 6465 7363  .          "desc
+00006af0: 7269 7074 696f 6e22 3a20 2243 6f6e 7472  ription": "Contr
+00006b00: 6f6c 6c65 6420 6375 7272 656e 7420 7465  olled current te
+00006b10: 6368 6e69 7175 652c 2077 6974 6820 6f70  chnique, with op
+00006b20: 7469 6f6e 616c 2076 6f6c 7461 6765 2061  tional voltage a
+00006b30: 6e64 2063 7572 7265 6e74 206c 696d 6974  nd current limit
+00006b40: 7322 0a20 2020 2020 2020 207d 2c0a 2020  s".        },.  
+00006b50: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00006b60: 2020 226e 616d 6522 3a20 2243 435f 3222    "name": "CC_2"
+00006b70: 2c0a 2020 2020 2020 2020 2020 2264 6576  ,.          "dev
+00006b80: 6963 6522 3a20 224d 5047 3222 2c0a 2020  ice": "MPG2",.  
+00006b90: 2020 2020 2020 2020 2274 6563 686e 6971          "techniq
+00006ba0: 7565 223a 2022 636f 6e73 7461 6e74 5f63  ue": "constant_c
+00006bb0: 7572 7265 6e74 222c 0a20 2020 2020 2020  urrent",.       
+00006bc0: 2020 2022 7061 7261 6d65 7465 7273 223a     "parameters":
+00006bd0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
+00006be0: 7469 6d65 223a 207b 0a20 2020 2020 2020  time": {.       
+00006bf0: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00006c00: 2254 696d 653a 222c 0a20 2020 2020 2020  "Time:",.       
+00006c10: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00006c20: 2273 222c 0a20 2020 2020 2020 2020 2020  "s",.           
+00006c30: 2020 2022 7661 6c75 6522 3a20 3336 3030     "value": 3600
+00006c40: 302e 302c 0a20 2020 2020 2020 2020 2020  0.0,.           
+00006c50: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
+00006c60: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00006c70: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00006c80: 3a20 224d 6178 696d 756d 2064 7572 6174  : "Maximum durat
+00006c90: 696f 6e20 6f66 2074 6865 2043 4320 7374  ion of the CC st
+00006ca0: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
+00006cb0: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
+00006cc0: 6522 3a20 302e 300a 2020 2020 2020 2020  e": 0.0.        
+00006cd0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00006ce0: 2020 2022 455f 7261 6e67 6522 3a20 7b0a     "E_range": {.
+00006cf0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00006d00: 6162 656c 223a 2022 4520 7261 6e67 6522  abel": "E range"
+00006d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006d20: 2275 6e69 7473 223a 2022 222c 0a20 2020  "units": "",.   
+00006d30: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00006d40: 6522 3a20 222b 2d35 2e30 2056 222c 0a20  e": "+-5.0 V",. 
+00006d50: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00006d60: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
+00006d70: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00006d80: 7363 7269 7074 696f 6e22 3a20 2253 656c  scription": "Sel
+00006d90: 6563 7420 7468 6520 766f 6c74 6167 6520  ect the voltage 
+00006da0: 7261 6e67 6520 6f66 2074 6865 2070 6f74  range of the pot
+00006db0: 656e 7469 6f73 7461 7422 2c0a 2020 2020  entiostat",.    
+00006dc0: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
+00006dd0: 6c74 5f76 616c 7565 223a 2022 6175 746f  lt_value": "auto
+00006de0: 220a 2020 2020 2020 2020 2020 2020 7d2c  ".            },
+00006df0: 0a20 2020 2020 2020 2020 2020 2022 495f  .            "I_
+00006e00: 7261 6e67 6522 3a20 7b0a 2020 2020 2020  range": {.      
+00006e10: 2020 2020 2020 2020 226c 6162 656c 223a          "label":
+00006e20: 2022 4920 7261 6e67 6522 2c0a 2020 2020   "I range",.    
+00006e30: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+00006e40: 223a 2022 222c 0a20 2020 2020 2020 2020  ": "",.         
+00006e50: 2020 2020 2022 7661 6c75 6522 3a20 2231       "value": "1
+00006e60: 3020 6d41 222c 0a20 2020 2020 2020 2020  0 mA",.         
+00006e70: 2020 2020 2022 7265 7175 6972 6564 223a       "required":
+00006e80: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
+00006e90: 2020 2020 2022 6465 7363 7269 7074 696f       "descriptio
+00006ea0: 6e22 3a20 2253 656c 6563 7420 7468 6520  n": "Select the 
+00006eb0: 6375 7272 656e 7420 7261 6e67 6520 6f66  current range of
+00006ec0: 2074 6865 2070 6f74 656e 7469 6f73 7461   the potentiosta
+00006ed0: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00006ee0: 2020 2264 6566 6175 6c74 5f76 616c 7565    "default_value
+00006ef0: 223a 2022 6b65 6570 220a 2020 2020 2020  ": "keep".      
+00006f00: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00006f10: 2020 2020 2022 6375 7272 656e 7422 3a20       "current": 
+00006f20: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00006f30: 226c 6162 656c 223a 2022 5374 6570 2063  "label": "Step c
+00006f40: 7572 7265 6e74 3a22 2c0a 2020 2020 2020  urrent:",.      
+00006f50: 2020 2020 2020 2020 2275 6e69 7473 223a          "units":
+00006f60: 2022 4922 2c0a 2020 2020 2020 2020 2020   "I",.          
+00006f70: 2020 2020 2276 616c 7565 223a 2022 442f      "value": "D/
+00006f80: 3130 222c 0a20 2020 2020 2020 2020 2020  10",.           
+00006f90: 2020 2022 7265 7175 6972 6564 223a 2074     "required": t
+00006fa0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00006fb0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+00006fc0: 3a20 2243 7572 7265 6e74 2064 7572 696e  : "Current durin
+00006fd0: 6720 7468 6520 6375 7272 656e 7420 7374  g the current st
+00006fe0: 6570 222c 0a20 2020 2020 2020 2020 2020  ep",.           
+00006ff0: 2020 2022 6465 6661 756c 745f 7661 6c75     "default_valu
+00007000: 6522 3a20 302e 300a 2020 2020 2020 2020  e": 0.0.        
+00007010: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00007020: 2020 2022 6973 5f64 656c 7461 223a 207b     "is_delta": {
+00007030: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00007040: 6c61 6265 6c22 3a20 225c 7530 3339 3424  label": "\u0394$
+00007050: 4924 3a22 2c0a 2020 2020 2020 2020 2020  I$:",.          
+00007060: 2020 2020 2275 6e69 7473 223a 2022 222c      "units": "",
+00007070: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00007080: 7661 6c75 6522 3a20 6661 6c73 652c 0a20  value": false,. 
+00007090: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+000070a0: 7175 6972 6564 223a 2074 7275 652c 0a20  quired": true,. 
+000070b0: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+000070c0: 7363 7269 7074 696f 6e22 3a20 2249 7320  scription": "Is 
+000070d0: 7468 6520 7374 6570 2063 7572 7265 6e74  the step current
+000070e0: 2061 2024 5c5c 4465 6c74 6124 2066 726f   a $\\Delta$ fro
+000070f0: 6d20 7072 6576 696f 7573 2073 7465 703f  m previous step?
+00007100: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00007110: 2022 6465 6661 756c 745f 7661 6c75 6522   "default_value"
+00007120: 3a20 6661 6c73 650a 2020 2020 2020 2020  : false.        
+00007130: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00007140: 2020 2022 6e5f 6379 636c 6573 223a 207b     "n_cycles": {
+00007150: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00007160: 6c61 6265 6c22 3a20 224e 756d 6265 7220  label": "Number 
+00007170: 6f66 2063 7963 6c65 733a 222c 0a20 2020  of cycles:",.   
+00007180: 2020 2020 2020 2020 2020 2022 756e 6974             "unit
+00007190: 7322 3a20 2222 2c0a 2020 2020 2020 2020  s": "",.        
+000071a0: 2020 2020 2020 2276 616c 7565 223a 2030        "value": 0
+000071b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000071c0: 2272 6571 7569 7265 6422 3a20 7472 7565  "required": true
+000071d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000071e0: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+000071f0: 4379 636c 6520 7468 726f 7567 6820 7468  Cycle through th
+00007200: 6520 6375 7272 656e 7420 7465 6368 6e69  e current techni
+00007210: 7175 6520 4e20 7469 6d65 732e 222c 0a20  que N times.",. 
+00007220: 2020 2020 2020 2020 2020 2020 2022 6465               "de
+00007230: 6661 756c 745f 7661 6c75 6522 3a20 300a  fault_value": 0.
+00007240: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00007250: 2020 2020 2020 2020 2020 2022 6578 6974             "exit
+00007260: 5f6f 6e5f 6c69 6d69 7422 3a20 7b0a 2020  _on_limit": {.  
+00007270: 2020 2020 2020 2020 2020 2020 226c 6162              "lab
+00007280: 656c 223a 2022 4578 6974 2077 6865 6e20  el": "Exit when 
+00007290: 6c69 6d69 7473 2072 6561 6368 6564 3f22  limits reached?"
+000072a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000072b0: 2275 6e69 7473 223a 2022 222c 0a20 2020  "units": "",.   
+000072c0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+000072d0: 6522 3a20 6661 6c73 652c 0a20 2020 2020  e": false,.     
+000072e0: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
+000072f0: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+00007300: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00007310: 7074 696f 6e22 3a20 2253 746f 7020 7468  ption": "Stop th
+00007320: 6520 7768 6f6c 6520 6578 7065 7269 6d65  e whole experime
+00007330: 6e74 2077 6865 6e20 6c69 6d69 7420 6973  nt when limit is
+00007340: 2072 6561 6368 6564 3f22 2c0a 2020 2020   reached?",.    
+00007350: 2020 2020 2020 2020 2020 2264 6566 6175            "defau
+00007360: 6c74 5f76 616c 7565 223a 2066 616c 7365  lt_value": false
+00007370: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00007380: 2020 2020 2020 2020 2020 2020 2272 6563              "rec
+00007390: 6f72 645f 6576 6572 795f 6445 223a 207b  ord_every_dE": {
+000073a0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000073b0: 6c61 6265 6c22 3a20 2252 6563 6f72 6420  label": "Record 
+000073c0: 6576 6572 7920 2464 4524 3a22 2c0a 2020  every $dE$:",.  
+000073d0: 2020 2020 2020 2020 2020 2020 2275 6e69              "uni
+000073e0: 7473 223a 2022 5622 2c0a 2020 2020 2020  ts": "V",.      
+000073f0: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
+00007400: 2030 2e31 2c0a 2020 2020 2020 2020 2020   0.1,.          
+00007410: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
+00007420: 7472 7565 2c0a 2020 2020 2020 2020 2020  true,.          
+00007430: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+00007440: 223a 2022 5265 636f 7264 2061 2064 6174  ": "Record a dat
+00007450: 6170 6f69 6e74 2061 7420 7072 6573 6372  apoint at prescr
+00007460: 6962 6564 2076 6f6c 7461 6765 2073 7061  ibed voltage spa
+00007470: 6369 6e67 222c 0a20 2020 2020 2020 2020  cing",.         
+00007480: 2020 2020 2022 6465 6661 756c 745f 7661       "default_va
+00007490: 6c75 6522 3a20 302e 3030 350a 2020 2020  lue": 0.005.    
+000074a0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000074b0: 2020 2020 2020 2022 7265 636f 7264 5f65         "record_e
+000074c0: 7665 7279 5f64 7422 3a20 7b0a 2020 2020  very_dt": {.    
+000074d0: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+000074e0: 223a 2022 5265 636f 7264 2065 7665 7279  ": "Record every
+000074f0: 2024 6474 243a 222c 0a20 2020 2020 2020   $dt$:",.       
+00007500: 2020 2020 2020 2022 756e 6974 7322 3a20         "units": 
+00007510: 2273 222c 0a20 2020 2020 2020 2020 2020  "s",.           
+00007520: 2020 2022 7661 6c75 6522 3a20 3630 2e30     "value": 60.0
+00007530: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007540: 2272 6571 7569 7265 6422 3a20 7472 7565  "required": true
+00007550: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007560: 2264 6573 6372 6970 7469 6f6e 223a 2022  "description": "
+00007570: 5265 636f 7264 2061 2064 6174 6170 6f69  Record a datapoi
+00007580: 6e74 2061 7420 7072 6573 6372 6962 6564  nt at prescribed
+00007590: 2074 696d 6520 7370 6163 696e 6722 2c0a   time spacing",.
+000075a0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000075b0: 6566 6175 6c74 5f76 616c 7565 223a 2033  efault_value": 3
+000075c0: 302e 300a 2020 2020 2020 2020 2020 2020  0.0.            
+000075d0: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+000075e0: 6c69 6d69 745f 6375 7272 656e 745f 6d61  limit_current_ma
+000075f0: 7822 3a20 7b0a 2020 2020 2020 2020 2020  x": {.          
+00007600: 2020 2020 226c 6162 656c 223a 2022 4d61      "label": "Ma
+00007610: 7869 6d75 6d20 6375 7272 656e 743a 222c  ximum current:",
+00007620: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00007630: 756e 6974 7322 3a20 2249 222c 0a20 2020  units": "I",.   
+00007640: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00007650: 6522 3a20 6e75 6c6c 2c0a 2020 2020 2020  e": null,.      
+00007660: 2020 2020 2020 2020 2272 6571 7569 7265          "require
+00007670: 6422 3a20 6661 6c73 652c 0a20 2020 2020  d": false,.     
+00007680: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00007690: 7074 696f 6e22 3a20 2244 6566 696e 6520  ption": "Define 
+000076a0: 7468 6520 7570 7065 7220 6c69 6d69 7420  the upper limit 
+000076b0: 6f66 2063 7572 7265 6e74 2066 6f72 2074  of current for t
+000076c0: 6869 7320 7374 6570 222c 0a20 2020 2020  his step",.     
+000076d0: 2020 2020 2020 2020 2022 6465 6661 756c           "defaul
+000076e0: 745f 7661 6c75 6522 3a20 6e75 6c6c 0a20  t_value": null. 
+000076f0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00007700: 2020 2020 2020 2020 2020 226c 696d 6974            "limit
+00007710: 5f63 7572 7265 6e74 5f6d 696e 223a 207b  _current_min": {
+00007720: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00007730: 6c61 6265 6c22 3a20 224d 696e 696d 756d  label": "Minimum
+00007740: 2063 7572 7265 6e74 3a22 2c0a 2020 2020   current:",.    
+00007750: 2020 2020 2020 2020 2020 2275 6e69 7473            "units
+00007760: 223a 2022 4922 2c0a 2020 2020 2020 2020  ": "I",.        
+00007770: 2020 2020 2020 2276 616c 7565 223a 206e        "value": n
+00007780: 756c 6c2c 0a20 2020 2020 2020 2020 2020  ull,.           
+00007790: 2020 2022 7265 7175 6972 6564 223a 2066     "required": f
+000077a0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+000077b0: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
+000077c0: 223a 2022 4465 6669 6e65 2074 6865 206c  ": "Define the l
+000077d0: 6f77 6572 206c 696d 6974 206f 6620 6375  ower limit of cu
+000077e0: 7272 656e 7420 666f 7220 7468 6973 2073  rrent for this s
+000077f0: 7465 7022 2c0a 2020 2020 2020 2020 2020  tep",.          
+00007800: 2020 2020 2264 6566 6175 6c74 5f76 616c      "default_val
+00007810: 7565 223a 206e 756c 6c0a 2020 2020 2020  ue": null.      
+00007820: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00007830: 2020 2020 2022 6c69 6d69 745f 766f 6c74       "limit_volt
+00007840: 6167 655f 6d61 7822 3a20 7b0a 2020 2020  age_max": {.    
+00007850: 2020 2020 2020 2020 2020 226c 6162 656c            "label
+00007860: 223a 2022 4d61 7869 6d75 6d20 766f 6c74  ": "Maximum volt
+00007870: 6167 653a 222c 0a20 2020 2020 2020 2020  age:",.         
+00007880: 2020 2020 2022 756e 6974 7322 3a20 2256       "units": "V
+00007890: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000078a0: 2022 7661 6c75 6522 3a20 322e 352c 0a20   "value": 2.5,. 
+000078b0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+000078c0: 7175 6972 6564 223a 2066 616c 7365 2c0a  quired": false,.
+000078d0: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+000078e0: 6573 6372 6970 7469 6f6e 223a 2022 4465  escription": "De
+000078f0: 6669 6e65 2074 6865 2075 7070 6572 206c  fine the upper l
+00007900: 696d 6974 206f 6620 766f 6c74 6167 6520  imit of voltage 
+00007910: 666f 7220 7468 6973 2073 7465 7022 2c0a  for this step",.
+00007920: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00007930: 6566 6175 6c74 5f76 616c 7565 223a 206e  efault_value": n
+00007940: 756c 6c0a 2020 2020 2020 2020 2020 2020  ull.            
+00007950: 7d2c 0a20 2020 2020 2020 2020 2020 2022  },.            "
+00007960: 6c69 6d69 745f 766f 6c74 6167 655f 6d69  limit_voltage_mi
+00007970: 6e22 3a20 7b0a 2020 2020 2020 2020 2020  n": {.          
+00007980: 2020 2020 226c 6162 656c 223a 2022 4d69      "label": "Mi
+00007990: 6e69 6d75 6d20 766f 6c74 6167 653a 222c  nimum voltage:",
+000079a0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+000079b0: 756e 6974 7322 3a20 2256 222c 0a20 2020  units": "V",.   
+000079c0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+000079d0: 6522 3a20 312e 352c 0a20 2020 2020 2020  e": 1.5,.       
+000079e0: 2020 2020 2020 2022 7265 7175 6972 6564         "required
+000079f0: 223a 2066 616c 7365 2c0a 2020 2020 2020  ": false,.      
+00007a00: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00007a10: 7469 6f6e 223a 2022 4465 6669 6e65 2074  tion": "Define t
+00007a20: 6865 206c 6f77 6572 206c 696d 6974 206f  he lower limit o
+00007a30: 6620 766f 6c74 6167 6520 666f 7220 7468  f voltage for th
+00007a40: 6973 2073 7465 7022 2c0a 2020 2020 2020  is step",.      
+00007a50: 2020 2020 2020 2020 2264 6566 6175 6c74          "default
+00007a60: 5f76 616c 7565 223a 206e 756c 6c0a 2020  _value": null.  
+00007a70: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00007a80: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00007a90: 2020 2022 7368 6f72 745f 6e61 6d65 223a     "short_name":
+00007aa0: 2022 4343 222c 0a20 2020 2020 2020 2020   "CC",.         
+00007ab0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
+00007ac0: 2243 6f6e 7472 6f6c 6c65 6420 6375 7272  "Controlled curr
+00007ad0: 656e 7420 7465 6368 6e69 7175 652c 2077  ent technique, w
+00007ae0: 6974 6820 6f70 7469 6f6e 616c 2076 6f6c  ith optional vol
+00007af0: 7461 6765 2061 6e64 2063 7572 7265 6e74  tage and current
+00007b00: 206c 696d 6974 7322 0a20 2020 2020 2020   limits".       
+00007b10: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00007b20: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00007b30: 224c 4f4f 505f 3122 2c0a 2020 2020 2020  "LOOP_1",.      
+00007b40: 2020 2020 2264 6576 6963 6522 3a20 224d      "device": "M
+00007b50: 5047 3222 2c0a 2020 2020 2020 2020 2020  PG2",.          
+00007b60: 2274 6563 686e 6971 7565 223a 2022 6c6f  "technique": "lo
+00007b70: 6f70 222c 0a20 2020 2020 2020 2020 2022  op",.          "
+00007b80: 7061 7261 6d65 7465 7273 223a 207b 0a20  parameters": {. 
+00007b90: 2020 2020 2020 2020 2020 2022 676f 746f             "goto
+00007ba0: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
+00007bb0: 2020 2022 6c61 6265 6c22 3a20 2247 6f20     "label": "Go 
+00007bc0: 746f 3a22 2c0a 2020 2020 2020 2020 2020  to:",.          
+00007bd0: 2020 2020 2275 6e69 7473 223a 2022 222c      "units": "",
+00007be0: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00007bf0: 7661 6c75 6522 3a20 312c 0a20 2020 2020  value": 1,.     
+00007c00: 2020 2020 2020 2020 2022 7265 7175 6972           "requir
+00007c10: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
+00007c20: 2020 2020 2020 2020 2022 6465 7363 7269           "descri
+00007c30: 7074 696f 6e22 3a20 2249 6e64 6578 206f  ption": "Index o
+00007c40: 6620 7468 6520 7465 6368 6e69 7175 6520  f the technique 
+00007c50: 746f 2067 6f20 6261 636b 2074 6f22 2c0a  to go back to",.
+00007c60: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00007c70: 6566 6175 6c74 5f76 616c 7565 223a 2031  efault_value": 1
+00007c80: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+00007c90: 2020 2020 2020 2020 2020 2020 226e 5f67              "n_g
+00007ca0: 6f74 6f73 223a 207b 0a20 2020 2020 2020  otos": {.       
+00007cb0: 2020 2020 2020 2022 6c61 6265 6c22 3a20         "label": 
+00007cc0: 2252 6570 6561 7473 222c 0a20 2020 2020  "Repeats",.     
+00007cd0: 2020 2020 2020 2020 2022 756e 6974 7322           "units"
+00007ce0: 3a20 2222 2c0a 2020 2020 2020 2020 2020  : "",.          
+00007cf0: 2020 2020 2276 616c 7565 223a 2032 2c0a      "value": 2,.
+00007d00: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00007d10: 6571 7569 7265 6422 3a20 7472 7565 2c0a  equired": true,.
+00007d20: 2020 2020 2020 2020 2020 2020 2020 2264                "d
+00007d30: 6573 6372 6970 7469 6f6e 223a 2022 4e75  escription": "Nu
+00007d40: 6d62 6572 206f 6620 7469 6d65 7320 7468  mber of times th
+00007d50: 6520 7465 6368 6e69 7175 6520 7769 6c6c  e technique will
+00007d60: 206a 756d 703b 2073 6574 2074 6f20 2d31   jump; set to -1
+00007d70: 2066 6f72 2075 6e6c 696d 6974 6564 222c   for unlimited",
+00007d80: 0a20 2020 2020 2020 2020 2020 2020 2022  .              "
+00007d90: 6465 6661 756c 745f 7661 6c75 6522 3a20  default_value": 
+00007da0: 2d31 0a20 2020 2020 2020 2020 2020 207d  -1.            }
+00007db0: 0a20 2020 2020 2020 2020 207d 2c0a 2020  .          },.  
+00007dc0: 2020 2020 2020 2020 2273 686f 7274 5f6e          "short_n
+00007dd0: 616d 6522 3a20 224c 4f4f 5022 2c0a 2020  ame": "LOOP",.  
+00007de0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
+00007df0: 7469 6f6e 223a 2022 4c6f 6f70 2074 6563  tion": "Loop tec
+00007e00: 686e 6971 7565 2c20 616c 6c6f 7769 6e67  hnique, allowing
+00007e10: 2074 6f20 7265 7065 6174 2061 2073 6574   to repeat a set
+00007e20: 206f 6620 7072 6563 6564 696e 6720 7465   of preceding te
+00007e30: 6368 6e69 7175 6573 2069 6e20 6120 7465  chniques in a te
+00007e40: 6368 6e69 7175 6520 6172 7261 7922 0a20  chnique array". 
+00007e50: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
+00007e60: 0a20 2020 207d 0a20 207d 0a              .    }.  }.
```

### Comparing `aiida_aurora-0.3.1/docs/Makefile` & `aiida_aurora-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/docs/source/conf.py` & `aiida_aurora-0.3.2/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 version = ".".join(release.split(".")[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
@@ -349,8 +349,12 @@
 # texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 # Warnings to ignore when using the -n (nitpicky) option
 # We should ignore any python built-in exception, for instance
-nitpick_ignore = []
+# nitpick_ignore = []
+with open('nitpick-exceptions') as handle:
+    nitpick_ignore = [
+        tuple(line.strip().split(None, 1)) for line in handle.readlines() if line.strip() and not line.startswith('#')
+    ]
```

### Comparing `aiida_aurora-0.3.1/docs/source/developer_guide/index.rst` & `aiida_aurora-0.3.2/docs/source/developer_guide/index.rst`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/docs/source/images/AiiDA_transparent_logo.png` & `aiida_aurora-0.3.2/docs/source/images/AiiDA_transparent_logo.png`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/docs/source/index.rst` & `aiida_aurora-0.3.2/docs/source/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -24,15 +24,21 @@
 .. highlights:: Giovanni Pizzi, Andrea Cepellotti, Riccardo Sabatini, Nicola Marzari,
   and Boris Kozinsky, *AiiDA: automated interactive infrastructure and database
   for computational science*, Comp. Mat. Sci 111, 218-230 (2016);
   https://doi.org/10.1016/j.commatsci.2015.09.013; http://www.aiida.net.
 
 ``aiida-aurora`` is released under the MIT license.
 
-Please contact loris.ercole@epfl.ch for information concerning ``aiida-aurora`` and the `AiiDA mailing list <http://www.aiida.net/mailing-list/>`_ for questions concerning ``aiida``.
+For information concerning ``aiida-aurora``, please contact:
+
+ - Francisco F. Ramirez (francisco.ramirez@epfl.ch)
+ - Edan Bainglass (edan.bainglass@psi.ch)
+ - Giovanni Pizzi (giovanni.pizzi@psi.ch)
+
+For questions concerning ``aiida``, please use the `AiiDA mailing list <http://www.aiida.net/mailing-list/>`_
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `aiida_aurora-0.3.1/docs/source/user_guide/get_started.rst` & `aiida_aurora-0.3.2/docs/source/user_guide/get_started.rst`

 * *Files 8% similar despite different names*

```diff
@@ -34,9 +34,9 @@
 ``verdi code setup``, you may want to try the following command::
 
     aurora-submit  # uses aiida_aurora.cli
 
 Available calculations
 ++++++++++++++++++++++
 
-.. aiida-calcjob:: DiffCalculation
+.. aiida-calcjob:: BatteryCyclerExperiment
     :module: aiida_aurora.calculations
```

### Comparing `aiida_aurora-0.3.1/examples/config_files/setup.sh` & `aiida_aurora-0.3.2/examples/config_files/setup.sh`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/examples/stress_test/batteries.json` & `aiida_aurora-0.3.2/examples/stress_test/batteries.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -166,8 +166,8 @@
 00000a50: 6122 3a20 7b22 6e61 6d65 223a 2022 3139  a": {"name": "19
 00000a60: 3038 3232 5f41 7572 6f72 615f 3136 222c  0822_Aurora_16",
 00000a70: 2022 6372 6561 7469 6f6e 5f64 6174 6574   "creation_datet
 00000a80: 696d 6522 3a20 2232 3032 322d 3038 2d32  ime": "2022-08-2
 00000a90: 3220 3035 3a35 393a 3030 2b30 303a 3030  2 05:59:00+00:00
 00000aa0: 222c 2022 6372 6561 7469 6f6e 5f70 726f  ", "creation_pro
 00000ab0: 6365 7373 223a 2022 4275 696c 7420 6279  cess": "Built by
-00000ac0: 2045 6d70 6122 7d7d 5d                    Empa"}}]
+00000ac0: 2045 6d70 6122 7d7d 5d0a                  Empa"}}].
```

### Comparing `aiida_aurora-0.3.1/examples/stress_test/submit_test.py` & `aiida_aurora-0.3.2/examples/stress_test/submit_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,122 +1,142 @@
 ####################################################################################################
 """Script to use as a template for the submission of the stress test."""
 ####################################################################################################
-import json
 import datetime
+import json
+from typing import Any, Dict, List
+
+from aurora.schemas.battery import BatterySample as BatterySampleSchema
 
 from aiida import orm
 from aiida.engine import submit
 from aiida.plugins import WorkflowFactory
 
 from aiida_aurora.data import BatterySampleData
-from aurora.schemas.battery import BatterySample as BatterySampleSchema
 
 BATTERIES_SPECIFICATIONS_LOCAL = [
     BatterySampleSchema(
-        manufacturer = 'fake',
-        composition = dict(description='C|E|A'),
-        form_factor = 'DUMB',
-        capacity = dict(nominal=1.0, units='Ah'),
-        battery_id = 666,
-        metadata = dict(
-            name = 'fake_sample01',
-            creation_datetime = datetime.datetime.now(tz=datetime.timezone.utc),
-            creation_process = 'This is a fake battery for testing purposes.'
-        )),
+        manufacturer='fake',
+        composition=dict(description='C|E|A'),
+        form_factor='DUMB',
+        capacity=dict(nominal=1.0, units='Ah'),
+        battery_id=666,
+        metadata=dict(
+            name='fake_sample01',
+            creation_datetime=datetime.datetime.now(tz=datetime.timezone.utc),
+            creation_process='This is a fake battery for testing purposes.'
+        )
+    ),
     BatterySampleSchema(
-        manufacturer = 'fake',
-        composition = dict(description='C|E|A'),
-        form_factor = 'DUMB',
-        capacity = dict(nominal=1.0, units='Ah'),
-        battery_id = 667,
-        metadata = dict(
-            name = 'fake_sample02',
-            creation_datetime = datetime.datetime.now(tz=datetime.timezone.utc),
-            creation_process = 'This is a fake battery for testing purposes.'
-        )),
+        manufacturer='fake',
+        composition=dict(description='C|E|A'),
+        form_factor='DUMB',
+        capacity=dict(nominal=1.0, units='Ah'),
+        battery_id=667,
+        metadata=dict(
+            name='fake_sample02',
+            creation_datetime=datetime.datetime.now(tz=datetime.timezone.utc),
+            creation_process='This is a fake battery for testing purposes.'
+        )
+    ),
 ]
 
-MONITOR_OVERRIDES = {}
+MONITOR_OVERRIDES: Dict[Any, Any] = {}
 
-TOMATO_OVERRIDES = {
+TOMATO_OVERRIDES: Dict[Any, Any] = {
     'protection_cycle': {},
     'formation_cycle': {},
     'longterm_cycle': {},
     'discharge_cycle': {},
 }
 
-PROTECTION_CYCLE_OVERSTEPS = [{}, {}, {}]
-FORMATION_CYCLE_OVERSTEPS = [{}, {}, {}]
-LONGTERM_CYCLE_OVERSTEPS = [{}, {}, {}]
-DISCHARGE_CYCLE_OVERSTEPS = [{}]
+PROTECTION_CYCLE_OVERSTEPS: List[Any] = [{}, {}, {}]
+FORMATION_CYCLE_OVERSTEPS: List[Any] = [{}, {}, {}]
+LONGTERM_CYCLE_OVERSTEPS: List[Any] = [{}, {}, {}]
+DISCHARGE_CYCLE_OVERSTEPS: List[Any] = [{}]
 
 CYCLER_OVERRIDES = {
-    'protection_cycle': {'method': PROTECTION_CYCLE_OVERSTEPS},
-    'formation_cycle': {'method': FORMATION_CYCLE_OVERSTEPS},
-    'longterm_cycle': {'method': LONGTERM_CYCLE_OVERSTEPS},
-    'discharge_cycle': {'method': DISCHARGE_CYCLE_OVERSTEPS},
+    'protection_cycle': {
+        'method': PROTECTION_CYCLE_OVERSTEPS
+    },
+    'formation_cycle': {
+        'method': FORMATION_CYCLE_OVERSTEPS
+    },
+    'longterm_cycle': {
+        'method': LONGTERM_CYCLE_OVERSTEPS
+    },
+    'discharge_cycle': {
+        'method': DISCHARGE_CYCLE_OVERSTEPS
+    },
 }
 
 
 ####################################################################################################
 def main_script():
     """Main script"""
     cycler_code = orm.load_code('ketchup-0.2rc2@localhost-tomato')
     monitor_code = orm.load_code('monitor@localhost-aiida')
-    
+
     batteries_specifications = BATTERIES_SPECIFICATIONS_LOCAL
-    #batteries_specifications = read_specifications('batteries.json')
+    # batteries_specifications = read_specifications('batteries.json')
 
     for battery_specification in batteries_specifications:
         print(battery_specification)
         continue
         sample_node = getmake_sample(battery_specification)
 
         WorkflowClass = WorkflowFactory('aurora.stress_test')
         workflow_builder = WorkflowClass.get_builder_from_protocol(
-            ketchup_code = cycler_code,
-            monitor_code = monitor_code,
-            battery_sample = sample_node,
-            tomato_overrides = TOMATO_OVERRIDES,
-            cycler_overrides = CYCLER_OVERRIDES,
-            monitor_overrides = MONITOR_OVERRIDES,
+            ketchup_code=cycler_code,
+            monitor_code=monitor_code,
+            battery_sample=sample_node,
+            tomato_overrides=TOMATO_OVERRIDES,
+            cycler_overrides=CYCLER_OVERRIDES,
+            monitor_overrides=MONITOR_OVERRIDES,
         )
         workflow_node = submit(workflow_builder)
 
         workflow_pk = workflow_node.pk
         battery_name = battery_specification.metadata.name
         print(f'Workflow <{workflow_pk}> submitted for battery `{battery_name}` ... ')
 
+
 ####################################################################################################
 def getmake_sample(battery_schema):
     """Gets the sample node from the DB or creates it."""
     battery_name = battery_schema.metadata.name
     queryb = orm.QueryBuilder()
     queryb.append(orm.Group, filters={'label': {'==': 'BatterySamples'}}, tag='group0')
-    queryb.append(BatterySampleData, filters={'attributes.metadata.name': {'==': battery_name}}, with_group='group0', )
+    queryb.append(
+        BatterySampleData,
+        filters={'attributes.metadata.name': {
+            '==': battery_name
+        }},
+        with_group='group0',
+    )
 
     battery_sample = queryb.first()
     if battery_sample is None:
         battery_sample = BatterySampleData(battery_schema.dict())
 
     return battery_sample
 
 
 ####################################################################################################
 def read_specifications(source_filepath):
     """Reads the battery specifications from a json file"""
 
-    with open(source_filepath, 'r') as fileobj:
+    with open(source_filepath) as fileobj:
         battery_datalist = json.load(fileobj)
 
     batteries_specifications = []
     for battery_data in battery_datalist:
         battery_sample = BatterySampleSchema(**battery_data)
         batteries_specifications.append(battery_sample)
 
     return batteries_specifications
 
+
 ####################################################################################################
 if __name__ == "__main__":
     main_script()
-####################################################################################################
+####################################################################################################
```

### Comparing `aiida_aurora-0.3.1/fake_aurora_server/server.py` & `aiida_aurora-0.3.2/fake_aurora_server/server.py`

 * *Files identical despite different names*

### Comparing `aiida_aurora-0.3.1/pyproject.toml` & `aiida_aurora-0.3.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,51 +2,58 @@
 # build the package with [flit](https://flit.readthedocs.io)
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # See https://www.python.org/dev/peps/pep-0621/
 name = "aiida-aurora"
-dynamic = ["version"]  # read from aiida_aurora/__init__.py
+dynamic = ["version"] # read from aiida_aurora/__init__.py
 description = "AiiDA plugin for the Aurora platform."
-authors = [{name = "Loris Ercole", email = "loris.ercole@epfl.ch"}]
+authors = [
+    { name = "Loris Ercole", email = "loris.ercole@epfl.ch" },
+    { name = "Francisco F. Ramirez", email = "francisco.ramirez@epfl.ch" },
+    { name = "Edan Bainglass", email = "edan.bainglass@psi.ch" },
+    { name = "Giovanni Pizzi", email = "giovanni.pizzi@psi.ch" },
+]
 readme = "README.md"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Development Status :: 3 - Alpha",
     "Framework :: AiiDA"
 ]
 keywords = ["aiida", "plugin", "aurora"]
 requires-python = ">=3.8"
 dependencies = [
     "aiida-core>=1.6.5,<2.0.0",
-    "pydantic"
+    "dgbowl-schemas>=111,<=113",
+    "pydantic",
+    "matplotlib",
+    "pandas",
+    "aiida-calcmonitor"
 ]
 
 [project.urls]
 Source = "https://github.com/epfl-theos/aiida-aurora"
 
 [project.optional-dependencies]
 testing = [
     "pgtest~=1.3.1",
     "wheel~=0.31",
     "coverage[toml]",
     "pytest~=6.0",
     "pytest-cov"
 ]
-pre-commit = [
-    "pre-commit~=2.2",
-    "pylint>=2.5.0,<2.9"
-]
+pre-commit = ["pre-commit~=2.2"]
 docs = [
     "sphinx",
+    "sphinx_rtd_theme",
     "sphinxcontrib-contentui",
     "sphinxcontrib-details-directive",
     "furo",
     "markupsafe<2.1"
 ]
 
 [project.entry-points."aiida.data"]
@@ -95,21 +102,28 @@
     "ignore::DeprecationWarning:plumpy:",
     "ignore::DeprecationWarning:yaml:",
 ]
 
 [tool.coverage.run]
 # Configuration of [coverage.py](https://coverage.readthedocs.io)
 # reporting which lines of your plugin are covered by tests
-source=["aiida_aurora"]
+source = ["aiida_aurora"]
 
 [tool.isort]
 # Configuration of [isort](https://isort.readthedocs.io)
 line_length = 120
 force_sort_within_sections = true
-sections = ['FUTURE', 'STDLIB', 'THIRDPARTY', 'AIIDA', 'FIRSTPARTY', 'LOCALFOLDER']
+sections = [
+    'FUTURE',
+    'STDLIB',
+    'THIRDPARTY',
+    'AIIDA',
+    'FIRSTPARTY',
+    'LOCALFOLDER'
+]
 known_aiida = ['aiida']
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py38
```

### Comparing `aiida_aurora-0.3.1/PKG-INFO` & `aiida_aurora-0.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: aiida-aurora
-Version: 0.3.1
+Version: 0.3.2
 Summary: AiiDA plugin for the Aurora platform.
 Keywords: aiida,plugin,aurora
-Author-email: Loris Ercole <loris.ercole@epfl.ch>
+Author-email: Loris Ercole <loris.ercole@epfl.ch>, "Francisco F. Ramirez" <francisco.ramirez@epfl.ch>, Edan Bainglass <edan.bainglass@psi.ch>, Giovanni Pizzi <giovanni.pizzi@psi.ch>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
 Requires-Dist: aiida-core>=1.6.5,<2.0.0
+Requires-Dist: dgbowl-schemas>=111,<=113
 Requires-Dist: pydantic
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: aiida-calcmonitor
 Requires-Dist: sphinx ; extra == "docs"
+Requires-Dist: sphinx_rtd_theme ; extra == "docs"
 Requires-Dist: sphinxcontrib-contentui ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive ; extra == "docs"
 Requires-Dist: furo ; extra == "docs"
 Requires-Dist: markupsafe<2.1 ; extra == "docs"
 Requires-Dist: pre-commit~=2.2 ; extra == "pre-commit"
-Requires-Dist: pylint>=2.5.0,<2.9 ; extra == "pre-commit"
 Requires-Dist: pgtest~=1.3.1 ; extra == "testing"
 Requires-Dist: wheel~=0.31 ; extra == "testing"
 Requires-Dist: coverage[toml] ; extra == "testing"
 Requires-Dist: pytest~=6.0 ; extra == "testing"
 Requires-Dist: pytest-cov ; extra == "testing"
 Project-URL: Source, https://github.com/epfl-theos/aiida-aurora
 Provides-Extra: docs
@@ -39,100 +43,102 @@
 # aiida-aurora
 
 AiiDA plugin for the Aurora project (autonomous robotic battery innovation platform).
 A collaboration between EPFL & Empa, within the BIG-MAP Stakeholder Initiative Call 2021.
 
 ## Repository contents
 
-* [`.github/`](.github/): [Github Actions](https://github.com/features/actions) configuration
-  * [`ci.yml`](.github/workflows/ci.yml): runs tests, checks test coverage and builds documentation at every new commit
-  * [`publish-on-pypi.yml`](.github/workflows/publish-on-pypi.yml): automatically deploy git tags to PyPI - just generate a [PyPI API token](https://pypi.org/help/#apitoken) for your PyPI account and add it to the `pypi_token` secret of your github repository
-* [`aiida_aurora/`](aiida_aurora/): The main source code of the plugin package
-  * [`data/`](aiida_aurora/data/): A new `DiffParameters` data class, used as input to the `DiffCalculation` `CalcJob` class
-  * [`calculations.py`](aiida_aurora/calculations.py): A new `DiffCalculation` `CalcJob` class
-  * [`cli.py`](aiida_aurora/cli.py): Extensions of the `verdi data` command line interface for the `DiffParameters` class
-  * [`helpers.py`](aiida_aurora/helpers.py): Helpers for setting up an AiiDA code for `diff` automatically
-  * [`parsers.py`](aiida_aurora/parsers.py): A new `Parser` for the `DiffCalculation`
-* [`docs/`](docs/): A documentation template ready for publication on [Read the Docs](http://aiida-diff.readthedocs.io/en/latest/)
-* [`examples/`](examples/): An example of how to submit a calculation using this plugin
-* [`tests/`](tests/): Basic regression tests using the [pytest](https://docs.pytest.org/en/latest/) framework (submitting a calculation, ...). Install `pip install -e .[testing]` and run `pytest`.
-* [`.coveragerc`](.coveragerc): Configuration of [coverage.py](https://coverage.readthedocs.io/en/latest) tool reporting which lines of your plugin are covered by tests
-* [`.gitignore`](.gitignore): Telling git which files to ignore
-* [`.pre-commit-config.yaml`](.pre-commit-config.yaml): Configuration of [pre-commit hooks](https://pre-commit.com/) that sanitize coding style and check for syntax errors. Enable via `pip install -e .[pre-commit] && pre-commit install`
-* [`.readthedocs.yml`](.readthedocs.yml): Configuration of documentation build for [Read the Docs](https://readthedocs.org/)
-* [`LICENSE`](LICENSE): License for your plugin
-* [`MANIFEST.in`](MANIFEST.in): Configure non-Python files to be included for publication on [PyPI](https://pypi.org/)
-* [`README.md`](README.md): This file
-* [`conftest.py`](conftest.py): Configuration of fixtures for [pytest](https://docs.pytest.org/en/latest/)
-* [`pytest.ini`](pytest.ini): Configuration of [pytest](https://docs.pytest.org/en/latest/) test discovery
-* [`setup.json`](setup.json): Plugin metadata for registration on [PyPI](https://pypi.org/) and the [AiiDA plugin registry](https://aiidateam.github.io/aiida-registry/) (including entry points)
-* [`setup.py`](setup.py): Installation script for pip / [PyPI](https://pypi.org/)
-
+- [`.github/`](.github/): [Github Actions](https://github.com/features/actions) configuration
+  - [`ci.yml`](.github/workflows/ci.yml): runs tests, checks test coverage and builds documentation at every new commit
+  - [`publish-on-pypi.yml`](.github/workflows/publish-on-pypi.yml): automatically deploy git tags to PyPI - just generate a [PyPI API token](https://pypi.org/help/#apitoken) for your PyPI account and add it to the `pypi_token` secret of your github repository
+- [`aiida_aurora/`](aiida_aurora/): The main source code of the plugin package
+  - [`data/`](aiida_aurora/data/): A new `DiffParameters` data class, used as input to the `DiffCalculation` `CalcJob` class
+  - [`calculations.py`](aiida_aurora/calculations.py): A new `DiffCalculation` `CalcJob` class
+  - [`cli.py`](aiida_aurora/cli.py): Extensions of the `verdi data` command line interface for the `DiffParameters` class
+  - [`helpers.py`](aiida_aurora/helpers.py): Helpers for setting up an AiiDA code for `diff` automatically
+  - [`parsers.py`](aiida_aurora/parsers.py): A new `Parser` for the `DiffCalculation`
+- [`docs/`](docs/): A documentation template ready for publication on [Read the Docs](http://aiida-diff.readthedocs.io/en/latest/)
+- [`examples/`](examples/): An example of how to submit a calculation using this plugin
+- [`tests/`](tests/): Basic regression tests using the [pytest](https://docs.pytest.org/en/latest/) framework (submitting a calculation, ...). Install `pip install -e .[testing]` and run `pytest`.
+- [`.coveragerc`](.coveragerc): Configuration of [coverage.py](https://coverage.readthedocs.io/en/latest) tool reporting which lines of your plugin are covered by tests
+- [`.gitignore`](.gitignore): Telling git which files to ignore
+- [`.pre-commit-config.yaml`](.pre-commit-config.yaml): Configuration of [pre-commit hooks](https://pre-commit.com/) that sanitize coding style and check for syntax errors. Enable via `pip install -e .[pre-commit] && pre-commit install`
+- [`.readthedocs.yml`](.readthedocs.yml): Configuration of documentation build for [Read the Docs](https://readthedocs.org/)
+- [`LICENSE`](LICENSE): License for your plugin
+- [`MANIFEST.in`](MANIFEST.in): Configure non-Python files to be included for publication on [PyPI](https://pypi.org/)
+- [`README.md`](README.md): This file
+- [`conftest.py`](conftest.py): Configuration of fixtures for [pytest](https://docs.pytest.org/en/latest/)
+- [`pytest.ini`](pytest.ini): Configuration of [pytest](https://docs.pytest.org/en/latest/) test discovery
+- [`setup.json`](setup.json): Plugin metadata for registration on [PyPI](https://pypi.org/) and the [AiiDA plugin registry](https://aiidateam.github.io/aiida-registry/) (including entry points)
+- [`setup.py`](setup.py): Installation script for pip / [PyPI](https://pypi.org/)
 
 See also the following video sequences from the 2019-05 AiiDA tutorial:
 
- * [aiida-diff setup.json](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=240s)
- * [run aiida-diff example calculation](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=403s)
- * [aiida-diff CalcJob plugin](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=685s)
- * [aiida-diff Parser plugin](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=936s)
- * [aiida-diff computer/code helpers](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1238s)
- * [aiida-diff input data (with validation)](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1353s)
- * [aiida-diff cli](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1621s)
- * [aiida-diff tests](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1931s)
- * [Adding your plugin to the registry](https://www.youtube.com/watch?v=760O2lDB-TM&t=112s)
- * [pre-commit hooks](https://www.youtube.com/watch?v=760O2lDB-TM&t=333s)
+- [aiida-diff setup.json](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=240s)
+- [run aiida-diff example calculation](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=403s)
+- [aiida-diff CalcJob plugin](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=685s)
+- [aiida-diff Parser plugin](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=936s)
+- [aiida-diff computer/code helpers](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1238s)
+- [aiida-diff input data (with validation)](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1353s)
+- [aiida-diff cli](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1621s)
+- [aiida-diff tests](https://www.youtube.com/watch?v=2CxiuiA1uVs&t=1931s)
+- [Adding your plugin to the registry](https://www.youtube.com/watch?v=760O2lDB-TM&t=112s)
+- [pre-commit hooks](https://www.youtube.com/watch?v=760O2lDB-TM&t=333s)
 
 For more information, see the [developer guide](https://aiida-diff.readthedocs.io/en/latest/developer_guide) of your plugin.
 
-
 ## Features
 
- * Add input files using `SinglefileData`:
-   ```python
-   SinglefileData = DataFactory('singlefile')
-   inputs['file1'] = SinglefileData(file='/path/to/file1')
-   inputs['file2'] = SinglefileData(file='/path/to/file2')
-   ```
-
- * Specify command line options via a python dictionary and `DiffParameters`:
-   ```python
-   d = { 'ignore-case': True }
-   DiffParameters = DataFactory('aurora')
-   inputs['parameters'] = DiffParameters(dict=d)
-   ```
-
- * `DiffParameters` dictionaries are validated using [voluptuous](https://github.com/alecthomas/voluptuous).
-   Find out about supported options:
-   ```python
-   DiffParameters = DataFactory('aurora')
-   print(DiffParameters.schema.schema)
-   ```
+- Add input files using `SinglefileData`:
+
+  ```python
+  SinglefileData = DataFactory('singlefile')
+  inputs['file1'] = SinglefileData(file='/path/to/file1')
+  inputs['file2'] = SinglefileData(file='/path/to/file2')
+  ```
+
+- Specify command line options via a python dictionary and `DiffParameters`:
+
+  ```python
+  d = { 'ignore-case': True }
+  DiffParameters = DataFactory('aurora')
+  inputs['parameters'] = DiffParameters(dict=d)
+  ```
+
+- `DiffParameters` dictionaries are validated using [voluptuous](https://github.com/alecthomas/voluptuous).
+  Find out about supported options:
+
+  ```python
+  DiffParameters = DataFactory('aurora')
+  print(DiffParameters.schema.schema)
+  ```
 
 ## Installation
 
 ```shell
 pip install aiida-aurora
 verdi quicksetup  # better to set up a new profile
 verdi plugin list aiida.calculations  # should now show your calclulation plugins
 ```
 
-
 ## Usage
 
 Here goes a complete example of how to submit a test calculation using this plugin.
 
 A quick demo of how to submit a calculation:
+
 ```shell
 verdi daemon start     # make sure the daemon is running
 cd examples
 ./example_01.py        # run test calculation
 verdi process list -a  # check record of calculation
 ```
 
 The plugin also includes verdi commands to inspect its data types:
+
 ```shell
 verdi data aurora list
 verdi data aurora export <PK>
 ```
 
 ## Development
 
@@ -145,11 +151,14 @@
 ```
 
 See the [developer guide](http://aiida-aurora.readthedocs.io/en/latest/developer_guide/index.html) for more information.
 
 ## License
 
 MIT
+
 ## Contact
 
-loris.ercole@epfl.ch
+francisco.ramirez@epfl.ch
+edan.bainglass@psi.ch
+giovanni.pizzi@psi.ch
```

