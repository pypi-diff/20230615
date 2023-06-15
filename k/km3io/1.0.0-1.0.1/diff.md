# Comparing `tmp/km3io-1.0.0.tar.gz` & `tmp/km3io-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "km3io-1.0.0.tar", last modified: Mon Feb 27 08:16:11 2023, max compression
+gzip compressed data, was "km3io-1.0.1.tar", last modified: Thu Jun 15 11:21:27 2023, max compression
```

## Comparing `km3io-1.0.0.tar` & `km3io-1.0.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.226608 km3io-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      305 2022-09-02 03:05:58.000000 km3io-1.0.0/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      439 2022-09-02 03:05:58.000000 km3io-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4757 2022-10-28 11:23:28.000000 km3io-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     8911 2023-02-27 08:11:33.000000 km3io-1.0.0/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6676 2022-10-28 11:23:28.000000 km3io-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-10-04 10:03:09.000000 km3io-1.0.0/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1077 2022-09-02 03:05:58.000000 km3io-1.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      184 2022-12-01 14:15:08.000000 km3io-1.0.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1018 2022-09-02 03:05:58.000000 km3io-1.0.0/Makefile
--rw-r--r--   0 root         (0) root         (0)    16219 2023-02-27 08:16:11.226608 km3io-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12439 2022-11-30 14:26:05.000000 km3io-1.0.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2264 2022-09-30 03:07:59.000000 km3io-1.0.0/codemeta.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.222608 km3io-1.0.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)      634 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.222608 km3io-1.0.0/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)       55 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/_static/default.css
--rw-rw-rw-   0 root         (0) root         (0)    24268 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/_static/default_gallery_thumbnail.png
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2912 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/contribute.rst
--rw-rw-rw-   0 root         (0) root         (0)       65 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)      625 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.218608 km3io-1.0.0/doc/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.222608 km3io-1.0.0/doc/modules/generated/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 03:05:58.000000 km3io-1.0.0/doc/modules/generated/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.222608 km3io-1.0.0/examples/
--rw-rw-rw-   0 root         (0) root         (0)      111 2022-09-02 03:05:58.000000 km3io-1.0.0/examples/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3260 2022-09-02 03:05:58.000000 km3io-1.0.0/examples/plot_offline_events.py
--rw-rw-rw-   0 root         (0) root         (0)     2740 2022-09-02 03:05:58.000000 km3io-1.0.0/examples/plot_offline_tracks.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2022-09-02 03:05:58.000000 km3io-1.0.0/examples/plot_offline_usr.py
--rw-rw-rw-   0 root         (0) root         (0)     2552 2022-09-02 03:05:58.000000 km3io-1.0.0/examples/plot_online_example.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2022-09-02 03:05:58.000000 km3io-1.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-02-27 08:16:11.226608 km3io-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       84 2022-09-02 03:05:58.000000 km3io-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.218608 km3io-1.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.222608 km3io-1.0.0/src/km3io/
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-01-29 03:10:30.000000 km3io-1.0.0/src/km3io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.222608 km3io-1.0.0/src/km3io/_definitions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-02 03:05:58.000000 km3io-1.0.0/src/km3io/_definitions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/applications.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/daqdatatypes.py
--rw-rw-rw-   0 root         (0) root         (0)      850 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/fitparameters.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2022-09-02 03:05:58.000000 km3io-1.0.0/src/km3io/_definitions/mc_header.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/module_status.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/pmt_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1055 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/reconstruction.py
--rw-rw-rw-   0 root         (0) root         (0)     2085 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/root.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/trigger.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/trkmembers.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/w2list_genhen.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/w2list_gseagen.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/w2list_km3buu.py
--rw-rw-rw-   0 root         (0) root         (0)      386 2022-11-07 16:13:39.000000 km3io-1.0.0/src/km3io/_definitions/weightlist.py
--rw-rw-rw-   0 root         (0) root         (0)     4149 2022-09-02 03:05:58.000000 km3io-1.0.0/src/km3io/acoustics.py
--rw-rw-rw-   0 root         (0) root         (0)     2085 2022-09-02 03:05:58.000000 km3io-1.0.0/src/km3io/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)     5440 2022-10-28 11:23:28.000000 km3io-1.0.0/src/km3io/offline.py
--rw-rw-rw-   0 root         (0) root         (0)    15443 2022-09-02 03:05:58.000000 km3io-1.0.0/src/km3io/online.py
--rw-rw-rw-   0 root         (0) root         (0)    14715 2022-09-02 03:05:58.000000 km3io-1.0.0/src/km3io/rootio.py
--rw-rw-rw-   0 root         (0) root         (0)    19286 2022-10-21 03:10:37.000000 km3io-1.0.0/src/km3io/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.222608 km3io-1.0.0/src/km3io/utils/
--rw-rw-rw-   0 root         (0) root         (0)      980 2022-09-02 03:05:58.000000 km3io-1.0.0/src/km3io/utils/kprinttree.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-02-27 08:16:11.000000 km3io-1.0.0/src/km3io/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.222608 km3io-1.0.0/src/km3io.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16219 2023-02-27 08:16:11.000000 km3io-1.0.0/src/km3io.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1705 2023-02-27 08:16:11.000000 km3io-1.0.0/src/km3io.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 08:16:11.000000 km3io-1.0.0/src/km3io.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-02-27 08:16:11.000000 km3io-1.0.0/src/km3io.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      359 2023-02-27 08:16:11.000000 km3io-1.0.0/src/km3io.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-27 08:16:11.000000 km3io-1.0.0/src/km3io.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.222608 km3io-1.0.0/talks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.226608 km3io-1.0.0/talks/images/
--rw-rw-rw-   0 root         (0) root         (0)    46060 2022-09-02 03:05:58.000000 km3io-1.0.0/talks/images/orca-du4.png
--rw-rw-rw-   0 root         (0) root         (0)    70542 2022-09-02 03:05:58.000000 km3io-1.0.0/talks/images/uproot_vs_root.png
--rw-rw-rw-   0 root         (0) root         (0)   102745 2022-09-02 03:05:58.000000 km3io-1.0.0/talks/images/uproot_vs_root_numpy.png
--rw-rw-rw-   0 root         (0) root         (0)    16185 2022-09-02 03:05:58.000000 km3io-1.0.0/talks/premiere.org
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 08:16:11.226608 km3io-1.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1017 2022-09-02 03:05:58.000000 km3io-1.0.0/tests/test_acoustics.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2022-09-02 03:05:58.000000 km3io-1.0.0/tests/test_km3io.py
--rw-rw-rw-   0 root         (0) root         (0)    18868 2022-09-02 03:05:58.000000 km3io-1.0.0/tests/test_offline.py
--rw-rw-rw-   0 root         (0) root         (0)    24172 2022-09-02 03:05:58.000000 km3io-1.0.0/tests/test_online.py
--rw-rw-rw-   0 root         (0) root         (0)    24966 2022-10-21 03:10:37.000000 km3io-1.0.0/tests/test_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.498321 km3io-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-05-02 03:04:08.000000 km3io-1.0.1/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      439 2023-05-02 03:04:08.000000 km3io-1.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4757 2023-05-02 03:04:08.000000 km3io-1.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     8986 2023-06-15 11:21:17.000000 km3io-1.0.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6676 2023-05-02 03:04:08.000000 km3io-1.0.1/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-02 03:04:08.000000 km3io-1.0.1/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-05-02 03:04:08.000000 km3io-1.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-05-02 03:04:08.000000 km3io-1.0.1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1018 2023-05-02 03:04:08.000000 km3io-1.0.1/Makefile
+-rw-r--r--   0 root         (0) root         (0)    17573 2023-06-15 11:21:27.498321 km3io-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    13609 2023-05-02 03:04:08.000000 km3io-1.0.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2384 2023-06-15 11:12:13.000000 km3io-1.0.1/codemeta.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.494321 km3io-1.0.1/doc/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.494321 km3io-1.0.1/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/_static/default.css
+-rw-rw-rw-   0 root         (0) root         (0)    24268 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/_static/default_gallery_thumbnail.png
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2912 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/contribute.rst
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.490321 km3io-1.0.1/doc/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.494321 km3io-1.0.1/doc/modules/generated/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 03:04:08.000000 km3io-1.0.1/doc/modules/generated/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.494321 km3io-1.0.1/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      111 2023-05-02 03:04:08.000000 km3io-1.0.1/examples/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2023-05-02 03:04:08.000000 km3io-1.0.1/examples/plot_offline_events.py
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-05-02 03:04:08.000000 km3io-1.0.1/examples/plot_offline_tracks.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-05-02 03:04:08.000000 km3io-1.0.1/examples/plot_offline_usr.py
+-rw-rw-rw-   0 root         (0) root         (0)     2552 2023-05-02 03:04:08.000000 km3io-1.0.1/examples/plot_online_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-05-02 03:04:08.000000 km3io-1.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2023-06-15 11:21:27.498321 km3io-1.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-05-02 03:04:08.000000 km3io-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.490321 km3io-1.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.494321 km3io-1.0.1/src/km3io/
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.498321 km3io-1.0.1/src/km3io/_definitions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/applications.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/daqdatatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/fitparameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/mc_header.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/module_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/pmt_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/reconstruction.py
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/root.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/trkmembers.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/w2list_genhen.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/w2list_gseagen.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/w2list_km3buu.py
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/_definitions/weightlist.py
+-rw-rw-rw-   0 root         (0) root         (0)     4149 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/acoustics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5440 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/offline.py
+-rw-rw-rw-   0 root         (0) root         (0)    15443 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/online.py
+-rw-rw-rw-   0 root         (0) root         (0)    14715 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/rootio.py
+-rw-rw-rw-   0 root         (0) root         (0)    19286 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.498321 km3io-1.0.1/src/km3io/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-05-02 03:04:08.000000 km3io-1.0.1/src/km3io/utils/kprinttree.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-15 11:21:27.000000 km3io-1.0.1/src/km3io/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.494321 km3io-1.0.1/src/km3io.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17573 2023-06-15 11:21:27.000000 km3io-1.0.1/src/km3io.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-06-15 11:21:27.000000 km3io-1.0.1/src/km3io.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 11:21:27.000000 km3io-1.0.1/src/km3io.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-15 11:21:27.000000 km3io-1.0.1/src/km3io.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-15 11:21:27.000000 km3io-1.0.1/src/km3io.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-15 11:21:27.000000 km3io-1.0.1/src/km3io.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.498321 km3io-1.0.1/talks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.498321 km3io-1.0.1/talks/images/
+-rw-rw-rw-   0 root         (0) root         (0)    46060 2023-05-02 03:04:08.000000 km3io-1.0.1/talks/images/orca-du4.png
+-rw-rw-rw-   0 root         (0) root         (0)    70542 2023-05-02 03:04:08.000000 km3io-1.0.1/talks/images/uproot_vs_root.png
+-rw-rw-rw-   0 root         (0) root         (0)   102745 2023-05-02 03:04:08.000000 km3io-1.0.1/talks/images/uproot_vs_root_numpy.png
+-rw-rw-rw-   0 root         (0) root         (0)    16185 2023-05-02 03:04:08.000000 km3io-1.0.1/talks/premiere.org
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 11:21:27.498321 km3io-1.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2023-05-02 03:04:08.000000 km3io-1.0.1/tests/test_acoustics.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-02 03:04:08.000000 km3io-1.0.1/tests/test_km3io.py
+-rw-rw-rw-   0 root         (0) root         (0)    18868 2023-05-02 03:04:08.000000 km3io-1.0.1/tests/test_offline.py
+-rw-rw-rw-   0 root         (0) root         (0)    24172 2023-05-02 03:04:08.000000 km3io-1.0.1/tests/test_online.py
+-rw-rw-rw-   0 root         (0) root         (0)    24966 2023-05-02 03:04:08.000000 km3io-1.0.1/tests/test_tools.py
```

### Comparing `km3io-1.0.0/.gitlab-ci.yml` & `km3io-1.0.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/CHANGELOG.rst` & `km3io-1.0.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Unreleased changes
 ------------------
 
