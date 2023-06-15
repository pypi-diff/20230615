# Comparing `tmp/absfuyu-2.1.0.tar.gz` & `tmp/absfuyu-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\.tmp-4gqxm6y2\absfuyu-2.1.0.tar", last modified: Thu Jun 15 07:31:15 2023, max compression
+gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\.tmp-ki_676fk\absfuyu-2.1.1.tar", last modified: Thu Jun 15 08:11:27 2023, max compression
```

## Comparing `absfuyu-2.1.0.tar` & `absfuyu-2.1.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/
--rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-2.1.0/LICENSE
--rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-2.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3836 2023-06-15 07:31:15.000000 absfuyu-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-2.1.0/README.md
--rw-rw-rw-   0        0        0     1161 2023-06-05 17:50:56.000000 absfuyu-2.1.0/extra_requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/images/
--rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-2.1.0/images/repository-image-crop.png
--rw-rw-rw-   0        0        0      193 2023-06-05 17:50:56.000000 absfuyu-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-2.1.0/requirements.txt
--rw-rw-rw-   0        0        0     1360 2023-06-15 07:31:15.000000 absfuyu-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1009 2022-06-19 18:29:54.000000 absfuyu-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/
--rw-rw-rw-   0        0        0     1004 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/__init__.py
--rw-rw-rw-   0        0        0     6530 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/__main__.py
--rw-rw-rw-   0        0        0     2566 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/calculation.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/code_red/
--rw-rw-rw-   0        0        0     5580 2022-02-17 09:30:21.000000 absfuyu-2.1.0/src/absfuyu/code_red/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/collections/
--rw-rw-rw-   0        0        0     1938 2023-06-09 13:43:36.000000 absfuyu-2.1.0/src/absfuyu/collections/__init__.py
--rw-rw-rw-   0        0        0    14620 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/collections/content.py
--rw-rw-rw-   0        0        0    20864 2023-06-15 07:26:41.000000 absfuyu-2.1.0/src/absfuyu/collections/data_extension.py
--rw-rw-rw-   0        0        0     6742 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/collections/generator.py
--rw-rw-rw-   0        0        0     5822 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/collections/human.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/config/
--rw-rw-rw-   0        0        0     4234 2023-05-24 23:10:03.000000 absfuyu-2.1.0/src/absfuyu/config/__init__.py
--rw-rw-rw-   0        0        0      791 2023-06-15 07:30:57.000000 absfuyu-2.1.0/src/absfuyu/config/config.json
--rw-rw-rw-   0        0        0     1555 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/config/config2.py
--rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-2.1.0/src/absfuyu/config/template.json
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/contrib/
--rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-2.1.0/src/absfuyu/contrib/__init__.py
--rw-rw-rw-   0        0        0     8190 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/contrib/basic_lunar_calendar.py
--rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-2.1.0/src/absfuyu/contrib/color_extract.py
--rw-rw-rw-   0        0        0     3313 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/core.py
--rw-rw-rw-   0        0        0      832 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/everything.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/extensions/
--rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-2.1.0/src/absfuyu/extensions/__init__.py
--rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-2.1.0/src/absfuyu/extensions/beautiful.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/
--rw-rw-rw-   0        0        0    11971 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/WGS.py
--rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/__init__.py
--rw-rw-rw-   0        0        0    11987 2022-06-19 18:02:35.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/horoscope.py
--rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/password_hash.py
--rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/pkglib.py
--rw-rw-rw-   0        0        0    16508 2022-06-19 15:56:37.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/primo_cal.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/short_link/
--rw-rw-rw-   0        0        0      150 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/short_link/__init__.py
--rw-rw-rw-   0        0        0     5069 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/short_link/rebrandly.py
--rw-rw-rw-   0        0        0     2775 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/tarot.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/extensions/extra/
--rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-2.1.0/src/absfuyu/extensions/extra/__init__.py
--rw-rw-rw-   0        0        0     6812 2023-05-24 23:10:03.000000 absfuyu-2.1.0/src/absfuyu/extensions/extra/data_analysis.py
--rw-rw-rw-   0        0        0     6001 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/fun.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/game/
--rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-2.1.0/src/absfuyu/game/__init__.py
--rw-rw-rw-   0        0        0     8258 2023-05-24 23:10:03.000000 absfuyu-2.1.0/src/absfuyu/game/sudoku.py
--rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-2.1.0/src/absfuyu/game/tictactoe.py
--rw-rw-rw-   0        0        0   101067 2023-05-24 23:10:03.000000 absfuyu-2.1.0/src/absfuyu/game/wordle.py
--rw-rw-rw-   0        0        0     3752 2023-06-09 09:17:28.000000 absfuyu-2.1.0/src/absfuyu/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/
--rw-rw-rw-   0        0        0     3043 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/__init__.py
--rw-rw-rw-   0        0        0   247094 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/chemistry.json
--rw-rw-rw-   0        0        0        0 2022-01-29 17:00:32.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/dummy.dat
--rw-rw-rw-   0        0        0       31 2022-02-03 13:01:43.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/punishment_windows.dat
--rw-rw-rw-   0        0        0    86614 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/tarot.json
--rw-rw-rw-   0        0        0     5882 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/sort.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/tools/
--rw-rw-rw-   0        0        0      136 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/__init__.py
--rw-rw-rw-   0        0        0     5853 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/converter.py
--rw-rw-rw-   0        0        0     7292 2023-06-09 14:49:10.000000 absfuyu-2.1.0/src/absfuyu/tools/keygen.py
--rw-rw-rw-   0        0        0     8482 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/obfuscator.py
--rw-rw-rw-   0        0        0     3008 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/stats.py
--rw-rw-rw-   0        0        0     1180 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/web.py
--rw-rw-rw-   0        0        0    12499 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/unused.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/util/
--rw-rw-rw-   0        0        0     2396 2023-06-09 13:47:13.000000 absfuyu-2.1.0/src/absfuyu/util/__init__.py
--rw-rw-rw-   0        0        0     2769 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/api.py
--rw-rw-rw-   0        0        0     2366 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/json_method.py
--rw-rw-rw-   0        0        0     5605 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/path.py
--rw-rw-rw-   0        0        0     3829 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/performance.py
--rw-rw-rw-   0        0        0     1230 2023-06-09 13:48:37.000000 absfuyu-2.1.0/src/absfuyu/util/pkl.py
--rw-rw-rw-   0        0        0     2499 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/zipped.py
--rw-rw-rw-   0        0        0     8504 2022-02-19 16:37:01.000000 absfuyu-2.1.0/src/absfuyu/version.py
--rw-rw-rw-   0        0        0     9951 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/version2.py
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/
--rw-rw-rw-   0        0        0     3836 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2639 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1266 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/tests/
--rw-rw-rw-   0        0        0      805 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_DictKai.py
--rw-rw-rw-   0        0        0     3049 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_Generator.py
--rw-rw-rw-   0        0        0     3206 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_IntNumber.py
--rw-rw-rw-   0        0        0     2068 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_ListKai.py
--rw-rw-rw-   0        0        0     3246 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_Text.py
--rw-rw-rw-   0        0        0      632 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_api.py
--rw-rw-rw-   0        0        0      111 2022-02-18 13:22:03.000000 absfuyu-2.1.0/tests/test_beautiful.py
--rw-rw-rw-   0        0        0      691 2022-02-18 12:50:08.000000 absfuyu-2.1.0/tests/test_config.py
--rw-rw-rw-   0        0        0      769 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_converter.py
--rw-rw-rw-   0        0        0      108 2022-02-18 13:23:43.000000 absfuyu-2.1.0/tests/test_everything.py
--rw-rw-rw-   0        0        0      111 2022-02-18 12:31:52.000000 absfuyu-2.1.0/tests/test_extensions.py
--rw-rw-rw-   0        0        0      205 2022-06-19 18:50:45.000000 absfuyu-2.1.0/tests/test_fun.py
--rw-rw-rw-   0        0        0      425 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_json_method.py
--rw-rw-rw-   0        0        0      706 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_obfuscator.py
--rw-rw-rw-   0        0        0      649 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_path.py
--rw-rw-rw-   0        0        0      119 2023-05-25 10:14:50.000000 absfuyu-2.1.0/tests/test_pkg_data.py
--rw-rw-rw-   0        0        0     1133 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/
+-rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-2.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3836 2023-06-15 08:11:27.000000 absfuyu-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-2.1.1/README.md
+-rw-rw-rw-   0        0        0     1161 2023-06-05 17:50:56.000000 absfuyu-2.1.1/extra_requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.000000 absfuyu-2.1.1/images/
+-rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-2.1.1/images/repository-image-crop.png
+-rw-rw-rw-   0        0        0      193 2023-06-05 17:50:56.000000 absfuyu-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-2.1.1/requirements.txt
+-rw-rw-rw-   0        0        0     1360 2023-06-15 08:11:27.000000 absfuyu-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2022-06-19 18:29:54.000000 absfuyu-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu/
+-rw-rw-rw-   0        0        0     1004 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/__init__.py
+-rw-rw-rw-   0        0        0     6530 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/__main__.py
+-rw-rw-rw-   0        0        0     2566 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/calculation.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/code_red/
+-rw-rw-rw-   0        0        0     5580 2022-02-17 09:30:21.000000 absfuyu-2.1.1/src/absfuyu/code_red/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/collections/
+-rw-rw-rw-   0        0        0     1938 2023-06-09 13:43:36.000000 absfuyu-2.1.1/src/absfuyu/collections/__init__.py
+-rw-rw-rw-   0        0        0    14620 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/collections/content.py
+-rw-rw-rw-   0        0        0    20864 2023-06-15 07:26:41.000000 absfuyu-2.1.1/src/absfuyu/collections/data_extension.py
+-rw-rw-rw-   0        0        0     6742 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/collections/generator.py
+-rw-rw-rw-   0        0        0     5822 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/collections/human.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/config/
+-rw-rw-rw-   0        0        0     4234 2023-05-24 23:10:03.000000 absfuyu-2.1.1/src/absfuyu/config/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-06-15 08:11:14.000000 absfuyu-2.1.1/src/absfuyu/config/config.json
+-rw-rw-rw-   0        0        0     1555 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/config/config2.py
+-rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-2.1.1/src/absfuyu/config/template.json
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/contrib/
+-rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-2.1.1/src/absfuyu/contrib/__init__.py
+-rw-rw-rw-   0        0        0     8190 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/contrib/basic_lunar_calendar.py
+-rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-2.1.1/src/absfuyu/contrib/color_extract.py
+-rw-rw-rw-   0        0        0     3313 2023-06-15 07:52:56.000000 absfuyu-2.1.1/src/absfuyu/core.py
+-rw-rw-rw-   0        0        0      832 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/everything.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/extensions/
+-rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-2.1.1/src/absfuyu/extensions/__init__.py
+-rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-2.1.1/src/absfuyu/extensions/beautiful.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/
+-rw-rw-rw-   0        0        0    11971 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/WGS.py
+-rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/__init__.py
+-rw-rw-rw-   0        0        0    11987 2022-06-19 18:02:35.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/horoscope.py
+-rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/password_hash.py
+-rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/pkglib.py
+-rw-rw-rw-   0        0        0    16508 2022-06-19 15:56:37.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/primo_cal.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/short_link/
+-rw-rw-rw-   0        0        0      150 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/short_link/__init__.py
+-rw-rw-rw-   0        0        0     5069 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/short_link/rebrandly.py
+-rw-rw-rw-   0        0        0     2775 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/extensions/dev/tarot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/extensions/extra/
+-rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-2.1.1/src/absfuyu/extensions/extra/__init__.py
+-rw-rw-rw-   0        0        0     6812 2023-05-24 23:10:03.000000 absfuyu-2.1.1/src/absfuyu/extensions/extra/data_analysis.py
+-rw-rw-rw-   0        0        0     6001 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/fun.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/game/
+-rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-2.1.1/src/absfuyu/game/__init__.py
+-rw-rw-rw-   0        0        0     8258 2023-05-24 23:10:03.000000 absfuyu-2.1.1/src/absfuyu/game/sudoku.py
+-rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-2.1.1/src/absfuyu/game/tictactoe.py
+-rw-rw-rw-   0        0        0   101067 2023-05-24 23:10:03.000000 absfuyu-2.1.1/src/absfuyu/game/wordle.py
+-rw-rw-rw-   0        0        0     3752 2023-06-09 09:17:28.000000 absfuyu-2.1.1/src/absfuyu/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/
+-rw-rw-rw-   0        0        0     3043 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/__init__.py
+-rw-rw-rw-   0        0        0   247094 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/chemistry.json
+-rw-rw-rw-   0        0        0        0 2022-01-29 17:00:32.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/dummy.dat
+-rw-rw-rw-   0        0        0       31 2022-02-03 13:01:43.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/punishment_windows.dat
+-rw-rw-rw-   0        0        0    86614 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/pkg_data/tarot.json
+-rw-rw-rw-   0        0        0     5882 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/sort.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/tools/
+-rw-rw-rw-   0        0        0      136 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/__init__.py
+-rw-rw-rw-   0        0        0     5853 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/converter.py
+-rw-rw-rw-   0        0        0     7292 2023-06-09 14:49:10.000000 absfuyu-2.1.1/src/absfuyu/tools/keygen.py
+-rw-rw-rw-   0        0        0     8482 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/obfuscator.py
+-rw-rw-rw-   0        0        0     3008 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/stats.py
+-rw-rw-rw-   0        0        0     1180 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/tools/web.py
+-rw-rw-rw-   0        0        0    12499 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/unused.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu/util/
+-rw-rw-rw-   0        0        0     2396 2023-06-09 13:47:13.000000 absfuyu-2.1.1/src/absfuyu/util/__init__.py
+-rw-rw-rw-   0        0        0     2769 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/util/api.py
+-rw-rw-rw-   0        0        0     2366 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/util/json_method.py
+-rw-rw-rw-   0        0        0     5512 2023-06-15 08:10:16.000000 absfuyu-2.1.1/src/absfuyu/util/path.py
+-rw-rw-rw-   0        0        0     3829 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/util/performance.py
+-rw-rw-rw-   0        0        0     1230 2023-06-09 13:48:37.000000 absfuyu-2.1.1/src/absfuyu/util/pkl.py
+-rw-rw-rw-   0        0        0     2499 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/util/zipped.py
+-rw-rw-rw-   0        0        0     8504 2022-02-19 16:37:01.000000 absfuyu-2.1.1/src/absfuyu/version.py
+-rw-rw-rw-   0        0        0     9951 2023-06-05 17:50:56.000000 absfuyu-2.1.1/src/absfuyu/version2.py
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/src/absfuyu.egg-info/
+-rw-rw-rw-   0        0        0     3836 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2639 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1266 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 08:11:26.000000 absfuyu-2.1.1/src/absfuyu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 08:11:27.000000 absfuyu-2.1.1/tests/
+-rw-rw-rw-   0        0        0      805 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_DictKai.py
+-rw-rw-rw-   0        0        0     3049 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_Generator.py
+-rw-rw-rw-   0        0        0     3206 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_IntNumber.py
+-rw-rw-rw-   0        0        0     2068 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_ListKai.py
+-rw-rw-rw-   0        0        0     3246 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_Text.py
+-rw-rw-rw-   0        0        0      632 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_api.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 13:22:03.000000 absfuyu-2.1.1/tests/test_beautiful.py
+-rw-rw-rw-   0        0        0      691 2022-02-18 12:50:08.000000 absfuyu-2.1.1/tests/test_config.py
+-rw-rw-rw-   0        0        0      769 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_converter.py
+-rw-rw-rw-   0        0        0      108 2022-02-18 13:23:43.000000 absfuyu-2.1.1/tests/test_everything.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 12:31:52.000000 absfuyu-2.1.1/tests/test_extensions.py
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:50:45.000000 absfuyu-2.1.1/tests/test_fun.py
+-rw-rw-rw-   0        0        0      425 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_json_method.py
+-rw-rw-rw-   0        0        0      706 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_obfuscator.py
+-rw-rw-rw-   0        0        0      649 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_path.py
+-rw-rw-rw-   0        0        0      119 2023-05-25 10:14:50.000000 absfuyu-2.1.1/tests/test_pkg_data.py
+-rw-rw-rw-   0        0        0     1133 2023-06-05 17:50:56.000000 absfuyu-2.1.1/tests/test_util.py
```

### Comparing `absfuyu-2.1.0/LICENSE` & `absfuyu-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/PKG-INFO` & `absfuyu-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 2.1.0
+Version: 2.1.1
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -21,16 +21,16 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: beautiful
 Provides-Extra: rich
