# Comparing `tmp/wagtail-katex-0.0.4.tar.gz` & `tmp/wagtail-katex-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-katex-0.0.4.tar", last modified: Wed Jun 14 14:56:31 2023, max compression
+gzip compressed data, was "wagtail-katex-0.0.5.tar", last modified: Thu Jun 15 13:37:30 2023, max compression
```

## Comparing `wagtail-katex-0.0.4.tar` & `wagtail-katex-0.0.5.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.178448 wagtail-katex-0.0.4/
--rw-r--r--   0 chii       (501) staff       (20)    11357 2022-03-05 02:43:30.000000 wagtail-katex-0.0.4/LICENSE
--rw-r--r--   0 chii       (501) staff       (20)      100 2023-06-14 14:55:14.000000 wagtail-katex-0.0.4/MANIFEST.in
--rw-r--r--   0 chii       (501) staff       (20)     2011 2023-06-14 14:56:31.178270 wagtail-katex-0.0.4/PKG-INFO
--rw-r--r--   0 chii       (501) staff       (20)      918 2022-05-28 08:01:07.000000 wagtail-katex-0.0.4/README.md
--rw-r--r--   0 chii       (501) staff       (20)       38 2023-06-14 14:56:31.178501 wagtail-katex-0.0.4/setup.cfg
--rw-r--r--   0 chii       (501) staff       (20)     1436 2023-06-14 14:44:59.000000 wagtail-katex-0.0.4/setup.py
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.164939 wagtail-katex-0.0.4/wagtail_katex.egg-info/
--rw-r--r--   0 chii       (501) staff       (20)     2011 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/PKG-INFO
--rw-r--r--   0 chii       (501) staff       (20)     4847 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/SOURCES.txt
--rw-r--r--   0 chii       (501) staff       (20)        1 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/dependency_links.txt
--rw-r--r--   0 chii       (501) staff       (20)       11 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/requires.txt
--rw-r--r--   0 chii       (501) staff       (20)       13 2023-06-14 14:56:31.000000 wagtail-katex-0.0.4/wagtail_katex.egg-info/top_level.txt
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.165453 wagtail-katex-0.0.4/wagtailkatex/
--rw-r--r--   0 chii       (501) staff       (20)       22 2023-06-13 00:40:46.000000 wagtail-katex-0.0.4/wagtailkatex/__init__.py
--rwxr-xr-x   0 chii       (501) staff       (20)      860 2023-06-13 00:40:46.000000 wagtail-katex-0.0.4/wagtailkatex/richtext.py
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.165614 wagtail-katex-0.0.4/wagtailkatex/static/
--rw-r--r--   0 chii       (501) staff       (20)     6148 2021-03-04 07:31:57.000000 wagtail-katex-0.0.4/wagtailkatex/static/.DS_Store
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.165776 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.166319 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/
--rw-r--r--   0 chii       (501) staff       (20)     7119 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/README.md
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.177824 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/
--rw-r--r--   0 chii       (501) staff       (20)    63632 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    33516 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    28076 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    12368 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)     7716 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)     6912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    12344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     7656 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     6908 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    19584 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)    13296 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)    11348 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    19572 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    13208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    11316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    51336 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)    29912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)    25324 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    32968 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    19412 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16780 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    33580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    19676 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16988 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    53580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    30772 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    26272 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    31196 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    18668 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16400 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    31308 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    18748 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 chii       (501) staff       (20)    16440 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    24504 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf
--rw-r--r--   0 chii       (501) staff       (20)    14408 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 chii       (501) staff       (20)    12216 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 chii       (501) staff       (20)    22364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf
--rw-r--r--   0 chii       (501) staff       (20)    14112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 chii       (501) staff       (20)    12028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 chii       (501) staff       (20)    19436 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    12316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    10344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    16648 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    10588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     9644 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    12228 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     6496 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     5468 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    11508 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     6188 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     5208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)     7588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     4420 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     3624 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    10364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)     5980 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)     4928 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    27556 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf
--rw-r--r--   0 chii       (501) staff       (20)    16028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 chii       (501) staff       (20)    13568 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2
--rw-r--r--   0 chii       (501) staff       (20)    23112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/katex.min.css
--rw-r--r--   0 chii       (501) staff       (20)   270375 2022-01-12 17:36:05.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/katex.min.js
--rwxr-xr-x   0 chii       (501) staff       (20)     3868 2022-05-28 07:44:46.000000 wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/wagtailkatex.js
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.163401 wagtail-katex-0.0.4/wagtailkatex/templates/
-drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-14 14:56:31.178011 wagtail-katex-0.0.4/wagtailkatex/templates/wagtailkatex/
--rw-r--r--   0 chii       (501) staff       (20)      875 2023-06-14 14:42:43.000000 wagtail-katex-0.0.4/wagtailkatex/templates/wagtailkatex/square-root-variable.svg
--rwxr-xr-x   0 chii       (501) staff       (20)     1562 2023-06-14 14:42:58.000000 wagtail-katex-0.0.4/wagtailkatex/wagtail_hooks.py
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.901672 wagtail-katex-0.0.5/
+-rw-r--r--   0 chii       (501) staff       (20)    11357 2022-03-05 02:43:30.000000 wagtail-katex-0.0.5/LICENSE
+-rw-r--r--   0 chii       (501) staff       (20)      100 2023-06-14 14:55:14.000000 wagtail-katex-0.0.5/MANIFEST.in
+-rw-r--r--   0 chii       (501) staff       (20)     1810 2023-06-15 13:37:30.901507 wagtail-katex-0.0.5/PKG-INFO
+-rw-r--r--   0 chii       (501) staff       (20)      717 2023-06-15 13:35:13.000000 wagtail-katex-0.0.5/README.md
+-rw-r--r--   0 chii       (501) staff       (20)       38 2023-06-15 13:37:30.901725 wagtail-katex-0.0.5/setup.cfg
+-rw-r--r--   0 chii       (501) staff       (20)     1436 2023-06-14 14:44:59.000000 wagtail-katex-0.0.5/setup.py
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.887086 wagtail-katex-0.0.5/wagtail_katex.egg-info/
+-rw-r--r--   0 chii       (501) staff       (20)     1810 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/PKG-INFO
+-rw-r--r--   0 chii       (501) staff       (20)     4897 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/SOURCES.txt
+-rw-r--r--   0 chii       (501) staff       (20)        1 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/dependency_links.txt
+-rw-r--r--   0 chii       (501) staff       (20)       11 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/requires.txt
+-rw-r--r--   0 chii       (501) staff       (20)       13 2023-06-15 13:37:30.000000 wagtail-katex-0.0.5/wagtail_katex.egg-info/top_level.txt
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.887632 wagtail-katex-0.0.5/wagtailkatex/
+-rw-r--r--   0 chii       (501) staff       (20)       22 2023-06-15 13:31:02.000000 wagtail-katex-0.0.5/wagtailkatex/__init__.py
+-rwxr-xr-x   0 chii       (501) staff       (20)      860 2023-06-15 12:07:36.000000 wagtail-katex-0.0.5/wagtailkatex/richtext.py
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.887817 wagtail-katex-0.0.5/wagtailkatex/static/
+-rw-r--r--   0 chii       (501) staff       (20)     6148 2021-03-04 07:31:57.000000 wagtail-katex-0.0.5/wagtailkatex/static/.DS_Store
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.888182 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.888808 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/
+-rw-r--r--   0 chii       (501) staff       (20)     7119 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/README.md
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.901032 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/
+-rw-r--r--   0 chii       (501) staff       (20)    63632 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    33516 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    28076 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    12368 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     7716 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)     6912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    12344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     7656 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     6908 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    19584 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    13296 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)    11348 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    19572 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    13208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    11316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    51336 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    29912 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)    25324 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    32968 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    19412 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16780 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    33580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    19676 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16988 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    53580 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    30772 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    26272 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    31196 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    18668 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16400 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    31308 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    18748 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    16440 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    24504 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    14408 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 chii       (501) staff       (20)    12216 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    22364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    14112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 chii       (501) staff       (20)    12028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    19436 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    12316 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    10344 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    16648 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    10588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     9644 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    12228 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     6496 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     5468 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    11508 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     6188 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     5208 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)     7588 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     4420 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     3624 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    10364 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)     5980 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)     4928 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    27556 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf
+-rw-r--r--   0 chii       (501) staff       (20)    16028 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 chii       (501) staff       (20)    13568 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2
+-rw-r--r--   0 chii       (501) staff       (20)    23112 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/katex.min.css
+-rw-r--r--   0 chii       (501) staff       (20)   270375 2022-01-12 17:36:05.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/katex.min.js
+-rw-r--r--   0 chii       (501) staff       (20)      736 2023-06-15 13:12:39.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/wagtailkatex.css
+-rwxr-xr-x   0 chii       (501) staff       (20)     5380 2023-06-15 12:07:10.000000 wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/wagtailkatex.js
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.885483 wagtail-katex-0.0.5/wagtailkatex/templates/
+drwxr-xr-x   0 chii       (501) staff       (20)        0 2023-06-15 13:37:30.901237 wagtail-katex-0.0.5/wagtailkatex/templates/wagtailkatex/
+-rw-r--r--   0 chii       (501) staff       (20)      875 2023-06-14 14:42:43.000000 wagtail-katex-0.0.5/wagtailkatex/templates/wagtailkatex/square-root-variable.svg
+-rwxr-xr-x   0 chii       (501) staff       (20)     1700 2023-06-15 13:27:25.000000 wagtail-katex-0.0.5/wagtailkatex/wagtail_hooks.py
```

### Comparing `wagtail-katex-0.0.4/LICENSE` & `wagtail-katex-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/PKG-INFO` & `wagtail-katex-0.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-katex
-Version: 0.0.4
+Version: 0.0.5
 Summary: KaTex for Wagtail CMS Draftail editor
 Home-page: https://github.com/ongchi/wagtail-katex
 Author: ongchi
 Author-email: ongchi@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ongchi/wagtail-katex/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -22,23 +22,21 @@
 Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
 Classifier: Framework :: Wagtail :: 5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# wagtail-katex ![Wagtail 2.x](https://img.shields.io/badge/wagtail-2.x-g.svg) ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg)
