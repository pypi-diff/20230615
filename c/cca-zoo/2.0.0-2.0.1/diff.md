# Comparing `tmp/cca_zoo-2.0.0.tar.gz` & `tmp/cca_zoo-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cca_zoo-2.0.0.tar", last modified: Fri Jun  9 14:21:14 2023, max compression
+gzip compressed data, was "dist/cca_zoo-2.0.1.tar", last modified: Thu Jun 15 12:07:42 2023, max compression
```

## Comparing `cca_zoo-2.0.0.tar` & `cca_zoo-2.0.1.tar`

### file list

```diff
@@ -1,109 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/data/deep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/data/simulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_barlow_twins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_noi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_sdl.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dtcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_dccae.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_splitae.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/objectives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/model_selection/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/model_selection/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_gcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_grcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_altmaxvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_elasticnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_gradkcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_incrementalpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_pls_als.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_pmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_admm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_hsic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_parkhomenko.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_stochasticpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_swcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_kcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_mcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_ncca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_partialcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_pcacca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_plsmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_prcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_rcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_tcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/plotting/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/probabilisticmodels/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/probabilisticmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/probabilisticmodels/_probabilisticcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_deepmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_probabilistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_regularised.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_unregularized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/utils/check_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_dcca_custom_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_dcca_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_hyperparameter_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_kernel_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_many_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_sparse_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-09 14:21:13.000000 cca_zoo-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/classical/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_gcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_grcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_altmaxvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_elasticnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_gradkcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_incrementalpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_pls_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_pmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_admm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_hsic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_stochasticpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_swcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_kcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_mcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_ncca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_partialcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_pcacca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_plsmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_prcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_tcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/data/deep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/data/simulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_noi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_sdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dgcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dtcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/_dccae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/_splitae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/objectives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/model_selection/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/model_selection/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/probabilistic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/probabilistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/probabilistic/_probabilisticcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_deepmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_probabilistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_regularised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_unregularized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/utils/check_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/visualisation/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_dcca_custom_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_dcca_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_hyperparameter_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_kernel_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_many_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_sparse_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-15 12:07:40.000000 cca_zoo-2.0.1/setup.py
```

### Comparing `cca_zoo-2.0.0/PKG-INFO` & `cca_zoo-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca_zoo
-Version: 2.0.0
+Version: 2.0.1
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.0/README.md` & `cca_zoo-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.0/cca_zoo/data/deep.py` & `cca_zoo-2.0.1/cca_zoo/data/deep.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.0/cca_zoo/data/simulated.py` & `cca_zoo-2.0.1/cca_zoo/data/simulated.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,202 +1,162 @@
 import itertools
 from typing import List, Union
 
 import numpy as np
-from scipy import linalg
 from scipy.linalg import block_diag
+from sklearn.datasets import make_spd_matrix
 from sklearn.utils.validation import check_random_state
 
 from cca_zoo.utils import _process_parameter
 
 
 class LinearSimulatedData:
+    # This class generates simulated data for linear classical with multiple views
     def __init__(
         self,
         view_features: List[int],
         latent_dims: int = 1,
-        view_sparsity: List[Union[int, float]] = None,
+        view_sparsity: Union[List[float], float] = None,
         correlation: Union[List[float], float] = 0.99,
-        structure: Union[str, List[str]] = None,
-        sigma: Union[List[float], float] = None,
-        decay: float = 0.5,
-        positive=None,
+        structure: str = "random",
+        positive: Union[bool, List[bool]] = False,
         random_state: Union[int, np.random.RandomState] = None,
     ):
-        """
-
-        Parameters
-        ----------
-        view_features : List[int]
-            Number of features in each view
-        latent_dims : int
-            Number of latent dimensions
-        view_sparsity : List[Union[int, float]]
-            Sparsity of each view
-        correlation : Union[List[float], float]
-            Correlation between views
-        structure : Union[str, List[str]]
-            Structure of each view
-        sigma : Union[List[float], float]
-            Noise level of each view
-        positive : None
-            Unused
-        random_state : Union[int, np.random.RandomState]
-            Random state
-        """
         self.view_features = view_features
         self.latent_dims = latent_dims
         self.correlation = correlation
         self.random_state = check_random_state(random_state)
+        # Process the correlation parameter to ensure it is a list of length latent_dimensions
         self.correlation = _process_parameter(
             "correlation", correlation, 0.99, latent_dims
         )
-        # correlation must all be less than 1
-        if np.any(np.abs(self.correlation) >= 1):
-            raise ValueError("Magnitude of Correlation must be less than 1")
-        self.structure = _process_parameter(
-            "structure", structure, "identity", len(view_features)
-        )
         self.view_sparsity = _process_parameter(
-            "view_sparsity", view_sparsity, 1, len(view_features)
+            "view_sparsity", view_sparsity, 0.5, len(view_features)
+        )
+        self.structure = _process_parameter(
+            "structure", structure, "random", len(view_features)
         )
         self.positive = _process_parameter(
             "positive", positive, False, len(view_features)
         )
-        self.sigma = _process_parameter("sigma", sigma, 0.5, len(view_features))
-
-        self.mean, covs, self.true_features = self._generate_covariance_matrices()
+        # Generate the covariance matrices and the true features for each view
+        covs, self.true_features = self._generate_covariance_matrices()
+        # Generate the joint covariance matrix by combining the view covariances and the cross-covariances
         joint_cov = self._generate_joint_covariance(covs)
+        # Compute the Cholesky decomposition of the joint covariance matrix
         self.chol = np.linalg.cholesky(joint_cov)
 
-    def _generate_covariance_matrix(self, view_p, view_structure, view_sigma):
+    def _generate_covariance_matrix(self, view_features, view_structure):
+        # Generate a covariance matrix for a single view based on its structure
         if view_structure == "identity":
-            cov = np.eye(view_p)
-        elif view_structure == "gaussian":
-            cov = _generate_gaussian_cov(view_p, view_sigma)
-        elif view_structure == "toeplitz":
-            cov = _generate_toeplitz_cov(view_p, view_sigma)
+            # Use an identity matrix as the covariance matrix
+            cov = np.eye(view_features)
         elif view_structure == "random":
-            cov = _generate_random_cov(view_p, self.random_state)
-        else:
-            raise ValueError(f"Unknown structure {view_structure}")
+            # Use a random positive definite matrix as the covariance matrix
+            cov = make_spd_matrix(view_features)
         return cov
 
     def _generate_joint_covariance(self, covs):
+        # Generate a joint covariance matrix for all views by stacking the view covariances and adding cross-covariances
         cov = block_diag(*covs)
         splits = np.concatenate(([0], np.cumsum(self.view_features)))
         for i, j in itertools.combinations(range(len(splits) - 1), 2):
             cross = np.zeros((self.view_features[i], self.view_features[j]))
             for _ in range(self.latent_dims):
+                # Compute the cross-covariance matrix for a pair of views and a latent dimension using the correlation coefficient and the true features
                 A = self.correlation[_] * np.outer(
                     self.true_features[i][:, _], self.true_features[j][:, _]
                 )
-                # Cross Bit
+                # Multiply the cross-covariance matrix by the view covariances to get the final cross-covariance matrix
                 cross += covs[i] @ A @ covs[j]
+            # Assign the cross-covariance matrix to the corresponding blocks in the joint covariance matrix
             cov[
                 splits[i] : splits[i] + self.view_features[i],
                 splits[j] : splits[j] + self.view_features[j],
             ] = cross
             cov[
                 splits[j] : splits[j] + self.view_features[j],
                 splits[i] : splits[i] + self.view_features[i],
             ] = cross.T
         return cov
 
     def _generate_covariance_matrices(self):
-        mean = np.zeros(sum(self.view_features))
-        covs = []
-        true_features = []
-        for view_p, sparsity, view_structure, view_positive, view_sigma in zip(
-            self.view_features,
-            self.view_sparsity,
-            self.structure,
-            self.positive,
-            self.sigma,
-        ):
-            cov = self._generate_covariance_matrix(view_p, view_structure, view_sigma)
-            weights = self.random_state.randn(view_p, self.latent_dims)
-            if sparsity <= 1:
-                sparsity = np.ceil(sparsity * view_p).astype("int")
-            if sparsity < view_p:
-                mask = np.stack(
-                    (
-                        np.concatenate(
-                            ([0] * (view_p - sparsity), [1] * sparsity)
-                        ).astype(bool),
-                    )
-                    * self.latent_dims,
-                    axis=0,
-                ).T
-                mask = mask.flatten()
-                self.random_state.shuffle(mask)
-                mask = mask.reshape(weights.shape)
-                weights = weights * mask
-                if view_positive:
-                    weights[weights < 0] = 0
-            weights = _decorrelate_dims(weights, cov)
-            weights /= np.sqrt(np.diag((weights.T @ cov @ weights)))
-            true_features.append(weights)
-            covs.append(cov)
-        return mean, covs, true_features
+        # Generate a list of covariance matrices and true features for each view using list comprehensions
+        covs = [
+            self._generate_covariance_matrix(view_features, structure)
+            for view_features, structure in zip(self.view_features, self.structure)
+        ]
+
+        true_features = [
+            self._generate_true_feature(cov, sparsity, view_positive)
+            for cov, sparsity, view_positive, view_features in zip(
+                covs, self.view_sparsity, self.positive, self.view_features
+            )
+        ]
+        return covs, true_features
+
+    def _generate_true_feature(self, cov, sparsity, view_positive):
+        # Generate a true feature matrix for a single view using its covariance matrix and sparsity level
+
+        # Generate a random weight matrix with normal distribution and the same shape as the covariance matrix
+        weights = self._generate_weights_matrix(cov.shape[0])
+
+        # Apply a sparsity mask to the weight matrix to make some elements zero
+        weights = self._apply_sparsity_mask(weights, sparsity)
+
+        # Make the weight matrix positive if needed by taking the absolute value of the elements
+        if view_positive:
+            weights = self._make_weights_positive(weights)
+
+        # Decorrelate the weight matrix from the covariance matrix and normalize it
+        weights = _decorrelate_dims(weights, cov)
+        weights /= np.sqrt(np.diag((weights.T @ cov @ weights)))
+        return weights
+
+    def _generate_weights_matrix(self, view_features):
+        # Generate a random matrix with normal distribution and the given number of rows and latent dimensions
+        return self.random_state.randn(view_features, self.latent_dims)
+
+    def _apply_sparsity_mask(self, weights, sparsity):
+        view_features = weights.shape[0]
+        # convert sparsity to an integer number of nonzero elements
+        if sparsity <= 1:
+            sparsity = np.ceil(sparsity * view_features).astype("int")
+        # create a binary mask with sparsity number of ones
+        mask = np.stack(
+            (
+                np.concatenate(
+                    ([0] * (view_features - sparsity), [1] * sparsity)
+                ).astype(bool),
+            )
+            * self.latent_dims,
+            axis=0,
+        ).T
+        # shuffle the mask randomly
+        mask = mask.flatten()
+        self.random_state.shuffle(mask)
+        mask = mask.reshape(weights.shape)
+        # apply the mask to the weights matrix
+        return weights * mask
+
+    def _make_weights_positive(self, weights):
+        # set all negative elements to zero
+        return np.abs(weights)
 
     def sample(self, n: int):
-        # check self.chol exists
         X = np.zeros((n, self.chol.shape[0]))
         for i in range(n):
-            X[i, :] = self._chol_sample(self.mean, self.chol, self.random_state)
+            X[i, :] = self._chol_sample(self.chol)
         views = np.split(X, np.cumsum(self.view_features)[:-1], axis=1)
         return views
 
-    @staticmethod
-    def _chol_sample(mean, chol, random_state):
-        rng = check_random_state(random_state)
-        return mean + chol @ rng.randn(mean.size)
+    def _chol_sample(self, chol):
+        rng = check_random_state(self.random_state)
+        return chol @ rng.randn(chol.shape[0])
 
 
 def _decorrelate_dims(up, cov):
     A = up.T @ cov @ up
     for k in range(1, A.shape[0]):
         up[:, k:] -= np.outer(up[:, k - 1], A[k - 1, k:] / A[k - 1, k - 1])
         A = up.T @ cov @ up
     return up
-
-
-def _gaussian(x, mu, sig, dn):
-    """
-    Generate a gaussian covariance matrix
-
-    :param x:
-    :param mu:
-    :param sig:
-    :param dn:
-    """
-    return (
-        np.exp(-np.power(x - mu, 2.0) / (2 * np.power(sig, 2.0)))
-        * dn
-        / (np.sqrt(2 * np.pi) * sig)
-    )
-
-
-def _generate_gaussian_cov(p, sigma):
-    x = np.linspace(-1, 1, p)
-    x_tile = np.tile(x, (p, 1))
-    mu_tile = np.transpose(x_tile)
-    dn = 2 / (p - 1)
-    cov = _gaussian(x_tile, mu_tile, sigma, dn)
-    cov /= cov.max()
-    return cov
-
-
-def _generate_toeplitz_cov(p, sigma):
-    c = np.arange(0, p)
-    c = sigma**c
-    cov = linalg.toeplitz(c, c)
-    return cov
-
-
-def _generate_random_cov(p, random_state):
-    rng = check_random_state(random_state)
-    cov_ = rng.randn(p, p)
-    U, S, Vt = np.linalg.svd(cov_.T @ cov_)
-    cov = U @ (1 + np.diag(rng.randn(p))) @ Vt
-    return cov
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/__init__.py` & `cca_zoo-2.0.1/cca_zoo/deep/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 from . import architectures, callbacks, objectives
-from ._discriminative import DCCA, DCCA_EY, DCCA_NOI, DCCA_SDL, DTCCA, BarlowTwins
+from ._discriminative import (
+    DCCA,
+    DCCA_EY,
+    DCCA_GH,
+    DCCA_SVD,
+    DCCA_NOI,
+    DCCA_SDL,
+    DTCCA,
+    BarlowTwins,
+    DGCCA,
+)
 from ._generative import DCCAE, DVCCA, SplitAE
 
 __all__ = [
     "DCCA",
     "DCCAE",
     "DCCA_NOI",
     "DCCA_SDL",
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_base.py` & `cca_zoo-2.0.1/cca_zoo/deep/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import numpy as np
 import pytorch_lightning as pl
 import torch
 from torch.optim.lr_scheduler import CosineAnnealingLR, MultiStepLR
 
 
 class BaseDeep(pl.LightningModule):
-    """A base class for deep learning models using PyTorch Lightning."""
+    """A base class for deep learning classical using PyTorch Lightning."""
 
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         optimizer: str = "adam",
         scheduler: Optional[str] = None,
         lr: float = 1e-2,
         weight_decay: float = 0,
         extra_optimizer_kwargs: Optional[Dict[str, Any]] = None,
         max_epochs: int = 1000,
         min_lr: float = 1e-9,
@@ -24,15 +24,15 @@
         correlation: bool = True,
         *args,
         **kwargs,
     ):
         super().__init__()
         if extra_optimizer_kwargs is None:
             extra_optimizer_kwargs = {}
-        self.latent_dims = latent_dims
+        self.latent_dimensions = latent_dimensions
         self.optimizer = optimizer
         self.scheduler = scheduler
         self.lr = lr
         self.weight_decay = weight_decay
         self.extra_optimizer_kwargs = extra_optimizer_kwargs
         self.max_epochs = max_epochs
         self.min_lr = min_lr
@@ -71,29 +71,37 @@
         """Performs one step of testing on a batch of views."""
         loss = self.loss(batch["views"])
         for k, v in loss.items():
             # Use f-string instead of concatenation
             self.log(f"test/{k}", v)
         return loss["objective"]
 
-    def transform(
+    @torch.no_grad()
+    def get_representations(
         self,
         loader: torch.utils.data.DataLoader,
-    ) -> List[np.ndarray]:
+    ):
         """Returns the latent representations for each view in the loader."""
-        with torch.no_grad():
-            # Use list comprehension instead of for loop
-            z = [
-                self([view.to(self.device) for view in batch["views"]])
-                for batch in loader
-            ]
+        # self.eval()
         # Use list comprehension instead of for loop
-        z = [torch.vstack(i).cpu().numpy() for i in zip(*z)]
+        z = [
+            self([view.to(self.device).detach().cpu() for view in batch["views"]])
+            for batch in loader
+        ]
+        # Use list comprehension instead of for loop
+        z = [torch.vstack(z_) for z_ in zip(*z)]
         return z
 
+    def transform(
+        self,
+        loader: torch.utils.data.DataLoader,
+    ) -> List[np.ndarray]:
+        """Returns the latent representations for each view in the loader."""
+        return [z.numpy() for z in self.get_representations(loader)]
+
     def configure_optimizers(
         self,
     ) -> Union[
         torch.optim.Optimizer,
         Tuple[List[torch.optim.Optimizer], List[torch.optim.lr_scheduler._LRScheduler]],
     ]:
         """Configures the optimizer and the learning rate scheduler."""
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca.py` & `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,56 @@
 import torch
 
-from cca_zoo.deepmodels import objectives
-from cca_zoo.deepmodels._base import BaseDeep
-from cca_zoo.deepmodels.callbacks import CorrelationCallback
-from cca_zoo.models import MCCA
-from cca_zoo.models._base import BaseModel
+from cca_zoo.deep import objectives
+from cca_zoo.deep._base import BaseDeep
+from cca_zoo.deep.metrics import MCCA
+from cca_zoo.classical._base import BaseModel
 
 
 class DCCA(BaseDeep, BaseModel):
     """
     A class used to fit a DCCA model.
 
     References
     ----------
     Andrew, Galen, et al. "Deep canonical correlation analysis." International conference on machine learning. PMLR, 2013.
 
     """
 
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         objective=objectives.MCCA,
         encoders=None,
         r: float = 0,
         eps: float = 1e-5,
         **kwargs,
     ):
-        super().__init__(latent_dims=latent_dims, **kwargs)
+        super().__init__(latent_dimensions=latent_dimensions, **kwargs)
         # Check if encoders are provided and have the same length as the number of views
         if encoders is None:
             raise ValueError(
                 "Encoders must be a list of torch.nn.Module with length equal to the number of views."
             )
         self.encoders = torch.nn.ModuleList(encoders)
-        self.objective = objective(latent_dims, r=r, eps=eps)
+        self.objective = objective(latent_dimensions, r=r, eps=eps)
+        self.correlation = MCCA()
 
     def forward(self, views, **kwargs):
+        if not hasattr(self, "n_views_"):
+            self.n_views_ = len(views)
         # Use list comprehension to encode each view
         z = [encoder(view) for encoder, view in zip(self.encoders, views)]
         return z
 
     def loss(self, views, **kwargs):
         z = self(views)
         return {"objective": self.objective.loss(z)}
 
-    def pairwise_correlations(
-        self,
-        loader: torch.utils.data.DataLoader,
-        train=False,
-    ):
+    def pairwise_correlations(self, loader: torch.utils.data.DataLoader):
         # Call the parent class method
-        return super().pairwise_correlations(loader, train=train)
+        return super().pairwise_correlations(loader)
 
     def score(self, loader: torch.utils.data.DataLoader, **kwargs):
-        z = self.transform(loader)
-        return MCCA(self.latent_dims).fit(z).score(z)
-
-    def configure_callbacks(self):
-        return [CorrelationCallback()]
+        z = self.get_representations(loader)
+        corr = self.correlation(z)
+        return corr.numpy()
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_barlow_twins.py` & `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,28 @@
     ----------
     Zbontar, Jure, et al. "Barlow twins: Self-supervised learning via redundancy reduction." arXiv preprint arXiv:2103.03230 (2021).
 
     """
 
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         encoders=None,
         lam=1,
         **kwargs,
     ):
-        super().__init__(latent_dims=latent_dims, encoders=encoders, **kwargs)
+        super().__init__(
+            latent_dimensions=latent_dimensions, encoders=encoders, **kwargs
+        )
         self.lam = lam  # the lambda parameter for the off-diagonal terms of the cross-covariance matrix
         self.bns = torch.nn.ModuleList(
-            [torch.nn.BatchNorm1d(latent_dims, affine=False) for _ in self.encoders]
+            [
+                torch.nn.BatchNorm1d(latent_dimensions, affine=False)
+                for _ in self.encoders
+            ]
         )  # a list of batch normalization layers for each encoder
 
     def forward(self, views, **kwargs):
         z = []
         for i, (encoder, bn) in enumerate(zip(self.encoders, self.bns)):
             z.append(bn(encoder(views[i])))  # encode and normalize each view
         return z  # return a list of normalized latent representations
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_ey.py` & `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_ey.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,16 +7,18 @@
     """
 
     References
     ----------
     Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A Generalized EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
     """
 
-    def __init__(self, latent_dims: int, encoders=None, r: float = 0, **kwargs):
-        super().__init__(latent_dims=latent_dims, encoders=encoders, **kwargs)
+    def __init__(self, latent_dimensions: int, encoders=None, r: float = 0, **kwargs):
+        super().__init__(
+            latent_dimensions=latent_dimensions, encoders=encoders, **kwargs
+        )
         self.r = r
 
     def forward(self, views, **kwargs):
         z = []
         for i, encoder in enumerate(self.encoders):
             z.append(encoder(views[i]))  # encode each view into a latent representation
         return z  # return a list of latent representations
@@ -35,23 +37,23 @@
             "objective": -rewards + penalties,  # return the negative objective value
             "rewards": rewards,  # return the total rewards
             "penalties": penalties,  # return the penalties matrix
         }
 
     def get_AB(self, z):
         A = torch.zeros(
-            self.latent_dims, self.latent_dims, device=z[0].device
+            self.latent_dimensions, self.latent_dimensions, device=z[0].device
         )  # initialize the cross-covariance matrix
         B = torch.zeros(
-            self.latent_dims, self.latent_dims, device=z[0].device
+            self.latent_dimensions, self.latent_dimensions, device=z[0].device
         )  # initialize the auto-covariance matrix
         for i, zi in enumerate(z):
             for j, zj in enumerate(z):
                 if i == j:
                     B += torch.cov(zi.T)  # add the auto-covariance of each view to B
                 else:
                     A += torch.cov(torch.hstack((zi, zj)).T)[
-                        self.latent_dims :, : self.latent_dims
+                        self.latent_dimensions :, : self.latent_dimensions
                     ]  # add the cross-covariance of each pair of views to A
         return A / len(z), B / len(
             z
         )  # return the normalized matrices (divided by the number of views)
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_gh.py` & `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_gh.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 from ._dcca_ey import DCCA_EY
 
 
 class DCCA_GH(DCCA_EY):
     def get_AB(self, z):
         A = torch.zeros(
-            self.latent_dims, self.latent_dims, device=z[0].device
+            self.latent_dimensions, self.latent_dimensions, device=z[0].device
         )  # initialize the cross-covariance matrix
         B = torch.zeros(
-            self.latent_dims, self.latent_dims, device=z[0].device
+            self.latent_dimensions, self.latent_dimensions, device=z[0].device
         )  # initialize the auto-covariance matrix
         for i, zi in enumerate(z):
             for j, zj in enumerate(z):
                 if i == j:
                     B += torch.cov(zi.T)  # add the auto-covariance of each view to B
                 A += torch.cov(torch.hstack((zi, zj)).T)[
-                    self.latent_dims :, : self.latent_dims
+                    self.latent_dimensions :, : self.latent_dimensions
                 ]  # add the cross-covariance of each pair of views to A
         return A / len(z), B / len(
             z
         )  # return the normalized matrices (divided by the number of views)
 
     def loss(self, views, **kwargs):
         z = self(views)
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_noi.py` & `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_noi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from ..objectives import _mat_pow
+from ..objectives import inv_sqrtm
 from ._dcca import DCCA
 
 
 class DCCA_NOI(DCCA):
     """
     A class used to fit a DCCA model by non-linear orthogonal iterations
 