-Version 0
+Version 1
 ---------
+1.0.1 / 2023-06-15
+~~~~~~~~~~~~~~~~~~
+* Minor changes
+
 1.0.0 / 2023-02-27
-~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~~~
 * API stabilised and v1 is now LTS
 * ``gSeaGen`` reader removed, only supported until v0.29.2
 
+Version 0
+---------
+
 0.29.2 / 2022-12-21
 ~~~~~~~~~~~~~~~~~~~
 * Hotfix for AwkwardArray 2.0 incompatibility, now restricted to
   be <2.0
 
 0.29.1 / 2022-12-01
 ~~~~~~~~~~~~~~~~~~~
```

### Comparing `km3io-1.0.0/CONTRIBUTING.rst` & `km3io-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/LICENSE` & `km3io-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/Makefile` & `km3io-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/PKG-INFO` & `km3io-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: km3io
-Version: 1.0.0
+Version: 1.0.1
 Summary: "KM3NeT I/O library without ROOT"
 Home-page: https://git.km3net.de/km3py/km3io
 Author: "Tamas Gal and Zineb Aly"
 Author-email: tgal@km3net.de
 Maintainer: Tamas Gal
 Maintainer-email: tgal@km3net.de
 License: MIT
@@ -24,16 +24,14 @@
            :target: https://doi.org/10.5281/zenodo.7382620
         
         This software provides a set of Python classes to read KM3NeT ROOT files
         without having ROOT, Jpp or aanet installed. It only depends on Python 3.5+ and the amazing `uproot <https://github.com/scikit-hep/uproot>`__ package and gives you access to the data via `numpy <https://www.numpy.org>`__ and `awkward <https://awkward-array.readthedocs.io>`__ arrays.
         
         It's very easy to use and according to the `uproot <https://github.com/scikit-hep/uproot>`__ benchmarks, it is able to outperform the original ROOT I/O performance. 
         
