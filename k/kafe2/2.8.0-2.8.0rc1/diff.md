# Comparing `tmp/kafe2-2.8.0.tar.gz` & `tmp/kafe2-2.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafe2-2.8.0.tar", last modified: Thu Jun 15 10:33:31 2023, max compression
+gzip compressed data, was "kafe2-2.8.0rc1.tar", last modified: Wed Apr 19 15:27:43 2023, max compression
```

## Comparing `kafe2-2.8.0.tar` & `kafe2-2.8.0rc1.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.152153 kafe2-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-15 10:33:14.000000 kafe2-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-15 10:33:31.152153 kafe2-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-15 10:33:14.000000 kafe2-2.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.140153 kafe2-2.8.0/kafe2/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/_version_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.140153 kafe2-2.8.0/kafe2/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/config/kafe2.matplotlibrc.conf
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/config/kafe2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/config/plot_style_color.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/core/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/confidence.py
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/contour.py
--rw-r--r--   0 runner    (1001) docker     (123)    24145 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/core/fitters/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/fitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50344 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/fitters/nexus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/fitters/nexus_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/fitters/simple_fitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/core/minimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/minimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/minimizers/iminuit_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31088 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/minimizers/minimizer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/minimizers/root_tminuit_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/core/minimizers/scipy_optimize_minimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/fit/
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/_aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/fit/_base/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/_base/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    33791 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/_base/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/_base/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    56936 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/_base/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    31671 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/_base/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/_base/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    68631 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/_base/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/fit/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/custom/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/fit/histogram/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/histogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/histogram/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/histogram/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/histogram/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/histogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/histogram/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/fit/indexed/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/indexed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/indexed/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/indexed/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/indexed/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/indexed/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/indexed/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/indexed/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/fit/io/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/io/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/io/handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/fit/multi/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/multi/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)    41242 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/multi/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.144152 kafe2-2.8.0/kafe2/fit/representation/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/_yaml_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/representation/constraint/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/constraint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/constraint/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/constraint/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/representation/container/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/container/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/container/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/representation/error/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/error/common_error_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/representation/fit/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/fit/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/fit/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/representation/format/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/format/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/format/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/representation/model/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/model/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/representation/model/yaml_drepr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46570 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/tools/contours_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31872 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/tools/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/tools/fit_wrapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/tools/kafe2go
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/tools/kafe2go.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/unbinned/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/unbinned/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/unbinned/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/unbinned/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/unbinned/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/unbinned/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/unbinned/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/util/function_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    35596 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/util/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/fit/xy/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/xy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/xy/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/xy/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/xy/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/xy/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/xy/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/fit/xy/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.148153 kafe2-2.8.0/kafe2/test/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.152153 kafe2-2.8.0/kafe2/test/core/minimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/minimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28560 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/minimizers/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/minimizers/test_iminuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/minimizers/test_root_tminuit.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/minimizers/test_scipy_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/test_confidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/test_cov_mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/test_gaussian_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    29537 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/test_nexus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/test_nexus_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/core/test_parameter_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.152153 kafe2-2.8.0/kafe2/test/fit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_containers_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_containers_indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_containers_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_cost_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_ensemble_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_fit_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    16202 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_fit_hist.py
--rw-r--r--   0 runner    (1001) docker     (123)    23697 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_fit_indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)    31993 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_fit_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_fit_unbinned.py
--rw-r--r--   0 runner    (1001) docker     (123)    40080 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_fit_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)    15958 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_fits_with_parameter_constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_model_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_representers_constraint_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_representers_container_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)    43978 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_representers_fit_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_representers_format_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)    18868 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_representers_model_function_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_representers_parametric_model_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/fit/test_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/test/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-06-15 10:33:14.000000 kafe2-2.8.0/kafe2/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:33:31.140153 kafe2-2.8.0/kafe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-15 10:33:30.000000 kafe2-2.8.0/kafe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-15 10:33:31.000000 kafe2-2.8.0/kafe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:33:30.000000 kafe2-2.8.0/kafe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-15 10:33:30.000000 kafe2-2.8.0/kafe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:33:30.000000 kafe2-2.8.0/kafe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 10:33:31.152153 kafe2-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-15 10:33:14.000000 kafe2-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.966598 kafe2-2.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-19 15:27:43.966598 kafe2-2.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.950596 kafe2-2.8.0rc1/kafe2/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/_version_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/config/kafe2.matplotlibrc.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/config/kafe2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/config/plot_style_color.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24145 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/core/fitters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/fitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50344 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/fitters/nexus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/fitters/nexus_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/fitters/simple_fitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/core/minimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/iminuit_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30571 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/minimizer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/root_tminuit_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27071 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/core/minimizers/scipy_optimize_minimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/fit/_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33791 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56936 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31671 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68406 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/_base/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/fit/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/custom/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.954597 kafe2-2.8.0rc1/kafe2/fit/histogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/histogram/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/indexed/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/indexed/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/io/handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/multi/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/multi/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41242 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/multi/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/_yaml_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/constraint/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/constraint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/constraint/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/constraint/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/container/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/container/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/container/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/error/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/error/common_error_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/fit/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/fit/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/format/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/format/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/format/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/representation/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/model/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/representation/model/yaml_drepr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.958597 kafe2-2.8.0rc1/kafe2/fit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45151 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/contours_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31872 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/fit_wrapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       88 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/kafe2go
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/tools/kafe2go.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/fit/unbinned/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/unbinned/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/fit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/util/function_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26729 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/util/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/fit/xy/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29429 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29129 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/fit/xy/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/test/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.962597 kafe2-2.8.0rc1/kafe2/test/core/minimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28560 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_iminuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_root_tminuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_scipy_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_confidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_cov_mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_gaussian_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29537 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_nexus_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/core/test_parameter_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.966598 kafe2-2.8.0rc1/kafe2/test/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_containers_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_containers_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_containers_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_cost_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_ensemble_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16202 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23697 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31993 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_unbinned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40080 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fit_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15958 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_fits_with_parameter_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_model_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_constraint_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23602 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_container_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43978 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_fit_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_format_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18868 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_model_function_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24649 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_representers_parametric_model_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/fit/test_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/test/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/kafe2/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:27:43.950596 kafe2-2.8.0rc1/kafe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-19 15:27:43.000000 kafe2-2.8.0rc1/kafe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:27:43.966598 kafe2-2.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-19 15:27:26.000000 kafe2-2.8.0rc1/setup.py
```

### Comparing `kafe2-2.8.0/LICENSE` & `kafe2-2.8.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/PKG-INFO` & `kafe2-2.8.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafe2
-Version: 2.8.0
+Version: 2.8.0rc1
 Summary: Karlsruhe Fit Environment 2: a package for fitting and elementary data analysis
 Home-page: https://github.com/PhiLFitters/kafe2
 Author: Daniel Savoiu
 Author-email: daniel.savoiu@cern.ch
 License: GPL3
 Keywords: kafe2 kit karlsruhe data analysis lab laboratory practical courses education university students physics fitting minimization minimisation regression parametric parameter estimation optimization optimisation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kafe2-2.8.0/README.rst` & `kafe2-2.8.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/config/__init__.py` & `kafe2-2.8.0rc1/kafe2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/config/kafe2.matplotlibrc.conf` & `kafe2-2.8.0rc1/kafe2/config/kafe2.matplotlibrc.conf`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/config/kafe2.yaml` & `kafe2-2.8.0rc1/kafe2/config/kafe2.yaml`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/config/plot_style_color.yaml` & `kafe2-2.8.0rc1/kafe2/config/plot_style_color.yaml`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/confidence.py` & `kafe2-2.8.0rc1/kafe2/core/confidence.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/constraint.py` & `kafe2-2.8.0rc1/kafe2/core/constraint.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/contour.py` & `kafe2-2.8.0rc1/kafe2/core/contour.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/error.py` & `kafe2-2.8.0rc1/kafe2/core/error.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/fitters/__init__.py` & `kafe2-2.8.0rc1/kafe2/core/fitters/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/fitters/nexus.py` & `kafe2-2.8.0rc1/kafe2/core/fitters/nexus.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/fitters/nexus_fitter.py` & `kafe2-2.8.0rc1/kafe2/core/fitters/nexus_fitter.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/fitters/simple_fitter.py` & `kafe2-2.8.0rc1/kafe2/core/fitters/simple_fitter.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/minimizers/__init__.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/minimizers/iminuit_minimizer.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/iminuit_minimizer.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/minimizers/minimizer_base.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/minimizer_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,17 +242,15 @@
         if high is not None and np.min(high) < _min_par_val:
             raise ValueError(f"high={high} must be larger than <{parameter_name}>={_min_par_val}")
 
         _arrow_specs = self._get_arrow_specs(
             parameter_name, low, high, cl, subtract_min, arrows, _min_cost, _min_par_val,
             _parameter_error, _min_par_vals)
         low = np.min(low)
-        _low_was_none = low is None
         high = np.max(high)
-        _high_was_none = high is None
         cl = np.max(cl)
         if sigma is not None:
             _low_sigma = _min_par_val - sigma * _parameter_error
             low = _low_sigma if low is None else min(low, _low_sigma)
             _high_sigma = _min_par_val + sigma * _parameter_error
             high = _high_sigma if high is None else max(high, _high_sigma)
         elif cl is None:
@@ -265,26 +263,16 @@
             for _arrow_spec in _arrow_specs:
                 low = _arrow_spec["x"] if low is None else min(low, _arrow_spec["x"])
                 high = _arrow_spec["x"] if high is None else max(high, _arrow_spec["x"])
             _original_low = low
             _original_high = high
             _margin = 0.13 if arrows else 0
             for _arrow_spec in _arrow_specs:
-                if _arrow_spec["side"] == "left":
-                    _arrow_spec["x_margin"] = _arrow_spec["x"] \
-                        + _margin * (_arrow_spec["x"] - _original_high)
-                    if _low_was_none:
-                        low = min(low, _arrow_spec["x_margin"])
-                elif _arrow_spec["side"] == "right":
-                    _arrow_spec["x_margin"] = _arrow_spec["x"] \
-                        + _margin * (_arrow_spec["x"] - _original_low)
-                    if _high_was_none:
-                        high = max(high, _arrow_spec["x_margin"])
-                else:
-                    assert False
+                low = min(low, _arrow_spec["x"] + _margin * (_arrow_spec["x"] - _original_high))
+                high = max(high, _arrow_spec["x"] + _margin * (_arrow_spec["x"] - _original_low))
 
         return low, high, _arrow_specs
 
     def _get_arrow_specs(
             self, parameter_name: str, low: Union[None, float, Sequence[float]],
             high: Union[None, float, Sequence[float]], cl: Union[None, float, Sequence[float]],
             subtract_min: bool, arrows: bool, min_cost: float, min_par_val: float,
```

