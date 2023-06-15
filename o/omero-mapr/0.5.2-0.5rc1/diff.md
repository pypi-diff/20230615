# Comparing `tmp/omero-mapr-0.5.2.tar.gz` & `tmp/omero-mapr-0.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-mapr-0.5.2.tar", last modified: Thu Jun 15 14:08:33 2023, max compression
+gzip compressed data, was "omero-mapr-0.5rc1.tar", last modified: Tue Mar 15 11:58:52 2022, max compression
```

## Comparing `omero-mapr-0.5.2.tar` & `omero-mapr-0.5rc1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 14:08:33.000000 omero-mapr-0.5.2/omero_mapr/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/custom_context_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/mapr_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/show.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.563534 omero-mapr-0.5.2/omero_mapr/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.563534 omero-mapr-0.5.2/omero_mapr/static/mapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/static/mapr/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/css/ome.mapr.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/static/mapr/image/
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/image/compound_icon_16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/image/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/image/gene_icon_16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/image/organism_icon_16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/image/phenotype_icon_16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/image/sirna_icon_16x16.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/static/mapr/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/javascript/center_plugin.thumbs.js
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/javascript/ome.mapr.js
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/static/mapr/javascript/ome.mapr.ui.autocomplete.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.563534 omero-mapr-0.5.2/omero_mapr/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/templates/mapr/
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/templates/mapr/base_mapr.html
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/templates/mapr/metadata_general.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.563534 omero-mapr-0.5.2/omero_mapr/templates/webclient/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.563534 omero-mapr-0.5.2/omero_mapr/templates/webclient/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/templates/webclient/data/includes/
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/templates/webclient/data/includes/right_plugin.general.js.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/templatetags/mapr_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/templatetags/mapr_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/testlib/
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/testlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36122 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr/utils/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-15 14:08:33.000000 omero-mapr-0.5.2/omero_mapr/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-15 14:08:33.000000 omero-mapr-0.5.2/omero_mapr/utils/__pycache__/version.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    23406 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/omero_mapr/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:08:33.567534 omero-mapr-0.5.2/omero_mapr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-15 14:08:33.000000 omero-mapr-0.5.2/omero_mapr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-15 14:08:33.000000 omero-mapr-0.5.2/omero_mapr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:08:33.000000 omero-mapr-0.5.2/omero_mapr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:08:33.000000 omero-mapr-0.5.2/omero_mapr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 14:08:33.000000 omero-mapr-0.5.2/omero_mapr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 14:08:33.000000 omero-mapr-0.5.2/omero_mapr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-15 14:08:33.571534 omero-mapr-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-15 14:08:31.000000 omero-mapr-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/
+-rw-r--r--   0 runner    (1001) docker     (121)    34520 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7994 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6760 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/
+-rw-r--r--   0 runner    (1001) docker     (121)     1021 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-03-15 11:58:52.000000 omero-mapr-0.5rc1/omero_mapr/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/custom_context_processor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2610 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/mapr_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11297 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/show.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.650572 omero-mapr-0.5rc1/omero_mapr/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.650572 omero-mapr-0.5rc1/omero_mapr/static/mapr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/static/mapr/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/css/ome.mapr.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/static/mapr/image/
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/image/compound_icon_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/image/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3539 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/image/gene_icon_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (121)     3419 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/image/organism_icon_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/image/phenotype_icon_16x16.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/image/sirna_icon_16x16.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/static/mapr/javascript/
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/javascript/center_plugin.thumbs.js
+-rw-r--r--   0 runner    (1001) docker     (121)     5812 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/javascript/ome.mapr.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3667 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/static/mapr/javascript/ome.mapr.ui.autocomplete.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.650572 omero-mapr-0.5rc1/omero_mapr/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/templates/mapr/
+-rw-r--r--   0 runner    (1001) docker     (121)     5584 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/templates/mapr/base_mapr.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/templates/mapr/metadata_general.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.650572 omero-mapr-0.5rc1/omero_mapr/templates/webclient/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.650572 omero-mapr-0.5rc1/omero_mapr/templates/webclient/data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/templates/webclient/data/includes/
+-rw-r--r--   0 runner    (1001) docker     (121)    12399 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/templates/webclient/data/includes/right_plugin.general.js.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/templatetags/mapr_filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/templatetags/mapr_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/testlib/
+-rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/testlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36122 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr/utils/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-03-15 11:58:52.000000 omero-mapr-0.5rc1/omero_mapr/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2022-03-15 11:58:52.000000 omero-mapr-0.5rc1/omero_mapr/utils/__pycache__/version.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23406 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/omero_mapr/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/omero_mapr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7994 2022-03-15 11:58:52.000000 omero-mapr-0.5rc1/omero_mapr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-03-15 11:58:52.000000 omero-mapr-0.5rc1/omero_mapr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 11:58:52.000000 omero-mapr-0.5rc1/omero_mapr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-15 11:58:52.000000 omero-mapr-0.5rc1/omero_mapr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-15 11:58:52.000000 omero-mapr-0.5rc1/omero_mapr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-15 11:58:52.000000 omero-mapr-0.5rc1/omero_mapr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-03-15 11:58:52.654572 omero-mapr-0.5rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2914 2022-03-15 11:58:50.000000 omero-mapr-0.5rc1/setup.py
```

### Comparing `omero-mapr-0.5.2/LICENSE` & `omero-mapr-0.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/PKG-INFO` & `omero-mapr-0.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omero-mapr
-Version: 0.5.2
+Version: 0.5rc1
 Summary: MAPR is a Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-mapr
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPLv3
-Download-URL: https://github.com/ome/omero-mapr/tarball/0.5.2
+Download-URL: https://github.com/ome/omero-mapr/tarball/0.5rc1
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `omero-mapr-0.5.2/README.rst` & `omero-mapr-0.5rc1/README.rst`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/__init__.py` & `omero-mapr-0.5rc1/omero_mapr/apps.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Author: Aleksandra Tarkowska <A(dot)Tarkowska(at)dundee(dot)ac(dot)uk>, 2008.
 #
 # Version: 1.0
 