+# wagtail-katex ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg) ![Wagtail 4.x](https://img.shields.io/badge/wagtail-4.x-g.svg) ![Wagtail 5.x](https://img.shields.io/badge/wagtail-5.x-g.svg)
 
 > This package is modified from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex)
 
-**[KaTex](https://katex.org)** support for Wagtail RichTextField.
+**[KaTeX](https://katex.org)** support for Wagtail RichTextField.
 
-![Inserting an Images](https://raw.githubusercontent.com/gatensj/wagtail-draftail-katex/master/images/screenshot06152018-1.png)
-
-![Image Editor](https://raw.githubusercontent.com/gatensj/wagtail-draftail-katex/master/images/screenshot06152018-2.png)
+![KaTeX Editor](https://raw.githubusercontent.com/ongchi/wagtail-katex/master/images/screenshot.png)
 
 ## Quick Start
 
 Install the package with
 
 ```sh
 pip install wagtail-katex
@@ -49,13 +47,7 @@
 ```python
 INSTALLED_APPS = [
     ...
     "wagtailkatex",
     ...
 ]
 ```
-
-Add `katex-embed` to `RichTextField` features:
-
-```python
-body = RichTextField(features=[..., "katex-embed"])
-```
```

### Comparing `wagtail-katex-0.0.4/README.md` & `wagtail-katex-0.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# wagtail-katex ![Wagtail 2.x](https://img.shields.io/badge/wagtail-2.x-g.svg) ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg)
+# wagtail-katex ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg) ![Wagtail 4.x](https://img.shields.io/badge/wagtail-4.x-g.svg) ![Wagtail 5.x](https://img.shields.io/badge/wagtail-5.x-g.svg)
 
 > This package is modified from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex)
 
-**[KaTex](https://katex.org)** support for Wagtail RichTextField.
+**[KaTeX](https://katex.org)** support for Wagtail RichTextField.
 
-![Inserting an Images](https://raw.githubusercontent.com/gatensj/wagtail-draftail-katex/master/images/screenshot06152018-1.png)
-
-![Image Editor](https://raw.githubusercontent.com/gatensj/wagtail-draftail-katex/master/images/screenshot06152018-2.png)
+![KaTeX Editor](https://raw.githubusercontent.com/ongchi/wagtail-katex/master/images/screenshot.png)
 
 ## Quick Start
 
 Install the package with
 
 ```sh
 pip install wagtail-katex
@@ -21,13 +19,7 @@
 ```python
 INSTALLED_APPS = [
     ...
     "wagtailkatex",
     ...
 ]
 ```
-
-Add `katex-embed` to `RichTextField` features:
-
-```python
-body = RichTextField(features=[..., "katex-embed"])
-```
```

### Comparing `wagtail-katex-0.0.4/setup.py` & `wagtail-katex-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtail_katex.egg-info/PKG-INFO` & `wagtail-katex-0.0.5/wagtail_katex.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-katex
-Version: 0.0.4
+Version: 0.0.5
 Summary: KaTex for Wagtail CMS Draftail editor
 Home-page: https://github.com/ongchi/wagtail-katex
 Author: ongchi
 Author-email: ongchi@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/ongchi/wagtail-katex/issues
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -22,23 +22,21 @@
 Classifier: Framework :: Wagtail :: 3
 Classifier: Framework :: Wagtail :: 4
 Classifier: Framework :: Wagtail :: 5
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# wagtail-katex ![Wagtail 2.x](https://img.shields.io/badge/wagtail-2.x-g.svg) ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg)
+# wagtail-katex ![Wagtail 3.x](https://img.shields.io/badge/wagtail-3.x-g.svg) ![Wagtail 4.x](https://img.shields.io/badge/wagtail-4.x-g.svg) ![Wagtail 5.x](https://img.shields.io/badge/wagtail-5.x-g.svg)
 
 > This package is modified from [gatensj/wagtail-draftail-katex](https://github.com/gatensj/wagtail-draftail-katex)
 
-**[KaTex](https://katex.org)** support for Wagtail RichTextField.
+**[KaTeX](https://katex.org)** support for Wagtail RichTextField.
 
-![Inserting an Images](https://raw.githubusercontent.com/gatensj/wagtail-draftail-katex/master/images/screenshot06152018-1.png)
-
-![Image Editor](https://raw.githubusercontent.com/gatensj/wagtail-draftail-katex/master/images/screenshot06152018-2.png)
+![KaTeX Editor](https://raw.githubusercontent.com/ongchi/wagtail-katex/master/images/screenshot.png)
 
 ## Quick Start
 
 Install the package with
 
 ```sh
 pip install wagtail-katex
@@ -49,13 +47,7 @@
 ```python
 INSTALLED_APPS = [
     ...
     "wagtailkatex",
     ...
 ]
 ```
-
-Add `katex-embed` to `RichTextField` features:
-
-```python
-body = RichTextField(features=[..., "katex-embed"])
-```
```

### Comparing `wagtail-katex-0.0.4/wagtail_katex.egg-info/SOURCES.txt` & `wagtail-katex-0.0.5/wagtail_katex.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 wagtail_katex.egg-info/dependency_links.txt
 wagtail_katex.egg-info/requires.txt
 wagtail_katex.egg-info/top_level.txt
 wagtailkatex/__init__.py
 wagtailkatex/richtext.py
 wagtailkatex/wagtail_hooks.py
 wagtailkatex/static/.DS_Store
+wagtailkatex/static/wagtailkatex/wagtailkatex.css
 wagtailkatex/static/wagtailkatex/wagtailkatex.js
 wagtailkatex/static/wagtailkatex/katex/README.md
 wagtailkatex/static/wagtailkatex/katex/katex.min.css
 wagtailkatex/static/wagtailkatex/katex/katex.min.js
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff
 wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2
```

### Comparing `wagtail-katex-0.0.4/wagtailkatex/richtext.py` & `wagtail-katex-0.0.5/wagtailkatex/richtext.py`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/.DS_Store` & `wagtail-katex-0.0.5/wagtailkatex/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/README.md` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/fonts/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/katex.min.css` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/katex.min.css`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/static/wagtailkatex/katex/katex.min.js` & `wagtail-katex-0.0.5/wagtailkatex/static/wagtailkatex/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/templates/wagtailkatex/square-root-variable.svg` & `wagtail-katex-0.0.5/wagtailkatex/templates/wagtailkatex/square-root-variable.svg`

 * *Files identical despite different names*

### Comparing `wagtail-katex-0.0.4/wagtailkatex/wagtail_hooks.py` & `wagtail-katex-0.0.5/wagtailkatex/wagtail_hooks.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from wagtail.admin.rich_text.editors.draftail import features as draftail_features
 from wagtail import hooks
 
 from .richtext import KaTeXEntityElementHandler, katex_entity_decorator
 
 
 @hooks.register('register_rich_text_features')
-def register_katex_features(features):
-    features.default_features.append('katex')
+def register_katex_feature(features):
+    features.default_features.append('katex-embed')
+
     """
-    Registering the `katex` feature, which uses the `KATEX` Draft.js entity type,
-    and is stored as HTML with a `<div data-katex-embed="c = \\pm\\sqrt{a^2 + b^2}">`
-    tag.
+    Registering the `katex-embed` feature, which uses the `KATEX` Draft.js entity type,
+    and is stored as HTML with a `div[data-katex-embed]` tag.
     """
     feature_name = 'katex-embed'
     type_ = 'KATEX-EMBED'
 
     features.register_editor_plugin(
         'draftail',
         feature_name,
@@ -29,23 +29,32 @@
             js=[
                 'wagtailkatex/katex/katex.min.js',
                 'wagtailkatex/wagtailkatex.js',
             ],
             css={
                 'all': [
                     'wagtailkatex/katex/katex.min.css',
+                    'wagtailkatex/wagtailkatex.css',
                 ]
-            }
-        )
+            },
+        ),
     )
 
-    features.register_converter_rule('contentstate', feature_name, {
-        'from_database_format': {'div[data-katex-embed]': KaTeXEntityElementHandler()},
-        'to_database_format': {'entity_decorators': {type_: katex_entity_decorator}},
-    })
+    features.register_converter_rule(
+        'contentstate',
+        feature_name,
+        {
+            'from_database_format': {
+                'div[data-katex-embed]': KaTeXEntityElementHandler()
+            },
+            'to_database_format': {
+                'entity_decorators': {type_: katex_entity_decorator}
+            },
+        },
+    )
 
 
 @hooks.register('register_icons')
 def register_icons(icons):
     return icons + [
-        "wagtailkatex/square-root-variable.svg"
+        'wagtailkatex/square-root-variable.svg',
     ]
```