### Comparing `kafe2-2.8.0/kafe2/core/minimizers/root_tminuit_minimizer.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/root_tminuit_minimizer.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/core/minimizers/scipy_optimize_minimizer.py` & `kafe2-2.8.0rc1/kafe2/core/minimizers/scipy_optimize_minimizer.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/_aux.py` & `kafe2-2.8.0rc1/kafe2/fit/_aux.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/_base/container.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/container.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/_base/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/_base/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/_base/format.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/format.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/_base/model.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/model.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/_base/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/_base/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from ..util.wrapper import _fit_history
 from ...config import kc, ConfigError, kafe2_rc
 
 from collections import OrderedDict
 from matplotlib import pyplot as plt
 from matplotlib import gridspec as gs
 from matplotlib.legend_handler import HandlerBase
-from matplotlib import rcParams, rc_context
+from matplotlib import rc_context
 
 try:
     import typing  # help IDEs with type-hinting inside docstrings
 except ImportError:
     pass
 
 __all__ = ["PlotAdapterBase", "Plot", "kc_plot_style"]
@@ -1052,15 +1052,14 @@
             # otherwise 'tight_layout' will consider it part of the axes
             # and produce undesirable layouts
 
             _leg = _axes.get_figure().legend(_hs_sorted, _ls_sorted,
                          mode=_mode,
                          borderaxespad=_borderaxespad,
                          ncol=_ncol,
-                         fontsize=rcParams["font.size"],
                          handler_map={'_nokey_': DummyLegendHandler()},
                          **kwargs)
             _leg.set_zorder(_zorder)
 
             # manually change bbox from figure to axes
             _leg._bbox_to_anchor = self._get_axes('__legendfakeaxes__').bbox
 
