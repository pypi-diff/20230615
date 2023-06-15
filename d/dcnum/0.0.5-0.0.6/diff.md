# Comparing `tmp/dcnum-0.0.5.tar.gz` & `tmp/dcnum-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.0.5.tar", last modified: Wed Jun 14 11:53:38 2023, max compression
+gzip compressed data, was "dcnum-0.0.6.tar", last modified: Thu Jun 15 21:46:04 2023, max compression
```

## Comparing `dcnum-0.0.5.tar` & `dcnum-0.0.6.tar`

### file list

```diff
@@ -1,76 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.497305 dcnum-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.489305 dcnum-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.489305 dcnum-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-14 11:53:23.000000 dcnum-0.0.5/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-14 11:53:23.000000 dcnum-0.0.5/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-14 11:53:23.000000 dcnum-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-14 11:53:23.000000 dcnum-0.0.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-14 11:53:23.000000 dcnum-0.0.5/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-14 11:53:23.000000 dcnum-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-14 11:53:38.497305 dcnum-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-14 11:53:23.000000 dcnum-0.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.489305 dcnum-0.0.5/dcnum/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 11:53:38.000000 dcnum-0.0.5/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/dcnum/feat/background/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/background/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/dcnum/feat/brightness/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/brightness/bright_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/dcnum/feat/haralick/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/haralick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/haralick/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/haralick/tex_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/dcnum/feat/moments/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/moments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/moments/ct_opencv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/feat/moments/mt_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/read/hdf5_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-06-14 11:53:23.000000 dcnum-0.0.5/dcnum/segm/segmenter_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.489305 dcnum-0.0.5/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-14 11:53:38.000000 dcnum-0.0.5/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-14 11:53:38.000000 dcnum-0.0.5/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:53:38.000000 dcnum-0.0.5/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 11:53:38.000000 dcnum-0.0.5/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-14 11:53:38.000000 dcnum-0.0.5/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-14 11:53:23.000000 dcnum-0.0.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.493305 dcnum-0.0.5/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-14 11:53:23.000000 dcnum-0.0.5/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-14 11:53:23.000000 dcnum-0.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-14 11:53:23.000000 dcnum-0.0.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-14 11:53:23.000000 dcnum-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 11:53:38.497305 dcnum-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.497305 dcnum-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:53:38.497305 dcnum-0.0.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_ppid.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-14 11:53:23.000000 dcnum-0.0.5/tests/test_segm_thresh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.651131 dcnum-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-15 21:45:50.000000 dcnum-0.0.6/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-15 21:45:50.000000 dcnum-0.0.6/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-15 21:45:50.000000 dcnum-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-15 21:45:50.000000 dcnum-0.0.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-15 21:45:50.000000 dcnum-0.0.6/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-15 21:45:50.000000 dcnum-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-15 21:46:04.651131 dcnum-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-15 21:45:50.000000 dcnum-0.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/dcnum/feat/background/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/background/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13626 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/feat/brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/brightness/bright_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/feat/haralick/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/haralick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/haralick/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/haralick/tex_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/feat/moments/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/moments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/moments/ct_opencv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/feat/moments/mt_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/read/hdf5_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/segm/segmenter_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/write/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-15 21:45:50.000000 dcnum-0.0.6/dcnum/write/writer_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.643130 dcnum-0.0.6/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 21:46:04.000000 dcnum-0.0.6/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-15 21:45:50.000000 dcnum-0.0.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-15 21:45:50.000000 dcnum-0.0.6/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-15 21:45:50.000000 dcnum-0.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 21:45:50.000000 dcnum-0.0.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-15 21:45:50.000000 dcnum-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 21:46:04.651131 dcnum-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.647131 dcnum-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 21:46:04.651131 dcnum-0.0.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   650653 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)   154010 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_ppid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_write_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-15 21:45:50.000000 dcnum-0.0.6/tests/test_write_writer_thread.py
```

### Comparing `dcnum-0.0.5/.github/workflows/check.yml` & `dcnum-0.0.6/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/.github/workflows/deploy_pypi.yml` & `dcnum-0.0.6/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/.gitignore` & `dcnum-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/LICENSE` & `dcnum-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/PKG-INFO` & `dcnum-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.5
+Version: 0.0.6
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.5/README.rst` & `dcnum-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/dcnum/feat/background/base.py` & `dcnum-0.0.6/dcnum/feat/background/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         """
         return self.get_ppid_from_kwargs(self.kwargs)
 
     def process(self):
         self.process_approach()
 
         bg_ppid = self.get_ppid()
-        # Write custom metadata
-        self.h5out.attrs["user:dcevent ppid background"] = bg_ppid
-        self.h5out.attrs["user:dcevent ppid generation"] = \
+        # Store pipeline information in the image_bg feature
+        self.h5out["events/image_bg"].attrs["dcnum ppid background"] = bg_ppid
+        self.h5out["events/image_bg"].attrs["dcnum ppid generation"] = \
             ppid.DCNUM_PPID_GENERATION
 
     @abc.abstractmethod
     def process_approach(self):
         """The actual background computation approach"""
```

### Comparing `dcnum-0.0.5/dcnum/feat/background/bg_roll_median.py` & `dcnum-0.0.6/dcnum/feat/background/bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/dcnum/feat/background/bg_sparse_median.py` & `dcnum-0.0.6/dcnum/feat/background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/dcnum/feat/brightness/bright_all.py` & `dcnum-0.0.6/dcnum/feat/brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/dcnum/feat/haralick/tex_all.py` & `dcnum-0.0.6/dcnum/feat/haralick/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/dcnum/feat/moments/mt_legacy.py` & `dcnum-0.0.6/dcnum/feat/moments/mt_legacy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/dcnum/meta/ppid.py` & `dcnum-0.0.6/dcnum/meta/ppid.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,18 @@
     hasher = hashlib.md5()
     hasher.update("|".join([gen_id, bg_id, seg_id, feat_id, gate_id]).encode())
     pph = hasher.hexdigest()
     return pph
 
 
 def convert_to_dtype(value, dtype):
-    if dtype is bool:
+    if isinstance(dtype, str):
+        raise ValueError("Annotations are strings, pleace make sure to not "
+                         "import __annotations__ from future!")
+    elif dtype is bool:
         if isinstance(value, str):
             if value.lower() in ["true", "yes"]:
                 value = True
             elif value.lower() in ["false", "no"]:
                 value = False
         value = bool(float(value))
     elif dtype in [pathlib.Path, pathlib.Path | str]:
```

### Comparing `dcnum-0.0.5/dcnum/read/cache.py` & `dcnum-0.0.6/dcnum/read/cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -28,14 +28,29 @@
         self.h5ds = h5ds
         self.chunk_size = chunk_size
         self.boolean = boolean
         self.cache_size = cache_size
         #: This is a FILO cache for the chunks
         self.cache = collections.OrderedDict()
         self.shape = h5ds.shape
+        self._len = len(self.h5ds)
+
+    def _get_chunk_index_for_index(self, index):
+        if index < 0:
+            index = len(self.h5ds) + index
+        chunk_index = index // self.chunk_size
+        sub_index = index % self.chunk_size
+        return chunk_index, sub_index
+
+    def __getitem__(self, index):
+        chunk_index, sub_index = self._get_chunk_index_for_index(index)
+        return self.get_chunk(chunk_index)[sub_index]
+
+    def __len__(self):
+        return self._len
 
     def get_chunk(self, chunk_index):
         """Get one chunk of images"""
         if chunk_index not in self.cache:
             fslice = slice(self.chunk_size * chunk_index,
                            self.chunk_size * (chunk_index + 1)
                            )
@@ -44,21 +59,24 @@
                 data = np.array(data, dtype=bool)
             self.cache[chunk_index] = data
             if len(self.cache) > self.cache_size:
                 # Remove the first item
                 self.cache.popitem(last=False)
         return self.cache[chunk_index]
 
-    def __getitem__(self, index):
-        """Return the image at the given index"""
-        if index < 0:
-            index = len(self.h5ds) + index
-        chunk_index = index // self.chunk_size
-        sub_index = index % self.chunk_size
-        return self.get_chunk(chunk_index)[sub_index]
+    def iter_chunks(self):
+        size = self.h5ds.shape[0]
+        index = 0
+        chunk = 0
+        while True:
+            yield chunk
+            chunk += 1
+            index += self.chunk_size
+            if index >= size:
+                break
 
 
 class ImageCorrCache:
     def __init__(self,
                  image: HDF5ImageCache,
                  image_bg: HDF5ImageCache):
         self.image = image
@@ -66,30 +84,40 @@
         self.chunk_size = image.chunk_size
         self.h5ds = image.h5ds
         self.shape = image.shape
         #: This is a FILO cache for the corrected image chunks
         self.cache = collections.OrderedDict()
         self.cache_size = image.cache_size
 
-    def _get_chunk(self, chunk_index):
+    def _get_chunk_index_for_index(self, index):
+        if index < 0:
+            index = len(self.h5ds) + index
+        chunk_index = index // self.chunk_size
+        sub_index = index % self.chunk_size
+        return chunk_index, sub_index
+
+    def __getitem__(self, index):
+        chunk_index, sub_index = self._get_chunk_index_for_index(index)
+        return self.get_chunk(chunk_index)[sub_index]
+
+    def __len__(self):
+        return len(self.image)
+
+    def get_chunk(self, chunk_index):
         if chunk_index not in self.cache:
             data = np.array(self.image.get_chunk(chunk_index), dtype=int) \
                 - self.image_bg.get_chunk(chunk_index)
             self.cache[chunk_index] = data
             if len(self.cache) > self.cache_size:
                 # Remove the first item
                 self.cache.popitem(last=False)
         return self.cache[chunk_index]
 
-    def __getitem__(self, index):
-        if index < 0:
-            index = len(self.h5ds) + index
-        chunk_index = index // self.chunk_size
-        sub_index = index % self.chunk_size
-        return self._get_chunk(chunk_index)[sub_index]
+    def iter_chunks(self):
+        return self.image.iter_chunks()
 
 
 @functools.cache
 def md5sum(path, blocksize=65536, count=0):
     """Compute (partial) MD5 sum of a file
 
     Parameters
