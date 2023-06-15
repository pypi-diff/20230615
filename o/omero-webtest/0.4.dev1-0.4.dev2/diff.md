# Comparing `tmp/omero-webtest-0.4.dev1.tar.gz` & `tmp/omero-webtest-0.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/omero-webtest-0.4.dev1.tar", last modified: Fri Nov 22 11:19:27 2019, max compression
+gzip compressed data, was "dist/omero-webtest-0.4.dev2.tar", last modified: Thu Jan  9 10:52:52 2020, max compression
```

## Comparing `omero-webtest-0.4.dev1.tar` & `omero-webtest-0.4.dev2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3870 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3870 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     2624 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest.egg-info/SOURCES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/static/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/channel_overlay/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2998 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/channel_overlay/plus12.png
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2985 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/channel_overlay/minus12.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     2992 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/channel_overlay-16.png
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3400 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/figure_icon-16.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     6182 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/background.png
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/js/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2425 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/static/webtest/js/image_dims.js
--rw-rw-r--   0 travis    (2000) travis    (2000)     4063 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/templates/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/dataset.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8715 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/examples/embed_viewer.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1245 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/examples/plate_viewer.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    15733 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/examples/embed_external_rois.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5974 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/examples/embed_big_image.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3650 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/index.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)      316 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/util/add_annotations.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/image_rois.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    12739 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/static_example.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     7505 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/split_view_figure.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4236 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/render_performance.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3367 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/image_dimensions.html
--rw-rw-r--   0 travis    (2000) travis    (2000)    12235 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/channel_overlay_viewer.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/base_header.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2290 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/base_main.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/base_frame.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/container2.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5221 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/container3.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/base_html.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2035 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/webclient_base_container.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1209 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/right_plugin.rois.js.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4140 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/center_plugin.fullviewer.js.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2783 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/center_plugin.overlay.js.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2716 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/split_view_fig_include.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/dataset_split_include.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     5860 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/split_view_figure.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3529 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/dataset_split_view.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2180 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/center_plugin.splitview.js.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3200 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/center_plugin.fullviewer.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      379 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/templates/webtest/stack_preview.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      975 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/apps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26762 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/omero_webtest/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-11-22 11:19:27.000000 omero-webtest-0.4.dev1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    34501 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2085 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2760 2019-11-22 11:14:46.000000 omero-webtest-0.4.dev1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3494 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3494 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2660 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest.egg-info/requires.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/static/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/channel_overlay/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2998 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/channel_overlay/plus12.png
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2985 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/channel_overlay/minus12.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2992 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/channel_overlay-16.png
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3400 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/figure_icon-16.png
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6182 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/background.png
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/js/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2425 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/static/webtest/js/image_dims.js
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4063 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/templates/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      342 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/dataset.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8715 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/examples/embed_viewer.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1245 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/examples/plate_viewer.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15733 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/examples/embed_external_rois.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5974 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/examples/embed_big_image.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3650 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/index.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      316 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/util/add_annotations.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      353 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/image_rois.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12739 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/static_example.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7505 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/split_view_figure.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4236 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/render_performance.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3367 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/image_dimensions.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12235 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/channel_overlay_viewer.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2782 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/base_header.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2290 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/base_main.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1140 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/base_frame.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/container2.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5221 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/container3.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/base_html.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2035 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/webclient_base_container.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1209 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/right_plugin.rois.js.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4140 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/center_plugin.fullviewer.js.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2783 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/center_plugin.overlay.js.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2716 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/split_view_fig_include.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1422 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/dataset_split_include.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5860 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/split_view_figure.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3529 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/dataset_split_view.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2180 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/center_plugin.splitview.js.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3200 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/center_plugin.fullviewer.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      379 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/templates/webtest/stack_preview.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      975 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/apps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26762 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/omero_webtest/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2020-01-09 10:52:52.000000 omero-webtest-0.4.dev2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34501 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1776 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2788 2020-01-09 10:47:35.000000 omero-webtest-0.4.dev2/setup.py
```

### Comparing `omero-webtest-0.4.dev1/PKG-INFO` & `omero-webtest-0.4.dev2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: omero-webtest
-Version: 0.4.dev1
+Version: 0.4.dev2
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-webtest
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-webtest/archive/v0.4.dev1.tar.gz
+Download-URL: https://github.com/ome/omero-webtest/archive/v0.4.dev2.tar.gz
 Description: .. image:: https://travis-ci.org/ome/omero-webtest.svg?branch=master
             :target: https://travis-ci.org/ome/omero-webtest
         
         .. image:: https://badge.fury.io/py/omero-webtest.svg
             :target: https://badge.fury.io/py/omero-webtest
         
         