@@ -13,41 +13,45 @@
     ----------
     Wang, Weiran, et al. "Stochastic optimization for deep CCA via nonlinear orthogonal iterations." 2015 53rd Annual Allerton Conference on Communication, Control, and Computing (Allerton). IEEE, 2015.
 
     """
 
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         N: int,
         encoders=None,
         r: float = 0,
         rho: float = 0.2,
         eps: float = 1e-9,
         shared_target: bool = False,
         **kwargs,
     ):
         super().__init__(
-            latent_dims=latent_dims, encoders=encoders, r=r, eps=eps, **kwargs
+            latent_dimensions=latent_dimensions,
+            encoders=encoders,
+            r=r,
+            eps=eps,
+            **kwargs,
         )
         self.N = N
         self.covs = None
         if rho < 0 or rho > 1:
             raise ValueError(f"rho should be between 0 and 1. rho={rho}")
         self.eps = eps
         self.rho = rho
         self.shared_target = shared_target
         self.mse = torch.nn.MSELoss(reduction="sum")
-        self.rand = torch.rand(N, self.latent_dims)
+        self.rand = torch.rand(N, self.latent_dimensions)
 
     def loss(self, views, **kwargs):
         z = self(views)
         z_copy = [z_.detach().clone() for z_ in z]
         self._update_covariances(z_copy, train=self.training)
-        covariance_inv = [_mat_pow(cov, -0.5, self.eps) for cov in self.covs]
+        covariance_inv = [inv_sqrtm(cov, self.eps) for cov in self.covs]
         preds = [z_ @ covariance_inv[i] for i, z_ in enumerate(z_copy)]
         loss = self.mse(z[0], preds[1]) + self.mse(z[1], preds[0])
         self.covs = [cov.detach() for cov in self.covs]
         return {"objective": loss}
 
     def _update_covariances(self, z, train=True):
         b = z[0].shape[0]
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_sdl.py` & `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_sdl.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,39 +12,42 @@
     ----------
     Chang, Xiaobin, Tao Xiang, and Timothy M. Hospedales. "Scalable and effective deep CCA via soft decorrelation." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2018.
 
     """
 
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         N: int,
         encoders=None,
         r: float = 0,
         rho: float = 0.2,
         eps: float = 1e-5,
         shared_target: bool = False,
         lam=0.5,
         **kwargs
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             N=N,
             encoders=encoders,
             r=r,
             rho=rho,
             eps=eps,
             shared_target=shared_target,
             **kwargs
         )
         self.c = None
         self.cross_cov = None
         self.lam = lam
         self.bns = torch.nn.ModuleList(
-            [torch.nn.BatchNorm1d(latent_dims, affine=False) for _ in self.encoders]
+            [
+                torch.nn.BatchNorm1d(latent_dimensions, affine=False)
+                for _ in self.encoders
+            ]
         )
 
     def forward(self, views, **kwargs):
         z = []
         for i, (encoder, bn) in enumerate(zip(self.encoders, self.bns)):
             z.append(bn(encoder(views[i])))
         return z
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dtcca.py` & `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dgcca.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import Iterable
-
-import numpy as np
-
-from ...models import TCCA
-from .. import objectives
 from ._dcca import DCCA
+from .. import objectives
 
 
-class DTCCA(DCCA):
+class DGCCA(DCCA):
     """
-    A class used to fit a DTCCA model.
+    A class used to fit a DGCCA model.
 
-    Is just a thin wrapper round DCCA with the DTCCA objective and a TCCA post-processing
+    Is just a thin wrapper round DCCA with the DGCCA objective
 
     References
     ----------
-    Wong, Hok Shing, et al. "Deep Tensor CCA for Multi-view Learning." IEEE Transactions on Big Data (2021).
+
 
     """
 
     def __init__(
-        self, latent_dims: int, encoders=None, r: float = 0, eps: float = 1e-5, **kwargs
+        self,
+        latent_dimensions: int,
+        encoders=None,
+        r: float = 0,
+        eps: float = 1e-5,
+        **kwargs
     ):
-        # Call the parent class constructor with the DTCCA objective function
+        # Call the parent class constructor with the DGCCA objective function
         super().__init__(
-            latent_dims=latent_dims,
-            objective=objectives.TCCA,
+            latent_dimensions=latent_dimensions,
+            objective=objectives.GCCA,
             encoders=encoders,
             r=r,
             eps=eps,
             **kwargs
         )
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_base.py` & `cca_zoo-2.0.1/cca_zoo/deep/_generative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_dccae.py` & `cca_zoo-2.0.1/cca_zoo/deep/_generative/_dccae.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,40 +13,40 @@
     ----------
     Wang, Weiran, et al. "On deep multi-view representation learning." International conference on machine learning. PMLR, 2015.
 
     """
 
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         objective=objectives.MCCA,
         encoders=None,
         decoders=None,
         r: float = 0,
         eps: float = 1e-5,
         lam=0.5,
         latent_dropout=0,
         img_dim=None,
         recon_loss_type="mse",
         **kwargs,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             objective=objective,
             encoders=encoders,
             r=r,
             eps=eps,
             **kwargs,
         )
         self.img_dim = img_dim
         self.decoders = torch.nn.ModuleList(decoders)
         if lam < 0 or lam > 1:
             raise ValueError(f"lam should be between 0 and 1. rho={lam}")
         self.lam = lam
-        self.objective = objective(latent_dims, r=r, eps=eps)
+        self.objective = objective(latent_dimensions, r=r, eps=eps)
         self.latent_dropout = torch.nn.Dropout(p=latent_dropout)
         self.recon_loss_type = recon_loss_type
 
     def forward(self, views, **kwargs):
         """
         Forward method for the model. Outputs latent encoding for each view
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_dvcca.py` & `cca_zoo-2.0.1/cca_zoo/deep/_generative/_dvcca.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,24 @@
     https: // arxiv.org / pdf / 1610.03454.pdf
     https: // github.com / pytorch / examples / blob / master / vae / main.py
 
     """
 
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         encoders=None,
         decoders=None,
         private_encoders: Iterable = None,
         latent_dropout=0,
         img_dim=None,
         recon_loss_type="mse",
         **kwargs,
     ):
-        super().__init__(latent_dims=latent_dims, **kwargs)
+        super().__init__(latent_dimensions=latent_dimensions, **kwargs)
         self.img_dim = img_dim
         self.latent_dropout = torch.nn.Dropout(p=latent_dropout)
         self.encoders = torch.nn.ModuleList(encoders)
         self.decoders = torch.nn.ModuleList(decoders)
         if private_encoders:
             self.private_encoders = torch.nn.ModuleList(private_encoders)
         else:
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_splitae.py` & `cca_zoo-2.0.1/cca_zoo/deep/_generative/_splitae.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,29 +13,29 @@
     ----------
     Ngiam, Jiquan, et al. "Multimodal deep learning." ICML. 2011.
 
     """
 
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         encoder=Encoder,
         decoders=None,
         latent_dropout=0,
         recon_loss_type="mse",
         img_dim=None,
         **kwargs
     ):
         """
 
-        :param latent_dims: # latent dimensions
+        :param latent_dimensions: # latent dimensions
         :param encoder: list of encoder networks
         :param decoders:  list of decoder networks
         """
-        super().__init__(latent_dims=latent_dims, **kwargs)
+        super().__init__(latent_dimensions=latent_dimensions, **kwargs)
         self.img_dim = img_dim
         self.encoder = encoder
         self.decoders = torch.nn.ModuleList(decoders)
         self.latent_dropout = torch.nn.Dropout(p=latent_dropout)
         self.recon_loss_type = recon_loss_type
 
     def forward(self, views, **kwargs):
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/architectures.py` & `cca_zoo-2.0.1/cca_zoo/deep/architectures.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 
 import torch
 from torch import nn
 
 
 class _BaseEncoder(torch.nn.Module):
     @abstractmethod
-    def __init__(self, latent_dims: int, variational: bool = False):
+    def __init__(self, latent_dimensions: int, variational: bool = False):
         super(_BaseEncoder, self).__init__()
         self.variational = variational
-        self.latent_dims = latent_dims
+        self.latent_dimensions = latent_dimensions
 
     @abstractmethod
     def forward(self, x):
         pass
 
 
 class _BaseDecoder(torch.nn.Module):
     @abstractmethod
-    def __init__(self, latent_dims: int):
+    def __init__(self, latent_dimensions: int):
         super(_BaseDecoder, self).__init__()
-        self.latent_dims = latent_dims
+        self.latent_dimensions = latent_dimensions
 
     @abstractmethod
     def forward(self, x):
         pass
 
 
 class Encoder(_BaseEncoder):
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         variational: bool = False,
         feature_size: int = 784,
         layer_sizes: tuple = None,
         activation=nn.LeakyReLU(),
         dropout=0,
     ):
-        super(Encoder, self).__init__(latent_dims, variational=variational)
+        super(Encoder, self).__init__(latent_dimensions, variational=variational)
         if layer_sizes is None:
             layer_sizes = (128,)
-        layer_sizes = (feature_size,) + layer_sizes + (latent_dims,)
+        layer_sizes = (feature_size,) + layer_sizes + (latent_dimensions,)
         layers = []
         # other layers
         for l_id in range(len(layer_sizes) - 2):
             layers.append(
                 torch.nn.Sequential(
                     nn.Dropout(p=dropout),
                     torch.nn.Linear(layer_sizes[l_id], layer_sizes[l_id + 1]),
@@ -77,24 +77,24 @@
             x = self.fc(x)
             return x
 
 
 class Decoder(_BaseDecoder):
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         feature_size: int = 784,
         layer_sizes: tuple = None,
         activation=nn.LeakyReLU(),
         dropout=0,
     ):
-        super(Decoder, self).__init__(latent_dims)
+        super(Decoder, self).__init__(latent_dimensions)
         if layer_sizes is None:
             layer_sizes = (128,)
-        layer_sizes = (latent_dims,) + layer_sizes + (feature_size,)
+        layer_sizes = (latent_dimensions,) + layer_sizes + (feature_size,)
         layers = []
         for l_id in range(len(layer_sizes) - 1):
             layers.append(
                 torch.nn.Sequential(
                     nn.Dropout(p=dropout),
                     torch.nn.Linear(layer_sizes[l_id], layer_sizes[l_id + 1]),
                     activation,
@@ -106,25 +106,25 @@
         x = self.layers(x)
         return x
 
 
 class CNNEncoder(_BaseEncoder):
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         variational: bool = False,
         feature_size: Iterable = (28, 28),
         channels: tuple = None,
         kernel_sizes: tuple = None,
         stride: tuple = None,
         padding: tuple = None,
         activation=nn.LeakyReLU(),
         dropout=0,
     ):
-        super(CNNEncoder, self).__init__(latent_dims, variational=variational)
+        super(CNNEncoder, self).__init__(latent_dimensions, variational=variational)
         if channels is None:
             channels = (1, 1)
         if kernel_sizes is None:
             kernel_sizes = (5,) * (len(channels))
         if stride is None:
             stride = (1,) * (len(channels))
         if padding is None:
@@ -151,28 +151,31 @@
             current_size = current_size
             current_channels = channels[l_id]
 
         if self.variational:
             self.fc_mu = torch.nn.Sequential(
                 nn.Dropout(p=dropout),
                 torch.nn.Linear(
-                    int(current_size * current_size * current_channels), latent_dims
+                    int(current_size * current_size * current_channels),
+                    latent_dimensions,
                 ),
             )
             self.fc_var = torch.nn.Sequential(
                 nn.Dropout(p=dropout),
                 torch.nn.Linear(
-                    int(current_size * current_size * current_channels), latent_dims
+                    int(current_size * current_size * current_channels),
+                    latent_dimensions,
                 ),
             )
         else:
             self.fc = torch.nn.Sequential(
                 nn.Dropout(p=dropout),
                 torch.nn.Linear(
-                    int(current_size * current_size * current_channels), latent_dims
+                    int(current_size * current_size * current_channels),
+                    latent_dimensions,
                 ),
             )
         self.conv_layers = torch.nn.Sequential(*conv_layers)
 
     def forward(self, x):
         x = self.conv_layers(x)
         x = x.reshape((x.shape[0], -1))
@@ -184,24 +187,24 @@
             x = self.fc(x)
             return x
 
 
 class CNNDecoder(_BaseDecoder):
     def __init__(
         self,
-        latent_dims: int,
+        latent_dimensions: int,
         feature_size: Iterable = (28, 28),
         channels: tuple = None,
         kernel_sizes=None,
         strides=None,
         paddings=None,
         activation=nn.LeakyReLU(),
         dropout=0,
     ):
-        super(CNNDecoder, self).__init__(latent_dims)
+        super(CNNDecoder, self).__init__(latent_dimensions)
         if channels is None:
             channels = (1, 1)
         if kernel_sizes is None:
             kernel_sizes = (5,) * len(channels)
         if strides is None:
             strides = (1,) * len(channels)
         if paddings is None:
@@ -230,15 +233,15 @@
             current_channels = channel
 
         # reverse layers as constructed in reverse
         self.conv_layers = torch.nn.Sequential(*conv_layers[::-1])
         self.fc_layer = torch.nn.Sequential(
             nn.Dropout(p=dropout),
             torch.nn.Linear(
-                latent_dims, int(current_size * current_size * current_channels)
+                latent_dimensions, int(current_size * current_size * current_channels)
             ),
             activation,
         )
 
     def forward(self, x):
         x = self.fc_layer(x)
         x = x.reshape((x.shape[0], self.conv_layers[0][0].in_channels, -1))
@@ -251,35 +254,37 @@
             )
         )
         x = self.conv_layers(x)
         return x
 
 
 class LinearEncoder(_BaseEncoder):
-    def __init__(self, latent_dims: int, feature_size: int, variational: bool = False):
-        super(LinearEncoder, self).__init__(latent_dims, variational=variational)
+    def __init__(
+        self, latent_dimensions: int, feature_size: int, variational: bool = False
+    ):
+        super(LinearEncoder, self).__init__(latent_dimensions, variational=variational)
         self.variational = variational
 
         if self.variational:
-            self.fc_mu = torch.nn.Linear(feature_size, latent_dims)
-            self.fc_var = torch.nn.Linear(feature_size, latent_dims)
+            self.fc_mu = torch.nn.Linear(feature_size, latent_dimensions)
+            self.fc_var = torch.nn.Linear(feature_size, latent_dimensions)
         else:
-            self.fc = torch.nn.Linear(feature_size, latent_dims)
+            self.fc = torch.nn.Linear(feature_size, latent_dimensions)
 
     def forward(self, x):
         if self.variational:
             mu = self.fc_mu(x)
             logvar = self.fc_var(x)
             return mu, logvar
         else:
             x = self.fc(x)
             return x
 
 
 class LinearDecoder(_BaseDecoder):
-    def __init__(self, latent_dims: int, feature_size: int):
-        super(LinearDecoder, self).__init__(latent_dims)
-        self.linear = torch.nn.Linear(latent_dims, feature_size)
+    def __init__(self, latent_dimensions: int, feature_size: int):
+        super(LinearDecoder, self).__init__(latent_dimensions)
+        self.linear = torch.nn.Linear(latent_dimensions, feature_size)
 
     def forward(self, x):
         out = self.linear(x)
         return out
```

### Comparing `cca_zoo-2.0.0/cca_zoo/deepmodels/objectives.py` & `cca_zoo-2.0.1/cca_zoo/deep/objectives.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 import tensorly as tl
 import torch
 from tensorly.cp_tensor import cp_to_tensor
 from tensorly.decomposition import parafac
 
 
-def _mat_pow(mat, pow_, epsilon):
-    # Computing matrix to the power of pow (pow can be negative as well)
-    [D, V] = torch.linalg.eigh(mat)
-    mat_pow = V @ torch.diag((D + epsilon).pow(pow_)) @ V.T
-    mat_pow[mat_pow != mat_pow] = epsilon  # For stability
-    return mat_pow
+def inv_sqrtm(A, eps=1e-9):
+    """Compute the inverse square-root of a positive definite matrix."""
+    # Perform eigendecomposition of covariance matrix
+    U, S, V = torch.svd(A)
+    # Enforce positive definite by taking a torch max() with eps
+    S = torch.max(S, torch.tensor(eps, device=S.device))
+    # Calculate inverse square-root
+    inv_sqrt_S = torch.diag_embed(torch.pow(S, -0.5))
+    # Calculate inverse square-root matrix
+    B = torch.matmul(torch.matmul(U, inv_sqrt_S), V.transpose(-1, -2))
+    return B
 
 
 def _demean(views):
     return tuple([view - view.mean(dim=0) for view in views])
 
 
 class MCCA:
@@ -33,48 +38,61 @@
         the number of latent dimensions
         :param eps: an epsilon parameter used in some operations
         """
         self.latent_dims = latent_dims
         self.r = r
         self.eps = eps
 
-    def loss(self, views):
-        # Subtract the mean from each output
-        views = _demean(views)
-
+    def C(self, views):
         # Concatenate all views and from this get the cross-covariance matrix
         all_views = torch.cat(views, dim=1)
         C = torch.cov(all_views.T)
+        C = C - torch.block_diag(*[torch.cov(view.T) for view in views])
+        return C / len(views)
 
+    def D(self, views):
         # Get the block covariance matrix placing Xi^TX_i on the diagonal
         D = torch.block_diag(
             *[
                 (1 - self.r) * torch.cov(view.T)
                 + self.r * torch.eye(view.shape[1], device=view.device)
                 for i, view in enumerate(views)
             ]
         )
+        return D / len(views)
+
+    def correlation(self, views):
+        # Subtract the mean from each output
+        views = _demean(views)
 
-        C = C - torch.block_diag(*[torch.cov(view.T) for view in views]) + D
+        C = self.C(views)
+        D = self.D(views)
 
-        R = _mat_pow(D, -0.5, self.eps)
+        C = C + D
+
+        R = inv_sqrtm(D, self.eps)
 
         # In MCCA our eigenvalue problem Cv = lambda Dv
         C_whitened = R @ C @ R.T
 
         eigvals = torch.linalg.eigvalsh(C_whitened)
 
         # Sort eigenvalues so lviewest first
         idx = torch.argsort(eigvals, descending=True)
 
         eigvals = eigvals[idx[: self.latent_dims]]
 
+        return eigvals
+
+    def loss(self, views):
+        eigvals = self.correlation(views)
+
         # leaky relu encourages the gradient to be driven by positively correlated dimensions while also encouraging
         # dimensions associated with spurious negative correlations to become more positive
-        eigvals = torch.nn.LeakyReLU()(eigvals[torch.gt(eigvals, 0)] - 1)
+        eigvals = torch.nn.LeakyReLU()(eigvals[torch.gt(eigvals, 0)])
 
         corr = eigvals.sum()
 
         return -corr
 
 
 class GCCA:
@@ -93,37 +111,43 @@
         the number of latent dimensions
         :param eps: an epsilon parameter used in some operations
         """
         self.latent_dims = latent_dims
         self.r = r
         self.eps = eps
 
-    def loss(self, views):
+    def Q(self, views):
+        eigen_views = [
+            view @ torch.linalg.inv(torch.cov(view.T)) @ view.T for view in views
+        ]
+        Q = torch.stack(eigen_views, dim=0).sum(dim=0)
+        return Q
+
+    def correlation(self, views):
         # https: // www.uta.edu / math / _docs / preprint / 2014 / rep2014_04.pdf
 
         # H is n_views * n_samples * k
         views = _demean(views)
 
-        eigen_views = [
-            view @ _mat_pow(torch.cov(view.T), -1, self.eps) @ view.T for view in views
-        ]
+        Q = self.Q(views)
 
-        Q = torch.stack(eigen_views, dim=0).sum(dim=0)
         eigvals = torch.linalg.eigvalsh(Q)
 
         idx = torch.argsort(eigvals, descending=True)
 
         eigvals = eigvals[idx[: self.latent_dims]]
 
         # leaky relu encourages the gradient to be driven by positively correlated dimensions while also encouraging
         # dimensions associated with spurious negative correlations to become more positive
-        eigvals = torch.nn.LeakyReLU()(eigvals[torch.gt(eigvals, 0)] - 1)
+        eigvals = torch.nn.LeakyReLU()(eigvals)
+        return eigvals
 
+    def loss(self, views):
+        eigvals = self.correlation(views)
         corr = eigvals.sum()
-
         return -corr
 
 
 # Original work Copyright (c) 2016 Vahid Noroozi
 # Modified work Copyright 2019 Zhanghao Wu
 
 # Permission is hereby granted, free of chviewe, to any person obtaining a copy
