# Comparing `tmp/resimpyx-0.0.0.3.tar.gz` & `tmp/resimpyx-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resimpyx-0.0.0.3.tar", last modified: Thu Jun 15 12:01:34 2023, max compression
+gzip compressed data, was "dist\resimpyx-0.0.1.tar", last modified: Wed Jan  5 02:00:41 2022, max compression
```

## Comparing `resimpyx-0.0.0.3.tar` & `resimpyx-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,126 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 12:01:34.896513 resimpyx-0.0.0.3/
--rw-rw-rw-   0        0        0     1089 2021-07-19 17:27:05.000000 resimpyx-0.0.0.3/LICENSE
--rw-rw-rw-   0        0        0      372 2023-06-15 12:01:34.893514 resimpyx-0.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7565 2022-01-05 22:42:22.000000 resimpyx-0.0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 12:01:34.888512 resimpyx-0.0.0.3/resimpyx.egg-info/
--rw-rw-rw-   0        0        0      372 2023-06-15 12:01:34.000000 resimpyx-0.0.0.3/resimpyx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-06-15 12:01:34.000000 resimpyx-0.0.0.3/resimpyx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 12:01:34.000000 resimpyx-0.0.0.3/resimpyx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      219 2023-06-15 12:01:34.000000 resimpyx-0.0.0.3/resimpyx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       70 2023-06-15 12:01:34.000000 resimpyx-0.0.0.3/resimpyx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 12:01:34.000000 resimpyx-0.0.0.3/resimpyx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 12:01:34.896513 resimpyx-0.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1133 2023-06-15 12:01:27.000000 resimpyx-0.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/
+-rw-rw-rw-   0        0        0      355 2022-01-05 02:00:41.000000 resimpyx-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1131 2021-10-31 14:11:38.000000 resimpyx-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/
+-rw-rw-rw-   0        0        0      413 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/Path.py
+-rw-rw-rw-   0        0        0      207 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/gmat/
+-rw-rw-rw-   0        0        0     2751 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/gmat/FromSimulator.py
+-rw-rw-rw-   0        0        0       60 2022-01-05 01:29:13.000000 resimpyx-0.0.1/resimpy/gmat/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/gspl/
+-rw-rw-rw-   0        0        0     1834 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/gspl/FromSimulator.py
+-rw-rw-rw-   0        0        0       58 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/gspl/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/pcr/
+-rw-rw-rw-   0        0        0      932 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/pcr/Amplify.py
+-rw-rw-rw-   0        0        0      956 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/pcr/AmplifyTransloc.py
+-rw-rw-rw-   0        0        0    10707 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/pcr/Error.py
+-rw-rw-rw-   0        0        0    11785 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/pcr/ErrorTransloc.py
+-rw-rw-rw-   0        0        0      136 2022-01-05 01:29:13.000000 resimpyx-0.0.1/resimpy/pcr/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/
+-rw-rw-rw-   0        0        0      185 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/read/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/barcode/
+-rw-rw-rw-   0        0        0      950 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/barcode/Design.py
+-rw-rw-rw-   0        0        0       51 2022-01-05 01:29:13.000000 resimpyx-0.0.1/resimpy/read/barcode/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/inf/
+-rw-rw-rw-   0        0        0      507 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/inf/Pseudo.py
+-rw-rw-rw-   0        0        0       51 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/inf/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/primer/
+-rw-rw-rw-   0        0        0      801 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/primer/Design.py
+-rw-rw-rw-   0        0        0       51 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/primer/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/seq/
+-rw-rw-rw-   0        0        0      637 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/seq/Design.py
+-rw-rw-rw-   0        0        0     1889 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/read/seq/RuleOut.py
+-rw-rw-rw-   0        0        0       75 2022-01-05 01:29:13.000000 resimpyx-0.0.1/resimpy/read/seq/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/similarity/
+-rw-rw-rw-   0        0        0       53 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/similarity/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/similarity/distance/
+-rw-rw-rw-   0        0        0      261 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/similarity/distance/Hamming.py
+-rw-rw-rw-   0        0        0       52 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/similarity/distance/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/spacer/
+-rw-rw-rw-   0        0        0      640 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/spacer/Design.py
+-rw-rw-rw-   0        0        0       51 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/spacer/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/umi/
+-rw-rw-rw-   0        0        0      950 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/umi/Design.py
+-rw-rw-rw-   0        0        0     1559 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/read/umi/Filter.py
+-rw-rw-rw-   0        0        0      843 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/read/umi/Library.py
+-rw-rw-rw-   0        0        0     2458 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/read/umi/RuleOut.py
+-rw-rw-rw-   0        0        0      122 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/umi/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/sequencing/
+-rw-rw-rw-   0        0        0      685 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/sequencing/Calling.py
+-rw-rw-rw-   0        0        0      709 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/sequencing/CallingTransloc.py
+-rw-rw-rw-   0        0        0     6130 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/sequencing/Error.py
+-rw-rw-rw-   0        0        0     6190 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/sequencing/ErrorTransloc.py
+-rw-rw-rw-   0        0        0      136 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/sequencing/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/
+-rw-rw-rw-   0        0        0       81 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/
+-rw-rw-rw-   0        0        0       73 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/
+-rw-rw-rw-   0        0        0    10792 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/Bulk.py
+-rw-rw-rw-   0        0        0    10932 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/CDNA.py
+-rw-rw-rw-   0        0        0    19723 2022-01-05 01:24:08.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/General.py
+-rw-rw-rw-   0        0        0     3938 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/GeneralCondi.py
+-rw-rw-rw-   0        0        0    19001 2022-01-05 01:24:08.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/SingleCell.py
+-rw-rw-rw-   0        0        0     1438 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/UMI.py
+-rw-rw-rw-   0        0        0    19373 2022-01-05 01:24:08.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/UMIDouble.py
+-rw-rw-rw-   0        0        0      196 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/
+-rw-rw-rw-   0        0        0    15638 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/Bulk.py
+-rw-rw-rw-   0        0        0     3904 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/CDNA.py
+-rw-rw-rw-   0        0        0    16455 2022-01-04 23:25:01.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/General.py
+-rw-rw-rw-   0        0        0     3649 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/GeneralCondi.py
+-rw-rw-rw-   0        0        0    15662 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/SingleCell.py
+-rw-rw-rw-   0        0        0     4358 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/UMI.py
+-rw-rw-rw-   0        0        0    16056 2022-01-05 00:09:48.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/UMIDouble.py
+-rw-rw-rw-   0        0        0      196 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/initiator/
+-rw-rw-rw-   0        0        0     6392 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/initiator/Bulk.py
+-rw-rw-rw-   0        0        0     4491 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/simulate/initiator/CDNA.py
+-rw-rw-rw-   0        0        0     5381 2022-01-04 23:41:23.000000 resimpyx-0.0.1/resimpy/simulate/initiator/General.py
+-rw-rw-rw-   0        0        0     6136 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/simulate/initiator/GeneralCondi.py
+-rw-rw-rw-   0        0        0     6524 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/initiator/SingleCell.py
+-rw-rw-rw-   0        0        0     4248 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/initiator/UMI.py
+-rw-rw-rw-   0        0        0     4910 2022-01-05 00:28:26.000000 resimpyx-0.0.1/resimpy/simulate/initiator/UMIDouble.py
+-rw-rw-rw-   0        0        0      196 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/initiator/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/
+-rw-rw-rw-   0        0        0       99 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/file/
+-rw-rw-rw-   0        0        0       94 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/file/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/file/create/
+-rw-rw-rw-   0        0        0      323 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/file/create/Folder.py
+-rw-rw-rw-   0        0        0       51 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/file/create/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/file/read/
+-rw-rw-rw-   0        0        0     2862 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/file/read/Reader.py
+-rw-rw-rw-   0        0        0       53 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/file/read/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/file/write/
+-rw-rw-rw-   0        0        0     2193 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/file/write/Writer.py
+-rw-rw-rw-   0        0        0       51 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/file/write/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/random/
+-rw-rw-rw-   0        0        0     2398 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/random/Number.py
+-rw-rw-rw-   0        0        0     2028 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/random/Ordering.py
+-rw-rw-rw-   0        0        0     2593 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/random/Sampling.py
+-rw-rw-rw-   0        0        0      101 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/random/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/
+-rw-rw-rw-   0        0        0      121 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/convert/
+-rw-rw-rw-   0        0        0     1779 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/util/sequence/convert/Length.py
+-rw-rw-rw-   0        0        0     2229 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/util/sequence/convert/ManyToSingle.py
+-rw-rw-rw-   0        0        0       82 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/convert/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/fasta/
+-rw-rw-rw-   0        0        0     1390 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/sequence/fasta/Read.py
+-rw-rw-rw-   0        0        0       51 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/fasta/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/fastq/
+-rw-rw-rw-   0        0        0     2742 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/fastq/Write.py
+-rw-rw-rw-   0        0        0       52 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/fastq/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/symbol/
+-rw-rw-rw-   0        0        0     2368 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/sequence/symbol/Single.py
+-rw-rw-rw-   0        0        0       53 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/symbol/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpyx.egg-info/
+-rw-rw-rw-   0        0        0      355 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3156 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-01-05 02:00:41.000000 resimpyx-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2022-01-05 02:00:37.000000 resimpyx-0.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `resimpyx-0.0.0.3/setup.py` & `resimpyx-0.0.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 from setuptools import setup, find_packages
 
 setup(
     name="resimpyx",
-    # version="0.0.1",
-    version="0.0.0.3",
+    version="0.0.1",
+    # name="resimpy",
+    # version="0.0.0.0.15",
     keywords=("pip", "resimpy"),
     description="REad SIMulation PY",
     long_description="sequencing read simulation python interface",
     license="MIT",
 
     url="https://github.com/cribbslab; https://github.com/2003100127",
     author="Jianfeng Sun",
     author_email="jianfeng.sun@ndorms.ox.ac.uk",
 
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
-    python_requires='==3.9.1',
+    python_requires='>3.6',
     install_requires=[
-        'numpy==1.22.1',
-        'scipy==1.7.2',
-        'pandas',
+        'pandas==1.3.2',
+        'numpy==1.19.5',
         'rpy2==3.4.5',
         'pyfastx==0.8.4',
+        'scipy==1.7.1',
         'pyfiglet',
-
-        # 'pandas==1.3.2',
-        # 'numpy==1.19.5',
-        # 'cython==0.29.35',
     ],
     entry_points={
         'console_scripts': [
             'resimpy_general=resimpy.simulate.dispatcher.batch.General:run',
             'resimpy_umi_transloc=resimpy.simulate.dispatcher.batch.UMIDouble:run',
             'resimpy_umi_sc=resimpy.simulate.dispatcher.batch.SingleCell:run',
         ],
```

