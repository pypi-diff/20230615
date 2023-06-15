# Comparing `tmp/nihtest-1.0.0.tar.gz` & `tmp/nihtest-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nihtest-1.0.0.tar", last modified: Fri Jun  9 15:37:47 2023, max compression
+gzip compressed data, was "nihtest-1.1.0.tar", last modified: Thu Jun 15 13:17:21 2023, max compression
```

## Comparing `nihtest-1.0.0.tar` & `nihtest-1.1.0.tar`

### file list

```diff
@@ -1,134 +1,143 @@
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-09 15:37:47.675057 nihtest-1.0.0/
--rw-r--r--   0 dillo      (501) staff       (20)      993 2023-06-09 15:33:15.000000 nihtest-1.0.0/CMakeLists.txt
--rw-r--r--   0 dillo      (501) staff       (20)     1406 2023-03-22 09:46:53.000000 nihtest-1.0.0/LICENSE
--rw-r--r--   0 dillo      (501) staff       (20)      142 2023-06-09 14:24:21.000000 nihtest-1.0.0/MANIFEST.in
--rw-r--r--   0 dillo      (501) staff       (20)       75 2023-06-09 14:24:21.000000 nihtest-1.0.0/NEWS.md
--rw-r--r--   0 dillo      (501) staff       (20)     1366 2023-06-09 15:37:47.675171 nihtest-1.0.0/PKG-INFO
--rw-r--r--   0 dillo      (501) staff       (20)      808 2023-06-09 15:21:43.000000 nihtest-1.0.0/README.md
--rw-r--r--   0 dillo      (501) staff       (20)      103 2023-06-09 15:22:18.000000 nihtest-1.0.0/TODO.md
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-09 15:37:47.661948 nihtest-1.0.0/manpages/
--rw-r--r--   0 dillo      (501) staff       (20)     9527 2023-06-09 14:52:52.000000 nihtest-1.0.0/manpages/nihtest-case.html
--rw-r--r--   0 dillo      (501) staff       (20)     5705 2023-06-09 14:53:29.000000 nihtest-1.0.0/manpages/nihtest-case.man
--rw-r--r--   0 dillo      (501) staff       (20)     5833 2023-06-09 14:24:21.000000 nihtest-1.0.0/manpages/nihtest-case.mdoc
--rw-r--r--   0 dillo      (501) staff       (20)    10478 2023-06-09 14:52:52.000000 nihtest-1.0.0/manpages/nihtest.conf.html
--rw-r--r--   0 dillo      (501) staff       (20)     5980 2023-06-09 14:53:29.000000 nihtest-1.0.0/manpages/nihtest.conf.man
--rw-r--r--   0 dillo      (501) staff       (20)     5712 2023-06-09 14:24:21.000000 nihtest-1.0.0/manpages/nihtest.conf.mdoc
--rw-r--r--   0 dillo      (501) staff       (20)     7824 2023-06-09 14:52:52.000000 nihtest-1.0.0/manpages/nihtest.html
--rw-r--r--   0 dillo      (501) staff       (20)     4533 2023-06-09 14:53:29.000000 nihtest-1.0.0/manpages/nihtest.man
--rw-r--r--   0 dillo      (501) staff       (20)     4141 2023-06-09 14:24:21.000000 nihtest-1.0.0/manpages/nihtest.mdoc
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-09 15:37:47.663250 nihtest-1.0.0/nihtest/
--rw-r--r--   0 dillo      (501) staff       (20)     1453 2023-06-09 14:24:21.000000 nihtest-1.0.0/nihtest/Command.py
--rw-r--r--   0 dillo      (501) staff       (20)     4976 2023-04-17 17:35:22.000000 nihtest-1.0.0/nihtest/CompareArrays.py
--rw-r--r--   0 dillo      (501) staff       (20)     3390 2023-06-09 14:24:21.000000 nihtest-1.0.0/nihtest/Configuration.py
--rw-r--r--   0 dillo      (501) staff       (20)      667 2023-04-24 10:05:06.000000 nihtest-1.0.0/nihtest/Features.py
--rw-r--r--   0 dillo      (501) staff       (20)     3186 2023-06-09 14:22:50.000000 nihtest-1.0.0/nihtest/File.py
--rw-r--r--   0 dillo      (501) staff       (20)     1056 2023-04-15 14:24:35.000000 nihtest-1.0.0/nihtest/Sandbox.py
--rw-r--r--   0 dillo      (501) staff       (20)     4568 2023-06-09 14:24:21.000000 nihtest-1.0.0/nihtest/Test.py
--rw-r--r--   0 dillo      (501) staff       (20)     8173 2023-06-09 14:24:21.000000 nihtest-1.0.0/nihtest/TestCase.py
--rw-r--r--   0 dillo      (501) staff       (20)      665 2023-04-24 10:05:06.000000 nihtest-1.0.0/nihtest/Utility.py
--rw-r--r--   0 dillo      (501) staff       (20)        0 2023-03-22 10:19:23.000000 nihtest-1.0.0/nihtest/__init__.py
--rw-r--r--   0 dillo      (501) staff       (20)     1475 2023-06-09 15:33:15.000000 nihtest-1.0.0/nihtest/__main__.py
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-09 15:37:47.663845 nihtest-1.0.0/nihtest.egg-info/
--rw-r--r--   0 dillo      (501) staff       (20)     1366 2023-06-09 15:37:47.000000 nihtest-1.0.0/nihtest.egg-info/PKG-INFO
--rw-r--r--   0 dillo      (501) staff       (20)     2991 2023-06-09 15:37:47.000000 nihtest-1.0.0/nihtest.egg-info/SOURCES.txt
--rw-r--r--   0 dillo      (501) staff       (20)        1 2023-06-09 15:37:47.000000 nihtest-1.0.0/nihtest.egg-info/dependency_links.txt
--rw-r--r--   0 dillo      (501) staff       (20)       50 2023-06-09 15:37:47.000000 nihtest-1.0.0/nihtest.egg-info/entry_points.txt
--rw-r--r--   0 dillo      (501) staff       (20)        8 2023-06-09 15:37:47.000000 nihtest-1.0.0/nihtest.egg-info/top_level.txt
--rw-r--r--   0 dillo      (501) staff       (20)      713 2023-06-09 15:33:15.000000 nihtest-1.0.0/pyproject.toml
--rw-r--r--   0 dillo      (501) staff       (20)       76 2023-06-09 15:37:47.675408 nihtest-1.0.0/setup.cfg
-drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-09 15:37:47.674932 nihtest-1.0.0/tests/
--rw-r--r--   0 dillo      (501) staff       (20)     2116 2023-05-19 12:07:31.000000 nihtest-1.0.0/tests/CMakeLists.txt
--rw-r--r--   0 dillo      (501) staff       (20)      143 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/argument-escaped.input
--rw-r--r--   0 dillo      (501) staff       (20)      138 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/argument-escaped.test
--rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/binary-1
--rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/binary-2
--rw-r--r--   0 dillo      (501) staff       (20)     1803 2023-04-12 13:00:35.000000 nihtest-1.0.0/tests/can-preload.c
--rw-r--r--   0 dillo      (501) staff       (20)     2586 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/cat.c
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-05-19 12:10:40.000000 nihtest-1.0.0/tests/comparator-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      305 2023-05-19 12:16:34.000000 nihtest-1.0.0/tests/comparator-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       66 2023-05-19 12:12:53.000000 nihtest-1.0.0/tests/comparator-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      219 2023-05-19 12:10:40.000000 nihtest-1.0.0/tests/comparator-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1585 2023-05-19 12:16:03.000000 nihtest-1.0.0/tests/comparator.c
--rw-r--r--   0 dillo      (501) staff       (20)       65 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/compare-binary-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      249 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/compare-binary-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       56 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/compare-binary-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      140 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/compare-binary-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       64 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/config.h
--rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/default-stderr-replace.input
--rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/default-stderr-replace.test
--rw-r--r--   0 dillo      (501) staff       (20)      103 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/description-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      136 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/diff-1.input
--rw-r--r--   0 dillo      (501) staff       (20)      218 2023-04-17 17:35:49.000000 nihtest-1.0.0/tests/diff-1.test
--rw-r--r--   0 dillo      (501) staff       (20)      106 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/diff-2.input
--rw-r--r--   0 dillo      (501) staff       (20)      188 2023-04-17 17:36:44.000000 nihtest-1.0.0/tests/diff-2.test
--rw-r--r--   0 dillo      (501) staff       (20)     1963 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/echo.c
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/failure.txt
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/false-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      201 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/false-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       31 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/false-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/false-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1664 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/false.c
--rw-r--r--   0 dillo      (501) staff       (20)       62 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/features-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      236 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/features-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/features-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      152 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/features-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       61 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/features-skip.input
--rw-r--r--   0 dillo      (501) staff       (20)      153 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/features-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/file-del-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      246 2023-04-12 10:14:06.000000 nihtest-1.0.0/tests/file-del-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       85 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/file-del-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      158 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/file-del-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       68 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/file-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      254 2023-04-15 15:28:11.000000 nihtest-1.0.0/tests/file-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      398 2023-04-15 14:27:28.000000 nihtest-1.0.0/tests/file-inline-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      320 2023-04-15 15:28:58.000000 nihtest-1.0.0/tests/file-inline-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       59 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/file-new-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      217 2023-04-12 10:14:06.000000 nihtest-1.0.0/tests/file-new-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      111 2023-04-12 10:55:14.000000 nihtest-1.0.0/tests/file-new-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/file-new-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:53:21.000000 nihtest-1.0.0/tests/file-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/file-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      165 2023-04-12 11:02:07.000000 nihtest-1.0.0/tests/file-subdirectory-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      156 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/file-subdirectory-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     3290 2023-04-12 11:02:07.000000 nihtest-1.0.0/tests/file.c
--rw-r--r--   0 dillo      (501) staff       (20)     2138 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/getenv.c
--rw-r--r--   0 dillo      (501) staff       (20)     1736 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/ineffective-remove.c
--rw-r--r--   0 dillo      (501) staff       (20)      325 2023-06-09 14:24:21.000000 nihtest-1.0.0/tests/nihtest-conf.in
--rw-r--r--   0 dillo      (501) staff       (20)      172 2023-04-12 10:40:04.000000 nihtest-1.0.0/tests/nihtest.conf.in
--rw-r--r--   0 dillo      (501) staff       (20)      326 2023-04-12 14:38:51.000000 nihtest-1.0.0/tests/parameter-tests-1.input
--rw-r--r--   0 dillo      (501) staff       (20)     1406 2023-04-12 14:52:24.000000 nihtest-1.0.0/tests/parameter-tests-1.test
--rw-r--r--   0 dillo      (501) staff       (20)       79 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/parameter-tests-2.input
--rw-r--r--   0 dillo      (501) staff       (20)      340 2023-04-12 14:53:18.000000 nihtest-1.0.0/tests/parameter-tests-2.test
--rw-r--r--   0 dillo      (501) staff       (20)       53 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/precheck-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      213 2023-04-12 12:29:19.000000 nihtest-1.0.0/tests/precheck-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       52 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/precheck-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/precheck-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       54 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/precheck-skip.input
--rw-r--r--   0 dillo      (501) staff       (20)      130 2023-04-12 12:29:19.000000 nihtest-1.0.0/tests/precheck-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)      174 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/preload-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      161 2023-04-12 13:00:35.000000 nihtest-1.0.0/tests/preload-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      163 2023-04-12 13:00:35.000000 nihtest-1.0.0/tests/preload-skip.test
--rw-r--r--   0 dillo      (501) staff       (20)      133 2023-04-15 11:30:23.000000 nihtest-1.0.0/tests/setenv-config-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      144 2023-04-15 11:30:23.000000 nihtest-1.0.0/tests/setenv-config-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      158 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/setenv-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/setenv-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      127 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/stderr-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      265 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/stderr-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/stderr-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/stderr-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      211 2023-04-12 11:16:36.000000 nihtest-1.0.0/tests/stderr-replace-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      147 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/stderr-replace-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      112 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/stdin-file-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      135 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/stdin-file-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      146 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/stdin-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/stdin-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)      124 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/stdout-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      253 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/stdout-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)      120 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/stdout-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/stdout-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)       27 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/success.txt
--rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/true-fail.input
--rw-r--r--   0 dillo      (501) staff       (20)      197 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/true-fail.test
--rw-r--r--   0 dillo      (501) staff       (20)       30 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/true-pass.input
--rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-12 10:10:55.000000 nihtest-1.0.0/tests/true-pass.test
--rw-r--r--   0 dillo      (501) staff       (20)     1663 2023-03-31 09:51:38.000000 nihtest-1.0.0/tests/true.c
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.228451 nihtest-1.1.0/
+-rw-r--r--   0 dillo      (501) staff       (20)      993 2023-06-15 12:45:47.000000 nihtest-1.1.0/CMakeLists.txt
+-rw-r--r--   0 dillo      (501) staff       (20)     1406 2023-04-15 19:42:21.000000 nihtest-1.1.0/LICENSE
+-rw-r--r--   0 dillo      (501) staff       (20)      142 2023-06-15 10:18:02.000000 nihtest-1.1.0/MANIFEST.in
+-rw-r--r--   0 dillo      (501) staff       (20)      200 2023-06-15 13:17:15.000000 nihtest-1.1.0/NEWS.md
+-rw-r--r--   0 dillo      (501) staff       (20)     1366 2023-06-15 13:17:21.228506 nihtest-1.1.0/PKG-INFO
+-rw-r--r--   0 dillo      (501) staff       (20)      808 2023-06-15 10:18:02.000000 nihtest-1.1.0/README.md
+-rw-r--r--   0 dillo      (501) staff       (20)      116 2023-06-15 13:14:31.000000 nihtest-1.1.0/TODO.md
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.213201 nihtest-1.1.0/manpages/
+-rw-r--r--   0 dillo      (501) staff       (20)     9383 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest-case.html
+-rw-r--r--   0 dillo      (501) staff       (20)     5701 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest-case.man
+-rw-r--r--   0 dillo      (501) staff       (20)     6209 2023-06-15 13:12:39.000000 nihtest-1.1.0/manpages/nihtest-case.mdoc
+-rw-r--r--   0 dillo      (501) staff       (20)    10371 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.conf.html
+-rw-r--r--   0 dillo      (501) staff       (20)     6000 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.conf.man
+-rw-r--r--   0 dillo      (501) staff       (20)     6163 2023-06-15 13:09:51.000000 nihtest-1.1.0/manpages/nihtest.conf.mdoc
+-rw-r--r--   0 dillo      (501) staff       (20)     7738 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.html
+-rw-r--r--   0 dillo      (501) staff       (20)     4599 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.man
+-rw-r--r--   0 dillo      (501) staff       (20)     4141 2023-06-15 10:18:02.000000 nihtest-1.1.0/manpages/nihtest.mdoc
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.215211 nihtest-1.1.0/nihtest/
+-rw-r--r--   0 dillo      (501) staff       (20)     1333 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/Command.py
+-rw-r--r--   0 dillo      (501) staff       (20)     4976 2023-05-01 09:06:04.000000 nihtest-1.1.0/nihtest/CompareArrays.py
+-rw-r--r--   0 dillo      (501) staff       (20)     5040 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/Configuration.py
+-rw-r--r--   0 dillo      (501) staff       (20)      676 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/Environment.py
+-rw-r--r--   0 dillo      (501) staff       (20)      667 2023-05-01 09:06:04.000000 nihtest-1.1.0/nihtest/Features.py
+-rw-r--r--   0 dillo      (501) staff       (20)     3282 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/File.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1056 2023-04-15 19:42:21.000000 nihtest-1.1.0/nihtest/Sandbox.py
+-rw-r--r--   0 dillo      (501) staff       (20)     4471 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/Test.py
+-rw-r--r--   0 dillo      (501) staff       (20)     9392 2023-06-15 12:45:46.000000 nihtest-1.1.0/nihtest/TestCase.py
+-rw-r--r--   0 dillo      (501) staff       (20)      665 2023-05-01 09:06:04.000000 nihtest-1.1.0/nihtest/Utility.py
+-rw-r--r--   0 dillo      (501) staff       (20)        0 2023-04-15 19:42:21.000000 nihtest-1.1.0/nihtest/__init__.py
+-rw-r--r--   0 dillo      (501) staff       (20)     1453 2023-06-15 12:45:47.000000 nihtest-1.1.0/nihtest/__main__.py
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.215727 nihtest-1.1.0/nihtest.egg-info/
+-rw-r--r--   0 dillo      (501) staff       (20)     1366 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/PKG-INFO
+-rw-r--r--   0 dillo      (501) staff       (20)     3348 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/SOURCES.txt
+-rw-r--r--   0 dillo      (501) staff       (20)        1 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/dependency_links.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       50 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/entry_points.txt
+-rw-r--r--   0 dillo      (501) staff       (20)        8 2023-06-15 13:17:21.000000 nihtest-1.1.0/nihtest.egg-info/top_level.txt
+-rw-r--r--   0 dillo      (501) staff       (20)      977 2023-06-15 12:45:47.000000 nihtest-1.1.0/pyproject.toml
+-rw-r--r--   0 dillo      (501) staff       (20)       76 2023-06-15 13:17:21.228707 nihtest-1.1.0/setup.cfg
+drwxr-xr-x   0 dillo      (501) staff       (20)        0 2023-06-15 13:17:21.228337 nihtest-1.1.0/tests/
+-rw-r--r--   0 dillo      (501) staff       (20)     2116 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/CMakeLists.txt
+-rw-r--r--   0 dillo      (501) staff       (20)      143 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/argument-escaped.input
+-rw-r--r--   0 dillo      (501) staff       (20)      138 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/argument-escaped.test
+-rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/binary-1
+-rw-r--r--   0 dillo      (501) staff       (20)        4 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/binary-2
+-rw-r--r--   0 dillo      (501) staff       (20)     1803 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/can-preload.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2586 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/cat.c
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      305 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       66 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1585 2023-06-03 15:23:12.000000 nihtest-1.1.0/tests/comparator.c
+-rw-r--r--   0 dillo      (501) staff       (20)       65 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/compare-binary-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      249 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/compare-binary-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       56 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/compare-binary-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      140 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/compare-binary-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       64 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/config.h
+-rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/default-stderr-replace.input
+-rw-r--r--   0 dillo      (501) staff       (20)      219 2023-06-15 10:18:02.000000 nihtest-1.1.0/tests/default-stderr-replace.test
+-rw-r--r--   0 dillo      (501) staff       (20)      103 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/description-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      136 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/diff-1.input
+-rw-r--r--   0 dillo      (501) staff       (20)      218 2023-05-01 09:06:04.000000 nihtest-1.1.0/tests/diff-1.test
+-rw-r--r--   0 dillo      (501) staff       (20)      106 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/diff-2.input
+-rw-r--r--   0 dillo      (501) staff       (20)      188 2023-05-01 09:06:04.000000 nihtest-1.1.0/tests/diff-2.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1963 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/echo.c
+-rw-r--r--   0 dillo      (501) staff       (20)      103 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-clear-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-clear-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       99 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-not-passed-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      172 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-not-passed-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      155 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-passthrough-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      173 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-passthrough-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      133 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-set-config-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      125 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-set-config-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      167 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-set-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      118 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-set-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      108 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-unset-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/environment-unset-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/failure.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      201 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       31 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1664 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/false.c
+-rw-r--r--   0 dillo      (501) staff       (20)       62 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      236 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       61 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      152 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       61 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-skip.input
+-rw-r--r--   0 dillo      (501) staff       (20)      153 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/features-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-del-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      246 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-del-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       85 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-del-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      158 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-del-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       68 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      254 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      398 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-inline-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      320 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-inline-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       59 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-new-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      217 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-new-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      111 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-new-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-new-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      165 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-subdirectory-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      156 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file-subdirectory-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     3290 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/file.c
+-rw-r--r--   0 dillo      (501) staff       (20)     2138 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/getenv.c
+-rw-r--r--   0 dillo      (501) staff       (20)     1736 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/ineffective-remove.c
+-rw-r--r--   0 dillo      (501) staff       (20)      330 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/nihtest-conf.in
+-rw-r--r--   0 dillo      (501) staff       (20)      172 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/nihtest.conf.in
+-rw-r--r--   0 dillo      (501) staff       (20)      415 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/parameter-tests-1.input
+-rw-r--r--   0 dillo      (501) staff       (20)     1647 2023-06-15 12:45:46.000000 nihtest-1.1.0/tests/parameter-tests-1.test
+-rw-r--r--   0 dillo      (501) staff       (20)       79 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/parameter-tests-2.input
+-rw-r--r--   0 dillo      (501) staff       (20)      340 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/parameter-tests-2.test
+-rw-r--r--   0 dillo      (501) staff       (20)       53 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      213 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       52 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      129 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       54 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-skip.input
+-rw-r--r--   0 dillo      (501) staff       (20)      130 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/precheck-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)      174 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/preload-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      161 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/preload-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      163 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/preload-skip.test
+-rw-r--r--   0 dillo      (501) staff       (20)      127 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      265 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      211 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-replace-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      147 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stderr-replace-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      112 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdin-file-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      135 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdin-file-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      146 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdin-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdin-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)      124 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdout-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      253 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdout-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)      120 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdout-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      123 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/stdout-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)       27 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/success.txt
+-rw-r--r--   0 dillo      (501) staff       (20)       30 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true-fail.input
+-rw-r--r--   0 dillo      (501) staff       (20)      197 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true-fail.test
+-rw-r--r--   0 dillo      (501) staff       (20)       30 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true-pass.input
+-rw-r--r--   0 dillo      (501) staff       (20)      117 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true-pass.test
+-rw-r--r--   0 dillo      (501) staff       (20)     1663 2023-04-15 19:42:21.000000 nihtest-1.1.0/tests/true.c
```

### Comparing `nihtest-1.0.0/CMakeLists.txt` & `nihtest-1.1.0/CMakeLists.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cmake_minimum_required(VERSION 3.12)
 
 # Also update version in nihtest/__main__.py and pyproject.toml
 project(nihtest
-        VERSION 1.0.0
+        VERSION 1.1.0
         DESCRIPTION "NiH testing framework"
         HOMEPAGE_URL "https://github.com/nih-at/nihtest"
         LANGUAGES C)
 
 enable_testing()
 
 find_package(Python3 REQUIRED COMPONENTS Interpreter)
