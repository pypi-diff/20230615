# Comparing `tmp/wnutils-3.0.0.tar.gz` & `tmp/wnutils-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnutils-3.0.0.tar", last modified: Thu Jun 15 14:10:16 2023, max compression
+gzip compressed data, was "wnutils-3.0.1.tar", last modified: Thu Jun 15 14:27:42 2023, max compression
```

## Comparing `wnutils-3.0.0.tar` & `wnutils-3.0.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.554400 wnutils-3.0.0/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       22 2021-04-30 17:40:33.000000 wnutils-3.0.0/.gitignore
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      607 2022-07-14 16:19:11.000000 wnutils-3.0.0/.readthedocs.yaml
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2021-04-30 17:40:33.000000 wnutils-3.0.0/LICENSE.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      135 2021-04-30 17:40:33.000000 wnutils-3.0.0/MANIFEST.in
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1922 2023-06-15 14:10:16.554702 wnutils-3.0.0/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1122 2022-12-26 18:13:59.000000 wnutils-3.0.0/README.rst
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.476472 wnutils-3.0.0/doc/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/.gitignore
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      608 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/Makefile
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      815 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/make.bat
--rwxr-xr-x   0 bradleymeyer   (501) staff       (20)      123 2022-07-14 16:19:11.000000 wnutils-3.0.0/doc/make_doc.sh
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       67 2022-07-14 16:19:11.000000 wnutils-3.0.0/doc/requirements.txt
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.503243 wnutils-3.0.0/doc/source/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        0 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/.gitignore
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.505000 wnutils-3.0.0/doc/source/_static/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       41 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/_static/custom.css
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.506868 wnutils-3.0.0/doc/source/_templates/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      158 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/_templates/layout.html
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      198 2022-12-26 18:13:59.000000 wnutils-3.0.0/doc/source/acknowledgments.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    14551 2021-05-08 13:55:17.000000 wnutils-3.0.0/doc/source/animate_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     7713 2023-06-15 14:09:47.000000 wnutils-3.0.0/doc/source/changelog.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     5800 2023-06-15 14:09:47.000000 wnutils-3.0.0/doc/source/conf.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1412 2022-10-08 19:12:16.000000 wnutils-3.0.0/doc/source/data_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       55 2022-05-27 01:50:21.000000 wnutils-3.0.0/doc/source/documentation.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      509 2023-01-01 16:17:13.000000 wnutils-3.0.0/doc/source/index.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1639 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/installation_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    18694 2022-07-14 16:51:29.000000 wnutils-3.0.0/doc/source/plot_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    23002 2022-12-26 18:13:59.000000 wnutils-3.0.0/doc/source/read_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       30 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/readme.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      166 2021-04-30 17:40:33.000000 wnutils-3.0.0/doc/source/tutorials.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      781 2022-05-02 22:17:17.000000 wnutils-3.0.0/doc/source/wnutils.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    20713 2023-06-15 14:09:47.000000 wnutils-3.0.0/doc/source/write_tutorial.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      106 2023-06-15 14:10:16.555883 wnutils-3.0.0/setup.cfg
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6085 2023-01-01 16:17:13.000000 wnutils-3.0.0/setup.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.521021 wnutils-3.0.0/wnutils/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       26 2022-10-08 19:12:16.000000 wnutils-3.0.0/wnutils/.gitignore
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      158 2022-10-08 19:12:16.000000 wnutils-3.0.0/wnutils/README
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      276 2023-06-15 14:09:47.000000 wnutils-3.0.0/wnutils/__about__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      462 2022-10-08 19:12:16.000000 wnutils-3.0.0/wnutils/__init__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    12755 2023-05-26 01:39:45.000000 wnutils-3.0.0/wnutils/base.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    33786 2022-10-08 19:12:16.000000 wnutils-3.0.0/wnutils/h5.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6389 2022-07-14 16:51:29.000000 wnutils-3.0.0/wnutils/multi_h5.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6097 2022-07-14 16:51:29.000000 wnutils-3.0.0/wnutils/multi_xml.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    61000 2023-06-15 14:09:47.000000 wnutils-3.0.0/wnutils/xml.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.553323 wnutils-3.0.0/wnutils/xsd_pub/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1535 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/catalog
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3494 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/input_nuclide_z_a.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     4211 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3625 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__net.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     2906 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__nuc.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     5455 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__nuc__types.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     2934 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__reac.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    10572 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/libnucnet__reac__types.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     5832 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/xml.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3316 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/zone_data.xsd
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     5301 2022-10-08 18:43:35.000000 wnutils-3.0.0/wnutils/xsd_pub/zone_data_types.xsd
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:10:16.531620 wnutils-3.0.0/wnutils.egg-info/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1922 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1315 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/SOURCES.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/dependency_links.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       72 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/requires.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        8 2023-06-15 14:10:16.000000 wnutils-3.0.0/wnutils.egg-info/top_level.txt
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:27:42.219429 wnutils-3.0.1/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       22 2021-04-30 17:40:33.000000 wnutils-3.0.1/.gitignore
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      607 2022-07-14 16:19:11.000000 wnutils-3.0.1/.readthedocs.yaml
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2021-04-30 17:40:33.000000 wnutils-3.0.1/LICENSE.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      135 2021-04-30 17:40:33.000000 wnutils-3.0.1/MANIFEST.in
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1922 2023-06-15 14:27:42.219708 wnutils-3.0.1/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1122 2022-12-26 18:13:59.000000 wnutils-3.0.1/README.rst
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:27:42.114268 wnutils-3.0.1/doc/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2021-04-30 17:40:33.000000 wnutils-3.0.1/doc/.gitignore
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      608 2021-04-30 17:40:33.000000 wnutils-3.0.1/doc/Makefile
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      815 2021-04-30 17:40:33.000000 wnutils-3.0.1/doc/make.bat
+-rwxr-xr-x   0 bradleymeyer   (501) staff       (20)      123 2022-07-14 16:19:11.000000 wnutils-3.0.1/doc/make_doc.sh
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       85 2023-06-15 14:21:18.000000 wnutils-3.0.1/doc/requirements.txt
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:27:42.132301 wnutils-3.0.1/doc/source/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        0 2021-04-30 17:40:33.000000 wnutils-3.0.1/doc/source/.gitignore
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:27:42.133774 wnutils-3.0.1/doc/source/_static/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       41 2021-04-30 17:40:33.000000 wnutils-3.0.1/doc/source/_static/custom.css
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:27:42.135189 wnutils-3.0.1/doc/source/_templates/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      158 2021-04-30 17:40:33.000000 wnutils-3.0.1/doc/source/_templates/layout.html
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      198 2022-12-26 18:13:59.000000 wnutils-3.0.1/doc/source/acknowledgments.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    14551 2021-05-08 13:55:17.000000 wnutils-3.0.1/doc/source/animate_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     7857 2023-06-15 14:25:25.000000 wnutils-3.0.1/doc/source/changelog.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     5800 2023-06-15 14:09:47.000000 wnutils-3.0.1/doc/source/conf.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1412 2022-10-08 19:12:16.000000 wnutils-3.0.1/doc/source/data_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       55 2022-05-27 01:50:21.000000 wnutils-3.0.1/doc/source/documentation.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      509 2023-01-01 16:17:13.000000 wnutils-3.0.1/doc/source/index.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1639 2021-04-30 17:40:33.000000 wnutils-3.0.1/doc/source/installation_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    18694 2022-07-14 16:51:29.000000 wnutils-3.0.1/doc/source/plot_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    23002 2022-12-26 18:13:59.000000 wnutils-3.0.1/doc/source/read_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       30 2021-04-30 17:40:33.000000 wnutils-3.0.1/doc/source/readme.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      166 2021-04-30 17:40:33.000000 wnutils-3.0.1/doc/source/tutorials.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      781 2022-05-02 22:17:17.000000 wnutils-3.0.1/doc/source/wnutils.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    20713 2023-06-15 14:09:47.000000 wnutils-3.0.1/doc/source/write_tutorial.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      106 2023-06-15 14:27:42.220977 wnutils-3.0.1/setup.cfg
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6085 2023-01-01 16:17:13.000000 wnutils-3.0.1/setup.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:27:42.157499 wnutils-3.0.1/wnutils/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       26 2022-10-08 19:12:16.000000 wnutils-3.0.1/wnutils/.gitignore
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      158 2022-10-08 19:12:16.000000 wnutils-3.0.1/wnutils/README
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      276 2023-06-15 14:21:18.000000 wnutils-3.0.1/wnutils/__about__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      462 2022-10-08 19:12:16.000000 wnutils-3.0.1/wnutils/__init__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    12755 2023-05-26 01:39:45.000000 wnutils-3.0.1/wnutils/base.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    33786 2022-10-08 19:12:16.000000 wnutils-3.0.1/wnutils/h5.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6389 2022-07-14 16:51:29.000000 wnutils-3.0.1/wnutils/multi_h5.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6097 2022-07-14 16:51:29.000000 wnutils-3.0.1/wnutils/multi_xml.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    61000 2023-06-15 14:09:47.000000 wnutils-3.0.1/wnutils/xml.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:27:42.218353 wnutils-3.0.1/wnutils/xsd_pub/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1535 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/catalog
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3494 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/input_nuclide_z_a.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     4211 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/libnucnet.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3625 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/libnucnet__net.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     2906 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/libnucnet__nuc.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     5455 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/libnucnet__nuc__types.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     2934 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/libnucnet__reac.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    10572 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/libnucnet__reac__types.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     5832 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/xml.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3316 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/zone_data.xsd
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     5301 2022-10-08 18:43:35.000000 wnutils-3.0.1/wnutils/xsd_pub/zone_data_types.xsd
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-06-15 14:27:42.168979 wnutils-3.0.1/wnutils.egg-info/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1922 2023-06-15 14:27:42.000000 wnutils-3.0.1/wnutils.egg-info/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1315 2023-06-15 14:27:42.000000 wnutils-3.0.1/wnutils.egg-info/SOURCES.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-06-15 14:27:42.000000 wnutils-3.0.1/wnutils.egg-info/dependency_links.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       72 2023-06-15 14:27:42.000000 wnutils-3.0.1/wnutils.egg-info/requires.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        8 2023-06-15 14:27:42.000000 wnutils-3.0.1/wnutils.egg-info/top_level.txt
```

### Comparing `wnutils-3.0.0/.readthedocs.yaml` & `wnutils-3.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/LICENSE.txt` & `wnutils-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/PKG-INFO` & `wnutils-3.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnutils
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python project to read and plot webnucleo files
 Home-page: https://github.com/mbradle/wnutils
 Author: Clemson University
 Author-email: mbradle@clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnutils/issues
 Project-URL: Source, https://github.com/mbradle/wnutils/