@@ -149,15 +173,15 @@
         :param r: regularisation as in regularized CCA. Makes the problem well posed when batch size is similar to the number of latent dimensions
         :param eps: an epsilon parameter used in some operations
         """
         self.latent_dims = latent_dims
         self.r = r
         self.eps = eps
 
-    def loss(self, views):
+    def correlation(self, views):
         o1 = views[0].shape[1]
         o2 = views[1].shape[1]
 
         n = views[0].shape[0]
 
         views = _demean(views)
 
@@ -167,28 +191,31 @@
         SigmaHat11 = torch.cov(views[0].T) + self.r * torch.eye(
             o1, device=views[0].device
         )
         SigmaHat22 = torch.cov(views[1].T) + self.r * torch.eye(
             o2, device=views[1].device
         )
 
-        SigmaHat11RootInv = _mat_pow(SigmaHat11, -0.5, self.eps)
-        SigmaHat22RootInv = _mat_pow(SigmaHat22, -0.5, self.eps)
+        SigmaHat11RootInv = inv_sqrtm(SigmaHat11, self.eps)
+        SigmaHat22RootInv = inv_sqrtm(SigmaHat22, self.eps)
 
         Tval = SigmaHat11RootInv @ SigmaHat12 @ SigmaHat22RootInv
         trace_TT = Tval.T @ Tval
         eigvals = torch.linalg.eigvalsh(trace_TT)
 
+        return eigvals
+
+    def loss(self, views):
+        eigvals = self.correlation(views)
+
         # leaky relu encourages the gradient to be driven by positively correlated dimensions while also encouraging
         # dimensions associated with spurious negative correlations to become more positive
-        eigvals = eigvals[torch.gt(eigvals, self.eps)]
+        eigvals = torch.nn.LeakyReLU()(eigvals[torch.gt(eigvals, 0)])
 
-        corr = torch.sum(torch.sqrt(eigvals))
-
-        return -corr
+        return -eigvals.sum()
 
 
 class TCCA:
     """
     Differentiable TCCA Loss.
 
     """
@@ -201,17 +228,15 @@
     def loss(self, views):
         views = _demean(views)
         covs = [
             (1 - self.r) * torch.cov(view.T)
             + self.r * torch.eye(view.size(1), device=view.device)
             for view in views
         ]
-        whitened_z = [
-            view @ _mat_pow(cov, -0.5, self.eps) for view, cov in zip(views, covs)
-        ]
+        whitened_z = [view @ inv_sqrtm(cov, self.eps) for view, cov in zip(views, covs)]
         # The idea here is to form a matrix with M dimensions one for each view where at index
         # M[p_i,p_j,p_k...] we have the sum over n samples of the product of the pth feature of the
         # ith, jth, kth view etc.
         for i, el in enumerate(whitened_z):
             # To achieve this we start with the first view so M is nxp.
             if i == 0:
                 M = el
```

### Comparing `cca_zoo-2.0.0/cca_zoo/model_selection/_search.py` & `cca_zoo-2.0.1/cca_zoo/model_selection/_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
 
 class GridSearchCV(BaseSearchCV):
     """
 
     :Example:
     >>> from cca_zoo.model_selection import GridSearchCV
-    >>> from cca_zoo.models import MCCA
+    >>> from cca_zoo.classical import MCCA
     >>> X1 = [[0, 0, 1], [1, 0, 0], [2, 2, 2], [3, 5, 4]]
     >>> X2 = [[0.1, -0.2], [0.9, 1.1], [6.2, 5.9], [11.9, 12.3]]
     >>> X3 = [[0, 1, 0], [1, 9, 0], [4, 3, 3,], [12, 8, 10]]
     >>> model = MCCA()
     >>> params = {'c': [[0.1, 0.2], [0.3, 0.4], 0.1]}
     >>> GridSearchCV(model,param_grid=params, cv=3).fit([X1,X2,X3]).best_estimator_.c
     [0.1, 0.3, 0.1]
@@ -214,15 +214,15 @@
 
 
 class RandomizedSearchCV(BaseSearchCV):
     """
 
     :Example:
     >>> from cca_zoo.model_selection import RandomizedSearchCV
-    >>> from cca_zoo.models import MCCA
+    >>> from cca_zoo.classical import MCCA
     >>> from sklearn._utils.fixes import loguniform
     >>> X1 = [[0, 0, 1], [1, 0, 0], [2, 2, 2], [3, 5, 4]]
     >>> X2 = [[0.1, -0.2], [0.9, 1.1], [6.2, 5.9], [11.9, 12.3]]
     >>> X3 = [[0, 1, 0], [1, 9, 0], [4, 3, 3,], [12, 8, 10]]
     >>> model = MCCA()
     >>> params = {'c': [loguniform(1e-4, 1e0), loguniform(1e-4, 1e0), [0.1]]}
     >>> def scorer(estimator, views):
```

### Comparing `cca_zoo-2.0.0/cca_zoo/model_selection/_validation.py` & `cca_zoo-2.0.1/cca_zoo/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.0/cca_zoo/models/__init__.py` & `cca_zoo-2.0.1/cca_zoo/classical/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._mcca import MCCA, CCA, PLS, rCCA
+from ._mcca import MCCA, CCA, PLS, rCCA, MPLS
 from ._gcca import GCCA
 from ._grcca import GRCCA
 from ._ncca import NCCA
 from ._partialcca import PartialCCA
 from ._prcca import PRCCA
 from ._tcca import TCCA
 from ._pcacca import PCACCA
@@ -19,14 +19,16 @@
     "PLS",
     "PRCCA",
     "KTCCA",
     "TCCA",
     "PartialCCA",
     "rCCA",
     "PCACCA",
+    "KGCCA",
+    "MPLS",
 ]
 
 # if pytorch-lightning is installed then import ._iterative
 
 try:
     from ._iterative import (
         CCAEY,
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_base.py` & `cca_zoo-2.0.1/cca_zoo/classical/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import numpy as np
 from sklearn.base import BaseEstimator, MultiOutputMixin, RegressorMixin
 from sklearn.utils.validation import FLOAT_DTYPES, check_is_fitted, check_random_state
 
 
 class BaseModel(BaseEstimator, MultiOutputMixin, RegressorMixin):
     """
-    A base class for multivariate latent variable models.
+    A base class for multivariate latent variable classical.
 
     This class implements common methods and attributes for fitting and transforming
-    multiple views of data using latent variable models. It inherits from scikit-learn's
+    multiple views of data using latent variable classical. It inherits from scikit-learn's
     BaseEstimator, MultiOutputMixin and RegressorMixin classes.
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to fit. Default is 1.
     copy_data : bool, optional
         Whether to copy the data. Default is True.
     accept_sparse : bool, optional
         Whether to accept sparse data. Default is False.
     random_state : int, RandomState instance or None, optional (default=None)
         Pass an int for reproducible output across multiple function calls.
@@ -33,20 +33,20 @@
     n_features_ : list of int
         Number of features for each view.
 
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         accept_sparse=False,
         random_state: Union[int, np.random.RandomState] = None,
     ):
-        self.latent_dims = latent_dims
+        self.latent_dimensions = latent_dimensions
         self.copy_data = copy_data
         self.accept_sparse = accept_sparse
         self.random_state = check_random_state(random_state)
         self.dtypes = FLOAT_DTYPES
 
     def _validate_data(
         self,
@@ -54,17 +54,19 @@
     ):
         if not all(view.shape[0] == views[0].shape[0] for view in views):
             raise ValueError("All views must have the same number of samples")
         if not all(view.ndim == 2 for view in views):
             raise ValueError("All views must have 2 dimensions")
         if not all(view.dtype in self.dtypes for view in views):
             raise ValueError("All views must have dtype of {}.".format(self.dtypes))
-        if not all(view.shape[1] >= self.latent_dims for view in views):
+        if not all(view.shape[1] >= self.latent_dimensions for view in views):
             raise ValueError(
-                "All views must have at least {} features.".format(self.latent_dims)
+                "All views must have at least {} features.".format(
+                    self.latent_dimensions
+                )
             )
         self.n_views_ = len(views)
         self.n_features_ = [view.shape[1] for view in views]
         self.n_samples_ = views[0].shape[0]
 
     def _check_params(self):
         """
@@ -133,25 +135,29 @@
         Parameters
         ----------
         views : list/tuple of numpy arrays or array likes with the same number of rows (samples)
         kwargs : any additional keyword arguments required by the given model
 
         Returns
         -------
-        pairwise_correlations : numpy array of shape (n_views, n_views, latent_dims)
+        pairwise_correlations : numpy array of shape (n_views, n_views, latent_dimensions)
 
         """
         transformed_views = self.transform(views, **kwargs)
         all_corrs = []
         for x, y in itertools.product(transformed_views, repeat=2):
             all_corrs.append(
-                np.diag(np.corrcoef(x.T, y.T)[: self.latent_dims, self.latent_dims :])
+                np.diag(
+                    np.corrcoef(x.T, y.T)[
+                        : self.latent_dimensions, self.latent_dimensions :
+                    ]
+                )
             )
         all_corrs = np.array(all_corrs).reshape(
-            (self.n_views_, self.n_views_, self.latent_dims)
+            (self.n_views_, self.n_views_, self.latent_dimensions)
         )
         return all_corrs
 
     def score(self, views: Iterable[np.ndarray], y=None, **kwargs):
         """
         Returns the average pairwise correlation between the views
 
@@ -166,17 +172,18 @@
         score : float
 
 
         """
         # by default return the average pairwise correlation in each dimension (for 2 views just the correlation)
         pair_corrs = self.pairwise_correlations(views, **kwargs)
         # sum all the pairwise correlations for each dimension. Subtract the self correlations. Divide by the number of views. Gives average correlation
-        dim_corrs = (
-            pair_corrs.sum(axis=tuple(range(pair_corrs.ndim - 1))) - self.n_views_
-        ) / (self.n_views_**2 - self.n_views_)
+        dim_corrs = np.sum(pair_corrs, axis=(0, 1)) - pair_corrs.shape[0]
+        # number of pairs is n_views choose 2
+        num_pairs = (self.n_views_ * (self.n_views_ - 1)) / 2
+        dim_corrs = dim_corrs / (2 * num_pairs)
         return dim_corrs
 
     def factor_loadings(self, views: Iterable[np.ndarray], normalize=True, **kwargs):
         """
         Returns the factor loadings for each view
 
         Parameters
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_dummy.py` & `cca_zoo-2.0.1/cca_zoo/classical/_dummy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from typing import Iterable
 
 import numpy as np
 
-from cca_zoo.models._base import BaseModel
+from cca_zoo.classical._base import BaseModel
 
 
 class DummyCCA(BaseModel):
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         accept_sparse=None,
         uniform=False,
     ):
         if accept_sparse is None:
             accept_sparse = ["csc", "csr"]
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             accept_sparse=accept_sparse,
             random_state=random_state,
         )
         self.uniform = uniform
 
     def fit(self, views: Iterable[np.ndarray], y=None, **kwargs):
         self._validate_data(views)
         if self.uniform:
             self.weights = [
-                np.ones((view.shape[1], self.latent_dims)) for view in views
+                np.ones((view.shape[1], self.latent_dimensions)) for view in views
             ]
         else:
             self.weights = [
-                self.random_state.normal(0, 1, size=(view.shape[1], self.latent_dims))
+                self.random_state.normal(
+                    0, 1, size=(view.shape[1], self.latent_dimensions)
+                )
                 for view in views
             ]
         self.normalize_weights(views)
         return self
 
     def normalize_weights(self, views):
         self.weights = [
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_gcca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_gcca.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Union
 
 import numpy as np
 
-from cca_zoo.models._mcca import MCCA
+from cca_zoo.classical._mcca import MCCA
 from cca_zoo.utils.check_values import _process_parameter
 
 
 class GCCA(MCCA):
     r"""
     A class used to fit GCCA model. This model extends CCA to more than two views by optimizing the sum of correlations with a shared auxiliary vector.
 
@@ -25,36 +25,36 @@
 
     References
     ----------
     Tenenhaus, Arthur, and Michel Tenenhaus. "Regularized generalized canonical correlation analysis." Psychometrika 76.2 (2011): 257.
 
     Examples
     --------
-    >>> from cca_zoo.models import GCCA
+    >>> from cca_zoo.classical import GCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = GCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
     array([0.97229856])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         c: Union[Iterable[float], float] = None,
         view_weights: Iterable[float] = None,
         eps: float = 1e-6,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             accept_sparse=["csc", "csr"],
             random_state=random_state,
             c=c,
             eps=eps,
             pca=False,
         )
@@ -100,12 +100,13 @@
         return Q
 
     def D(self, views, **kwargs):
         return None
 
     def _weights(self, eigvals, eigvecs, views, **kwargs):
         self.weights = [
-            np.linalg.pinv(view) @ eigvecs[:, : self.latent_dims] for view in views
+            np.linalg.pinv(view) @ eigvecs[:, : self.latent_dimensions]
+            for view in views
         ]
 
     def _more_tags(self):
         return {"multiview": True}
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_grcca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_grcca.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import warnings
 from typing import Iterable
 
 import numpy as np
 
-from cca_zoo.models._mcca import MCCA
+from cca_zoo.classical._mcca import MCCA
 from cca_zoo.utils import _process_parameter
 
 
 class GRCCA(MCCA):
     """
     Grouped Regularized Canonical Correlation Analysis
 
     Parameters
     ----------
-    latent_dims : int, default=1
+    latent_dimensions : int, default=1
         Number of latent dimensions to use
     copy_data : bool, default=True
         Whether to copy the data
     random_state : int, default=None
         Random state for initialisation
     eps : float, default=1e-3
         Tolerance for convergence
@@ -30,23 +30,23 @@
     References
     ----------
     Tuzhilina, Elena, Leonardo Tozzi, and Trevor Hastie. "Canonical correlation analysis in high dimensions with structured regularization." Statistical Modelling (2021): 1471082X211041033.
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         eps=1e-3,
         c: float = 0,
         mu: float = 0,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             eps=eps,
             c=c,
             pca=False,
         )
         self.mu = mu
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/__init__.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_altmaxvar.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_altmaxvar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Iterable, Union
 
 import numpy as np
 import torch
 from skprox.proximal_operators import _proximal_operators
 
-from cca_zoo.models._iterative._base import BaseIterative, BaseLoop
+from cca_zoo.classical._iterative._base import BaseIterative, BaseLoop
 from cca_zoo.utils import _process_parameter
 
 
 class AltMaxVar(BaseIterative):
     def __init__(
         self,
-        latent_dims=1,
+        latent_dimensions=1,
         copy_data=True,
         random_state=None,
         epochs=100,
         tol=1e-3,
         proximal="L1",
         positive=False,
         tau: Union[Iterable[float], float] = None,
@@ -24,15 +24,15 @@
         learning_rate=0.1,
         T=100,
         convergence_checking=None,
         track=None,
         verbose=False,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             tol=tol,
             epochs=epochs,
             convergence_checking=convergence_checking,
             track=track,
             verbose=verbose,
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_base.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from pytorch_lightning.callbacks import Callback, EarlyStopping
 from torch import Tensor
 from torch.utils import data
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from cca_zoo.data.deep import NumpyDataset
-from cca_zoo.models import MCCA, rCCA
-from cca_zoo.models._base import BaseModel
-from cca_zoo.models._dummy import DummyCCA
+from cca_zoo.classical import MCCA, rCCA
+from cca_zoo.classical._base import BaseModel
+from cca_zoo.classical._dummy import DummyCCA
 
 # Default Trainer kwargs
 DEFAULT_TRAINER_KWARGS = dict(
     enable_checkpointing=False,
     logger=False,
     enable_model_summary=False,
     enable_progress_bar=False,
@@ -27,15 +27,15 @@
     num_workers=0, pin_memory=True, drop_last=False, shuffle=False
 )
 
 
 class BaseIterative(BaseModel):
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         tol=1e-3,
         deflation="cca",
         accept_sparse=None,
         batch_size=None,
         dataloader_kwargs=None,
@@ -47,15 +47,15 @@
         trainer_kwargs=None,
         convergence_checking=None,
         patience=10,
         track=None,
         verbose=False,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             accept_sparse=accept_sparse,
         )
         self.tol = tol
         self.batch_size = batch_size
         self.epochs = epochs
@@ -181,25 +181,30 @@
 
         Parameters
         ----------
         views : Iterable[np.ndarray]
             The input views to initialize the CCA weights from
         """
         initializer = _default_initializer(
-            self.initialization, self.random_state, self.latent_dims
+            self.initialization, self.random_state, self.latent_dimensions
         )
         # Fit the initializer on the input views and get the weights as numpy arrays
         self.weights = initializer.fit(views).weights
         self.weights = [weights.astype(np.float32) for weights in self.weights]
 
 
 class BaseDeflation(BaseIterative, ABC):
     def _fit(self, views: Iterable[np.ndarray]):
+        # if views is a tuple then convert to a list
+        if isinstance(views, tuple):
+            views = list(views)
         # tqdm for each latent dimension
-        for k in tqdm(range(self.latent_dims), desc="Latent Dimension", leave=False):
+        for k in tqdm(
+            range(self.latent_dimensions), desc="Latent Dimension", leave=False
+        ):
             train_dataloader, val_dataloader = self.get_dataloader(views)
             loop = self._get_module(weights=self.weights, k=k)
             # make a trainer
             trainer = pl.Trainer(
                 max_epochs=self.epochs, callbacks=self.callbacks, **self.trainer_kwargs
             )
             trainer.fit(loop, train_dataloader, val_dataloader)
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_elasticnet.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_elasticnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
 from typing import Iterable, Union
 
 import numpy as np
 import torch
 from sklearn.linear_model import ElasticNet, Lasso, Ridge, SGDRegressor
 
-from cca_zoo.models._iterative._base import BaseDeflation, BaseLoop
+from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
 from cca_zoo.utils import _process_parameter
 
 
 class ElasticCCA(BaseDeflation):
     r"""
     A class used to fit an elastic CCA model for two or more views of data.
 
@@ -25,15 +25,15 @@
 
         t^Tt=n
 
     Where :math:`\alpha_i` is the constant that multiplies the penalty terms for view i and :math:`\text{l1_ratio}` is the ratio between L1 and L2 penalties.
 
     Parameters
     ----------
-    latent_dims : int, default=1
+    latent_dimensions : int, default=1
         Number of latent dimensions to use
     copy_data : bool, default=True
         Whether to copy the data or overwrite it
     random_state : int, default=None
         Random seed for initialization
     deflation : str, default="cca"
         Whether to use CCA or PLS deflation
@@ -48,27 +48,27 @@
     stochastic : bool, default=False
         Whether to use stochastic gradient descent
     positive : bool or list of bools, default=None
         Whether to use non-negative constraints
 
     Examples
     --------
-    >>> from cca_zoo.models import ElasticCCA
+    >>> from cca_zoo.classical import ElasticCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = ElasticCCA(c=[1e-1,1e-1],l1_ratio=[0.5,0.5], random_state=0)
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.9316638])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         epochs: int = 100,
         deflation="cca",
         initialization: Union[str, callable] = "pls",
         tol: float = 1e-3,
         alpha: Union[Iterable[float], float] = None,
@@ -85,15 +85,15 @@
         self.positive = positive
         if self.positive is not None and stochastic:
             self.stochastic = False
             warnings.warn(
                 "Non negative constraints cannot be used with _stochastic regressors. Switching to _stochastic=False"
             )
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             epochs=epochs,
             deflation=deflation,
             initialization=initialization,
             tol=tol,
             random_state=random_state,
             convergence_checking=convergence_checking,
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_ey.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_ey.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Union
 
 import numpy as np
 import torch
 
-from cca_zoo.models._plsmixin import PLSMixin
-from cca_zoo.models._iterative._base import BaseGradientLoop, BaseIterative
+from cca_zoo.classical._plsmixin import PLSMixin
+from cca_zoo.classical._iterative._base import BaseGradientLoop, BaseIterative
 
 
 class CCAEY(BaseIterative):
     """
     A class used to fit Regularized CCA by Delta-EigenGame
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random state to use, by default None
     accept_sparse : bool, optional
         Whether to accept sparse data, by default None
@@ -31,33 +31,33 @@
     References
     ----------
     Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A Generalized EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         tol=1e-9,
         accept_sparse=None,
         batch_size=None,
         epochs=100,
         learning_rate=1e-1,
         initialization: Union[str, callable] = "random",
         dataloader_kwargs=None,
         optimizer_kwargs=None,
-        convergence_checking=False,
+        convergence_checking=None,
         patience=10,
-        track=False,
+        track=None,
         verbose=False,
     ):
         self.optimizer_kwargs = optimizer_kwargs
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             accept_sparse=accept_sparse,
             random_state=random_state,
             tol=tol,
             batch_size=batch_size,
             epochs=epochs,
             learning_rate=learning_rate,
@@ -74,27 +74,29 @@
     def _get_module(self, weights=None, k=None):
         return EYLoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="cca",
