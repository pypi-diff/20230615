# Comparing `tmp/cca_zoo-2.0.1.tar.gz` & `tmp/cca_zoo-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cca_zoo-2.0.1.tar", last modified: Thu Jun 15 12:07:42 2023, max compression
+gzip compressed data, was "dist/cca_zoo-2.0.2.tar", last modified: Thu Jun 15 16:21:36 2023, max compression
```

## Comparing `cca_zoo-2.0.1.tar` & `cca_zoo-2.0.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/classical/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_gcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_grcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_altmaxvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_elasticnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_gradkcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_incrementalpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_pls_als.py
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_pmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_admm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_hsic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_parkhomenko.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_stochasticpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_iterative/_swcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_kcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_mcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_ncca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_partialcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_pcacca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_plsmixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_prcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/classical/_tcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/data/deep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/data/simulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/deep/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_noi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_sdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dgcca.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dtcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/_dccae.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/_generative/_splitae.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/deep/objectives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/model_selection/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/model_selection/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/probabilistic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/probabilistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/probabilistic/_probabilisticcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_deepmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_probabilistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_regularised.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_unregularized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/utils/check_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/cca_zoo/visualisation/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/cca_zoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 12:07:41.000000 cca_zoo-2.0.1/cca_zoo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_dcca_custom_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_dcca_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_hyperparameter_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_kernel_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_many_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_sparse_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-15 12:07:26.000000 cca_zoo-2.0.1/examples/plot_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 12:07:42.000000 cca_zoo-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-15 12:07:40.000000 cca_zoo-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/classical/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_gcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_grcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_altmaxvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_elasticnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_gradkcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_incrementalpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_pls_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_pmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_admm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_hsic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_stochasticpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_iterative/_swcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_kcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_mcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_ncca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_partialcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_pcacca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_prcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/classical/_tcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/data/deep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/data/simulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_noi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_sdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dgcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dtcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/_dccae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/_generative/_splitae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/deep/objectives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/model_selection/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/model_selection/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/probabilistic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/probabilistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/probabilistic/_probabilisticcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_deepmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_probabilistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_regularised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_unregularized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/utils/check_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/cca_zoo/visualisation/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/cca_zoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 16:21:35.000000 cca_zoo-2.0.2/cca_zoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_dcca_custom_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_dcca_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_hyperparameter_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_kernel_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_many_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_sparse_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-15 16:21:24.000000 cca_zoo-2.0.2/examples/plot_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:21:36.000000 cca_zoo-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-15 16:21:34.000000 cca_zoo-2.0.2/setup.py
```

### Comparing `cca_zoo-2.0.1/PKG-INFO` & `cca_zoo-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca_zoo
-Version: 2.0.1
+Version: 2.0.2
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.1/README.md` & `cca_zoo-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/__init__.py` & `cca_zoo-2.0.2/cca_zoo/classical/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ._mcca import MCCA, CCA, PLS, rCCA, MPLS
+from ._mcca import MCCA, CCA, rCCA
+from ._pls import PLS, MPLS
 from ._gcca import GCCA
 from ._grcca import GRCCA
 from ._ncca import NCCA
 from ._partialcca import PartialCCA
 from ._prcca import PRCCA
 from ._tcca import TCCA
 from ._pcacca import PCACCA
```

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_base.py` & `cca_zoo-2.0.2/cca_zoo/classical/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_dummy.py` & `cca_zoo-2.0.2/cca_zoo/classical/_dummy.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_gcca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_gcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_grcca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_grcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/__init__.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_altmaxvar.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_altmaxvar.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_base.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_elasticnet.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_elasticnet.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_ey.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_ey.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
 import numpy as np
 import torch
 
-from cca_zoo.classical._plsmixin import PLSMixin
 from cca_zoo.classical._iterative._base import BaseGradientLoop, BaseIterative
+from cca_zoo.classical._pls import PLSMixin
 
 
 class CCAEY(BaseIterative):
     """
     A class used to fit Regularized CCA by Delta-EigenGame
 
     Parameters
```

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_gh.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_gradkcca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_gradkcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_incrementalpls.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_incrementalpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_pls_als.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_pls_als.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Union
 
 import numpy as np
 