@@ -1283,15 +1282,15 @@
         """Convenience wrapper for matplotlib.pyplot.show()"""
         plt.show(*args, **kwargs)
 
 
     def plot(self, legend=True, fit_info=True, asymmetric_parameter_errors=False,
              ratio=False, ratio_range=None, ratio_height_share=0.25,
              residual=False, residual_range=None, residual_height_share=0.25,
-             plot_width_share=0.5, font_scale=1.0, figsize=None):
+             plot_width_share=0.5, figsize=None):
         """
         Plot data, model (and other subplots) for all child :py:obj:`Fit` objects.
 
         :param legend: if ``True``, a legend is rendered
         :param fit_info: If :py:obj:`True`, fit results will be shown in the legend. This can also
             be a list of booleans, corresponding to the fits handled by this
             :py:obj:`~.Plot`-object.
@@ -1300,27 +1299,24 @@
         :param ratio: if ``True``, a secondary plot containing data/model ratios is shown below the main plot
         :param ratio_range: the *y* range to set in the secondary plot
         :type ratio_range: tuple of 2 floats
         :param ratio_height_share: share of the total height to be taken up by the secondary plot
         :type ratio_height_share: float
         :param plot_width_share: share of the total width to be taken up by the plot(s)
         :type plot_width_share: float
-        :param font_scale: multiply font size by this amount.
-        :type font_scale: float
         :param figsize: the (*width*, *height*) of the figure (in inches) or ``None`` to use default
         :type figsize: tuple of 2 floats
 
         :return: dictionary containing information about the plotted objects
         :rtype: dict
         """
         if ratio and residual:
             raise NotImplementedError("Cannot plot ratio and residual at the same time.")
 
         with rc_context(kafe2_rc):