+            tracking=self.track,
+            convergence_checking=self.convergence_checking,
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
 class PLSEY(CCAEY, PLSMixin):
     """
     A class used to fit Regularized CCA by Delta-EigenGame
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random state to use, by default None
     accept_sparse : bool, optional
         Whether to accept sparse data, by default None
@@ -108,15 +110,15 @@
     References
     ----------
     Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A Generalized EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         tol=1e-9,
         accept_sparse=None,
         batch_size=None,
         epochs=1,
         learning_rate=1,
@@ -124,15 +126,15 @@
         dataloader_kwargs=None,
         convergence_checking=False,
         patience=10,
         track=False,
         verbose=False,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             accept_sparse=accept_sparse,
             random_state=random_state,
             tol=tol,
             batch_size=batch_size,
             epochs=epochs,
             learning_rate=learning_rate,
@@ -148,34 +150,40 @@
     def _get_module(self, weights=None, k=None):
         return EYLoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="pls",
+            tracking=self.track,
+            convergence_checking=self.convergence_checking,
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
 class EYLoop(BaseGradientLoop):
     def __init__(
         self,
         weights=None,
         k=None,
         learning_rate=1e-3,
         optimizer_kwargs=None,
         objective="cca",
+        tracking=False,
+        convergence_checking=False,
     ):
         super().__init__(
             weights=weights,
             k=k,
             learning_rate=learning_rate,
             optimizer_kwargs=optimizer_kwargs,
+            tracking=tracking,
+            convergence_checking=convergence_checking,
         )
         self.objective = objective
         self.batch_queue = []
         self.val_batch_queue = []
 
     def training_step(self, batch, batch_idx):
         # Checking if the queue has at least one batch
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_gh.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_gh.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import torch
 
-from cca_zoo.models._iterative._ey import CCAEY, EYLoop
+from cca_zoo.classical._iterative._ey import CCAEY, EYLoop
 
 
 class CCAGH(CCAEY):
     def _get_module(self, weights=None, k=None):
         return GHALoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="cca",
+            tracking=self.track,
+            convergence_checking=self.convergence_checking,
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
 class GHALoop(EYLoop):
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_gradkcca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_gradkcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 import numpy as np
 import numpy.linalg as la
 from sklearn.kernel_approximation import Nystroem
 from sklearn.metrics import pairwise_kernels
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.models._iterative._base import BaseIterative
+from cca_zoo.classical._iterative._base import BaseIterative
 from cca_zoo.utils import _process_parameter
 
 
 class GradKCCA(BaseIterative):
     """
     References
     ----------
     [1] Viivi Uurtio, Sahely Bhadra, and Juho Rousu. Large-scale sparse kernel canonical correlation analysis. In Kamalika Chaudhuri and Ruslan Salakhutdinov, editors, Proceedings of the 36th International Conference on Machine Learning, volume 97 of Proceedings of Machine Learning Research, pages 6383–6391, Long Beach, California, USA, 09–15 Jun 2019. PMLR.
 
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         scale: bool = True,
         centre=True,
         copy_data=True,
         random_state=None,
         proj: Union[Iterable[float], float] = "l1",
         kernel: Iterable[Union[float, callable]] = None,
         gamma: Iterable[float] = None,
@@ -33,15 +33,15 @@
         kernel_params: Iterable[dict] = None,
         repetitions=5,
         initialization: Union[str, callable] = "random",
         nystrom=False,
         nystrom_components=100,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             scale=scale,
             centre=centre,
             copy_data=copy_data,
             random_state=random_state,
             initialization=initialization,
         )
         self.proj = proj
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_incrementalpls.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_incrementalpls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Union
 
 import numpy as np
 
-from cca_zoo.models._iterative._base import BaseIterative
+from cca_zoo.classical._iterative._base import BaseIterative
 
 
 class IncrementalPLS(BaseIterative):
     r"""
     A class used to fit Incremental PLS
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random state to use, by default None
     accept_sparse : bool, optional
         Whether to accept sparse data, by default None
@@ -29,37 +29,37 @@
     References
     ----------
     Arora, Raman, et al. "Stochastic optimization for PCA and PLS." 2012 50th Annual Allerton Conference on Communication, Control, and Computing (Allerton). IEEE, 2012.
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         accept_sparse=None,
         batch_size=1,
         epochs=1,
         simple=False,
         initialization: Union[str, callable] = "random",
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             accept_sparse=accept_sparse,
             random_state=random_state,
             batch_size=batch_size,
             epochs=epochs,
             initialization=initialization,
         )
         self.simple = simple
 
     def _update(self, views):
         if not hasattr(self, "S"):
-            self.S = np.zeros(self.latent_dims)
+            self.S = np.zeros(self.latent_dimensions)
             self.count = 0
         if self.simple:
             self.simple_update(views)
         else:
             self.incremental_update(views)
         return False
 
@@ -75,17 +75,17 @@
         if not hasattr(self, "M"):
             self.M = np.zeros((views[0].shape[1], views[1].shape[1]))
         self.M = (
             views[0].T @ views[1]
             + self.weights[0] @ np.diag(self.S) @ self.weights[1].T
         )
         U, S, Vt = np.linalg.svd(self.M)
-        self.weights[0] = U[:, : self.latent_dims]
-        self.weights[1] = Vt.T[:, : self.latent_dims]
-        self.S = S[: self.latent_dims]
+        self.weights[0] = U[:, : self.latent_dimensions]
+        self.weights[1] = Vt.T[:, : self.latent_dimensions]
+        self.S = S[: self.latent_dimensions]
 
     def incrsvd(self, hats, orths):
         Q = np.vstack(
             (
                 np.hstack(
                     (
                         np.diag(self.S) + hats[0].T @ hats[1],
@@ -102,14 +102,14 @@
                     )
                 ),
             )
         )
         U, S, Vt = np.linalg.svd(Q)
         self.weights[0] = (
             np.hstack((self.weights[0], orths[0].T / np.linalg.norm(orths[0])))
-            @ U[:, : self.latent_dims]
+            @ U[:, : self.latent_dimensions]
         )
         self.weights[1] = (
             np.hstack((self.weights[1], orths[1].T / np.linalg.norm(orths[1])))
-            @ Vt.T[:, : self.latent_dims]
+            @ Vt.T[:, : self.latent_dimensions]
         )
-        self.S = S[: self.latent_dims]
+        self.S = S[: self.latent_dimensions]
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_pls_als.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_pls_als.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union
 
 import numpy as np
 
-from cca_zoo.models._plsmixin import PLSMixin
-from cca_zoo.models._iterative._base import BaseDeflation, BaseLoop
+from cca_zoo.classical._plsmixin import PLSMixin
+from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
 
 
 class PLS_ALS(BaseDeflation, PLSMixin):
     r"""
     A class used to fit a PLS model by alternating least squares (ALS).
 
     This model finds the linear projections of two views that maximize their covariance while minimizing their residual variance.
@@ -22,15 +22,15 @@
 
         w_i^Tw_i=1
 
     The algorithm alternates between updating :math:`w_1` and :math:`w_2` until convergence.
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random seed for reproducibility, by default None
     epochs : int, optional
         Number of iterations to run the algorithm, by default 100
@@ -40,15 +40,15 @@
         Initialization scheme to use, by default "pls"
     tol : float, optional
         Tolerance for convergence, by default 1e-3
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         tol=1e-3,
         deflation="pls",
         accept_sparse=None,
         batch_size=None,
         dataloader_kwargs=None,
@@ -56,15 +56,15 @@
         val_split=None,
         learning_rate=1,
         initialization: Union[str, callable] = "random",
         callbacks=None,
         trainer_kwargs=None,
     ):
         super().__init__(
-            latent_dims,
+            latent_dimensions,
             copy_data,
             random_state,
             tol,
             deflation=deflation,
             accept_sparse=accept_sparse,
             batch_size=batch_size,
             dataloader_kwargs=dataloader_kwargs,
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_pmd.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_pmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import itertools
 import warnings
 
 import numpy as np
 import torch
 
-from cca_zoo.models._iterative._base import BaseDeflation, BaseLoop
-from cca_zoo.models._plsmixin import PLSMixin
-from cca_zoo.models._search import _delta_search
+from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
+from cca_zoo.classical._plsmixin import PLSMixin
+from cca_zoo.classical._search import _delta_search
 from cca_zoo.utils import _check_converged_weights, _process_parameter
 
 
 class SCCA_PMD(BaseDeflation, PLSMixin):
     r"""
     A class used to fit a sparse CCA model by penalized matrix decomposition (PMD).
 
@@ -30,15 +30,15 @@
 
     where :math:`\tau_i` are the sparsity parameters for each view.
 
     The algorithm alternates between updating the weights for each view and applying a soft thresholding operator to enforce the sparsity constraints.
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random seed for reproducibility, by default None
     epochs : int, optional
         Number of iterations to run the algorithm, by default 100
@@ -58,29 +58,29 @@
         List of metrics to track during training, by default None
     verbose : bool, optional
         Whether to print progress, by default False
     """
 
     def __init__(
         self,
-        latent_dims=1,
+        latent_dimensions=1,
         copy_data=True,
         random_state=None,
         epochs=100,
         deflation="cca",
         initialization="pls",
         tol=1e-3,
         positive=False,
         tau=None,
         convergence_checking=None,
         track=None,
         verbose=False,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             epochs=epochs,
             deflation=deflation,
             initialization=initialization,
             tol=tol,
             convergence_checking=convergence_checking,
@@ -146,17 +146,15 @@
         old_weights = self.weights.copy()
         # Update each view using loop update function
         for view_index, view in enumerate(batch["views"]):
             # create a mask that is True for elements not equal to k along dim k
             mask = np.arange(scores.shape[0]) != view_index
             # apply the mask to scores and sum along dim k
             target = np.sum(scores[mask], axis=0)
-            self.weights[view_index] = np.cov(
-                np.hstack((batch["views"][view_index], target[:, np.newaxis])).T
-            )[:-1, -1]
+            self.weights[view_index] = batch["views"][view_index].T @ target
             self.weights[view_index] = _delta_search(
                 self.weights[view_index],
                 self.t[view_index],
                 tol=self.tol,
             )
             _check_converged_weights(self.weights[view_index], view_index)
         # if tracking or convergence_checking is enabled, compute the objective function
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_admm.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_admm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Iterable, Union
 
 import numpy as np
 
-from ...utils import _process_parameter
+from cca_zoo.utils import _process_parameter
 from ._base import BaseIterative, BaseLoop
 
 
 class SCCA_ADMM(BaseIterative):
     r"""
     Fits a sparse CCA model by alternating ADMM for two or more views.
 
@@ -16,15 +16,15 @@
 
         \text{subject to:}
 
         w_i^TX_i^TX_iw_i=1
 
     Parameters
     ----------
-    latent_dims : int, default=1
+    latent_dimensions : int, default=1
         Number of latent dimensions to use in the model.
     copy_data : bool, default=True
         Whether to copy the data or overwrite it.
     random_state : int, default=None
         Random seed for initialisation.
     deflation : str, default="cca"
         Deflation method to use. Options are "cca" and "pls".
@@ -45,27 +45,27 @@
 
     References
     ----------
     Suo, Xiaotong, et al. "Sparse canonical correlation analysis." arXiv preprint arXiv:1705.10865 (2017).
 
     Examples
     --------
-    >>> from cca_zoo.models import SCCA_ADMM
+    >>> from cca_zoo.classical import SCCA_ADMM
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = SCCA_ADMM(random_state=0,tau=[1e-1,1e-1])
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.84348183])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         deflation="cca",
         tau: Union[Iterable[float], float] = None,
         mu: Union[Iterable[float], float] = None,
         lam: Union[Iterable[float], float] = None,
         eta: Union[Iterable[float], float] = None,
@@ -73,15 +73,15 @@
         tol: float = 1e-3,
     ):
         self.tau = tau
         self.mu = mu
         self.lam = lam
         self.eta = eta
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             initialization=initialization,
             tol=tol,
             random_state=random_state,
             deflation=deflation,
         )
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_hsic.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_hsic.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,44 +2,44 @@
 
 import numpy as np
 import numpy.linalg as la
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import KernelCenterer
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.models._iterative._gradkcca import GradKCCA
+from cca_zoo.classical._iterative._gradkcca import GradKCCA
 from cca_zoo.utils import _process_parameter
 
 
 class SCCA_HSIC(GradKCCA):
     """
     References
     ----------
     [1] Uurtio, V., Bhadra, S., Rousu, J. Sparse Non-Linear CCA through Hilbert-Schmidt Independence Criterion. IEEE International Conference on Data Mining (ICDM 2018), to appear
 
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         scale: bool = True,
         centre=True,
         copy_data=True,
         random_state=None,
         proj: Union[Iterable[float], float] = "l1",
         gamma: Iterable[float] = None,
         coef0: Iterable[float] = None,
         repetitions=5,
         initialization: Union[str, callable] = "random",
         nystrom=False,
         nystrom_components=100,
         c=1,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             scale=scale,
             centre=centre,
             copy_data=copy_data,
             random_state=random_state,
             initialization=initialization,
             proj=proj,
             gamma=gamma,
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_parkhomenko.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_parkhomenko.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Iterable, Union
 
 import numpy as np
 import pytorch_lightning as pl
 
-from cca_zoo.models._iterative._base import BaseDeflation, BaseLoop
-from cca_zoo.models._search import _softthreshold
+from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
+from cca_zoo.classical._search import _softthreshold
 from cca_zoo.utils import _process_parameter
 
 
 class SCCA_Parkhomenko(BaseDeflation):
     r"""
     A class used to fit a sparse CCA (penalized CCA) model for two or more views.
 
@@ -28,41 +28,41 @@
 
     References
     ----------
     Parkhomenko, Elena, David Tritchler, and Joseph Beyene. "Sparse canonical correlation analysis with application to genomic data integration." Statistical applications in genetics and molecular biology 8.1 (2009).
 
     Examples
     --------
-    >>> from cca_zoo.models import SCCA_Parkhomenko
+    >>> from cca_zoo.classical import SCCA_Parkhomenko
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = SCCA_Parkhomenko(tau=[0.001,0.001],random_state=0)
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.81803527])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         deflation="cca",
         tau: Union[Iterable[float], float] = None,
         initialization: Union[str, callable] = "pls",
         tol: float = 1e-3,
         convergence_checking=False,
         patience=10,
         track=False,
         verbose=False,
     ):
         self.tau = tau
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             initialization=initialization,
             tol=tol,
             random_state=random_state,
             deflation=deflation,
             convergence_checking=convergence_checking,
             patience=patience,
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_span.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_span.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, Union
 
 import numpy as np
 
-from cca_zoo.models._iterative._base import BaseIterative, BaseLoop
-from cca_zoo.models._search import _delta_search, support_threshold
+from cca_zoo.classical._iterative._base import BaseIterative, BaseLoop
+from cca_zoo.classical._search import _delta_search, support_threshold
 from cca_zoo.utils import _process_parameter
 
 
 class SCCA_Span(BaseIterative):
     r"""
     Fits a Sparse CCA model using SpanCCA.
 
@@ -22,41 +22,41 @@
     References
     ----------
     Asteris, Megasthenis, et al. "A simple and provable algorithm for sparse diagonal CCA." International Conference on Machine Learning. PMLR, 2016.
 
 
     Examples
     --------
-    >>> from cca_zoo.models import SCCA_Span
+    >>> from cca_zoo.classical import SCCA_Span
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = SCCA_Span(regularisation="l0", tau=[2, 2])
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.84556666])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         epochs: int = 100,
         copy_data=True,
         initialization: str = "uniform",
         tol: float = 1e-3,
         regularisation="l0",
         tau: Union[Iterable[Union[float, int]], Union[float, int]] = None,
         rank=1,
         positive: Union[Iterable[bool], bool] = None,
         random_state=None,
         deflation="cca",
         verbose=0,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             epochs=epochs,
             copy_data=copy_data,
             initialization=initialization,
             tol=tol,
             random_state=random_state,
             deflation=deflation,
             verbose=verbose,
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_stochasticpls.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_stochasticpls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 
-from cca_zoo.models._iterative._ey import PLSEY
-from cca_zoo.models._plsmixin import PLSMixin
-from cca_zoo.models._iterative._base import BaseGradientLoop
+from cca_zoo.classical._iterative._ey import PLSEY
+from cca_zoo.classical._plsmixin import PLSMixin
+from cca_zoo.classical._iterative._base import BaseGradientLoop
 
 
 class PLSStochasticPower(PLSEY, PLSMixin):
     def _get_module(self, weights=None, k=None):
         return StochasticPowerLoopBase(
             weights=weights,
             k=k,
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_svd.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_svd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 from typing import Union
 
 import torch
 
-from cca_zoo.models._plsmixin import PLSMixin
-from cca_zoo.models._iterative._ey import CCAEY, EYLoop
+from cca_zoo.classical._plsmixin import PLSMixin
+from cca_zoo.classical._iterative._ey import CCAEY, EYLoop
 
 
 class CCASVD(CCAEY):
     def _get_module(self, weights=None, k=None):
         return SVDLoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="cca",
+            tracking=self.track,
+            convergence_checking=self.convergence_checking,
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
 class PLSSVD(CCASVD, PLSMixin):
     def _get_module(self, weights=None, k=None):
         return SVDLoop(
             weights=weights,
             k=k,
             learning_rate=self.learning_rate,
             optimizer_kwargs=self.optimizer_kwargs,
             objective="pls",
+            tracking=self.track,
+            convergence_checking=self.convergence_checking,
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
 class SVDLoop(EYLoop):
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_iterative/_swcca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_swcca.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from itertools import combinations
 from typing import Iterable, Union
 
 import numpy as np
 
-from cca_zoo.models._base import _BaseIterative
-from cca_zoo.models._search import _delta_search, support_threshold
+from cca_zoo.classical._base import _BaseIterative
+from cca_zoo.classical._search import _delta_search, support_threshold
 from cca_zoo.utils import _process_parameter
 
 
 class SWCCA(_BaseIterative):
     r"""
     A class used to fit SWCCA model
 
     References
     ----------
     .. Wenwen, M. I. N., L. I. U. Juan, and Shihua Zhang. "Sparse Weighted Canonical Correlation Analysis." Chinese Journal of Electronics 27.3 (2018): 459-466.
 
     Examples
     --------
-    >>> from cca_zoo.models import SWCCA
+    >>> from cca_zoo.classical import SWCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = SWCCA(regularisation='l0',tau=[2, 2], sample_support=5, random_state=0)
     >>> model.fit((X1,X2)).score((X1,X2))
     array([0.61620969])
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_kcca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_kcca.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         c_i\alpha_i^TK_i\alpha_i + (1-c_i)\alpha_i^TK_i^TK_i\alpha_i=1
 
     where :math:`K_i` are the kernel matrices for each view and :math:`c_i` are the regularization parameters for each view.
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random seed for reproducibility, by default None
     c : Union[Iterable[float], float], optional
         Regularization parameter or list of parameters for each view, by default None. If None, it will be set to zero for each view.
@@ -99,41 +99,41 @@
     coef0: Iterable[float], optional
         Coef0 parameter or list of parameters for the polynomial or sigmoid kernel for each view, by default None. Ignored if kernel is not polynomial or sigmoid.
     kernel_params: Iterable[dict], optional
         Additional parameters or list of parameters for the kernel function for each view, by default None.
 
     Examples
     --------
-    >>> from cca_zoo.models import KCCA
+    >>> from cca_zoo.classical import KCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = KCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
     array([0.96893666])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         c: Union[Iterable[float], float] = None,
         eps=1e-3,
         kernel: Iterable[Union[str, float, callable]] = None,
         gamma: Iterable[float] = None,
         degree: Iterable[float] = None,
         coef0: Iterable[float] = None,
         kernel_params: Iterable[dict] = None,
     ):
         # Call the parent class constructor
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             c=c,
             eps=eps,
             pca=False,
         )
         # Store the kernel parameters
@@ -173,15 +173,15 @@
 
     T^TT=1
 
     where :math:`K_i` are the kernel matrices for each view and :math:`T` is the auxiliary vector.
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random seed for reproducibility, by default None
     c : Union[Iterable[float], float], optional
         Regularization parameter or list of parameters for each view, by default None. If None, it will be set to zero for each view.
@@ -200,41 +200,41 @@
 
     References
     ----------
     Tenenhaus, Arthur, Cathy Philippe, and Vincent Frouin. "Kernel generalized canonical correlation analysis." Computational Statistics & Data Analysis 90 (2015): 114-131.
 
     Examples
     --------
-    >>> from cca_zoo.models import KGCCA
+    >>> from cca_zoo.classical import KGCCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = KGCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
     array([0.97019284])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         c: Union[Iterable[float], float] = None,
         kernel: Iterable[Union[float, callable]] = None,
         gamma: Iterable[float] = None,
         degree: Iterable[float] = None,
         coef0: Iterable[float] = None,
         kernel_params: Iterable[dict] = None,
         view_weights: Iterable[float] = None,
         eps: float = 1e-6,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             c=c,
             view_weights=view_weights,
             eps=eps,
         )
         self.kernel_params = kernel_params
@@ -252,15 +252,15 @@
                 degree=self.degree[i],
                 coef0=self.coef0[i],
                 **self.kernel_params[i]
             )
             for i, view in enumerate(self.train_views)
         ]
         self.weights = [
-            np.linalg.pinv(kernel) @ eigvecs[:, : self.latent_dims]
+            np.linalg.pinv(kernel) @ eigvecs[:, : self.latent_dimensions]
             for kernel in kernels
         ]
 
     def _more_tags(self):
         # Indicate that this class is for multiview data
         return {"multiview": True, "kernel": True}
 
@@ -283,39 +283,39 @@
 
     References
     ----------
     Kim, Tae-Kyun, Shu-Fai Wong, and Roberto Cipolla. "Tensor canonical correlation analysis for action classification." 2007 IEEE Conference on Computer Vision and Pattern Recognition. IEEE, 2007
 
     Examples
     --------
-    >>> from cca_zoo.models import KTCCA
+    >>> from cca_zoo.classical import KTCCA
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = KTCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
     array([1.69896269])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         eps=1e-3,
         c: Union[Iterable[float], float] = None,
         kernel: Iterable[Union[float, callable]] = None,
         gamma: Iterable[float] = None,
         degree: Iterable[float] = None,
         coef0: Iterable[float] = None,
         kernel_params: Iterable[dict] = None,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             eps=eps,
             c=c,
         )
         self.kernel_params = kernel_params
         self.gamma = gamma
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_mcca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_mcca.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from typing import Iterable, Union
+
+import numpy as np
 from scipy.linalg import block_diag
+from scipy.linalg import eigh
 from sklearn.decomposition import PCA
-import numpy as np
 
-from typing import Iterable, Union
-from scipy.linalg import eigh
-from cca_zoo.models._plsmixin import PLSMixin
-from cca_zoo.models._base import BaseModel
+from cca_zoo.classical._base import BaseModel
+from cca_zoo.classical._plsmixin import PLSMixin
 from cca_zoo.utils import _process_parameter
 
 
 class MCCA(BaseModel):
     r"""
     A class used to fit Regularised CCA (canonical ridge) model. This model adds a regularization term to the CCA objective function to avoid overfitting and improve stability. It uses PCA to perform the optimization efficiently for high dimensional data.
 
@@ -25,15 +26,15 @@
 
         (1-c_2)w_2^TX_2^TX_2w_2+c_2w_2^Tw_2=n
 
     where :math:`c_i` are the regularization parameters for each view.
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random state, by default None
     c : Union[Iterable[float], float], optional
         Regularisation parameter, by default None
@@ -44,28 +45,28 @@
     References
     --------
     Vinod, Hrishikesh D. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         c: Union[Iterable[float], float] = None,
         accept_sparse=None,
         eps: float = 1e-6,
         pca: bool = True,
     ):
         # Set the default value for accept_sparse
         if accept_sparse is None:
             accept_sparse = ["csc", "csr"]
         # Call the parent class constructor
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             accept_sparse=accept_sparse,
             random_state=random_state,
         )
         # Store the c parameter
         self.c = c
         self.eps = eps