-        **Note:** Beware that this package is in the development phase, so the API will change until version ``1.0.0`` is released!
-        
         Installation
         ============
         
         Install km3io using pip::
         
             pip install km3io 
         
@@ -91,14 +89,39 @@
             >>> f = km3io.OfflineReader(data_path("offline/numucc.root"))
             >>> f[:4].tracks.dir_z
             <Array [[0.213, 0.213, ... 0.229, 0.323]] type='4 * var * float64'>
         
         The same concept applies to all other branches, including ``hits``, ``mc_hits``,
         ``mc_tracks``, ``t_sec`` etc.
         
+        Architecture overview
+        ---------------------
+        
+        ``km3io`` utilises ``uproot`` behind the scenes and creates a lazy and thin
+        wrapper which offers convenient slicing and iterations by delaying the access to
+        the actual ROOT data branches to the very last moment. When using the iteration
+        functionality, the data is loaded in chunks and the iteration is done over e.g.
+        events in each chunk or a bunch of frames in case of the summaryslice reader.
+        
+        The base class for the event-based readout is the ``km3io.rootio.EventReader``
+        class. When subclassing this class, the branches, aliases and nested branches
+        need to be defined in the static variables which are then used to mask unwanted
+        attributes. Especially in case of the Offline ROOT format, where the "one class
+        fits all" design was chosen, it is distracting that e.g. a `Hit` has many
+        attributes which make no sense depending on the context (MC hit, raw hit etc.).
+        By specifing the branches explicitely, the user API will only expose the
+        meaningful fields.
+        
+        The online ROOT format support is partly still based on ``uproot3``.
+        
+        Many of the utility functions are using Numba to achieve the best possible
+        performance. ``km3io`` does not offer alternative implementations, so Numba is a
+        strict dependency and an integral part of the implementation.
+        
+        
         Offline files reader
         --------------------
         
         In general an offline file has two attributes to access data: the header and the events. Let's start with the header.
         
         Reading the file header
         """""""""""""""""""""""
```

### Comparing `km3io-1.0.0/README.rst` & `km3io-1.0.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,14 @@
    :target: https://doi.org/10.5281/zenodo.7382620
 
 This software provides a set of Python classes to read KM3NeT ROOT files
 without having ROOT, Jpp or aanet installed. It only depends on Python 3.5+ and the amazing `uproot <https://github.com/scikit-hep/uproot>`__ package and gives you access to the data via `numpy <https://www.numpy.org>`__ and `awkward <https://awkward-array.readthedocs.io>`__ arrays.
 
 It's very easy to use and according to the `uproot <https://github.com/scikit-hep/uproot>`__ benchmarks, it is able to outperform the original ROOT I/O performance. 
 
-**Note:** Beware that this package is in the development phase, so the API will change until version ``1.0.0`` is released!
-
 Installation
 ============
 
 Install km3io using pip::
 
     pip install km3io 
 
@@ -81,14 +79,39 @@
     >>> f = km3io.OfflineReader(data_path("offline/numucc.root"))
     >>> f[:4].tracks.dir_z
     <Array [[0.213, 0.213, ... 0.229, 0.323]] type='4 * var * float64'>
 
 The same concept applies to all other branches, including ``hits``, ``mc_hits``,
 ``mc_tracks``, ``t_sec`` etc.
 
+Architecture overview
+---------------------
+
+``km3io`` utilises ``uproot`` behind the scenes and creates a lazy and thin
+wrapper which offers convenient slicing and iterations by delaying the access to
+the actual ROOT data branches to the very last moment. When using the iteration
+functionality, the data is loaded in chunks and the iteration is done over e.g.
+events in each chunk or a bunch of frames in case of the summaryslice reader.
+
+The base class for the event-based readout is the ``km3io.rootio.EventReader``
+class. When subclassing this class, the branches, aliases and nested branches
+need to be defined in the static variables which are then used to mask unwanted
+attributes. Especially in case of the Offline ROOT format, where the "one class
+fits all" design was chosen, it is distracting that e.g. a `Hit` has many
+attributes which make no sense depending on the context (MC hit, raw hit etc.).
+By specifing the branches explicitely, the user API will only expose the
+meaningful fields.
+
+The online ROOT format support is partly still based on ``uproot3``.
+
+Many of the utility functions are using Numba to achieve the best possible
+performance. ``km3io`` does not offer alternative implementations, so Numba is a
+strict dependency and an integral part of the implementation.
+
+
 Offline files reader
 --------------------
 
 In general an offline file has two attributes to access data: the header and the events. Let's start with the header.
 
 Reading the file header
 """""""""""""""""""""""
