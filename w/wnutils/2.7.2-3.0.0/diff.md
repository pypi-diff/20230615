# Comparing `tmp/wnutils-2.7.2.tar.gz` & `tmp/wnutils-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnutils-2.7.2.tar", last modified: Fri May 26 01:50:17 2023, max compression
+gzip compressed data, was "wnutils-3.0.0.tar", last modified: Thu Jun 15 14:10:16 2023, max compression
```

## Comparing `wnutils-2.7.2.tar` & `wnutils-3.0.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 01:50:17.229021 wnutils-2.7.2/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       22 2021-04-30 17:40:33.000000 wnutils-2.7.2/.gitignore
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      607 2022-07-14 16:19:11.000000 wnutils-2.7.2/.readthedocs.yaml
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2021-04-30 17:40:33.000000 wnutils-2.7.2/LICENSE.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      135 2021-04-30 17:40:33.000000 wnutils-2.7.2/MANIFEST.in
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1922 2023-05-26 01:50:17.229235 wnutils-2.7.2/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1122 2022-12-26 18:13:59.000000 wnutils-2.7.2/README.rst
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 01:50:17.141532 wnutils-2.7.2/doc/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2021-04-30 17:40:33.000000 wnutils-2.7.2/doc/.gitignore
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      608 2021-04-30 17:40:33.000000 wnutils-2.7.2/doc/Makefile
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      815 2021-04-30 17:40:33.000000 wnutils-2.7.2/doc/make.bat
--rwxr-xr-x   0 bradleymeyer   (501) staff       (20)      123 2022-07-14 16:19:11.000000 wnutils-2.7.2/doc/make_doc.sh
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       67 2022-07-14 16:19:11.000000 wnutils-2.7.2/doc/requirements.txt
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 01:50:17.176448 wnutils-2.7.2/doc/source/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        0 2021-04-30 17:40:33.000000 wnutils-2.7.2/doc/source/.gitignore
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 01:50:17.178451 wnutils-2.7.2/doc/source/_static/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       41 2021-04-30 17:40:33.000000 wnutils-2.7.2/doc/source/_static/custom.css
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 01:50:17.179724 wnutils-2.7.2/doc/source/_templates/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      158 2021-04-30 17:40:33.000000 wnutils-2.7.2/doc/source/_templates/layout.html
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      198 2022-12-26 18:13:59.000000 wnutils-2.7.2/doc/source/acknowledgments.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    14551 2021-05-08 13:55:17.000000 wnutils-2.7.2/doc/source/animate_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     7490 2023-05-26 01:39:45.000000 wnutils-2.7.2/doc/source/changelog.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     5651 2023-02-25 17:36:06.000000 wnutils-2.7.2/doc/source/conf.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1412 2022-10-08 19:12:16.000000 wnutils-2.7.2/doc/source/data_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       55 2022-05-27 01:50:21.000000 wnutils-2.7.2/doc/source/documentation.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      509 2023-01-01 16:17:13.000000 wnutils-2.7.2/doc/source/index.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1639 2021-04-30 17:40:33.000000 wnutils-2.7.2/doc/source/installation_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    18694 2022-07-14 16:51:29.000000 wnutils-2.7.2/doc/source/plot_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    23002 2022-12-26 18:13:59.000000 wnutils-2.7.2/doc/source/read_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       30 2021-04-30 17:40:33.000000 wnutils-2.7.2/doc/source/readme.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      166 2021-04-30 17:40:33.000000 wnutils-2.7.2/doc/source/tutorials.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      781 2022-05-02 22:17:17.000000 wnutils-2.7.2/doc/source/wnutils.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    20661 2022-07-30 11:47:08.000000 wnutils-2.7.2/doc/source/write_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      106 2023-05-26 01:50:17.230314 wnutils-2.7.2/setup.cfg
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6085 2023-01-01 16:17:13.000000 wnutils-2.7.2/setup.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 01:50:17.193060 wnutils-2.7.2/wnutils/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       26 2022-10-08 19:12:16.000000 wnutils-2.7.2/wnutils/.gitignore
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      158 2022-10-08 19:12:16.000000 wnutils-2.7.2/wnutils/README
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      276 2023-05-26 01:39:45.000000 wnutils-2.7.2/wnutils/__about__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      462 2022-10-08 19:12:16.000000 wnutils-2.7.2/wnutils/__init__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    12755 2023-05-26 01:39:45.000000 wnutils-2.7.2/wnutils/base.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    33786 2022-10-08 19:12:16.000000 wnutils-2.7.2/wnutils/h5.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6389 2022-07-14 16:51:29.000000 wnutils-2.7.2/wnutils/multi_h5.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6097 2022-07-14 16:51:29.000000 wnutils-2.7.2/wnutils/multi_xml.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    60846 2023-04-27 11:21:48.000000 wnutils-2.7.2/wnutils/xml.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 01:50:17.227818 wnutils-2.7.2/wnutils/xsd_pub/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1535 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/catalog
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3494 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/input_nuclide_z_a.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     4211 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/libnucnet.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3625 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/libnucnet__net.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     2906 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/libnucnet__nuc.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     5455 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/libnucnet__nuc__types.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     2934 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/libnucnet__reac.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    10572 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/libnucnet__reac__types.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     5832 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/xml.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3316 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/zone_data.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     5301 2022-10-08 18:43:35.000000 wnutils-2.7.2/wnutils/xsd_pub/zone_data_types.xsd
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-05-26 01:50:17.199947 wnutils-2.7.2/wnutils.egg-info/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1922 2023-05-26 01:50:17.000000 wnutils-2.7.2/wnutils.egg-info/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1315 2023-05-26 01:50:17.000000 wnutils-2.7.2/wnutils.egg-info/SOURCES.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-05-26 01:50:17.000000 wnutils-2.7.2/wnutils.egg-info/dependency_links.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       72 2023-05-26 01:50:17.000000 wnutils-2.7.2/wnutils.egg-info/requires.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        8 2023-05-26 01:50:17.000000 wnutils-2.7.2/wnutils.egg-info/top_level.txt
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.554400 wnutils-3.0.0/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       22 2021-04-30 17:40:33.000000 wnutils-3.0.0/.gitignore
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      607 2022-07-14 16:19:11.000000 wnutils-3.0.0/.readthedocs.yaml
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2021-04-30 17:40:33.000000 wnutils-3.0.0/LICENSE.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      135 2021-04-30 17:40:33.000000 wnutils-3.0.0/MANIFEST.in
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1922 2023-06-15 14:10:16.554702 wnutils-3.0.0/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1122 2022-12-26 18:13:59.000000 wnutils-3.0.0/README.rst
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.476472 wnutils-3.0.0/doc/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/.gitignore
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      608 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/Makefile
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      815 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/make.bat
+-rwxr-xr-x   0 bradleymeyer   (501) staff       (20)      123 2022-07-14 16:19:11.000000 wnutils-3.0.0/doc/make_doc.sh
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       67 2022-07-14 16:19:11.000000 wnutils-3.0.0/doc/requirements.txt
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.503243 wnutils-3.0.0/doc/source/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        0 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/.gitignore
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.505000 wnutils-3.0.0/doc/source/_static/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       41 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/_static/custom.css
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.506868 wnutils-3.0.0/doc/source/_templates/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      158 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/_templates/layout.html
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      198 2022-12-26 18:13:59.000000 wnutils-3.0.0/doc/source/acknowledgments.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    14551 2021-05-08 13:55:17.000000 wnutils-3.0.0/doc/source/animate_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     7713 2023-06-15 14:09:47.000000 wnutils-3.0.0/doc/source/changelog.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     5800 2023-06-15 14:09:47.000000 wnutils-3.0.0/doc/source/conf.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1412 2022-10-08 19:12:16.000000 wnutils-3.0.0/doc/source/data_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       55 2022-05-27 01:50:21.000000 wnutils-3.0.0/doc/source/documentation.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      509 2023-01-01 16:17:13.000000 wnutils-3.0.0/doc/source/index.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1639 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/installation_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    18694 2022-07-14 16:51:29.000000 wnutils-3.0.0/doc/source/plot_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    23002 2022-12-26 18:13:59.000000 wnutils-3.0.0/doc/source/read_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       30 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/readme.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      166 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/tutorials.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      781 2022-05-02 22:17:17.000000 wnutils-3.0.0/doc/source/wnutils.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    20713 2023-06-15 14:09:47.000000 wnutils-3.0.0/doc/source/write_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      106 2023-06-15 14:10:16.555883 wnutils-3.0.0/setup.cfg
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6085 2023-01-01 16:17:13.000000 wnutils-3.0.0/setup.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.521021 wnutils-3.0.0/wnutils/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       26 2022-10-08 19:12:16.000000 wnutils-3.0.0/wnutils/.gitignore
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      158 2022-10-08 19:12:16.000000 wnutils-3.0.0/wnutils/README
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      276 2023-06-15 14:09:47.000000 wnutils-3.0.0/wnutils/__about__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      462 2022-10-08 19:12:16.000000 wnutils-3.0.0/wnutils/__init__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    12755 2023-05-26 01:39:45.000000 wnutils-3.0.0/wnutils/base.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    33786 2022-10-08 19:12:16.000000 wnutils-3.0.0/wnutils/h5.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6389 2022-07-14 16:51:29.000000 wnutils-3.0.0/wnutils/multi_h5.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6097 2022-07-14 16:51:29.000000 wnutils-3.0.0/wnutils/multi_xml.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    61000 2023-06-15 14:09:47.000000 wnutils-3.0.0/wnutils/xml.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.553323 wnutils-3.0.0/wnutils/xsd_pub/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1535 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/catalog
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3494 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/input_nuclide_z_a.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     4211 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3625 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__net.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     2906 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__nuc.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     5455 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__nuc__types.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     2934 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__reac.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    10572 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__reac__types.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     5832 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/xml.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3316 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/zone_data.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     5301 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/zone_data_types.xsd
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.531620 wnutils-3.0.0/wnutils.egg-info/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1922 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1315 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/SOURCES.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/dependency_links.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       72 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/requires.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        8 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/top_level.txt
```

### Comparing `wnutils-2.7.2/.readthedocs.yaml` & `wnutils-3.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/LICENSE.txt` & `wnutils-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/PKG-INFO` & `wnutils-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnutils
-Version: 2.7.2
+Version: 3.0.0
 Summary: Python project to read and plot webnucleo files
 Home-page: https://github.com/mbradle/wnutils
 Author: Clemson University
 Author-email: mbradle@clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnutils/issues
 Project-URL: Source, https://github.com/mbradle/wnutils/
