# Comparing `tmp/gstools-1.4.1.tar.gz` & `tmp/gstools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gstools-1.4.1.tar", last modified: Thu Nov  3 13:09:52 2022, max compression
+gzip compressed data, was "gstools-1.5.0.tar", last modified: Thu Jun 15 19:25:25 2023, max compression
```

## Comparing `gstools-1.4.1.tar` & `gstools-1.5.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.590161 gstools-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-11-03 13:06:45.000000 gstools-1.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-03 13:06:45.000000 gstools-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    20804 2022-11-03 13:09:52.590161 gstools-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18835 2022-11-03 13:06:45.000000 gstools-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4307 2022-11-03 13:06:45.000000 gstools-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-03 13:09:52.590161 gstools-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-11-03 13:06:45.000000 gstools-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.582160 gstools-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.586160 gstools-1.4.1/src/gstools/
--rw-r--r--   0 runner    (1001) docker     (121)     4026 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-11-03 13:09:52.000000 gstools-1.4.1/src/gstools/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.586160 gstools-1.4.1/src/gstools/covmodel/
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/covmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    39574 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/covmodel/base.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    20677 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/covmodel/fit.py
--rw-r--r--   0 runner    (1001) docker     (121)    27726 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/covmodel/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8367 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/covmodel/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)    17576 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/covmodel/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    18517 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/covmodel/tpl_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.586160 gstools-1.4.1/src/gstools/field/
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/field/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23682 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/field/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    10391 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/field/cond_srf.py
--rw-r--r--   0 runner    (1001) docker     (121)    16921 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/field/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)    12391 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/field/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     7953 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/field/srf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/field/summator.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     9271 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/field/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/field/upscaling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.586160 gstools-1.4.1/src/gstools/krige/
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/krige/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    28691 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/krige/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1619 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/krige/krigesum.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    19905 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/krige/methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/krige/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.586160 gstools-1.4.1/src/gstools/normalizer/
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8530 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/normalizer/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    10378 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/normalizer/methods.py
--rw-r--r--   0 runner    (1001) docker     (121)     6409 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/normalizer/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.590161 gstools-1.4.1/src/gstools/random/
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7791 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/random/rng.py
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/random/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.590161 gstools-1.4.1/src/gstools/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7893 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/tools/export.py
--rw-r--r--   0 runner    (1001) docker     (121)    20463 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/tools/geometric.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4315 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/tools/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7476 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/tools/special.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.590161 gstools-1.4.1/src/gstools/transform/
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10988 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/transform/array.py
--rw-r--r--   0 runner    (1001) docker     (121)    19751 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/transform/field.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.590161 gstools-1.4.1/src/gstools/variogram/
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/variogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3057 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/variogram/binning.py
--rw-r--r--   0 runner    (1001) docker     (121)    10854 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/variogram/estimator.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    18130 2022-11-03 13:06:45.000000 gstools-1.4.1/src/gstools/variogram/variogram.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.590161 gstools-1.4.1/src/gstools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-11-03 13:09:52.000000 gstools-1.4.1/src/gstools.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 13:09:52.590161 gstools-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_condition.py
--rw-r--r--   0 runner    (1001) docker     (121)    17002 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_covmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     4077 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_incomprrandmeth.py
--rw-r--r--   0 runner    (1001) docker     (121)    11119 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_krige.py
--rw-r--r--   0 runner    (1001) docker     (121)     5863 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_latlon.py
--rw-r--r--   0 runner    (1001) docker     (121)     7166 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_randmeth.py
--rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (121)    12993 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_srf.py
--rw-r--r--   0 runner    (1001) docker     (121)     6375 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)    11207 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_variogram_structured.py
--rw-r--r--   0 runner    (1001) docker     (121)    15048 2022-11-03 13:06:45.000000 gstools-1.4.1/tests/test_variogram_unstructured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.068425 gstools-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-15 19:20:43.000000 gstools-1.5.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 19:20:43.000000 gstools-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20802 2023-06-15 19:25:25.064425 gstools-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18833 2023-06-15 19:20:43.000000 gstools-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-15 19:20:43.000000 gstools-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:25:25.068425 gstools-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-15 19:20:43.000000 gstools-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.052425 gstools-1.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.052425 gstools-1.5.0/src/gstools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 19:25:24.000000 gstools-1.5.0/src/gstools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.052425 gstools-1.5.0/src/gstools/covmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/covmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41881 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/covmodel/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20705 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/covmodel/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27702 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/covmodel/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/covmodel/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19517 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/covmodel/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18493 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/covmodel/tpl_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.056425 gstools-1.5.0/src/gstools/field/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/field/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23829 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/field/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10367 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/field/cond_srf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/field/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/field/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/field/srf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/field/summator.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/field/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/field/upscaling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.056425 gstools-1.5.0/src/gstools/krige/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/krige/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29420 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/krige/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/krige/krigesum.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/krige/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/krige/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.056425 gstools-1.5.0/src/gstools/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/normalizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/normalizer/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/normalizer/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.060425 gstools-1.5.0/src/gstools/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/random/rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/random/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.060425 gstools-1.5.0/src/gstools/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/tools/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22104 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/tools/geometric.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4291 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/tools/special.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.060425 gstools-1.5.0/src/gstools/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/transform/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20441 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/transform/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.060425 gstools-1.5.0/src/gstools/variogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/variogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/variogram/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/variogram/estimator.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    18829 2023-06-15 19:20:43.000000 gstools-1.5.0/src/gstools/variogram/variogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.064425 gstools-1.5.0/src/gstools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-15 19:25:25.000000 gstools-1.5.0/src/gstools.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:25:25.064425 gstools-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16978 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_covmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_incomprrandmeth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_krige.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_latlon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_randmeth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_srf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_variogram_structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-06-15 19:20:43.000000 gstools-1.5.0/tests/test_variogram_unstructured.py
```

### Comparing `gstools-1.4.1/AUTHORS.md` & `gstools-1.5.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `gstools-1.4.1/LICENSE` & `gstools-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gstools-1.4.1/PKG-INFO` & `gstools-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gstools
-Version: 1.4.1
+Version: 1.5.0
 Summary: GSTools: A geostatistical toolbox.
 Author-email: "Sebastian Müller, Lennart Schüler" <info@geostat-framework.org>
 License: LGPL-3.0
 Project-URL: Changelog, https://github.com/GeoStat-Framework/GSTools/blob/main/CHANGELOG.md
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/gstools
 Project-URL: Documentation, https://gstools.readthedocs.io
 Project-URL: Homepage, https://geostat-framework.org/#gstools
@@ -187,15 +187,15 @@
 
 ```python
 import matplotlib.pyplot as plt
 import cartopy.crs as ccrs
 import gstools as gs
 # define a structured field by latitude and longitude
 lat = lon = range(-80, 81)
-model = gs.Gaussian(latlon=True, len_scale=777, rescale=gs.EARTH_RADIUS)
+model = gs.Gaussian(latlon=True, len_scale=777, geo_scale=gs.KM_SCALE)
 srf = gs.SRF(model, seed=12345)
 field = srf.structured((lat, lon))
 # Orthographic plotting with cartopy
 ax = plt.subplot(projection=ccrs.Orthographic(-45, 45))
 cont = ax.contourf(lon, lat, field, transform=ccrs.PlateCarree())
 ax.coastlines()
 ax.set_global()
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gstools Version: 1.4.1 Summary: GSTools: A
+Metadata-Version: 2.1 Name: gstools Version: 1.5.0 Summary: GSTools: A
 geostatistical toolbox. Author-email: "Sebastian MÃ¼ller, Lennart SchÃ¼ler"
 geostat-framework.org> License: LGPL-3.0 Project-URL: Changelog, https://
 github.com/GeoStat-Framework/GSTools/blob/main/CHANGELOG.md Project-URL: Conda-
 Forge, https://anaconda.org/conda-forge/gstools Project-URL: Documentation,
 https://gstools.readthedocs.io Project-URL: Homepage, https://geostat-
 framework.org/#gstools Project-URL: Source, https://github.com/GeoStat-
 Framework/GSTools Project-URL: Tracker, https://github.com/GeoStat-Framework/
@@ -90,16 +90,16 @@
                                 [Random field]
 GSTools also provides support for [geographic coordinates](https://
 en.wikipedia.org/wiki/Geographic_coordinate_system). This works perfectly well
 with [cartopy](https://scitools.org.uk/cartopy/docs/latest/index.html).
 ```python import matplotlib.pyplot as plt import cartopy.crs as ccrs import
 gstools as gs # define a structured field by latitude and longitude lat = lon =
 range(-80, 81) model = gs.Gaussian(latlon=True, len_scale=777,
-rescale=gs.EARTH_RADIUS) srf = gs.SRF(model, seed=12345) field = srf.structured
-((lat, lon)) # Orthographic plotting with cartopy ax = plt.subplot
+geo_scale=gs.KM_SCALE) srf = gs.SRF(model, seed=12345) field = srf.structured(
+(lat, lon)) # Orthographic plotting with cartopy ax = plt.subplot
 (projection=ccrs.Orthographic(-45, 45)) cont = ax.contourf(lon, lat, field,
 transform=ccrs.PlateCarree()) ax.coastlines() ax.set_global() plt.colorbar
 (cont) ```
                             [lat-lon random field]
 A similar example but for a three dimensional field is exported to a [VTK]
 (https://vtk.org/) file, which can be visualized with [ParaView](https://
 www.paraview.org/) or [PyVista](https://docs.pyvista.org) in Python: ```python
```

### Comparing `gstools-1.4.1/README.md` & `gstools-1.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
 ```python
 import matplotlib.pyplot as plt
 import cartopy.crs as ccrs
 import gstools as gs
 # define a structured field by latitude and longitude
 lat = lon = range(-80, 81)
-model = gs.Gaussian(latlon=True, len_scale=777, rescale=gs.EARTH_RADIUS)
+model = gs.Gaussian(latlon=True, len_scale=777, geo_scale=gs.KM_SCALE)
 srf = gs.SRF(model, seed=12345)
 field = srf.structured((lat, lon))
 # Orthographic plotting with cartopy
 ax = plt.subplot(projection=ccrs.Orthographic(-45, 45))
 cont = ax.contourf(lon, lat, field, transform=ccrs.PlateCarree())
 ax.coastlines()
 ax.set_global()
```

#### html2text {}

```diff
@@ -64,16 +64,16 @@
                                 [Random field]
 GSTools also provides support for [geographic coordinates](https://
 en.wikipedia.org/wiki/Geographic_coordinate_system). This works perfectly well
 with [cartopy](https://scitools.org.uk/cartopy/docs/latest/index.html).
 ```python import matplotlib.pyplot as plt import cartopy.crs as ccrs import
 gstools as gs # define a structured field by latitude and longitude lat = lon =
 range(-80, 81) model = gs.Gaussian(latlon=True, len_scale=777,
-rescale=gs.EARTH_RADIUS) srf = gs.SRF(model, seed=12345) field = srf.structured
-((lat, lon)) # Orthographic plotting with cartopy ax = plt.subplot
+geo_scale=gs.KM_SCALE) srf = gs.SRF(model, seed=12345) field = srf.structured(
+(lat, lon)) # Orthographic plotting with cartopy ax = plt.subplot
 (projection=ccrs.Orthographic(-45, 45)) cont = ax.contourf(lon, lat, field,
 transform=ccrs.PlateCarree()) ax.coastlines() ax.set_global() plt.colorbar
 (cont) ```
                             [lat-lon random field]
 A similar example but for a three dimensional field is exported to a [VTK]
 (https://vtk.org/) file, which can be visualized with [ParaView](https://
 www.paraview.org/) or [PyVista](https://docs.pyvista.org) in Python: ```python
```

### Comparing `gstools-1.4.1/pyproject.toml` & `gstools-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -143,17 +143,17 @@
     [tool.pylint.reports]
     output-format = "colorized"
 
     [tool.pylint.design]
     max-args = 20
     max-locals = 50
     max-branches = 30
-    max-statements = 80
+    max-statements = 85
     max-attributes = 25
-    max-public-methods = 75
+    max-public-methods = 80
 
 [tool.cibuildwheel]
 # Switch to using build
 build-frontend = "build"
 # Disable building PyPy wheels on all platforms, 32bit for py3.10/11 and musllinux builds, py3.6
 skip = ["cp36-*", "pp*", "cp31*-win32", "cp31*-manylinux_i686", "*-musllinux_*"]
 # Run the package tests using `pytest`
```

### Comparing `gstools-1.4.1/setup.py` & `gstools-1.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """GSTools: A geostatistical toolbox."""
 import os
 
 import numpy as np
 from Cython.Build import cythonize
 from extension_helpers import add_openmp_flags_if_available
 from setuptools import Extension, setup
```

### Comparing `gstools-1.4.1/src/gstools/__init__.py` & `gstools-1.5.0/src/gstools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Purpose
 =======
 
 GeoStatTools is a library providing geostatistical tools
 for random field generation, conditioned field generation,
 kriging and variogram estimation
@@ -10,15 +9,15 @@
 
 The following functionalities are directly provided on module-level.
 
 Subpackages
 ===========
 
 .. autosummary::
-   :toctree: generated
+   :toctree: api
 
     covmodel
     field
     variogram
     krige
     random
     tools
@@ -122,14 +121,17 @@
 Misc
 ====
 
 .. currentmodule:: gstools.tools
 
 .. autosummary::
    EARTH_RADIUS
+   KM_SCALE
+   DEGREE_SCALE
+   RADIAN_SCALE
 """
 # Hooray!
 from gstools import (
     config,
     covmodel,
     field,
     krige,
@@ -158,15 +160,18 @@
     TPLGaussian,
     TPLSimple,
     TPLStable,
 )
 from gstools.field import SRF, CondSRF
 from gstools.krige import Krige
 from gstools.tools import (
+    DEGREE_SCALE,
     EARTH_RADIUS,
+    KM_SCALE,
+    RADIAN_SCALE,
     generate_grid,
     generate_st_grid,
     rotated_main_axes,
     to_vtk,
     to_vtk_structured,
     to_vtk_unstructured,
     vtk_export,
@@ -185,15 +190,15 @@
     from gstools._version import __version__
 except ModuleNotFoundError:  # pragma: no cover
     # package is not installed
     __version__ = "0.0.0.dev0"
 
 __all__ = ["__version__"]
 __all__ += ["covmodel", "field", "variogram", "krige", "random", "tools"]
-__all__ += ["transform", "normalizer"]
+__all__ += ["transform", "normalizer", "config"]
 __all__ += [
     "CovModel",
     "Gaussian",
     "Exponential",
     "Matern",
     "Integral",
     "Stable",
@@ -223,14 +228,17 @@
     "Krige",
     "SRF",
     "CondSRF",
     "rotated_main_axes",
     "generate_grid",
     "generate_st_grid",
     "EARTH_RADIUS",
+    "KM_SCALE",
+    "DEGREE_SCALE",
+    "RADIAN_SCALE",
     "vtk_export",
     "vtk_export_structured",
     "vtk_export_unstructured",
     "to_vtk",
     "to_vtk_structured",
     "to_vtk_unstructured",
 ]
```

### Comparing `gstools-1.4.1/src/gstools/covmodel/__init__.py` & `gstools-1.5.0/src/gstools/covmodel/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing a set of handy covariance models.
 
 .. currentmodule:: gstools.covmodel
 
 Subpackages
 ^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    plot
 
 Covariance Base-Class
 ^^^^^^^^^^^^^^^^^^^^^
 Class to construct user defined covariance models
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    CovModel
 
 Covariance Models
 ^^^^^^^^^^^^^^^^^
 Standard Covariance Models
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    Gaussian
    Exponential
    Matern
    Integral
    Stable
    Rational
@@ -39,17 +38,18 @@
    Circular
    Spherical
    HyperSpherical
    SuperSpherical
    JBessel
 
 Truncated Power Law Covariance Models
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    TPLGaussian
    TPLExponential
    TPLStable
    TPLSimple
 """
```

### Comparing `gstools-1.4.1/src/gstools/covmodel/base.py` & `gstools-1.5.0/src/gstools/covmodel/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing the base class for covariance models.
 
 .. currentmodule:: gstools.covmodel.base
 
 The following classes are provided
 
@@ -25,39 +24,44 @@
     compare,
     default_arg_from_bounds,
     model_repr,
     percentile_scale,
     set_arg_bounds,
     set_dim,
     set_len_anis,
+    set_model_angles,
     set_opt_args,
     spectral_rad_pdf,
 )
