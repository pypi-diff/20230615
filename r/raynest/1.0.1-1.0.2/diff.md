# Comparing `tmp/raynest-1.0.1.tar.gz` & `tmp/raynest-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raynest-1.0.1.tar", last modified: Tue Jun 13 11:15:01 2023, max compression
+gzip compressed data, was "raynest-1.0.2.tar", last modified: Thu Jun 15 13:50:15 2023, max compression
```

## Comparing `raynest-1.0.1.tar` & `raynest-1.0.2.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-13 11:15:01.902919 raynest-1.0.1/
--rw-r--r--   0 wdp        (501) staff       (20)       76 2023-05-19 12:56:52.000000 raynest-1.0.1/DESCRIPTION.rst
--rw-r--r--   0 wdp        (501) staff       (20)      438 2023-05-19 12:56:52.000000 raynest-1.0.1/INSTALL.txt
--rw-r--r--   0 wdp        (501) staff       (20)     1091 2023-05-19 12:56:52.000000 raynest-1.0.1/LICENSE
--rw-r--r--   0 wdp        (501) staff       (20)      142 2023-05-19 12:56:52.000000 raynest-1.0.1/MANIFEST.in
--rw-r--r--   0 wdp        (501) staff       (20)      724 2023-06-13 11:15:01.902981 raynest-1.0.1/PKG-INFO
--rw-r--r--   0 wdp        (501) staff       (20)      898 2023-05-19 13:02:57.000000 raynest-1.0.1/README.rst
-drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-13 11:15:01.893486 raynest-1.0.1/docs/
--rw-r--r--   0 wdp        (501) staff       (20)      603 2023-05-19 12:56:52.000000 raynest-1.0.1/docs/Makefile
--rw-r--r--   0 wdp        (501) staff       (20)     5836 2023-05-19 12:56:52.000000 raynest-1.0.1/docs/conf.py
--rw-r--r--   0 wdp        (501) staff       (20)     4077 2023-05-19 12:56:52.000000 raynest-1.0.1/docs/index.rst
-drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-13 11:15:01.895459 raynest-1.0.1/examples/
--rw-r--r--   0 wdp        (501) staff       (20)     1062 2023-05-19 12:56:52.000000 raynest-1.0.1/examples/ackley.py
--rw-r--r--   0 wdp        (501) staff       (20)     2057 2023-05-23 06:50:15.000000 raynest-1.0.1/examples/burst.py
--rw-r--r--   0 wdp        (501) staff       (20)     1089 2023-05-19 12:56:52.000000 raynest-1.0.1/examples/diagnose_trajectory.py
--rw-r--r--   0 wdp        (501) staff       (20)      729 2023-05-19 12:56:52.000000 raynest-1.0.1/examples/eggbox.py
--rw-r--r--   0 wdp        (501) staff       (20)      365 2023-05-19 12:56:52.000000 raynest-1.0.1/examples/eggbox_profile.py
--rw-r--r--   0 wdp        (501) staff       (20)     1644 2023-05-19 12:56:52.000000 raynest-1.0.1/examples/gaussianmixture.py
--rw-r--r--   0 wdp        (501) staff       (20)     2293 2023-05-19 12:56:52.000000 raynest-1.0.1/examples/memory_footprint.py
--rw-r--r--   0 wdp        (501) staff       (20)      212 2023-05-19 12:56:52.000000 raynest-1.0.1/examples/profiling.py
--rw-r--r--   0 wdp        (501) staff       (20)     1260 2023-05-20 11:54:48.000000 raynest-1.0.1/examples/rosenbrock.py
--rw-r--r--   0 wdp        (501) staff       (20)     2254 2023-06-07 14:29:31.000000 raynest-1.0.1/examples/test_50d.py
--rw-r--r--   0 wdp        (501) staff       (20)      132 2023-05-19 13:39:33.000000 raynest-1.0.1/pyproject.toml
-drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-13 11:15:01.899021 raynest-1.0.1/raynest/
--rw-r--r--   0 wdp        (501) staff       (20)    26312 2023-05-23 06:43:20.000000 raynest-1.0.1/raynest/NestedSampling.py
--rw-r--r--   0 wdp        (501) staff       (20)     1051 2023-06-13 11:10:32.000000 raynest-1.0.1/raynest/__init__.py
-drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-13 11:15:01.901058 raynest-1.0.1/raynest/__pycache__/
--rw-r--r--   0 wdp        (501) staff       (20)    26742 2023-05-23 06:52:49.000000 raynest-1.0.1/raynest/__pycache__/NestedSampling.cpython-39.pyc
--rw-r--r--   0 wdp        (501) staff       (20)      688 2023-05-23 06:52:45.000000 raynest-1.0.1/raynest/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 wdp        (501) staff       (20)    16217 2023-05-19 12:56:52.000000 raynest-1.0.1/raynest/__pycache__/cpnest.cpython-39.pyc
--rw-r--r--   0 wdp        (501) staff       (20)     6076 2023-05-20 11:54:48.000000 raynest-1.0.1/raynest/__pycache__/model.cpython-39.pyc
--rw-r--r--   0 wdp        (501) staff       (20)     8701 2023-05-20 11:54:48.000000 raynest-1.0.1/raynest/__pycache__/nest2pos.cpython-39.pyc
--rw-r--r--   0 wdp        (501) staff       (20)     4636 2023-05-20 11:54:48.000000 raynest-1.0.1/raynest/__pycache__/plot.cpython-39.pyc
--rw-r--r--   0 wdp        (501) staff       (20)    24908 2023-05-24 13:16:55.000000 raynest-1.0.1/raynest/__pycache__/proposal.cpython-39.pyc
--rw-r--r--   0 wdp        (501) staff       (20)    10605 2023-05-23 06:52:49.000000 raynest-1.0.1/raynest/__pycache__/sampler.cpython-39.pyc
--rw-r--r--   0 wdp        (501) staff       (20)     4446 2023-05-20 11:54:48.000000 raynest-1.0.1/raynest/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 wdp        (501) staff       (20)     1763 2023-05-23 11:06:38.000000 raynest-1.0.1/raynest/figaro_gradient.py
--rw-r--r--   0 wdp        (501) staff       (20)     4964 2023-05-19 12:56:52.000000 raynest-1.0.1/raynest/model.py
--rw-r--r--   0 wdp        (501) staff       (20)     8031 2023-05-19 12:56:52.000000 raynest-1.0.1/raynest/nest2pos.py
--rw-r--r--   0 wdp        (501) staff       (20)   446835 2023-06-13 11:15:01.000000 raynest-1.0.1/raynest/parameter.c
--rwxr-xr-x   0 wdp        (501) staff       (20)   114747 2023-05-21 20:18:14.000000 raynest-1.0.1/raynest/parameter.cpython-39-darwin.so
--rw-r--r--   0 wdp        (501) staff       (20)      391 2023-05-19 12:56:52.000000 raynest-1.0.1/raynest/parameter.pxd
--rw-r--r--   0 wdp        (501) staff       (20)     4735 2023-05-19 12:56:52.000000 raynest-1.0.1/raynest/parameter.pyx
--rw-r--r--   0 wdp        (501) staff       (20)     4826 2023-05-19 12:56:52.000000 raynest-1.0.1/raynest/plot.py
--rw-r--r--   0 wdp        (501) staff       (20)    26631 2023-05-24 13:15:28.000000 raynest-1.0.1/raynest/proposal.py
--rw-r--r--   0 wdp        (501) staff       (20)    21569 2023-05-20 11:54:48.000000 raynest-1.0.1/raynest/raynest.py
--rw-r--r--   0 wdp        (501) staff       (20)    14184 2023-06-13 10:40:23.000000 raynest-1.0.1/raynest/sampler.py
--rw-r--r--   0 wdp        (501) staff       (20)     3178 2023-05-19 12:56:52.000000 raynest-1.0.1/raynest/utils.py
-drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-13 11:15:01.899698 raynest-1.0.1/raynest.egg-info/
--rw-r--r--   0 wdp        (501) staff       (20)      724 2023-06-13 11:15:01.000000 raynest-1.0.1/raynest.egg-info/PKG-INFO
--rw-r--r--   0 wdp        (501) staff       (20)     1451 2023-06-13 11:15:01.000000 raynest-1.0.1/raynest.egg-info/SOURCES.txt
--rw-r--r--   0 wdp        (501) staff       (20)        1 2023-06-13 11:15:01.000000 raynest-1.0.1/raynest.egg-info/dependency_links.txt
--rw-r--r--   0 wdp        (501) staff       (20)       63 2023-06-13 11:15:01.000000 raynest-1.0.1/raynest.egg-info/requires.txt
--rw-r--r--   0 wdp        (501) staff       (20)        8 2023-06-13 11:15:01.000000 raynest-1.0.1/raynest.egg-info/top_level.txt
--rw-r--r--   0 wdp        (501) staff       (20)       64 2023-05-19 12:56:52.000000 raynest-1.0.1/requirements.txt
--rw-r--r--   0 wdp        (501) staff       (20)      125 2023-06-13 11:15:01.903210 raynest-1.0.1/setup.cfg
--rw-r--r--   0 wdp        (501) staff       (20)     2795 2023-06-13 11:13:17.000000 raynest-1.0.1/setup.py
-drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-13 11:15:01.902701 raynest-1.0.1/tests/
--rw-r--r--   0 wdp        (501) staff       (20)       46 2023-05-19 12:56:52.000000 raynest-1.0.1/tests/__init__.py
--rw-r--r--   0 wdp        (501) staff       (20)     2354 2023-05-19 12:56:52.000000 raynest-1.0.1/tests/test_1d.py
--rw-r--r--   0 wdp        (501) staff       (20)     1512 2023-05-19 12:56:52.000000 raynest-1.0.1/tests/test_2d.py
--rw-r--r--   0 wdp        (501) staff       (20)     1439 2023-05-23 06:50:15.000000 raynest-1.0.1/tests/test_2d_hmc.py
--rw-r--r--   0 wdp        (501) staff       (20)     1334 2023-05-19 12:56:52.000000 raynest-1.0.1/tests/test_2d_slice.py
--rw-r--r--   0 wdp        (501) staff       (20)     1183 2023-05-19 12:56:52.000000 raynest-1.0.1/tests/test_gaussian.py
--rw-r--r--   0 wdp        (501) staff       (20)     2122 2023-05-19 12:56:52.000000 raynest-1.0.1/tests/test_half_gaussian.py
--rw-r--r--   0 wdp        (501) staff       (20)     1537 2023-05-19 12:56:52.000000 raynest-1.0.1/tests/test_ring.py
--rw-r--r--   0 wdp        (501) staff       (20)     1526 2023-05-19 12:56:52.000000 raynest-1.0.1/tests/test_ring_slice.py
--rw-r--r--   0 wdp        (501) staff       (20)     1299 2023-05-19 12:56:52.000000 raynest-1.0.1/tests/test_verbosity.py
+drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-15 13:50:15.876257 raynest-1.0.2/
+-rw-r--r--   0 wdp        (501) staff       (20)       76 2023-05-19 12:56:52.000000 raynest-1.0.2/DESCRIPTION.rst
+-rw-r--r--   0 wdp        (501) staff       (20)      438 2023-05-19 12:56:52.000000 raynest-1.0.2/INSTALL.txt
+-rw-r--r--   0 wdp        (501) staff       (20)     1091 2023-05-19 12:56:52.000000 raynest-1.0.2/LICENSE
+-rw-r--r--   0 wdp        (501) staff       (20)      142 2023-05-19 12:56:52.000000 raynest-1.0.2/MANIFEST.in
+-rw-r--r--   0 wdp        (501) staff       (20)      724 2023-06-15 13:50:15.876330 raynest-1.0.2/PKG-INFO
+-rw-r--r--   0 wdp        (501) staff       (20)      898 2023-05-19 13:02:57.000000 raynest-1.0.2/README.rst
+drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-15 13:50:15.865944 raynest-1.0.2/docs/
+-rw-r--r--   0 wdp        (501) staff       (20)      603 2023-05-19 12:56:52.000000 raynest-1.0.2/docs/Makefile
+-rw-r--r--   0 wdp        (501) staff       (20)     5836 2023-05-19 12:56:52.000000 raynest-1.0.2/docs/conf.py
+-rw-r--r--   0 wdp        (501) staff       (20)     4077 2023-05-19 12:56:52.000000 raynest-1.0.2/docs/index.rst
+drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-15 13:50:15.867650 raynest-1.0.2/examples/
+-rw-r--r--   0 wdp        (501) staff       (20)     1062 2023-05-19 12:56:52.000000 raynest-1.0.2/examples/ackley.py
+-rw-r--r--   0 wdp        (501) staff       (20)     2057 2023-05-23 06:50:15.000000 raynest-1.0.2/examples/burst.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1089 2023-05-19 12:56:52.000000 raynest-1.0.2/examples/diagnose_trajectory.py
+-rw-r--r--   0 wdp        (501) staff       (20)      729 2023-05-19 12:56:52.000000 raynest-1.0.2/examples/eggbox.py
+-rw-r--r--   0 wdp        (501) staff       (20)      365 2023-05-19 12:56:52.000000 raynest-1.0.2/examples/eggbox_profile.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1644 2023-05-19 12:56:52.000000 raynest-1.0.2/examples/gaussianmixture.py
+-rw-r--r--   0 wdp        (501) staff       (20)     2293 2023-05-19 12:56:52.000000 raynest-1.0.2/examples/memory_footprint.py
+-rw-r--r--   0 wdp        (501) staff       (20)      212 2023-05-19 12:56:52.000000 raynest-1.0.2/examples/profiling.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1260 2023-05-20 11:54:48.000000 raynest-1.0.2/examples/rosenbrock.py
+-rw-r--r--   0 wdp        (501) staff       (20)     2254 2023-06-07 14:29:31.000000 raynest-1.0.2/examples/test_50d.py
+-rw-r--r--   0 wdp        (501) staff       (20)      132 2023-05-19 13:39:33.000000 raynest-1.0.2/pyproject.toml
+drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-15 13:50:15.871325 raynest-1.0.2/raynest/
+-rw-r--r--   0 wdp        (501) staff       (20)    26312 2023-05-23 06:43:20.000000 raynest-1.0.2/raynest/NestedSampling.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1051 2023-06-15 13:29:24.000000 raynest-1.0.2/raynest/__init__.py
+drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-15 13:50:15.874381 raynest-1.0.2/raynest/__pycache__/
+-rw-r--r--   0 wdp        (501) staff       (20)    26742 2023-05-23 06:52:49.000000 raynest-1.0.2/raynest/__pycache__/NestedSampling.cpython-39.pyc
+-rw-r--r--   0 wdp        (501) staff       (20)      688 2023-06-13 16:12:35.000000 raynest-1.0.2/raynest/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 wdp        (501) staff       (20)    16217 2023-05-19 12:56:52.000000 raynest-1.0.2/raynest/__pycache__/cpnest.cpython-39.pyc
+-rw-r--r--   0 wdp        (501) staff       (20)     6076 2023-05-20 11:54:48.000000 raynest-1.0.2/raynest/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0 wdp        (501) staff       (20)     8701 2023-05-20 11:54:48.000000 raynest-1.0.2/raynest/__pycache__/nest2pos.cpython-39.pyc
+-rw-r--r--   0 wdp        (501) staff       (20)     4636 2023-05-20 11:54:48.000000 raynest-1.0.2/raynest/__pycache__/plot.cpython-39.pyc
+-rw-r--r--   0 wdp        (501) staff       (20)    24908 2023-05-24 13:16:55.000000 raynest-1.0.2/raynest/__pycache__/proposal.cpython-39.pyc
+-rw-r--r--   0 wdp        (501) staff       (20)    10722 2023-06-13 16:13:11.000000 raynest-1.0.2/raynest/__pycache__/sampler.cpython-39.pyc
+-rw-r--r--   0 wdp        (501) staff       (20)     4446 2023-05-20 11:54:48.000000 raynest-1.0.2/raynest/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 wdp        (501) staff       (20)     1877 2023-06-15 13:29:02.000000 raynest-1.0.2/raynest/figaro_gradient.py
+-rw-r--r--   0 wdp        (501) staff       (20)     4964 2023-05-19 12:56:52.000000 raynest-1.0.2/raynest/model.py
+-rw-r--r--   0 wdp        (501) staff       (20)     8031 2023-05-19 12:56:52.000000 raynest-1.0.2/raynest/nest2pos.py
+-rw-r--r--   0 wdp        (501) staff       (20)   446835 2023-06-15 13:50:14.000000 raynest-1.0.2/raynest/parameter.c
+-rw-r--r--   0 wdp        (501) staff       (20)      391 2023-05-19 12:56:52.000000 raynest-1.0.2/raynest/parameter.pxd
+-rw-r--r--   0 wdp        (501) staff       (20)     4735 2023-05-19 12:56:52.000000 raynest-1.0.2/raynest/parameter.pyx
+-rw-r--r--   0 wdp        (501) staff       (20)     4826 2023-05-19 12:56:52.000000 raynest-1.0.2/raynest/plot.py
+-rw-r--r--   0 wdp        (501) staff       (20)    26631 2023-05-24 13:15:28.000000 raynest-1.0.2/raynest/proposal.py
+-rw-r--r--   0 wdp        (501) staff       (20)    21422 2023-06-15 13:46:20.000000 raynest-1.0.2/raynest/raynest.py
+-rw-r--r--   0 wdp        (501) staff       (20)    14184 2023-06-13 10:40:23.000000 raynest-1.0.2/raynest/sampler.py
+-rw-r--r--   0 wdp        (501) staff       (20)     3178 2023-05-19 12:56:52.000000 raynest-1.0.2/raynest/utils.py
+drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-15 13:50:15.872016 raynest-1.0.2/raynest.egg-info/
+-rw-r--r--   0 wdp        (501) staff       (20)      724 2023-06-15 13:50:15.000000 raynest-1.0.2/raynest.egg-info/PKG-INFO
+-rw-r--r--   0 wdp        (501) staff       (20)     1412 2023-06-15 13:50:15.000000 raynest-1.0.2/raynest.egg-info/SOURCES.txt
+-rw-r--r--   0 wdp        (501) staff       (20)        1 2023-06-15 13:50:15.000000 raynest-1.0.2/raynest.egg-info/dependency_links.txt
+-rw-r--r--   0 wdp        (501) staff       (20)       63 2023-06-15 13:50:15.000000 raynest-1.0.2/raynest.egg-info/requires.txt
+-rw-r--r--   0 wdp        (501) staff       (20)        8 2023-06-15 13:50:15.000000 raynest-1.0.2/raynest.egg-info/top_level.txt
+-rw-r--r--   0 wdp        (501) staff       (20)       64 2023-05-19 12:56:52.000000 raynest-1.0.2/requirements.txt
+-rw-r--r--   0 wdp        (501) staff       (20)      125 2023-06-15 13:50:15.876549 raynest-1.0.2/setup.cfg
+-rw-r--r--   0 wdp        (501) staff       (20)     2795 2023-06-15 13:29:35.000000 raynest-1.0.2/setup.py
+drwxr-xr-x   0 wdp        (501) staff       (20)        0 2023-06-15 13:50:15.876050 raynest-1.0.2/tests/
+-rw-r--r--   0 wdp        (501) staff       (20)       46 2023-05-19 12:56:52.000000 raynest-1.0.2/tests/__init__.py
+-rw-r--r--   0 wdp        (501) staff       (20)     2354 2023-05-19 12:56:52.000000 raynest-1.0.2/tests/test_1d.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1512 2023-05-19 12:56:52.000000 raynest-1.0.2/tests/test_2d.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1439 2023-05-23 06:50:15.000000 raynest-1.0.2/tests/test_2d_hmc.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1334 2023-05-19 12:56:52.000000 raynest-1.0.2/tests/test_2d_slice.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1183 2023-05-19 12:56:52.000000 raynest-1.0.2/tests/test_gaussian.py
+-rw-r--r--   0 wdp        (501) staff       (20)     2122 2023-05-19 12:56:52.000000 raynest-1.0.2/tests/test_half_gaussian.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1537 2023-05-19 12:56:52.000000 raynest-1.0.2/tests/test_ring.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1526 2023-05-19 12:56:52.000000 raynest-1.0.2/tests/test_ring_slice.py
+-rw-r--r--   0 wdp        (501) staff       (20)     1299 2023-05-19 12:56:52.000000 raynest-1.0.2/tests/test_verbosity.py
```

### Comparing `raynest-1.0.1/LICENSE` & `raynest-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/PKG-INFO` & `raynest-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raynest
-Version: 1.0.1
+Version: 1.0.2
 Summary: raynest: Parallel nested sampling based on ray
 Home-page: https://github.com/wdpozzo/raynest
 Author: Walter Del Pozzo, John Veitch
 Author-email: walter.delpozzo@ligo.org, john.veitch@ligo.org
 License: MIT
 Keywords: nested sampling bayesian inference
 Classifier: Development Status :: 4 - Beta