@@ -18,15 +18,15 @@
         =============
         OMERO.web app for various prototypes and examples.
         This was removed from the main OMERO.web in the 5.0.6 release of OMERO.
         
         Requirements
         ============
         
-        * OMERO.web 5.2.6 or newer.
+        * OMERO.web 5.6 or newer.
         
         Installing from PyPI
         ====================
         
         This section assumes that an OMERO.web is already installed.
         
         Install the app using `pip <https://pip.pypa.io/en/stable/>`_:
@@ -35,30 +35,25 @@
         
             $ pip install omero-webtest
         
         Add webtest custom app to your installed web apps:
         
         ::
         
-            $ bin/omero config append omero.web.apps '"omero_webtest"'
+            $ omero config append omero.web.apps '"omero_webtest"'
         
         Optional: install example webclient plugins:
         
         ::
         
-            $ bin/omero config append omero.web.ui.right_plugins '["ROIs", "webtest/webclient_plugins/right_plugin.rois.js.html", "image_roi_tab"]'
-            $ bin/omero config append omero.web.ui.center_plugins '["Split View", "webtest/webclient_plugins/center_plugin.splitview.js.html", "split_view_panel"]'
+            $ omero config append omero.web.ui.right_plugins '["ROIs", "webtest/webclient_plugins/right_plugin.rois.js.html", "image_roi_tab"]'
+            $ omero config append omero.web.ui.center_plugins '["Split View", "webtest/webclient_plugins/center_plugin.splitview.js.html", "split_view_panel"]'
         
         Now restart OMERO.web as normal.
         
-        **Warning**:
-        
-        OMERO.webtest version 0.2.x requires OMERO.web **5.2.6 or newer**.
-        This is due to Django Framework compatibility and to a required package reorganization in OMERO.webtest in version 0.2.0 so the application can be distributed from Python Package Index `PyPI <https://pypi.org>`_.
-        
         
         Examples
         ========
         
         Existing examples are available on the following URLs:
         
         ::
@@ -76,27 +71,27 @@
         -------
         
         OMERO.webtest is released under the AGPL.
         
         Copyright
         ---------
         
-        2016-2017, The Open Microscopy Environment
+        2016-2020, The Open Microscopy Environment
         
 Keywords: OMERO.web,plugin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Processing :: Markup :: HTML
+Requires-Python: >=3
```

### Comparing `omero-webtest-0.4.dev1/omero_webtest.egg-info/PKG-INFO` & `omero-webtest-0.4.dev2/omero_webtest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: omero-webtest
-Version: 0.4.dev1
+Version: 0.4.dev2
 Summary: A Python plugin for OMERO.web
 Home-page: https://github.com/ome/omero-webtest
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-webtest/archive/v0.4.dev1.tar.gz
+Download-URL: https://github.com/ome/omero-webtest/archive/v0.4.dev2.tar.gz
 Description: .. image:: https://travis-ci.org/ome/omero-webtest.svg?branch=master
             :target: https://travis-ci.org/ome/omero-webtest
         
         .. image:: https://badge.fury.io/py/omero-webtest.svg
             :target: https://badge.fury.io/py/omero-webtest
         
         
@@ -18,15 +18,15 @@
         =============
         OMERO.web app for various prototypes and examples.
         This was removed from the main OMERO.web in the 5.0.6 release of OMERO.
         
         Requirements
         ============
         
-        * OMERO.web 5.2.6 or newer.
+        * OMERO.web 5.6 or newer.
         
         Installing from PyPI
         ====================
         
         This section assumes that an OMERO.web is already installed.
         
         Install the app using `pip <https://pip.pypa.io/en/stable/>`_:
@@ -35,30 +35,25 @@
         
             $ pip install omero-webtest
         
         Add webtest custom app to your installed web apps:
         
         ::
         
-            $ bin/omero config append omero.web.apps '"omero_webtest"'
+            $ omero config append omero.web.apps '"omero_webtest"'
         
         Optional: install example webclient plugins:
         
         ::
         