@@ -99,15 +100,15 @@
         # Solve the eigenvalue problem
         # Get the dimension of C
         p = C.shape[0]
         # Solve the generalized eigenvalue problem Cx=lambda Dx using a subset of eigenvalues and eigenvectors
         [eigvals, eigvecs] = eigh(
             C,
             D,
-            subset_by_index=[p - self.latent_dims, p - 1],
+            subset_by_index=[p - self.latent_dimensions, p - 1],
         )
         # Sort the eigenvalues and eigenvectors in descending order
         idx = np.argsort(eigvals, axis=0)[::-1]
         eigvecs = eigvecs[:, idx].real
         return np.flip(eigvals), eigvecs
 
     def _weights(self, eigvals, eigvecs, views, **kwargs):
@@ -256,54 +257,54 @@
 
         w_1^TX_1^TX_1w_1=n
 
         w_2^TX_2^TX_2w_2=n
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random seed for reproducibility, by default None
 
     References
     --------
 
     Hotelling, Harold. "Relations between two sets of variates." Breakthroughs in statistics. Springer, New York, NY, 1992. 162-190.
 
     Example
     -------
-    >>> from cca_zoo.models import CCA
+    >>> from cca_zoo.classical import CCA
     >>> import numpy as np
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = CCA()
     >>> model.fit((X1,X2)).score((X1,X2))
     array([1.])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
     ):
         # Call the parent class constructor with c=0.0 to disable regularization
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             c=0.0,
             random_state=random_state,
         )
 
 
-class PLS(MCCA, PLSMixin):
+class PLS(rCCA, PLSMixin):
     r"""
     A class used to fit a simple PLS model. This model finds the linear projections of two views that maximize their covariance.
 
     Implements PLS by inheriting regularised CCA with maximal regularisation. This is equivalent to solving the following optimization problem:
 
     .. math::
 
@@ -313,28 +314,59 @@
 
         w_1^Tw_1=1
 
         w_2^Tw_2=1
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
+        Number of latent dimensions to use, by default 1
+    copy_data : bool, optional
+        Whether to copy the data, by default True
+    random_state : int, optional
+        Random state, by default None
+    """
+
+    def __init__(
+        self,
+        latent_dimensions: int = 1,
+        copy_data=True,
+        random_state=None,
+    ):
+        # Call the parent class constructor with c=1 to enable maximal regularization
+        super().__init__(
+            latent_dimensions=latent_dimensions,
+            copy_data=copy_data,
+            c=1,
+            random_state=random_state,
+        )
+
+
+class MPLS(MCCA, PLSMixin):
+    r"""
+    A class used to fit a mutiview PLS model. This model finds the linear projections of two views that maximize their covariance.
+
+    Implements PLS by inheriting regularised CCA with maximal regularisation. This is equivalent to solving the following optimization problem:
+
+    Parameters
+    ----------
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random state, by default None
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
     ):
         # Call the parent class constructor with c=1 to enable maximal regularization
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             c=1,
             random_state=random_state,
         )
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_ncca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_ncca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Iterable, Union
 
 import numpy as np
 from sklearn.metrics import pairwise_kernels
 from sklearn.neighbors import NearestNeighbors
 
-from cca_zoo.models._base import BaseModel
+from cca_zoo.classical._base import BaseModel
 from cca_zoo.utils.check_values import _process_parameter
 
 
 class NCCA(BaseModel):
     """
     A class used to fit nonparametric (NCCA) model. This model extends CCA to nonlinear relationships by using local linear projections based on nearest neighbors.
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     accept_sparse : bool, optional
         Whether to accept sparse data as input, by default False
     random_state : Union[int, np.random.RandomState], optional
         Random seed for reproducibility, by default None
@@ -30,34 +30,34 @@
 
     References
     ----------
     Michaeli, Tomer, Weiran Wang, and Karen Livescu. "Nonparametric canonical correlation analysis." International conference on machine learning. PMLR, 2016.
 
     Example
     -------
-    >>> from cca_zoo.models import NCCA
+    >>> from cca_zoo.classical import NCCA
     >>> X1 = np.random.rand(10,5)
     >>> X2 = np.random.rand(10,5)
     >>> model = NCCA()
     >>> model.fit((X1,X2)).score((X1,X2))
     array([1.])
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         accept_sparse=False,
         random_state: Union[int, np.random.RandomState] = None,
         nearest_neighbors=None,
         gamma: Iterable[float] = None,
     ):
         # Call the parent class constructor
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             accept_sparse=accept_sparse,
             random_state=random_state,
         )
         # Store the nearest neighbors and gamma parameters
         self.nearest_neighbors = nearest_neighbors
         self.gamma = gamma
@@ -98,18 +98,18 @@
             self.Ws[1] / self.Ws[1].sum(axis=0, keepdims=True),
         ]
         # Compute the cross-covariance matrix between the weight matrices
         S = self.Ws[0] @ self.Ws[1]
         # Perform singular value decomposition on the cross-covariance matrix
         U, S, Vt = np.linalg.svd(S)
         # Compute the canonical score vectors for each view
-        self.f = U[:, 1 : self.latent_dims + 1] * np.sqrt(self.n_samples_)
-        self.g = Vt[1 : self.latent_dims + 1, :].T * np.sqrt(self.n_samples_)
+        self.f = U[:, 1 : self.latent_dimensions + 1] * np.sqrt(self.n_samples_)
+        self.g = Vt[1 : self.latent_dimensions + 1, :].T * np.sqrt(self.n_samples_)
         # Store the canonical correlations
-        self.S = S[1 : self.latent_dims + 1]
+        self.S = S[1 : self.latent_dimensions + 1]
         return self
 
     def transform(self, views: Iterable[np.ndarray], **kwargs):
         # Find the nearest neighbors for each view
         nns = [
             self.knns[i].kneighbors(view, self.nearest_neighbors[i])
             for i, view in enumerate(views)
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_partialcca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_partialcca.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Iterable, Union
 
 import numpy as np
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.models import MCCA
+from cca_zoo.classical import MCCA
 
 
 class PartialCCA(MCCA):
     r"""
     A class used to fit a partial CCA model. This model extends CCA to account for confounding variables that may affect the correlation between views.
 
     .. math::
@@ -23,15 +23,15 @@
 
     References
     ----------
     Rao, B. Raja. "Partial canonical correlations." Trabajos de estadistica y de investigación operativa 20.2-3 (1969): 211-219.
 
     Example
     -------
-    >>> from cca_zoo.models import PartialCCA
+    >>> from cca_zoo.classical import PartialCCA
     >>> X1 = np.random.rand(10,5)
     >>> X2 = np.random.rand(10,5)
     >>> partials = np.random.rand(10,3)
     >>> model = PartialCCA()
     >>> model.fit((X1,X2),partials=partials).score((X1,X2))
     array([0.99993046])
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_pcacca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_pcacca.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Iterable, Union
 
 from sklearn.decomposition import PCA
 import numpy as np
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.models._mcca import MCCA
+from cca_zoo.classical._mcca import MCCA
 
 
 class PCACCA(MCCA):
     """
     Principal Component Analysis CCA
 
     Data driven PCA on each view followed by CCA on the PCA components. Keep percentage of variance
     """
 
     def __init__(
         self,
-        latent_dims=1,
+        latent_dimensions=1,
         copy_data=True,
         random_state=None,
         c: Union[Iterable[float], float] = None,
         eps=1e-9,
         percent_variance=0.99,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             c=c,
             eps=eps,
         )
         # ensure that the percent variance is less than 1 and give a warning if not
         assert percent_variance <= 1, "percent_variance must be less than 1"
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_plsmixin.py` & `cca_zoo-2.0.1/cca_zoo/classical/_plsmixin.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,19 +11,26 @@
         Parameters
         ----------
         views : list/tuple of numpy arrays or array likes with the same number of rows (samples)
         kwargs : any additional keyword arguments required by the given model
 
         Returns
         -------
-        variance : numpy array of shape (n_views, latent_dims)
+        variance : numpy array of shape (n_views, latent_dimensions)
 
         """
         # Calculate total variance in each view by SVD
         n = views[0].shape[0]
+        if n < min(views[0].shape[1], views[1].shape[1]):
+
+            def reduce_dims(x):
+                U, S, _ = np.linalg.svd(x, full_matrices=False)
+                return U @ np.diag(S)
+
+            views = [reduce_dims(view) for view in views]
         variance = np.array(
             [np.sum(np.linalg.svd(view)[1] ** 2, keepdims=True) / n for view in views]
         )
         return variance
 
     def total_covariance_(self, views: Iterable[np.ndarray], **kwargs) -> float:
         """
@@ -44,33 +51,30 @@
         # if n<p calculate views[0]@views[0].T@views[1]@views[1].T else calculate views[0].T@views[1]
         if n < min(views[0].shape[1], views[1].shape[1]):
 
             def reduce_dims(x):
                 U, S, _ = np.linalg.svd(x, full_matrices=False)
                 return U @ np.diag(S)
 
-            covariance = np.sum(
-                np.linalg.svd(reduce_dims(views[0]).T @ reduce_dims(views[1]))[1]
-            ) / (n - 1)
-        else:
-            covariance = np.sum(np.linalg.svd(views[0].T @ views[1])[1]) / (n - 1)
+            views = [reduce_dims(view) for view in views]
+        covariance = np.sum(np.linalg.svd(views[0].T @ views[1])[1]) / (n - 1)
         return covariance
 
     def explained_variance_(self, views: Iterable[np.ndarray], **kwargs) -> np.ndarray:
         """
         Returns the total variance for each view
 
         Parameters
         ----------
         views : list/tuple of numpy arrays or array likes with the same number of rows (samples)
         kwargs : any additional keyword arguments required by the given model
 
         Returns
         -------
-        variance : numpy array of shape (n_views, latent_dims)
+        variance : numpy array of shape (n_views, latent_dimensions)
 
         """
         transformed_views = self.transform(views, **kwargs)
         variance = np.array([np.var(view, axis=0) for view in transformed_views])
         return variance
 
     def explained_covariance_(
@@ -82,21 +86,21 @@
         Parameters
         ----------
         views : list/tuple of numpy arrays or array likes with the same number of rows (samples)
         kwargs : any additional keyword arguments required by the given model
 
         Returns
         -------
-        covariance : numpy array of shape (n_views, latent_dims)
+        covariance : numpy array of shape (n_views, latent_dimensions)
 
         """
         transformed_views = self.transform(views, **kwargs)
         covariance = np.diag(
             np.cov(*transformed_views, rowvar=False)[
-                : self.latent_dims, self.latent_dims :
+                : self.latent_dimensions, self.latent_dimensions :
             ]
         )
         return covariance
 
     def explained_covariance_ratio_(
         self, views: Iterable[np.ndarray], **kwargs
     ) -> np.ndarray:
@@ -106,15 +110,15 @@
         Parameters
         ----------
         views : list/tuple of numpy arrays or array likes with the same number of rows (samples)
         kwargs : any additional keyword arguments required by the given model
 
         Returns
         -------
-        explained_covariance_ratio_ : numpy array of shape (n_views, latent_dims)
+        explained_covariance_ratio_ : numpy array of shape (n_views, latent_dimensions)
 
         """
         explained_covariance = self.explained_covariance_(views, **kwargs)
         covariance = self.total_covariance_(views, **kwargs)
         explained_covariance_ratio = explained_covariance / covariance
         return explained_covariance_ratio
 
@@ -127,15 +131,15 @@
         Parameters
         ----------
         views : list/tuple of numpy arrays or array likes with the same number of rows (samples)
         kwargs : any additional keyword arguments required by the given model
 
         Returns
         -------
-        explained_variance_ratio : numpy array of shape (n_views, latent_dims)
+        explained_variance_ratio : numpy array of shape (n_views, latent_dimensions)
 
         """
         component_variance = self.explained_variance_(views, **kwargs)
         variance = self.total_variance_(views, **kwargs)
         explained_variance_ratio = component_variance / variance
         return explained_variance_ratio
 
@@ -148,15 +152,15 @@
         Parameters
         ----------
         views : list/tuple of numpy arrays or array likes with the same number of rows (samples)
         kwargs : any additional keyword arguments required by the given model
 
         Returns
         -------
-        explained_variance_cumulative_ : numpy array of shape (n_views, latent_dims)
+        explained_variance_cumulative_ : numpy array of shape (n_views, latent_dimensions)
 
         """
         explained_variance_ratio = self.explained_variance_ratio_(views, **kwargs)
         explained_variance_cumulative = np.cumsum(explained_variance_ratio, axis=1)
         return explained_variance_cumulative
 
     def explained_covariance_cumulative_(self, views: Iterable[np.ndarray], **kwargs):
@@ -166,13 +170,13 @@
         Parameters
         ----------
         views : list/tuple of numpy arrays or array likes with the same number of rows (samples)
         kwargs : any additional keyword arguments required by the given model
 
         Returns
         -------
-        explained_covariance_cumulative_ : numpy array of shape (n_views, latent_dims)
+        explained_covariance_cumulative_ : numpy array of shape (n_views, latent_dimensions)
 
         """
         explained_covariance_ratio = self.explained_covariance_ratio_(views, **kwargs)
         explained_covariance_cumulative = np.cumsum(explained_covariance_ratio)
         return explained_covariance_cumulative
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_prcca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_prcca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import warnings
 from typing import Iterable
 
 import numpy as np
 from scipy.linalg import block_diag
 
-from cca_zoo.models._mcca import MCCA
+from cca_zoo.classical._mcca import MCCA
 
 
 class PRCCA(MCCA):
     """
     Partially Regularized Canonical Correlation Analysis
 
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random state for reproducibility, by default None
     eps : float, optional
         Tolerance for convergence, by default 1e-3
@@ -28,30 +28,30 @@
     References
     ----------
     Tuzhilina, Elena, Leonardo Tozzi, and Trevor Hastie. "Canonical correlation analysis in high dimensions with structured regularization." Statistical Modelling (2021): 1471082X211041033.
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
         eps=1e-3,
         c=0,
     ):
         """
         Parameters
         ----------
         c : Union[Iterable[float], float], optional
             Regularisation parameter, by default None
         eps : float, optional
             Tolerance for convergence, by default 1e-3
         """
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             random_state=random_state,
             eps=eps,
             c=c,
             pca=False,
         )
 
@@ -99,15 +99,17 @@
                 for i, view in enumerate(views)
             ]
         )
         D_smallest_eig = min(0, np.linalg.eigvalsh(D).min()) - self.eps
         D = D - D_smallest_eig * np.eye(D.shape[0])
         return D
 
-    def _transform_weights(self, views, idxs=None):
+    def _weights(self, eigvals, eigvecs, views, idxs=None, **kwargs):
+        # split eigvecs into weights for each view
+        self.weights = np.split(eigvecs, self.splits[:-1], axis=0)
         for i, idx in enumerate(idxs):
             alpha_1 = self.weights[i][idx]
             alpha_2 = np.delete(self.weights[i], idx, axis=0)
             alpha_2 -= self.B[i] @ alpha_1
             mask = np.ones(self.weights[i].shape[0], dtype=bool)
             mask[idx] = False
             self.weights[i][mask] = alpha_2
```

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_search.py` & `cca_zoo-2.0.1/cca_zoo/classical/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.0/cca_zoo/models/_tcca.py` & `cca_zoo-2.0.1/cca_zoo/classical/_tcca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable
 
 import numpy as np
 import tensorly as tl
 from scipy.linalg import sqrtm
 from tensorly.decomposition import parafac
 
-from cca_zoo.models import MCCA
+from cca_zoo.classical import MCCA
 
 
 class TCCA(MCCA):
     r"""
     A class used to fit TCCA model. This model extends MCCA to higher order correlations by using tensor products of the views.
 
     The objective function of TCCA is:
@@ -26,15 +26,15 @@
 
     References
     ----------
     Kim, Tae-Kyun, Shu-Fai Wong, and Roberto Cipolla. "Tensor canonical correlation analysis for action classification." 2007 IEEE Conference on Computer Vision and Pattern Recognition. IEEE, 2007
 
     Examples
     --------
-    >>> from cca_zoo.models import TCCA
+    >>> from cca_zoo.classical import TCCA
     >>> rng=np.random.RandomState(0)
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> X3 = rng.random((10,5))
     >>> model = TCCA()
     >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
     array([1.14595755])
@@ -57,15 +57,15 @@
                 for _ in range(len(M.shape) - 1):
                     el = np.expand_dims(el, 1)
                 # Then we perform an outer product by expanding the dimensionality of M and
                 # outer product with the expanded el
                 M = np.expand_dims(M, -1) @ el
         M = np.mean(M, 0)
         tl.set_backend("numpy")
-        M_parafac = parafac(M, self.latent_dims, verbose=False)
+        M_parafac = parafac(M, self.latent_dimensions, verbose=False)
         self.weights = [
             cov_invsqrt @ fac
             for i, (view, cov_invsqrt, fac) in enumerate(
                 zip(whitened_views, covs_invsqrt, M_parafac.factors)
             )
         ]
         return self
```

### Comparing `cca_zoo-2.0.0/cca_zoo/plotting/plotting.py` & `cca_zoo-2.0.1/cca_zoo/visualisation/plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.0/cca_zoo/probabilisticmodels/_probabilisticcca.py` & `cca_zoo-2.0.1/cca_zoo/probabilistic/_probabilisticcca.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 import numpy as np
 import numpyro
 import numpyro.distributions as dist
 from jax.random import PRNGKey
 from numpyro.infer import MCMC, NUTS, Predictive
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.models._base import BaseModel
+from cca_zoo.classical._base import BaseModel
 
 
 class ProbabilisticCCA(BaseModel):
     """
     A class used to fit a Probabilistic CCA. Not quite the same due to using VI methods rather than EM
 
     Parameters
     ----------
-    latent_dims : int, optional
+    latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
     copy_data : bool, optional
         Whether to copy the data, by default True
     random_state : int, optional
         Random state, by default 0
     num_samples : int, optional
         Number of samples to use in VI, by default 100
@@ -34,22 +34,22 @@
     Bach, Francis R., and Michael I. Jordan. "A probabilistic interpretation of canonical correlation analysis." (2005).
     Wang, Chong. "Variational Bayesian approach to canonical correlation analysis." IEEE Transactions on Neural Networks 18.3 (2007): 905-910.
 
     """
 
     def __init__(
         self,
-        latent_dims: int = 1,
+        latent_dimensions: int = 1,
         copy_data=True,
         random_state: int = 0,
         num_samples=100,
         num_warmup=100,
     ):
         super().__init__(
-            latent_dims=latent_dims,
+            latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             accept_sparse=False,
             random_state=random_state,
         )
         self.num_samples = num_samples
         self.num_warmup = num_warmup
         self.rng_key = PRNGKey(random_state)
@@ -91,26 +91,29 @@
         ]
         # parameter representing the within view variance for each view of data
         psi = [
             numpyro.sample("psi_" + str(i), dist.LKJCholesky(p_))
             for i, p_ in enumerate(p)
         ]
         # parameter representing weights applied to latent variables