```

### Comparing `wnutils-2.7.2/README.rst` & `wnutils-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/doc/Makefile` & `wnutils-3.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/doc/make.bat` & `wnutils-3.0.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/doc/source/animate_tutorial.rst` & `wnutils-3.0.0/doc/source/animate_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/doc/source/changelog.rst` & `wnutils-3.0.0/doc/source/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 Changelog
 =========
 
 All notable changes to this project will be documented in this file.  This
 project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
 
+Version 3.0.0
+--------------
+
+New:
+
+  * Copy buttons have been added to the tutorial pages.
+
+Fix:
+
+  * XML validation has been moved out of the Xml class to a separate routine.
+    This is a backwards-incompatible change.
+
 Version 2.7.2
 --------------
 
 Fix:
 
   * A typo on the non-nuclide reaction element anti-neutrino_tau has been fixed.
```

### Comparing `wnutils-2.7.2/doc/source/conf.py` & `wnutils-3.0.0/doc/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "sphinx.ext.doctest",
     "sphinx.ext.mathjax",
     "sphinx.ext.intersphinx",
     "sphinx.ext.todo",
     "sphinx.ext.coverage",
     "sphinx.ext.viewcode",
     "sphinx.ext.githubpages",
+    "sphinx_copybutton",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -163,14 +164,19 @@
         "Miscellaneous",
     )
 ]
 
 
 # -- Extension configuration -------------------------------------------------
 