+from gstools.tools import RADIAN_SCALE
 from gstools.tools.geometric import (
+    great_circle_to_chordal,
     latlon2pos,
     matrix_anisometrize,
     matrix_isometrize,
     pos2latlon,
     rotated_main_axes,
-    set_angles,
 )
 
 __all__ = ["CovModel"]
 
 # default arguments for hankel.SymmetricFourierTransform
 HANKEL_DEFAULT = {"a": -1, "b": 1, "N": 200, "h": 0.001, "alt": True}
 
 
 class CovModel:
     r"""Base class for the GSTools covariance models.
 
     Parameters
     ----------
     dim : :class:`int`, optional
-        dimension of the model. Default: ``3``
+        dimension of the model.
+        Includes the temporal dimension if temporal is true.
+        To specify only the spatial dimension in that case, use `spatial_dim`.
+        Default: ``3``
     var : :class:`float`, optional
         variance of the model (the nugget is not included in "this" variance)
         Default: ``1.0``
     len_scale : :class:`float` or :class:`list`, optional
         length scale of the model.
         If a single value is given, the same length-scale will be used for
         every direction. If multiple values (for main and transversal
@@ -97,17 +101,35 @@
         Whether the model is describing 2D fields on earths surface described
         by latitude and longitude. When using this, the model will internally
         use the associated 'Yadrenko' model to represent a valid model.
         This means, the spatial distance :math:`r` will be replaced by
         :math:`2\sin(\alpha/2)`, where :math:`\alpha` is the great-circle
         distance, which is equal to the spatial distance of two points in 3D.
         As a consequence, `dim` will be set to `3` and anisotropy will be
-        disabled. `rescale` can be set to e.g. earth's radius,
+        disabled. `geo_scale` can be set to e.g. earth's radius,
         to have a meaningful `len_scale` parameter.
         Default: False
+    geo_scale : :class:`float`, optional
+        Geographic unit scaling in case of latlon coordinates to get a
+        meaningful length scale unit.
+        By default, len_scale is assumed to be in radians with latlon=True.
+        Can be set to :any:`KM_SCALE` to have len_scale in km or
+        :any:`DEGREE_SCALE` to have len_scale in degrees.
+        Default: :any:`RADIAN_SCALE`
+    temporal : :class:`bool`, optional
+        Create a metric spatio-temporal covariance model.
+        Setting this to true will increase `dim` and `field_dim` by 1.
+        `spatial_dim` will be `field_dim - 1`.
+        The time-dimension is appended, meaning the pos tuple is (x,y,z,...,t).
+        Default: False
+    spatial_dim : :class:`int`, optional
+        spatial dimension of the model.
+        If given, the model dimension will be determined from this spatial dimension
+        and the possible temporal dimension if temporal is ture.
+        Default: None
     var_raw : :class:`float` or :any:`None`, optional
         raw variance of the model which will be multiplied with
         :any:`CovModel.var_factor` to result in the actual variance.
         If given, ``var`` will be ignored.
         (This is just for models that override :any:`CovModel.var_factor`)
         Default: :any:`None`
     hankel_kw: :class:`dict` or :any:`None`, optional
@@ -125,17 +147,21 @@
         self,
         dim=3,
         var=1.0,
         len_scale=1.0,
         nugget=0.0,
         anis=1.0,
         angles=0.0,
+        *,
         integral_scale=None,
         rescale=None,
         latlon=False,
+        geo_scale=RADIAN_SCALE,
+        temporal=False,
+        spatial_dim=None,
         var_raw=None,
         hankel_kw=None,
         **opt_arg,
     ):
         # assert, that we use a subclass
         # this is the case, if __init_subclass__ is called, which creates
         # the "variogram"... so we check for that
@@ -153,39 +179,45 @@
         self._angles = None
         # prepare parameters boundaries
         self._var_bounds = None
         self._len_scale_bounds = None
         self._nugget_bounds = None
         self._anis_bounds = None
         self._opt_arg_bounds = {}
-        # Set latlon first
+        # Set latlon and temporal first
         self._latlon = bool(latlon)
+        self._temporal = bool(temporal)
+        self._geo_scale = abs(float(geo_scale))
         # SFT class will be created within dim.setter but needs hankel_kw
         self.hankel_kw = hankel_kw
-        self.dim = dim
+        # using time increases model dimension given by "spatial_dim"
+        self.dim = (
+            dim if spatial_dim is None else spatial_dim + int(self.temporal)
+        )
 
         # optional arguments for the variogram-model
         set_opt_args(self, opt_arg)
 
         # set standard boundaries for variance, len_scale, nugget and opt_arg
         bounds = self.default_arg_bounds()
         bounds.update(self.default_opt_arg_bounds())
         self.set_arg_bounds(check_args=False, **bounds)
 
         # set parameters
         self.rescale = rescale
         self._nugget = float(nugget)
+
         # set anisotropy and len_scale, disable anisotropy for latlon models
-        self._len_scale, anis = set_len_anis(self.dim, len_scale, anis)
-        if self.latlon:
-            self._anis = np.array((self.dim - 1) * [1], dtype=np.double)
-            self._angles = np.array(self.dim * [0], dtype=np.double)
-        else:
-            self._anis = anis
-            self._angles = set_angles(self.dim, angles)
+        self._len_scale, self._anis = set_len_anis(
+            self.dim, len_scale, anis, self.latlon
+        )
+        self._angles = set_model_angles(
+            self.dim, angles, self.latlon, self.temporal
+        )
+
         # set var at last, because of the var_factor (to be right initialized)
         if var_raw is None:
             self._var = None
             self.var = var
         else:
             self._var = float(var_raw)
         self._integral_scale = None
@@ -239,23 +271,23 @@
         r"""Correlation along axis of anisotropy."""
         if axis == 0:
             return self.correlation(r)
         return self.correlation(np.abs(r) / self.anis[axis - 1])
 
     def vario_yadrenko(self, zeta):
         r"""Yadrenko variogram for great-circle distance from latlon-pos."""
-        return self.variogram(2 * np.sin(zeta / 2))
+        return self.variogram(great_circle_to_chordal(zeta, self.geo_scale))
 
     def cov_yadrenko(self, zeta):
         r"""Yadrenko covariance for great-circle distance from latlon-pos."""
-        return self.covariance(2 * np.sin(zeta / 2))
+        return self.covariance(great_circle_to_chordal(zeta, self.geo_scale))
 
     def cor_yadrenko(self, zeta):
         r"""Yadrenko correlation for great-circle distance from latlon-pos."""
-        return self.correlation(2 * np.sin(zeta / 2))
+        return self.correlation(great_circle_to_chordal(zeta, self.geo_scale))
 
     def vario_spatial(self, pos):
         r"""Spatial variogram respecting anisotropy and rotation."""
         return self.variogram(self._get_iso_rad(pos))
 
     def cov_spatial(self, pos):
         r"""Spatial covariance respecting anisotropy and rotation."""
@@ -527,33 +559,45 @@
 
     # spatial routines
 
     def isometrize(self, pos):
         """Make a position tuple ready for isotropic operations."""
         pos = np.asarray(pos, dtype=np.double).reshape((self.field_dim, -1))
         if self.latlon:
-            return latlon2pos(pos)
+            return latlon2pos(
+                pos,
+                radius=self.geo_scale,
+                temporal=self.temporal,
+                time_scale=self.anis[-1],
+            )
         return np.dot(matrix_isometrize(self.dim, self.angles, self.anis), pos)
 
     def anisometrize(self, pos):
         """Bring a position tuple into the anisotropic coordinate-system."""
         pos = np.asarray(pos, dtype=np.double).reshape((self.dim, -1))
         if self.latlon:
-            return pos2latlon(pos)
+            return pos2latlon(
+                pos,
+                radius=self.geo_scale,
+                temporal=self.temporal,
+                time_scale=self.anis[-1],
+            )
         return np.dot(
             matrix_anisometrize(self.dim, self.angles, self.anis), pos
         )
 
     def main_axes(self):
         """Axes of the rotated coordinate-system."""
         return rotated_main_axes(self.dim, self.angles)
 
     def _get_iso_rad(self, pos):
         """Isometrized radians."""
-        return np.linalg.norm(self.isometrize(pos), axis=0)
+        pos = np.asarray(pos, dtype=np.double).reshape((self.dim, -1))
+        iso = np.dot(matrix_isometrize(self.dim, self.angles, self.anis), pos)
+        return np.linalg.norm(iso, axis=0)
 
     # fitting routine
 
     def fit_variogram(
         self,
         x_data,
         y_data,
@@ -859,25 +903,40 @@
             "len_scale": self.len_scale_bounds,
             "nugget": self.nugget_bounds,
             "anis": self.anis_bounds,
         }
         res.update(self.opt_arg_bounds)
         return res
 
+    @property
+    def temporal(self):
+        """:class:`bool`: Whether the model is a metric spatio-temporal one."""
+        return self._temporal
+
     # geographical coordinates related
 
     @property
     def latlon(self):
         """:class:`bool`: Whether the model depends on geographical coords."""
         return self._latlon
 
     @property
+    def geo_scale(self):
+        """:class:`float`: Geographic scaling for geographical coords."""
+        return self._geo_scale
+
+    @property
     def field_dim(self):
-        """:class:`int`: The field dimension of the model."""
-        return 2 if self.latlon else self.dim
+        """:class:`int`: The (parametric) field dimension of the model (with time)."""
+        return 2 + int(self.temporal) if self.latlon else self.dim
+
+    @property
+    def spatial_dim(self):
+        """:class:`int`: The spatial field dimension of the model (without time)."""
+        return 2 if self.latlon else self.dim - int(self.temporal)
 
     # standard parameters
 
     @property
     def dim(self):
         """:class:`int`: The dimension of the model."""
         return self._dim
@@ -922,15 +981,17 @@
     @property
     def len_scale(self):
         """:class:`float`: The main length scale of the model."""
         return self._len_scale
 
     @len_scale.setter
     def len_scale(self, len_scale):
-        self._len_scale, anis = set_len_anis(self.dim, len_scale, self.anis)
+        self._len_scale, anis = set_len_anis(
+            self.dim, len_scale, self.anis, self.latlon
+        )
         if self.latlon:
             self._anis = np.array((self.dim - 1) * [1], dtype=np.double)
         else:
             self._anis = anis
         self.check_arg_bounds()
 
     @property
@@ -951,33 +1012,29 @@
     @property
     def anis(self):
         """:class:`numpy.ndarray`: The anisotropy factors of the model."""
         return self._anis
 
     @anis.setter
     def anis(self, anis):
-        if self.latlon:
-            self._anis = np.array((self.dim - 1) * [1], dtype=np.double)
-        else:
-            self._len_scale, self._anis = set_len_anis(
-                self.dim, self.len_scale, anis
-            )
+        self._len_scale, self._anis = set_len_anis(
+            self.dim, self.len_scale, anis, self.latlon
+        )
         self.check_arg_bounds()
 
     @property
     def angles(self):
         """:class:`numpy.ndarray`: Rotation angles (in rad) of the model."""
         return self._angles
 
     @angles.setter
     def angles(self, angles):
-        if self.latlon:
-            self._angles = np.array(self.dim * [0], dtype=np.double)
-        else:
-            self._angles = set_angles(self.dim, angles)
+        self._angles = set_model_angles(
+            self.dim, angles, self.latlon, self.temporal
+        )
         self.check_arg_bounds()
 
     @property
     def integral_scale(self):
         """:class:`float`: The main integral scale of the model.
 
         Raises