```

### Comparing `raynest-1.0.1/README.rst` & `raynest-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/docs/Makefile` & `raynest-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/docs/conf.py` & `raynest-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/docs/index.rst` & `raynest-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/examples/ackley.py` & `raynest-1.0.2/examples/ackley.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/examples/burst.py` & `raynest-1.0.2/examples/burst.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/examples/diagnose_trajectory.py` & `raynest-1.0.2/examples/diagnose_trajectory.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/examples/eggbox.py` & `raynest-1.0.2/examples/eggbox.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/examples/gaussianmixture.py` & `raynest-1.0.2/examples/gaussianmixture.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/examples/memory_footprint.py` & `raynest-1.0.2/examples/memory_footprint.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/examples/rosenbrock.py` & `raynest-1.0.2/examples/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/examples/test_50d.py` & `raynest-1.0.2/examples/test_50d.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/NestedSampling.py` & `raynest-1.0.2/raynest/NestedSampling.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/__init__.py` & `raynest-1.0.2/raynest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 logger.addHandler(logging.NullHandler())
 
 console_handler = StreamHandler(verbose=0)  # default console verbosity is 0
 logger.addHandler(console_handler)
 # To change the console handler verbosity:
 #   from raynest import console_handler
 #   console_handler.set_verbosity(2)
-__version__="1.0.1"
+__version__="1.0.2"
 
 from .raynest import raynest
 
 # Get the version number from git tag
 from pkg_resources import get_distribution, DistributionNotFound
 try:
     __version__ = get_distribution(__name__).version
```

### Comparing `raynest-1.0.1/raynest/__pycache__/NestedSampling.cpython-39.pyc` & `raynest-1.0.2/raynest/__pycache__/NestedSampling.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/__pycache__/__init__.cpython-39.pyc` & `raynest-1.0.2/raynest/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat May 20 11:54:48 2023 UTC, .py size: 1051 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 08b5 6864 1b04 0000  a.........hd....
+00000000: 610d 0d0a 0000 0000 a84e 8864 1b04 0000  a........N.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 a400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6500 a004 6404 a101 5a05  m.Z...e...d...Z.
 00000050: 6505 a006 6503 6405 1900 a101 0100 6505  e...e.d.......e.
 00000060: a007 6500 a008 a100 a101 0100 6502 6400  ..e.........e.d.
 00000070: 6406 8d01 5a09 6505 a007 6509 a101 0100  d...Z.e...e.....
@@ -11,33 +11,33 @@
 000000a0: 7a0e 650d 650f 8301 6a10 5a0a 5700 6e16  z.e.e...j.Z.W.n.
 000000b0: 0400 650e 7996 0100 0100 0100 640a 5a0a  ..e.y.......d.Z.
 000000c0: 5900 6e02 3000 6700 640b a201 5a11 6401  Y.n.0.g.d...Z.d.
 000000d0: 5300 290c e900 0000 004e e901 0000 0029  S.)......N.....)
 000000e0: 02da 0d53 7472 6561 6d48 616e 646c 6572  ...StreamHandler
 000000f0: da06 4c45 5645 4c53 da07 7261 796e 6573  ..LEVELS..raynes
 00000100: 74e9 ffff ffff 2901 da07 7665 7262 6f73  t.....)...verbos
-00000110: 657a 0531 2e30 2e30 2901 7205 0000 0029  ez.1.0.0).r....)
+00000110: 657a 0531 2e30 2e31 2901 7205 0000 0029  ez.1.0.1).r....)
 00000120: 02da 1067 6574 5f64 6973 7472 6962 7574  ...get_distribut
 00000130: 696f 6eda 1444 6973 7472 6962 7574 696f  ion..Distributio
 00000140: 6e4e 6f74 466f 756e 64da 0364 6576 2909  nNotFound..dev).
 00000150: da05 6d6f 6465 6c5a 0e4e 6573 7465 6453  ..modelZ.NestedS
 00000160: 616d 706c 696e 675a 0970 6172 616d 6574  amplingZ.paramet
-00000170: 6572 5a07 7361 6d70 6c65 7272 0500 0000  erZ.samplerr....
+00000170: 6572 da07 7361 6d70 6c65 7272 0500 0000  er..samplerr....
 00000180: 5a08 6e65 7374 3270 6f73 5a08 7072 6f70  Z.nest2posZ.prop
-00000190: 6f73 616c 5a04 706c 6f74 da06 6c6f 6767  osalZ.plot..logg
+00000190: 6f73 616c da04 706c 6f74 da06 6c6f 6767  osal..plot..logg
 000001a0: 6572 2912 da07 6c6f 6767 696e 67da 0575  er)...logging..u
-000001b0: 7469 6c73 7203 0000 0072 0400 0000 5a09  tilsr....r....Z.
-000001c0: 6765 744c 6f67 6765 7272 0c00 0000 5a08  getLoggerr....Z.
-000001d0: 7365 744c 6576 656c 5a0a 6164 6448 616e  setLevelZ.addHan
-000001e0: 646c 6572 5a0b 4e75 6c6c 4861 6e64 6c65  dlerZ.NullHandle
+000001b0: 7469 6c73 7203 0000 0072 0400 0000 da09  tilsr....r......
+000001c0: 6765 744c 6f67 6765 7272 0e00 0000 da08  getLoggerr......
+000001d0: 7365 744c 6576 656c da0a 6164 6448 616e  setLevel..addHan
+000001e0: 646c 6572 da0b 4e75 6c6c 4861 6e64 6c65  dler..NullHandle
 000001f0: 725a 0f63 6f6e 736f 6c65 5f68 616e 646c  rZ.console_handl
 00000200: 6572 da0b 5f5f 7665 7273 696f 6e5f 5f72  er..__version__r
-00000210: 0500 0000 5a0d 706b 675f 7265 736f 7572  ....Z.pkg_resour
+00000210: 0500 0000 da0d 706b 675f 7265 736f 7572  ......pkg_resour
 00000220: 6365 7372 0800 0000 7209 0000 00da 085f  cesr....r......_
 00000230: 5f6e 616d 655f 5fda 0776 6572 7369 6f6e  _name__..version
-00000240: da07 5f5f 616c 6c5f 5fa9 0072 1300 0000  ..__all__..r....
-00000250: 7213 0000 00fa 2a2f 5573 6572 732f 7764  r.....*/Users/wd
+00000240: da07 5f5f 616c 6c5f 5fa9 0072 1a00 0000  ..__all__..r....
+00000250: 721a 0000 00fa 2a2f 5573 6572 732f 7764  r.....*/Users/wd
 00000260: 702f 7372 632f 7261 796e 6573 742f 7261  p/src/raynest/ra
 00000270: 796e 6573 742f 5f5f 696e 6974 5f5f 2e70  ynest/__init__.p
 00000280: 79da 083c 6d6f 6475 6c65 3e01 0000 0073  y..<module>....s
 00000290: 1c00 0000 0801 1003 0a01 0e01 0e02 0a01  ................
 000002a0: 0a04 0402 0c03 1001 0201 0e01 0c02 0a02  ................
```

### Comparing `raynest-1.0.1/raynest/__pycache__/cpnest.cpython-39.pyc` & `raynest-1.0.2/raynest/__pycache__/cpnest.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/__pycache__/model.cpython-39.pyc` & `raynest-1.0.2/raynest/__pycache__/model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/__pycache__/nest2pos.cpython-39.pyc` & `raynest-1.0.2/raynest/__pycache__/nest2pos.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/__pycache__/plot.cpython-39.pyc` & `raynest-1.0.2/raynest/__pycache__/plot.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/__pycache__/proposal.cpython-39.pyc` & `raynest-1.0.2/raynest/__pycache__/proposal.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/__pycache__/sampler.cpython-39.pyc` & `raynest-1.0.2/raynest/__pycache__/sampler.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue May 23 06:50:21 2023 UTC, .py size: 14077 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,663 +1,671 @@
-00000000: 610d 0d0a 0000 0000 2d62 6c64 fd36 0000  a.......-bld.6..
+00000000: 610d 0d0a 0000 0000 9747 8864 6837 0000  a........G.dh7..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 2a01 0000 6400  .....@...s*...d.
+00000020: 0006 0000 0040 0000 0073 4401 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6400 6402 6c05 5a06 6400 6403 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6405 6406 6c0b 6d0c 5a0c 0100 6405  ..d.d.l.m.Z...d.
 00000080: 6407 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6405  d.l.m.Z.m.Z...d.
 00000090: 6408 6c0b 6d0d 5a0d 0100 6400 6402 6c10  d.l.m.Z...d.d.l.
 000000a0: 6d11 0200 0100 6d12 5a13 0100 6400 6402  m.....m.Z...d.d.
 000000b0: 6c14 5a14 6405 6409 6c15 6d16 5a16 6d17  l.Z.d.d.l.m.Z.m.
 000000c0: 5a17 0100 6400 6402 6c18 5a18 6400 6402  Z...d.d.l.Z.d.d.
 000000d0: 6c19 5a19 6400 6402 6c1a 5a1a 640a 5a1b  l.Z.d.d.l.Z.d.Z.
 000000e0: 4700 640b 640c 8400 640c 651c 8303 5a1d  G.d.d...d.e...Z.
 000000f0: 6518 6a1e 4700 640d 640e 8400 640e 651d  e.j.G.d.d...d.e.
