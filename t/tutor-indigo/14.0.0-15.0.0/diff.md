# Comparing `tmp/tutor-indigo-14.0.0.tar.gz` & `tmp/tutor-indigo-15.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-indigo-14.0.0.tar", last modified: Thu Jun  9 19:45:23 2022, max compression
+gzip compressed data, was "dist/tutor-indigo-15.0.0.tar", last modified: Mon Dec 12 17:21:37 2022, max compression
```

## Comparing `tutor-indigo-14.0.0.tar` & `tutor-indigo-15.0.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)       42 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6369 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4705 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1676 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutor_indigo.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6369 2022-06-09 19:45:22.000000 tutor-indigo-14.0.0/tutor_indigo.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     3097 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutor_indigo.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2022-06-09 19:45:22.000000 tutor-indigo-14.0.0/tutor_indigo.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       47 2022-06-09 19:45:22.000000 tutor-indigo-14.0.0/tutor_indigo.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2022-06-09 19:45:22.000000 tutor-indigo-14.0.0/tutor_indigo.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       12 2022-06-09 19:45:22.000000 tutor-indigo-14.0.0/tutor_indigo.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1800 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/cms/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/cms/static/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/cms/static/images/
--rw-r--r--   0 ci        (1000) ci        (1000)    12206 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/cms/static/images/favicon.ico
--rw-r--r--   0 ci        (1000) ci        (1000)     1681 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/cms/static/images/studio-logo.png
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/
--rw-r--r--   0 ci        (1000) ci        (1000)    64424 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Bold.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)    50132 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-BoldItalic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)    87932 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Italic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   125568 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Regular.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)    52612 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-SemiBold.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)    50000 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-SemiBoldItalic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   180352 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Bold.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   189096 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-BoldItalic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   183760 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ExtraLight.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   191888 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ExtraLightItalic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   189048 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Italic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   182496 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Light.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   191240 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-LightItalic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   181536 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Medium.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   190196 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-MediumItalic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   180372 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Regular.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   181760 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-SemiBold.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   190736 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-SemiBoldItalic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   183484 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Thin.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)   192604 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ThinItalic.ttf
--rw-r--r--   0 ci        (1000) ci        (1000)     4514 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/OFL.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/images/
--rw-r--r--   0 ci        (1000) ci        (1000)    12206 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/images/favicon.ico
--rw-r--r--   0 ci        (1000) ci        (1000)     1681 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/images/logo.png
--rw-r--r--   0 ci        (1000) ci        (1000)     8031 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/images/openedx-logo.png
--rw-r--r--   0 ci        (1000) ci        (1000)    14135 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/images/tutor-logo.png
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/sass/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/
--rw-r--r--   0 ci        (1000) ci        (1000)     4504 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_extras.scss
--rw-r--r--   0 ci        (1000) ci        (1000)     2368 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_fonts.scss
--rw-r--r--   0 ci        (1000) ci        (1000)      270 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_variables.scss
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/
--rw-r--r--   0 ci        (1000) ci        (1000)     6672 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/footer.html
--rw-r--r--   0 ci        (1000) ci        (1000)       71 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/index_overlay.html
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/
--rw-r--r--   0 ci        (1000) ci        (1000)      724 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/about.html
--rw-r--r--   0 ci        (1000) ci        (1000)      612 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/contact.html
--rw-r--r--   0 ci        (1000) ci        (1000)      644 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/tos.html
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/
--rw-r--r--   0 ci        (1000) ci        (1000)     6672 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/footer.html
--rw-r--r--   0 ci        (1000) ci        (1000)       71 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/index_overlay.html
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-06-09 19:45:23.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/
--rw-r--r--   0 ci        (1000) ci        (1000)      724 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/about.html
--rw-r--r--   0 ci        (1000) ci        (1000)      612 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/contact.html
--rw-r--r--   0 ci        (1000) ci        (1000)      644 2022-06-09 19:45:17.000000 tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/tos.html
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/
+-rw-r--r--   0 ci        (1000) ci        (1000)       42 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6636 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4818 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1848 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutor_indigo.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6636 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutor_indigo.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     3097 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutor_indigo.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutor_indigo.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       47 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutor_indigo.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutor_indigo.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       12 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutor_indigo.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/
+-rw-r--r--   0 ci        (1000) ci        (1000)       23 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1806 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/cms/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/cms/static/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/cms/static/images/
+-rw-r--r--   0 ci        (1000) ci        (1000)    12206 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/cms/static/images/favicon.ico
+-rw-r--r--   0 ci        (1000) ci        (1000)     1681 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/cms/static/images/studio-logo.png
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/
+-rw-r--r--   0 ci        (1000) ci        (1000)    64424 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Bold.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)    50132 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-BoldItalic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)    87932 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Italic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   125568 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Regular.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)    52612 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-SemiBold.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)    50000 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-SemiBoldItalic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   180352 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Bold.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   189096 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-BoldItalic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   183760 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ExtraLight.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   191888 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ExtraLightItalic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   189048 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Italic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   182496 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Light.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   191240 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-LightItalic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   181536 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Medium.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   190196 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-MediumItalic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   180372 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Regular.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   181760 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-SemiBold.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   190736 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-SemiBoldItalic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   183484 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Thin.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)   192604 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ThinItalic.ttf
+-rw-r--r--   0 ci        (1000) ci        (1000)     4514 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/OFL.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/images/
+-rw-r--r--   0 ci        (1000) ci        (1000)    12206 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/images/favicon.ico
+-rw-r--r--   0 ci        (1000) ci        (1000)     1681 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/images/logo.png
+-rw-r--r--   0 ci        (1000) ci        (1000)     8031 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/images/openedx-logo.png
+-rw-r--r--   0 ci        (1000) ci        (1000)    14135 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/images/tutor-logo.png
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/sass/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/
+-rw-r--r--   0 ci        (1000) ci        (1000)     4504 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_extras.scss
+-rw-r--r--   0 ci        (1000) ci        (1000)     2368 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_fonts.scss
+-rw-r--r--   0 ci        (1000) ci        (1000)      270 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_variables.scss
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6711 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/footer.html
+-rw-r--r--   0 ci        (1000) ci        (1000)       71 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/index_overlay.html
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/
+-rw-r--r--   0 ci        (1000) ci        (1000)      724 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/about.html
+-rw-r--r--   0 ci        (1000) ci        (1000)      612 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/contact.html
+-rw-r--r--   0 ci        (1000) ci        (1000)      644 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/tos.html
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6711 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/footer.html
+-rw-r--r--   0 ci        (1000) ci        (1000)       71 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/index_overlay.html
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2022-12-12 17:21:37.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/
+-rw-r--r--   0 ci        (1000) ci        (1000)      724 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/about.html
+-rw-r--r--   0 ci        (1000) ci        (1000)      612 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/contact.html
+-rw-r--r--   0 ci        (1000) ci        (1000)      644 2022-12-12 17:21:29.000000 tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/tos.html
```

### Comparing `tutor-indigo-14.0.0/PKG-INFO` & `tutor-indigo-15.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 1.2
 Name: tutor-indigo
