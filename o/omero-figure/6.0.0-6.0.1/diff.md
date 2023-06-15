# Comparing `tmp/omero-figure-6.0.0.tar.gz` & `tmp/omero-figure-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-figure-6.0.0.tar", last modified: Wed May  3 13:29:57 2023, max compression
+gzip compressed data, was "omero-figure-6.0.1.tar", last modified: Thu Jun 15 14:17:00 2023, max compression
```

## Comparing `omero-figure-6.0.0.tar` & `omero-figure-6.0.1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.493957 omero-figure-6.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-05-03 13:29:42.000000 omero-figure-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 13:29:42.000000 omero-figure-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-03 13:29:57.493957 omero-figure-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-05-03 13:29:42.000000 omero-figure-6.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 13:29:46.000000 omero-figure-6.0.0/omero_figure/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 13:29:46.000000 omero-figure-6.0.0/omero_figure/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/omeroutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/scripts/omero/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/scripts/omero/figure_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    93011 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    59497 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone-1.0.0.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/
--rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/
--rw-r--r--   0 runner    (1001) docker     (123)   119892 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)    97339 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14079 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    63157 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    29512 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    16448 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/
--rw-r--r--   0 runner    (1001) docker     (123)    58458 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4143 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     3487 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     3271 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2837 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2972 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     8817 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/
--rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js
--rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-1.11.1/
--rw-r--r--   0 runner    (1001) docker     (123)    95786 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css
--rw-r--r--   0 runner    (1001) docker     (123)   228478 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/json2.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/
--rw-r--r--   0 runner    (1001) docker     (123)    53802 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js
--rw-r--r--   0 runner    (1001) docker     (123)    16798 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4695 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/ome.csrf.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    91476 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js
--rw-r--r--   0 runner    (1001) docker     (123)   299677 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    74385 2023-05-03 13:29:53.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js
--rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/css/
--rw-r--r--   0 runner    (1001) docker     (123)    22795 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/css/figure.css
--rw-r--r--   0 runner    (1001) docker     (123)   372938 2023-05-03 13:29:55.000000 omero-figure-6.0.0/omero_figure/static/figure/figure.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.493957 omero-figure-6.0.0/omero_figure/static/figure/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/arrow-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/button-down-grey.png
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/button-down.png
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/button-flat.png
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/button-up.png
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/crop20.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/cursor-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/ellipse-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/gradient.png
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/line-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (123)    18556 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/luts_10.png
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/markdown_dark32x20.png
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/markdown_light32x20.png
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/polygon-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/polyline-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/projection20.png
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/square-outline-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (123)    66715 2023-05-03 13:29:55.000000 omero-figure-6.0.0/omero_figure/static/figure/templates.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.493957 omero-figure-6.0.0/omero_figure/templates/figure/
--rw-r--r--   0 runner    (1001) docker     (123)    61917 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/templates/figure/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24215 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 13:29:57.493957 omero-figure-6.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-03 13:29:42.000000 omero-figure-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.825353 omero-figure-6.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-06-15 14:16:46.000000 omero-figure-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 14:16:46.000000 omero-figure-6.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-06-15 14:17:00.825353 omero-figure-6.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-15 14:16:46.000000 omero-figure-6.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.817353 omero-figure-6.0.1/omero_figure/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.817353 omero-figure-6.0.1/omero_figure/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-15 14:16:48.000000 omero-figure-6.0.1/omero_figure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-15 14:16:48.000000 omero-figure-6.0.1/omero_figure/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/omeroutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.813353 omero-figure-6.0.1/omero_figure/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.813353 omero-figure-6.0.1/omero_figure/scripts/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.817353 omero-figure-6.0.1/omero_figure/scripts/omero/figure_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    93011 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.813353 omero-figure-6.0.1/omero_figure/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.817353 omero-figure-6.0.1/omero_figure/static/figure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.817353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    59497 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/backbone-1.0.0.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.813353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   119892 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)    97339 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14079 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63157 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29512 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16448 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    58458 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.813353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4143 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3487 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.813353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3271 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2837 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2972 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8817 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-1.11.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    95786 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)   228478 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/json2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    53802 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16798 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.821353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4695 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/ome.csrf.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.825353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    91476 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   299677 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.825353 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    74385 2023-06-15 14:16:56.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.825353 omero-figure-6.0.1/omero_figure/static/figure/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    22795 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/css/figure.css
+-rw-r--r--   0 runner    (1001) docker     (123)   372938 2023-06-15 14:16:59.000000 omero-figure-6.0.1/omero_figure/static/figure/figure.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.825353 omero-figure-6.0.1/omero_figure/static/figure/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/arrow-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/button-down-grey.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/button-down.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/button-flat.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/button-up.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/crop20.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/cursor-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/ellipse-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/gradient.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/line-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18556 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/luts_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/markdown_dark32x20.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/markdown_light32x20.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/polygon-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/polyline-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/projection20.png
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/static/figure/images/square-outline-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66715 2023-06-15 14:16:58.000000 omero-figure-6.0.1/omero_figure/static/figure/templates.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.813353 omero-figure-6.0.1/omero_figure/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.825353 omero-figure-6.0.1/omero_figure/templates/figure/
+-rw-r--r--   0 runner    (1001) docker     (123)    61917 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/templates/figure/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24215 2023-06-15 14:16:46.000000 omero-figure-6.0.1/omero_figure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:17:00.817353 omero-figure-6.0.1/omero_figure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-06-15 14:17:00.000000 omero-figure-6.0.1/omero_figure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-15 14:17:00.000000 omero-figure-6.0.1/omero_figure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:17:00.000000 omero-figure-6.0.1/omero_figure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:17:00.000000 omero-figure-6.0.1/omero_figure.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 14:17:00.000000 omero-figure-6.0.1/omero_figure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 14:17:00.000000 omero-figure-6.0.1/omero_figure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-15 14:17:00.825353 omero-figure-6.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-15 14:16:46.000000 omero-figure-6.0.1/setup.py
```

### Comparing `omero-figure-6.0.0/LICENSE` & `omero-figure-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/PKG-INFO` & `omero-figure-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omero-figure
-Version: 6.0.0
+Version: 6.0.1
 Summary: OMERO figure creation app
 Home-page: https://github.com/ome/omero-figure
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-figure/archive/v6.0.0.tar.gz
+Download-URL: https://github.com/ome/omero-figure/archive/v6.0.1.tar.gz
 Keywords: OMERO.web,figure
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omero-figure-6.0.0/README.rst` & `omero-figure-6.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/__pycache__/utils.cpython-310.pyc` & `omero-figure-6.0.1/omero_figure/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May  3 13:29:42 2023 UTC, .py size: 981 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-00000000: 6f0d 0d0a 0000 0000 c661 5264 d503 0000  o........aRd....
+00000000: 6f0d 0d0a 0000 0000 4e1d 8b64 d503 0000  o.......N..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 5a02 6405 6403 6404 8401 5a03 6401 5300  Z.d.d.d...Z.d.S.
-00000050: 2906 e900 0000 004e 7a05 362e 302e 3063  )......Nz.6.0.0c
+00000050: 2906 e900 0000 004e 7a05 362e 302e 3163  )......Nz.6.0.1c
 00000060: 0200 0000 0000 0000 0000 0000 0500 0000  ................
 00000070: 0800 0000 4300 0000 7366 0000 0074 006a  ....C...sf...t.j
 00000080: 01a0 027c 00a1 017d 0274 037c 0283 018f  ...|...}.t.|....
 00000090: 1f7d 037c 0164 0176 0072 1574 04a0 057c  .}.|.d.v.r.t...|
 000000a0: 03a1 017d 046e 0c7c 03a0 06a1 007d 0457  ...}.n.|.....}.W
 000000b0: 0064 0004 0004 0083 0301 007c 0453 0057  .d.........|.S.W
 000000c0: 0064 0004 0004 0083 0301 007c 0453 0031  .d.........|.S.1
