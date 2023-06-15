# Comparing `tmp/absfuyu-2.0.0.tar.gz` & `tmp/absfuyu-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\.tmp-011s6zg4\absfuyu-2.0.0.tar", last modified: Mon Jun  5 17:18:25 2023, max compression
+gzip compressed data, was "C:\Users\NamSo\Documents\GitHub\absfuyu\dist\.tmp-4gqxm6y2\absfuyu-2.1.0.tar", last modified: Thu Jun 15 07:31:15 2023, max compression
```

## Comparing `absfuyu-2.0.0.tar` & `absfuyu-2.1.0.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/
--rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-2.0.0/LICENSE
--rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3836 2023-06-05 17:18:25.000000 absfuyu-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-2.0.0/README.md
--rw-rw-rw-   0        0        0     1161 2023-05-24 23:25:15.000000 absfuyu-2.0.0/extra_requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:24.000000 absfuyu-2.0.0/images/
--rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-2.0.0/images/repository-image-crop.png
--rw-rw-rw-   0        0        0      193 2023-06-05 17:18:06.000000 absfuyu-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-2.0.0/requirements.txt
--rw-rw-rw-   0        0        0     1360 2023-06-05 17:18:25.000000 absfuyu-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1009 2022-06-19 18:29:54.000000 absfuyu-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/
--rw-rw-rw-   0        0        0     1004 2023-06-05 10:10:40.000000 absfuyu-2.0.0/src/absfuyu/__init__.py
--rw-rw-rw-   0        0        0     6530 2023-06-05 10:08:56.000000 absfuyu-2.0.0/src/absfuyu/__main__.py
--rw-rw-rw-   0        0        0     2566 2023-06-04 16:54:26.000000 absfuyu-2.0.0/src/absfuyu/calculation.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/code_red/
--rw-rw-rw-   0        0        0     5580 2022-02-17 09:30:21.000000 absfuyu-2.0.0/src/absfuyu/code_red/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/collections/
--rw-rw-rw-   0        0        0     1264 2023-05-25 00:03:43.000000 absfuyu-2.0.0/src/absfuyu/collections/__init__.py
--rw-rw-rw-   0        0        0    14620 2023-05-24 23:35:16.000000 absfuyu-2.0.0/src/absfuyu/collections/content.py
--rw-rw-rw-   0        0        0    20344 2023-06-05 09:59:00.000000 absfuyu-2.0.0/src/absfuyu/collections/data_extension.py
--rw-rw-rw-   0        0        0     6742 2023-06-05 14:26:41.000000 absfuyu-2.0.0/src/absfuyu/collections/generator.py
--rw-rw-rw-   0        0        0     5822 2023-05-24 23:57:55.000000 absfuyu-2.0.0/src/absfuyu/collections/human.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/config/
--rw-rw-rw-   0        0        0     4234 2023-05-24 23:10:03.000000 absfuyu-2.0.0/src/absfuyu/config/__init__.py
--rw-rw-rw-   0        0        0      791 2023-06-05 17:18:13.000000 absfuyu-2.0.0/src/absfuyu/config/config.json
--rw-rw-rw-   0        0        0     1555 2023-05-24 23:30:58.000000 absfuyu-2.0.0/src/absfuyu/config/config2.py
--rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-2.0.0/src/absfuyu/config/template.json
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/contrib/
--rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-2.0.0/src/absfuyu/contrib/__init__.py
--rw-rw-rw-   0        0        0     8190 2023-05-25 00:27:41.000000 absfuyu-2.0.0/src/absfuyu/contrib/basic_lunar_calendar.py
--rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-2.0.0/src/absfuyu/contrib/color_extract.py
--rw-rw-rw-   0        0        0     3313 2023-06-05 09:42:30.000000 absfuyu-2.0.0/src/absfuyu/core.py
--rw-rw-rw-   0        0        0      832 2023-06-05 10:09:19.000000 absfuyu-2.0.0/src/absfuyu/everything.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/extensions/
--rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-2.0.0/src/absfuyu/extensions/__init__.py
--rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-2.0.0/src/absfuyu/extensions/beautiful.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/
--rw-rw-rw-   0        0        0    11971 2023-06-05 17:02:34.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/WGS.py
--rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/__init__.py
--rw-rw-rw-   0        0        0    11987 2022-06-19 18:02:35.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/horoscope.py
--rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/password_hash.py
--rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/pkglib.py
--rw-rw-rw-   0        0        0    16508 2022-06-19 15:56:37.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/primo_cal.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/short_link/
--rw-rw-rw-   0        0        0      150 2022-03-07 17:01:51.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/short_link/__init__.py
--rw-rw-rw-   0        0        0     5069 2022-03-07 17:01:43.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/short_link/rebrandly.py
--rw-rw-rw-   0        0        0     2775 2023-06-04 19:15:00.000000 absfuyu-2.0.0/src/absfuyu/extensions/dev/tarot.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/extensions/extra/
--rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-2.0.0/src/absfuyu/extensions/extra/__init__.py
--rw-rw-rw-   0        0        0     6812 2023-05-24 23:10:03.000000 absfuyu-2.0.0/src/absfuyu/extensions/extra/data_analysis.py
--rw-rw-rw-   0        0        0     6001 2023-06-04 17:07:41.000000 absfuyu-2.0.0/src/absfuyu/fun.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/game/
--rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-2.0.0/src/absfuyu/game/__init__.py
--rw-rw-rw-   0        0        0     8258 2023-05-24 23:10:03.000000 absfuyu-2.0.0/src/absfuyu/game/sudoku.py
--rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-2.0.0/src/absfuyu/game/tictactoe.py
--rw-rw-rw-   0        0        0   101067 2023-05-24 23:10:03.000000 absfuyu-2.0.0/src/absfuyu/game/wordle.py
--rw-rw-rw-   0        0        0     3612 2023-05-25 00:07:58.000000 absfuyu-2.0.0/src/absfuyu/logger.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/
--rw-rw-rw-   0        0        0     3043 2023-06-04 18:25:52.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/__init__.py
--rw-rw-rw-   0        0        0   247094 2023-05-27 07:47:21.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/chemistry.json
--rw-rw-rw-   0        0        0        0 2022-01-29 17:00:32.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/dummy.dat
--rw-rw-rw-   0        0        0       31 2022-02-03 13:01:43.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/punishment_windows.dat
--rw-rw-rw-   0        0        0    86614 2023-06-04 18:47:18.000000 absfuyu-2.0.0/src/absfuyu/pkg_data/tarot.json
--rw-rw-rw-   0        0        0     5882 2023-05-27 10:46:34.000000 absfuyu-2.0.0/src/absfuyu/sort.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/tools/
--rw-rw-rw-   0        0        0      136 2023-05-26 15:55:24.000000 absfuyu-2.0.0/src/absfuyu/tools/__init__.py
--rw-rw-rw-   0        0        0     5853 2023-06-05 17:07:39.000000 absfuyu-2.0.0/src/absfuyu/tools/converter.py
--rw-rw-rw-   0        0        0     9264 2023-02-16 09:21:06.000000 absfuyu-2.0.0/src/absfuyu/tools/keygen.py
--rw-rw-rw-   0        0        0     8482 2023-06-05 09:33:57.000000 absfuyu-2.0.0/src/absfuyu/tools/obfuscator.py
--rw-rw-rw-   0        0        0     3008 2023-06-05 10:41:12.000000 absfuyu-2.0.0/src/absfuyu/tools/stats.py
--rw-rw-rw-   0        0        0     1180 2023-05-27 10:43:07.000000 absfuyu-2.0.0/src/absfuyu/tools/web.py
--rw-rw-rw-   0        0        0    12499 2023-06-05 10:13:07.000000 absfuyu-2.0.0/src/absfuyu/unused.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu/util/
--rw-rw-rw-   0        0        0     2358 2023-06-05 15:57:31.000000 absfuyu-2.0.0/src/absfuyu/util/__init__.py
--rw-rw-rw-   0        0        0     2769 2023-05-27 10:21:24.000000 absfuyu-2.0.0/src/absfuyu/util/api.py
--rw-rw-rw-   0        0        0     2366 2023-05-27 10:30:03.000000 absfuyu-2.0.0/src/absfuyu/util/json_method.py
--rw-rw-rw-   0        0        0     5605 2023-05-27 10:34:09.000000 absfuyu-2.0.0/src/absfuyu/util/path.py
--rw-rw-rw-   0        0        0     3829 2023-05-27 10:38:41.000000 absfuyu-2.0.0/src/absfuyu/util/performance.py
--rw-rw-rw-   0        0        0     2499 2023-05-27 19:37:56.000000 absfuyu-2.0.0/src/absfuyu/util/zipped.py
--rw-rw-rw-   0        0        0     8504 2022-02-19 16:37:01.000000 absfuyu-2.0.0/src/absfuyu/version.py
--rw-rw-rw-   0        0        0     9951 2023-06-05 14:44:21.000000 absfuyu-2.0.0/src/absfuyu/version2.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/src/absfuyu.egg-info/
--rw-rw-rw-   0        0        0     3836 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2591 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1266 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-05 17:18:24.000000 absfuyu-2.0.0/src/absfuyu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 17:18:25.000000 absfuyu-2.0.0/tests/
--rw-rw-rw-   0        0        0      805 2023-05-25 06:54:29.000000 absfuyu-2.0.0/tests/test_DictKai.py
--rw-rw-rw-   0        0        0     2941 2023-05-26 16:32:44.000000 absfuyu-2.0.0/tests/test_Generator.py
--rw-rw-rw-   0        0        0     3206 2023-06-05 06:47:06.000000 absfuyu-2.0.0/tests/test_IntNumber.py
--rw-rw-rw-   0        0        0     2068 2023-05-25 04:14:43.000000 absfuyu-2.0.0/tests/test_ListKai.py
--rw-rw-rw-   0        0        0     3246 2023-06-05 09:58:53.000000 absfuyu-2.0.0/tests/test_Text.py
--rw-rw-rw-   0        0        0      632 2023-05-27 19:12:16.000000 absfuyu-2.0.0/tests/test_api.py
--rw-rw-rw-   0        0        0      111 2022-02-18 13:22:03.000000 absfuyu-2.0.0/tests/test_beautiful.py
--rw-rw-rw-   0        0        0      691 2022-02-18 12:50:08.000000 absfuyu-2.0.0/tests/test_config.py
--rw-rw-rw-   0        0        0      769 2023-05-27 10:06:18.000000 absfuyu-2.0.0/tests/test_converter.py
--rw-rw-rw-   0        0        0      108 2022-02-18 13:23:43.000000 absfuyu-2.0.0/tests/test_everything.py
--rw-rw-rw-   0        0        0      111 2022-02-18 12:31:52.000000 absfuyu-2.0.0/tests/test_extensions.py
--rw-rw-rw-   0        0        0      205 2022-06-19 18:50:45.000000 absfuyu-2.0.0/tests/test_fun.py
--rw-rw-rw-   0        0        0      425 2023-05-27 19:15:29.000000 absfuyu-2.0.0/tests/test_json_method.py
--rw-rw-rw-   0        0        0      706 2023-06-05 09:45:00.000000 absfuyu-2.0.0/tests/test_obfuscator.py
--rw-rw-rw-   0        0        0      649 2023-05-27 18:57:56.000000 absfuyu-2.0.0/tests/test_path.py
--rw-rw-rw-   0        0        0      119 2023-05-25 10:14:50.000000 absfuyu-2.0.0/tests/test_pkg_data.py
--rw-rw-rw-   0        0        0     1133 2023-06-05 15:55:36.000000 absfuyu-2.0.0/tests/test_util.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/
+-rw-rw-rw-   0        0        0     1071 2022-01-19 10:26:14.000000 absfuyu-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:27:30.000000 absfuyu-2.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3836 2023-06-15 07:31:15.000000 absfuyu-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1973 2022-02-16 17:39:44.000000 absfuyu-2.1.0/README.md
+-rw-rw-rw-   0        0        0     1161 2023-06-05 17:50:56.000000 absfuyu-2.1.0/extra_requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/images/
+-rw-rw-rw-   0        0        0    34015 2022-01-20 09:25:05.000000 absfuyu-2.1.0/images/repository-image-crop.png
+-rw-rw-rw-   0        0        0      193 2023-06-05 17:50:56.000000 absfuyu-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2022-02-16 18:36:40.000000 absfuyu-2.1.0/requirements.txt
+-rw-rw-rw-   0        0        0     1360 2023-06-15 07:31:15.000000 absfuyu-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1009 2022-06-19 18:29:54.000000 absfuyu-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/
+-rw-rw-rw-   0        0        0     1004 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/__init__.py
+-rw-rw-rw-   0        0        0     6530 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/__main__.py
+-rw-rw-rw-   0        0        0     2566 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/calculation.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/code_red/
+-rw-rw-rw-   0        0        0     5580 2022-02-17 09:30:21.000000 absfuyu-2.1.0/src/absfuyu/code_red/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/collections/
+-rw-rw-rw-   0        0        0     1938 2023-06-09 13:43:36.000000 absfuyu-2.1.0/src/absfuyu/collections/__init__.py
+-rw-rw-rw-   0        0        0    14620 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/collections/content.py
+-rw-rw-rw-   0        0        0    20864 2023-06-15 07:26:41.000000 absfuyu-2.1.0/src/absfuyu/collections/data_extension.py
+-rw-rw-rw-   0        0        0     6742 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/collections/generator.py
+-rw-rw-rw-   0        0        0     5822 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/collections/human.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/config/
+-rw-rw-rw-   0        0        0     4234 2023-05-24 23:10:03.000000 absfuyu-2.1.0/src/absfuyu/config/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-06-15 07:30:57.000000 absfuyu-2.1.0/src/absfuyu/config/config.json
+-rw-rw-rw-   0        0        0     1555 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/config/config2.py
+-rw-rw-rw-   0        0        0      791 2022-02-17 10:39:37.000000 absfuyu-2.1.0/src/absfuyu/config/template.json
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/contrib/
+-rw-rw-rw-   0        0        0       48 2022-03-06 07:36:09.000000 absfuyu-2.1.0/src/absfuyu/contrib/__init__.py
+-rw-rw-rw-   0        0        0     8190 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/contrib/basic_lunar_calendar.py
+-rw-rw-rw-   0        0        0     2492 2022-03-06 07:33:39.000000 absfuyu-2.1.0/src/absfuyu/contrib/color_extract.py
+-rw-rw-rw-   0        0        0     3313 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/core.py
+-rw-rw-rw-   0        0        0      832 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/everything.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/extensions/
+-rw-rw-rw-   0        0        0       74 2022-02-17 13:08:03.000000 absfuyu-2.1.0/src/absfuyu/extensions/__init__.py
+-rw-rw-rw-   0        0        0     4927 2022-03-06 07:55:00.000000 absfuyu-2.1.0/src/absfuyu/extensions/beautiful.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/
+-rw-rw-rw-   0        0        0    11971 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/WGS.py
+-rw-rw-rw-   0        0        0     2994 2022-03-01 11:04:11.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/__init__.py
+-rw-rw-rw-   0        0        0    11987 2022-06-19 18:02:35.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/horoscope.py
+-rw-rw-rw-   0        0        0     1799 2022-02-16 17:39:44.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/password_hash.py
+-rw-rw-rw-   0        0        0     2005 2022-03-07 17:29:22.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/pkglib.py
+-rw-rw-rw-   0        0        0    16508 2022-06-19 15:56:37.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/primo_cal.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/short_link/
+-rw-rw-rw-   0        0        0      150 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/short_link/__init__.py
+-rw-rw-rw-   0        0        0     5069 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/short_link/rebrandly.py
+-rw-rw-rw-   0        0        0     2775 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/extensions/dev/tarot.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/extensions/extra/
+-rw-rw-rw-   0        0        0     2249 2022-02-18 10:17:34.000000 absfuyu-2.1.0/src/absfuyu/extensions/extra/__init__.py
+-rw-rw-rw-   0        0        0     6812 2023-05-24 23:10:03.000000 absfuyu-2.1.0/src/absfuyu/extensions/extra/data_analysis.py
+-rw-rw-rw-   0        0        0     6001 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/fun.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/game/
+-rw-rw-rw-   0        0        0     4443 2022-03-06 07:39:46.000000 absfuyu-2.1.0/src/absfuyu/game/__init__.py
+-rw-rw-rw-   0        0        0     8258 2023-05-24 23:10:03.000000 absfuyu-2.1.0/src/absfuyu/game/sudoku.py
+-rw-rw-rw-   0        0        0    15826 2022-03-18 02:04:47.000000 absfuyu-2.1.0/src/absfuyu/game/tictactoe.py
+-rw-rw-rw-   0        0        0   101067 2023-05-24 23:10:03.000000 absfuyu-2.1.0/src/absfuyu/game/wordle.py
+-rw-rw-rw-   0        0        0     3752 2023-06-09 09:17:28.000000 absfuyu-2.1.0/src/absfuyu/logger.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/
+-rw-rw-rw-   0        0        0     3043 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/__init__.py
+-rw-rw-rw-   0        0        0   247094 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/chemistry.json
+-rw-rw-rw-   0        0        0        0 2022-01-29 17:00:32.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/dummy.dat
+-rw-rw-rw-   0        0        0       31 2022-02-03 13:01:43.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/punishment_windows.dat
+-rw-rw-rw-   0        0        0    86614 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/pkg_data/tarot.json
+-rw-rw-rw-   0        0        0     5882 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/sort.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/tools/
+-rw-rw-rw-   0        0        0      136 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/__init__.py
+-rw-rw-rw-   0        0        0     5853 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/converter.py
+-rw-rw-rw-   0        0        0     7292 2023-06-09 14:49:10.000000 absfuyu-2.1.0/src/absfuyu/tools/keygen.py
+-rw-rw-rw-   0        0        0     8482 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/obfuscator.py
+-rw-rw-rw-   0        0        0     3008 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/stats.py
+-rw-rw-rw-   0        0        0     1180 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/tools/web.py
+-rw-rw-rw-   0        0        0    12499 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/unused.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu/util/
+-rw-rw-rw-   0        0        0     2396 2023-06-09 13:47:13.000000 absfuyu-2.1.0/src/absfuyu/util/__init__.py
+-rw-rw-rw-   0        0        0     2769 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/api.py
+-rw-rw-rw-   0        0        0     2366 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/json_method.py
+-rw-rw-rw-   0        0        0     5605 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/path.py
+-rw-rw-rw-   0        0        0     3829 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/performance.py
+-rw-rw-rw-   0        0        0     1230 2023-06-09 13:48:37.000000 absfuyu-2.1.0/src/absfuyu/util/pkl.py
+-rw-rw-rw-   0        0        0     2499 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/util/zipped.py
+-rw-rw-rw-   0        0        0     8504 2022-02-19 16:37:01.000000 absfuyu-2.1.0/src/absfuyu/version.py
+-rw-rw-rw-   0        0        0     9951 2023-06-05 17:50:56.000000 absfuyu-2.1.0/src/absfuyu/version2.py
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/
+-rw-rw-rw-   0        0        0     3836 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2639 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1266 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 07:31:15.000000 absfuyu-2.1.0/src/absfuyu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 07:31:15.000000 absfuyu-2.1.0/tests/
+-rw-rw-rw-   0        0        0      805 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_DictKai.py
+-rw-rw-rw-   0        0        0     3049 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_Generator.py
+-rw-rw-rw-   0        0        0     3206 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_IntNumber.py
+-rw-rw-rw-   0        0        0     2068 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_ListKai.py
+-rw-rw-rw-   0        0        0     3246 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_Text.py
+-rw-rw-rw-   0        0        0      632 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_api.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 13:22:03.000000 absfuyu-2.1.0/tests/test_beautiful.py
+-rw-rw-rw-   0        0        0      691 2022-02-18 12:50:08.000000 absfuyu-2.1.0/tests/test_config.py
+-rw-rw-rw-   0        0        0      769 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_converter.py
+-rw-rw-rw-   0        0        0      108 2022-02-18 13:23:43.000000 absfuyu-2.1.0/tests/test_everything.py
+-rw-rw-rw-   0        0        0      111 2022-02-18 12:31:52.000000 absfuyu-2.1.0/tests/test_extensions.py
+-rw-rw-rw-   0        0        0      205 2022-06-19 18:50:45.000000 absfuyu-2.1.0/tests/test_fun.py
+-rw-rw-rw-   0        0        0      425 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_json_method.py
+-rw-rw-rw-   0        0        0      706 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_obfuscator.py
+-rw-rw-rw-   0        0        0      649 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_path.py
+-rw-rw-rw-   0        0        0      119 2023-05-25 10:14:50.000000 absfuyu-2.1.0/tests/test_pkg_data.py
+-rw-rw-rw-   0        0        0     1133 2023-06-05 17:50:56.000000 absfuyu-2.1.0/tests/test_util.py
```

### Comparing `absfuyu-2.0.0/LICENSE` & `absfuyu-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/PKG-INFO` & `absfuyu-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 2.0.0
+Version: 2.1.0
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -19,16 +19,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: rich
 Provides-Extra: beautiful
