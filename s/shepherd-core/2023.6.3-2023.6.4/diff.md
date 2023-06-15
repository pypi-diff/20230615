# Comparing `tmp/shepherd_core-2023.6.3.tar.gz` & `tmp/shepherd_core-2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_core-2023.6.3.tar", last modified: Tue Jun  6 10:59:08 2023, max compression
+gzip compressed data, was "shepherd_core-2023.6.4.tar", last modified: Thu Jun 15 00:28:00 2023, max compression
```

## Comparing `shepherd_core-2023.6.3.tar` & `shepherd_core-2023.6.4.tar`

### file list

```diff
@@ -1,108 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-06 10:59:08.283409 shepherd_core-2023.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/calibration_hw_def.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/commons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/data_models/base/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/cal_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/shepherd.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/base/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/data_models/content/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/energy_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/energy_environment_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/firmware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/firmware_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_harvester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_source_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/doc_virtual_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.271409 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/observer_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/experiment/target_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.275409 shepherd_core-2023.6.3/shepherd_core/data_models/task/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/emulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/firmware_mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/harvest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/observer_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/programming.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/task/testbed_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.275409 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/cape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/cape_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/gpio_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/mcu.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/mcu_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/observer_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/target_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/testbed.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/data_models/testbed/testbed_fixture.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.275409 shepherd_core-2023.6.3/shepherd_core/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/vsource/virtual_converter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/vsource/virtual_harvester_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/vsource/virtual_source_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/shepherd_core/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/shepherd_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:59:08.000000 shepherd_core-2023.6.3/shepherd_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.275409 shepherd_core-2023.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/tests/data_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_data_faulty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_meas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_meas_faulty1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_cal_meas_faulty2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_emulator.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_experiment_alternative.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_harvester.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_testbed.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/example_config_virtsource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_content_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_content_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_experiment_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_task_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_task_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_testbed_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/data_models/test_testbed_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_cal_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/test_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:59:08.279409 shepherd_core-2023.6.3/tests/vsource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/vsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/vsource/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/vsource/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-06 10:58:57.000000 shepherd_core-2023.6.3/tests/vsource/test_harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.237828 shepherd_core-2023.6.4/shepherd_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/calibration_hw_def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/commons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.237828 shepherd_core-2023.6.4/shepherd_core/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.237828 shepherd_core-2023.6.4/shepherd_core/data_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/cal_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/shepherd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/base/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.241828 shepherd_core-2023.6.4/shepherd_core/data_models/content/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/energy_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/energy_environment_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/firmware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/firmware_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_harvester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_harvester_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_source_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/doc_virtual_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.241828 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/observer_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/experiment/target_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.245828 shepherd_core-2023.6.4/shepherd_core/data_models/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/emulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/firmware_mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/harvest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/observer_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/task/testbed_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.249828 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/cape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/cape_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/gpio_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/mcu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/mcu_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/observer_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/target_fixture.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/testbed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/data_models/testbed/testbed_fixture.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.249828 shepherd_core-2023.6.4/shepherd_core/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/fw_tools/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/fw_tools/patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20847 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.249828 shepherd_core-2023.6.4/shepherd_core/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10497 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/vsource/virtual_converter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/vsource/virtual_harvester_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/vsource/virtual_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/shepherd_core/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/shepherd_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:28:00.000000 shepherd_core-2023.6.4/shepherd_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.249828 shepherd_core-2023.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/tests/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_data_faulty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_meas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_meas_faulty1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_cal_meas_faulty2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_emulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_experiment_alternative.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_harvester.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_testbed.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/example_config_virtsource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_content_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_content_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_experiment_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_task_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_task_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_testbed_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/data_models/test_testbed_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/tests/fw_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/fw_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/fw_tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/fw_tools/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/fw_tools/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_cal_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:28:00.253828 shepherd_core-2023.6.4/tests/vsource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/vsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/vsource/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/vsource/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-15 00:27:50.000000 shepherd_core-2023.6.4/tests/vsource/test_harvester.py
```

### Comparing `shepherd_core-2023.6.3/PKG-INFO` & `shepherd_core-2023.6.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_core
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: elf
 Provides-Extra: dev
 Provides-Extra: test
 
 # Shepherd - Core
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
 [![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
@@ -46,7 +47,16 @@
 ---
 
 **Main Project**: [https://github.com/orgua/shepherd](https://github.com/orgua/shepherd)
 
 **Source Code**: [https://github.com/orgua/shepherd-datalib](https://github.com/orgua/shepherd-datalib)
 
 ---
+
+This library allows to
+
+- read and write shepherds h5-files
+- create experiments (all data-models included)
+- simulate the virtual source
+- work with target-firmwares
+
+see [examples](/examples) for more details.
```

### Comparing `shepherd_core-2023.6.3/setup.cfg` & `shepherd_core-2023.6.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 	pyYAML
 	chromalog
 	pydantic[email]<2.0.0
 	tqdm
 	scipy
 
 [options.extras_require]
+elf = 
+	pwntools
 dev = 
 	black
 	pylint
 	flake8
 	twine
 	pre-commit
 	pyright
```

### Comparing `shepherd_core-2023.6.3/shepherd_core/__init__.py` & `shepherd_core-2023.6.4/shepherd_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .data_models.task import Compression
 from .logger import get_verbose_level
 from .logger import logger
 from .logger import set_verbose_level
 from .reader import BaseReader
 from .writer import BaseWriter
 
-__version__ = "2023.6.3"
+__version__ = "2023.6.4"
 
 __all__ = [
     "BaseReader",
     "BaseWriter",
     "get_verbose_level",
     "set_verbose_level",
     "logger",
```

### Comparing `shepherd_core-2023.6.3/shepherd_core/calibration_hw_def.py` & `shepherd_core-2023.6.4/shepherd_core/calibration_hw_def.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/__init__.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/base/cal_measurement.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/base/cal_measurement.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         dcal = CalibrationHarvester().dict()
         for key in dv.keys():
             dcal[key] = meas_to_cal(self[key], f"hrv_{key}")
         return CalibrationHarvester(**dcal)
 
 
 class CalMeasurementEmulator(ShpModel):
-    dac_V_A: CalMeasPairs
+    dac_V_A: CalMeasPairs  # TODO: why not V_dac_A or V_dac_a
     dac_V_B: CalMeasPairs
     adc_C_A: CalMeasPairs
     adc_C_B: CalMeasPairs
 
     def to_cal(self) -> CalibrationEmulator:
         dv = self.dict()
         dcal = CalibrationEmulator().dict()
```

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/base/calibration.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/base/calibration.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/base/content.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/base/content.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/base/fixture.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/base/fixture.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/base/shepherd.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/base/shepherd.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 
 
 def path2str(dumper, data):
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data.as_posix()))
 
 
 def time2int(dumper, data):
-    return dumper.represent_scalar("tag:yaml.org,2002:int", str(data.seconds))
+    return dumper.represent_scalar(
+        "tag:yaml.org,2002:int", str(int(data.total_seconds()))
+    )
 
 
 yaml.add_representer(pathlib.PosixPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.WindowsPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.Path, path2str, SafeDumper)
 yaml.add_representer(timedelta, time2int, SafeDumper)
```

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/content/energy_environment.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/content/energy_environment.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/content/energy_environment_fixture.yaml` & `shepherd_core-2023.6.4/shepherd_core/data_models/content/energy_environment_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/content/firmware.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/content/firmware.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/content/firmware_fixture.yaml` & `shepherd_core-2023.6.4/shepherd_core/data_models/content/firmware_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_harvester.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_harvester.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_harvester_fixture.yaml` & `shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_harvester_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_source.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/content/virtual_source_fixture.yaml` & `shepherd_core-2023.6.4/shepherd_core/data_models/content/virtual_source_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/doc_virtual_source.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/doc_virtual_source.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/experiment/__init__.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/experiment/experiment.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/experiment/experiment.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     # targets
     target_configs: conlist(item_type=TargetConfig, min_items=1, max_items=64)
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         cls.validate_targets(values)
         cls.validate_observers(values)
+        if values.get("duration") and values["duration"].total_seconds() < 0:
+            raise ValueError("Duration of experiment can't be negative.")
         return values
 
     @staticmethod
     def validate_targets(values: dict) -> None:
         target_ids = []
         custom_ids = []
         for _config in values.get("target_configs"):
```

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/experiment/observer_features.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/experiment/observer_features.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,26 +19,31 @@
     """
 
     intermediate_voltage: bool = False
     # ⤷ for EMU: record buffer capacitor instead of output (good for V_out = const)
     #            this also includes current!
 
     # time
-    delay: conint(ge=0) = 0
-    duration: conint(ge=0) = timedelta(days=200).seconds
+    delay: timedelta = 0  # seconds
+    duration: Optional[timedelta] = None  # till EOF
 
     # post-processing
     calculate_power: bool = False
     samplerate: conint(ge=10, le=100_000) = 100_000  # down-sample
     discard_current: bool = False
     discard_voltage: bool = False
     # ⤷ reduce file-size by omitting current / voltage
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
+        if values.get("delay") and values["delay"].total_seconds() < 0:
+            raise ValueError("Delay can't be negative.")
+        if values.get("duration") and values["duration"].total_seconds() < 0:
+            raise ValueError("Duration can't be negative.")
+
         discard_all = values.get("discard_current") and values.get("discard_voltage")
         if not values.get("calculate_power") and discard_all:
             raise ValueError(
                 "Error in config -> tracing enabled, but output gets discarded"
             )
         if values.get("calculate_power"):
             raise ValueError("postprocessing not implemented ATM")
@@ -53,27 +58,31 @@
     # initial recording
     mask: conint(ge=0, lt=2**10) = 0b11_1111_1111  # all
     # ⤷ TODO: custom mask not implemented
     gpios: Optional[conlist(item_type=GPIO, min_items=1, max_items=10)]  # = all
     # ⤷ TODO: list of GPIO to build mask, one of both should be internal
 
     # time
-    delay: conint(ge=0) = 0  # seconds
-    duration: conint(ge=0) = timedelta(days=200).seconds
+    delay: timedelta = 0  # seconds
+    duration: Optional[timedelta] = None  # till EOF
 
     # post-processing,
     uart_decode: bool = False  # todo: is currently done online by system-service
     uart_pin: GPIO = GPIO(name="GPIO8")
     uart_baudrate: conint(ge=2_400, le=921_600) = 115_200
     # TODO: add a "discard_gpio" (if only uart is wanted)
 
     @root_validator(pre=False)
     def post_validation(cls, values: dict) -> dict:
         if values.get("mask") == 0:
             raise ValueError("Error in config -> tracing enabled but mask is 0")
+        if values.get("delay") and values["delay"].total_seconds() < 0:
+            raise ValueError("Delay can't be negative.")
+        if values.get("duration") and values["duration"].total_seconds() < 0:
+            raise ValueError("Duration can't be negative.")
         return values
 
 
 class GpioLevel(str, Enum):
     low = "L"
     high = "H"
     toggle = "X"  # TODO: not the smartest decision for writing a converter
```

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/experiment/target_config.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/experiment/target_config.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/task/emulation.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/task/emulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,16 @@
         # TODO: limit paths
         has_start = values.get("time_start") is not None
         # add local timezone-data
         if has_start and values["time_start"].tzinfo is None:
             values["time_start"] = values["time_start"].astimezone()
         if has_start and values.get("time_start") < datetime.now().astimezone():
             raise ValueError("Start-Time for Emulation can't be in the past.")
+        if values.get("duration") and values["duration"].total_seconds() < 0:
+            raise ValueError("Task-Duration can't be negative.")
         if isinstance(values.get("voltage_aux"), str) and values.get(
             "voltage_aux"
         ) not in [
             "main",
             "buffer",
         ]:
             raise ValueError(
```

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/task/firmware_mod.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/task/firmware_mod.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/task/harvest.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/task/harvest.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,8 +56,10 @@
         # TODO: limit paths
         has_start = values.get("time_start") is not None
         if has_start and values["time_start"].tzinfo is None:
             # add local timezone-data
             values["time_start"] = values["time_start"].astimezone()
         if has_start and values["time_start"] < datetime.now().astimezone():
             raise ValueError("Start-Time for Harvest can't be in the past.")
+        if values.get("duration") and values["duration"].total_seconds() < 0:
+            raise ValueError("Task-Duration can't be negative.")
         return values
```

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/task/observer_tasks.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/task/observer_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/task/programming.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/task/programming.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/task/testbed_tasks.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/task/testbed_tasks.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/__init__.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/__init__.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/cape.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/cape.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/cape_fixture.yaml` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/cape_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/gpio.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/gpio.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/gpio_fixture.yaml` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/gpio_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/mcu.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/mcu.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/mcu_fixture.yaml` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/mcu_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/observer.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/observer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/observer_fixture.yaml` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/observer_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/target.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/target.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/target_fixture.yaml` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/target_fixture.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/data_models/testbed/testbed.py` & `shepherd_core-2023.6.4/shepherd_core/data_models/testbed/testbed.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,16 @@
             raise ValueError("Observers-MAC-Address used more than once in Testbed")
         if len(capes) > len(set(capes)):
             raise ValueError("Cape used more than once in Testbed")
         if len(targets) > len(set(targets)):
             raise ValueError("Target used more than once in Testbed")
         if len(eth_ports) > len(set(eth_ports)):
             raise ValueError("Observers-Ethernet-Port used more than once in Testbed")
-
+        if values.get("prep_duration") and values["prep_duration"].total_seconds() < 0:
+            raise ValueError("Task-Duration can't be negative.")
         if not values.get("shared_storage"):
             raise ValueError("Only shared-storage-option is implemented")
         return values
 
     def get_observer(self, target_id: int) -> Observer:
         for _observer in self.observers:
             has_tgt_a = _observer.target_a is not None
```

### Comparing `shepherd_core-2023.6.3/shepherd_core/logger.py` & `shepherd_core-2023.6.4/shepherd_core/logger.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/reader.py` & `shepherd_core-2023.6.4/shepherd_core/reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/vsource/virtual_converter_model.py` & `shepherd_core-2023.6.4/shepherd_core/vsource/virtual_converter_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/vsource/virtual_harvester_model.py` & `shepherd_core-2023.6.4/shepherd_core/vsource/virtual_harvester_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/vsource/virtual_source_model.py` & `shepherd_core-2023.6.4/shepherd_core/vsource/virtual_source_model.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/shepherd_core/writer.py` & `shepherd_core-2023.6.4/shepherd_core/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 
 # copy of core/models/base/shepherd - needed also here
 def path2str(dumper, data):
     return dumper.represent_scalar("tag:yaml.org,2002:str", str(data.as_posix()))
 
 
 def time2int(dumper, data):
-    return dumper.represent_scalar("tag:yaml.org,2002:int", str(data.seconds))
+    return dumper.represent_scalar(
+        "tag:yaml.org,2002:int", str(int(data.total_seconds()))
+    )
 
 
 yaml.add_representer(pathlib.PosixPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.WindowsPath, path2str, SafeDumper)
 yaml.add_representer(pathlib.Path, path2str, SafeDumper)
 yaml.add_representer(timedelta, time2int, SafeDumper)
 
@@ -92,21 +94,24 @@
     def __init__(
         self,
         file_path: Path,
         mode: Optional[str] = None,
         datatype: Union[str, EnergyDType, None] = None,
         window_samples: Optional[int] = None,
         cal_data: Union[CalSeries, CalEmu, CalHrv, None] = None,
-        compression: Compression = Compression.default,
+        compression: Optional[Compression] = Compression.default,
         modify_existing: bool = False,
         force_overwrite: bool = False,
         verbose: Optional[bool] = True,
     ):
         self._modify = modify_existing
-        self._compression = c_translate[compression.value]
+        if compression is not None:
+            self._compression = c_translate[compression.value]
+        else:
+            self._compression = None
 
         if not hasattr(self, "_logger"):
             self._logger: logging.Logger = logging.getLogger("SHPCore.Writer")
         # -> logger gets configured in reader()
 
         if self._modify or force_overwrite or not file_path.exists():
             self.file_path: Path = file_path.resolve()
```

### Comparing `shepherd_core-2023.6.3/shepherd_core.egg-info/PKG-INFO` & `shepherd_core-2023.6.4/shepherd_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-core
-Version: 2023.6.3
+Version: 2023.6.4
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-core/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: elf
 Provides-Extra: dev
 Provides-Extra: test
 
 # Shepherd - Core
 
 [![PyPiVersion](https://img.shields.io/pypi/v/shepherd_core.svg)](https://pypi.org/project/shepherd_core)
 [![Pytest](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml/badge.svg)](https://github.com/orgua/shepherd-datalib/actions/workflows/python-app.yml)
@@ -46,7 +47,16 @@
 ---
 
 **Main Project**: [https://github.com/orgua/shepherd](https://github.com/orgua/shepherd)
 
 **Source Code**: [https://github.com/orgua/shepherd-datalib](https://github.com/orgua/shepherd-datalib)
 
 ---
+
+This library allows to
+
+- read and write shepherds h5-files
+- create experiments (all data-models included)
+- simulate the virtual source
+- work with target-firmwares
+
+see [examples](/examples) for more details.
```

### Comparing `shepherd_core-2023.6.3/shepherd_core.egg-info/SOURCES.txt` & `shepherd_core-2023.6.4/shepherd_core.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 ./shepherd_core/data_models/testbed/mcu_fixture.yaml
 ./shepherd_core/data_models/testbed/observer.py
 ./shepherd_core/data_models/testbed/observer_fixture.yaml
 ./shepherd_core/data_models/testbed/target.py
 ./shepherd_core/data_models/testbed/target_fixture.yaml
 ./shepherd_core/data_models/testbed/testbed.py
 ./shepherd_core/data_models/testbed/testbed_fixture.yaml
+./shepherd_core/fw_tools/__init__.py
+./shepherd_core/fw_tools/converter.py
+./shepherd_core/fw_tools/patcher.py
 ./shepherd_core/vsource/__init__.py
 ./shepherd_core/vsource/virtual_converter_model.py
 ./shepherd_core/vsource/virtual_harvester_model.py
 ./shepherd_core/vsource/virtual_source_model.py
 ./tests/__init__.py
 ./tests/conftest.py
 ./tests/test_cal_hw.py
@@ -78,14 +81,18 @@
 ./tests/data_models/test_content_models.py
 ./tests/data_models/test_examples.py
 ./tests/data_models/test_experiment_models.py
 ./tests/data_models/test_task_generation.py
 ./tests/data_models/test_task_models.py
 ./tests/data_models/test_testbed_fixtures.py
 ./tests/data_models/test_testbed_models.py
+./tests/fw_tools/__init__.py
+./tests/fw_tools/conftest.py
+./tests/fw_tools/test_converter.py
+./tests/fw_tools/test_patcher.py
 ./tests/vsource/__init__.py
 ./tests/vsource/conftest.py
 ./tests/vsource/test_converter.py
 ./tests/vsource/test_harvester.py
 shepherd_core.egg-info/PKG-INFO
 shepherd_core.egg-info/SOURCES.txt
 shepherd_core.egg-info/dependency_links.txt
```

### Comparing `shepherd_core-2023.6.3/tests/conftest.py` & `shepherd_core-2023.6.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/example_cal_data.yaml` & `shepherd_core-2023.6.4/tests/data_models/example_cal_data.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 datatype: CalibrationCape
-comment: sheep0
 parameters:
+  host: sheep0
+  cape: xyz1
   emulator:
     adc_C_A:
       gain: 2.2306053900482405e-07
       offset: -0.0026222400965270985
     adc_C_B:
       gain: 2.2306053900482405e-07
       offset: -0.0026222400965270985
```

### Comparing `shepherd_core-2023.6.3/tests/data_models/example_cal_data_faulty.yaml` & `shepherd_core-2023.6.4/tests/data_models/example_cal_data_faulty.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/example_cal_meas.yaml` & `shepherd_core-2023.6.4/tests/data_models/example_cal_meas.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ---
 datatype: CalMeasurementCape
-comment: sheep0
 parameters:
+  host: sheep0
+  cape: xyz1
   emulator:
     adc_C_A:
     - reference_si: 1.0e-05
       shepherd_raw: 647.0605606009001
     - reference_si: 3.0e-05
       shepherd_raw: 759.2687092956633
     - reference_si: 0.0001
```

### Comparing `shepherd_core-2023.6.3/tests/data_models/example_cal_meas_faulty1.yaml` & `shepherd_core-2023.6.4/tests/data_models/example_cal_meas_faulty1.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/example_cal_meas_faulty2.yaml` & `shepherd_core-2023.6.4/tests/data_models/example_cal_meas_faulty2.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/example_config_emulator.yaml` & `shepherd_core-2023.6.4/tests/data_models/example_config_emulator.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/example_config_harvester.yaml` & `shepherd_core-2023.6.4/tests/data_models/example_config_harvester.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/example_config_virtsource.yaml` & `shepherd_core-2023.6.4/tests/data_models/example_config_virtsource.yaml`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/test_base_models.py` & `shepherd_core-2023.6.4/tests/data_models/test_base_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/test_content_fixtures.py` & `shepherd_core-2023.6.4/tests/data_models/test_content_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/test_content_models.py` & `shepherd_core-2023.6.4/tests/data_models/test_content_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/test_examples.py` & `shepherd_core-2023.6.4/tests/data_models/test_examples.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/test_experiment_models.py` & `shepherd_core-2023.6.4/tests/data_models/test_experiment_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/test_task_generation.py` & `shepherd_core-2023.6.4/tests/data_models/test_task_generation.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/test_task_models.py` & `shepherd_core-2023.6.4/tests/data_models/test_task_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 
 def test_task_model_hrv_duration() -> None:
     hrv = HarvestTask(
         output_path="./here",
         duration=42,
     )
-    assert hrv.duration.seconds == 42
+    assert hrv.duration.total_seconds() == 42
 
 
 def test_task_model_hrv_too_late() -> None:
     with pytest.raises(ValueError):
         HarvestTask(
             output_path="./here",
             time_start="1984-01-01 11:12:13",
```

### Comparing `shepherd_core-2023.6.3/tests/data_models/test_testbed_fixtures.py` & `shepherd_core-2023.6.4/tests/data_models/test_testbed_fixtures.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/data_models/test_testbed_models.py` & `shepherd_core-2023.6.4/tests/data_models/test_testbed_models.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/test_cal_hw.py` & `shepherd_core-2023.6.4/tests/test_cal_hw.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/test_reader.py` & `shepherd_core-2023.6.4/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/test_writer.py` & `shepherd_core-2023.6.4/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/vsource/conftest.py` & `shepherd_core-2023.6.4/tests/vsource/conftest.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/vsource/test_converter.py` & `shepherd_core-2023.6.4/tests/vsource/test_converter.py`

 * *Files identical despite different names*

### Comparing `shepherd_core-2023.6.3/tests/vsource/test_harvester.py` & `shepherd_core-2023.6.4/tests/vsource/test_harvester.py`

 * *Files identical despite different names*

