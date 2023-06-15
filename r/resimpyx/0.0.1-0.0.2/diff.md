# Comparing `tmp/resimpyx-0.0.1.tar.gz` & `tmp/resimpyx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\resimpyx-0.0.1.tar", last modified: Wed Jan  5 02:00:41 2022, max compression
+gzip compressed data, was "resimpyx-0.0.2.tar", last modified: Thu Jun 15 13:58:22 2023, max compression
```

## Comparing `resimpyx-0.0.1.tar` & `resimpyx-0.0.2.tar`

### file list

```diff
@@ -1,126 +1,121 @@
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/
--rw-rw-rw-   0        0        0      355 2022-01-05 02:00:41.000000 resimpyx-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1131 2021-10-31 14:11:38.000000 resimpyx-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/
--rw-rw-rw-   0        0        0      413 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/Path.py
--rw-rw-rw-   0        0        0      207 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/gmat/
--rw-rw-rw-   0        0        0     2751 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/gmat/FromSimulator.py
--rw-rw-rw-   0        0        0       60 2022-01-05 01:29:13.000000 resimpyx-0.0.1/resimpy/gmat/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/gspl/
--rw-rw-rw-   0        0        0     1834 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/gspl/FromSimulator.py
--rw-rw-rw-   0        0        0       58 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/gspl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/pcr/
--rw-rw-rw-   0        0        0      932 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/pcr/Amplify.py
--rw-rw-rw-   0        0        0      956 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/pcr/AmplifyTransloc.py
--rw-rw-rw-   0        0        0    10707 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/pcr/Error.py
--rw-rw-rw-   0        0        0    11785 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/pcr/ErrorTransloc.py
--rw-rw-rw-   0        0        0      136 2022-01-05 01:29:13.000000 resimpyx-0.0.1/resimpy/pcr/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/
--rw-rw-rw-   0        0        0      185 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/read/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/barcode/
--rw-rw-rw-   0        0        0      950 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/barcode/Design.py
--rw-rw-rw-   0        0        0       51 2022-01-05 01:29:13.000000 resimpyx-0.0.1/resimpy/read/barcode/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/inf/
--rw-rw-rw-   0        0        0      507 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/inf/Pseudo.py
--rw-rw-rw-   0        0        0       51 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/inf/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/primer/
--rw-rw-rw-   0        0        0      801 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/primer/Design.py
--rw-rw-rw-   0        0        0       51 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/primer/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/seq/
--rw-rw-rw-   0        0        0      637 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/seq/Design.py
--rw-rw-rw-   0        0        0     1889 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/read/seq/RuleOut.py
--rw-rw-rw-   0        0        0       75 2022-01-05 01:29:13.000000 resimpyx-0.0.1/resimpy/read/seq/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/similarity/
--rw-rw-rw-   0        0        0       53 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/similarity/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/similarity/distance/
--rw-rw-rw-   0        0        0      261 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/similarity/distance/Hamming.py
--rw-rw-rw-   0        0        0       52 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/similarity/distance/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/spacer/
--rw-rw-rw-   0        0        0      640 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/spacer/Design.py
--rw-rw-rw-   0        0        0       51 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/spacer/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/read/umi/
--rw-rw-rw-   0        0        0      950 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/read/umi/Design.py
--rw-rw-rw-   0        0        0     1559 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/read/umi/Filter.py
--rw-rw-rw-   0        0        0      843 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/read/umi/Library.py
--rw-rw-rw-   0        0        0     2458 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/read/umi/RuleOut.py
--rw-rw-rw-   0        0        0      122 2022-01-05 01:29:14.000000 resimpyx-0.0.1/resimpy/read/umi/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/sequencing/
--rw-rw-rw-   0        0        0      685 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/sequencing/Calling.py
--rw-rw-rw-   0        0        0      709 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/sequencing/CallingTransloc.py
--rw-rw-rw-   0        0        0     6130 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/sequencing/Error.py
--rw-rw-rw-   0        0        0     6190 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/sequencing/ErrorTransloc.py
--rw-rw-rw-   0        0        0      136 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/sequencing/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/
--rw-rw-rw-   0        0        0       81 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/
--rw-rw-rw-   0        0        0       73 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/
--rw-rw-rw-   0        0        0    10792 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/Bulk.py
--rw-rw-rw-   0        0        0    10932 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/CDNA.py
--rw-rw-rw-   0        0        0    19723 2022-01-05 01:24:08.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/General.py
--rw-rw-rw-   0        0        0     3938 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/GeneralCondi.py
--rw-rw-rw-   0        0        0    19001 2022-01-05 01:24:08.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/SingleCell.py
--rw-rw-rw-   0        0        0     1438 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/UMI.py
--rw-rw-rw-   0        0        0    19373 2022-01-05 01:24:08.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/UMIDouble.py
--rw-rw-rw-   0        0        0      196 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/
--rw-rw-rw-   0        0        0    15638 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/Bulk.py
--rw-rw-rw-   0        0        0     3904 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/CDNA.py
--rw-rw-rw-   0        0        0    16455 2022-01-04 23:25:01.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/General.py
--rw-rw-rw-   0        0        0     3649 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/GeneralCondi.py
--rw-rw-rw-   0        0        0    15662 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/SingleCell.py
--rw-rw-rw-   0        0        0     4358 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/UMI.py
--rw-rw-rw-   0        0        0    16056 2022-01-05 00:09:48.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/UMIDouble.py
--rw-rw-rw-   0        0        0      196 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/dispatcher/single/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/simulate/initiator/
--rw-rw-rw-   0        0        0     6392 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/initiator/Bulk.py
--rw-rw-rw-   0        0        0     4491 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/simulate/initiator/CDNA.py
--rw-rw-rw-   0        0        0     5381 2022-01-04 23:41:23.000000 resimpyx-0.0.1/resimpy/simulate/initiator/General.py
--rw-rw-rw-   0        0        0     6136 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/simulate/initiator/GeneralCondi.py
--rw-rw-rw-   0        0        0     6524 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/initiator/SingleCell.py
--rw-rw-rw-   0        0        0     4248 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/simulate/initiator/UMI.py
--rw-rw-rw-   0        0        0     4910 2022-01-05 00:28:26.000000 resimpyx-0.0.1/resimpy/simulate/initiator/UMIDouble.py
--rw-rw-rw-   0        0        0      196 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/simulate/initiator/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/
--rw-rw-rw-   0        0        0       99 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/file/
--rw-rw-rw-   0        0        0       94 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/file/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/file/create/
--rw-rw-rw-   0        0        0      323 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/file/create/Folder.py
--rw-rw-rw-   0        0        0       51 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/file/create/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/file/read/
--rw-rw-rw-   0        0        0     2862 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/file/read/Reader.py
--rw-rw-rw-   0        0        0       53 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/file/read/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/file/write/
--rw-rw-rw-   0        0        0     2193 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/file/write/Writer.py
--rw-rw-rw-   0        0        0       51 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/file/write/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/random/
--rw-rw-rw-   0        0        0     2398 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/random/Number.py
--rw-rw-rw-   0        0        0     2028 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/random/Ordering.py
--rw-rw-rw-   0        0        0     2593 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/random/Sampling.py
--rw-rw-rw-   0        0        0      101 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/random/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/
--rw-rw-rw-   0        0        0      121 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/convert/
--rw-rw-rw-   0        0        0     1779 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/util/sequence/convert/Length.py
--rw-rw-rw-   0        0        0     2229 2022-01-04 21:47:29.000000 resimpyx-0.0.1/resimpy/util/sequence/convert/ManyToSingle.py
--rw-rw-rw-   0        0        0       82 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/convert/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/fasta/
--rw-rw-rw-   0        0        0     1390 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/sequence/fasta/Read.py
--rw-rw-rw-   0        0        0       51 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/fasta/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/fastq/
--rw-rw-rw-   0        0        0     2742 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/fastq/Write.py
--rw-rw-rw-   0        0        0       52 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/fastq/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpy/util/sequence/symbol/
--rw-rw-rw-   0        0        0     2368 2022-01-04 20:06:45.000000 resimpyx-0.0.1/resimpy/util/sequence/symbol/Single.py
--rw-rw-rw-   0        0        0       53 2022-01-05 01:43:33.000000 resimpyx-0.0.1/resimpy/util/sequence/symbol/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-05 02:00:41.000000 resimpyx-0.0.1/resimpyx.egg-info/
--rw-rw-rw-   0        0        0      355 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3156 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-01-05 02:00:40.000000 resimpyx-0.0.1/resimpyx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-05 02:00:41.000000 resimpyx-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1075 2022-01-05 02:00:37.000000 resimpyx-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.310783 resimpyx-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2021-07-19 17:27:05.000000 resimpyx-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      367 2023-06-15 13:58:22.309782 resimpyx-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7598 2023-06-15 13:57:51.000000 resimpyx-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.062785 resimpyx-0.0.2/resimpy/
+-rw-rw-rw-   0        0        0      407 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/Path.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.077785 resimpyx-0.0.2/resimpy/pcr/
+-rw-rw-rw-   0        0        0      926 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/pcr/Amplify.py
+-rw-rw-rw-   0        0        0      950 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/pcr/AmplifyTransloc.py
+-rw-rw-rw-   0        0        0    10707 2023-06-15 13:37:29.000000 resimpyx-0.0.2/resimpy/pcr/Error.py
+-rw-rw-rw-   0        0        0    11785 2023-06-15 13:37:29.000000 resimpyx-0.0.2/resimpy/pcr/ErrorTransloc.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/pcr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.079785 resimpyx-0.0.2/resimpy/read/
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/read/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.084783 resimpyx-0.0.2/resimpy/read/barcode/
+-rw-rw-rw-   0        0        0      944 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/barcode/Design.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/read/barcode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.091785 resimpyx-0.0.2/resimpy/read/inf/
+-rw-rw-rw-   0        0        0      501 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/inf/Pseudo.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/read/inf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.097787 resimpyx-0.0.2/resimpy/read/primer/
+-rw-rw-rw-   0        0        0      795 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/primer/Design.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/read/primer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.106784 resimpyx-0.0.2/resimpy/read/seq/
+-rw-rw-rw-   0        0        0      631 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/seq/Design.py
+-rw-rw-rw-   0        0        0     1883 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/seq/RuleOut.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/read/seq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.108784 resimpyx-0.0.2/resimpy/read/similarity/
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/read/similarity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.115784 resimpyx-0.0.2/resimpy/read/similarity/distance/
+-rw-rw-rw-   0        0        0      255 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/similarity/distance/Hamming.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/read/similarity/distance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.121786 resimpyx-0.0.2/resimpy/read/spacer/
+-rw-rw-rw-   0        0        0      634 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/spacer/Design.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/read/spacer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.136784 resimpyx-0.0.2/resimpy/read/umi/
+-rw-rw-rw-   0        0        0      944 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/umi/Design.py
+-rw-rw-rw-   0        0        0     1553 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/umi/Filter.py
+-rw-rw-rw-   0        0        0      837 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/umi/Library.py
+-rw-rw-rw-   0        0        0     2452 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/read/umi/RuleOut.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/read/umi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.153785 resimpyx-0.0.2/resimpy/sequencing/
+-rw-rw-rw-   0        0        0      679 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/sequencing/Calling.py
+-rw-rw-rw-   0        0        0      703 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/sequencing/CallingTransloc.py
+-rw-rw-rw-   0        0        0     6130 2023-06-15 13:37:29.000000 resimpyx-0.0.2/resimpy/sequencing/Error.py
+-rw-rw-rw-   0        0        0     6190 2023-06-15 13:37:29.000000 resimpyx-0.0.2/resimpy/sequencing/ErrorTransloc.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/sequencing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.155785 resimpyx-0.0.2/resimpy/simulate/
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/simulate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.157783 resimpyx-0.0.2/resimpy/simulate/dispatcher/
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.180785 resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/
+-rw-rw-rw-   0        0        0    10786 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/Bulk.py
+-rw-rw-rw-   0        0        0    10926 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/CDNA.py
+-rw-rw-rw-   0        0        0    19736 2023-06-15 12:55:06.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/General.py
+-rw-rw-rw-   0        0        0     3932 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/GeneralCondi.py
+-rw-rw-rw-   0        0        0    18995 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/SingleCell.py
+-rw-rw-rw-   0        0        0     1432 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/UMI.py
+-rw-rw-rw-   0        0        0    19367 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/UMIDouble.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.200784 resimpyx-0.0.2/resimpy/simulate/dispatcher/single/
+-rw-rw-rw-   0        0        0    15632 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/single/Bulk.py
+-rw-rw-rw-   0        0        0     3898 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/single/CDNA.py
+-rw-rw-rw-   0        0        0    16449 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/single/General.py
+-rw-rw-rw-   0        0        0     3643 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/single/GeneralCondi.py
+-rw-rw-rw-   0        0        0    15656 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/single/SingleCell.py
+-rw-rw-rw-   0        0        0     4352 2023-06-15 13:38:04.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/single/UMI.py
+-rw-rw-rw-   0        0        0    16050 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/single/UMIDouble.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/simulate/dispatcher/single/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.222783 resimpyx-0.0.2/resimpy/simulate/initiator/
+-rw-rw-rw-   0        0        0     6386 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/initiator/Bulk.py
+-rw-rw-rw-   0        0        0     4342 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/initiator/CDNA.py
+-rw-rw-rw-   0        0        0     5268 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/initiator/General.py
+-rw-rw-rw-   0        0        0     6056 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/initiator/GeneralCondi.py
+-rw-rw-rw-   0        0        0     6518 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/initiator/SingleCell.py
+-rw-rw-rw-   0        0        0     4168 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/initiator/UMI.py
+-rw-rw-rw-   0        0        0     4871 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/simulate/initiator/UMIDouble.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/simulate/initiator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.224784 resimpyx-0.0.2/resimpy/util/
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.226785 resimpyx-0.0.2/resimpy/util/file/
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.233784 resimpyx-0.0.2/resimpy/util/file/create/
+-rw-rw-rw-   0        0        0      317 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/util/file/create/Folder.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/file/create/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.238788 resimpyx-0.0.2/resimpy/util/file/read/
+-rw-rw-rw-   0        0        0     2786 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/util/file/read/Reader.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/file/read/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.244786 resimpyx-0.0.2/resimpy/util/file/write/
+-rw-rw-rw-   0        0        0     2117 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/util/file/write/Writer.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/file/write/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.254783 resimpyx-0.0.2/resimpy/util/random/
+-rw-rw-rw-   0        0        0     2392 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/util/random/Number.py
+-rw-rw-rw-   0        0        0     2028 2023-06-15 13:37:29.000000 resimpyx-0.0.2/resimpy/util/random/Ordering.py
+-rw-rw-rw-   0        0        0     2587 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/util/random/Sampling.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/random/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.256785 resimpyx-0.0.2/resimpy/util/sequence/
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/sequence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.265785 resimpyx-0.0.2/resimpy/util/sequence/convert/
+-rw-rw-rw-   0        0        0     1779 2023-06-15 13:37:29.000000 resimpyx-0.0.2/resimpy/util/sequence/convert/Length.py
+-rw-rw-rw-   0        0        0     2184 2023-06-15 13:37:29.000000 resimpyx-0.0.2/resimpy/util/sequence/convert/ManyToSingle.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/sequence/convert/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.270784 resimpyx-0.0.2/resimpy/util/sequence/fasta/
+-rw-rw-rw-   0        0        0     1244 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/util/sequence/fasta/Read.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/sequence/fasta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.276783 resimpyx-0.0.2/resimpy/util/sequence/fastq/
+-rw-rw-rw-   0        0        0     2736 2023-06-15 13:38:03.000000 resimpyx-0.0.2/resimpy/util/sequence/fastq/Write.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/sequence/fastq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.281783 resimpyx-0.0.2/resimpy/util/sequence/symbol/
+-rw-rw-rw-   0        0        0     2318 2023-06-15 13:37:29.000000 resimpyx-0.0.2/resimpy/util/sequence/symbol/Single.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 13:13:25.000000 resimpyx-0.0.2/resimpy/util/sequence/symbol/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 13:58:22.304783 resimpyx-0.0.2/resimpyx.egg-info/
+-rw-rw-rw-   0        0        0      367 2023-06-15 13:58:21.000000 resimpyx-0.0.2/resimpyx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3054 2023-06-15 13:58:21.000000 resimpyx-0.0.2/resimpyx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 13:58:21.000000 resimpyx-0.0.2/resimpyx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      219 2023-06-15 13:58:21.000000 resimpyx-0.0.2/resimpyx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-06-15 13:58:21.000000 resimpyx-0.0.2/resimpyx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 13:58:21.000000 resimpyx-0.0.2/resimpyx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 13:58:22.310783 resimpyx-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-06-15 13:58:11.000000 resimpyx-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `resimpyx-0.0.1/resimpy/pcr/Amplify.py` & `resimpyx-0.0.2/resimpy/pcr/AmplifyTransloc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.util.random.Ordering import ordering as ranord
 from resimpy.util.random.Sampling import sampling as ranspl
 from resimpy.util.random.Number import number as rannum
-from resimpy.pcr.Error import error as pcrerr
+from resimpy.pcr.ErrorTransloc import errorTransloc as pcrerr
 
 
-class amplify(object):
+class amplifyTransloc(object):
 
     def __init__(self, pcr_params):
         self.pcr_params = pcr_params
 
     def np(self, ):
         for ipcr in range(self.pcr_params['pcr_num']):
             print('===>at PCR {}'.format(ipcr + 1))
```