-Version: 14.0.0
+Version: 15.0.0
 Summary: Indigo theme plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-indigo
 Author: Overhang.IO
+Author-email: contact@overhang.io
+Maintainer: Overhang.IO
+Maintainer-email: regis@overhang.io
 License: AGPLv3
+Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor-indigo
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-indigo/issues
-Project-URL: Community, https://discuss.overhang.io
+Project-URL: Community, https://discuss.openedx.org
 Description: Indigo, a cool blue theme for Open edX
         ======================================
         
         Indigo is an elegant, customizable theme for `Open edX <https://open.edx.org>`__.
         
         .. image:: ./screenshots/01-landing-page.png
             :alt: Platform landing page
         
-        **Note**: This version of the Indigo theme is compatible with the Maple release of Open edX.
+        **Note**: This version of the Indigo theme is compatible with the Olive release of Open edX.
         
         You can view the theme in action at https://demo.openedx.overhang.io.
         
         Installation
         ------------
         
-        Indigo was specially developed to be used with `Tutor <https://docs.overhang.io>`__ (at least v12.0.0). If you have not installed Open edX with Tutor, then installation instructions will vary.
+        Indigo was specially developed to be used with `Tutor <https://docs.overhang.io>`__ (at least v14.0.0). If you have not installed Open edX with Tutor, then installation instructions will vary.
         
         Since Tutor v13.2.0, Indigo can be installed as a Tutor plugin::
         
             pip install tutor-indigo
             tutor plugins enable indigo