-            rcParams["font.size"] *= font_scale
             _axes_keys = ('main',)
             _height_ratios = [1.0]
             _width_ratios = (plot_width_share, 1.0 - plot_width_share)
 
             if ratio:
                 _axes_keys += ('ratio',)
                 _height_ratios[0] -= ratio_height_share
```

### Comparing `kafe2-2.8.0/kafe2/fit/custom/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/custom/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/histogram/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/histogram/container.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/container.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,68 +16,58 @@
     divide the continuum into intervals ("bins") and count the number of entries
     per interval.
 
     .. .. inheritance-diagram:: HistContainer
     ..    :parts: 1
 
     """
-    def __init__(self, n_bins=None, bin_range=None, bin_edges=None, fill_data=None, dtype=int):
+    def __init__(self, n_bins, bin_range, bin_edges=None, fill_data=None, dtype=int):
         """
         Construct a histogram:
 
-        :param n_bins: how many bins raw data should be split into.
+        :param n_bins: number of bins
         :type n_bins: int
-        :param bin_range: the lower and upper bound for the bins specified by n_bins.
-        :type bin_range: iterable[float] of length 2
-        :param bin_edges: explicit bin edges for raw data. If ``None``, each bin will have the same
-            width.
-        :type bin_edges: iterable[float]
+        :param bin_range: the lower and upper edges of the entire histogram
+        :type bin_range: tuple of floats
+        :param bin_edges: the bin edges (if ``None``, each bin will have the same width)
+        :type bin_edges: list of floats
         :param fill_data: entries to fill into the histogram
