# Comparing `tmp/jj_wingman-0.2.2.tar.gz` & `tmp/jj_wingman-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj_wingman-0.2.2.tar", last modified: Wed May 31 18:27:20 2023, max compression
+gzip compressed data, was "jj_wingman-0.2.3.tar", last modified: Thu Jun 15 19:07:33 2023, max compression
```

## Comparing `jj_wingman-0.2.2.tar` & `jj_wingman-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-31 18:27:20.297665 jj_wingman-0.2.2/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.2.2/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-05-31 18:27:20.297665 jj_wingman-0.2.2/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)    13489 2023-03-07 18:53:37.000000 jj_wingman-0.2.2/README.md
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-31 18:27:20.293665 jj_wingman-0.2.2/jj_wingman.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-05-31 18:27:20.000000 jj_wingman-0.2.2/jj_wingman.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-05-31 18:27:20.000000 jj_wingman-0.2.2/jj_wingman.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-31 18:27:20.000000 jj_wingman-0.2.2/jj_wingman.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-05-31 18:27:20.000000 jj_wingman-0.2.2/jj_wingman.egg-info/entry_points.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-05-31 18:27:20.000000 jj_wingman-0.2.2/jj_wingman.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-05-31 18:27:20.000000 jj_wingman-0.2.2/jj_wingman.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-05-31 18:27:15.000000 jj_wingman-0.2.2/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-31 18:27:20.297665 jj_wingman-0.2.2/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.2.2/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-31 18:27:20.293665 jj_wingman-0.2.2/test/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3917 2023-05-29 12:52:26.000000 jj_wingman-0.2.2/test/test_replay_buffer.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-31 18:27:20.293665 jj_wingman-0.2.2/wingman/
--rw-rw-r--   0 jet       (1000) jet       (1000)      218 2022-12-10 02:36:58.000000 jj_wingman-0.2.2/wingman/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.2.2/wingman/cli_scripts.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      288 2022-11-26 07:59:06.000000 jj_wingman-0.2.2/wingman/config.yaml
--rw-rw-r--   0 jet       (1000) jet       (1000)    10283 2023-05-31 18:27:09.000000 jj_wingman-0.2.2/wingman/neural_blocks.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      777 2023-03-07 18:47:29.000000 jj_wingman-0.2.2/wingman/print_utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5617 2023-05-21 21:59:51.000000 jj_wingman-0.2.2/wingman/replay_buffer.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1033 2023-03-07 18:51:03.000000 jj_wingman-0.2.2/wingman/utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15009 2023-03-07 18:51:08.000000 jj_wingman-0.2.2/wingman/wingman.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-15 19:07:33.078592 jj_wingman-0.2.3/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.2.3/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-06-15 19:07:33.078592 jj_wingman-0.2.3/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)    13489 2023-03-07 18:53:37.000000 jj_wingman-0.2.3/README.md
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-15 19:07:33.078592 jj_wingman-0.2.3/jj_wingman.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-06-15 19:07:33.000000 jj_wingman-0.2.3/jj_wingman.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-06-15 19:07:33.000000 jj_wingman-0.2.3/jj_wingman.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-06-15 19:07:33.000000 jj_wingman-0.2.3/jj_wingman.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-06-15 19:07:33.000000 jj_wingman-0.2.3/jj_wingman.egg-info/entry_points.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-06-15 19:07:33.000000 jj_wingman-0.2.3/jj_wingman.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-06-15 19:07:33.000000 jj_wingman-0.2.3/jj_wingman.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-06-15 19:07:30.000000 jj_wingman-0.2.3/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-06-15 19:07:33.078592 jj_wingman-0.2.3/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.2.3/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-15 19:07:33.078592 jj_wingman-0.2.3/test/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3917 2023-05-29 12:52:26.000000 jj_wingman-0.2.3/test/test_replay_buffer.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-15 19:07:33.078592 jj_wingman-0.2.3/wingman/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      218 2023-06-02 11:46:07.000000 jj_wingman-0.2.3/wingman/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.2.3/wingman/cli_scripts.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      288 2022-11-26 07:59:06.000000 jj_wingman-0.2.3/wingman/config.yaml
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10283 2023-06-02 11:46:40.000000 jj_wingman-0.2.3/wingman/neural_blocks.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      777 2023-03-07 18:47:29.000000 jj_wingman-0.2.3/wingman/print_utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5617 2023-05-21 21:59:51.000000 jj_wingman-0.2.3/wingman/replay_buffer.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1033 2023-06-01 08:57:08.000000 jj_wingman-0.2.3/wingman/utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15173 2023-06-15 19:07:07.000000 jj_wingman-0.2.3/wingman/wingman.py
```

### Comparing `jj_wingman-0.2.2/LICENSE.txt` & `jj_wingman-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.2/PKG-INFO` & `jj_wingman-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.2.2
+Version: 0.2.3
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `jj_wingman-0.2.2/README.md` & `jj_wingman-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.2/jj_wingman.egg-info/PKG-INFO` & `jj_wingman-0.2.3/jj_wingman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj-wingman
-Version: 0.2.2
+Version: 0.2.3
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `jj_wingman-0.2.2/pyproject.toml` & `jj_wingman-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jj_wingman"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "Wingman library for AI projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jj_wingman-0.2.2/test/test_replay_buffer.py` & `jj_wingman-0.2.3/test/test_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.2/wingman/cli_scripts.py` & `jj_wingman-0.2.3/wingman/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.2/wingman/neural_blocks.py` & `jj_wingman-0.2.3/wingman/neural_blocks.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.2/wingman/print_utils.py` & `jj_wingman-0.2.3/wingman/print_utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.2/wingman/replay_buffer.py` & `jj_wingman-0.2.3/wingman/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.2/wingman/utils.py` & `jj_wingman-0.2.3/wingman/utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.2.2/wingman/wingman.py` & `jj_wingman-0.2.3/wingman/wingman.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,14 +388,17 @@
         # if we don't need the latest file, get the one specified
         if not latest:
             if os.path.isfile(self.model_file):
                 self.model_file = os.path.join(
                     self.version_directory,
                     f"weights{self.mark_number}.pth",
                 )
+                wm_print(
+                    f"Using weights file: {cstr(f'{self.version_directory}/weights{self.mark_number}.pth', 'OKGREEN')}"
+                )
                 return True, self.model_file, self.optim_file
             else:
                 raise ValueError(
                     cstr(
                         f"Mark number {self.mark_number} was requested, but it doesn't exist.",
                         "FAIL",
                     )
```