-Provides-Extra: cli
 Provides-Extra: click
+Provides-Extra: cli
 Provides-Extra: extra
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
 Provides-Extra: setuptools
 Provides-Extra: wheel
@@ -38,16 +38,16 @@
 Provides-Extra: tools
 Provides-Extra: requests
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
-Provides-Extra: fixers
 Provides-Extra: autoimport
+Provides-Extra: fixers
 Provides-Extra: black
 Provides-Extra: pytest
 Provides-Extra: test
 Provides-Extra: tox
 Provides-Extra: sphinx
 Provides-Extra: sphinx_rtd_theme
 Provides-Extra: python-dateutil
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: absfuyu Version: 2.1.0 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.1.1 Summary: A small collection
 of code Home-page: https://github.com/AbsoluteWinter/absfuyu Author:
 somewhatcold (AbsoluteWinter) Author-email:
 this.is.a.fake.mail@fakemail.absfuyu.com License: MIT Project-URL:
 Documentation, https://absolutewinter.github.io/absfuyu Project-URL: Source
 Code, https://github.com/AbsoluteWinter/absfuyu Project-URL: Bug Tracker,
 https://github.com/AbsoluteWinter/absfuyu/issues Keywords: utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Development Status :: 5 - Production/
 Stable Classifier: Natural Language :: English Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