+Provides-Extra: rich
 Provides-Extra: cli
 Provides-Extra: click
 Provides-Extra: extra
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
@@ -38,16 +38,16 @@
 Provides-Extra: tools
 Provides-Extra: requests
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
-Provides-Extra: autoimport
 Provides-Extra: fixers
+Provides-Extra: autoimport
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
-Metadata-Version: 2.1 Name: absfuyu Version: 2.0.0 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.1.0 Summary: A small collection
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
-rich Provides-Extra: beautiful Provides-Extra: cli Provides-Extra: click
+beautiful Provides-Extra: rich Provides-Extra: cli Provides-Extra: click
 Provides-Extra: extra Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
 Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
 requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
 matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-autoimport Provides-Extra: fixers Provides-Extra: black Provides-Extra: pytest
+fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
 Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
 sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
 Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
```

### Comparing `absfuyu-2.0.0/README.md` & `absfuyu-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/extra_requirements.txt` & `absfuyu-2.1.0/extra_requirements.txt`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/images/repository-image-crop.png` & `absfuyu-2.1.0/images/repository-image-crop.png`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/setup.cfg` & `absfuyu-2.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/setup.py` & `absfuyu-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/__init__.py` & `absfuyu-2.1.0/src/absfuyu/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/__main__.py` & `absfuyu-2.1.0/src/absfuyu/__main__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/calculation.py` & `absfuyu-2.1.0/src/absfuyu/calculation.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/code_red/__init__.py` & `absfuyu-2.1.0/src/absfuyu/code_red/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/collections/content.py` & `absfuyu-2.1.0/src/absfuyu/collections/content.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/collections/data_extension.py` & `absfuyu-2.1.0/src/absfuyu/collections/data_extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Absfuyu: Data extension
 ---
 Extension for data type such as `list`, `str`, ...
 
