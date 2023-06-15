# Comparing `tmp/Parman-0.3.0.tar.gz` & `tmp/Parman-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Parman-0.3.0.tar", last modified: Thu Jun 15 10:55:22 2023, max compression
+gzip compressed data, was "Parman-0.3.1.tar", last modified: Thu Jun 15 11:00:46 2023, max compression
```

## Comparing `Parman-0.3.0.tar` & `Parman-0.3.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.725360 Parman-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-15 10:55:02.000000 Parman-0.3.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-15 10:55:02.000000 Parman-0.3.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-15 10:55:02.000000 Parman-0.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-15 10:55:02.000000 Parman-0.3.0/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 10:55:02.000000 Parman-0.3.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-15 10:55:02.000000 Parman-0.3.0/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-15 10:55:02.000000 Parman-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-15 10:55:02.000000 Parman-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-15 10:55:02.000000 Parman-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 10:55:02.000000 Parman-0.3.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-15 10:55:02.000000 Parman-0.3.0/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-06-15 10:55:22.725360 Parman-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-15 10:55:02.000000 Parman-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/demc/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     6485 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/demc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4625 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/linreg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5231 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/demc/naivemc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/inspiration/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/inspiration/plastic/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/alumina.json
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/ibuprofen.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8333 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/plastic.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/inspiration/plastic/run
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/jobdemo/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)     6604 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/jobdemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.713360 Parman-0.3.0/demos/jobdemo/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/jobdemo/templates/boot/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/boot/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/boot/run
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/boot/submit.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/jobdemo/templates/compute/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/compute/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/compute/run
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/compute/submit.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.717360 Parman-0.3.0/demos/jobdemo/templates/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/sample/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/sample/run
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/sample/submit.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/demos/jobdemo/templates/train/
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/train/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/train/jobinfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/train/run
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/jobdemo/templates/train/submit.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1080 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/mindmutable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/scheduledemo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1002 2023-06-15 10:55:02.000000 Parman-0.3.0/demos/waitdemo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-15 10:55:02.000000 Parman-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 10:55:22.725360 Parman-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.713360 Parman-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/Parman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 10:55:22.000000 Parman-0.3.0/src/Parman.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/parman/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 10:55:22.000000 Parman-0.3.0/src/parman/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/parman/clerks/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/clerks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/clerks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/clerks/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/clerks/localtemp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/closure.py
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/metafunc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/parman/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/dry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/future.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/parsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/runners/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.721360 Parman-0.3.0/src/parman/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/scripts/sbatch_wait.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/treeleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/waitfuture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-15 10:55:02.000000 Parman-0.3.0/src/parman/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:55:22.725360 Parman-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    81848 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/jobdemo-results.sha256
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_metafunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_runners.py
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_treeleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-15 10:55:02.000000 Parman-0.3.0/tests/test_waitfuture.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.714451 Parman-0.3.1/
+-rw-r--r--   0 toon      (1000) toon      (1000)      283 2023-03-26 18:10:25.000000 Parman-0.3.1/.editorconfig
+-rw-r--r--   0 toon      (1000) toon      (1000)      125 2023-05-07 10:00:26.000000 Parman-0.3.1/.git_archival.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       32 2023-05-07 10:00:26.000000 Parman-0.3.1/.gitattributes
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.704451 Parman-0.3.1/.github/
+-rw-r--r--   0 toon      (1000) toon      (1000)      257 2023-05-09 18:09:03.000000 Parman-0.3.1/.github/dependabot.yaml
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.704451 Parman-0.3.1/.github/workflows/
+-rw-r--r--   0 toon      (1000) toon      (1000)     1038 2023-05-10 14:57:38.000000 Parman-0.3.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 toon      (1000) toon      (1000)      863 2023-05-09 08:26:29.000000 Parman-0.3.1/.github/workflows/pytest.yaml
+-rw-r--r--   0 toon      (1000) toon      (1000)      108 2023-05-07 09:14:41.000000 Parman-0.3.1/.gitignore
+-rw-r--r--   0 toon      (1000) toon      (1000)     1006 2023-06-15 10:54:31.000000 Parman-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 toon      (1000) toon      (1000)     1890 2023-06-15 10:57:02.000000 Parman-0.3.1/CHANGELOG.md
+-rw-r--r--   0 toon      (1000) toon      (1000)     7652 2017-09-30 07:16:26.000000 Parman-0.3.1/COPYING
+-rw-r--r--   0 toon      (1000) toon      (1000)      189 2023-06-15 10:54:31.000000 Parman-0.3.1/DEVELOPMENT.md
+-rw-r--r--   0 toon      (1000) toon      (1000)    13321 2023-06-15 11:00:46.713451 Parman-0.3.1/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)     3407 2023-05-10 04:14:13.000000 Parman-0.3.1/README.md
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.704451 Parman-0.3.1/demos/
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.705452 Parman-0.3.1/demos/demc/
+-rw-r--r--   0 toon      (1000) toon      (1000)        6 2023-05-05 04:46:51.000000 Parman-0.3.1/demos/demc/.gitignore
+-rw-r--r--   0 toon      (1000) toon      (1000)     3374 2023-05-06 10:51:55.000000 Parman-0.3.1/demos/demc/README.md
+-rwxr-xr-x   0 toon      (1000) toon      (1000)     6485 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/demc/demc.py
+-rwxr-xr-x   0 toon      (1000) toon      (1000)     4625 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/demc/linreg.py
+-rwxr-xr-x   0 toon      (1000) toon      (1000)     5231 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/demc/naivemc.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.705452 Parman-0.3.1/demos/inspiration/
+-rw-r--r--   0 toon      (1000) toon      (1000)       99 2023-04-26 17:51:38.000000 Parman-0.3.1/demos/inspiration/README.md
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.706452 Parman-0.3.1/demos/inspiration/plastic/
+-rw-r--r--   0 toon      (1000) toon      (1000)       17 2023-04-26 17:51:38.000000 Parman-0.3.1/demos/inspiration/plastic/.gitignore
+-rw-r--r--   0 toon      (1000) toon      (1000)      541 2023-04-26 17:51:38.000000 Parman-0.3.1/demos/inspiration/plastic/README.md
+-rw-r--r--   0 toon      (1000) toon      (1000)    16805 2023-04-26 17:51:38.000000 Parman-0.3.1/demos/inspiration/plastic/alumina.json
+-rw-r--r--   0 toon      (1000) toon      (1000)     1625 2023-04-26 17:51:38.000000 Parman-0.3.1/demos/inspiration/plastic/ibuprofen.xyz
+-rw-r--r--   0 toon      (1000) toon      (1000)      204 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/inspiration/plastic/jobinfo.py
+-rwxr-xr-x   0 toon      (1000) toon      (1000)     8333 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/inspiration/plastic/plastic.py
+-rw-r--r--   0 toon      (1000) toon      (1000)      413 2023-04-26 17:51:38.000000 Parman-0.3.1/demos/inspiration/plastic/run
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.706452 Parman-0.3.1/demos/jobdemo/
+-rw-r--r--   0 toon      (1000) toon      (1000)       39 2023-04-17 04:49:28.000000 Parman-0.3.1/demos/jobdemo/.gitignore
+-rwxr-xr-x   0 toon      (1000) toon      (1000)     6604 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/jobdemo/jobdemo.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.702452 Parman-0.3.1/demos/jobdemo/templates/
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.707451 Parman-0.3.1/demos/jobdemo/templates/boot/
+-rw-r--r--   0 toon      (1000) toon      (1000)      213 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/jobdemo/templates/boot/jobinfo.py
+-rwxr-xr-x   0 toon      (1000) toon      (1000)      562 2023-04-15 10:09:17.000000 Parman-0.3.1/demos/jobdemo/templates/boot/run
+-rwxr-xr-x   0 toon      (1000) toon      (1000)      103 2023-05-03 16:22:17.000000 Parman-0.3.1/demos/jobdemo/templates/boot/submit.sh
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.707451 Parman-0.3.1/demos/jobdemo/templates/compute/
+-rw-r--r--   0 toon      (1000) toon      (1000)      175 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/jobdemo/templates/compute/jobinfo.py
+-rwxr-xr-x   0 toon      (1000) toon      (1000)      649 2023-05-07 15:59:48.000000 Parman-0.3.1/demos/jobdemo/templates/compute/run
+-rwxr-xr-x   0 toon      (1000) toon      (1000)      103 2023-05-03 16:22:17.000000 Parman-0.3.1/demos/jobdemo/templates/compute/submit.sh
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.707451 Parman-0.3.1/demos/jobdemo/templates/sample/
+-rw-r--r--   0 toon      (1000) toon      (1000)      255 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/jobdemo/templates/sample/jobinfo.py
+-rwxr-xr-x   0 toon      (1000) toon      (1000)      852 2023-05-09 14:55:20.000000 Parman-0.3.1/demos/jobdemo/templates/sample/run
+-rwxr-xr-x   0 toon      (1000) toon      (1000)      103 2023-05-03 16:22:17.000000 Parman-0.3.1/demos/jobdemo/templates/sample/submit.sh
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.708452 Parman-0.3.1/demos/jobdemo/templates/train/
+-rwxr-xr-x   0 toon      (1000) toon      (1000)      654 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/jobdemo/templates/train/helper.py
+-rw-r--r--   0 toon      (1000) toon      (1000)      191 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/jobdemo/templates/train/jobinfo.py
+-rwxr-xr-x   0 toon      (1000) toon      (1000)      273 2023-05-09 09:51:25.000000 Parman-0.3.1/demos/jobdemo/templates/train/run
+-rwxr-xr-x   0 toon      (1000) toon      (1000)      103 2023-05-03 16:22:17.000000 Parman-0.3.1/demos/jobdemo/templates/train/submit.sh
+-rwxr-xr-x   0 toon      (1000) toon      (1000)     1080 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/mindmutable.py
+-rwxr-xr-x   0 toon      (1000) toon      (1000)     1301 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/scheduledemo.py
+-rwxr-xr-x   0 toon      (1000) toon      (1000)     1002 2023-05-16 14:28:11.000000 Parman-0.3.1/demos/waitdemo.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1582 2023-06-15 10:36:04.000000 Parman-0.3.1/pyproject.toml
+-rw-r--r--   0 toon      (1000) toon      (1000)       38 2023-06-15 11:00:46.714451 Parman-0.3.1/setup.cfg
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.702452 Parman-0.3.1/src/
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.709452 Parman-0.3.1/src/Parman.egg-info/
+-rw-r--r--   0 toon      (1000) toon      (1000)    13321 2023-06-15 11:00:46.000000 Parman-0.3.1/src/Parman.egg-info/PKG-INFO
+-rw-r--r--   0 toon      (1000) toon      (1000)     2223 2023-06-15 11:00:46.000000 Parman-0.3.1/src/Parman.egg-info/SOURCES.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)        1 2023-06-15 11:00:46.000000 Parman-0.3.1/src/Parman.egg-info/dependency_links.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       71 2023-06-15 11:00:46.000000 Parman-0.3.1/src/Parman.egg-info/entry_points.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)       21 2023-06-15 11:00:46.000000 Parman-0.3.1/src/Parman.egg-info/requires.txt
+-rw-r--r--   0 toon      (1000) toon      (1000)        7 2023-06-15 11:00:46.000000 Parman-0.3.1/src/Parman.egg-info/top_level.txt
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.710451 Parman-0.3.1/src/parman/
+-rw-r--r--   0 toon      (1000) toon      (1000)      943 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/__init__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)      160 2023-06-15 11:00:46.000000 Parman-0.3.1/src/parman/_version.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.710451 Parman-0.3.1/src/parman/clerks/
+-rw-r--r--   0 toon      (1000) toon      (1000)      849 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/clerks/__init__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5155 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/clerks/base.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1875 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/clerks/local.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2904 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/clerks/localtemp.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4209 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/closure.py
+-rw-r--r--   0 toon      (1000) toon      (1000)    19574 2023-06-15 10:36:04.000000 Parman-0.3.1/src/parman/job.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     8461 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/metafunc.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.711452 Parman-0.3.1/src/parman/runners/
+-rw-r--r--   0 toon      (1000) toon      (1000)      830 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/runners/__init__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1264 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/runners/base.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1766 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/runners/concurrent.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1238 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/runners/dry.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     4556 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/runners/future.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2110 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/runners/parsl.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1181 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/runners/serial.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     9245 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/scheduler.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.712452 Parman-0.3.1/src/parman/scripts/
+-rw-r--r--   0 toon      (1000) toon      (1000)      814 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/scripts/__init__.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     7642 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/scripts/sbatch_wait.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5186 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/treeleaf.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     7040 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/waitfuture.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1322 2023-05-16 14:28:11.000000 Parman-0.3.1/src/parman/wrapper.py
+drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2023-06-15 11:00:46.713451 Parman-0.3.1/tests/
+-rw-r--r--   0 toon      (1000) toon      (1000)     1381 2023-05-16 14:28:11.000000 Parman-0.3.1/tests/conftest.py
+-rw-r--r--   0 toon      (1000) toon      (1000)    81848 2023-05-09 15:15:57.000000 Parman-0.3.1/tests/jobdemo-results.sha256
+-rw-r--r--   0 toon      (1000) toon      (1000)     5490 2023-05-16 14:28:11.000000 Parman-0.3.1/tests/test_demos.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5328 2023-06-15 10:36:04.000000 Parman-0.3.1/tests/test_job.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     1480 2023-05-16 14:28:11.000000 Parman-0.3.1/tests/test_metafunc.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     2111 2023-05-16 14:28:11.000000 Parman-0.3.1/tests/test_runners.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5561 2023-05-16 14:28:11.000000 Parman-0.3.1/tests/test_scheduler.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     3738 2023-05-16 14:28:11.000000 Parman-0.3.1/tests/test_treeleaf.py
+-rw-r--r--   0 toon      (1000) toon      (1000)     5812 2023-05-16 14:28:11.000000 Parman-0.3.1/tests/test_waitfuture.py
```

### Comparing `Parman-0.3.0/.github/workflows/pypi.yaml` & `Parman-0.3.1/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/.github/workflows/pytest.yaml` & `Parman-0.3.1/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/.pre-commit-config.yaml` & `Parman-0.3.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,14 @@
   hooks:
     - id: remove-crlf
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
     - id: black
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: 'v0.0.269'
+  rev: 'v0.0.272'
   hooks:
     - id: ruff
 - repo: https://github.com/python-jsonschema/check-jsonschema