```

### Comparing `dcnum-0.0.5/dcnum/read/hdf5_data.py` & `dcnum-0.0.6/dcnum/read/hdf5_data.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/dcnum/segm/segm_thresh.py` & `dcnum-0.0.6/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/dcnum/segm/segmenter.py` & `dcnum-0.0.6/dcnum/segm/segmenter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import abc
 import functools
 import inspect
 import logging
 
 import cv2
 import numpy as np
-from skimage import measure, morphology
+import scipy.ndimage as ndi
+from skimage import morphology
 
 from ..meta.ppid import kwargs_to_ppid
 
 
 class Segmenter(abc.ABC):
     #: Whether to enable mask post-processing. If disabled, you should
     #: make sure that your mask is properly defined and cleaned or you
@@ -112,28 +113,29 @@
     @staticmethod
     @functools.cache
     def get_disk(radius):
         """Cached `skimage.morphology.disk(radius)`"""
         return morphology.disk(radius)
 
     @staticmethod
-    def process_mask(mask, *,
+    def process_mask(labels, *,
                      clear_border: bool = True,
                      fill_holes: bool = True,
                      closing_disk: int = 5):
         """Post-process retrieved mask image
 
         This is an optional convenience method that is called for each
         subclass individually. To enable mask post-processing, set
         `mask_postprocessing=True` in the subclass and specify default
         `mask_default_kwargs`.
 
         Parameters
         ----------
-        mask: 2d boolean ndarray
+        labels: 2d integer ndarray
+            Labeled input (contains blobs with same number)
         clear_border: bool
             clear the image boarder using
             :func:`skimage.segmentation.clear_border`
         fill_holes: bool
             binary-fill-holes in the binary mask image using
             :func:`scipy.ndimage.binary_fill_holes`
         closing_disk: int or None
@@ -141,84 +143,98 @@
             of that radius in pixels
         """
         if clear_border:
             #
             # from skimage import segmentation
             # segmentation.clear_border(mask, out=mask)
             #
-            if (mask[0, :].sum() or mask[-1, :].sum()
-                    or mask[:, 0].sum() or mask[:, -1].sum()):
-                border = np.zeros_like(mask)
+            if (labels[0, :].sum() or labels[-1, :].sum()
+                    or labels[:, 0].sum() or labels[:, -1].sum()):
+                border = np.zeros_like(labels, dtype=bool)
                 border[0] = True
                 border[-1] = True
                 border[:, 0] = True
                 border[:, -1] = True
-                label = measure.label(mask)
-                indices = sorted(np.unique(label[border]))
+                indices = sorted(np.unique(labels[border]))
                 for ii in indices[1:]:
-                    mask[label == ii] = False
+                    labels[labels == ii] = 0
 
         # scikit-image is too slow for us here. So we use OpenCV.
         # https://github.com/scikit-image/scikit-image/issues/1190
-        mask_int = np.array(mask, dtype=np.uint8) * 255
 
         if closing_disk:
             #
             # from skimage import morphology
             # morphology.binary_closing(
             #    mask,
             #    footprint=morphology.disk(closing_disk),
             #    out=mask)
             #
             element = Segmenter.get_disk(closing_disk)
-            mask_dilated = cv2.dilate(mask_int, element)
-            mask_int = cv2.erode(mask_dilated, element)
+            labels_uint8 = np.array(labels, dtype=np.uint8)
+            labels_dilated = cv2.dilate(labels_uint8, element)
+            labels_eroded = cv2.erode(labels_dilated, element)
+            labels, _ = ndi.label(labels_eroded > 0)
 
         if fill_holes:
+            # Floodfill only works with uint8 (too small) or int32
+            if not labels.dtype == np.int32:
+                labels = np.array(labels, dtype=np.int32)
             #
             # from scipy import ndimage
             # mask_old = ndimage.binary_fill_holes(mask)
             #
             # Floodfill algorithm fills the background image and
             # the resulting inversion is the image with holes filled.
-            im_floodfill = mask_int.copy()
-            h, w = mask_int.shape
-            ff_mask = np.zeros((h + 2, w + 2), np.uint8)
-            cv2.floodFill(im_floodfill, ff_mask, (0, 0), 255)
-            im_floodfill_inv = cv2.bitwise_not(im_floodfill)
-            mask_int = mask_int | im_floodfill_inv
-
-        mask = mask_int > 0
-        return mask
+            # This will destroy labels (adding 2,147,483,647 to background)
+            cv2.floodFill(labels, None, (0, 0), 2147483647)
+            mask = labels != 2147483647
+            labels, _ = ndi.label(
+                input=mask,
+                structure=ndi.generate_binary_structure(2, 2))
+
+        return labels
+
+    def segment_chunk(self, image_data, chunk, debug=False):
+        """Return the integer labels for one `image_data` chunk"""
+        data = image_data.get_chunk(chunk)
+        return self.segment_batch(data, debug=debug)
 
     def segment_frame(self, image):
-        """Return the frame mask for one image at `index`"""
+        """Return the integer label image for `index`"""
         segm_wrap = self.segment_frame_wrapper()
-        # obtain mask
-        mask = segm_wrap(image)
+        # obtain mask or label
+        mol = segm_wrap(image)
+        if mol.dtype == bool:
+            # convert mask to label
+            labels, num_labels = ndi.label(
+                input=mol,
+                structure=ndi.generate_binary_structure(2, 2))
+        else:
+            labels = mol
         # optional postprocessing
         if self.mask_postprocessing:
-            mask = self.process_mask(mask, **self.kwargs_mask)
-        return mask
+            labels = self.process_mask(labels, **self.kwargs_mask)
+        return labels
 
     @functools.cache
     def segment_frame_wrapper(self):
         if self.kwargs:
             # For segmenters that accept keyword arguments.
             segm_wrap = functools.partial(self.segment_approach,
                                           **self.kwargs)
         else:
             # For segmenters that don't accept keyword arguments.
             segm_wrap = self.segment_approach
         return segm_wrap
 
     @staticmethod
     @abc.abstractmethod
-    def segment_approach(image, image_bg):
-        """Perform segmentation and return binary mask
+    def segment_approach(image):
+        """Perform segmentation and return integer label or binary mask image
 
         This is the approach the subclasses implements.
         """
 
     @abc.abstractmethod
-    def segment_batch(self, data, start, stop):
-        """Return the frame mask array for an entire batch"""
+    def segment_batch(self, data, start=None, stop=None, debug=False):
+        """Return the integer labels for an entire batch"""
```

### Comparing `dcnum-0.0.5/dcnum/segm/segmenter_cpu.py` & `dcnum-0.0.6/dcnum/segm/segmenter_cpu.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
     #: Number of segmenter processes to use.
     num_processes = None
 
     def __init__(self, *args, **kwargs):
         super(CPUSegmenter, self).__init__(*args, **kwargs)
         self.mp_image_raw = None
         self._mp_image_np = None
-        self.mp_mask_raw = None
-        self._mp_mask_np = None
+        self.mp_labels_raw = None
+        self._mp_labels_np = None
         self._mp_workers = []
         # Image shape of the input array
         self.image_shape = None
         # Processing control values
         # <-1: exit
         # -1: idle
         # 0: start
@@ -39,15 +39,15 @@
         # This is important when using "spawn" to create new processes,
         # because then the entire object gets pickled and some things
         # cannot be pickled!
         state = self.__dict__.copy()
         # Remove the unpicklable entries.
         del state["logger"]
         del state["_mp_image_np"]
-        del state["_mp_mask_np"]
+        del state["_mp_labels_np"]
         del state["_mp_workers"]
         return state
 
     def __setstate__(self, state):
         # Restore instance attributes (i.e., filename and lineno).
         self.__dict__.update(state)
 
@@ -58,15 +58,15 @@
         Parameters
         ----------
         image_shape: tuple of int
             Shape of one single image in the array
         batch_size: int
             Number of images in the array
         dtype:
-            ctype, e.g. `np.ctypeslib.ctypes.c_int8`
+            ctype, e.g. `np.ctypeslib.ctypes.c_uint8`
             or `np.ctypeslib.ctypes.c_bool`
         """
         sx, sy = image_shape
         sa_raw = mp.RawArray(dtype, int(sx * sy * batch_size))
         # Convert the RawArray to something we can write to fast
         # (similar to memory view, but without having to cast) using
         # np.ctypeslib.as_array. See discussion in
@@ -75,27 +75,31 @@
         return sa_raw, sa_np
 
     @property
     def image_array(self):
         return self._mp_image_np
 
     @property
+    def labels_array(self):
+        return self._mp_labels_np
+
+    @property
     def mask_array(self):
-        return self._mp_mask_np
+        return np.array(self._mp_labels_np, dtype=bool)
 
     def join_workers(self):
         """Ask all workers to stop and join them"""
         if self._mp_workers:
             self.mp_shutdown.value = 1
             [w.join() for w in self._mp_workers]
 
     def segment_batch(self,
                       image_data: np.ndarray,
-                      start: int,
-                      stop: int,
+                      start: int = None,
+                      stop: int = None,
                       debug: bool = False):
         """Perform batch segmentation of `image_data`
 
         Parameters
         ----------
         image_data: 3d np.ndarray
             The time-series image data. First axis is time.
@@ -107,44 +111,48 @@
             Whether to run this in debug mode (using a single thread)
 
         Notes
         -----
         - If the segmentation algorithm only accepts background-corrected
           images, then `image_data` must already be background-corrected.
         """
+        if stop is None or start is None:
+            start = 0
+            stop = len(image_data)
+
         batch_size = stop - start
         size = np.prod(image_data[0]) * batch_size
 
         if self.image_shape is None:
             self.image_shape = image_data[0].shape
 
         if self._mp_image_np is not None and self._mp_image_np.size != size:
             # reset image data
             self._mp_image_np = None
-            self._mp_mask_np = None
+            self._mp_labels_np = None
             # TODO: If only the batch_size changes, don't
             #  reinitialize the workers. Otherwise, the final rest of
             #  analyzing a dataset would always take a little longer.
             self.join_workers()
             self._mp_workers = []
             self.mp_batch_index.value = -1
             self.mp_shutdown.value = 0
 
         if self._mp_image_np is None:
             self.mp_image_raw, self._mp_image_np = self._create_shared_array(
                 image_shape=self.image_shape,
                 batch_size=batch_size,
-                dtype=np.ctypeslib.ctypes.c_int8,
+                dtype=np.ctypeslib.ctypes.c_int32,
             )
 
-        if self._mp_mask_np is None:
-            self.mp_mask_raw, self._mp_mask_np = self._create_shared_array(
+        if self._mp_labels_np is None:
+            self.mp_labels_raw, self._mp_labels_np = self._create_shared_array(
                 image_shape=self.image_shape,
                 batch_size=batch_size,
-                dtype=np.ctypeslib.ctypes.c_bool,
+                dtype=np.ctypeslib.ctypes.c_uint16,
             )
 
         # populate image data
         self._mp_image_np[:] = image_data[start:stop]
 
         # Create the workers
         if debug:
@@ -178,15 +186,15 @@
         # Tell workers to get going
         self.mp_batch_worker.value = 0
 
         # Wait for all workers to complete
         while self.mp_batch_worker.value != num_workers:
             time.sleep(.1)
 
-        return self._mp_mask_np
+        return self._mp_labels_np
 
 
 class CPUSegmenterWorker:
     def __init__(self,
                  segmenter,
                  sl_start: int,
                  sl_stop: int,
@@ -213,25 +221,25 @@
         # their part of the batch.
         self.batch_worker = segmenter.mp_batch_worker
         # Shutdown bit tells workers to stop when set to != 0
         self.shutdown = segmenter.mp_shutdown
         # The image data for segmentation
         self.image_data_raw = segmenter.mp_image_raw
         # Boolean mask array
-        self.mask_data_raw = segmenter.mp_mask_raw
+        self.labels_data_raw = segmenter.mp_labels_raw
         # The shape of one image
         self.image_shape = segmenter.image_shape
         self.sl_start = sl_start
         self.sl_stop = sl_stop
 
     def run(self):
         # We have to create the numpy-versions of the mp.RawArrays here,
         # otherwise we only get some kind of copy in the new process
         # when we use "spawn" instead of "fork".
-        mask_data = np.ctypeslib.as_array(self.mask_data_raw).reshape(
+        labels_data = np.ctypeslib.as_array(self.labels_data_raw).reshape(
             -1, self.image_shape[0], self.image_shape[1])
         image_data = np.ctypeslib.as_array(self.image_data_raw).reshape(
             -1, self.image_shape[0], self.image_shape[1])
 
         idx = self.sl_start
         itr = 0  # current iteration (incremented when we reach self.sl_stop)
         while True:
@@ -240,15 +248,15 @@
                 if idx == self.sl_stop:
                     # We finished processing everything.
                     itr += 1  # prevent running same things again
                     idx = self.sl_start  # reset counter for next batch
                     with self.batch_worker:
                         self.batch_worker.value += 1
                 else:
-                    mask_data[idx, :, :] = self.segmenter.segment_frame(
+                    labels_data[idx, :, :] = self.segmenter.segment_frame(
                         image_data[idx])
                     idx += 1
             elif self.shutdown.value:
                 break
             else:
                 # Wait for more data to arrive
                 time.sleep(.03)
```

### Comparing `dcnum-0.0.5/dcnum.egg-info/PKG-INFO` & `dcnum-0.0.6/dcnum.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.0.5
+Version: 0.0.6
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.0.5/dcnum.egg-info/SOURCES.txt` & `dcnum-0.0.6/dcnum.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 dcnum/read/cache.py
 dcnum/read/const.py
 dcnum/read/hdf5_data.py
 dcnum/segm/__init__.py
 dcnum/segm/segm_thresh.py
 dcnum/segm/segmenter.py
 dcnum/segm/segmenter_cpu.py
+dcnum/write/__init__.py
+dcnum/write/writer.py
+dcnum/write/writer_thread.py
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/extensions/github_changelog.py
 tests/conftest.py
 tests/helper_methods.py
 tests/requirements.txt
@@ -49,9 +52,11 @@
 tests/test_feat_moments_based.py
 tests/test_init.py
 tests/test_ppid.py
 tests/test_ppid_segm.py
 tests/test_read_concat_hdf5.py
 tests/test_read_hdf5.py
 tests/test_segm_thresh.py
+tests/test_write_writer.py
+tests/test_write_writer_thread.py
 tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
 tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
```

### Comparing `dcnum-0.0.5/docs/conf.py` & `dcnum-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/docs/extensions/github_changelog.py` & `dcnum-0.0.6/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/pyproject.toml` & `dcnum-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.0.6/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.0.6/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/helper_methods.py` & `dcnum-0.0.6/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.0.6/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/test_feat_brightness.py` & `dcnum-0.0.6/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/test_feat_haralick.py` & `dcnum-0.0.6/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/test_feat_moments_based.py` & `dcnum-0.0.6/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/test_ppid.py` & `dcnum-0.0.6/tests/test_ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/test_read_concat_hdf5.py` & `dcnum-0.0.6/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.0.5/tests/test_read_hdf5.py` & `dcnum-0.0.6/tests/test_read_hdf5.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pathlib
 import pickle
 
 import h5py
 import numpy as np
+import pytest
 
 from dcnum import read
 
 from helper_methods import retrieve_data
 
 data_path = pathlib.Path(__file__).parent / "data"
 
@@ -43,14 +44,28 @@
         assert np.allclose(hic[140], h5["events/image"][140])
         assert len(hic.cache) == 2  # limited to two
         assert 0 not in hic.cache  # first item gets removed
         assert 1 in hic.cache
         assert 2 in hic.cache
 
 
+@pytest.mark.parametrize("size, chunks", [(209, 21),
+                                          (210, 21),
+                                          (211, 22)])
+def test_image_cache_iter_chunks(size, chunks, tmp_path):
+    path = tmp_path / "test.hdf5"
+    with h5py.File(path, "w") as hw:
+        hw["events/image"] = np.random.rand(size, 80, 180)
+    with h5py.File(path, "r") as h5:
+        hic = read.HDF5ImageCache(h5["events/image"],
+                                  chunk_size=10,
+                                  cache_size=2)
+        assert list(hic.iter_chunks()) == list(range(chunks))
+
+
 def test_pixel_size_getset(tmp_path):
     path = tmp_path / "test.hdf5"
     with h5py.File(path, "w") as hw:
         hw["events/image"] = np.random.rand(10, 80, 180)
         hw.attrs["imaging:pixel size"] = 0.123
 
     h5dat = read.HDF5Data(path)
```