+copybutton_prompt_text = r">>> |\.\.\. |\# |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
+copybutton_prompt_is_regexp = True
+
+
+
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "numpy": ("https://docs.scipy.org/doc/numpy/", None),
 }
```

### Comparing `wnutils-2.7.2/doc/source/data_tutorial.rst` & `wnutils-3.0.0/doc/source/data_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/doc/source/installation_tutorial.rst` & `wnutils-3.0.0/doc/source/installation_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/doc/source/plot_tutorial.rst` & `wnutils-3.0.0/doc/source/plot_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/doc/source/read_tutorial.rst` & `wnutils-3.0.0/doc/source/read_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/doc/source/wnutils.rst` & `wnutils-3.0.0/doc/source/wnutils.rst`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/doc/source/write_tutorial.rst` & `wnutils-3.0.0/doc/source/write_tutorial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 You can now read those data into an Xml object by typing
 
     >>> xml = wx.Xml('updated_nuclear_data.xml')
 
 Validate those data against the libnucnet XML nuclear data schema by typing
 
-    >>> xml.validate()
+    >>> wx.validate('updated_nuclear_data.xml')
 
 This will simply return, which shows that the data are valid.  Next, retrieve
 the nuclide data and print out the o16 data:
 
     >>> updated_nuclides = xml.get_nuclide_data()
     >>> print(updated_nuclides['o16'])
 
@@ -151,19 +151,19 @@
 
 Create the new XML, set the data, and write out the XML:
 
     >>> extended_xml = wx.New_Xml(xml_type='nuclear_data')
     >>> extended_xml.set_nuclide_data(nuclides)
     >>> extended_xml.write('extended_nuclear_data.xml')
 
-Read in the extended XML, validate, and print out the nuclide data to confirm
+Validate the extended XML, read in, and print out the nuclide data to confirm
 the new species has been added:
 
+    >>> wx.validate('extended_nuclear_data.xml')
     >>> xml = wx.Xml('extended_nuclear_data.xml')
-    >>> xml.validate()
     >>> extended_nuclides = xml.get_nuclide_data()
     >>> for nuc in extended_nuclides:
     ...     print(nuc, extended_nuclides[nuc]['z'], extended_nuclides[nuc]['a'])
     ...
 
 Create new nuclide data.
 ^^^^^^^^^^^^^^^^^^^^^^^^
@@ -214,18 +214,18 @@
 The reactions data includes all reactions in the old data set except those
 involving *kr85*.  Now create and write to XML:
 
     >>> subset_xml = wx.New_Xml(xml_type='reaction_data')
     >>> subset_xml.set_reaction_data(reactions)
     >>> subset_xml.write('subset_reaction_data.xml')
 
-One can now read in the data and validate:
+One can now validate and read in the data:
 
+    >>> wx.validate('subset_reaction_data.xml')
     >>> xml = wx.Xml('subset_reaction_data.xml')
-    >>> xml.validate()
 
 Now check that the *kr85* reactions have been excluded:
 
     >>> old_kr85 = old_xml.get_reaction_data("[reactant = 'kr85' or product = 'kr85']")
     >>> new_kr85 = xml.get_reaction_data("[reactant = 'kr85' or product = 'kr85']")
     >>> for reaction in old_kr85:
     ...     print(reaction)
@@ -521,16 +521,15 @@
     >>> zone_xml = wx.New_Xml('zone_data')
     >>> zone_xml.set_zone_data(zones)
     >>> zone_xml.write('new_zone_data.xml')
 
 The file *new_zone_data.xml* contains the data you created.
 You can validate it to ensure the data are the right XML format:
 
-    >>> xml = wx.Xml('new_zone_data.xml')
-    >>> xml.validate()
+    >>> wx.validate('new_zone_data.xml')
 
 Libnucnet XML Data
 ..................
 
 Full libnucnet data comprises nuclear network and zone data.  If you
 have created nuclide data (*nuclides*), reaction data (*reactions*),
 and zone data (*zones*), you can create full libnucnet data by typing:
```

