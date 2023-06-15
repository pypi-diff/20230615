# Comparing `tmp/webviz_config_equinor-0.2.4-py3-none-any.whl.zip` & `tmp/webviz_config_equinor-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6571 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1342 b- defN 22-Aug-03 11:59 webviz_config_equinor/__init__.py
--rw-r--r--  2.0 unx     1449 b- defN 22-Aug-03 11:59 webviz_config_equinor/assets/equinor_logo_symbol.svg
--rw-r--r--  2.0 unx     4526 b- defN 22-Aug-03 11:59 webviz_config_equinor/assets/equinor_theme.css
--rw-r--r--  2.0 unx     1150 b- defN 22-Aug-03 11:59 webviz_config_equinor/assets/favicon.ico
--rw-r--r--  2.0 unx     3483 b- defN 22-Aug-03 12:00 webviz_config_equinor-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-03 12:00 webviz_config_equinor-0.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       76 b- defN 22-Aug-03 12:00 webviz_config_equinor-0.2.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 22-Aug-03 12:00 webviz_config_equinor-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      862 b- defN 22-Aug-03 12:00 webviz_config_equinor-0.2.4.dist-info/RECORD
-9 files, 13002 bytes uncompressed, 5047 bytes compressed:  61.2%
+Zip file size: 6538 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1330 b- defN 23-Jun-15 11:55 webviz_config_equinor/__init__.py
+-rw-r--r--  2.0 unx     1449 b- defN 23-Jun-15 11:55 webviz_config_equinor/assets/equinor_logo_symbol.svg
+-rw-r--r--  2.0 unx     4523 b- defN 23-Jun-15 11:55 webviz_config_equinor/assets/equinor_theme.css
+-rw-r--r--  2.0 unx     1150 b- defN 23-Jun-15 11:55 webviz_config_equinor/assets/favicon.ico
+-rw-r--r--  2.0 unx     3434 b- defN 23-Jun-15 11:56 webviz_config_equinor-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 11:56 webviz_config_equinor-0.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-15 11:56 webviz_config_equinor-0.2.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-15 11:56 webviz_config_equinor-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      862 b- defN 23-Jun-15 11:56 webviz_config_equinor-0.2.5.dist-info/RECORD
+9 files, 12937 bytes uncompressed, 5014 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: webviz_config_equinor/assets/equinor_theme.css
 Comment: 
 
 Filename: webviz_config_equinor/assets/favicon.ico
 Comment: 
 
-Filename: webviz_config_equinor-0.2.4.dist-info/METADATA
+Filename: webviz_config_equinor-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: webviz_config_equinor-0.2.4.dist-info/WHEEL
+Filename: webviz_config_equinor-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: webviz_config_equinor-0.2.4.dist-info/entry_points.txt
+Filename: webviz_config_equinor-0.2.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: webviz_config_equinor-0.2.4.dist-info/top_level.txt
+Filename: webviz_config_equinor-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: webviz_config_equinor-0.2.4.dist-info/RECORD
+Filename: webviz_config_equinor-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webviz_config_equinor/__init__.py

```diff
@@ -11,22 +11,22 @@
     # package is not installed
     pass
 
 
 equinor_theme = WebvizConfigTheme(theme_name="equinor")
 
 equinor_theme.external_stylesheets = [
-    "https://eds-static.equinor.com/font/equinor-font.css"
+    "https://cdn.eds.equinor.com/font/equinor-font.css"
 ]
 
 equinor_theme.adjust_csp(
     {
-        "font-src": ["https://eds-static.equinor.com"],
-        "img-src": ["https://eds-static.equinor.com"],
-        "style-src": ["https://eds-static.equinor.com"],
+        "font-src": ["https://cdn.eds.equinor.com"],
+        "img-src": ["https://cdn.eds.equinor.com"],
+        "style-src": ["https://cdn.eds.equinor.com"],
     },
     append=True,
 )
 
 equinor_theme.assets = glob.glob(
     os.path.join(os.path.dirname(os.path.abspath(__file__)), "assets", "*")
 )
```

## webviz_config_equinor/assets/equinor_theme.css

```diff
@@ -105,15 +105,15 @@
   border-top: 1px #e1e1e1 solid;
 }
 
 #LogoLarge {
   height: 100px;
   width: 200px;
   background-size: contain;
-  background-image: url("https://eds-static.equinor.com/logo/equinor-logo-primary.svg#red");
+  background-image: url("https://cdn.eds.equinor.com/logo/equinor-logo-primary.svg#red");
   background-repeat: no-repeat;
 }
 
 #LogoSmall {
   height: 56px;
   width: 56px;
   background-size: contain;
```

