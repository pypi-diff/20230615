# Comparing `tmp/ncOrtho-0.4.0.tar.gz` & `tmp/ncOrtho-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncOrtho-0.4.0.tar", last modified: Thu Jun 15 12:30:17 2023, max compression
+gzip compressed data, was "ncOrtho-0.4.1.tar", last modified: Thu Jun 15 12:34:27 2023, max compression
```

## Comparing `ncOrtho-0.4.0.tar` & `ncOrtho-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:17.287569 ncOrtho-0.4.0/
--rw-r--r--   0 felixl   (10024) users      (501)    35149 2021-06-22 08:19:32.000000 ncOrtho-0.4.0/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-15 12:30:17.285568 ncOrtho-0.4.0/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)     6480 2023-03-09 13:27:30.000000 ncOrtho-0.4.0/README.md
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:16.842597 ncOrtho-0.4.0/ncOrtho/
--rw-r--r--   0 felixl   (10024) users      (501)       43 2021-06-22 08:19:32.000000 ncOrtho-0.4.0/ncOrtho/__init__.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:16.937583 ncOrtho-0.4.0/ncOrtho/analysis/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2021-07-08 09:25:07.000000 ncOrtho-0.4.0/ncOrtho/analysis/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     5931 2021-07-08 10:23:46.000000 ncOrtho-0.4.0/ncOrtho/analysis/concat_alignments_dmp.pl
--rw-r--r--   0 felixl   (10024) users      (501)     1596 2021-07-08 10:23:46.000000 ncOrtho-0.4.0/ncOrtho/analysis/degapper.pl
--rw-r--r--   0 felixl   (10024) users      (501)    11977 2023-03-09 15:33:35.000000 ncOrtho-0.4.0/ncOrtho/analysis/ncAnalyze.py
--rw-r--r--   0 felixl   (10024) users      (501)     7691 2023-06-13 14:46:25.000000 ncOrtho-0.4.0/ncOrtho/blastparser.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:17.006584 ncOrtho-0.4.0/ncOrtho/check/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2023-02-01 12:48:24.000000 ncOrtho-0.4.0/ncOrtho/check/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     8997 2023-03-08 09:37:40.000000 ncOrtho-0.4.0/ncOrtho/check/core_synteny.py
--rw-r--r--   0 felixl   (10024) users      (501)     6037 2023-02-03 14:32:30.000000 ncOrtho-0.4.0/ncOrtho/check/tmp.py
--rw-r--r--   0 felixl   (10024) users      (501)    12394 2023-06-14 11:24:43.000000 ncOrtho-0.4.0/ncOrtho/cmsearch.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:17.180570 ncOrtho-0.4.0/ncOrtho/coreset/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2021-06-22 08:19:32.000000 ncOrtho-0.4.0/ncOrtho/coreset/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     6840 2023-06-14 15:25:46.000000 ncOrtho-0.4.0/ncOrtho/coreset/core_reblast.py
--rw-r--r--   0 felixl   (10024) users      (501)     9906 2023-06-14 15:15:29.000000 ncOrtho-0.4.0/ncOrtho/coreset/coreset.py
--rw-r--r--   0 felixl   (10024) users      (501)     8473 2023-04-27 13:13:52.000000 ncOrtho-0.4.0/ncOrtho/coreset/coreset_utils.py
--rw-r--r--   0 felixl   (10024) users      (501)     3813 2023-06-14 15:25:46.000000 ncOrtho-0.4.0/ncOrtho/coreset/createcm.py
--rw-r--r--   0 felixl   (10024) users      (501)     1019 2021-06-22 08:54:38.000000 ncOrtho-0.4.0/ncOrtho/coreset/example_parameters.yaml
--rw-r--r--   0 felixl   (10024) users      (501)     7002 2023-06-14 14:54:01.000000 ncOrtho-0.4.0/ncOrtho/coreset/locate_position.py
--rw-r--r--   0 felixl   (10024) users      (501)     5065 2023-03-20 09:25:58.000000 ncOrtho-0.4.0/ncOrtho/coreset/synteny.py
--rw-r--r--   0 felixl   (10024) users      (501)      473 2023-06-15 08:43:32.000000 ncOrtho-0.4.0/ncOrtho/figletest.py
--rw-r--r--   0 felixl   (10024) users      (501)     1971 2021-06-23 13:13:57.000000 ncOrtho-0.4.0/ncOrtho/genparser.py
--rwxr-xr-x   0 felixl   (10024) users      (501)    16810 2023-06-14 12:32:57.000000 ncOrtho-0.4.0/ncOrtho/ncortho.py
--rw-r--r--   0 felixl   (10024) users      (501)     1713 2023-06-14 11:59:44.000000 ncOrtho-0.4.0/ncOrtho/reblast.py
--rw-r--r--   0 felixl   (10024) users      (501)     3749 2023-06-14 11:24:43.000000 ncOrtho-0.4.0/ncOrtho/rna_object.py
--rw-r--r--   0 felixl   (10024) users      (501)    14873 2023-06-13 09:37:44.000000 ncOrtho-0.4.0/ncOrtho/tmp_old_cmsearch.py
--rw-r--r--   0 felixl   (10024) users      (501)      989 2023-06-15 12:25:12.000000 ncOrtho-0.4.0/ncOrtho/utils.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:16.874590 ncOrtho-0.4.0/ncOrtho.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      896 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)      176 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       34 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        8 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/top_level.txt
--rw-r--r--   0 felixl   (10024) users      (501)      103 2021-06-30 12:35:13.000000 ncOrtho-0.4.0/pyproject.toml
--rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-15 12:30:17.288565 ncOrtho-0.4.0/setup.cfg
--rw-r--r--   0 felixl   (10024) users      (501)     1979 2023-06-15 08:42:22.000000 ncOrtho-0.4.0/setup.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:34:27.218480 ncOrtho-0.4.1/
+-rw-r--r--   0 felixl   (10024) users      (501)    35149 2021-06-22 08:19:32.000000 ncOrtho-0.4.1/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-15 12:34:27.216480 ncOrtho-0.4.1/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)     6480 2023-03-09 13:27:30.000000 ncOrtho-0.4.1/README.md
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:34:26.939495 ncOrtho-0.4.1/ncOrtho/
+-rw-r--r--   0 felixl   (10024) users      (501)       43 2021-06-22 08:19:32.000000 ncOrtho-0.4.1/ncOrtho/__init__.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:34:27.050491 ncOrtho-0.4.1/ncOrtho/analysis/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2021-07-08 09:25:07.000000 ncOrtho-0.4.1/ncOrtho/analysis/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     5931 2021-07-08 10:23:46.000000 ncOrtho-0.4.1/ncOrtho/analysis/concat_alignments_dmp.pl
+-rw-r--r--   0 felixl   (10024) users      (501)     1596 2021-07-08 10:23:46.000000 ncOrtho-0.4.1/ncOrtho/analysis/degapper.pl
+-rw-r--r--   0 felixl   (10024) users      (501)    11977 2023-03-09 15:33:35.000000 ncOrtho-0.4.1/ncOrtho/analysis/ncAnalyze.py
+-rw-r--r--   0 felixl   (10024) users      (501)     7691 2023-06-13 14:46:25.000000 ncOrtho-0.4.1/ncOrtho/blastparser.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:34:27.102495 ncOrtho-0.4.1/ncOrtho/check/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2023-02-01 12:48:24.000000 ncOrtho-0.4.1/ncOrtho/check/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     8997 2023-03-08 09:37:40.000000 ncOrtho-0.4.1/ncOrtho/check/core_synteny.py
+-rw-r--r--   0 felixl   (10024) users      (501)     6037 2023-02-03 14:32:30.000000 ncOrtho-0.4.1/ncOrtho/check/tmp.py
+-rw-r--r--   0 felixl   (10024) users      (501)    12394 2023-06-14 11:24:43.000000 ncOrtho-0.4.1/ncOrtho/cmsearch.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:34:27.149503 ncOrtho-0.4.1/ncOrtho/coreset/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2021-06-22 08:19:32.000000 ncOrtho-0.4.1/ncOrtho/coreset/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     6840 2023-06-14 15:25:46.000000 ncOrtho-0.4.1/ncOrtho/coreset/core_reblast.py
+-rw-r--r--   0 felixl   (10024) users      (501)     9915 2023-06-15 12:34:05.000000 ncOrtho-0.4.1/ncOrtho/coreset/coreset.py
+-rw-r--r--   0 felixl   (10024) users      (501)     8473 2023-04-27 13:13:52.000000 ncOrtho-0.4.1/ncOrtho/coreset/coreset_utils.py
+-rw-r--r--   0 felixl   (10024) users      (501)     3813 2023-06-14 15:25:46.000000 ncOrtho-0.4.1/ncOrtho/coreset/createcm.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1019 2021-06-22 08:54:38.000000 ncOrtho-0.4.1/ncOrtho/coreset/example_parameters.yaml
+-rw-r--r--   0 felixl   (10024) users      (501)     7002 2023-06-14 14:54:01.000000 ncOrtho-0.4.1/ncOrtho/coreset/locate_position.py
+-rw-r--r--   0 felixl   (10024) users      (501)     5065 2023-03-20 09:25:58.000000 ncOrtho-0.4.1/ncOrtho/coreset/synteny.py
+-rw-r--r--   0 felixl   (10024) users      (501)      473 2023-06-15 08:43:32.000000 ncOrtho-0.4.1/ncOrtho/figletest.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1971 2021-06-23 13:13:57.000000 ncOrtho-0.4.1/ncOrtho/genparser.py
+-rwxr-xr-x   0 felixl   (10024) users      (501)    16810 2023-06-14 12:32:57.000000 ncOrtho-0.4.1/ncOrtho/ncortho.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1713 2023-06-14 11:59:44.000000 ncOrtho-0.4.1/ncOrtho/reblast.py
+-rw-r--r--   0 felixl   (10024) users      (501)     3749 2023-06-14 11:24:43.000000 ncOrtho-0.4.1/ncOrtho/rna_object.py
+-rw-r--r--   0 felixl   (10024) users      (501)    14873 2023-06-13 09:37:44.000000 ncOrtho-0.4.1/ncOrtho/tmp_old_cmsearch.py
+-rw-r--r--   0 felixl   (10024) users      (501)      989 2023-06-15 12:25:12.000000 ncOrtho-0.4.1/ncOrtho/utils.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:34:27.016506 ncOrtho-0.4.1/ncOrtho.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-15 12:34:26.000000 ncOrtho-0.4.1/ncOrtho.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      896 2023-06-15 12:34:26.000000 ncOrtho-0.4.1/ncOrtho.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-15 12:34:26.000000 ncOrtho-0.4.1/ncOrtho.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)      176 2023-06-15 12:34:26.000000 ncOrtho-0.4.1/ncOrtho.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       34 2023-06-15 12:34:26.000000 ncOrtho-0.4.1/ncOrtho.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        8 2023-06-15 12:34:26.000000 ncOrtho-0.4.1/ncOrtho.egg-info/top_level.txt
+-rw-r--r--   0 felixl   (10024) users      (501)      103 2021-06-30 12:35:13.000000 ncOrtho-0.4.1/pyproject.toml
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-15 12:34:27.219478 ncOrtho-0.4.1/setup.cfg
+-rw-r--r--   0 felixl   (10024) users      (501)     1979 2023-06-15 12:32:39.000000 ncOrtho-0.4.1/setup.py
```

### Comparing `ncOrtho-0.4.0/LICENSE` & `ncOrtho-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/PKG-INFO` & `ncOrtho-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncOrtho
-Version: 0.4.0
+Version: 0.4.1
 Summary:  Targeted ortholog search for miRNAs 
 Home-page: https://github.com/felixlangschied/ncortho
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncOrtho-0.4.0/README.md` & `ncOrtho-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/analysis/concat_alignments_dmp.pl` & `ncOrtho-0.4.1/ncOrtho/analysis/concat_alignments_dmp.pl`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/analysis/degapper.pl` & `ncOrtho-0.4.1/ncOrtho/analysis/degapper.pl`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/analysis/ncAnalyze.py` & `ncOrtho-0.4.1/ncOrtho/analysis/ncAnalyze.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/blastparser.py` & `ncOrtho-0.4.1/ncOrtho/blastparser.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/check/core_synteny.py` & `ncOrtho-0.4.1/ncOrtho/check/core_synteny.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/check/tmp.py` & `ncOrtho-0.4.1/ncOrtho/check/tmp.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/cmsearch.py` & `ncOrtho-0.4.1/ncOrtho/cmsearch.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/coreset/core_reblast.py` & `ncOrtho-0.4.1/ncOrtho/coreset/core_reblast.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/coreset/coreset.py` & `ncOrtho-0.4.1/ncOrtho/coreset/coreset.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 try:
     from createcm import create_cm, create_phmm
     from core_reblast import blastsearch
     from locate_position import categorize_mirna_position
     from synteny import analyze_synteny
     import coreset_utils as cu
 except ModuleNotFoundError:
-    from ncOrtho.coreset.createcm import CmConstructor
+    from ncOrtho.coreset.createcm import create_cm, create_phmm
     from ncOrtho.coreset.core_reblast import blastsearch
-    from ncOrtho.coreset.synteny import analyze_synteny
     from ncOrtho.coreset.locate_position import categorize_mirna_position
+    from ncOrtho.coreset.synteny import analyze_synteny
     import ncOrtho.coreset.coreset_utils as cu
 
 
 ###############################################################################
 def main():
     parser = argparse.ArgumentParser(
         description=(
```

### Comparing `ncOrtho-0.4.0/ncOrtho/coreset/coreset_utils.py` & `ncOrtho-0.4.1/ncOrtho/coreset/coreset_utils.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/coreset/createcm.py` & `ncOrtho-0.4.1/ncOrtho/coreset/createcm.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/coreset/example_parameters.yaml` & `ncOrtho-0.4.1/ncOrtho/coreset/example_parameters.yaml`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/coreset/locate_position.py` & `ncOrtho-0.4.1/ncOrtho/coreset/locate_position.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/coreset/synteny.py` & `ncOrtho-0.4.1/ncOrtho/coreset/synteny.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/genparser.py` & `ncOrtho-0.4.1/ncOrtho/genparser.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/ncortho.py` & `ncOrtho-0.4.1/ncOrtho/ncortho.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/reblast.py` & `ncOrtho-0.4.1/ncOrtho/reblast.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/rna_object.py` & `ncOrtho-0.4.1/ncOrtho/rna_object.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/tmp_old_cmsearch.py` & `ncOrtho-0.4.1/ncOrtho/tmp_old_cmsearch.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho/utils.py` & `ncOrtho-0.4.1/ncOrtho/utils.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/ncOrtho.egg-info/PKG-INFO` & `ncOrtho-0.4.1/ncOrtho.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncOrtho
-Version: 0.4.0
+Version: 0.4.1
 Summary:  Targeted ortholog search for miRNAs 
 Home-page: https://github.com/felixlangschied/ncortho
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncOrtho-0.4.0/ncOrtho.egg-info/SOURCES.txt` & `ncOrtho-0.4.1/ncOrtho.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.4.0/setup.py` & `ncOrtho-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncOrtho",
-    version="0.4.0",
+    version="0.4.1",
     python_requires='>=3.7.0',
     description=" Targeted ortholog search for miRNAs ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     url="https://github.com/felixlangschied/ncortho",
```

