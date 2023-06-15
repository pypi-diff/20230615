# Comparing `tmp/ParMan-0.2.0.tar.gz` & `tmp/Parman-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ParMan-0.2.0.tar", last modified: Sun May  7 14:49:42 2023, max compression
+gzip compressed data, was "Parman-0.3.0.tar", last modified: Thu Jun 15 10:55:22 2023, max compression
```

## Comparing `ParMan-0.2.0.tar` & `Parman-0.3.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.722784 ParMan-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-07 14:49:33.000000 ParMan-0.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-07 14:49:33.000000 ParMan-0.2.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-07 14:49:33.000000 ParMan-0.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.710784 ParMan-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-07 14:49:33.000000 ParMan-0.2.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-07 14:49:33.000000 ParMan-0.2.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-07 14:49:33.000000 ParMan-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-07 14:49:33.000000 ParMan-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-07 14:49:33.000000 ParMan-0.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-07 14:49:33.000000 ParMan-0.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-07 14:49:33.000000 ParMan-0.2.0/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-07 14:49:33.000000 ParMan-0.2.0/HEADER
--rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-05-07 14:49:42.722784 ParMan-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-07 14:49:33.000000 ParMan-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/demc/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     6485 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/demc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4625 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/linreg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5231 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/demc/naivemc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/inspiration/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/inspiration/plastic/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/alumina.json
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/ibuprofen.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8333 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/plastic.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/inspiration/plastic/run
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/jobdemo/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     6604 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/jobdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.710784 ParMan-0.2.0/demos/jobdemo/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/jobdemo/templates/boot/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/boot/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/boot/run
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/boot/submit.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/jobdemo/templates/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/compute/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      579 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/compute/run
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/compute/submit.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.714784 ParMan-0.2.0/demos/jobdemo/templates/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/sample/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      837 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/sample/run
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/sample/submit.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/demos/jobdemo/templates/train/
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/train/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/train/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/train/run
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/jobdemo/templates/train/submit.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1080 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/mindmutable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/scheduledemo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-05-07 14:49:33.000000 ParMan-0.2.0/demos/waitdemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-07 14:49:33.000000 ParMan-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 14:49:42.722784 ParMan-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.710784 ParMan-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/ParMan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/ParMan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/parman/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 14:49:42.000000 ParMan-0.2.0/src/parman/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/parman/clerks/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/clerks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/clerks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/clerks/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/clerks/localtemp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)    19453 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/metafunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/parman/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/dry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/future.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/parsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/runners/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.718784 ParMan-0.2.0/src/parman/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/scripts/sbatch_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/treeleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/waitfuture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-07 14:49:33.000000 ParMan-0.2.0/src/parman/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:49:42.722784 ParMan-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    71045 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/jobdemo-results.sha256
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_metafunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_treeleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-07 14:49:33.000000 ParMan-0.2.0/tests/test_waitfuture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.725360 Parman-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-15 10:55:02.000000 Parman-0.3.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-15 10:55:02.000000 Parman-0.3.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 10:55:02.000000 Parman-0.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-15 10:55:02.000000 Parman-0.3.0/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 10:55:02.000000 Parman-0.3.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-15 10:55:02.000000 Parman-0.3.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 10:55:02.000000 Parman-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 10:55:02.000000 Parman-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-15 10:55:02.000000 Parman-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 10:55:02.000000 Parman-0.3.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-15 10:55:02.000000 Parman-0.3.0/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-06-15 10:55:22.725360 Parman-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-15 10:55:02.000000 Parman-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/demc/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6485 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/demc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4625 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/linreg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5231 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/naivemc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/inspiration/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/inspiration/plastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/alumina.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/ibuprofen.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8333 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/plastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/run
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/jobdemo/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6604 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/jobdemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.713360 Parman-0.3.0/demos/jobdemo/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/jobdemo/templates/boot/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/boot/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/boot/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/boot/submit.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/jobdemo/templates/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/compute/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/compute/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/compute/submit.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/jobdemo/templates/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/sample/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/sample/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/sample/submit.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/demos/jobdemo/templates/train/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/train/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/train/jobinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/train/run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/train/submit.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1080 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/mindmutable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/scheduledemo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/waitdemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-15 10:55:02.000000 Parman-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 10:55:22.725360 Parman-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.713360 Parman-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/Parman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/parman/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 10:55:22.000000 Parman-0.3.0/src/parman/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/parman/clerks/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/clerks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/clerks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/clerks/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/clerks/localtemp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/closure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/metafunc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/parman/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/dry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/parsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/parman/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/scripts/sbatch_wait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/treeleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/waitfuture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.725360 Parman-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81848 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/jobdemo-results.sha256
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_metafunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_runners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_treeleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_waitfuture.py
```

### Comparing `ParMan-0.2.0/.github/workflows/pypi.yaml` & `Parman-0.3.0/.github/workflows/pypi.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # See https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
 
 name: pypi upload
 
-on: push
+on:
+  push:
+    branches:
+    - main
+    tags:
+    - 'v*'
 
 jobs:
   build-n-publish:
     name: Build and publish
     runs-on: ubuntu-latest
 
     steps:
```

### Comparing `ParMan-0.2.0/.github/workflows/pytest.yaml` & `Parman-0.3.0/.github/workflows/pytest.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 name: pytest
 
 on:
   push:
+    branches:
+     - main
+    tags-ignore:
+      - '**'
   pull_request:
 
 jobs:
   tests:
     name: "Python ${{ matrix.py }}"
     runs-on: "ubuntu-latest"
```

### Comparing `ParMan-0.2.0/.pre-commit-config.yaml` & `Parman-0.3.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -25,10 +25,14 @@
   hooks:
     - id: remove-crlf
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
     - id: black
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: 'v0.0.265'
+  rev: 'v0.0.269'
   hooks:
     - id: ruff