```

### Comparing `gstools-1.4.1/src/gstools/covmodel/fit.py` & `gstools-1.5.0/src/gstools/covmodel/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing tools for the covariance-model.
 
 .. currentmodule:: gstools.covmodel.fit
 
 The following classes and functions are provided
 
@@ -10,15 +9,15 @@
    fit_variogram
 """
 # pylint: disable=C0103, W0632
 import numpy as np
 from scipy.optimize import curve_fit
 
 from gstools.covmodel.tools import check_arg_in_bounds, default_arg_from_bounds
-from gstools.tools.geometric import set_anis
+from gstools.tools.geometric import great_circle_to_chordal, set_anis
 
 __all__ = ["fit_variogram"]
 
 
 DEFAULT_PARA = ["var", "len_scale", "nugget"]
 
 
@@ -338,15 +337,15 @@
         )
     if is_dir_vario and model.latlon:
         raise ValueError(
             "CovModel.fit_variogram: lat-lon models don't support anisotropy."
         )
     if model.latlon:
         # convert to yadrenko model
-        x_data = 2 * np.sin(x_data / 2)
+        x_data = great_circle_to_chordal(x_data, model.geo_scale)
     return x_data, y_data, is_dir_vario
 
 
 def _set_weights(model, weights, x_data, curve_fit_kwargs, is_dir_vario):
     if weights is not None:
         if callable(weights):
             weights = 1.0 / weights(x_data)
@@ -519,14 +518,15 @@
         sigmoid's midpoint. The default is 0.7.
 
     Returns
     -------
     callable
         Weighting function.
     """
+
     # define the callable weights function
     def func(x_data):
         """Callable function for the weights."""
         x_range = np.amax(x_data) - np.amin(x_data)
         # logit function for growth rate
         growth = np.log(p / (1 - p)) / (p * x_range)
         x_mean = mean * x_range + np.amin(x_data)
```

### Comparing `gstools-1.4.1/src/gstools/covmodel/models.py` & `gstools-1.5.0/src/gstools/covmodel/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing different covariance models.
 
 .. currentmodule:: gstools.covmodel.models
 
 The following classes are provided
```

### Comparing `gstools-1.4.1/src/gstools/covmodel/plot.py` & `gstools-1.5.0/src/gstools/covmodel/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing plotting routines for the covariance models.
 
 .. currentmodule:: gstools.covmodel.plot
 
 The following classes and functions are provided
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    plot_variogram
    plot_covariance
    plot_correlation
    plot_vario_yadrenko
    plot_cov_yadrenko
    plot_cor_yadrenko
@@ -49,59 +48,67 @@
     "plot_spectral_rad_pdf",
 ]
 
 
 # plotting routines #######################################################
 
 
-def _plot_spatial(dim, pos, field, fig, ax, latlon, **kwargs):
+def _plot_spatial(dim, pos, field, fig, ax, temporal, **kwargs):
     from gstools.field.plot import plot_1d, plot_nd
 
     if dim == 1:
-        return plot_1d(pos, field, fig, ax, **kwargs)
-    return plot_nd(pos, field, "structured", fig, ax, latlon, **kwargs)
+        return plot_1d(pos, field, fig, ax, temporal, **kwargs)
+    return plot_nd(
+        pos, field, "structured", fig, ax, temporal=temporal, **kwargs
+    )
 
 
 def plot_vario_spatial(
     model, x_min=0.0, x_max=None, fig=None, ax=None, **kwargs
 ):  # pragma: no cover
     """Plot spatial variogram of a given CovModel."""
     if x_max is None:
         x_max = 3 * model.len_scale
     x_s = np.linspace(-x_max, x_max) + x_min
     pos = [x_s] * model.dim
     shp = tuple(len(p) for p in pos)
     fld = model.vario_spatial(generate_grid(pos)).reshape(shp)
-    return _plot_spatial(model.dim, pos, fld, fig, ax, model.latlon, **kwargs)
+    return _plot_spatial(
+        model.dim, pos, fld, fig, ax, model.temporal, **kwargs
+    )
 
 
 def plot_cov_spatial(
     model, x_min=0.0, x_max=None, fig=None, ax=None, **kwargs
 ):  # pragma: no cover
     """Plot spatial covariance of a given CovModel."""
     if x_max is None:
         x_max = 3 * model.len_scale
     x_s = np.linspace(-x_max, x_max) + x_min
     pos = [x_s] * model.dim
     shp = tuple(len(p) for p in pos)
     fld = model.cov_spatial(generate_grid(pos)).reshape(shp)
-    return _plot_spatial(model.dim, pos, fld, fig, ax, model.latlon, **kwargs)
+    return _plot_spatial(
+        model.dim, pos, fld, fig, ax, model.temporal, **kwargs
+    )
 
 
 def plot_cor_spatial(
     model, x_min=0.0, x_max=None, fig=None, ax=None, **kwargs
 ):  # pragma: no cover
     """Plot spatial correlation of a given CovModel."""
     if x_max is None:
         x_max = 3 * model.len_scale
     x_s = np.linspace(-x_max, x_max) + x_min
     pos = [x_s] * model.dim
     shp = tuple(len(p) for p in pos)
     fld = model.cor_spatial(generate_grid(pos)).reshape(shp)
-    return _plot_spatial(model.dim, pos, fld, fig, ax, model.latlon, **kwargs)
+    return _plot_spatial(
+        model.dim, pos, fld, fig, ax, model.temporal, **kwargs
+    )
 
 
 def plot_variogram(
     model, x_min=0.0, x_max=None, fig=None, ax=None, **kwargs
 ):  # pragma: no cover
     """Plot variogram of a given CovModel."""
     fig, ax = get_fig_ax(fig, ax)
@@ -147,45 +154,45 @@
 
 def plot_vario_yadrenko(
     model, x_min=0.0, x_max=None, fig=None, ax=None, **kwargs
 ):  # pragma: no cover
     """Plot Yadrenko variogram of a given CovModel."""
     fig, ax = get_fig_ax(fig, ax)
     if x_max is None:
-        x_max = min(3 * model.len_rescaled, np.pi)
+        x_max = min(3 * model.len_scale, model.geo_scale * np.pi)
     x_s = np.linspace(x_min, x_max)
     kwargs.setdefault("label", f"{model.name} Yadrenko variogram")
     ax.plot(x_s, model.vario_yadrenko(x_s), **kwargs)
     ax.legend()
     fig.show()
     return ax
 
 
 def plot_cov_yadrenko(
     model, x_min=0.0, x_max=None, fig=None, ax=None, **kwargs
 ):  # pragma: no cover
     """Plot Yadrenko covariance of a given CovModel."""
     fig, ax = get_fig_ax(fig, ax)
     if x_max is None:
-        x_max = min(3 * model.len_rescaled, np.pi)
+        x_max = min(3 * model.len_scale, model.geo_scale * np.pi)
     x_s = np.linspace(x_min, x_max)
     kwargs.setdefault("label", f"{model.name} Yadrenko covariance")
     ax.plot(x_s, model.cov_yadrenko(x_s), **kwargs)
     ax.legend()
     fig.show()
     return ax
 
 
 def plot_cor_yadrenko(
     model, x_min=0.0, x_max=None, fig=None, ax=None, **kwargs
 ):  # pragma: no cover
     """Plot Yadrenko correlation function of a given CovModel."""
     fig, ax = get_fig_ax(fig, ax)
     if x_max is None:
-        x_max = min(3 * model.len_rescaled, np.pi)
+        x_max = min(3 * model.len_scale, model.geo_scale * np.pi)
     x_s = np.linspace(x_min, x_max)
     kwargs.setdefault("label", f"{model.name} Yadrenko correlation")
     ax.plot(x_s, model.cor_yadrenko(x_s), **kwargs)
     ax.legend()
     fig.show()
     return ax
```

### Comparing `gstools-1.4.1/src/gstools/covmodel/tools.py` & `gstools-1.5.0/src/gstools/covmodel/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing tools for the covariance-model.
 
 .. currentmodule:: gstools.covmodel.tools
 
 The following classes and functions are provided
 
@@ -27,22 +26,23 @@
 import warnings
 
 import numpy as np
 from hankel import SymmetricFourierTransform as SFT
 from scipy import special as sps
 from scipy.optimize import root
 
-from gstools.tools.geometric import set_angles, set_anis
+from gstools.tools.geometric import no_of_angles, set_angles, set_anis
 from gstools.tools.misc import list_format
 
 __all__ = [
     "AttributeWarning",
     "rad_fac",
     "set_opt_args",
     "set_len_anis",
+    "set_model_angles",
     "check_bounds",
     "check_arg_in_bounds",
     "default_arg_from_bounds",
     "spectral_rad_pdf",
     "percentile_scale",
     "set_arg_bounds",
     "check_arg_bounds",
@@ -180,25 +180,29 @@
                 "since it is already present in "
                 "the class. It could not be added to the model."
             )
         # Magic happens here
         setattr(model, opt_name, float(opt_arg[opt_name]))
 
 
-def set_len_anis(dim, len_scale, anis):
+def set_len_anis(dim, len_scale, anis, latlon=False):
     """Set the length scale and anisotropy factors for the given dimension.
 
     Parameters
     ----------
     dim : :class:`int`
         spatial dimension
     len_scale : :class:`float` or :class:`list`
         the length scale of the SRF in x direction or in x- (y-, ...) direction
     anis : :class:`float` or :class:`list`
         the anisotropy of length scales along the transversal axes
+    latlon : :class:`bool`, optional
+        Whether the model is describing 2D fields on earths surface described
+        by latitude and longitude. In this case there is no spatial anisotropy.
+        Default: False
 
     Returns
     -------
     len_scale : :class:`float`
         the main length scale of the SRF in x direction
     anis : :class:`list`, optional
         the anisotropy of length scales along the transversal axes
@@ -230,19 +234,57 @@
         out_anis = np.zeros(dim - 1, dtype=np.double)
         for i in range(1, dim):
             out_anis[i - 1] = ls_tmp[i] / ls_tmp[0]
     # sanity check
     for ani in out_anis:
         if not ani > 0.0:
             raise ValueError(
-                "anisotropy-ratios needs to be > 0, " + "got: " + str(out_anis)
+                f"anisotropy-ratios needs to be > 0, got: {out_anis}"
             )
+    # no spatial anisotropy for latlon
+    if latlon:
+        out_anis[:2] = 1.0
     return out_len_scale, out_anis
 
 
+def set_model_angles(dim, angles, latlon=False, temporal=False):
+    """Set the model angles for the given dimension.
+
+    Parameters
+    ----------
+    dim : :class:`int`
+        spatial dimension
+    angles : :class:`float` or :class:`list`
+        the angles of the SRF
+    latlon : :class:`bool`, optional
+        Whether the model is describing 2D fields on earths surface described
+        by latitude and longitude.
+        Default: False
+    temporal : :class:`bool`, optional
+        Whether a time-dimension is appended.
+        Default: False
+
+    Returns
+    -------
+    angles : :class:`float`
+        the angles fitting to the dimension
+
+    Notes
+    -----
+        If too few angles are given, they are filled up with `0`.
+    """
+    if latlon:
+        return np.array(no_of_angles(dim) * [0], dtype=np.double)
+    out_angles = set_angles(dim, angles)
+    if temporal:
+        # no rotation between spatial dimensions and temporal dimension
+        out_angles[no_of_angles(dim - 1) :] = 0.0
+    return out_angles
+
+
 def check_bounds(bounds):
     """
     Check if given bounds are valid.
 
     Parameters
     ----------
     bounds : list