-from cca_zoo.classical._plsmixin import PLSMixin
+
 from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
+from cca_zoo.classical._pls import PLSMixin
 
 
 class PLS_ALS(BaseDeflation, PLSMixin):
     r"""
     A class used to fit a PLS model by alternating least squares (ALS).
 
     This model finds the linear projections of two views that maximize their covariance while minimizing their residual variance.
```

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_pmd.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_pmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import itertools
 import warnings
 
 import numpy as np
 import torch
 
 from cca_zoo.classical._iterative._base import BaseDeflation, BaseLoop
-from cca_zoo.classical._plsmixin import PLSMixin
+from cca_zoo.classical._pls import PLSMixin
 from cca_zoo.classical._search import _delta_search
 from cca_zoo.utils import _check_converged_weights, _process_parameter
 
 
 class SCCA_PMD(BaseDeflation, PLSMixin):
     r"""
     A class used to fit a sparse CCA model by penalized matrix decomposition (PMD).
```

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_admm.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_admm.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_hsic.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_hsic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_parkhomenko.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_parkhomenko.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_scca_span.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_scca_span.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_stochasticpls.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_stochasticpls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 
 from cca_zoo.classical._iterative._ey import PLSEY
-from cca_zoo.classical._plsmixin import PLSMixin
 from cca_zoo.classical._iterative._base import BaseGradientLoop
+from cca_zoo.classical._pls import PLSMixin
 
 
 class PLSStochasticPower(PLSEY, PLSMixin):
     def _get_module(self, weights=None, k=None):
         return StochasticPowerLoopBase(
             weights=weights,
             k=k,
```

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_svd.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_svd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union
 
 import torch
 
-from cca_zoo.classical._plsmixin import PLSMixin
 from cca_zoo.classical._iterative._ey import CCAEY, EYLoop
