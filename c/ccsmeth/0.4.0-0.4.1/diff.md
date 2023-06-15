# Comparing `tmp/ccsmeth-0.4.0.tar.gz` & `tmp/ccsmeth-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccsmeth-0.4.0.tar", last modified: Thu Jun  8 06:50:24 2023, max compression
+gzip compressed data, was "ccsmeth-0.4.1.tar", last modified: Thu Jun 15 02:59:35 2023, max compression
```

## Comparing `ccsmeth-0.4.0.tar` & `ccsmeth-0.4.1.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 06:50:24.398489 ccsmeth-0.4.0/
--rw-rw-rw-   0        0        0     1683 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2405 2023-06-08 06:50:24.398489 ccsmeth-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1594 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-08 06:50:24.369586 ccsmeth-0.4.0/ccsmeth/
--rw-rw-rw-   0        0        0        0 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/__init__.py
--rw-rw-rw-   0        0        0    15258 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/_bam2modbam.py
--rw-rw-rw-   0        0        0    16985 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/_call_modifications_txt.py
--rw-rw-rw-   0        0        0       18 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/_version.py
--rw-rw-rw-   0        0        0     9673 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/align_hifi_reads.py
--rw-rw-rw-   0        0        0     5907 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/call_hifi_reads.py
--rw-rw-rw-   0        0        0    32638 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/call_modifications.py
--rw-rw-rw-   0        0        0    37997 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/call_mods_freq_bam.py
--rw-rw-rw-   0        0        0    18546 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/call_mods_freq_txt.py
--rw-rw-rw-   0        0        0    54821 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/ccsmeth.py
--rw-rw-rw-   0        0        0     6872 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/dataloader.py
--rw-rw-rw-   0        0        0    30220 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/extract_features.py
--rw-rw-rw-   0        0        0    10097 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/models.py
--rw-rw-rw-   0        0        0    20305 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/train.py
--rw-rw-rw-   0        0        0    25193 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/train_multigpu.py
-drwxrwxrwx   0        0        0        0 2023-06-08 06:50:24.397492 ccsmeth-0.4.0/ccsmeth/utils/
--rw-rw-rw-   0        0        0        0 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/__init__.py
--rw-rw-rw-   0        0        0     2801 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/attention.py
--rw-rw-rw-   0        0        0      756 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/constants_torch.py
--rw-rw-rw-   0        0        0     4077 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/lookahead.py
--rw-rw-rw-   0        0        0    13971 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/utils/process_utils.py
--rw-rw-rw-   0        0        0     9051 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/ranger2020.py
--rw-rw-rw-   0        0        0     2789 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/ref_reader.py
--rw-rw-rw-   0        0        0      963 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/sam2fastq_std.py
-drwxrwxrwx   0        0        0        0 2023-06-08 06:50:24.389520 ccsmeth-0.4.0/ccsmeth.egg-info/
--rw-rw-rw-   0        0        0     2405 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      888 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      134 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      152 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-06-08 06:50:24.403473 ccsmeth-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2034 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:59:35.924517 ccsmeth-0.4.1/
+-rw-rw-rw-   0        0        0     1683 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0       78 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2580 2023-06-15 02:59:35.924517 ccsmeth-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0    37330 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/README.md
+-rw-rw-rw-   0        0        0     1760 2023-06-14 03:55:29.000000 ccsmeth-0.4.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-15 02:59:35.869995 ccsmeth-0.4.1/ccsmeth/
+-rw-rw-rw-   0        0        0        0 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/__init__.py
+-rw-rw-rw-   0        0        0    15159 2023-06-14 03:55:29.000000 ccsmeth-0.4.1/ccsmeth/_bam2modbam.py
+-rw-rw-rw-   0        0        0    17064 2023-06-14 03:55:29.000000 ccsmeth-0.4.1/ccsmeth/_call_modifications_txt.py
+-rw-rw-rw-   0        0        0       18 2023-06-15 02:58:17.000000 ccsmeth-0.4.1/ccsmeth/_version.py
+-rw-rw-rw-   0        0        0     9678 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/align_hifi_reads.py
+-rw-rw-rw-   0        0        0     5915 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/call_hifi_reads.py
+-rw-rw-rw-   0        0        0    32340 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/call_modifications.py
+-rw-rw-rw-   0        0        0    38541 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/call_mods_freq_bam.py
+-rw-rw-rw-   0        0        0    18742 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/call_mods_freq_txt.py
+-rw-rw-rw-   0        0        0    54308 2023-06-14 03:55:29.000000 ccsmeth-0.4.1/ccsmeth/ccsmeth.py
+-rw-rw-rw-   0        0        0     6872 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/dataloader.py
+-rw-rw-rw-   0        0        0    29662 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/extract_features.py
+-rw-rw-rw-   0        0        0    10097 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/models.py
+-rw-rw-rw-   0        0        0    20359 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/train.py
+-rw-rw-rw-   0        0        0    25457 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/train_multigpu.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:59:35.923516 ccsmeth-0.4.1/ccsmeth/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/utils/__init__.py
+-rw-rw-rw-   0        0        0     2801 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/utils/attention.py
+-rw-rw-rw-   0        0        0      756 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/utils/constants_torch.py
+-rw-rw-rw-   0        0        0     1269 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/utils/logging.py
+-rw-rw-rw-   0        0        0     4077 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/utils/lookahead.py
+-rw-rw-rw-   0        0        0    14127 2023-06-14 11:25:49.000000 ccsmeth-0.4.1/ccsmeth/utils/process_utils.py
+-rw-rw-rw-   0        0        0     9051 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/utils/ranger2020.py
+-rw-rw-rw-   0        0        0     2789 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/utils/ref_reader.py
+-rw-rw-rw-   0        0        0      963 2023-06-04 08:15:25.000000 ccsmeth-0.4.1/ccsmeth/utils/sam2fastq_std.py
+drwxrwxrwx   0        0        0        0 2023-06-15 02:59:35.886008 ccsmeth-0.4.1/ccsmeth.egg-info/
+-rw-rw-rw-   0        0        0     2580 2023-06-15 02:59:35.000000 ccsmeth-0.4.1/ccsmeth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2023-06-15 02:59:35.000000 ccsmeth-0.4.1/ccsmeth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 02:59:35.000000 ccsmeth-0.4.1/ccsmeth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-15 02:59:35.000000 ccsmeth-0.4.1/ccsmeth.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 02:59:35.000000 ccsmeth-0.4.1/ccsmeth.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      134 2023-06-15 02:59:35.000000 ccsmeth-0.4.1/ccsmeth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 02:59:35.000000 ccsmeth-0.4.1/ccsmeth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      152 2023-06-12 08:51:43.000000 ccsmeth-0.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-06-15 02:59:35.928517 ccsmeth-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     2034 2023-06-08 06:45:58.000000 ccsmeth-0.4.1/setup.py
```

### Comparing `ccsmeth-0.4.0/LICENSE` & `ccsmeth-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.4.0/PKG-INFO` & `ccsmeth-0.4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ccsmeth
-Version: 0.4.0
+Version: 0.4.1
 Summary: Detecting DNA methylation from PacBio CCS reads
 Home-page: https://github.com/PengNi/ccsmeth
-Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.4.0.tar.gz
+Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.4.1.tar.gz
 Author: Peng Ni
 Author-email: 543943952@qq.com
 License: BSD-3-Clause-Clear license
 Keywords: methylation,pacbio,neural network
 Platform: Linux
 Platform: MacOS
 Classifier: Programming Language :: Python :: 3
@@ -18,16 +18,25 @@
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
 
 ccsmeth
 ========
 
 
-Documentation
+Changelog
 -------------
+v0.4.1
+----------
+handle ValueError when fetching bam items in call_freqb module
+
+change pytorch max version to 1.12.1
+
+using logging instead of print/sys.stderr.write
+
+
 v0.4.0
 ----------
 optimieze call_mods module, faster generating of modbam file
 
 
 v0.3.4
 ----------
```

### Comparing `ccsmeth-0.4.0/README.rst` & `ccsmeth-0.4.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 ccsmeth
 ========
 
 
-Documentation
+Changelog
 -------------
+v0.4.1
+----------
+handle ValueError when fetching bam items in call_freqb module
+
+change pytorch max version to 1.12.1
+
+using logging instead of print/sys.stderr.write
+
+
 v0.4.0
 ----------
 optimieze call_mods module, faster generating of modbam file
 
 
 v0.3.4
 ----------
```

### Comparing `ccsmeth-0.4.0/ccsmeth/_bam2modbam.py` & `ccsmeth-0.4.1/ccsmeth/_bam2modbam.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 import argparse
 import pysam
 import re
 import math
-import sys
 import time
 import tabix
 import pybedtools
 import gzip
 
 import multiprocessing as mp
 from multiprocessing import Queue
 
 from .utils.process_utils import complement_seq
 from .utils.process_utils import max_queue_size
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
+
 base = "C"
 pred_base = "CG"
 
 queue_size_border = max_queue_size
 time_wait = 1
 
 
@@ -134,15 +136,15 @@
             reads_batch = []
             while rreads_q.qsize() > queue_size_border:
                 time.sleep(time_wait)
     ori_bam.close()
     if len(reads_batch) > 0:
         rreads_q.put(reads_batch)
     rreads_q.put("kill")
-    sys.stderr.write("read {} reads from input file\n".format(cnt_all))
+    LOGGER.info("read {} reads from input file".format(cnt_all))
 
 
 def _convert_locstr(locstr):
     return [int(x) for x in locstr.split(",")]
 
 
 def _convert_probstr(probstr):
@@ -249,15 +251,15 @@
                 try:
                     mm_values = _convert_locs_to_mmtag(locs, seq_fwdseq)
                     ml_values = _convert_probs_to_mltag(probs)
                     mm_flag = 1
                 except AssertionError:
                     # sys.stderr.write("AssertionError, skip this alignment.\n"
                     #       "\tDetails: {}, {}, {}\n".format(seq_name, locs, probs))
-                    sys.stderr.write("AssertionError, skip this alignment-{}.\n".format(seq_name))
+                    LOGGER.warning("AssertionError, skip this alignment-{}.".format(seq_name))
                     continue
             new_tags = _refill_tags(all_tags, mm_values, ml_values, rm_pulse)
             wreads_tmp.append((seq_name, flag, ref_name, ref_start, mapq, cigartuples, rnext, pnext, tlen,
                                seq_seq, seq_qual, new_tags, mm_flag))
         if len(wreads_tmp) > 0:
             wreads_q.put(wreads_tmp)
             while wreads_q.qsize() > queue_size_border:
@@ -299,35 +301,34 @@
     while True:
         if wreads_q.empty():
             time.sleep(time_wait)
             continue
         wreads_batch = wreads_q.get()
         if wreads_batch == "kill":
             w_bam.close()
-            sys.stderr.write("write {} reads, in which {} were added mm tags\n".format(cnt_w,
-                                                                                       cnt_mm))
+            LOGGER.info("write {} reads, in which {} were added mm tags".format(cnt_w, cnt_mm))
             break
         for walignseg in wreads_batch:
             mm_flag = walignseg[-1]
             write_alignedsegment(walignseg, w_bam)
             cnt_w += 1
             cnt_mm += mm_flag
 
 
 def add_mm_ml_tags_to_bam(bamfile, per_readsite, modbamfile,
                           rm_pulse=True, threads=3,
                           reads_batch=100, mode="align"):
-    sys.stderr.write("[generate_modbam_file]starts\n")
-    sys.stderr.flush()
+    LOGGER.info("[generate_modbam_file]starts")
+    # sys.stderr.flush()
     start = time.time()
 
-    sys.stderr.write("generating per_read mod_calls..\n")
+    LOGGER.info("generating per_read mod_calls..")
     per_read_file = _generate_sorted_per_read_calls(per_readsite, None)
 
-    sys.stderr.write("add per_read mod_calls to bam file..\n")
+    LOGGER.info("add per_read mod_calls to bam file..")
     rreads_q = Queue()
     wreads_q = Queue()
 
     nproc = threads
     if nproc < 5:
         nproc = 5
     if nproc > 8:
@@ -362,33 +363,33 @@
         p.join()
     p_read.join()
     wreads_q.put("kill")
     p_w.join()
 
     if modbamfile.endswith(".bam"):
         try:
-            sys.stderr.write("sorting modbam file..\n")
+            LOGGER.info("sorting modbam file..")
             modbam_sorted = os.path.splitext(modbamfile)[0] + ".sorted.bam"
             pysam.sort("-o", modbam_sorted, "-@", str(threads), modbamfile)
             os.rename(modbam_sorted, modbamfile)
         except Exception:
-            sys.stderr.write("failed sorting modbam file..\n")
+            LOGGER.warning("failed sorting modbam file..")
         try:
-            sys.stderr.write("indexing modbam file..\n")
+            LOGGER.info("indexing modbam file..")
             pysam.index("-@", str(threads), modbamfile)
         except Exception:
-            sys.stderr.write("failed indexing modbam file..\n")
+            LOGGER.warning("failed indexing modbam file..")
 
     if os.path.exists(per_read_file):
         os.remove(per_read_file)
     if os.path.exists(per_read_file + ".tbi"):
         os.remove(per_read_file + ".tbi")
 
     endtime = time.time()
-    sys.stderr.write("[generate_modbam_file]costs {:.1f} seconds\n".format(endtime - start))
+    LOGGER.info("[generate_modbam_file]costs {:.1f} seconds".format(endtime - start))
 
 
 def main():
     parser = argparse.ArgumentParser("add MM/ML tags to bam/sam")
     parser.add_argument("--per_readsite", type=str, required=True, help="from call_mods module")
     parser.add_argument("--bam", type=str, required=True, help="input bam file")
