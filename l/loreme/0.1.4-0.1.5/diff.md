# Comparing `tmp/loreme-0.1.4.tar.gz` & `tmp/loreme-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loreme-0.1.4.tar", last modified: Wed Jun 14 05:06:06 2023, max compression
+gzip compressed data, was "loreme-0.1.5.tar", last modified: Thu Jun 15 18:32:59 2023, max compression
```

## Comparing `loreme-0.1.4.tar` & `loreme-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-14 05:06:06.869357 loreme-0.1.4/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.4/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-06-14 05:06:06.869016 loreme-0.1.4/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.4/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-14 05:06:06.821605 loreme-0.1.4/loreme.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-14 05:06:06.000000 loreme-0.1.4/loreme.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-14 04:51:11.000000 loreme-0.1.4/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-14 05:06:06.869778 loreme-0.1.4/setup.cfg
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-14 05:06:06.811983 loreme-0.1.4/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-14 05:06:06.868207 loreme-0.1.4/src/loreme/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/check_gpu_availability.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/check_tags.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/dorado.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5921 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3602 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/export_bedgraph.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/gene_body_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/intersect.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    37347 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/loreme.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5191 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/mean.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/merge.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/methylation_hist.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/modkit.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/parse_gff.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/pbcpg.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6487 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/plot.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2440 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/plot_bedtools.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/plot_genes.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/plot_repeats.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/promoter_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-14 04:51:11.000000 loreme-0.1.4/src/loreme/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-15 18:32:59.075977 loreme-0.1.5/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-14 04:51:11.000000 loreme-0.1.5/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-06-15 18:32:59.075378 loreme-0.1.5/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4730 2023-06-14 04:58:53.000000 loreme-0.1.5/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-15 18:32:58.873185 loreme-0.1.5/loreme.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5245 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-15 18:32:58.000000 loreme-0.1.5/loreme.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-14 05:34:47.000000 loreme-0.1.5/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-15 18:32:59.077527 loreme-0.1.5/setup.cfg
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-15 18:32:58.800566 loreme-0.1.5/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-15 18:32:59.074226 loreme-0.1.5/src/loreme/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/check_gpu_availability.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/check_tags.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/dorado.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6063 2023-06-15 18:05:04.000000 loreme-0.1.5/src/loreme/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3907 2023-06-15 18:07:10.000000 loreme-0.1.5/src/loreme/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/export_bedgraph.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/gene_body_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/intersect.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    37390 2023-06-15 18:22:10.000000 loreme-0.1.5/src/loreme/loreme.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5235 2023-06-14 05:31:42.000000 loreme-0.1.5/src/loreme/mean.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/merge.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/methylation_hist.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/modkit.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/parse_gff.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/pbcpg.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6531 2023-06-14 05:32:28.000000 loreme-0.1.5/src/loreme/plot.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2483 2023-06-14 05:33:30.000000 loreme-0.1.5/src/loreme/plot_bedtools.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/plot_genes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/plot_repeats.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-14 04:51:11.000000 loreme-0.1.5/src/loreme/promoter_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-14 05:34:58.000000 loreme-0.1.5/src/loreme/version.py
```

### Comparing `loreme-0.1.4/LICENSE` & `loreme-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/PKG-INFO` & `loreme-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.4/README.md` & `loreme-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/loreme.egg-info/PKG-INFO` & `loreme-0.1.5/loreme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loreme
-Version: 0.1.4
+Version: 0.1.5
 Summary: Extract Methylation calls from ONT or PB long read data
 Author-email: Anthony Aylward <aaylward@salk.edu>
 Project-URL: Homepage, https://gitlab.com/salk-tm/loreme
 Project-URL: Documentation, https://salk-tm.gitlab.io/loreme
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `loreme-0.1.4/loreme.egg-info/SOURCES.txt` & `loreme-0.1.5/loreme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/pyproject.toml` & `loreme-0.1.5/pyproject.toml`

 * *Files identical despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loreme"
-version = "0.1.4" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.1.5" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
     { name="Anthony Aylward", email="aaylward@salk.edu" },
 ]
 description = "Extract Methylation calls from ONT or PB long read data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `loreme-0.1.4/src/loreme/__init__.py` & `loreme-0.1.5/src/loreme/__init__.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/check_gpu_availability.py` & `loreme-0.1.5/src/loreme/check_gpu_availability.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/dorado.py` & `loreme-0.1.5/src/loreme/dorado.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/download.py` & `loreme-0.1.5/src/loreme/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import shutil
 import os
 import os.path
 import ftplib
 import gzip
 import tarfile
 import subprocess