```

### Comparing `omero-figure-6.0.0/omero_figure/apps.py` & `omero-figure-6.0.1/omero_figure/apps.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/omeroutils.py` & `omero-figure-6.0.1/omero_figure/omeroutils.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py` & `omero-figure-6.0.1/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/settings.py` & `omero-figure-6.0.1/omero_figure/settings.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone-1.0.0.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/backbone-1.0.0.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/json2.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/json2.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/ome.csrf.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/ome.csrf.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js` & `omero-figure-6.0.1/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/css/figure.css` & `omero-figure-6.0.1/omero_figure/static/figure/css/figure.css`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/figure.js` & `omero-figure-6.0.1/omero_figure/static/figure/figure.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/arrow-icon-16.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/arrow-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/button-down-grey.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/button-down-grey.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/button-down.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/button-down.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/button-flat.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/button-flat.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/button-up.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/button-up.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/crop20.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/crop20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/ellipse-icon-16.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/ellipse-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/gradient.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/gradient.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/line-icon-16.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/line-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/luts_10.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/luts_10.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/markdown_dark32x20.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/markdown_dark32x20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/markdown_light32x20.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/markdown_light32x20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/polygon-icon-16.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/polygon-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/polyline-icon-16.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/polyline-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/images/projection20.png` & `omero-figure-6.0.1/omero_figure/static/figure/images/projection20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/static/figure/templates.js` & `omero-figure-6.0.1/omero_figure/static/figure/templates.js`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/templates/figure/index.html` & `omero-figure-6.0.1/omero_figure/templates/figure/index.html`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure/urls.py` & `omero-figure-6.0.1/omero_figure/urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,79 +14,82 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 from omeroweb.webgateway import views as webgateway_views
 from . import views
-from django.conf.urls import url
+from django.urls import re_path
 
 
 urlpatterns = [
 
     # index 'home page' of the figure app
-    url(r'^$', views.index, name='figure_index'),
-    url(r'^new/$', views.index, name='new_figure'),
-    url(r'^recover/$', views.index, name='recover_figure'),
-    url(r'^open/$', views.index, name='open_figure'),
-    url(r'^file/(?P<file_id>[0-9]+)/$', views.index, name='load_figure'),
+    re_path(r'^$', views.index, name='figure_index'),
+    re_path(r'^new/$', views.index, name='new_figure'),
+    re_path(r'^recover/$', views.index, name='recover_figure'),
+    re_path(r'^open/$', views.index, name='open_figure'),
+    re_path(r'^file/(?P<file_id>[0-9]+)/$', views.index, name='load_figure'),
 
-    url(r'^imgData/(?P<image_id>[0-9]+)/$', views.img_data_json,
-        name='figure_imgData'),
+    re_path(r'^imgData/(?P<image_id>[0-9]+)/$', views.img_data_json,
+            name='figure_imgData'),
 
     # Send json to OMERO to create pdf using scripting service
-    url(r'^make_web_figure/', views.make_web_figure, name='make_web_figure'),
+    re_path(r'^make_web_figure/', views.make_web_figure,
+            name='make_web_figure'),
 
     # Save json to file annotation
-    url(r'^save_web_figure/', views.save_web_figure, name='save_web_figure'),
+    re_path(r'^save_web_figure/', views.save_web_figure,
+            name='save_web_figure'),
 
     # Get json from file (file annotation Id)
-    url(r'^load_web_figure/(?P<file_id>[0-9]+)/$', views.load_web_figure,
-        name='load_web_figure'),
+    re_path(r'^load_web_figure/(?P<file_id>[0-9]+)/$', views.load_web_figure,
+            name='load_web_figure'),
 
     # List file annotations of saved Figures
-    url(r'^list_web_figures/', views.list_web_figures,
-        name='list_web_figures'),
+    re_path(r'^list_web_figures/', views.list_web_figures,
+            name='list_web_figures'),
 
-    url(r'^render_thumbnail/(?P<iid>[0-9]+)/$',
-        webgateway_views.render_thumbnail,
-        {'_defcb': views.default_thumbnail},
-        name="figure_render_thumbnail"),
+    re_path(r'^render_thumbnail/(?P<iid>[0-9]+)/$',
+            webgateway_views.render_thumbnail,
+            {'_defcb': views.default_thumbnail},
+            name="figure_render_thumbnail"),
 
     # Region defined by ?region=x,y,w,h
-    url(r'^render_scaled_region/(?P<iid>[0-9]+)/(?P<z>[0-9]+)/(?P<t>[0-9]+)/$',
+    re_path(
+        r'^render_scaled_region/(?P<iid>[0-9]+)/(?P<z>[0-9]+)/(?P<t>[0-9]+)/$',
         views.render_scaled_region,
         name="figure_render_scaled_region"),
 
     # Delete file annotations of saved Figures - 'POST' with 'fileId' of file
     # annotation
-    url(r'^delete_web_figure/$', views.delete_web_figure,
-        name='delete_web_figure'),
+    re_path(r'^delete_web_figure/$', views.delete_web_figure,
+            name='delete_web_figure'),
 
     # Converts Lengths of value in 'fromUnit' to 'toUnit'.
     # E.g. unit_conversion/1.12/MICROMETER/ANGSTROM/.
     # Returns result as json with keys of 'value', 'unit' and 'symbol'
-    url(r'^unit_conversion/(?P<value>[0-9.]+)/(?P<from_unit>[A-Z]+)/'
-        '(?P<to_unit>[A-Z]+)/$',
-        views.unit_conversion, name='unit_conversion'),
+    re_path(r'^unit_conversion/(?P<value>[0-9.]+)/(?P<from_unit>[A-Z]+)/'
+            '(?P<to_unit>[A-Z]+)/$',
+            views.unit_conversion, name='unit_conversion'),
 
     # Get timestamps in seconds for images
     # Use query ?image=1&image=2
-    url(r'^timestamps/$', views.timestamps, name='figure_timestamps'),
+    re_path(r'^timestamps/$', views.timestamps, name='figure_timestamps'),
 
     # Get Z scale for images
     # Use query ?image=1&image=2
-    url(r'^z_scale/$', views.z_scale, name='figure_z_scale'),
+    re_path(r'^z_scale/$', views.z_scale, name='figure_z_scale'),
 
-    url(r'^roiCount/(?P<image_id>[0-9]+)/$', views.roi_count,
-        name='figure_roiCount'),
+    re_path(r'^roiCount/(?P<image_id>[0-9]+)/$', views.roi_count,
+            name='figure_roiCount'),
 
-    url(r'^roiRectangles/(?P<image_id>[0-9]+)/$', views.roi_rectangles,
-        name='figure_roiRectangles'),
+    re_path(r'^roiRectangles/(?P<image_id>[0-9]+)/$', views.roi_rectangles,
+            name='figure_roiRectangles'),
 
     # POST to change figure to new group with ann_id and group_id
-    url(r'chgrp/$', views.chgrp, name='figure_chgrp'),
+    re_path(r'chgrp/$', views.chgrp, name='figure_chgrp'),
 
     # Get group and owner info for multiple images. ?image=1,2,3
-    url(r'images_details/', views.images_details,
-        name="figure_images_details")
+    re_path(r'images_details/', views.images_details,
+            name="figure_images_details")
 ]
```