```

### Comparing `nihtest-1.0.0/LICENSE` & `nihtest-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/PKG-INFO` & `nihtest-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nihtest
-Version: 1.0.0
+Version: 1.1.0
 Summary: A testing tool for command line utilities.
 Author-email: Dieter Baron <dillo@nih.at>, Thomas Klausner <wiz@gatalith.at>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/nih-at/nihtest
 Project-URL: Bug Tracker, https://github.com/nih-at/nihtest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nihtest-1.0.0/README.md` & `nihtest-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/manpages/nihtest-case.html` & `nihtest-1.1.0/manpages/nihtest-case.html`

 * *Files 4% similar despite different names*

```diff
@@ -30,60 +30,59 @@
    INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
    IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
    OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
    IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
    -->
 <head>
   <meta charset="utf-8"/>
-  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
   <link rel="stylesheet" href="../nih-man.css" type="text/css" media="all"/>
   <title>NIHTEST-CASE(5)</title>
 </head>
 <body>
 <table class="head">
   <tr>
     <td class="head-ltitle">NIHTEST-CASE(5)</td>
     <td class="head-vol">File Formats Manual</td>
     <td class="head-rtitle">NIHTEST-CASE(5)</td>
   </tr>
 </table>
 <div class="manual-text">
 <section class="Sh">
 <h1 class="Sh" id="NAME"><a class="permalink" href="#NAME">NAME</a></h1>
-<p class="Pp"><code class="Nm">nihtest-case</code> &#x2014;
-    <span class="Nd">test case format for nihtest</span></p>
+<code class="Nm">nihtest-case</code> &#x2014;
+<div class="Nd">test case format for nihtest</div>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="DESCRIPTION"><a class="permalink" href="#DESCRIPTION">DESCRIPTION</a></h1>
-<p class="Pp"><a class="Xr" href="nihtest.html">nihtest(1)</a> is a testing
-    tool. It uses <span class="Pa">.test</span> files as input. This man page
-    describes the format of these test files.</p>
+<a class="Xr" href="nihtest.html">nihtest(1)</a> is a testing tool. It uses
+  <span class="Pa">.test</span> files as input. This man page describes the
+  format of these test files.
 <p class="Pp">Lines beginning with &#x201C;#&#x201D; are comments.</p>
 <p class="Pp">The following commands are recognized. The
     <code class="Ic">return</code> and <code class="Ic">args</code> commands
     must appear exactly once, the others are optional.</p>
 <dl class="Bl-tag">
-  <dt id="arguments"><a class="permalink" href="#arguments"><code class="Ic">arguments</code></a>
+  <dt><a class="permalink" href="#arguments"><code class="Ic" id="arguments">arguments</code></a>
     [<var class="Ar">argument ...</var>]</dt>
   <dd>Run the program with command line arguments <var class="Ar">args</var>.
       Shell style quoting is supported.</dd>
-  <dt id="description"><a class="permalink" href="#description"><code class="Ic">description</code></a>
+  <dt><a class="permalink" href="#description"><code class="Ic" id="description">description</code></a>
     <var class="Ar">text</var></dt>
   <dd>Describes the purpose of the test.</dd>
-  <dt id="features"><a class="permalink" href="#features"><code class="Ic">features</code></a>
+  <dt><a class="permalink" href="#features"><code class="Ic" id="features">features</code></a>
     <var class="Ar">feature ...</var></dt>
   <dd>Only run test if all
       <var class="Ar">feature</var><span class="No">s</span> are present,
       otherwise skip it. The features are extracted from a top-level
       <span class="Pa">config.h</span> file. If the string
-      <code class="Dv">HAVE_FOO</code> is defined in the file, the feature
+      <code class="Dv">FOO</code> is defined in the file, the feature
       <code class="Dv">FOO</code> is assumed to be available, otherwise not. See
       also the description of <code class="Ic">top-build-directory</code> in
       <a class="Xr" href="nihtest-config.html">nihtest-config(5)</a>.</dd>
-  <dt id="file"><a class="permalink" href="#file"><code class="Ic">file</code></a>
+  <dt><a class="permalink" href="#file"><code class="Ic" id="file">file</code></a>
     <var class="Ar">name in</var> [<var class="Ar">out</var>]</dt>
   <dd>The arguments <var class="Ar">in</var> and <var class="Ar">out</var>
       specify the contents of the file <var class="Ar">name</var> in the test
       directory before and after the program is run, respectively. If
       <var class="Ar">out</var> is omitted, the file is expected to remain
       unchanged.
     <p class="Pp">&#x201C;{}&#x201D; specifies that the file does not exist (i.
@@ -91,86 +90,86 @@
     <p class="Pp">For &#x201C;&lt;inline&gt;&#x201D; the contents of the file
         are taken from the test case, up to a line consisting of
         &#x201C;end-of-inline-data&#x201D;. If both <var class="Ar">in</var> and
         <var class="Ar">out</var> are &#x201C;&lt;inline&gt;&#x201D;, the input
         data comes first. Otherwise the argument specifies the name of the file
         to copy or compare againts.</p>
   </dd>
-  <dt id="mkdir"><a class="permalink" href="#mkdir"><code class="Ic">mkdir</code></a>
+  <dt><a class="permalink" href="#mkdir"><code class="Ic" id="mkdir">mkdir</code></a>
     <var class="Ar">name</var></dt>
   <dd>Create directory <var class="Ar">name</var>
     <br/>
      in the test directory.</dd>
-  <dt id="precheck"><a class="permalink" href="#precheck"><code class="Ic">precheck</code></a>
+  <dt><a class="permalink" href="#precheck"><code class="Ic" id="precheck">precheck</code></a>
     <var class="Ar">command</var> [<var class="Ar">argument ...</var>]</dt>
   <dd>If <var class="Ar">command</var> exits with non-zero status, skip the
       test.</dd>
-  <dt id="preload"><a class="permalink" href="#preload"><code class="Ic">preload</code></a>
+  <dt><a class="permalink" href="#preload"><code class="Ic" id="preload">preload</code></a>
     <var class="Ar">object</var></dt>
   <dd>Pre-load the shared object <var class="Ar">object</var> before running the
       program.
     <p class="Pp">This is not supported on macOS and Windows, where tests with
         <code class="Ic">preload</code> will be skipped.</p>
   </dd>
-  <dt id="program"><a class="permalink" href="#program"><code class="Ic">program</code></a>
+  <dt><a class="permalink" href="#program"><code class="Ic" id="program">program</code></a>
     <var class="Ar">name</var></dt>
   <dd>Run <var class="Ar">name</var>. See the description of
       <code class="Ic">arguments</code> above for its command line arguments. If
       this directive is omitted, <code class="Ic">default-program</code> from
       <span class="Pa">nihtest.conf</span> is run.</dd>
-  <dt id="return"><a class="permalink" href="#return"><code class="Ic">return</code></a>
+  <dt><a class="permalink" href="#return"><code class="Ic" id="return">return</code></a>
     <var class="Ar">exit-code</var></dt>
   <dd><var class="Ar">exit-code</var> is the expected exit code (usually 0 on
       success).</dd>
-  <dt id="setenv"><a class="permalink" href="#setenv"><code class="Ic">setenv</code></a>
+  <dt><a class="permalink" href="#setenv"><code class="Ic" id="setenv">setenv</code></a>
     <var class="Ar">variable value</var></dt>
   <dd>Set the environment variable <var class="Ar">variable</var> to
       <var class="Ar">value</var>.</dd>
-  <dt id="stderr"><a class="permalink" href="#stderr"><code class="Ic">stderr</code></a>
+  <dt><a class="permalink" href="#stderr"><code class="Ic" id="stderr">stderr</code></a>
     [<var class="Ar">file</var>]</dt>
   <dd>Specify the expect standard error output (stderr). If
       <var class="Ar">file</var> is given, the output is compared with that
       file, otherwise the expected text is taken from the following lines of the
       test case, up to a line consisting of
     &#x201C;end-of-inline-data&#x201D;.</dd>
-  <dt id="stderr-replace"><a class="permalink" href="#stderr-replace"><code class="Ic">stderr-replace</code></a>
+  <dt><a class="permalink" href="#stderr-replace"><code class="Ic" id="stderr-replace">stderr-replace</code></a>
     <var class="Ar">pattern replacement</var></dt>
   <dd>Run regular expression replacement over the standard error output and the
       expected output as provided by <code class="Ic">stderr</code> before
       comparing them. <var class="Ar">pattern</var> is the match expression,
       <var class="Ar">replacement</var> is the replacement expression. In the
       replacement expression, &#x201C;$1&#x201D; to &#x201C;$9&#x201D; are
       replaced with the content of the corresponding &#x201C;(...)&#x201D; match
       in the <var class="Ar">pattern</var>. See
       <a class="Xr" href="http://pubs.opengroup.org/onlinepubs/9699919799/functions/re_format.html">re_format(7)</a> for details.</dd>
-  <dt id="stdin"><a class="permalink" href="#stdin"><code class="Ic">stdin</code></a>
+  <dt><a class="permalink" href="#stdin"><code class="Ic" id="stdin">stdin</code></a>
     [<var class="Ar">file</var>]</dt>
   <dd>If <var class="Ar">file</var> is given, standard input (stdin) is
       redirected from this file, which means the program has direct access to
       the file, including the ability to seek within it.
     <p class="Pp">Otherwise the text provided to the program via a pipe is taken
         from the test case, up to a line consisting of
         &#x201C;end-of-inline-data&#x201D;.</p>
   </dd>
-  <dt id="stdout"><a class="permalink" href="#stdout"><code class="Ic">stdout</code></a>
+  <dt><a class="permalink" href="#stdout"><code class="Ic" id="stdout">stdout</code></a>
     [<var class="Ar">file</var>]</dt>
   <dd>Specify the expect standard output (stdout). If <var class="Ar">file</var>
       is given, the output is compared with that file, otherwise the expected
       text is taken from the following lines of the test case, up to a line
       consisting of &#x201C;end-of-inline-data&#x201D;.</dd>
 </dl>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="SEE_ALSO"><a class="permalink" href="#SEE_ALSO">SEE
   ALSO</a></h1>
-<p class="Pp"><a class="Xr" href="nihtest.html">nihtest(1)</a>,
-    <a class="Xr" href="nihtest-config.html">nihtest-config(5)</a></p>
+<a class="Xr" href="nihtest.html">nihtest(1)</a>,
+  <a class="Xr" href="nihtest-config.html">nihtest-config(5)</a>
 </section>
 </div>
 <table class="foot">
   <tr>
-    <td class="foot-date">June 9, 2023</td>
+    <td class="foot-date">June 15, 2023</td>
     <td class="foot-os">NiH</td>
   </tr>
 </table>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
 
-
 NIHTEST-CASE(5) File Formats Manual NIHTEST-CASE(5)
 ****** NAME ******
-nihtest-case &#x2014; test case format for nihtest
+nihtest-case &#x2014;
+test case format for nihtest
 
 ****** DESCRIPTION ******
 nihtest(1) is a testing tool. It uses .test files as input. This man page
 describes the format of these test files.
 Lines beginning with &#x201C;#&#x201D; are comments.
 The following commands are recognized. The return and args commands must appear
 exactly once, the others are optional.
   arguments [argument ...]
       Run the program with command line arguments args. Shell style quoting is
       supported.
   description text
       Describes the purpose of the test.
   features feature ...
       Only run test if all features are present, otherwise skip it. The
-      features are extracted from a top-level config.h file. If the string
-      HAVE_FOO is defined in the file, the feature FOO is assumed to be
-      available, otherwise not. See also the description of top-build-directory
-      in nihtest-config(5).
+      features are extracted from a top-level config.h file. If the string FOO
+      is defined in the file, the feature FOO is assumed to be available,
+      otherwise not. See also the description of top-build-directory in
+      nihtest-config(5).
   file name in [out]
       The arguments in and out specify the contents of the file name in the
       test directory before and after the program is run, respectively. If out
       is omitted, the file is expected to remain unchanged.
       &#x201C;{}&#x201D; specifies that the file does not exist (i. e. that it
       is created or deleted by the program).
       For &#x201C;<inline>&#x201D; the contents of the file are taken from the
@@ -71,8 +71,8 @@
       Specify the expect standard output (stdout). If file is given, the output
       is compared with that file, otherwise the expected text is taken from the
       following lines of the test case, up to a line consisting of &#x201C;end-
       of-inline-data&#x201D;.
 
 ****** SEE_ALSO ******
 nihtest(1), nihtest-config(5)
-June 9, 2023 NiH
+June 15, 2023 NiH
```

