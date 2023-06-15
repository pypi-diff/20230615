# Comparing `tmp/current_events_magnifier-0.0.1.tar.gz` & `tmp/current_events_magnifier-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/current_events_magnifier-0.0.1.tar", last modified: Wed Jun 14 12:09:07 2023, max compression
+DOS/MBR boot sector; partition 1 : ID=0xdf, active 0x98, start-CHS (0x32,229,62), end-CHS (0x128,14,2), startsector 3408066016, 3315601777 sectors; partition 2 : ID=0x39, active 0xfa, start-CHS (0x26,80,53), end-CHS (0x80,163,49), startsector 1952562441, 1681261935 sectors
```

## Comparing `current_events_magnifier-0.0.1.tar` & `current_events_magnifier-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:09:07.730323 current_events_magnifier-0.0.1/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.1/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6018 2023-06-14 12:09:07.730323 current_events_magnifier-0.0.1/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5408 2023-06-14 11:16:12.000000 current_events_magnifier-0.0.1/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:09:07.730323 current_events_magnifier-0.0.1/current_events_magnifier/
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     5889 2023-06-14 11:45:23.000000 current_events_magnifier-0.0.1/current_events_magnifier/CE_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:01:39.000000 current_events_magnifier-0.0.1/current_events_magnifier/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.1/current_events_magnifier/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.1/current_events_magnifier/cem_utils.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.1/current_events_magnifier/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7556 2023-06-14 11:49:38.000000 current_events_magnifier-0.0.1/current_events_magnifier/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.1/current_events_magnifier/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.1/current_events_magnifier/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:09:07.730323 current_events_magnifier-0.0.1/current_events_magnifier.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6018 2023-06-14 12:09:07.000000 current_events_magnifier-0.0.1/current_events_magnifier.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      600 2023-06-14 12:09:07.000000 current_events_magnifier-0.0.1/current_events_magnifier.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-14 12:09:07.000000 current_events_magnifier-0.0.1/current_events_magnifier.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-14 12:09:07.000000 current_events_magnifier-0.0.1/current_events_magnifier.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-14 12:09:07.000000 current_events_magnifier-0.0.1/current_events_magnifier.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-14 12:09:07.730323 current_events_magnifier-0.0.1/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1092 2023-06-14 12:09:03.000000 current_events_magnifier-0.0.1/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 08:28:59.615149 current_events_magnifier-0.0.2/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 current_events_magnifier-0.0.2/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6018 2023-06-15 08:28:59.615149 current_events_magnifier-0.0.2/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5408 2023-06-14 11:16:12.000000 current_events_magnifier-0.0.2/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 08:28:59.615149 current_events_magnifier-0.0.2/current_events_magnifier/
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     6268 2023-06-15 02:13:38.000000 current_events_magnifier-0.0.2/current_events_magnifier/CE_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2023-06-14 12:01:39.000000 current_events_magnifier-0.0.2/current_events_magnifier/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 current_events_magnifier-0.0.2/current_events_magnifier/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 current_events_magnifier-0.0.2/current_events_magnifier/cem_utils.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 current_events_magnifier-0.0.2/current_events_magnifier/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7556 2023-06-14 11:49:38.000000 current_events_magnifier-0.0.2/current_events_magnifier/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9027 2023-06-14 10:46:36.000000 current_events_magnifier-0.0.2/current_events_magnifier/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13168 2023-06-14 12:00:50.000000 current_events_magnifier-0.0.2/current_events_magnifier/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-06-15 08:28:59.615149 current_events_magnifier-0.0.2/current_events_magnifier.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6018 2023-06-15 08:28:59.000000 current_events_magnifier-0.0.2/current_events_magnifier.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      600 2023-06-15 08:28:59.000000 current_events_magnifier-0.0.2/current_events_magnifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-06-15 08:28:59.000000 current_events_magnifier-0.0.2/current_events_magnifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       98 2023-06-15 08:28:59.000000 current_events_magnifier-0.0.2/current_events_magnifier.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       25 2023-06-15 08:28:59.000000 current_events_magnifier-0.0.2/current_events_magnifier.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-06-15 08:28:59.615149 current_events_magnifier-0.0.2/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1092 2023-06-15 08:28:37.000000 current_events_magnifier-0.0.2/setup.py
```

### Comparing `current_events_magnifier-0.0.1/LICENSE` & `current_events_magnifier-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.1/PKG-INFO` & `current_events_magnifier-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current_events_magnifier
-Version: 0.0.1
+Version: 0.0.2
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.1/README.md` & `current_events_magnifier-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.1/current_events_magnifier/CE_magnifier.py` & `current_events_magnifier-0.0.2/current_events_magnifier/CE_magnifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 #!/usr/bin/env python
 import argparse
 import os
 from current_events_magnifier.cem_utils import read_fasta_to_dic,reverse_fasta
 import pandas as pd
 from current_events_magnifier.plot import signal_plot
+from plotnine.exceptions import PlotnineWarning
+import warnings
+warnings.filterwarnings("ignore", category=PlotnineWarning)
+
 def init_parser():
     def add_public_argument(parser_input):
         parser_input.add_argument("--chrom", required=True, help="Gene or chromosome name(head of your fasta file)")
         parser_input.add_argument("--pos", required=True, type=int, help="site of your interest")
         parser_input.add_argument("--len", default=10, type=int, help="region around the position")
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument("--ref", required=True, help="fasta file")
@@ -45,15 +49,20 @@
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
 
     args.pos = args.pos - 1
     subsample_num = args.overplot_number
     fasta = read_fasta_to_dic(args.ref)
+    # length filter
+    length_gene = len(fasta[args.chrom])
+    if args.pos + args.len + 1 >= length_gene or args.pos - args.len <= 0:
+        raise Exception("The position requested is too close to the border (pos-len>0 and pos+len<length of fasta)")
     base_list = fasta[args.chrom][args.pos - args.len:args.pos + args.len + 1]
+
     if args.strand == '-':
         base_list = "".join(list(reversed(base_list)))
         base_list = reverse_fasta(base_list)
     results_path = args.output
     if not os.path.exists(results_path):
         os.mkdir(results_path)
```

### Comparing `current_events_magnifier-0.0.1/current_events_magnifier/cem_utils.py` & `current_events_magnifier-0.0.2/current_events_magnifier/cem_utils.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.1/current_events_magnifier/normalization.py` & `current_events_magnifier-0.0.2/current_events_magnifier/normalization.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.1/current_events_magnifier/plot.py` & `current_events_magnifier-0.0.2/current_events_magnifier/plot.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.1/current_events_magnifier/read_f5c_resquiggle.py` & `current_events_magnifier-0.0.2/current_events_magnifier/read_f5c_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.1/current_events_magnifier/read_tombo_resquiggle.py` & `current_events_magnifier-0.0.2/current_events_magnifier/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.1/current_events_magnifier.egg-info/PKG-INFO` & `current_events_magnifier-0.0.2/current_events_magnifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: current-events-magnifier
-Version: 0.0.1
+Version: 0.0.2
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `current_events_magnifier-0.0.1/current_events_magnifier.egg-info/SOURCES.txt` & `current_events_magnifier-0.0.2/current_events_magnifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `current_events_magnifier-0.0.1/setup.py` & `current_events_magnifier-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="current_events_magnifier",
-    version="0.0.1",
+    version="0.0.2",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