-beautiful Provides-Extra: rich Provides-Extra: cli Provides-Extra: click
+beautiful Provides-Extra: rich Provides-Extra: click Provides-Extra: cli
 Provides-Extra: extra Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
 Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
 requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
 matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
+autoimport Provides-Extra: fixers Provides-Extra: black Provides-Extra: pytest
 Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
 sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
 Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
```

### Comparing `absfuyu-2.1.0/README.md` & `absfuyu-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/extra_requirements.txt` & `absfuyu-2.1.1/extra_requirements.txt`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/images/repository-image-crop.png` & `absfuyu-2.1.1/images/repository-image-crop.png`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/setup.cfg` & `absfuyu-2.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/setup.py` & `absfuyu-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/__init__.py` & `absfuyu-2.1.1/src/absfuyu/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/__main__.py` & `absfuyu-2.1.1/src/absfuyu/__main__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/calculation.py` & `absfuyu-2.1.1/src/absfuyu/calculation.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/code_red/__init__.py` & `absfuyu-2.1.1/src/absfuyu/code_red/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/collections/__init__.py` & `absfuyu-2.1.1/src/absfuyu/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/collections/content.py` & `absfuyu-2.1.1/src/absfuyu/collections/content.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/collections/data_extension.py` & `absfuyu-2.1.1/src/absfuyu/collections/data_extension.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/collections/generator.py` & `absfuyu-2.1.1/src/absfuyu/collections/generator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/collections/human.py` & `absfuyu-2.1.1/src/absfuyu/collections/human.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/config/__init__.py` & `absfuyu-2.1.1/src/absfuyu/config/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/config/config.json` & `absfuyu-2.1.1/src/absfuyu/config/template.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "{'major': 1, 'patch': 4}"}*