### Comparing `nihtest-1.0.0/manpages/nihtest-case.man` & `nihtest-1.1.0/manpages/nihtest-case.man`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 .\" DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
 .\" GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 .\" INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 .\" IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 .\" OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 .\" IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 .\"
-.TH "NIHTEST-CASE" "5" "June 9, 2023" "NiH" "File Formats Manual"
+.TH "NIHTEST-CASE" "5" "June 15, 2023" "NiH" "File Formats Manual"
 .nh
 .if n .ad l
 .SH "NAME"
 \fBnihtest-case\fR
 \- test case format for nihtest
 .SH "DESCRIPTION"
 nihtest(1)
@@ -67,15 +67,15 @@
 Only run test if all
 \fIfeature\fRs
 are present, otherwise skip it.
 The features are extracted from a top-level
 \fIconfig.h\fR
 file.
 If the string
-\fRHAVE_FOO\fR
+\fRFOO\fR
 is defined in the file, the feature
 \fRFOO\fR
 is assumed to be available, otherwise not.
 See also the description of
 \fBtop-build-directory\fR
 in
 nihtest-config(5).
```

### Comparing `nihtest-1.0.0/manpages/nihtest-case.mdoc` & `nihtest-1.1.0/manpages/nihtest-case.mdoc`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 .\" DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
 .\" GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 .\" INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 .\" IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 .\" OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 .\" IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 .\"
-.Dd June 9, 2023
+.Dd June 15, 2023
 .Dt NIHTEST-CASE 5
 .Os
 .Sh NAME
 .Nm nihtest-case
 .Nd test case format for nihtest
 .Sh DESCRIPTION
 .Xr nihtest 1
@@ -56,23 +56,36 @@
 .Bl -tag -width 20n
 .It Ic arguments Op Ar argument ...
 Run the program with command line arguments
 .Ar args .
 Shell style quoting is supported.
 .It Ic description Ar text
 Describes the purpose of the test.
+.It Ic environment-clear
+Only variables explicitly set or passed through are included in the environment passed to the tested program.
+.It Ic environment-passthrough Ar variable ...
+Passes the named environment variables from the environment
+.Xr nihtest 1
+is run in to the tested program.
+.It Ic environment-set Ar variable value
+Set the environment variable
+.Ar variable
+to
+.Ar value .
+.It Ic environment-unset Ar variable ...
+Removes the named environment variables.
 .It Ic features Ar feature ...
 Only run test if all
 .Ar feature Ns No s
 are present, otherwise skip it.
 The features are extracted from a top-level
 .Pa config.h
 file.
 If the string
-.Dv HAVE_FOO
+.Dv FOO
 is defined in the file, the feature
 .Dv FOO
 is assumed to be available, otherwise not.
 See also the description of
 .Ic top-build-directory
 in
 .Xr nihtest-config 5 .
@@ -129,19 +142,14 @@
 .Ic default-program
 from
 .Pa nihtest.conf
 is run.
 .It Ic return Ar exit-code
 .Ar exit-code
 is the expected exit code (usually 0 on success).
-.It Ic setenv Ar variable value
-Set the environment variable
-.Ar variable
-to
-.Ar value .
 .It Ic stderr Op Ar file
 Specify the expect standard error output (stderr).
 If
 .Ar file
 is given, the output is compared with that file,
 otherwise the expected text is taken from the following lines of the test case, up to a line consisting of
 .Dq end-of-inline-data .
```