+            tutor config save
         
         Rebuild the Openedx docker image::
         
             tutor images build openedx
         
         Restart your platform::
         
@@ -65,19 +70,19 @@
         The theme images are stored in `tutorindigo/templates/indigo/lms/static/images <https://github.com/overhangio/tutor-indigo/tree/master/tutorindigo/templates/indigo/lms/static/images>`__ for the LMS, and in `tutorindigo/templates/indigo/cms/static/images <https://github.com/overhangio/tutor-indigo/tree/master/tutorindigo/templates/indigo/cms/static/images>`__ for the CMS. To use custom images in your theme, just replace the files stored in these folders with your own.
         
         Overriding the default "about", "contact", etc. static pages
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         By default, the ``/about`` and ``/contact`` pages contain a simple line of text: "This page left intentionally blank. Feel free to add your own content". This is of course unusable in production. In the following, we detail how to override just any of the static templates used in Open edX.
         
-        The static templates used by Open edX to render those pages are all stored in the `edx-platform/lms/templates/static_templates <https://github.com/edx/edx-platform/tree/open-release/maple.master/lms/templates/static_templates>`__ folder. To override those templates, you should add your own in the following folder::
+        The static templates used by Open edX to render those pages are all stored in the `edx-platform/lms/templates/static_templates <https://github.com/edx/edx-platform/tree/open-release/olive.master/lms/templates/static_templates>`__ folder. To override those templates, you should add your own in the following folder::
         
             ls tutorindigo/templates/indigo/lms/templates/static_templates"
         
-        For instance, edit the "donate.html" file in this directory. We can derive the content of this file from the contents of the `donate.html <https://github.com/edx/edx-platform/blob/open-release/maple.master/lms/templates/static_templates/donate.html>`__ static template in edx-platform::
+        For instance, edit the "donate.html" file in this directory. We can derive the content of this file from the contents of the `donate.html <https://github.com/edx/edx-platform/blob/open-release/olive.master/lms/templates/static_templates/donate.html>`__ static template in edx-platform::
         
             <%page expression_filter="h"/>
             <%! from django.utils.translation import ugettext as _ %>
             <%inherit file="../main.html" />
         
             <%block name="pagetitle">${_("Donate")}</%block>
         
@@ -93,17 +98,16 @@
             </main>
         
         This new template will then be used to render the /donate url.
         
         Troubleshooting
         ---------------
         
-        Please refer to the troubleshooting section of the Tutor documentation: https://docs.tutor.overhang.io/troubleshooting.html
+        This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
         
-        In particular, *do not* open a GitHub issue to ask about your issues. Instead, go to the Tutor forum: https://discuss.overhang.io/
         
         License
         -------
         
         This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-indigo/blob/master/LICENSE.txt>`_.
         
 Platform: UNKNOWN
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tutor-indigo-14.0.0/README.rst` & `tutor-indigo-15.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 ======================================
 
 Indigo is an elegant, customizable theme for `Open edX <https://open.edx.org>`__.
 
 .. image:: ./screenshots/01-landing-page.png
     :alt: Platform landing page
 
-**Note**: This version of the Indigo theme is compatible with the Maple release of Open edX.
+**Note**: This version of the Indigo theme is compatible with the Olive release of Open edX.
 
 You can view the theme in action at https://demo.openedx.overhang.io.
 
 Installation
 ------------
 
-Indigo was specially developed to be used with `Tutor <https://docs.overhang.io>`__ (at least v12.0.0). If you have not installed Open edX with Tutor, then installation instructions will vary.
+Indigo was specially developed to be used with `Tutor <https://docs.overhang.io>`__ (at least v14.0.0). If you have not installed Open edX with Tutor, then installation instructions will vary.
 
 Since Tutor v13.2.0, Indigo can be installed as a Tutor plugin::
 
     pip install tutor-indigo
     tutor plugins enable indigo