### Comparing `wnutils-2.7.2/setup.py` & `wnutils-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/base.py` & `wnutils-3.0.0/wnutils/base.py`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/h5.py` & `wnutils-3.0.0/wnutils/h5.py`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/multi_h5.py` & `wnutils-3.0.0/wnutils/multi_h5.py`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/multi_xml.py` & `wnutils-3.0.0/wnutils/multi_xml.py`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xml.py` & `wnutils-3.0.0/wnutils/xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,46 @@
 from matplotlib.colors import LogNorm
 import matplotlib.animation as animation
 import numpy as np
 from lxml import etree
 from scipy.interpolate import interp1d
 
 
+def validate(file):
+    """Method to validate input Webnucleo XML.
+
+    Args:
+        ``file`` (:obj:`str`): The name of the xml file to validate.
+
+    Returns:
+        An error message if invalid and nothing if valid.
+
+    """
+
+    parser = etree.XMLParser(remove_blank_text=True)
+    _xml = etree.parse(file, parser)
+    _xml.xinclude()
+    _root = _xml.getroot()
+
+    xsd_dict = {
+        "nuclear_data": "libnucnet__nuc.xsd",
+        "reaction_data": "libnucnet__reac.xsd",
+        "nuclear_network": "libnucnet__net.xsd",
+        "zone_data": "zone_data.xsd",
+        "libnucnet_input": "libnucnet.xsd",
+    }
+
+    schema_file = os.path.join(
+        os.path.dirname(__file__), "xsd_pub", xsd_dict[_root.tag]
+    )
+
+    xml_validator = etree.XMLSchema(file=schema_file)
+    xml_validator.assert_(_xml)
+
+
 class Reaction(wb.Base):
     """A class for storing and retrieving data about reactions."""
 
     def __init__(self):
         self.reactants = []
         self.nuclide_reactants = []
         self.products = []