```

### Comparing `wnutils-3.0.0/README.rst` & `wnutils-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/Makefile` & `wnutils-3.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/make.bat` & `wnutils-3.0.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/source/animate_tutorial.rst` & `wnutils-3.0.1/doc/source/animate_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/source/changelog.rst` & `wnutils-3.0.1/doc/source/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 Changelog
 =========
 
 All notable changes to this project will be documented in this file.  This
 project adheres to `Semantic Versioning <http://semver.org/spec/v2.0.0.html>`_.
 
+Version 3.0.1
+--------------
+
+Fix:
+
+  * The copy button requirement has been added to the package to enable proper
+    documentation building.
+
 Version 3.0.0
 --------------
 
 New:
 
   * Copy buttons have been added to the tutorial pages.
```

### Comparing `wnutils-3.0.0/doc/source/conf.py` & `wnutils-3.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/source/data_tutorial.rst` & `wnutils-3.0.1/doc/source/data_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/source/installation_tutorial.rst` & `wnutils-3.0.1/doc/source/installation_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/source/plot_tutorial.rst` & `wnutils-3.0.1/doc/source/plot_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/source/read_tutorial.rst` & `wnutils-3.0.1/doc/source/read_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/source/wnutils.rst` & `wnutils-3.0.1/doc/source/wnutils.rst`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/doc/source/write_tutorial.rst` & `wnutils-3.0.1/doc/source/write_tutorial.rst`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/setup.py` & `wnutils-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/base.py` & `wnutils-3.0.1/wnutils/base.py`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/h5.py` & `wnutils-3.0.1/wnutils/h5.py`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/multi_h5.py` & `wnutils-3.0.1/wnutils/multi_h5.py`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/multi_xml.py` & `wnutils-3.0.1/wnutils/multi_xml.py`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xml.py` & `wnutils-3.0.1/wnutils/xml.py`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/catalog` & `wnutils-3.0.1/wnutils/xsd_pub/catalog`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/input_nuclide_z_a.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/input_nuclide_z_a.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/libnucnet.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/libnucnet.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__net.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/libnucnet__net.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__nuc.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/libnucnet__nuc.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__nuc__types.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/libnucnet__nuc__types.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__reac.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/libnucnet__reac.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/libnucnet__reac__types.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/libnucnet__reac__types.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/xml.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/xml.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/zone_data.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/zone_data.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils/xsd_pub/zone_data_types.xsd` & `wnutils-3.0.1/wnutils/xsd_pub/zone_data_types.xsd`

 * *Files identical despite different names*

### Comparing `wnutils-3.0.0/wnutils.egg-info/PKG-INFO` & `wnutils-3.0.1/wnutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnutils
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python project to read and plot webnucleo files
 Home-page: https://github.com/mbradle/wnutils
 Author: Clemson University
 Author-email: mbradle@clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnutils/issues
 Project-URL: Source, https://github.com/mbradle/wnutils/
```

### Comparing `wnutils-3.0.0/wnutils.egg-info/SOURCES.txt` & `wnutils-3.0.1/wnutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