```

### Comparing `ccsmeth-0.4.0/ccsmeth/_call_modifications_txt.py` & `ccsmeth-0.4.1/ccsmeth/_call_modifications_txt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 call modifications from bam/sam files or extracted features.
 output format: chromosome, pos, strand, read_name, read_loc, depth,
 prob_0, prob_1, called_label, seq
 """
 
 import os
-import sys
 
 import numpy as np
 import torch
 import torch.multiprocessing as mp
 
 import gzip
 
@@ -34,14 +33,17 @@
 from .utils.process_utils import nproc_to_call_mods_in_cpu_mode
 from .utils.process_utils import str2bool
 from .utils.process_utils import max_queue_size
 
 from .utils.constants_torch import FloatTensor
 from .utils.constants_torch import use_cuda
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
+
 # add this export temporarily
 # https://github.com/pytorch/pytorch/issues/37377
 os.environ['MKL_THREADING_LAYER'] = 'GNU'
 
 queue_size_border = max_queue_size
 time_wait = 1
 
@@ -64,22 +66,22 @@
             h_num += 1
     h_num += 1
     infile.close()
     return h_num
 
 
 def _read_features_file_to_str(features_file, featurestrs_batch_q, holes_batch=50):
-    print("read_features process-{} starts".format(os.getpid()))
+    LOGGER.info("read_features process-{} starts".format(os.getpid()))
     h_num_total = _count_holenum(features_file)
     hbatch_num = h_num_total // holes_batch
     if h_num_total % holes_batch > 0:
         hbatch_num += 1
-    print("read_features process-{} - generate {} hole/read batches({})\n".format(os.getpid(),
-                                                                                  hbatch_num,
-                                                                                  holes_batch))
+    LOGGER.info("read_features process-{} - generate {} hole/read batches({})".format(os.getpid(),
+                                                                                      hbatch_num,
+                                                                                      holes_batch))
 
     h_num = 0
     hbatch_num_got = 0
     preholeid = None
     if features_file.endswith(".gz"):
         infile = gzip.open(features_file, 'rt')
     else:
@@ -107,22 +109,22 @@
         h_num += 1
         if len(featurestrs) > 0:
             featurestrs_batch_q.put(featurestrs)
             pbar.update(1)
             hbatch_num_got += 1
         assert hbatch_num_got == hbatch_num
     featurestrs_batch_q.put("kill")
-    print("read_features process-{} ending, read {} reads/holes batches({})".format(os.getpid(),
-                                                                                    hbatch_num_got,
-                                                                                    holes_batch))
+    LOGGER.info("read_features process-{} ending, read {} reads/holes batches({})".format(os.getpid(),
+                                                                                          hbatch_num_got,
+                                                                                          holes_batch))
 
 
 def _format_features_from_strbatch2s(featurestrs_batch_q, features_batch_q, seq_len,
                                      holeids_e, holeids_ne):
-    print("format_features process-{} starts".format(os.getpid()))
+    LOGGER.info("format_features process-{} starts".format(os.getpid()))
     b_num = 0
     while True:
         if featurestrs_batch_q.empty():
             time.sleep(time_wait)
             continue
         featurestrs = featurestrs_batch_q.get()
         if featurestrs == "kill":
@@ -193,15 +195,15 @@
 
             labels.append(int(words[21]))
 
         features_batch_q.put((sampleinfo, fkmers, fpasss, fipdms, fipdsds, fpwms, fpwsds, fquals, fmaps,
                               rkmers, rpasss, ripdms, ripdsds, rpwms, rpwsds, rquals, rmaps, labels))
         while features_batch_q.qsize() > queue_size_border:
             time.sleep(time_wait)
-    print("format_features process-{} ending, read {} batches".format(os.getpid(), b_num))
+    LOGGER.info("format_features process-{} ending, read {} batches".format(os.getpid(), b_num))
 
 
 # call mods =============================================================
 def _call_mods2s(features_batch, model, batch_size, device=0):
     sampleinfo, fkmers, fpasss, fipdms, fipdsds, fpwms, fpwsds, fquals, fmaps, \
         rkmers, rpasss, ripdms, ripdsds, rpwms, rpwsds, rquals, rmaps, labels = features_batch
     labels = np.reshape(labels, (len(labels)))
@@ -263,15 +265,15 @@
                                            b_idx_kmer[bkmer_start:bkmer_end]]))
             batch_num += 1
 
     return pred_str, batch_num
 
 
 def _call_mods_q(model_path, features_batch_q, pred_str_q, args, device=0):
-    print('call_mods process-{} starts'.format(os.getpid()))
+    LOGGER.info('call_mods process-{} starts'.format(os.getpid()))
     if args.model_type in {"attbigru2s", "attbilstm2s"}:
         model = ModelAttRNN(args.seq_len, args.layer_rnn, args.class_num,
                             args.dropout_rate, args.hid_rnn,
                             args.n_vocab, args.n_embed,
                             is_qual=str2bool(args.is_qual),
                             is_map=str2bool(args.is_map),
                             is_stds=str2bool(args.is_stds),
@@ -283,29 +285,27 @@
 
     try:
         para_dict = torch.load(model_path, map_location=torch.device('cpu'))
         # para_dict = torch.load(model_path, map_location=torch.device(device))
         model_dict = model.state_dict()
         model_dict.update(para_dict)
         model.load_state_dict(model_dict)
-        if str2bool(args.loginfo):
-            print('call_mods process-{} loads model param successfully'.format(os.getpid()))
+        LOGGER.debug('call_mods process-{} loads model param successfully'.format(os.getpid()))
         del model_dict
     except RuntimeError:
         # for DDP model convertion (key: module.embed.weight -> embed.weight)
         from collections import OrderedDict
         para_dict = torch.load(model_path, map_location=torch.device('cpu'))
         para_dict_new = OrderedDict()
         for param_tensor in para_dict.keys():
             para_dict_new[param_tensor[7:]] = para_dict[param_tensor]
         model.load_state_dict(para_dict_new)
-        if str2bool(args.loginfo):
-            print('call_mods process-{} loads model param successfully-1'.format(os.getpid()))
+        LOGGER.debug('call_mods process-{} loads model param successfully-1'.format(os.getpid()))
         del para_dict_new
-    sys.stdout.flush()
+    # sys.stdout.flush()
 
     if use_cuda:
         model = model.cuda(device)
     model.eval()
 
     batch_num_total = 0
     while True:
@@ -327,35 +327,35 @@
         pred_str_q.put(pred_str)
         while pred_str_q.qsize() > queue_size_border:
             time.sleep(time_wait)
         # for debug
         # print("call_mods process-{} reads 1 batch, features_batch_q:{}, "
         #       "pred_str_q: {}".format(os.getpid(), features_batch_q.qsize(), pred_str_q.qsize()))
         batch_num_total += batch_num
-    print('call_mods process-{} ending, proceed {} batches({})'.format(os.getpid(), batch_num_total,
-                                                                       args.batch_size))
+    LOGGER.info('call_mods process-{} ending, proceed {} batches({})'.format(os.getpid(), batch_num_total,
+                                                                             args.batch_size))
 
 
 def _write_predstr_to_file(write_fp, predstr_q, is_gzip):
-    print('write_process-{} starts'.format(os.getpid()))
+    LOGGER.info('write_process-{} starts'.format(os.getpid()))
     if is_gzip:
         if not write_fp.endswith(".gz"):
             write_fp += ".gz"
         wf = gzip.open(write_fp, "wt")
     else:
         wf = open(write_fp, 'w')
     while True:
         # during test, it's ok without the sleep()
         if predstr_q.empty():
             time.sleep(time_wait)
             continue
         pred_str = predstr_q.get()
         if pred_str == "kill":
             wf.close()
-            print('write_process-{} finished'.format(os.getpid()))
+            LOGGER.info('write_process-{} finished'.format(os.getpid()))
             break
         for one_pred_str in pred_str:
             wf.write(one_pred_str + "\n")
         wf.flush()
 
 
 def _get_gpus():
@@ -380,15 +380,15 @@
     if use_cuda:
         if nproc_dp < 1:
             nproc_dp = 1
     else:
         if nproc_dp > nproc_to_call_mods_in_cpu_mode:
             nproc_dp = nproc_to_call_mods_in_cpu_mode
     if nproc < nproc_dp + 2:
-        print("--threads must be > --threads_call + 2!!")
+        LOGGER.warning("--threads must be > --threads_call + 2!!")
         nproc = nproc_dp + 2 + 1  # 1 for reading, 1 for writing, 1 for extracting
     nproc_cnvt = nproc - nproc_dp - 2
 
     p_read = mp.Process(target=_read_features_file_to_str, args=(input_path, featurestrs_batch_q,
                                                                     args.holes_batch))
     p_read.daemon = True
     p_read.start()
```

### Comparing `ccsmeth-0.4.0/ccsmeth/align_hifi_reads.py` & `ccsmeth-0.4.1/ccsmeth/align_hifi_reads.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
 import argparse
-import sys
 import time
 
 from .utils.process_utils import run_cmd
 from .utils.process_utils import display_args
 from .utils.process_utils import pbmm2_exec
 from .utils.process_utils import minimap2_exec
 from .utils.process_utils import bwa_exec
 from .utils.process_utils import generate_samtools_view_cmd
 from .utils.process_utils import generate_samtools_index_cmd
 from .utils.process_utils import generate_samtools_sort_cmd
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
 
 here = os.path.abspath(os.path.dirname(__file__))
 sam2fq_exec = "python " + here + "/utils/sam2fastq_std.py"
 
 
 def check_input_file(inputfile):
     if not (inputfile.endswith(".bam") or inputfile.endswith(".sam") or inputfile.endswith(".fq")
@@ -60,20 +61,20 @@
         aligner = bwa_exec
         if path_to_bwa is not None:
             aligner = os.path.abspath(path_to_bwa)
         aligner += " mem -x pacbio -C -V -t {t}".format(t=threads)
     else:
         if path_to_pbmm2 is not None:
             aligner = os.path.abspath(path_to_pbmm2)
-        aligner += " align --preset HIFI -j {t} --sort ".format(t=threads)
+        aligner += " align --preset CCS -j {t} --sort ".format(t=threads)
     return aligner
 
 
 def align_hifi_reads_to_genome(args):
-    sys.stderr.write("[align_hifi_reads]start..\n")
+    LOGGER.info("[main]align_hifi_reads starts")
     start = time.time()
     inputpath = check_input_file(args.hifireads)
     outputpath = check_output_file(args.output, inputpath, args.minimap2, args.bwa)
     reference = os.path.abspath(args.ref)
 
     if not os.path.exists(inputpath):
         raise IOError("input file does not exist!")
@@ -132,26 +133,26 @@
             pass
 
         if pre_align_cmds != "":
             align_cmds = " | ".join([pre_align_cmds, align_cmds])
         if post_align_cmds != "":
             align_cmds = " | ".join([align_cmds, post_align_cmds])
 
-    sys.stderr.write("cmds: {}\n".format(align_cmds))
+    LOGGER.info("cmds: {}".format(align_cmds))
     stdinfo, returncode = run_cmd(align_cmds)
     stdout, stderr = stdinfo
     if returncode:
-        sys.stderr.write("failed..\n")
+        LOGGER.warning("failed..")
     else:
-        sys.stderr.write("succeeded..\n")
-    sys.stderr.write("==stdout:\n{}\n".format(str(stdout, 'utf-8')))
-    sys.stderr.write("==stderr:\n{}\n".format(str(stderr, 'utf-8')))
+        LOGGER.info("succeeded..")
+    LOGGER.info("stdout:\n{}".format(str(stdout, 'utf-8')))
+    LOGGER.info("stderr:\n{}".format(str(stderr, 'utf-8')))
 
     endtime = time.time()
-    sys.stderr.write("[align_hifi_reads]costs {:.1f} seconds\n".format(endtime - start))
+    LOGGER.info("[main]align_hifi_reads costs {:.1f} seconds".format(endtime - start))
 
 
 def main():
     parser = argparse.ArgumentParser("align hifi reads using pbmm2/minimap2/bwa, default pbmm2")
     p_input = parser.add_argument_group("INPUT")
     p_input.add_argument("--hifireads", "-i", type=str, required=True,
                          help="path to hifireads.bam/sam/fastq_with_pulseinfo file as input")
@@ -193,13 +194,13 @@
                               "If not specified, it is assumed that samtools is in "
                               "the PATH.")
     p_align.add_argument("--threads", "-t", type=int, default=5, required=False,
                          help="number of threads, default 5")
 
     args = parser.parse_args()
 
-    display_args(args, True)
+    display_args(args)
     align_hifi_reads_to_genome(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ccsmeth-0.4.0/ccsmeth/call_hifi_reads.py` & `ccsmeth-0.4.1/ccsmeth/call_hifi_reads.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import argparse
-import sys
 import time
 
 from .utils.process_utils import run_cmd
 from .utils.process_utils import display_args
 from .utils.process_utils import ccs_exec
 from .utils.process_utils import generate_samtools_view_cmd
 from .utils.process_utils import generate_samtools_index_cmd
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
+
 
 def check_input_file(inputfile):
     if not inputfile.endswith(".bam"):
         raise ValueError("--subreads/-i must be in bam format!")
     inputpath = os.path.abspath(inputfile)
     return inputpath
 
@@ -43,15 +45,15 @@
         ccs_cmd += " --by-strand"
     if args.hd_finder:
         ccs_cmd += " --hd-finder"
     return ccs_cmd
 
 
 def ccs_call_hifi_reads(args):
-    sys.stderr.write("[call_hifi_reads]starts\n")
+    LOGGER.info("[main]call_hifi_reads starts")
     start = time.time()
     inputpath = check_input_file(args.subreads)
     if not os.path.exists(inputpath):
         raise IOError("input file does not exist!")
     outputpath = check_output_file(args.output, inputpath)
 
     ccscaller = generate_ccscmd_with_options(args)
@@ -68,26 +70,26 @@
         post_ccs_cmd = "echo '@SQ\tSN:chr\tLN:1' > {} && ".format(outputpath)
         post_ccs_cmd += " ".join([samtools_view, tmp_bam, " >>", outputpath])
         clean_cmd = " ".join(["rm", tmp_bam + "*"])
         ccs_cmds = " && ".join([ccs_cmds, post_ccs_cmd, clean_cmd])
     else:
         raise ValueError("--output/-o must be in bam/sam format!")
 
-    sys.stderr.write("cmds: {}\n".format(ccs_cmds))
+    LOGGER.info("cmds: {}".format(ccs_cmds))
     stdinfo, returncode = run_cmd(ccs_cmds)
     stdout, stderr = stdinfo
     if returncode:
-        sys.stderr.write("failed\n")
+        LOGGER.warning("failed")
     else:
-        sys.stderr.write("succeeded\n")
-    sys.stderr.write("==stdout:\n{}\n".format(str(stdout, 'utf-8')))
-    sys.stderr.write("==stderr:\n{}\n".format(str(stderr, 'utf-8')))
+        LOGGER.info("succeeded")
+    LOGGER.info("stdout:\n{}".format(str(stdout, 'utf-8')))
+    LOGGER.info("stderr:\n{}".format(str(stderr, 'utf-8')))
 
     endtime = time.time()
-    sys.stderr.write("[call_hifi_reads]costs {:.1f} seconds\n".format(endtime - start))
+    LOGGER.info("[main]call_hifi_reads costs {:.1f} seconds".format(endtime - start))
 
 
 def main():
     parser = argparse.ArgumentParser("call hifi reads with kinetics from subreads.bam using CCS, "
                                      "save in bam/sam format.\n"
                                      "  cmd: ccsmeth call_hifi -i input.subreads.bam")
     p_input = parser.add_argument_group("INPUT")
@@ -122,13 +124,13 @@
     parser.add_argument("--path_to_samtools", type=str, default=None, required=False,
                         help="full path to the executable binary samtools file. "
                              "If not specified, it is assumed that samtools is in "
                              "the PATH.")
 
     args = parser.parse_args()
 
-    display_args(args, True)
+    display_args(args)
     ccs_call_hifi_reads(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ccsmeth-0.4.0/ccsmeth/call_modifications.py` & `ccsmeth-0.4.1/ccsmeth/call_modifications.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 from .utils.process_utils import base2code_dna
 from .utils.process_utils import display_args
 from .utils.process_utils import nproc_to_call_mods_in_cpu_mode
 from .utils.process_utils import str2bool
 from .utils.process_utils import get_motif_seqs
 from .utils.process_utils import index_bam_if_needed2
-from .utils.process_utils import max_queue_size
+# from .utils.process_utils import max_queue_size
 from .utils.process_utils import complement_seq
 
 from .utils.ref_reader import DNAReference
 
 from .utils.constants_torch import FloatTensor
 from .utils.constants_torch import use_cuda
 
@@ -52,14 +52,17 @@
 from ._bam2modbam import _get_necessary_alignment_items
 from ._bam2modbam import _convert_locs_to_mmtag
 from ._bam2modbam import _convert_probs_to_mltag
 from ._bam2modbam import _refill_tags
 
 from ._version import VERSION
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
+
 # add this export temporarily
 # https://github.com/pytorch/pytorch/issues/37377
 os.environ['MKL_THREADING_LAYER'] = 'GNU'
 
 # queue_size_border = max_queue_size
 time_wait = 0.2
 
@@ -116,15 +119,15 @@
         labels.append(label)
     return sampleinfo, fkmers, fpasss, fipdms, fipdsds, fpwms, fpwsds, fquals, fmaps, \
         rkmers, rpasss, ripdms, ripdsds, rpwms, rpwsds, rquals, rmaps, labels
 
 
 def worker_extract_features_with_holeinfo(input_header, holebatch_q, features_q,
                                           motifs, holeids_e, holeids_ne, dnacontigs, args):
-    sys.stderr.write("extract_features process-{} starts\n".format(os.getpid()))
+    LOGGER.info("extract_features process-{} starts".format(os.getpid()))
 
     if isinstance(input_header, OrderedDict) or isinstance(input_header, dict):
         input_header2 = pysam.AlignmentHeader.from_dict(input_header)
     else:
         input_header2 = input_header
 
     cnt_holesbatch = 0
@@ -148,21 +151,21 @@
             feature_batch = _batch_feature_list2s(feature_list)
             features_oneholebatch = (holebatch, holeidxes, feature_batch)
             features_q.put(features_oneholebatch)
             # while features_q.qsize() > queue_size_border:
             while features_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
                 time.sleep(time_wait)
         cnt_holesbatch += 1
-    sys.stderr.write("extract_features process-{} ending, proceed {} "
-                     "hole_batches({}): {} holes/reads in total, "
-                     "{} skipped/failed.\n".format(os.getpid(),
-                                                   cnt_holesbatch,
-                                                   args.holes_batch,
-                                                   total_num_batch,
-                                                   failed_num_batch))
+    LOGGER.info("extract_features process-{} ending, proceed {} "
+                "hole_batches({}): {} holes/reads in total, "
+                "{} skipped/failed.".format(os.getpid(),
+                                            cnt_holesbatch,
+                                            args.holes_batch,
+                                            total_num_batch,
+                                            failed_num_batch))
 
 
 # call mods =============================================================
 def _call_mods2s(features_batch, model, batch_size, device=0):
     sampleinfo, fkmers, fpasss, fipdms, fipdsds, fpwms, fpwsds, fquals, fmaps, \
         rkmers, rpasss, ripdms, ripdsds, rpwms, rpwsds, rquals, rmaps, labels = features_batch
     labels = np.reshape(labels, (len(labels)))
@@ -251,15 +254,15 @@
         probs = locs_probs[1]
         mm_values = _convert_locs_to_mmtag(locs, seq_fwdseq)
         ml_values = _convert_probs_to_mltag(probs)
         mm_flag = 1
     except AssertionError:
         # sys.stderr.write("AssertionError, skip this alignment.\n"
         #       "\tDetails: {}, {}, {}\n".format(seq_name, locs, probs))
-        sys.stderr.write("AssertionError, skip this alignment-{}.\n".format(seq_name))
+        LOGGER.info("AssertionError, skip this alignment-{}.".format(seq_name))
     new_tags = _refill_tags(all_tags, mm_values, ml_values, rm_pulse)
     return (seq_name, flag, ref_name, ref_start, mapq, cigartuples, rnext, pnext, tlen,
             seq_seq, seq_qual, new_tags, mm_flag)
 
 
 def _add_modinfo2alignedseg_batch(holebatch, holeidxes, preds_info, input_header, rm_pulse):
     new_read_infos = []
@@ -302,15 +305,15 @@
             new_read_info = _add_modinfo2alignedseg(holebatch[idx], [], input_header, rm_pulse)
             new_read_infos.append(new_read_info)
     assert len(holebatch) == len(new_read_infos)
     return new_read_infos
 
 
 def _call_mods_q(model_path, features_batch_q, out_info_q, input_header, args, device=0):
-    print('call_mods process-{} starts'.format(os.getpid()))
+    LOGGER.info('call_mods process-{} starts'.format(os.getpid()))
     if args.model_type in {"attbigru2s", "attbilstm2s"}:
         model = ModelAttRNN(args.seq_len, args.layer_rnn, args.class_num,
                             args.dropout_rate, args.hid_rnn,
                             args.n_vocab, args.n_embed,
                             is_qual=str2bool(args.is_qual),
                             is_map=str2bool(args.is_map),
                             is_stds=str2bool(args.is_stds),
@@ -322,28 +325,26 @@
 
     try:
         para_dict = torch.load(model_path, map_location=torch.device('cpu'))
         # para_dict = torch.load(model_path, map_location=torch.device(device))
         model_dict = model.state_dict()
         model_dict.update(para_dict)
         model.load_state_dict(model_dict)
-        if str2bool(args.loginfo):
-            print('call_mods process-{} loads model param successfully'.format(os.getpid()))
+        LOGGER.debug('call_mods process-{} loads model param successfully'.format(os.getpid()))
         del model_dict
     except RuntimeError:
         # for DDP model convertion (key: module.embed.weight -> embed.weight)
         para_dict = torch.load(model_path, map_location=torch.device('cpu'))
         para_dict_new = OrderedDict()
         for param_tensor in para_dict.keys():
             para_dict_new[param_tensor[7:]] = para_dict[param_tensor]
         model.load_state_dict(para_dict_new)
-        if str2bool(args.loginfo):
-            print('call_mods process-{} loads model param successfully-1'.format(os.getpid()))
+        LOGGER.debug('call_mods process-{} loads model param successfully-1'.format(os.getpid()))
         del para_dict_new
-    sys.stdout.flush()
+    # sys.stdout.flush()
 
     if use_cuda:
         model = model.cuda(device)
     model.eval()
 
     if isinstance(input_header, OrderedDict) or isinstance(input_header, dict):
         input_header2 = pysam.AlignmentHeader.from_dict(input_header)
@@ -375,16 +376,16 @@
         # while out_info_q.qsize() > queue_size_border:
         while out_info_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
             time.sleep(time_wait)
         # for debug
         # print("call_mods process-{} reads 1 batch, features_batch_q:{}, "
         #       "pred_info_q: {}".format(os.getpid(), features_batch_q.qsize(), pred_info_q.qsize()))
         batch_num_total += batch_num
-    print('call_mods process-{} ending, proceed {} batches({})'.format(os.getpid(), batch_num_total,
-                                                                       args.batch_size))
+    LOGGER.info('call_mods process-{} ending, proceed {} batches({})'.format(os.getpid(), batch_num_total,
+                                                                             args.batch_size))
 
 
 # write modbam =============================================================
 def write_alignedsegment(readitem_info, output_bam):
     """
     Writes the readitem_info(tuple) to a bam file
     :param readitem_info:
@@ -426,16 +427,15 @@
     while True:
         if wreads_q.empty():
             time.sleep(time_wait)
             continue
         wreads_batch = wreads_q.get()
         if wreads_batch == "kill":
             w_bam.close()
-            sys.stderr.write("wrote {} reads, in which {} were added mm tags\n".format(cnt_w,
-                                                                                       cnt_mm))
+            LOGGER.info("wrote {} reads, in which {} were added mm tags".format(cnt_w, cnt_mm))
             break
         for walignseg in wreads_batch:
             mm_flag = walignseg[-1]
             write_alignedsegment(walignseg, w_bam)
             cnt_w += 1
             cnt_mm += mm_flag
 
@@ -446,17 +446,17 @@
         gpulist = list(range(num_gpus))
     else:
         gpulist = [0]
     return gpulist * 1000
 
 
 def call_mods(args):
-    print("[main]call_mods starts..")
+    LOGGER.info("[main]call_mods starts")
     start = time.time()
-    print("cuda availability: {}".format(use_cuda))
+    LOGGER.info("cuda availability: {}".format(use_cuda))
 
     torch.manual_seed(args.tseed)
     if use_cuda:
         torch.cuda.manual_seed(args.tseed)
 
     model_path = os.path.abspath(args.model_file)
     if not os.path.exists(model_path):
@@ -475,15 +475,15 @@
     holeids_ne = None if args.holeids_ne is None else _get_holes(args.holeids_ne)
 
     if input_path.endswith(".bam") or input_path.endswith(".sam"):
         if args.seq_len % 2 == 0:
             raise ValueError("--seq_len must be odd")
 
         if str2bool(args.is_map) and not str2bool(args.is_mapfea):
-            print("as --is_map is True, setting --is_mapfea as True")
+            LOGGER.info("as --is_map is True, setting --is_mapfea as True")
             args.is_mapfea = "yes"
 
         index_bam_if_needed2(input_path, args.threads)
 
         dnacontigs = None
         if args.mode == "align":
             if args.ref is None:
@@ -504,15 +504,15 @@
         if use_cuda:
             if nproc_dp < 1:
                 nproc_dp = 1
         else:
             if nproc_dp > nproc_to_call_mods_in_cpu_mode:
                 nproc_dp = nproc_to_call_mods_in_cpu_mode
         if nproc <= nproc_dp + 4:
-            print("--threads must be > --threads_call + 4!!")
+            LOGGER.warning("--threads must be > --threads_call + 4!!")
             nproc = nproc_dp + 4 + 1  # 2 for reading, 2 for writing, 1 for extracting
             threads_r, threads_w = 2, 2
         else:
             threads_r = 2
             if nproc - nproc_dp - threads_r >= 16:
                 threads_w = 4
             elif nproc - nproc_dp - threads_r >= 12:
@@ -565,34 +565,34 @@
             p.join()
         out_info_q.put("kill")
 
         p_w.join()
 
         if not args.no_sort:
             post_time_start = time.time()
-            print("[post_process] bam_sort_index starts..")
+            LOGGER.info("[post_process] bam_sort_index starts")
             try:
-                sys.stderr.write("sorting modbam file..\n")
+                LOGGER.info("sorting modbam file..")
                 modbam_sorted = os.path.splitext(out_modbam)[0] + ".sorted.bam"
                 pysam.sort("-o", modbam_sorted, "-@", str(args.threads), out_modbam)
                 os.rename(modbam_sorted, out_modbam)
             except Exception:
-                sys.stderr.write("failed sorting modbam file..\n")
+                LOGGER.warning("failed sorting modbam file..")
             try:
-                sys.stderr.write("indexing modbam file..\n")
+                LOGGER.info("indexing modbam file..")
                 pysam.index("-@", str(args.threads), out_modbam)
             except Exception:
-                sys.stderr.write("failed indexing modbam file..\n")
-            print("[post_process] bam_sort_index costs %.2f seconds.." % (time.time() - post_time_start))
+                LOGGER.warning("failed indexing modbam file..")
+            LOGGER.info("[post_process] bam_sort_index costs %.2f seconds" % (time.time() - post_time_start))
     else:
         from ._call_modifications_txt import call_mods_txt
         out_per_readsite = args.output + ".per_readsite.tsv"
         call_mods_txt(input_path, holeids_e, holeids_ne, out_per_readsite, model_path, args)
 
-    print("[main]call_mods costs %.2f seconds.." % (time.time() - start))
+    LOGGER.info("[main]call_mods costs %.2f seconds" % (time.time() - start))
 
 
 def main():
     parser = argparse.ArgumentParser("call modifications")
 
     p_input = parser.add_argument_group("INPUT")
     p_input.add_argument("--input", "-i", action="store", type=str,
@@ -669,27 +669,25 @@
                                 'the same')
     p_extract.add_argument("--mod_loc", action="store", type=int, required=False, default=0,
                            help='0-based location of the targeted base in the motif, default 0')
     p_extract.add_argument("--methy_label", action="store", type=int,
                            choices=[1, 0], required=False, default=1,
                            help="the label of the interested modified bases, this is for training."
                                 " 0 or 1, default 1")
-    p_extract.add_argument("--norm", action="store", type=str, choices=["zscore", "min-mean", "min-max", "mad"],
+    p_extract.add_argument("--norm", action="store", type=str, 
+                           choices=["zscore", "min-mean", "min-max", "mad", "none"],
                            default="zscore", required=False,
                            help="method for normalizing ipd/pw in subread level. "
-                                "zscore, min-mean, min-max or mad, default zscore")
+                                "zscore, min-mean, min-max, mad, or none. default zscore")
     p_extract.add_argument("--no_decode", action="store_true", default=False, required=False,
                            help="not use CodecV1 to decode ipd/pw")
     # p_extract.add_argument("--path_to_samtools", type=str, default=None, required=False,
     #                        help="full path to the executable binary samtools file. "
     #                             "If not specified, it is assumed that samtools is in "
     #                             "the PATH.")