## Comparing `webviz_config_equinor-0.2.4.dist-info/METADATA` & `webviz_config_equinor-0.2.5.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: webviz-config-equinor
-Version: 0.2.4
+Version: 0.2.5
 Summary: Webviz config Equinor theme
 Home-page: https://github.com/equinor/webviz-config-equinor
 Author: R&T Equinor
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: Other/Proprietary License
-Requires-Python: ~=3.6
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: plotly (>=5.0)
 Requires-Dist: webviz-config (>=0.0.48)
 Provides-Extra: tests
 Requires-Dist: black ; extra == 'tests'
 
 [![PyPI version](https://badge.fury.io/py/webviz-config-equinor.svg)](https://badge.fury.io/py/webviz-config-equinor)
 [![Build Status](https://github.com/equinor/webviz-config-equinor/workflows/webviz-config-equinor/badge.svg)](https://github.com/equinor/webviz-config-equinor/actions?query=branch%3Amaster)
 [![Total alerts](https://img.shields.io/lgtm/alerts/g/equinor/webviz-config-equinor.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/equinor/webviz-config-equinor/alerts/)
 [![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/equinor/webviz-config-equinor.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/equinor/webviz-config-equinor/context:python)
-[![Python 3.6 | 3.7 | 3.8 | 3.9](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9-blue.svg)](https://www.python.org/)
+[![Python 3.8 | 3.9](https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9-blue.svg)](https://www.python.org/)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
 # Webviz config theme for Equinor
 
 Enables Equinor theme for Webviz applications build through `webviz-config`.
 
 The simplest way of installing `webviz-config-equinor` is to run
@@ -75,9 +73,7 @@
 information contained in it.
 
 This notice shall be governed by and construed in accordance with Norwegian law.
 
 If any provision of this notice shall be unlawful, void or for any reason
 unenforceable then that provision shall be deemed severable and shall not
 affect the validity and enforcability of the remaining provisions.
-
-
```

## Comparing `webviz_config_equinor-0.2.4.dist-info/RECORD` & `webviz_config_equinor-0.2.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-webviz_config_equinor/__init__.py,sha256=vmeWR_tO7klDhGEuS6tEPK6Zz9-wb0sdj0KA1MDCl7U,1342
+webviz_config_equinor/__init__.py,sha256=2rRQ3bF94BPQrOAH94zXpE_RV558h4gTitRMsJS8A2c,1330
 webviz_config_equinor/assets/equinor_logo_symbol.svg,sha256=YX9f78vDemT6NtMpKtfkz2X1Z8D8t2MFadYSEZpO5vE,1449
-webviz_config_equinor/assets/equinor_theme.css,sha256=2Hyg9-0AWUCSkdfkB4PTnbiqGjjmVt6kYFoCOlhj-FU,4526
+webviz_config_equinor/assets/equinor_theme.css,sha256=j-5gnLHk6bs51uhCazdhMD7w3oHPeo7lyUbn5-vw-DI,4523
 webviz_config_equinor/assets/favicon.ico,sha256=Tm2cuq-XhjbPGWBtyMY1BV51bpFma2QN6MPGbT3Qpuo,1150
-webviz_config_equinor-0.2.4.dist-info/METADATA,sha256=mhk8YfBcjF7U6yLcqaGsTbE3zTWeTinRwLD2C0td-pA,3483
-webviz_config_equinor-0.2.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-webviz_config_equinor-0.2.4.dist-info/entry_points.txt,sha256=Ryi2u_g6rADTw-aQaYfoHI1tNZwtpUuWHYskNRr9Q3M,76
-webviz_config_equinor-0.2.4.dist-info/top_level.txt,sha256=Ldkcj1DKhEniKeAhFDgD8SQp-8l67fvWHOiUFIkwle4,22
-webviz_config_equinor-0.2.4.dist-info/RECORD,,
+webviz_config_equinor-0.2.5.dist-info/METADATA,sha256=L2cC0oqk5wlu2LHEZZ5jFGytktSbiCAOGziNYI7EeFM,3434
+webviz_config_equinor-0.2.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+webviz_config_equinor-0.2.5.dist-info/entry_points.txt,sha256=dV7eHkGrE6pvbVsGraByJk1D1lHUzv0_rcZ604OS2Do,75
+webviz_config_equinor-0.2.5.dist-info/top_level.txt,sha256=Ldkcj1DKhEniKeAhFDgD8SQp-8l67fvWHOiUFIkwle4,22
+webviz_config_equinor-0.2.5.dist-info/RECORD,,
```