```diff
@@ -18,14 +18,14 @@
         "test": {
             "default": false,
             "help": "Test",
             "value": false
         }
     },
     "version": {
-        "major": 2,
+        "major": 1,
         "minor": 1,
-        "patch": 0,
+        "patch": 4,
         "release_level": "final",
         "serial": 0
     }
 }
```

### Comparing `absfuyu-2.1.0/src/absfuyu/config/config2.py` & `absfuyu-2.1.1/src/absfuyu/config/config2.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/config/template.json` & `absfuyu-2.1.1/src/absfuyu/config/config.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "{'major': 2, 'patch': 1}"}*

```diff
@@ -18,14 +18,14 @@
         "test": {
             "default": false,
             "help": "Test",
             "value": false
         }
     },
     "version": {
-        "major": 1,
+        "major": 2,
         "minor": 1,
-        "patch": 4,
+        "patch": 1,
         "release_level": "final",
         "serial": 0
     }
 }
```

### Comparing `absfuyu-2.1.0/src/absfuyu/contrib/basic_lunar_calendar.py` & `absfuyu-2.1.1/src/absfuyu/contrib/basic_lunar_calendar.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/contrib/color_extract.py` & `absfuyu-2.1.1/src/absfuyu/contrib/color_extract.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/core.py` & `absfuyu-2.1.1/src/absfuyu/core.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/everything.py` & `absfuyu-2.1.1/src/absfuyu/everything.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/beautiful.py` & `absfuyu-2.1.1/src/absfuyu/extensions/beautiful.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/dev/WGS.py` & `absfuyu-2.1.1/src/absfuyu/extensions/dev/WGS.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/dev/__init__.py` & `absfuyu-2.1.1/src/absfuyu/extensions/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/dev/horoscope.py` & `absfuyu-2.1.1/src/absfuyu/extensions/dev/horoscope.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/dev/password_hash.py` & `absfuyu-2.1.1/src/absfuyu/extensions/dev/password_hash.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/dev/pkglib.py` & `absfuyu-2.1.1/src/absfuyu/extensions/dev/pkglib.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/dev/primo_cal.py` & `absfuyu-2.1.1/src/absfuyu/extensions/dev/primo_cal.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/dev/short_link/rebrandly.py` & `absfuyu-2.1.1/src/absfuyu/extensions/dev/short_link/rebrandly.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/dev/tarot.py` & `absfuyu-2.1.1/src/absfuyu/extensions/dev/tarot.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/extra/__init__.py` & `absfuyu-2.1.1/src/absfuyu/extensions/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/extensions/extra/data_analysis.py` & `absfuyu-2.1.1/src/absfuyu/extensions/extra/data_analysis.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/fun.py` & `absfuyu-2.1.1/src/absfuyu/fun.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/game/__init__.py` & `absfuyu-2.1.1/src/absfuyu/game/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/game/sudoku.py` & `absfuyu-2.1.1/src/absfuyu/game/sudoku.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/game/tictactoe.py` & `absfuyu-2.1.1/src/absfuyu/game/tictactoe.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/game/wordle.py` & `absfuyu-2.1.1/src/absfuyu/game/wordle.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/logger.py` & `absfuyu-2.1.1/src/absfuyu/logger.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/pkg_data/__init__.py` & `absfuyu-2.1.1/src/absfuyu/pkg_data/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/pkg_data/chemistry.json` & `absfuyu-2.1.1/src/absfuyu/pkg_data/chemistry.json`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/pkg_data/tarot.json` & `absfuyu-2.1.1/src/absfuyu/pkg_data/tarot.json`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/sort.py` & `absfuyu-2.1.1/src/absfuyu/sort.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/tools/converter.py` & `absfuyu-2.1.1/src/absfuyu/tools/converter.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/tools/keygen.py` & `absfuyu-2.1.1/src/absfuyu/tools/keygen.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/tools/obfuscator.py` & `absfuyu-2.1.1/src/absfuyu/tools/obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/tools/stats.py` & `absfuyu-2.1.1/src/absfuyu/tools/stats.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/tools/web.py` & `absfuyu-2.1.1/src/absfuyu/tools/web.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/unused.py` & `absfuyu-2.1.1/src/absfuyu/unused.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/util/__init__.py` & `absfuyu-2.1.1/src/absfuyu/util/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/util/api.py` & `absfuyu-2.1.1/src/absfuyu/util/api.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/util/json_method.py` & `absfuyu-2.1.1/src/absfuyu/util/json_method.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/util/path.py` & `absfuyu-2.1.1/src/absfuyu/util/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Absfuyu: Path
 ---
 Path related
 