-00000100: 8303 8301 5a1f 6405 640f 6c20 6d21 5a21  ....Z.d.d.l m!Z!
-00000110: 0100 6518 6a1e 4700 6410 6411 8400 6411  ..e.j.G.d.d...d.
-00000120: 651d 8303 8301 5a22 6518 6a1e 4700 6412  e.....Z"e.j.G.d.
-00000130: 6413 8400 6413 651d 8303 8301 5a23 6518  d...d.e.....Z#e.
-00000140: 6a1e 4700 6414 6415 8400 6415 651d 8303  j.G.d.d...d.e...
-00000150: 8301 5a24 6402 5300 2916 e900 0000 0029  ..Z$d.S.)......)
-00000160: 01da 0864 6976 6973 696f 6e4e 2901 da03  ...divisionN)...
-00000170: 6c6f 6729 01da 0564 6571 7565 e901 0000  log)...deque....
-00000180: 0029 01da 0970 6172 616d 6574 6572 2902  .)...parameter).
-00000190: da14 4465 6661 756c 7450 726f 706f 7361  ..DefaultProposa
-000001a0: 6c43 7963 6c65 da10 456e 7365 6d62 6c65  lCycle..Ensemble
-000001b0: 5072 6f70 6f73 616c 2901 da08 7072 6f70  Proposal)...prop
-000001c0: 6f73 616c 2902 da03 6163 6cda 0f61 7574  osal)...acl..aut
-000001d0: 6f63 6f72 7265 6c61 7469 6f6e 4663 0000  ocorrelationFc..
-000001e0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-000001f0: 0000 4000 0000 733e 0000 0065 005a 0164  ..@...s>...e.Z.d
-00000200: 005a 0264 015a 0364 1064 0464 0584 015a  .Z.d.Z.d.d.d...Z
-00000210: 0464 1164 0764 0884 015a 0564 1264 0a64  .d.d.d...Z.d.d.d
-00000220: 0b84 015a 0664 0c64 0d84 005a 0764 0e64  ...Z.d.d...Z.d.d
-00000230: 0f84 005a 0864 0253 0029 13da 0753 616d  ...Z.d.S.)...Sam
-00000240: 706c 6572 61e5 0100 000a 2020 2020 5361  plera.....    Sa
-00000250: 6d70 6c65 7220 636c 6173 732e 0a20 2020  mpler class..   
-00000260: 202d 2d2d 2d2d 2d2d 2d2d 0a0a 2020 2020   ---------..    
-00000270: 496e 6974 6961 6c69 7361 7469 6f6e 2061  Initialisation a
-00000280: 7267 756d 656e 7473 3a0a 0a20 2020 2061  rguments:..    a
-00000290: 7267 733a 0a20 2020 206d 6f64 656c 3a20  rgs:.    model: 
-000002a0: 3a6f 626a 3a60 7261 796e 6573 742e 4d6f  :obj:`raynest.Mo
-000002b0: 6465 6c60 2075 7365 7220 6465 6669 6e65  del` user define
-000002c0: 6420 6d6f 6465 6c20 746f 2073 616d 706c  d model to sampl
-000002d0: 650a 0a20 2020 206d 6178 6d63 6d63 3a0a  e..    maxmcmc:.
-000002e0: 2020 2020 2020 2020 3a69 6e74 3a20 6d61          :int: ma
-000002f0: 7869 6d75 6d20 6e75 6d62 6572 206f 6620  ximum number of 
-00000300: 6d63 6d63 2073 7465 7073 2074 6f20 6265  mcmc steps to be
-00000310: 2075 7365 6420 696e 2074 6865 203a 6f62   used in the :ob
-00000320: 6a3a 6063 6e65 7374 2e73 616d 706c 6572  j:`cnest.sampler
-00000330: 2e53 616d 706c 6572 600a 0a20 2020 202d  .Sampler`..    -
-00000340: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6b77  ---------.    kw
-00000350: 6172 6773 3a0a 0a20 2020 2076 6572 626f  args:..    verbo
-00000360: 7365 3a0a 2020 2020 2020 2020 3a69 6e74  se:.        :int
-00000370: 3a20 6469 7370 6c61 7920 6465 6275 6720  : display debug 
-00000380: 696e 666f 726d 6174 696f 6e20 6f6e 2073  information on s
-00000390: 6372 6565 6e0a 2020 2020 2020 2020 4465  creen.        De
-000003a0: 6661 756c 743a 2030 0a0a 2020 2020 7072  fault: 0..    pr
-000003b0: 6f70 6f73 616c 3a0a 2020 2020 2020 2020  oposal:.        
-000003c0: 3a6f 626a 3a60 7261 796e 6573 742e 7072  :obj:`raynest.pr
-000003d0: 6f70 6f73 616c 732e 5072 6f70 6f73 616c  oposals.Proposal
-000003e0: 6020 746f 2075 7365 0a20 2020 2020 2020  ` to use.       
-000003f0: 2044 6566 6175 6c74 733a 203a 6f62 6a3a   Defaults: :obj:
-00000400: 6072 6179 6e65 7374 2e70 726f 706f 7361  `raynest.proposa
-00000410: 6c73 2e44 6566 6175 6c74 5072 6f70 6f73  ls.DefaultPropos
-00000420: 616c 4379 636c 6560 290a 2020 2020 4e72  alCycle`).    Nr
-00000430: 0100 0000 6306 0000 0000 0000 0000 0000  ....c...........
-00000440: 0006 0000 0004 0000 0043 0000 0073 d000  .........C...s..
-00000450: 0000 6401 7c00 5f00 7c01 7c00 5f01 7c03  ..d.|._.|.|._.|.
-00000460: 6400 6b02 7222 7402 6a03 a004 a100 7c00  d.k.r"t.j.....|.
-00000470: 5f05 6e06 7c03 7c00 5f05 7c02 6402 1a00  _.n.|.|._.|.d...
-00000480: 7c00 5f06 7c02 7c00 5f07 6400 7c00 5f08  |._.|.|._.d.|._.
-00000490: 7409 a00a 6403 a101 7c00 5f0b 7c05 6400  t...d...|._.|.d.
-000004a0: 7500 7260 740c 7c00 6a05 8301 7c00 5f0d  u.r`t.|.j...|._.
-000004b0: 6e12 7c05 7c00 6a05 7c00 6a01 6404 8d02  n.|.|.j.|.j.d...
-000004c0: 7c00 5f0d 7c00 6a06 7c00 5f0e 740f 7c00  |._.|.j.|._.t.|.
-000004d0: 6a06 8301 7c00 5f10 7c04 7c00 5f11 6405  j...|._.|.|._.d.
-000004e0: 7c00 5f12 6405 7c00 5f13 6401 7c00 5f14  |._.d.|._.d.|._.
-000004f0: 6401 7c00 5f15 6406 7c00 5f16 6407 7c00  d.|._.d.|._.d.|.
-00000500: 5f17 7418 7c00 6a11 6408 6b05 72c0 6400  _.t.|.j.d.k.r.d.
-00000510: 6e04 7c00 6a17 6409 8d01 7c00 5f19 6400  n.|.j.d...|._.d.
-00000520: 5300 290a 4e72 0100 0000 e90a 0000 00da  S.).Nr..........
-00000530: 0772 6179 6e65 7374 2901 da05 6d6f 6465  .raynest)...mode
-00000540: 6ce7 0000 0000 0000 0000 4669 0080 0000  l.........Fi....
-00000550: e903 0000 0029 01da 066d 6178 6c65 6e29  .....)...maxlen)
-00000560: 1ada 0763 6f75 6e74 6572 720f 0000 00da  ...counterr.....
-00000570: 026e 70da 0672 616e 646f 6dda 0b64 6566  .np..random..def
-00000580: 6175 6c74 5f72 6e67 da03 726e 675a 0c69  ault_rng..rngZ.i
-00000590: 6e69 7469 616c 5f6d 636d 63da 076d 6178  nitial_mcmc..max
-000005a0: 6d63 6d63 da03 7461 75da 076c 6f67 6769  mcmc..tau..loggi
-000005b0: 6e67 da09 6765 744c 6f67 6765 72da 066c  ng..getLogger..l
-000005c0: 6f67 6765 7272 0700 0000 7209 0000 00da  oggerr....r.....
-000005d0: 054e 6d63 6d63 da05 666c 6f61 74da 0b4e  .Nmcmc..float..N
-000005e0: 6d63 6d63 5f65 7861 6374 da07 7665 7262  mcmc_exact..verb
-000005f0: 6f73 65da 0a61 6363 6570 7461 6e63 65da  ose..acceptance.
-00000600: 0e73 7562 5f61 6363 6570 7461 6e63 65da  .sub_acceptance.
-00000610: 0d6d 636d 635f 6163 6365 7074 6564 da0c  .mcmc_accepted..
-00000620: 6d63 6d63 5f63 6f75 6e74 6572 da0b 696e  mcmc_counter..in
-00000630: 6974 6961 6c69 7365 64da 0b6d 6178 5f73  itialised..max_s
-00000640: 746f 7261 6765 7204 0000 00da 0773 616d  torager......sam
-00000650: 706c 6573 2906 da04 7365 6c66 720f 0000  ples)...selfr...
-00000660: 0072 1800 0000 7217 0000 0072 2000 0000  .r....r....r ...
-00000670: 7209 0000 00a9 0072 2900 0000 fa29 2f55  r......r)....)/U
-00000680: 7365 7273 2f77 6470 2f73 7263 2f72 6179  sers/wdp/src/ray
-00000690: 6e65 7374 2f72 6179 6e65 7374 2f73 616d  nest/raynest/sam
-000006a0: 706c 6572 2e70 79da 085f 5f69 6e69 745f  pler.py..__init_
-000006b0: 5f2f 0000 0073 2c00 0000 0007 0601 0601  _/...s,.........
-000006c0: 0801 0e02 0601 0a01 0601 0601 0c02 0801  ................
-000006d0: 0e02 1202 0801 0c02 0601 0601 0601 0601  ................
-000006e0: 0601 0601 0601 7a10 5361 6d70 6c65 722e  ......z.Sampler.
-000006f0: 5f5f 696e 6974 5f5f e905 0000 0063 0300  __init__.....c..
-00000700: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00000710: 0000 4300 0000 7384 0000 007c 0264 0175  ..C...s....|.d.u
-00000720: 0072 0e7c 006a 007d 027c 006a 0164 026b  .r.|.j.}.|.j.d.k
-00000730: 0272 2e64 0364 037c 021b 0017 007c 006a  .r.d.d.|.....|.j
-00000740: 0214 007c 005f 026e 2a64 0364 037c 021b  ...|._.n*d.d.|..
-00000750: 0018 007c 006a 0214 007c 017c 021b 0064  ...|.j...|.|...d
-00000760: 047c 006a 011b 0064 0318 0014 0017 007c  .|.j...d.......|
-00000770: 005f 0274 0374 047c 006a 027c 006a 0083  ._.t.t.|.j.|.j..
-00000780: 0283 017c 005f 0274 057c 0174 067c 006a  ...|._.t.|.t.|.j
-00000790: 0283 0183 027c 005f 077c 006a 0753 0029  .....|._.|.j.S.)
-000007a0: 0561 3601 0000 0a20 2020 2020 2020 2045  .a6....        E
-000007b0: 7374 696d 6174 6520 6175 746f 636f 7272  stimate autocorr
-000007c0: 656c 6174 696f 6e20 6c65 6e67 7468 206f  elation length o
-000007d0: 6620 6368 6169 6e20 7573 696e 6720 6163  f chain using ac
-000007e0: 6365 7074 616e 6365 2066 7261 6374 696f  ceptance fractio
-000007f0: 6e0a 2020 2020 2020 2020 4143 4c20 3d20  n.        ACL = 
-00000800: 2832 2f61 6363 2920 2d20 310a 2020 2020  (2/acc) - 1.    
-00000810: 2020 2020 6d75 6c74 6970 6c69 6564 2062      multiplied b
-00000820: 7920 6120 7361 6665 7479 206d 6172 6769  y a safety margi
-00000830: 6e20 6f66 2035 0a20 2020 2020 2020 2055  n of 5.        U
-00000840: 7365 7320 6d6f 7669 6e67 2061 7665 7261  ses moving avera
-00000850: 6765 2077 6974 6820 6465 6361 7920 7469  ge with decay ti
-00000860: 6d65 2074 6175 2069 7465 7261 7469 6f6e  me tau iteration
-00000870: 730a 2020 2020 2020 2020 2864 6566 6175  s.        (defau
-00000880: 6c74 3a20 3a69 6e74 3a60 7365 6c66 2e6d  lt: :int:`self.m
-00000890: 6178 6d63 6d63 6029 0a0a 2020 2020 2020  axmcmc`)..      
-000008a0: 2020 5461 6b65 6e20 6672 6f6d 2068 7474    Taken from htt
-000008b0: 703a 2f2f 6769 7468 7562 2e63 6f6d 2f66  p://github.com/f
-000008c0: 6172 722f 456e 7365 6d62 6c65 4e65 7374  arr/EnsembleNest
-000008d0: 2e6a 6c0a 2020 2020 2020 2020 4e72 1000  .jl.        Nr..
-000008e0: 0000 e700 0000 0000 00f0 3f67 0000 0000  ..........?g....
-000008f0: 0000 0040 2908 7218 0000 0072 2200 0000  ...@).r....r"...
-00000900: 721f 0000 0072 1e00 0000 da03 6d69 6eda  r....r......min.
-00000910: 036d 6178 da03 696e 7472 1d00 0000 2903  .max..intr....).
-00000920: 7228 0000 00da 0673 6166 6574 7972 1900  r(.....safetyr..
-00000930: 0000 7229 0000 0072 2900 0000 722a 0000  ..r)...r)...r*..
-00000940: 00da 1965 7374 696d 6174 655f 6e6d 636d  ...estimate_nmcm
-00000950: 635f 6f6e 5f74 6865 5f66 6c79 5200 0000  c_on_the_flyR...
-00000960: 730e 0000 0000 0c0e 030a 0116 022a 0214  s............*..
-00000970: 0112 027a 2153 616d 706c 6572 2e65 7374  ...z!Sampler.est
-00000980: 696d 6174 655f 6e6d 636d 635f 6f6e 5f74  imate_nmcmc_on_t
-00000990: 6865 5f66 6c79 7205 0000 0063 0200 0000  he_flyr....c....
-000009a0: 0000 0000 0000 0000 0500 0000 0900 0000  ................
-000009b0: 0300 0000 73b2 0000 0067 007d 0274 007c  ....s....g.}.t.|
-000009c0: 006a 0183 017d 0374 02a0 0364 0164 0284  .j...}.t...d.d..
-000009d0: 007c 037c 006a 040b 0064 0385 0219 0044  .|.|.j...d.....D
-000009e0: 0083 01a1 0189 0087 0066 0164 0464 0284  .........f.d.d..
-000009f0: 0874 0588 006a 0664 0519 0083 0144 0083  .t...j.d.....D..
-00000a00: 017d 027c 006a 0764 066b 0572 9074 0574  .}.|.j.d.k.r.t.t
-00000a10: 087c 006a 096a 0a83 0183 0144 005d 2a7d  .|.j.j.....D.]*}
-00000a20: 047c 006a 0ba0 0c64 07a0 0d74 0ea0 0fa1  .|.j...d...t....
-00000a30: 007c 006a 096a 0a7c 0419 007c 027c 0419  .|.j.j.|...|.|..
-00000a40: 00a1 03a1 0101 0071 6474 02a0 107c 02a1  .......qdt...|..
-00000a50: 017c 005f 1174 127c 017c 006a 1114 0083  .|._.t.|.|.j....
-00000a60: 017c 005f 137c 006a 1353 0029 087a 960a  .|._.|.j.S.).z..
-00000a70: 2020 2020 2020 2020 4573 7469 6d61 7465          Estimate
-00000a80: 2061 7574 6f63 6f72 7265 6c61 7469 6f6e   autocorrelation
-00000a90: 206c 656e 6774 6820 6f66 2074 6865 2063   length of the c
-00000aa0: 6861 696e 0a20 2020 2020 2020 200a 2020  hain.        .  
-00000ab0: 2020 2020 2020 7361 6665 7479 2064 6574        safety det
-00000ac0: 6572 6d69 6e65 7320 7468 6520 6e75 6d62  ermines the numb
-00000ad0: 6572 206f 6620 4143 4c20 7468 6520 6368  er of ACL the ch
-00000ae0: 6169 6e73 2061 7265 2067 6f69 6e67 2074  ains are going t
-00000af0: 6f20 6265 2072 756e 2066 6f72 0a20 2020  o be run for.   
-00000b00: 2020 2020 2063 0100 0000 0000 0000 0000       c..........
-00000b10: 0000 0200 0000 0300 0000 5300 0000 7312  ..........S...s.
-00000b20: 0000 0067 007c 005d 0a7d 017c 016a 0091  ...g.|.].}.|.j..
-00000b30: 0271 0453 0072 2900 0000 2901 da06 7661  .q.S.r)...)...va
-00000b40: 6c75 6573 2902 da02 2e30 da01 7872 2900  lues)....0..xr).
-00000b50: 0000 7229 0000 0072 2a00 0000 da0a 3c6c  ..r)...r*.....<l
-00000b60: 6973 7463 6f6d 703e 7500 0000 f300 0000  istcomp>u.......
-00000b70: 007a 2853 616d 706c 6572 2e65 7374 696d  .z(Sampler.estim
-00000b80: 6174 655f 6163 6c2e 3c6c 6f63 616c 733e  ate_acl.<locals>
-00000b90: 2e3c 6c69 7374 636f 6d70 3e4e 6301 0000  .<listcomp>Nc...
-00000ba0: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00000bb0: 0013 0000 0073 2400 0000 6700 7c00 5d1c  .....s$...g.|.].
-00000bc0: 7d01 7400 8800 6400 6400 8502 7c01 6602  }.t...d.d...|.f.
-00000bd0: 1900 6401 6402 8d02 9102 7104 5300 2903  ..d.d.....q.S.).
-00000be0: 4e72 2c00 0000 2901 da01 6329 0172 0a00  Nr,...)...c).r..
-00000bf0: 0000 2902 7234 0000 00da 0169 a901 7227  ..).r4.....i..r'
-00000c00: 0000 0072 2900 0000 722a 0000 0072 3600  ...r)...r*...r6.
-00000c10: 0000 7700 0000 7237 0000 0072 0500 0000  ..w...r7...r....
-00000c20: 7211 0000 007a 1e53 616d 706c 6572 207b  r....z.Sampler {
-00000c30: 307d 202d 2d20 4143 4c28 7b31 7d29 2020  0} -- ACL({1})  
-00000c40: 3d20 7b32 7d29 14da 046c 6973 7472 2700  = {2})...listr'.
-00000c50: 0000 7214 0000 00da 0561 7272 6179 7226  ..r......arrayr&
-00000c60: 0000 00da 0572 616e 6765 da05 7368 6170  .....range..shap
-00000c70: 6572 2000 0000 da03 6c65 6e72 0f00 0000  er .....lenr....
-00000c80: da05 6e61 6d65 7372 1c00 0000 da04 696e  ..namesr......in
-00000c90: 666f da06 666f 726d 6174 da02 6f73 da06  fo..format..os..
-00000ca0: 6765 7470 6964 722f 0000 0072 1900 0000  getpidr/...r....
-00000cb0: 7230 0000 0072 1d00 0000 2905 7228 0000  r0...r....).r(..
-00000cc0: 0072 3100 0000 5a03 4143 4cda 0173 7239  .r1...Z.ACL..sr9
-00000cd0: 0000 0072 2900 0000 723a 0000 0072 2a00  ...r)...r:...r*.
-00000ce0: 0000 da0c 6573 7469 6d61 7465 5f61 636c  ....estimate_acl
-00000cf0: 6b00 0000 7314 0000 0000 0804 010a 0120  k...s.......... 
-00000d00: 021c 020a 0114 0128 030c 0210 017a 1453  .......(.....z.S
-00000d10: 616d 706c 6572 2e65 7374 696d 6174 655f  ampler.estimate_
-00000d20: 6163 6c63 0300 0000 0000 0000 0000 0000  aclc............
-00000d30: 0500 0000 0400 0000 4300 0000 7344 0000  ........C...sD..
-00000d40: 007c 00a0 007c 017c 02a1 025c 027d 037d  .|...|.|...\.}.}
-00000d50: 047c 0004 006a 0164 0137 0002 005f 017c  .|...j.d.7..._.|
-00000d60: 006a 0164 0216 0064 036b 0272 347c 00a0  .j.d...d.k.r4|..
-00000d70: 02a1 0001 007c 006a 037c 006a 047c 037c  .....|.j.|.j.|.|
-00000d80: 0466 0453 0029 047a b60a 2020 2020 2020  .f.S.).z..      
-00000d90: 2020 6d61 696e 206c 6f6f 7020 7468 6174    main loop that
-00000da0: 2074 616b 6573 2074 6865 2077 6f72 7374   takes the worst
-00000db0: 203a 6f62 6a3a 6072 6179 6e65 7374 2e70   :obj:`raynest.p
-00000dc0: 6172 616d 6574 6572 2e4c 6976 6550 6f69  arameter.LivePoi
-00000dd0: 6e74 6020 616e 640a 2020 2020 2020 2020  nt` and.        
-00000de0: 6576 6f6c 7665 7320 6974 2e20 5072 6f70  evolves it. Prop
-00000df0: 6f73 6564 2073 616d 706c 6520 6973 2074  osed sample is t
-00000e00: 6865 6e20 7365 6e74 2062 6163 6b0a 2020  hen sent back.  
-00000e10: 2020 2020 2020 746f 203a 6f62 6a3a 6072        to :obj:`r
-00000e20: 6179 6e65 7374 2e4e 6573 7465 6453 616d  aynest.NestedSam
-00000e30: 706c 6572 602e 0a20 2020 2020 2020 2072  pler`..        r
-00000e40: 0500 0000 720d 0000 0072 0100 0000 2905  ....r....r....).
-00000e50: da0d 7265 7475 726e 5f73 616d 706c 6572  ..return_sampler
-00000e60: 1300 0000 7246 0000 0072 2100 0000 7222  ....rF...r!...r"
-00000e70: 0000 0029 0572 2800 0000 da03 6f6c 64da  ...).r(.....old.
-00000e80: 076c 6f67 4c6d 696e 721d 0000 005a 086f  .logLminr....Z.o
-00000e90: 7574 5061 7261 6d72 2900 0000 7229 0000  utParamr)...r)..
-00000ea0: 0072 2a00 0000 da0e 7072 6f64 7563 655f  .r*.....produce_
-00000eb0: 7361 6d70 6c65 8300 0000 730a 0000 0000  sample....s.....
-00000ec0: 0610 030e 010e 0108 027a 1653 616d 706c  .........z.Sampl
-00000ed0: 6572 2e70 726f 6475 6365 5f73 616d 706c  er.produce_sampl
-00000ee0: 6563 0200 0000 0000 0000 0000 0000 0400  ec..............
-00000ef0: 0000 0600 0000 4300 0000 7356 0000 007c  ......C...sV...|
-00000f00: 006a 0064 016b 0472 207c 006a 01a0 0264  .j.d.k.r |.j...d
-00000f10: 02a0 0374 04a0 05a1 00a1 01a1 0101 0074  ...t...........t
-00000f20: 06a0 077c 01a1 0164 0319 007d 027c 006a  ...|...d...}.|.j
-00000f30: 086a 0944 005d 187d 0374 0a7c 0374 0b83  .j.D.].}.t.|.t..
-00000f40: 0272 367c 03a0 0c7c 02a1 0101 0071 367e  .r6|...|.....q6~
-00000f50: 0264 0353 0029 044e 7211 0000 007a 1f53  .d.S.).Nr....z.S
-00000f60: 616d 706c 6572 207b 307d 202d 2d20 7365  ampler {0} -- se
-00000f70: 7474 696e 6720 656e 7365 6d62 6c65 7201  tting ensembler.
-00000f80: 0000 0029 0d72 2000 0000 721c 0000 0072  ...).r ...r....r
-00000f90: 4100 0000 7242 0000 0072 4300 0000 7244  A...rB...rC...rD
-00000fa0: 0000 00da 0372 6179 da03 6765 7472 0900  .....ray..getr..
-00000fb0: 0000 da09 7072 6f70 6f73 616c 73da 0a69  ....proposals..i
-00000fc0: 7369 6e73 7461 6e63 6572 0800 0000 da0c  sinstancer......
-00000fd0: 7365 745f 656e 7365 6d62 6c65 2904 7228  set_ensemble).r(
-00000fe0: 0000 00da 0c65 6e73 656d 626c 655f 7265  .....ensemble_re
-00000ff0: 66da 0865 6e73 656d 626c 65da 0170 7229  f..ensemble..pr)
-00001000: 0000 0072 2900 0000 722a 0000 0072 4f00  ...r)...r*...rO.
-00001010: 0000 9200 0000 7310 0000 0000 010a 0116  ......s.........
-00001020: 020e 010c 010a 010c 0102 027a 1453 616d  ...........z.Sam
-00001030: 706c 6572 2e73 6574 5f65 6e73 656d 626c  pler.set_ensembl
-00001040: 6529 034e 7201 0000 004e 2902 722c 0000  e).Nr....N).r,..
-00001050: 004e 2901 7205 0000 0029 09da 085f 5f6e  .N).r....)...__n
-00001060: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00001070: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
-00001080: 075f 5f64 6f63 5f5f 722b 0000 0072 3200  .__doc__r+...r2.
-00001090: 0000 7246 0000 0072 4a00 0000 724f 0000  ..rF...rJ...rO..
-000010a0: 0072 2900 0000 7229 0000 0072 2900 0000  .r)...r)...r)...
-000010b0: 722a 0000 0072 0c00 0000 1600 0000 7312  r*...r........s.
-000010c0: 0000 0008 0104 1b00 0100 0100 fb0a 230a  ..............#.
-000010d0: 190a 1808 0f72 0c00 0000 6300 0000 0000  .....r....c.....
-000010e0: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
-000010f0: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00001100: 6401 5a03 6402 6403 8400 5a04 6404 5300  d.Z.d.d...Z.d.S.
-00001110: 2905 da19 4d65 7472 6f70 6f6c 6973 4861  )...MetropolisHa
-00001120: 7374 696e 6773 5361 6d70 6c65 727a 5e0a  stingsSamplerz^.
-00001130: 2020 2020 6d65 7472 6f70 6f6c 6973 2d68      metropolis-h
-00001140: 6173 7469 6e67 7320 6163 6365 7074 616e  astings acceptan
-00001150: 6365 2072 756c 650a 2020 2020 666f 7220  ce rule.    for 
-00001160: 3a6f 626a 3a60 7261 796e 6573 742e 7072  :obj:`raynest.pr
-00001170: 6f70 6f73 616c 2e45 6e73 656d 626c 6550  oposal.EnsembleP
-00001180: 726f 706f 7361 6c60 0a20 2020 2063 0300  roposal`.    c..
-00001190: 0000 0000 0000 0000 0000 0700 0000 0500  ................
-000011a0: 0000 4300 0000 7302 0100 0064 017d 0364  ..C...s....d.}.d
-000011b0: 017d 047c 006a 00a0 017c 01a1 017d 057c  .}.|.j...|...}.|
-000011c0: 0364 0237 007d 037c 006a 02a0 037c 01a0  .d.7.}.|.j...|..
-000011d0: 04a1 00a1 017d 067c 006a 00a0 017c 06a1  .....}.|.j...|..
-000011e0: 017c 065f 057c 066a 057c 0518 007c 006a  .|._.|.j.|...|.j
-000011f0: 026a 0617 0074 07a0 087c 006a 09a0 0aa1  .j...t...|.j....
-00001200: 00a1 016b 0472 8a7c 006a 00a0 0b7c 06a1  ...k.r.|.j...|..
-00001210: 017c 065f 0c7c 066a 0c7c 026b 0472 8a7c  .|._.|.j.|.k.r.|
-00001220: 06a0 04a1 007d 017c 066a 057d 057c 0464  .....}.|.j.}.|.d
-00001230: 0237 007d 047c 006a 0da0 0e7c 01a1 0101  .7.}.|.j...|....
-00001240: 007c 037c 006a 0f6b 0572 a87c 0464 016b  .|.|.j.k.r.|.d.k
-00001250: 0473 b67c 037c 006a 106b 0572 1471 b671  .s.|.|.j.k.r.q.q
-00001260: 1474 117c 0483 0174 117c 0383 011b 007c  .t.|...t.|.....|
-00001270: 005f 127c 0004 006a 137c 0437 0002 005f  ._.|...j.|.7..._
-00001280: 137c 0004 006a 147c 0337 0002 005f 1474  .|...j.|.7..._.t
-00001290: 117c 006a 1383 0174 117c 006a 1483 011b  .|.j...t.|.j....
-000012a0: 007c 005f 157c 037c 0166 0253 0029 034e  .|._.|.|.f.S.).N
-000012b0: 7201 0000 0072 0500 0000 2916 720f 0000  r....r....).r...
-000012c0: 00da 096c 6f67 5f70 7269 6f72 7209 0000  ...log_priorr...
-000012d0: 00da 0a67 6574 5f73 616d 706c 65da 0463  ...get_sample..c
-000012e0: 6f70 79da 046c 6f67 50da 056c 6f67 5f4a  opy..logP..log_J
-000012f0: 7214 0000 0072 0300 0000 7217 0000 0072  r....r....r....r
-00001300: 1500 0000 da0e 6c6f 675f 6c69 6b65 6c69  ......log_likeli
-00001310: 686f 6f64 da04 6c6f 674c 7227 0000 00da  hood..logLr'....
-00001320: 0661 7070 656e 6472 1d00 0000 7218 0000  .appendr....r...
-00001330: 0072 1e00 0000 7222 0000 0072 2300 0000  .r....r"...r#...
-00001340: 7224 0000 0072 2100 0000 2907 7228 0000  r$...r!...).r(..
-00001350: 00da 086f 6c64 7061 7261 6d72 4900 0000  ...oldparamrI...
-00001360: da0b 7375 625f 636f 756e 7465 72da 0c73  ..sub_counter..s
-00001370: 7562 5f61 6363 6570 7465 645a 086c 6f67  ub_acceptedZ.log
-00001380: 705f 6f6c 64da 086e 6577 7061 7261 6d72  p_old..newparamr
-00001390: 2900 0000 7229 0000 0072 2a00 0000 7247  )...r)...r*...rG
-000013a0: 0000 00a4 0000 0073 2800 0000 0002 0401  .......s(.......
-000013b0: 0401 0c04 0801 1001 0e02 2202 0e02 0a02  ..........".....
-000013c0: 0801 0601 0803 0c02 1c01 0402 1201 0e01  ................
-000013d0: 0e01 1602 7a27 4d65 7472 6f70 6f6c 6973  ....z'Metropolis
-000013e0: 4861 7374 696e 6773 5361 6d70 6c65 722e  HastingsSampler.
-000013f0: 7265 7475 726e 5f73 616d 706c 654e 2905  return_sampleN).
-00001400: 7253 0000 0072 5400 0000 7255 0000 0072  rS...rT...rU...r
-00001410: 5600 0000 7247 0000 0072 2900 0000 7229  V...rG...r)...r)
-00001420: 0000 0072 2900 0000 722a 0000 0072 5700  ...r)...r*...rW.
-00001430: 0000 9e00 0000 7304 0000 0008 0204 0472  ......s........r
-00001440: 5700 0000 2901 da06 4144 5047 4d4d 6300  W...)...ADPGMMc.
-00001450: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-00001460: 0000 0040 0000 0073 2800 0000 6500 5a01  ...@...s(...e.Z.
-00001470: 6400 5a02 6401 5a03 6402 5a04 6403 5a05  d.Z.d.Z.d.Z.d.Z.
-00001480: 6404 6405 8400 5a06 6406 6407 8400 5a07  d.d...Z.d.d...Z.
-00001490: 6403 5300 2908 da1c 4861 6d69 6c74 6f6e  d.S.)...Hamilton
-000014a0: 6961 6e4d 6f6e 7465 4361 726c 6f53 616d  ianMonteCarloSam
-000014b0: 706c 6572 7a63 0a20 2020 2048 616d 696c  plerzc.    Hamil
-000014c0: 746f 6e69 616e 4d6f 6e74 6543 6172 6c6f  tonianMonteCarlo
-000014d0: 2061 6363 6570 7461 6e63 6520 7275 6c65   acceptance rule
-000014e0: 0a20 2020 2066 6f72 203a 6f62 6a3a 6072  .    for :obj:`r
-000014f0: 6179 6e65 7374 2e70 726f 706f 7361 6c2e  aynest.proposal.
-00001500: 4861 6d69 6c74 6f6e 6961 6e50 726f 706f  HamiltonianPropo
-00001510: 7361 6c60 0a20 2020 2046 4e63 0200 0000  sal`.    FNc....
-00001520: 0000 0000 0000 0000 0500 0000 0400 0000  ................
-00001530: 4300 0000 7360 0000 0074 00a0 017c 01a1  C...s`...t...|..
-00001540: 0164 0119 007d 027c 02a0 02a1 0001 007c  .d...}.|.......|
-00001550: 02a0 03a1 007d 0374 047c 006a 056a 0664  .....}.t.|.j.j.d
-00001560: 0264 038d 027c 005f 077c 026a 0844 005d  .d...|._.|.j.D.]
-00001570: 127d 047c 006a 07a0 097c 046a 0aa1 0101  .}.|.j...|.j....
-00001580: 0071 367c 006a 0ba0 0c7c 006a 077c 0366  .q6|.j...|.j.|.f
-00001590: 02a1 0101 0064 0153 0029 044e 7201 0000  .....d.S.).Nr...
-000015a0: 0046 2901 5a06 7072 6f62 6974 290d 724b  .F).Z.probit).rK
-000015b0: 0000 0072 4c00 0000 5a16 7570 6461 7465  ...rL...Z.update
-000015c0: 5f6d 6561 6e5f 636f 7661 7269 616e 6365  _mean_covariance
-000015d0: 5a0e 6765 745f 636f 7661 7269 616e 6365  Z.get_covariance
-000015e0: 7264 0000 0072 0f00 0000 da06 626f 756e  rd...r......boun
-000015f0: 6473 da07 6465 6e73 6974 795a 055f 6c69  ds..densityZ._li
-00001600: 7374 da0d 6164 645f 6e65 775f 706f 696e  st..add_new_poin
-00001610: 7472 3300 0000 7209 0000 0072 4f00 0000  tr3...r....rO...
-00001620: 2905 7228 0000 0072 5000 0000 7251 0000  ).r(...rP...rQ..
-00001630: 00da 0a63 6f76 6172 6961 6e63 65da 0165  ...covariance..e
-00001640: 7229 0000 0072 2900 0000 722a 0000 0072  r)...r)...r*...r
-00001650: 4f00 0000 d200 0000 7310 0000 0000 020e  O.......s.......
-00001660: 0208 0108 0212 010a 0110 0212 017a 2948  .............z)H
-00001670: 616d 696c 746f 6e69 616e 4d6f 6e74 6543  amiltonianMonteC
-00001680: 6172 6c6f 5361 6d70 6c65 722e 7365 745f  arloSampler.set_
-00001690: 656e 7365 6d62 6c65 6303 0000 0000 0000  ensemblec.......
-000016a0: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
-000016b0: 0073 d200 0000 6401 7d03 6401 7d04 7c04  .s....d.}.d.}.|.
-000016c0: 6402 3700 7d04 7c00 6a00 6a01 7c01 a002  d.7.}.|.j.j.|...
-000016d0: a100 7c02 6403 8d02 7d05 7c00 6a00 6a03  ..|.d...}.|.j.j.
-000016e0: 7404 a005 7c00 6a06 a007 a100 a101 6b04  t...|.j.......k.
-000016f0: 7256 7c05 6a08 7c02 6b04 7256 7c05 a002  rV|.j.|.k.rV|...
-00001700: a100 7d01 7c03 6402 3700 7d03 7c00 6a09  ..}.|.d.7.}.|.j.
-00001710: a00a 7c01 a101 0100 7c04 7c00 6a0b 6b05  ..|.....|.|.j.k.
-00001720: 7208 7c03 6401 6b04 7208 7178 7108 740c  r.|.d.k.r.qxq.t.
-00001730: 7c03 8301 740c 7c04 8301 1b00 7c00 5f0d  |...t.|.....|._.
-00001740: 7c00 0400 6a0e 7c03 3700 0200 5f0e 7c00  |...j.|.7..._.|.
-00001750: 0400 6a0f 7c04 3700 0200 5f0f 740c 7c00  ..j.|.7..._.t.|.
-00001760: 6a0e 8301 740c 7c00 6a0f 8301 1b00 7c00  j...t.|.j.....|.
-00001770: 5f10 7c00 6a11 a012 7c01 6a13 a101 0100  _.|.j...|.j.....
-00001780: 7c04 7c01 6602 5300 2904 4e72 0100 0000  |.|.f.S.).Nr....
-00001790: 7205 0000 0029 0172 4900 0000 2914 7209  r....).rI...).r.
-000017a0: 0000 0072 5900 0000 725a 0000 0072 5c00  ...rY...rZ...r\.
-000017b0: 0000 7214 0000 0072 0300 0000 7217 0000  ..r....r....r...
-000017c0: 0072 1500 0000 725e 0000 0072 2700 0000  .r....r^...r'...
-000017d0: 725f 0000 0072 1d00 0000 721e 0000 0072  r_...r....r....r
-000017e0: 2200 0000 7223 0000 0072 2400 0000 7221  "...r#...r$...r!
-000017f0: 0000 0072 6700 0000 7268 0000 0072 3300  ...rg...rh...r3.
-00001800: 0000 2906 7228 0000 0072 6000 0000 7249  ..).r(...r`...rI
-00001810: 0000 0072 6200 0000 7261 0000 0072 6300  ...rb...ra...rc.
-00001820: 0000 7229 0000 0072 2900 0000 722a 0000  ..r)...r)...r*..
-00001830: 0072 4700 0000 e000 0000 7322 0000 0000  .rG.......s"....
-00001840: 0204 0104 0408 0114 0218 020a 0108 0108  ................
-00001850: 030c 0212 0104 0512 010e 010e 0116 020e  ................
-00001860: 027a 2a48 616d 696c 746f 6e69 616e 4d6f  .z*HamiltonianMo
-00001870: 6e74 6543 6172 6c6f 5361 6d70 6c65 722e  nteCarloSampler.
-00001880: 7265 7475 726e 5f73 616d 706c 6529 0872  return_sample).r
-00001890: 5300 0000 7254 0000 0072 5500 0000 7256  S...rT...rU...rV
-000018a0: 0000 0072 2500 0000 7267 0000 0072 4f00  ...r%...rg...rO.
-000018b0: 0000 7247 0000 0072 2900 0000 7229 0000  ..rG...r)...r)..
-000018c0: 0072 2900 0000 722a 0000 0072 6500 0000  .r)...r*...re...
-000018d0: c900 0000 730a 0000 0008 0204 0404 0104  ....s...........
-000018e0: 0208 0e72 6500 0000 6300 0000 0000 0000  ...re...c.......
-000018f0: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
-00001900: 0073 4400 0000 6500 5a01 6400 5a02 6401  .sD...e.Z.d.Z.d.
-00001910: 5a03 6402 5a04 6403 5a05 6403 5a06 6404  Z.d.Z.d.Z.d.Z.d.
-00001920: 6405 8400 5a07 6406 6407 8400 5a08 6408  d...Z.d.d...Z.d.
-00001930: 6409 8400 5a09 640a 640b 8400 5a0a 640c  d...Z.d.d...Z.d.
-00001940: 640d 8400 5a0b 640e 5300 290f da0c 536c  d...Z.d.S.)...Sl
-00001950: 6963 6553 616d 706c 6572 7a68 0a20 2020  iceSamplerzh.   
-00001960: 2054 6865 2045 6e73 656d 626c 6520 536c   The Ensemble Sl
-00001970: 6963 6520 7361 6d70 6c65 7220 6672 6f6d  ice sampler from
-00001980: 204b 6172 616d 616e 6973 2026 2042 6575   Karamanis & Beu
-00001990: 746c 6572 0a20 2020 2068 7474 7073 3a2f  tler.    https:/
-000019a0: 2f61 7278 6976 2e6f 7267 2f70 6466 2f32  /arxiv.org/pdf/2
-000019b0: 3030 322e 3036 3231 3276 312e 7064 660a  002.06212v1.pdf.
-000019c0: 2020 2020 722d 0000 0069 e803 0000 6301      r-...i....c.
-000019d0: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-000019e0: 0000 0043 0000 0073 3a00 0000 7400 6401  ...C...s:...t.d.
-000019f0: 7c00 6a01 8302 7d01 7400 6401 7c00 6a02  |.j...}.t.d.|.j.
-00001a00: 8302 7d02 7c01 7c01 7c02 1700 1b00 7d03  ..}.|.|.|.....}.
-00001a10: 7c00 0400 6a03 6402 7c03 1400 3900 0200  |...j.d.|...9...
-00001a20: 5f03 6403 5300 2904 7a97 0a20 2020 2020  _.d.S.).z..     
-00001a30: 2020 2061 6461 7074 7320 7468 6520 6c65     adapts the le
-00001a40: 6e67 7468 2073 6361 6c65 206f 6620 7468  ngth scale of th
-00001a50: 6520 6578 7061 6e73 696f 6e2f 636f 6e74  e expansion/cont
-00001a60: 7261 6374 696f 6e0a 2020 2020 2020 2020  raction.        
-00001a70: 666f 6c6c 6f77 696e 6720 7468 6520 7275  following the ru
-00001a80: 6c65 2069 6e20 2852 6f62 6269 6e73 2061  le in (Robbins a
-00001a90: 6e64 204d 6f6e 726f 2c20 3139 3531 2920  nd Monro, 1951) 
-00001aa0: 6f66 2054 6962 6269 7473 2065 7420 616c  of Tibbits et al
-00001ab0: 2e20 2832 3031 3429 0a20 2020 2020 2020  . (2014).       
-00001ac0: 2072 0500 0000 e902 0000 004e 2904 722f   r.........N).r/
-00001ad0: 0000 00da 024e 65da 024e 63da 026d 7529  .....Ne..Nc..mu)
-00001ae0: 0472 2800 0000 726d 0000 0072 6e00 0000  .r(...rm...rn...
-00001af0: da05 7261 7469 6f72 2900 0000 7229 0000  ..ratior)...r)..
-00001b00: 0072 2a00 0000 da12 6164 6170 745f 6c65  .r*.....adapt_le
-00001b10: 6e67 7468 5f73 6361 6c65 0c01 0000 7308  ngth_scale....s.
-00001b20: 0000 0000 050c 010c 010c 017a 1f53 6c69  ...........z.Sli
-00001b30: 6365 5361 6d70 6c65 722e 6164 6170 745f  ceSampler.adapt_
-00001b40: 6c65 6e67 7468 5f73 6361 6c65 6301 0000  length_scalec...
-00001b50: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00001b60: 0043 0000 0073 2a00 0000 7c00 6a00 a001  .C...s*...|.j...
-00001b70: a100 0b00 7c00 5f02 7c00 6a02 6401 1700  ....|._.|.j.d...
-00001b80: 7c00 5f03 6402 7c00 5f04 6402 7c00 5f05  |._.d.|._.d.|._.
-00001b90: 6403 5300 2904 7a4a 0a20 2020 2020 2020  d.S.).zJ.       
-00001ba0: 2072 6573 6574 7320 7468 6520 626f 756e   resets the boun
-00001bb0: 6461 7269 6573 2061 6e64 2063 6f75 6e74  daries and count
-00001bc0: 730a 2020 2020 2020 2020 666f 7220 7468  s.        for th
-00001bd0: 6520 736c 6963 696e 670a 2020 2020 2020  e slicing.      
-00001be0: 2020 722d 0000 0072 1000 0000 4e29 0672    r-...r....N).r
-00001bf0: 1700 0000 7215 0000 00da 014c da01 5272  ....r......L..Rr
-00001c00: 6d00 0000 726e 0000 00a9 0172 2800 0000  m...rn.....r(...
-00001c10: 7229 0000 0072 2900 0000 722a 0000 00da  r)...r)...r*....
-00001c20: 1072 6573 6574 5f62 6f75 6e64 6172 6965  .reset_boundarie
-00001c30: 7316 0100 0073 0800 0000 0005 0e01 0c01  s....s..........
-00001c40: 0601 7a1d 536c 6963 6553 616d 706c 6572  ..z.SliceSampler
-00001c50: 2e72 6573 6574 5f62 6f75 6e64 6172 6965  .reset_boundarie
-00001c60: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
-00001c70: 0000 0200 0000 4300 0000 731c 0000 007c  ......C...s....|
-00001c80: 006a 0064 0118 007c 005f 007c 006a 0164  .j.d...|._.|.j.d
-00001c90: 0217 007c 005f 0164 0353 0029 047a 4b0a  ...|._.d.S.).zK.
-00001ca0: 2020 2020 2020 2020 696e 6372 6561 7365          increase
-00001cb0: 2074 6865 206c 6566 7420 626f 756e 6461   the left bounda
-00001cc0: 7279 2061 6e64 2063 6f75 6e74 730a 2020  ry and counts.  
-00001cd0: 2020 2020 2020 6279 206f 6e65 2075 6e69        by one uni
-00001ce0: 740a 2020 2020 2020 2020 722d 0000 0072  t.        r-...r
-00001cf0: 0500 0000 4e29 0272 7200 0000 726d 0000  ....N).rr...rm..
-00001d00: 0072 7400 0000 7229 0000 0072 2900 0000  .rt...r)...r)...
-00001d10: 722a 0000 00da 1669 6e63 7265 6173 655f  r*.....increase_
-00001d20: 6c65 6674 5f62 6f75 6e64 6172 7920 0100  left_boundary ..
-00001d30: 0073 0400 0000 0005 0c01 7a23 536c 6963  .s........z#Slic
-00001d40: 6553 616d 706c 6572 2e69 6e63 7265 6173  eSampler.increas
-00001d50: 655f 6c65 6674 5f62 6f75 6e64 6172 7963  e_left_boundaryc
-00001d60: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00001d70: 0200 0000 4300 0000 731c 0000 007c 006a  ....C...s....|.j
-00001d80: 0064 0117 007c 005f 007c 006a 0164 0217  .d...|._.|.j.d..
-00001d90: 007c 005f 0164 0353 0029 047a 4c0a 2020  .|._.d.S.).zL.  
-00001da0: 2020 2020 2020 696e 6372 6561 7365 2074        increase t
-00001db0: 6865 2072 6967 6874 2062 6f75 6e64 6172  he right boundar
-00001dc0: 7920 616e 6420 636f 756e 7473 0a20 2020  y and counts.   
-00001dd0: 2020 2020 2062 7920 6f6e 6520 756e 6974       by one unit
-00001de0: 0a20 2020 2020 2020 2072 2d00 0000 7205  .        r-...r.
-00001df0: 0000 004e 2902 7273 0000 0072 6d00 0000  ...N).rs...rm...
-00001e00: 7274 0000 0072 2900 0000 7229 0000 0072  rt...r)...r)...r
-00001e10: 2a00 0000 da17 696e 6372 6561 7365 5f72  *.....increase_r
-00001e20: 6967 6874 5f62 6f75 6e64 6172 7928 0100  ight_boundary(..
-00001e30: 0073 0400 0000 0005 0c01 7a24 536c 6963  .s........z$Slic
-00001e40: 6553 616d 706c 6572 2e69 6e63 7265 6173  eSampler.increas
-00001e50: 655f 7269 6768 745f 626f 756e 6461 7279  e_right_boundary
-00001e60: 6303 0000 0000 0000 0000 0000 000f 0000  c...............
-00001e70: 0005 0000 0043 0000 0073 7402 0000 6401  .....C...st...d.
-00001e80: 7d03 6401 7d04 7c00 a000 a100 0100 7c04  }.d.}.|.......|.
-00001e90: 6402 3700 7d04 7c00 6a01 6a02 7c00 6a03  d.7.}.|.j.j.|.j.
-00001ea0: 6403 8d01 7d05 7404 7c05 7405 6a06 8302  d...}.t.|.t.j...
-00001eb0: 7344 7405 6a06 7c01 6a07 7c05 6404 8d02  sDt.j.|.j.|.d...
-00001ec0: 7d05 7c02 7d06 7c01 6a08 7c00 6a09 a00a  }.|.}.|.j.|.j...
-00001ed0: a100 1800 7d07 740b a00c 7c00 6a0d 7c00  ....}.t...|.j.|.
-00001ee0: 6a09 a00e a100 1400 a101 7d08 7c00 6a0d  j.........}.|.j.
-00001ef0: 6402 1800 7c08 1800 7d09 7c08 6401 6b04  d...|...}.|.d.k.
-00001f00: 72c8 7c05 7c00 6a0f 1400 7c01 1700 7d0a  r.|.|.j...|...}.
-00001f10: 7c00 6a10 a011 7c0a a101 72c8 7c07 7c00  |.j...|...r.|.|.
-00001f20: 6a10 a012 7c0a a101 6b04 72b2 71c8 71c6  j...|...k.r.q.q.
-00001f30: 7c00 a013 a100 0100 7c08 6402 3800 7d08  |.......|.d.8.}.
-00001f40: 717c 71c8 717c 7c09 6401 6b04 9001 721e  q|q.q||.d.k...r.
-00001f50: 7c05 7c00 6a14 1400 7c01 1700 7d0b 7c00  |.|.j...|...}.|.
-00001f60: 6a10 a011 7c0b a101 9001 721e 7c07 7c00  j...|.....r.|.|.
-00001f70: 6a10 a012 7c0b a101 6b04 9001 7206 9001  j...|...k...r...
-00001f80: 711e 6e10 7c00 a015 a100 0100 7c09 6402  q.n.|.......|.d.
-00001f90: 3800 7d09 71c8 9001 711e 71c8 6401 7d0c  8.}.q...q.q.d.}.
-00001fa0: 7c0c 7c00 6a16 6b00 9001 72da 7c00 6a09  |.|.j.k...r.|.j.
-00001fb0: a017 7c00 6a0f 7c00 6a14 a102 7d0d 7c05  ..|.j.|.j...}.|.
-00001fc0: 7c0d 1400 7c01 1700 7d0e 7c00 6a10 a012  |...|...}.|.j...
-00001fd0: 7c0e a101 7c0e 5f08 7c0e 6a08 7c07 6b04  |...|._.|.j.|.k.
-00001fe0: 9001 7294 7c00 6a10 a018 7c0e a101 7c0e  ..r.|.j...|...|.
-00001ff0: 5f19 7c0e 6a19 7c06 6b04 9001 7294 7c0e  _.|.j.|.k...r.|.
-00002000: a01a a100 7d01 7c03 6402 3700 7d03 9001  ....}.|.d.7.}...
-00002010: 71da 7c0d 6405 6b00 9001 72b2 7c0d 7c00  q.|.d.k...r.|.|.
-00002020: 5f0f 7c00 6a1b 6402 1700 7c00 5f1b 6e1c  _.|.j.d...|._.n.
-00002030: 7c0d 6405 6b04 9001 72ce 7c0d 7c00 5f14  |.d.k...r.|.|._.
-00002040: 7c00 6a1b 6402 1700 7c00 5f1b 7c0c 6402  |.j.d...|._.|.d.
-00002050: 3700 7d0c 9001 7122 7c04 7c00 6a1c 6b05  7.}...q"|.|.j.k.
-00002060: 9001 72f4 7c03 6401 6b04 9001 72f4 9002  ..r.|.d.k...r...
-00002070: 7112 7c04 7c00 6a1d 6b05 9002 7204 9002  q.|.|.j.k...r...
-00002080: 7112 7c00 6a1e a01f 7c01 a101 0100 7108  q.|.j...|.....q.
-00002090: 7420 7c03 8301 7420 7c04 8301 1b00 7c00  t |...t |.....|.
-000020a0: 5f21 7c00 0400 6a22 7c03 3700 0200 5f22  _!|...j"|.7..._"
-000020b0: 7c00 0400 6a23 7c04 3700 0200 5f23 7420  |...j#|.7..._#t 
-000020c0: 7c00 6a22 8301 7420 7c00 6a23 8301 1b00  |.j"..t |.j#....
-000020d0: 7c00 5f24 7c02 740b 6a25 0b00 6b02 9002  |._$|.t.j%..k...
-000020e0: 726c 7c00 a026 a100 0100 7c04 7c01 6602  rl|..&....|.|.f.
-000020f0: 5300 2906 4e72 0100 0000 7205 0000 0029  S.).Nr....r....)
-00002100: 0172 6f00 0000 2901 da01 6472 1000 0000  .ro...)...dr....
-00002110: 2927 7275 0000 0072 0900 0000 5a0d 6765  )'ru...r....Z.ge
-00002120: 745f 6469 7265 6374 696f 6e72 6f00 0000  t_directionro...
-00002130: 724e 0000 0072 0600 0000 da09 4c69 7665  rN...r......Live
-00002140: 506f 696e 7472 4000 0000 725b 0000 0072  Pointr@...r[...r
-00002150: 1700 0000 da0b 6578 706f 6e65 6e74 6961  ......exponentia
-00002160: 6c72 1400 0000 da05 666c 6f6f 72da 0d6d  lr......floor..m
-00002170: 6178 5f73 7465 7073 5f6f 7574 7215 0000  ax_steps_outr...
-00002180: 0072 7200 0000 720f 0000 00da 0969 6e5f  .rr...r......in_
-00002190: 626f 756e 6473 7258 0000 0072 7600 0000  boundsrX...rv...
-000021a0: 7273 0000 0072 7700 0000 da0a 6d61 785f  rs...rw.....max_
-000021b0: 736c 6963 6573 da07 756e 6966 6f72 6d72  slices..uniformr
-000021c0: 5d00 0000 725e 0000 0072 5a00 0000 726e  ]...r^...rZ...rn
-000021d0: 0000 0072 1d00 0000 7218 0000 0072 2700  ...r....r....r'.
-000021e0: 0000 725f 0000 0072 1e00 0000 7222 0000  ..r_...r....r"..
-000021f0: 0072 2300 0000 7224 0000 0072 2100 0000  .r#...r$...r!...
-00002200: da03 696e 6672 7100 0000 290f 7228 0000  ..infrq...).r(..
-00002210: 0072 6000 0000 7249 0000 0072 6200 0000  .r`...rI...rb...
-00002220: 7261 0000 005a 1064 6972 6563 7469 6f6e  ra...Z.direction
-00002230: 5f76 6563 746f 72da 0159 5a02 5970 da01  _vector..YZ.Yp..
-00002240: 4ada 014b 5a0e 7061 7261 6d65 7465 725f  J..KZ.parameter_
-00002250: 6c65 6674 5a0f 7061 7261 6d65 7465 725f  leftZ.parameter_
-00002260: 7269 6768 74da 0573 6c69 6365 5a06 5870  right..sliceZ.Xp
-00002270: 7269 6d65 7263 0000 0072 2900 0000 7229  rimerc...r)...r)
-00002280: 0000 0072 2a00 0000 7247 0000 0030 0100  ...r*...rG...0..
-00002290: 0073 7200 0000 0002 0401 0404 0801 0802  .sr.............
-000022a0: 1001 0c01 1002 0401 1001 1601 0e03 0802  ................
-000022b0: 0e02 0c01 1001 0402 0801 0a03 0404 0a02  ................
-000022c0: 0e02 0e02 1201 0602 0801 0a03 0603 0401  ................
-000022d0: 0c02 1201 0c01 0e02 0c02 0e01 0c01 0801  ................
-000022e0: 0801 0402 0a01 0601 0e01 0a01 0601 0c02  ................
-000022f0: 0c02 1601 0402 0c01 0402 0e01 1201 0e01  ................
-00002300: 0e01 1602 0e01 0802 7a1a 536c 6963 6553  ........z.SliceS
-00002310: 616d 706c 6572 2e72 6574 7572 6e5f 7361  ampler.return_sa
-00002320: 6d70 6c65 4e29 0c72 5300 0000 7254 0000  mpleN).rS...rT..
-00002330: 0072 5500 0000 7256 0000 0072 6f00 0000  .rU...rV...ro...
-00002340: 727c 0000 0072 7e00 0000 7271 0000 0072  r|...r~...rq...r
-00002350: 7500 0000 7276 0000 0072 7700 0000 7247  u...rv...rw...rG
-00002360: 0000 0072 2900 0000 7229 0000 0072 2900  ...r)...r)...r).
-00002370: 0000 722a 0000 0072 6b00 0000 0201 0000  ..r*...rk.......
-00002380: 7312 0000 0008 0204 0404 0104 0104 0208  s...............
-00002390: 0a08 0a08 0808 0872 6b00 0000 6300 0000  .......rk...c...
-000023a0: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-000023b0: 0040 0000 0073 3000 0000 6500 5a01 6400  .@...s0...e.Z.d.
-000023c0: 5a02 6401 5a03 6402 5a04 6402 5a05 6403  Z.d.Z.d.Z.d.Z.d.
-000023d0: 6404 8400 5a06 6405 6406 8400 5a07 6407  d...Z.d.d...Z.d.
-000023e0: 6408 8400 5a08 6409 5300 290a da0d 5361  d...Z.d.S.)...Sa
-000023f0: 6d70 6c65 7273 4379 636c 657a d70a 2020  mplersCyclez..  
-00002400: 2020 4120 7361 6d70 6c65 7220 7468 6174    A sampler that
-00002410: 2063 7963 6c65 7320 7468 726f 7567 6820   cycles through 
-00002420: 6120 6c69 7374 206f 660a 2020 2020 7361  a list of.    sa
-00002430: 6d70 6c65 7273 2e0a 0a20 2020 2049 6e69  mplers...    Ini
-00002440: 7469 616c 6973 6174 696f 6e20 6172 6775  tialisation argu
-00002450: 6d65 6e74 733a 0a0a 2020 2020 7361 6d70  ments:..    samp
-00002460: 6c65 7273 203a 2041 206c 6973 7420 6f66  lers : A list of
-00002470: 2073 616d 706c 6572 730a 0a20 2020 204f   samplers..    O
-00002480: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
-00002490: 733a 0a20 2020 2063 7963 6c65 6c65 6e67  s:.    cycleleng
-000024a0: 7468 203a 206c 656e 6774 6820 6f66 2074  th : length of t
-000024b0: 6865 2073 616d 706c 6572 2063 7963 6c65  he sampler cycle
-000024c0: 2e20 4465 6661 756c 743a 2031 3030 0a0a  . Default: 100..
-000024d0: 2020 2020 7201 0000 0063 0200 0000 0000      r....c......
-000024e0: 0000 0000 0000 0400 0000 0200 0000 4f00  ..............O.
-000024f0: 0000 7316 0000 007c 017c 005f 0074 017c  ..s....|.|._.t.|
-00002500: 006a 0083 017c 005f 0264 0053 0029 014e  .j...|._.d.S.).N
-00002510: 2903 da08 7361 6d70 6c65 7273 723f 0000  )...samplersr?..
-00002520: 00da 014e 2904 7228 0000 0072 8600 0000  ...N).r(...r....
-00002530: da04 6172 6773 da06 6b77 6172 6773 7229  ..args..kwargsr)
-00002540: 0000 0072 2900 0000 722a 0000 0072 2b00  ...r)...r*...r+.
-00002550: 0000 9d01 0000 7304 0000 0000 0106 017a  ......s........z
-00002560: 1653 616d 706c 6572 7343 7963 6c65 2e5f  .SamplersCycle._
-00002570: 5f69 6e69 745f 5f63 0300 0000 0000 0000  _init__c........
-00002580: 0000 0000 0900 0000 0400 0000 4b00 0000  ............K...
-00002590: 7346 0000 007c 006a 0064 0117 007c 006a  sF...|.j.d...|.j
-000025a0: 0116 007c 005f 007c 006a 027c 006a 0019  ...|._.|.j.|.j..
-000025b0: 007d 047c 046a 037c 017c 0266 0269 007c  .}.|.j.|.|.f.i.|
-000025c0: 03a4 018e 015c 047d 057d 067d 077d 087c  .....\.}.}.}.}.|
-000025d0: 057c 067c 077c 0866 0453 0029 024e 7205  .|.|.|.f.S.).Nr.
-000025e0: 0000 0029 04da 0369 6478 7287 0000 0072  ...)...idxr....r
-000025f0: 8600 0000 724a 0000 0029 0972 2800 0000  ....rJ...).r(...
-00002600: 7248 0000 0072 4900 0000 7289 0000 0072  rH...rI...r....r
-00002610: 5200 0000 7221 0000 0072 2200 0000 721d  R...r!...r"...r.
-00002620: 0000 00da 036e 6577 7229 0000 0072 2900  .....newr)...r).
-00002630: 0000 722a 0000 0072 4a00 0000 a101 0000  ..r*...rJ.......
-00002640: 7308 0000 0000 0212 010c 011c 017a 1c53  s............z.S
-00002650: 616d 706c 6572 7343 7963 6c65 2e70 726f  amplersCycle.pro
-00002660: 6475 6365 5f73 616d 706c 6563 0200 0000  duce_samplec....
-00002670: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00002680: 4300 0000 7332 0000 007c 006a 0044 005d  C...s2...|.j.D.]
-00002690: 267d 027c 026a 016a 0244 005d 187d 0374  &}.|.j.j.D.].}.t
-000026a0: 037c 0374 0483 0272 127c 03a0 057c 01a1  .|.t...r.|...|..
-000026b0: 0101 0071 1271 0664 0153 0029 027a 670a  ...q.q.d.S.).zg.
-000026c0: 2020 2020 2020 2020 5570 6461 7465 7320          Updates 
-000026d0: 7468 6520 656e 7365 6d62 6c65 2073 7461  the ensemble sta
-000026e0: 7469 7374 6963 730a 2020 2020 2020 2020  tistics.        
-000026f0: 6279 2063 616c 6c69 6e67 2069 7420 6f6e  by calling it on
-00002700: 2065 6163 6820 3a6f 626a 3a60 456e 7365   each :obj:`Ense
-00002710: 6d62 6c65 5072 6f70 6f73 616c 600a 2020  mbleProposal`.  
-00002720: 2020 2020 2020 4e29 0672 8600 0000 7209        N).r....r.
-00002730: 0000 0072 4d00 0000 724e 0000 0072 0800  ...rM...rN...r..
-00002740: 0000 724f 0000 0029 0472 2800 0000 7251  ..rO...).r(...rQ
-00002750: 0000 0072 4500 0000 7252 0000 0072 2900  ...rE...rR...r).
-00002760: 0000 7229 0000 0072 2a00 0000 724f 0000  ..r)...r*...rO..
-00002770: 00a8 0100 0073 0800 0000 0005 0a01 0c01  .....s..........
-00002780: 0a01 7a1a 5361 6d70 6c65 7273 4379 636c  ..z.SamplersCycl
-00002790: 652e 7365 745f 656e 7365 6d62 6c65 4e29  e.set_ensembleN)
-000027a0: 0972 5300 0000 7254 0000 0072 5500 0000  .rS...rT...rU...
-000027b0: 7256 0000 0072 8a00 0000 7287 0000 0072  rV...r....r....r
-000027c0: 2b00 0000 724a 0000 0072 4f00 0000 7229  +...rJ...rO...r)
-000027d0: 0000 0072 2900 0000 7229 0000 0072 2a00  ...r)...r)...r*.
-000027e0: 0000 7285 0000 008d 0100 0073 0c00 0000  ..r........s....
-000027f0: 0802 040c 0401 0401 0804 0807 7285 0000  ............r...
-00002800: 0029 25da 0a5f 5f66 7574 7572 655f 5f72  .)%..__future__r
-00002810: 0200 0000 da03 7379 7372 4300 0000 721a  ......sysrC...r.
-00002820: 0000 00da 056e 756d 7079 7214 0000 00da  .....numpyr.....
-00002830: 046d 6174 6872 0300 0000 da0b 636f 6c6c  .mathr......coll
-00002840: 6563 7469 6f6e 7372 0400 0000 da00 7206  ectionsr......r.
-00002850: 0000 0072 0900 0000 7207 0000 0072 0800  ...r....r....r..
-00002860: 0000 da16 6e75 6d70 792e 6c69 622e 7265  ....numpy.lib.re
-00002870: 6366 756e 6374 696f 6e73 da03 6c69 62da  cfunctions..lib.
-00002880: 0c72 6563 6675 6e63 7469 6f6e 73da 0372  .recfunctions..r
-00002890: 666e 723c 0000 00da 086e 6573 7432 706f  fnr<.....nest2po
-000028a0: 7372 0a00 0000 720b 0000 0072 4b00 0000  sr....r....rK...
-000028b0: da02 6763 da06 7069 636b 6c65 5a11 5f5f  ..gc..pickleZ.__
-000028c0: 6368 6563 6b70 6f69 6e74 5f66 6c61 67da  checkpoint_flag.
-000028d0: 066f 626a 6563 7472 0c00 0000 da06 7265  .objectr......re
-000028e0: 6d6f 7465 7257 0000 005a 0f66 6967 6172  moterW...Z.figar
-000028f0: 6f5f 6772 6164 6965 6e74 7264 0000 0072  o_gradientrd...r
-00002900: 6500 0000 726b 0000 0072 8500 0000 7229  e...rk...r....r)
-00002910: 0000 0072 2900 0000 7229 0000 0072 2a00  ...r)...r)...r*.
-00002920: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002930: 7338 0000 000c 0108 0108 0108 0108 010c  s8..............
-00002940: 010c 020c 0110 010c 0112 0108 0110 0108  ................
-00002950: 0108 0208 0104 0310 7f00 0904 0112 290c  ..............).
-00002960: 0104 0112 3804 0112 7f00 0b04 01         ....8........
+00000100: 8303 8301 5a1f 7a10 6405 640f 6c20 6d21  ....Z.z.d.d.l m!
+00000110: 5a21 0100 5700 6e14 0100 0100 0100 6522  Z!..W.n.......e"
+00000120: 6410 8301 0100 5900 6e02 3000 6518 6a1e  d.....Y.n.0.e.j.
+00000130: 4700 6411 6412 8400 6412 651d 8303 8301  G.d.d...d.e.....
+00000140: 5a23 6518 6a1e 4700 6413 6414 8400 6414  Z#e.j.G.d.d...d.
+00000150: 651d 8303 8301 5a24 6518 6a1e 4700 6415  e.....Z$e.j.G.d.
+00000160: 6416 8400 6416 651d 8303 8301 5a25 6402  d...d.e.....Z%d.
+00000170: 5300 2917 e900 0000 0029 01da 0864 6976  S.)......)...div
+00000180: 6973 696f 6e4e 2901 da03 6c6f 6729 01da  isionN)...log)..
+00000190: 0564 6571 7565 e901 0000 0029 01da 0970  .deque.....)...p
+000001a0: 6172 616d 6574 6572 2902 da14 4465 6661  arameter)...Defa
+000001b0: 756c 7450 726f 706f 7361 6c43 7963 6c65  ultProposalCycle
+000001c0: da10 456e 7365 6d62 6c65 5072 6f70 6f73  ..EnsemblePropos
+000001d0: 616c 2901 da08 7072 6f70 6f73 616c 2902  al)...proposal).
+000001e0: da03 6163 6cda 0f61 7574 6f63 6f72 7265  ..acl..autocorre
+000001f0: 6c61 7469 6f6e 4663 0000 0000 0000 0000  lationFc........
+00000200: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000210: 733e 0000 0065 005a 0164 005a 0264 015a  s>...e.Z.d.Z.d.Z
+00000220: 0364 1064 0464 0584 015a 0464 1164 0764  .d.d.d...Z.d.d.d
+00000230: 0884 015a 0564 1264 0a64 0b84 015a 0664  ...Z.d.d.d...Z.d
+00000240: 0c64 0d84 005a 0764 0e64 0f84 005a 0864  .d...Z.d.d...Z.d
+00000250: 0253 0029 13da 0753 616d 706c 6572 61e5  .S.)...Samplera.
+00000260: 0100 000a 2020 2020 5361 6d70 6c65 7220  ....    Sampler 
+00000270: 636c 6173 732e 0a20 2020 202d 2d2d 2d2d  class..    -----
+00000280: 2d2d 2d2d 0a0a 2020 2020 496e 6974 6961  ----..    Initia
+00000290: 6c69 7361 7469 6f6e 2061 7267 756d 656e  lisation argumen
+000002a0: 7473 3a0a 0a20 2020 2061 7267 733a 0a20  ts:..    args:. 
+000002b0: 2020 206d 6f64 656c 3a20 3a6f 626a 3a60     model: :obj:`
+000002c0: 7261 796e 6573 742e 4d6f 6465 6c60 2075  raynest.Model` u
+000002d0: 7365 7220 6465 6669 6e65 6420 6d6f 6465  ser defined mode
+000002e0: 6c20 746f 2073 616d 706c 650a 0a20 2020  l to sample..   
+000002f0: 206d 6178 6d63 6d63 3a0a 2020 2020 2020   maxmcmc:.      
+00000300: 2020 3a69 6e74 3a20 6d61 7869 6d75 6d20    :int: maximum 
+00000310: 6e75 6d62 6572 206f 6620 6d63 6d63 2073  number of mcmc s
+00000320: 7465 7073 2074 6f20 6265 2075 7365 6420  teps to be used 
+00000330: 696e 2074 6865 203a 6f62 6a3a 6063 6e65  in the :obj:`cne
+00000340: 7374 2e73 616d 706c 6572 2e53 616d 706c  st.sampler.Sampl
+00000350: 6572 600a 0a20 2020 202d 2d2d 2d2d 2d2d  er`..    -------
+00000360: 2d2d 2d0a 2020 2020 6b77 6172 6773 3a0a  ---.    kwargs:.
+00000370: 0a20 2020 2076 6572 626f 7365 3a0a 2020  .    verbose:.  
+00000380: 2020 2020 2020 3a69 6e74 3a20 6469 7370        :int: disp
+00000390: 6c61 7920 6465 6275 6720 696e 666f 726d  lay debug inform
+000003a0: 6174 696f 6e20 6f6e 2073 6372 6565 6e0a  ation on screen.
+000003b0: 2020 2020 2020 2020 4465 6661 756c 743a          Default:
+000003c0: 2030 0a0a 2020 2020 7072 6f70 6f73 616c   0..    proposal
+000003d0: 3a0a 2020 2020 2020 2020 3a6f 626a 3a60  :.        :obj:`
+000003e0: 7261 796e 6573 742e 7072 6f70 6f73 616c  raynest.proposal
+000003f0: 732e 5072 6f70 6f73 616c 6020 746f 2075  s.Proposal` to u
+00000400: 7365 0a20 2020 2020 2020 2044 6566 6175  se.        Defau
+00000410: 6c74 733a 203a 6f62 6a3a 6072 6179 6e65  lts: :obj:`rayne
+00000420: 7374 2e70 726f 706f 7361 6c73 2e44 6566  st.proposals.Def
+00000430: 6175 6c74 5072 6f70 6f73 616c 4379 636c  aultProposalCycl
+00000440: 6560 290a 2020 2020 4e72 0100 0000 6306  e`).    Nr....c.
+00000450: 0000 0000 0000 0000 0000 0006 0000 0004  ................
+00000460: 0000 0043 0000 0073 d000 0000 6401 7c00  ...C...s....d.|.
+00000470: 5f00 7c01 7c00 5f01 7c03 6400 6b02 7222  _.|.|._.|.d.k.r"
+00000480: 7402 6a03 a004 a100 7c00 5f05 6e06 7c03  t.j.....|._.n.|.
+00000490: 7c00 5f05 7c02 6402 1a00 7c00 5f06 7c02  |._.|.d...|._.|.
+000004a0: 7c00 5f07 6400 7c00 5f08 7409 a00a 6403  |._.d.|._.t...d.
+000004b0: a101 7c00 5f0b 7c05 6400 7500 7260 740c  ..|._.|.d.u.r`t.
+000004c0: 7c00 6a05 8301 7c00 5f0d 6e12 7c05 7c00  |.j...|._.n.|.|.
+000004d0: 6a05 7c00 6a01 6404 8d02 7c00 5f0d 7c00  j.|.j.d...|._.|.
+000004e0: 6a06 7c00 5f0e 740f 7c00 6a06 8301 7c00  j.|._.t.|.j...|.
+000004f0: 5f10 7c04 7c00 5f11 6405 7c00 5f12 6405  _.|.|._.d.|._.d.
+00000500: 7c00 5f13 6401 7c00 5f14 6401 7c00 5f15  |._.d.|._.d.|._.
+00000510: 6406 7c00 5f16 6407 7c00 5f17 7418 7c00  d.|._.d.|._.t.|.
+00000520: 6a11 6408 6b05 72c0 6400 6e04 7c00 6a17  j.d.k.r.d.n.|.j.
+00000530: 6409 8d01 7c00 5f19 6400 5300 290a 4e72  d...|._.d.S.).Nr
+00000540: 0100 0000 e90a 0000 00da 0772 6179 6e65  ...........rayne
+00000550: 7374 2901 da05 6d6f 6465 6ce7 0000 0000  st)...model.....
+00000560: 0000 0000 4669 0080 0000 e903 0000 0029  ....Fi.........)
+00000570: 01da 066d 6178 6c65 6e29 1ada 0763 6f75  ...maxlen)...cou
+00000580: 6e74 6572 720f 0000 00da 026e 70da 0672  nterr......np..r
+00000590: 616e 646f 6dda 0b64 6566 6175 6c74 5f72  andom..default_r
+000005a0: 6e67 da03 726e 675a 0c69 6e69 7469 616c  ng..rngZ.initial
+000005b0: 5f6d 636d 63da 076d 6178 6d63 6d63 da03  _mcmc..maxmcmc..
+000005c0: 7461 75da 076c 6f67 6769 6e67 da09 6765  tau..logging..ge
+000005d0: 744c 6f67 6765 72da 066c 6f67 6765 7272  tLogger..loggerr
+000005e0: 0700 0000 7209 0000 00da 054e 6d63 6d63  ....r......Nmcmc
+000005f0: da05 666c 6f61 74da 0b4e 6d63 6d63 5f65  ..float..Nmcmc_e
+00000600: 7861 6374 da07 7665 7262 6f73 65da 0a61  xact..verbose..a
+00000610: 6363 6570 7461 6e63 65da 0e73 7562 5f61  cceptance..sub_a
+00000620: 6363 6570 7461 6e63 65da 0d6d 636d 635f  cceptance..mcmc_
+00000630: 6163 6365 7074 6564 da0c 6d63 6d63 5f63  accepted..mcmc_c
+00000640: 6f75 6e74 6572 da0b 696e 6974 6961 6c69  ounter..initiali
+00000650: 7365 64da 0b6d 6178 5f73 746f 7261 6765  sed..max_storage
+00000660: 7204 0000 00da 0773 616d 706c 6573 2906  r......samples).
+00000670: da04 7365 6c66 720f 0000 0072 1800 0000  ..selfr....r....
+00000680: 7217 0000 0072 2000 0000 7209 0000 00a9  r....r ...r.....
+00000690: 0072 2900 0000 fa29 2f55 7365 7273 2f77  .r)....)/Users/w
+000006a0: 6470 2f73 7263 2f72 6179 6e65 7374 2f72  dp/src/raynest/r
+000006b0: 6179 6e65 7374 2f73 616d 706c 6572 2e70  aynest/sampler.p
+000006c0: 79da 085f 5f69 6e69 745f 5f2f 0000 0073  y..__init__/...s
+000006d0: 2c00 0000 0007 0601 0601 0801 0e02 0601  ,...............
+000006e0: 0a01 0601 0601 0c02 0801 0e02 1202 0801  ................
+000006f0: 0c02 0601 0601 0601 0601 0601 0601 0601  ................
+00000700: 7a10 5361 6d70 6c65 722e 5f5f 696e 6974  z.Sampler.__init
+00000710: 5f5f e905 0000 0063 0300 0000 0000 0000  __.....c........
+00000720: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+00000730: 7384 0000 007c 0264 0175 0072 0e7c 006a  s....|.d.u.r.|.j
+00000740: 007d 027c 006a 0164 026b 0272 2e64 0364  .}.|.j.d.k.r.d.d
+00000750: 037c 021b 0017 007c 006a 0214 007c 005f  .|.....|.j...|._
+00000760: 026e 2a64 0364 037c 021b 0018 007c 006a  .n*d.d.|.....|.j
+00000770: 0214 007c 017c 021b 0064 047c 006a 011b  ...|.|...d.|.j..
+00000780: 0064 0318 0014 0017 007c 005f 0274 0374  .d.......|._.t.t
+00000790: 047c 006a 027c 006a 0083 0283 017c 005f  .|.j.|.j.....|._
+000007a0: 0274 057c 0174 067c 006a 0283 0183 027c  .t.|.t.|.j.....|
+000007b0: 005f 077c 006a 0753 0029 0561 3601 0000  ._.|.j.S.).a6...
+000007c0: 0a20 2020 2020 2020 2045 7374 696d 6174  .        Estimat
+000007d0: 6520 6175 746f 636f 7272 656c 6174 696f  e autocorrelatio
+000007e0: 6e20 6c65 6e67 7468 206f 6620 6368 6169  n length of chai
+000007f0: 6e20 7573 696e 6720 6163 6365 7074 616e  n using acceptan
+00000800: 6365 2066 7261 6374 696f 6e0a 2020 2020  ce fraction.    
+00000810: 2020 2020 4143 4c20 3d20 2832 2f61 6363      ACL = (2/acc
+00000820: 2920 2d20 310a 2020 2020 2020 2020 6d75  ) - 1.        mu
+00000830: 6c74 6970 6c69 6564 2062 7920 6120 7361  ltiplied by a sa
+00000840: 6665 7479 206d 6172 6769 6e20 6f66 2035  fety margin of 5
+00000850: 0a20 2020 2020 2020 2055 7365 7320 6d6f  .        Uses mo
+00000860: 7669 6e67 2061 7665 7261 6765 2077 6974  ving average wit
+00000870: 6820 6465 6361 7920 7469 6d65 2074 6175  h decay time tau
+00000880: 2069 7465 7261 7469 6f6e 730a 2020 2020   iterations.    
+00000890: 2020 2020 2864 6566 6175 6c74 3a20 3a69      (default: :i
+000008a0: 6e74 3a60 7365 6c66 2e6d 6178 6d63 6d63  nt:`self.maxmcmc
+000008b0: 6029 0a0a 2020 2020 2020 2020 5461 6b65  `)..        Take
+000008c0: 6e20 6672 6f6d 2068 7474 703a 2f2f 6769  n from http://gi
+000008d0: 7468 7562 2e63 6f6d 2f66 6172 722f 456e  thub.com/farr/En
+000008e0: 7365 6d62 6c65 4e65 7374 2e6a 6c0a 2020  sembleNest.jl.  
+000008f0: 2020 2020 2020 4e72 1000 0000 e700 0000        Nr........
+00000900: 0000 00f0 3f67 0000 0000 0000 0040 2908  ....?g.......@).
+00000910: 7218 0000 0072 2200 0000 721f 0000 0072  r....r"...r....r
+00000920: 1e00 0000 da03 6d69 6eda 036d 6178 da03  ......min..max..
+00000930: 696e 7472 1d00 0000 2903 7228 0000 00da  intr....).r(....
+00000940: 0673 6166 6574 7972 1900 0000 7229 0000  .safetyr....r)..
+00000950: 0072 2900 0000 722a 0000 00da 1965 7374  .r)...r*.....est
+00000960: 696d 6174 655f 6e6d 636d 635f 6f6e 5f74  imate_nmcmc_on_t
+00000970: 6865 5f66 6c79 5200 0000 730e 0000 0000  he_flyR...s.....
+00000980: 0c0e 030a 0116 022a 0214 0112 027a 2153  .......*.....z!S
+00000990: 616d 706c 6572 2e65 7374 696d 6174 655f  ampler.estimate_
+000009a0: 6e6d 636d 635f 6f6e 5f74 6865 5f66 6c79  nmcmc_on_the_fly
+000009b0: 7205 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000009c0: 0000 0500 0000 0900 0000 0300 0000 73b2  ..............s.
+000009d0: 0000 0067 007d 0274 007c 006a 0183 017d  ...g.}.t.|.j...}
+000009e0: 0374 02a0 0364 0164 0284 007c 037c 006a  .t...d.d...|.|.j
+000009f0: 040b 0064 0385 0219 0044 0083 01a1 0189  ...d.....D......
+00000a00: 0087 0066 0164 0464 0284 0874 0588 006a  ...f.d.d...t...j
+00000a10: 0664 0519 0083 0144 0083 017d 027c 006a  .d.....D...}.|.j
+00000a20: 0764 066b 0572 9074 0574 087c 006a 096a  .d.k.r.t.t.|.j.j
+00000a30: 0a83 0183 0144 005d 2a7d 047c 006a 0ba0  .....D.]*}.|.j..
+00000a40: 0c64 07a0 0d74 0ea0 0fa1 007c 006a 096a  .d...t.....|.j.j
+00000a50: 0a7c 0419 007c 027c 0419 00a1 03a1 0101  .|...|.|........
+00000a60: 0071 6474 02a0 107c 02a1 017c 005f 1174  .qdt...|...|._.t
+00000a70: 127c 017c 006a 1114 0083 017c 005f 137c  .|.|.j.....|._.|
+00000a80: 006a 1353 0029 087a 960a 2020 2020 2020  .j.S.).z..      
+00000a90: 2020 4573 7469 6d61 7465 2061 7574 6f63    Estimate autoc
+00000aa0: 6f72 7265 6c61 7469 6f6e 206c 656e 6774  orrelation lengt
+00000ab0: 6820 6f66 2074 6865 2063 6861 696e 0a20  h of the chain. 
+00000ac0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000ad0: 7361 6665 7479 2064 6574 6572 6d69 6e65  safety determine
+00000ae0: 7320 7468 6520 6e75 6d62 6572 206f 6620  s the number of 
+00000af0: 4143 4c20 7468 6520 6368 6169 6e73 2061  ACL the chains a
+00000b00: 7265 2067 6f69 6e67 2074 6f20 6265 2072  re going to be r
+00000b10: 756e 2066 6f72 0a20 2020 2020 2020 2063  un for.        c
+00000b20: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000b30: 0300 0000 5300 0000 7312 0000 0067 007c  ....S...s....g.|
+00000b40: 005d 0a7d 017c 016a 0091 0271 0453 0072  .].}.|.j...q.S.r
+00000b50: 2900 0000 2901 da06 7661 6c75 6573 2902  )...)...values).
+00000b60: da02 2e30 da01 7872 2900 0000 7229 0000  ...0..xr)...r)..
+00000b70: 0072 2a00 0000 da0a 3c6c 6973 7463 6f6d  .r*.....<listcom
+00000b80: 703e 7500 0000 f300 0000 007a 2853 616d  p>u........z(Sam
+00000b90: 706c 6572 2e65 7374 696d 6174 655f 6163  pler.estimate_ac
+00000ba0: 6c2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  l.<locals>.<list
+00000bb0: 636f 6d70 3e4e 6301 0000 0000 0000 0000  comp>Nc.........
+00000bc0: 0000 0002 0000 0006 0000 0013 0000 0073  ...............s
+00000bd0: 2400 0000 6700 7c00 5d1c 7d01 7400 8800  $...g.|.].}.t...
+00000be0: 6400 6400 8502 7c01 6602 1900 6401 6402  d.d...|.f...d.d.
+00000bf0: 8d02 9102 7104 5300 2903 4e72 2c00 0000  ....q.S.).Nr,...
+00000c00: 2901 da01 6329 0172 0a00 0000 2902 7234  )...c).r....).r4
+00000c10: 0000 00da 0169 a901 7227 0000 0072 2900  .....i..r'...r).
+00000c20: 0000 722a 0000 0072 3600 0000 7700 0000  ..r*...r6...w...
+00000c30: 7237 0000 0072 0500 0000 7211 0000 007a  r7...r....r....z
+00000c40: 1e53 616d 706c 6572 207b 307d 202d 2d20  .Sampler {0} -- 
+00000c50: 4143 4c28 7b31 7d29 2020 3d20 7b32 7d29  ACL({1})  = {2})
+00000c60: 14da 046c 6973 7472 2700 0000 7214 0000  ...listr'...r...
+00000c70: 00da 0561 7272 6179 7226 0000 00da 0572  ...arrayr&.....r
+00000c80: 616e 6765 da05 7368 6170 6572 2000 0000  ange..shaper ...
+00000c90: da03 6c65 6e72 0f00 0000 da05 6e61 6d65  ..lenr......name
+00000ca0: 7372 1c00 0000 da04 696e 666f da06 666f  sr......info..fo
+00000cb0: 726d 6174 da02 6f73 da06 6765 7470 6964  rmat..os..getpid
+00000cc0: 722f 0000 0072 1900 0000 7230 0000 0072  r/...r....r0...r
+00000cd0: 1d00 0000 2905 7228 0000 0072 3100 0000  ....).r(...r1...
+00000ce0: 5a03 4143 4cda 0173 7239 0000 0072 2900  Z.ACL..sr9...r).
+00000cf0: 0000 723a 0000 0072 2a00 0000 da0c 6573  ..r:...r*.....es
+00000d00: 7469 6d61 7465 5f61 636c 6b00 0000 7314  timate_aclk...s.
+00000d10: 0000 0000 0804 010a 0120 021c 020a 0114  ......... ......
+00000d20: 0128 030c 0210 017a 1453 616d 706c 6572  .(.....z.Sampler
+00000d30: 2e65 7374 696d 6174 655f 6163 6c63 0300  .estimate_aclc..
+00000d40: 0000 0000 0000 0000 0000 0500 0000 0400  ................
+00000d50: 0000 4300 0000 7344 0000 007c 00a0 007c  ..C...sD...|...|
+00000d60: 017c 02a1 025c 027d 037d 047c 0004 006a  .|...\.}.}.|...j
+00000d70: 0164 0137 0002 005f 017c 006a 0164 0216  .d.7..._.|.j.d..
+00000d80: 0064 036b 0272 347c 00a0 02a1 0001 007c  .d.k.r4|.......|
+00000d90: 006a 037c 006a 047c 037c 0466 0453 0029  .j.|.j.|.|.f.S.)
+00000da0: 047a b60a 2020 2020 2020 2020 6d61 696e  .z..        main
+00000db0: 206c 6f6f 7020 7468 6174 2074 616b 6573   loop that takes
+00000dc0: 2074 6865 2077 6f72 7374 203a 6f62 6a3a   the worst :obj:
+00000dd0: 6072 6179 6e65 7374 2e70 6172 616d 6574  `raynest.paramet
+00000de0: 6572 2e4c 6976 6550 6f69 6e74 6020 616e  er.LivePoint` an
+00000df0: 640a 2020 2020 2020 2020 6576 6f6c 7665  d.        evolve
+00000e00: 7320 6974 2e20 5072 6f70 6f73 6564 2073  s it. Proposed s
+00000e10: 616d 706c 6520 6973 2074 6865 6e20 7365  ample is then se
+00000e20: 6e74 2062 6163 6b0a 2020 2020 2020 2020  nt back.        
+00000e30: 746f 203a 6f62 6a3a 6072 6179 6e65 7374  to :obj:`raynest
+00000e40: 2e4e 6573 7465 6453 616d 706c 6572 602e  .NestedSampler`.
+00000e50: 0a20 2020 2020 2020 2072 0500 0000 720d  .        r....r.
+00000e60: 0000 0072 0100 0000 2905 da0d 7265 7475  ...r....)...retu
+00000e70: 726e 5f73 616d 706c 6572 1300 0000 7246  rn_sampler....rF
+00000e80: 0000 0072 2100 0000 7222 0000 0029 0572  ...r!...r"...).r
+00000e90: 2800 0000 da03 6f6c 64da 076c 6f67 4c6d  (.....old..logLm
+00000ea0: 696e 721d 0000 005a 086f 7574 5061 7261  inr....Z.outPara
+00000eb0: 6d72 2900 0000 7229 0000 0072 2a00 0000  mr)...r)...r*...
+00000ec0: da0e 7072 6f64 7563 655f 7361 6d70 6c65  ..produce_sample
+00000ed0: 8300 0000 730a 0000 0000 0610 030e 010e  ....s...........
+00000ee0: 0108 027a 1653 616d 706c 6572 2e70 726f  ...z.Sampler.pro
+00000ef0: 6475 6365 5f73 616d 706c 6563 0200 0000  duce_samplec....
+00000f00: 0000 0000 0000 0000 0400 0000 0600 0000  ................
+00000f10: 4300 0000 7356 0000 007c 006a 0064 016b  C...sV...|.j.d.k
+00000f20: 0472 207c 006a 01a0 0264 02a0 0374 04a0  .r |.j...d...t..
+00000f30: 05a1 00a1 01a1 0101 0074 06a0 077c 01a1  .........t...|..
+00000f40: 0164 0319 007d 027c 006a 086a 0944 005d  .d...}.|.j.j.D.]
+00000f50: 187d 0374 0a7c 0374 0b83 0272 367c 03a0  .}.t.|.t...r6|..
+00000f60: 0c7c 02a1 0101 0071 367e 0264 0353 0029  .|.....q6~.d.S.)
+00000f70: 044e 7211 0000 007a 1f53 616d 706c 6572  .Nr....z.Sampler
+00000f80: 207b 307d 202d 2d20 7365 7474 696e 6720   {0} -- setting 
+00000f90: 656e 7365 6d62 6c65 7201 0000 0029 0d72  ensembler....).r
+00000fa0: 2000 0000 721c 0000 0072 4100 0000 7242   ...r....rA...rB
+00000fb0: 0000 0072 4300 0000 7244 0000 00da 0372  ...rC...rD.....r
+00000fc0: 6179 da03 6765 7472 0900 0000 da09 7072  ay..getr......pr
+00000fd0: 6f70 6f73 616c 73da 0a69 7369 6e73 7461  oposals..isinsta
+00000fe0: 6e63 6572 0800 0000 da0c 7365 745f 656e  ncer......set_en
+00000ff0: 7365 6d62 6c65 2904 7228 0000 00da 0c65  semble).r(.....e
+00001000: 6e73 656d 626c 655f 7265 66da 0865 6e73  nsemble_ref..ens
+00001010: 656d 626c 65da 0170 7229 0000 0072 2900  emble..pr)...r).
+00001020: 0000 722a 0000 0072 4f00 0000 9200 0000  ..r*...rO.......
+00001030: 7310 0000 0000 010a 0116 020e 010c 010a  s...............
+00001040: 010c 0102 027a 1453 616d 706c 6572 2e73  .....z.Sampler.s
+00001050: 6574 5f65 6e73 656d 626c 6529 034e 7201  et_ensemble).Nr.
+00001060: 0000 004e 2902 722c 0000 004e 2901 7205  ...N).r,...N).r.
+00001070: 0000 0029 09da 085f 5f6e 616d 655f 5fda  ...)...__name__.
+00001080: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00001090: 7561 6c6e 616d 655f 5fda 075f 5f64 6f63  ualname__..__doc
+000010a0: 5f5f 722b 0000 0072 3200 0000 7246 0000  __r+...r2...rF..
+000010b0: 0072 4a00 0000 724f 0000 0072 2900 0000  .rJ...rO...r)...
+000010c0: 7229 0000 0072 2900 0000 722a 0000 0072  r)...r)...r*...r
+000010d0: 0c00 0000 1600 0000 7312 0000 0008 0104  ........s.......
+000010e0: 1b00 0100 0100 fb0a 230a 190a 1808 0f72  ........#......r
+000010f0: 0c00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00001100: 0000 0000 0002 0000 0040 0000 0073 1800  .........@...s..
+00001110: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00001120: 6403 8400 5a04 6404 5300 2905 da19 4d65  d...Z.d.S.)...Me
+00001130: 7472 6f70 6f6c 6973 4861 7374 696e 6773  tropolisHastings
+00001140: 5361 6d70 6c65 727a 5e0a 2020 2020 6d65  Samplerz^.    me
+00001150: 7472 6f70 6f6c 6973 2d68 6173 7469 6e67  tropolis-hasting
+00001160: 7320 6163 6365 7074 616e 6365 2072 756c  s acceptance rul
+00001170: 650a 2020 2020 666f 7220 3a6f 626a 3a60  e.    for :obj:`
+00001180: 7261 796e 6573 742e 7072 6f70 6f73 616c  raynest.proposal
+00001190: 2e45 6e73 656d 626c 6550 726f 706f 7361  .EnsembleProposa
+000011a0: 6c60 0a20 2020 2063 0300 0000 0000 0000  l`.    c........
+000011b0: 0000 0000 0700 0000 0500 0000 4300 0000  ............C...
+000011c0: 7302 0100 0064 017d 0364 017d 047c 006a  s....d.}.d.}.|.j
+000011d0: 00a0 017c 01a1 017d 057c 0364 0237 007d  ...|...}.|.d.7.}
+000011e0: 037c 006a 02a0 037c 01a0 04a1 00a1 017d  .|.j...|.......}
+000011f0: 067c 006a 00a0 017c 06a1 017c 065f 057c  .|.j...|...|._.|
+00001200: 066a 057c 0518 007c 006a 026a 0617 0074  .j.|...|.j.j...t
+00001210: 07a0 087c 006a 09a0 0aa1 00a1 016b 0472  ...|.j.......k.r
+00001220: 8a7c 006a 00a0 0b7c 06a1 017c 065f 0c7c  .|.j...|...|._.|
+00001230: 066a 0c7c 026b 0472 8a7c 06a0 04a1 007d  .j.|.k.r.|.....}
+00001240: 017c 066a 057d 057c 0464 0237 007d 047c  .|.j.}.|.d.7.}.|
+00001250: 006a 0da0 0e7c 01a1 0101 007c 037c 006a  .j...|.....|.|.j
+00001260: 0f6b 0572 a87c 0464 016b 0473 b67c 037c  .k.r.|.d.k.s.|.|
+00001270: 006a 106b 0572 1471 b671 1474 117c 0483  .j.k.r.q.q.t.|..
+00001280: 0174 117c 0383 011b 007c 005f 127c 0004  .t.|.....|._.|..
+00001290: 006a 137c 0437 0002 005f 137c 0004 006a  .j.|.7..._.|...j
+000012a0: 147c 0337 0002 005f 1474 117c 006a 1383  .|.7..._.t.|.j..
+000012b0: 0174 117c 006a 1483 011b 007c 005f 157c  .t.|.j.....|._.|
+000012c0: 037c 0166 0253 0029 034e 7201 0000 0072  .|.f.S.).Nr....r
+000012d0: 0500 0000 2916 720f 0000 00da 096c 6f67  ....).r......log
+000012e0: 5f70 7269 6f72 7209 0000 00da 0a67 6574  _priorr......get
+000012f0: 5f73 616d 706c 65da 0463 6f70 79da 046c  _sample..copy..l
+00001300: 6f67 50da 056c 6f67 5f4a 7214 0000 0072  ogP..log_Jr....r
+00001310: 0300 0000 7217 0000 0072 1500 0000 da0e  ....r....r......
+00001320: 6c6f 675f 6c69 6b65 6c69 686f 6f64 da04  log_likelihood..
+00001330: 6c6f 674c 7227 0000 00da 0661 7070 656e  logLr'.....appen
+00001340: 6472 1d00 0000 7218 0000 0072 1e00 0000  dr....r....r....
+00001350: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
+00001360: 2100 0000 2907 7228 0000 00da 086f 6c64  !...).r(.....old
+00001370: 7061 7261 6d72 4900 0000 da0b 7375 625f  paramrI.....sub_
+00001380: 636f 756e 7465 72da 0c73 7562 5f61 6363  counter..sub_acc
+00001390: 6570 7465 645a 086c 6f67 705f 6f6c 64da  eptedZ.logp_old.
+000013a0: 086e 6577 7061 7261 6d72 2900 0000 7229  .newparamr)...r)
+000013b0: 0000 0072 2a00 0000 7247 0000 00a4 0000  ...r*...rG......
+000013c0: 0073 2800 0000 0002 0401 0401 0c04 0801  .s(.............
+000013d0: 1001 0e02 2202 0e02 0a02 0801 0601 0803  ...."...........
+000013e0: 0c02 1c01 0402 1201 0e01 0e01 1602 7a27  ..............z'
+000013f0: 4d65 7472 6f70 6f6c 6973 4861 7374 696e  MetropolisHastin
+00001400: 6773 5361 6d70 6c65 722e 7265 7475 726e  gsSampler.return
+00001410: 5f73 616d 706c 654e 2905 7253 0000 0072  _sampleN).rS...r
+00001420: 5400 0000 7255 0000 0072 5600 0000 7247  T...rU...rV...rG
+00001430: 0000 0072 2900 0000 7229 0000 0072 2900  ...r)...r)...r).
+00001440: 0000 722a 0000 0072 5700 0000 9e00 0000  ..r*...rW.......
+00001450: 7304 0000 0008 0204 0472 5700 0000 2901  s........rW...).
+00001460: da06 4144 5047 4d4d 7a4c 5761 726e 696e  ..ADPGMMzLWarnin
+00001470: 6721 2066 6967 6172 6f20 7061 636b 6167  g! figaro packag
+00001480: 6520 6e6f 7420 6176 6169 6c61 626c 652c  e not available,
+00001490: 2074 6865 2048 4d43 2073 616d 706c 6572   the HMC sampler
+000014a0: 2077 696c 6c20 6e6f 7420 6265 2061 7661   will not be ava
+000014b0: 696c 6162 6c65 6300 0000 0000 0000 0000  ilablec.........
+000014c0: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
+000014d0: 2800 0000 6500 5a01 6400 5a02 6401 5a03  (...e.Z.d.Z.d.Z.
+000014e0: 6402 5a04 6403 5a05 6404 6405 8400 5a06  d.Z.d.Z.d.d...Z.
+000014f0: 6406 6407 8400 5a07 6403 5300 2908 da1c  d.d...Z.d.S.)...
+00001500: 4861 6d69 6c74 6f6e 6961 6e4d 6f6e 7465  HamiltonianMonte
+00001510: 4361 726c 6f53 616d 706c 6572 7a63 0a20  CarloSamplerzc. 
+00001520: 2020 2048 616d 696c 746f 6e69 616e 4d6f     HamiltonianMo
+00001530: 6e74 6543 6172 6c6f 2061 6363 6570 7461  nteCarlo accepta
+00001540: 6e63 6520 7275 6c65 0a20 2020 2066 6f72  nce rule.    for
+00001550: 203a 6f62 6a3a 6072 6179 6e65 7374 2e70   :obj:`raynest.p
+00001560: 726f 706f 7361 6c2e 4861 6d69 6c74 6f6e  roposal.Hamilton
+00001570: 6961 6e50 726f 706f 7361 6c60 0a20 2020  ianProposal`.   
+00001580: 2046 4e63 0200 0000 0000 0000 0000 0000   FNc............
+00001590: 0500 0000 0400 0000 4300 0000 7360 0000  ........C...s`..
+000015a0: 0074 00a0 017c 01a1 0164 0119 007d 027c  .t...|...d...}.|
+000015b0: 02a0 02a1 0001 007c 02a0 03a1 007d 0374  .......|.....}.t
+000015c0: 047c 006a 056a 0664 0264 038d 027c 005f  .|.j.j.d.d...|._
+000015d0: 077c 026a 0844 005d 127d 047c 006a 07a0  .|.j.D.].}.|.j..
+000015e0: 097c 046a 0aa1 0101 0071 367c 006a 0ba0  .|.j.....q6|.j..
+000015f0: 0c7c 006a 077c 0366 02a1 0101 0064 0153  .|.j.|.f.....d.S
+00001600: 0029 044e 7201 0000 0046 2901 5a06 7072  .).Nr....F).Z.pr
+00001610: 6f62 6974 290d 724b 0000 0072 4c00 0000  obit).rK...rL...
+00001620: 5a16 7570 6461 7465 5f6d 6561 6e5f 636f  Z.update_mean_co
+00001630: 7661 7269 616e 6365 5a0e 6765 745f 636f  varianceZ.get_co
+00001640: 7661 7269 616e 6365 7264 0000 0072 0f00  variancerd...r..
+00001650: 0000 da06 626f 756e 6473 da07 6465 6e73  ....bounds..dens
+00001660: 6974 79da 055f 6c69 7374 da0d 6164 645f  ity.._list..add_
+00001670: 6e65 775f 706f 696e 7472 3300 0000 7209  new_pointr3...r.
+00001680: 0000 0072 4f00 0000 2905 7228 0000 0072  ...rO...).r(...r
+00001690: 5000 0000 7251 0000 00da 0a63 6f76 6172  P...rQ.....covar
+000016a0: 6961 6e63 65da 0165 7229 0000 0072 2900  iance..er)...r).
+000016b0: 0000 722a 0000 0072 4f00 0000 d500 0000  ..r*...rO.......
+000016c0: 7310 0000 0000 020e 0208 0108 0212 010a  s...............
+000016d0: 0110 0212 017a 2948 616d 696c 746f 6e69  .....z)Hamiltoni
+000016e0: 616e 4d6f 6e74 6543 6172 6c6f 5361 6d70  anMonteCarloSamp
+000016f0: 6c65 722e 7365 745f 656e 7365 6d62 6c65  ler.set_ensemble
+00001700: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
+00001710: 0005 0000 0043 0000 0073 d200 0000 6401  .....C...s....d.
+00001720: 7d03 6401 7d04 7c04 6402 3700 7d04 7c00  }.d.}.|.d.7.}.|.
+00001730: 6a00 6a01 7c01 a002 a100 7c02 6403 8d02  j.j.|.....|.d...
+00001740: 7d05 7c00 6a00 6a03 7404 a005 7c00 6a06  }.|.j.j.t...|.j.
+00001750: a007 a100 a101 6b04 7256 7c05 6a08 7c02  ......k.rV|.j.|.
+00001760: 6b04 7256 7c05 a002 a100 7d01 7c03 6402  k.rV|.....}.|.d.
+00001770: 3700 7d03 7c00 6a09 a00a 7c01 a101 0100  7.}.|.j...|.....
+00001780: 7c04 7c00 6a0b 6b05 7208 7c03 6401 6b04  |.|.j.k.r.|.d.k.
+00001790: 7208 7178 7108 740c 7c03 8301 740c 7c04  r.qxq.t.|...t.|.
+000017a0: 8301 1b00 7c00 5f0d 7c00 0400 6a0e 7c03  ....|._.|...j.|.
+000017b0: 3700 0200 5f0e 7c00 0400 6a0f 7c04 3700  7..._.|...j.|.7.
+000017c0: 0200 5f0f 740c 7c00 6a0e 8301 740c 7c00  .._.t.|.j...t.|.
+000017d0: 6a0f 8301 1b00 7c00 5f10 7c00 6a11 a012  j.....|._.|.j...
+000017e0: 7c01 6a13 a101 0100 7c04 7c01 6602 5300  |.j.....|.|.f.S.
+000017f0: 2904 4e72 0100 0000 7205 0000 0029 0172  ).Nr....r....).r
+00001800: 4900 0000 2914 7209 0000 0072 5900 0000  I...).r....rY...
+00001810: 725a 0000 0072 5c00 0000 7214 0000 0072  rZ...r\...r....r
+00001820: 0300 0000 7217 0000 0072 1500 0000 725e  ....r....r....r^
+00001830: 0000 0072 2700 0000 725f 0000 0072 1d00  ...r'...r_...r..
+00001840: 0000 721e 0000 0072 2200 0000 7223 0000  ..r....r"...r#..
+00001850: 0072 2400 0000 7221 0000 0072 6700 0000  .r$...r!...rg...
+00001860: 7269 0000 0072 3300 0000 2906 7228 0000  ri...r3...).r(..
+00001870: 0072 6000 0000 7249 0000 0072 6200 0000  .r`...rI...rb...
+00001880: 7261 0000 0072 6300 0000 7229 0000 0072  ra...rc...r)...r
+00001890: 2900 0000 722a 0000 0072 4700 0000 e300  )...r*...rG.....
+000018a0: 0000 7322 0000 0000 0204 0104 0408 0114  ..s"............
+000018b0: 0218 020a 0108 0108 030c 0212 0104 0512  ................
+000018c0: 010e 010e 0116 020e 027a 2a48 616d 696c  .........z*Hamil
+000018d0: 746f 6e69 616e 4d6f 6e74 6543 6172 6c6f  tonianMonteCarlo
+000018e0: 5361 6d70 6c65 722e 7265 7475 726e 5f73  Sampler.return_s
+000018f0: 616d 706c 6529 0872 5300 0000 7254 0000  ample).rS...rT..
+00001900: 0072 5500 0000 7256 0000 0072 2500 0000  .rU...rV...r%...
+00001910: 7267 0000 0072 4f00 0000 7247 0000 0072  rg...rO...rG...r
+00001920: 2900 0000 7229 0000 0072 2900 0000 722a  )...r)...r)...r*
+00001930: 0000 0072 6500 0000 cc00 0000 730a 0000  ...re.......s...
+00001940: 0008 0204 0404 0104 0208 0e72 6500 0000  ...........re...
+00001950: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001960: 0002 0000 0040 0000 0073 4400 0000 6500  .....@...sD...e.
+00001970: 5a01 6400 5a02 6401 5a03 6402 5a04 6403  Z.d.Z.d.Z.d.Z.d.
+00001980: 5a05 6403 5a06 6404 6405 8400 5a07 6406  Z.d.Z.d.d...Z.d.
+00001990: 6407 8400 5a08 6408 6409 8400 5a09 640a  d...Z.d.d...Z.d.
+000019a0: 640b 8400 5a0a 640c 640d 8400 5a0b 640e  d...Z.d.d...Z.d.
+000019b0: 5300 290f da0c 536c 6963 6553 616d 706c  S.)...SliceSampl
+000019c0: 6572 7a68 0a20 2020 2054 6865 2045 6e73  erzh.    The Ens
+000019d0: 656d 626c 6520 536c 6963 6520 7361 6d70  emble Slice samp
+000019e0: 6c65 7220 6672 6f6d 204b 6172 616d 616e  ler from Karaman
+000019f0: 6973 2026 2042 6575 746c 6572 0a20 2020  is & Beutler.   
+00001a00: 2068 7474 7073 3a2f 2f61 7278 6976 2e6f   https://arxiv.o
+00001a10: 7267 2f70 6466 2f32 3030 322e 3036 3231  rg/pdf/2002.0621
+00001a20: 3276 312e 7064 660a 2020 2020 722d 0000  2v1.pdf.    r-..
+00001a30: 0069 e803 0000 6301 0000 0000 0000 0000  .i....c.........
+00001a40: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
+00001a50: 3a00 0000 7400 6401 7c00 6a01 8302 7d01  :...t.d.|.j...}.
+00001a60: 7400 6401 7c00 6a02 8302 7d02 7c01 7c01  t.d.|.j...}.|.|.
+00001a70: 7c02 1700 1b00 7d03 7c00 0400 6a03 6402  |.....}.|...j.d.
+00001a80: 7c03 1400 3900 0200 5f03 6403 5300 2904  |...9..._.d.S.).
+00001a90: 7a97 0a20 2020 2020 2020 2061 6461 7074  z..        adapt
+00001aa0: 7320 7468 6520 6c65 6e67 7468 2073 6361  s the length sca
+00001ab0: 6c65 206f 6620 7468 6520 6578 7061 6e73  le of the expans
+00001ac0: 696f 6e2f 636f 6e74 7261 6374 696f 6e0a  ion/contraction.
+00001ad0: 2020 2020 2020 2020 666f 6c6c 6f77 696e          followin
+00001ae0: 6720 7468 6520 7275 6c65 2069 6e20 2852  g the rule in (R
+00001af0: 6f62 6269 6e73 2061 6e64 204d 6f6e 726f  obbins and Monro
+00001b00: 2c20 3139 3531 2920 6f66 2054 6962 6269  , 1951) of Tibbi
+00001b10: 7473 2065 7420 616c 2e20 2832 3031 3429  ts et al. (2014)
+00001b20: 0a20 2020 2020 2020 2072 0500 0000 e902  .        r......
+00001b30: 0000 004e 2904 722f 0000 00da 024e 65da  ...N).r/.....Ne.
+00001b40: 024e 63da 026d 7529 0472 2800 0000 726e  .Nc..mu).r(...rn
+00001b50: 0000 0072 6f00 0000 da05 7261 7469 6f72  ...ro.....ratior
+00001b60: 2900 0000 7229 0000 0072 2a00 0000 da12  )...r)...r*.....
+00001b70: 6164 6170 745f 6c65 6e67 7468 5f73 6361  adapt_length_sca
+00001b80: 6c65 0f01 0000 7308 0000 0000 050c 010c  le....s.........
+00001b90: 010c 017a 1f53 6c69 6365 5361 6d70 6c65  ...z.SliceSample
+00001ba0: 722e 6164 6170 745f 6c65 6e67 7468 5f73  r.adapt_length_s
+00001bb0: 6361 6c65 6301 0000 0000 0000 0000 0000  calec...........
+00001bc0: 0001 0000 0002 0000 0043 0000 0073 2a00  .........C...s*.
+00001bd0: 0000 7c00 6a00 a001 a100 0b00 7c00 5f02  ..|.j.......|._.
+00001be0: 7c00 6a02 6401 1700 7c00 5f03 6402 7c00  |.j.d...|._.d.|.
+00001bf0: 5f04 6402 7c00 5f05 6403 5300 2904 7a4a  _.d.|._.d.S.).zJ
+00001c00: 0a20 2020 2020 2020 2072 6573 6574 7320  .        resets 
+00001c10: 7468 6520 626f 756e 6461 7269 6573 2061  the boundaries a
+00001c20: 6e64 2063 6f75 6e74 730a 2020 2020 2020  nd counts.      
+00001c30: 2020 666f 7220 7468 6520 736c 6963 696e    for the slicin
+00001c40: 670a 2020 2020 2020 2020 722d 0000 0072  g.        r-...r
+00001c50: 1000 0000 4e29 0672 1700 0000 7215 0000  ....N).r....r...
+00001c60: 00da 014c da01 5272 6e00 0000 726f 0000  ...L..Rrn...ro..
+00001c70: 00a9 0172 2800 0000 7229 0000 0072 2900  ...r(...r)...r).
+00001c80: 0000 722a 0000 00da 1072 6573 6574 5f62  ..r*.....reset_b
+00001c90: 6f75 6e64 6172 6965 7319 0100 0073 0800  oundaries....s..
+00001ca0: 0000 0005 0e01 0c01 0601 7a1d 536c 6963  ..........z.Slic
+00001cb0: 6553 616d 706c 6572 2e72 6573 6574 5f62  eSampler.reset_b
+00001cc0: 6f75 6e64 6172 6965 7363 0100 0000 0000  oundariesc......
+00001cd0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00001ce0: 0000 731c 0000 007c 006a 0064 0118 007c  ..s....|.j.d...|
+00001cf0: 005f 007c 006a 0164 0217 007c 005f 0164  ._.|.j.d...|._.d
+00001d00: 0353 0029 047a 4b0a 2020 2020 2020 2020  .S.).zK.        
+00001d10: 696e 6372 6561 7365 2074 6865 206c 6566  increase the lef
+00001d20: 7420 626f 756e 6461 7279 2061 6e64 2063  t boundary and c
+00001d30: 6f75 6e74 730a 2020 2020 2020 2020 6279  ounts.        by
+00001d40: 206f 6e65 2075 6e69 740a 2020 2020 2020   one unit.      
+00001d50: 2020 722d 0000 0072 0500 0000 4e29 0272    r-...r....N).r
+00001d60: 7300 0000 726e 0000 0072 7500 0000 7229  s...rn...ru...r)
+00001d70: 0000 0072 2900 0000 722a 0000 00da 1669  ...r)...r*.....i
+00001d80: 6e63 7265 6173 655f 6c65 6674 5f62 6f75  ncrease_left_bou
+00001d90: 6e64 6172 7923 0100 0073 0400 0000 0005  ndary#...s......
+00001da0: 0c01 7a23 536c 6963 6553 616d 706c 6572  ..z#SliceSampler
+00001db0: 2e69 6e63 7265 6173 655f 6c65 6674 5f62  .increase_left_b
+00001dc0: 6f75 6e64 6172 7963 0100 0000 0000 0000  oundaryc........
+00001dd0: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00001de0: 731c 0000 007c 006a 0064 0117 007c 005f  s....|.j.d...|._
+00001df0: 007c 006a 0164 0217 007c 005f 0164 0353  .|.j.d...|._.d.S
+00001e00: 0029 047a 4c0a 2020 2020 2020 2020 696e  .).zL.        in
+00001e10: 6372 6561 7365 2074 6865 2072 6967 6874  crease the right
+00001e20: 2062 6f75 6e64 6172 7920 616e 6420 636f   boundary and co
+00001e30: 756e 7473 0a20 2020 2020 2020 2062 7920  unts.        by 
+00001e40: 6f6e 6520 756e 6974 0a20 2020 2020 2020  one unit.       
+00001e50: 2072 2d00 0000 7205 0000 004e 2902 7274   r-...r....N).rt
+00001e60: 0000 0072 6e00 0000 7275 0000 0072 2900  ...rn...ru...r).
+00001e70: 0000 7229 0000 0072 2a00 0000 da17 696e  ..r)...r*.....in
+00001e80: 6372 6561 7365 5f72 6967 6874 5f62 6f75  crease_right_bou
+00001e90: 6e64 6172 792b 0100 0073 0400 0000 0005  ndary+...s......
+00001ea0: 0c01 7a24 536c 6963 6553 616d 706c 6572  ..z$SliceSampler
+00001eb0: 2e69 6e63 7265 6173 655f 7269 6768 745f  .increase_right_
+00001ec0: 626f 756e 6461 7279 6303 0000 0000 0000  boundaryc.......
+00001ed0: 0000 0000 000f 0000 0005 0000 0043 0000  .............C..
+00001ee0: 0073 7402 0000 6401 7d03 6401 7d04 7c00  .st...d.}.d.}.|.
+00001ef0: a000 a100 0100 7c04 6402 3700 7d04 7c00  ......|.d.7.}.|.
+00001f00: 6a01 6a02 7c00 6a03 6403 8d01 7d05 7404  j.j.|.j.d...}.t.
+00001f10: 7c05 7405 6a06 8302 7344 7405 6a06 7c01  |.t.j...sDt.j.|.
+00001f20: 6a07 7c05 6404 8d02 7d05 7c02 7d06 7c01  j.|.d...}.|.}.|.
+00001f30: 6a08 7c00 6a09 a00a a100 1800 7d07 740b  j.|.j.......}.t.
+00001f40: a00c 7c00 6a0d 7c00 6a09 a00e a100 1400  ..|.j.|.j.......
+00001f50: a101 7d08 7c00 6a0d 6402 1800 7c08 1800  ..}.|.j.d...|...
+00001f60: 7d09 7c08 6401 6b04 72c8 7c05 7c00 6a0f  }.|.d.k.r.|.|.j.
+00001f70: 1400 7c01 1700 7d0a 7c00 6a10 a011 7c0a  ..|...}.|.j...|.
+00001f80: a101 72c8 7c07 7c00 6a10 a012 7c0a a101  ..r.|.|.j...|...
+00001f90: 6b04 72b2 71c8 71c6 7c00 a013 a100 0100  k.r.q.q.|.......
+00001fa0: 7c08 6402 3800 7d08 717c 71c8 717c 7c09  |.d.8.}.q|q.q||.
+00001fb0: 6401 6b04 9001 721e 7c05 7c00 6a14 1400  d.k...r.|.|.j...
+00001fc0: 7c01 1700 7d0b 7c00 6a10 a011 7c0b a101  |...}.|.j...|...
+00001fd0: 9001 721e 7c07 7c00 6a10 a012 7c0b a101  ..r.|.|.j...|...
+00001fe0: 6b04 9001 7206 9001 711e 6e10 7c00 a015  k...r...q.n.|...
+00001ff0: a100 0100 7c09 6402 3800 7d09 71c8 9001  ....|.d.8.}.q...
+00002000: 711e 71c8 6401 7d0c 7c0c 7c00 6a16 6b00  q.q.d.}.|.|.j.k.
+00002010: 9001 72da 7c00 6a09 a017 7c00 6a0f 7c00  ..r.|.j...|.j.|.
+00002020: 6a14 a102 7d0d 7c05 7c0d 1400 7c01 1700  j...}.|.|...|...
+00002030: 7d0e 7c00 6a10 a012 7c0e a101 7c0e 5f08  }.|.j...|...|._.
+00002040: 7c0e 6a08 7c07 6b04 9001 7294 7c00 6a10  |.j.|.k...r.|.j.
+00002050: a018 7c0e a101 7c0e 5f19 7c0e 6a19 7c06  ..|...|._.|.j.|.
+00002060: 6b04 9001 7294 7c0e a01a a100 7d01 7c03  k...r.|.....}.|.
+00002070: 6402 3700 7d03 9001 71da 7c0d 6405 6b00  d.7.}...q.|.d.k.
+00002080: 9001 72b2 7c0d 7c00 5f0f 7c00 6a1b 6402  ..r.|.|._.|.j.d.
+00002090: 1700 7c00 5f1b 6e1c 7c0d 6405 6b04 9001  ..|._.n.|.d.k...
+000020a0: 72ce 7c0d 7c00 5f14 7c00 6a1b 6402 1700  r.|.|._.|.j.d...
+000020b0: 7c00 5f1b 7c0c 6402 3700 7d0c 9001 7122  |._.|.d.7.}...q"
+000020c0: 7c04 7c00 6a1c 6b05 9001 72f4 7c03 6401  |.|.j.k...r.|.d.
+000020d0: 6b04 9001 72f4 9002 7112 7c04 7c00 6a1d  k...r...q.|.|.j.
+000020e0: 6b05 9002 7204 9002 7112 7c00 6a1e a01f  k...r...q.|.j...
+000020f0: 7c01 a101 0100 7108 7420 7c03 8301 7420  |.....q.t |...t 
+00002100: 7c04 8301 1b00 7c00 5f21 7c00 0400 6a22  |.....|._!|...j"
+00002110: 7c03 3700 0200 5f22 7c00 0400 6a23 7c04  |.7..._"|...j#|.
+00002120: 3700 0200 5f23 7420 7c00 6a22 8301 7420  7..._#t |.j"..t 
+00002130: 7c00 6a23 8301 1b00 7c00 5f24 7c02 740b  |.j#....|._$|.t.
+00002140: 6a25 0b00 6b02 9002 726c 7c00 a026 a100  j%..k...rl|..&..
+00002150: 0100 7c04 7c01 6602 5300 2906 4e72 0100  ..|.|.f.S.).Nr..
+00002160: 0000 7205 0000 0029 0172 7000 0000 2901  ..r....).rp...).
+00002170: da01 6472 1000 0000 2927 7276 0000 0072  ..dr....)'rv...r
+00002180: 0900 0000 5a0d 6765 745f 6469 7265 6374  ....Z.get_direct
+00002190: 696f 6e72 7000 0000 724e 0000 0072 0600  ionrp...rN...r..
+000021a0: 0000 da09 4c69 7665 506f 696e 7472 4000  ....LivePointr@.
+000021b0: 0000 725b 0000 0072 1700 0000 da0b 6578  ..r[...r......ex
+000021c0: 706f 6e65 6e74 6961 6c72 1400 0000 da05  ponentialr......
+000021d0: 666c 6f6f 72da 0d6d 6178 5f73 7465 7073  floor..max_steps
+000021e0: 5f6f 7574 7215 0000 0072 7300 0000 720f  _outr....rs...r.
+000021f0: 0000 00da 0969 6e5f 626f 756e 6473 7258  .....in_boundsrX
+00002200: 0000 0072 7700 0000 7274 0000 0072 7800  ...rw...rt...rx.
+00002210: 0000 da0a 6d61 785f 736c 6963 6573 da07  ....max_slices..
+00002220: 756e 6966 6f72 6d72 5d00 0000 725e 0000  uniformr]...r^..
+00002230: 0072 5a00 0000 726f 0000 0072 1d00 0000  .rZ...ro...r....
+00002240: 7218 0000 0072 2700 0000 725f 0000 0072  r....r'...r_...r
+00002250: 1e00 0000 7222 0000 0072 2300 0000 7224  ....r"...r#...r$
+00002260: 0000 0072 2100 0000 da03 696e 6672 7200  ...r!.....infrr.
+00002270: 0000 290f 7228 0000 0072 6000 0000 7249  ..).r(...r`...rI
+00002280: 0000 0072 6200 0000 7261 0000 005a 1064  ...rb...ra...Z.d
+00002290: 6972 6563 7469 6f6e 5f76 6563 746f 72da  irection_vector.
+000022a0: 0159 5a02 5970 da01 4ada 014b 5a0e 7061  .YZ.Yp..J..KZ.pa
+000022b0: 7261 6d65 7465 725f 6c65 6674 5a0f 7061  rameter_leftZ.pa
+000022c0: 7261 6d65 7465 725f 7269 6768 74da 0573  rameter_right..s
+000022d0: 6c69 6365 5a06 5870 7269 6d65 7263 0000  liceZ.Xprimerc..
+000022e0: 0072 2900 0000 7229 0000 0072 2a00 0000  .r)...r)...r*...
+000022f0: 7247 0000 0033 0100 0073 7200 0000 0002  rG...3...sr.....
+00002300: 0401 0404 0801 0802 1001 0c01 1002 0401  ................
+00002310: 1001 1601 0e03 0802 0e02 0c01 1001 0402  ................
+00002320: 0801 0a03 0404 0a02 0e02 0e02 1201 0602  ................
+00002330: 0801 0a03 0603 0401 0c02 1201 0c01 0e02  ................
+00002340: 0c02 0e01 0c01 0801 0801 0402 0a01 0601  ................
+00002350: 0e01 0a01 0601 0c02 0c02 1601 0402 0c01  ................
+00002360: 0402 0e01 1201 0e01 0e01 1602 0e01 0802  ................
+00002370: 7a1a 536c 6963 6553 616d 706c 6572 2e72  z.SliceSampler.r
+00002380: 6574 7572 6e5f 7361 6d70 6c65 4e29 0c72  eturn_sampleN).r
+00002390: 5300 0000 7254 0000 0072 5500 0000 7256  S...rT...rU...rV
+000023a0: 0000 0072 7000 0000 727d 0000 0072 7f00  ...rp...r}...r..
+000023b0: 0000 7272 0000 0072 7600 0000 7277 0000  ..rr...rv...rw..
+000023c0: 0072 7800 0000 7247 0000 0072 2900 0000  .rx...rG...r)...
+000023d0: 7229 0000 0072 2900 0000 722a 0000 0072  r)...r)...r*...r
+000023e0: 6c00 0000 0501 0000 7312 0000 0008 0204  l.......s.......
+000023f0: 0404 0104 0104 0208 0a08 0a08 0808 0872  ...............r
+00002400: 6c00 0000 6300 0000 0000 0000 0000 0000  l...c...........
+00002410: 0000 0000 0002 0000 0040 0000 0073 3000  .........@...s0.
+00002420: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
+00002430: 5a04 6402 5a05 6403 6404 8400 5a06 6405  Z.d.Z.d.d...Z.d.
+00002440: 6406 8400 5a07 6407 6408 8400 5a08 6409  d...Z.d.d...Z.d.
+00002450: 5300 290a da0d 5361 6d70 6c65 7273 4379  S.)...SamplersCy
+00002460: 636c 657a d70a 2020 2020 4120 7361 6d70  clez..    A samp
+00002470: 6c65 7220 7468 6174 2063 7963 6c65 7320  ler that cycles 
+00002480: 7468 726f 7567 6820 6120 6c69 7374 206f  through a list o
+00002490: 660a 2020 2020 7361 6d70 6c65 7273 2e0a  f.    samplers..
+000024a0: 0a20 2020 2049 6e69 7469 616c 6973 6174  .    Initialisat
+000024b0: 696f 6e20 6172 6775 6d65 6e74 733a 0a0a  ion arguments:..
+000024c0: 2020 2020 7361 6d70 6c65 7273 203a 2041      samplers : A
+000024d0: 206c 6973 7420 6f66 2073 616d 706c 6572   list of sampler
+000024e0: 730a 0a20 2020 204f 7074 696f 6e61 6c20  s..    Optional 
+000024f0: 6172 6775 6d65 6e74 733a 0a20 2020 2063  arguments:.    c
+00002500: 7963 6c65 6c65 6e67 7468 203a 206c 656e  yclelength : len
+00002510: 6774 6820 6f66 2074 6865 2073 616d 706c  gth of the sampl
+00002520: 6572 2063 7963 6c65 2e20 4465 6661 756c  er cycle. Defaul
+00002530: 743a 2031 3030 0a0a 2020 2020 7201 0000  t: 100..    r...
+00002540: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
+00002550: 0000 0200 0000 4f00 0000 7316 0000 007c  ......O...s....|
+00002560: 017c 005f 0074 017c 006a 0083 017c 005f  .|._.t.|.j...|._
+00002570: 0264 0053 0029 014e 2903 da08 7361 6d70  .d.S.).N)...samp
+00002580: 6c65 7273 723f 0000 00da 014e 2904 7228  lersr?.....N).r(
+00002590: 0000 0072 8700 0000 da04 6172 6773 da06  ...r......args..
+000025a0: 6b77 6172 6773 7229 0000 0072 2900 0000  kwargsr)...r)...
+000025b0: 722a 0000 0072 2b00 0000 a001 0000 7304  r*...r+.......s.
+000025c0: 0000 0000 0106 017a 1653 616d 706c 6572  .......z.Sampler
+000025d0: 7343 7963 6c65 2e5f 5f69 6e69 745f 5f63  sCycle.__init__c
+000025e0: 0300 0000 0000 0000 0000 0000 0900 0000  ................
+000025f0: 0400 0000 4b00 0000 7346 0000 007c 006a  ....K...sF...|.j
+00002600: 0064 0117 007c 006a 0116 007c 005f 007c  .d...|.j...|._.|
+00002610: 006a 027c 006a 0019 007d 047c 046a 037c  .j.|.j...}.|.j.|
+00002620: 017c 0266 0269 007c 03a4 018e 015c 047d  .|.f.i.|.....\.}
+00002630: 057d 067d 077d 087c 057c 067c 077c 0866  .}.}.}.|.|.|.|.f
+00002640: 0453 0029 024e 7205 0000 0029 04da 0369  .S.).Nr....)...i
+00002650: 6478 7288 0000 0072 8700 0000 724a 0000  dxr....r....rJ..
+00002660: 0029 0972 2800 0000 7248 0000 0072 4900  .).r(...rH...rI.
+00002670: 0000 728a 0000 0072 5200 0000 7221 0000  ..r....rR...r!..
+00002680: 0072 2200 0000 721d 0000 00da 036e 6577  .r"...r......new
+00002690: 7229 0000 0072 2900 0000 722a 0000 0072  r)...r)...r*...r
+000026a0: 4a00 0000 a401 0000 7308 0000 0000 0212  J.......s.......
+000026b0: 010c 011c 017a 1c53 616d 706c 6572 7343  .....z.SamplersC
+000026c0: 7963 6c65 2e70 726f 6475 6365 5f73 616d  ycle.produce_sam
+000026d0: 706c 6563 0200 0000 0000 0000 0000 0000  plec............
+000026e0: 0400 0000 0500 0000 4300 0000 7332 0000  ........C...s2..
+000026f0: 007c 006a 0044 005d 267d 027c 026a 016a  .|.j.D.]&}.|.j.j
+00002700: 0244 005d 187d 0374 037c 0374 0483 0272  .D.].}.t.|.t...r
+00002710: 127c 03a0 057c 01a1 0101 0071 1271 0664  .|...|.....q.q.d
+00002720: 0153 0029 027a 670a 2020 2020 2020 2020  .S.).zg.        
+00002730: 5570 6461 7465 7320 7468 6520 656e 7365  Updates the ense
+00002740: 6d62 6c65 2073 7461 7469 7374 6963 730a  mble statistics.
+00002750: 2020 2020 2020 2020 6279 2063 616c 6c69          by calli
+00002760: 6e67 2069 7420 6f6e 2065 6163 6820 3a6f  ng it on each :o
+00002770: 626a 3a60 456e 7365 6d62 6c65 5072 6f70  bj:`EnsembleProp
+00002780: 6f73 616c 600a 2020 2020 2020 2020 4e29  osal`.        N)
+00002790: 0672 8700 0000 7209 0000 0072 4d00 0000  .r....r....rM...
+000027a0: 724e 0000 0072 0800 0000 724f 0000 0029  rN...r....rO...)
+000027b0: 0472 2800 0000 7251 0000 0072 4500 0000  .r(...rQ...rE...
+000027c0: 7252 0000 0072 2900 0000 7229 0000 0072  rR...r)...r)...r
+000027d0: 2a00 0000 724f 0000 00ab 0100 0073 0800  *...rO.......s..
+000027e0: 0000 0005 0a01 0c01 0a01 7a1a 5361 6d70  ..........z.Samp
+000027f0: 6c65 7273 4379 636c 652e 7365 745f 656e  lersCycle.set_en
+00002800: 7365 6d62 6c65 4e29 0972 5300 0000 7254  sembleN).rS...rT
+00002810: 0000 0072 5500 0000 7256 0000 0072 8b00  ...rU...rV...r..
+00002820: 0000 7288 0000 0072 2b00 0000 724a 0000  ..r....r+...rJ..
+00002830: 0072 4f00 0000 7229 0000 0072 2900 0000  .rO...r)...r)...
+00002840: 7229 0000 0072 2a00 0000 7286 0000 0090  r)...r*...r.....
+00002850: 0100 0073 0c00 0000 0802 040c 0401 0401  ...s............
+00002860: 0804 0807 7286 0000 0029 26da 0a5f 5f66  ....r....)&..__f
+00002870: 7574 7572 655f 5f72 0200 0000 da03 7379  uture__r......sy
+00002880: 7372 4300 0000 721a 0000 00da 056e 756d  srC...r......num
+00002890: 7079 7214 0000 00da 046d 6174 6872 0300  pyr......mathr..
+000028a0: 0000 da0b 636f 6c6c 6563 7469 6f6e 7372  ....collectionsr
+000028b0: 0400 0000 da00 7206 0000 0072 0900 0000  ......r....r....
+000028c0: 7207 0000 0072 0800 0000 da16 6e75 6d70  r....r......nump
+000028d0: 792e 6c69 622e 7265 6366 756e 6374 696f  y.lib.recfunctio
+000028e0: 6e73 da03 6c69 62da 0c72 6563 6675 6e63  ns..lib..recfunc
+000028f0: 7469 6f6e 73da 0372 666e 723c 0000 00da  tions..rfnr<....
+00002900: 086e 6573 7432 706f 7372 0a00 0000 720b  .nest2posr....r.
+00002910: 0000 0072 4b00 0000 da02 6763 da06 7069  ...rK.....gc..pi
+00002920: 636b 6c65 5a11 5f5f 6368 6563 6b70 6f69  ckleZ.__checkpoi
+00002930: 6e74 5f66 6c61 67da 066f 626a 6563 7472  nt_flag..objectr
+00002940: 0c00 0000 da06 7265 6d6f 7465 7257 0000  ......remoterW..
+00002950: 005a 0f66 6967 6172 6f5f 6772 6164 6965  .Z.figaro_gradie
+00002960: 6e74 7264 0000 00da 0570 7269 6e74 7265  ntrd.....printre
+00002970: 0000 0072 6c00 0000 7286 0000 0072 2900  ...rl...r....r).
+00002980: 0000 7229 0000 0072 2900 0000 722a 0000  ..r)...r)...r*..
+00002990: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000029a0: 3e00 0000 0c01 0801 0801 0801 0801 0c01  >...............
+000029b0: 0c02 0c01 1001 0c01 1201 0801 1001 0801  ................
+000029c0: 0802 0801 0403 107f 0009 0401 1229 0201  .............)..
+000029d0: 1001 0601 0e01 0401 1238 0401 127f 000b  .........8......
+000029e0: 0401                                     ..
```

### Comparing `raynest-1.0.1/raynest/__pycache__/utils.cpython-39.pyc` & `raynest-1.0.2/raynest/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/figaro_gradient.py` & `raynest-1.0.2/raynest/figaro_gradient.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-from figaro.mixture import DPGMM
-from figaro.likelihood import log_norm
+try:
+    from figaro.mixture import DPGMM
+    from figaro.likelihood import log_norm
+except:
+    print("FIGARO not available! Hamiltonian Monte Carlo sampling not supported!")
+    pass
+
 import numpy as np
 from tqdm import tqdm
 from scipy.stats import multivariate_normal as mn
 
 class ADPGMM(DPGMM):
     def __init__(self, *args, **kwargs):
         super(ADPGMM, self).__init__(*args, **kwargs)