### Comparing `nihtest-1.0.0/manpages/nihtest.conf.html` & `nihtest-1.1.0/manpages/nihtest.conf.html`

 * *Files 4% similar despite different names*

```diff
@@ -30,143 +30,143 @@
    INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
    IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
    OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
    IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
    -->
 <head>
   <meta charset="utf-8"/>
-  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
   <link rel="stylesheet" href="../nih-man.css" type="text/css" media="all"/>
   <title>NIHTEST.CONF(5)</title>
 </head>
 <body>
 <table class="head">
   <tr>
     <td class="head-ltitle">NIHTEST.CONF(5)</td>
     <td class="head-vol">File Formats Manual</td>
     <td class="head-rtitle">NIHTEST.CONF(5)</td>
   </tr>
 </table>
 <div class="manual-text">
 <section class="Sh">
 <h1 class="Sh" id="NAME"><a class="permalink" href="#NAME">NAME</a></h1>
-<p class="Pp"><code class="Nm">nihtest.conf</code> &#x2014;
-    <span class="Nd">testing tool configuration file format</span></p>
+<code class="Nm">nihtest.conf</code> &#x2014;
+<div class="Nd">testing tool configuration file format</div>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="DESCRIPTION"><a class="permalink" href="#DESCRIPTION">DESCRIPTION</a></h1>
-<p class="Pp"><a class="Xr" href="nihtest.html">nihtest(1)</a> is a testing
-    tool. It reads a configuration file to get its default settings. The default
-    path for the file is <span class="Pa">nihtest.conf</span> in the current
-    directory; this can be overridden with
-    <a class="Xr" href="nihtest.html">nihtest(1)</a>'s
-    <code class="Fl">-C</code> flag. This man page describes the format of this
-    configuration file.</p>
+<a class="Xr" href="nihtest.html">nihtest(1)</a> is a testing tool. It reads a
+  configuration file to get its default settings. The default path for the file
+  is <span class="Pa">nihtest.conf</span> in the current directory; this can be
+  overridden with <a class="Xr" href="nihtest.html">nihtest(1)</a>'s
+  <code class="Fl">-C</code> flag. This man page describes the format of this
+  configuration file.
 </section>
 <section class="Sh">
 <h1 class="Sh" id="FILE_FORMAT"><a class="permalink" href="#FILE_FORMAT">FILE
   FORMAT</a></h1>
-<p class="Pp">The configuration file consists of multiple sections, which are
-    started with [<var class="Ar">section-name</var>]. The supported sections
-    are <code class="Ic">settings</code>, <code class="Ic">setenv</code>, and
-    <code class="Ic">comparators</code>.</p>
+The configuration file consists of multiple sections, which are started with
+  [<var class="Ar">section-name</var>]. The supported sections are
+  <code class="Ic">settings</code>, <code class="Ic">setenv</code>, and
+  <code class="Ic">comparators</code>.
 <p class="Pp">Each section consists of variable assignments in the format
     <var class="Ar">name =</var> <var class="Ar">value</var>, one per line.</p>
 <p class="Pp">Multiple values for the same variable can be specified, one per
     line, where subsequent lines must be indented with spaces.</p>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="SETTINGS"><a class="permalink" href="#SETTINGS">SETTINGS</a></h1>
-<p class="Pp">In the <code class="Ic">settings</code> section, the following
-    variables are recognized:</p>
+In the <code class="Ic">settings</code> section, the following variables are
+  recognized:
 <dl class="Bl-tag">
-  <dt id="default-program"><a class="permalink" href="#default-program"><code class="Ic">default-program
+  <dt><a class="permalink" href="#default-program_="><code class="Ic" id="default-program_=">default-program
     =</code></a> <var class="Ar">program</var></dt>
   <dd>Test <var class="Ar">program</var> if no <code class="Ic">program</code>
       directive is found in the test.</dd>
-  <dt id="default-stderr-replace"><a class="permalink" href="#default-stderr-replace"><code class="Ic">default-stderr-replace
+  <dt><a class="permalink" href="#default-stderr-replace_="><code class="Ic" id="default-stderr-replace_=">default-stderr-replace
     =</code></a> <var class="Ar">pattern replacement ...</var></dt>
   <dd>Each line consists of two values, <var class="Ar">pattern</var> is a
       regular expression and <var class="Ar">replacement</var> the corresponding
       replacement string. These are used for test cases without
       <code class="Ic">stderr-replace</code> directives. See
       <a class="Xr" href="nihtest-case.html">nihtest-case(5)</a> for details on
       <code class="Ic">stderr-replace</code>.</dd>
-  <dt id="features-files"><a class="permalink" href="#features-files"><code class="Ic">features-files
+  <dt><a class="permalink" href="#features-files_="><code class="Ic" id="features-files_=">features-files
     =</code></a> <var class="Ar">file ...</var></dt>
   <dd>Specifies the files to search for feature defines. This is used in the
       <code class="Ic">features</code> directive in test cases.</dd>
-  <dt id="keep-sandbox"><a class="permalink" href="#keep-sandbox"><code class="Ic">keep-sandbox
+  <dt><a class="permalink" href="#keep-sandbox_="><code class="Ic" id="keep-sandbox_=">keep-sandbox
     =</code></a> <var class="Ar">when</var></dt>
   <dd>Describe when to keep the sandbox (i.e., not delete it) after running the
       test. The following values are supported:
     <div class="Bd-indent">
     <dl class="Bl-tag Bl-compact">
-      <dt id="never"><a class="permalink" href="#never"><code class="Dv">never</code></a></dt>
+      <dt><a class="permalink" href="#never"><code class="Dv" id="never">never</code></a></dt>
       <dd>Never keep the sandbox.</dd>
-      <dt id="failed"><a class="permalink" href="#failed"><code class="Dv">failed</code></a></dt>
+      <dt><a class="permalink" href="#failed"><code class="Dv" id="failed">failed</code></a></dt>
       <dd>Keep the sandbox when the test failed.</dd>
-      <dt id="always"><a class="permalink" href="#always"><code class="Dv">always</code></a></dt>
+      <dt><a class="permalink" href="#always"><code class="Dv" id="always">always</code></a></dt>
       <dd>Always keep the sandbox.</dd>
     </dl>
     </div>
     This can be overridden with the
       <a class="Xr" href="nihtest.html">nihtest(1)</a> flags
-      <code class="Fl">--keep-broken</code> <code class="Fl">-=</code>
-      <var class="Ar">when</var> or <code class="Fl">--no-cleanup</code>. The
-      default is <code class="Dv">never</code>.</dd>
-  <dt id="print-results"><a class="permalink" href="#print-results"><code class="Ic">print-results
+      <code class="Fl">-</code> <code class="Fl">-keep-broken</code>
+      <code class="Fl">-=</code> <var class="Ar">when</var> or
+      <code class="Fl">-</code><code class="Fl">-no-cleanup</code>. The default
+      is <code class="Dv">never</code>.</dd>
+  <dt><a class="permalink" href="#print-results_="><code class="Ic" id="print-results_=">print-results
     =</code></a> <var class="Ar">when</var></dt>
   <dd>Describe when to print the test results verbosely. The following values
       are supported:
     <div class="Bd-indent">
     <dl class="Bl-tag Bl-compact">
-      <dt id="never~2"><a class="permalink" href="#never~2"><code class="Dv">never</code></a></dt>
+      <dt><a class="permalink" href="#never_2"><code class="Dv" id="never_2">never</code></a></dt>
       <dd>Quiet mode.</dd>
-      <dt id="failed~2"><a class="permalink" href="#failed~2"><code class="Dv">failed</code></a></dt>
+      <dt><a class="permalink" href="#failed_2"><code class="Dv" id="failed_2">failed</code></a></dt>
       <dd>Print details when the test failed.</dd>
-      <dt id="always~2"><a class="permalink" href="#always~2"><code class="Dv">always</code></a></dt>
+      <dt><a class="permalink" href="#always_2"><code class="Dv" id="always_2">always</code></a></dt>
       <dd>Verbose mode.</dd>
     </dl>
     </div>
     This can be overridden with the
       <a class="Xr" href="nihtest.html">nihtest(1)</a> flags
-      <code class="Fl">--quiet</code> or <code class="Fl">--verbose</code>. The
-      default is <code class="Dv">failed</code>.</dd>
-  <dt id="program-directories"><a class="permalink" href="#program-directories"><code class="Ic">program-directories
+      <code class="Fl">-</code> <code class="Fl">-quiet</code> or
+      <code class="Fl">-</code><code class="Fl">-verbose</code>. The default is
+      <code class="Dv">failed</code>.</dd>
+  <dt><a class="permalink" href="#program-directories_="><code class="Ic" id="program-directories_=">program-directories
     =</code></a> <var class="Ar">directory ...</var></dt>
   <dd>Specifies the directories programs are searched for. They are prepended to
       <code class="Ev">PATH</code>.</dd>
-  <dt id="sandbox-directories"><a class="permalink" href="#sandbox-directories"><code class="Ic">sandbox-directories
+  <dt><a class="permalink" href="#sandbox-directories_="><code class="Ic" id="sandbox-directories_=">sandbox-directories
     =</code></a> <var class="Ar">directory ...</var></dt>
   <dd>Create sandboxes in <var class="Ar">directory</var>. By default, the
       sandboxes will be created in the current directory. A random directory of
       the pattern <span class="Pa">sandbox_*</span> will be used.</dd>
-  <dt id="test-input-directories"><a class="permalink" href="#test-input-directories"><code class="Ic">test-input-directories
+  <dt><a class="permalink" href="#test-input-directories_="><code class="Ic" id="test-input-directories_=">test-input-directories
     =</code></a> <var class="Ar">directory ...</var></dt>
   <dd><a class="Xr" href="nihtest.html">nihtest(1)</a> searches the current
       directory and <var class="Ar">directory</var> for test cases, input and
       output files.</dd>
 </dl>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="SETENV"><a class="permalink" href="#SETENV">SETENV</a></h1>
-<p class="Pp">The <code class="Ic">setenv</code> section contains variable and
-    values that will be added as environment variables when the test program is
-    run. If the test case contains a <code class="Ic">setenv</code> directive,
-    this section will be ignored.</p>
+The <code class="Ic">setenv</code> section contains variable and values that
+  will be added as environment variables when the test program is run. If the
+  test case contains a <code class="Ic">setenv</code> directive, this section
+  will be ignored.
 </section>
 <section class="Sh">
 <h1 class="Sh" id="COMPARATORS"><a class="permalink" href="#COMPARATORS">COMPARATORS</a></h1>
-<p class="Pp">The <code class="Ic">comparators</code> section specifies programs
-    to use to compare files of certain types. The variable names have the format
-    <var class="Ar">got-extension</var>.
-    <var class="Ar">expected-extension</var>, the value specifies the command
-    line to use to compare these files. The command will be run with the two
-    files as arguments, the file in the sandbox first and the expected last.</p>
+The <code class="Ic">comparators</code> section specifies programs to use to
+  compare files of certain types. The variable names have the format
+  <var class="Ar">got-extension</var>. <var class="Ar">expected-extension</var>,
+  the value specifies the command line to use to compare these files. The
+  command will be run with the two files as arguments, the file in the sandbox
+  first and the expected last.
 <p class="Pp">The command is expected to exit with code 0 if the two files are
     considered equal, any other exit code if not. The command output will be
     displayed if verbose test results are enabled (see
     <code class="Ic">print-results</code> above).</p>
 <p class="Pp">For example, with comparators containing</p>
 <div class="Bd Bd-indent"><code class="Li">zip.zip = zipcmp -v</code></div>
 and the test case containing
@@ -175,32 +175,34 @@
 the command
 <div class="Bd Bd-indent"><code class="Li">zipcmp -v got.zip
   expected.zip</code></div>
 will be run to compare the files.
 </section>
 <section class="Sh">
 <h1 class="Sh" id="EXAMPLES"><a class="permalink" href="#EXAMPLES">EXAMPLES</a></h1>
-<div class="Bd Li">
-<pre>[settings]
+<div class="Bd">
+<pre>
+[settings]
 default-program = program_to_test
 program-directories = bin
     tests
-[environment]
+[setenv]
 LC_ALL=en_US.UTF-8
 [comparators]
-zip.zip = zipcmp -v</pre>
+zip.zip = zipcmp -v
+</pre>
 </div>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="SEE_ALSO"><a class="permalink" href="#SEE_ALSO">SEE
   ALSO</a></h1>
-<p class="Pp"><a class="Xr" href="nihtest.html">nihtest(1)</a></p>
+<a class="Xr" href="nihtest.html">nihtest(1)</a>
 </section>
 </div>
 <table class="foot">
   <tr>
-    <td class="foot-date">June 9, 2023</td>
+    <td class="foot-date">June 15, 2023</td>
     <td class="foot-os">NiH</td>
   </tr>
 </table>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
 
-
 NIHTEST.CONF(5) File Formats Manual NIHTEST.CONF(5)
 ****** NAME ******
-nihtest.conf &#x2014; testing tool configuration file format
+nihtest.conf &#x2014;
+testing tool configuration file format
 
 ****** DESCRIPTION ******
 nihtest(1) is a testing tool. It reads a configuration file to get its default
 settings. The default path for the file is nihtest.conf in the current
 directory; this can be overridden with nihtest(1)'s -C flag. This man page
 describes the format of this configuration file.
-
 ****** FILE_FORMAT ******
 The configuration file consists of multiple sections, which are started with
 [section-name]. The supported sections are settings, setenv, and comparators.
 Each section consists of variable assignments in the format name = value, one
 per line.
 Multiple values for the same variable can be specified, one per line, where
 subsequent lines must be indented with spaces.
@@ -35,26 +34,26 @@
       test. The following values are supported:
         never
             Never keep the sandbox.
         failed
             Keep the sandbox when the test failed.
         always
             Always keep the sandbox.
-      This can be overridden with the nihtest(1) flags --keep-broken -= when or
-      --no-cleanup. The default is never.
+      This can be overridden with the nihtest(1) flags - -keep-broken -= when
+      or --no-cleanup. The default is never.
   print-results_= when
       Describe when to print the test results verbosely. The following values
       are supported:
         never
             Quiet mode.
         failed
             Print details when the test failed.
         always
             Verbose mode.
-      This can be overridden with the nihtest(1) flags --quiet or --verbose.
+      This can be overridden with the nihtest(1) flags - -quiet or --verbose.
       The default is failed.
   program-directories_= directory ...
       Specifies the directories programs are searched for. They are prepended
       to PATH.
   sandbox-directories_= directory ...
       Create sandboxes in directory. By default, the sandboxes will be created
       in the current directory. A random directory of the pattern sandbox_*
@@ -63,15 +62,14 @@
       nihtest(1) searches the current directory and directory for test cases,
       input and output files.
 
 ****** SETENV ******
 The setenv section contains variable and values that will be added as
 environment variables when the test program is run. If the test case contains a
 setenv directive, this section will be ignored.
-
 ****** COMPARATORS ******
 The comparators section specifies programs to use to compare files of certain
 types. The variable names have the format got-extension. expected-extension,
 the value specifies the command line to use to compare these files. The command
 will be run with the two files as arguments, the file in the sandbox first and
 the expected last.
 The command is expected to exit with code 0 if the two files are considered
@@ -85,15 +83,15 @@
 zipcmp -v got.zip expected.zip
 will be run to compare the files.
 ****** EXAMPLES ******
 [settings]
 default-program = program_to_test
 program-directories = bin
     tests
-[environment]
+[setenv]
 LC_ALL=en_US.UTF-8
 [comparators]
 zip.zip = zipcmp -v
 
 ****** SEE_ALSO ******
 nihtest(1)
-June 9, 2023 NiH
+June 15, 2023 NiH
```