-Version: 1.1.0
-Date updated: 27/05/2023 (dd/mm/yyyy)
+Version: 1.1.1
+Date updated: 15/06/2023 (dd/mm/yyyy)
 
 Feature:
 - DirStructure
 """
 
 
 # Module level
@@ -21,15 +21,15 @@
 
 
 # Library
 ###########################################################################
 import os
 from pathlib import Path
 import re
-from typing import Union
+from typing import List, Union
 
 from absfuyu.logger import logger
 
 
 # Function
 ###########################################################################
 def here_location():
@@ -134,35 +134,27 @@
 
         temp = self.source_path.glob("**/*")
         # No ignore rules
         if len(ignore) == 0:
             return (x.relative_to(self.source_path) for x in temp)
 
         # With ignore rules
-        out = []
         ignore_pattern = "|".join(ignore)
         logger.debug(f"Ignore pattern: {ignore_pattern}")
-        for x in temp:
-            if re.search(ignore_pattern, x.name) is None:
-                out.append(x.relative_to(self.source_path))
-        return out
+        return [x.relative_to(self.source_path) for x in temp if re.search(ignore_pattern, x.name) is None]
 
-    def _separate_dir_and_files(self, list_of_path: list):
+    def _separate_dir_and_files(self, list_of_path: List[Path]) -> List[str]:
         """Separate dir and file and transform into folder structure"""
-        temp = sorted([str(x).split("\\") for x in list_of_path])
+        temp = sorted([str(x).split("/") for x in list_of_path]) # Linux
+        if max(map(len, temp)) == 1:
+            temp = sorted([str(x).split("\\") for x in list_of_path]) # Windows
 
-        output = []
-        for x in temp:
-            if len(x) > 1:
-                output.append(f"{self.tab_symbol*(len(x)-1)}{self.sub_dir_symbol}{x[-1]}")
-            else:
-                output.append(f"{self.sub_dir_symbol}{x[0]}")
-        return output
+        return [f"{self.tab_symbol*(len(x)-1)}{self.sub_dir_symbol}{x[-1]}" for x in temp]
 
-    def list_structure(self, *ignore: str):
+    def list_structure(self, *ignore: str) -> str:
         """
         List folder structure
 
         Example
         ---
         For typical python library
         ```
```