### Comparing `resimpyx-0.0.1/resimpy/pcr/AmplifyTransloc.py` & `resimpyx-0.0.2/resimpy/pcr/Amplify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.util.random.Ordering import ordering as ranord
 from resimpy.util.random.Sampling import sampling as ranspl
 from resimpy.util.random.Number import number as rannum
-from resimpy.pcr.ErrorTransloc import errorTransloc as pcrerr
+from resimpy.pcr.Error import error as pcrerr
 
 
-class amplifyTransloc(object):
+class amplify(object):
 
     def __init__(self, pcr_params):
         self.pcr_params = pcr_params
 
     def np(self, ):
         for ipcr in range(self.pcr_params['pcr_num']):
             print('===>at PCR {}'.format(ipcr + 1))
```

### Comparing `resimpyx-0.0.1/resimpy/pcr/Error.py` & `resimpyx-0.0.2/resimpy/pcr/Error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
 __author__ = "Adam Cribbs lab"
 
 import time
 import numpy as np
 import pandas as pd
 from resimpy.util.random.Number import number as rannum
```

### Comparing `resimpyx-0.0.1/resimpy/pcr/ErrorTransloc.py` & `resimpyx-0.0.2/resimpy/pcr/ErrorTransloc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
 __author__ = "Adam Cribbs lab"
 
 import time
 import numpy as np
 import pandas as pd
 from resimpy.util.random.Number import number as rannum