+- repo: https://github.com/python-jsonschema/check-jsonschema
+  rev: 0.23.0
+  hooks:
+    - id: check-github-workflows
```

### Comparing `ParMan-0.2.0/CHANGELOG.md` & `Parman-0.3.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,35 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.0] - 2023-06-15
+
+### Added
+
+- When `kwargs.json` is manually filled with `null`, it is refreshed under the assumption
+  that the existing results are consistent with the new `kwargs.json` file.
+  This is useful when one is refactoring workflows and one wants to reuse some results of
+  a previous run.
+- When `kwargs.sha256` is manually removed, it is refreshed for the same reasons as in the
+  previous point.
+
+### Fixed
+
+- Fixed mistake in `jobdemo` example (writing `result.extra`).
+- Add support for `None` return value in jobs.
+
+### Changed
+
+- Update [`cattrs`](https://github.com/python-attrs/cattrs) dependency to `>=23.1.2`.
+
+
 ## [0.2.0] - 2023-05-07
 
 ### Added
 
 - A pure Python usage example (Differential Evolution Monte Carlo).
 - The `parman-sbatch-wait` script to facilitate running workflow jobs on a Slurm cluster.
 - Support for optional arguments in `jobinfo.py`.
```

### Comparing `ParMan-0.2.0/COPYING` & `Parman-0.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/HEADER` & `Parman-0.3.0/src/parman/clerks/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
+"""Mapping between local job files and global storage layout."""
```

### Comparing `ParMan-0.2.0/PKG-INFO` & `Parman-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: ParMan
-Version: 0.2.0
-Summary: ParMan extends Python concurrent.futures to facilitate parallel workflows
+Name: Parman
+Version: 0.3.0
+Summary: Parman extends Python concurrent.futures to facilitate parallel workflows
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -182,22 +182,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 [![pytest](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml)
 [![PyPI Upload](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml)
-[![PyPI Version](https://img.shields.io/pypi/v/parman)](https://pypi.org/project/ParMan/)
+[![PyPI Version](https://img.shields.io/pypi/v/parman)](https://pypi.org/project/Parman/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parman)
+![LGPL-3 License](https://img.shields.io/github/license/reproducible-reporting/parman)
 
 # Parman
 
-At this stage, ParMan is an experimental project, so expect a rocky road ahead.
+At this stage, Parman is an experimental project, so expect a rocky road ahead.
 
-The goal of ParMan is to extend `concurrent.futures` (and compatible implementations)
+The goal of Parman is to extend `concurrent.futures` (and compatible implementations)
 with features that facilitate a transparent implementation of workflows.
 
 - `WaitFuture`: a Future subclass that is "finished" after its dependencies have finished.
   (To be created with `WaitGraph.submit`, which never blocks.)
 - `ScheduledFuture`: a Future subclass that submits a Future after its dependencies have finished.
   (To be created with `Scheduler.submit`, which never blocks.)
 - Various `Runner` classes, similar to Executors, which dispatch function calls elsewhere.
@@ -237,23 +238,23 @@
 ```bash
 python -m pip install parman
 ```
 
 ### Examples
 
 At this stage, there is no documentation as such.
-If you want to learn how to use ParMan, check out the [demos](demos/).
+If you want to learn how to use Parman, check out the [demos](demos/).
 If you want to understand the internals, read the source and the docstrings.
 
 
 ## Non-goals
 
 - Support for Dask, because:
   1. The Dask `Future` does not subclass from `concurrent.futures.Future`.
-     Supporting dask would imply a lot of extra boilerplate code in ParMan.
+     Supporting dask would imply a lot of extra boilerplate code in Parman.
   2. The Dask `Future` implements only a subset of `concurrent.futures.Future`.
   3. Dask Distributed has a large memory and time overhead.
 
 
 ## Plans
 
 - Simplify usage.
```

### Comparing `ParMan-0.2.0/README.md` & `Parman-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [![pytest](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml)
 [![PyPI Upload](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml)
-[![PyPI Version](https://img.shields.io/pypi/v/parman)](https://pypi.org/project/ParMan/)
+[![PyPI Version](https://img.shields.io/pypi/v/parman)](https://pypi.org/project/Parman/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parman)
+![LGPL-3 License](https://img.shields.io/github/license/reproducible-reporting/parman)
 
 # Parman
 
-At this stage, ParMan is an experimental project, so expect a rocky road ahead.
+At this stage, Parman is an experimental project, so expect a rocky road ahead.
 
-The goal of ParMan is to extend `concurrent.futures` (and compatible implementations)
+The goal of Parman is to extend `concurrent.futures` (and compatible implementations)
 with features that facilitate a transparent implementation of workflows.
 
 - `WaitFuture`: a Future subclass that is "finished" after its dependencies have finished.
   (To be created with `WaitGraph.submit`, which never blocks.)
 - `ScheduledFuture`: a Future subclass that submits a Future after its dependencies have finished.
   (To be created with `Scheduler.submit`, which never blocks.)
 - Various `Runner` classes, similar to Executors, which dispatch function calls elsewhere.
@@ -51,23 +52,23 @@
 ```bash
 python -m pip install parman
 ```
 
 ### Examples
 
 At this stage, there is no documentation as such.
-If you want to learn how to use ParMan, check out the [demos](demos/).
+If you want to learn how to use Parman, check out the [demos](demos/).
 If you want to understand the internals, read the source and the docstrings.
 
 
 ## Non-goals
 
 - Support for Dask, because:
   1. The Dask `Future` does not subclass from `concurrent.futures.Future`.
-     Supporting dask would imply a lot of extra boilerplate code in ParMan.
+     Supporting dask would imply a lot of extra boilerplate code in Parman.
   2. The Dask `Future` implements only a subset of `concurrent.futures.Future`.
   3. Dask Distributed has a large memory and time overhead.
 
 
 ## Plans
 
 - Simplify usage.
```

### Comparing `ParMan-0.2.0/demos/demc/README.md` & `Parman-0.3.0/demos/demc/README.md`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/demos/demc/demc.py` & `Parman-0.3.0/demos/demc/demc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/demos/demc/linreg.py` & `Parman-0.3.0/demos/demc/linreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/demos/demc/naivemc.py` & `Parman-0.3.0/demos/demc/naivemc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/demos/inspiration/plastic/README.md` & `Parman-0.3.0/demos/inspiration/plastic/README.md`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/demos/inspiration/plastic/alumina.json` & `Parman-0.3.0/demos/inspiration/plastic/alumina.json`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/demos/inspiration/plastic/ibuprofen.xyz` & `Parman-0.3.0/demos/inspiration/plastic/ibuprofen.xyz`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/demos/inspiration/plastic/plastic.py` & `Parman-0.3.0/demos/inspiration/plastic/plastic.py`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/demos/jobdemo/jobdemo.py` & `Parman-0.3.0/demos/jobdemo/jobdemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,26 +42,26 @@
     if args.queue:
         job.script = "submit.sh"
     workflow(runner, args.pause)
 
 
 def parse_args() -> argparse.Namespace:
     """Parse the command-line arguments."""
-    parser = argparse.ArgumentParser("ParMan demo with job scripts")
+    parser = argparse.ArgumentParser("Parman demo with job scripts")
     parser.add_argument(
         "framework",
         help="The framework to execute the workflow",
         choices=["dry", "serial", "threads", "processes", "parsl-local", "parsl-slurm"],
     )
     parser.add_argument(
         "-s",
         "--schedule",
         default=False,
         action="store_true",
-        help="Enable the ParMan scheduler, not relevant for serial and dry.",
+        help="Enable the Parman scheduler, not relevant for serial and dry.",
     )
     parser.add_argument(
         "-p", "--pause", default=1.0, type=float, help="The time to pause in each job, in seconds."
     )
     parser.add_argument(
         "-t",
         "--in-temp",
```

### Comparing `ParMan-0.2.0/demos/jobdemo/templates/boot/run` & `Parman-0.3.0/demos/jobdemo/templates/boot/run`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/demos/jobdemo/templates/compute/run` & `Parman-0.3.0/demos/jobdemo/templates/compute/run`

 * *Files 10% similar despite different names*

```diff
@@ -3,12 +3,13 @@
 # Extract config file from json with Python inline code
 FN_CONFIG=$(python -c 'import json; print(json.load(open("kwargs.json"))["config"])')
 PAUSE=$(python -c 'import json; print(json.load(open("kwargs.json"))["pause"])')
 # Alternative tools doing the same, which need to be installed:
 # FN_CONFIG=$(jq -r .config kwargs.json)
 # FN_CONFIG=$(gojq -r .config kwargs.json)
 # FN_CONFIG=$(jql -r '."config"' kwargs.json)
+# Note that the -r option is needed to get rid of JSON string quotes.
 
 echo "Computing some result"
 echo "Did something with ${FN_CONFIG}" > computation.out
 sleep ${PAUSE}
 echo '"computation.out"' > result.json
```

### Comparing `ParMan-0.2.0/demos/jobdemo/templates/sample/run` & `Parman-0.3.0/demos/jobdemo/templates/sample/run`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 
 import json
-import os
 import time
+from pathlib import Path
 
 
 def main():
     print("loading kwargs file")
     with open("kwargs.json") as f:
         kwargs = json.load(f)
 
     print("loading models")
     for model in kwargs["models"]:
         # Just checking the presence of the file.
         # A Realistic example would load and use it.
-        assert os.path.isfile(model)
+        assert Path(model).is_file()
 
     print("sampling new configurations")
     configs = []
     for i in range(kwargs["sample_size"]):
         fn_out = f"config_{i:03d}.txt"
         with open(fn_out, "w") as f:
             f.write(f"Bla bla {i} at temperature {kwargs['temperature']}\n")
```

### Comparing `ParMan-0.2.0/demos/jobdemo/templates/train/helper.py` & `Parman-0.3.0/demos/jobdemo/templates/train/helper.py`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/demos/mindmutable.py` & `Parman-0.3.0/demos/mindmutable.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """Simple example showing the dangers of mutable Future arguments.
 
 When submitting a function to an executor with mutable arguments,
 these can be changed prior to the actual execution.
 The result seen by the remote function depends on the executor,
 which is generally not what you want.
 
-The ParMan runners make a deepcopy of closure arguments, to avoid this point of confusion.
+The Parman runners make a deepcopy of closure arguments, to avoid this point of confusion.
 The (remotely) executed closure always sees the arguments as they were at the time of submission.
 """
 
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 from time import sleep
```

### Comparing `ParMan-0.2.0/demos/scheduledemo.py` & `Parman-0.3.0/demos/scheduledemo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 """A simple usage example of parman.scheduler.
 
-Note: ParMan Runner classes hide most of the technical complexity seen in this example.
+Note: Parman Runner classes hide most of the technical complexity seen in this example.
 """
 
 import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 from parman.scheduler import Scheduler
```

### Comparing `ParMan-0.2.0/demos/waitdemo.py` & `Parman-0.3.0/demos/waitdemo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 """A simple usage example of parman.waitfuture.
 
 Note: Direct use of WaitGraph by end-users is expected to be marginal.
-It is used extensively by ParMan Runners to hide technical complexities.
+It is used extensively by Parman Runners to hide technical complexities.
 """
 
 import time
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 from parman.waitfuture import WaitGraph
```

### Comparing `ParMan-0.2.0/pyproject.toml` & `Parman-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["setuptools>=65.0", "setuptools_scm[toml]>=7.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "ParMan"
+name = "Parman"
 authors = [
   { name="Toon Verstraelen", email="toon.verstraelen@ugent.be" },
 ]
-description = "ParMan extends Python concurrent.futures to facilitate parallel workflows"
+description = "Parman extends Python concurrent.futures to facilitate parallel workflows"
 readme = "README.md"
 license = {file = "COPYING"}
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Education",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dependencies = ["attrs", "cattrs"]
+dependencies = ["attrs", "cattrs>=23.1.2"]
 dynamic = ["version"]
 
 [project.urls]
 Issues = "https://github.com/reproducible-reporting/parman/issues"
 Source = "https://github.com/reproducible-reporting/parman/"
 Changelog = "https://github.com/reproducible-reporting/parman/blob/main/CHANGELOG.md"
 
@@ -36,14 +36,15 @@
 [tool.black]
 line-length = 100
 target-version = ['py310']
 
 [tool.ruff]
 select = ["E", "F", "UP", "B", "I", "PGH", "PL", "RUF"]
 line-length = 100
+target-version = "py310"
 ignore = ["PLR2004", "PLR0913", "PLR0912", "PLW2901"]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 testpaths = ["tests"]
 addopts = "-v"
```

### Comparing `ParMan-0.2.0/src/ParMan.egg-info/PKG-INFO` & `Parman-0.3.0/src/Parman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: ParMan
-Version: 0.2.0
-Summary: ParMan extends Python concurrent.futures to facilitate parallel workflows
+Name: Parman
+Version: 0.3.0
+Summary: Parman extends Python concurrent.futures to facilitate parallel workflows
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -182,22 +182,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 [![pytest](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pytest.yaml)
 [![PyPI Upload](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/parman/actions/workflows/pypi.yaml)
-[![PyPI Version](https://img.shields.io/pypi/v/parman)](https://pypi.org/project/ParMan/)
+[![PyPI Version](https://img.shields.io/pypi/v/parman)](https://pypi.org/project/Parman/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/parman)
+![LGPL-3 License](https://img.shields.io/github/license/reproducible-reporting/parman)
 
 # Parman
 
-At this stage, ParMan is an experimental project, so expect a rocky road ahead.
+At this stage, Parman is an experimental project, so expect a rocky road ahead.
 
-The goal of ParMan is to extend `concurrent.futures` (and compatible implementations)
+The goal of Parman is to extend `concurrent.futures` (and compatible implementations)
 with features that facilitate a transparent implementation of workflows.
 
 - `WaitFuture`: a Future subclass that is "finished" after its dependencies have finished.
   (To be created with `WaitGraph.submit`, which never blocks.)
 - `ScheduledFuture`: a Future subclass that submits a Future after its dependencies have finished.
   (To be created with `Scheduler.submit`, which never blocks.)
 - Various `Runner` classes, similar to Executors, which dispatch function calls elsewhere.
@@ -237,23 +238,23 @@
 ```bash
 python -m pip install parman
 ```
 
 ### Examples
 
 At this stage, there is no documentation as such.
-If you want to learn how to use ParMan, check out the [demos](demos/).
+If you want to learn how to use Parman, check out the [demos](demos/).
 If you want to understand the internals, read the source and the docstrings.
 
 
 ## Non-goals
 
 - Support for Dask, because:
   1. The Dask `Future` does not subclass from `concurrent.futures.Future`.
-     Supporting dask would imply a lot of extra boilerplate code in ParMan.
+     Supporting dask would imply a lot of extra boilerplate code in Parman.
   2. The Dask `Future` implements only a subset of `concurrent.futures.Future`.
   3. Dask Distributed has a large memory and time overhead.
 
 
 ## Plans
 
 - Simplify usage.
```

### Comparing `ParMan-0.2.0/src/ParMan.egg-info/SOURCES.txt` & `Parman-0.3.0/src/Parman.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 .git_archival.txt
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 COPYING
 DEVELOPMENT.md
-HEADER
 README.md
 pyproject.toml
+.github/dependabot.yaml
 .github/workflows/pypi.yaml
 .github/workflows/pytest.yaml
 demos/mindmutable.py
 demos/scheduledemo.py
 demos/waitdemo.py
 demos/demc/.gitignore
 demos/demc/README.md
@@ -38,20 +38,20 @@
 demos/jobdemo/templates/sample/jobinfo.py
 demos/jobdemo/templates/sample/run
 demos/jobdemo/templates/sample/submit.sh
 demos/jobdemo/templates/train/helper.py
 demos/jobdemo/templates/train/jobinfo.py
 demos/jobdemo/templates/train/run
 demos/jobdemo/templates/train/submit.sh
-src/ParMan.egg-info/PKG-INFO
-src/ParMan.egg-info/SOURCES.txt
-src/ParMan.egg-info/dependency_links.txt
-src/ParMan.egg-info/entry_points.txt
-src/ParMan.egg-info/requires.txt
-src/ParMan.egg-info/top_level.txt
+src/Parman.egg-info/PKG-INFO
+src/Parman.egg-info/SOURCES.txt
+src/Parman.egg-info/dependency_links.txt
+src/Parman.egg-info/entry_points.txt
+src/Parman.egg-info/requires.txt
+src/Parman.egg-info/top_level.txt
 src/parman/__init__.py
 src/parman/_version.py
 src/parman/closure.py
 src/parman/job.py
 src/parman/metafunc.py
 src/parman/scheduler.py
 src/parman/treeleaf.py
@@ -66,16 +66,16 @@
 src/parman/runners/concurrent.py
 src/parman/runners/dry.py
 src/parman/runners/future.py
 src/parman/runners/parsl.py
 src/parman/runners/serial.py
 src/parman/scripts/__init__.py
 src/parman/scripts/sbatch_wait.py
-tests/__init__.py
 tests/conftest.py
 tests/jobdemo-results.sha256
 tests/test_demos.py
 tests/test_job.py
 tests/test_metafunc.py
+tests/test_runners.py
 tests/test_scheduler.py
 tests/test_treeleaf.py
 tests/test_waitfuture.py
```

### Comparing `ParMan-0.2.0/src/parman/__init__.py` & `Parman-0.3.0/src/parman/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""ParMan package."""
+"""Parman package."""
 
 try:
     from _version import __version__
 except ImportError:
     __version__ = "0.0.0a-dev"
     __version_tuple__ = (0, 0, 0, "a-dev")
```

### Comparing `ParMan-0.2.0/src/parman/clerks/__init__.py` & `Parman-0.3.0/src/parman/runners/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Mapping between local job files and global storage layout."""
+"""Wrappers around Future-based libraries."""
```

### Comparing `ParMan-0.2.0/src/parman/clerks/base.py` & `Parman-0.3.0/src/parman/clerks/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/src/parman/clerks/local.py` & `Parman-0.3.0/src/parman/clerks/local.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/src/parman/clerks/localtemp.py` & `Parman-0.3.0/src/parman/clerks/localtemp.py`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/src/parman/closure.py` & `Parman-0.3.0/src/parman/closure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
@@ -55,18 +55,14 @@
         parameters_api = self.get_parameter_api()
         validate("parameters", parameters, parameters_api)
         result = self.metafunc(*self.args, **self.kwargs)
         result_api = self.get_result_api()
         validate("result", result, result_api)
         return result
 
-    def cached_result(self) -> Any:
-        """Get the cached result."""
-        return self.metafunc.cached_result(*self.args, **self.kwargs)
-
     def get_parameters(self) -> dict[str, Any]:
         """Return a dictionary with all parameters (including positional ones)."""
         signature = self.metafunc.get_signature()
         bound_arguments = signature.bind(*self.args, **self.kwargs)
         bound_arguments.apply_defaults()
         return dict(bound_arguments.arguments)
```

### Comparing `ParMan-0.2.0/src/parman/job.py` & `Parman-0.3.0/src/parman/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
@@ -65,32 +65,33 @@
 import re
 import shutil
 import string
 import subprocess
 import sys
 import types
 from pathlib import Path
+from types import NoneType
 from typing import Any
 
 import attrs
 import cattrs
 
 from .clerks.base import ClerkBase
 from .clerks.local import LocalClerk
 from .closure import Closure
 from .metafunc import MetaFuncBase, type_api_from_mock, type_api_from_signature
 from .treeleaf import iterate_tree, transform_tree
 
 __all__ = ("job", "structure", "unstructure")
 
 
-# The following can be removed once cattrs 23 is released:
-# See https://github.com/python-attrs/cattrs/issues/81
-cattrs.register_structure_hook(Path, lambda d, t: Path(d))
-cattrs.register_unstructure_hook(Path, lambda d: str(d))
+# Support for None and NoneType can be convenient
+# See https://github.com/python-attrs/cattrs/issues/346
+cattrs.register_structure_hook(NoneType, lambda d, t: None)
+cattrs.register_unstructure_hook(NoneType, lambda d: None)
 
 
 @attrs.define
 class Job(MetaFuncBase):
     """A metafunction implementation of a job script.
 
     Attributes
@@ -128,48 +129,48 @@
         ns = {}
         exec(self.jobinfo_source, ns)
         self.resources = ns.get("resources", {})
         self.parameters_func = ns.get("parameters")
         self.mock_func = ns["mock"]
 
     @classmethod
-    def from_template(cls, template: str) -> "Job":
+    def from_template(cls, template: str | Path) -> "Job":
         """Initialize a job script from a template directory.
 
         Parameters
         ----------
         template
             The template directory must contain a ``jobinfo.py`` file with the metadata
-            needed to schedule the job in ParMan.
+            needed to schedule the job in Parman.
             See module-level docstring for more information on this file.
             When the template is a relative path, it gets converted to an absolute one.
         """
         template = Path(template).absolute()
         with open(template / "jobinfo.py") as f:
             jobinfo_source = f.read()
         return cls(template, jobinfo_source)
 
     def describe(
         self,
         clerk: ClerkBase,
-        locator: str,
+        locator: str | Path,
         script: str,
         kwargs: dict[str, Any],
         env: dict[str, str],
     ) -> Any:
         """Short descriptor of the job.
 
         See ``__call__`` method for parameter documentation.
         """
         return locator
 
-    def __call__(
+    def __call__(  # noqa: PLR0915
         self,
         clerk: ClerkBase,
-        locator: str,
+        locator: str | Path,
         script: str,
         kwargs: dict[str, Any],
         env: dict[str, str],
     ) -> Any:
         """Execute the job unconditionally.
 
         Parameters
@@ -191,156 +192,136 @@
 
         Returns
         -------
         result
             The structured contents of the ``result.json`` file created by the job script.
             Output files needed by following jobs must be included here.
         """
-
-        def run(workdir: Path) -> bool:
-            print(f"Starting {locator}")
-
-            # Define useful environment variable
-            parman_env = env | {"PARMAN_WORKDIR": os.getcwd()}
-            write_sh_env(workdir / "jobenv.sh", parman_env)
-
-            # Initialize the work directory
-            shutil.copytree(self.template, workdir, dirs_exist_ok=True)
-            local_kwargs = clerk.localize(kwargs, locator, workdir)
-            with open(workdir / "kwargs.json", "w") as f:
-                json.dump(unstructure(local_kwargs), f)
-            dump_hashes(workdir / "kwargs.sha256", compute_hashes(local_kwargs, workdir))
-
-            # Run the job
-            fn_out = workdir / f"{script}.out"
-            fn_err = workdir / f"{script}.err"
-            try:
-                with open(fn_out, "w") as fo, open(fn_err, "w") as fe:
-                    subprocess.run(
-                        f"./{script}",
-                        stdin=subprocess.DEVNULL,
-                        stdout=fo,
-                        stderr=fe,
-                        shell=True,
-                        cwd=workdir,
-                        check=True,
-                        env=os.environ | parman_env,
-                    )
-            except subprocess.CalledProcessError as exc:
-                if fn_err.is_file():
-                    with open(fn_err) as f:
-                        sys.stderr.write(f.read())
-                raise RuntimeError(f"Script {locator} failed: {script}.") from exc
-
-            # When we got here, the job ran as hoped, and files can be pushed back.
-            clerk.push("kwargs.json", locator, workdir)
-            clerk.push("kwargs.sha256", locator, workdir)
-            clerk.push(script, locator, workdir)
-            clerk.push(f"{script}.out", locator, workdir)
-            clerk.push(f"{script}.err", locator, workdir)
-
-            # There may be some extra files, not explicitly included in the results, worth keeping.
-            fn_extra = workdir / "result.extra"
-            if fn_extra.is_file():
-                with open(fn_extra) as f:
-                    for line in f:
-                        line = strip_line(line)
-                        if len(line) > 0:
-                            clerk.push(line.strip(), locator, workdir)
-                clerk.push("result.extra", locator, workdir)
-
-            return True
-
-        result = self._in_workdir(run, clerk, locator, kwargs)
-        if result is NotImplemented:
-            raise OSError(f"No result.json after completion of {locator}")
-        print(f"Completed {locator}")
-        return result
-
-    def cached_result(
-        self,
-        clerk: ClerkBase,
-        locator: str,
-        script: str,
-        kwargs: dict[str, Any],
-        env: dict[str, str],
-    ) -> Any:
-        """Return the result from a previous run if available.
-
-        See ``__call__`` method for parameter documentation.
-
-        Returns
-        -------
-        result
-            The result that ``__call__`` would give with running any job
-            (if previous results can be loaded) or ``NotImplemented`` otherwise.
-            The existing results are only returned when the kwargs on disk match
-            the ones given here. Any inconsistency in inputs implies execution needed.
-        """
-
-        def run(workdir: Path) -> bool:
-            # If kwargs absent, so we'll assume the job has never been run before.
+        result_api = type_api_from_mock(self.mock_func(**kwargs))
+        with clerk.workdir(locator) as workdir:
             path_kwargs = workdir / clerk.pull(locator / Path("kwargs.json"), locator, workdir)
-            if not path_kwargs.is_file():
-                return False
+            path_result = workdir / clerk.pull(locator / Path("result.json"), locator, workdir)
+            todo_job = False
 
-            # If kwargs inconsistent -> rerun
-            with open(path_kwargs) as f:
-                found_kwargs = json.load(f)
+            # If kwargs present, we'll assume the job has been executed before.
             expected_kwargs = clerk.localize(kwargs, locator, workdir)
-            unstruct_kwargs = unstructure(expected_kwargs)
-            if found_kwargs != unstruct_kwargs:
-                with open(workdir / "kwargs-new.json", "w") as f:
-                    json.dump(unstruct_kwargs, f)
-                os.system(f"ls {workdir}")
-                clerk.push("kwargs-new.json", locator, workdir)
-                raise ValueError(
-                    f"Existing kwarg.json in {locator} inconsistent with new kwargs. "
-                    "Added kwargs-new.json for comparison."
-                )
+            if path_kwargs.is_file():
+                # If kwargs inconsistent -> refresh or raise exception
+                with open(path_kwargs) as f:
+                    found_kwargs = json.load(f)
+                unstruct_kwargs = unstructure(expected_kwargs)
+                if found_kwargs is None:
+                    # It is assumed that the old kwargs.json is manually flagged as outdated
+                    # and safe to be refreshed.
+                    print(f"Rewriting nullified kwargs.json in {locator}")
+                    with open(workdir / "kwargs.json", "w") as f:
+                        json.dump(unstruct_kwargs, f)
+                    clerk.push("kwargs.json", locator, workdir)
+                elif found_kwargs != unstruct_kwargs:
+                    with open(workdir / "kwargs-new.json", "w") as f:
+                        json.dump(unstruct_kwargs, f)
+                    clerk.push("kwargs-new.json", locator, workdir)
+                    raise ValueError(
+                        f"Existing kwarg.json in {locator} inconsistent with new kwargs. "
+                        "Added kwargs-new.json for comparison."
+                    )
+            else:
+                # Check for the presence of a result.json file,
+                # If present, this would suggest a broken state of the job
+                if path_result.is_file():
+                    raise ValueError(f"Found result.json in {locator} while kwargs.json is absent.")
+                todo_job = True
 
-            # If hashes file (even if it should be empty) is missing -> rerun
+            # If hashes file is present, even if empty, it should match the computed hashes.
+            # If missing -> recreate.
             path_sha256 = workdir / clerk.pull(locator / Path("kwargs.sha256"), locator, workdir)
-            if not path_sha256.is_file():
-                raise ValueError(f"File kwarg.sha256 not found in existing {locator}.")
-
-            # If files in kwargs have changes hashes -> rerun
-            found_hashes = load_hashes(path_sha256)
             expected_hashes = compute_hashes(expected_kwargs, workdir)
-            if found_hashes != expected_hashes:
-                dump_hashes(workdir / "kwargs-new.sha256", expected_hashes)
-                clerk.push("kwargs-new.sha256", locator, workdir)
-                raise ValueError(
-                    f"Existing kwarg.json in {locator} inconsistent with new hashes. "
-                    "Added kwargs-new.sha256 for comparison."
-                )
-
-            return True
-
-        return self._in_workdir(run, clerk, locator, kwargs)
+            if path_sha256.is_file():
+                # If files in kwargs have changes hashes -> raise exception
+                found_hashes = load_hashes(path_sha256)
+                if found_hashes != expected_hashes:
+                    dump_hashes(workdir / "kwargs-new.sha256", expected_hashes)
+                    clerk.push("kwargs-new.sha256", locator, workdir)
+                    raise ValueError(
+                        f"Existing kwarg.json in {locator} inconsistent with new hashes. "
+                        "Added kwargs-new.sha256 for comparison."
+                    )
+            else:
+                dump_hashes(workdir / "kwargs.sha256", expected_hashes)
+                clerk.push("kwargs.sha256", locator, workdir)
+
+            if todo_job:
+                print(f"Starting {locator}")
+
+                # Define useful environment variable
+                parman_env = env | {"PARMAN_WORKDIR": os.getcwd()}
+                write_sh_env(workdir / "jobenv.sh", parman_env)
+
+                # Initialize the work directory
+                shutil.copytree(self.template, workdir, dirs_exist_ok=True)
+                local_kwargs = clerk.localize(kwargs, locator, workdir)
+                with open(workdir / "kwargs.json", "w") as f:
+                    json.dump(unstructure(local_kwargs), f)
+                dump_hashes(workdir / "kwargs.sha256", compute_hashes(local_kwargs, workdir))
+
+                # Run the job
+                fn_out = workdir / f"{script}.out"
+                fn_err = workdir / f"{script}.err"
+                try:
+                    with open(fn_out, "w") as fo, open(fn_err, "w") as fe:
+                        subprocess.run(
+                            f"./{script}",
+                            stdin=subprocess.DEVNULL,
+                            stdout=fo,
+                            stderr=fe,
+                            shell=True,
+                            cwd=workdir,
+                            check=True,
+                            env=os.environ | parman_env,
+                        )
+                except subprocess.CalledProcessError as exc:
+                    if fn_err.is_file():
+                        with open(fn_err) as f:
+                            sys.stderr.write(f.read())
+                    raise RuntimeError(f"Script {locator} failed: {script}.") from exc
+
+                # When we got here, the job ran without raising an exception.
+                clerk.push("kwargs.json", locator, workdir)
+                clerk.push("kwargs.sha256", locator, workdir)
+                clerk.push(script, locator, workdir)
+                clerk.push(f"{script}.out", locator, workdir)
+                clerk.push(f"{script}.err", locator, workdir)
+
+                # There may be some extra files, not explicitly included in the results,
+                # worth keeping.
+                clerk.push("jobinfo.py", locator, workdir)
+                fn_extra = workdir / "result.extra"
+                if fn_extra.is_file():
+                    with open(fn_extra) as f:
+                        for line in f:
+                            line = strip_line(line)
+                            if len(line) > 0:
+                                clerk.push(line.strip(), locator, workdir)
+                    clerk.push("result.extra", locator, workdir)
 
-    def _in_workdir(
-        self, run: callable, clerk: ClerkBase, locator: str, kwargs: dict[str, Any]
-    ) -> dict[str, Any]:
-        """Internal method for running something in a job work directory."""
-        result_api = type_api_from_mock(self.mock_func(**kwargs))
-        with clerk.workdir(locator) as workdir:
-            path_result = workdir / clerk.pull(locator / Path("result.json"), locator, workdir)
-            success = run(workdir)
-            if success and path_result.exists():
+            if path_result.exists():
                 clerk.push("result.json", locator, workdir)
                 with open(path_result) as f:
-                    result = structure("result", json.load(f), result_api)
-                    return clerk.globalize(result, locator, workdir)
-            return NotImplemented
+                    result_local = structure("result", json.load(f), result_api)
+                    result = clerk.globalize(result_local, locator, workdir)
+            else:
+                raise OSError(f"No result.json after completion of {locator}")
+
+        print(f"Completed {locator}")
+        return result
 
     def get_parameters_api(
         self,
         clerk: ClerkBase,
-        locator: str,
+        locator: str | Path,
         script: str,
         kwargs: dict[str, Any],
         env: dict[str, str],
     ) -> dict[str, Any]:
         """Return the parameter API derived from the ``jobinfo.py`` metadata.
 
         See ``__call__`` method for parameter documentation.
@@ -351,29 +332,29 @@
         else:
             parameters_api["kwargs"] = self.parameters_func(**kwargs)
         return parameters_api
 
     def get_result_mock(
         self,
         clerk: ClerkBase,
-        locator: str,
+        locator: str | Path,
         script: str,
         kwargs: dict[str, Any],
         env: dict[str, str],
     ) -> Any:
         """Return a mock result, derived from the ``jobinfo.py`` metadata.
 
         See ``__call__`` method for parameter documentation.
         """
         return self.mock_func(**kwargs)
 
     def get_resources(
         self,
         clerk: ClerkBase,
-        locator: str,
+        locator: str | Path,
         script: str,
         kwargs: dict[str, Any],
         env: dict[str, str],
     ) -> dict:
         """Return the value of the resources dictionary in ``jobinfo.py``
 
         See ``__call__`` method for parameter documentation.
@@ -410,15 +391,17 @@
     -------
     structured
         A structured copy of the JSON data.
     """
 
     def transform(mulidx, json_leaf, leaf_api):
         if not isinstance(leaf_api, type | types.GenericAlias):
-            raise TypeError(f"{prefix} at {mulidx}: cannot structure type {leaf_api}")
+            raise TypeError(
+                f"{prefix} at {mulidx}: cannot structure type {leaf_api}, leaf = {json_leaf}"
+            )
         try:
             return cattrs.structure(json_leaf, leaf_api)
         except cattrs.IterableValidationError as exc:
             raise TypeError(
                 f"{prefix} at {mulidx}: {json_leaf} does not conform {leaf_api}"
             ) from exc
         except cattrs.StructureHandlerNotFoundError as exc:
```

### Comparing `ParMan-0.2.0/src/parman/metafunc.py` & `Parman-0.3.0/src/parman/metafunc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
@@ -84,22 +84,14 @@
     def __call__(self, *args, **kwargs) -> Any:
         """The method to be submitted to an executor."""
         raise NotImplementedError
 
     def get_signature(self):
         return inspect.signature(self.__call__)
 
-    def cached_result(self, *args, **kwargs) -> Any:
-        """Return a cached result in case recomputation can be avoided.
-
-        This should give the same result as __call__, but fast enough for the main process.
-        When no cached result is available, NotImplemented is returned.
-        """
-        return NotImplemented
-
     def get_parameters_api(self, *args, **kwargs) -> dict[str, Any]:
         """A method returning API details for function parameters.
 
         The default behavior is to deduce this API from the signature.
         From that signature, only the parameters are used, not the return annotation.
         Annotations take precedence over default values to infer the type
 
@@ -156,31 +148,35 @@
     Raises
     ------
     TypeError
         When a type error is encountered in the data.
     """
     for mulidx, (leaf, leaf_type) in iterate_tree(data, type_api):
         if isinstance(leaf_type, types.GenericAlias):
-            # Use cattrs magic to check the type
+            # Use cattrs magic to check the type.
+            # The GenericAlias types cannot be checked with isinstance.
             try:
                 cattrs.structure(leaf, leaf_type)
             except cattrs.IterableValidationError as exc:
                 raise TypeError(
                     f"{prefix} at {mulidx}: {leaf} does not conform {leaf_type}"
                 ) from exc
             except cattrs.StructureHandlerNotFoundError as exc:
                 raise TypeError(
                     f"{prefix} at {mulidx}: type {leaf_type} cannot be instantiated"
                 ) from exc
-        elif isinstance(leaf_type, type):
-            # Standard Python type check
-            if not isinstance(leaf, leaf_type):
-                raise TypeError(f"{prefix} at {mulidx} is not of type {leaf_type}")
         else:
-            raise TypeError(f"{prefix} at {mulidx}: cannot type-check {leaf} with {leaf_type}")
+            # Standard Python type check
+            try:
+                if not isinstance(leaf, leaf_type):
+                    raise TypeError(f"{prefix} at {mulidx} is not of type {leaf_type}")
+            except Exception as exc:
+                raise TypeError(
+                    f"{prefix} at {mulidx}: cannot type-check {leaf} with {leaf_type}"
+                ) from exc
 
 
 def type_api_from_signature(signature):
     """Construct a type api from a function signature (inspect module)."""
     result = {}
     for name, parameter in signature.parameters.items():
         if parameter.annotation != parameter.empty:
```

### Comparing `ParMan-0.2.0/src/parman/runners/__init__.py` & `Parman-0.3.0/src/parman/scripts/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Wrappers around Future-based libraries."""
+"""Parman utility scripts."""
```

### Comparing `ParMan-0.2.0/src/parman/runners/base.py` & `Parman-0.3.0/src/parman/runners/base.py`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/src/parman/runners/concurrent.py` & `Parman-0.3.0/src/parman/runners/concurrent.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,13 @@
         if self.executor is None:
             self.executor = ThreadPoolExecutor()
 
     def _submit(self, closure: Closure) -> Future:
         closure = self._unpack_data(closure)
         print(f"Submitting {closure.describe()}")
         with self._submit_lock:
-            future = self.executor.submit(Closure.validated_call, closure)
-        return future
+            return self.executor.submit(Closure.validated_call, closure)
 
     def shutdown(self):
         """Wait for all futures to complete."""
         FutureRunnerBase.shutdown(self)
         self.executor.shutdown()
```

### Comparing `ParMan-0.2.0/src/parman/runners/dry.py` & `Parman-0.3.0/src/parman/runners/dry.py`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/src/parman/runners/future.py` & `Parman-0.3.0/src/parman/runners/future.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
@@ -49,31 +49,26 @@
     _submit_lock: Lock = attrs.field(init=False, default=attrs.Factory(Lock))
 
     def __attrs_post_init__(self):
         if self.schedule:
             self._scheduler = Scheduler(self._submit, self.wait_graph)
 
     def __call__(self, closure: Closure) -> Any:
-        result = closure.cached_result()
-        if result is NotImplemented:
-            if self.schedule:
-                dependencies = []
-                for data in closure.args, closure.kwargs:
-                    for _, leaf in iterate_tree(data):
-                        if isinstance(leaf, Future):
-                            dependencies.append(leaf)
-                print(f"Scheduling {closure.describe()} after {len(dependencies)} futures")
-                future = self._scheduler.submit([closure], {}, dependencies)
-            else:
-                future = self._submit(closure)
-            self._futures.append(future)
-            result = _promise_data(future, self.wait_graph, closure.get_result_api())
+        if self.schedule:
+            dependencies = []
+            for data in closure.args, closure.kwargs:
+                for _, leaf in iterate_tree(data):
+                    if isinstance(leaf, Future):
+                        dependencies.append(leaf)
+            print(f"Scheduling {closure.describe()} after {len(dependencies)} futures")
+            future = self._scheduler.submit([closure], {}, dependencies)
         else:
-            print(f"Reusing {closure.describe()}")
-        return result
+            future = self._submit(closure)
+        self._futures.append(future)
+        return _promise_data(future, self.wait_graph, closure.get_result_api())
 
     def _unpack_data(self, closure):
         """Recursively transform Futures into actual results."""
         if self.schedule:
             _validate_done(closure.describe(), closure.args)
             _validate_done(closure.describe(), closure.kwargs)
         return Closure(
@@ -106,19 +101,23 @@
     """Recursively replace Futures by actual results, waiting if needed."""
     return transform_tree(
         lambda _, leaf: leaf.result() if isinstance(leaf, Future) else leaf,
         data,
     )
 
 
+class FutureNotDone(RuntimeError):
+    pass
+
+
 def _validate_done(needed_for: str, data: Any) -> Any:
     """Validate that all futures (nested recursively) are done."""
     for mulidx, leaf in iterate_tree(data):
         if isinstance(leaf, Future) and not leaf.done():
-            raise RuntimeError(
+            raise FutureNotDone(
                 f"Trying to get an unavailable result for argument {mulidx} of {needed_for}."
             )
 
 
 def _promise_data(future: Future, wait_graph: WaitGraph, data_api: Any) -> Any:
     """Build a result, recursively inserting Futures for all return values."""
     return transform_tree(
```

### Comparing `ParMan-0.2.0/src/parman/runners/parsl.py` & `Parman-0.3.0/src/parman/runners/parsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/src/parman/runners/serial.py` & `Parman-0.3.0/src/parman/runners/serial.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,13 +30,8 @@
 
 
 @attrs.define
 class SerialRunner(RunnerBase):
     """Just execute everything right away."""
 
     def __call__(self, closure: Closure) -> Any:
-        result = closure.cached_result()
-        if result is NotImplemented:
-            result = closure.validated_call()
-        else:
-            print(f"Reusing {closure.describe()}")
-        return result
+        return closure.validated_call()
```

### Comparing `ParMan-0.2.0/src/parman/scheduler.py` & `Parman-0.3.0/src/parman/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/src/parman/scripts/sbatch_wait.py` & `Parman-0.3.0/src/parman/scripts/sbatch_wait.py`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/src/parman/treeleaf.py` & `Parman-0.3.0/src/parman/treeleaf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/src/parman/waitfuture.py` & `Parman-0.3.0/src/parman/waitfuture.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/src/parman/wrapper.py` & `Parman-0.3.0/src/parman/wrapper.py`

 * *Files identical despite different names*

### Comparing `ParMan-0.2.0/tests/conftest.py` & `Parman-0.3.0/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
 """Shared fixtures for the unit tests."""
 
-import pathlib
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
 
 import pytest
 
 
 @pytest.fixture(params=[ProcessPoolExecutor, ThreadPoolExecutor])
 def pool(request):
@@ -35,13 +34,7 @@
 
 @pytest.fixture(params=[ProcessPoolExecutor, ThreadPoolExecutor])
 def pool1(request):
     """Single-worker executor from concurrent.futures."""
     PoolExecutor = request.param
     with PoolExecutor(max_workers=1) as pool:
         yield pool
-
-
-@pytest.fixture
-def tmppath(tmpdir):
-    """Temperory path version of tmpdir."""
-    return pathlib.Path(tmpdir)
```

### Comparing `ParMan-0.2.0/tests/jobdemo-results.sha256` & `Parman-0.3.0/tests/jobdemo-results.sha256`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+756c6ebbb4146299a5f59042d4379ee712bdbbfe2254a2b435796d6601c4c058  results/g00/boot/run
+e94622ec4345e1ebb00e935375acf57da1d04a5154c2448835f0ca551daa47d4  results/g00/boot/jobinfo.py
 49d9d754e5f25fbc1ae17cfa435bc9a82c0d9f263ffe3f3d57fd607c4dd2a83f  results/g00/boot/kwargs.json
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/boot/kwargs.sha256
-756c6ebbb4146299a5f59042d4379ee712bdbbfe2254a2b435796d6601c4c058  results/g00/boot/run
 d5373beaba58c9fb81f84f2817be8daba7b1ce34fc747e85290cc7d1652ecc98  results/g00/boot/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/boot/run.err
-ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g00/boot/result.json
 dfd5e34c237dd37954b75197397d2b1584bc16aba7c967ae30d404ec4664ce34  results/g00/boot/config_000.txt
 b91ac83d0d94fd201cf116e98602f019c6ecb585f714b8125b527f45b56d582d  results/g00/boot/config_001.txt
 1a0347b7f455554e86fcf4429abe98fb7a745fa7a6e7d73643452b93ced982fe  results/g00/boot/config_002.txt
 dd2e21ab00356adc202df0217564acc57b6fe00e7b913b07e17477a48d79092a  results/g00/boot/config_003.txt
 e9807e0e267aad4758b8b94f10298b289bf1ae5b81a1713cba0ea9626ca987fd  results/g00/boot/config_004.txt
 e21056d0f9d74eeec1c993f15893653c723936bd3868970eca34fb560cb26c0e  results/g00/boot/config_005.txt
 09bdaa0a36702a094896ce874386f3d4fcefe9224b5a74b86ccecb6e2d543345  results/g00/boot/config_006.txt
@@ -15,149 +15,174 @@
 188643b2c96ce540cb9e497b053c47496fe374c9428de391f39d7deb7cdb1a25  results/g00/boot/config_008.txt
 a0a82998e343539bb9780c8639ac561a665b0a8d6cd1bd75072264062685be0b  results/g00/boot/config_009.txt
 5be0426bfe7609a468a7ca4d917f12418c99f980cf636411a85d497078c08c73  results/g00/boot/config_010.txt
 2bc6d4fcf7a8f495754b40acc6b5b2e09497969fec54f8d5c8a28098ecff04ed  results/g00/boot/config_011.txt
 085b5457f1414f55dc8320c3f8e0179d2be1dd2d3c1937d4018a6e15125421d7  results/g00/boot/config_012.txt
 bface360aa78749f1359c3a3e0a3b9fdf0e9fd639bd6e71d467e02895295a197  results/g00/boot/config_013.txt
 d9731efdafff252d041f15fca1b103ca17b9e3d5434232d1e9010127f71fae69  results/g00/boot/config_014.txt
+ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g00/boot/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0000/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0000/run
 c08931c152c23d02d9cffe009f6bf64fa0719584b789acb2b098459016908854  results/g00/compute/0000/kwargs.json
 5eabc9c27a840bb494c554ec424d04470d3fb72fcdf026818ea6b36f2cb4bf67  results/g00/compute/0000/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0000/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0000/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0000/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0000/result.json
 89e354207ef7c50ea7147e48b21971c4c93206860d070842ef80ecb2b57ddb67  results/g00/compute/0000/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0000/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0001/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0001/run
 e7402e75e5b75d9cb272f10988fd717a3ea2ad58ac8db1872d4460959aec1b57  results/g00/compute/0001/kwargs.json
 99a0203e9b3ea4f5d6dca3f6dea972d698b1fe2bcf0581ae0f62a043545b1402  results/g00/compute/0001/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0001/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0001/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0001/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0001/result.json
 203072a33ae64e2b774e054186538f4c68a98fa800349259ab4aed2197d48565  results/g00/compute/0001/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0001/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0002/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0002/run
 95c89300816fbaa61fca11f9666af70f4ece6dfcaf2b868c42f884c344901d62  results/g00/compute/0002/kwargs.json
 9c0f1701de1ecb332b78d1b30f3a281125fff38d4457d343cb899f8199c2576b  results/g00/compute/0002/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0002/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0002/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0002/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0002/result.json
 47000c98130446201b62ccb7963614e89373f1f9060c2dc5cfe13b6f1bbc1dd1  results/g00/compute/0002/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0002/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0003/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0003/run
 6790d3b4900c2993011d94a08d772d23212131fbfd000e291effa451de656202  results/g00/compute/0003/kwargs.json
 105c52bdc8f6bf15220d8f9d24d5c40e2d7af8d4797ff1ee4cd6a4d63aa821a8  results/g00/compute/0003/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0003/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0003/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0003/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0003/result.json
 6a6aa73c2edfe9e1feb32b9bf930b75284f633e0e55f0ff9024e91da35d769ff  results/g00/compute/0003/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0003/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0004/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0004/run
 4044aeeb742cd2c1590dce1375b8d23c2aed1a66d6ec4477e736b4e2902457eb  results/g00/compute/0004/kwargs.json
 fce9c3ebcfd1583056a384c8ac8e09d24cdae009eee4c0f17946014ec512eb8f  results/g00/compute/0004/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0004/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0004/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0004/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0004/result.json
 8307404fb29c8c4ea90ef7d815169827d017e361124f7e589db86e1b2d4cf316  results/g00/compute/0004/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0004/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0005/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0005/run
 b363ac81ad4b6a9a20fc73f94da13ac7cbf0ebb543e6ce68f7f15785bfe41a02  results/g00/compute/0005/kwargs.json
 5b05a8f63c794935609a5b85e60dc6d406c1ef483aa637b4dbe07081425436c0  results/g00/compute/0005/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0005/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0005/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0005/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0005/result.json
 809fe3062ce5971af4775f609a8c3e1cba5c6c7517c6785ae85be2eef68ddfa6  results/g00/compute/0005/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0005/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0006/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0006/run
 ad5eeaaee14ab975684308a23133e4718e46af01460ba9a2c454b925a02d5b31  results/g00/compute/0006/kwargs.json
 e8721bdeac78223ab4ce4603296f2279928c0495229a50e828f4962a882c62c5  results/g00/compute/0006/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0006/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0006/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0006/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0006/result.json
 6c11d0595a67cc897b8f57b2f41c913011394ed3d669a540ef91716fbcdc0e43  results/g00/compute/0006/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0006/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0007/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0007/run
 e338fc483999c02adf5c7bc99d59928a7eab0ff11a39fa311d13122d653c8146  results/g00/compute/0007/kwargs.json
 e8986c2739e21b8d24f51ee94c7e0f29630e3d5433aec62607cf2c5a0ab0b910  results/g00/compute/0007/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0007/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0007/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0007/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0007/result.json
 c02c34ff3e5931bb628b169f3a76dd54ca6dd0db76f0378c6974df0ab8da5b58  results/g00/compute/0007/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0007/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0008/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0008/run
 bb7cbcd7e2574cfdbc0a1c2e993e38e4f5e39e301e7957805453b724ef04df5d  results/g00/compute/0008/kwargs.json
 a23fa4a3a6d7dafb373a9320c1abdd16edc8744d95c55bcc085475cb45ca6658  results/g00/compute/0008/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0008/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0008/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0008/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0008/result.json
 6cb7b809886d21582c23d96383b0ec032f1fcc4ac4c98945303745b2c3f01e45  results/g00/compute/0008/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0008/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0009/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0009/run
 8687f596e6bf5d3b81261ac5e7fa78dabbe17c9c369442197748d4038be227bb  results/g00/compute/0009/kwargs.json
 65a7d74da44c15d34bec2779beb88b0a905bc40c64d78c68e8bd0bce0b3b6998  results/g00/compute/0009/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0009/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0009/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0009/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0009/result.json
 2742ec834ee85c62c788b19be5f5ba65b9f599b2125fb6dcf22094ab7c864b87  results/g00/compute/0009/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0009/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0010/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0010/run
 8ba35571bf2fbf94648cc558509624c415bf0fdfeeea1249a1a6d3d3b49a1cb9  results/g00/compute/0010/kwargs.json
 2465f6a70bff8abd8587f0396d0acd6d6e57d2996d229e8e84ff68ecccbd94d1  results/g00/compute/0010/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0010/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0010/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0010/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0010/result.json
 94610eb20025ed3571768a186d3c60530aa59583a0890f4712caa0332e6ffd53  results/g00/compute/0010/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0010/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0011/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0011/run
 1c123fce864ab411d68de3121ec4ce748827002402e87a2f127fa0e5d2c7033b  results/g00/compute/0011/kwargs.json
 d8069cfa683231e52f68a086502d6bffe31c463f7711bd844994ef7e8b4995b4  results/g00/compute/0011/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0011/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0011/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0011/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0011/result.json
 28afd41d4dc17750b193662f60cc578dcd14c5f2765d72e6772a8aa9909a6121  results/g00/compute/0011/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0011/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0012/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0012/run
 c375230e794c8f12d78700cab2fd0e6f8948dc4eae2409c93b566cd02fc9119b  results/g00/compute/0012/kwargs.json
 aeae7b6ea682f88f595c3821939d62b5f5d88e1b51c171befe754ea52690fd26  results/g00/compute/0012/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0012/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0012/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0012/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0012/result.json
 9d2a2a0714dabc5080e4c2ac2632fe2112a150b443e0c33b5bddb9ee1583605f  results/g00/compute/0012/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0012/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0013/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0013/run
 a6d704a1c3082c70ae92a5215e13b4004577d43ff8d4eada3abb1fb1b0c7f6e9  results/g00/compute/0013/kwargs.json
 b852df08f5b555eb8eee95c5412d6ef691ae45339e2f7fc175bd9336d4b49b41  results/g00/compute/0013/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0013/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0013/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0013/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0013/result.json
 63603b4318368cff6b77a6075d909d204369d701b0b3d63a0df28398f8454bcf  results/g00/compute/0013/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0013/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g00/compute/0014/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g00/compute/0014/run
 46e158f1a6c5bef6830be219d7b090dcfcb0c25be3d11c8e45e701ebab5ac1ec  results/g00/compute/0014/kwargs.json
 8c557301a062bb8c9449d93eecc14259810dd61e32885d67d50d341fcd05d6f1  results/g00/compute/0014/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g00/compute/0014/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g00/compute/0014/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/compute/0014/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0014/result.json
 a3a3ad9943f610209ded1df2c3989d515ee6c148583a5985f07de8996372a274  results/g00/compute/0014/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g00/compute/0014/result.json
+03d9234c1e884bcf52da8017a3ec2e2ed0246044460347e6b9899192fa9534f1  results/g00/train/00/helper.py
+02128fada93585c4c4a2f3b380490249eeb53d5129ec5d134ad09c18ef335409  results/g00/train/00/jobinfo.py
+4b6cd8bfd5f8950524210590ccde0f2dff2bf5df564c223fbab9c07cd27e47df  results/g00/train/00/run
 d961b2c284dee45abfaf0280ea0b89f6443079d551470ea81c7fe27e469bd431  results/g00/train/00/kwargs.json
 b1e099297a23c4eff460474e1e239489a8feb3d5d50f02157540bd77bb6fa74f  results/g00/train/00/kwargs.sha256
-76e2b71e767b296c95c7ba699a7f2772cf6eb0ddc0505fa1d258d8324f420e60  results/g00/train/00/run
 ce37875a696b48641d8ca83b33f5fa5a055a508a397606aab6f0979699270163  results/g00/train/00/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/train/00/run.err
-01ba4719c80b6fe911b091a7c05124b64eeece964e09c058ef8f9805daca546b  results/g00/train/00/result.extra
-64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g00/train/00/result.json
 9baa08eb3ceea1816175e869de0270da128c192577528e696931365555105d03  results/g00/train/00/model.json
+64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g00/train/00/result.json
+78f6d7c3a681c95a8257e22c0a30bccdb430932050ce3f4c1da706f8563b07aa  results/g00/train/00/valuable.txt
+cc603c786fca9379cae82b35f1cc120fcf5cc60983cf8d6077abfab81d0ef0c9  results/g00/train/00/result.extra
+03d9234c1e884bcf52da8017a3ec2e2ed0246044460347e6b9899192fa9534f1  results/g00/train/01/helper.py
+02128fada93585c4c4a2f3b380490249eeb53d5129ec5d134ad09c18ef335409  results/g00/train/01/jobinfo.py
+4b6cd8bfd5f8950524210590ccde0f2dff2bf5df564c223fbab9c07cd27e47df  results/g00/train/01/run
 e6013541489afc2d034a7276080571bf66cf21d85e8ed5936f0616c09548ea6d  results/g00/train/01/kwargs.json
 b1e099297a23c4eff460474e1e239489a8feb3d5d50f02157540bd77bb6fa74f  results/g00/train/01/kwargs.sha256
-76e2b71e767b296c95c7ba699a7f2772cf6eb0ddc0505fa1d258d8324f420e60  results/g00/train/01/run
 eabcd256d5aee5b5ed87956d0d4160f474e0986ce26b5bc867b244a7c7028c4b  results/g00/train/01/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/train/01/run.err
-01ba4719c80b6fe911b091a7c05124b64eeece964e09c058ef8f9805daca546b  results/g00/train/01/result.extra
-64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g00/train/01/result.json
 9baa08eb3ceea1816175e869de0270da128c192577528e696931365555105d03  results/g00/train/01/model.json
+64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g00/train/01/result.json
+78f6d7c3a681c95a8257e22c0a30bccdb430932050ce3f4c1da706f8563b07aa  results/g00/train/01/valuable.txt
+cc603c786fca9379cae82b35f1cc120fcf5cc60983cf8d6077abfab81d0ef0c9  results/g00/train/01/result.extra
+03d9234c1e884bcf52da8017a3ec2e2ed0246044460347e6b9899192fa9534f1  results/g00/train/02/helper.py
+02128fada93585c4c4a2f3b380490249eeb53d5129ec5d134ad09c18ef335409  results/g00/train/02/jobinfo.py
+4b6cd8bfd5f8950524210590ccde0f2dff2bf5df564c223fbab9c07cd27e47df  results/g00/train/02/run
 b3e5bb883540e4d1aaef8f94ed84528ffcb8f63e50abf6e1a2cd4bb68b42af96  results/g00/train/02/kwargs.json
 b1e099297a23c4eff460474e1e239489a8feb3d5d50f02157540bd77bb6fa74f  results/g00/train/02/kwargs.sha256
-76e2b71e767b296c95c7ba699a7f2772cf6eb0ddc0505fa1d258d8324f420e60  results/g00/train/02/run
 c25dee08024c1798a4af758091b9decd3f301635713357322e75dcc85abd7a5e  results/g00/train/02/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g00/train/02/run.err
-01ba4719c80b6fe911b091a7c05124b64eeece964e09c058ef8f9805daca546b  results/g00/train/02/result.extra
-64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g00/train/02/result.json
 9baa08eb3ceea1816175e869de0270da128c192577528e696931365555105d03  results/g00/train/02/model.json
+64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g00/train/02/result.json
+78f6d7c3a681c95a8257e22c0a30bccdb430932050ce3f4c1da706f8563b07aa  results/g00/train/02/valuable.txt
+cc603c786fca9379cae82b35f1cc120fcf5cc60983cf8d6077abfab81d0ef0c9  results/g00/train/02/result.extra
+90e80c71a80a7ae2a4509ec049ea95b2010aed532ac7f5364492b538e47a1e9f  results/g01/sample/0300/jobinfo.py
+646d17457558f13ac33fb444aba41fc5ebf026622932f37f17f750c4dfd6225e  results/g01/sample/0300/run
 06aebf55488a55dd28b31bfbf1d8ab090bc49a7cbfa944c6100264fba74cc376  results/g01/sample/0300/kwargs.json
 a22b897041b0e047b556f82fde55c2b8125ed435eabd095b6926255f710623e7  results/g01/sample/0300/kwargs.sha256
-00d4d8350d6eb91c9a7bafb77c7c8eb1f6b8103b6cf7cf2806a4ab353f77b86d  results/g01/sample/0300/run
 933c4c01e6bfbdb5071acec5f6f90fbebf8ba86c1c4ef990e2d1a3b70a15b1ac  results/g01/sample/0300/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/sample/0300/run.err
-ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g01/sample/0300/result.json
 0bb8eff61ab5b091015cb261867608866fe8e52b5c5006d6abee6ceb1ffa07ff  results/g01/sample/0300/config_000.txt
 832abd02ef78fc600dc347d8001a5ee8ec49fe6e1d54fe298edf4dfd112136df  results/g01/sample/0300/config_001.txt
 f539123d1384c05eeba5b1aa0b78db3f3476931a04c0d5aec617750699e3eccc  results/g01/sample/0300/config_002.txt
 e2d13ecf09810202838e9b648fd92e76de63cc6e0443573b2aef96ff20c08bfb  results/g01/sample/0300/config_003.txt
 d8c20072efa62a869630b9ea9f6653f64c923894c1e4870314be7ef96b965bdf  results/g01/sample/0300/config_004.txt
 a39fede7d4ef33628821e1a66392e3f66dd7a7c4d0d5ea57ecfd82673463321a  results/g01/sample/0300/config_005.txt
 4aae2f230e6e17c1b9935a3f8e00f7c7afb5ccc338e7d94fe97cf870fbced1e5  results/g01/sample/0300/config_006.txt
@@ -165,20 +190,21 @@
 d347adc1c720cc02b9df505a31ff6a94f1e766180829aef462334fd6aa544f8e  results/g01/sample/0300/config_008.txt
 40d91f798f9962f6bbe707a6c63ed6adfe91637ff93ee2c1621c963ef47936f8  results/g01/sample/0300/config_009.txt
 57989c9ed0588af6201db4fbbdf617b23c0aecfaa0adc056e8e5a89519f9fdf0  results/g01/sample/0300/config_010.txt
 02d75ea5e13bac08ec3f1b92893ec15c603903bf61e5362c4c15e8b1cd763d5c  results/g01/sample/0300/config_011.txt
 48e917360dc830ac5aa1385a23ae37a0e72418a60dda99f087a86f2406130f70  results/g01/sample/0300/config_012.txt
 fd0d4f4d8ef9b86cd36900af2f6cfa169808bd7f5a91d1e668958658cfe932ef  results/g01/sample/0300/config_013.txt
 d044ddcea5ea24b4eca8eb51bf87af04018820a32a053ae93df3f524cbede4bf  results/g01/sample/0300/config_014.txt
+ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g01/sample/0300/result.json
+90e80c71a80a7ae2a4509ec049ea95b2010aed532ac7f5364492b538e47a1e9f  results/g01/sample/0400/jobinfo.py
+646d17457558f13ac33fb444aba41fc5ebf026622932f37f17f750c4dfd6225e  results/g01/sample/0400/run
 4f8566f4adc8f8ab5d1256d3aa4d0af852c85ff0872b3485121b1a6d020bbaed  results/g01/sample/0400/kwargs.json
 a22b897041b0e047b556f82fde55c2b8125ed435eabd095b6926255f710623e7  results/g01/sample/0400/kwargs.sha256
-00d4d8350d6eb91c9a7bafb77c7c8eb1f6b8103b6cf7cf2806a4ab353f77b86d  results/g01/sample/0400/run
 933c4c01e6bfbdb5071acec5f6f90fbebf8ba86c1c4ef990e2d1a3b70a15b1ac  results/g01/sample/0400/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/sample/0400/run.err
-ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g01/sample/0400/result.json
 946745d8d2a148fdc25881bf8b3b8900ce03cc9fe43797cdee5dddf5ace17c0e  results/g01/sample/0400/config_000.txt
 f66fe5f26b48c00a716acb3c18b951eeb5c9f3e84c0cab011cc69b0a71a726b6  results/g01/sample/0400/config_001.txt
 8187ef8b719106ffbd9955364edb96ad13f5356ab5e17e381cd2ef30fcff6ed6  results/g01/sample/0400/config_002.txt
 e2d6cd8dc1f42e84d7505a69767fc6763717de16c8cd315d49d79d352bb95a28  results/g01/sample/0400/config_003.txt
 bddb587d83807369f4fdb4196ac78220df8e47d4d4511294cf367e31aa0b44fe  results/g01/sample/0400/config_004.txt
 42512e9ac76e68195560505878b92f7074b04e91bc1e252ac0f7adb8fbd3fd55  results/g01/sample/0400/config_005.txt
 9b08f133ff3b3c37926c6a3ed69014d6282cc043f0d326086bf7474ed961103e  results/g01/sample/0400/config_006.txt
@@ -186,254 +212,294 @@
 51514ee2c4ae10a475fbe8be3d76ddc322c709937573f71fd0360f9ee5638a2f  results/g01/sample/0400/config_008.txt
 bba63bc5c1fbb10cfc1c09329334b349f5c27262833743cad5a23dda724d5b72  results/g01/sample/0400/config_009.txt
 025ece6d59f92229e646524753f1bec3c7315a74d1a45ddfbb64d489b69b4127  results/g01/sample/0400/config_010.txt
 6e9277cba787907044753b6c6b5711750beb94542252dc77d55a228b3f21283d  results/g01/sample/0400/config_011.txt
 7c7f3daa876d2a06c7264f6dcaf3aa13c8dc127f44ba776e15b113bf3f938935  results/g01/sample/0400/config_012.txt
 42b4b3c54aa1870aee98803cdfb6b100e2364461325a215aee15a82a8f1fd494  results/g01/sample/0400/config_013.txt
 c881dc9087ee49940baec12da2b704e403a56d1160235a54957dd6273c1f1a2a  results/g01/sample/0400/config_014.txt
+ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g01/sample/0400/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0000/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0000/run
 284e543f529863919bf7bba8cb25445b5fdcb3b27a37946bd021a157fd5c404b  results/g01/compute/0000/kwargs.json
 fb3df32d67daaf155efc1ef7f9374a52d305cabeaf654dfee46b063ee1349e5a  results/g01/compute/0000/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0000/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0000/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0000/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0000/result.json
 3e77f5e7348ef99bf88de47fa93e3c00261b6244dd46a366eec0431ebbe6025f  results/g01/compute/0000/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0000/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0001/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0001/run
 47c661d8cebba4e5b96720353c526dcecefa319fc1fe73cf6c54b3dc98b30ffd  results/g01/compute/0001/kwargs.json
 daa80c0f0f4232f34b2690e7ff90d50712ead8309665b0e065951e5dcc5827a3  results/g01/compute/0001/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0001/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0001/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0001/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0001/result.json
 743f84922f7f179eb3aca3b3b7b1d682bc701a029241e1c4bc3d5d9f94b91e2d  results/g01/compute/0001/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0001/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0002/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0002/run
 3ac6d77cc7696fd6bf15f06d7fb036f7fb56d496a81b87a13097964ddb1200fe  results/g01/compute/0002/kwargs.json
 741f996ecd209bac37cfc8aa51b113930d066780025e5f22711ecff79cd07530  results/g01/compute/0002/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0002/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0002/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0002/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0002/result.json
 1cc8edec81662b108f0307c4b469e790171148044671fd7053995fd14ac7c88c  results/g01/compute/0002/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0002/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0003/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0003/run
 2372518482ce722a780f62df8c800abbd054faf6221a6c5f4d2c428c3610c3f9  results/g01/compute/0003/kwargs.json
 67e106a76a9dce75be36a676b8a494c7d91bd5798a65df13dc42054cdb428dc9  results/g01/compute/0003/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0003/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0003/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0003/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0003/result.json
 b7940296fa12656ec34b3e70ff17f0757b96d50c59dde2c068fb57f5418688af  results/g01/compute/0003/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0003/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0004/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0004/run
 54356c66beba57fbf09c53031300b3f552920d2b90fa8dd9d4ff073d06321d1b  results/g01/compute/0004/kwargs.json
 8aa39d75ec59173a2a92ec7d4a9cfd92eb9df9e3be5034614eed1a0e605d9ffa  results/g01/compute/0004/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0004/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0004/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0004/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0004/result.json
 abe9f36962a3bd47e97a1479fe90cb5517e1bd0a5dad71e1ad86504d065521ad  results/g01/compute/0004/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0004/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0005/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0005/run
 758462d2cfd0aca472f9c25de2945db3cf4fcacff78b54883694069793c52768  results/g01/compute/0005/kwargs.json
 5ac6fb9b9538e2f7cbd34524972ae2247f305c429fcdd38e6183a52b200d2710  results/g01/compute/0005/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0005/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0005/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0005/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0005/result.json
 98f1f16bcc7d4e3764be2fa75d968d49b66b119886383dab80146ae416460f0d  results/g01/compute/0005/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0005/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0006/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0006/run
 5dfa9738368497f89ae0df61ffcfa0e8d69e61193bf9668c13e9ddf606880d8f  results/g01/compute/0006/kwargs.json
 18552857a270f71479f60f4d5684321d3e6c5b476b608257a240bd0e01eaffdd  results/g01/compute/0006/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0006/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0006/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0006/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0006/result.json
 8a1de8a112f635d6152d515d4f915e28637d2c3b1b72b92c38d47e1fcb5037c8  results/g01/compute/0006/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0006/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0007/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0007/run
 79b404bd75570e45c6f6de4dfc8165567ad72aa2ee0fcfb68537e4107dfb3651  results/g01/compute/0007/kwargs.json
 c6125ca416afa01b24800e38112782a289a8d47f4ee7aa596fb17ec8c0c70859  results/g01/compute/0007/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0007/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0007/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0007/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0007/result.json
 cb89db3eb7c0e8b6d284fb9c3b5a4885548418a44ae5ffe9a21781189f7b887b  results/g01/compute/0007/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0007/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0008/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0008/run
 7b3c6694601e9a812d46a2a7504e696ad4da8a394004c066215dc67fd1812a09  results/g01/compute/0008/kwargs.json
 3e0a2b0bdc0221059174d6b4e878e6e4fcfcb9158cf3d51be0b8690bb75020ba  results/g01/compute/0008/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0008/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0008/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0008/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0008/result.json
 14d3c298262648f77c66df02bd23232bc1919f6798d4ad0d1ae0c971c06f0aa6  results/g01/compute/0008/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0008/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0009/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0009/run
 f698e7e9f2e1eb6e1c4370869d26e5f4365988c4ba3555a7201fcd0f76db1e04  results/g01/compute/0009/kwargs.json
 ec8bcd851289ffc0fbb016e823eeaff736eb178d7001ec8213bb18831789f12a  results/g01/compute/0009/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0009/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0009/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0009/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0009/result.json
 c31138621f78f2a2a465444b4184f5734e6db7bab6c2976140bbca3fc984101c  results/g01/compute/0009/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0009/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0010/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0010/run
 f3ee02a79af2eec16db84c12e59dc3c5ae73a8fe3c7a675e147ff04a20458001  results/g01/compute/0010/kwargs.json
 8a1718e5a70c30260424dfd33b90ef221558a084f6c4498c12eda18fce8ca4f9  results/g01/compute/0010/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0010/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0010/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0010/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0010/result.json
 b75fbd35d285a394813029a0b2405e27fe2be0a0a681325a4a7439af7e8bebfc  results/g01/compute/0010/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0010/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0011/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0011/run
 f6ea23f7860d6a3e64d19f45a709c191fdcb17627890a5e45cd572f8113a2884  results/g01/compute/0011/kwargs.json
 24e1fbbb41351e90951c659eb9d316aae21986602959ebd8d21ad008573a134b  results/g01/compute/0011/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0011/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0011/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0011/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0011/result.json
 be8e13fbe48878a3473be349c522bc2753d69c5455925a4318a6569127cd98f9  results/g01/compute/0011/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0011/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0012/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0012/run
 9e4a32d6a254ff3185acc9d555d208f03d5c2ac0775dbb66f31c29f515013430  results/g01/compute/0012/kwargs.json
 b41f6e0df16f7637cf3afd618a5d6b83b1ff443c1a6710614ed26c37a42ac89e  results/g01/compute/0012/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0012/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0012/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0012/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0012/result.json
 f9740c55152e88a5a6123a55cba9b9580b81e2e77b7a53129b543b86a9669a91  results/g01/compute/0012/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0012/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0013/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0013/run
 44e237f746a7075fddeacb9655c709cc28f6277a764520e06cef15b79052732e  results/g01/compute/0013/kwargs.json
 5d924b2ea156c1b2028654b66af473b3c5e51fd6941825b2d57db645483c297d  results/g01/compute/0013/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0013/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0013/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0013/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0013/result.json
 1f261dc2531692dffced71da3f22277e9bacf24593b510e06e20be3ab878c44d  results/g01/compute/0013/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0013/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0014/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0014/run
 5d5c3efa80936a973fde9b28c0357073a07df23ea5ae5290313352ef30d78ea9  results/g01/compute/0014/kwargs.json
 eb1bec5ce62166d3ed2af62735715b30ddeedfe62b88ebd22ed660fa54e852de  results/g01/compute/0014/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0014/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0014/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0014/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0014/result.json
 6e6c643bb4758813dcb96746d97a611882a51e3b41336a337dcafdbcc2f51023  results/g01/compute/0014/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0014/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0015/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0015/run
 9d32d6e7fb9a1a64272480761624b39d1d4e7e04fca384207c3e6e350b696ea1  results/g01/compute/0015/kwargs.json
 8dba13f8c967bd92d8b3ab5b3b5cfdde4357b9bf4e4e46c5eac03194be4496cd  results/g01/compute/0015/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0015/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0015/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0015/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0015/result.json
 aa878d88183a22bc00d9e7d25901182313d2d9d34e5bc92833760222b9002504  results/g01/compute/0015/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0015/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0016/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0016/run
 b9918f527fffd2b9306c7c2e8d27e899aec49490c3c642944d39a2c7e4efa04c  results/g01/compute/0016/kwargs.json
 0665fd1a8c02e4b5d837fb65bba036076bdc267c0fdea63f3092aed1cc37608e  results/g01/compute/0016/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0016/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0016/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0016/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0016/result.json
 0e6886135cfd015e56c69a0e2442a94c6d4aba9255663887dcbe98c531ee9d38  results/g01/compute/0016/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0016/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0017/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0017/run
 1c2f9d6d332c46f1e5ddb174b7923755e5480c054470498fbd063aafc4ec7b1d  results/g01/compute/0017/kwargs.json
 a6a71e6a98a3c38d09d1cd65d3522de92e148eb48546a41e373442e7122d89c8  results/g01/compute/0017/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0017/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0017/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0017/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0017/result.json
 e79ce77b90ddcf4abaed81bb43bb8ca6b877afea329373f78cfc5211e207f051  results/g01/compute/0017/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0017/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0018/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0018/run
 8764346f07b2bbbb499326df321bee898c7846e6c3a1629855367062b2d679d2  results/g01/compute/0018/kwargs.json
 06156d2e2cd27781436740f303b48dce5462b8c0caa2d0efb4fe347cf6c4a7f8  results/g01/compute/0018/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0018/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0018/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0018/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0018/result.json
 0e8b0daf30d09fb107b36a40fed2fcc8b2029f3e104a2b9f3414bf4ec49ceb97  results/g01/compute/0018/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0018/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0019/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0019/run
 737212165bd64f22fc8399523fd264896459966ab92bc3464d2b96b0b2c94530  results/g01/compute/0019/kwargs.json
 ef6fa763b4c0db20c7c3916382c169adb6b15c604e6675107e5dd5ada672d197  results/g01/compute/0019/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0019/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0019/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0019/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0019/result.json
 2f6b7618ee4fc6501e4dc729c6bfa2d88b71bbed289774696feb7324cc7c6fb1  results/g01/compute/0019/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0019/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0020/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0020/run
 a658a46f23168cc0056fd594b7e0f3b128ddd82e3cc4136e494cc58971945864  results/g01/compute/0020/kwargs.json
 3eda7160ce838c4776a5b5ba2b8ca1d3fe7c48e2ad0e17ff03f5ae26f0d9474c  results/g01/compute/0020/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0020/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0020/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0020/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0020/result.json
 db5db248053f658b2862733cf3946ec156d430c2e6305d178315361c90611d83  results/g01/compute/0020/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0020/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0021/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0021/run
 ff88cde4da9742868c386a3477a9b94db1dc49f8123cce7310d155a82e7df5ac  results/g01/compute/0021/kwargs.json
 18e09fdc954880bf09b29167e16b640e2a9427db0a5f2b6e98c6646d0f6d8048  results/g01/compute/0021/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0021/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0021/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0021/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0021/result.json
 480c503f99f9cf4c41c3cc2a69072f2d7171a3782ffe3db22caf67e81617e3bc  results/g01/compute/0021/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0021/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0022/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0022/run
 938c6c2046b0ded704dacd50f8ece2104455199409701ba475e43d3b3fca04c7  results/g01/compute/0022/kwargs.json
 773c9df91facf2506c8efcb801413bda8a9f10633a1a6dabd2d66ed02555b55b  results/g01/compute/0022/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0022/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0022/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0022/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0022/result.json
 8257fc83a37838ca8546c7ef64b22f480427063abb8c64ce8c421cda89426a91  results/g01/compute/0022/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0022/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0023/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0023/run
 e7e29c1a5bd6d06a8cde9f63a6503f7fb83f8f030c0b899fd60a6daaca500918  results/g01/compute/0023/kwargs.json
 765f7f83279d86e12ecebb632f122605c0b0871c1d3f987933fff6dd1b5a12cc  results/g01/compute/0023/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0023/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0023/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0023/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0023/result.json
 908f746aca20a3c516674896ab0994cba66aaa1f0db52699985b96144d375c29  results/g01/compute/0023/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0023/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0024/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0024/run
 abbae7c01749c1b59e1733f7aa521b7f6adebae6fc5116336f4444a5ab0a7d39  results/g01/compute/0024/kwargs.json
 0b89103bbf657d82bd01238affd2f3649114e5c0a630f2340ab6591301528881  results/g01/compute/0024/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0024/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0024/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0024/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0024/result.json
 7a93aaad4286285c01e42f6037a5644a2fb16cb7e4e3acfbb0210f482720b3b8  results/g01/compute/0024/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0024/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0025/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0025/run
 a579173fbcc88a04ccc8abd26a24189602a12f6c1229ffc91f1fa9ef8aa1e4fd  results/g01/compute/0025/kwargs.json
 e9625686e9b2be018ae49ddcbeaf4c4c7251cac2a049cfe8833b6183c9c58d24  results/g01/compute/0025/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0025/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0025/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0025/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0025/result.json
 78210a865d11fb0bd6217fa2b78c179575c9c860712a7691bf8ade7bbd233a00  results/g01/compute/0025/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0025/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0026/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0026/run
 d0db1d4131294f248fb45b5677105db74d21891e66c1c8a9a2496b5925c49721  results/g01/compute/0026/kwargs.json
 f4a810458a4d99797ff7a52103323f212f99f8f205a9979aba9245c894036992  results/g01/compute/0026/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0026/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0026/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0026/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0026/result.json
 5734762465ff02c4b8559e26cf8ae91aed363822e9da2f2598a33ec36590e4a8  results/g01/compute/0026/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0026/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0027/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0027/run
 41a1c8a8902ee8bf0b27de93de11bacfc5a50a777fb973ae927f8ddb70a5bf16  results/g01/compute/0027/kwargs.json
 26bf4cb2971b5ddb71444f1b24116f647cbb454d1da37a4f908918b690e9ad08  results/g01/compute/0027/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0027/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0027/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0027/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0027/result.json
 ed14783dae2db651ffac89a510d61d20861e4efe7af60b4c3a8cc688bacebbae  results/g01/compute/0027/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0027/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0028/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0028/run
 a0ea987f2f1807b98b6ea7c006324b9b18943d68eacff53133f37c0826d277d4  results/g01/compute/0028/kwargs.json
 ed8515fa8f2eed49a635e3da0c1d6c177195ee0fa4389ed2919eceb5e14e3615  results/g01/compute/0028/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0028/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0028/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0028/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0028/result.json
 bd8560128be8478f201aa14bebd683e634a7e57623a4939c069d1db951984cc3  results/g01/compute/0028/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0028/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g01/compute/0029/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g01/compute/0029/run
 d4a413283f837ed1b17b2a3278b19d31c6ad15c790fdbab9873fb781ff54c477  results/g01/compute/0029/kwargs.json
 fa66bf772cc6e0a1e9663b7f100c4b8f816454b825cea1655526795d634a7873  results/g01/compute/0029/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g01/compute/0029/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g01/compute/0029/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/compute/0029/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0029/result.json
 e83fe6c7a6d0b094c8e22ef7b062636cdbf778f9a5539d6dacba0f950ea7793f  results/g01/compute/0029/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g01/compute/0029/result.json
+03d9234c1e884bcf52da8017a3ec2e2ed0246044460347e6b9899192fa9534f1  results/g01/train/00/helper.py
+02128fada93585c4c4a2f3b380490249eeb53d5129ec5d134ad09c18ef335409  results/g01/train/00/jobinfo.py
+4b6cd8bfd5f8950524210590ccde0f2dff2bf5df564c223fbab9c07cd27e47df  results/g01/train/00/run
 8897d4c81479b6c08f511e5215b72c58146fa15c94d714f66dc6f5992ea5479a  results/g01/train/00/kwargs.json
 88d18bb7b988079330e08727736246ac6223b1ec6bb95bc4c7e7c4ff55def9c4  results/g01/train/00/kwargs.sha256
-76e2b71e767b296c95c7ba699a7f2772cf6eb0ddc0505fa1d258d8324f420e60  results/g01/train/00/run
 fae41f84fa34d91e9c46ea5bb29e3092e1abe0a205621258ffd419adc929dac3  results/g01/train/00/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/train/00/run.err
-01ba4719c80b6fe911b091a7c05124b64eeece964e09c058ef8f9805daca546b  results/g01/train/00/result.extra
-64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g01/train/00/result.json
 f1d11a7e993ef6c8a4c0b67f819c96b608b1b4980ac00bff66235a11c6589112  results/g01/train/00/model.json
+64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g01/train/00/result.json
+78f6d7c3a681c95a8257e22c0a30bccdb430932050ce3f4c1da706f8563b07aa  results/g01/train/00/valuable.txt
+cc603c786fca9379cae82b35f1cc120fcf5cc60983cf8d6077abfab81d0ef0c9  results/g01/train/00/result.extra
+03d9234c1e884bcf52da8017a3ec2e2ed0246044460347e6b9899192fa9534f1  results/g01/train/01/helper.py
+02128fada93585c4c4a2f3b380490249eeb53d5129ec5d134ad09c18ef335409  results/g01/train/01/jobinfo.py
+4b6cd8bfd5f8950524210590ccde0f2dff2bf5df564c223fbab9c07cd27e47df  results/g01/train/01/run
 99d0bece80d3a3577df93c898226a91a635bfc0fd037a95eaddfe00a3a689871  results/g01/train/01/kwargs.json
 88d18bb7b988079330e08727736246ac6223b1ec6bb95bc4c7e7c4ff55def9c4  results/g01/train/01/kwargs.sha256
-76e2b71e767b296c95c7ba699a7f2772cf6eb0ddc0505fa1d258d8324f420e60  results/g01/train/01/run
 fea5f0a15c9ae715b2ff1e05c3e55c1151a86eadb0fd1db3d40c80d9296bb0cc  results/g01/train/01/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/train/01/run.err
-01ba4719c80b6fe911b091a7c05124b64eeece964e09c058ef8f9805daca546b  results/g01/train/01/result.extra
-64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g01/train/01/result.json
 f1d11a7e993ef6c8a4c0b67f819c96b608b1b4980ac00bff66235a11c6589112  results/g01/train/01/model.json
+64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g01/train/01/result.json
+78f6d7c3a681c95a8257e22c0a30bccdb430932050ce3f4c1da706f8563b07aa  results/g01/train/01/valuable.txt
+cc603c786fca9379cae82b35f1cc120fcf5cc60983cf8d6077abfab81d0ef0c9  results/g01/train/01/result.extra
+03d9234c1e884bcf52da8017a3ec2e2ed0246044460347e6b9899192fa9534f1  results/g01/train/02/helper.py
+02128fada93585c4c4a2f3b380490249eeb53d5129ec5d134ad09c18ef335409  results/g01/train/02/jobinfo.py
+4b6cd8bfd5f8950524210590ccde0f2dff2bf5df564c223fbab9c07cd27e47df  results/g01/train/02/run
 4814f1b2390d61870fbaa160bf954c3fe7276b3fcb0b3cdbec861efda82564dd  results/g01/train/02/kwargs.json
 88d18bb7b988079330e08727736246ac6223b1ec6bb95bc4c7e7c4ff55def9c4  results/g01/train/02/kwargs.sha256
-76e2b71e767b296c95c7ba699a7f2772cf6eb0ddc0505fa1d258d8324f420e60  results/g01/train/02/run
 1689b335ea6c3201bd2f8af7a907c6667d6ad9825fe4d73673c30ffe0b587168  results/g01/train/02/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g01/train/02/run.err
-01ba4719c80b6fe911b091a7c05124b64eeece964e09c058ef8f9805daca546b  results/g01/train/02/result.extra
-64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g01/train/02/result.json
 f1d11a7e993ef6c8a4c0b67f819c96b608b1b4980ac00bff66235a11c6589112  results/g01/train/02/model.json
+64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g01/train/02/result.json
+78f6d7c3a681c95a8257e22c0a30bccdb430932050ce3f4c1da706f8563b07aa  results/g01/train/02/valuable.txt
+cc603c786fca9379cae82b35f1cc120fcf5cc60983cf8d6077abfab81d0ef0c9  results/g01/train/02/result.extra
+90e80c71a80a7ae2a4509ec049ea95b2010aed532ac7f5364492b538e47a1e9f  results/g02/sample/0300/jobinfo.py
+646d17457558f13ac33fb444aba41fc5ebf026622932f37f17f750c4dfd6225e  results/g02/sample/0300/run
 540d70567226479c912caffed911e57d3758deee9552170eab1cb3467759de7a  results/g02/sample/0300/kwargs.json
 ef5d3842e5947475309d6ea38d8f80dfa9c0206b76368d26a241b911f2e8d03f  results/g02/sample/0300/kwargs.sha256
-00d4d8350d6eb91c9a7bafb77c7c8eb1f6b8103b6cf7cf2806a4ab353f77b86d  results/g02/sample/0300/run
 933c4c01e6bfbdb5071acec5f6f90fbebf8ba86c1c4ef990e2d1a3b70a15b1ac  results/g02/sample/0300/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/sample/0300/run.err
-ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g02/sample/0300/result.json
 0bb8eff61ab5b091015cb261867608866fe8e52b5c5006d6abee6ceb1ffa07ff  results/g02/sample/0300/config_000.txt
 832abd02ef78fc600dc347d8001a5ee8ec49fe6e1d54fe298edf4dfd112136df  results/g02/sample/0300/config_001.txt
 f539123d1384c05eeba5b1aa0b78db3f3476931a04c0d5aec617750699e3eccc  results/g02/sample/0300/config_002.txt
 e2d13ecf09810202838e9b648fd92e76de63cc6e0443573b2aef96ff20c08bfb  results/g02/sample/0300/config_003.txt
 d8c20072efa62a869630b9ea9f6653f64c923894c1e4870314be7ef96b965bdf  results/g02/sample/0300/config_004.txt
 a39fede7d4ef33628821e1a66392e3f66dd7a7c4d0d5ea57ecfd82673463321a  results/g02/sample/0300/config_005.txt
 4aae2f230e6e17c1b9935a3f8e00f7c7afb5ccc338e7d94fe97cf870fbced1e5  results/g02/sample/0300/config_006.txt
@@ -441,20 +507,21 @@
 d347adc1c720cc02b9df505a31ff6a94f1e766180829aef462334fd6aa544f8e  results/g02/sample/0300/config_008.txt
 40d91f798f9962f6bbe707a6c63ed6adfe91637ff93ee2c1621c963ef47936f8  results/g02/sample/0300/config_009.txt
 57989c9ed0588af6201db4fbbdf617b23c0aecfaa0adc056e8e5a89519f9fdf0  results/g02/sample/0300/config_010.txt
 02d75ea5e13bac08ec3f1b92893ec15c603903bf61e5362c4c15e8b1cd763d5c  results/g02/sample/0300/config_011.txt
 48e917360dc830ac5aa1385a23ae37a0e72418a60dda99f087a86f2406130f70  results/g02/sample/0300/config_012.txt
 fd0d4f4d8ef9b86cd36900af2f6cfa169808bd7f5a91d1e668958658cfe932ef  results/g02/sample/0300/config_013.txt
 d044ddcea5ea24b4eca8eb51bf87af04018820a32a053ae93df3f524cbede4bf  results/g02/sample/0300/config_014.txt
+ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g02/sample/0300/result.json
+90e80c71a80a7ae2a4509ec049ea95b2010aed532ac7f5364492b538e47a1e9f  results/g02/sample/0400/jobinfo.py
+646d17457558f13ac33fb444aba41fc5ebf026622932f37f17f750c4dfd6225e  results/g02/sample/0400/run
 be3777e053de6fa434678e8f71d578fde616cd61c3aedaeb1cd54ec764f9e3e3  results/g02/sample/0400/kwargs.json
 ef5d3842e5947475309d6ea38d8f80dfa9c0206b76368d26a241b911f2e8d03f  results/g02/sample/0400/kwargs.sha256
-00d4d8350d6eb91c9a7bafb77c7c8eb1f6b8103b6cf7cf2806a4ab353f77b86d  results/g02/sample/0400/run
 933c4c01e6bfbdb5071acec5f6f90fbebf8ba86c1c4ef990e2d1a3b70a15b1ac  results/g02/sample/0400/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/sample/0400/run.err
-ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g02/sample/0400/result.json
 946745d8d2a148fdc25881bf8b3b8900ce03cc9fe43797cdee5dddf5ace17c0e  results/g02/sample/0400/config_000.txt
 f66fe5f26b48c00a716acb3c18b951eeb5c9f3e84c0cab011cc69b0a71a726b6  results/g02/sample/0400/config_001.txt
 8187ef8b719106ffbd9955364edb96ad13f5356ab5e17e381cd2ef30fcff6ed6  results/g02/sample/0400/config_002.txt
 e2d6cd8dc1f42e84d7505a69767fc6763717de16c8cd315d49d79d352bb95a28  results/g02/sample/0400/config_003.txt
 bddb587d83807369f4fdb4196ac78220df8e47d4d4511294cf367e31aa0b44fe  results/g02/sample/0400/config_004.txt
 42512e9ac76e68195560505878b92f7074b04e91bc1e252ac0f7adb8fbd3fd55  results/g02/sample/0400/config_005.txt
 9b08f133ff3b3c37926c6a3ed69014d6282cc043f0d326086bf7474ed961103e  results/g02/sample/0400/config_006.txt
@@ -462,241 +529,281 @@
 51514ee2c4ae10a475fbe8be3d76ddc322c709937573f71fd0360f9ee5638a2f  results/g02/sample/0400/config_008.txt
 bba63bc5c1fbb10cfc1c09329334b349f5c27262833743cad5a23dda724d5b72  results/g02/sample/0400/config_009.txt
 025ece6d59f92229e646524753f1bec3c7315a74d1a45ddfbb64d489b69b4127  results/g02/sample/0400/config_010.txt
 6e9277cba787907044753b6c6b5711750beb94542252dc77d55a228b3f21283d  results/g02/sample/0400/config_011.txt
 7c7f3daa876d2a06c7264f6dcaf3aa13c8dc127f44ba776e15b113bf3f938935  results/g02/sample/0400/config_012.txt
 42b4b3c54aa1870aee98803cdfb6b100e2364461325a215aee15a82a8f1fd494  results/g02/sample/0400/config_013.txt
 c881dc9087ee49940baec12da2b704e403a56d1160235a54957dd6273c1f1a2a  results/g02/sample/0400/config_014.txt
+ec6a4aa709b9078b2c30b7162582752bb010fbff91d40f26054d5d1075d8f143  results/g02/sample/0400/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0000/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0000/run
 284e543f529863919bf7bba8cb25445b5fdcb3b27a37946bd021a157fd5c404b  results/g02/compute/0000/kwargs.json
 fb3df32d67daaf155efc1ef7f9374a52d305cabeaf654dfee46b063ee1349e5a  results/g02/compute/0000/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0000/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0000/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0000/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0000/result.json
 3e77f5e7348ef99bf88de47fa93e3c00261b6244dd46a366eec0431ebbe6025f  results/g02/compute/0000/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0000/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0001/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0001/run
 47c661d8cebba4e5b96720353c526dcecefa319fc1fe73cf6c54b3dc98b30ffd  results/g02/compute/0001/kwargs.json
 daa80c0f0f4232f34b2690e7ff90d50712ead8309665b0e065951e5dcc5827a3  results/g02/compute/0001/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0001/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0001/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0001/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0001/result.json
 743f84922f7f179eb3aca3b3b7b1d682bc701a029241e1c4bc3d5d9f94b91e2d  results/g02/compute/0001/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0001/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0002/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0002/run
 3ac6d77cc7696fd6bf15f06d7fb036f7fb56d496a81b87a13097964ddb1200fe  results/g02/compute/0002/kwargs.json
 741f996ecd209bac37cfc8aa51b113930d066780025e5f22711ecff79cd07530  results/g02/compute/0002/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0002/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0002/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0002/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0002/result.json
 1cc8edec81662b108f0307c4b469e790171148044671fd7053995fd14ac7c88c  results/g02/compute/0002/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0002/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0003/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0003/run
 2372518482ce722a780f62df8c800abbd054faf6221a6c5f4d2c428c3610c3f9  results/g02/compute/0003/kwargs.json
 67e106a76a9dce75be36a676b8a494c7d91bd5798a65df13dc42054cdb428dc9  results/g02/compute/0003/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0003/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0003/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0003/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0003/result.json
 b7940296fa12656ec34b3e70ff17f0757b96d50c59dde2c068fb57f5418688af  results/g02/compute/0003/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0003/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0004/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0004/run
 54356c66beba57fbf09c53031300b3f552920d2b90fa8dd9d4ff073d06321d1b  results/g02/compute/0004/kwargs.json
 8aa39d75ec59173a2a92ec7d4a9cfd92eb9df9e3be5034614eed1a0e605d9ffa  results/g02/compute/0004/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0004/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0004/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0004/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0004/result.json
 abe9f36962a3bd47e97a1479fe90cb5517e1bd0a5dad71e1ad86504d065521ad  results/g02/compute/0004/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0004/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0005/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0005/run
 758462d2cfd0aca472f9c25de2945db3cf4fcacff78b54883694069793c52768  results/g02/compute/0005/kwargs.json
 5ac6fb9b9538e2f7cbd34524972ae2247f305c429fcdd38e6183a52b200d2710  results/g02/compute/0005/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0005/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0005/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0005/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0005/result.json
 98f1f16bcc7d4e3764be2fa75d968d49b66b119886383dab80146ae416460f0d  results/g02/compute/0005/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0005/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0006/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0006/run
 5dfa9738368497f89ae0df61ffcfa0e8d69e61193bf9668c13e9ddf606880d8f  results/g02/compute/0006/kwargs.json
 18552857a270f71479f60f4d5684321d3e6c5b476b608257a240bd0e01eaffdd  results/g02/compute/0006/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0006/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0006/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0006/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0006/result.json
 8a1de8a112f635d6152d515d4f915e28637d2c3b1b72b92c38d47e1fcb5037c8  results/g02/compute/0006/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0006/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0007/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0007/run
 79b404bd75570e45c6f6de4dfc8165567ad72aa2ee0fcfb68537e4107dfb3651  results/g02/compute/0007/kwargs.json
 c6125ca416afa01b24800e38112782a289a8d47f4ee7aa596fb17ec8c0c70859  results/g02/compute/0007/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0007/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0007/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0007/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0007/result.json
 cb89db3eb7c0e8b6d284fb9c3b5a4885548418a44ae5ffe9a21781189f7b887b  results/g02/compute/0007/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0007/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0008/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0008/run
 7b3c6694601e9a812d46a2a7504e696ad4da8a394004c066215dc67fd1812a09  results/g02/compute/0008/kwargs.json
 3e0a2b0bdc0221059174d6b4e878e6e4fcfcb9158cf3d51be0b8690bb75020ba  results/g02/compute/0008/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0008/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0008/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0008/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0008/result.json
 14d3c298262648f77c66df02bd23232bc1919f6798d4ad0d1ae0c971c06f0aa6  results/g02/compute/0008/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0008/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0009/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0009/run
 f698e7e9f2e1eb6e1c4370869d26e5f4365988c4ba3555a7201fcd0f76db1e04  results/g02/compute/0009/kwargs.json
 ec8bcd851289ffc0fbb016e823eeaff736eb178d7001ec8213bb18831789f12a  results/g02/compute/0009/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0009/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0009/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0009/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0009/result.json
 c31138621f78f2a2a465444b4184f5734e6db7bab6c2976140bbca3fc984101c  results/g02/compute/0009/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0009/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0010/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0010/run
 f3ee02a79af2eec16db84c12e59dc3c5ae73a8fe3c7a675e147ff04a20458001  results/g02/compute/0010/kwargs.json
 8a1718e5a70c30260424dfd33b90ef221558a084f6c4498c12eda18fce8ca4f9  results/g02/compute/0010/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0010/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0010/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0010/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0010/result.json
 b75fbd35d285a394813029a0b2405e27fe2be0a0a681325a4a7439af7e8bebfc  results/g02/compute/0010/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0010/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0011/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0011/run
 f6ea23f7860d6a3e64d19f45a709c191fdcb17627890a5e45cd572f8113a2884  results/g02/compute/0011/kwargs.json
 24e1fbbb41351e90951c659eb9d316aae21986602959ebd8d21ad008573a134b  results/g02/compute/0011/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0011/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0011/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0011/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0011/result.json
 be8e13fbe48878a3473be349c522bc2753d69c5455925a4318a6569127cd98f9  results/g02/compute/0011/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0011/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0012/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0012/run
 9e4a32d6a254ff3185acc9d555d208f03d5c2ac0775dbb66f31c29f515013430  results/g02/compute/0012/kwargs.json
 b41f6e0df16f7637cf3afd618a5d6b83b1ff443c1a6710614ed26c37a42ac89e  results/g02/compute/0012/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0012/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0012/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0012/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0012/result.json
 f9740c55152e88a5a6123a55cba9b9580b81e2e77b7a53129b543b86a9669a91  results/g02/compute/0012/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0012/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0013/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0013/run
 44e237f746a7075fddeacb9655c709cc28f6277a764520e06cef15b79052732e  results/g02/compute/0013/kwargs.json
 5d924b2ea156c1b2028654b66af473b3c5e51fd6941825b2d57db645483c297d  results/g02/compute/0013/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0013/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0013/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0013/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0013/result.json
 1f261dc2531692dffced71da3f22277e9bacf24593b510e06e20be3ab878c44d  results/g02/compute/0013/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0013/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0014/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0014/run
 5d5c3efa80936a973fde9b28c0357073a07df23ea5ae5290313352ef30d78ea9  results/g02/compute/0014/kwargs.json
 eb1bec5ce62166d3ed2af62735715b30ddeedfe62b88ebd22ed660fa54e852de  results/g02/compute/0014/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0014/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0014/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0014/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0014/result.json
 6e6c643bb4758813dcb96746d97a611882a51e3b41336a337dcafdbcc2f51023  results/g02/compute/0014/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0014/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0015/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0015/run
 9d32d6e7fb9a1a64272480761624b39d1d4e7e04fca384207c3e6e350b696ea1  results/g02/compute/0015/kwargs.json
 8dba13f8c967bd92d8b3ab5b3b5cfdde4357b9bf4e4e46c5eac03194be4496cd  results/g02/compute/0015/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0015/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0015/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0015/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0015/result.json
 aa878d88183a22bc00d9e7d25901182313d2d9d34e5bc92833760222b9002504  results/g02/compute/0015/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0015/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0016/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0016/run
 b9918f527fffd2b9306c7c2e8d27e899aec49490c3c642944d39a2c7e4efa04c  results/g02/compute/0016/kwargs.json
 0665fd1a8c02e4b5d837fb65bba036076bdc267c0fdea63f3092aed1cc37608e  results/g02/compute/0016/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0016/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0016/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0016/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0016/result.json
 0e6886135cfd015e56c69a0e2442a94c6d4aba9255663887dcbe98c531ee9d38  results/g02/compute/0016/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0016/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0017/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0017/run
 1c2f9d6d332c46f1e5ddb174b7923755e5480c054470498fbd063aafc4ec7b1d  results/g02/compute/0017/kwargs.json
 a6a71e6a98a3c38d09d1cd65d3522de92e148eb48546a41e373442e7122d89c8  results/g02/compute/0017/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0017/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0017/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0017/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0017/result.json
 e79ce77b90ddcf4abaed81bb43bb8ca6b877afea329373f78cfc5211e207f051  results/g02/compute/0017/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0017/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0018/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0018/run
 8764346f07b2bbbb499326df321bee898c7846e6c3a1629855367062b2d679d2  results/g02/compute/0018/kwargs.json
 06156d2e2cd27781436740f303b48dce5462b8c0caa2d0efb4fe347cf6c4a7f8  results/g02/compute/0018/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0018/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0018/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0018/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0018/result.json
 0e8b0daf30d09fb107b36a40fed2fcc8b2029f3e104a2b9f3414bf4ec49ceb97  results/g02/compute/0018/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0018/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0019/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0019/run
 737212165bd64f22fc8399523fd264896459966ab92bc3464d2b96b0b2c94530  results/g02/compute/0019/kwargs.json
 ef6fa763b4c0db20c7c3916382c169adb6b15c604e6675107e5dd5ada672d197  results/g02/compute/0019/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0019/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0019/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0019/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0019/result.json
 2f6b7618ee4fc6501e4dc729c6bfa2d88b71bbed289774696feb7324cc7c6fb1  results/g02/compute/0019/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0019/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0020/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0020/run
 a658a46f23168cc0056fd594b7e0f3b128ddd82e3cc4136e494cc58971945864  results/g02/compute/0020/kwargs.json
 3eda7160ce838c4776a5b5ba2b8ca1d3fe7c48e2ad0e17ff03f5ae26f0d9474c  results/g02/compute/0020/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0020/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0020/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0020/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0020/result.json
 db5db248053f658b2862733cf3946ec156d430c2e6305d178315361c90611d83  results/g02/compute/0020/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0020/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0021/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0021/run
 ff88cde4da9742868c386a3477a9b94db1dc49f8123cce7310d155a82e7df5ac  results/g02/compute/0021/kwargs.json
 18e09fdc954880bf09b29167e16b640e2a9427db0a5f2b6e98c6646d0f6d8048  results/g02/compute/0021/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0021/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0021/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0021/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0021/result.json
 480c503f99f9cf4c41c3cc2a69072f2d7171a3782ffe3db22caf67e81617e3bc  results/g02/compute/0021/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0021/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0022/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0022/run
 938c6c2046b0ded704dacd50f8ece2104455199409701ba475e43d3b3fca04c7  results/g02/compute/0022/kwargs.json
 773c9df91facf2506c8efcb801413bda8a9f10633a1a6dabd2d66ed02555b55b  results/g02/compute/0022/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0022/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0022/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0022/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0022/result.json
 8257fc83a37838ca8546c7ef64b22f480427063abb8c64ce8c421cda89426a91  results/g02/compute/0022/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0022/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0023/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0023/run
 e7e29c1a5bd6d06a8cde9f63a6503f7fb83f8f030c0b899fd60a6daaca500918  results/g02/compute/0023/kwargs.json
 765f7f83279d86e12ecebb632f122605c0b0871c1d3f987933fff6dd1b5a12cc  results/g02/compute/0023/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0023/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0023/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0023/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0023/result.json
 908f746aca20a3c516674896ab0994cba66aaa1f0db52699985b96144d375c29  results/g02/compute/0023/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0023/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0024/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0024/run
 abbae7c01749c1b59e1733f7aa521b7f6adebae6fc5116336f4444a5ab0a7d39  results/g02/compute/0024/kwargs.json
 0b89103bbf657d82bd01238affd2f3649114e5c0a630f2340ab6591301528881  results/g02/compute/0024/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0024/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0024/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0024/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0024/result.json
 7a93aaad4286285c01e42f6037a5644a2fb16cb7e4e3acfbb0210f482720b3b8  results/g02/compute/0024/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0024/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0025/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0025/run
 a579173fbcc88a04ccc8abd26a24189602a12f6c1229ffc91f1fa9ef8aa1e4fd  results/g02/compute/0025/kwargs.json
 e9625686e9b2be018ae49ddcbeaf4c4c7251cac2a049cfe8833b6183c9c58d24  results/g02/compute/0025/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0025/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0025/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0025/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0025/result.json
 78210a865d11fb0bd6217fa2b78c179575c9c860712a7691bf8ade7bbd233a00  results/g02/compute/0025/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0025/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0026/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0026/run
 d0db1d4131294f248fb45b5677105db74d21891e66c1c8a9a2496b5925c49721  results/g02/compute/0026/kwargs.json
 f4a810458a4d99797ff7a52103323f212f99f8f205a9979aba9245c894036992  results/g02/compute/0026/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0026/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0026/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0026/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0026/result.json
 5734762465ff02c4b8559e26cf8ae91aed363822e9da2f2598a33ec36590e4a8  results/g02/compute/0026/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0026/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0027/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0027/run
 41a1c8a8902ee8bf0b27de93de11bacfc5a50a777fb973ae927f8ddb70a5bf16  results/g02/compute/0027/kwargs.json
 26bf4cb2971b5ddb71444f1b24116f647cbb454d1da37a4f908918b690e9ad08  results/g02/compute/0027/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0027/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0027/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0027/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0027/result.json
 ed14783dae2db651ffac89a510d61d20861e4efe7af60b4c3a8cc688bacebbae  results/g02/compute/0027/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0027/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0028/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0028/run
 a0ea987f2f1807b98b6ea7c006324b9b18943d68eacff53133f37c0826d277d4  results/g02/compute/0028/kwargs.json
 ed8515fa8f2eed49a635e3da0c1d6c177195ee0fa4389ed2919eceb5e14e3615  results/g02/compute/0028/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0028/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0028/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0028/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0028/result.json
 bd8560128be8478f201aa14bebd683e634a7e57623a4939c069d1db951984cc3  results/g02/compute/0028/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0028/result.json
+f3835beb24686be2b6739e345eb1142dcc2a436750577efacd2406252cb7c6bf  results/g02/compute/0029/jobinfo.py
+3b9f0ce4d532fe3fa049a34a8e46d8496f021e563df302bbdc931c9ba25245a2  results/g02/compute/0029/run
 d4a413283f837ed1b17b2a3278b19d31c6ad15c790fdbab9873fb781ff54c477  results/g02/compute/0029/kwargs.json
 fa66bf772cc6e0a1e9663b7f100c4b8f816454b825cea1655526795d634a7873  results/g02/compute/0029/kwargs.sha256
-c3e244cec5275bdb6c8ed8dbe6adc1cc30f578de51218039abb6c001555e78da  results/g02/compute/0029/run
 e361bf2923e1d88cc26c6490400c215db2bca93f5f765ed75d3d68c2285997f0  results/g02/compute/0029/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/compute/0029/run.err
-59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0029/result.json
 e83fe6c7a6d0b094c8e22ef7b062636cdbf778f9a5539d6dacba0f950ea7793f  results/g02/compute/0029/computation.out
+59dd3cd371df26aad678954a383fc5170c6b62317efd4f39f5a3ced9a6087bad  results/g02/compute/0029/result.json
+03d9234c1e884bcf52da8017a3ec2e2ed0246044460347e6b9899192fa9534f1  results/g02/train/00/helper.py
+02128fada93585c4c4a2f3b380490249eeb53d5129ec5d134ad09c18ef335409  results/g02/train/00/jobinfo.py
+4b6cd8bfd5f8950524210590ccde0f2dff2bf5df564c223fbab9c07cd27e47df  results/g02/train/00/run
 a91741fa0c790fe06cce14c46c9db099216678f1705b4323a7d7115ae2c049d9  results/g02/train/00/kwargs.json
 5d840ed88e41611d621f682ab632ae1b222dfaa58a1fbcdee147138a6c0f6fb4  results/g02/train/00/kwargs.sha256
-76e2b71e767b296c95c7ba699a7f2772cf6eb0ddc0505fa1d258d8324f420e60  results/g02/train/00/run
 9e1f20c2d44da467e31b53318b1da2c15476b144be1af26636cdd53e02dcd958  results/g02/train/00/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/train/00/run.err
-01ba4719c80b6fe911b091a7c05124b64eeece964e09c058ef8f9805daca546b  results/g02/train/00/result.extra
-64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g02/train/00/result.json
 258d95d479176069a2c58e99dd6669e0ad387001e8e34e941fa2098c8fb42885  results/g02/train/00/model.json
+64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g02/train/00/result.json
+78f6d7c3a681c95a8257e22c0a30bccdb430932050ce3f4c1da706f8563b07aa  results/g02/train/00/valuable.txt
+cc603c786fca9379cae82b35f1cc120fcf5cc60983cf8d6077abfab81d0ef0c9  results/g02/train/00/result.extra
+03d9234c1e884bcf52da8017a3ec2e2ed0246044460347e6b9899192fa9534f1  results/g02/train/01/helper.py
+02128fada93585c4c4a2f3b380490249eeb53d5129ec5d134ad09c18ef335409  results/g02/train/01/jobinfo.py
+4b6cd8bfd5f8950524210590ccde0f2dff2bf5df564c223fbab9c07cd27e47df  results/g02/train/01/run
 8f5710e5d6dfa25de9c8ae0c13a4aac4791235e307cbd900cb5306d6accc4810  results/g02/train/01/kwargs.json
 5d840ed88e41611d621f682ab632ae1b222dfaa58a1fbcdee147138a6c0f6fb4  results/g02/train/01/kwargs.sha256
-76e2b71e767b296c95c7ba699a7f2772cf6eb0ddc0505fa1d258d8324f420e60  results/g02/train/01/run
 947f5bc3478669f6467001592d2a97656a9701e80ad787eec02cf70d523f9f0a  results/g02/train/01/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/train/01/run.err
-01ba4719c80b6fe911b091a7c05124b64eeece964e09c058ef8f9805daca546b  results/g02/train/01/result.extra
-64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g02/train/01/result.json
 258d95d479176069a2c58e99dd6669e0ad387001e8e34e941fa2098c8fb42885  results/g02/train/01/model.json
+64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g02/train/01/result.json
+78f6d7c3a681c95a8257e22c0a30bccdb430932050ce3f4c1da706f8563b07aa  results/g02/train/01/valuable.txt
+cc603c786fca9379cae82b35f1cc120fcf5cc60983cf8d6077abfab81d0ef0c9  results/g02/train/01/result.extra
+03d9234c1e884bcf52da8017a3ec2e2ed0246044460347e6b9899192fa9534f1  results/g02/train/02/helper.py
+02128fada93585c4c4a2f3b380490249eeb53d5129ec5d134ad09c18ef335409  results/g02/train/02/jobinfo.py
+4b6cd8bfd5f8950524210590ccde0f2dff2bf5df564c223fbab9c07cd27e47df  results/g02/train/02/run
 1c3e87ef5113aac1fa5be415be6b50b3860f4ca90db72508b005c9b42c9f01a8  results/g02/train/02/kwargs.json
 5d840ed88e41611d621f682ab632ae1b222dfaa58a1fbcdee147138a6c0f6fb4  results/g02/train/02/kwargs.sha256
-76e2b71e767b296c95c7ba699a7f2772cf6eb0ddc0505fa1d258d8324f420e60  results/g02/train/02/run
 eb550b977e98fe486bad5b551a3a3e48ede11983f50b4cf470ead702448c4005  results/g02/train/02/run.out
 e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855  results/g02/train/02/run.err
-01ba4719c80b6fe911b091a7c05124b64eeece964e09c058ef8f9805daca546b  results/g02/train/02/result.extra
-64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g02/train/02/result.json
 258d95d479176069a2c58e99dd6669e0ad387001e8e34e941fa2098c8fb42885  results/g02/train/02/model.json
+64579890c3411f35e91b00df834119152809aec357d592bdd6a1675edb51376f  results/g02/train/02/result.json
+78f6d7c3a681c95a8257e22c0a30bccdb430932050ce3f4c1da706f8563b07aa  results/g02/train/02/valuable.txt
+cc603c786fca9379cae82b35f1cc120fcf5cc60983cf8d6077abfab81d0ef0c9  results/g02/train/02/result.extra
```

### Comparing `ParMan-0.2.0/tests/test_demos.py` & `Parman-0.3.0/tests/test_demos.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,76 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
 # --
-"""Run the demos to verify that they run without errors."""
+"""Run the demos to verify that they run without errors.
+
+If the files in the jobdemo are updated, refresh the hashes as follows:
+
+(
+    cd demos/jobdemo && ./jobdemo.py serial -p 0 &&
+    find results -type f | grep -v -E '(jobenv.sh|submit.sh)' | \
+     xargs sha256sum > ../../tests/jobdemo-results.sha256
+)
+"""
 
 
 import hashlib
 import os
 import runpy
 import shutil
 import subprocess
 from pathlib import Path
 
 import pytest
 
 
-def test_linreg(tmppath: Path):
-    run_script(["python3", "linreg.py"], Path("demos/demc"), [Path("linreg.py")], tmppath)
+def test_linreg(tmp_path: Path):
+    run_script(["python3", "linreg.py"], Path("demos", "demc"), [Path("linreg.py")], tmp_path)
 
 
-def test_naivemc(tmppath: Path):
+def test_naivemc(tmp_path: Path):
     run_script(
         ["python3", "naivemc.py", "1000", "10"],
-        Path("demos/demc"),
+        Path("demos", "demc"),
         [Path("linreg.py"), Path("naivemc.py")],
-        tmppath,
+        tmp_path,
     )
 
 
-def test_demc_serial(tmppath: Path):
+def test_demc_serial(tmp_path: Path):
     run_script(
         ["python3", "demc.py", "1000", "10"],
-        Path("demos/demc"),
+        Path("demos", "demc"),
         [Path("linreg.py"), Path("naivemc.py"), Path("demc.py")],
-        tmppath,
+        tmp_path,
     )
 
 
-def test_demc_parman(tmppath: Path):
+def test_demc_parman(tmp_path: Path):
     run_script(
         ["python3", "demc.py", "1000", "10", "--parman"],
-        Path("demos/demc"),
+        Path("demos", "demc"),
         [Path("linreg.py"), Path("naivemc.py"), Path("demc.py")],
-        tmppath,
+        tmp_path,
     )
 
 
 @pytest.mark.parametrize(
     "framework, schedule, in_temp",
     [
         ("dry", False, False),
@@ -77,97 +86,102 @@
         ("processes", True, True),
         ("parsl-local", False, False),
         ("parsl-local", False, True),
         ("parsl-local", True, False),
         ("parsl-local", True, True),
     ],
 )
-def test_jobdemo(framework: str, schedule: bool, in_temp: bool, tmppath: Path):
+def test_jobdemo(framework: str, schedule: bool, in_temp: bool, tmp_path: Path):
     args = ["python3", "jobdemo.py", framework, "--pause=0"]
     if schedule:
         args.append("-s")
     if in_temp:
         args.append("-t")
 
     relpaths = [
         Path("jobdemo.py"),
-        Path("templates/boot/jobinfo.py"),
-        Path("templates/boot/run"),
-        Path("templates/compute/jobinfo.py"),
-        Path("templates/compute/run"),
-        Path("templates/sample/jobinfo.py"),
-        Path("templates/sample/run"),
-        Path("templates/train/helper.py"),
-        Path("templates/train/jobinfo.py"),
-        Path("templates/train/run"),
+        Path("templates", "boot", "jobinfo.py"),
+        Path("templates", "boot", "run"),
+        Path("templates", "compute", "jobinfo.py"),
+        Path("templates", "compute", "run"),
+        Path("templates", "sample", "jobinfo.py"),
+        Path("templates", "sample", "run"),
+        Path("templates", "train", "helper.py"),
+        Path("templates", "train", "jobinfo.py"),
+        Path("templates", "train", "run"),
     ]
 
     # Run the jobdemo in a subprocess. (runpy does not work with parsl.)
-    run_script(args, Path("demos/jobdemo"), relpaths, tmppath)
+    run_script(args, Path("demos", "jobdemo"), relpaths, tmp_path)
     if framework != "dry":
-        check_files(tmppath, "tests/jobdemo-results.sha256")
+        check_files(tmp_path, Path("tests", "jobdemo-results.sha256"))
+
+
+def check_files(root, fn_sha):
+    with open(fn_sha) as f:
+        for line in f:
+            sha256, path = line.split()
+            check_hash(sha256, root / path)
+
+
+def check_hash(expected_sha256, path):
+    with open(path, "rb") as f:
+        content = f.read()
+        if hashlib.sha256(content).hexdigest() != expected_sha256:
+            raise AssertionError(f"SHA256 mismatch: {path}")
 
 
-def test_plastic_ibuprofen(tmppath: Path):
+def test_plastic_ibuprofen(tmp_path: Path):
     run_script(
         [
             "python3",
             "plastic.py",
             "ibuprofen.xyz",
             "ibuprofen.traj",
             "ibuprofen_final.xyz",
             "--steps=100",
         ],
-        Path("demos/inspiration/plastic"),
+        Path("demos", "inspiration", "plastic"),
         [Path("plastic.py"), Path("ibuprofen.xyz")],
-        tmppath,
+        tmp_path,
     )
 
 
-def test_plastic_alumina(tmppath: Path):
+def test_plastic_alumina(tmp_path: Path):
     run_script(
         [
             "python3",
             "plastic.py",
             "alumina.json",
             "alumina.traj",
             "alumina_final.xyz",
             "--steps=100",
         ],
-        Path("demos/inspiration/plastic"),
+        Path("demos", "inspiration", "plastic"),
         [Path("plastic.py"), Path("alumina.json")],
-        tmppath,
+        tmp_path,
     )
 
 
-def run_script(args: list[str], root: Path, relpaths: list[Path], tmppath: Path, nrepeat: int = 1):
+def run_script(args: list[str], root: Path, relpaths: list[Path], tmp_path: Path, nrepeat: int = 1):
     """Run a script with auxiliary files in a temporary directory."""
     # Put the files in place
     for relpath in relpaths:
-        dn_dst = tmppath / relpath.parent
+        dn_dst = tmp_path / relpath.parent
         dn_dst.mkdir(parents=True, exist_ok=True)
-        shutil.copy(root / relpath, tmppath / relpath)
+        shutil.copy(root / relpath, tmp_path / relpath)
     # Execute the script
-    env = os.environ | {"PYTHONPATH": Path("src/").absolute()}
+    env = os.environ | {"PYTHONPATH": Path("src").absolute()}
     for _ in range(nrepeat):
-        subprocess.run(args, check=True, cwd=tmppath, env=env)
-
-
-def check_files(root, fn_sha):
-    with open(fn_sha) as f:
-        for line in f:
-            sha256, path = line.split()
-            check_hash(sha256, root / path)
-
-
-def check_hash(expected_sha256, path):
-    with open(path, "rb") as f:
-        content = f.read()
-        if hashlib.sha256(content).hexdigest() != expected_sha256:
-            raise AssertionError(f"SHA256 mismatch: {path}")
+        subprocess.run(args, check=True, cwd=tmp_path, env=env)
 
 
 @pytest.mark.parametrize(
-    "path", ["demos/mindmutable.py", "demos/scheduledemo.py", "demos/waitdemo.py"]
+    "path",
+    [
+        Path("demos", "mindmutable.py"),
+        Path("demos", "scheduledemo.py"),
+        Path("demos", "waitdemo.py"),
+    ],
 )
 def test_simpledemo(path):
     runpy.run_path(path)
```

### Comparing `ParMan-0.2.0/tests/test_job.py` & `Parman-0.3.0/tests/test_job.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
@@ -62,24 +62,24 @@
 
 
 if __name__ == "__main__":
     main()
 """
 
 
-def test_envvar(tmppath: Path):
-    job, template_path = setup_jobfactory(tmppath, ENVVAR_JOBINFO, ENVVAR_RUN)
+def test_envvar(tmp_path: Path):
+    job, template_path = setup_jobfactory(tmp_path, ENVVAR_JOBINFO, ENVVAR_RUN)
     job.env = {"PARMAN_TEST_JOB_BBBB": "correct_b"}
     closure = job(template_path, "sample")
     os.environ["PARMAN_TEST_JOB_AAAA"] = "correct_a"
     result = closure.validated_call()
     assert result["aaaa"] == "correct_a"
     assert result["bbbb"] == "correct_b"
     assert len(result) == 2
-    with open(tmppath / "results" / "sample" / "jobenv.sh") as f:
+    with open(tmp_path / "results" / "sample" / "jobenv.sh") as f:
         lines = f.readlines()
     assert lines[0] == 'export PARMAN_TEST_JOB_BBBB="correct_b"\n'
     assert lines[1] == f'export PARMAN_WORKDIR="{os.getcwd()}"\n'
     assert len(lines) == 2
 
 
 OPTIONAL_JOBINFO = """
@@ -103,16 +103,16 @@
 
 
 if __name__ == "__main__":
     main()
 """
 
 
-def test_optional(tmppath: Path):
-    job, template_path = setup_jobfactory(tmppath, OPTIONAL_JOBINFO, OPTIONAL_RUN)
+def test_optional(tmp_path: Path):
+    job, template_path = setup_jobfactory(tmp_path, OPTIONAL_JOBINFO, OPTIONAL_RUN)
     closure = job(template_path, "sample", first=1)
     result = closure.validated_call()
     assert result == 3
 
 
 @pytest.mark.parametrize(
     "inp, out",
@@ -122,24 +122,92 @@
         ("  #  aaa # bbb \n", ""),
     ],
 )
 def test_strip_line(inp, out):
     assert strip_line(inp) == out
 
 
-def test_write_sh_env(tmppath: Path):
-    path_rc = tmppath / "test.sh"
+def test_write_sh_env(tmp_path: Path):
+    path_rc = tmp_path / "test.sh"
     write_sh_env(path_rc, {"ABC": "123", "FOO": "BAR"})
     with open(path_rc) as f:
         lines = f.readlines()
     assert lines[0] == 'export ABC="123"\n'
     assert lines[1] == 'export FOO="BAR"\n'
 
 
-def test_write_sh_env_exceptions(tmppath: Path):
-    path_rc = tmppath / "test.sh"
+def test_write_sh_env_exceptions(tmp_path: Path):
+    path_rc = tmp_path / "test.sh"
     with pytest.raises(ValueError):
         write_sh_env(path_rc, {"1ABC": "z"})
     with pytest.raises(ValueError):
         write_sh_env(path_rc, {"": "z"})
     with pytest.raises(ValueError):
         write_sh_env(path_rc, {1: "z"})
+
+
+NONE_JOBINFO = """
+def mock(first: int, second: int = 2) -> int:
+    return None
+"""
+
+NONE_RUN = """\
+#!/usr/bin/env python
+
+import json
+import os
+
+
+def main():
+    with open("kwargs.json") as f:
+        kwargs = json.load(f)
+
+    with open("result.json", "w") as f:
+        f.write("null")
+
+
+if __name__ == "__main__":
+    main()
+"""
+
+
+def test_none(tmp_path: Path):
+    job, template_path = setup_jobfactory(tmp_path, NONE_JOBINFO, NONE_RUN)
+    closure = job(template_path, "sample", first=1, second=3)
+    result = closure.validated_call()
+    assert result is None
+
+
+PATH_JOBINFO = """
+from pathlib import Path
+def mock(some_input: Path) -> Path:
+    return Path("__foo__")
+"""
+
+PATH_RUN = """\
+#!/usr/bin/env python
+
+import json
+import os
+
+
+def main():
+    with open("kwargs.json") as f:
+        kwargs = json.load(f)
+
+    with open("result.json", "w") as f:
+        json.dump("some_output.txt", f)
+
+
+if __name__ == "__main__":
+    main()
+"""
+
+
+def test_path(tmp_path: Path):
+    job, template_path = setup_jobfactory(tmp_path, PATH_JOBINFO, PATH_RUN)
+    (tmp_path / "results").mkdir()
+    with open(tmp_path / "results/some_input.txt", "w") as f:
+        f.write("foo bar\n")
+    closure = job(template_path, "sample", some_input=Path("some_input.txt"))
+    result = closure.validated_call()
+    assert result == Path("sample/some_output.txt")
```

### Comparing `ParMan-0.2.0/tests/test_metafunc.py` & `Parman-0.3.0/tests/test_metafunc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# ParMan extends Python concurrent.futures to facilitate parallel workflows.
+# Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
@@ -34,12 +34,11 @@
 
 
 def test_basics():
     metafunc = MinimalMetaFunc(compute_sum, compute_sum_mock)
     assert metafunc.describe() == "compute_sum"
     assert metafunc(1) == 3
     assert metafunc.get_signature() == inspect.signature(compute_sum)
-    assert metafunc.cached_result("does", "not", "matter") == NotImplemented
     assert metafunc.get_parameters_api() == {"first": int, "second": int}
     assert metafunc.get_result_mock(1, 3) == 42
     assert metafunc.get_result_api(1, 3) == int
     assert metafunc.get_resources() == {}
```

### Comparing `ParMan-0.2.0/tests/test_scheduler.py` & `Parman-0.3.0/tests/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/tests/test_treeleaf.py` & `Parman-0.3.0/tests/test_treeleaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

### Comparing `ParMan-0.2.0/tests/test_waitfuture.py` & `Parman-0.3.0/tests/test_waitfuture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Parman extends Python concurrent.futures to facilitate parallel workflows.
 # Copyright (C) 2023 Toon Verstraelen
 #
-# This file is part of ParMan.
+# This file is part of Parman.
 #
-# ParMan is free software; you can redistribute it and/or
+# Parman is free software; you can redistribute it and/or
 # modify it under the terms of the GNU General Public License
 # as published by the Free Software Foundation; either version 3
 # of the License, or (at your option) any later version.
 #
-# ParMan is distributed in the hope that it will be useful,
+# Parman is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>
 #
```