```

### Comparing `raynest-1.0.1/raynest/model.py` & `raynest-1.0.2/raynest/model.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/nest2pos.py` & `raynest-1.0.2/raynest/nest2pos.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/parameter.c` & `raynest-1.0.2/raynest/parameter.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 /* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h",
-            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/core/include/numpy/npy_math.h",
+            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-O3",
             "-ffast-math",
             "-mavx2",
             "-ftree-vectorize"
         ],
         "include_dirs": [
             "raynest",
-            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/core/include"
+            "/private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m"
         ],
         "name": "raynest.parameter",
         "sources": [
             "raynest/parameter.pyx"
@@ -1022,195 +1022,195 @@
 static const char *__pyx_f[] = {
   "raynest/parameter.pyx",
   "raynest/parameter.pxd",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":715
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":717
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":719
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":724
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1238,42 +1238,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_7raynest_9parameter_LivePoint;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":728
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":732
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -5433,15 +5433,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5450,29 +5450,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5483,15 +5483,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5500,29 +5500,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5533,15 +5533,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5550,29 +5550,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5583,15 +5583,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5600,29 +5600,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5633,15 +5633,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5650,29 +5650,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5683,212 +5683,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":749
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":750
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":753
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":928
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":932
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":934
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":936
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":940
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5904,15 +5904,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5920,53 +5920,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":941
+      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":943
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":944
+      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
@@ -5974,30 +5974,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6012,15 +6012,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":946
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6036,15 +6036,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6052,53 +6052,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":947
+      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":949
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":950
+      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
@@ -6106,30 +6106,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6144,15 +6144,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":952
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6168,15 +6168,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6184,53 +6184,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":953
+      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":955
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":956
+      /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
@@ -6238,30 +6238,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6276,176 +6276,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":966
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":978
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":981
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":993
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":996
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+/* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6885,26 +6885,26 @@
  *         for n in self.names:
  *             x[n] = self[n]
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_int_1); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 950, __pyx_L1_error)
@@ -7454,15 +7454,15 @@
  * # cython: linetrace=False
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-6ey0uypn/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../private/var/folders/84/glnt1smx4x19w5vffjltdlpr0000gn/T/build-env-e0znm81r/lib/python3.9/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `raynest-1.0.1/raynest/parameter.pyx` & `raynest-1.0.2/raynest/parameter.pyx`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/plot.py` & `raynest-1.0.2/raynest/plot.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/proposal.py` & `raynest-1.0.2/raynest/proposal.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/raynest.py` & `raynest-1.0.2/raynest/raynest.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                  object_store_memory=10**9
                  ):
 
         self.verbose   = verbose
         self.logger    = logging.getLogger('raynest.raynest.raynest')
         self.nsamplers = nensemble+nhamiltonian+nslice
         self.nnest     = nnest
-
+        
         assert self.nsamplers > 0, "no sampler processes requested!"
         import psutil
         self.max_threads = psutil.cpu_count()
 
         if self.nsamplers%self.nnest != 0:
             self.logger.warning("Error! Number of samplers not balanced")
             self.logger.warning("to the number of nested samplers! Exiting.")
@@ -132,26 +132,23 @@
         if self.nthreads > self.max_threads:
             self.logger.warning("More cpus than available are being requested!")
             self.logger.warning("This might result in excessive overhead")
 
         self.ns_pool = []
         self.pool    = []
 
-        if not ray.is_initialized():
-            self.existing_cluster = False
-            ray.init(num_cpus=self.nthreads,
-                     ignore_reinit_error=True,
-                     object_store_memory=object_store_memory)
-        else:
+        try:
+            ray.init(address='auto')
             self.existing_cluster = True
-            ray.init(address='auto',
-                     num_cpus=self.nthreads,
+        except:
+            ray.init(num_cpus=self.nthreads,
                      ignore_reinit_error=True,
                      object_store_memory=object_store_memory)
-
+            self.existing_cluster = False
+                     
         assert ray.is_initialized() == True
         output = os.path.join(output, '')
         checkpoint_folder = os.path.join(output,'checkpoints')
         os.makedirs(output, exist_ok=True)
         os.makedirs(checkpoint_folder, exist_ok=True)
         
         # Import placement group APIs.
```

### Comparing `raynest-1.0.1/raynest/sampler.py` & `raynest-1.0.2/raynest/sampler.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest/utils.py` & `raynest-1.0.2/raynest/utils.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/raynest.egg-info/PKG-INFO` & `raynest-1.0.2/raynest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raynest
-Version: 1.0.1
+Version: 1.0.2
 Summary: raynest: Parallel nested sampling based on ray
 Home-page: https://github.com/wdpozzo/raynest
 Author: Walter Del Pozzo, John Veitch
 Author-email: walter.delpozzo@ligo.org, john.veitch@ligo.org
 License: MIT
 Keywords: nested sampling bayesian inference
 Classifier: Development Status :: 4 - Beta
```

### Comparing `raynest-1.0.1/raynest.egg-info/SOURCES.txt` & `raynest-1.0.2/raynest.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 examples/test_50d.py
 raynest/NestedSampling.py
 raynest/__init__.py
 raynest/figaro_gradient.py
 raynest/model.py
 raynest/nest2pos.py
 raynest/parameter.c
-raynest/parameter.cpython-39-darwin.so
 raynest/parameter.pxd
 raynest/parameter.pyx
 raynest/plot.py
 raynest/proposal.py
 raynest/raynest.py
 raynest/sampler.py
 raynest/utils.py
```

### Comparing `raynest-1.0.1/setup.py` & `raynest-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 with open("requirements.txt") as requires_file:
     requirements = requires_file.read().split("\n")
 
 setup(
         name='raynest',
-        version='1.0.1',
+        version='1.0.2',
         description='raynest: Parallel nested sampling based on ray',
         long_description=long_description,
         author='Walter Del Pozzo, John Veitch',
         author_email='walter.delpozzo@ligo.org, john.veitch@ligo.org',
         url='https://github.com/wdpozzo/raynest',
         license='MIT',
         python_requires='>=3.6',
```

### Comparing `raynest-1.0.1/tests/test_1d.py` & `raynest-1.0.2/tests/test_1d.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/tests/test_2d.py` & `raynest-1.0.2/tests/test_2d.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/tests/test_2d_hmc.py` & `raynest-1.0.2/tests/test_2d_hmc.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/tests/test_2d_slice.py` & `raynest-1.0.2/tests/test_2d_slice.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/tests/test_gaussian.py` & `raynest-1.0.2/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/tests/test_half_gaussian.py` & `raynest-1.0.2/tests/test_half_gaussian.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/tests/test_ring.py` & `raynest-1.0.2/tests/test_ring.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/tests/test_ring_slice.py` & `raynest-1.0.2/tests/test_ring_slice.py`

 * *Files identical despite different names*

### Comparing `raynest-1.0.1/tests/test_verbosity.py` & `raynest-1.0.2/tests/test_verbosity.py`

 * *Files identical despite different names*