```

### Comparing `km3io-1.0.0/codemeta.json` & `km3io-1.0.1/codemeta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8846153846153846%*

 * *Differences: {"'copyrightHolder'": "'KM3NeT Collaboration'",*

 * * "'dateModified'": "'2023-06-15'",*

 * * "'releaseNotes'": "'https://km3py.pages.km3net.de/km3io/changelog.html'",*

 * * "'softwareVersion'": "'1.0.0'"}*

```diff
@@ -31,16 +31,17 @@
         {
             "@id": "https://orcid.org/0000-0002-5593-2580",
             "@type": "Person",
             "familyName": "Aly",
             "givenName": "Zineb"
         }
     ],
+    "copyrightHolder": "KM3NeT Collaboration",
     "dateCreated": "2019-11-15",
-    "dateModified": "2022-09-23",
+    "dateModified": "2023-06-15",
     "datePublished": "2019-11-15",
     "description": "Pure Python I/O library for KM3NeT related files.",
     "developmentStatus": "active",
     "downloadUrl": "https://git.km3net.de/km3py/km3io",
     "issueTracker": "https://git.km3net.de/km3py/km3io/-/issues",
     "keywords": [
         "i/o",
@@ -59,9 +60,10 @@
         "Python 3"
     ],
     "readme": "https://git.km3net.de/km3py/km3io/-/blob/master/README.rst",
     "referencePublication": "https://doi.org/10.5281/zenodo.808829",
     "relatedLink": [
         "https://km3py.pages.km3net.de/km3io/"
     ],
-    "softwareVersion": "0.27.0"
+    "releaseNotes": "https://km3py.pages.km3net.de/km3io/changelog.html",
+    "softwareVersion": "1.0.0"
 }
```