```

### Comparing `resimpyx-0.0.1/resimpy/read/barcode/Design.py` & `resimpyx-0.0.2/resimpy/read/barcode/Design.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.read.umi.Library import library as liblogginger
 from resimpy.read.inf.Pseudo import pseudo as seqpseudo
 
 
 class design(seqpseudo):
```

### Comparing `resimpyx-0.0.1/resimpy/read/primer/Design.py` & `resimpyx-0.0.2/resimpy/read/primer/Design.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.read.inf.Pseudo import pseudo as seqpseudo
 from resimpy.read.umi.Library import library as liblogginger
 
 
 class design(seqpseudo):
```

### Comparing `resimpyx-0.0.1/resimpy/read/seq/Design.py` & `resimpyx-0.0.2/resimpy/read/seq/Design.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.read.inf.Pseudo import pseudo as seqpseudo
 from resimpy.read.umi.Library import library as liblogginger
 
 
 class design(seqpseudo):
```

### Comparing `resimpyx-0.0.1/resimpy/read/seq/RuleOut.py` & `resimpyx-0.0.2/resimpy/read/seq/RuleOut.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.Path import to
 
 
 class ruleOut(object):
 
     def __init__(self, read_summary):
```

### Comparing `resimpyx-0.0.1/resimpy/read/spacer/Design.py` & `resimpyx-0.0.2/resimpy/read/spacer/Design.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.read.inf.Pseudo import pseudo as seqpseudo
 from resimpy.read.umi.Library import library as liblogginger
 
 
 class design(seqpseudo):