-Version: 1.1.2
-Date updated: 05/06/2023 (dd/mm/yyyy)
+Version: 1.2.0
+Date updated: 15/06/2023 (dd/mm/yyyy)
 
 Features:
 - Text
 - ListKai
 - DictKai
 - IntNumber
 """
@@ -21,15 +21,15 @@
     "ListKai", "DictKai"
 ]
 
 
 # Library
 ###########################################################################
 from collections import Counter
-from itertools import accumulate
+from itertools import accumulate, groupby
 import math
 import operator
 import random
 from typing import Union
 
 from absfuyu.collections.generator import Generator, Charset
 from absfuyu.logger import logger, log_debug
@@ -506,16 +506,14 @@
         list
             A list with all items with type: string
         """
         return ListKai(map(str, self))
 
     def sorts(self, reverse: bool = False):
         """
-        Summary
-        -------
         Sort all items (with different type) in list
         
         Parameters
         ----------
         reverse : bool
             if True then sort in descending order
 
@@ -534,25 +532,23 @@
         output = sorted(
             lst,
             key=lambda x: (type_weights[type(x)], str(x)),
             reverse=reverse
         )
 
         logger.debug(output)
-        return output
+        return __class__(output)
     
     def freq(
             self,
             sort: bool = False,
             num_of_first_char: int = None,
             appear_increment: bool = False
         ):
         """
-        Summary
-        -------
         Find frequency of each item in list
 
         Parameters
         ----------
         sort : bool
             if True: sort the dict in ascending order
         
@@ -624,14 +620,15 @@
         else:
             logger.debug("List empty!")
             return None
     
     def len_items(self):
         """`len()` for every item in list"""
         out = ListKai([len(str(x)) for x in self])
+        # out = ListKai(map(lambda x: len(str(x)), self))
         logger.debug(out)
         return out
 
     def mean_len(self):
         """Average length of every item"""
         out = sum(self.len_items())/len(self)
         logger.debug(out)
@@ -641,14 +638,32 @@
         """Apply function to each entry"""
         # return __class__(func(x) for x in self)
         return __class__(map(func, self))
 
     def unique(self):
         """Remove duplicates"""
         return __class__(set(self))