### Comparing `absfuyu-2.1.0/src/absfuyu/util/performance.py` & `absfuyu-2.1.1/src/absfuyu/util/performance.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/util/pkl.py` & `absfuyu-2.1.1/src/absfuyu/util/pkl.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/util/zipped.py` & `absfuyu-2.1.1/src/absfuyu/util/zipped.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/version.py` & `absfuyu-2.1.1/src/absfuyu/version.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu/version2.py` & `absfuyu-2.1.1/src/absfuyu/version2.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu.egg-info/PKG-INFO` & `absfuyu-2.1.1/src/absfuyu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 2.1.0
+Version: 2.1.1
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -21,16 +21,16 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: beautiful
 Provides-Extra: rich
-Provides-Extra: cli
 Provides-Extra: click
+Provides-Extra: cli
 Provides-Extra: extra
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
 Provides-Extra: setuptools
 Provides-Extra: wheel
@@ -38,16 +38,16 @@
 Provides-Extra: tools
 Provides-Extra: requests
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
-Provides-Extra: fixers
 Provides-Extra: autoimport
+Provides-Extra: fixers
 Provides-Extra: black
 Provides-Extra: pytest
 Provides-Extra: test
 Provides-Extra: tox
 Provides-Extra: sphinx
 Provides-Extra: sphinx_rtd_theme
 Provides-Extra: python-dateutil
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: absfuyu Version: 2.1.0 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.1.1 Summary: A small collection
 of code Home-page: https://github.com/AbsoluteWinter/absfuyu Author:
 somewhatcold (AbsoluteWinter) Author-email:
 this.is.a.fake.mail@fakemail.absfuyu.com License: MIT Project-URL:
 Documentation, https://absolutewinter.github.io/absfuyu Project-URL: Source
 Code, https://github.com/AbsoluteWinter/absfuyu Project-URL: Bug Tracker,
 https://github.com/AbsoluteWinter/absfuyu/issues Keywords: utilities
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3 ::
 Only Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Development Status :: 5 - Production/
 Stable Classifier: Natural Language :: English Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