+import json
 from itertools import product
 from loreme.env import (PBCPG_URL, PBCPG_DIR, EXAMPLE_DATA_URLS, EXAMPLE_DATA_DIR, HG38_FTP,
                        HG38_GENOME_PATH, HG38_ANNOT_PATH, DORADO_DIR, DORADO_URL, DORADO_URL_024,
-                       DORADO_MODEL_DIR, DORADO_PATH_024, MODKIT_URL, MODKIT_DIR)
+                       DORADO_MODEL_DIR, DORADO_CONFIG, DORADO_PATH_024, MODKIT_URL, MODKIT_DIR)
 
 def download_pbcpg(directory: str = PBCPG_DIR):
     """Download pb-CpG-tools
 
     Parameters
     ----------
     directory : str
@@ -70,15 +71,16 @@
         if os.path.exists(file_path):
             print(f'destination {file_path} already exists')
             continue
         with http.request('GET', example_data_url, preload_content=False) as r, open(file_path, 'wb') as out_file:
             shutil.copyfileobj(r, out_file)
 
 
-def download_dorado(pfm, directory: str = DORADO_DIR, model_dir: str = DORADO_MODEL_DIR):
+def download_dorado(pfm, directory=DORADO_DIR, model_dir=DORADO_MODEL_DIR,
+                    dorado_config=DORADO_CONFIG):
     """Download dorado
 
     Parameters
     ----------
     pfm : str
         platform string (linux-x86, linux-arm64, osx-arm64, win64)
     directory : str
@@ -113,14 +115,16 @@
     #     subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
     #         '--model', f'dna_r10.4.1_e8.2_400bps_{accuracy}@v4.2.0'))
     #     subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
     #         '--model', f'dna_r10.4.1_e8.2_400bps_{accuracy}@v4.2.0_5mCG_5hmCG@v2'))
     # for modified_bases in '5mC', '6mA':
     #     subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
     #         '--model', f'dna_r10.4.1_e8.2_400bps_sup@v4.2.0_{modified_bases}@v2'))
+    with open(dorado_config, 'w') as f:
+        json.dump({'platform': pfm}, f)
 
 def download_modkit(directory: str = MODKIT_DIR):
     """Download pb-CpG-tools
 
     Parameters
     ----------
     directory : str
```

### Comparing `loreme-0.1.4/src/loreme/env.py` & `loreme-0.1.5/src/loreme/env.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import os.path
+import json
 
 PBCPG_DIR = os.environ.get('LOREME_PBCPG_DIR',
     os.path.join(os.path.dirname(__file__)))
 PBCPG_PATH = os.path.join(PBCPG_DIR, 'pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu',
                          'bin', 'aligned_bam_to_cpg_scores')
 PBCPG_MODEL = os.path.join(PBCPG_DIR, 'pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu',
                                'models', 'pileup_calling_model.v1.tflite')
@@ -17,15 +18,22 @@
 HG38_FTP = 'ftp.ncbi.nlm.nih.gov'
 HG38_GENOME_PATH = 'genomes/all/GCA/000/001/405/GCA_000001405.15_GRCh38/seqs_for_alignment_pipelines.ucsc_ids/GCA_000001405.15_GRCh38_no_alt_analysis_set.fna.gz'
 HG38_ANNOT_PATH = 'genomes/all/GCA/000/001/405/GCA_000001405.15_GRCh38/seqs_for_alignment_pipelines.ucsc_ids/GCA_000001405.15_GRCh38_full_analysis_set.refseq_annotation.gff.gz'
 EXAMPLE_DATA_DIR = os.environ.get('LOREME_EXAMPLE_DATA_DIR', os.path.dirname(__file__))
 
 DORADO_DIR = os.environ.get('LOREME_DORADO_DIR',
     os.path.join(os.path.dirname(__file__)))
-DORADO_PLATFORM = os.environ.get('LOREME_DORADO_PLATFORM')
+DORADO_CONFIG = os.environ.get('LOREME_DORADO_CONFIG',
+    os.path.join(os.path.dirname(__file__), 'dorado-config.json'))
+if os.path.isfile(DORADO_CONFIG):
+    with open(DORADO_CONFIG, 'r') as f:
+        dorado_config = json.load(f)
+else:
+    dorado_config = {}
+DORADO_PLATFORM = os.environ.get('LOREME_DORADO_PLATFORM', dorado_config.get('platform'))
 DORADO_PATH = {
     'linux-x64': os.path.join(DORADO_DIR, 'dorado-0.3.0-linux-x64', 'bin', 'dorado'),
     'linux-arm64': os.path.join(DORADO_DIR, 'dorado-0.3.0-linux-arm64', 'bin', 'dorado'),
     'osx-arm64': os.path.join(DORADO_DIR, 'dorado-0.3.0-osx-arm64', 'bin', 'dorado'),
     'win64': os.path.join(DORADO_DIR, 'dorado-0.3.0-win64', 'bin', 'dorado')
 }
 DORADO_PATH_024 = {
```

### Comparing `loreme-0.1.4/src/loreme/export_bedgraph.py` & `loreme-0.1.5/src/loreme/export_bedgraph.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/gene_body_methylation.py` & `loreme-0.1.5/src/loreme/gene_body_methylation.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/intersect.py` & `loreme-0.1.5/src/loreme/intersect.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/loreme.py` & `loreme-0.1.5/src/loreme/loreme.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,16 @@
                     coverage=args.coverage)
 
 def clean(args):
     for root in args.dirs:
         for file in ('pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu.tar.gz',
                      'dorado-0.2.4-linux-x64.tar.gz',
                      'dorado-0.3.0-linux-x64.tar.gz',
-                     'modkit_v0.1.8_centos7_x86_64.tar.gz'):
+                     'modkit_v0.1.8_centos7_x86_64.tar.gz',
+                     'dorado-config.json'):
             if os.path.isfile(os.path.join(root, file)):
                 os.remove(os.path.join(root, file))
         for directory in ('pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu/',
                           f'dorado-0.2.4-{DORADO_PLATFORM}/',
                           f'dorado-0.3.0-{DORADO_PLATFORM}/',
                           'dna_r10.4.1_e8.2_260bps_fast@v4.1.0/',
                           'dna_r10.4.1_e8.2_260bps_hac@v4.1.0/',
```

### Comparing `loreme-0.1.4/src/loreme/mean.py` & `loreme-0.1.5/src/loreme/mean.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,17 @@
         ((chrom, methylation_level), group)
     """
     if chromosomes is not None:
         chromosomes = set(chromosomes)
     for bt, g in zip(bedtools, groups):
         for i in bt:
             n_fields = len(i.fields)