### Comparing `nihtest-1.0.0/manpages/nihtest.conf.man` & `nihtest-1.1.0/manpages/nihtest.conf.man`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 .\" DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
 .\" GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 .\" INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 .\" IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 .\" OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 .\" IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 .\"
-.TH "NIHTEST.CONF" "5" "June 9, 2023" "NiH" "File Formats Manual"
+.TH "NIHTEST.CONF" "5" "June 15, 2023" "NiH" "File Formats Manual"
 .nh
 .if n .ad l
 .SH "NAME"
 \fBnihtest.conf\fR
 \- testing tool configuration file format
 .SH "DESCRIPTION"
 nihtest(1)
@@ -108,16 +108,18 @@
 .TP 8n
 \fRalways\fR
 Always keep the sandbox.
 .RE
 .RS 22n
 This can be overridden with the
 nihtest(1)
-flags \fB\-\-keep-broken\fR \fB\-=\fR \fIwhen\fR
-or \fB\-\-no-cleanup\fR.
+flags
+\fB\-\fR\fB\-keep-broken\fR \fB\-=\fR \fIwhen\fR
+or
+\fB\-\fR\fB\-no-cleanup\fR.
 The default is
 \fRnever\fR.
 .RE
 .PD
 .TP 22n
 \fBprint-results =\fR \fIwhen\fR
 Describe when to print the test results verbosely.