-        :type fill_data: iterable[float]
+        :type fill_data: list of floats
         :param dtype: data type of histogram entries
         :type dtype: type
         """
-        if bin_edges is None:
-            if n_bins is None or bin_range is None:
-                raise ValueError("Either n_bins and bin_range or bin_edges must be specified.")
-        else:
-            if n_bins is None:
-                n_bins = len(bin_edges) - 1
-            if n_bins != len(bin_edges) - 1 and n_bins != len(bin_edges) + 1:
-                raise ValueError(f"n_bins is {n_bins} but bin_edges implies either "
-                                 f"{len(bin_edges) - 1} or {len(bin_edges) - 1} bins")
-            if bin_range is None:
-                bin_range = (bin_edges[0], bin_edges[-1])
-            if n_bins == len(bin_edges) - 1:
-                if bin_range[0] != bin_edges[0] or bin_range[1] != bin_edges[-1]:
-                    raise ValueError(f"bin_range is {bin_range} but bin_edges implies "
-                                     f"{(bin_edges[0], bin_edges[-1])}")
-            if n_bins == len(bin_edges) + 1:
-                if bin_range[0] > bin_edges[0] or bin_range[1] < bin_edges[-1]:
-                    raise ValueError(f"bin_range is {bin_range} but does not encompass inner "
-                                     f"bin edges {(bin_edges[0], bin_edges[-1])}")
-
-        if len(bin_range) != 2:
-            raise ValueError(f"bin_range must be iterable of 2 floats but received {bin_range}")
-        low, high = tuple(bin_range)
-
         super(HistContainer, self).__init__(data=np.zeros(n_bins+2), dtype=dtype)  # underflow and overflow bins
         self._manual_heights = False
         self._processed_entries = []
         self._unprocessed_entries = []
         # TODO: think of a way to implement weights
 
+        if len(bin_range) != 2:
+            raise ValueError(
+                "Invalid bin range specification: %r! Must be tuple of 2 floats..." % (bin_range,))
+        low, high = tuple(bin_range)
+
         if bin_edges is not None:
-            if len(bin_edges) == self.size + 1:
-                self.rebin(bin_edges)
-            elif len(bin_edges) == self.size - 1:
-                # Add low and high to edges if inner edges specified:
-                self.rebin([low] + list(bin_edges) + [high])
+            # user specified bin edges -> check that these match the given 'n_bins' and 'bin_range'
+            _sz = self.size
+            if len(bin_edges) == _sz + 1:
+                # assume bin edges given including bin range
+                if not (bin_edges[0] == low and bin_edges[-1] == high):
+                    raise ValueError(
+                        "Invalid bin edge specification! First and last elements %r must match histogram bin range %r."
+                        % ((bin_edges[0], bin_edges[-1]), bin_range))
+                _bin_edges_including_low_and_high = bin_edges
+            elif len(bin_edges) == _sz - 1:
+                # <check if ordered and strictly within bin range>
+                _bin_edges_including_low_and_high = [low] + bin_edges + [high]
             else:
-                assert False
+                raise ValueError(
+                    "Invalid bin edge specification! Number of elements (%d) must match histogram bin number (%d) +/- 1."
+                    % (len(bin_edges), _sz))
+            self.rebin(new_bin_edges=_bin_edges_including_low_and_high)
         else:
             # construct own bin edges
             self._bin_edges = np.linspace(bin_range[0], bin_range[1], n_bins+1)
 
         if fill_data is not None:
             self.fill(fill_data)
```

### Comparing `kafe2-2.8.0/kafe2/fit/histogram/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/histogram/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/histogram/model.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/model.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/histogram/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/histogram/plot.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/indexed/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/indexed/container.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/container.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/indexed/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/indexed/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/indexed/format.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/format.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/indexed/model.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/model.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/indexed/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/indexed/plot.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/io/file.py` & `kafe2-2.8.0rc1/kafe2/fit/io/file.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/io/handle.py` & `kafe2-2.8.0rc1/kafe2/fit/io/handle.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/multi/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/multi/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/multi/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/multi/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/_yaml_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/_yaml_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/constraint/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/constraint/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/constraint/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/constraint/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/container/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/container/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/container/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/container/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/error/common_error_tools.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/error/common_error_tools.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/fit/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/fit/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/fit/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/fit/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/format/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/format/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/format/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/format/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/model/_base.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/model/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/representation/model/yaml_drepr.py` & `kafe2-2.8.0rc1/kafe2/fit/representation/model/yaml_drepr.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/tools/contours_profiler.py` & `kafe2-2.8.0rc1/kafe2/fit/tools/contours_profiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import os
 
 from collections.abc import Iterable
 from ...config import kafe2_rc
 from ...core.confidence import ConfidenceLevel
 from .._base import FitBase
 from .._base.format import ScalarFormatter as ScalarBaseFormatter
-from matplotlib import pyplot as plt
+from matplotlib import pyplot as plt, rcParams
 from matplotlib import gridspec as gs
 from matplotlib import ticker as plticker
 from matplotlib.axes import Axes
-from matplotlib import rcParams, rc_context
+from matplotlib import rc_context
 
 
 __all__ = ["ContoursProfiler"]
 
 _python_version = sys.version_info[0]
 _float_template = ".2g" if _python_version == 2 else "#.2g"
 
@@ -390,16 +390,15 @@
                      show_parabolic=True,
                      show_grid=True,
                      show_legend=True,
                      show_fit_minimum=True,
                      show_error_span=True,
                      show_ticks=True,
                      label_ticks_in_sigma=True,
-                     label_fit_minimum=True,
-                     font_scale=1.0):
+                     label_fit_minimum=True):
         """
         Plot the profile cost function for a parameter.
 
         :param parameter: name of the parameter to profile in
         :type parameter: str
         :param low: Lower bound(s) at which to display confidence levels.
         :type low: float or Sequence[float] or None
@@ -428,23 +427,20 @@
         :param show_ticks: if ``True``, *x* and *y* ticks are displayed
         :type show_ticks: bool
         :param label_ticks_in_sigma: if ``True``, label ticks are in units of 1 sigma
         :type label_ticks_in_sigma: bool
         :param label_fit_minimum: if ``True``, the parameter value and the 1 sigma error
             will be shown as an annotation
         :type label_fit_minimum: bool