+from django.apps import AppConfig
+from django.utils.version import get_complete_version
 
-from omero_mapr.utils.version import get_version
+if get_complete_version() < (3, 2):
+    raise RuntimeError('MAPR requires Django 3.2+')
 
 
-VERSION = "0.5.2"
-
-__version__ = get_version(VERSION)
-
-default_app_config = 'omero_mapr.apps.MaprAppConfig'
+class MaprAppConfig(AppConfig):
+    name = "omero_mapr"
+    label = "mapr"
```

### Comparing `omero-mapr-0.5.2/omero_mapr/apps.py` & `omero-mapr-0.5rc1/omero_mapr/templatetags/mapr_tags.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
+# #!/usr/bin/env python
 #
 #
 #
 # Copyright (c) 2016 University of Dundee.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
@@ -17,18 +18,24 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Author: Aleksandra Tarkowska <A(dot)Tarkowska(at)dundee(dot)ac(dot)uk>, 2008.
 #
 # Version: 1.0
+#
+
+import logging
+import json
+
+from django import template
+from django.utils.safestring import mark_safe
+from ..mapr_settings import mapr_settings
 
-from django.apps import AppConfig
-from django.utils.version import get_complete_version
+register = template.Library()
 
-if get_complete_version() < (3, 2):
-    raise RuntimeError('MAPR requires Django 3.2+')
+logger = logging.getLogger(__name__)
 
 
-class MaprAppConfig(AppConfig):
-    name = "omero_mapr"
-    label = "mapr"
+@register.simple_tag
+def mapr_menu_config():
+    return mark_safe(json.dumps(mapr_settings.CONFIG))
```

### Comparing `omero-mapr-0.5.2/omero_mapr/mapr_settings.py` & `omero-mapr-0.5rc1/omero_mapr/mapr_settings.py`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/show.py` & `omero-mapr-0.5rc1/omero_mapr/show.py`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/static/mapr/css/ome.mapr.css` & `omero-mapr-0.5rc1/omero_mapr/static/mapr/css/ome.mapr.css`

 * *Files 11% similar despite different names*

```diff
@@ -22,22 +22,14 @@
     background: #D4D6D8;
 }
 
 .ui-menu-item a{
     background:#ffffff;
     font-size: 10px;
     width: 135px;
-    /* https://github.com/ome/omero-web/pull/433#issuecomment-1396774881 */
-    display: block;
-}
-
-/* removed in jquery-ui 1.13.2, but we still want this */
-.ui-menu-item a.ui-state-active {
-    background: #D4D6D8;
-    margin: 0;
 }
 
 #autocompletesearch {
     /* override .filtersearch width from webclient */
     width: 180px;
 }