@@ -1440,37 +1472,14 @@
 
         anim = animation.FuncAnimation(fig, updatefig, abunds.shape[0])
         if movie_name:
             anim.save(movie_name, fps=fps)
 
         return anim
 
-    def validate(self):
-        """Method to validate the xml
-
-        Returns:
-            An error message if invalid and nothing if valid.
-
-        """
-
-        xsd_dict = {
-            "nuclear_data": "libnucnet__nuc.xsd",
-            "reaction_data": "libnucnet__reac.xsd",
-            "nuclear_network": "libnucnet__net.xsd",
-            "zone_data": "zone_data.xsd",
-            "libnucnet_input": "libnucnet.xsd",
-        }
-
-        schema_file = os.path.join(
-            os.path.dirname(__file__), "xsd_pub", xsd_dict[self._root.tag]
-        )
-
-        xml_validator = etree.XMLSchema(file=schema_file)
-        xml_validator.assert_(self._xml)
-
     def get_zone_data(self, zone_xpath=""):
         """Method to retrieve zone data from webnucleo XML.
 
         Args:
             ``zone_xpath`` (:obj:`str`, optional): XPath expression to select
             zones.  Defaults to all zones.
```

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/catalog` & `wnutils-3.0.0/wnutils/xsd_pub/catalog`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/input_nuclide_z_a.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/input_nuclide_z_a.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/libnucnet.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/libnucnet.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/libnucnet__net.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__net.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/libnucnet__nuc.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__nuc.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/libnucnet__nuc__types.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__nuc__types.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/libnucnet__reac.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__reac.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/libnucnet__reac__types.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__reac__types.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/xml.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/xml.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/zone_data.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/zone_data.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils/xsd_pub/zone_data_types.xsd` & `wnutils-3.0.0/wnutils/xsd_pub/zone_data_types.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-2.7.2/wnutils.egg-info/PKG-INFO` & `wnutils-3.0.0/wnutils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnutils
-Version: 2.7.2
+Version: 3.0.0
 Summary: Python project to read and plot webnucleo files
 Home-page: https://github.com/mbradle/wnutils
 Author: Clemson University
 Author-email: mbradle@clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnutils/issues
 Project-URL: Source, https://github.com/mbradle/wnutils/
```

### Comparing `wnutils-2.7.2/wnutils.egg-info/SOURCES.txt` & `wnutils-3.0.0/wnutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