-        :param font_scale: multiply font size by this amount.
-        :type font_scale: float
 
         :return: figure containing the plot result
         :rtype: `matplotlib.figure.Figure`
         """
 
         with rc_context(kafe2_rc):
-            rcParams["font.size"] *= font_scale
             if target_axes is None:
                 _fig, _gs = self._make_figure_gs(1, 1)
                 _axes = plt.subplot(_gs[0, 0])
             else:
                 _axes = target_axes
 
             _par_val = self._fit.parameter_name_value_dict[parameter]
@@ -456,35 +452,29 @@
             (_x, _y), _arrow_specs = self._get_profile(
                 parameter, low, high, sigma, cl,
                 arrows=True)
 
             _profile_artist = self._plot_profile_xy(
                 _axes, _x, _y, label="profile %s" % (self._cost_function_formatted_name,))
 
-            _x_min_parabola = np.min(_x)
-            _x_max_parabola = np.max(_x)
             _x_span = np.max(_x) - np.min(_x)
             _y_span = max(np.max(_y) - np.min(_y), np.max(((_x - _par_val) / _par_err) ** 2))
             if _arrow_specs is not None:
                 for _arrow_spec in _arrow_specs:
-                    _x_margin = _arrow_spec.pop("x_margin")
-                    _x_min_parabola = min(_x_min_parabola, _x_margin)
-                    _x_max_parabola = max(_x_max_parabola, _x_margin)
                     self._plot_profile_arrow(
                         _axes, _x_span, _y_span,
                         self._fit._get_model_function_parameter_formatters()[_par_id],
                         **_arrow_spec)
 
             _y_offset = _cost_function_min if not self._profile_kwargs['subtract_min'] else 0.0
 
             _parabola_artist = None
             if show_parabolic:
-                _x_parabola = np.linspace(_x_min_parabola, _x_max_parabola, 101)
                 _parabola_artist = self._plot_parabolic_cost(_axes,
-                                                             _x_parabola,
+                                                             _x,
                                                              quad_coeff=1. / (_par_err**2),
                                                              x_offset=_par_val,
                                                              y_offset=_y_offset,
                                                              label="parabolic approximation")
 
             _minimum_artist = None
             if show_fit_minimum:
@@ -521,15 +511,15 @@
                                                                     label="parameter error")
 
             _axes.set_xlabel(_par_formatted_name)
             _axes.set_ylabel(self._cost_function_formatted_name if not self._profile_kwargs['subtract_min']
                              else '$\\Delta$%s' % self._cost_function_formatted_name)
 
             if show_legend:
-                _axes.legend(loc='center', fontsize=float(rcParams["font.size"]))
+                _axes.legend(loc='center')
 
             if show_grid:
                 _axes.grid('on')
 
             if show_ticks:
                 _loc_x = SigmaLocator(central_value=_par_val, sigma=_par_err)
                 _axes.xaxis.set_major_locator(_loc_x)
@@ -554,16 +544,15 @@
 
     def plot_contours(self, parameter_1, parameter_2, target_axes=None,
                       show_grid=True,
                       show_legend=True,
                       show_fit_minimum=True,
                       show_ticks=True,
                       label_ticks_in_sigma=True,
-                      naming_convention='sigma',
-                      font_scale=1.0):
+                      naming_convention='sigma'):
         """
         Plot the contour for a parameter pair.
 
         :param parameter_1: name of the parameter appearing on the *x* axis
         :type parameter_1: str
         :param parameter_2:  name of the parameter appearing on the *y* axis
         :type parameter_2: str
@@ -578,22 +567,19 @@
         :param show_ticks: if ``True``, *x* and *y* ticks are displayed
         :type show_ticks: bool
         :param label_ticks_in_sigma: if ``True``, label ticks are in units of 1 sigma
         :type label_ticks_in_sigma: bool
         :param naming_convention: if ``'sigma'`` the contour is labelled in sigma, if ``'cl'`` the contour is labelled
                                   in confidence level
         :type naming_convention: str
-        :param font_scale: multiply font size by this amount.
-        :type font_scale: float
 
         :return: figure containing the plot result
         :rtype: `matplotlib.figure.Figure`
         """
         with rc_context(kafe2_rc):
-            rcParams["font.size"] *= font_scale
             if target_axes is None:
                 _fig, _gs = self._make_figure_gs(1, 1)
                 _axes = plt.subplot(_gs[0, 0])
             else:
                 _axes = target_axes
 
             _par_1_id = list(self._fit.parameter_name_value_dict.keys()).index(parameter_1)
@@ -633,15 +619,15 @@
                                                      xerr=_par_1_err, yerr=_par_2_err,
                                                      label="fit minimum")
 
             _axes.set_xlabel(_par_1_formatted_name)
             _axes.set_ylabel(_par_2_formatted_name)
 
             if show_legend:
-                _axes.legend(loc='best', fontsize=float(rcParams["font.size"]))
+                _axes.legend(loc='best')
 
             if show_grid:
                 _axes.grid('on')
 
             if show_ticks:
                 _loc_x = SigmaLocator(central_value=_par_1_val, sigma=_par_1_err)
                 _loc_y = SigmaLocator(central_value=_par_2_val, sigma=_par_2_err)
@@ -673,16 +659,15 @@
                                       show_ticks_for='all',
                                       show_fit_minimum_for='contours',
                                       show_legend=True,
                                       show_parabolic_profiles=True,
                                       show_error_span_profiles=False,
                                       full_matrix=False,
                                       label_ticks_in_sigma=True,
-                                      contour_naming_convention='sigma',
-                                      font_scale=1.0):
+                                      contour_naming_convention='sigma'):
         """
         Plot all profiles and contours to subplots arranges in a matrix-like fashion.
 
         :param parameters: parameters for which to display profiles and contours. If ``None``, all parameters.
         :type parameters: list of parameter names or ``None``
         :param show_grid_for: subplots for which to show a grid
         :type show_grid_for: ``None``, ``'profiles'``, ``'contours'`` or ``'all'``