-  rev: 0.23.0
+  rev: 0.23.1
   hooks:
     - id: check-github-workflows
```

### Comparing `Parman-0.3.0/CHANGELOG.md` & `Parman-0.3.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.1] - 2023-06-15
+
+### Fixed
+
+- Fix PyPI mistake. 0.3.0 will be yanked.
+
 ## [0.3.0] - 2023-06-15
 
 ### Added
 
 - When `kwargs.json` is manually filled with `null`, it is refreshed under the assumption
   that the existing results are consistent with the new `kwargs.json` file.
   This is useful when one is refactoring workflows and one wants to reuse some results of
```

### Comparing `Parman-0.3.0/COPYING` & `Parman-0.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/PKG-INFO` & `Parman-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Parman
-Version: 0.3.0
+Version: 0.3.1
 Summary: Parman extends Python concurrent.futures to facilitate parallel workflows
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `Parman-0.3.0/README.md` & `Parman-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/demc/README.md` & `Parman-0.3.1/demos/demc/README.md`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/demc/demc.py` & `Parman-0.3.1/demos/demc/demc.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/demc/linreg.py` & `Parman-0.3.1/demos/demc/linreg.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/demc/naivemc.py` & `Parman-0.3.1/demos/demc/naivemc.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/inspiration/plastic/README.md` & `Parman-0.3.1/demos/inspiration/plastic/README.md`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/inspiration/plastic/alumina.json` & `Parman-0.3.1/demos/inspiration/plastic/alumina.json`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/inspiration/plastic/ibuprofen.xyz` & `Parman-0.3.1/demos/inspiration/plastic/ibuprofen.xyz`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/inspiration/plastic/plastic.py` & `Parman-0.3.1/demos/inspiration/plastic/plastic.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/jobdemo/jobdemo.py` & `Parman-0.3.1/demos/jobdemo/jobdemo.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/jobdemo/templates/boot/run` & `Parman-0.3.1/demos/jobdemo/templates/boot/run`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/jobdemo/templates/compute/run` & `Parman-0.3.1/demos/jobdemo/templates/compute/run`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/jobdemo/templates/sample/run` & `Parman-0.3.1/demos/jobdemo/templates/sample/run`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/jobdemo/templates/train/helper.py` & `Parman-0.3.1/demos/jobdemo/templates/train/helper.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/mindmutable.py` & `Parman-0.3.1/demos/mindmutable.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/scheduledemo.py` & `Parman-0.3.1/demos/scheduledemo.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/demos/waitdemo.py` & `Parman-0.3.1/demos/waitdemo.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/pyproject.toml` & `Parman-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/Parman.egg-info/PKG-INFO` & `Parman-0.3.1/src/Parman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Parman
-Version: 0.3.0
+Version: 0.3.1
 Summary: Parman extends Python concurrent.futures to facilitate parallel workflows
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `Parman-0.3.0/src/Parman.egg-info/SOURCES.txt` & `Parman-0.3.1/src/Parman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/__init__.py` & `Parman-0.3.1/src/parman/__init__.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/clerks/__init__.py` & `Parman-0.3.1/src/parman/clerks/__init__.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/clerks/base.py` & `Parman-0.3.1/src/parman/clerks/base.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/clerks/local.py` & `Parman-0.3.1/src/parman/clerks/local.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/clerks/localtemp.py` & `Parman-0.3.1/src/parman/clerks/localtemp.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/closure.py` & `Parman-0.3.1/src/parman/closure.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/job.py` & `Parman-0.3.1/src/parman/job.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/metafunc.py` & `Parman-0.3.1/src/parman/metafunc.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/runners/__init__.py` & `Parman-0.3.1/src/parman/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/runners/base.py` & `Parman-0.3.1/src/parman/runners/base.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/runners/concurrent.py` & `Parman-0.3.1/src/parman/runners/concurrent.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/runners/dry.py` & `Parman-0.3.1/src/parman/runners/dry.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/runners/future.py` & `Parman-0.3.1/src/parman/runners/future.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/runners/parsl.py` & `Parman-0.3.1/src/parman/runners/parsl.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/runners/serial.py` & `Parman-0.3.1/src/parman/runners/serial.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/scheduler.py` & `Parman-0.3.1/src/parman/scheduler.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/scripts/__init__.py` & `Parman-0.3.1/src/parman/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/scripts/sbatch_wait.py` & `Parman-0.3.1/src/parman/scripts/sbatch_wait.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/treeleaf.py` & `Parman-0.3.1/src/parman/treeleaf.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/waitfuture.py` & `Parman-0.3.1/src/parman/waitfuture.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/src/parman/wrapper.py` & `Parman-0.3.1/src/parman/wrapper.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/tests/conftest.py` & `Parman-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/tests/jobdemo-results.sha256` & `Parman-0.3.1/tests/jobdemo-results.sha256`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/tests/test_demos.py` & `Parman-0.3.1/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/tests/test_job.py` & `Parman-0.3.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/tests/test_metafunc.py` & `Parman-0.3.1/tests/test_metafunc.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/tests/test_runners.py` & `Parman-0.3.1/tests/test_runners.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/tests/test_scheduler.py` & `Parman-0.3.1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/tests/test_treeleaf.py` & `Parman-0.3.1/tests/test_treeleaf.py`

 * *Files identical despite different names*

### Comparing `Parman-0.3.0/tests/test_waitfuture.py` & `Parman-0.3.1/tests/test_waitfuture.py`

 * *Files identical despite different names*