```

### Comparing `resimpyx-0.0.1/resimpy/read/umi/Design.py` & `resimpyx-0.0.2/resimpy/read/umi/Design.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.read.umi.Library import library as liblogginger
 from resimpy.read.inf.Pseudo import pseudo as seqpseudo
 
 
 class design(seqpseudo):
```

### Comparing `resimpyx-0.0.1/resimpy/read/umi/Filter.py` & `resimpyx-0.0.2/resimpy/read/umi/Filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.Path import to
 
 
 class filter(object):
 
     def __init__(self, ):
```

### Comparing `resimpyx-0.0.1/resimpy/read/umi/Library.py` & `resimpyx-0.0.2/resimpy/read/umi/Library.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from functools import wraps
 
 
 class library(object):
 
     def __init__(self, *args, **kwargs):
```

### Comparing `resimpyx-0.0.1/resimpy/read/umi/RuleOut.py` & `resimpyx-0.0.2/resimpy/read/umi/RuleOut.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.Path import to
 
 
 class ruleOut(object):
 
     def __init__(self, read_summary):
```

### Comparing `resimpyx-0.0.1/resimpy/sequencing/Calling.py` & `resimpyx-0.0.2/resimpy/sequencing/Calling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.sequencing.Error import error as seqerr
 from resimpy.util.random.Sampling import sampling as ranspl
 
 
 class calling(object):