+    tutor config save
 
 Rebuild the Openedx docker image::
 
     tutor images build openedx
 
 Restart your platform::
 
@@ -55,19 +56,19 @@
 The theme images are stored in `tutorindigo/templates/indigo/lms/static/images <https://github.com/overhangio/tutor-indigo/tree/master/tutorindigo/templates/indigo/lms/static/images>`__ for the LMS, and in `tutorindigo/templates/indigo/cms/static/images <https://github.com/overhangio/tutor-indigo/tree/master/tutorindigo/templates/indigo/cms/static/images>`__ for the CMS. To use custom images in your theme, just replace the files stored in these folders with your own.
 
 Overriding the default "about", "contact", etc. static pages
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 By default, the ``/about`` and ``/contact`` pages contain a simple line of text: "This page left intentionally blank. Feel free to add your own content". This is of course unusable in production. In the following, we detail how to override just any of the static templates used in Open edX.
 
-The static templates used by Open edX to render those pages are all stored in the `edx-platform/lms/templates/static_templates <https://github.com/edx/edx-platform/tree/open-release/maple.master/lms/templates/static_templates>`__ folder. To override those templates, you should add your own in the following folder::
+The static templates used by Open edX to render those pages are all stored in the `edx-platform/lms/templates/static_templates <https://github.com/edx/edx-platform/tree/open-release/olive.master/lms/templates/static_templates>`__ folder. To override those templates, you should add your own in the following folder::
 
     ls tutorindigo/templates/indigo/lms/templates/static_templates"
 
-For instance, edit the "donate.html" file in this directory. We can derive the content of this file from the contents of the `donate.html <https://github.com/edx/edx-platform/blob/open-release/maple.master/lms/templates/static_templates/donate.html>`__ static template in edx-platform::
+For instance, edit the "donate.html" file in this directory. We can derive the content of this file from the contents of the `donate.html <https://github.com/edx/edx-platform/blob/open-release/olive.master/lms/templates/static_templates/donate.html>`__ static template in edx-platform::
 
     <%page expression_filter="h"/>
     <%! from django.utils.translation import ugettext as _ %>
     <%inherit file="../main.html" />
 
     <%block name="pagetitle">${_("Donate")}</%block>
 
@@ -83,15 +84,14 @@
     </main>
 
 This new template will then be used to render the /donate url.
 
 Troubleshooting
 ---------------
 
