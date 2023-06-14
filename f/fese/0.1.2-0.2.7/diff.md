# Comparing `tmp/fese-0.1.2.tar.gz` & `tmp/fese-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fese-0.1.2.tar", last modified: Mon Feb 21 06:36:43 2022, max compression
+gzip compressed data, was "fese-0.2.7.tar", last modified: Wed Jun 14 22:05:12 2023, max compression
```

## Comparing `fese-0.1.2.tar` & `fese-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxr-xr-x   0 victor    (1000) users      (100)        0 2022-02-21 06:36:43.248766 fese-0.1.2/
--rwxr-xr-x   0 victor    (1000) users      (100)    35149 2021-12-23 20:46:44.000000 fese-0.1.2/LICENSE
--rw-r--r--   0 victor    (1000) users      (100)      923 2022-02-21 06:36:43.248766 fese-0.1.2/PKG-INFO
--rwxr-xr-x   0 victor    (1000) users      (100)      325 2021-12-23 20:24:34.000000 fese-0.1.2/README.md
-drwxr-xr-x   0 victor    (1000) users      (100)        0 2022-02-21 06:36:43.246766 fese-0.1.2/fese/
--rwxr-xr-x   0 victor    (1000) users      (100)    13155 2022-02-21 06:28:56.000000 fese-0.1.2/fese/__init__.py
-drwxr-xr-x   0 victor    (1000) users      (100)        0 2022-02-21 06:36:43.247766 fese-0.1.2/fese.egg-info/
--rw-r--r--   0 victor    (1000) users      (100)      923 2022-02-21 06:36:42.000000 fese-0.1.2/fese.egg-info/PKG-INFO
--rw-r--r--   0 victor    (1000) users      (100)      312 2022-02-21 06:36:43.000000 fese-0.1.2/fese.egg-info/SOURCES.txt
--rw-r--r--   0 victor    (1000) users      (100)        1 2022-02-21 06:36:42.000000 fese-0.1.2/fese.egg-info/dependency_links.txt
--rw-r--r--   0 victor    (1000) users      (100)       75 2022-02-21 06:36:43.000000 fese-0.1.2/fese.egg-info/requires.txt
--rw-r--r--   0 victor    (1000) users      (100)       11 2022-02-21 06:36:43.000000 fese-0.1.2/fese.egg-info/top_level.txt
--rw-r--r--   0 victor    (1000) users      (100)      788 2022-02-21 06:36:43.248766 fese-0.1.2/setup.cfg
--rw-r--r--   0 victor    (1000) users      (100)       38 2021-12-22 18:36:46.000000 fese-0.1.2/setup.py
-drwxr-xr-x   0 victor    (1000) users      (100)        0 2022-02-21 06:36:43.247766 fese-0.1.2/tests/
--rw-r--r--   0 victor    (1000) users      (100)        0 2021-12-28 18:46:44.000000 fese-0.1.2/tests/__init__.py
--rw-r--r--   0 victor    (1000) users      (100)     4321 2022-02-21 06:28:56.000000 fese-0.1.2/tests/test_subtitle_stream.py
--rw-r--r--   0 victor    (1000) users      (100)     1112 2021-12-22 18:36:46.000000 fese-0.1.2/tests/test_subtitle_stream_disposition.py
--rw-r--r--   0 victor    (1000) users      (100)     1591 2021-12-28 19:28:59.000000 fese-0.1.2/tests/test_video_container.py
+drwxr-xr-x   0 victor    (1000) users      (100)        0 2023-06-14 22:05:12.359917 fese-0.2.7/
+-rwxr-xr-x   0 victor    (1000) users      (100)    35149 2022-06-20 22:07:53.000000 fese-0.2.7/LICENSE
+-rw-r--r--   0 victor    (1000) users      (100)      607 2023-06-14 22:05:12.358918 fese-0.2.7/PKG-INFO
+-rwxr-xr-x   0 victor    (1000) users      (100)      362 2022-07-19 21:45:29.000000 fese-0.2.7/README.md
+drwxr-xr-x   0 victor    (1000) users      (100)        0 2023-06-14 22:05:12.357917 fese-0.2.7/fese/
+-rwxr-xr-x   0 victor    (1000) users      (100)      150 2023-06-14 21:45:58.000000 fese-0.2.7/fese/__init__.py
+-rwxr-xr-x   0 victor    (1000) users      (100)     8140 2022-07-19 23:03:05.000000 fese-0.2.7/fese/container.py
+-rw-r--r--   0 victor    (1000) users      (100)     2116 2023-06-14 21:45:58.000000 fese-0.2.7/fese/disposition.py
+-rw-r--r--   0 victor    (1000) users      (100)      372 2023-06-14 21:52:50.000000 fese-0.2.7/fese/exceptions.py
+-rwxr-xr-x   0 victor    (1000) users      (100)     4866 2023-06-14 21:45:58.000000 fese-0.2.7/fese/stream.py
+-rw-r--r--   0 victor    (1000) users      (100)     5454 2023-06-14 21:45:58.000000 fese-0.2.7/fese/tags.py
+drwxr-xr-x   0 victor    (1000) users      (100)        0 2023-06-14 22:05:12.358918 fese-0.2.7/fese.egg-info/
+-rw-r--r--   0 victor    (1000) users      (100)      607 2023-06-14 22:05:12.000000 fese-0.2.7/fese.egg-info/PKG-INFO
+-rw-r--r--   0 victor    (1000) users      (100)      363 2023-06-14 22:05:12.000000 fese-0.2.7/fese.egg-info/SOURCES.txt
+-rw-r--r--   0 victor    (1000) users      (100)        1 2023-06-14 22:05:12.000000 fese-0.2.7/fese.egg-info/dependency_links.txt
+-rw-r--r--   0 victor    (1000) users      (100)       18 2023-06-14 22:05:12.000000 fese-0.2.7/fese.egg-info/requires.txt
+-rw-r--r--   0 victor    (1000) users      (100)        5 2023-06-14 22:05:12.000000 fese-0.2.7/fese.egg-info/top_level.txt
+-rw-r--r--   0 victor    (1000) users      (100)      385 2023-06-14 21:58:23.000000 fese-0.2.7/pyproject.toml
+-rw-r--r--   0 victor    (1000) users      (100)       38 2023-06-14 22:05:12.359917 fese-0.2.7/setup.cfg
+drwxr-xr-x   0 victor    (1000) users      (100)        0 2023-06-14 22:05:12.358918 fese-0.2.7/tests/
+-rw-r--r--   0 victor    (1000) users      (100)     3704 2022-09-20 21:10:17.000000 fese-0.2.7/tests/test_container.py
+-rw-r--r--   0 victor    (1000) users      (100)     1840 2023-06-14 21:45:58.000000 fese-0.2.7/tests/test_disposition.py
+-rw-r--r--   0 victor    (1000) users      (100)     5368 2023-06-14 21:52:16.000000 fese-0.2.7/tests/test_stream.py
+-rw-r--r--   0 victor    (1000) users      (100)     3301 2022-09-20 21:12:27.000000 fese-0.2.7/tests/test_tags.py
```

### Comparing `fese-0.1.2/LICENSE` & `fese-0.2.7/LICENSE`

 * *Files identical despite different names*