### Comparing `km3io-1.0.0/doc/Makefile` & `km3io-1.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/doc/_static/default_gallery_thumbnail.png` & `km3io-1.0.1/doc/_static/default_gallery_thumbnail.png`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/doc/conf.py` & `km3io-1.0.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/doc/index.rst` & `km3io-1.0.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/doc/make.bat` & `km3io-1.0.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/examples/plot_offline_events.py` & `km3io-1.0.1/examples/plot_offline_events.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/examples/plot_offline_tracks.py` & `km3io-1.0.1/examples/plot_offline_tracks.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/examples/plot_offline_usr.py` & `km3io-1.0.1/examples/plot_offline_usr.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/examples/plot_online_example.py` & `km3io-1.0.1/examples/plot_online_example.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/setup.cfg` & `km3io-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 	pytest-cov
 	pytest-flake8
 	pytest-pylint
 	pytest-watch
 	scipy
 	sphinx
 	sphinx-autoapi
-	sphinx-gallery>=0.1.12
+	sphinx-gallery
 	sphinx_rtd_theme
 	sphinxcontrib-versioning
 	wheel
 
 [options.entry_points]
 console_scripts = 
 	KPrintTree = km3io.utils.kprinttree:main
```

### Comparing `km3io-1.0.0/src/km3io/__init__.py` & `km3io-1.0.1/src/km3io/__init__.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/_definitions/fitparameters.py` & `km3io-1.0.1/src/km3io/_definitions/fitparameters.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/_definitions/mc_header.py` & `km3io-1.0.1/src/km3io/_definitions/mc_header.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/_definitions/reconstruction.py` & `km3io-1.0.1/src/km3io/_definitions/reconstruction.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/_definitions/root.py` & `km3io-1.0.1/src/km3io/_definitions/root.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/_definitions/trkmembers.py` & `km3io-1.0.1/src/km3io/_definitions/trkmembers.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/_definitions/w2list_gseagen.py` & `km3io-1.0.1/src/km3io/_definitions/w2list_gseagen.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/_definitions/w2list_km3buu.py` & `km3io-1.0.1/src/km3io/_definitions/w2list_km3buu.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/acoustics.py` & `km3io-1.0.1/src/km3io/acoustics.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/definitions.py` & `km3io-1.0.1/src/km3io/definitions.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/offline.py` & `km3io-1.0.1/src/km3io/offline.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/online.py` & `km3io-1.0.1/src/km3io/online.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/rootio.py` & `km3io-1.0.1/src/km3io/rootio.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/tools.py` & `km3io-1.0.1/src/km3io/tools.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io/utils/kprinttree.py` & `km3io-1.0.1/src/km3io/utils/kprinttree.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/src/km3io.egg-info/PKG-INFO` & `km3io-1.0.1/src/km3io.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: km3io
-Version: 1.0.0
+Version: 1.0.1
 Summary: "KM3NeT I/O library without ROOT"
 Home-page: https://git.km3net.de/km3py/km3io
 Author: "Tamas Gal and Zineb Aly"
 Author-email: tgal@km3net.de
 Maintainer: Tamas Gal
 Maintainer-email: tgal@km3net.de
 License: MIT