-        with numpyro.plate("plate_views", self.latent_dims):
+        with numpyro.plate("plate_views", self.latent_dimensions):
             self.weights_list = [
                 numpyro.sample(
                     "W_" + str(i),
                     dist.MultivariateNormal(0.0, 10 * jnp.diag(jnp.ones(p_))),
                 )
                 for i, p_ in enumerate(p)
             ]
         with numpyro.plate("plate_i", n):
             # sample from latent z: the latent variables of the model
             z = numpyro.sample(
-                "z", dist.MultivariateNormal(0.0, jnp.diag(jnp.ones(self.latent_dims)))
+                "z",
+                dist.MultivariateNormal(
+                    0.0, jnp.diag(jnp.ones(self.latent_dimensions))
+                ),
             )
             # sample from multivariate normal and observe data
             [
                 numpyro.sample(
                     "obs" + str(i),
                     dist.MultivariateNormal((z @ W_) + mu_, scale_tril=psi_),
                     obs=X_,
```

### Comparing `cca_zoo-2.0.0/cca_zoo/test/test_deepmodels.py` & `cca_zoo-2.0.1/cca_zoo/test/test_deepmodels.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 import numpy as np
 import pytorch_lightning as pl
 from sklearn.utils.validation import check_random_state
 from torch import manual_seed
 from torch.utils.data import random_split
 
 from cca_zoo.data.deep import NumpyDataset, check_dataset, get_dataloaders
-from cca_zoo.deepmodels import (
+from cca_zoo.deep import (
     DCCA,
     DCCA_EY,
+    DCCA_GH,
+    DCCA_SVD,
     DCCA_NOI,
     DCCA_SDL,
     DCCAE,
     DTCCA,
     DVCCA,
+    DGCCA,
     BarlowTwins,
     SplitAE,
     architectures,
     objectives,
 )
-from cca_zoo.models import CCA, MCCA
+from cca_zoo.classical import CCA, MCCA, GCCA
 
 manual_seed(0)
 rng = check_random_state(0)
 X = rng.rand(256, 10)
 Y = rng.rand(256, 12)
 Z = rng.rand(256, 14)
+X -= X.mean(axis=0)
+Y -= Y.mean(axis=0)
+Z -= Z.mean(axis=0)
 X_conv = rng.rand(256, 1, 16, 16)
 Y_conv = rng.rand(256, 1, 16, 16)
+X_conv -= X_conv.mean(axis=0)
+Y_conv -= Y_conv.mean(axis=0)
 dataset = NumpyDataset([X, Y, Z])
 check_dataset(dataset)
-train_dataset, val_dataset = random_split(dataset, [200, 56])
+train_dataset, val_dataset = random_split(dataset, [256 - 56, 56])
 loader = get_dataloaders(dataset)
 train_loader, val_loader = get_dataloaders(train_dataset, val_dataset)
 conv_dataset = NumpyDataset((X_conv, Y_conv))
 conv_loader = get_dataloaders(conv_dataset)
 train_ids = train_dataset.indices
 trainer_kwargs = dict(
     enable_checkpointing=False,
@@ -45,285 +53,364 @@
 
 def test_numpy_dataset():
     dataset = NumpyDataset([X, Y, Z])
     check_dataset(dataset)
     get_dataloaders(dataset)
 
 
-def test_linear():
+def test_linear_mcca():
     max_epochs = 100
-    latent_dims = 2
-    cca = CCA(latent_dims=latent_dims).fit((X, Y))
-    encoder_1 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=12)
-    dcca = DCCA(
-        latent_dims=latent_dims,
-        encoders=[encoder_1, encoder_2],
+    latent_dimensions = 2
+    mcca = MCCA(latent_dimensions=latent_dimensions).fit((X, Y, Z))
+    # DCCA_MCCA
+    encoder_1 = architectures.LinearEncoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.LinearEncoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
+    encoder_3 = architectures.LinearEncoder(
+        latent_dimensions=latent_dimensions, feature_size=14
+    )
+    dmcca = DCCA(
+        latent_dimensions=latent_dimensions,
+        encoders=[encoder_1, encoder_2, encoder_3],
         lr=1e-1,
         objective=objectives.MCCA,
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
-    trainer.fit(dcca, loader)
-    # check linear encoder with SGD matches vanilla linear CCA
-    assert (
-        np.testing.assert_array_almost_equal(
-            cca.score((X, Y)), dcca.score(loader), decimal=2
-        )
-        is None
-    )
-    encoder_1 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=12)
-    dcca = DCCA_EY(latent_dims=latent_dims, encoders=[encoder_1, encoder_2], lr=5e-1)
-    trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
-    trainer.fit(dcca, loader)
-    # check linear encoder with EG matches vanilla linear CCA
+    trainer.fit(dmcca, loader)
     assert (
         np.testing.assert_array_almost_equal(
-            cca.score((X, Y)), dcca.score(loader), decimal=2
+            mcca.score((X, Y, Z)).sum(), dmcca.score(loader).sum(), decimal=2
         )
         is None
     )
 
 
-def test_linear_mcca():
+def test_linear_gcca():
     max_epochs = 100
-    latent_dims = 2
-    cca = MCCA(latent_dims=latent_dims).fit((X, Y, Z))
-    # DCCA_MCCA
-    encoder_1 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=12)
-    encoder_3 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=14)
-    dmcca = DCCA(
-        latent_dims=latent_dims,
+    latent_dimensions = 2
+    gcca = GCCA(latent_dimensions=latent_dimensions).fit((X, Y, Z))
+    # DCCA_GCCA
+    encoder_1 = architectures.LinearEncoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.LinearEncoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
+    encoder_3 = architectures.LinearEncoder(
+        latent_dimensions=latent_dimensions, feature_size=14
+    )
+    dgcca = DGCCA(
+        latent_dimensions=latent_dimensions,
         encoders=[encoder_1, encoder_2, encoder_3],
-        lr=1e-1,
-        objective=objectives.MCCA,
+        lr=1e-2,
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
-    trainer.fit(dmcca, loader)
+    trainer.fit(dgcca, loader)
     assert (
         np.testing.assert_array_almost_equal(
-            cca.score((X, Y, Z)).sum(), dmcca.score(loader).sum(), decimal=2
+            gcca.score((X, Y, Z)).sum(), dgcca.score(loader).sum(), decimal=2
         )
         is None
     )
-    # DCCA_EY
-    encoder_1 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=12)
-    encoder_3 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=14)
-    dmccaeg = DCCA_EY(
-        latent_dims=latent_dims, encoders=[encoder_1, encoder_2, encoder_3], lr=1e-1
+
+
+def test_DTCCA_methods():
+    max_epochs = 100
+    # check that DTCCA is equivalent to CCA for 2 views with linear encoders
+    latent_dimensions = 2
+    cca = CCA(latent_dimensions=latent_dimensions)
+    encoder_1 = architectures.LinearEncoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.LinearEncoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
+    dtcca = DTCCA(
+        latent_dimensions=latent_dimensions, encoders=[encoder_1, encoder_2], lr=1e-2
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
-    trainer.fit(dmccaeg, loader)
+    trainer.fit(dtcca, train_loader)
+    z = dtcca.transform(train_loader)
     assert (
         np.testing.assert_array_almost_equal(
-            cca.score((X, Y, Z)).sum(), dmccaeg.score(loader).sum(), decimal=2
+            cca.fit((X[train_ids], Y[train_ids]))
+            .score((X[train_ids], Y[train_ids]))
+            .sum(),
+            cca.fit((z)).score((z)).sum(),
+            decimal=1,
         )
         is None
     )
 
 
 def test_DCCA_methods():
     N = len(train_dataset)
     max_epochs = 100
-    latent_dims = 2
-    cca = CCA(latent_dims=latent_dims).fit((X, Y))
+    latent_dimensions = 2
+    cca = CCA(latent_dimensions=latent_dimensions).fit((X, Y))
     # DCCA
-    encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
+    encoder_1 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
     dcca = DCCA(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dimensions,
         encoders=[encoder_1, encoder_2],
         objective=objectives.CCA,
         lr=1e-3,
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(dcca, train_loader, val_dataloaders=val_loader)
     assert (
         np.testing.assert_array_less(
             cca.score((X, Y)).sum(), dcca.score(train_loader).sum()
         )
         is None
     )
+    # DCCA_GH
+    encoder_1 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
+    dcca_gh = DCCA_GH(
+        latent_dimensions=latent_dimensions,
+        encoders=[encoder_1, encoder_2],
+        lr=1e-1,
+    )
+    trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
+    trainer.fit(dcca_gh, train_loader, val_dataloaders=val_loader)
+    assert (
+        np.testing.assert_array_less(
+            cca.score((X, Y)).sum(), dcca_gh.score(train_loader).sum()
+        )
+        is None
+    )
+    # DCCA_SVD
+    encoder_1 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
+    dcca_svd = DCCA_SVD(
+        latent_dimensions=latent_dimensions,
+        encoders=[encoder_1, encoder_2],
+        lr=1e-1,
+    )
+    trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
+    trainer.fit(dcca_svd, train_loader, val_dataloaders=val_loader)
+    assert (
+        np.testing.assert_array_less(
+            cca.score((X, Y)).sum(), dcca_svd.score(train_loader).sum()
+        )
+        is None
+    )
     # DCCA_EY
-    encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
-    dcca_eg = DCCA_EY(
-        latent_dims=latent_dims,
+    encoder_1 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
+    dcca_ey = DCCA_EY(
+        latent_dimensions=latent_dimensions,
         encoders=[encoder_1, encoder_2],
         lr=1e-1,
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
-    trainer.fit(dcca_eg, train_loader, val_dataloaders=val_loader)
+    trainer.fit(dcca_ey, train_loader, val_dataloaders=val_loader)
     assert (
         np.testing.assert_array_less(
-            cca.score((X, Y)).sum(), dcca_eg.score(train_loader).sum()
+            cca.score((X, Y)).sum(), dcca_ey.score(train_loader).sum()
         )
         is None
     )
     # DCCA_NOI
-    encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
-    dcca_noi = DCCA_NOI(latent_dims, N, encoders=[encoder_1, encoder_2], rho=0.2)
+    encoder_1 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
+    dcca_noi = DCCA_NOI(latent_dimensions, N, encoders=[encoder_1, encoder_2], rho=0.2)
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(dcca_noi, train_loader)
     assert (
         np.testing.assert_array_less(
             cca.score((X, Y)).sum(), dcca_noi.score(train_loader).sum()
         )
         is None
     )
     # Soft Decorrelation (_stochastic Decorrelation Loss)
-    encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
-    sdl = DCCA_SDL(latent_dims, N, encoders=[encoder_1, encoder_2], lam=1e-2, lr=1e-3)
+    encoder_1 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
+    sdl = DCCA_SDL(
+        latent_dimensions, N, encoders=[encoder_1, encoder_2], lam=1e-2, lr=1e-3
+    )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(sdl, train_loader)
     assert (
         np.testing.assert_array_less(
             cca.score((X, Y)).sum(), sdl.score(train_loader).sum()
         )
         is None
     )
     # Barlow Twins
-    encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
+    encoder_1 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
     barlowtwins = BarlowTwins(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dimensions,
         encoders=[encoder_1, encoder_2],
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(barlowtwins, train_loader)
     assert (
         np.testing.assert_array_less(
             cca.score((X, Y)).sum(), barlowtwins.score(train_loader).sum()
         )
         is None
     )
     # DGCCA
-    encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
+    encoder_1 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
     dgcca = DCCA(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dimensions,
         encoders=[encoder_1, encoder_2],
         objective=objectives.GCCA,
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(dgcca, train_loader)
     assert (
         np.testing.assert_array_less(
             cca.score((X, Y)).sum(), dgcca.score(train_loader).sum()
         )
         is None
     )
     # DMCCA
-    encoder_1 = architectures.Encoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.Encoder(latent_dims=latent_dims, feature_size=12)
+    encoder_1 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    encoder_2 = architectures.Encoder(
+        latent_dimensions=latent_dimensions, feature_size=12
+    )
     dmcca = DCCA(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dimensions,
         encoders=[encoder_1, encoder_2],
         objective=objectives.MCCA,
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(dmcca, train_loader)
     assert (
         np.testing.assert_array_less(
             cca.score((X, Y)).sum(), dmcca.score(train_loader).sum()
         )
         is None
     )
 
 
-def test_DTCCA_methods():
-    max_epochs = 100
-    # check that DTCCA is equivalent to CCA for 2 views with linear encoders
-    latent_dims = 2
-    cca = CCA(latent_dims=latent_dims)
-    encoder_1 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=10)
-    encoder_2 = architectures.LinearEncoder(latent_dims=latent_dims, feature_size=12)
-    dtcca = DTCCA(latent_dims=latent_dims, encoders=[encoder_1, encoder_2], lr=1e-2)
-    trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
-    trainer.fit(dtcca, train_loader)
-    z = dtcca.transform(train_loader)
-    assert (
-        np.testing.assert_array_almost_equal(
-            cca.fit((X[train_ids], Y[train_ids]))
-            .score((X[train_ids], Y[train_ids]))
-            .sum(),
-            cca.fit((z)).score((z)).sum(),
-            decimal=1,
-        )
-        is None
-    )
-
-
 def test_DCCAE_methods():
     max_epochs = 2
-    latent_dims = 2
-    encoder_1 = architectures.CNNEncoder(latent_dims=latent_dims, feature_size=(16, 16))
-    encoder_2 = architectures.CNNEncoder(latent_dims=latent_dims, feature_size=(16, 16))
-    decoder_1 = architectures.CNNDecoder(latent_dims=latent_dims, feature_size=(16, 16))
-    decoder_2 = architectures.CNNDecoder(latent_dims=latent_dims, feature_size=(16, 16))
+    latent_dimensions = 2
+    encoder_1 = architectures.CNNEncoder(
+        latent_dimensions=latent_dimensions, feature_size=(16, 16)
+    )
+    encoder_2 = architectures.CNNEncoder(
+        latent_dimensions=latent_dimensions, feature_size=(16, 16)
+    )
+    decoder_1 = architectures.CNNDecoder(
+        latent_dimensions=latent_dimensions, feature_size=(16, 16)
+    )
+    decoder_2 = architectures.CNNDecoder(
+        latent_dimensions=latent_dimensions, feature_size=(16, 16)
+    )
     # SplitAE
     splitae = SplitAE(
-        latent_dims=latent_dims, encoder=encoder_1, decoders=[decoder_1, decoder_2]
+        latent_dimensions=latent_dimensions,
+        encoder=encoder_1,
+        decoders=[decoder_1, decoder_2],
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(splitae, conv_loader)
     # DCCAE
     dccae = DCCAE(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dimensions,
         encoders=[encoder_1, encoder_2],
         decoders=[decoder_1, decoder_2],
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(dccae, conv_loader)
 
 
 def test_DVCCA_p_methods():
     max_epochs = 2
-    latent_dims = 2
+    latent_dimensions = 2
     encoder_1 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=10, variational=True
+        latent_dimensions=latent_dimensions, feature_size=10, variational=True
     )
     encoder_2 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=12, variational=True
+        latent_dimensions=latent_dimensions, feature_size=12, variational=True
     )
     private_encoder_1 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=10, variational=True
+        latent_dimensions=latent_dimensions, feature_size=10, variational=True
     )
     private_encoder_2 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=12, variational=True
+        latent_dimensions=latent_dimensions, feature_size=12, variational=True
+    )
+    decoder_1 = architectures.Decoder(
+        latent_dimensions=2 * latent_dimensions, feature_size=10
+    )
+    decoder_2 = architectures.Decoder(
+        latent_dimensions=2 * latent_dimensions, feature_size=12
     )
-    decoder_1 = architectures.Decoder(latent_dims=2 * latent_dims, feature_size=10)
-    decoder_2 = architectures.Decoder(latent_dims=2 * latent_dims, feature_size=12)
     # DVCCA
     dvcca = DVCCA(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dimensions,
         encoders=[encoder_1, encoder_2],
         decoders=[decoder_1, decoder_2],
         private_encoders=[private_encoder_1, private_encoder_2],
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(dvcca, train_loader)
     dvcca.transform(train_loader)
 
 
 def test_DVCCA_methods():
     max_epochs = 2
-    latent_dims = 2
+    latent_dimensions = 2
     encoder_1 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=10, variational=True
+        latent_dimensions=latent_dimensions, feature_size=10, variational=True
     )
     encoder_2 = architectures.Encoder(
-        latent_dims=latent_dims, feature_size=12, variational=True
+        latent_dimensions=latent_dimensions, feature_size=12, variational=True
+    )
+    decoder_1 = architectures.Decoder(
+        latent_dimensions=latent_dimensions, feature_size=10
+    )
+    decoder_2 = architectures.Decoder(
+        latent_dimensions=latent_dimensions, feature_size=12
     )
-    decoder_1 = architectures.Decoder(latent_dims=latent_dims, feature_size=10)
-    decoder_2 = architectures.Decoder(latent_dims=latent_dims, feature_size=12)
     dvcca = DVCCA(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dimensions,
         encoders=[encoder_1, encoder_2],
         decoders=[decoder_1, decoder_2],
     )
     trainer = pl.Trainer(max_epochs=max_epochs, **trainer_kwargs)
     trainer.fit(dvcca, train_loader)
```

### Comparing `cca_zoo-2.0.0/cca_zoo/test/test_kernel.py` & `cca_zoo-2.0.1/cca_zoo/test/test_kernel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 """
 Test the kernel methods
 """
 
 
 import numpy as np
-from cca_zoo.models import KCCA, KTCCA, KGCCA, MCCA, GCCA, TCCA
+from cca_zoo.classical import KCCA, KTCCA, KGCCA, MCCA, GCCA, TCCA
 
 np.random.seed(1)
 X = np.random.normal(size=(100, 10))
 Y = np.random.normal(size=(100, 10))
 Z = np.random.normal(size=(100, 10))
 
 
 # test that MCCA is the same as KCCA with linear kernel
 def test_MCCA_KCCA():
-    kcca = KCCA(latent_dims=2)
-    mcca = MCCA(latent_dims=2)
+    kcca = KCCA(latent_dimensions=2)
+    mcca = MCCA(latent_dimensions=2)
     kcca.fit([X, Y, Z])
     mcca.fit([X, Y, Z])
     mcca_score = mcca.score([X, Y, Z])
     kcca_score = kcca.score([X, Y, Z])
     assert np.allclose(mcca_score, kcca_score)
 
 
 # test that GCCA is the same as KGCCA with linear kernel
 def test_GCCA_KGCCA():
-    kgcca = KGCCA(latent_dims=2)
-    gcca = GCCA(latent_dims=2)
+    kgcca = KGCCA(latent_dimensions=2)
+    gcca = GCCA(latent_dimensions=2)
     kgcca.fit([X, Y, Z])
     gcca.fit([X, Y, Z])
     gcca_score = gcca.score([X, Y, Z])
     kgcca_score = kgcca.score([X, Y, Z])
     assert np.allclose(gcca_score, kgcca_score)
 
 
 # test that TCCA is the same as KTCCA with linear kernel
 def test_TCCA_KTCCA():
-    ktcca = KTCCA(latent_dims=2)
-    tcca = TCCA(latent_dims=2)
+    ktcca = KTCCA(latent_dimensions=2)
+    tcca = TCCA(latent_dimensions=2)
     ktcca.fit([X, Y, Z])
     tcca.fit([X, Y, Z])
     tcca_score = tcca.score([X, Y, Z])
     ktcca_score = ktcca.score([X, Y, Z])
     assert np.allclose(tcca_score, ktcca_score)
 
 
 def test_rbf_kernel():
-    kcca = KCCA(latent_dims=2, kernel="rbf").fit((X, Y, Z))
-    kgcca = KGCCA(latent_dims=2, kernel="rbf").fit((X, Y, Z))
-    ktcca = KTCCA(latent_dims=2, kernel="rbf").fit((X, Y, Z))
+    kcca = KCCA(latent_dimensions=2, kernel="rbf").fit((X, Y, Z))
+    kgcca = KGCCA(latent_dimensions=2, kernel="rbf").fit((X, Y, Z))
+    ktcca = KTCCA(latent_dimensions=2, kernel="rbf").fit((X, Y, Z))
 
 
 def test_poly_kernel():
-    kcca = KCCA(latent_dims=2, kernel="poly").fit((X, Y, Z))
-    kgcca = KGCCA(latent_dims=2, kernel="poly").fit((X, Y, Z))
-    ktcca = KTCCA(latent_dims=2, kernel="poly").fit((X, Y, Z))
+    kcca = KCCA(latent_dimensions=2, kernel="poly").fit((X, Y, Z))
+    kgcca = KGCCA(latent_dimensions=2, kernel="poly").fit((X, Y, Z))
+    ktcca = KTCCA(latent_dimensions=2, kernel="poly").fit((X, Y, Z))
 
 
 def test_sigmoid_kernel():
-    kcca = KCCA(latent_dims=2, kernel="sigmoid").fit((X, Y, Z))
-    kgcca = KGCCA(latent_dims=2, kernel="sigmoid").fit((X, Y, Z))
-    ktcca = KTCCA(latent_dims=2, kernel="sigmoid").fit((X, Y, Z))
+    kcca = KCCA(latent_dimensions=2, kernel="sigmoid").fit((X, Y, Z))
+    kgcca = KGCCA(latent_dimensions=2, kernel="sigmoid").fit((X, Y, Z))
+    ktcca = KTCCA(latent_dimensions=2, kernel="sigmoid").fit((X, Y, Z))
 
 
 def test_cosine_kernel():
-    kcca = KCCA(latent_dims=2, kernel="cosine").fit((X, Y, Z))
-    kgcca = KGCCA(latent_dims=2, kernel="cosine").fit((X, Y, Z))
-    ktcca = KTCCA(latent_dims=2, kernel="cosine").fit((X, Y, Z))
+    kcca = KCCA(latent_dimensions=2, kernel="cosine").fit((X, Y, Z))
+    kgcca = KGCCA(latent_dimensions=2, kernel="cosine").fit((X, Y, Z))
+    ktcca = KTCCA(latent_dimensions=2, kernel="cosine").fit((X, Y, Z))
 
 
 def test_callable_kernel():
     def my_kernel(X, Y, **kwargs):
         return np.dot(X, Y.T)
 
-    kcca = KCCA(latent_dims=2, kernel=my_kernel).fit((X, Y, Z))
-    kgcca = KGCCA(latent_dims=2, kernel=my_kernel).fit((X, Y, Z))
-    ktcca = KTCCA(latent_dims=2, kernel=my_kernel).fit((X, Y, Z))
+    kcca = KCCA(latent_dimensions=2, kernel=my_kernel).fit((X, Y, Z))
+    kgcca = KGCCA(latent_dimensions=2, kernel=my_kernel).fit((X, Y, Z))
+    ktcca = KTCCA(latent_dimensions=2, kernel=my_kernel).fit((X, Y, Z))
```

### Comparing `cca_zoo-2.0.0/cca_zoo/test/test_probabilistic.py` & `cca_zoo-2.0.1/cca_zoo/test/test_probabilistic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import numpy as np
 import pytest
 
 from cca_zoo.data.simulated import LinearSimulatedData
-from cca_zoo.models import CCA
+from cca_zoo.classical import CCA
 
 
 def test_PCCA():
     # some might not have access to jax/numpyro so leave this as an optional test locally.
     numpyro = pytest.importorskip("numpyro")
-    from cca_zoo.probabilisticmodels import ProbabilisticCCA
+    from cca_zoo.probabilistic import ProbabilisticCCA
 
     np.random.seed(0)
     # Tests tensor CCA methods
     X, Y = LinearSimulatedData([5, 5]).sample(100)
     latent_dims = 1
-    cca = CCA(latent_dims=latent_dims).fit([X, Y])
+    cca = CCA(latent_dimensions=latent_dims).fit([X, Y])
     pcca = ProbabilisticCCA(
-        latent_dims=latent_dims, num_warmup=1000, num_samples=1000
+        latent_dimensions=latent_dims, num_warmup=1000, num_samples=1000
     ).fit([X, Y])
     # Test that vanilla CCA and VCCA produce roughly similar latent space ie they are correlated
     assert (
         np.abs(
             np.corrcoef(
                 cca.transform([X, Y])[1].T,
                 pcca.posterior_samples["z"].mean(axis=0)[:, 0],
```

### Comparing `cca_zoo-2.0.0/cca_zoo/test/test_regularised.py` & `cca_zoo-2.0.1/cca_zoo/test/test_regularised.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import scipy.sparse as sp
 from sklearn.utils.fixes import loguniform
 from sklearn.utils.validation import check_random_state
 
 from cca_zoo.data.simulated import LinearSimulatedData
 from cca_zoo.model_selection import GridSearchCV, RandomizedSearchCV
-from cca_zoo.models import (
+from cca_zoo.classical import (
     CCA,
     GCCA,
     GRCCA,
     KCCA,
     MCCA,
     NCCA,  # SCCA_ADMM,
     PLS,
@@ -18,14 +18,15 @@
     SCCA_PMD,
     AltMaxVar,
     ElasticCCA,
     PartialCCA,
     SCCA_Parkhomenko,
     SCCA_Span,
     rCCA,
+    MPLS,
 )
 
 n = 50
 rng = check_random_state(0)
 X = rng.rand(n, 10)
 Y = rng.rand(n, 11)
 Z = rng.rand(n, 12)
@@ -44,32 +45,35 @@
     assert CCA().fit(sim_data).score(sim_data) > 0.9
 
 
 def test_regularized_methods():
     # Test that linear regularized methods match PLS solution when using maximum regularisation.
     latent_dims = 2
     c = 1
-    rcca = rCCA(latent_dims=latent_dims, c=[c, c]).fit([X, Y])
-    mcca = MCCA(latent_dims=latent_dims, c=[c, c]).fit([X, Y])
-    pls = PLS(latent_dims=latent_dims).fit([X, Y])
-    gcca = GCCA(latent_dims=latent_dims, c=[c, c]).fit([X, Y])
-    kernel = KCCA(latent_dims=latent_dims, c=[c, c], kernel=["linear", "linear"]).fit(
-        (X, Y)
-    )
+    rcca = rCCA(latent_dimensions=latent_dims, c=[c, c]).fit([X, Y])
+    mcca = MCCA(latent_dimensions=latent_dims, c=[c, c]).fit([X, Y])
+    pls = PLS(latent_dimensions=latent_dims).fit([X, Y])
+    gcca = GCCA(latent_dimensions=latent_dims, c=[c, c]).fit([X, Y])
+    kernel = KCCA(
+        latent_dimensions=latent_dims, c=[c, c], kernel=["linear", "linear"]
+    ).fit((X, Y))
+    mpls = MPLS(latent_dimensions=latent_dims).fit([X, Y])
     corr_gcca = gcca.score((X, Y))
     corr_mcca = mcca.score((X, Y))
     corr_kernel = kernel.score((X, Y))
     corr_pls = pls.score((X, Y))
     corr_rcca = rcca.score((X, Y))
+    corr_mpls = mpls.score((X, Y))
     # Check the correlations from each unregularized method are the same
     assert np.testing.assert_array_almost_equal(corr_pls, corr_mcca, decimal=1) is None
     assert (
         np.testing.assert_array_almost_equal(corr_pls, corr_kernel, decimal=1) is None
     )
     assert np.testing.assert_array_almost_equal(corr_pls, corr_rcca, decimal=1) is None
+    assert np.testing.assert_array_almost_equal(corr_pls, corr_mpls, decimal=1) is None
 
 
 def test_sparse_methods():
     tau1 = [5e-1]
     tau2 = [5e-1]
     param_grid = {"tau": [tau1, tau2]}
     pdd_cv = GridSearchCV(
@@ -117,79 +121,79 @@
     assert (elastic_cv.best_estimator_.weights[1] == 0).sum() > 0
 
 
 def test_weighted_GCCA_methods():
     # TODO we have view weighted GCCA and missing observation GCCA
     latent_dims = 2
     c = 0
-    unweighted_gcca = GCCA(latent_dims=latent_dims, c=[c, c]).fit([X, Y])
+    unweighted_gcca = GCCA(latent_dimensions=latent_dims, c=[c, c]).fit([X, Y])
     deweighted_gcca = GCCA(
-        latent_dims=latent_dims, c=[c, c], view_weights=[0.5, 0.5]
+        latent_dimensions=latent_dims, c=[c, c], view_weights=[0.5, 0.5]
     ).fit([X, Y])
     corr_unweighted_gcca = unweighted_gcca.score((X, Y))
     corr_deweighted_gcca = deweighted_gcca.score((X, Y))
     # Check the correlations from each unregularized method are the same
     K = np.ones((2, X.shape[0]))
     K[0, 200:] = 0
-    unobserved_gcca = GCCA(latent_dims=latent_dims, c=[c, c]).fit((X, Y), K=K)
+    unobserved_gcca = GCCA(latent_dimensions=latent_dims, c=[c, c]).fit((X, Y), K=K)
     assert (
         np.testing.assert_array_almost_equal(
             corr_unweighted_gcca, corr_deweighted_gcca, decimal=1
         )
         is None
     )
 
 
 def test_NCCA():
     latent_dims = 1
-    ncca = NCCA(latent_dims=latent_dims).fit((X, Y))
+    ncca = NCCA(latent_dimensions=latent_dims).fit((X, Y))
     corr_ncca = ncca.score((X, Y))
     assert corr_ncca > 0.9
 
 
 def test_l0():
     span_cca = SCCA_Span(
-        latent_dims=1, regularisation="l0", tau=[2, 2], random_state=rng
+        latent_dimensions=1, regularisation="l0", tau=[2, 2], random_state=rng
     ).fit([X, Y])
     # swcca = SWCCA(tau=[5, 5], sample_support=5, random_state=rng).fit([X, Y])
     assert (np.abs(span_cca.weights[0]) > 1e-5).sum() == 2
     assert (np.abs(span_cca.weights[1]) > 1e-5).sum() == 2
     # assert (np.abs(swcca.weights[0]) > 1e-5).sum() == 5
     # assert (np.abs(swcca.weights[1]) > 1e-5).sum() == 5
     # assert (np.abs(swcca.sample_weights) > 1e-5).sum() == 5
 
 
 def test_partialcca():
     # Tests that partial CCA scores are not correlated with partials
-    pcca = PartialCCA(latent_dims=3)
+    pcca = PartialCCA(latent_dimensions=3)
     pcca.fit((X, Y), partials=Z)
     assert np.allclose(
         np.corrcoef(pcca.transform((X, Y), partials=Z)[0], Z, rowvar=False)[:3, :3]
         - np.eye(3),
         0,
         atol=0.001,
     )
 
 
 def test_PRCCA():
     # Test that PRCCA works
-    prcca = PRCCA(latent_dims=2, c=[0, 0]).fit(
+    prcca = PRCCA(latent_dimensions=2, c=[0, 0]).fit(
         (X, Y), idxs=(np.arange(10), np.arange(11))
     )
-    cca = CCA(latent_dims=2).fit([X, Y])
+    cca = CCA(latent_dimensions=2).fit([X, Y])
     assert (
         np.testing.assert_array_almost_equal(
             cca.score((X, Y)), prcca.score((X, Y)), decimal=1
         )
         is None
     )
-    prcca = PRCCA(latent_dims=2, c=[1, 1]).fit(
+    prcca = PRCCA(latent_dimensions=2, c=[1, 1]).fit(
         (X, Y), idxs=(np.arange(10), np.arange(11))
     )
-    pls = PLS(latent_dims=2).fit([X, Y])
+    pls = PLS(latent_dimensions=2).fit([X, Y])
     assert (
         np.testing.assert_array_almost_equal(
             pls.score((X, Y)), prcca.score((X, Y)), decimal=1
         )
         is None
     )
 
@@ -201,15 +205,31 @@
     feature_group_2 = np.zeros(Y.shape[1], dtype=int)
     feature_group_2[:3] = 1
     feature_group_2[3:6] = 2
     feature_group_3 = np.zeros(Z.shape[1], dtype=int)
     feature_group_3[:3] = 1
     feature_group_3[3:6] = 2
     # Test that GRCCA works
-    grcca = GRCCA(latent_dims=1, c=[100, 0], mu=0).fit(
+    grcca = GRCCA(latent_dimensions=1, c=[100, 0], mu=0).fit(
         (X, Y), feature_groups=[feature_group_1, feature_group_2]
     )
     grcca.score((X, Y))
     grcca.transform((X, Y))
     grcca = GRCCA(c=[100, 0, 50]).fit(
         (X, Y, Z), feature_groups=[feature_group_1, feature_group_2, feature_group_3]
     )
+
+
+def test_deflation():
+    # test deflation works with pls and cca using SCCA_PMD
+    ccamodel = SCCA_PMD(latent_dimensions=2, tau=1, random_state=rng, deflation="cca")
+    ccamodel.fit([X, Y])
+    pls = PLS(latent_dimensions=2)
+    pls.fit([X, Y])
+    plsmodel = SCCA_PMD(latent_dimensions=2, tau=1, random_state=rng, deflation="pls")
+    plsmodel.fit([X, Y])
+    assert (
+        np.testing.assert_array_almost_equal(
+            pls.score((X, Y)), plsmodel.score((X, Y)), decimal=1
+        )
+        is None
+    )
```

### Comparing `cca_zoo-2.0.0/cca_zoo/test/test_stochastic.py` & `cca_zoo-2.0.1/cca_zoo/test/test_stochastic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pytest
 import scipy.sparse as sp
 from sklearn.utils import check_random_state
 
-from cca_zoo.models import CCA, PLS, MCCA
+from cca_zoo.classical import CCA, PLS, MCCA
 
 n = 50
 rng = check_random_state(0)
 X = rng.rand(n, 10)
 Y = rng.rand(n, 11)
 Z = rng.rand(n, 12)
 X_sp = sp.random(n, 10, density=0.5, random_state=rng)
@@ -32,38 +32,38 @@
     return np.sign(obj) * np.log(np.abs(obj) + 1e-10)
 
 
 def test_stochastic_pls():
     pytest.importorskip("torch")
     from torch import manual_seed
 
-    from cca_zoo.models import PLSEY, PLSSVD, PLSStochasticPower
+    from cca_zoo.classical import PLSEY, PLSSVD, PLSStochasticPower
 
-    pls = PLS(latent_dims=3).fit((X, Y))
+    pls = PLS(latent_dimensions=3).fit((X, Y))
     manual_seed(42)
     plsey = PLSEY(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
         track=True,
         verbose=False,
     ).fit((X, Y))
     plssvd = PLSSVD(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
         track=True,
         verbose=False,
     ).fit((X, Y))
     spls = PLSStochasticPower(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
         track=True,
         verbose=False,
     ).fit((X, Y))
@@ -82,37 +82,37 @@
     assert np.allclose(np.trace(pls_score), np.trace(spls_score), atol=1e-1)
     assert np.allclose(np.trace(pls_score), np.trace(plsey_score), atol=1e-1)
     assert np.allclose(np.trace(pls_score), np.trace(plssvd_score), atol=1e-1)
 
 
 def test_stochastic_cca():
     pytest.importorskip("torch")
-    from cca_zoo.models import CCAEY, CCAGH, CCASVD
+    from cca_zoo.classical import CCAEY, CCAGH, CCASVD
 
-    cca = CCA(latent_dims=3).fit((X, Y))
+    cca = CCA(latent_dimensions=3).fit((X, Y))
     ccaey = CCAEY(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
         track=True,
         verbose=False,
     ).fit((X, Y))
     ccagh = CCAGH(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
         track=True,
         verbose=False,
     ).fit((X, Y))
     ccasvd = CCASVD(
-        latent_dims=latent_dims,
+        latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
         track=True,
         verbose=False,
     ).fit((X, Y))
```

### Comparing `cca_zoo-2.0.0/cca_zoo/test/test_unregularized.py` & `cca_zoo-2.0.1/cca_zoo/test/test_unregularized.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import scipy.sparse as sp
 from sklearn.utils.validation import check_random_state
 
-from cca_zoo.models import (
+from cca_zoo.classical import (
     CCA,
     GCCA,
     KCCA,
     KGCCA,
     KTCCA,
     MCCA,
     PLS,
@@ -30,23 +30,23 @@
 X_sp -= X_sp.mean(axis=0)
 Y_sp -= Y_sp.mean(axis=0)
 
 
 def test_unregularized_methods():
     # This function tests unregularized CCA methods. The idea is that all of these should give the same result.
     latent_dims = 2
-    rcca = rCCA(latent_dims=latent_dims).fit([X, Y])
-    cca = CCA(latent_dims=latent_dims).fit([X, Y])
-    gcca = GCCA(latent_dims=latent_dims).fit([X, Y])
-    mcca = MCCA(latent_dims=latent_dims, pca=False).fit([X, Y])
-    mcca_pca = MCCA(latent_dims=latent_dims, pca=True).fit([X, Y])
-    kcca = KCCA(latent_dims=latent_dims).fit([X, Y])
-    kgcca = KGCCA(latent_dims=latent_dims).fit([X, Y])
-    tcca = TCCA(latent_dims=latent_dims).fit([X, Y])
-    pcacca = PCACCA(latent_dims=latent_dims).fit([X, Y])
+    rcca = rCCA(latent_dimensions=latent_dims).fit([X, Y])
+    cca = CCA(latent_dimensions=latent_dims).fit([X, Y])
+    gcca = GCCA(latent_dimensions=latent_dims).fit([X, Y])
+    mcca = MCCA(latent_dimensions=latent_dims, pca=False).fit([X, Y])
+    mcca_pca = MCCA(latent_dimensions=latent_dims, pca=True).fit([X, Y])
+    kcca = KCCA(latent_dimensions=latent_dims).fit([X, Y])
+    kgcca = KGCCA(latent_dimensions=latent_dims).fit([X, Y])
+    tcca = TCCA(latent_dimensions=latent_dims).fit([X, Y])
+    pcacca = PCACCA(latent_dimensions=latent_dims).fit([X, Y])
 
     # Get the correlation scores for each method
     corr_rcca = rcca.score((X, Y))
     corr_cca = cca.score((X, Y))
     corr_gcca = gcca.score((X, Y))
     corr_mcca = mcca.score((X, Y))
     corr_mcca_pca = mcca_pca.score((X, Y))
@@ -64,17 +64,17 @@
         np.testing.assert_array_almost_equal(corr_kgcca, corr_gcca, decimal=1) is None
     )
 
 
 def test_unregularized_multi():
     # This function tests unregularized CCA methods for more than 2 views. The idea is that all of these should give the same result.
     latent_dims = 2
-    gcca = GCCA(latent_dims=latent_dims).fit((X, Y, Z))
-    mcca = MCCA(latent_dims=latent_dims).fit((X, Y, Z))
-    kcca = KCCA(latent_dims=latent_dims).fit((X, Y, Z))
+    gcca = GCCA(latent_dimensions=latent_dims).fit((X, Y, Z))
+    mcca = MCCA(latent_dimensions=latent_dims).fit((X, Y, Z))
+    kcca = KCCA(latent_dimensions=latent_dims).fit((X, Y, Z))
     # Get the correlation scores for each method
     corr_gcca = gcca.score((X, Y, Z))
     corr_mcca = mcca.score((X, Y, Z))
     corr_kcca = kcca.score((X, Y, Z))
 
     # Assert that the correlation scores are all equal
     assert np.testing.assert_array_almost_equal(corr_mcca, corr_gcca, decimal=1) is None
@@ -87,33 +87,33 @@
     # Assert that the correlation scores are all equal
     assert np.testing.assert_array_almost_equal(corr_mcca, corr_gcca, decimal=1) is None
     assert np.testing.assert_array_almost_equal(corr_mcca, corr_kcca, decimal=1) is None
 
 
 def test_pls():
     # This function tests PLS and PLS_ALS
-    pls_als = PLS_ALS(latent_dims=3, random_state=0)
-    pls = PLS(latent_dims=3)
+    pls_als = PLS_ALS(latent_dimensions=3, random_state=0)
+    pls = PLS(latent_dimensions=3)
 
-    # Fit both models to the same data
+    # Fit both classical to the same data
     pls_als.fit([X, Y])
     pls.fit((X, Y))
 
     # Assert that the scores are close
     pls_score = pls.score((X, Y))
     pls_als_score = pls_als.score((X, Y))
 
     assert np.allclose(np.abs(pls_als_score), pls_score, rtol=1e-1)
 
 
 def test_TCCA():
     # This function tests TCCA and KTCCA
     latent_dims = 1
-    tcca = TCCA(latent_dims=latent_dims, c=[0.2, 0.2, 0.2]).fit([X, X, Y])
-    ktcca = KTCCA(latent_dims=latent_dims, c=[0.2, 0.2]).fit([X, Y])
+    tcca = TCCA(latent_dimensions=latent_dims, c=[0.2, 0.2, 0.2]).fit([X, X, Y])
+    ktcca = KTCCA(latent_dimensions=latent_dims, c=[0.2, 0.2]).fit([X, Y])
 
     # Get the correlation scores for each method
     corr_tcca = tcca.score((X, X, Y))
     corr_ktcca = ktcca.score((X, Y))
 
     # Assert that the correlation scores are greater than 0.1
     assert corr_tcca > 0.1
```

### Comparing `cca_zoo-2.0.0/cca_zoo/utils/check_values.py` & `cca_zoo-2.0.1/cca_zoo/utils/check_values.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.0/cca_zoo.egg-info/PKG-INFO` & `cca_zoo-2.0.1/cca_zoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca-zoo
-Version: 2.0.0
+Version: 2.0.1
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.0/examples/__init__.py` & `cca_zoo-2.0.1/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.0/examples/plot_dcca.py` & `cca_zoo-2.0.1/examples/plot_dcca.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,72 +1,76 @@
 """
 Deep CCA
 ===========================
 
-This example demonstrates how to easily train Deep CCA models and variants
+This example demonstrates how to easily train Deep CCA classical and variants
 """
 
 import pytorch_lightning as pl
 from matplotlib import pyplot as plt
 
 # %%
-from cca_zoo.deepmodels import (
+from cca_zoo.deep import (
     DCCA,
     DCCA_EY,
     DCCA_NOI,
     DCCA_SDL,
     BarlowTwins,
     architectures,
 )
-from cca_zoo.plotting import pairplot_label
+from cca_zoo.visualisation import pairplot_label
 from examples import example_mnist_data
 
 # %%
 # Data
 # -----
 LATENT_DIMS = 2
 EPOCHS = 10
 N_TRAIN = 500
 N_VAL = 100
 
 train_loader, val_loader, train_labels = example_mnist_data(N_TRAIN, N_VAL)
 
-encoder_1 = architectures.Encoder(latent_dims=LATENT_DIMS, feature_size=392)
-encoder_2 = architectures.Encoder(latent_dims=LATENT_DIMS, feature_size=392)
+encoder_1 = architectures.Encoder(latent_dimensions=LATENT_DIMS, feature_size=392)
+encoder_2 = architectures.Encoder(latent_dimensions=LATENT_DIMS, feature_size=392)
 
 # %%
 # Deep CCA
 # ----------------------------
-dcca = DCCA(latent_dims=LATENT_DIMS, encoders=[encoder_1, encoder_2])
+dcca = DCCA(latent_dimensions=LATENT_DIMS, encoders=[encoder_1, encoder_2])
 trainer = pl.Trainer(
     max_epochs=EPOCHS,
     enable_checkpointing=False,
     log_every_n_steps=1,
 )
 trainer.fit(dcca, train_loader, val_loader)
 pairplot_label(dcca.transform(train_loader), train_labels, title="DCCA")
 plt.show()
 
 # %%
 # Deep CCA EigenGame
 # ----------------------------
-dcca_eg = DCCA_EY(latent_dims=LATENT_DIMS, encoders=[encoder_1, encoder_2], lr=1e-5)
+dcca_eg = DCCA_EY(
+    latent_dimensions=LATENT_DIMS, encoders=[encoder_1, encoder_2], lr=1e-5
+)
 trainer = pl.Trainer(
     max_epochs=EPOCHS,
     enable_checkpointing=False,
     log_every_n_steps=1,
 )
 trainer.fit(dcca_eg, train_loader, val_loader)
 pairplot_label(dcca_eg.transform(train_loader), train_labels, title="DCCA-EigenGame")
 plt.show()
 
 # %%
 # Deep CCA by Non-Linear Orthogonal Iterations
 # ----------------------------------------------
-dcca_noi = DCCA_NOI(latent_dims=LATENT_DIMS, N=N_TRAIN, encoders=[encoder_1, encoder_2])
+dcca_noi = DCCA_NOI(
+    latent_dimensions=LATENT_DIMS, N=N_TRAIN, encoders=[encoder_1, encoder_2]
+)
 trainer = pl.Trainer(
     max_epochs=EPOCHS,
     enable_checkpointing=False,
     log_every_n_steps=1,
 )
 trainer.fit(dcca_noi, train_loader, val_loader)
 pairplot_label(
@@ -75,15 +79,17 @@
     title="DCCA by Non-Linear Orthogonal Iterations",
 )
 plt.show()
 
 # %%
 # Deep CCA by Stochastic Decorrelation Loss
 # ----------------------------------------------
-dcca_sdl = DCCA_SDL(latent_dims=LATENT_DIMS, N=N_TRAIN, encoders=[encoder_1, encoder_2])
+dcca_sdl = DCCA_SDL(
+    latent_dimensions=LATENT_DIMS, N=N_TRAIN, encoders=[encoder_1, encoder_2]
+)
 trainer = pl.Trainer(
     max_epochs=EPOCHS,
     enable_checkpointing=False,
     log_every_n_steps=1,
 )
 trainer.fit(dcca_sdl, train_loader, val_loader)
 pairplot_label(
@@ -92,15 +98,17 @@
     title="DCCA by Stochastic Decorrelation",
 )
 plt.show()
 
 # %%
 # Deep CCA by Barlow Twins
 # ----------------------------------------------
-barlowtwins = BarlowTwins(latent_dims=LATENT_DIMS, encoders=[encoder_1, encoder_2])
+barlowtwins = BarlowTwins(
+    latent_dimensions=LATENT_DIMS, encoders=[encoder_1, encoder_2]
+)
 trainer = pl.Trainer(
     max_epochs=EPOCHS,
     enable_checkpointing=False,
     log_every_n_steps=1,
 )
 trainer.fit(barlowtwins, train_loader, val_loader)
 pairplot_label(
```

### Comparing `cca_zoo-2.0.0/examples/plot_dcca_custom_data.py` & `cca_zoo-2.0.1/examples/plot_dcca_custom_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # This is arguably the easiest way to
 # use your own data with CCA-Zoo. You can use the NumpyDataset class to convert your data into a valid dataset. This
 # class takes in a list of numpy arrays, each representing a view. It also takes in a list of labels, which can be
 # None if you don't have labels. The NumpyDataset class will automatically convert your data into a valid dataset.
 # You can then use the get_dataloaders function to convert your dataset into dataloaders, which can be used with
 # CCA-Zoo.
 from cca_zoo.data.deep import NumpyDataset
-from cca_zoo.deepmodels import DCCA, architectures
+from cca_zoo.deep import DCCA, architectures
 
 X = np.random.normal(size=(100, 10))
 Y = np.random.normal(size=(100, 10))
 Z = np.random.normal(size=(100, 10))
 numpy_dataset = NumpyDataset([X, Y, Z], labels=None)
 
 # %% Checking the dataset
@@ -68,20 +68,20 @@
 
 # %%
 # Training
 # -----
 LATENT_DIMS = 1
 EPOCHS = 10
 
-encoder_1 = architectures.Encoder(latent_dims=LATENT_DIMS, feature_size=10)
-encoder_2 = architectures.Encoder(latent_dims=LATENT_DIMS, feature_size=10)
+encoder_1 = architectures.Encoder(latent_dimensions=LATENT_DIMS, feature_size=10)
+encoder_2 = architectures.Encoder(latent_dimensions=LATENT_DIMS, feature_size=10)
 
 # %%
 # Deep CCA
 # ----------------------------
-dcca = DCCA(latent_dims=LATENT_DIMS, encoders=[encoder_1, encoder_2])
+dcca = DCCA(latent_dimensions=LATENT_DIMS, encoders=[encoder_1, encoder_2])
 trainer = pl.Trainer(
     max_epochs=EPOCHS,
     enable_checkpointing=False,
     log_every_n_steps=1,
 )
 trainer.fit(dcca, train_loader)
```

### Comparing `cca_zoo-2.0.0/examples/plot_dcca_multi.py` & `cca_zoo-2.0.1/examples/plot_dcca_multi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 """
 Deep CCA for more than 2 views
 =================================
 
-This example demonstrates how to easily train Deep CCA models and variants
+This example demonstrates how to easily train Deep CCA classical and variants
 """
 
 import pytorch_lightning as pl
 
-from cca_zoo.deepmodels import DCCA, DTCCA, architectures, objectives
+from cca_zoo.deep import DCCA, DTCCA, architectures, objectives
 
 # %%
 # Data
 # -----
 from examples import example_mnist_data
 
 LATENT_DIMS = 2
 EPOCHS = 10
 N_TRAIN = 500
 N_VAL = 100
 
 train_loader, val_loader, train_labels = example_mnist_data(N_TRAIN, N_VAL)
 
-encoder_1 = architectures.Encoder(latent_dims=LATENT_DIMS, feature_size=392)
-encoder_2 = architectures.Encoder(latent_dims=LATENT_DIMS, feature_size=392)
+encoder_1 = architectures.Encoder(latent_dimensions=LATENT_DIMS, feature_size=392)
+encoder_2 = architectures.Encoder(latent_dimensions=LATENT_DIMS, feature_size=392)
 
 # %%
 # Deep MCCA
 # ----------
 dcca = DCCA(
-    latent_dims=LATENT_DIMS, encoders=[encoder_1, encoder_2], objective=objectives.MCCA
+    latent_dimensions=LATENT_DIMS,
+    encoders=[encoder_1, encoder_2],
+    objective=objectives.MCCA,
 )
 trainer = pl.Trainer(max_epochs=EPOCHS, enable_checkpointing=False)
 trainer.fit(dcca, train_loader, val_loader)
 
 # %%
 # Deep GCCA
 # ---------
 dcca = DCCA(
-    latent_dims=LATENT_DIMS, encoders=[encoder_1, encoder_2], objective=objectives.GCCA
+    latent_dimensions=LATENT_DIMS,
+    encoders=[encoder_1, encoder_2],
+    objective=objectives.GCCA,
 )
 trainer = pl.Trainer(max_epochs=EPOCHS, enable_checkpointing=False)
 trainer.fit(dcca, train_loader, val_loader)
 
 # %%
 # Deep TCCA
 # ---------
-dcca = DTCCA(latent_dims=LATENT_DIMS, encoders=[encoder_1, encoder_2])
+dcca = DTCCA(latent_dimensions=LATENT_DIMS, encoders=[encoder_1, encoder_2])
 trainer = pl.Trainer(max_epochs=EPOCHS, enable_checkpointing=False)
 trainer.fit(dcca, train_loader, val_loader)
```

### Comparing `cca_zoo-2.0.0/examples/plot_dvcca.py` & `cca_zoo-2.0.1/examples/plot_dvcca.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Deep Variational CCA and Deep Canonically Correlated Autoencoders
 ====================================================================
 
-This example demonstrates multiview models which can reconstruct their inputs
+This example demonstrates multiview classical which can reconstruct their inputs
 """
 import matplotlib.pyplot as plt
 import pytorch_lightning as pl
 
-from cca_zoo.deepmodels import DCCAE, DVCCA, SplitAE, architectures
-from cca_zoo.plotting import tsne_label
+from cca_zoo.deep import DCCAE, DVCCA, SplitAE, architectures
+from cca_zoo.visualisation import tsne_label
 from examples import example_mnist_data
 
 
 def plot_reconstruction(model, loader):
     recons = model.recon(loader, mle=True)
     originals = loader.dataset.dataset[0]["views"]
     n_cols = 2
@@ -39,28 +39,34 @@
     N_TRAIN, N_VAL, type="noisy"
 )
 
 # %%
 # Deep Variational CCA
 # ----------------------------
 encoder_1 = architectures.Encoder(
-    latent_dims=LATENT_DIMS,
+    latent_dimensions=LATENT_DIMS,
     feature_size=784,
     variational=True,
     layer_sizes=layer_sizes,
     dropout=dropout,
 )
 decoder_1 = architectures.Decoder(
-    latent_dims=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes, dropout=dropout
+    latent_dimensions=LATENT_DIMS,
+    feature_size=784,
+    layer_sizes=layer_sizes,
+    dropout=dropout,
 )
 decoder_2 = architectures.Decoder(
-    latent_dims=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes, dropout=dropout
+    latent_dimensions=LATENT_DIMS,
+    feature_size=784,
+    layer_sizes=layer_sizes,
+    dropout=dropout,
 )
 dvcca = DVCCA(
-    latent_dims=LATENT_DIMS,
+    latent_dimensions=LATENT_DIMS,
     encoders=[encoder_1],
     decoders=[decoder_1, decoder_2],
     lr=lr,
 )
 trainer = pl.Trainer(
     max_epochs=EPOCHS,
     enable_checkpointing=False,
@@ -72,41 +78,41 @@
 plt.suptitle("DVCCA")
 plt.show()
 
 # %%
 # Deep Variational CCA (Private)
 # -------------------------------
 private_encoder_1 = architectures.Encoder(
-    latent_dims=LATENT_DIMS,
+    latent_dimensions=LATENT_DIMS,
     feature_size=784,
     variational=True,
     layer_sizes=layer_sizes,
     dropout=dropout,
 )
 private_encoder_2 = architectures.Encoder(
-    latent_dims=LATENT_DIMS,
+    latent_dimensions=LATENT_DIMS,
     feature_size=784,
     variational=True,
     layer_sizes=layer_sizes,
     dropout=dropout,
 )
 private_decoder_1 = architectures.Decoder(
-    latent_dims=2 * LATENT_DIMS,
+    latent_dimensions=2 * LATENT_DIMS,
     feature_size=784,
     layer_sizes=layer_sizes,
     dropout=dropout,
 )
 private_decoder_2 = architectures.Decoder(
-    latent_dims=2 * LATENT_DIMS,
+    latent_dimensions=2 * LATENT_DIMS,
     feature_size=784,
     layer_sizes=layer_sizes,
     dropout=dropout,
 )
 dvccap = DVCCA(
-    latent_dims=LATENT_DIMS,
+    latent_dimensions=LATENT_DIMS,
     encoders=[encoder_1],
     decoders=[private_decoder_1, private_decoder_2],
     private_encoders=[private_encoder_1, private_encoder_2],
     lr=lr,
 )
 trainer = pl.Trainer(
     max_epochs=EPOCHS,
@@ -119,27 +125,33 @@
 plt.suptitle("DVCCA Private")
 plt.show()
 
 # %%
 # Deep Canonically Correlated Autoencoders
 # -----------------------------------------
 encoder_1 = architectures.Encoder(
-    latent_dims=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes
+    latent_dimensions=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes
 )
 encoder_2 = architectures.Encoder(
-    latent_dims=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes
+    latent_dimensions=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes
 )
 decoder_1 = architectures.Decoder(
-    latent_dims=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes, dropout=dropout
+    latent_dimensions=LATENT_DIMS,
+    feature_size=784,
+    layer_sizes=layer_sizes,
+    dropout=dropout,
 )
 decoder_2 = architectures.Decoder(
-    latent_dims=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes, dropout=dropout
+    latent_dimensions=LATENT_DIMS,
+    feature_size=784,
+    layer_sizes=layer_sizes,
+    dropout=dropout,
 )
 dccae = DCCAE(
-    latent_dims=LATENT_DIMS,
+    latent_dimensions=LATENT_DIMS,
     encoders=[encoder_1, encoder_2],
     decoders=[decoder_1, decoder_2],
     lr=lr,
     lam=0.5,
     optimizer="adam",
 )
 trainer = pl.Trainer(
@@ -153,24 +165,30 @@
 plt.suptitle("DCCAE")
 plt.show()
 
 # %%
 # Split Autoencoders
 # -------------------
 encoder_1 = architectures.Encoder(
-    latent_dims=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes
+    latent_dimensions=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes
 )
 decoder_1 = architectures.Decoder(
-    latent_dims=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes, dropout=dropout
+    latent_dimensions=LATENT_DIMS,
+    feature_size=784,
+    layer_sizes=layer_sizes,
+    dropout=dropout,
 )
 decoder_2 = architectures.Decoder(
-    latent_dims=LATENT_DIMS, feature_size=784, layer_sizes=layer_sizes, dropout=dropout
+    latent_dimensions=LATENT_DIMS,
+    feature_size=784,
+    layer_sizes=layer_sizes,
+    dropout=dropout,
 )
 splitae = SplitAE(
-    latent_dims=LATENT_DIMS,
+    latent_dimensions=LATENT_DIMS,
     encoder=encoder_1,
     decoders=[decoder_1, decoder_2],
     lr=lr,
     optimizer="adam",
 )
 trainer = pl.Trainer(
     max_epochs=EPOCHS,
```

### Comparing `cca_zoo-2.0.0/examples/plot_hyperparameter_selection.py` & `cca_zoo-2.0.1/examples/plot_hyperparameter_selection.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # %%
 import numpy as np
 import pandas as pd
 from sklearn.utils.fixes import loguniform
 
 from cca_zoo.data.simulated import LinearSimulatedData
 from cca_zoo.model_selection import GridSearchCV, RandomizedSearchCV
-from cca_zoo.models import KCCA
+from cca_zoo.classical import KCCA
 
 # %%
 # Data
 # ------
 np.random.seed(42)
 n = 200
 p = 100
@@ -38,24 +38,27 @@
 # We form a parameter grid with the search space for each view for each parameter.
 # This search space must be entered as a list but can be any of
 #  - a single value (as in "kernel") where this value will be used for each view
 #  - a list for each view
 #  - a mixture of a single value for one view and a distribution or list for the other
 param_grid = {"kernel": ["poly"], "c": [[1e-1], [1e-1, 2e-1]], "degree": [[2], [2, 3]]}
 kernel_reg = GridSearchCV(
-    KCCA(latent_dims=latent_dims), param_grid=param_grid, cv=cv, verbose=True
+    KCCA(latent_dimensions=latent_dims), param_grid=param_grid, cv=cv, verbose=True
 ).fit([X, Y])
 print(pd.DataFrame(kernel_reg.cv_results_))
 
 # %%
 # Randomized Search
 # --------------------
 # With Randomized Search we can additionally use distributions from scikit-learn to define the parameter search space
 param_grid = {
     "kernel": ["poly"],
     "c": [loguniform(1e-1, 2e-1), [1e-1]],
     "degree": [[2], [2, 3]],
 }
 kernel_reg = RandomizedSearchCV(
-    KCCA(latent_dims=latent_dims), param_distributions=param_grid, cv=cv, verbose=True
+    KCCA(latent_dimensions=latent_dims),
+    param_distributions=param_grid,
+    cv=cv,
+    verbose=True,
 ).fit([X, Y])
 print(pd.DataFrame(kernel_reg.cv_results_))
```

### Comparing `cca_zoo-2.0.0/examples/plot_kernel_cca.py` & `cca_zoo-2.0.1/examples/plot_kernel_cca.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 # %%
 import numpy as np
 
 from cca_zoo.data.simulated import LinearSimulatedData
 from cca_zoo.model_selection import GridSearchCV
-from cca_zoo.models import KCCA
+from cca_zoo.classical import KCCA
 
 # %%
 # Data
 # -----
 np.random.seed(42)
 n = 200
 p = 100
@@ -35,49 +35,49 @@
 
     """
 
     return np.random.normal(0, param)
 
 
 kernel_custom = KCCA(
-    latent_dims=latent_dims,
+    latent_dimensions=latent_dims,
     kernel=[my_kernel, my_kernel],
     kernel_params=[{"param": 1}, {"param": 1}],
 ).fit([X, Y])
 
 # %%
 # Linear
 c1 = [0.9, 0.99]
 c2 = [0.9, 0.99]
 param_grid = {"kernel": ["linear"], "c": [c1, c2]}
 kernel_reg = GridSearchCV(
-    KCCA(latent_dims=latent_dims), param_grid=param_grid, cv=cv, verbose=True
+    KCCA(latent_dimensions=latent_dims), param_grid=param_grid, cv=cv, verbose=True
 ).fit([X, Y])
 
 # %%
 # Polynomial
 degree1 = [2, 3]
 degree2 = [2, 3]
 param_grid = {"kernel": ["poly"], "degree": [degree1, degree2], "c": [c1, c2]}
 kernel_poly = (
     GridSearchCV(
-        KCCA(latent_dims=latent_dims), param_grid=param_grid, cv=cv, verbose=True
+        KCCA(latent_dimensions=latent_dims), param_grid=param_grid, cv=cv, verbose=True
     )
     .fit([X, Y])
     .best_estimator_
 )
 
 # %%
 # kernel cca (gaussian/rbf)
 gamma1 = [1e-1, 1e-2]
 gamma2 = [1e-1, 1e-2]
 param_grid = {"kernel": ["rbf"], "gamma": [gamma1, gamma2], "c": [c1, c2]}
 kernel_poly = (
     GridSearchCV(
-        KCCA(latent_dims=latent_dims), param_grid=param_grid, cv=cv, verbose=True
+        KCCA(latent_dimensions=latent_dims), param_grid=param_grid, cv=cv, verbose=True
     )
     .fit([X, Y])
     .best_estimator_
 )
 
 
 # %%
@@ -88,11 +88,11 @@
 
     """
     M = np.random.rand(X.shape[0], X.shape[0]) + param
     return X @ M @ M.T @ Y.T
 
 
 kernel_custom = KCCA(
-    latent_dims=latent_dims,
+    latent_dimensions=latent_dims,
     kernel=[my_kernel, my_kernel],
     kernel_params=[{"param": 1}, {"param": 1}],
 ).fit([X, Y])
```

### Comparing `cca_zoo-2.0.0/examples/plot_many_views.py` & `cca_zoo-2.0.1/examples/plot_many_views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 More than 2 views
 ===========================
 
-This will compare MCCA, GCCA, TCCA for linear models with more than 2 views
+This will compare MCCA, GCCA, TCCA for linear classical with more than 2 views
 """
 import numpy as np
 
 from cca_zoo.data.simulated import LinearSimulatedData
-from cca_zoo.models import GCCA, KCCA, KGCCA, KTCCA, MCCA, SCCA_PMD, TCCA
+from cca_zoo.classical import GCCA, KCCA, KGCCA, KTCCA, MCCA, SCCA_PMD, TCCA
 
 """
 Data
 -----
 """
 # %%
 np.random.seed(42)
@@ -31,42 +31,44 @@
 # ---------------------------------
 
 # %%
 # Linear
 # ^^^^^^^^
 
 # %%
-mcca = MCCA(latent_dims=latent_dims).fit((X, Y, X)).score((X, Y, Z))
+mcca = MCCA(latent_dimensions=latent_dims).fit((X, Y, X)).score((X, Y, Z))
 
 # %%
-gcca = GCCA(latent_dims=latent_dims).fit((X, Y, X)).score((X, Y, Z))
+gcca = GCCA(latent_dimensions=latent_dims).fit((X, Y, X)).score((X, Y, Z))
 
 # %%
 # Kernel
 # ^^^^^^^^
 
 # %%
-kcca = KCCA(latent_dims=latent_dims).fit((X, Y, X)).score((X, Y, Z))
+kcca = KCCA(latent_dimensions=latent_dims).fit((X, Y, X)).score((X, Y, Z))
 
 # %%
-kgcca = KGCCA(latent_dims=latent_dims).fit((X, Y, X)).score((X, Y, Z))
+kgcca = KGCCA(latent_dimensions=latent_dims).fit((X, Y, X)).score((X, Y, Z))
 
 # %%
 # Iterative Methods
 # ^^^^^^^^^^^^^^^^^^
 
 # Most of the _iterative methods can also use multiple views e.g.
 
 pmd = (
-    SCCA_PMD(latent_dims=latent_dims, tau=0.1, tol=1e-5).fit((X, Y, X)).score((X, Y, Z))
+    SCCA_PMD(latent_dimensions=latent_dims, tau=0.1, tol=1e-5)
+    .fit((X, Y, X))
+    .score((X, Y, Z))
 )
 
 # %%
 # Higher Order Correlations
 # -------------------------
 
 # %%
 # Tensor CCA finds higher order correlations so scores are not comparable (but TCCA is equivalent for 2 views)
-tcca = TCCA(latent_dims=latent_dims).fit((X, Y, X)).score((X, Y, Z))
+tcca = TCCA(latent_dimensions=latent_dims).fit((X, Y, X)).score((X, Y, Z))
 
 # %%
-ktcca = KTCCA(latent_dims=latent_dims).fit((X, Y, X)).score((X, Y, Z))
+ktcca = KTCCA(latent_dimensions=latent_dims).fit((X, Y, X)).score((X, Y, Z))
```

### Comparing `cca_zoo-2.0.0/examples/plot_plotting.py` & `cca_zoo-2.0.1/examples/plot_plotting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Model Plotting
 ===========================
 
-This script will show how to use the plotting functions of the CCA-Zoo package.
+This script will show how to use the visualisation functions of the CCA-Zoo package.
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
 from sklearn.model_selection import train_test_split
 
 from cca_zoo.data.simulated import LinearSimulatedData
-from cca_zoo.models import CCA
-from cca_zoo.plotting import pairplot_train_test
+from cca_zoo.classical import CCA
+from cca_zoo.visualisation import pairplot_train_test
 
 # Data
 # ------
 np.random.seed(42)
 n = 200
 p = 25
 q = 25
@@ -27,15 +27,15 @@
 
 X_tr, X_te, Y_tr, Y_te = train_test_split(X, Y, test_size=0.2, random_state=42)
 
 # %%
 # Model
 # ------
 
-cca = CCA(latent_dims=latent_dims).fit((X_tr, Y_tr))
+cca = CCA(latent_dimensions=latent_dims).fit((X_tr, Y_tr))
 
 # %%
 # Plotting
 # ---------
 
 pairplot_train_test(cca.transform((X_tr, Y_tr)), cca.transform((X_te, Y_te)))
 plt.show()
```

### Comparing `cca_zoo-2.0.0/examples/plot_sparse_cca.py` & `cca_zoo-2.0.1/examples/plot_sparse_cca.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 from cca_zoo.data.simulated import LinearSimulatedData
 from cca_zoo.model_selection import GridSearchCV
-from cca_zoo.models import (
+from cca_zoo.classical import (
     CCA,
     PLS,
     SCCA_IPLS,
     SCCA_PMD,
     AltMaxVar,
     ElasticCCA,
     SCCA_Span,
```

### Comparing `cca_zoo-2.0.0/examples/plot_validation.py` & `cca_zoo-2.0.1/examples/plot_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 permutation testing, learning curves, and cross-validation.
 """
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from cca_zoo.data.simulated import LinearSimulatedData
-from cca_zoo.models import CCA
+from cca_zoo.classical import CCA
 
 # %%
 # Data
 # ------
 np.random.seed(42)
 n = 200
 p = 15
@@ -30,15 +30,15 @@
 # -------------------
 
 from sklearn.model_selection import KFold, ShuffleSplit
 
 from cca_zoo.model_selection import learning_curve, permutation_test_score
 
 LATENT_DIMS = 3
-model = CCA(latent_dims=LATENT_DIMS)
+model = CCA(latent_dimensions=LATENT_DIMS)
 cv = KFold(2, shuffle=True, random_state=0)
 score, perm_scores, pvalue = permutation_test_score(
     model, (X, Y), cv=cv, n_permutations=100
 )
 
 # %%
 fig, ax = plt.subplots(LATENT_DIMS, figsize=[12, 8])
@@ -89,15 +89,15 @@
         ``n_features`` is the number of features.
 
     y : array-like of shape (n_samples) or (n_samples, n_features)
         Target relative to ``views`` for classification or regression;
         None for unsupervised learning.
 
     axes : array-like of shape (3,), default=None
-        Axes to use for plotting the curves.
+        Axes to use for visualisation the curves.
 
     ylim : tuple of shape (2,), default=None
         Defines minimum and maximum y-values plotted, e.g. (ymin, ymax).
 
     cv : int, cross-validation generator or an iterable, default=None
         Determines the cross-validation splitting strategy.
         Possible inputs for cv are:
```

### Comparing `cca_zoo-2.0.0/setup.py` & `cca_zoo-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "deep": ["torch", "torchvision", "pytorch-lightning"],
     "probabilistic": ["jax", "numpyro", "arviz"],
 }
 EXTRA_PACKAGES["all"] = EXTRA_PACKAGES["deep"] + EXTRA_PACKAGES["probabilistic"]
 
 setup(
     name="cca_zoo",
-    version="2.0.0",
+    version="2.0.1",
     include_package_data=True,
     keywords="cca",
     packages=find_packages(),
     url="https://github.com/jameschapman19/cca_zoo",
     license="MIT",
     author="jameschapman",
     description=(
```