+    
+    def group_by_unique(self):
+        """
+        Group duplicated elements into list
+        
+        Example:
+        ---
+        >>> test = ListKai([1, 2, 3, 1, 3, 3, 2])
+        >>> test.group_by_unique()
+        [[1, 1], [2, 2], [3, 3, 3]]
+        """
+        # Old
+        # out = self.sorts().slice_points(self.freq(appear_increment=True))
+        # return __class__(out[:-1])
+
+        # New
+        temp = groupby(self.sorts())
+        return __class__([list(g) for _, g in temp])
 
 
 class DictKai(dict):
     """
     `dict` extension
     """
     def analyze(self):
@@ -688,10 +703,9 @@
         """Swap keys with values"""
         return __class__(zip(self.values(), self.keys()))
 
 
 
 # Run
 ###########################################################################
-if __name__ == '__main__':
+if __name__ == "__main__":
     logger.setLevel(10)
-
```

### Comparing `absfuyu-2.0.0/src/absfuyu/collections/generator.py` & `absfuyu-2.1.0/src/absfuyu/collections/generator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/collections/human.py` & `absfuyu-2.1.0/src/absfuyu/collections/human.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/config/__init__.py` & `absfuyu-2.1.0/src/absfuyu/config/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/config/config.json` & `absfuyu-2.1.0/src/absfuyu/config/config.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "{'minor': 1}"}*

```diff
@@ -19,13 +19,13 @@
             "default": false,
             "help": "Test",
             "value": false
         }
     },
     "version": {
         "major": 2,
-        "minor": 0,
+        "minor": 1,
         "patch": 0,
         "release_level": "final",
         "serial": 0
     }
 }
```

### Comparing `absfuyu-2.0.0/src/absfuyu/config/config2.py` & `absfuyu-2.1.0/src/absfuyu/config/config2.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/config/template.json` & `absfuyu-2.1.0/src/absfuyu/config/template.json`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/contrib/basic_lunar_calendar.py` & `absfuyu-2.1.0/src/absfuyu/contrib/basic_lunar_calendar.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/contrib/color_extract.py` & `absfuyu-2.1.0/src/absfuyu/contrib/color_extract.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/core.py` & `absfuyu-2.1.0/src/absfuyu/core.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/everything.py` & `absfuyu-2.1.0/src/absfuyu/everything.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/beautiful.py` & `absfuyu-2.1.0/src/absfuyu/extensions/beautiful.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/dev/WGS.py` & `absfuyu-2.1.0/src/absfuyu/extensions/dev/WGS.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/dev/__init__.py` & `absfuyu-2.1.0/src/absfuyu/extensions/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/dev/horoscope.py` & `absfuyu-2.1.0/src/absfuyu/extensions/dev/horoscope.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/dev/password_hash.py` & `absfuyu-2.1.0/src/absfuyu/extensions/dev/password_hash.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/dev/pkglib.py` & `absfuyu-2.1.0/src/absfuyu/extensions/dev/pkglib.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/dev/primo_cal.py` & `absfuyu-2.1.0/src/absfuyu/extensions/dev/primo_cal.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/dev/short_link/rebrandly.py` & `absfuyu-2.1.0/src/absfuyu/extensions/dev/short_link/rebrandly.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/dev/tarot.py` & `absfuyu-2.1.0/src/absfuyu/extensions/dev/tarot.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/extra/__init__.py` & `absfuyu-2.1.0/src/absfuyu/extensions/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/extensions/extra/data_analysis.py` & `absfuyu-2.1.0/src/absfuyu/extensions/extra/data_analysis.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/fun.py` & `absfuyu-2.1.0/src/absfuyu/fun.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/game/__init__.py` & `absfuyu-2.1.0/src/absfuyu/game/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/game/sudoku.py` & `absfuyu-2.1.0/src/absfuyu/game/sudoku.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/game/tictactoe.py` & `absfuyu-2.1.0/src/absfuyu/game/tictactoe.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/game/wordle.py` & `absfuyu-2.1.0/src/absfuyu/game/wordle.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/logger.py` & `absfuyu-2.1.0/src/absfuyu/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,50 @@
 """
 Absfuyu: Logger
 ---
 Logger Module
 
-Version: 1.0.1
-Last update: 19/04/2023 (mm/dd/yyyy)
+Version: 1.1.0
+Last update: 09/06/2023 (mm/dd/yyyy)
 
 Usage:
-```
-from absfuyu.logger import logger, log_debug
-```
+>>> from absfuyu.logger import logger, log_debug, LogLevel
 """
 
 
 # Module level
 ###########################################################################
 __all__ = [
-    "logger", "log_debug"
+    "logger", "log_debug",
+    "LogLevel"
 ]
 
 
 # Library
 ###########################################################################
 from itertools import chain
 import logging
 import math
 
 
 # Setup
 ###########################################################################
 logger = logging.getLogger(__name__)
-# FORMAT = "[%(asctime)s] [%(process)-d] [%(module)s] [%(name)s] [%(funcName)s] [%(levelname)-s] %(message)s"
-FORMAT = "[%(module)s] [%(name)s] [%(funcName)s] [%(levelname)-s] %(message)s"
-handler = logging.StreamHandler()
-handler.setLevel(logging.DEBUG)
-handler.setFormatter(logging.Formatter(FORMAT, "%Y-%m-%d %H:%M:%S"))
-logger.addHandler(handler)
+class _LogFormat:
+    FULL = "[%(asctime)s] [%(process)-d] [%(module)s] [%(name)s] [%(funcName)s] [%(levelname)-s] %(message)s"
+    SHORT = "[%(module)s] [%(name)s] [%(funcName)s] [%(levelname)-s] %(message)s"
+_handler = logging.StreamHandler()
+_handler.setLevel(logging.DEBUG)
+_handler.setFormatter(logging.Formatter(_LogFormat.SHORT, "%Y-%m-%d %H:%M:%S"))
+logger.addHandler(_handler)
 logger.setLevel(logging.WARNING)
 
 
 # Functions
 ###########################################################################
-def __log_level():
-    """Show log level in int value"""
-    log_dict = {
-        "DEBUG": logging.DEBUG,
-        "INFO": logging.INFO,
-        "WARNING": logging.WARNING,
-        "ERROR": logging.ERROR,
-        "CRITICAL": logging.CRITICAL,
-    }
-    return log_dict
-
-
 def _compress_list_for_print(iterable: list, max_visible: int = 3) -> str:
     """
     Compress the list to be more log-readable
     
     iterable : list
     max_visible : int
         maximum items can be printed on screen
@@ -114,11 +102,23 @@
         logger.debug(_compress_list_for_print(temp, max_visible))
     elif isinstance(object_, str):
         logger.debug(_compress_string_for_print(object_, max_visible))
     else:
         logger.debug(object_)
 
 
+# Functions
+###########################################################################
+class LogLevel:
+    """`logging`'s log level wrapper"""
+    __TRACE: int = logging.DEBUG - 5 # Soon
+    DEBUG: int = logging.DEBUG
+    INFO: int = logging.INFO
+    WARNING: int = logging.WARNING
+    ERROR: int = logging.ERROR
+    CRITICAL: int = logging.CRITICAL
+
+
 # Run
 ###########################################################################
 if __name__ == "__main__":
     logger.setLevel(logging.DEBUG)
```

### Comparing `absfuyu-2.0.0/src/absfuyu/pkg_data/__init__.py` & `absfuyu-2.1.0/src/absfuyu/pkg_data/__init__.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/pkg_data/chemistry.json` & `absfuyu-2.1.0/src/absfuyu/pkg_data/chemistry.json`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/pkg_data/tarot.json` & `absfuyu-2.1.0/src/absfuyu/pkg_data/tarot.json`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/sort.py` & `absfuyu-2.1.0/src/absfuyu/sort.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/tools/converter.py` & `absfuyu-2.1.0/src/absfuyu/tools/converter.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/tools/keygen.py` & `absfuyu-2.1.0/src/absfuyu/tools/keygen.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,331 +1,257 @@
 # -*- coding: utf-8 -*-
 """
+Absfuyu: Keygen
+---
 Mod7 product key generator (90's)
 
 This is for educational and informative purposes only.
-"""
 