-beautiful Provides-Extra: rich Provides-Extra: cli Provides-Extra: click
+beautiful Provides-Extra: rich Provides-Extra: click Provides-Extra: cli
 Provides-Extra: extra Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
 Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
 requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
 matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
+autoimport Provides-Extra: fixers Provides-Extra: black Provides-Extra: pytest
 Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
 sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
 Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
```

### Comparing `absfuyu-2.1.0/src/absfuyu.egg-info/SOURCES.txt` & `absfuyu-2.1.1/src/absfuyu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/src/absfuyu.egg-info/requires.txt` & `absfuyu-2.1.1/src/absfuyu.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -2,90 +2,90 @@
 [:python_version == "3.7"]
 typing_extensions>=3.7.4
 
 [LunarCalendar]
 LunarCalendar>=0.0.9
 
 [all]
-colorama>=0.4
-unidecode
-wheel
-tox>=3.24.5
-pipx
-pandas
 autoimport
-numpy
-build
-python-dateutil
-setuptools>=51.0.0
+matplotlib
+sphinx_rtd_theme
 virtualenv>=20.13.0
-scipy
+pipx
+pytest>=6.2.5
 LunarCalendar>=0.0.9
-requests
-rich
-matplotlib
-twine>=3.7.1
+tox>=3.24.5
+sphinx
+scipy
+python-dateutil
 click>=8.0.0