@@ -375,17 +417,15 @@
     -------
     float
         Percentile scale.
 
     """
     # check the given percentile
     if not 0.0 < per < 1.0:
-        raise ValueError(
-            "percentile needs to be within (0, 1), got: " + str(per)
-        )
+        raise ValueError(f"percentile needs to be within (0, 1), got: {per}")
 
     # define a curve, that has its root at the wanted point
     def curve(x):
         return 1.0 - model.correlation(x) - per
 
     # take 'per * len_rescaled' as initial guess
     return root(curve, per * model.len_rescaled)["x"][0]
@@ -491,25 +531,25 @@
     ------
     ValueError
         When dimension is < 1.
     """
     # check if a fixed dimension should be used
     if model.fix_dim() is not None and model.fix_dim() != dim:
         warnings.warn(
-            model.name + ": using fixed dimension " + str(model.fix_dim()),
+            f"{model.name}: using fixed dimension {model.fix_dim()}",
             AttributeWarning,
         )
         dim = model.fix_dim()
-        if model.latlon and dim != 3:
+        if model.latlon and dim != (3 + int(model.temporal)):
             raise ValueError(
                 f"{model.name}: using fixed dimension {model.fix_dim()}, "
-                "which is not compatible with a latlon model."
+                f"which is not compatible with a latlon model (with temporal={model.temporal})."
             )