@@ -133,16 +135,18 @@
 .TP 8n
 \fRalways\fR
 Verbose mode.
 .RE
 .RS 22n
 This can be overridden with the
 nihtest(1)
-flags \fB\-\-quiet\fR
-or \fB\-\-verbose\fR.
+flags
+\fB\-\fR\fB\-quiet\fR
+or
+\fB\-\fR\fB\-verbose\fR.
 The default is
 \fRfailed\fR.
 .RE
 .PD
 .TP 22n
 \fBprogram-directories =\fR \fIdirectory ...\fR
 Specifies the directories programs are searched for.
@@ -199,15 +203,15 @@
 .SH "EXAMPLES"
 .nf
 .RS 0n
 [settings]
 default-program = program_to_test
 program-directories = bin
     tests
-[environment]
+[setenv]
 LC_ALL=en_US.UTF-8
 [comparators]
 zip.zip = zipcmp -v
 .RE
 .fi
 .SH "SEE ALSO"
 nihtest(1)
```

### Comparing `nihtest-1.0.0/manpages/nihtest.conf.mdoc` & `nihtest-1.1.0/manpages/nihtest.conf.mdoc`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 .\" DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
 .\" GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 .\" INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 .\" IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
 .\" OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
 .\" IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 .\"
-.Dd June 9, 2023
+.Dd June 15, 2023
 .Dt NIHTEST.CONF 5
 .Os
 .Sh NAME
 .Nm nihtest.conf
 .Nd testing tool configuration file format
 .Sh DESCRIPTION
 .Xr nihtest 1
@@ -81,14 +81,26 @@
 These are used for test cases without
 .Ic stderr-replace
 directives.
 See
 .Xr nihtest-case 5
 for details on
 .Ic stderr-replace .
+.It Ic environment-clear = true
+If
+.Ic environment-clear
+is set to
+.Dv true ,
+only variables explicitly set or passed through are included in the environment passed to the tested program.
+.It Ic environment-passthrough = Ar variable ...
+The named environment variables are passed through from the environment
+.Xr nihtest 1
+is run in to the environment passed to the tested program.
+.It Ic environment-unset = Ar variable ...
+The named environment variables are removed from the environment passed to the tested program.
 .It Ic features-files = Ar file ...
 Specifies the files to search for feature defines.
 This is used in the
 .Ic features
 directive in test cases.
 .It Ic keep-sandbox = Ar when
 Describe when to keep the sandbox (i.e., not delete it) after running the test.
@@ -141,21 +153,18 @@
 will be used.
 .It Ic test-input-directories = Ar directory ...
 .Xr nihtest 1
 searches the current directory and
 .Ar directory
 for test cases, input and output files.
 .El
-.Sh SETENV
+.Sh ENVIRONMENT
 The
-.Ic setenv
+.Ic environment
 section contains variable and values that will be added as environment variables when the test program is run.
-If the test case contains a
-.Ic setenv
-directive, this section will be ignored.
 .Sh COMPARATORS
 The
 .Ic comparators
 section specifies programs to use to compare files of certain types.
 The variable names have the format
 .Ar got-extension . expected-extension ,
 the value specifies the command line to use to compare these files.
```

### Comparing `nihtest-1.0.0/manpages/nihtest.html` & `nihtest-1.1.0/manpages/nihtest.html`

 * *Files 13% similar despite different names*

```diff
@@ -30,84 +30,85 @@
    INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
    IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
    OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN
    IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
    -->
 <head>
   <meta charset="utf-8"/>
-  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
   <link rel="stylesheet" href="../nih-man.css" type="text/css" media="all"/>
   <title>NIHTEST(1)</title>
 </head>
 <body>
 <table class="head">
   <tr>
     <td class="head-ltitle">NIHTEST(1)</td>
     <td class="head-vol">General Commands Manual</td>
     <td class="head-rtitle">NIHTEST(1)</td>
   </tr>
 </table>
 <div class="manual-text">
 <section class="Sh">
 <h1 class="Sh" id="NAME"><a class="permalink" href="#NAME">NAME</a></h1>
-<p class="Pp"><code class="Nm">nihtest</code> &#x2014; <span class="Nd">testing
-    tool</span></p>
+<code class="Nm">nihtest</code> &#x2014;
+<div class="Nd">testing tool</div>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="SYNOPSIS"><a class="permalink" href="#SYNOPSIS">SYNOPSIS</a></h1>
 <table class="Nm">
   <tr>
     <td><code class="Nm">nihtest</code></td>
     <td>[<code class="Fl">-hqVv</code>] [<code class="Fl">-C</code>
-      <var class="Ar">config</var>] [<code class="Fl">--keep-broken</code>]
-      [<code class="Fl">--no-cleanup</code>]
-      [<code class="Fl">--setup-only</code>] <var class="Ar">testcase</var></td>
+      <var class="Ar">config</var>]
+      [<code class="Fl">-</code><code class="Fl">-keep-broken</code>]
+      [<code class="Fl">-</code><code class="Fl">-no-cleanup</code>]
+      [<code class="Fl">-</code><code class="Fl">-setup-only</code>]
+      <var class="Ar">testcase</var></td>
   </tr>
 </table>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="DESCRIPTION"><a class="permalink" href="#DESCRIPTION">DESCRIPTION</a></h1>
-<p class="Pp"><code class="Nm">nihtest</code> is a testing tool for command line
-    utilities. It uses <span class="Pa">.test</span> files as input. The format
-    of these files is described in
-    <a class="Xr" href="nihtest-case.html">nihtest-case(5)</a>.</p>
+<code class="Nm">nihtest</code> is a testing tool for command line utilities. It
+  uses <span class="Pa">.test</span> files as input. The format of these files
+  is described in <a class="Xr" href="nihtest-case.html">nihtest-case(5)</a>.
 <p class="Pp"><code class="Nm">nihtest</code> runs the test case
     <var class="Ar">testcase</var> expected in the test case directory (see
     <a class="Xr" href="nihtest.conf.html">nihtest.conf(5)</a>) in the file
     <span class="Pa">testcase</span> or <span class="Pa">testcase.test</span>.
     <code class="Nm">nihtest</code> searches the current directory and the
     <code class="Ic">source-directory</code> specified in
     <a class="Xr" href="nihtest.conf.html">nihtest.conf(5)</a> for test cases,
     input and output files.</p>
 <p class="Pp"><code class="Nm">nihtest</code> supports the following options</p>
 <div class="Bd-indent">
 <dl class="Bl-tag">
-  <dt id="C"><a class="permalink" href="#C"><code class="Fl">-C</code></a>
-    <var class="Ar">config</var>, <code class="Fl">--config-file</code>
+  <dt><a class="permalink" href="#C"><code class="Fl" id="C">-C</code></a>
+    <var class="Ar">config</var>,
+    <code class="Fl">-</code><code class="Fl">-config-file</code>
     <var class="Ar">config</var></dt>
   <dd>Use <var class="Ar">config</var> as configuration file instead of
       <span class="Pa">./nihtest.conf</span>.</dd>
-  <dt id="h"><a class="permalink" href="#h"><code class="Fl">-h</code></a>,
-    <code class="Fl">--help</code></dt>
+  <dt><a class="permalink" href="#h"><code class="Fl" id="h">-h</code></a>,
+    <code class="Fl">-</code><code class="Fl">-help</code></dt>
   <dd>Display a short help message and exit.</dd>
-  <dt id="keep-broken"><a class="permalink" href="#keep-broken"><code class="Fl">--keep-broken</code></a></dt>
+  <dt><code class="Fl">-</code><code class="Fl">-keep-broken</code></dt>
   <dd>Do not delete the sandbox if the test fails.</dd>
-  <dt id="no-cleanup"><a class="permalink" href="#no-cleanup"><code class="Fl">--no-cleanup</code></a></dt>
+  <dt><code class="Fl">-</code><code class="Fl">-no-cleanup</code></dt>
   <dd>Do not delete the sandbox after the test finishes (successfully or
     not).</dd>
-  <dt id="q"><a class="permalink" href="#q"><code class="Fl">-q</code></a>,
-    <code class="Fl">--quiet</code></dt>
+  <dt><a class="permalink" href="#q"><code class="Fl" id="q">-q</code></a>,
+    <code class="Fl">-</code><code class="Fl">-quiet</code></dt>
   <dd>Do not print test results.</dd>
-  <dt id="setup-only"><a class="permalink" href="#setup-only"><code class="Fl">--setup-only</code></a></dt>
+  <dt><code class="Fl">-</code><code class="Fl">-setup-only</code></dt>
   <dd>Only populate the sandbox, but do not run the actual test.</dd>
-  <dt id="v"><a class="permalink" href="#v"><code class="Fl">-v</code></a>,
-    <code class="Fl">--verbose</code></dt>
+  <dt><a class="permalink" href="#v"><code class="Fl" id="v">-v</code></a>,
+    <code class="Fl">-</code><code class="Fl">-verbose</code></dt>
   <dd>Print detailed test results.</dd>
-  <dt id="V"><a class="permalink" href="#V"><code class="Fl">-V</code></a>,
-    <code class="Fl">--version</code></dt>
+  <dt><a class="permalink" href="#V"><code class="Fl" id="V">-V</code></a>,
+    <code class="Fl">-</code><code class="Fl">-version</code></dt>
   <dd>Print <code class="Nm">nihtest</code> version number and exit.</dd>
 </dl>
 </div>
 <p class="Pp">A test run consists of the following steps:</p>
 <ul class="Bl-bullet Bd-indent Bl-compact">
   <li>check if test should be skipped</li>
   <li>create sandbox directory</li>
@@ -125,15 +126,15 @@
       <a class="Xr" href="nihtest.conf.html">nihtest.conf(5)</a> for
     details</dd>
 </dl>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="EXIT_STATUS"><a class="permalink" href="#EXIT_STATUS">EXIT
   STATUS</a></h1>
-<p class="Pp"><code class="Nm">nihtest</code> uses the following exit codes:</p>
+<code class="Nm">nihtest</code> uses the following exit codes:
 <div class="Bd-indent">
 <dl class="Bl-tag Bl-compact">
   <dt>0</dt>
   <dd>Test passed</dd>
   <dt>1</dt>
   <dd>Test failed</dd>
   <dt>2</dt>
@@ -141,31 +142,31 @@
   <dt>77</dt>
   <dd>Test was skipped.</dd>
 </dl>
 </div>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="DIAGNOSTICS"><a class="permalink" href="#DIAGNOSTICS">DIAGNOSTICS</a></h1>
-<p class="Pp">In general, differences to the test case expectation are marked up
-    with &#x201C;-&#x201D; if something expected did not happen and
-    &#x201C;+&#x201D; if something unexpected happened.</p>
+In general, differences to the test case expectation are marked up with
+  &#x201C;-&#x201D; if something expected did not happen and &#x201C;+&#x201D;
+  if something unexpected happened.
 <p class="Pp">In case the return value does not match,
     <code class="Nm">nihtest</code> will report &#x201C;Exit code not as
     expected&#x201D;. If the standard output or standard error output are not
     correct, <code class="Nm">nihtest</code> will report &#x201C;Output not as
     expected&#x201D; or &#x201C;Error output not as expected&#x201D;
     respectively. And finally, if the file contents of the sandbox are not
     correct, <code class="Nm">nihtest</code> will report &#x201C;Files in
     sandbox not as expected&#x201D;.</p>
 </section>
 <section class="Sh">
 <h1 class="Sh" id="SEE_ALSO"><a class="permalink" href="#SEE_ALSO">SEE
   ALSO</a></h1>
-<p class="Pp"><a class="Xr" href="nihtest-case.html">nihtest-case(5)</a>,
-    <a class="Xr" href="nihtest.conf.html">nihtest.conf(5)</a></p>
+<a class="Xr" href="nihtest-case.html">nihtest-case(5)</a>,
+  <a class="Xr" href="nihtest.conf.html">nihtest.conf(5)</a>
 </section>
 </div>
 <table class="foot">
   <tr>
     <td class="foot-date">June 9, 2023</td>
     <td class="foot-os">NiH</td>
   </tr>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 
-
 NIHTEST(1) General Commands Manual NIHTEST(1)
 ****** NAME ******
-nihtest &#x2014; testing tool
+nihtest &#x2014;
+testing tool
 
 ****** SYNOPSIS ******
 nihtest [-hqVv] [-C config] [--keep-broken] [--no-cleanup] [--setup-only]
         testcase
 
 ****** DESCRIPTION ******
 nihtest is a testing tool for command line utilities. It uses .test files as
```