-# Library
-##############################################################
-import random as __random
+Version: 2.0.0
+Date updated: 09/06/2023 (dd/mm/yyyy)
+"""
 
-from absfuyu import core as __core
 
+# Module level
+###########################################################################
+__all__ = [
+    "Keygen"
+]
 
 
-# Function
-##############################################################
-def __add_char_to_fixed_str_length(
-        text: str,
-        desired_length: int,
-        filled_text: str = "0",
-        align: __core.AlignPosition = "left",
-    ) -> str:
-    """
-    This function add a specified character into a string with fixed length
-
-    For example:
-    - str = "2" 
-    - desired length = 3
-     -> new_str = "002"
-    
-    Parameters:
-    ---
-    text : str
-        Text
-    
-    desired_length : int
-        Length of new text
-    
-    filled_text : str
-        Fill the blank with `filled_text`
-    
-    align : AlignPosition
-        "left"
-        "right"
-        "center"
-    
-    Return:
-    ---
-    str:
-        Filled string
-    """
-    
-    # Check conditions
-    text = str(text) # Convert again to make sure
-    len_different = desired_length - len(text)
-    if len_different < 0: # Small length
-        raise ValueError("Desired length smaller than string length.")
-    if align not in ["left", "right"]: # Invalid option
-        align = "left" # Default value
-    
-    # Start
-    if align.startswith("left"):
-        return f"{filled_text*len_different}{text}"
-    elif align.startswith("right"):
-        return f"{text}{filled_text*len_different}"
-    else: # Center alignment
-        return f"{filled_text*int(len_different/2)}{text}{filled_text*int(len_different/2)}"
-
-def __is_mod7(text: str) -> bool:
-    """Check if sum of elements in a string is divisible by 7"""
-    text = str(text) # Safety convert
-    try:
-        return sum([int(x) for x in text]) % 7 == 0
-    except:
-        raise ValueError("Invalid string")
-
-def __mod7_gen(num_of_digits: int) -> str:
-    """
-    Generate a number with desired length that is divisible by 7
-
-    Parameters:
-    ---
-    num_of_digits : int
-        Length of number
-
-    Return:
-    ---
-    str:
-        Mod7 number
-    """
-    
-    # Init
-    mod7_num: int = 0
-    
-    # Conditions
-    max_value = 10**num_of_digits-1
-    mod7_valid = False
-    invalid_digits = [0,8,9] # Invalid last digit
-    
-    # Loop
-    while not mod7_valid:
-        # Gen num
-        mod7_num = __random.randint(0,max_value)
-        
-        # Check last digit
-        if int(str(mod7_num)[-1]) in invalid_digits:
-            continue
-        
-        # Check divide by 7
-        if __is_mod7(mod7_num):
-            mod7_valid = True
-    
-    # Output
-    return __add_char_to_fixed_str_length(
-        text=mod7_num,
-        desired_length=num_of_digits)
+# Library
+###########################################################################
+import random
 
 
-def mod7_cd_key(fast: bool = False) -> str:
-    r"""
-    CD Key generator
-
-    Format: XXX-XXXXXXX                               \
-    Rules:
-    - Last seven digits must add to be divisible by 7
-    - First 3 digits cannot be 333, 444,..., 999
-    - Last digit of last seven digits cannot be 0, 8 or 9
-    
-    Parameters:
-    ---
-    fast : bool
-        Use pre-generated key
-        [Default: False]
-    
-    Return:
-    ---
-    str:
-        Mod7 Key
-    """
-
-    # Fast mode: pre-generated key
-    if fast:
-        return "111-1111111"
-
-    # PART 01
-    part1_valid = False
-    part1_not_valid_digits = [333, 444, 555, 666, 777, 888]
-    part1: str = ""
-    while not part1_valid: # Loop check
-        part1_num = __random.randint(0,998) # Gen random int from 0 to 998
-        # part1_num = __random.randint(100,300) # or just use this
-        if part1_num not in part1_not_valid_digits:
-            part1 = __add_char_to_fixed_str_length(
-                text=str(part1_num), desired_length=3) # Convert into string
-            part1_valid = True # Break loop
-
-    # PART 02
-    part2 = __mod7_gen(num_of_digits=7)
-
-    # OUTPUT
-    return f"{part1}-{part2}"
-
-
-def mod7_11_digit_key(fast: bool = False) -> str:
-    """
-    11-digit CD Key generator
-
-    Format: XXXX-XXXXXXX
-    - XXXX: Can be anything from 0001 to 9991.
-    The last digit must be 3rd digit + 1 or 2.
-    When the result is > 9, it overflows to 0 or 1.
-    - XXXXXXX: Same as CD Key
-    
-    Parameters:
-    ---
-    fast : bool
-        Use pre-generated key
-        [Default: False]
-    
-    Return:
-    ---
-    str:
-        Mod7 Key
-    """
-    
-    # Fast mode: pre-generated key
-    if fast:
-        return "0001-0000007"
-    
-    # PART 01
-    part1_valid = False
-    part1: str = ""
-    while not part1_valid:
-        part1_1_num = __random.randint(0,999) # Random 3-digit number
-        last_digit_choice = [1, 2] # Choice for last digit
-        part1_2_num = int(str(part1_1_num)[-1]) + __random.choice(last_digit_choice) # Make last digit
-        if part1_2_num > 9: # Check condition then overflow
-            part1_2_num = int(str(part1_2_num)[-1])
-        part1_str = str(part1_1_num) + str(part1_2_num) # Concat string
-        if int(part1_str) > 9991: # Check if < 9991
-            continue
-        else:
-            part1 = __add_char_to_fixed_str_length(text=part1_str, desired_length=4)
-            part1_valid = True
+# Class
+###########################################################################
+class Keygen:
+    """Key generator"""
+    @staticmethod
+    def _is_mod7(text: str) -> bool:
+        """
+        Check if sum of elements in a string is divisible by 7
+
+        text: number in str type to check
+        """
+        text = str(text) # Safety convert
+        try:
+            res = sum(map(int, text)) % 7
+            # logger.debug(f"Sum value: {res}")
+            return res == 0
+        except:
+            raise ValueError("Invalid string")
+    
+    @staticmethod
+    def _mod7_gen(
+            num_of_digits: int,
+            *,
+            fillchar: str = "0"
+        ) -> str:
+        """
+        Generate a number with desired length that is divisible by 7
+
+        Parameters:
+        ---
+        num_of_digits : int
+            Length of number
 
-    # PART 02
-    part2 = __mod7_gen(num_of_digits=7)
-
-    # OUTPUT
-    return f"{part1}-{part2}"
-    
-
-def mod7_oem_key(fast: bool = False) -> str:
-    """
-    OEM Key generator
-
-    Format: ABCYY-OEM-0XXXXXX-XXXXX
-    - ABC: The day of the year. It can be any value from 001 to 366
-    - YY: The last two digits of the year. It can be anything from 95 to 03
-    - 0XXXXXX: A random number that has a sum that is divisible by 7 and does not end with 0, 8 or 3.
-    - XXXXX: A random 5-digit number
-
-    Parameters:
-    ---
-    fast : bool
-        Use pre-generated key
-        [Default: False]
-    
-    Return:
-    ---
-    str:
-        Mod7 Key
-    """
-    
-    # Fast mode: pre-generated key
-    if fast:
-        return "00100-OEM-0000007-00000"
-    
-    # PART ABC
-    abc_num = str(__random.randint(1,365))
-    # abc_num = str(__random.randint(1,366))
-    abc_part = __add_char_to_fixed_str_length(text=abc_num, desired_length=3)
-
-    # PART YY
-    year_choice = ["95", "96", "97", "98", "99", "00", "01", "02"]
-    # isleap = [False, True, False, False, False, True, False, False]
-    # year_choice = ["95", "96", "97", "98", "99", "00", "01", "02", "03"] # "03" not wotk on win95
-    y_part = __random.choice(year_choice)
-
-    # NUM PART
-    num_part = __mod7_gen(num_of_digits=6)
-
-    # NUM PART 02
-    num_2 = str(__random.randint(0,99999))
-    num_part_2 = __add_char_to_fixed_str_length(text=num_2, desired_length=5)
-
-    # OUTPUT
-    return f"{abc_part}{y_part}-OEM-0{num_part}-{num_part_2}"
-
-
-def mod7_combo(fast: bool = False):
-    """
-    A combo that consist of CD, 11-digit, and OEM Key
-
-    Parameters:
-    ---
-    fast : bool
-        Use pre-generated key
-        [Default: False]
-    
-    Return:
-    ---
-    dict:
-        Mod7 Key combo
-    """
-    out = {
-        "CD Key": mod7_cd_key(fast=fast),
-        "OEM Key": mod7_oem_key(fast=fast),
-        "11-digit Key": mod7_11_digit_key(fast=fast)
-    }
-    return out
-
-
-def __xp_gen(show_all: bool = False) -> str:
-    """
-    XP Gen
+        fillchar : str
+            filled character when `len(generated number)` < `num_of_digits`
+        
+        Return:
+        ---
+        str:
+            Mod7 number
+        """
+        
+        # Init
+        mod7_num: int = 0
+        
+        # Conditions
+        max_value = 10**num_of_digits-1
+        mod7_valid = False
+        invalid_digits = [0,8,9] # Invalid last digit
+        
+        # Loop
+        while not mod7_valid:
+            # Gen num
+            mod7_num = random.randint(0, max_value)
+            
+            # Check last digit
+            if int(str(mod7_num)[-1]) in invalid_digits:
+                continue
+            
+            # Check divide by 7
+            if __class__._is_mod7(mod7_num):
+                mod7_valid = True
+        
+        # Output
+        return str(mod7_num).rjust(num_of_digits, fillchar)
 
