# Comparing `tmp/twtr-nuuuwan-1.0.0.tar.gz` & `tmp/twtr-nuuuwan-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twtr-nuuuwan-1.0.0.tar", last modified: Thu Jun 15 06:25:07 2023, max compression
+gzip compressed data, was "twtr-nuuuwan-1.0.1.tar", last modified: Thu Jun 15 06:30:25 2023, max compression
```

## Comparing `twtr-nuuuwan-1.0.0.tar` & `twtr-nuuuwan-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:25:07.601662 twtr-nuuuwan-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 06:24:18.000000 twtr-nuuuwan-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 06:25:07.601662 twtr-nuuuwan-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:25:07.605662 twtr-nuuuwan-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-15 06:24:18.000000 twtr-nuuuwan-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:25:07.601662 twtr-nuuuwan-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:25:07.601662 twtr-nuuuwan-1.0.0/src/twtr/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 06:24:18.000000 twtr-nuuuwan-1.0.0/src/twtr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 06:24:18.000000 twtr-nuuuwan-1.0.0/src/twtr/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:25:07.601662 twtr-nuuuwan-1.0.0/src/twtr_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 06:25:07.000000 twtr-nuuuwan-1.0.0/src/twtr_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-15 06:25:07.000000 twtr-nuuuwan-1.0.0/src/twtr_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:25:07.000000 twtr-nuuuwan-1.0.0/src/twtr_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 06:25:07.000000 twtr-nuuuwan-1.0.0/src/twtr_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 06:25:07.000000 twtr-nuuuwan-1.0.0/src/twtr_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:25:07.601662 twtr-nuuuwan-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-15 06:24:18.000000 twtr-nuuuwan-1.0.0/tests/test_twitter_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/src/twtr/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/src/twtr/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/core/Tweet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/core/Twitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/src/twtr/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 06:30:25.000000 twtr-nuuuwan-1.0.1/src/twtr_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:30:25.165940 twtr-nuuuwan-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-15 06:29:36.000000 twtr-nuuuwan-1.0.1/tests/test_twitter_basic.py
```

### Comparing `twtr-nuuuwan-1.0.0/LICENSE` & `twtr-nuuuwan-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twtr-nuuuwan-1.0.0/setup.py` & `twtr-nuuuwan-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'twtr'
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = "Wrapper library for the Twitter API and tweepy"
 
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
@@ -22,14 +22,11 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.10",
-    install_requires=[
-        'tweepy',
-        'utils-nuuuwan'
-    ],
+    install_requires=['tweepy', 'utils-nuuuwan'],
     test_suite='nose.collector',
     tests_require=['nose'],
 )
```

### Comparing `twtr-nuuuwan-1.0.0/tests/test_twitter_basic.py` & `twtr-nuuuwan-1.0.1/tests/test_twitter_basic.py`

 * *Files identical despite different names*

