# Comparing `tmp/learnMSA-1.2.3.tar.gz` & `tmp/learnMSA-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learnMSA-1.2.3.tar", last modified: Tue Jun 13 16:56:47 2023, max compression
+gzip compressed data, was "learnMSA-1.2.4.tar", last modified: Thu Jun 15 06:46:30 2023, max compression
```

## Comparing `learnMSA-1.2.3.tar` & `learnMSA-1.2.4.tar`

### file list

```diff
@@ -1,292 +1,292 @@
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.483928 learnMSA-1.2.3/
--rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-13 16:56:47.483622 learnMSA-1.2.3/PKG-INFO
--rw-r--r--   0 jovyan   (17731) root         (0)     3721 2023-06-07 06:46:13.000000 learnMSA-1.2.3/README.md
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.141970 learnMSA-1.2.3/learnMSA/
--rw-r--r--   0 jovyan   (17731) root         (0)       33 2023-01-12 09:31:05.000000 learnMSA-1.2.3/learnMSA/__init__.py
--rw-r--r--   0 jovyan   (17731) root         (0)       21 2023-06-13 16:51:52.000000 learnMSA-1.2.3/learnMSA/_version.py
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.170435 learnMSA-1.2.3/learnMSA/msa_hmm/
--rw-r--r--   0 jovyan   (17731) root         (0)    34665 2023-06-13 16:22:00.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Align.py
--rw-r--r--   0 jovyan   (17731) root         (0)     6542 2023-06-12 08:50:18.000000 learnMSA-1.2.3/learnMSA/msa_hmm/AlignInsertions.py
--rw-r--r--   0 jovyan   (17731) root         (0)    34733 2023-06-13 16:50:24.000000 learnMSA-1.2.3/learnMSA/msa_hmm/AlignmentModel.py
--rw-r--r--   0 jovyan   (17731) root         (0)    25907 2023-04-17 07:14:46.000000 learnMSA-1.2.3/learnMSA/msa_hmm/AncProbsLayer.py
--rw-r--r--   0 jovyan   (17731) root         (0)     4510 2023-06-01 14:05:27.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Configuration.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7999 2023-02-27 14:23:42.000000 learnMSA-1.2.3/learnMSA/msa_hmm/DirichletMixture.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7519 2023-05-08 08:03:16.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Emitter.py
--rw-r--r--   0 jovyan   (17731) root         (0)    11353 2023-06-01 11:47:09.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Fasta.py
--rw-r--r--   0 jovyan   (17731) root         (0)     6065 2023-04-18 09:17:14.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Initializers.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7824 2023-05-08 09:04:58.000000 learnMSA-1.2.3/learnMSA/msa_hmm/MsaHmmCell.py
--rw-r--r--   0 jovyan   (17731) root         (0)     5645 2023-05-08 08:54:55.000000 learnMSA-1.2.3/learnMSA/msa_hmm/MsaHmmLayer.py
--rw-r--r--   0 jovyan   (17731) root         (0)     9183 2023-04-06 07:04:35.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Priors.py
--rw-r--r--   0 jovyan   (17731) root         (0)     9857 2023-04-18 10:52:29.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Training.py
--rw-r--r--   0 jovyan   (17731) root         (0)    29732 2023-06-01 16:57:53.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Transitioner.py
--rw-r--r--   0 jovyan   (17731) root         (0)     1119 2023-01-12 09:37:48.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Utility.py
--rw-r--r--   0 jovyan   (17731) root         (0)    13807 2023-04-18 10:55:32.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Visualize.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7809 2023-05-08 08:18:25.000000 learnMSA-1.2.3/learnMSA/msa_hmm/Viterbi.py
--rw-r--r--   0 jovyan   (17731) root         (0)      897 2023-06-01 11:39:37.000000 learnMSA-1.2.3/learnMSA/msa_hmm/__init__.py
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.121900 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.175149 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    53002 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1434 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.180630 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   518353 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.185960 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      818 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.190677 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.195447 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    35917 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1627 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.200242 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    68449 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.204997 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    67114 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.209669 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1745 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.214565 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1997 2023-01-12 09:32:03.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.219269 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3913 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1598 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.223857 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     4441 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.228695 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3106 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.233440 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.238122 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   130517 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.243254 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    68173 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1641 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.248347 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   132961 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.256561 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   131626 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.261169 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     9557 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.265645 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.270200 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    11725 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.275076 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    20065 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1617 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.279952 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    18730 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1415 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.284562 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     2249 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.289410 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3005 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.293933 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     4417 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.298497 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     5449 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.303009 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     4114 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.308082 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)   260305 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.312958 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.317652 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      812 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.322486 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    19789 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1610 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.327107 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    36193 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1624 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.331932 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)    34858 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1425 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.338882 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     3761 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.343668 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     6029 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.348283 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     5929 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.352819 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     8473 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.357427 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     7138 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.136268 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.362391 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.367899 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.372833 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.377656 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.382482 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.387380 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.392215 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.397055 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.401979 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.406877 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.412716 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1601 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      792 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.417566 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1709 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.421731 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1673 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      794 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.426391 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1853 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      800 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.431064 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1437 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.435605 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.440515 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     2453 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.445341 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1541 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.450134 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.454812 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.459654 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1685 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.464428 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.469236 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1781 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.474363 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1733 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.479653 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/
--rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/checkpoint
--rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001
--rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.482263 learnMSA-1.2.3/learnMSA/run/
--rw-r--r--   0 jovyan   (17731) root         (0)       41 2022-08-17 06:53:42.000000 learnMSA-1.2.3/learnMSA/run/__init__.py
--rw-r--r--   0 jovyan   (17731) root         (0)     7910 2023-06-08 09:43:01.000000 learnMSA-1.2.3/learnMSA/run/console.py
-drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-13 16:56:47.148664 learnMSA-1.2.3/learnMSA.egg-info/
--rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-13 16:56:46.000000 learnMSA-1.2.3/learnMSA.egg-info/PKG-INFO
--rw-r--r--   0 jovyan   (17731) root         (0)    15625 2023-06-13 16:56:47.000000 learnMSA-1.2.3/learnMSA.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan   (17731) root         (0)        1 2023-06-13 16:56:46.000000 learnMSA-1.2.3/learnMSA.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan   (17731) root         (0)       51 2023-06-13 16:56:46.000000 learnMSA-1.2.3/learnMSA.egg-info/entry_points.txt
--rw-r--r--   0 jovyan   (17731) root         (0)       45 2023-06-13 16:56:46.000000 learnMSA-1.2.3/learnMSA.egg-info/requires.txt
--rw-r--r--   0 jovyan   (17731) root         (0)        9 2023-06-13 16:56:46.000000 learnMSA-1.2.3/learnMSA.egg-info/top_level.txt
--rw-r--r--   0 jovyan   (17731) root         (0)       80 2022-08-09 12:49:25.000000 learnMSA-1.2.3/pyproject.toml
--rw-r--r--   0 jovyan   (17731) root         (0)       38 2023-06-13 16:56:47.484224 learnMSA-1.2.3/setup.cfg
--rw-r--r--   0 jovyan   (17731) root         (0)     1015 2023-02-01 15:12:42.000000 learnMSA-1.2.3/setup.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:30.145690 learnMSA-1.2.4/
+-rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-15 06:46:30.145291 learnMSA-1.2.4/PKG-INFO
+-rw-r--r--   0 jovyan   (17731) root         (0)     3721 2023-06-07 06:46:13.000000 learnMSA-1.2.4/README.md
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.075392 learnMSA-1.2.4/learnMSA/
+-rw-r--r--   0 jovyan   (17731) root         (0)       33 2023-01-12 09:31:05.000000 learnMSA-1.2.4/learnMSA/__init__.py
+-rw-r--r--   0 jovyan   (17731) root         (0)       21 2023-06-14 05:34:10.000000 learnMSA-1.2.4/learnMSA/_version.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.261531 learnMSA-1.2.4/learnMSA/msa_hmm/
+-rw-r--r--   0 jovyan   (17731) root         (0)    34665 2023-06-13 16:22:00.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Align.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     6583 2023-06-14 05:42:02.000000 learnMSA-1.2.4/learnMSA/msa_hmm/AlignInsertions.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    34733 2023-06-13 16:50:24.000000 learnMSA-1.2.4/learnMSA/msa_hmm/AlignmentModel.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    25907 2023-04-17 07:14:46.000000 learnMSA-1.2.4/learnMSA/msa_hmm/AncProbsLayer.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     4510 2023-06-01 14:05:27.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Configuration.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7999 2023-02-27 14:23:42.000000 learnMSA-1.2.4/learnMSA/msa_hmm/DirichletMixture.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7519 2023-05-08 08:03:16.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Emitter.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    11353 2023-06-01 11:47:09.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Fasta.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     6065 2023-04-18 09:17:14.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Initializers.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7824 2023-05-08 09:04:58.000000 learnMSA-1.2.4/learnMSA/msa_hmm/MsaHmmCell.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     5645 2023-05-08 08:54:55.000000 learnMSA-1.2.4/learnMSA/msa_hmm/MsaHmmLayer.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     9183 2023-04-06 07:04:35.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Priors.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     9857 2023-04-18 10:52:29.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Training.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    29732 2023-06-01 16:57:53.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Transitioner.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     1119 2023-01-12 09:37:48.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Utility.py
+-rw-r--r--   0 jovyan   (17731) root         (0)    13807 2023-04-18 10:55:32.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Visualize.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7809 2023-05-08 08:18:25.000000 learnMSA-1.2.4/learnMSA/msa_hmm/Viterbi.py
+-rw-r--r--   0 jovyan   (17731) root         (0)      897 2023-06-01 11:39:37.000000 learnMSA-1.2.4/learnMSA/msa_hmm/__init__.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.015513 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.273040 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    53002 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1434 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.316313 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   518353 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.328598 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      818 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.338312 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.347948 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    35917 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1627 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.377776 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    68449 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.398584 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    67114 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.428994 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1745 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.463063 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1997 2023-01-12 09:32:03.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.506152 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3913 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1598 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.552410 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     4441 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.560936 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3106 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.603441 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    66005 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.677374 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   130517 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      828 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.689293 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    68173 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1641 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.718926 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   132961 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1644 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.766794 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   131626 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.820729 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     9557 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.830670 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.877673 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    11725 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.904821 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    20065 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1617 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.952987 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    18730 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1415 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.998052 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     2249 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.005687 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3005 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.027600 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     4417 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.043619 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     5449 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.088635 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     4114 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.101106 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)   260305 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1444 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.110272 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    17621 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      808 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.141891 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    33749 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      812 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.159859 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    19789 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1610 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.231558 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    36193 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1624 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.255615 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)    34858 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1425 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.265219 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     3761 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.330286 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     6029 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.373939 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     5929 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1606 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.384052 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     8473 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1609 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.450993 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     7138 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)     1412 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.026454 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.477912 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.486767 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.494992 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.504012 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.556191 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.643387 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1413 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.708104 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1529 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.749361 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.814970 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1565 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.824083 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.852948 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1601 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      792 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.861261 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1709 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.889299 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:04.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1673 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      794 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.897363 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1853 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      800 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.928016 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1437 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      789 2022-08-16 08:25:07.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.947431 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.974180 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     2453 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      805 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.983433 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1541 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:29.991622 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:30.000455 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1589 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      791 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:30.040461 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1685 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:30.048557 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1637 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      793 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:30.086710 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1781 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:30.094363 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1733 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      795 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:30.114386 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/
+-rw-r--r--   0 jovyan   (17731) root         (0)       65 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/checkpoint
+-rw-r--r--   0 jovyan   (17731) root         (0)     1973 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001
+-rw-r--r--   0 jovyan   (17731) root         (0)      801 2023-01-12 09:32:05.000000 learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:30.142257 learnMSA-1.2.4/learnMSA/run/
+-rw-r--r--   0 jovyan   (17731) root         (0)       41 2022-08-17 06:53:42.000000 learnMSA-1.2.4/learnMSA/run/__init__.py
+-rw-r--r--   0 jovyan   (17731) root         (0)     7910 2023-06-08 09:43:01.000000 learnMSA-1.2.4/learnMSA/run/console.py
+drwxr-xr-x   0 jovyan   (17731) root         (0)        0 2023-06-15 06:46:28.083632 learnMSA-1.2.4/learnMSA.egg-info/
+-rw-r--r--   0 jovyan   (17731) root         (0)      242 2023-06-15 06:46:27.000000 learnMSA-1.2.4/learnMSA.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan   (17731) root         (0)    15625 2023-06-15 06:46:27.000000 learnMSA-1.2.4/learnMSA.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)        1 2023-06-15 06:46:27.000000 learnMSA-1.2.4/learnMSA.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)       51 2023-06-15 06:46:27.000000 learnMSA-1.2.4/learnMSA.egg-info/entry_points.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)       45 2023-06-15 06:46:27.000000 learnMSA-1.2.4/learnMSA.egg-info/requires.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)        9 2023-06-15 06:46:27.000000 learnMSA-1.2.4/learnMSA.egg-info/top_level.txt
+-rw-r--r--   0 jovyan   (17731) root         (0)       80 2022-08-09 12:49:25.000000 learnMSA-1.2.4/pyproject.toml
+-rw-r--r--   0 jovyan   (17731) root         (0)       38 2023-06-15 06:46:30.146102 learnMSA-1.2.4/setup.cfg
+-rw-r--r--   0 jovyan   (17731) root         (0)     1015 2023-02-01 15:12:42.000000 learnMSA-1.2.4/setup.py
```

### Comparing `learnMSA-1.2.3/README.md` & `learnMSA-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Align.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Align.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/AlignInsertions.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/AlignInsertions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,15 @@
         Args: 
             fasta_file: Fasta file containing the complete sequences.
             lens, starts: Arrays of length n where n is the number of sequences in fasta_file. Indicate how long insertions are and where they start respectively.
             name: Identifier for the location of the slice (e.g. left_flank or match_5).
         """
         at_least_t = lens >= t
         lengths = lens[at_least_t]
-        if lengths.size > k:
-            if verbose:
-                print(f"Long insertions found at {name}: {lengths.size}.")
+        if lengths.size > 1:
             which = np.squeeze(np.argwhere(at_least_t))
             start = starts[at_least_t]
             filename = f"{directory}/slice_{name}"
             to_delete = []
             with open(filename, "w") as slice_file:
                 for j in range(lengths.size):
                     aa_seq = fasta_file.aminoacid_seq_str(which[j])
@@ -34,15 +32,18 @@
                             break
                     if only_non_standard_aa or lengths[j] > max_insertions_len:
                         to_delete.append(j)
                     else:
                         slice_file.write(">"+fasta_file.seq_ids[which[j]]+"\n")
                         slice_file.write(segment+"\n")
             which = np.delete(which, to_delete)
-            return (which, filename)
+            if which.size > k:
+                if verbose:
+                    print(f"Long insertions found at {name}: {which.size}.")
+                return (which, filename)
         
         
 def make_aligned_insertions(am, directory, method="famsa", threads=0, verbose=True):
     if not am.best_model in am.metadata:
         am._build_alignment([am.best_model])
     data = am.metadata[am.best_model]
     num_seq = data.left_flank_len.shape[0]
```

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/AlignmentModel.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/AlignmentModel.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/AncProbsLayer.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/AncProbsLayer.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Configuration.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Configuration.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/DirichletMixture.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/DirichletMixture.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Emitter.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Emitter.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Fasta.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Fasta.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Initializers.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Initializers.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/MsaHmmCell.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/MsaHmmCell.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/MsaHmmLayer.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/MsaHmmLayer.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Priors.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Priors.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Training.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Training.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Transitioner.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Transitioner.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Utility.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Utility.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Visualize.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Visualize.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/Viterbi.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/Viterbi.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/__init__.py` & `learnMSA-1.2.4/learnMSA/msa_hmm/__init__.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/100_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1024_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/128_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/1_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/256_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/32_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/3_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/512_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/64_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_False_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float32__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_True_float64__dirichlet/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/9_components_prior_pdf/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_1_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/delete_prior_2_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_1_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_2_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_3_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/insert_prior_5_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_10_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_1_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_2_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_3_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float32/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index` & `learnMSA-1.2.4/learnMSA/msa_hmm/trained_prior/transition_priors/match_prior_5_float64/ckpt.index`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA/run/console.py` & `learnMSA-1.2.4/learnMSA/run/console.py`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/learnMSA.egg-info/SOURCES.txt` & `learnMSA-1.2.4/learnMSA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `learnMSA-1.2.3/setup.py` & `learnMSA-1.2.4/setup.py`

 * *Files identical despite different names*

