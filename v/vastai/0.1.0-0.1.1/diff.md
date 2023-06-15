# Comparing `tmp/vastai-0.1.0.tar.gz` & `tmp/vastai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastai-0.1.0.tar", last modified: Thu Jun 15 21:02:56 2023, max compression
+gzip compressed data, was "vastai-0.1.1.tar", last modified: Thu Jun 15 21:36:07 2023, max compression
```

## Comparing `vastai-0.1.0.tar` & `vastai-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:56.793838 vastai-0.1.0/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1064 2023-06-15 20:54:21.000000 vastai-0.1.0/LICENSE.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 20:55:37.000000 vastai-0.1.0/MANIFEST.in
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      671 2023-06-15 21:02:56.793838 vastai-0.1.0/PKG-INFO
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33346 2023-06-15 20:53:50.000000 vastai-0.1.0/README.md
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 21:02:56.793838 vastai-0.1.0/setup.cfg
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1029 2023-06-15 20:37:00.000000 vastai-0.1.0/setup.py
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:56.793838 vastai-0.1.0/vastai/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:15.000000 vastai-0.1.0/vastai/__init__.py
--rwxrwxr-x   0 jcannell  (1000) jcannell  (1000)    75501 2023-06-15 20:33:35.000000 vastai-0.1.0/vastai/vast.py
-drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:56.793838 vastai-0.1.0/vastai.egg-info/
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      671 2023-06-15 21:02:56.000000 vastai-0.1.0/vastai.egg-info/PKG-INFO
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      268 2023-06-15 21:02:56.000000 vastai-0.1.0/vastai.egg-info/SOURCES.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        1 2023-06-15 21:02:56.000000 vastai-0.1.0/vastai.egg-info/dependency_links.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       45 2023-06-15 21:02:56.000000 vastai-0.1.0/vastai.egg-info/entry_points.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        9 2023-06-15 21:02:56.000000 vastai-0.1.0/vastai.egg-info/requires.txt
--rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        7 2023-06-15 21:02:56.000000 vastai-0.1.0/vastai.egg-info/top_level.txt
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:36:07.426611 vastai-0.1.1/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1064 2023-06-15 20:54:21.000000 vastai-0.1.1/LICENSE.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 20:55:37.000000 vastai-0.1.1/MANIFEST.in
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33957 2023-06-15 21:36:07.426611 vastai-0.1.1/PKG-INFO
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33346 2023-06-15 20:53:50.000000 vastai-0.1.1/README.md
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      641 2023-06-15 21:33:27.000000 vastai-0.1.1/pyproject.toml
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       38 2023-06-15 21:36:07.426611 vastai-0.1.1/setup.cfg
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)     1054 2023-06-15 21:20:12.000000 vastai-0.1.1/setup.py
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:36:07.426611 vastai-0.1.1/vastai/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:02:15.000000 vastai-0.1.1/vastai/__init__.py
+-rwxrwxr-x   0 jcannell  (1000) jcannell  (1000)    75501 2023-06-15 20:33:35.000000 vastai-0.1.1/vastai/vast.py
+drwxrwxr-x   0 jcannell  (1000) jcannell  (1000)        0 2023-06-15 21:36:07.426611 vastai-0.1.1/vastai.egg-info/
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)    33957 2023-06-15 21:36:07.000000 vastai-0.1.1/vastai.egg-info/PKG-INFO
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)      283 2023-06-15 21:36:07.000000 vastai-0.1.1/vastai.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        1 2023-06-15 21:36:07.000000 vastai-0.1.1/vastai.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)       44 2023-06-15 21:36:07.000000 vastai-0.1.1/vastai.egg-info/entry_points.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        9 2023-06-15 21:36:07.000000 vastai-0.1.1/vastai.egg-info/requires.txt
+-rw-rw-r--   0 jcannell  (1000) jcannell  (1000)        7 2023-06-15 21:36:07.000000 vastai-0.1.1/vastai.egg-info/top_level.txt
```

### Comparing `vastai-0.1.0/LICENSE.txt` & `vastai-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vastai-0.1.0/README.md` & `vastai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vastai-0.1.0/setup.py` & `vastai-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     packages=['vastai'],
     entry_points={
         'console_scripts': [
             'vastai = vastai.vast:main',  # you need a main function in your vast.py file
         ],
     },
     description='Vast.ai Python CLI',
+    #readme='README.md',
     url='https://github.com/vast-ai/vast-python',
     author='Vast.ai',
     author_email='support@vast.ai',
     license='MIT',  # choose your own license
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `vastai-0.1.0/vastai/vast.py` & `vastai-0.1.1/vastai/vast.py`

 * *Files identical despite different names*