```

### Comparing `omero-mapr-0.5.2/omero_mapr/static/mapr/image/compound_icon_16x16.png` & `omero-mapr-0.5rc1/omero_mapr/static/mapr/image/compound_icon_16x16.png`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/static/mapr/image/gene_icon_16x16.png` & `omero-mapr-0.5rc1/omero_mapr/static/mapr/image/gene_icon_16x16.png`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/static/mapr/image/organism_icon_16x16.png` & `omero-mapr-0.5rc1/omero_mapr/static/mapr/image/organism_icon_16x16.png`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/static/mapr/image/phenotype_icon_16x16.png` & `omero-mapr-0.5rc1/omero_mapr/static/mapr/image/phenotype_icon_16x16.png`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/static/mapr/image/sirna_icon_16x16.png` & `omero-mapr-0.5rc1/omero_mapr/static/mapr/image/sirna_icon_16x16.png`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/static/mapr/javascript/center_plugin.thumbs.js` & `omero-mapr-0.5rc1/omero_mapr/static/mapr/javascript/center_plugin.thumbs.js`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/static/mapr/javascript/ome.mapr.js` & `omero-mapr-0.5rc1/omero_mapr/static/mapr/javascript/ome.mapr.js`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/static/mapr/javascript/ome.mapr.ui.autocomplete.js` & `omero-mapr-0.5rc1/omero_mapr/static/mapr/javascript/ome.mapr.ui.autocomplete.js`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/templates/mapr/base_mapr.html` & `omero-mapr-0.5rc1/omero_mapr/templates/mapr/base_mapr.html`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/templates/mapr/metadata_general.html` & `omero-mapr-0.5rc1/omero_mapr/templates/mapr/metadata_general.html`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/templates/webclient/data/includes/right_plugin.general.js.html` & `omero-mapr-0.5rc1/omero_mapr/templates/webclient/data/includes/right_plugin.general.js.html`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/templatetags/mapr_filters.py` & `omero-mapr-0.5rc1/omero_mapr/templatetags/mapr_filters.py`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/templatetags/mapr_tags.py` & `omero-mapr-0.5rc1/omero_mapr/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# #!/usr/bin/env python
 #
 #
 #
 # Copyright (c) 2016 University of Dundee.
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU Affero General Public License as
@@ -18,24 +17,17 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Author: Aleksandra Tarkowska <A(dot)Tarkowska(at)dundee(dot)ac(dot)uk>, 2008.
 #
 # Version: 1.0
-#
 
-import logging
-import json
 
-from django import template
-from django.utils.safestring import mark_safe
-from ..mapr_settings import mapr_settings
+from omero_mapr.utils.version import get_version
 
-register = template.Library()
 
-logger = logging.getLogger(__name__)
+VERSION = (0, 5, 0, "rc1")
 
+__version__ = get_version(VERSION)
 
-@register.simple_tag
-def mapr_menu_config():
-    return mark_safe(json.dumps(mapr_settings.CONFIG))
+default_app_config = 'omero_mapr.apps.MaprAppConfig'
```

### Comparing `omero-mapr-0.5.2/omero_mapr/testlib/__init__.py` & `omero-mapr-0.5rc1/omero_mapr/testlib/__init__.py`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/tree.py` & `omero-mapr-0.5rc1/omero_mapr/tree.py`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/urls.py` & `omero-mapr-0.5rc1/omero_mapr/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Author: Aleksandra Tarkowska <A(dot)Tarkowska(at)dundee(dot)ac(dot)uk>,
 #
 # Version: 1.0
 
 from . import views