-            $ bin/omero config append omero.web.ui.right_plugins '["ROIs", "webtest/webclient_plugins/right_plugin.rois.js.html", "image_roi_tab"]'
-            $ bin/omero config append omero.web.ui.center_plugins '["Split View", "webtest/webclient_plugins/center_plugin.splitview.js.html", "split_view_panel"]'
+            $ omero config append omero.web.ui.right_plugins '["ROIs", "webtest/webclient_plugins/right_plugin.rois.js.html", "image_roi_tab"]'
+            $ omero config append omero.web.ui.center_plugins '["Split View", "webtest/webclient_plugins/center_plugin.splitview.js.html", "split_view_panel"]'
         
         Now restart OMERO.web as normal.
         
-        **Warning**:
-        
-        OMERO.webtest version 0.2.x requires OMERO.web **5.2.6 or newer**.
-        This is due to Django Framework compatibility and to a required package reorganization in OMERO.webtest in version 0.2.0 so the application can be distributed from Python Package Index `PyPI <https://pypi.org>`_.
-        
         
         Examples
         ========
         
         Existing examples are available on the following URLs:
         
         ::
@@ -76,27 +71,27 @@
         -------
         
         OMERO.webtest is released under the AGPL.
         
         Copyright
         ---------
         
-        2016-2017, The Open Microscopy Environment
+        2016-2020, The Open Microscopy Environment
         
 Keywords: OMERO.web,plugin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Text Processing :: Markup :: HTML
+Requires-Python: >=3
```

### Comparing `omero-webtest-0.4.dev1/omero_webtest.egg-info/SOURCES.txt` & `omero-webtest-0.4.dev2/omero_webtest.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 omero_webtest/apps.py
 omero_webtest/urls.py
 omero_webtest/views.py
 omero_webtest.egg-info/PKG-INFO
 omero_webtest.egg-info/SOURCES.txt
 omero_webtest.egg-info/dependency_links.txt
 omero_webtest.egg-info/not-zip-safe
+omero_webtest.egg-info/requires.txt
 omero_webtest.egg-info/top_level.txt
 omero_webtest/static/webtest/img/background.png
 omero_webtest/static/webtest/img/channel_overlay-16.png
 omero_webtest/static/webtest/img/figure_icon-16.png
 omero_webtest/static/webtest/img/channel_overlay/minus12.png
 omero_webtest/static/webtest/img/channel_overlay/plus12.png
 omero_webtest/static/webtest/js/image_dims.js
```

### Comparing `omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/channel_overlay/plus12.png` & `omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/channel_overlay/plus12.png`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/channel_overlay/minus12.png` & `omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/channel_overlay/minus12.png`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/channel_overlay-16.png` & `omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/channel_overlay-16.png`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/figure_icon-16.png` & `omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/figure_icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/static/webtest/img/background.png` & `omero-webtest-0.4.dev2/omero_webtest/static/webtest/img/background.png`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/static/webtest/js/image_dims.js` & `omero-webtest-0.4.dev2/omero_webtest/static/webtest/js/image_dims.js`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/urls.py` & `omero-webtest-0.4.dev2/omero_webtest/urls.py`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/examples/embed_viewer.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/examples/embed_viewer.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/examples/plate_viewer.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/examples/plate_viewer.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/examples/embed_external_rois.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/examples/embed_external_rois.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/examples/embed_big_image.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/examples/embed_big_image.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/index.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/index.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/static_example.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/static_example.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/split_view_figure.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/split_view_figure.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/render_performance.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/render_performance.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/image_dimensions.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/image_dimensions.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/demo_viewers/channel_overlay_viewer.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/demo_viewers/channel_overlay_viewer.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/base_header.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/base_header.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/base_main.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/base_main.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/base_frame.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/base_frame.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/container2.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/container2.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/container3.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/container3.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/base_html.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/base_html.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webgateway/webclient_base_container.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webgateway/webclient_base_container.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/right_plugin.rois.js.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/right_plugin.rois.js.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/center_plugin.fullviewer.js.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/center_plugin.fullviewer.js.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/center_plugin.overlay.js.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/center_plugin.overlay.js.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/split_view_fig_include.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/split_view_fig_include.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/dataset_split_include.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/dataset_split_include.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/split_view_figure.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/split_view_figure.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/dataset_split_view.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/dataset_split_view.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/center_plugin.splitview.js.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/center_plugin.splitview.js.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/templates/webtest/webclient_plugins/center_plugin.fullviewer.html` & `omero-webtest-0.4.dev2/omero_webtest/templates/webtest/webclient_plugins/center_plugin.fullviewer.html`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/apps.py` & `omero-webtest-0.4.dev2/omero_webtest/apps.py`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/omero_webtest/views.py` & `omero-webtest-0.4.dev2/omero_webtest/views.py`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/LICENSE` & `omero-webtest-0.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-webtest-0.4.dev1/README.rst` & `omero-webtest-0.4.dev2/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 =============
 OMERO.web app for various prototypes and examples.
 This was removed from the main OMERO.web in the 5.0.6 release of OMERO.
 
 Requirements
 ============
 
-* OMERO.web 5.2.6 or newer.
+* OMERO.web 5.6 or newer.
 
 Installing from PyPI
 ====================
 
 This section assumes that an OMERO.web is already installed.
 
 Install the app using `pip <https://pip.pypa.io/en/stable/>`_:
@@ -26,30 +26,25 @@
 
     $ pip install omero-webtest
 
 Add webtest custom app to your installed web apps:
 
 ::
 
-    $ bin/omero config append omero.web.apps '"omero_webtest"'
+    $ omero config append omero.web.apps '"omero_webtest"'
 
 Optional: install example webclient plugins:
 
 ::
 
-    $ bin/omero config append omero.web.ui.right_plugins '["ROIs", "webtest/webclient_plugins/right_plugin.rois.js.html", "image_roi_tab"]'
-    $ bin/omero config append omero.web.ui.center_plugins '["Split View", "webtest/webclient_plugins/center_plugin.splitview.js.html", "split_view_panel"]'
+    $ omero config append omero.web.ui.right_plugins '["ROIs", "webtest/webclient_plugins/right_plugin.rois.js.html", "image_roi_tab"]'
+    $ omero config append omero.web.ui.center_plugins '["Split View", "webtest/webclient_plugins/center_plugin.splitview.js.html", "split_view_panel"]'
 
 Now restart OMERO.web as normal.
 
-**Warning**:
-
-OMERO.webtest version 0.2.x requires OMERO.web **5.2.6 or newer**.
-This is due to Django Framework compatibility and to a required package reorganization in OMERO.webtest in version 0.2.0 so the application can be distributed from Python Package Index `PyPI <https://pypi.org>`_.
-
 
 Examples
 ========
 
 Existing examples are available on the following URLs:
 
 ::
@@ -67,8 +62,8 @@
 -------
 
 OMERO.webtest is released under the AGPL.
 
 Copyright
 ---------
 
-2016-2017, The Open Microscopy Environment
+2016-2020, The Open Microscopy Environment
```

### Comparing `omero-webtest-0.4.dev1/setup.py` & `omero-webtest-0.4.dev2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
-VERSION = '0.4.dev1'
+VERSION = '0.4.dev2'
 
 
 setup(name="omero-webtest",
       packages=find_packages(exclude=['ez_setup']),
       version=VERSION,
       description="A Python plugin for OMERO.web",
       long_description=read('README.rst'),
@@ -44,15 +44,14 @@
           'Development Status :: 5 - Production/Stable',
           'Environment :: Web Environment',
           'Framework :: Django',
           'Intended Audience :: Developers',
           'Natural Language :: English',
           'Operating System :: OS Independent',
           'Programming Language :: JavaScript',
-          'Programming Language :: Python :: 2',
           'Programming Language :: Python :: 3',
           'Topic :: Internet :: WWW/HTTP',
           'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
           'Topic :: Internet :: WWW/HTTP :: WSGI',
           'Topic :: Scientific/Engineering :: Visualization',
           'Topic :: Software Development :: Libraries :: '
           'Application Frameworks',
@@ -62,10 +61,12 @@
           # http://pypi.python.org/pypi?%3Aaction=list_classifiers
       author='The Open Microscopy Team',
       author_email='ome-devel@lists.openmicroscopy.org.uk',
       license='AGPL-3.0',
       url="https://github.com/ome/omero-webtest",
       download_url='https://github.com/ome/omero-webtest/archive/v%s.tar.gz' % VERSION,  # NOQA
       keywords=['OMERO.web', 'plugin'],
+      install_requires=['omero-web>=5.6.dev7'],
+      python_requires='>=3',
       include_package_data=True,
       zip_safe=False,
       )
```