```

### Comparing `resimpyx-0.0.1/resimpy/sequencing/CallingTransloc.py` & `resimpyx-0.0.2/resimpy/sequencing/CallingTransloc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.sequencing.ErrorTransloc import errorTransloc as seqerr
 from resimpy.util.random.Sampling import sampling as ranspl
 
 
 class callingTransloc(object):
```

### Comparing `resimpyx-0.0.1/resimpy/sequencing/Error.py` & `resimpyx-0.0.2/resimpy/sequencing/Error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
 __author__ = "Adam Cribbs lab"
 
 import time
 import numpy as np
 import pandas as pd
 from resimpy.util.random.Number import number as rannum
```

### Comparing `resimpyx-0.0.1/resimpy/sequencing/ErrorTransloc.py` & `resimpyx-0.0.2/resimpy/sequencing/ErrorTransloc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
 __author__ = "Adam Cribbs lab"
 
 import time
 import numpy as np
 import pandas as pd
 from resimpy.util.random.Number import number as rannum
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/Bulk.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/Bulk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 from resimpy.simulate.dispatcher.single.Bulk import bulk as simubulk
 from resimpy.gspl.FromSimulator import fromSimulator
 from resimpy.Path import to
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/CDNA.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/CDNA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 from resimpy.simulate.dispatcher.single.CDNA import cdna as simucdna
 from resimpy.Path import to
 
 
 class general(object):
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/General.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/General.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import argparse
 from resimpy.simulate.dispatcher.single.General import general as simugeneral
 
 
-class general(object):
+class general():
 
     def __init__(self,
                  mode,
                  permutation_num=10,
                  umi_unit_pattern=1,
                  umi_unit_len_fixed=10,
                  seq_len=20,
@@ -435,14 +435,15 @@
             }
             p = simugeneral(simu_params)
             print(p.ondemandAmplRates())
         return
 
 
 def run():