-    # force dim=3 for latlon models
-    dim = 3 if model.latlon else dim
+    # force dim=3 (or 4 when temporal=True) for latlon models
+    dim = (3 + int(model.temporal)) if model.latlon else dim
     # set the dimension
     if dim < 1:
         raise ValueError("Only dimensions of d >= 1 are supported.")
     if not model.check_dim(dim):
         warnings.warn(
             f"Dimension {dim} is not appropriate for this model.",
             AttributeWarning,
@@ -519,15 +559,17 @@
     model._sft = SFT(ndim=model.dim, **model.hankel_kw)
     # recalculate dimension related parameters
     if model._anis is not None:
         model._len_scale, model._anis = set_len_anis(
             model.dim, model._len_scale, model._anis
         )
     if model._angles is not None:
-        model._angles = set_angles(model.dim, model._angles)
+        model._angles = set_model_angles(
+            model.dim, model._angles, model.latlon, model.temporal
+        )
     model.check_arg_bounds()
 
 
 def compare(this, that):
     """
     Compare CovModels.
 
@@ -548,14 +590,15 @@
     equal &= np.isclose(this.var_raw, that.var_raw)  # ?! needless?
     equal &= np.isclose(this.nugget, that.nugget)
     equal &= np.isclose(this.len_scale, that.len_scale)
     equal &= np.all(np.isclose(this.anis, that.anis))
     equal &= np.all(np.isclose(this.angles, that.angles))
     equal &= np.isclose(this.rescale, that.rescale)
     equal &= this.latlon == that.latlon
+    equal &= this.temporal == that.temporal
     for opt in this.opt_arg:
         equal &= np.isclose(getattr(this, opt), getattr(that, opt))
     return equal
 
 
 def model_repr(model):  # pragma: no cover
     """
@@ -565,26 +608,40 @@
     ----------
     model : :any:`CovModel`
         The covariance model in use.
     """
     m = model
     p = model._prec
     opt_str = ""
+    t_str = ", temporal=True" if m.temporal else ""
     if not np.isclose(m.rescale, m.default_rescale()):
         opt_str += f", rescale={m.rescale:.{p}}"
     for opt in m.opt_arg:
         opt_str += f", {opt}={getattr(m, opt):.{p}}"
-    # only print anis and angles if model is anisotropic or rotated
-    ani_str = "" if m.is_isotropic else f", anis={list_format(m.anis, p)}"
-    ang_str = f", angles={list_format(m.angles, p)}" if m.do_rotation else ""
     if m.latlon:
+        ani_str = (
+            ""
+            if m.is_isotropic or not m.temporal
+            else f", anis={m.anis[-1]:.{p}}"
+        )
+        r_str = (
+            ""
+            if np.isclose(m.geo_scale, 1)
+            else f", geo_scale={m.geo_scale:.{p}}"
+        )
         repr_str = (
-            f"{m.name}(latlon={m.latlon}, var={m.var:.{p}}, "
-            f"len_scale={m.len_scale:.{p}}, nugget={m.nugget:.{p}}{opt_str})"
+            f"{m.name}(latlon={m.latlon}{t_str}, var={m.var:.{p}}, "
+            f"len_scale={m.len_scale:.{p}}, nugget={m.nugget:.{p}}"
+            f"{ani_str}{r_str}{opt_str})"
         )
     else:
+        # only print anis and angles if model is anisotropic or rotated
+        ani_str = "" if m.is_isotropic else f", anis={list_format(m.anis, p)}"
+        ang_str = (
+            f", angles={list_format(m.angles, p)}" if m.do_rotation else ""
+        )
         repr_str = (
-            f"{m.name}(dim={m.dim}, var={m.var:.{p}}, "
+            f"{m.name}(dim={m.spatial_dim}{t_str}, var={m.var:.{p}}, "
             f"len_scale={m.len_scale:.{p}}, nugget={m.nugget:.{p}}"
             f"{ani_str}{ang_str}{opt_str})"
         )
     return repr_str
```

### Comparing `gstools-1.4.1/src/gstools/covmodel/tpl_models.py` & `gstools-1.5.0/src/gstools/covmodel/tpl_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing truncated power law covariance models.
 
 .. currentmodule:: gstools.covmodel.tpl_models
 
 The following classes and functions are provided
```

### Comparing `gstools-1.4.1/src/gstools/field/__init__.py` & `gstools-1.5.0/src/gstools/field/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing tools for spatial random fields.
 
 .. currentmodule:: gstools.field
 
 Subpackages
 ^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
     generator
     upscaling
 
 Spatial Random Field
 ^^^^^^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    SRF
    CondSRF
 
 Field Base Class
 ^^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    Field
 """
 
 from gstools.field.base import Field
 from gstools.field.cond_srf import CondSRF
 from gstools.field.srf import SRF
```

### Comparing `gstools-1.4.1/src/gstools/field/base.py` & `gstools-1.5.0/src/gstools/field/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing a base class for spatial fields.
 
 .. currentmodule:: gstools.field.base
 
 The following classes are provided
 
@@ -676,14 +675,19 @@
 
     @property
     def latlon(self):
         """:class:`bool`: Whether the field depends on geographical coords."""
         return False if self.model is None else self.model.latlon
 
     @property
+    def temporal(self):
+        """:class:`bool`: Whether the field depends on time."""
+        return False if self.model is None else self.model.temporal
+
+    @property
     def name(self):
         """:class:`str`: The name of the class."""
         return self.__class__.__name__
 
     def _fmt_mean_norm_trend(self):
         # fmt_mean_norm_trend for all child classes
         return fmt_mean_norm_trend(self)
```

### Comparing `gstools-1.4.1/src/gstools/field/cond_srf.py` & `gstools-1.5.0/src/gstools/field/cond_srf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing a class for conditioned spatial random fields.
 
 .. currentmodule:: gstools.field.cond_srf
 
 The following classes are provided
```

### Comparing `gstools-1.4.1/src/gstools/field/generator.py` & `gstools-1.5.0/src/gstools/field/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing generators for spatial random fields.
 
 .. currentmodule:: gstools.field.generator
 
 The following classes are provided
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    Generator
    RandMeth
    IncomprRandMeth
 """
 # pylint: disable=C0103, W0222, C0412, W0231
 import warnings
@@ -121,17 +120,14 @@
     model : :any:`CovModel`
         Covariance model
     mode_no : :class:`int`, optional
         Number of Fourier modes. Default: ``1000``
     seed : :class:`int` or :any:`None`, optional
         The seed of the random number generator.
         If "None", a random seed is used. Default: :any:`None`
-    verbose : :class:`bool`, optional
-        Be chatty during the generation.
-        Default: :any:`False`
     sampling : :class:`str`, optional
         Sampling strategy. Either
 
             * "auto": select best strategy depending on given model
             * "inversion": use inversion method
             * "mcmc": use mcmc sampling
 
@@ -166,25 +162,24 @@
            A comparison of several numerical methods",
            Environmental Modelling & Software, 55, 32-48., (2014)
     """
 
     def __init__(
         self,
         model,
+        *,
         mode_no=1000,
         seed=None,
-        verbose=False,
         sampling="auto",
         **kwargs,
     ):
         if kwargs:
             warnings.warn("gstools.RandMeth: **kwargs are ignored")
         # initialize attributes
         self._mode_no = int(mode_no)
-        self._verbose = bool(verbose)
         # initialize private attributes
         self._model = None
         self._seed = None
         self._rng = None
         self._z_1 = None
         self._z_2 = None
         self._cov_sample = None
@@ -271,23 +266,20 @@
                 self.seed = seed
             else:
                 raise ValueError(
                     "gstools.field.generator.RandMeth: no 'model' given"
                 )
         # if the user tries to trick us, we beat him!
         elif model is None and np.isnan(seed):
-            if (
+            if not (
                 isinstance(self._model, CovModel)
                 and self._z_1 is not None
                 and self._z_2 is not None
                 and self._cov_sample is not None
             ):
-                if self.verbose:
-                    print("RandMeth.update: Nothing will be done...")
-            else:
                 raise ValueError(
                     "gstools.field.generator.RandMeth: "
                     "neither 'model' nor 'seed' given!"
                 )
         # wrong model type
         else:
             raise ValueError(
@@ -379,23 +371,14 @@
     @mode_no.setter
     def mode_no(self, mode_no):
         if int(mode_no) != self._mode_no:
             self._mode_no = int(mode_no)
             self.reset_seed(self._seed)
 
     @property
-    def verbose(self):
-        """:class:`bool`: Verbosity of the generator."""
-        return self._verbose
-
-    @verbose.setter
-    def verbose(self, verbose):
-        self._verbose = bool(verbose)
-
-    @property
     def value_type(self):
         """:class:`str`: Type of the field values (scalar, vector)."""
         return self._value_type
 
     def __repr__(self):
         """Return String representation."""
         return (
@@ -414,17 +397,14 @@
     mean_velocity : :class:`float`, optional
         the mean velocity in x-direction
     mode_no : :class:`int`, optional
         number of Fourier modes. Default: ``1000``
     seed : :class:`int` or :any:`None`, optional
         the seed of the random number generator.
         If "None", a random seed is used. Default: :any:`None`
-    verbose : :class:`bool`, optional
-        State if there should be output during the generation.
-        Default: :any:`False`
     sampling : :class:`str`, optional
         Sampling strategy. Either
 
             * "auto": select best strategy depending on given model
             * "inversion": use inversion method
             * "mcmc": use mcmc sampling
 
@@ -461,26 +441,32 @@
            "Diffusion by a random velocity field.",
            The physics of fluids, 13(1), 22-31., (1970)
     """
 
     def __init__(
         self,
         model,
+        *,
         mean_velocity=1.0,
         mode_no=1000,
         seed=None,
-        verbose=False,
         sampling="auto",
         **kwargs,
     ):
         if model.dim < 2 or model.dim > 3:
             raise ValueError(
                 "Only 2D and 3D incompressible fields can be generated."
             )
-        super().__init__(model, mode_no, seed, verbose, sampling, **kwargs)
+        super().__init__(
+            model=model,
+            mode_no=mode_no,
+            seed=seed,
+            sampling=sampling,
+            **kwargs,
+        )
 
         self.mean_u = mean_velocity
         self._value_type = "vector"
 
     def __call__(self, pos, add_nugget=True):
         """Calculate the random modes for the randomization method.
```

### Comparing `gstools-1.4.1/src/gstools/field/plot.py` & `gstools-1.5.0/src/gstools/field/plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing plotting routines for spatial fields.
 
 .. currentmodule:: gstools.field.plot
 
 The following classes and functions are provided
 
@@ -49,31 +48,45 @@
     ax : :class:`Axes` or :any:`None`, optional
         Axes to plot on. If `None`, a new one will be added to the figure.
         Default: `None`
     **kwargs
         Forwarded to the plotting routine.
     """
     if fld.dim == 1:
-        return plot_1d(fld.pos, fld[field], fig, ax, **kwargs)
+        return plot_1d(fld.pos, fld[field], fig, ax, fld.temporal, **kwargs)
     return plot_nd(
-        fld.pos, fld[field], fld.mesh_type, fig, ax, fld.latlon, **kwargs
+        fld.pos,
+        fld[field],
+        fld.mesh_type,
+        fig,
+        ax,
+        fld.latlon,
+        fld.temporal,
+        **kwargs,
     )
 
 
-def plot_1d(pos, field, fig=None, ax=None, ax_names=None):  # pragma: no cover
+def plot_1d(
+    pos, field, fig=None, ax=None, temporal=False, ax_names=None
+):  # pragma: no cover
     """
     Plot a 1D field.
 
     Parameters
     ----------
     pos : :class:`list`
         the position tuple, containing either the point coordinates (x, y, ...)
         or the axes descriptions (for mesh_type='structured')
     field : :class:`numpy.ndarray`
         Field values.
+    temporal : :class:`bool`, optional
+        Indicate a metric spatio-temporal covariance model.
+        The time-dimension is assumed to be appended,
+        meaning the pos tuple is (x,y,z,...,t) or (lat, lon, t).
+        Default: False
     fig : :class:`Figure` or :any:`None`, optional
         Figure to plot the axes on. If `None`, a new one will be created.
         Default: `None`
     ax : :class:`Axes` or :any:`None`, optional
         Axes to plot on. If `None`, a new one will be added to the figure.
         Default: `None`
     ax_names : :class:`list` of :class:`str`, optional
@@ -85,15 +98,15 @@
         Axis containing the plot.
     """
     fig, ax = get_fig_ax(fig, ax)
     title = f"Field 1D: {field.shape}"
     x = pos[0]
     x = x.flatten()
     arg = np.argsort(x)
-    ax_names = _ax_names(1, ax_names=ax_names)
+    ax_names = _ax_names(1, temporal=temporal, ax_names=ax_names)
     ax.plot(x[arg], field.ravel()[arg])
     ax.set_xlabel(ax_names[0])
     ax.set_ylabel(ax_names[1])
     ax.set_title(title)
     fig.show()
     return ax
 
@@ -101,14 +114,15 @@
 def plot_nd(
     pos,
     field,
     mesh_type,
     fig=None,
     ax=None,
     latlon=False,
+    temporal=False,
     resolution=128,
     ax_names=None,
     aspect="quad",
     show_colorbar=True,
     convex_hull=False,
     contour_plot=True,
     **kwargs,
@@ -133,14 +147,19 @@
         Whether the data is representing 2D fields on earths surface described
         by latitude and longitude. When using this, the estimator will
         use great-circle distance for variogram estimation.
         Note, that only an isotropic variogram can be estimated and a
         ValueError will be raised, if a direction was specified.
         Bin edges need to be given in radians in this case.
         Default: False
+    temporal : :class:`bool`, optional
+        Indicate a metric spatio-temporal covariance model.
+        The time-dimension is assumed to be appended,
+        meaning the pos tuple is (x,y,z,...,t) or (lat, lon, t).
+        Default: False
     resolution : :class:`int`, optional
         Resolution of the imshow plot. The default is 128.
     ax_names : :class:`list` of :class:`str`, optional
         Axes names. The default is ["$x$", "field"].
     aspect : :class:`str` or :any:`None` or :class:`float`, optional
         Aspect of the plot. Can be "auto", "equal", "quad", None or a number
         describing the aspect ratio.
@@ -156,22 +175,36 @@
     Returns
     -------
     ax : :class:`Axes`
         Axis containing the plot.
     """
     dim = len(pos)
     assert dim > 1
-    assert not latlon or dim == 2
+    assert not latlon or dim == 2 + int(bool(temporal))
     if dim == 2 and contour_plot:
         return _plot_2d(
-            pos, field, mesh_type, fig, ax, latlon, ax_names, **kwargs
+            pos,
+            field,
+            mesh_type,
+            fig,
+            ax,
+            latlon,
+            temporal,
+            ax_names,
+            **kwargs,
         )
-    pos = pos[::-1] if latlon else pos
-    field = field.T if (latlon and mesh_type != "unstructured") else field
-    ax_names = _ax_names(dim, latlon, ax_names)
+    if latlon:
+        # swap lat-lon to lon-lat (x-y)
+        if temporal:
+            pos = (pos[1], pos[0], pos[2])
+        else:
+            pos = (pos[1], pos[0])
+        if mesh_type != "unstructured":
+            field = np.moveaxis(field, [0, 1], [1, 0])
+    ax_names = _ax_names(dim, latlon, temporal, ax_names)
     # init planes
     planes = rotation_planes(dim)
     plane_names = [f" {ax_names[p[0]]} - {ax_names[p[1]]}" for p in planes]
     ax_ends = [[p.min(), p.max()] for p in pos]
     ax_rngs = [end[1] - end[0] for end in ax_ends]
     ax_steps = [rng / resolution for rng in ax_rngs]
     ax_extents = [ax_ends[p[0]] + ax_ends[p[1]] for p in planes]
@@ -320,40 +353,46 @@
     ax.set_ylabel("Y")
     ax.set_title(title)
     fig.colorbar(sp.lines)
     fig.show()
     return ax
 
 
-def _ax_names(dim, latlon=False, ax_names=None):
+def _ax_names(dim, latlon=False, temporal=False, ax_names=None):
+    t_fac = int(bool(temporal))
     if ax_names is not None:
         assert len(ax_names) >= dim
         return ax_names[:dim]
-    if dim == 2 and latlon:
-        return ["lon", "lat"]
-    if dim <= 3:
-        return ["$x$", "$y$", "$z$"][:dim] + (dim == 1) * ["field"]
-    return [f"$x_{{{i}}}$" for i in range(dim)]
+    if dim == 2 + t_fac and latlon:
+        return ["lon", "lat"] + t_fac * ["time"]
+    if dim - t_fac <= 3:
+        return (
+            ["$x$", "$y$", "$z$"][: dim - t_fac]
+            + t_fac * ["time"]
+            + (dim == 1) * ["field"]
+        )
+    return [f"$x_{{{i}}}$" for i in range(dim - t_fac)] + t_fac * ["time"]
 
 
 def _plot_2d(
     pos,
     field,
     mesh_type,
     fig=None,
     ax=None,
     latlon=False,
+    temporal=False,
     ax_names=None,
     levels=64,
     antialias=True,
 ):  # pragma: no cover
     """Plot a 2d field with a contour plot."""
     fig, ax = get_fig_ax(fig, ax)
     title = f"Field 2D {mesh_type}: {field.shape}"
-    ax_names = _ax_names(2, latlon, ax_names=ax_names)
+    ax_names = _ax_names(2, latlon, temporal, ax_names=ax_names)
     x, y = pos[::-1] if latlon else pos
     if mesh_type == "unstructured":
         cont = ax.tricontourf(x, y, field.ravel(), levels=levels)
         if antialias:
             ax.tricontour(x, y, field.ravel(), levels=levels, zorder=-10)
     else:
         plt_fld = field if latlon else field.T
```

### Comparing `gstools-1.4.1/src/gstools/field/srf.py` & `gstools-1.5.0/src/gstools/field/srf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing a class for standard spatial random fields.
 
 .. currentmodule:: gstools.field.srf
 
 The following classes are provided
```

### Comparing `gstools-1.4.1/src/gstools/field/summator.pyx` & `gstools-1.5.0/src/gstools/field/summator.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
-# -*- coding: utf-8 -*-
 """
 This is the randomization method summator, implemented in cython.
 """
 
 import numpy as np
 
 cimport cython
```

### Comparing `gstools-1.4.1/src/gstools/field/tools.py` & `gstools-1.5.0/src/gstools/field/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing tools for Fields.
 
 .. currentmodule:: gstools.field.tools
 
 The following classes and functions are provided
```

### Comparing `gstools-1.4.1/src/gstools/field/upscaling.py` & `gstools-1.5.0/src/gstools/field/upscaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing upscaling routines for the spatial random field.
 
 .. currentmodule:: gstools.field.upscaling
 
 The following functions are provided
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    var_coarse_graining
    var_no_scaling
 """
 # pylint: disable=W0613
 import warnings
```

### Comparing `gstools-1.4.1/src/gstools/krige/base.py` & `gstools-1.5.0/src/gstools/krige/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing a base class for kriging.
 
 .. currentmodule:: gstools.krige.base
 
 The following classes are provided
 
@@ -110,16 +109,20 @@
         you can pass a callable which takes a matrix and returns the inverse.
         Default: `"pinv"`
     fit_normalizer : :class:`bool`, optional
         Whether to fit the data-normalizer to the given conditioning data.
         Default: False
     fit_variogram : :class:`bool`, optional
         Whether to fit the given variogram model to the data.
-        This is done by using isotropy settings of the given model,
-        assuming the sill to be the data variance and with the
+        Directional variogram fitting is triggered by setting
+        any anisotropy factor of the model to anything unequal 1
+        but the main axes of correlation are taken from the model
+        rotation angles. If the model is a spatio-temporal latlon
+        model, this will raise an error.
+        This assumes the sill to be the data variance and with
         standard bins provided by the :any:`standard_bins` routine.
         Default: False
 
     Notes
     -----
     If you have changed any properties in the class, you can update the kriging
     setup by calling :any:`Krige.set_condition` without any arguments.
@@ -493,16 +496,20 @@
             The "exact=True" variant only works with "cond_err='nugget'".
             Default: "nugget"
         fit_normalizer : :class:`bool`, optional
             Whether to fit the data-normalizer to the given conditioning data.
             Default: False
         fit_variogram : :class:`bool`, optional
             Whether to fit the given variogram model to the data.
-            This is done by using isotropy settings of the given model,
-            assuming the sill to be the data variance and with the
+            Directional variogram fitting is triggered by setting
+            any anisotropy factor of the model to anything unequal 1
+            but the main axes of correlation are taken from the model
+            rotation angles. If the model is a spatio-temporal latlon
+            model, this will raise an error.
+            This assumes the sill to be the data variance and with
             standard bins provided by the :any:`standard_bins` routine.
             Default: False
         """
         # only use existing external drift, if no new positions are given
         ext_drift = (
             self._cond_ext_drift
             if (ext_drift is None and cond_pos is None)
@@ -519,20 +526,26 @@
         self._cond_pos, self._cond_val = set_condition(
             cond_pos, cond_val, self.dim
         )
         if fit_normalizer:  # fit normalizer to detrended data
             self.normalizer.fit(self.cond_val - self.cond_trend)
         if fit_variogram:  # fitting model to empirical variogram of data
             # normalize field
+            if self.model.latlon and self.model.temporal:
+                msg = "Krige: can't fit variogram for spatio-temporal latlon data."
+                raise ValueError(msg)
             field = self.normalizer.normalize(self.cond_val - self.cond_trend)
             field -= self.cond_mean
             sill = np.var(field)
             if self.model.is_isotropic:
                 emp_vario = vario_estimate(
-                    self.cond_pos, field, latlon=self.model.latlon
+                    self.cond_pos,
+                    field,
+                    latlon=self.model.latlon,
+                    geo_scale=self.model.geo_scale,
                 )
             else:
                 axes = rotated_main_axes(self.model.dim, self.model.angles)
                 emp_vario = vario_estimate(
                     self.cond_pos, field, direction=axes
                 )
             # set the sill to the field variance
```

### Comparing `gstools-1.4.1/src/gstools/krige/krigesum.pyx` & `gstools-1.5.0/src/gstools/krige/krigesum.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
-# -*- coding: utf-8 -*-
 """
 This is a summator for the kriging routines
 """
 
 import numpy as np
 
 cimport cython
```

### Comparing `gstools-1.4.1/src/gstools/krige/methods.py` & `gstools-1.5.0/src/gstools/krige/methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing a class for simple kriging.
 
 .. currentmodule:: gstools.krige.methods
 
 The following classes are provided
 
@@ -74,16 +73,20 @@
         you can pass a callable which takes a matrix and returns the inverse.
         Default: `"pinv"`
     fit_normalizer : :class:`bool`, optional
         Whether to fit the data-normalizer to the given conditioning data.
         Default: False
     fit_variogram : :class:`bool`, optional
         Whether to fit the given variogram model to the data.
-        This is done by using isotropy settings of the given model,
-        assuming the sill to be the data variance and with the
+        Directional variogram fitting is triggered by setting
+        any anisotropy factor of the model to anything unequal 1
+        but the main axes of correlation are taken from the model
+        rotation angles. If the model is a spatio-temporal latlon
+        model, this will raise an error.
+        This assumes the sill to be the data variance and with
         standard bins provided by the :any:`standard_bins` routine.
         Default: False
     """
 
     def __init__(
         self,
         model,
@@ -168,16 +171,20 @@
         you can pass a callable which takes a matrix and returns the inverse.
         Default: `"pinv"`
     fit_normalizer : :class:`bool`, optional
         Whether to fit the data-normalizer to the given conditioning data.
         Default: False
     fit_variogram : :class:`bool`, optional
         Whether to fit the given variogram model to the data.
-        This is done by using isotropy settings of the given model,
-        assuming the sill to be the data variance and with the
+        Directional variogram fitting is triggered by setting
+        any anisotropy factor of the model to anything unequal 1
+        but the main axes of correlation are taken from the model
+        rotation angles. If the model is a spatio-temporal latlon
+        model, this will raise an error.
+        This assumes the sill to be the data variance and with
         standard bins provided by the :any:`standard_bins` routine.
         Default: False
     """
 
     def __init__(
         self,
         model,
@@ -272,16 +279,20 @@
         you can pass a callable which takes a matrix and returns the inverse.
         Default: `"pinv"`
     fit_normalizer : :class:`bool`, optional
         Whether to fit the data-normalizer to the given conditioning data.
         Default: False
     fit_variogram : :class:`bool`, optional
         Whether to fit the given variogram model to the data.
-        This is done by using isotropy settings of the given model,
-        assuming the sill to be the data variance and with the
+        Directional variogram fitting is triggered by setting
+        any anisotropy factor of the model to anything unequal 1
+        but the main axes of correlation are taken from the model
+        rotation angles. If the model is a spatio-temporal latlon
+        model, this will raise an error.
+        This assumes the sill to be the data variance and with
         standard bins provided by the :any:`standard_bins` routine.
         Default: False
     """
 
     def __init__(
         self,
         model,
@@ -373,16 +384,20 @@
         you can pass a callable which takes a matrix and returns the inverse.
         Default: `"pinv"`
     fit_normalizer : :class:`bool`, optional
         Whether to fit the data-normalizer to the given conditioning data.
         Default: False
     fit_variogram : :class:`bool`, optional
         Whether to fit the given variogram model to the data.
-        This is done by using isotropy settings of the given model,
-        assuming the sill to be the data variance and with the
+        Directional variogram fitting is triggered by setting
+        any anisotropy factor of the model to anything unequal 1
+        but the main axes of correlation are taken from the model
+        rotation angles. If the model is a spatio-temporal latlon
+        model, this will raise an error.
+        This assumes the sill to be the data variance and with
         standard bins provided by the :any:`standard_bins` routine.
         Default: False
     """
 
     def __init__(
         self,
         model,
@@ -464,16 +479,20 @@
             * `"pinvh"`: use `pinvh` from `scipy` which uses eigen-values
 
         If you want to use another routine to invert the kriging matrix,
         you can pass a callable which takes a matrix and returns the inverse.
         Default: `"pinv"`
     fit_variogram : :class:`bool`, optional
         Whether to fit the given variogram model to the data.
-        This is done by using isotropy settings of the given model,
-        assuming the sill to be the data variance and with the
+        Directional variogram fitting is triggered by setting
+        any anisotropy factor of the model to anything unequal 1
+        but the main axes of correlation are taken from the model
+        rotation angles. If the model is a spatio-temporal latlon
+        model, this will raise an error.
+        This assumes the sill to be the data variance and with
         standard bins provided by the :any:`standard_bins` routine.
         Default: False
     """
 
     def __init__(
         self,
         model,
```

### Comparing `gstools-1.4.1/src/gstools/krige/tools.py` & `gstools-1.5.0/src/gstools/krige/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing tools for Kriging.
 
 .. currentmodule:: gstools.krige.tools
 
 The following classes and functions are provided
```

### Comparing `gstools-1.4.1/src/gstools/normalizer/__init__.py` & `gstools-1.5.0/src/gstools/normalizer/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing normalization routines.
 
 .. currentmodule:: gstools.normalizer
 
 Base-Normalizer
 ^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    Normalizer
 
 Field-Normalizer
 ^^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    LogNormal
    BoxCox
    BoxCoxShift
    YeoJohnson
    Modulus
    Manly
 
 Convenience Routines
 ^^^^^^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    apply_mean_norm_trend
    remove_trend_norm_mean
 """
 
 from gstools.normalizer.base import Normalizer
 from gstools.normalizer.methods import (
```

### Comparing `gstools-1.4.1/src/gstools/normalizer/base.py` & `gstools-1.5.0/src/gstools/normalizer/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing the base class for normalizers.
 
 .. currentmodule:: gstools.normalizer.base
 
 The following classes are provided
```

### Comparing `gstools-1.4.1/src/gstools/normalizer/methods.py` & `gstools-1.5.0/src/gstools/normalizer/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing different normalizer transformations.
 
 .. currentmodule:: gstools.normalizer.methods
 
 The following classes are provided
```

### Comparing `gstools-1.4.1/src/gstools/normalizer/tools.py` & `gstools-1.5.0/src/gstools/normalizer/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing tools for Normalizers.
 
 .. currentmodule:: gstools.normalizer.tools
 
 The following classes and functions are provided
```

### Comparing `gstools-1.4.1/src/gstools/random/rng.py` & `gstools-1.5.0/src/gstools/random/rng.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing the core of the spatial random field generation.
 
 .. currentmodule:: gstools.random.rng
 
 The following classes are provided
```

### Comparing `gstools-1.4.1/src/gstools/random/tools.py` & `gstools-1.5.0/src/gstools/random/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing tools for random sampling.
 
 .. currentmodule:: gstools.random.tools
 
 The following classes are provided
```

### Comparing `gstools-1.4.1/src/gstools/tools/__init__.py` & `gstools-1.5.0/src/gstools/tools/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing miscellaneous tools.
 
 .. currentmodule:: gstools.tools
 
 Export
 ^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    vtk_export
    vtk_export_structured
    vtk_export_unstructured
    to_vtk
    to_vtk_structured
    to_vtk_unstructured
 
 Special functions
 ^^^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    confidence_scaling
    inc_gamma
    inc_gamma_low
    exp_int
    inc_beta
    tplstable_cor
    tpl_exp_spec_dens
    tpl_gau_spec_dens
 
 Geometric
 ^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    rotated_main_axes
    set_angles
    set_anis
    no_of_angles
    rotation_planes
    givens_rotation
@@ -55,18 +54,27 @@
    generate_st_grid
 
 Misc
 ^^^^
 
 .. autosummary::
    EARTH_RADIUS
+   KM_SCALE
+   DEGREE_SCALE
+   RADIAN_SCALE
 
 ----
 
 .. autodata:: EARTH_RADIUS
+
+.. autodata:: KM_SCALE
+
+.. autodata:: DEGREE_SCALE
+
+.. autodata:: RADIAN_SCALE
 """
 
 from gstools.tools.export import (
     to_vtk,
     to_vtk_structured,
     to_vtk_unstructured,
     vtk_export,
@@ -100,14 +108,23 @@
     tpl_gau_spec_dens,
     tplstable_cor,
 )
 
 EARTH_RADIUS = 6371.0
 """float: earth radius for WGS84 ellipsoid in km"""
 
+KM_SCALE = 6371.0
+"""float: earth radius for WGS84 ellipsoid in km"""
+
+DEGREE_SCALE = 57.29577951308232
+"""float: radius for unit sphere in degree"""
+
+RADIAN_SCALE = 1.0
+"""float: radius for unit sphere"""
+
 
 __all__ = [
     "vtk_export",
     "vtk_export_structured",
     "vtk_export_unstructured",
     "to_vtk",
     "to_vtk_structured",
@@ -132,8 +149,11 @@
     "matrix_isometrize",
     "matrix_anisometrize",
     "rotated_main_axes",
     "ang2dir",
     "generate_grid",
     "generate_st_grid",
     "EARTH_RADIUS",
+    "KM_SCALE",
+    "DEGREE_SCALE",
+    "RADIAN_SCALE",
 ]
```

### Comparing `gstools-1.4.1/src/gstools/tools/export.py` & `gstools-1.5.0/src/gstools/tools/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing export routines.
 
 .. currentmodule:: gstools.tools.export
 
 The following functions are provided
```

### Comparing `gstools-1.4.1/src/gstools/tools/geometric.py` & `gstools-1.5.0/src/gstools/tools/geometric.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing geometric tools.
 
 .. currentmodule:: gstools.tools.geometric
 
 The following functions are provided
 
@@ -24,14 +23,15 @@
    format_struct_pos_dim
    format_struct_pos_shape
    format_unstruct_pos_shape
    ang2dir
    latlon2pos
    pos2latlon
    chordal_to_great_circle
+   great_circle_to_chordal
 """
 # pylint: disable=C0103
 import numpy as np
 
 __all__ = [
     "set_angles",
     "set_anis",
@@ -621,83 +621,133 @@
         vec[:, i] = np.prod(np.sin(angles[:, i:]), axis=1)  # empty prod = 1
         vec[:, i] *= np.cos(angles[:, (i - 1)])
     if dim in [2, 3]:
         vec[:, [0, 1]] = vec[:, [1, 0]]  # to match convention in 2D and 3D
     return vec
 
 
-def latlon2pos(latlon, radius=1.0, dtype=np.double):
+def latlon2pos(
+    latlon, radius=1.0, dtype=np.double, temporal=False, time_scale=1.0
+):
     """Convert lat-lon geo coordinates to 3D position tuple.
 
     Parameters
     ----------
     latlon : :class:`list` of :class:`numpy.ndarray`
         latitude and longitude given in degrees.
+        May includes an appended time axis if `time=True`.
     radius : :class:`float`, optional
-        Earth radius. Default: `1.0`
+        Sphere radius. Default: `1.0`
     dtype : data-type, optional
         The desired data-type for the array.
         If not given, then the type will be determined as the minimum type
         required to hold the objects in the sequence. Default: None
+    temporal : :class:`bool`, optional
+        Whether latlon includes an appended time axis.
+        Default: False
+    time_scale : :class:`float`, optional
+        Scaling factor (e.g. anisotropy) for the time axis.
+        Default: `1.0`
 
     Returns
     -------
     :class:`numpy.ndarray`
         the 3D position array
     """
-    latlon = np.asarray(latlon, dtype=dtype).reshape((2, -1))
-    lat, lon = np.deg2rad(latlon)
-    return np.array(
-        (
-            radius * np.cos(lat) * np.cos(lon),
-            radius * np.cos(lat) * np.sin(lon),
-            radius * np.sin(lat) * np.ones_like(lon),
-        ),
-        dtype=dtype,
+    latlon = np.asarray(latlon, dtype=dtype).reshape(
+        (3 if temporal else 2, -1)
     )
+    lat, lon = np.deg2rad(latlon[:2])
+    pos_tuple = (
+        radius * np.cos(lat) * np.cos(lon),
+        radius * np.cos(lat) * np.sin(lon),
+        radius * np.sin(lat) * np.ones_like(lon),
+    )
+    if temporal:
+        return np.array(pos_tuple + (latlon[2] / time_scale,), dtype=dtype)
+    return np.array(pos_tuple, dtype=dtype)
 
 
-def pos2latlon(pos, radius=1.0, dtype=np.double):
+def pos2latlon(
+    pos, radius=1.0, dtype=np.double, temporal=False, time_scale=1.0
+):
     """Convert 3D position tuple from sphere to lat-lon geo coordinates.
 
     Parameters
     ----------
     pos : :class:`list` of :class:`numpy.ndarray`
         The position tuple containing points on a unit-sphere.
+        May includes an appended time axis if `time=True`.
     radius : :class:`float`, optional
-        Earth radius. Default: `1.0`
+        Sphere radius. Default: `1.0`
     dtype : data-type, optional
         The desired data-type for the array.
         If not given, then the type will be determined as the minimum type
         required to hold the objects in the sequence. Default: None
+    temporal : :class:`bool`, optional
+        Whether latlon includes an appended time axis.
+        Default: False
+    time_scale : :class:`float`, optional
+        Scaling factor (e.g. anisotropy) for the time axis.
+        Default: `1.0`
 
     Returns
     -------
     :class:`numpy.ndarray`
         the 3D position array
     """
-    pos = np.asarray(pos, dtype=dtype).reshape((3, -1))
+    pos = np.asarray(pos, dtype=dtype).reshape((4 if temporal else 3, -1))
     # prevent numerical errors in arcsin
     lat = np.arcsin(np.maximum(np.minimum(pos[2] / radius, 1.0), -1.0))
     lon = np.arctan2(pos[1], pos[0])
-    return np.rad2deg((lat, lon), dtype=dtype)
+    latlon = np.rad2deg((lat, lon), dtype=dtype)
+    if temporal:
+        return np.array(
+            (latlon[0], latlon[1], pos[3] * time_scale), dtype=dtype
+        )
+    return latlon
 
 
-def chordal_to_great_circle(dist):
+def chordal_to_great_circle(dist, radius=1.0):
     """
     Calculate great circle distance corresponding to given chordal distance.
 
     Parameters
     ----------
     dist : array_like
-        Chordal distance of two points on the unit-sphere.
+        Chordal distance of two points on the sphere.
+    radius : :class:`float`, optional
+        Sphere radius. Default: `1.0`
 
     Returns
     -------
     :class:`numpy.ndarray`
         Great circle distance corresponding to given chordal distance.
 
     Notes
     -----
-    If given values are not in [0, 1], they will be truncated.
+    If given values are not in [0, 2 * radius], they will be truncated.
+    """
+    diameter = 2 * radius
+    return diameter * np.arcsin(
+        np.maximum(np.minimum(np.divide(dist, diameter), 1), 0)
+    )
+
+
+def great_circle_to_chordal(dist, radius=1.0):
+    """
+    Calculate chordal distance corresponding to given great circle distance.
+
+    Parameters
+    ----------
+    dist : array_like
+        Great circle distance of two points on the sphere.
+    radius : :class:`float`, optional
+        Sphere radius. Default: `1.0`
+
+    Returns
+    -------
+    :class:`numpy.ndarray`
+        Chordal distance corresponding to given great circle distance.
     """
-    return 2 * np.arcsin(np.maximum(np.minimum(np.divide(dist, 2), 1), 0))
+    diameter = 2 * radius
+    return diameter * np.sin(np.divide(dist, diameter))
```

### Comparing `gstools-1.4.1/src/gstools/tools/misc.py` & `gstools-1.5.0/src/gstools/tools/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing miscellaneous tools.
 
 .. currentmodule:: gstools.tools.misc
 
 The following functions are provided
```

### Comparing `gstools-1.4.1/src/gstools/tools/special.py` & `gstools-1.5.0/src/gstools/tools/special.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing special functions.
 
 .. currentmodule:: gstools.tools.special
 
 The following functions are provided
```

### Comparing `gstools-1.4.1/src/gstools/transform/__init__.py` & `gstools-1.5.0/src/gstools/transform/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing transformations to post-process normal fields.
 
 .. currentmodule:: gstools.transform
 
 Wrapper
 ^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    apply
 
 Field Transformations
 ^^^^^^^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    binary
    discrete
    boxcox
    zinnharvey
    normal_force_moments
    normal_to_lognormal
@@ -29,15 +28,15 @@
    normal_to_uquad
    apply_function
 
 Array Transformations
 ^^^^^^^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    array_discrete
    array_boxcox
    array_zinnharvey
    array_force_moments
    array_to_lognormal
    array_to_uniform
```

### Comparing `gstools-1.4.1/src/gstools/transform/array.py` & `gstools-1.5.0/src/gstools/transform/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing array transformations.
 
 .. currentmodule:: gstools.transform.array
 
 The following functions are provided
 
@@ -212,39 +211,47 @@
     -------
     :class:`numpy.ndarray`
         Transformed field.
     """
     return np.exp(field)
 
 
-def array_to_uniform(field, mean=None, var=None):
+def array_to_uniform(field, mean=None, var=None, low=0.0, high=1.0):
     """
-    Transform normal distribution to uniform distribution on [0, 1].
+    Transform normal distribution to uniform distribution on [low, high].
 
     Parameters
     ----------
     field : :class:`numpy.ndarray`
         Normal distributed values.
     mean : :class:`float` or :any:`None`, optional
         Mean of the given field. If None is given, the mean will be calculated.
         Default: :any:`None`
     var : :class:`float` or :any:`None`, optional
         Variance of the given field.
         If None is given, the variance will be calculated.
         Default: :any:`None`
+    low : :class:`float`, optional
+        Lower bound for the uniform distribution.
+        Default: 0.0
+    high : :class:`float`, optional
+        Upper bound for the uniform distribution.
+        Default: 1.0
 
     Returns
     -------
     :class:`numpy.ndarray`
         Transformed field.
     """
     field = np.asarray(field)
     mean = np.mean(field) if mean is None else float(mean)
     var = np.var(field) if var is None else float(var)
-    return 0.5 * (1 + erf((field - mean) / np.sqrt(2 * var)))
+    return (
+        0.5 * (1 + erf((field - mean) / np.sqrt(2 * var))) * (high - low) + low
+    )
 
 
 def array_to_arcsin(field, mean=None, var=None, a=None, b=None):
     """
     Transform normal distribution to arcsin distribution.
 
     See: https://en.wikipedia.org/wiki/Arcsine_distribution
```

### Comparing `gstools-1.4.1/src/gstools/transform/field.py` & `gstools-1.5.0/src/gstools/transform/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing field transformations.
 
 .. currentmodule:: gstools.transform.field
 
 The following functions are provided
 
@@ -23,15 +22,15 @@
    zinnharvey
    normal_force_moments
    normal_to_lognormal
    normal_to_uniform
    normal_to_arcsin
    normal_to_uquad
 """
-# pylint: disable=C0103, C0123, R0911
+# pylint: disable=C0103, C0123, R0911, R1735
 import numpy as np
 
 from gstools.normalizer import (
     Normalizer,
     apply_mean_norm_trend,
     remove_trend_norm_mean,
 )
@@ -545,36 +544,55 @@
         process=process,
         keep_mean=keep_mean,
     )
 
 
 def normal_to_uniform(
     fld,
+    low=0.0,
+    high=1.0,
     field="field",
     store=True,
     process=False,
     keep_mean=True,
 ):
     """
     Transform normal distribution to uniform distribution on [0, 1].
 
     After this transformation, the field is uniformly distributed on [0, 1].
 
     Parameters
     ----------
     fld : :any:`Field`
         Field class containing a generated field.
+    low : :class:`float`, optional
+        Lower bound for the uniform distribution.
+        Default: 0.0
+    high : :class:`float`, optional
+        Upper bound for the uniform distribution.
+        Default: 1.0
+    field : :class:`str`, optional
+        Name of field to be transformed. The default is "field".
+    store : :class:`str` or :class:`bool`, optional
+        Whether to store field inplace (True/False) or under a given name.
+        The default is True.
+    process : :class:`bool`, optional
+        Whether to process in/out fields with trend, normalizer and mean
+        of given Field instance. The default is False.
     keep_mean : :class:`bool`, optional
         Whether to keep the mean of the field if process=True.
         The default is True.
     """
     if not process:
         _check_for_default_normal(fld)
     kw = dict(
-        mean=0.0 if process and not keep_mean else fld.mean, var=fld.model.sill
+        mean=0.0 if process and not keep_mean else fld.mean,
+        var=fld.model.sill,
+        low=low,
+        high=high,
     )
     return apply_function(
         fld=fld,
         function=array_to_uniform,
         field=field,
         store=store,
         process=process,
```

### Comparing `gstools-1.4.1/src/gstools/variogram/__init__.py` & `gstools-1.5.0/src/gstools/variogram/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing tools for estimating and fitting variograms.
 
 .. currentmodule:: gstools.variogram
 
 Variogram estimation
 ^^^^^^^^^^^^^^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    vario_estimate
    vario_estimate_axis
 
 Binning
 ^^^^^^^
 
 .. autosummary::
-   :toctree: generated
+   :toctree:
 
    standard_bins
 
 ----
 """
 
 from gstools.variogram.binning import standard_bins
```

### Comparing `gstools-1.4.1/src/gstools/variogram/binning.py` & `gstools-1.5.0/src/gstools/variogram/binning.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing binning routines.
 
 .. currentmodule:: gstools.variogram.binning
 
 The following functions are provided
 
 .. autosummary::
    standard_bins
 """
 import numpy as np
 
+from gstools.tools import RADIAN_SCALE
 from gstools.tools.geometric import (
     chordal_to_great_circle,
     format_struct_pos_dim,
     generate_grid,
     latlon2pos,
 )
 
@@ -28,14 +28,15 @@
 def standard_bins(
     pos=None,
     dim=2,
     latlon=False,
     mesh_type="unstructured",
     bin_no=None,
     max_dist=None,
+    geo_scale=RADIAN_SCALE,
 ):
     r"""
     Get standard binning.
 
     Parameters
     ----------
     pos : :class:`list`, optional
@@ -59,14 +60,21 @@
         number of bins to create. If None is given, will be determined by
         Sturges' rule from the number of points.
         Default: None
     max_dist: :class:`float`, optional
         Cut of length for the bins. If None is given, it will be set to one
         third of the box-diameter from the given points.
         Default: None
+    geo_scale : :class:`float`, optional
+        Geographic unit scaling in case of latlon coordinates to get a
+        meaningful bins unit.
+        By default, bins are assumed to be in radians with latlon=True.
+        Can be set to :any:`KM_SCALE` to have bins in km or
+        :any:`DEGREE_SCALE` to have bins in degrees.
+        Default: :any:`RADIAN_SCALE`
 
     Returns
     -------
     :class:`numpy.ndarray`
         The generated bin edges.
 
     Notes
@@ -77,19 +85,19 @@
     if bin_no is None or max_dist is None:
         if pos is None:
             raise ValueError("standard_bins: no pos tuple given.")
         if mesh_type != "unstructured":
             pos = generate_grid(format_struct_pos_dim(pos, dim)[0])
         else:
             pos = np.asarray(pos, dtype=np.double).reshape(dim, -1)
-        pos = latlon2pos(pos) if latlon else pos
+        pos = latlon2pos(pos, radius=geo_scale) if latlon else pos
         pnt_cnt = len(pos[0])
         box = []
         for axis in pos:
             box.append([np.min(axis), np.max(axis)])
         box = np.asarray(box)
         diam = np.linalg.norm(box[:, 0] - box[:, 1])
         # convert diameter to great-circle distance if using latlon
-        diam = chordal_to_great_circle(diam) if latlon else diam
+        diam = chordal_to_great_circle(diam, geo_scale) if latlon else diam
         bin_no = _sturges(pnt_cnt) if bin_no is None else int(bin_no)
         max_dist = diam / 3 if max_dist is None else float(max_dist)
     return np.linspace(0, max_dist, num=bin_no + 1, dtype=np.double)
```

### Comparing `gstools-1.4.1/src/gstools/variogram/estimator.pyx` & `gstools-1.5.0/src/gstools/variogram/estimator.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #cython: language_level=3, boundscheck=False, wraparound=False, cdivision=True
 # distutils: language = c++
-# -*- coding: utf-8 -*-
 """
 This is the variogram estimater, implemented in cython.
 """
 
 import numpy as np
 
 cimport cython
@@ -184,16 +183,15 @@
     const double[:,:] direction,  # should be normed
     const double angles_tol=M_PI/8.0,
     const double bandwidth=-1.0,  # negative values to turn of bandwidth search
     const bint separate_dirs=False,  # whether the direction bands don't overlap
     str estimator_type='m',
 ):
     if pos.shape[1] != f.shape[1]:
-        raise ValueError('len(pos) = {0} != len(f) = {1} '.
-                         format(pos.shape[1], f.shape[1]))
+        raise ValueError(f'len(pos) = {pos.shape[1]} != len(f) = {f.shape[1])}')
 
     if bin_edges.shape[0] < 2:
         raise ValueError('len(bin_edges) too small')
 
     if angles_tol <= 0:
         raise ValueError('tolerance for angle search masks must be > 0')
 
@@ -247,19 +245,18 @@
     cdef _dist_func distance
 
     if distance_type == 'e':
         distance = dist_euclid
     else:
         distance = dist_haversine
         if dim != 2:
-            raise ValueError('Haversine: dim = {0} != 2'.format(dim))
+            raise ValueError(f'Haversine: dim = {dim} != 2')
 
     if pos.shape[1] != f.shape[1]:
-        raise ValueError('len(pos) = {0} != len(f) = {1} '.
-                         format(pos.shape[1], f.shape[1]))
+        raise ValueError(f'len(pos) = {pos.shape[1]} != len(f) = {f.shape[1])}')
 
     if bin_edges.shape[0] < 2:
         raise ValueError('len(bin_edges) too small')
 
     cdef _estimator_func estimator_func = choose_estimator_func(estimator_type)
     cdef _normalization_func normalization_func = (
         choose_estimator_normalization(estimator_type)
```

### Comparing `gstools-1.4.1/src/gstools/variogram/variogram.py` & `gstools-1.5.0/src/gstools/variogram/variogram.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 GStools subpackage providing tools for estimating and fitting variograms.
 
 .. currentmodule:: gstools.variogram.variogram
 
 The following functions are provided
 
@@ -11,14 +10,15 @@
    vario_estimate_axis
 """
 # pylint: disable=C0412
 import numpy as np
 
 from gstools import config
 from gstools.normalizer.tools import remove_trend_norm_mean
+from gstools.tools import RADIAN_SCALE
 from gstools.tools.geometric import (
     ang2dir,
     format_struct_pos_shape,
     format_unstruct_pos_shape,
     generate_grid,
 )
 from gstools.variogram.binning import standard_bins
@@ -89,14 +89,16 @@
     mask=np.ma.nomask,
     mesh_type="unstructured",
     return_counts=False,
     mean=None,
     normalizer=None,
     trend=None,
     fit_normalizer=False,
+    geo_scale=RADIAN_SCALE,
+    **std_bins,
 ):
     r"""
     Estimates the empirical variogram.
 
     The algorithm calculates following equation:
 
     .. math::
@@ -219,18 +221,28 @@
     trend : :any:`None` or :class:`float` or :any:`callable`, optional
         A callable trend function. Should have the signature: f(x, [y, z, ...])
         If no normalizer is applied, this behaves equal to 'mean'.
         The default is None.
     fit_normalizer : :class:`bool`, optional
         Whether to fit the data-normalizer to the given (detrended) field.
         Default: False
+    geo_scale : :class:`float`, optional
+        Geographic unit scaling in case of latlon coordinates to get a
+        meaningful bins unit.
+        By default, bins are assumed to be in radians with latlon=True.
+        Can be set to :any:`KM_SCALE` to have bins in km or
+        :any:`DEGREE_SCALE` to have bins in degrees.
+        Default: :any:`RADIAN_SCALE`
+    **std_bins
+        Optional arguments that are forwarded to the :any:`standard_bins` routine
+        if no bins are given (bin_no, max_dist).
 
     Returns
     -------
-    bin_center : (n), :class:`numpy.ndarray`
+    bin_centers : (n), :class:`numpy.ndarray`
         The bin centers.
     gamma : (n) or (d, n), :class:`numpy.ndarray`
         The estimated variogram values at bin centers.
         Is stacked if multiple `directions` (d>1) are given.
     counts : (n) or (d, n), :class:`numpy.ndarray`, optional
         The number of point pairs found for each bin.
         Is stacked if multiple `directions` (d>1) are given.
@@ -247,26 +259,26 @@
     ----------
     .. [Webster2007] Webster, R. and Oliver, M. A.
            "Geostatistics for environmental scientists.",
            John Wiley & Sons. (2007)
     """
     if bin_edges is not None:
         bin_edges = np.array(bin_edges, ndmin=1, dtype=np.double, copy=False)
-        bin_centres = (bin_edges[:-1] + bin_edges[1:]) / 2.0
+        bin_centers = (bin_edges[:-1] + bin_edges[1:]) / 2.0
     # allow multiple fields at same positions (ndmin=2: first axis -> field ID)
     # need to convert to ma.array, since list of ma.array is not recognised
     field = np.ma.array(field, ndmin=2, dtype=np.double, copy=True)
     masked = np.ma.is_masked(field) or np.any(mask)
     # catch special case if everything is masked
     if masked and np.all(mask):
-        bin_centres = np.empty(0) if bin_edges is None else bin_centres
-        estimates = np.zeros_like(bin_centres)
+        bin_centers = np.empty(0) if bin_edges is None else bin_centers
+        estimates = np.zeros_like(bin_centers)
         if return_counts:
-            return bin_centres, estimates, np.zeros_like(estimates, dtype=int)
-        return bin_centres, estimates
+            return bin_centers, estimates, np.zeros_like(estimates, dtype=int)
+        return bin_centers, estimates
     if not masked:
         field = field.filled()
     # check mesh shape
     if mesh_type != "unstructured":
         pos, __, dim = format_struct_pos_shape(
             pos, field.shape, check_stacked_shape=True
         )
@@ -328,18 +340,23 @@
     # prepare sampled variogram
     if sampling_size is not None and sampling_size < pnt_cnt:
         sampled_idx = np.random.RandomState(sampling_seed).choice(
             np.arange(pnt_cnt), sampling_size, replace=False
         )
         field = field[:, sampled_idx]
         pos = pos[:, sampled_idx]
-    # create bining if not given
+    # create bins
     if bin_edges is None:
-        bin_edges = standard_bins(pos, dim, latlon)
-        bin_centres = (bin_edges[:-1] + bin_edges[1:]) / 2.0
+        bin_edges = standard_bins(
+            pos, dim, latlon, geo_scale=geo_scale, **std_bins
+        )
+        bin_centers = (bin_edges[:-1] + bin_edges[1:]) / 2.0
+    if latlon:
+        # internally we always use radians
+        bin_edges /= geo_scale
     # normalize field
     norm_field_out = remove_trend_norm_mean(
         *(pos, field, mean, normalizer, trend),
         check_shape=False,
         stacked=True,
         fit_normalizer=fit_normalizer,
     )
@@ -368,15 +385,15 @@
             bandwidth,
             separate_dirs=_separate_dirs_test(direction, angles_tol),
             estimator_type=cython_estimator,
         )
         if dir_no == 1:
             estimates, counts = estimates[0], counts[0]
     est_out = (estimates, counts)
-    return (bin_centres,) + est_out[: 2 if return_counts else 1] + norm_out
+    return (bin_centers,) + est_out[: 2 if return_counts else 1] + norm_out
 
 
 def vario_estimate_axis(
     field, direction="x", estimator="matheron", no_data=np.nan
 ):
     r"""Estimates the variogram along array axis.
```

### Comparing `gstools-1.4.1/src/gstools.egg-info/SOURCES.txt` & `gstools-1.5.0/src/gstools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,11 @@
 tests/test_incomprrandmeth.py
 tests/test_krige.py
 tests/test_latlon.py
 tests/test_normalizer.py
 tests/test_randmeth.py
 tests/test_rng.py
 tests/test_srf.py
+tests/test_temporal.py
 tests/test_transform.py
 tests/test_variogram_structured.py
 tests/test_variogram_unstructured.py
```

### Comparing `gstools-1.4.1/tests/test_condition.py` & `gstools-1.5.0/tests/test_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """This is the unittest of CondSRF class."""
 import unittest
 from copy import copy
 
 import numpy as np
 
 import gstools as gs
```

### Comparing `gstools-1.4.1/tests/test_covmodel.py` & `gstools-1.5.0/tests/test_covmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest of CovModel class.
 """
 import unittest
 
 import numpy as np
```

### Comparing `gstools-1.4.1/tests/test_export.py` & `gstools-1.5.0/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `gstools-1.4.1/tests/test_field.py` & `gstools-1.5.0/tests/test_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 This is the unittest of SRF class.
 """
 
 import unittest
 
 import numpy as np
```

### Comparing `gstools-1.4.1/tests/test_incomprrandmeth.py` & `gstools-1.5.0/tests/test_incomprrandmeth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest of the RandMeth class.
 """
 
 import copy
 import unittest
```

### Comparing `gstools-1.4.1/tests/test_krige.py` & `gstools-1.5.0/tests/test_krige.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest of the kriging module.
 """
 
 import unittest
 
 import numpy as np
@@ -129,15 +128,14 @@
                     )
                     for i, val in enumerate(self.cond_val):
                         self.assertAlmostEqual(
                             field_2[self.data_idx[:dim]][i], val, places=2
                         )
 
     def test_detrended(self):
-
         for Model in self.cov_models:
             for dim in self.dims:
                 model = Model(
                     dim=dim,
                     var=2,
                     len_scale=10,
                     anis=[0.5, 0.2],
```

### Comparing `gstools-1.4.1/tests/test_latlon.py` & `gstools-1.5.0/tests/test_latlon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest for latlon related routines.
 """
 
 import unittest
 
 import numpy as np
@@ -21,15 +20,15 @@
     def fix_dim(self):
         return 2
 
 
 class TestLatLon(unittest.TestCase):
     def setUp(self):
         self.cmod = gs.Gaussian(
-            latlon=True, var=2, len_scale=777, rescale=gs.EARTH_RADIUS
+            latlon=True, var=2, len_scale=777, geo_scale=gs.KM_SCALE
         )
         self.lat = self.lon = range(-80, 81)
 
         self.data = np.array(
             [
                 [52.9336, 8.237, 15.7],
                 [48.6159, 13.0506, 13.9],
@@ -63,15 +62,18 @@
         self.assertAlmostEqual(
             8, self.cmod.anisometrize(self.cmod.isometrize((8, 6)))[0, 0]
         )
         self.assertAlmostEqual(
             6, self.cmod.anisometrize(self.cmod.isometrize((8, 6)))[1, 0]
         )
         self.assertAlmostEqual(
-            1, self.cmod.isometrize(self.cmod.anisometrize((1, 0, 0)))[0, 0]
+            gs.EARTH_RADIUS,
+            self.cmod.isometrize(
+                self.cmod.anisometrize((gs.EARTH_RADIUS, 0, 0))
+            )[0, 0],
         )
 
     def test_cov_model(self):
         self.assertAlmostEqual(
             self.cmod.vario_yadrenko(1.234),
             self.cmod.sill - self.cmod.cov_yadrenko(1.234),
         )
@@ -88,38 +90,39 @@
         self.assertAlmostEqual(self.cmod.angles[1], 0)
         self.assertAlmostEqual(self.cmod.angles[2], 0)
 
     def test_vario_est(self):
         srf = gs.SRF(self.cmod, seed=12345)
         field = srf.structured((self.lat, self.lon))
 
-        bin_edges = [0.01 * i for i in range(30)]
+        bin_edges = np.linspace(0, 3 * 777, 30)
         bin_center, emp_vario = gs.vario_estimate(
             *((self.lat, self.lon), field, bin_edges),
             latlon=True,
             mesh_type="structured",
             sampling_size=2000,
             sampling_seed=12345,
+            geo_scale=gs.KM_SCALE,
         )
-        mod = gs.Gaussian(latlon=True, rescale=gs.EARTH_RADIUS)
+        mod = gs.Gaussian(latlon=True, geo_scale=gs.KM_SCALE)
         mod.fit_variogram(bin_center, emp_vario, nugget=False)
         # allow 10 percent relative error
         self.assertLess(_rel_err(mod.var, self.cmod.var), 0.1)
         self.assertLess(_rel_err(mod.len_scale, self.cmod.len_scale), 0.1)
 
     def test_krige(self):
         bin_max = np.deg2rad(8)
         bin_edges = np.linspace(0, bin_max, 5)
         emp_vario = gs.vario_estimate(
             (self.data[:, 0], self.data[:, 1]),
             self.data[:, 2],
             bin_edges,
             latlon=True,
         )
-        mod = gs.Spherical(latlon=True, rescale=gs.EARTH_RADIUS)
+        mod = gs.Spherical(latlon=True, geo_scale=gs.KM_SCALE)
         mod.fit_variogram(*emp_vario, nugget=False)
         kri = gs.krige.Ordinary(
             mod,
             (self.data[:, 0], self.data[:, 1]),
             self.data[:, 2],
         )
         field, var = kri((self.data[:, 0], self.data[:, 1]))
@@ -131,25 +134,25 @@
         bin_edges = np.linspace(0, bin_max, 5)
         emp_vario = gs.vario_estimate(
             (self.data[:, 0], self.data[:, 1]),
             self.data[:, 2],
             bin_edges,
             latlon=True,
         )
-        mod = gs.Spherical(latlon=True, rescale=gs.EARTH_RADIUS)
+        mod = gs.Spherical(latlon=True, geo_scale=gs.KM_SCALE)
         mod.fit_variogram(*emp_vario, nugget=False)
         krige = gs.krige.Ordinary(
             mod, (self.data[:, 0], self.data[:, 1]), self.data[:, 2]
         )
         crf = gs.CondSRF(krige)
         field = crf((self.data[:, 0], self.data[:, 1]))
         for i, dat in enumerate(self.data[:, 2]):
             self.assertAlmostEqual(field[i], dat, 3)
 
-    def error_test(self):
+    def test_error(self):
         # try fitting directional variogram
         mod = gs.Gaussian(latlon=True)
         with self.assertRaises(ValueError):
             mod.fit_variogram([0, 1], [[0, 1], [0, 1], [0, 1]])
         # try to use fixed dim=2 with latlon
         with self.assertRaises(ValueError):
             ErrMod(latlon=True)
```

### Comparing `gstools-1.4.1/tests/test_normalizer.py` & `gstools-1.5.0/tests/test_normalizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest of the Normalizer class.
 """
 
 import unittest
 
 import numpy as np
```

### Comparing `gstools-1.4.1/tests/test_randmeth.py` & `gstools-1.5.0/tests/test_randmeth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest of the RandMeth class.
 """
 
 import copy
 import unittest
 
@@ -23,17 +22,17 @@
         self.x_grid = np.linspace(0.0, 10.0, 9)
         self.y_grid = np.linspace(-5.0, 5.0, 16)
         self.z_grid = np.linspace(-6.0, 7.0, 8)
         self.x_tuple = np.linspace(0.0, 10.0, 10)
         self.y_tuple = np.linspace(-5.0, 5.0, 10)
         self.z_tuple = np.linspace(-6.0, 8.0, 10)
 
-        self.rm_1d = RandMeth(self.cov_model_1d, 100, self.seed)
-        self.rm_2d = RandMeth(self.cov_model_2d, 100, self.seed)
-        self.rm_3d = RandMeth(self.cov_model_3d, 100, self.seed)
+        self.rm_1d = RandMeth(self.cov_model_1d, mode_no=100, seed=self.seed)
+        self.rm_2d = RandMeth(self.cov_model_2d, mode_no=100, seed=self.seed)
+        self.rm_3d = RandMeth(self.cov_model_3d, mode_no=100, seed=self.seed)
 
     def test_unstruct_1d(self):
         modes = self.rm_1d((self.x_tuple,))
         self.assertAlmostEqual(modes[0], 3.19799030)
         self.assertAlmostEqual(modes[1], 2.44848295)
 
     def test_unstruct_2d(self):
```

### Comparing `gstools-1.4.1/tests/test_rng.py` & `gstools-1.5.0/tests/test_rng.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This is the unittest of the RNG class.
 """
 
 import unittest
 
 import numpy as np
```

### Comparing `gstools-1.4.1/tests/test_srf.py` & `gstools-1.5.0/tests/test_srf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 """
 This is the unittest of SRF class.
 """
 
 import unittest
 
 import meshio
```

### Comparing `gstools-1.4.1/tests/test_transform.py` & `gstools-1.5.0/tests/test_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """This is the unittest of the transform submodule."""
 import unittest
 
 import numpy as np
 
 import gstools as gs
```

### Comparing `gstools-1.4.1/tests/test_variogram_structured.py` & `gstools-1.5.0/tests/test_variogram_structured.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This is a unittest of the variogram module.
 """
 
 import unittest
 
 import numpy as np
```

### Comparing `gstools-1.4.1/tests/test_variogram_unstructured.py` & `gstools-1.5.0/tests/test_variogram_unstructured.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This is a unittest of the variogram module.
 """
 
 import unittest
 
 import numpy as np
```