-    p_extract.add_argument("--loginfo", type=str, default="no", required=False,
-                           help="if printing more info of feature extraction on reads. "
-                                "yes or no, default no")
 
     p_extract_ref = parser.add_argument_group("EXTRACTION ALIGN_MODE")
     p_extract_ref.add_argument("--ref", type=str, required=False,
                                help="path to genome reference to be aligned, in fasta/fa format.")
     p_extract_ref.add_argument("--mapq", type=int, default=1, required=False,
                                help="MAPping Quality cutoff for selecting alignment items, default 1")
     p_extract_ref.add_argument("--identity", type=float, default=0.0, required=False,
```

### Comparing `ccsmeth-0.4.0/ccsmeth/call_mods_freq_bam.py` & `ccsmeth-0.4.1/ccsmeth/call_mods_freq_bam.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 from .utils.process_utils import index_bam_if_needed2
 from .utils.process_utils import get_motif_seqs
 from .utils.process_utils import complement_seq
 from .utils.process_utils import get_refloc_of_methysite_in_motif
 
 from numpy.lib.stride_tricks import sliding_window_view
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
+
 time_wait = 1
 key_sep = "||"
 
 
 def _check_input_file(inputpath):
     if not inputpath.endswith(".bam"):
         raise ValueError("--input_bam not a bam file!")
@@ -60,15 +63,15 @@
             if i + chunk_len < contig_len:
                 istart, iend = i, i + chunk_len
             else:
                 istart, iend = i, contig_len
             ref_chunks.append((contig, istart, iend))
     # adjust start, end if motifs=='CG'
     if motifs == "CG":
-        sys.stderr.write("adjust regions for CG motif\n")
+        LOGGER.info("adjust regions for CG motif")
         for idx in range(1, len(ref_chunks)):
             pre_ref, pre_s, pre_e = ref_chunks[idx-1]
             cur_ref, cur_s, cur_e = ref_chunks[idx]
             if pre_ref != cur_ref:
                 continue
             assert cur_s == pre_e
             if dnacontigs[pre_ref][(pre_e-1):(pre_e+1)] == "CG":
@@ -78,18 +81,18 @@
                 #                                                          (cur_ref, cur_s, cur_e),
                 #                                                          ref_chunks[idx - 1],
                 #                                                          ref_chunks[idx]))
     return ref_chunks
 
 
 def _worker_split_ref_regions(dnacontigs, region_q, args):
-    sys.stderr.write("worker_split_regions process-{} starts\n".format(os.getpid()))
+    LOGGER.info("worker_split_regions process-{} starts".format(os.getpid()))
     ref_chunks = _get_reference_chunks(dnacontigs, args.contigs, args.chunk_len, args.motifs)
-    sys.stderr.write("worker_split_regions process-{} generates {} regions\n".format(os.getpid(),
-                                                                                     len(ref_chunks)))
+    LOGGER.info("worker_split_regions process-{} generates {} regions".format(os.getpid(),
+                                                                              len(ref_chunks)))
     with tqdm(total=len(ref_chunks),
               desc="region_reader") as pbar:
         for ref_chunk in ref_chunks:
             region_q.put(ref_chunk)
             pbar.update(1)
             while region_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
                 time.sleep(time_wait)
@@ -155,19 +158,19 @@
             for idx in range(len(modbases)):
                 mod_pos = modbases[idx]
                 if is_reverse:
                     mod_pos = seq_len - 1 - mod_pos
                 moddict[mod_pos] = _cal_mod_prob(mltag[idx])
             return moddict
         except IndexError:
-            sys.stderr.write("[WARN] read {}: MM tag length does not match length of modbases "
-                             "in read!\n".format(readitem.query_name))
+            LOGGER.warning("read {}: MM tag length does not match length of modbases "
+                           "in read!".format(readitem.query_name))
             return {}
         except AssertionError:
-            sys.stderr.write("[WARN] read {}: MM tag length != ML tag length!\n".format(readitem.query_name))
+            LOGGER.warning("read {}: MM tag length != ML tag length!".format(readitem.query_name))
             return {}
 
 
 def _get_moddict(readitem, modbase="C", modification="m"):
     """
 
     :param readitem:
@@ -476,67 +479,75 @@
                                                              motifs_filter, args.mod_loc)
         refmotifsites_rev = set([ref_end - 1 - x for x in refmotifsites_rev])
     refposinfo = {}  # {loc: [(prob, hap), ]), }
     refposes = set()
     refposinfo_rev = {}
     refposes_rev = set()
     cnt_all, cnt_used = 0, 0
-    for readitem in bam_reader.fetch(contig=ref_name, start=ref_start, stop=ref_end):
-        cnt_all += 1
-        if readitem.is_unmapped or readitem.is_secondary or readitem.is_duplicate:
-            continue
-        if args.no_supplementary and readitem.is_supplementary:
-            continue
-        if readitem.mapping_quality < args.mapq:
-            continue
-        identity = compute_pct_identity(np.array(readitem.get_cigar_stats()[0]))
-        if identity < args.identity:
-            continue
+    # check if (ref_name, ref_start, ref_end) is valid in bam_reader.references
+    try:
+        for readitem in bam_reader.fetch(contig=ref_name, start=ref_start, stop=ref_end):
+            cnt_all += 1
+            if readitem.is_unmapped or readitem.is_secondary or readitem.is_duplicate:
+                continue
+            if args.no_supplementary and readitem.is_supplementary:
+                continue
+            if readitem.mapping_quality < args.mapq:
+                continue
+            identity = compute_pct_identity(np.array(readitem.get_cigar_stats()[0]))
+            if identity < args.identity:
+                continue
 
-        try:
-            hap_val = readitem.get_tag(args.hap_tag)
-            hap = int(hap_val)
-        except ValueError:
-            hap = 0
-        except KeyError:
-            hap = 0
-        is_reverse = 1 if readitem.is_reverse else 0
-        moddict = _get_moddict(readitem, modbase, modification)
-        modlocs = set(moddict.keys())
-        matches_only = False if args.refsites_all else True
-        aligned_pairs = readitem.get_aligned_pairs(matches_only=matches_only)
-        if args.base_clip > 0:
-            aligned_pairs = aligned_pairs[args.base_clip:(-args.base_clip)]
-        if is_reverse:
-            for q_pos, r_pos in aligned_pairs:
-                if r_pos is not None and ref_start <= r_pos < ref_end:
-                    if q_pos is not None and q_pos in modlocs:
-                        if r_pos not in refposes_rev:
-                            refposes_rev.add(r_pos)
-                            refposinfo_rev[r_pos] = []
-                        refposinfo_rev[r_pos].append((moddict[q_pos], hap))
-                    elif args.refsites_all and (r_pos in refmotifsites_rev):
-                        if r_pos not in refposes_rev:
-                            refposes_rev.add(r_pos)
-                            refposinfo_rev[r_pos] = []
-                        refposinfo_rev[r_pos].append((0.0, hap))
-        else:
-            for q_pos, r_pos in aligned_pairs:
-                if r_pos is not None and ref_start <= r_pos < ref_end:
-                    if q_pos is not None and q_pos in modlocs:
-                        if r_pos not in refposes:
-                            refposes.add(r_pos)
-                            refposinfo[r_pos] = []
-                        refposinfo[r_pos].append((moddict[q_pos], hap))
-                    elif args.refsites_all and (r_pos in refmotifsites):
-                        if r_pos not in refposes:
-                            refposes.add(r_pos)
-                            refposinfo[r_pos] = []
-                        refposinfo[r_pos].append((0.0, hap))
-        cnt_used += 1
+            try:
+                hap_val = readitem.get_tag(args.hap_tag)
+                hap = int(hap_val)
+            except ValueError:
+                hap = 0
+            except KeyError:
+                hap = 0
+            is_reverse = 1 if readitem.is_reverse else 0
+            moddict = _get_moddict(readitem, modbase, modification)
+            modlocs = set(moddict.keys())
+            matches_only = False if args.refsites_all else True
+            aligned_pairs = readitem.get_aligned_pairs(matches_only=matches_only)
+            if args.base_clip > 0:
+                aligned_pairs = aligned_pairs[args.base_clip:(-args.base_clip)]
+            if is_reverse:
+                for q_pos, r_pos in aligned_pairs:
+                    if r_pos is not None and ref_start <= r_pos < ref_end:
+                        if q_pos is not None and q_pos in modlocs:
+                            if r_pos not in refposes_rev:
+                                refposes_rev.add(r_pos)
+                                refposinfo_rev[r_pos] = []
+                            refposinfo_rev[r_pos].append((moddict[q_pos], hap))
+                        elif args.refsites_all and (r_pos in refmotifsites_rev):
+                            if r_pos not in refposes_rev:
+                                refposes_rev.add(r_pos)
+                                refposinfo_rev[r_pos] = []
+                            refposinfo_rev[r_pos].append((0.0, hap))
+            else:
+                for q_pos, r_pos in aligned_pairs:
+                    if r_pos is not None and ref_start <= r_pos < ref_end:
+                        if q_pos is not None and q_pos in modlocs:
+                            if r_pos not in refposes:
+                                refposes.add(r_pos)
+                                refposinfo[r_pos] = []
+                            refposinfo[r_pos].append((moddict[q_pos], hap))
+                        elif args.refsites_all and (r_pos in refmotifsites):
+                            if r_pos not in refposes:
+                                refposes.add(r_pos)
+                                refposinfo[r_pos] = []
+                            refposinfo[r_pos].append((0.0, hap))
+            cnt_used += 1
+    except ValueError:
+        LOGGER.warning("worker_gen_bed process-%d: "
+                       "region %s:%d-%d is not valid in bam file" % (os.getpid(), ref_name, 
+                                                                     ref_start, ref_end))
+        return [], [], []
+    
     if args.motifs == "CG" and not args.no_comb:
         for rev_pos in refposes_rev:
             if rev_pos == 0:
                 continue
             fwd_pos = rev_pos - 1
             if fwd_pos not in refposes:
                 refposes.add(fwd_pos)
@@ -580,15 +591,15 @@
                 bed_hp1.append((ref_name, refpos, "-", hp1_info[0], hp1_info[1], hp1_info[2]))
             if hp2_info is not None:
                 bed_hp2.append((ref_name, refpos, "-", hp2_info[0], hp2_info[1], hp2_info[2]))
     return bed_all, bed_hp1, bed_hp2
 
 
 def _worker_generate_bed_of_regions(inputbam, region_q, bed_q, dnacontigs, motifs_filter, args):
-    sys.stderr.write("worker_gen_bed process-{} starts\n".format(os.getpid()))
+    LOGGER.info("worker_gen_bed process-{} starts".format(os.getpid()))
     try:
         bam_reader = pysam.AlignmentFile(inputbam, 'rb')
     except ValueError:
         raise ValueError("file has no sequences defined (mode='rb') - pysam - "
                          "Please check and make sure that the reads are aligned to genome referece!")
     cnt_regions = 0
     while True:
@@ -604,31 +615,31 @@
                                                                    dnacontigs, motifs_filter, args)
         if len(bed_all) > 0:
             bed_q.put((bed_all, bed_hp1, bed_hp2))
             while bed_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
                 time.sleep(time_wait)
 
     bam_reader.close()
-    sys.stderr.write("worker_gen_bed process-{} ending, proceed {} regions\n".format(os.getpid(),
-                                                                                     cnt_regions))
+    LOGGER.info("worker_gen_bed process-{} ending, proceed {} regions".format(os.getpid(),
+                                                                              cnt_regions))
 
 
 def _write_one_line(beditem, wf, is_bed):
     ref_name, refpos, strand, cov, met, metprob = beditem
     if is_bed:
         wf.write("\t".join([ref_name, str(refpos), str(refpos + 1), ".", str(cov),
                             strand, str(refpos), str(refpos + 1),
                             "0,0,0", str(cov), str(int(round(metprob * 100 + 0.001, 0)))]) + "\n")
     else:
         wf.write("\t".join([ref_name, str(refpos), str(refpos + 1), strand, ".", ".", str(met),
                             str(cov-met), str(cov), str(round(metprob + 0.000001, 4)), "."]) + "\n")
 
 
 def _worker_write_bed_result(output_prefix, bed_q, args):
-    sys.stderr.write('write_process-{} starts\n'.format(os.getpid()))
+    LOGGER.info('write_process-{} starts'.format(os.getpid()))
 
     fext = "bed" if args.bed else "freq.txt"
     op_all = output_prefix + ".{}.all.{}".format(args.call_mode, fext)
     op_hp1 = output_prefix + ".{}.hp1.{}".format(args.call_mode, fext)
     op_hp2 = output_prefix + ".{}.hp2.{}".format(args.call_mode, fext)
     wf_all = open(op_all, "w")
     wf_hp1 = open(op_hp1, "w")
@@ -651,27 +662,27 @@
     wf_hp1.close()
     wf_hp2.close()
     for bedfile in (op_all, op_hp1, op_hp2):
         if is_file_empty(bedfile):
             os.remove(bedfile)
             continue
         if args.sort or args.gzip:
-            sys.stderr.write('write_process-{} sorting results\n'.format(os.getpid()))
+            LOGGER.info('write_process-{} sorting results - {}'.format(os.getpid(), bedfile))
             ori_bed = pybedtools.BedTool(bedfile)
             ori_bed.sort().moveto(bedfile)
         if args.gzip:
-            sys.stderr.write('write_process-{} gzipping results\n'.format(os.getpid()))
+            LOGGER.info('write_process-{} gzipping results - {}'.format(os.getpid(), bedfile))
             pysam.tabix_index(bedfile, force=True,
                               preset="bed",
                               keep_original=False)
-    sys.stderr.write('write_process-{} finished\n'.format(os.getpid()))
+    LOGGER.info('write_process-{} finished'.format(os.getpid()))
 
 
 def call_mods_frequency_from_bamfile(args):
-    sys.stderr.write("[main]call_freq_bam starts..\n")
+    LOGGER.info("[main]call_freq_bam starts")
     start = time.time()
 
     if args.call_mode == "aggregate" and not os.path.exists(args.aggre_model):
         raise ValueError("--aggre_model is not set right!")
 
     inputpath = _check_input_file(args.input_bam)
     index_bam_if_needed2(inputpath, args.threads)
@@ -684,17 +695,17 @@
 
     dnacontigs = DNAReference(args.ref).getcontigs()
     motifs = get_motif_seqs(args.motifs)
 
     motifs_filter = None
     if args.refsites_only or args.refsites_all:
         motifs_filter = motifs
-        sys.stderr.write("[###] --refsites_only (or/and --refsites_all) is set as True, "
-                         "gonna keep only motifs({}) sites of genome reference in the "
-                         "results\n".format(motifs_filter))
+        LOGGER.info("[###] --refsites_only (or/and --refsites_all) is set as True, "
+                    "gonna keep only motifs({}) sites of genome reference in the "
+                    "results".format(motifs_filter))
 
     nproc = args.threads
     if nproc < 3:
         nproc = 3
     region_q = Queue()
     bed_q = Queue()
 
@@ -718,15 +729,15 @@
 
     for p in ps_gen:
         p.join()
     p_read.join()
     bed_q.put("kill")
     p_w.join()
 
-    sys.stderr.write("[main]call_freq_bam costs %.1f seconds..\n" % (time.time() - start))
+    LOGGER.info("[main]call_freq_bam costs %.1f seconds" % (time.time() - start))
 
 
 def main():
     parser = argparse.ArgumentParser(description='calculate frequency of interested sites at genome level '
                                                  'from aligned.sorted.bam')
 
     parser.add_argument('--threads', action="store", type=int, required=False, default=5,
```

### Comparing `ccsmeth-0.4.0/ccsmeth/call_mods_freq_txt.py` & `ccsmeth-0.4.1/ccsmeth/call_mods_freq_txt.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from multiprocessing import Queue
 from .utils.process_utils import is_file_empty
 import uuid
 
 from .utils.process_utils import default_ref_loc
 from .utils.process_utils import complement_seq
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
+
 time_wait = 1
 key_sep = "||"
 
 
 class ModRecord:
     def __init__(self, fields):
         self._chromosome = fields[0]
@@ -108,17 +111,17 @@
             else:
                 sitekey2stats[mod_record._site_key]._unmet += 1
             used += 1
         infile.close()
     if count == 0:
         raise ValueError("No modification calls found in {}..".format(mods_files))
     if contig_name is None:
-        print("{:.2f}% ({} of {}) calls used..".format(used/float(count) * 100, used, count))
+        LOGGER.info("{:.2f}% ({} of {}) calls used..".format(used/float(count) * 100, used, count))
     else:
-        print("{:.2f}% ({} of {}) calls used for {}..".format(used / float(count) * 100, used, count, contig_name))
+        LOGGER.info("{:.2f}% ({} of {}) calls used for {}..".format(used / float(count) * 100, used, count, contig_name))
     return sitekey2stats
 
 
 def write_sitekey2stats(sitekey2stats, result_file, is_sort, is_bed, is_gzip,
                         motifs=None, mod_loc=None, dnacontigs=None):
     """
     write methylfreq of sites into files
@@ -177,15 +180,15 @@
                                                                                  sitestats._prob_1,
                                                                                  sitestats._met,
                                                                                  sitestats._unmet,
                                                                                  sitestats._coverage,
                                                                                  rmet + 0.000001,
                                                                                  sitestats._kmer))
         else:
-            print("{} {} has no coverage..".format(chrom, pos))
+            LOGGER.info("{} {} has no coverage..".format(chrom, pos))
     wf.flush()
     wf.close()
 
 
 def _read_file_lines(cfile):
     with open(cfile, "r") as rf:
         return rf.read().splitlines()
@@ -235,39 +238,39 @@
         wfs[contig].flush()
         wfs[contig].close()
 
 
 def _call_and_write_modsfreq_process(wprefix, prob_cf, result_file, issort, isbed, rm_1strand, isgzip,
                                      motifs, modloc, dnacontigs,
                                      contigs_q, resfiles_q):
-    print("process-{} -- starts".format(os.getpid()))
+    LOGGER.info("process-{} -- starts".format(os.getpid()))
     while True:
         if contigs_q.empty():
             time.sleep(time_wait)
         contig_name = contigs_q.get()
         if contig_name == "kill":
             contigs_q.put("kill")
             break
-        print("process-{} for contig-{} -- reading the input files..".format(os.getpid(), contig_name))
+        LOGGER.info("process-{} for contig-{} -- reading the input files..".format(os.getpid(), contig_name))
         input_file = _get_contigfile_name(wprefix, contig_name)
         if not os.path.isfile(input_file):
-            print("process-{} for contig-{} -- the input file does not exist..".format(os.getpid(), contig_name))
+            LOGGER.warning("process-{} for contig-{} -- the input file does not exist..".format(os.getpid(), contig_name))
             continue
         if is_file_empty(input_file):
-            print("process-{} for contig-{} -- the input file is empty..".format(os.getpid(), contig_name))
+            LOGGER.warning("process-{} for contig-{} -- the input file is empty..".format(os.getpid(), contig_name))
         else:
             sites_stats = calculate_mods_frequency(input_file, prob_cf, rm_1strand, contig_name)
-            print("process-{} for contig-{} -- writing the result..".format(os.getpid(), contig_name))
+            LOGGER.info("process-{} for contig-{} -- writing the result..".format(os.getpid(), contig_name))
             fname, fext = os.path.splitext(result_file)
             c_result_file = fname + "." + contig_name + "." + str(uuid.uuid1()) + fext
             write_sitekey2stats(sites_stats, c_result_file, issort, isbed, isgzip,
                                 motifs, modloc, dnacontigs)
             resfiles_q.put(c_result_file)
         os.remove(input_file)
-    print("process-{} -- ends".format(os.getpid()))
+    LOGGER.info("process-{} -- ends".format(os.getpid()))
 
 
 def _concat_contig_results(contig_files, result_file, is_gzip=False):
     if is_gzip:
         if not result_file.endswith(".gz"):
             result_file += ".gz"
         wf = gzip.open(result_file, "wt")
@@ -278,15 +281,15 @@
             for line in rf:
                 wf.write(line)
         os.remove(cfile)
     wf.close()
 
 
 def call_mods_frequency_to_file(args):
-    print("[main]call_freq starts..")
+    LOGGER.info("[main]call_freq starts")
     start = time.time()
 
     input_paths = args.input_path
     result_file = args.result_file
     prob_cf = args.prob_cf
     file_uid = args.file_uid
     issort = args.sort
@@ -304,56 +307,56 @@
         if args.ref is None:
             raise ValueError("--ref must be set when --refsites_only is True!")
         if not os.path.exists(args.ref):
             raise ValueError("--ref doesn't exist!")
         dnacontigs = DNAReference(args.ref).getcontigs()
         motifs = get_motif_seqs(args.motifs)
         modloc = args.mod_loc
-        print("[###] --refsites_only is set as True, gonna keep only motifs({}) sites of genome reference "
-              "in the results".format(motifs))
+        LOGGER.info("[###] --refsites_only is set as True, gonna keep only motifs({}) sites of genome reference "
+                    "in the results".format(motifs))
 
     mods_files = []
     for ipath in input_paths:
         input_path = os.path.abspath(ipath)
         if os.path.isdir(input_path):
             for ifile in os.listdir(input_path):
                 if file_uid is None:
                     mods_files.append('/'.join([input_path, ifile]))
                 elif ifile.find(file_uid) != -1:
                     mods_files.append('/'.join([input_path, ifile]))
         elif os.path.isfile(input_path):
             mods_files.append(input_path)
         else:
             raise ValueError("--input_path is not a file or a directory!")
-    print("get {} input file(s)..".format(len(mods_files)))
+    LOGGER.info("get {} input file(s)..".format(len(mods_files)))
 
     contigs = None
     if args.contigs is not None:
         if os.path.isfile(args.contigs):
             if args.contigs.endswith(".fa") or args.contigs.endswith(".fasta") or args.contigs.endswith(".fna"):
                 contigs = _get_contignams_from_genome_fasta(args.contigs)
             elif _is_file_a_genome_fasta(args.contigs):
                 contigs = _get_contignams_from_genome_fasta(args.contigs)
             else:
                 contigs = sorted(list(set(_read_file_lines(args.contigs))))
         else:
             contigs = sorted(list(set(args.contigs.strip().split(","))))
 
     if contigs is None:
-        print("read the input files..")
+        LOGGER.info("read the input files..")
         sites_stats = calculate_mods_frequency(mods_files, prob_cf, rm_1strand)
-        print("write the result..")
+        LOGGER.info("write the result..")
         write_sitekey2stats(sites_stats, result_file, issort, isbed, is_gzip,
                             motifs, modloc, dnacontigs)
     else:
-        print("start processing {} contigs..".format(len(contigs)))
+        LOGGER.info("start processing {} contigs..".format(len(contigs)))
         wprefix = os.path.dirname(os.path.abspath(result_file)) + "/tmp." + str(uuid.uuid1())
-        print("generate input files for each contig..")
+        LOGGER.info("generate input files for each contig..")
         _split_file_by_contignames(mods_files, wprefix, contigs)
-        print("read the input files of each contig..")
+        LOGGER.info("read the input files of each contig..")
         contigs_q = Queue()
         for contig in contigs:
             contigs_q.put(contig)
         contigs_q.put("kill")
         resfiles_q = Queue()
         procs_contig = []
         for _ in range(args.threads):
@@ -372,18 +375,18 @@
             if not running:
                 break
         for p in procs_contig:
             p.join()
         try:
             assert len(contigs) == len(resfiles_cs)
         except AssertionError:
-            print("!!!Please check the result files -- seems not all inputed contigs have result!!!")
-        print("combine results of {} contigs..".format(len(resfiles_cs)))
+            LOGGER.warning("!!!Please check the result files -- seems not all inputed contigs have result!!!")
+        LOGGER.info("combine results of {} contigs..".format(len(resfiles_cs)))
         _concat_contig_results(resfiles_cs, result_file, is_gzip)
-    print("[main]call_freq costs %.1f seconds.." % (time.time() - start))
+    LOGGER.info("[main]call_freq costs %.1f seconds" % (time.time() - start))
 
 
 def main():
     parser = argparse.ArgumentParser(description='calculate frequency of interested sites at genome level')
     parser.add_argument('--input_path', '-i', action="append", type=str, required=True,
                         help='an output file from call_mods/call_modifications.py, or a directory contains '
                              'a bunch of output files. this arg is in "append" mode, can be used multiple times')
```

### Comparing `ccsmeth-0.4.0/ccsmeth/ccsmeth.py` & `ccsmeth-0.4.1/ccsmeth/ccsmeth.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 from ._version import VERSION
 
 
 def main_call_hifi(args):
     from .call_hifi_reads import ccs_call_hifi_reads
 
-    display_args(args, True)
+    display_args(args)
     ccs_call_hifi_reads(args)
 
 
 def main_align_hifi(args):
     from .align_hifi_reads import align_hifi_reads_to_genome
 
-    display_args(args, True)
+    display_args(args)
     align_hifi_reads_to_genome(args)
 
 
 def main_call_mods(args):
     from .call_modifications import call_mods
 
     display_args(args)
@@ -43,15 +43,15 @@
     display_args(args)
     call_mods_frequency_from_bamfile(args)
 
 
 def main_extract(args):
     from .extract_features import extract_hifireads_features
 
-    display_args(args, True)
+    display_args(args)
     extract_hifireads_features(args)
 
 
 def main_train(args):
     from .train import train
 
     display_args(args)
@@ -61,20 +61,14 @@
 def main_trainm(args):
     from .train_multigpu import train
 
     display_args(args)
     train(args)
 
 
-# def main_denoise(args):
-#     from .denoise import denoise
-#     display_args(args)
-#     denoise(args)
-
-
 def main():
     parser = argparse.ArgumentParser(prog='ccsmeth',
                                      description="ccsmeth detects methylation from PacBio CCS reads, "
                                                  "which contains 8 modules:\n"
                                                  "\t%(prog)s call_hifi: call hifi reads from subreads "
                                                  "using CCS (PBCCS)\n"
                                                  "\t%(prog)s call_mods: call modifications\n"
@@ -274,27 +268,25 @@
                                   'the same')
     scm_extract.add_argument("--mod_loc", action="store", type=int, required=False, default=0,
                              help='0-based location of the targeted base in the motif, default 0')
     scm_extract.add_argument("--methy_label", action="store", type=int,
                              choices=[1, 0], required=False, default=1,
                              help="the label of the interested modified bases, this is for training."
                                   " 0 or 1, default 1")
-    scm_extract.add_argument("--norm", action="store", type=str, choices=["zscore", "min-mean", "min-max", "mad"],
-                             default="zscore", required=False,
-                             help="method for normalizing ipd/pw in subread level. "
-                                  "zscore, min-mean, min-max or mad, default zscore")
+    scm_extract.add_argument("--norm", action="store", type=str, 
+                           choices=["zscore", "min-mean", "min-max", "mad", "none"],
+                           default="zscore", required=False,
+                           help="method for normalizing ipd/pw in subread level. "
+                                "zscore, min-mean, min-max, mad, or none. default zscore")
     scm_extract.add_argument("--no_decode", action="store_true", default=False, required=False,
                              help="not use CodecV1 to decode ipd/pw")
     # scm_extract.add_argument("--path_to_samtools", type=str, default=None, required=False,
     #                          help="full path to the executable binary samtools file. "
     #                               "If not specified, it is assumed that samtools is in "
     #                               "the PATH.")
-    scm_extract.add_argument("--loginfo", type=str, default="no", required=False,
-                             help="if printing more info of feature extraction on reads. "
-                                  "yes or no, default no")
 
     scm_extract_ref = sub_call_mods.add_argument_group("EXTRACTION ALIGN_MODE")
     scm_extract_ref.add_argument("--ref", type=str, required=False,
                                  help="path to genome reference to be aligned, in fasta/fa format.")
     scm_extract_ref.add_argument("--mapq", type=int, default=1, required=False,
                                  help="MAPping Quality cutoff for selecting alignment items, default 1")
     scm_extract_ref.add_argument("--identity", type=float, default=0.0, required=False,
@@ -352,18 +344,19 @@
                                  'the same')
     se_extract.add_argument("--mod_loc", action="store", type=int, required=False, default=0,
                             help='0-based location of the targeted base in the motif, default 0')
     se_extract.add_argument("--methy_label", action="store", type=int,
                             choices=[1, 0], required=False, default=1,
                             help="the label of the interested modified bases, this is for training."
                                  " 0 or 1, default 1")