+    print(123123123132)
     from pyfiglet import Figlet
     vignette1 = Figlet(font='standard')
     print(vignette1.renderText('Resimpy Toolkit'))
     vignette2 = Figlet(font='doom')
     print(vignette2.renderText('Welcome'))
     p = general(
         mode='external',
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/GeneralCondi.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/GeneralCondi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 from resimpy.simulate.dispatcher.single.GeneralCondi import generalCondi as simugcondi
 from resimpy.Path import to
 
 
 class generalCondi(object):
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/SingleCell.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/SingleCell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import argparse
 from resimpy.simulate.dispatcher.single.SingleCell import singleCell as simusc
 from resimpy.gmat.FromSimulator import fromSimulator
 
 
 class singleCell(object):
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/UMI.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/UMI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 
 class umi(object):
 
     def __init__(self, ):
         self.umi_unit_len_fixed = 12
         self.umi_unit_pattern = 1
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/batch/UMIDouble.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/batch/UMIDouble.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import argparse
 from resimpy.simulate.dispatcher.single.UMIDouble import umiDouble as simugeneral
 
 
 class umiDouble(object):
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/single/Bulk.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/single/Bulk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 from resimpy.simulate.initiator.Bulk import bulk as simuip
 from resimpy.pcr.Amplify import amplify as pcr
 from resimpy.sequencing.Calling import calling as seq
 from resimpy.util.sequence.fastq.Write import write as wfastq
 from resimpy.Path import to
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/single/CDNA.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/single/CDNA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.simulate.initiator.CDNA import cdna as simuip
 from resimpy.pcr.Amplify import amplify as pcr
 from resimpy.sequencing.Calling import calling as seq
 from resimpy.util.sequence.fastq.Write import write as wfastq
 from resimpy.Path import to
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/single/General.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/single/General.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 from resimpy.simulate.initiator.General import general as simuip
 from resimpy.pcr.Amplify import amplify as pcr
 from resimpy.sequencing.Calling import calling as seq
 from resimpy.util.sequence.fastq.Write import write as wfastq
 from resimpy.Path import to
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/single/GeneralCondi.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/single/GeneralCondi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 from resimpy.simulate.initiator.GeneralCondi import generalCondi as simuip
 from resimpy.pcr.Amplify import amplify as pcr
 from resimpy.sequencing.Calling import calling as seq
 from resimpy.util.sequence.fastq.Write import write as wfastq
 from resimpy.Path import to
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/single/SingleCell.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/single/SingleCell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 from resimpy.simulate.initiator.SingleCell import singleCell as simuip
 from resimpy.pcr.Amplify import amplify as pcr
 from resimpy.sequencing.Calling import calling as seq
 from resimpy.util.sequence.fastq.Write import write as wfastq
 from resimpy.Path import to
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/single/UMI.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/single/UMI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 from resimpy.simulate.initiator.UMI import umi as simuip
 from resimpy.pcr.Amplify import amplify as pcr
 from resimpy.sequencing.Calling import calling as seq
 from resimpy.util.sequence.fastq.Write import write as wfastq
 from resimpy.Path import to
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/dispatcher/single/UMIDouble.py` & `resimpyx-0.0.2/resimpy/simulate/dispatcher/single/UMIDouble.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 from resimpy.simulate.initiator.UMIDouble import umiDouble as simuip
 from resimpy.pcr.AmplifyTransloc import amplifyTransloc as pcr
 from resimpy.sequencing.CallingTransloc import callingTransloc as seq
 from resimpy.util.sequence.fastq.Write import write as wfastq
 from resimpy.Path import to
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/initiator/Bulk.py` & `resimpyx-0.0.2/resimpy/simulate/initiator/Bulk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import time
 import numpy as np
 from scipy.sparse import coo_matrix
+from resimpy.read.barcode.Design import design as dbc
+from resimpy.read.umi.Design import design as dumi
+from resimpy.read.seq.Design import design as dseq
+from resimpy.read.similarity.distance.Hamming import hamming
 from resimpy.util.random.Sampling import sampling as ranspl
 from resimpy.util.random.Number import number as rannum
 from resimpy.util.file.read.Reader import reader as pfreader
 from resimpy.util.file.create.Folder import folder as crtfolder
 from resimpy.util.sequence.symbol.Single import single as dnasgl
-from resimpy.read.barcode.Design import design as dbc
-from resimpy.read.umi.Design import design as dumi
-from resimpy.read.seq.Design import design as dseq
-from resimpy.read.similarity.distance.Hamming import hamming
 
 
 class bulk(object):
 
     def __init__(self, gspl, is_seed=False, umi_unit_pattern=3, umi_unit_len=12, seq_len=100, is_sv_umi_lib=True, is_sv_seq_lib=True, umi_lib_fpn='./umi.txt', seq_lib_fpn='./seq.txt', working_dir='./simu/', condis=['umi'], sim_thres=2, permutation=0):
         self.pfreader = pfreader()
         self.ranspl = ranspl()
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/initiator/CDNA.py` & `resimpyx-0.0.2/resimpy/simulate/initiator/CDNA.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
-import os, sys
-dis = '../../../'
-sys.path.append(os.path.abspath(dis))
 import time
-# from numba import jit
 from resimpy.util.sequence.fasta.Read import read as sfasta
 from resimpy.util.random.Sampling import sampling as ranspl
 from resimpy.util.random.Number import number as rannum
 from resimpy.util.file.read.Reader import reader as pfreader
 from resimpy.util.file.create.Folder import folder as crtfolder
 from resimpy.util.sequence.symbol.Single import single as dnasgl
 from resimpy.read.umi.Design import design as umi
@@ -95,18 +91,18 @@
         return seqs
 
     def paste(self, seq, umi, primer):
         return primer + umi + seq + umi + ''.join(list(reversed(primer)))
 
 
 if __name__ == "__main__":
-    offset = '../' * 5 + dis
+
     DEFINE = {
-        'cand_pool_fpn': offset + 'data/omics/genomics/fasta/cdna/GRCh38/cdna_n.txt',
-        'cdna_fp': offset + 'data/omics/genomics/fasta/cdna/GRCh38/',
+        'cand_pool_fpn':  'data/omics/genomics/fasta/cdna/GRCh38/cdna_n.txt',
+        'cdna_fp':  'data/omics/genomics/fasta/cdna/GRCh38/',
     }
     # print(DEFINE['cand_pool_fpn'])
     p = cdna(
         cand_pool_fpn=DEFINE['cand_pool_fpn'],
         cdna_fp=DEFINE['cdna_fp'],
         cdna_num=10,
         umi_unit_pattern=3,
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/initiator/General.py` & `resimpyx-0.0.2/resimpy/simulate/initiator/General.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import time
-import os, sys
 import numpy as np
-dis = '../../../'
-sys.path.append(os.path.abspath(dis))
 from resimpy.util.random.Sampling import sampling as ranspl
 from resimpy.util.random.Number import number as rannum
 from resimpy.util.file.read.Reader import reader as pfreader
 from resimpy.util.file.create.Folder import folder as crtfolder
 from resimpy.util.sequence.symbol.Single import single as dnasgl
 from resimpy.read.umi.Design import design as dumi
 from resimpy.read.similarity.distance.Hamming import hamming
@@ -117,15 +114,14 @@
         return seqs
 
     def paste(self, read_struct=[]):
         return ''.join(read_struct)
 
 
 if __name__ == "__main__":
-    from resimpy.Path import to
     DEFINE = {
         '': '',
     }
     # print(DEFINE['cand_pool_fpn'])
     p = general(
         seq_num=50,
         umi_unit_pattern=1,
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/initiator/GeneralCondi.py` & `resimpyx-0.0.2/resimpy/simulate/initiator/GeneralCondi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import time
-import os, sys
 import numpy as np
-dis = '../../../'
-sys.path.append(os.path.abspath(dis))
 from resimpy.util.sequence.fasta.Read import read as sfasta
 from resimpy.util.random.Sampling import sampling as ranspl
 from resimpy.util.random.Number import number as rannum
 from resimpy.util.file.read.Reader import reader as pfreader
 from resimpy.util.file.create.Folder import folder as crtfolder
 from resimpy.util.sequence.symbol.Single import single as dnasgl
 from resimpy.read.umi.Design import design as umi
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/initiator/SingleCell.py` & `resimpyx-0.0.2/resimpy/simulate/initiator/SingleCell.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import time
 import numpy as np
 from resimpy.util.random.Sampling import sampling as ranspl
 from resimpy.util.random.Number import number as rannum
 from resimpy.util.file.read.Reader import reader as pfreader
 from resimpy.util.file.create.Folder import folder as crtfolder
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/initiator/UMI.py` & `resimpyx-0.0.2/resimpy/simulate/initiator/UMI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import time
-import os, sys
 import numpy as np
-dis = '../../../'
-sys.path.append(os.path.abspath(dis))
 from resimpy.util.random.Sampling import sampling as ranspl
 from resimpy.util.random.Number import number as rannum
 from resimpy.util.file.read.Reader import reader as pfreader
 from resimpy.util.file.create.Folder import folder as crtfolder
 from resimpy.util.sequence.symbol.Single import single as dnasgl
 from resimpy.read.umi.Design import design as dumi
 from resimpy.read.similarity.distance.Hamming import hamming
```

### Comparing `resimpyx-0.0.1/resimpy/simulate/initiator/UMIDouble.py` & `resimpyx-0.0.2/resimpy/simulate/initiator/UMIDouble.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import time
 import numpy as np
 from resimpy.util.random.Sampling import sampling as ranspl
 from resimpy.util.random.Number import number as rannum
 from resimpy.util.file.read.Reader import reader as pfreader
 from resimpy.util.file.create.Folder import folder as crtfolder
@@ -105,15 +105,14 @@
         return c
 
     def paste(self, read_struct=[]):
         return ''.join(read_struct)
 
 
 if __name__ == "__main__":
-    from resimpy.Path import to
     DEFINE = {
         '': '',
     }
     # print(DEFINE['cand_pool_fpn'])
     p = umiDouble(
         seq_num=100,
         umi_unit_pattern=3,
```

### Comparing `resimpyx-0.0.1/resimpy/util/file/read/Reader.py` & `resimpyx-0.0.2/resimpy/util/file/read/Reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
-import os
-import sys
-sys.path.append(os.path.abspath('../../../'))
 import pandas as pd
 from functools import wraps
 
 
 class reader(object):
 
     def __init__(self, ):
```

### Comparing `resimpyx-0.0.1/resimpy/util/file/write/Writer.py` & `resimpyx-0.0.2/resimpy/util/file/write/Writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
-import os
-import sys
-sys.path.append(os.path.abspath('../../../'))
 import pandas as pd
 from functools import wraps
 
 
 class writer(object):
 
     def __init__(self, ):
```

### Comparing `resimpyx-0.0.1/resimpy/util/random/Number.py` & `resimpyx-0.0.2/resimpy/util/random/Number.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 from functools import wraps
 
 
 class number(object):
```

### Comparing `resimpyx-0.0.1/resimpy/util/random/Ordering.py` & `resimpyx-0.0.2/resimpy/util/random/Ordering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
 __author__ = "Adam Cribbs lab"
 
 import numpy as np
 import pandas as pd
 from functools import wraps
```

### Comparing `resimpyx-0.0.1/resimpy/util/random/Sampling.py` & `resimpyx-0.0.2/resimpy/util/random/Sampling.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import numpy as np
 import pandas as pd
 from functools import wraps
 
 
 class sampling(object):
```

### Comparing `resimpyx-0.0.1/resimpy/util/sequence/convert/Length.py` & `resimpyx-0.0.2/resimpy/util/sequence/convert/Length.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
 __author__ = "Adam Cribbs lab"
 
 import sys
 
 import pandas as pd
```

### Comparing `resimpyx-0.0.1/resimpy/util/sequence/convert/ManyToSingle.py` & `resimpyx-0.0.2/resimpy/util/sequence/convert/ManyToSingle.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
 __author__ = "Adam Cribbs lab"
 
 import re
-import sys
-sys.path.append('../../../../')
 from Bio import SeqIO
 from resimpy.util.file.write.Writer import writer as pfwriter
 from resimpy.Path import to
 
 
 class manyToSingle(object):
```

### Comparing `resimpyx-0.0.1/resimpy/util/sequence/fasta/Read.py` & `resimpyx-0.0.2/resimpy/util/sequence/fasta/Read.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
-import os, sys
-dis = os.path.abspath("../../../../")
-print(dis)
-sys.path.append(dis)
 from Bio import SeqIO
 from resimpy.read import library as liblogginger
 
 
 class read(object):
 
     def __init__(self):
@@ -37,13 +33,11 @@
             f.write(seq + '\n')
             f.close()
         return 0
 
 
 if __name__ == "__main__":
     p = read()
-    offset = '../' * 7
-    print(offset)
     print(p.get(
-        fasta_path=offset + 'data/omics/genomics/fasta/cdna/GRCh38/',
+        fasta_path= 'data/omics/genomics/fasta/cdna/GRCh38/',
         fasta_name='ENST00000379435.3',
     ))
```

### Comparing `resimpyx-0.0.1/resimpy/util/sequence/fastq/Write.py` & `resimpyx-0.0.2/resimpy/util/sequence/fastq/Write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
-__lab__ = "Adam Cribbs lab"
+__lab__ = "cribbslab"
 
 import gzip
 import pandas as pd
 from functools import wraps
 from resimpy.util.file.create.Folder import folder as crtfolder
```

### Comparing `resimpyx-0.0.1/resimpy/util/sequence/symbol/Single.py` & `resimpyx-0.0.2/resimpy/util/sequence/symbol/Single.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 __version__ = "v1.0"
-__copyright__ = "Copyright 2022"
+__copyright__ = "Copyright 2023"
 __license__ = "MIT"
 __author__ = "Adam Cribbs lab"
 
-import sys
-sys.path.append('../../../../../')
-
 
 class single(object):
 
     def __init__(self, ):
         pass
 
     def trim(action):
```

### Comparing `resimpyx-0.0.1/resimpyx.egg-info/SOURCES.txt` & `resimpyx-0.0.2/resimpyx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
+LICENSE
 README.md
 setup.py
 resimpy/Path.py
 resimpy/__init__.py
-resimpy/gmat/FromSimulator.py
-resimpy/gmat/__init__.py
-resimpy/gspl/FromSimulator.py
-resimpy/gspl/__init__.py
 resimpy/pcr/Amplify.py
 resimpy/pcr/AmplifyTransloc.py
 resimpy/pcr/Error.py
 resimpy/pcr/ErrorTransloc.py
 resimpy/pcr/__init__.py
 resimpy/read/__init__.py
 resimpy/read/barcode/Design.py
```

### Comparing `resimpyx-0.0.1/setup.py` & `resimpyx-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from setuptools import setup, find_packages
 
 setup(
     name="resimpyx",
-    version="0.0.1",
-    # name="resimpy",
-    # version="0.0.0.0.15",
+    version="0.0.2",
+    # version="0.0.0.7",
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
     python_requires='>3.6',
     install_requires=[
-        'pandas==1.3.2',
-        'numpy==1.19.5',
-        'rpy2==3.4.5',
+        'numpy==1.22.1',
+        'scipy==1.7.2',
         'pyfastx==0.8.4',
-        'scipy==1.7.1',
+        'pandas==1.4.1',
         'pyfiglet',
     ],
     entry_points={
         'console_scripts': [
             'resimpy_general=resimpy.simulate.dispatcher.batch.General:run',
             'resimpy_umi_transloc=resimpy.simulate.dispatcher.batch.UMIDouble:run',
             'resimpy_umi_sc=resimpy.simulate.dispatcher.batch.SingleCell:run',
```