-pytest>=6.2.5
-sphinx_rtd_theme
+numpy
+unidecode
+setuptools>=51.0.0
+rich
+wheel
+colorama>=0.4
 black>=22.1.0
-sphinx
+pandas
+requests
+twine>=3.7.1
+build
 
 [autoimport]
 autoimport
 
 [beautiful]
 rich
 
 [black]
 black>=22.1.0
 
 [build]
 build
 
 [cli]
-colorama>=0.4
 click>=8.0.0
+colorama>=0.4
 
 [click]
 click>=8.0.0
 
 [colorama]
 colorama>=0.4
 
 [dev]
 virtualenv>=20.13.0
-pipx
-twine>=3.7.1
-colorama>=0.4
-unidecode
-click>=8.0.0
 rich
-pytest>=6.2.5
+sphinx_rtd_theme
 sphinx
+wheel
+click>=8.0.0
+colorama>=0.4
+pipx
+pytest>=6.2.5
+unidecode
+twine>=3.7.1
 build
-sphinx_rtd_theme
 setuptools>=51.0.0
-wheel
 
 [extra]
+matplotlib
 scipy
-pandas
+python-dateutil
+click>=8.0.0
 colorama>=0.4
 LunarCalendar>=0.0.9
-click>=8.0.0
-requests
 numpy
+pandas
+requests
 unidecode
-python-dateutil
-matplotlib
 
 [fixers]
-black>=22.1.0
 autoimport
+black>=22.1.0
 
 [matplotlib]
 matplotlib
 
 [numpy]
 numpy
 
@@ -116,16 +116,16 @@
 [sphinx]
 sphinx
 
 [sphinx_rtd_theme]
 sphinx_rtd_theme
 
 [test]
-tox>=3.24.5
 pytest>=6.2.5
+tox>=3.24.5
 
 [tools]
 requests
 
 [tox]
 tox>=3.24.5
```

### Comparing `absfuyu-2.1.0/tests/test_DictKai.py` & `absfuyu-2.1.1/tests/test_DictKai.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_Generator.py` & `absfuyu-2.1.1/tests/test_Generator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_IntNumber.py` & `absfuyu-2.1.1/tests/test_IntNumber.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_ListKai.py` & `absfuyu-2.1.1/tests/test_ListKai.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_Text.py` & `absfuyu-2.1.1/tests/test_Text.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_api.py` & `absfuyu-2.1.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_config.py` & `absfuyu-2.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_converter.py` & `absfuyu-2.1.1/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_obfuscator.py` & `absfuyu-2.1.1/tests/test_obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_path.py` & `absfuyu-2.1.1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.1.0/tests/test_util.py` & `absfuyu-2.1.1/tests/test_util.py`

 * *Files identical despite different names*