-    Unused
 
-    and
+    @staticmethod
+    def mod7_cd_key(fast: bool = False) -> str:
+        r"""
+        CD Key generator
+
+        Format: `XXX-XXXXXXX`                              \
+        Rules:
+        - Last seven digits must add to be divisible by `7`
+        - First 3 digits cannot be `333`, `444`,..., `999`
+        - Last digit of last seven digits cannot be `0`, `8` or `9`
+        
+        Parameters:
+        ---
+        fast : bool
+            Use pre-generated key
+            [Default: False]
+        
+        Return:
+        ---
+        str:
+            Mod7 Key
+        """
+
+        # Fast mode: pre-generated key
+        if fast:
+            return "111-1111111"
+
+        # PART 01
+        part1_valid = False
+        part1_not_valid_digits = [333, 444, 555, 666, 777, 888]
+        part1: str = ""
+        while not part1_valid: # Loop check
+            part1_num = random.randint(0, 998) # Gen random int from 0 to 998
+            # part1_num = random.randint(100,300) # or just use this
+            if part1_num not in part1_not_valid_digits:
+                part1 = str(part1_num).rjust(3, "0") # Convert into string
+                part1_valid = True # Break loop
+
+        # PART 02
+        part2 = __class__._mod7_gen(num_of_digits=7)
+
+        # OUTPUT
+        return f"{part1}-{part2}"
+
+    @staticmethod
+    def mod7_11_digit_key(fast: bool = False) -> str:
+        """
+        11-digit CD Key generator
+
+        Format: `XXXX-XXXXXXX`
+        - `XXXX`: Can be anything from `0001` to `9991`.
+        The last digit must be 3rd digit + `1` or `2`.
+        When the result is > `9`, it overflows to `0` or `1`.
+        - `XXXXXXX`: Same as CD Key
+        
+        Parameters:
+        ---
+        fast : bool
+            Use pre-generated key
+            [Default: False]
+        
+        Return:
+        ---
+        str:
+            Mod7 Key
+        """
+        
+        # Fast mode: pre-generated key
+        if fast:
+            return "0001-0000007"
+        
+        # PART 01
+        part1_valid = False
+        part1: str = ""
+        while not part1_valid:
+            part1_1_num = random.randint(0, 999) # Random 3-digit number
+            last_digit_choice = [1, 2] # Choice for last digit
+            part1_2_num = int(str(part1_1_num)[-1]) + random.choice(last_digit_choice) # Make last digit
+            if part1_2_num > 9: # Check condition then overflow
+                part1_2_num = str(part1_2_num)[-1]
+            part1_str = f"{part1_1_num}{part1_2_num}" # Concat string
+            if int(part1_str) < 9991: # Check if < 9991
+                part1 = part1_str.rjust(4, "0")
+                part1_valid = True
+
+        # PART 02
+        part2 = __class__._mod7_gen(num_of_digits=7)
+
+        # OUTPUT
+        return f"{part1}-{part2}"
+
+    @staticmethod
+    def mod7_oem_key(fast: bool = False) -> str:
+        """
+        OEM Key generator
+
+        Format: `ABCYY-OEM-0XXXXXX-XXXXX`
+        - `ABC`: The day of the year. It can be any value from `001` to `366`
+        - `YY`: The last two digits of the year. It can be anything from `95` to `03`
+        - `0XXXXXX`: A random number that has a sum that is divisible by `7` and does not end with `0`, `8` or `3`.
+        - `XXXXX`: A random 5-digit number
+
+        Parameters:
+        ---
+        fast : bool
+            Use pre-generated key
+            [Default: False]
+        
+        Return:
+        ---
+        str:
+            Mod7 Key
+        """
+        
+        # Fast mode: pre-generated key
+        if fast:
+            return "00100-OEM-0000007-00000"
+        
+        # PART ABC
+        abc_part = str(random.randint(1, 365)).rjust(3, "0")
 
-    **SHOULD NOT BE USED!**
-    """
-    
-    # Library
-    import base64
-    import json
-
-    # Data
-    data1='ewogICAgIk1haW4gWFAiOiBbCiAgICAgICAgIkpEM1QyLVFIMzZSLVg'
-    data2='3VzJXLTdSM1hULURWUlBRIgogICAgXSwKICAgICJXaW5kb3dzIFhQIF'
-    data3='NQMiI6IFsKICAgICAgICAiUVc5QjgtM1RKWFctWDM2SEYtUVQ5NFgtO'
-    data4='FJYR0QiLAogICAgICAgICJKVkJGUS1LREI4Sy1GOTdNUi1LNEdUSC1E'
-    data5='VDRXNiIsCiAgICAgICAgIkZWN1hNLUM0UVdDLTlSS1Q5LVg3MldZLU0'
-    data6='zRlc4IiwKICAgICAgICAiRzlEMlQtTUg5QkYtSEs3NjQtUUpSN1gtTU'
-    data7='pLR00iLAogICAgICAgICJUSDdUTS1CQkhZSi03N0cyNi1NMlcyVC1DS'
-    data8='kJDMyIsCiAgICAgICAgIlZDRlFELVY5Rlg5LTQ2V1ZILUszQ0Q0LTRK'
-    data9='M0pNIiwKICAgICAgICAiRFEzUEctMlBUR0otNDNGUDItUlBSS0ItUUJ'
-    data10='ZUlkiLAogICAgICAgICJCNjZWWS00RDk0VC1UUFBENC00M0Y3Mi04WD'
-    data11='RGWSIKICAgIF0sCiAgICAiV2luZG93cyBYUCBTUDMiOiBbCiAgICAgI'
-    data12='CAgIkpEM1QyLVFIMzZSLVg3VzJXLTdSM1hULURWUlBRIiwKICAgICAg'
-    data13='ICAiWE1EQ1YtMlRKTVItN0pENjYtWVRWTUstVjdQQkQiLAogICAgICA'
-    data14='gICJYNk1ZWS02QkgzVC1ZUkJUOC1IOFlQSC1SRzY4VCIsCiAgICAgIC'
-    data15='AgIk1ZSFZULVdRNDlNLVFSUFZGLVY4NkZDLVAzUjhZIiwKICAgICAgI'
-    data16='CAiUlQzUUQtVjhQNFAtQzczRFktUkNHNFItUU02WUQiLAogICAgICAg'
-    data17='ICJNUjQ5Ui1EUkpYWC1NNlBYMi1WOTZCRi04Q0tCSiIsCiAgICAgICA'
-    data18='gIk1WRjRELVc3NzRLLU1DNFZNLVFZNlhZLVIzOFRCIgogICAgXQp9'
-    data98=data1+data2+data3+data4+data5+data6+data7+data8+data9+data10
-    data99=data11+data12+data13+data14+data15+data16+data17+data18
-    data=data98+data99
-
-    # Convert data
-    decoded_data = base64.b64decode(data.encode("utf-8")).decode("utf-8")
-    real_data = json.loads(decoded_data)
-    
-    # Output
-    if show_all:
-        return real_data
-    else:
-        return real_data['Main XP'][0]
+        # PART YY
+        year_choice = ["95", "96", "97", "98", "99", "00", "01", "02"]
+        # isleap = [False, True, False, False, False, True, False, False]
+        # year_choice = ["95", "96", "97", "98", "99", "00", "01", "02", "03"] # "03" not wotk on win95
+        y_part = random.choice(year_choice)
+
+        # NUM PART
+        num_part = __class__._mod7_gen(num_of_digits=6)
+
+        # NUM PART 02
+        num_part_2 = str(random.randint(0, 99999)).rjust(5, "0")
+
+        # OUTPUT
+        return f"{abc_part}{y_part}-OEM-0{num_part}-{num_part_2}"
+
+    @staticmethod
+    def mod7_combo(fast: bool = False):
+        """
+        A combo that consist of CD, 11-digit, and OEM Key
+
+        Parameters:
+        ---
+        fast : bool
+            Use pre-generated key
+            [Default: False]
+        
+        Return:
+        ---
+        dict:
+            Mod7 Key combo
+        """
+        out = {
+            "CD Key": __class__.mod7_cd_key(fast=fast),
+            "OEM Key": __class__.mod7_oem_key(fast=fast),
+            "11-digit Key": __class__.mod7_11_digit_key(fast=fast)
+        }
+        return out
+
+
+# Run
+###########################################################################
+if __name__ == "__main__":
+    test = Keygen()
+    print(test.mod7_combo())
```

### Comparing `absfuyu-2.0.0/src/absfuyu/tools/obfuscator.py` & `absfuyu-2.1.0/src/absfuyu/tools/obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/tools/stats.py` & `absfuyu-2.1.0/src/absfuyu/tools/stats.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/tools/web.py` & `absfuyu-2.1.0/src/absfuyu/tools/web.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/unused.py` & `absfuyu-2.1.0/src/absfuyu/unused.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/util/__init__.py` & `absfuyu-2.1.0/src/absfuyu/util/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 Absufyu: Utilities
 ---
 Some random utilities
 
-Version: 1.1.0
-Date updated: 05/06/2023 (dd/mm/yyyy)
+Version: 1.2.0
+Date updated: 09/06/2023 (dd/mm/yyyy)
 """
 
 
 # Library
 ###########################################################################
 import pkg_resources
 from typing import Union
 
 from absfuyu.logger import logger, log_debug
 from absfuyu.util.api import APIRequest
 from absfuyu.util.json_method import JsonFile, load_json
 from absfuyu.util.path import DirStructure
 from absfuyu.util.performance import *