-            if n_fields == 11:
-                chrom, _, _, _, _, _, _, _, _, _, meth, group = i.fields + [g]
+            if n_fields == 10:
+                chrom, _, _, _, _, _, _, _, _, meth_col, group = i.fields + [g]
+                meth = meth_col.split()[1]
             elif n_fields == 9:
                 chrom, _, _, meth, _, _, _, _, _, group = i.fields + [g]
             else:
                 raise RuntimeError('Invalid methylation BED file')
             if (chromosomes is None) or (chrom in chromosomes):
                 yield chrom, float(meth), group
```

### Comparing `loreme-0.1.4/src/loreme/merge.py` & `loreme-0.1.5/src/loreme/merge.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/methylation_hist.py` & `loreme-0.1.5/src/loreme/methylation_hist.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/parse_gff.py` & `loreme-0.1.5/src/loreme/parse_gff.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/pbcpg.py` & `loreme-0.1.5/src/loreme/pbcpg.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/plot.py` & `loreme-0.1.5/src/loreme/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,17 @@
     tuple
         bin coordinate, value, and group ID of a methylation data point
     """
 
     for bt, g in zip(bedtools, groups):
         for i in bt:
             n_fields = len(i.fields)
-            if n_fields == 11:
-                chrom, _, pos, _, _, _, _, _, _, _, meth, group = i.fields + [g]
+            if n_fields == 10:
+                chrom, _, pos, _, _, _, _, _, _, meth_col, group = i.fields + [g]
+                meth = meth_col.split()[1]
             elif n_fields == 9:
                 chrom, _, pos, meth, _, _, _, _, _, group = i.fields + [g]
             else:
                 raise RuntimeError('Invalid methylation BED file')
             yield (min(round(int(pos), -6-bin_size), size)/size*scale + shift,
                 float(meth), group, f'{group}_{chrom}')
```

### Comparing `loreme-0.1.4/src/loreme/plot_bedtools.py` & `loreme-0.1.5/src/loreme/plot_bedtools.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,17 @@
     tuple
     """
 
     if chromosomes is not None:
         chromosomes = set(chromosomes)
     for i in bedtool:
         n_fields = len(i.fields)
-        if n_fields == 17:
-            chrom, _, _, _, _, _, _, _, _, coverage, meth, _, start, end, strand, gene, _ = i.fields
+        if n_fields == 16:
+            chrom, _, _, _, _, _, _, _, _, coverage, meth_col, _, start, end, strand, gene, _ = i.fields
+            meth = meth_col.split()[1]
         elif n_fields == 15:
             chrom, _, _, meth, _, coverage, _, _, _, _, start, end, strand, gene, _ = i.fields
         else:
             raise RuntimeError('Invalid methylation BED file')
         if (chromosomes is None) or (chrom in chromosomes):
             yield chrom, int(start), int(end), gene, strand, 1, int(coverage), float(meth)
```

### Comparing `loreme-0.1.4/src/loreme/plot_genes.py` & `loreme-0.1.5/src/loreme/plot_genes.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/plot_repeats.py` & `loreme-0.1.5/src/loreme/plot_repeats.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.4/src/loreme/promoter_methylation.py` & `loreme-0.1.5/src/loreme/promoter_methylation.py`

 * *Files identical despite different names*