### Comparing `nihtest-1.0.0/manpages/nihtest.man` & `nihtest-1.1.0/manpages/nihtest.man`

 * *Files 8% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 \fBnihtest\fR
 \- testing tool
 .SH "SYNOPSIS"
 .HP 8n
 \fBnihtest\fR
 [\fB\-hqVv\fR]
 [\fB\-C\fR\ \fIconfig\fR]
-[\fB\-\-keep-broken\fR]
-[\fB\-\-no-cleanup\fR]
-[\fB\-\-setup-only\fR]
+[\fB\-\fR\fB\-keep-broken\fR]
+[\fB\-\fR\fB\-no-cleanup\fR]
+[\fB\-\fR\fB\-setup-only\fR]
 \fItestcase\fR
 .SH "DESCRIPTION"
 \fBnihtest\fR
 is a testing tool for command line utilities.
 It uses
 \fI.test\fR
 files as input.
@@ -70,40 +70,40 @@
 nihtest.conf(5)
 for test cases, input and output files.
 .PP
 \fBnihtest\fR
 supports the following options
 .RS 8n
 .TP 17n
-\fB\-C\fR \fIconfig\fR, \fB\-\-config-file\fR \fIconfig\fR
+\fB\-C\fR \fIconfig\fR, \fB\-\fR\fB\-config-file\fR \fIconfig\fR
 Use
 \fIconfig\fR
 as configuration file instead of
 \fI./nihtest.conf\fR.
 .TP 17n
-\fB\-h\fR, \fB\-\-help\fR
+\fB\-h\fR, \fB\-\fR\fB\-help\fR
 Display a short help message and exit.
 .TP 17n
-\fB\-\-keep-broken\fR
+\fB\-\fR\fB\-keep-broken\fR
 Do not delete the sandbox if the test fails.
 .TP 17n
-\fB\-\-no-cleanup\fR
+\fB\-\fR\fB\-no-cleanup\fR
 Do not delete the sandbox after the test finishes (successfully or not).
 .TP 17n
-\fB\-q\fR, \fB\-\-quiet\fR
+\fB\-q\fR, \fB\-\fR\fB\-quiet\fR
 Do not print test results.
 .TP 17n
-\fB\-\-setup-only\fR
+\fB\-\fR\fB\-setup-only\fR
 Only populate the sandbox, but do not run the actual test.
 .TP 17n
-\fB\-v\fR, \fB\-\-verbose\fR
+\fB\-v\fR, \fB\-\fR\fB\-verbose\fR
 .br
 Print detailed test results.
 .TP 17n
-\fB\-V\fR, \fB\-\-version\fR
+\fB\-V\fR, \fB\-\fR\fB\-version\fR
 .br
 Print
 \fBnihtest\fR
 version number and exit.
 .RE
 .PP
 A test run consists of the following steps:
```

### Comparing `nihtest-1.0.0/manpages/nihtest.mdoc` & `nihtest-1.1.0/manpages/nihtest.mdoc`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/nihtest/Command.py` & `nihtest-1.1.0/nihtest/Command.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,19 +20,15 @@
         self.stderr = None
         self.exit_code = None
 
     def run(self):
         program = self.program if os.path.exists(self.program) else shutil.which(self.program)
         if program is None:
             raise RuntimeError(f"can't find program {self.program}")
-        if self.environment:
-            environment = os.environ | self.environment
-        else:
-            environment = None
         if self.stdin_file is not None:
             with open(self.stdin_file, "rb") as stdin:
-                result = subprocess.run([program] + self.arguments, capture_output=True, check=False, text=True, stdin=stdin, env=environment)
+                result = subprocess.run([program] + self.arguments, capture_output=True, check=False, text=True, stdin=stdin, env=self.environment)
         else:
-            result = subprocess.run([program] + self.arguments, capture_output=True, check=False, text=True, input=self.stdin, env=environment)
+            result = subprocess.run([program] + self.arguments, capture_output=True, check=False, text=True, input=self.stdin, env=self.environment)
         self.exit_code = result.returncode
         self.stdout = result.stdout.splitlines()
         self.stderr = result.stderr.splitlines()
```

### Comparing `nihtest-1.0.0/nihtest/CompareArrays.py` & `nihtest-1.1.0/nihtest/CompareArrays.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/nihtest/Features.py` & `nihtest-1.1.0/nihtest/Features.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/nihtest/File.py` & `nihtest-1.1.0/nihtest/File.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import pathlib
 import shutil
 
 from nihtest import Command
+from nihtest import Environment
 from nihtest import Configuration
 from nihtest import Utility
 
 
 class Data:
     def __init__(self, file_name=None, data=None):
         if (file_name is not None and data is not None) or (file_name is None and data is None):
@@ -32,15 +33,15 @@
             output_file_name = configuration.find_input_file(self.result.file_name)
             file_extension = pathlib.Path(self.name).suffix[1:]
             output_extension = pathlib.Path(self.result.file_name).suffix[1:]
             key = f"{file_extension}.{output_extension}"
             if key in configuration.comparators:
                 comparator = configuration.comparators[key]
                 arguments = comparator[1:] + [input_file_name, output_file_name]
-                command = Command.Command(configuration.find_program(comparator[0]), arguments)
+                command = Command.Command(configuration.find_program(comparator[0]), arguments, environment=Environment.Environment(configuration).environment)
                 command.run()
                 if command.exit_code != 0:
                     print(f"{self.name} differs:")
                     print("\n".join(command.stdout))
                 return command.exit_code == 0
             try:
                 output_data = Utility.read_lines(output_file_name)
```

### Comparing `nihtest-1.0.0/nihtest/Sandbox.py` & `nihtest-1.1.0/nihtest/Sandbox.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/nihtest/Test.py` & `nihtest-1.1.0/nihtest/Test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import enum
 import os
 import platform
 import re
 
 from nihtest import Command
 from nihtest import Configuration
+from nihtest import Environment
 from nihtest import Features
 from nihtest import TestCase
 from nihtest import Sandbox
 from nihtest import Utility
 
 
 def process_stderr_line(line, replacements):
@@ -53,21 +54,15 @@
             file.prepare(self.case.configuration, self.sandbox.directory)
 
         if not self.case.configuration.run_test:
             return TestResult.OK
 
         self.sandbox.enter()
         program = self.case.configuration.find_program(self.case.program)
-        environment = {
-            "TZ": "UTC",
-            "LANG": "C",
-            "LC_CTYPE": "C",
-            "POSIXLY_CORRECT": "1"
-        }
-        environment.update(self.case.environment)
+        environment = Environment.Environment(self.case).environment
         if self.case.preload:
             environment["LD_PRELOAD"] = " ".join(map(lambda file: self.case.configuration.find_program("lib" + file), self.case.preload))
         command = Command.Command(program, self.case.arguments, self.case.stdin, environment=environment)
         command.run()
         files_got = self.list_files()
         self.sandbox.leave()
```

### Comparing `nihtest-1.0.0/nihtest/TestCase.py` & `nihtest-1.1.0/nihtest/TestCase.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import re
 import shlex
 import sys
 
 from nihtest import File
 from nihtest import Utility
 
+
 def decode_escapes(string):
     return string.replace("\\n", "\n").replace("\\r", "\r").replace("\\t", "\t").replace("\\\\", "\\")
 
+
 class Directive:
     def __init__(self, usage, method, minimum_arguments, maximum_arguments=None, only_once=False):
         self.usage = usage
         self.method = method
         self.minimum_arguments = minimum_arguments
         if maximum_arguments:
             self.maximum_arguments = maximum_arguments
@@ -24,14 +26,17 @@
     def __init__(self, configuration, args):
         self.name = args.testcase
         if self.name[-5:] == ".test":
             self.name = self.name[:-5]
         self.args = args
         self.configuration = configuration
         self.environment = configuration.environment.copy()
+        self.environment_clear = configuration.environment_clear
+        self.environment_passthrough = configuration.environment_passthrough.copy()
+        self.environment_unset = configuration.environment_unset.copy()
         file_name = args.testcase
         if file_name[-5:] != ".test":
             file_name += ".test"
         self.file_name = self.configuration.find_input_file(file_name)
         self.file = open(self.file_name, mode="r")
         self.line_number = 0
         self.directives_seen = {}
@@ -119,14 +124,26 @@
 
     def directive_arguments(self, arguments):
         self.arguments = arguments
 
     def directive_description(self, text):
         self.description = text
 
+    def directive_environment_clear(self, _arguments):
+        self.environment_clear = True
+
+    def directive_environment_passthrough(self, arguments):
+        self.environment_passthrough += arguments
+
+    def directive_environment_set(self, arguments):
+        self.environment[arguments[0]] = arguments[1]
+
+    def directive_environment_unset(self, arguments):
+        self.environment_unset += arguments
+
     def directive_features(self, arguments):
         self.features = arguments
 
     def directive_file(self, arguments):
         input_source = self.file_data(arguments[1])
         if len(arguments) > 2:
             result = self.file_data(arguments[2])