-    se_extract.add_argument("--norm", action="store", type=str, choices=["zscore", "min-mean", "min-max", "mad"],
-                            default="zscore", required=False,
-                            help="method for normalizing ipd/pw in subread level. "
-                                 "zscore, min-mean, min-max or mad, default zscore")
+    se_extract.add_argument("--norm", action="store", type=str, 
+                           choices=["zscore", "min-mean", "min-max", "mad", "none"],
+                           default="zscore", required=False,
+                           help="method for normalizing ipd/pw in subread level. "
+                                "zscore, min-mean, min-max, mad, or none. default zscore")
     se_extract.add_argument("--no_decode", action="store_true", default=False, required=False,
                             help="not use CodecV1 to decode ipd/pw")
     # se_extract.add_argument("--path_to_samtools", type=str, default=None, required=False,
     #                         help="full path to the executable binary samtools file. "
     #                              "If not specified, it is assumed that samtools is in "
     #                              "the PATH.")
     se_extract.add_argument("--holes_batch", type=int, default=50, required=False,
@@ -381,17 +374,14 @@
     se_extract_ref.add_argument("--is_mapfea", type=str, default="no", required=False,
                                 help="if extract mapping features, yes or no, default no")
     se_extract_ref.add_argument("--skip_unmapped", type=str, default="yes", required=False,
                                 help="if skipping unmapped sites in reads, yes or no, default yes")
 
     sub_extract.add_argument("--threads", type=int, default=5, required=False,
                              help="number of threads, default 5")
-    sub_extract.add_argument("--loginfo", type=str, default="no", required=False,
-                             help="if printing more info of feature extraction on reads. "
-                                  "yes or no, default no")
 
     sub_extract.set_defaults(func=main_extract)
 
     # sub_call_freq_txt =====================================================================================
     scf_input = sub_call_freqt.add_argument_group("INPUT")
     scf_input.add_argument('--input_path', '-i', action="append", type=str, required=True,
                            help='an output file from call_mods/call_modifications.py, or a directory contains '
```

### Comparing `ccsmeth-0.4.0/ccsmeth/dataloader.py` & `ccsmeth-0.4.1/ccsmeth/dataloader.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.4.0/ccsmeth/extract_features.py` & `ccsmeth-0.4.1/ccsmeth/extract_features.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import argparse
-import sys
 import time
 import numpy as np
 from statsmodels import robust
 import multiprocessing as mp
 from multiprocessing import Queue
 import gzip
 
@@ -13,28 +12,31 @@
 from tqdm import tqdm
 
 from .utils.process_utils import display_args
 from .utils.process_utils import codecv1_to_frame2
 from .utils.process_utils import get_refloc_of_methysite_in_motif
 from .utils.process_utils import get_motif_seqs
 from .utils.process_utils import complement_seq
-from .utils.process_utils import base2code_dna
+# from .utils.process_utils import base2code_dna
 from .utils.process_utils import compute_pct_identity
 from .utils.process_utils import get_q2tloc_from_cigar
 from .utils.process_utils import str2bool
 from .utils.process_utils import index_bam_if_needed2
-from .utils.process_utils import max_queue_size
+# from .utils.process_utils import max_queue_size
 
 # from .utils.process_utils import run_cmd
 # from .utils.process_utils import generate_samtools_index_cmd
 
 from .utils.ref_reader import DNAReference
 
 from .utils.process_utils import default_ref_loc
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
+
 code2frames = codecv1_to_frame2()
 # queue_size_border = max_queue_size
 time_wait = 0.2
 
 
 # check and read some inputs =============================================
 def check_input_file(inputfile):
@@ -55,16 +57,16 @@
 
 def _open_inputfile(inputfile, rmode, threads=1):
     if inputfile.endswith(".bam"):
         if rmode == "align":
             try:
                 inputreads = pysam.AlignmentFile(inputfile, 'rb', threads=threads)
             except ValueError:
-                sys.stderr.write("[WARN] The input file has no sequences defined - Please align "
-                                 "the reads to genome reference first, or use '--mode denovo'\n")
+                LOGGER.warning("The input file has no sequences defined - Please align "
+                               "the reads to genome reference first, or use '--mode denovo'")
                 return None
         else:
             inputreads = pysam.AlignmentFile(inputfile, 'rb', check_sq=False, threads=threads)
     else:
         inputreads = pysam.AlignmentFile(inputfile, 'r', threads=threads)
     return inputreads
 
@@ -72,15 +74,15 @@
 def _get_holes(holeidfile):
     holes = set()
     with open(holeidfile, "r") as rf:
         for line in rf:
             words = line.strip().split("\t")
             holeid = words[0]
             holes.add(holeid)
-    sys.stderr.write("get {} holeids from {}\n".format(len(holes), holeidfile))
+    LOGGER.info("get {} holeids from {}".format(len(holes), holeidfile))
     return holes
 
 
 # read bam/sam inputfile =============================================
 def _get_necessary_items_of_a_alignedsegment(readitem):
     seq_name = readitem.query_name
     qalign_start = readitem.query_alignment_start
@@ -114,15 +116,15 @@
         tag_fn = tag_rn = 0
     return seq_name, qalign_start, qalign_end, fwd_seq, fwd_qual, ref_name, ref_start, ref_end, \
         cigar_tuples, cigar_stats, flag, mapq, is_unmapped, is_secondary, is_duplicate, is_supplementary, \
         is_reverse, tag_fi, tag_ri, tag_fp, tag_rp, tag_fn, tag_rn
 
 
 def worker_read_split_holebatches_to_queue(inputfile, holebatch_q, threads, args):
-    sys.stderr.write("split_holebatches process-{} starts\n".format(os.getpid()))
+    LOGGER.info("split_holebatches process-{} starts".format(os.getpid()))
     inputreads = _open_inputfile(inputfile, args.mode, threads=args.threads)
     if inputreads is None:
         holebatch_q.put("kill")
         return
     # TODO: check if input is generated by --by-strand/--hd-finder?
     if args.mode == "align":
         # totalnum = inputreads.count()
@@ -131,17 +133,17 @@
         totalnum = inputreads.count(until_eof=True)
     inputreads.close()
 
     holebatches = []
     for i in np.arange(0, totalnum, args.holes_batch):
         # holebatches.append((i, (i + args.holes_batch)))
         holebatches.append(i)
-    sys.stderr.write("split_holebatches process-{} generates {} "
-                     "hole/read batches({})\n".format(os.getpid(), len(holebatches),
-                                                      args.holes_batch))
+    LOGGER.info("split_holebatches process-{} generates {} "
+                "hole/read batches({})".format(os.getpid(), len(holebatches),
+                                               args.holes_batch))
 
     with tqdm(total=len(holebatches),
               desc="batch_reader") as pbar:
         inputreads = _open_inputfile(inputfile, args.mode, threads=threads)
         all_reads = inputreads.fetch(until_eof=True)
         count = 0
         count_batch = 0
@@ -156,25 +158,27 @@
                 count_batch += 1
                 holebatchtmp = []
                 # while holebatch_q.qsize() > queue_size_border:
                 while holebatch_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
                     time.sleep(time_wait)
         inputreads.close()
         if count_batch != len(holebatches):
-            sys.stderr.write("[WARN]read {} batches while it should be {} batches!".format(count_batch,
-                                                                                           len(holebatches)))
+            LOGGER.warning("read {} batches while it should be {} batches!".format(count_batch,
+                                                                                   len(holebatches)))
         if len(holebatchtmp) > 0:
-            sys.stderr.write("[WARN]There are still holes/reads that do not belong any batches!")
+            LOGGER.warning("There are still holes/reads that do not belong any batches!")
     holebatch_q.put("kill")
-    sys.stderr.write("split_holebatches process-{} finished\n".format(os.getpid()))
+    LOGGER.info("split_holebatches process-{} finished".format(os.getpid()))
 
 
 # extract features =============================================
 def _normalize_signals(signals, normalize_method="zscore"):
-    if normalize_method == 'zscore':
+    if normalize_method == 'none':
+        sshift, sscale = 0.0, 1.0
+    elif normalize_method == 'zscore':
         sshift, sscale = np.mean(signals), np.std(signals)
     elif normalize_method == 'min-max':
         sshift, sscale = np.min(signals), np.max(signals) - np.min(signals)
     elif normalize_method == 'min-mean':
         sshift, sscale = np.min(signals), np.mean(signals)
     elif normalize_method == 'mad':
         sshift, sscale = np.median(signals), float(robust.scale.mad(signals))
@@ -254,37 +258,32 @@
 
     if holeids_e is not None and seq_name not in holeids_e:
         return []
     if holeids_ne is not None and seq_name in holeids_ne:
         return []
     if args.mode == "align":
         if is_unmapped or is_secondary or is_duplicate:
-            if str2bool(args.loginfo):
-                sys.stderr.write("[WARN]read-{} is unmapped/secondary/duplicate\n".format(seq_name))
+            LOGGER.debug("read-{} is unmapped/secondary/duplicate".format(seq_name))
             return []
         if args.no_supplementary and is_supplementary:
-            if str2bool(args.loginfo):
-                sys.stderr.write("[WARN]read-{} is supplementary\n".format(seq_name))
+            LOGGER.debug("read-{} is supplementary".format(seq_name))
             return []
         if mapq < args.mapq:
-            if str2bool(args.loginfo):
-                sys.stderr.write("[WARN]read-{} has low mapQ({})\n".format(seq_name, mapq))
+            LOGGER.debug("read-{} has low mapQ({})".format(seq_name, mapq))
             return []
         identity = compute_pct_identity(np.array(cigar_stats[0]))
         if identity < args.identity:
-            if str2bool(args.loginfo):
-                sys.stderr.write("[WARN]read-{} has low map identity({})\n".format(seq_name, identity))
+            LOGGER.debug("read-{} has low map identity({})".format(seq_name, identity))
             return []
 
     # extract features
     seq_seq = fwd_seq
     seq_rc = complement_seq(seq_seq)
     seq_qual = np.array(fwd_qual, dtype=int) if len(fwd_qual) > 0 else np.full(len(seq_seq), 0, dtype=np.int32)
-    if str2bool(args.loginfo):
-        sys.stderr.write("[WARN]read-{} has no base quality\n".format(seq_name))
+    LOGGER.debug("read-{} has no base quality".format(seq_name))
     seq_qual = _normalize_signals(seq_qual, args.norm)
     reverse = is_reverse
 
     # change seq_start/seq_end if is_reverse
     if reverse:
         seq_start = len(seq_seq) - qalign_end
         seq_end = len(seq_seq) - qalign_start
@@ -306,20 +305,18 @@
     ipdmean_fwd = np.array(tag_fi, dtype=int)
     # ipdmean_rev = np.flip(np.array(tag_ri, dtype=int))
     ipdmean_rev = np.array(tag_ri, dtype=int)  # no need to use np.filp to reverse
     pwmean_fwd = np.array(tag_fp, dtype=int)
     # pwmean_rev = np.flip(np.array(tag_rp, dtype=int))
     pwmean_rev = np.array(tag_rp, dtype=int)
     if len(ipdmean_fwd) != len(seq_seq) or len(pwmean_fwd) != len(seq_seq):
-        if str2bool(args.loginfo):
-            sys.stderr.write("[WARN]read-{} has no/uncomplated fwd ipd/pw values\n".format(seq_name))
+        LOGGER.debug("read-{} has no/uncomplated fwd ipd/pw values".format(seq_name))
         return []
     if len(ipdmean_rev) != len(seq_seq) or len(pwmean_rev) != len(seq_seq):
-        if str2bool(args.loginfo):
-            sys.stderr.write("[WARN]read-{} has no/uncomplated rev ipd/pw values\n".format(seq_name))
+        LOGGER.debug("read-{} has no/uncomplated rev ipd/pw values".format(seq_name))
         return []
     if not args.no_decode:
         ipdmean_fwd = np.array([code2frames[val] for val in ipdmean_fwd])
         ipdmean_rev = np.array([code2frames[val] for val in ipdmean_rev])
         pwmean_fwd = np.array([code2frames[val] for val in pwmean_fwd])
         pwmean_rev = np.array([code2frames[val] for val in pwmean_rev])
     ipdmean_fwd = _normalize_signals(ipdmean_fwd, args.norm)
@@ -409,15 +406,15 @@
                                                                     args)
             if len(features_one) == 0:
                 failed_num += 1
             else:
                 feature_list += features_one
                 holeidxes += [read_idx] * len(features_one)
         except Exception as e:
-            print("Exception: ", e)
+            LOGGER.warning("Exception: ", e)
             failed_num += 1
         total_num += 1
     return holeidxes, feature_list, total_num, failed_num
 
 
 def _features_to_str(features):
     """
@@ -452,15 +449,15 @@
                       rkmer_seq, str(npass_rev), rkmer_im_str, rkmer_isd_str, rkmer_pm_str, rkmer_psd_str,
                       rkmer_qual_str, rkmer_map_str,
                       str(label)])
 
 
 def worker_extract_features_from_holebatches(input_header, holebatch_q, features_q,
                                              motifs, holeids_e, holeids_ne, dnacontigs, args):
-    sys.stderr.write("extract_features process-{} starts\n".format(os.getpid()))
+    LOGGER.info("extract_features process-{} starts".format(os.getpid()))
     
     if isinstance(input_header, OrderedDict) or isinstance(input_header, dict):
         input_header2 = pysam.AlignmentHeader.from_dict(input_header)
     else:
         input_header2 = input_header
     
     cnt_holesbatch = 0
@@ -486,49 +483,49 @@
             for feature in feature_list:
                 features_batch.append(_features_to_str(feature))
             features_q.put(features_batch)
             # while features_q.qsize() > queue_size_border:
             while features_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
                 time.sleep(time_wait)
         cnt_holesbatch += 1
-    sys.stderr.write("extract_features process-{} ending, proceed {} "
-                     "hole_batches({}): {} holes/reads in total, "
-                     "{} skipped/failed.\n".format(os.getpid(),
-                                                   cnt_holesbatch,
-                                                   args.holes_batch,
-                                                   total_num_batch,
-                                                   failed_num_batch))
+    LOGGER.info("extract_features process-{} ending, proceed {} "
+                "hole_batches({}): {} holes/reads in total, "
+                "{} skipped/failed.".format(os.getpid(),
+                                            cnt_holesbatch,
+                                            args.holes_batch,
+                                            total_num_batch,
+                                            failed_num_batch))
 
 
 # write to file =============================================
 def _write_featurestr_to_file(write_fp, featurestr_q, is_gzip):
-    sys.stderr.write('write_process-{} starts\n'.format(os.getpid()))
+    LOGGER.info('write_process-{} starts'.format(os.getpid()))
     if is_gzip:
         if not write_fp.endswith(".gz"):
             write_fp += ".gz"
         wf = gzip.open(write_fp, "wt")
     else:
         wf = open(write_fp, 'w')
     while True:
         # during test, it's ok without the sleep(time_wait)
         if featurestr_q.empty():
             time.sleep(time_wait)
             continue
         features_str = featurestr_q.get()
         if features_str == "kill":
             wf.close()
-            sys.stderr.write('write_process-{} finished\n'.format(os.getpid()))
+            LOGGER.info('write_process-{} finished'.format(os.getpid()))
             break
         for one_features_str in features_str:
             wf.write(one_features_str + "\n")
         wf.flush()
 
 
 def extract_hifireads_features(args):
-    sys.stderr.write("[extract_features_hifi]starts\n")
+    LOGGER.info("[main]extract_features_hifi starts")
     start = time.time()
 
     inputpath = check_input_file(args.input)
     if not os.path.exists(inputpath):
         raise IOError("input file does not exist!")
     index_bam_if_needed2(inputpath, args.threads)
 
@@ -589,15 +586,15 @@
         p.join()
     p_split.join()
 
     features_q.put("kill")
     p_w.join()
 
     endtime = time.time()
-    sys.stderr.write("[extract_features_hifi]costs {:.1f} seconds\n".format(endtime - start))
+    LOGGER.info("[main]extract_features_hifi costs {:.1f} seconds".format(endtime - start))
 
 
 def main():
     parser = argparse.ArgumentParser()
 
     p_input = parser.add_argument_group("INPUT")
     p_input.add_argument("--input", "-i", type=str, required=True,
@@ -634,18 +631,19 @@
                                 'the same')
     p_extract.add_argument("--mod_loc", action="store", type=int, required=False, default=0,
                            help='0-based location of the targeted base in the motif, default 0')
     p_extract.add_argument("--methy_label", action="store", type=int,
                            choices=[1, 0], required=False, default=1,
                            help="the label of the interested modified bases, this is for training."
                                 " 0 or 1, default 1")
-    p_extract.add_argument("--norm", action="store", type=str, choices=["zscore", "min-mean", "min-max", "mad"],
+    p_extract.add_argument("--norm", action="store", type=str, 
+                           choices=["zscore", "min-mean", "min-max", "mad", "none"],
                            default="zscore", required=False,
                            help="method for normalizing ipd/pw in subread level. "
-                                "zscore, min-mean, min-max or mad, default zscore")
+                                "zscore, min-mean, min-max, mad, or none. default zscore")
     p_extract.add_argument("--no_decode", action="store_true", default=False, required=False,
                            help="not use CodecV1 to decode ipd/pw")
     # p_extract.add_argument("--path_to_samtools", type=str, default=None, required=False,
     #                        help="full path to the executable binary samtools file. "
     #                             "If not specified, it is assumed that samtools is in "
     #                             "the PATH.")
     p_extract.add_argument("--holes_batch", type=int, default=50, required=False,
@@ -663,19 +661,16 @@
     p_extract_ref.add_argument("--is_mapfea", type=str, default="no", required=False,
                                help="if extract mapping features, yes or no, default no")
     p_extract_ref.add_argument("--skip_unmapped", type=str, default="yes", required=False,
                                help="if skipping unmapped sites in reads, yes or no, default yes")
 
     parser.add_argument("--threads", type=int, default=5, required=False,
                         help="number of threads, default 5")
-    parser.add_argument("--loginfo", type=str, default="no", required=False,
-                        help="if printing more info of feature extraction on reads. "
-                             "yes or no, default no")
 
     args = parser.parse_args()
 
-    display_args(args, True)
+    display_args(args)
     extract_hifireads_features(args)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ccsmeth-0.4.0/ccsmeth/models.py` & `ccsmeth-0.4.1/ccsmeth/models.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.4.0/ccsmeth/train.py` & `ccsmeth-0.4.1/ccsmeth/train.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 import argparse
 import os
 import re
-import sys
 import time
 
 import numpy as np
 import torch
 import torch.nn as nn
 from sklearn import metrics
 from torch.optim.lr_scheduler import StepLR
@@ -18,30 +17,33 @@
 
 from .models import ModelAttRNN
 
 from .utils.constants_torch import use_cuda
 from .utils.process_utils import display_args
 from .utils.process_utils import str2bool
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
+
 device = "cuda" if use_cuda else "cpu"
 
 
 def train(args):
     total_start = time.time()
     torch.manual_seed(args.tseed)
     if use_cuda:
         torch.cuda.manual_seed(args.tseed)
 
-    print("[main]train starts..")
+    LOGGER.info("[main]train starts")
     if use_cuda:
-        print("GPU is available!")
+        LOGGER.info("GPU is available!")
     else:
-        print("GPU is not available!")
+        LOGGER.info("GPU is not available!")
 
-    print("reading data..")
+    LOGGER.info("reading data..")
     if args.model_type in {"attbigru2s", "attbilstm2s"}:
         if args.dl_offsets:
             if args.dl_num_workers > 1:
                 raise ValueError("--dl_num_workers should not be >1 when --dl_offsets is True!")
             from .utils.process_utils import count_line_num
             from .dataloader import generate_offsets
             train_linenum = count_line_num(args.train_file, False)
@@ -86,15 +88,15 @@
                             is_npass=str2bool(args.is_npass),
                             model_type=args.model_type,
                             device=device)
     else:
         raise ValueError("--model_type not right!")
 
     if args.init_model is not None:
-        print("loading pre-trained model: {}".format(args.init_model))
+        LOGGER.info("loading pre-trained model: {}".format(args.init_model))
         para_dict = torch.load(args.init_model, map_location=torch.device('cpu'))
         # para_dict = torch.load(model_path, map_location=torch.device(device))
         model_dict = model.state_dict()
         model_dict.update(para_dict)
         model.load_state_dict(model_dict)
 
     if use_cuda:
@@ -140,15 +142,15 @@
         scheduler = ReduceLROnPlateau(optimizer, mode='max', factor=args.lr_decay,
                                       patience=args.lr_patience, verbose=True)
     else:
         raise ValueError("--lr_scheduler is not right!")
 
     # Train the model
     total_step = len(train_loader)
-    print("total_step: {}".format(total_step))
+    LOGGER.info("total_step: {}".format(total_step))
     curr_best_accuracy = 0
     curr_best_accuracy_loc = 0
     curr_best_accuracy_epoches = []
     model.train()
     for epoch in range(args.max_epoch_num):
         curr_best_accuracy_epoch = 0
         accuracies_per_epoch = []
@@ -263,33 +265,33 @@
                                        model_dir + args.model_type +
                                        '.betterthanlast.b{}_epoch{}.ckpt'.format(args.seq_len,
                                                                                  epoch + 1))
 
                     time_cost = time.time() - start
                     try:
                         last_lr = scheduler.get_last_lr()
-                        print('Epoch [{}/{}], Step [{}/{}]; LR: {:.4e}; TrainLoss: {:.4f}; '
-                              'ValidLoss: {:.4f}, '
-                              'Acc: {:.4f}, Prec: {:.4f}, Reca: {:.4f}, '
-                              'CurrE_best_acc: {:.4f}, Best_acc: {:.4f}; Time: {:.2f}s'
-                              .format(epoch + 1, args.max_epoch_num, i + 1, total_step, last_lr,
-                                      np.mean(tlosses), v_meanloss, v_accuracy, v_precision, v_recall,
-                                      curr_best_accuracy_epoch, curr_best_accuracy, time_cost))
+                        LOGGER.info('Epoch [{}/{}], Step [{}/{}]; LR: {:.4e}; TrainLoss: {:.4f}; '
+                                    'ValidLoss: {:.4f}, '
+                                    'Acc: {:.4f}, Prec: {:.4f}, Reca: {:.4f}, '
+                                    'CurrE_best_acc: {:.4f}, Best_acc: {:.4f}; Time: {:.2f}s'
+                                    .format(epoch + 1, args.max_epoch_num, i + 1, total_step, last_lr,
+                                            np.mean(tlosses), v_meanloss, v_accuracy, v_precision, v_recall,
+                                            curr_best_accuracy_epoch, curr_best_accuracy, time_cost))
                     except Exception:
-                        print('Epoch [{}/{}], Step [{}/{}]; TrainLoss: {:.4f}; '
-                              'ValidLoss: {:.4f}, '
-                              'Acc: {:.4f}, Prec: {:.4f}, Reca: {:.4f}, '
-                              'CurrE_best_acc: {:.4f}, Best_acc: {:.4f}; Time: {:.2f}s'
-                              .format(epoch + 1, args.max_epoch_num, i + 1, total_step,
-                                      np.mean(tlosses), v_meanloss, v_accuracy, v_precision, v_recall,
-                                      curr_best_accuracy_epoch, curr_best_accuracy, time_cost))
+                        LOGGER.info('Epoch [{}/{}], Step [{}/{}]; TrainLoss: {:.4f}; '
+                                    'ValidLoss: {:.4f}, '
+                                    'Acc: {:.4f}, Prec: {:.4f}, Reca: {:.4f}, '
+                                    'CurrE_best_acc: {:.4f}, Best_acc: {:.4f}; Time: {:.2f}s'
+                                    .format(epoch + 1, args.max_epoch_num, i + 1, total_step,
+                                            np.mean(tlosses), v_meanloss, v_accuracy, v_precision, v_recall,
+                                            curr_best_accuracy_epoch, curr_best_accuracy, time_cost))
 
                     tlosses = []
                     start = time.time()
-                    sys.stdout.flush()
+                    # sys.stdout.flush()
                 model.train()
 
         if args.lr_scheduler == "ReduceLROnPlateau":
             if args.lr_mode_strategy == "mean":
                 reduce_metric = np.mean(accuracies_per_epoch)
             elif args.lr_mode_strategy == "last":
                 reduce_metric = accuracies_per_epoch[-1]
@@ -299,25 +301,25 @@
                 raise ValueError("--lr_mode_strategy is not right!")
             scheduler.step(reduce_metric)
         else:
             scheduler.step()
 
         curr_best_accuracy_epoches.append(curr_best_accuracy_epoch)
         if no_best_model and epoch >= args.min_epoch_num - 1:
-            print("early stop!")
+            LOGGER.info("early stop!")
             break
     endtime = time.time()
     clear_linecache()
     if args.dl_offsets:
         train_dataset.close()
         valid_dataset.close()
-    print("[main]train costs {} seconds, "
-          "best accuracy: {} (epoch {})".format(endtime - total_start,
-                                                curr_best_accuracy,
-                                                curr_best_accuracy_loc))
+    LOGGER.info("[main]train costs {:.1f} seconds, "
+                "best accuracy: {} (epoch {})".format(endtime - total_start,
+                                                      curr_best_accuracy,
+                                                      curr_best_accuracy_loc))
 
 
 def main():
     parser = argparse.ArgumentParser("train a model")
     st_input = parser.add_argument_group("INPUT")
     st_input.add_argument('--train_file', type=str, required=True)
     st_input.add_argument('--valid_file', type=str, required=True)
@@ -390,20 +392,13 @@
     st_training.add_argument('--init_model', type=str, default=None, required=False,
                              help="file path of pre-trained model parameters to load before training")
     st_training.add_argument('--tseed', type=int, default=1234,
                              help='random seed for pytorch')
 
     args = parser.parse_args()
 
-    print("[main] start..")
-    total_start = time.time()
-
     display_args(args)
-
     train(args)
 
-    endtime = time.time()
-    print("[main] costs {} seconds".format(endtime - total_start))
-
 
 if __name__ == '__main__':
     main()
```

### Comparing `ccsmeth-0.4.0/ccsmeth/train_multigpu.py` & `ccsmeth-0.4.1/ccsmeth/train_multigpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import argparse
 import os
-import re
 import sys
+import re
 import time
 
 import numpy as np
 import torch
 import torch.nn as nn
 from sklearn import metrics
 from torch.optim.lr_scheduler import StepLR
@@ -24,14 +24,17 @@
 from .utils.process_utils import str2bool
 from .utils.process_utils import count_line_num
 
 import torch.distributed as dist
 import torch.multiprocessing as mp
 from torch.nn.parallel import DistributedDataParallel as DDP
 
+from .utils.logging import mylogger
+LOGGER = mylogger(__name__)
+
 # add this export temporarily
 # https://github.com/pytorch/pytorch/issues/37377
 os.environ['MKL_THREADING_LAYER'] = 'GNU'
 
 
 # https://zhuanlan.zhihu.com/p/350301395
 # https://github.com/tczhangzhi/pytorch-distributed/blob/master/multiprocessing_distributed.py
@@ -72,30 +75,29 @@
     map_location = {'cuda:%d' % 0: 'cuda:%d' % gpu}
     model.module.load_state_dict(
         torch.load(model_save_path, map_location=map_location))
 
 
 # https://github.com/BIGBALLON/distribuuuu/blob/master/tutorial/mnmc_ddp_mp.py
 def train_worker(local_rank, global_world_size, args):
-
     global_rank = args.node_rank * args.ngpus_per_node + local_rank
 
     dist.init_process_group(
         backend="nccl",
         init_method=args.dist_url,
         world_size=global_world_size,
         rank=global_rank,
     )
 
     # device = torch.device("cuda", local_rank)
     # torch.cuda.set_device(local_rank)
 
-    print("training_process-{} [init] == local rank: {}, global rank: {} ==".format(os.getpid(),
-                                                                                    local_rank,
-                                                                                    global_rank))
+    sys.stderr.write("training_process-{} [init] == local rank: {}, global rank: {} ==\n".format(os.getpid(),
+                                                                                                local_rank,
+                                                                                                global_rank))
 
     # 1. define network
     if global_rank == 0 or args.epoch_sync:
         model_dir = args.model_dir
         if model_dir != "/":
             model_dir = os.path.abspath(model_dir).rstrip("/")
             if local_rank == 0:
@@ -118,29 +120,29 @@
                             is_npass=str2bool(args.is_npass),
                             model_type=args.model_type,
                             device=local_rank)
     else:
         raise ValueError("--model_type not right!")
 
     if args.init_model is not None:
-        print("training_process-{} loading pre-trained model: {}".format(os.getpid(), args.init_model))
+        sys.stderr.write("training_process-{} loading pre-trained model: {}\n".format(os.getpid(), args.init_model))
         para_dict = torch.load(args.init_model, map_location=torch.device('cpu'))
         model_dict = model.state_dict()
         model_dict.update(para_dict)
         model.load_state_dict(model_dict)
 
     dist.barrier()
 
     model = model.cuda(local_rank)
     # DistributedDataParallel
     model = DDP(model, device_ids=[local_rank], output_device=local_rank,
                 find_unused_parameters=False)
 
     # 2. define dataloader
-    print("training_process-{} reading data..".format(os.getpid()))
+    sys.stderr.write("training_process-{} reading data..\n".format(os.getpid()))
     if args.model_type in {"attbigru2s", "attbilstm2s"}:
         train_linenum = count_line_num(args.train_file, False)
         train_offsets = generate_offsets(args.train_file)
         train_dataset = FeaData3(args.train_file, train_offsets, train_linenum)
         train_sampler = torch.utils.data.distributed.DistributedSampler(train_dataset,
                                                                         shuffle=True)
         train_loader = torch.utils.data.DataLoader(dataset=train_dataset,
@@ -198,15 +200,15 @@
         scheduler = ReduceLROnPlateau(optimizer, mode='min', factor=args.lr_decay,
                                       patience=args.lr_patience, verbose=True)
     else:
         raise ValueError("--lr_scheduler is not right!")
 
     # Train the model
     total_step = len(train_loader)
-    print("training_process-{} total_step: {}".format(os.getpid(), total_step))
+    sys.stderr.write("training_process-{} total_step: {}\n".format(os.getpid(), total_step))
     curr_best_accuracy = 0
     curr_best_accuracy_loc = 0
     curr_lowest_loss = 10000
     v_accuracy_epoches = []
     model.train()
     for epoch in range(args.max_epoch_num):
         # set train sampler
@@ -257,22 +259,22 @@
             loss.backward()
             torch.nn.utils.clip_grad_norm_(model.parameters(), 0.5)
             optimizer.step()
 
             tlosses.append(loss.detach().item())
             if global_rank == 0 and ((i + 1) % args.step_interval == 0 or (i + 1) == total_step):
                 time_cost = time.time() - start
-                print("Epoch [{}/{}], Step [{}/{}]; "
-                      "TrainLoss: {:.4f}; Time: {:.2f}s".format(epoch + 1,
-                                                                args.max_epoch_num, i + 1,
-                                                                total_step, np.mean(tlosses),
-                                                                time_cost))
+                sys.stderr.write("Epoch [{}/{}], Step [{}/{}]; "
+                                 "TrainLoss: {:.4f}; Time: {:.2f}s\n".format(epoch + 1,
+                                                                             args.max_epoch_num, i + 1,
+                                                                             total_step, np.mean(tlosses),
+                                                                             time_cost))
+                sys.stderr.flush()
                 start = time.time()
                 tlosses = []
-                sys.stdout.flush()
 
         model.eval()
         with torch.no_grad():
             vlosses, vlabels_total, vpredicted_total = [], [], []
             v_meanloss = 10000
             for vi, vsfeatures in enumerate(valid_loader):
                 if args.model_type in {"attbigru2s", "attbilstm2s"}:
@@ -348,81 +350,81 @@
 
             v_accuracy_epoches.append(v_accuracy)
 
             time_cost = time.time() - start
             if global_rank == 0:
                 try:
                     last_lr = scheduler.get_last_lr()
-                    print('Epoch [{}/{}]; LR: {:.4e}; '
-                          'ValidLoss: {:.4f}, '
-                          'Acc: {:.4f}, Prec: {:.4f}, Reca: {:.4f}, '
-                          'Best_acc: {:.4f}; Time: {:.2f}s'
-                          .format(epoch + 1, args.max_epoch_num, last_lr,
-                                  v_meanloss, v_accuracy, v_precision, v_recall,
-                                  curr_best_accuracy, time_cost))
+                    sys.stderr.write('Epoch [{}/{}]; LR: {:.4e}; '
+                                     'ValidLoss: {:.4f}, '
+                                     'Acc: {:.4f}, Prec: {:.4f}, Reca: {:.4f}, '
+                                     'Best_acc: {:.4f}; Time: {:.2f}s\n'
+                                     .format(epoch + 1, args.max_epoch_num, last_lr,
+                                             v_meanloss, v_accuracy, v_precision, v_recall,
+                                             curr_best_accuracy, time_cost))
                 except Exception:
-                    print('Epoch [{}/{}]; '
-                          'ValidLoss: {:.4f}, '
-                          'Acc: {:.4f}, Prec: {:.4f}, Reca: {:.4f}, '
-                          'Best_acc: {:.4f}; Time: {:.2f}s'
-                          .format(epoch + 1, args.max_epoch_num,
-                                  v_meanloss, v_accuracy, v_precision, v_recall,
-                                  curr_best_accuracy, time_cost))
+                    sys.stderr.write('Epoch [{}/{}]; '
+                                    'ValidLoss: {:.4f}, '
+                                    'Acc: {:.4f}, Prec: {:.4f}, Reca: {:.4f}, '
+                                    'Best_acc: {:.4f}; Time: {:.2f}s\n'
+                                    .format(epoch + 1, args.max_epoch_num,
+                                            v_meanloss, v_accuracy, v_precision, v_recall,
+                                            curr_best_accuracy, time_cost))
 
-                sys.stdout.flush()
+                sys.stderr.flush()
         model.train()
 
         if no_best_model and epoch >= args.min_epoch_num - 1:
-            print("training_process-{} early stop!".format(os.getpid()))
+            sys.stderr.write("training_process-{} early stop!\n".format(os.getpid()))
             break
 
         if args.epoch_sync:
             sync_ckpt = model_dir + args.model_type + \
                         '.epoch_sync_node{}.b{}_epoch{}.ckpt'.format(args.node_rank, args.seq_len, epoch + 1)
             checkpoint(model, local_rank, sync_ckpt)
 
         if args.lr_scheduler == "ReduceLROnPlateau":
             lr_reduce_metric = v_meanloss
             scheduler.step(lr_reduce_metric)
         else:
             scheduler.step()
 
     if global_rank == 0:
-        print("best model is in epoch {} (Acc: {})".format(curr_best_accuracy_loc,
-                                                           curr_best_accuracy))
+        sys.stderr.write("best model is in epoch {} (Acc: {})\n".format(curr_best_accuracy_loc,
+                                                                        curr_best_accuracy))
     clear_linecache()
     cleanup()
 
 
 def train(args):
+    LOGGER.info("[main]train_multigpu starts")
+    total_start = time.time()
+
     torch.manual_seed(args.tseed)
     if use_cuda:
         torch.cuda.manual_seed(args.tseed)
 
     if use_cuda:
-        print("GPU is available!")
+        LOGGER.info("GPU is available!")
     else:
         raise RuntimeError("No GPU is available!")
 
     if not dist.is_available():
         raise RuntimeError("torch.distributed is not available!")
 
-    print("[main]train_multigpu starts..")
-    total_start = time.time()
-
     if torch.cuda.device_count() < args.ngpus_per_node:
         raise RuntimeError("There are not enough gpus, has {}, request {}.".format(torch.cuda.device_count(),
                                                                                    args.ngpus_per_node))
 
     global_world_size = args.ngpus_per_node * args.nodes
     mp.spawn(train_worker, nprocs=args.ngpus_per_node, args=(global_world_size, args))
 
     endtime = time.time()
     clear_linecache()
-    print("[main]train_multigpu costs {} seconds".format(endtime - total_start))
+    LOGGER.info("[main]train_multigpu costs {:.1f} seconds".format(endtime - total_start))
 
 
 def main():
     parser = argparse.ArgumentParser("[EXPERIMENTAL]train a model, use torch.nn.parallel.DistributedDataParallel")
     st_input = parser.add_argument_group("INPUT")
     st_input.add_argument('--train_file', type=str, required=True)
     st_input.add_argument('--valid_file', type=str, required=True)
@@ -505,21 +507,14 @@
                               help="url used to set up distributed training")
     st_trainingp.add_argument("--node_rank", default=0, type=int,
                               help="node rank for distributed training, default 0")
     st_trainingp.add_argument("--epoch_sync", action="store_true", default=False,
                               help="if sync model params of gpu0 to other local gpus after per epoch")
 
     args = parser.parse_args()
-
-    print("[main] start..")
-    total_start = time.time()
-
+    
     display_args(args)
-
     train(args)
 
-    endtime = time.time()
-    print("[main] costs {} seconds".format(endtime - total_start))
-
 
 if __name__ == '__main__':
     main()
```

### Comparing `ccsmeth-0.4.0/ccsmeth/utils/attention.py` & `ccsmeth-0.4.1/ccsmeth/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.4.0/ccsmeth/utils/constants_torch.py` & `ccsmeth-0.4.1/ccsmeth/utils/constants_torch.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.4.0/ccsmeth/utils/lookahead.py` & `ccsmeth-0.4.1/ccsmeth/utils/lookahead.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.4.0/ccsmeth/utils/process_utils.py` & `ccsmeth-0.4.1/ccsmeth/utils/process_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import gc
 from subprocess import Popen, PIPE
 import os
 import sys
 import re
 import pysam
 
+from .logging import mylogger
+LOGGER = mylogger(__name__)
 
 basepairs = {'A': 'T', 'C': 'G', 'G': 'C', 'T': 'A', 'N': 'N',
              'W': 'W', 'S': 'S', 'M': 'K', 'K': 'M', 'R': 'Y',
              'Y': 'R', 'B': 'V', 'V': 'B', 'D': 'H', 'H': 'D',
              'Z': 'Z'}
 basepairs_rna = {'A': 'U', 'C': 'G', 'G': 'C', 'U': 'A', 'N': 'N',
                  'W': 'W', 'S': 'S', 'M': 'K', 'K': 'M', 'R': 'Y',
@@ -71,31 +73,31 @@
 
 def _alphabet(letter, dbasepairs):
     if letter in dbasepairs.keys():
         return dbasepairs[letter]
     return 'N'
 
 
-def complement_seq(base_seq, seq_type="DNA"):
+def complement_seq(base_seq, seq_type="DNA") -> str:
     rbase_seq = base_seq[::-1]
     comseq = ''
     try:
         if seq_type == "DNA":
             comseq = ''.join([_alphabet(x, basepairs) for x in rbase_seq])
         elif seq_type == "RNA":
             comseq = ''.join([_alphabet(x, basepairs_rna) for x in rbase_seq])
         else:
             raise ValueError("the seq_type must be DNA or RNA")
     except Exception:
-        print('something wrong in the dna/rna sequence.')
+        LOGGER.warning('something wrong in the dna/rna sequence.')
     return comseq
 
 
 # motifs ======================================================================
-def get_refloc_of_methysite_in_motif(seqstr, motifset, methyloc_in_motif=0):
+def get_refloc_of_methysite_in_motif(seqstr, motifset, methyloc_in_motif=0) -> list:
     """
 
     :param seqstr:
     :param motifset:
     :param methyloc_in_motif: 0-based
     :return:
     """
@@ -195,20 +197,22 @@
     if q_to_r_poss[-1] == fill_invalid:
         raise ValueError(('Invalid cigar string encountered. Reference length: {}  Cigar ' +
                           'implied reference length: {}').format(seq_len, curr_r_pos))
     return q_to_r_poss
 
 
 # arg display ========================================================================
-def display_args(args, is_stderr=False):
+def display_args(args, is_stderr=True):
     def print_outputstr(outstr):
         if is_stderr:
             sys.stderr.write(outstr + "\n")
+            sys.stderr.flush()
         else:
             print(outstr)
+            sys.stdout.flush()
     arg_vars = vars(args)
     outputstr = "# ===============================================\n## parameters: "
     print_outputstr(outputstr)
     for arg_key in arg_vars.keys():
         if arg_key != 'func':
             outputstr = "{}:\n\t{}".format(arg_key, arg_vars[arg_key])
             print_outputstr(outputstr)
@@ -268,15 +272,15 @@
 #             raise ValueError("indexing bam file failed, please try indexing it mannually using samtools")
 #         else:
 #             sys.stderr.write("indexing bam file succeeded..\n")
 
 
 def index_bam_if_needed2(inputfile, threads):
     if str(inputfile).endswith(".bam") and not os.path.exists(inputfile + ".bai"):
-        sys.stderr.write("indexing bam file-{}\n".format(inputfile))
+        LOGGER.info("indexing bam file-{}\n".format(inputfile))
         pysam.index("-@", str(threads), inputfile)
 
 
 # =================================================================
 def count_line_num(sl_filepath, fheader=False):
     count = 0
     with open(sl_filepath, 'r') as rf:
@@ -302,15 +306,15 @@
         lines_num = min(shuffle_lines_num, (total_lines_num - checked_lines_num))
         for line in rf:
             if count < lines_num:
                 lines_info.append(line.strip())
                 count += 1
             else:
                 break
-        print('done reading file {}'.format(filepath))
+        LOGGER.info('done reading file {}'.format(filepath))
         return lines_info
 
 
 def shuffle_samples(samples_info):
     mark = list(range(len(samples_info)))
     np.random.shuffle(mark)
     shuffled_samples = []
@@ -319,15 +323,15 @@
     return shuffled_samples
 
 
 def write_to_one_file_append(features_info, wfilepath):
     with open(wfilepath, 'a') as wf:
         for i in range(0, len(features_info)):
             wf.write(features_info[i] + '\n')
-    print('done writing features info to {}'.format(wfilepath))
+    LOGGER.info('done writing features info to {}'.format(wfilepath))
 
 
 def concat_two_files(file1, file2, concated_fp, shuffle_lines_num=2000000,
                      lines_num=1000000000000, isheader=False):
     open(concated_fp, 'w').close()
 
     if isheader:
@@ -354,15 +358,15 @@
         samples_info = shuffle_samples(file1_info + file2_info)
         write_to_one_file_append(samples_info, concated_fp)
 
         del file1_info
         del file2_info
         del samples_info
         gc.collect()
-    print('done concating files to: {}'.format(concated_fp))
+    LOGGER.info('done concating files to: {}'.format(concated_fp))
 # =================================================================
 
 
 def codecv1_to_frame():
     code2frames = dict()
     for i in range(0, 64):
         code2frames[i] = i
```

### Comparing `ccsmeth-0.4.0/ccsmeth/utils/ranger2020.py` & `ccsmeth-0.4.1/ccsmeth/utils/ranger2020.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.4.0/ccsmeth/utils/ref_reader.py` & `ccsmeth-0.4.1/ccsmeth/utils/ref_reader.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.4.0/ccsmeth/utils/sam2fastq_std.py` & `ccsmeth-0.4.1/ccsmeth/utils/sam2fastq_std.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.4.0/ccsmeth.egg-info/PKG-INFO` & `ccsmeth-0.4.1/ccsmeth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ccsmeth
-Version: 0.4.0
+Version: 0.4.1
 Summary: Detecting DNA methylation from PacBio CCS reads
 Home-page: https://github.com/PengNi/ccsmeth
-Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.4.0.tar.gz
+Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.4.1.tar.gz
 Author: Peng Ni
 Author-email: 543943952@qq.com
 License: BSD-3-Clause-Clear license
 Keywords: methylation,pacbio,neural network
 Platform: Linux
 Platform: MacOS
 Classifier: Programming Language :: Python :: 3
@@ -18,16 +18,25 @@
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
 
 ccsmeth
 ========
 
 
-Documentation
+Changelog
 -------------
+v0.4.1
+----------
+handle ValueError when fetching bam items in call_freqb module
+
+change pytorch max version to 1.12.1
+
+using logging instead of print/sys.stderr.write
+
+
 v0.4.0
 ----------
 optimieze call_mods module, faster generating of modbam file
 
 
 v0.3.4
 ----------
```

### Comparing `ccsmeth-0.4.0/ccsmeth.egg-info/SOURCES.txt` & `ccsmeth-0.4.1/ccsmeth.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 MANIFEST.in
+README.md
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 ccsmeth/__init__.py
 ccsmeth/_bam2modbam.py
 ccsmeth/_call_modifications_txt.py
@@ -25,12 +26,13 @@
 ccsmeth.egg-info/entry_points.txt
 ccsmeth.egg-info/not-zip-safe
 ccsmeth.egg-info/requires.txt
 ccsmeth.egg-info/top_level.txt
 ccsmeth/utils/__init__.py
 ccsmeth/utils/attention.py
 ccsmeth/utils/constants_torch.py
+ccsmeth/utils/logging.py
 ccsmeth/utils/lookahead.py
 ccsmeth/utils/process_utils.py
 ccsmeth/utils/ranger2020.py
 ccsmeth/utils/ref_reader.py
 ccsmeth/utils/sam2fastq_std.py
```

### Comparing `ccsmeth-0.4.0/setup.py` & `ccsmeth-0.4.1/setup.py`

 * *Files identical despite different names*