@@ -701,39 +686,32 @@
         :param full_matrix: if ``True``, contour subplots are also shown above the main diagonal
         :type full_matrix: bool
         :param label_ticks_in_sigma: if ``True``, label ticks are in units of 1 sigma
         :type label_ticks_in_sigma: bool
         :param contour_naming_convention: if ``'sigma'`` the contour is labelled in sigma, if ``'cl'`` the contour is
                                           labelled in confidence level
         :type contour_naming_convention: str
-        :param font_scale: multiply font size by this amount.
-        :type font_scale: float
 
         :return: figure containing the plot result
         :rtype: `matplotlib.figure.Figure`
         """
         with rc_context(kafe2_rc):
-            rcParams["font.size"] *= font_scale
             _par_names = parameters
-            _fixed_pars = list(self._fit._fitter.fixed_parameters.keys())
             if _par_names is None:
                 _par_names = list(self._fit.parameter_name_value_dict.keys())
-                _par_names = [_pn for _pn in _par_names if _pn not in _fixed_pars]
             else:
                 # check if there are any unknown parameters
                 _unknown_parameters = set(_par_names) - set(self._fit.parameter_name_value_dict.keys())
                 if _unknown_parameters:
                     raise ValueError("Unknown parameters: {}".format(_unknown_parameters))
 
-                # check if any of the explicitly requested parameters are fixed
-                _fixed_pars = [_pn for _pn in _par_names if _pn in _fixed_pars]
-                if _fixed_pars:
-                    raise ValueError(
-                        "The following parameters cannot be profiled because they are fixed: "
-                        f"{_fixed_pars}")
+            # # check if any parameters are fixed and exclude them from the matrix:
+            # # TODO: public interface for querying parameter status
+            # _free_pars = set(self._fit._fitter._fit_pars)
+            # _par_names = [_par for _par in _par_names if _par in _free_pars]
 
             _npar = len(_par_names)
             _fig, _gs = self._make_figure_gs(_npar, _npar)
 
             _show_spec_options = ('all', 'profiles', 'contours')
 
             if show_grid_for is not None and show_grid_for not in _show_spec_options:
@@ -764,16 +742,15 @@
                 self.plot_profile(_par_names[row], target_axes=_axes,
                                   show_parabolic=show_parabolic_profiles,
                                   show_grid=_show_grid_profiles,
                                   show_legend=False,
                                   show_fit_minimum=_show_minimum_profiles,
                                   show_error_span=show_error_span_profiles,
                                   label_ticks_in_sigma=label_ticks_in_sigma,
-                                  show_ticks=_show_ticks_profiles,
-                                  font_scale=font_scale)
+                                  show_ticks=_show_ticks_profiles)
 
                 if show_legend:
                     _hs, _ls = _axes.get_legend_handles_labels()
                     _all_legend_handles += tuple(_hs)
                     _all_legend_labels += tuple(_ls)
 
             # draw contours to subplots in the lower (and possibly upper) triangle
@@ -783,16 +760,15 @@
                     self.plot_contours(_par_names[col], _par_names[row],
                                        target_axes=_axes,
                                        show_grid=_show_grid_contours,
                                        show_legend=False,
                                        show_fit_minimum=_show_minimum_contours,
                                        show_ticks=_show_ticks_contours,
                                        label_ticks_in_sigma=label_ticks_in_sigma,
-                                       naming_convention=contour_naming_convention,
-                                       font_scale=font_scale)
+                                       naming_convention=contour_naming_convention)
 
                     if show_legend:
                         _hs, _ls = _axes.get_legend_handles_labels()
                         _all_legend_handles += tuple(_hs)
                         _all_legend_labels += tuple(_ls)
 
                     if full_matrix:
@@ -883,16 +859,15 @@
                     # attach legend to invisible Axes in top right corner
                     _ax_for_legend = _fig.add_subplot(_gs[0, _npar - 1])
                     _ax_for_legend.set_visible(False)
                     _leg = _fig.legend(
                         _hs, _ls,
                         loc='upper right',
                         borderpad=0,
-                        borderaxespad=0,
-                        fontsize=float(rcParams["font.size"])
+                        borderaxespad=0
                     )
                     # patch legend bbox to correspond to axes
                     _leg._bbox_to_anchor = _ax_for_legend.bbox
                 else:
                     # place legend outside regular Axes in top right corner
                     _ax_for_legend = _subplots[0, _npar - 1]
                     _leg = _ax_for_legend.legend(
```

### Comparing `kafe2-2.8.0/kafe2/fit/tools/ensemble.py` & `kafe2-2.8.0rc1/kafe2/fit/tools/ensemble.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/tools/fit_wrapper.py` & `kafe2-2.8.0rc1/kafe2/fit/tools/fit_wrapper.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/tools/kafe2go.py` & `kafe2-2.8.0rc1/kafe2/fit/tools/kafe2go.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/unbinned/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/unbinned/container.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/container.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/unbinned/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/unbinned/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/unbinned/model.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/model.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/unbinned/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/unbinned/plot.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/util/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/util/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/util/function_library.py` & `kafe2-2.8.0rc1/kafe2/fit/util/function_library.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/xy/__init__.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/__init__.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/xy/container.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/container.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/xy/cost.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/cost.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/xy/ensemble.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/ensemble.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/xy/fit.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/xy/model.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/model.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/fit/xy/plot.py` & `kafe2-2.8.0rc1/kafe2/fit/xy/plot.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/minimizers/_base.py` & `kafe2-2.8.0rc1/kafe2/test/core/minimizers/_base.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/minimizers/test_iminuit.py` & `kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_iminuit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/minimizers/test_root_tminuit.py` & `kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_root_tminuit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/minimizers/test_scipy_optimize.py` & `kafe2-2.8.0rc1/kafe2/test/core/minimizers/test_scipy_optimize.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/test_confidence.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_confidence.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/test_cov_mat.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_cov_mat.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/test_gaussian_error.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_gaussian_error.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/test_nexus.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_nexus.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/test_nexus_fitter.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_nexus_fitter.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/core/test_parameter_constraints.py` & `kafe2-2.8.0rc1/kafe2/test/core/test_parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_containers_histogram.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_containers_histogram.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_containers_indexed.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_containers_indexed.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_containers_xy.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_containers_xy.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_cost_functions.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_cost_functions.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_ensemble_tools.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_ensemble_tools.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_fit.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_fit_custom.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_custom.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_fit_hist.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_hist.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_fit_indexed.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_indexed.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_fit_multi.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_multi.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_fit_unbinned.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_unbinned.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_fit_xy.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fit_xy.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_fits_with_parameter_constraints.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_fits_with_parameter_constraints.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_model_functions.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_model_functions.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_plot.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_plot.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_representers_constraint_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_constraint_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_representers_container_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_container_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_representers_fit_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_fit_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_representers_format_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_format_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_representers_model_function_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_model_function_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_representers_parametric_model_yaml.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_representers_parametric_model_yaml.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/fit/test_wrappers.py` & `kafe2-2.8.0rc1/kafe2/test/fit/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/test/tools.py` & `kafe2-2.8.0rc1/kafe2/test/tools.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2/tools.py` & `kafe2-2.8.0rc1/kafe2/tools.py`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/kafe2.egg-info/PKG-INFO` & `kafe2-2.8.0rc1/kafe2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafe2
-Version: 2.8.0
+Version: 2.8.0rc1
 Summary: Karlsruhe Fit Environment 2: a package for fitting and elementary data analysis
 Home-page: https://github.com/PhiLFitters/kafe2
 Author: Daniel Savoiu
 Author-email: daniel.savoiu@cern.ch
 License: GPL3
 Keywords: kafe2 kit karlsruhe data analysis lab laboratory practical courses education university students physics fitting minimization minimisation regression parametric parameter estimation optimization optimisation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `kafe2-2.8.0/kafe2.egg-info/SOURCES.txt` & `kafe2-2.8.0rc1/kafe2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kafe2-2.8.0/setup.py` & `kafe2-2.8.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     test_suite='setup.discover_kafe_tests',
     keywords=("kafe2 kit karlsruhe data analysis lab laboratory practical courses "
               "education university students physics fitting minimization minimisation "
               "regression parametric parameter estimation optimization optimisation"),
     license='GPL3',
     #TODO requirement versions
     install_requires=[
-        'iminuit',
         'NumPy',
         'Numdifftools',
         'Scipy',
         'tabulate',
         'matplotlib',
         'PyYaml',
         'six',
```