+from cca_zoo.classical._pls import PLSMixin
 
 
 class CCASVD(CCAEY):
     def _get_module(self, weights=None, k=None):
         return SVDLoop(
             weights=weights,
             k=k,
```

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_iterative/_swcca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_iterative/_swcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_kcca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_kcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_mcca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_mcca.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import numpy as np
 from scipy.linalg import block_diag
 from scipy.linalg import eigh
 from sklearn.decomposition import PCA
 
 from cca_zoo.classical._base import BaseModel
-from cca_zoo.classical._plsmixin import PLSMixin
 from cca_zoo.utils import _process_parameter
 
 
 class MCCA(BaseModel):
     r"""
     A class used to fit Regularised CCA (canonical ridge) model. This model adds a regularization term to the CCA objective function to avoid overfitting and improve stability. It uses PCA to perform the optimization efficiently for high dimensional data.
 
@@ -294,79 +293,7 @@
         # Call the parent class constructor with c=0.0 to disable regularization
         super().__init__(
             latent_dimensions=latent_dimensions,
             copy_data=copy_data,
             c=0.0,
             random_state=random_state,
         )
-
-
-class PLS(rCCA, PLSMixin):
-    r"""
-    A class used to fit a simple PLS model. This model finds the linear projections of two views that maximize their covariance.
-
-    Implements PLS by inheriting regularised CCA with maximal regularisation. This is equivalent to solving the following optimization problem:
-
-    .. math::
-
-        w_{opt}=\underset{w}{\mathrm{argmax}}\{ w_1^TX_1^TX_2w_2  \}\\
-
-        \text{subject to:}
-
-        w_1^Tw_1=1
-
-        w_2^Tw_2=1
-
-    Parameters
-    ----------
-    latent_dimensions : int, optional
-        Number of latent dimensions to use, by default 1
-    copy_data : bool, optional
-        Whether to copy the data, by default True
-    random_state : int, optional
-        Random state, by default None
-    """
-
-    def __init__(
-        self,
-        latent_dimensions: int = 1,
-        copy_data=True,
-        random_state=None,
-    ):
-        # Call the parent class constructor with c=1 to enable maximal regularization
-        super().__init__(
-            latent_dimensions=latent_dimensions,
-            copy_data=copy_data,
-            c=1,
-            random_state=random_state,
-        )
-
-
-class MPLS(MCCA, PLSMixin):
-    r"""
-    A class used to fit a mutiview PLS model. This model finds the linear projections of two views that maximize their covariance.
-
-    Implements PLS by inheriting regularised CCA with maximal regularisation. This is equivalent to solving the following optimization problem:
-
-    Parameters
-    ----------
-    latent_dimensions : int, optional
-        Number of latent dimensions to use, by default 1
-    copy_data : bool, optional
-        Whether to copy the data, by default True
-    random_state : int, optional
-        Random state, by default None
-    """
-
-    def __init__(
-        self,
-        latent_dimensions: int = 1,
-        copy_data=True,
-        random_state=None,
-    ):
-        # Call the parent class constructor with c=1 to enable maximal regularization
-        super().__init__(
-            latent_dimensions=latent_dimensions,
-            copy_data=copy_data,
-            c=1,
-            random_state=random_state,
-        )
```

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_ncca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_ncca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_partialcca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_partialcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_pcacca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_pcacca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_prcca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_prcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_search.py` & `cca_zoo-2.0.2/cca_zoo/classical/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/classical/_tcca.py` & `cca_zoo-2.0.2/cca_zoo/classical/_tcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/data/deep.py` & `cca_zoo-2.0.2/cca_zoo/data/deep.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/data/simulated.py` & `cca_zoo-2.0.2/cca_zoo/data/simulated.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/__init__.py` & `cca_zoo-2.0.2/cca_zoo/deep/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_base.py` & `cca_zoo-2.0.2/cca_zoo/deep/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca.py` & `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py` & `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_ey.py` & `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_ey.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_gh.py` & `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_noi.py` & `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_noi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_sdl.py` & `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_sdl.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dcca_svd.py` & `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dcca_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dgcca.py` & `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dgcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_discriminative/_dtcca.py` & `cca_zoo-2.0.2/cca_zoo/deep/_discriminative/_dtcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_generative/_base.py` & `cca_zoo-2.0.2/cca_zoo/deep/_generative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_generative/_dccae.py` & `cca_zoo-2.0.2/cca_zoo/deep/_generative/_dccae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_generative/_dvcca.py` & `cca_zoo-2.0.2/cca_zoo/deep/_generative/_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/_generative/_splitae.py` & `cca_zoo-2.0.2/cca_zoo/deep/_generative/_splitae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/architectures.py` & `cca_zoo-2.0.2/cca_zoo/deep/architectures.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/metrics.py` & `cca_zoo-2.0.2/cca_zoo/deep/metrics.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/deep/objectives.py` & `cca_zoo-2.0.2/cca_zoo/deep/objectives.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/model_selection/_search.py` & `cca_zoo-2.0.2/cca_zoo/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/model_selection/_validation.py` & `cca_zoo-2.0.2/cca_zoo/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/probabilistic/_probabilisticcca.py` & `cca_zoo-2.0.2/cca_zoo/probabilistic/_probabilisticcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/test/test_callbacks.py` & `cca_zoo-2.0.2/cca_zoo/test/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/test/test_data.py` & `cca_zoo-2.0.2/cca_zoo/test/test_data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/test/test_deepmodels.py` & `cca_zoo-2.0.2/cca_zoo/test/test_deepmodels.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/test/test_kernel.py` & `cca_zoo-2.0.2/cca_zoo/test/test_kernel.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/test/test_probabilistic.py` & `cca_zoo-2.0.2/cca_zoo/test/test_probabilistic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/test/test_regularised.py` & `cca_zoo-2.0.2/cca_zoo/test/test_regularised.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/test/test_stochastic.py` & `cca_zoo-2.0.2/cca_zoo/test/test_stochastic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/test/test_unregularized.py` & `cca_zoo-2.0.2/cca_zoo/test/test_unregularized.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/test/test_utils.py` & `cca_zoo-2.0.2/cca_zoo/test/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,16 @@
         explained_covariance_cumulative = pls.explained_covariance_cumulative_((X, X))
         # explained_covariance_ratio should sum to 1 for each view
         assert np.allclose(explained_covariance_ratio.sum(), 1)
         # explained_covariance_cumulative should be monotonically increasing
         assert np.all(np.diff(explained_covariance_cumulative) >= 0)
 
 
+# def test_explained_correlation():
+
+
 def test_validation():
     # Test that validation works
     pls = MPLS(latent_dimensions=1).fit((X_low, Y_low))
     cross_validate(pls, (X_low, Y_low))
     permutation_test_score(pls, (X_low, Y_low))
     learning_curve(pls, (X_low, Y_low))
```

### Comparing `cca_zoo-2.0.1/cca_zoo/utils/check_values.py` & `cca_zoo-2.0.2/cca_zoo/utils/check_values.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo/visualisation/plotting.py` & `cca_zoo-2.0.2/cca_zoo/visualisation/plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/cca_zoo.egg-info/PKG-INFO` & `cca_zoo-2.0.2/cca_zoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca-zoo
-Version: 2.0.1
+Version: 2.0.2
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.1/cca_zoo.egg-info/SOURCES.txt` & `cca_zoo-2.0.2/cca_zoo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 cca_zoo/classical/_gcca.py
 cca_zoo/classical/_grcca.py
 cca_zoo/classical/_kcca.py
 cca_zoo/classical/_mcca.py
 cca_zoo/classical/_ncca.py
 cca_zoo/classical/_partialcca.py
 cca_zoo/classical/_pcacca.py
-cca_zoo/classical/_plsmixin.py
+cca_zoo/classical/_pls.py
 cca_zoo/classical/_prcca.py
 cca_zoo/classical/_search.py
 cca_zoo/classical/_tcca.py
 cca_zoo/classical/_iterative/__init__.py
 cca_zoo/classical/_iterative/_altmaxvar.py
 cca_zoo/classical/_iterative/_base.py
 cca_zoo/classical/_iterative/_elasticnet.py
```

### Comparing `cca_zoo-2.0.1/examples/__init__.py` & `cca_zoo-2.0.2/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_dcca.py` & `cca_zoo-2.0.2/examples/plot_dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_dcca_custom_data.py` & `cca_zoo-2.0.2/examples/plot_dcca_custom_data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_dcca_multi.py` & `cca_zoo-2.0.2/examples/plot_dcca_multi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_dvcca.py` & `cca_zoo-2.0.2/examples/plot_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_hyperparameter_selection.py` & `cca_zoo-2.0.2/examples/plot_hyperparameter_selection.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_kernel_cca.py` & `cca_zoo-2.0.2/examples/plot_kernel_cca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_many_views.py` & `cca_zoo-2.0.2/examples/plot_many_views.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_plotting.py` & `cca_zoo-2.0.2/examples/plot_plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_sparse_cca.py` & `cca_zoo-2.0.2/examples/plot_sparse_cca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/examples/plot_validation.py` & `cca_zoo-2.0.2/examples/plot_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.1/setup.py` & `cca_zoo-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "deep": ["torch", "torchvision", "pytorch-lightning"],
     "probabilistic": ["jax", "numpyro", "arviz"],
 }
 EXTRA_PACKAGES["all"] = EXTRA_PACKAGES["deep"] + EXTRA_PACKAGES["probabilistic"]
 
 setup(
     name="cca_zoo",
-    version="2.0.1",
+    version="2.0.2",
     include_package_data=True,
     keywords="cca",
     packages=find_packages(),
     url="https://github.com/jameschapman19/cca_zoo",
     license="MIT",
     author="jameschapman",
     description=(
```