-from django.urls import re_path
+from django.conf.urls import url
 from django.urls import reverse
 from django.utils.functional import lazy
 from django.views.generic import RedirectView
 from django.views.decorators.cache import never_cache
 
 from .mapr_settings import mapr_settings
 
@@ -36,65 +36,65 @@
 DEFAULT_CONFIG = list(mapr_settings.CONFIG.keys())[0]
 
 urlpatterns = []
 
 # alias
 for m in mapr_settings.CONFIG:
     urlpatterns.append(
-        re_path(r'^%s/$' % m,
-                views.index, {'menu': m},
-                name="maprindex_%s" % m)
+        url(r'^%s/$' % m,
+            views.index, {'menu': m},
+            name="maprindex_%s" % m)
         )
 
 urlpatterns += [
 
     # core
-    re_path(r'^$', never_cache(
-            RedirectView.as_view(
-                url=reverse_lazy('maprindex_%s' % DEFAULT_CONFIG),
-                permanent=True,
-                query_string=True)),
-            name="maprindex"),
-
-    re_path(r'^api/config/$', views.api_mapr_config, name='mapr_config'),
-
-    re_path(r'^api/(?P<menu>%s)/count/$' % (CONFIG_REGEX),
-            views.api_experimenter_list,
-            name='mapannotations_api_experimenters'),
-    re_path(r'^api/(?P<menu>%s)/datasets/$' % CONFIG_REGEX,
-            views.api_datasets_list,
-            name='mapannotations_api_datasets'),
-    re_path(r'^api/(?P<menu>%s)/plates/$' % CONFIG_REGEX,
-            views.api_plate_list,
-            name='mapannotations_api_plates'),
-    re_path(r'^api/(?P<menu>%s)/images/$' % CONFIG_REGEX,
-            views.api_image_list,
-            name='mapannotations_api_images'),
-
-    re_path(r'^api/(?P<menu>%s)/paths_to_object/$' % CONFIG_REGEX,
-            views.api_paths_to_object,
-            name='mapannotations_api_paths_to_object'),
-
-    re_path(r'^metadata_details/(?P<c_type>%s)/$' % CONFIG_REGEX,
-            views.load_metadata_details,
-            name="mapannotations_load_metadata_details"),
-
-    re_path(r'^api/(?P<menu>%s)/annotations/$' % CONFIG_REGEX,
-            views.api_annotations,
-            name='mapannotations_api_annotations'),
+    url(r'^$', never_cache(
+        RedirectView.as_view(
+            url=reverse_lazy('maprindex_%s' % DEFAULT_CONFIG),
+            permanent=True,
+            query_string=True)),
+        name="maprindex"),
+
+    url(r'^api/config/$', views.api_mapr_config, name='mapr_config'),
+
+    url(r'^api/(?P<menu>%s)/count/$' % (CONFIG_REGEX),
+        views.api_experimenter_list,
+        name='mapannotations_api_experimenters'),
+    url(r'^api/(?P<menu>%s)/datasets/$' % CONFIG_REGEX,
+        views.api_datasets_list,
+        name='mapannotations_api_datasets'),
+    url(r'^api/(?P<menu>%s)/plates/$' % CONFIG_REGEX,
+        views.api_plate_list,
+        name='mapannotations_api_plates'),
+    url(r'^api/(?P<menu>%s)/images/$' % CONFIG_REGEX,
+        views.api_image_list,
+        name='mapannotations_api_images'),
+
+    url(r'^api/(?P<menu>%s)/paths_to_object/$' % CONFIG_REGEX,
+        views.api_paths_to_object,
+        name='mapannotations_api_paths_to_object'),
+
+    url(r'^metadata_details/(?P<c_type>%s)/$' % CONFIG_REGEX,
+        views.load_metadata_details,
+        name="mapannotations_load_metadata_details"),
+
+    url(r'^api/(?P<menu>%s)/annotations/$' % CONFIG_REGEX,
+        views.api_annotations,
+        name='mapannotations_api_annotations'),
 
     # must be last on the list
-    re_path(r'^api/(?P<menu>%s)/$' % CONFIG_REGEX,
-            views.api_mapannotation_list,
-            name='mapannotations_api_mapannotations'),
+    url(r'^api/(?P<menu>%s)/$' % CONFIG_REGEX,
+        views.api_mapannotation_list,
+        name='mapannotations_api_mapannotations'),
 
     # autocomplete
-    re_path(r'^api/autocomplete/(?P<menu>%s)/$' % CONFIG_REGEX,
-            views.mapannotations_autocomplete,
-            name='mapannotations_autocomplete'),
+    url(r'^api/autocomplete/(?P<menu>%s)/$' % CONFIG_REGEX,
+        views.mapannotations_autocomplete,
+        name='mapannotations_autocomplete'),
 
     # favicon
-    re_path(r'^favicon/$',
-            views.mapannotations_favicon,
-            name='mapannotations_favicon'),
+    url(r'^favicon/$',
+        views.mapannotations_favicon,
+        name='mapannotations_favicon'),
 
 ]