+from absfuyu.util.pkl import Pickler
 from absfuyu.util.zipped import Zipper
 
 
 # Function
 ###########################################################################
 def get_installed_package(version_included: bool = False):
     """
```

### Comparing `absfuyu-2.0.0/src/absfuyu/util/api.py` & `absfuyu-2.1.0/src/absfuyu/util/api.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/util/json_method.py` & `absfuyu-2.1.0/src/absfuyu/util/json_method.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/util/path.py` & `absfuyu-2.1.0/src/absfuyu/util/path.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/util/performance.py` & `absfuyu-2.1.0/src/absfuyu/util/performance.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/util/zipped.py` & `absfuyu-2.1.0/src/absfuyu/util/zipped.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/version.py` & `absfuyu-2.1.0/src/absfuyu/version.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu/version2.py` & `absfuyu-2.1.0/src/absfuyu/version2.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/src/absfuyu.egg-info/PKG-INFO` & `absfuyu-2.1.0/src/absfuyu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absfuyu
-Version: 2.0.0
+Version: 2.1.0
 Summary: A small collection of code
 Home-page: https://github.com/AbsoluteWinter/absfuyu
 Author: somewhatcold (AbsoluteWinter)
 Author-email: this.is.a.fake.mail@fakemail.absfuyu.com
 License: MIT
 Project-URL: Documentation, https://absolutewinter.github.io/absfuyu
 Project-URL: Source Code, https://github.com/AbsoluteWinter/absfuyu
@@ -19,16 +19,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: rich
 Provides-Extra: beautiful
+Provides-Extra: rich
 Provides-Extra: cli
 Provides-Extra: click
 Provides-Extra: extra
 Provides-Extra: colorama
 Provides-Extra: build
 Provides-Extra: twine
 Provides-Extra: virtualenv
@@ -38,16 +38,16 @@
 Provides-Extra: tools
 Provides-Extra: requests
 Provides-Extra: numpy
 Provides-Extra: pandas
 Provides-Extra: matplotlib
 Provides-Extra: scipy
 Provides-Extra: LunarCalendar
-Provides-Extra: autoimport
 Provides-Extra: fixers
+Provides-Extra: autoimport
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
-Metadata-Version: 2.1 Name: absfuyu Version: 2.0.0 Summary: A small collection
+Metadata-Version: 2.1 Name: absfuyu Version: 2.1.0 Summary: A small collection
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
-rich Provides-Extra: beautiful Provides-Extra: cli Provides-Extra: click
+beautiful Provides-Extra: rich Provides-Extra: cli Provides-Extra: click
 Provides-Extra: extra Provides-Extra: colorama Provides-Extra: build Provides-
 Extra: twine Provides-Extra: virtualenv Provides-Extra: setuptools Provides-
 Extra: wheel Provides-Extra: pipx Provides-Extra: tools Provides-Extra:
 requests Provides-Extra: numpy Provides-Extra: pandas Provides-Extra:
 matplotlib Provides-Extra: scipy Provides-Extra: LunarCalendar Provides-Extra:
-autoimport Provides-Extra: fixers Provides-Extra: black Provides-Extra: pytest
+fixers Provides-Extra: autoimport Provides-Extra: black Provides-Extra: pytest
 Provides-Extra: test Provides-Extra: tox Provides-Extra: sphinx Provides-Extra:
 sphinx_rtd_theme Provides-Extra: python-dateutil Provides-Extra: unidecode
 Provides-Extra: all License-File: LICENSE
                             ****** [absfuyu] ******
   [pypi] [https://img.shields.io/pypi/v/absfuyu?style=flat-square] [https://
            img.shields.io/badge/license-MIT-blue?style=flat-square]
 --- ## **SUMMARY:** *TL;DR: A collection of code* ## **INSTALLATION:** ```bash
```

### Comparing `absfuyu-2.0.0/src/absfuyu.egg-info/SOURCES.txt` & `absfuyu-2.1.0/src/absfuyu.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -66,25 +66,27 @@
 src/absfuyu/tools/stats.py
 src/absfuyu/tools/web.py
 src/absfuyu/util/__init__.py
 src/absfuyu/util/api.py
 src/absfuyu/util/json_method.py
 src/absfuyu/util/path.py
 src/absfuyu/util/performance.py
+src/absfuyu/util/pkl.py
 src/absfuyu/util/zipped.py
 tests/test_DictKai.py
 tests/test_Generator.py
 tests/test_IntNumber.py
 tests/test_ListKai.py
 tests/test_Text.py
 tests/test_api.py
 tests/test_beautiful.py
 tests/test_config.py
 tests/test_converter.py
 tests/test_everything.py
 tests/test_extensions.py
 tests/test_fun.py
+tests/test_generator.py
 tests/test_json_method.py
 tests/test_obfuscator.py
 tests/test_path.py
 tests/test_pkg_data.py
 tests/test_util.py
```

### Comparing `absfuyu-2.0.0/src/absfuyu.egg-info/requires.txt` & `absfuyu-2.1.0/src/absfuyu.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 [:python_version == "3.7"]
 typing_extensions>=3.7.4
 
 [LunarCalendar]
 LunarCalendar>=0.0.9
 
 [all]
-scipy
-tox>=3.24.5
-pytest>=6.2.5
+colorama>=0.4
 unidecode
-twine>=3.7.1
 wheel
+tox>=3.24.5
 pipx
-matplotlib
-autoimport
 pandas
-sphinx_rtd_theme
-sphinx
-click>=8.0.0
+autoimport
+numpy
 build
-black>=22.1.0
-LunarCalendar>=0.0.9
-colorama>=0.4
 python-dateutil
 setuptools>=51.0.0
-numpy
 virtualenv>=20.13.0
+scipy
+LunarCalendar>=0.0.9
 requests
 rich
+matplotlib
+twine>=3.7.1
+click>=8.0.0
+pytest>=6.2.5
+sphinx_rtd_theme
+black>=22.1.0
+sphinx
 
 [autoimport]
 autoimport
 
 [beautiful]
 rich
 
@@ -49,43 +49,43 @@
 [click]
 click>=8.0.0
 
 [colorama]
 colorama>=0.4
 
 [dev]
-setuptools>=51.0.0
+virtualenv>=20.13.0
+pipx
 twine>=3.7.1
-sphinx_rtd_theme
+colorama>=0.4
+unidecode
 click>=8.0.0
-pipx
-build
+rich
 pytest>=6.2.5
 sphinx
-virtualenv>=20.13.0
-unidecode
-colorama>=0.4
+build
+sphinx_rtd_theme
+setuptools>=51.0.0
 wheel
-rich
 
 [extra]
 scipy
-numpy
-click>=8.0.0
-matplotlib
 pandas
-LunarCalendar>=0.0.9
-unidecode
 colorama>=0.4
+LunarCalendar>=0.0.9
+click>=8.0.0
 requests
+numpy
+unidecode
 python-dateutil
+matplotlib
 
 [fixers]
-autoimport
 black>=22.1.0
+autoimport
 
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
-pytest>=6.2.5
 tox>=3.24.5
+pytest>=6.2.5
 
 [tools]
 requests
 
 [tox]
 tox>=3.24.5
```

### Comparing `absfuyu-2.0.0/tests/test_DictKai.py` & `absfuyu-2.1.0/tests/test_DictKai.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/tests/test_Generator.py` & `absfuyu-2.1.0/tests/test_Generator.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-"""
-Test: Generator
-
-Version: 1.0.0
-Date updated: 25/05/2023 (dd/mm/yyyy)
-"""
-
-
-# Library
-###########################################################################
-import re
-import string
-
-import pytest
-
-from absfuyu.collections.generator import Generator, Charset
-
-
-# Test
-###########################################################################
-# Charset
-def test_Charset():
-    assert Charset.PRODUCT_KEY == "BCDFGHJKMNPQRTVWXY2346789"
-
-def test_Charset_2():
-    """[a-zA-Z0-9]"""
-    assert Charset.DEFAULT == string.ascii_letters + string.digits
-
-
-# generate_string
-def test_generate_string():
-    """Correct len and a list"""
-    temp = Generator.generate_string(
-        charset=Charset.DEFAULT,
-        size=8,
-        times=1,
-        unique=False,
-        string_type_if_1=False
-    )
-    assert isinstance(temp, list) and len(temp[0])==8
-
-def test_generate_string_2():
-    """Correct len and a str"""
-    temp = Generator.generate_string(
-        charset=Charset.DEFAULT,
-        size=8,
-        times=1,
-        unique=False,
-        string_type_if_1=True
-    )
-    assert isinstance(temp, str) and len(temp)==8
-
-def test_generate_string_3():
-    """Unique generate"""
-    temp = Generator.generate_string(
-        charset=Charset.DEFAULT,
-        size=2,
-        times=600,
-        unique=True,
-    )
-    assert len(temp) == len(list(set(temp)))
-
-
-# generate_key
-def test_generate_key():
-    """Check if key generate correctly"""
-    key = Generator.generate_key(
-        charset=Charset.PRODUCT_KEY,
-        letter_per_block=5,
-        number_of_block=5,
-        sep="-"
-    )
-    key_pattern = r"[A-Z0-9]{5}-[A-Z0-9]{5}-[A-Z0-9]{5}-[A-Z0-9]{5}-[A-Z0-9]{5}"
-    check_result = re.search(key_pattern, key) # Correct default key pattern
-    correct_len = len(key) == 29 # Correct default key length
-    assert check_result is not None and correct_len
-
-
-# generate_check_digit
-def test_generate_check_digit():
-    assert Generator.generate_check_digit(95489683516944151927) == 0
-
-def test_generate_check_digit_2():
-    assert Generator.generate_check_digit(15392479156575151882) == 1
-
-def test_generate_check_digit_3():
-    assert Generator.generate_check_digit(74662116892282572844) == 2
-
-def test_generate_check_digit_4():
-    assert Generator.generate_check_digit(91274812716671415644) == 3
-
-def test_generate_check_digit_5():
-    assert Generator.generate_check_digit(94984564168167844561) == 4
-
-def test_generate_check_digit_6():
-    assert Generator.generate_check_digit(94273419372476632513) == 5
-
-def test_generate_check_digit_7():
-    assert Generator.generate_check_digit(78985469454121383396) == 6
-
-def test_generate_check_digit_8():
-    assert Generator.generate_check_digit(34458526632449856638) == 7
-
-def test_generate_check_digit_9():
-    assert Generator.generate_check_digit(95486688921998713381) == 8
-
-def test_generate_check_digit_10():
-    assert Generator.generate_check_digit(48981383446354864289) == 9
+"""
+Test: Generator
+
+Version: 1.0.0
+Date updated: 25/05/2023 (dd/mm/yyyy)
+"""
+
+
+# Library
+###########################################################################
+import re
+import string
+
+import pytest
+
+from absfuyu.collections.generator import Generator, Charset
+
+
+# Test
+###########################################################################
+# Charset
+def test_Charset():
+    assert Charset.PRODUCT_KEY == "BCDFGHJKMNPQRTVWXY2346789"
+
+def test_Charset_2():
+    """[a-zA-Z0-9]"""
+    assert Charset.DEFAULT == string.ascii_letters + string.digits
+
+
+# generate_string
+def test_generate_string():
+    """Correct len and a list"""
+    temp = Generator.generate_string(
+        charset=Charset.DEFAULT,
+        size=8,
+        times=1,
+        unique=False,
+        string_type_if_1=False
+    )
+    assert isinstance(temp, list) and len(temp[0])==8
+
+def test_generate_string_2():
+    """Correct len and a str"""
+    temp = Generator.generate_string(
+        charset=Charset.DEFAULT,
+        size=8,
+        times=1,
+        unique=False,
+        string_type_if_1=True
+    )
+    assert isinstance(temp, str) and len(temp)==8
+
+def test_generate_string_3():
+    """Unique generate"""
+    temp = Generator.generate_string(
+        charset=Charset.DEFAULT,
+        size=2,
+        times=600,
+        unique=True,
+    )
+    assert len(temp) == len(list(set(temp)))
+
+
+# generate_key
+def test_generate_key():
+    """Check if key generate correctly"""
+    key = Generator.generate_key(
+        charset=Charset.PRODUCT_KEY,
+        letter_per_block=5,
+        number_of_block=5,
+        sep="-"
+    )
+    key_pattern = r"[A-Z0-9]{5}-[A-Z0-9]{5}-[A-Z0-9]{5}-[A-Z0-9]{5}-[A-Z0-9]{5}"
+    check_result = re.search(key_pattern, key) # Correct default key pattern
+    correct_len = len(key) == 29 # Correct default key length
+    assert check_result is not None and correct_len
+
+
+# generate_check_digit
+def test_generate_check_digit():
+    assert Generator.generate_check_digit(95489683516944151927) == 0
+
+def test_generate_check_digit_2():
+    assert Generator.generate_check_digit(15392479156575151882) == 1
+
+def test_generate_check_digit_3():
+    assert Generator.generate_check_digit(74662116892282572844) == 2
+
+def test_generate_check_digit_4():
+    assert Generator.generate_check_digit(91274812716671415644) == 3
+
+def test_generate_check_digit_5():
+    assert Generator.generate_check_digit(94984564168167844561) == 4
+
+def test_generate_check_digit_6():
+    assert Generator.generate_check_digit(94273419372476632513) == 5
+
+def test_generate_check_digit_7():
+    assert Generator.generate_check_digit(78985469454121383396) == 6
+
+def test_generate_check_digit_8():
+    assert Generator.generate_check_digit(34458526632449856638) == 7
+
+def test_generate_check_digit_9():
+    assert Generator.generate_check_digit(95486688921998713381) == 8
+
+def test_generate_check_digit_10():
+    assert Generator.generate_check_digit(48981383446354864289) == 9
```

### Comparing `absfuyu-2.0.0/tests/test_IntNumber.py` & `absfuyu-2.1.0/tests/test_IntNumber.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/tests/test_ListKai.py` & `absfuyu-2.1.0/tests/test_ListKai.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/tests/test_Text.py` & `absfuyu-2.1.0/tests/test_Text.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/tests/test_api.py` & `absfuyu-2.1.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/tests/test_config.py` & `absfuyu-2.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/tests/test_converter.py` & `absfuyu-2.1.0/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/tests/test_obfuscator.py` & `absfuyu-2.1.0/tests/test_obfuscator.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/tests/test_path.py` & `absfuyu-2.1.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `absfuyu-2.0.0/tests/test_util.py` & `absfuyu-2.1.0/tests/test_util.py`

 * *Files identical despite different names*