### Comparing `omero-figure-6.0.0/omero_figure/utils.py` & `omero-figure-6.0.1/omero_figure/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 
 import json
 import os
 
-__version__ = "6.0.0"
+__version__ = "6.0.1"
 
 
 def read_file(fname, content_type=None):
     p = os.path.abspath(fname)
     with open(p) as f:
         if content_type in ('json',):
             data = json.load(f)
```

### Comparing `omero-figure-6.0.0/omero_figure/views.py` & `omero-figure-6.0.1/omero_figure/views.py`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/omero_figure.egg-info/PKG-INFO` & `omero-figure-6.0.1/omero_figure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: omero-figure
-Version: 6.0.0
+Version: 6.0.1
 Summary: OMERO figure creation app
 Home-page: https://github.com/ome/omero-figure
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
-Download-URL: https://github.com/ome/omero-figure/archive/v6.0.0.tar.gz
+Download-URL: https://github.com/ome/omero-figure/archive/v6.0.1.tar.gz
 Keywords: OMERO.web,figure
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omero-figure-6.0.0/omero_figure.egg-info/SOURCES.txt` & `omero-figure-6.0.1/omero_figure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omero-figure-6.0.0/setup.py` & `omero-figure-6.0.1/setup.py`

 * *Files identical despite different names*

