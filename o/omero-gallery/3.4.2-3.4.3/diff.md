# Comparing `tmp/omero-gallery-3.4.2.tar.gz` & `tmp/omero-gallery-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-gallery-3.4.2.tar", last modified: Wed Mar 16 16:58:14 2022, max compression
+gzip compressed data, was "omero-gallery-3.4.3.tar", last modified: Thu Jun 15 13:32:54 2023, max compression
```

## Comparing `omero-gallery-3.4.2.tar` & `omero-gallery-3.4.3.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)    34501 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9876 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8701 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.309639 omero-gallery-3.4.2/omero_gallery/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     5815 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/gallery_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.305639 omero-gallery-3.4.2/omero_gallery/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.309639 omero-gallery-3.4.2/omero_gallery/static/gallery/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.305639 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.305639 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.309639 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/
--rw-r--r--   0 runner    (1001) docker     (121)    14936 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (121)    38388 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css.map
--rw-r--r--   0 runner    (1001) docker     (121)    13185 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.min.css
--rw-r--r--   0 runner    (1001) docker     (121)   121220 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (121)   245960 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (121)    99961 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)    20335 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (121)    62927 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (121)    41280 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    23320 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/
--rw-r--r--   0 runner    (1001) docker     (121)    55258 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (121)    29110 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/foundation/
--rw-r--r--   0 runner    (1001) docker     (121)    78738 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/foundation/foundation.min.css
--rw-r--r--   0 runner    (1001) docker     (121)   107910 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/foundation/foundation.min.js
--rw-r--r--   0 runner    (1001) docker     (121)    12824 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/categories.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/omero_gallery/static/gallery/css/
--rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/css/idr.css
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/css/openmicroscopy.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/omero_gallery/static/gallery/images/
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/images/omero.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2934 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/images/transparent.png
--rw-r--r--   0 runner    (1001) docker     (121)    18924 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/model.js
--rw-r--r--   0 runner    (1001) docker     (121)    25244 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/search.js
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/static/gallery/studies.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.309639 omero-gallery-3.4.2/omero_gallery/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/omero_gallery/templates/webgallery/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/omero_gallery/templates/webgallery/base/
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/base/base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/omero_gallery/templates/webgallery/categories/
--rw-r--r--   0 runner    (1001) docker     (121)     7166 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/categories/base.html
--rw-r--r--   0 runner    (1001) docker     (121)     3500 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/categories/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/categories/search.html
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/dataset_thumbs.html
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/index.html
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/show_dataset.html
--rw-r--r--   0 runner    (1001) docker     (121)     3503 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/show_group.html
--rw-r--r--   0 runner    (1001) docker     (121)     2846 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/show_image.html
--rw-r--r--   0 runner    (1001) docker     (121)     1609 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/templates/webgallery/show_project.html
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)    15224 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/omero_gallery/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 16:58:14.309639 omero-gallery-3.4.2/omero_gallery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9876 2022-03-16 16:58:14.000000 omero-gallery-3.4.2/omero_gallery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2470 2022-03-16 16:58:14.000000 omero-gallery-3.4.2/omero_gallery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 16:58:14.000000 omero-gallery-3.4.2/omero_gallery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 16:58:14.000000 omero-gallery-3.4.2/omero_gallery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-03-16 16:58:14.000000 omero-gallery-3.4.2/omero_gallery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-16 16:58:14.000000 omero-gallery-3.4.2/omero_gallery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-03-16 16:58:14.313639 omero-gallery-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-03-16 16:58:11.000000 omero-gallery-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.686387 omero-gallery-3.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34501 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-15 13:32:54.686387 omero-gallery-3.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.678387 omero-gallery-3.4.3/omero_gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/gallery_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.678387 omero-gallery-3.4.3/omero_gallery/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.682387 omero-gallery-3.4.3/omero_gallery/static/gallery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.678387 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.678387 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.682387 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    14936 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)    38388 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   121220 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   245960 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    99961 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.682387 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    62927 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41280 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.682387 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    55258 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29110 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.682387 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/foundation/
+-rw-r--r--   0 runner    (1001) docker     (123)    78738 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/foundation/foundation.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   107910 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/foundation/foundation.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/categories.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.682387 omero-gallery-3.4.3/omero_gallery/static/gallery/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/css/idr.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/css/openmicroscopy.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.686387 omero-gallery-3.4.3/omero_gallery/static/gallery/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/images/omero.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/images/transparent.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18924 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/model.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25244 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/search.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/static/gallery/studies.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.678387 omero-gallery-3.4.3/omero_gallery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.686387 omero-gallery-3.4.3/omero_gallery/templates/webgallery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.686387 omero-gallery-3.4.3/omero_gallery/templates/webgallery/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/base/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.686387 omero-gallery-3.4.3/omero_gallery/templates/webgallery/categories/
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/categories/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/categories/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/categories/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/dataset_thumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/show_dataset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/show_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/show_image.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/templates/webgallery/show_project.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15224 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/omero_gallery/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:54.682387 omero-gallery-3.4.3/omero_gallery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-06-15 13:32:54.000000 omero-gallery-3.4.3/omero_gallery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-15 13:32:54.000000 omero-gallery-3.4.3/omero_gallery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:32:54.000000 omero-gallery-3.4.3/omero_gallery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:32:54.000000 omero-gallery-3.4.3/omero_gallery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 13:32:54.000000 omero-gallery-3.4.3/omero_gallery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 13:32:54.000000 omero-gallery-3.4.3/omero_gallery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 13:32:54.686387 omero-gallery-3.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-15 13:32:49.000000 omero-gallery-3.4.3/setup.py
```

### Comparing `omero-gallery-3.4.2/LICENSE` & `omero-gallery-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/PKG-INFO` & `omero-gallery-3.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omero-gallery
-Version: 3.4.2
+Version: 3.4.3
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-gallery
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-gallery/archive/v3.4.2.tar.gz
+Download-URL: https://github.com/ome/omero-gallery/archive/v3.4.3.tar.gz
 Keywords: OMERO.web,plugin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omero-gallery-3.4.2/README.rst` & `omero-gallery-3.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/apps.py` & `omero-gallery-3.4.3/omero_gallery/apps.py`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/gallery_settings.py` & `omero-gallery-3.4.3/omero_gallery/gallery_settings.py`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css.map` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.min.css` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css.map` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.min.css` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.eot` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.svg` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.ttf` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.woff` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.js` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.min.js` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/bootstrap-3.1.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/foundation/foundation.min.css` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/foundation/foundation.min.css`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/3rdparty/foundation/foundation.min.js` & `omero-gallery-3.4.3/omero_gallery/static/gallery/3rdparty/foundation/foundation.min.js`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/categories.js` & `omero-gallery-3.4.3/omero_gallery/static/gallery/categories.js`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/css/idr.css` & `omero-gallery-3.4.3/omero_gallery/static/gallery/css/idr.css`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/css/openmicroscopy.css` & `omero-gallery-3.4.3/omero_gallery/static/gallery/css/openmicroscopy.css`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/images/favicon.ico` & `omero-gallery-3.4.3/omero_gallery/static/gallery/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/images/omero.svg` & `omero-gallery-3.4.3/omero_gallery/static/gallery/images/omero.svg`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/images/transparent.png` & `omero-gallery-3.4.3/omero_gallery/static/gallery/images/transparent.png`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/model.js` & `omero-gallery-3.4.3/omero_gallery/static/gallery/model.js`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/search.js` & `omero-gallery-3.4.3/omero_gallery/static/gallery/search.js`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/static/gallery/studies.css` & `omero-gallery-3.4.3/omero_gallery/static/gallery/studies.css`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/templates/webgallery/base/base.html` & `omero-gallery-3.4.3/omero_gallery/templates/webgallery/base/base.html`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/templates/webgallery/categories/base.html` & `omero-gallery-3.4.3/omero_gallery/templates/webgallery/categories/base.html`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/templates/webgallery/categories/index.html` & `omero-gallery-3.4.3/omero_gallery/templates/webgallery/categories/index.html`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/templates/webgallery/categories/search.html` & `omero-gallery-3.4.3/omero_gallery/templates/webgallery/categories/search.html`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/templates/webgallery/index.html` & `omero-gallery-3.4.3/omero_gallery/templates/webgallery/index.html`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/templates/webgallery/show_dataset.html` & `omero-gallery-3.4.3/omero_gallery/templates/webgallery/show_dataset.html`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/templates/webgallery/show_group.html` & `omero-gallery-3.4.3/omero_gallery/templates/webgallery/show_group.html`

 * *Files 3% similar despite different names*