-Please refer to the troubleshooting section of the Tutor documentation: https://docs.tutor.overhang.io/troubleshooting.html
+This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
-In particular, *do not* open a GitHub issue to ask about your issues. Instead, go to the Tutor forum: https://discuss.overhang.io/
 
 License
 -------
 
 This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-indigo/blob/master/LICENSE.txt>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tutor-indigo-14.0.0/setup.py` & `tutor-indigo-15.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,26 +25,30 @@
 
 
 setup(
     name="tutor-indigo",
     version=ABOUT["__version__"],
     url="https://github.com/overhangio/tutor-indigo",
     project_urls={
+        "Documentation": "https://docs.tutor.overhang.io/",
         "Code": "https://github.com/overhangio/tutor-indigo",
         "Issue tracker": "https://github.com/overhangio/tutor-indigo/issues",
-        "Community": "https://discuss.overhang.io",
+        "Community": "https://discuss.openedx.org",
     },
     license="AGPLv3",
     author="Overhang.IO",
+    author_email="contact@overhang.io",
+    maintainer="Overhang.IO",
+    maintainer_email="regis@overhang.io",
     description="Indigo theme plugin for Tutor",
     long_description=load_readme(),
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.7",
-    install_requires=["tutor>=14.0.0,<15.0.0"],
+    install_requires=["tutor>=15.0.0,<16.0.0"],
     entry_points={"tutor.plugin.v1": ["indigo = tutorindigo.plugin"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `tutor-indigo-14.0.0/tutor_indigo.egg-info/PKG-INFO` & `tutor-indigo-15.0.0/tutor_indigo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 Metadata-Version: 1.2
 Name: tutor-indigo
-Version: 14.0.0
+Version: 15.0.0
 Summary: Indigo theme plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-indigo
 Author: Overhang.IO
+Author-email: contact@overhang.io
+Maintainer: Overhang.IO
+Maintainer-email: regis@overhang.io
 License: AGPLv3
+Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor-indigo
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-indigo/issues
-Project-URL: Community, https://discuss.overhang.io
+Project-URL: Community, https://discuss.openedx.org
 Description: Indigo, a cool blue theme for Open edX
         ======================================
         
         Indigo is an elegant, customizable theme for `Open edX <https://open.edx.org>`__.
         
         .. image:: ./screenshots/01-landing-page.png
             :alt: Platform landing page
         
-        **Note**: This version of the Indigo theme is compatible with the Maple release of Open edX.
+        **Note**: This version of the Indigo theme is compatible with the Olive release of Open edX.
         
         You can view the theme in action at https://demo.openedx.overhang.io.
         
         Installation
         ------------
         
-        Indigo was specially developed to be used with `Tutor <https://docs.overhang.io>`__ (at least v12.0.0). If you have not installed Open edX with Tutor, then installation instructions will vary.
+        Indigo was specially developed to be used with `Tutor <https://docs.overhang.io>`__ (at least v14.0.0). If you have not installed Open edX with Tutor, then installation instructions will vary.
         
         Since Tutor v13.2.0, Indigo can be installed as a Tutor plugin::
         
             pip install tutor-indigo
             tutor plugins enable indigo
+            tutor config save
         
         Rebuild the Openedx docker image::
         
             tutor images build openedx
         
         Restart your platform::
         
@@ -65,19 +70,19 @@
         The theme images are stored in `tutorindigo/templates/indigo/lms/static/images <https://github.com/overhangio/tutor-indigo/tree/master/tutorindigo/templates/indigo/lms/static/images>`__ for the LMS, and in `tutorindigo/templates/indigo/cms/static/images <https://github.com/overhangio/tutor-indigo/tree/master/tutorindigo/templates/indigo/cms/static/images>`__ for the CMS. To use custom images in your theme, just replace the files stored in these folders with your own.
         
         Overriding the default "about", "contact", etc. static pages
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         By default, the ``/about`` and ``/contact`` pages contain a simple line of text: "This page left intentionally blank. Feel free to add your own content". This is of course unusable in production. In the following, we detail how to override just any of the static templates used in Open edX.
         
-        The static templates used by Open edX to render those pages are all stored in the `edx-platform/lms/templates/static_templates <https://github.com/edx/edx-platform/tree/open-release/maple.master/lms/templates/static_templates>`__ folder. To override those templates, you should add your own in the following folder::
+        The static templates used by Open edX to render those pages are all stored in the `edx-platform/lms/templates/static_templates <https://github.com/edx/edx-platform/tree/open-release/olive.master/lms/templates/static_templates>`__ folder. To override those templates, you should add your own in the following folder::
         
             ls tutorindigo/templates/indigo/lms/templates/static_templates"
         
-        For instance, edit the "donate.html" file in this directory. We can derive the content of this file from the contents of the `donate.html <https://github.com/edx/edx-platform/blob/open-release/maple.master/lms/templates/static_templates/donate.html>`__ static template in edx-platform::
+        For instance, edit the "donate.html" file in this directory. We can derive the content of this file from the contents of the `donate.html <https://github.com/edx/edx-platform/blob/open-release/olive.master/lms/templates/static_templates/donate.html>`__ static template in edx-platform::
         
             <%page expression_filter="h"/>
             <%! from django.utils.translation import ugettext as _ %>
             <%inherit file="../main.html" />
         
             <%block name="pagetitle">${_("Donate")}</%block>
         
@@ -93,17 +98,16 @@
             </main>
         
         This new template will then be used to render the /donate url.
         
         Troubleshooting
         ---------------
         
-        Please refer to the troubleshooting section of the Tutor documentation: https://docs.tutor.overhang.io/troubleshooting.html
+        This Tutor plugin is maintained by Régis Behmo from `Overhang.IO <https://overhang.io>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
         
-        In particular, *do not* open a GitHub issue to ask about your issues. Instead, go to the Tutor forum: https://discuss.overhang.io/
         
         License
         -------
         
         This work is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-indigo/blob/master/LICENSE.txt>`_.
         
 Platform: UNKNOWN
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tutor-indigo-14.0.0/tutor_indigo.egg-info/SOURCES.txt` & `tutor-indigo-15.0.0/tutor_indigo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/plugin.py` & `tutor-indigo-15.0.0/tutorindigo/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 hooks.Filters.ENV_TEMPLATE_TARGETS.add_items(
     [
         ("indigo", "build/openedx/themes"),
     ],
 )
 
 # Force the rendering of scss files, even though they are included in a "partials" directory
-hooks.Filters.ENV_PATTERNS_INCLUDE.add_item(r"indigo/lms/static/sass/partials/lms/theme/")
+hooks.Filters.ENV_PATTERNS_INCLUDE.add_item(
+    r"indigo/lms/static/sass/partials/lms/theme/"
+)
 
 # Load all configuration entries
 hooks.Filters.CONFIG_DEFAULTS.add_items(
     [(f"INDIGO_{key}", value) for key, value in config["defaults"].items()]
 )
 hooks.Filters.CONFIG_UNIQUE.add_items(
     [(f"INDIGO_{key}", value) for key, value in config["unique"].items()]
```

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/cms/static/images/favicon.ico` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/cms/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/cms/static/images/studio-logo.png` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/cms/static/images/studio-logo.png`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Bold.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Bold.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-BoldItalic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Italic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Italic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Regular.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-Regular.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-SemiBold.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-SemiBoldItalic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/CrimsonText-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Bold.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-BoldItalic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ExtraLight.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ExtraLightItalic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Italic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Light.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-LightItalic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Medium.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Medium.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-MediumItalic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Regular.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-SemiBold.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-SemiBoldItalic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Thin.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-Thin.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ThinItalic.ttf` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/IBMPlexSans-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/fonts/OFL.txt` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/images/favicon.ico` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/images/logo.png` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/images/openedx-logo.png` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/images/openedx-logo.png`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/images/tutor-logo.png` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/images/tutor-logo.png`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_extras.scss` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_extras.scss`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_fonts.scss` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/sass/partials/lms/theme/_fonts.scss`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/footer.html` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/footer.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## mako
 <%page expression_filter="h"/>
 <%!
   from django.urls import reverse
-  from django.utils.translation import ugettext as _
+  from django.utils.translation import gettext as _
   from lms.djangoapps.branding.api import get_footer
   from openedx.core.djangoapps.lang_pref.api import footer_language_selector_is_enabled
 %>
 <% footer = get_footer(is_secure=is_secure) %>
 <% icp_license_info = getattr(settings, 'ICP_LICENSE_INFO', {})%>
 <%namespace name='static' file='static_content.html'/>
 
@@ -54,15 +54,15 @@
           ## The OpenEdX link may be hidden when this view is served
           ## through an API to partner sites (such as marketing sites or blogs),
           ## which are not technically powered by Open edX.
           % if not hide_openedx_link:
             <div class="footer-about-openedx">
               <p>
                 <a href="https://docs.tutor.overhang.io" rel="noopener" target="_blank">
-                  <img src="${static.url('images/tutor-logo.png')}" width="140" />
+                  <img src="${static.url('images/tutor-logo.png')}" alt="Runs on Tutor" width="140" />
                 </a>
                 <a href="${footer['openedx_link']['url']}" rel="noopener" target="_blank">
                   <img src="${static.url('images/openedx-logo.png')}" alt="${footer['openedx_link']['title']}" width="140" />
                 </a>
               </p>
             </div>
           % endif
@@ -138,15 +138,15 @@
       ## The OpenEdX link may be hidden when this view is served
       ## through an API to partner sites (such as marketing sites or blogs),
       ## which are not technically powered by OpenEdX.
       % if not hide_openedx_link:
       <div class="footer-about-openedx">
         <p>
           <a href="https://docs.tutor.overhang.io" rel="noopener" target="_blank">
-            <img src="${static.url('images/tutor-logo.png')}" height="42" />
+            <img src="${static.url('images/tutor-logo.png')}" alt="Runs on Tutor" height="42" />
           </a>
           <a href="${footer['openedx_link']['url']}" rel="noopener" target="_blank">
             <img src="${static.url('images/openedx-logo.png')}" alt="${footer['openedx_link']['title']}" width="140" />
           </a>
         </p>
       </div>
       % endif
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 ## mako <%page expression_filter="h"/> <%! from django.urls import reverse from
-django.utils.translation import ugettext as _ from lms.djangoapps.branding.api
+django.utils.translation import gettext as _ from lms.djangoapps.branding.api
 import get_footer from openedx.core.djangoapps.lang_pref.api import
 footer_language_selector_is_enabled %> <% footer = get_footer
 (is_secure=is_secure) %> <% icp_license_info = getattr(settings,
 'ICP_LICENSE_INFO', {})%> <%namespace name='static' file='static_content.html'/
 > % if uses_bootstrap:
 {% if INDIGO_FOOTER_NAV_LINKS %}
     * {% for link in INDIGO_FOOTER_NAV_LINKS %}
@@ -20,15 +20,15 @@
     * {{_link['title']_}}
     * {% endfor %}
  {% endif %}
 ## Please leave this link and use one of the logos provided ## The OpenEdX link
 may be hidden when this view is served ## through an API to partner sites (such
 as marketing sites or blogs), ## which are not technically powered by Open edX.
 % if not hide_openedx_link:
-[${static.url('images/tutor-logo.png')}] [${footer['openedx_link']['title']}]
+[Runs_on_Tutor] [${footer['openedx_link']['title']}]
 % endif
 % else:
 # When rendering the footer through the branding API, ## the direction may not
 be set on the parent element, ## so we set it here. % if bidi: dir=${bidi} %
 endif >
 {% if INDIGO_FOOTER_NAV_LINKS %}
    1. {% for link in INDIGO_FOOTER_NAV_LINKS %}
@@ -53,14 +53,14 @@
     * {{_link['title']_}}
     * {% endfor %}
  {% endif %}
 ## Please leave this link and use one of the logos provided ## The OpenEdX link
 may be hidden when this view is served ## through an API to partner sites (such
 as marketing sites or blogs), ## which are not technically powered by OpenEdX.
 % if not hide_openedx_link:
-[${static.url('images/tutor-logo.png')}] [${footer['openedx_link']['title']}]
+[Runs_on_Tutor] [${footer['openedx_link']['title']}]
 % endif
 % endif % if include_dependencies: <%static:js group='base_vendor'/> <%static:
 css group='style-vendor'/> <%include file="widgets/segment-io.html" /
 > <%include file="widgets/segment-io-footer.html" /> % endif % if
 footer_css_urls: % for url in footer_css_urls:
  % endfor % endif
```

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/about.html` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/about.html`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/contact.html` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/contact.html`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/tos.html` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/static/templates/static_templates/tos.html`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/footer.html` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/footer.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## mako
 <%page expression_filter="h"/>
 <%!
   from django.urls import reverse
-  from django.utils.translation import ugettext as _
+  from django.utils.translation import gettext as _
   from lms.djangoapps.branding.api import get_footer
   from openedx.core.djangoapps.lang_pref.api import footer_language_selector_is_enabled
 %>
 <% footer = get_footer(is_secure=is_secure) %>
 <% icp_license_info = getattr(settings, 'ICP_LICENSE_INFO', {})%>
 <%namespace name='static' file='static_content.html'/>
 
@@ -54,15 +54,15 @@
           ## The OpenEdX link may be hidden when this view is served
           ## through an API to partner sites (such as marketing sites or blogs),
           ## which are not technically powered by Open edX.
           % if not hide_openedx_link:
             <div class="footer-about-openedx">
               <p>
                 <a href="https://docs.tutor.overhang.io" rel="noopener" target="_blank">
-                  <img src="${static.url('images/tutor-logo.png')}" width="140" />
+                  <img src="${static.url('images/tutor-logo.png')}" alt="Runs on Tutor" width="140" />
                 </a>
                 <a href="${footer['openedx_link']['url']}" rel="noopener" target="_blank">
                   <img src="${static.url('images/openedx-logo.png')}" alt="${footer['openedx_link']['title']}" width="140" />
                 </a>
               </p>
             </div>
           % endif
@@ -138,15 +138,15 @@
       ## The OpenEdX link may be hidden when this view is served
       ## through an API to partner sites (such as marketing sites or blogs),
       ## which are not technically powered by OpenEdX.
       % if not hide_openedx_link:
       <div class="footer-about-openedx">
         <p>
           <a href="https://docs.tutor.overhang.io" rel="noopener" target="_blank">
-            <img src="${static.url('images/tutor-logo.png')}" height="42" />
+            <img src="${static.url('images/tutor-logo.png')}" alt="Runs on Tutor" height="42" />
           </a>
           <a href="${footer['openedx_link']['url']}" rel="noopener" target="_blank">
             <img src="${static.url('images/openedx-logo.png')}" alt="${footer['openedx_link']['title']}" width="140" />
           </a>
         </p>
       </div>
       % endif
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 ## mako <%page expression_filter="h"/> <%! from django.urls import reverse from
-django.utils.translation import ugettext as _ from lms.djangoapps.branding.api
+django.utils.translation import gettext as _ from lms.djangoapps.branding.api
 import get_footer from openedx.core.djangoapps.lang_pref.api import
 footer_language_selector_is_enabled %> <% footer = get_footer
 (is_secure=is_secure) %> <% icp_license_info = getattr(settings,
 'ICP_LICENSE_INFO', {})%> <%namespace name='static' file='static_content.html'/
 > % if uses_bootstrap:
 {% if INDIGO_FOOTER_NAV_LINKS %}
     * {% for link in INDIGO_FOOTER_NAV_LINKS %}
@@ -20,15 +20,15 @@
     * {{_link['title']_}}
     * {% endfor %}
  {% endif %}
 ## Please leave this link and use one of the logos provided ## The OpenEdX link
 may be hidden when this view is served ## through an API to partner sites (such
 as marketing sites or blogs), ## which are not technically powered by Open edX.
 % if not hide_openedx_link:
-[${static.url('images/tutor-logo.png')}] [${footer['openedx_link']['title']}]
+[Runs_on_Tutor] [${footer['openedx_link']['title']}]
 % endif
 % else:
 # When rendering the footer through the branding API, ## the direction may not
 be set on the parent element, ## so we set it here. % if bidi: dir=${bidi} %
 endif >
 {% if INDIGO_FOOTER_NAV_LINKS %}
    1. {% for link in INDIGO_FOOTER_NAV_LINKS %}
@@ -53,14 +53,14 @@
     * {{_link['title']_}}
     * {% endfor %}
  {% endif %}
 ## Please leave this link and use one of the logos provided ## The OpenEdX link
 may be hidden when this view is served ## through an API to partner sites (such
 as marketing sites or blogs), ## which are not technically powered by OpenEdX.
 % if not hide_openedx_link:
-[${static.url('images/tutor-logo.png')}] [${footer['openedx_link']['title']}]
+[Runs_on_Tutor] [${footer['openedx_link']['title']}]
 % endif
 % endif % if include_dependencies: <%static:js group='base_vendor'/> <%static:
 css group='style-vendor'/> <%include file="widgets/segment-io.html" /
 > <%include file="widgets/segment-io-footer.html" /> % endif % if
 footer_css_urls: % for url in footer_css_urls:
  % endfor % endif
```

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/about.html` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/about.html`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/contact.html` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/contact.html`

 * *Files identical despite different names*

### Comparing `tutor-indigo-14.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/tos.html` & `tutor-indigo-15.0.0/tutorindigo/templates/indigo/lms/templates/static_templates/tos.html`

 * *Files identical despite different names*