@@ -24,16 +24,14 @@
            :target: https://doi.org/10.5281/zenodo.7382620
         
         This software provides a set of Python classes to read KM3NeT ROOT files
         without having ROOT, Jpp or aanet installed. It only depends on Python 3.5+ and the amazing `uproot <https://github.com/scikit-hep/uproot>`__ package and gives you access to the data via `numpy <https://www.numpy.org>`__ and `awkward <https://awkward-array.readthedocs.io>`__ arrays.
         
         It's very easy to use and according to the `uproot <https://github.com/scikit-hep/uproot>`__ benchmarks, it is able to outperform the original ROOT I/O performance. 
         
-        **Note:** Beware that this package is in the development phase, so the API will change until version ``1.0.0`` is released!
-        
         Installation
         ============
         
         Install km3io using pip::
         
             pip install km3io 
         
@@ -91,14 +89,39 @@
             >>> f = km3io.OfflineReader(data_path("offline/numucc.root"))
             >>> f[:4].tracks.dir_z
             <Array [[0.213, 0.213, ... 0.229, 0.323]] type='4 * var * float64'>
         
         The same concept applies to all other branches, including ``hits``, ``mc_hits``,
         ``mc_tracks``, ``t_sec`` etc.
         
+        Architecture overview
+        ---------------------
+        
+        ``km3io`` utilises ``uproot`` behind the scenes and creates a lazy and thin
+        wrapper which offers convenient slicing and iterations by delaying the access to
+        the actual ROOT data branches to the very last moment. When using the iteration
+        functionality, the data is loaded in chunks and the iteration is done over e.g.
+        events in each chunk or a bunch of frames in case of the summaryslice reader.
+        
+        The base class for the event-based readout is the ``km3io.rootio.EventReader``
+        class. When subclassing this class, the branches, aliases and nested branches
+        need to be defined in the static variables which are then used to mask unwanted
+        attributes. Especially in case of the Offline ROOT format, where the "one class
+        fits all" design was chosen, it is distracting that e.g. a `Hit` has many
+        attributes which make no sense depending on the context (MC hit, raw hit etc.).
+        By specifing the branches explicitely, the user API will only expose the
+        meaningful fields.
+        
+        The online ROOT format support is partly still based on ``uproot3``.
+        
+        Many of the utility functions are using Numba to achieve the best possible
+        performance. ``km3io`` does not offer alternative implementations, so Numba is a
+        strict dependency and an integral part of the implementation.
+        
+        
         Offline files reader
         --------------------
         
         In general an offline file has two attributes to access data: the header and the events. Let's start with the header.
         
         Reading the file header
         """""""""""""""""""""""
```

### Comparing `km3io-1.0.0/src/km3io.egg-info/SOURCES.txt` & `km3io-1.0.1/src/km3io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/talks/images/orca-du4.png` & `km3io-1.0.1/talks/images/orca-du4.png`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/talks/images/uproot_vs_root.png` & `km3io-1.0.1/talks/images/uproot_vs_root.png`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/talks/images/uproot_vs_root_numpy.png` & `km3io-1.0.1/talks/images/uproot_vs_root_numpy.png`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/talks/premiere.org` & `km3io-1.0.1/talks/premiere.org`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/tests/test_acoustics.py` & `km3io-1.0.1/tests/test_acoustics.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/tests/test_offline.py` & `km3io-1.0.1/tests/test_offline.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/tests/test_online.py` & `km3io-1.0.1/tests/test_online.py`

 * *Files identical despite different names*

### Comparing `km3io-1.0.0/tests/test_tools.py` & `km3io-1.0.1/tests/test_tools.py`

 * *Files identical despite different names*