```diff
@@ -70,23 +70,23 @@
 
 <!--         User:
         <select id="users_chooser">
             <option value="-1">All Members</option>
             {% if group_owners %}
                 <optgroup label="Owners">
                 {% for user in group_owners %}
-                    <option value="{{ user.id }}" {% ifequal user.id ome.user_id %}selected{% endifequal %}>
+                    <option value="{{ user.id }}" {% if user.id == ome.user_id %}selected{% endif %}>
                         {{ user.getFullName }}
                     </option>
                 {% endfor %}
             {% endif %}
             {% if group_members %}
                 <optgroup label="Members">
                 {% for user in group_members %}
-                    <option value="{{ user.id }}" {% ifequal user.id ome.user_id %}selected{% endifequal %}>
+                    <option value="{{ user.id }}" {% if user.id == ome.user_id %}selected{% endif %}>
                         {{ user.getFullName }}
                     </option>
                 {% endfor %}
             {% endif %}
         </select> -->
 
     <!-- Adding Scripts - First we link to the 'current' jQuery used by OMERO.web -->
```

### Comparing `omero-gallery-3.4.2/omero_gallery/templates/webgallery/show_image.html` & `omero-gallery-3.4.3/omero_gallery/templates/webgallery/show_image.html`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/templates/webgallery/show_project.html` & `omero-gallery-3.4.3/omero_gallery/templates/webgallery/show_project.html`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery/urls.py` & `omero-gallery-3.4.3/omero_gallery/urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-from django.conf.urls import url
+from django.urls import re_path
 from .gallery_settings import SUPER_CATEGORIES
 
 from . import views
 
 urlpatterns = [
     # index 'home page' of the webgallery app
-    url(r'^$', views.index, name='webgallery_index'),
+    re_path(r'^$', views.index, name='webgallery_index'),
 
     # All settings as JSON
-    url(r'^gallery_settings/$', views.gallery_settings),
+    re_path(r'^gallery_settings/$', views.gallery_settings),
 
     # group view
-    url(r'show_group/(?P<group_id>[0-9]+)/$',
-        views.show_group,
-        name='webgallery_show_group'),
+    re_path(r'show_group/(?P<group_id>[0-9]+)/$',
+            views.show_group,
+            name='webgallery_show_group'),
 
     # project view
-    url(r'show_project/(?P<project_id>[0-9]+)/$',
-        views.show_project,
-        name='webgallery_show_project'),
+    re_path(r'show_project/(?P<project_id>[0-9]+)/$',
+            views.show_project,
+            name='webgallery_show_project'),
 
     # dataset view
-    url(r'show_dataset/(?P<dataset_id>[0-9]+)/$',
-        views.show_dataset,
-        name='webgallery_show_dataset'),
+    re_path(r'show_dataset/(?P<dataset_id>[0-9]+)/$',
+            views.show_dataset,
+            name='webgallery_show_dataset'),
     # use the same dataset view, with a different
     # template that only shows thumbnails
-    url(r'dataset_thumbs/(?P<dataset_id>[0-9]+)/$',
-        views.show_dataset,
-        {'template': 'webgallery/dataset_thumbs.html'},
-        name='webgallery_dataset_thumbs'),
+    re_path(r'dataset_thumbs/(?P<dataset_id>[0-9]+)/$',
+            views.show_dataset,
+            {'template': 'webgallery/dataset_thumbs.html'},
+            name='webgallery_dataset_thumbs'),
 
     # image view
-    url(r'show_image/(?P<image_id>[0-9]+)/$',
-        views.show_image, name='webgallery_show_image'),
+    re_path(r'show_image/(?P<image_id>[0-9]+)/$',
+            views.show_image, name='webgallery_show_image'),
 
     # Search page shows Projects / Screens filtered by Map Annotation
-    url(r'^search/$', views.search, {'super_category': None}),
+    re_path(r'^search/$', views.search, {'super_category': None}),
 
     # list images within container. NB: not used but potentially useful
-    url(r'^gallery-api/(?P<obj_type>[screen|project]+)s/'
-        r'(?P<obj_id>[0-9]+)/images/$',
-        views.study_images, name='webgallery_study_image'),
+    re_path(r'^gallery-api/(?P<obj_type>[screen|project]+)s/'
+            r'(?P<obj_id>[0-9]+)/images/$',
+            views.study_images, name='webgallery_study_image'),
 
     # Supports e.g. ?project=1&project=2&screen=3
-    url(r'^gallery-api/thumbnails/$', views.api_thumbnails,
-        name='webgallery_api_thumbnails'),
+    re_path(r'^gallery-api/thumbnails/$', views.api_thumbnails,
+            name='webgallery_api_thumbnails'),
 ]
 
 for c in SUPER_CATEGORIES:
-    urlpatterns.append(url(r'^%s/$' % c, views.index, {'super_category': c},
-                           name="gallery_super_category"))
-    urlpatterns.append(url(r'^%s/search/$' % c, views.search,
-                           {'super_category': c}))
+    urlpatterns.append(re_path(r'^%s/$' % c, views.index,
+                               {'super_category': c},
+                               name="gallery_super_category"))
+    urlpatterns.append(re_path(r'^%s/search/$' % c, views.search,
+                               {'super_category': c}))
```

### Comparing `omero-gallery-3.4.2/omero_gallery/views.py` & `omero-gallery-3.4.3/omero_gallery/views.py`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/omero_gallery.egg-info/PKG-INFO` & `omero-gallery-3.4.3/omero_gallery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omero-gallery
-Version: 3.4.2
+Version: 3.4.3
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-gallery
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-gallery/archive/v3.4.2.tar.gz
+Download-URL: https://github.com/ome/omero-gallery/archive/v3.4.3.tar.gz
 Keywords: OMERO.web,plugin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omero-gallery-3.4.2/omero_gallery.egg-info/SOURCES.txt` & `omero-gallery-3.4.3/omero_gallery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omero-gallery-3.4.2/setup.py` & `omero-gallery-3.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
-VERSION = '3.4.2'
+VERSION = '3.4.3'
 HOMEPAGE = "https://github.com/ome/omero-gallery"
 
 setup(name="omero-gallery",
       packages=find_packages(exclude=['ez_setup']),
       version=VERSION,
       description="A Python plugin for OMERO.web",
       long_description=read('README.rst'),
```