@@ -145,17 +162,14 @@
 
     def directive_program(self, arguments):
         self.program = arguments[0]
 
     def directive_return(self, arguments):
         self.exit_code = int(arguments[0])  # TODO: error check?
 
-    def directive_setenv(self, arguments):
-        self.environment[arguments[0]] = arguments[1]
-
     def directive_stderr(self, arguments):
         self.stderr = self.io_data(arguments)
 
     def directive_stderr_replace(self, arguments):
         self.stderr_replace.append((re.compile(arguments[0]), arguments[1]))
 
     def directive_stdin(self, arguments):
@@ -170,14 +184,26 @@
     directives = {
         "arguments": Directive(method=directive_arguments,
                                usage="[argument ...]",
                                minimum_arguments=0, maximum_arguments=-1),
         "description": Directive(method=directive_description,
                                  minimum_arguments=0, maximum_arguments=-1,
                                  usage="text"),
+        "environment-clear": Directive(method=directive_environment_clear,
+                                       usage="",
+                                       minimum_arguments=0),
+        "environment-passthrough": Directive(method=directive_environment_passthrough,
+                                             usage="variable ...",
+                                             minimum_arguments=1, maximum_arguments=-1),
+        "environment-set": Directive(method=directive_environment_set,
+                                     usage="variable value",
+                                     minimum_arguments=2),
+        "environment-unset": Directive(method=directive_environment_unset,
+                                       usage="variable ...",
+                                       minimum_arguments=1, maximum_arguments=-1),
         "features": Directive(method=directive_features,
                               usage="feature ...",
                               minimum_arguments=1),
         "file": Directive(method=directive_file,
                           usage="name in [out]",
                           minimum_arguments=2, maximum_arguments=3),
         "mkdir": Directive(method=directive_mkdir,
@@ -194,17 +220,14 @@
                              usage="name",
                              minimum_arguments=1,
                              only_once=True),
         "return": Directive(method=directive_return,
                             usage="exit-code",
                             minimum_arguments=1,
                             only_once=True),
-        "setenv": Directive(method=directive_setenv,
-                            usage="variable value",
-                            minimum_arguments=2),
         "stderr": Directive(method=directive_stderr,
                             usage="[file]",
                             minimum_arguments=0, maximum_arguments=1,
                             only_once=True),
         "stderr-replace": Directive(method=directive_stderr_replace,
                                     usage="pattern replacement",
                                     minimum_arguments=2),
```

### Comparing `nihtest-1.0.0/nihtest/Utility.py` & `nihtest-1.1.0/nihtest/Utility.py`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/nihtest/__main__.py` & `nihtest-1.1.0/nihtest/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import sys
 
 from nihtest import Test
 from nihtest import Configuration
 
-VERSION = "1.0.0" # TODO: get from Cmake
+VERSION = "1.1.0"
+
 
 def main():
     parser = argparse.ArgumentParser(
         prog='nihtest',
         description="nihtest " + VERSION  + "\nCopyright (C) 2023 Dieter Baron and Thomas Klausner")
     parser.add_argument('testcase', help='Testcase to run')
     parser.add_argument('-C', '--config-file', metavar='FILE', help='use FILE as config file', default="nihtest.conf")
```

### Comparing `nihtest-1.0.0/nihtest.egg-info/PKG-INFO` & `nihtest-1.1.0/nihtest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nihtest
-Version: 1.0.0
+Version: 1.1.0
 Summary: A testing tool for command line utilities.
 Author-email: Dieter Baron <dillo@nih.at>, Thomas Klausner <wiz@gatalith.at>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/nih-at/nihtest
 Project-URL: Bug Tracker, https://github.com/nih-at/nihtest/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `nihtest-1.0.0/nihtest.egg-info/SOURCES.txt` & `nihtest-1.1.0/nihtest.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 manpages/nihtest.conf.mdoc
 manpages/nihtest.html
 manpages/nihtest.man
 manpages/nihtest.mdoc
 nihtest/Command.py
 nihtest/CompareArrays.py
 nihtest/Configuration.py
+nihtest/Environment.py
 nihtest/Features.py
 nihtest/File.py
 nihtest/Sandbox.py
 nihtest/Test.py
 nihtest/TestCase.py
 nihtest/Utility.py
 nihtest/__init__.py
@@ -52,14 +53,26 @@
 tests/default-stderr-replace.test
 tests/description-pass.test
 tests/diff-1.input
 tests/diff-1.test
 tests/diff-2.input
 tests/diff-2.test
 tests/echo.c
+tests/environment-clear-pass.input
+tests/environment-clear-pass.test
+tests/environment-not-passed-pass.input
+tests/environment-not-passed-pass.test
+tests/environment-passthrough-pass.input
+tests/environment-passthrough-pass.test
+tests/environment-set-config-pass.input
+tests/environment-set-config-pass.test
+tests/environment-set-pass.input
+tests/environment-set-pass.test
+tests/environment-unset-pass.input
+tests/environment-unset-pass.test
 tests/failure.txt
 tests/false-fail.input
 tests/false-fail.test
 tests/false-pass.input
 tests/false-pass.test
 tests/false.c
 tests/features-fail.input
@@ -98,18 +111,14 @@
 tests/precheck-pass.input
 tests/precheck-pass.test
 tests/precheck-skip.input
 tests/precheck-skip.test
 tests/preload-pass.input
 tests/preload-pass.test
 tests/preload-skip.test
-tests/setenv-config-pass.input
-tests/setenv-config-pass.test
-tests/setenv-pass.input
-tests/setenv-pass.test
 tests/stderr-fail.input
 tests/stderr-fail.test
 tests/stderr-pass.input
 tests/stderr-pass.test
 tests/stderr-replace-pass.input
 tests/stderr-replace-pass.test
 tests/stdin-file-pass.input
```

### Comparing `nihtest-1.0.0/pyproject.toml` & `nihtest-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nihtest"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
     { name="Dieter Baron", email="dillo@nih.at" },
     { name="Thomas Klausner", email="wiz@gatalith.at"}
 ]
 description = "A testing tool for command line utilities."
 license = {text = "BSD-3-Clause"}
 readme = "README.md"
@@ -21,7 +21,22 @@
 
 [project.urls]
 "Homepage" = "https://github.com/nih-at/nihtest"
 "Bug Tracker" = "https://github.com/nih-at/nihtest/issues"
 
 [project.scripts]
 nihtest = "nihtest.__main__:main"
+
+[tool.bumpver]
+current_version = "1.1.0"
+version_pattern = "MAJOR.MINOR.PATCH"
+
+[tool.bumpver.file_patterns]
+"nihtest/__main__.py" = [
+    'VERSION = "{version}"'
+]
+"pyproject.toml" = [
+    'version = "{version}"'
+]
+"CMakeLists.txt" = [
+    "VERSION {version}"
+]
```

### Comparing `nihtest-1.0.0/tests/CMakeLists.txt` & `nihtest-1.1.0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/tests/can-preload.c` & `nihtest-1.1.0/tests/can-preload.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/tests/cat.c` & `nihtest-1.1.0/tests/cat.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/tests/comparator.c` & `nihtest-1.1.0/tests/comparator.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/tests/echo.c` & `nihtest-1.1.0/tests/echo.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/tests/false.c` & `nihtest-1.1.0/tests/false.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/tests/file.c` & `nihtest-1.1.0/tests/file.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/tests/getenv.c` & `nihtest-1.1.0/tests/getenv.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/tests/ineffective-remove.c` & `nihtest-1.1.0/tests/ineffective-remove.c`

 * *Files identical despite different names*

### Comparing `nihtest-1.0.0/tests/parameter-tests-1.test` & `nihtest-1.1.0/tests/parameter-tests-1.test`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 program nihtest
 return 99
 arguments parameter-tests-1.test
 file parameter-tests-1.test parameter-tests-1.input parameter-tests-1.input
 stderr
-parameter-tests-1.test:3: too few arguments for 'features'
-parameter-tests-1.test:4: too few arguments for 'file'
-parameter-tests-1.test:5: too few arguments for 'file'
-parameter-tests-1.test:6: too many arguments for 'file'
-parameter-tests-1.test:7: too few arguments for 'mkdir'
-parameter-tests-1.test:8: too many arguments for 'mkdir'
-parameter-tests-1.test:9: too few arguments for 'precheck'
-parameter-tests-1.test:10: too few arguments for 'preload'
-parameter-tests-1.test:11: too many arguments for 'preload'
-parameter-tests-1.test:12: too few arguments for 'program'
-parameter-tests-1.test:13: too few arguments for 'return'
-parameter-tests-1.test:14: too few arguments for 'setenv'
-parameter-tests-1.test:15: too few arguments for 'setenv'
-parameter-tests-1.test:16: too many arguments for 'setenv'
-parameter-tests-1.test:17: too many arguments for 'stderr'
-parameter-tests-1.test:18: too few arguments for 'stderr-replace'
-parameter-tests-1.test:19: too few arguments for 'stderr-replace'
-parameter-tests-1.test:20: too many arguments for 'stderr-replace'
-parameter-tests-1.test:21: too many arguments for 'stdin'
-parameter-tests-1.test:22: too many arguments for 'stdout'
+parameter-tests-1.test:3: too many arguments for 'environment-clear'
+parameter-tests-1.test:4: too few arguments for 'environment-passthrough'
+parameter-tests-1.test:5: too few arguments for 'environment-set'
+parameter-tests-1.test:6: too few arguments for 'environment-set'
+parameter-tests-1.test:7: too many arguments for 'environment-set'
+parameter-tests-1.test:8: too few arguments for 'environment-unset'
+parameter-tests-1.test:9: too few arguments for 'features'
+parameter-tests-1.test:10: too few arguments for 'file'
+parameter-tests-1.test:11: too few arguments for 'file'
+parameter-tests-1.test:12: too many arguments for 'file'
+parameter-tests-1.test:13: too few arguments for 'mkdir'
+parameter-tests-1.test:14: too many arguments for 'mkdir'
+parameter-tests-1.test:15: too few arguments for 'precheck'
+parameter-tests-1.test:16: too few arguments for 'preload'
+parameter-tests-1.test:17: too many arguments for 'preload'
+parameter-tests-1.test:18: too few arguments for 'program'
+parameter-tests-1.test:19: too few arguments for 'return'
+parameter-tests-1.test:20: too many arguments for 'stderr'
+parameter-tests-1.test:21: too few arguments for 'stderr-replace'
+parameter-tests-1.test:22: too few arguments for 'stderr-replace'
+parameter-tests-1.test:23: too many arguments for 'stderr-replace'
+parameter-tests-1.test:24: too many arguments for 'stdin'
+parameter-tests-1.test:25: too many arguments for 'stdout'
 nihtest: invalid test case
 end-of-inline-data
 stderr-replace ^.*/([^/:]*): "\1:"
```

### Comparing `nihtest-1.0.0/tests/true.c` & `nihtest-1.1.0/tests/true.c`

 * *Files identical despite different names*

