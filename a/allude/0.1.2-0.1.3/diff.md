# Comparing `tmp/allude-0.1.2.tar.gz` & `tmp/allude-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allude-0.1.2.tar", last modified: Wed Sep  8 01:15:26 2021, max compression
+gzip compressed data, was "allude-0.1.3.tar", last modified: Thu Jun 15 13:29:33 2023, max compression
```

## Comparing `allude-0.1.2.tar` & `allude-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 01:15:26.122521 allude-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-09-08 01:14:56.000000 allude-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      410 2021-09-08 01:15:26.122521 allude-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-09-08 01:14:56.000000 allude-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 01:15:26.122521 allude-0.1.2/allude/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-09-08 01:14:56.000000 allude-0.1.2/allude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20719 2021-09-08 01:14:56.000000 allude-0.1.2/allude/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 01:15:26.122521 allude-0.1.2/allude/inspiration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-08 01:14:56.000000 allude-0.1.2/allude/inspiration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2223 2021-09-08 01:14:56.000000 allude-0.1.2/allude/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-08 01:15:26.122521 allude-0.1.2/allude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      410 2021-09-08 01:15:25.000000 allude-0.1.2/allude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      294 2021-09-08 01:15:25.000000 allude-0.1.2/allude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-08 01:15:25.000000 allude-0.1.2/allude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-08 01:15:25.000000 allude-0.1.2/allude.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-09-08 01:15:25.000000 allude-0.1.2/allude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-09-08 01:15:25.000000 allude-0.1.2/allude.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      538 2021-09-08 01:15:26.122521 allude-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-09-08 01:14:56.000000 allude-0.1.2/setup.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-06-15 13:29:33.773447 allude-0.1.3/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)    11357 2022-10-25 12:53:20.000000 allude-0.1.3/LICENSE
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      379 2023-06-15 13:29:33.773717 allude-0.1.3/PKG-INFO
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      105 2022-10-25 12:53:20.000000 allude-0.1.3/README.md
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-06-15 13:29:33.522333 allude-0.1.3/allude/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       90 2023-06-15 11:40:01.000000 allude-0.1.3/allude/__init__.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      101 2023-06-15 12:06:32.000000 allude-0.1.3/allude/base.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-06-15 13:29:33.771731 allude-0.1.3/allude/examples/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        0 2023-01-11 09:10:33.000000 allude-0.1.3/allude/examples/__init__.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     8141 2023-06-15 11:35:53.000000 allude-0.1.3/allude/examples/gantt.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      149 2023-01-11 09:29:33.000000 allude-0.1.3/allude/examples/sequence_diagram.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     5401 2023-01-11 09:09:44.000000 allude-0.1.3/allude/util.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-06-15 13:29:33.710857 allude-0.1.3/allude.egg-info/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      379 2023-06-15 13:29:32.000000 allude-0.1.3/allude.egg-info/PKG-INFO
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      352 2023-06-15 13:29:32.000000 allude-0.1.3/allude.egg-info/SOURCES.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-06-15 13:29:32.000000 allude-0.1.3/allude.egg-info/dependency_links.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-06-15 13:29:32.000000 allude-0.1.3/allude.egg-info/not-zip-safe
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       31 2023-06-15 13:29:32.000000 allude-0.1.3/allude.egg-info/requires.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        7 2023-06-15 13:29:32.000000 allude-0.1.3/allude.egg-info/top_level.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      555 2023-06-15 13:29:33.776135 allude-0.1.3/setup.cfg
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       91 2022-10-25 12:53:20.000000 allude-0.1.3/setup.py
```

### Comparing `allude-0.1.2/LICENSE` & `allude-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `allude-0.1.2/setup.cfg` & `allude-0.1.3/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = allude
-version = 0.1.2
+version = 0.1.3
 url = https://github.com/i2mint/allude
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = Building precise functionality from vague specifications
@@ -17,12 +17,14 @@
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
 	i2
 	lined
 	meshed
+	graphviz
+	pydot
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