```

### Comparing `omero-mapr-0.5.2/omero_mapr/utils/__init__.py` & `omero-mapr-0.5rc1/omero_mapr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr/utils/__pycache__/version.cpython-310.pyc` & `omero-mapr-0.5rc1/omero_mapr/utils/__pycache__/version.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 15 14:08:31 2023 UTC, .py size: 1235 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,56 @@
-00000000: 6f0d 0d0a 0000 0000 5f1b 8b64 d304 0000  o......._..d....
+00000000: 6f0d 0d0a 0000 0000 7a7f 3062 8805 0000  o.......z.0b....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1800 0000 6405  .....@...s....d.
 00000030: 6401 6402 8401 5a00 6405 6403 6404 8401  d.d...Z.d.d.d...
 00000040: 5a01 6400 5300 2906 4e63 0100 0000 0000  Z.d.S.).Nc......
-00000050: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00000060: 0000 7308 0000 0074 007c 0083 0153 0029  ..s....t.|...S.)
-00000070: 017a 670a 2020 2020 5265 7475 726e 7320  .zg.    Returns 
-00000080: 6120 5045 5020 3338 362d 636f 6d70 6c69  a PEP 386-compli
-00000090: 616e 7420 7665 7273 696f 6e20 6e75 6d62  ant version numb
-000000a0: 6572 2e0a 2020 2020 5365 6520 6874 7470  er..    See http
-000000b0: 733a 2f2f 7777 772e 7079 7468 6f6e 2e6f  s://www.python.o
-000000c0: 7267 2f64 6576 2f70 6570 732f 7065 702d  rg/dev/peps/pep-
-000000d0: 3034 3430 2f0a 2020 2020 2901 da10 6765  0440/.    )...ge
-000000e0: 745f 6675 6c6c 5f76 6572 7369 6f6e a901  t_full_version..
-000000f0: da07 7665 7273 696f 6ea9 0072 0400 0000  ..version..r....
-00000100: fa43 2f68 6f6d 652f 7275 6e6e 6572 2f77  .C/home/runner/w
-00000110: 6f72 6b2f 6f6d 6572 6f2d 6d61 7072 2f6f  ork/omero-mapr/o
-00000120: 6d65 726f 2d6d 6170 722f 6f6d 6572 6f5f  mero-mapr/omero_
-00000130: 6d61 7072 2f75 7469 6c73 2f76 6572 7369  mapr/utils/versi
-00000140: 6f6e 2e70 79da 0b67 6574 5f76 6572 7369  on.py..get_versi
-00000150: 6f6e 1a00 0000 7302 0000 0008 0772 0600  on....s......r..
-00000160: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00000170: 0000 0002 0000 0043 0000 0073 1800 0000  .......C...s....
-00000180: 7c00 6401 7500 720a 6402 6403 6c00 6d01  |.d.u.r.d.d.l.m.
-00000190: 7d00 0100 7c00 5300 2904 7a2e 0a20 2020  }...|.S.).z..   
-000001a0: 2052 6574 7572 6e73 2061 2074 7570 6c65   Returns a tuple
-000001b0: 206f 6620 7468 6520 6d61 7072 2076 6572   of the mapr ver
-000001c0: 7369 6f6e 2e0a 2020 2020 4ee9 0000 0000  sion..    N.....
-000001d0: 2901 da07 5645 5253 494f 4e29 02da 0a6f  )...VERSION)...o
-000001e0: 6d65 726f 5f6d 6170 7272 0800 0000 7202  mero_maprr....r.
-000001f0: 0000 0072 0400 0000 7204 0000 0072 0500  ...r....r....r..
-00000200: 0000 7201 0000 0024 0000 0073 0600 0000  ..r....$...s....
-00000210: 0806 0c01 0401 7201 0000 0029 014e 2902  ......r....).N).
-00000220: 7206 0000 0072 0100 0000 7204 0000 0072  r....r....r....r
-00000230: 0400 0000 7204 0000 0072 0500 0000 da08  ....r....r......
-00000240: 3c6d 6f64 756c 653e 0100 0000 7304 0000  <module>....s...
-00000250: 000a 190e 0a                             .....
+00000050: 0000 0000 0000 0300 0000 0600 0000 4300  ..............C.
+00000060: 0000 735c 0000 0074 007c 0083 017d 007c  ..s\...t.|...}.|
+00000070: 0064 0119 0064 026b 0272 0c64 016e 0164  .d...d.k.r.d.n.d
+00000080: 037d 0164 04a0 0164 0564 0684 007c 0064  .}.d...d.d...|.d
+00000090: 077c 0185 0219 0044 0083 01a1 017d 0274  .|.....D.....}.t
+000000a0: 027c 0083 0164 036b 0472 2a64 087c 027c  .|...d.k.r*d.|.|
+000000b0: 0064 0319 0066 0216 007d 0274 037c 0283  .d...f...}.t.|..
+000000c0: 0153 0029 097a 670a 2020 2020 5265 7475  .S.).zg.    Retu
+000000d0: 726e 7320 6120 5045 5020 3338 362d 636f  rns a PEP 386-co
+000000e0: 6d70 6c69 616e 7420 7665 7273 696f 6e20  mpliant version 
+000000f0: 6e75 6d62 6572 2e0a 2020 2020 5365 6520  number..    See 
+00000100: 6874 7470 733a 2f2f 7777 772e 7079 7468  https://www.pyth
+00000110: 6f6e 2e6f 7267 2f64 6576 2f70 6570 732f  on.org/dev/peps/
+00000120: 7065 702d 3034 3430 2f0a 2020 2020 e902  pep-0440/.    ..
+00000130: 0000 00e9 0000 0000 e903 0000 00da 012e  ................
+00000140: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000150: 0003 0000 0073 0000 0073 1800 0000 8100  .....s...s......
+00000160: 7c00 5d07 7d01 7400 7c01 8301 5600 0100  |.].}.t.|...V...
+00000170: 7102 6400 5300 a901 4e29 01da 0373 7472  q.d.S...N)...str
+00000180: 2902 da02 2e30 da01 78a9 0072 0900 0000  )....0..x..r....
+00000190: fa43 2f68 6f6d 652f 7275 6e6e 6572 2f77  .C/home/runner/w
+000001a0: 6f72 6b2f 6f6d 6572 6f2d 6d61 7072 2f6f  ork/omero-mapr/o
+000001b0: 6d65 726f 2d6d 6170 722f 6f6d 6572 6f5f  mero-mapr/omero_
+000001c0: 6d61 7072 2f75 7469 6c73 2f76 6572 7369  mapr/utils/versi
+000001d0: 6f6e 2e70 79da 093c 6765 6e65 7870 723e  on.py..<genexpr>
+000001e0: 2300 0000 7304 0000 0002 8016 007a 1e67  #...s........z.g
+000001f0: 6574 5f76 6572 7369 6f6e 2e3c 6c6f 6361  et_version.<loca
+00000200: 6c73 3e2e 3c67 656e 6578 7072 3e4e 7a04  ls>.<genexpr>Nz.
+00000210: 2573 2573 2904 da10 6765 745f 6675 6c6c  %s%s)...get_full
+00000220: 5f76 6572 7369 6f6e da04 6a6f 696e da03  _version..join..
+00000230: 6c65 6e72 0600 0000 2903 da07 7665 7273  lenr....)...vers
+00000240: 696f 6eda 0570 6172 7473 da03 7265 7372  ion..parts..resr
+00000250: 0900 0000 7209 0000 0072 0a00 0000 da0b  ....r....r......
+00000260: 6765 745f 7665 7273 696f 6e1a 0000 0073  get_version....s
+00000270: 0c00 0000 0807 1401 1c01 0c01 1001 0801  ................
+00000280: 7212 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00000290: 0000 0100 0000 0200 0000 4300 0000 7318  ..........C...s.
+000002a0: 0000 007c 0064 0175 0072 0a64 0264 036c  ...|.d.u.r.d.d.l
+000002b0: 006d 017d 0001 007c 0053 0029 047a 2e0a  .m.}...|.S.).z..
+000002c0: 2020 2020 5265 7475 726e 7320 6120 7475      Returns a tu
+000002d0: 706c 6520 6f66 2074 6865 206d 6170 7220  ple of the mapr 
+000002e0: 7665 7273 696f 6e2e 0a20 2020 204e 7202  version..    Nr.
+000002f0: 0000 0029 01da 0756 4552 5349 4f4e 2902  ...)...VERSION).
+00000300: da0a 6f6d 6572 6f5f 6d61 7072 7213 0000  ..omero_maprr...
+00000310: 0029 0172 0f00 0000 7209 0000 0072 0900  .).r....r....r..
+00000320: 0000 720a 0000 0072 0c00 0000 2900 0000  ..r....r....)...
+00000330: 7306 0000 0008 060c 0104 0172 0c00 0000  s..........r....
+00000340: 7205 0000 0029 0272 1200 0000 720c 0000  r....).r....r...
+00000350: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
+00000360: 720a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000370: 0000 0073 0400 0000 0a19 0e0f            ...s........
```

### Comparing `omero-mapr-0.5.2/omero_mapr/utils/version.py` & `omero-mapr-0.5rc1/omero_mapr/utils/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,20 @@
 def get_version(version=None):
 
     """
     Returns a PEP 386-compliant version number.
     See https://www.python.org/dev/peps/pep-0440/
     """
 
-    return get_full_version(version)
+    version = get_full_version(version)
+    parts = 2 if version[2] == 0 else 3
+    res = '.'.join(str(x) for x in version[:parts])
+    if len(version) > 3:
+        res = "%s%s" % (res, version[3])
+    return str(res)
 
 
 def get_full_version(version=None):
 
     """
     Returns a tuple of the mapr version.
     """
```

### Comparing `omero-mapr-0.5.2/omero_mapr/views.py` & `omero-mapr-0.5rc1/omero_mapr/views.py`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/omero_mapr.egg-info/PKG-INFO` & `omero-mapr-0.5rc1/omero_mapr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omero-mapr
-Version: 0.5.2
+Version: 0.5rc1
 Summary: MAPR is a Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-mapr
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPLv3
-Download-URL: https://github.com/ome/omero-mapr/tarball/0.5.2
+Download-URL: https://github.com/ome/omero-mapr/tarball/0.5rc1
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `omero-mapr-0.5.2/omero_mapr.egg-info/SOURCES.txt` & `omero-mapr-0.5rc1/omero_mapr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omero-mapr-0.5.2/setup.py` & `omero-mapr-0.5rc1/setup.py`

 * *Files identical despite different names*

