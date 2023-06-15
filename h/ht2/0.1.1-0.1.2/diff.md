# Comparing `tmp/ht2-0.1.1.tar.gz` & `tmp/ht2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht2-0.1.1.tar", last modified: Tue May 16 10:14:28 2023, max compression
+gzip compressed data, was "ht2-0.1.2.tar", last modified: Thu Jun 15 10:48:40 2023, max compression
```

## Comparing `ht2-0.1.1.tar` & `ht2-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 10:14:28.444777 ht2-0.1.1/
--rw-r--r--   0 agent_h    (501) staff       (20)     1070 2023-05-16 03:28:49.000000 ht2-0.1.1/LICENSE
--rw-r--r--   0 agent_h    (501) staff       (20)      754 2023-05-16 10:14:28.444643 ht2-0.1.1/PKG-INFO
--rw-r--r--   0 agent_h    (501) staff       (20)      246 2023-05-16 06:43:21.000000 ht2-0.1.1/README.md
--rw-r--r--   0 agent_h    (501) staff       (20)      644 2023-05-16 10:13:29.000000 ht2-0.1.1/pyproject.toml
--rw-r--r--   0 agent_h    (501) staff       (20)       38 2023-05-16 10:14:28.444819 ht2-0.1.1/setup.cfg
-drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 10:14:28.441529 ht2-0.1.1/src/
-drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 10:14:28.443608 ht2-0.1.1/src/ht2/
--rw-r--r--   0 agent_h    (501) staff       (20)       95 2023-05-16 09:09:51.000000 ht2-0.1.1/src/ht2/__init__.py
--rw-r--r--   0 agent_h    (501) staff       (20)       71 2023-05-16 03:37:28.000000 ht2-0.1.1/src/ht2/example.py
--rw-r--r--   0 agent_h    (501) staff       (20)        0 2023-05-16 06:35:46.000000 ht2-0.1.1/src/ht2/files_io.py
--rw-r--r--   0 agent_h    (501) staff       (20)      495 2023-05-16 06:50:54.000000 ht2-0.1.1/src/ht2/isp.py
--rw-r--r--   0 agent_h    (501) staff       (20)      672 2023-05-16 09:14:17.000000 ht2-0.1.1/src/ht2/text_utils.py
--rw-r--r--   0 agent_h    (501) staff       (20)      503 2023-05-16 06:16:09.000000 ht2-0.1.1/src/ht2/visualize.py
-drwxr-xr-x   0 agent_h    (501) staff       (20)        0 2023-05-16 10:14:28.444462 ht2-0.1.1/src/ht2.egg-info/
--rw-r--r--   0 agent_h    (501) staff       (20)      754 2023-05-16 10:14:28.000000 ht2-0.1.1/src/ht2.egg-info/PKG-INFO
--rw-r--r--   0 agent_h    (501) staff       (20)      303 2023-05-16 10:14:28.000000 ht2-0.1.1/src/ht2.egg-info/SOURCES.txt
--rw-r--r--   0 agent_h    (501) staff       (20)        1 2023-05-16 10:14:28.000000 ht2-0.1.1/src/ht2.egg-info/dependency_links.txt
--rw-r--r--   0 agent_h    (501) staff       (20)       31 2023-05-16 10:14:28.000000 ht2-0.1.1/src/ht2.egg-info/requires.txt
--rw-r--r--   0 agent_h    (501) staff       (20)        4 2023-05-16 10:14:28.000000 ht2-0.1.1/src/ht2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:48:40.138352 ht2-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-06-12 07:05:14.000000 ht2-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      775 2023-06-15 10:48:40.138352 ht2-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-15 08:25:10.000000 ht2-0.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      713 2023-06-15 10:47:36.000000 ht2-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 10:48:40.138352 ht2-0.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:48:40.134352 ht2-0.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:48:40.138352 ht2-0.1.2/src/ht2/
+-rw-r--r--   0 root         (0) root         (0)      126 2023-06-15 10:32:09.000000 ht2-0.1.2/src/ht2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-12 07:05:14.000000 ht2-0.1.2/src/ht2/example.py
+-rw-r--r--   0 root         (0) root         (0)     6351 2023-06-15 06:22:24.000000 ht2-0.1.2/src/ht2/files.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-13 07:59:41.000000 ht2-0.1.2/src/ht2/image.py
+-rw-r--r--   0 root         (0) root         (0)      467 2023-06-15 10:31:54.000000 ht2-0.1.2/src/ht2/misc.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-12 09:33:27.000000 ht2-0.1.2/src/ht2/os.py
+-rw-r--r--   0 root         (0) root         (0)      672 2023-06-12 07:05:14.000000 ht2-0.1.2/src/ht2/text.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-12 07:05:14.000000 ht2-0.1.2/src/ht2/visualize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:48:40.138352 ht2-0.1.2/src/ht2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      775 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-15 10:48:40.000000 ht2-0.1.2/src/ht2.egg-info/top_level.txt
```

### Comparing `ht2-0.1.1/LICENSE` & `ht2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ht2-0.1.1/pyproject.toml` & `ht2-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ht2"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Haotian Zhang", email="z.haotian@columbia.edu" },
 ]
-description = "Frequently used tools and wrappers for efficiency"
+description = "Just a bag of quality of life tools for Machine Learning Engineers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "opencv-python",
   "matplotlib",
-  "numpy"
+  "numpy",
+  "lmdb",
+  "msgpack",
+  "msgpack_numpy",
+  "tqdm"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/htplex/ht2"
 "Bug Tracker" = "https://github.com/htplex/ht2/issues"
```

### Comparing `ht2-0.1.1/src/ht2/text_utils.py` & `ht2-0.1.2/src/ht2/text.py`

 * *Files identical despite different names*

