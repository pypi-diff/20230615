# Comparing `tmp/ncOrtho-0.3.9.tar.gz` & `tmp/ncOrtho-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/felixl/PycharmProjects/ncOrtho/dist/.tmp-fekyc34f/ncOrtho-0.3.9.tar", last modified: Thu Feb  9 10:54:16 2023, max compression
+gzip compressed data, was "ncOrtho-0.4.0.tar", last modified: Thu Jun 15 12:30:17 2023, max compression
```

## Comparing `ncOrtho-0.3.9.tar` & `ncOrtho-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.379438 ncOrtho-0.3.9/
--rw-r--r--   0 felixl   (10024) users      (501)    35149 2021-06-22 08:19:32.000000 ncOrtho-0.3.9/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)     6388 2023-02-09 10:54:16.378440 ncOrtho-0.3.9/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)     5798 2022-12-12 15:43:22.000000 ncOrtho-0.3.9/README.md
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.208456 ncOrtho-0.3.9/ncOrtho/
--rw-r--r--   0 felixl   (10024) users      (501)       43 2021-06-22 08:19:32.000000 ncOrtho-0.3.9/ncOrtho/__init__.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.283451 ncOrtho-0.3.9/ncOrtho/analysis/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2021-07-08 09:25:07.000000 ncOrtho-0.3.9/ncOrtho/analysis/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     5931 2021-07-08 10:23:46.000000 ncOrtho-0.3.9/ncOrtho/analysis/concat_alignments_dmp.pl
--rw-r--r--   0 felixl   (10024) users      (501)     1596 2021-07-08 10:23:46.000000 ncOrtho-0.3.9/ncOrtho/analysis/degapper.pl
--rw-r--r--   0 felixl   (10024) users      (501)    11893 2022-12-14 16:24:43.000000 ncOrtho-0.3.9/ncOrtho/analysis/ncAnalyze.py
--rw-r--r--   0 felixl   (10024) users      (501)     7367 2021-11-16 15:22:46.000000 ncOrtho-0.3.9/ncOrtho/blastparser.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.321445 ncOrtho-0.3.9/ncOrtho/check/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2023-02-01 12:48:24.000000 ncOrtho-0.3.9/ncOrtho/check/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     6967 2023-02-09 10:46:00.000000 ncOrtho-0.3.9/ncOrtho/check/core_synteny.py
--rw-r--r--   0 felixl   (10024) users      (501)     6037 2023-02-03 14:32:30.000000 ncOrtho-0.3.9/ncOrtho/check/tmp.py
--rw-r--r--   0 felixl   (10024) users      (501)    14276 2021-11-16 15:30:23.000000 ncOrtho-0.3.9/ncOrtho/cmsearch.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.360446 ncOrtho-0.3.9/ncOrtho/coreset/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2021-06-22 08:19:32.000000 ncOrtho-0.3.9/ncOrtho/coreset/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     6308 2022-12-14 12:48:16.000000 ncOrtho-0.3.9/ncOrtho/coreset/core_reblast.py
--rw-r--r--   0 felixl   (10024) users      (501)     9117 2023-02-09 09:45:50.000000 ncOrtho-0.3.9/ncOrtho/coreset/coreset.py
--rw-r--r--   0 felixl   (10024) users      (501)     8446 2023-02-09 09:41:32.000000 ncOrtho-0.3.9/ncOrtho/coreset/coreset_utils.py
--rw-r--r--   0 felixl   (10024) users      (501)     3163 2021-11-16 15:37:13.000000 ncOrtho-0.3.9/ncOrtho/coreset/createcm.py
--rw-r--r--   0 felixl   (10024) users      (501)     1019 2021-06-22 08:54:38.000000 ncOrtho-0.3.9/ncOrtho/coreset/example_parameters.yaml
--rw-r--r--   0 felixl   (10024) users      (501)     6493 2022-12-14 12:42:11.000000 ncOrtho-0.3.9/ncOrtho/coreset/locate_position.py
--rw-r--r--   0 felixl   (10024) users      (501)     4640 2023-01-30 12:01:49.000000 ncOrtho-0.3.9/ncOrtho/coreset/synteny.py
--rw-r--r--   0 felixl   (10024) users      (501)    17311 2022-12-12 15:44:00.000000 ncOrtho-0.3.9/ncOrtho/coreset/tmp.py
--rw-r--r--   0 felixl   (10024) users      (501)     1971 2021-06-23 13:13:57.000000 ncOrtho-0.3.9/ncOrtho/genparser.py
--rwxr-xr-x   0 felixl   (10024) users      (501)    21811 2022-12-12 16:48:28.000000 ncOrtho-0.3.9/ncOrtho/ncortho.py
--rw-r--r--   0 felixl   (10024) users      (501)      913 2022-12-09 10:21:59.000000 ncOrtho-0.3.9/ncOrtho/utils.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.246447 ncOrtho-0.3.9/ncOrtho.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     6388 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      829 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)      176 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       25 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        8 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/top_level.txt
--rw-r--r--   0 felixl   (10024) users      (501)      103 2021-06-30 12:35:13.000000 ncOrtho-0.3.9/pyproject.toml
--rw-r--r--   0 felixl   (10024) users      (501)       38 2023-02-09 10:54:16.380439 ncOrtho-0.3.9/setup.cfg
--rw-r--r--   0 felixl   (10024) users      (501)     1959 2023-02-09 10:10:05.000000 ncOrtho-0.3.9/setup.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:17.287569 ncOrtho-0.4.0/
+-rw-r--r--   0 felixl   (10024) users      (501)    35149 2021-06-22 08:19:32.000000 ncOrtho-0.4.0/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-15 12:30:17.285568 ncOrtho-0.4.0/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)     6480 2023-03-09 13:27:30.000000 ncOrtho-0.4.0/README.md
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:16.842597 ncOrtho-0.4.0/ncOrtho/
+-rw-r--r--   0 felixl   (10024) users      (501)       43 2021-06-22 08:19:32.000000 ncOrtho-0.4.0/ncOrtho/__init__.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:16.937583 ncOrtho-0.4.0/ncOrtho/analysis/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2021-07-08 09:25:07.000000 ncOrtho-0.4.0/ncOrtho/analysis/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     5931 2021-07-08 10:23:46.000000 ncOrtho-0.4.0/ncOrtho/analysis/concat_alignments_dmp.pl
+-rw-r--r--   0 felixl   (10024) users      (501)     1596 2021-07-08 10:23:46.000000 ncOrtho-0.4.0/ncOrtho/analysis/degapper.pl
+-rw-r--r--   0 felixl   (10024) users      (501)    11977 2023-03-09 15:33:35.000000 ncOrtho-0.4.0/ncOrtho/analysis/ncAnalyze.py
+-rw-r--r--   0 felixl   (10024) users      (501)     7691 2023-06-13 14:46:25.000000 ncOrtho-0.4.0/ncOrtho/blastparser.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:17.006584 ncOrtho-0.4.0/ncOrtho/check/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2023-02-01 12:48:24.000000 ncOrtho-0.4.0/ncOrtho/check/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     8997 2023-03-08 09:37:40.000000 ncOrtho-0.4.0/ncOrtho/check/core_synteny.py
+-rw-r--r--   0 felixl   (10024) users      (501)     6037 2023-02-03 14:32:30.000000 ncOrtho-0.4.0/ncOrtho/check/tmp.py
+-rw-r--r--   0 felixl   (10024) users      (501)    12394 2023-06-14 11:24:43.000000 ncOrtho-0.4.0/ncOrtho/cmsearch.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:17.180570 ncOrtho-0.4.0/ncOrtho/coreset/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2021-06-22 08:19:32.000000 ncOrtho-0.4.0/ncOrtho/coreset/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     6840 2023-06-14 15:25:46.000000 ncOrtho-0.4.0/ncOrtho/coreset/core_reblast.py
+-rw-r--r--   0 felixl   (10024) users      (501)     9906 2023-06-14 15:15:29.000000 ncOrtho-0.4.0/ncOrtho/coreset/coreset.py
+-rw-r--r--   0 felixl   (10024) users      (501)     8473 2023-04-27 13:13:52.000000 ncOrtho-0.4.0/ncOrtho/coreset/coreset_utils.py
+-rw-r--r--   0 felixl   (10024) users      (501)     3813 2023-06-14 15:25:46.000000 ncOrtho-0.4.0/ncOrtho/coreset/createcm.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1019 2021-06-22 08:54:38.000000 ncOrtho-0.4.0/ncOrtho/coreset/example_parameters.yaml
+-rw-r--r--   0 felixl   (10024) users      (501)     7002 2023-06-14 14:54:01.000000 ncOrtho-0.4.0/ncOrtho/coreset/locate_position.py
+-rw-r--r--   0 felixl   (10024) users      (501)     5065 2023-03-20 09:25:58.000000 ncOrtho-0.4.0/ncOrtho/coreset/synteny.py
+-rw-r--r--   0 felixl   (10024) users      (501)      473 2023-06-15 08:43:32.000000 ncOrtho-0.4.0/ncOrtho/figletest.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1971 2021-06-23 13:13:57.000000 ncOrtho-0.4.0/ncOrtho/genparser.py
+-rwxr-xr-x   0 felixl   (10024) users      (501)    16810 2023-06-14 12:32:57.000000 ncOrtho-0.4.0/ncOrtho/ncortho.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1713 2023-06-14 11:59:44.000000 ncOrtho-0.4.0/ncOrtho/reblast.py
+-rw-r--r--   0 felixl   (10024) users      (501)     3749 2023-06-14 11:24:43.000000 ncOrtho-0.4.0/ncOrtho/rna_object.py
+-rw-r--r--   0 felixl   (10024) users      (501)    14873 2023-06-13 09:37:44.000000 ncOrtho-0.4.0/ncOrtho/tmp_old_cmsearch.py
+-rw-r--r--   0 felixl   (10024) users      (501)      989 2023-06-15 12:25:12.000000 ncOrtho-0.4.0/ncOrtho/utils.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-06-15 12:30:16.874590 ncOrtho-0.4.0/ncOrtho.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     7070 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      896 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)      176 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       34 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        8 2023-06-15 12:30:16.000000 ncOrtho-0.4.0/ncOrtho.egg-info/top_level.txt
+-rw-r--r--   0 felixl   (10024) users      (501)      103 2021-06-30 12:35:13.000000 ncOrtho-0.4.0/pyproject.toml
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-06-15 12:30:17.288565 ncOrtho-0.4.0/setup.cfg
+-rw-r--r--   0 felixl   (10024) users      (501)     1979 2023-06-15 08:42:22.000000 ncOrtho-0.4.0/setup.py
```

### Comparing `ncOrtho-0.3.9/LICENSE` & `ncOrtho-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.9/PKG-INFO` & `ncOrtho-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncOrtho
-Version: 0.3.9
+Version: 0.4.0
 Summary:  Targeted ortholog search for miRNAs 
 Home-page: https://github.com/felixlangschied/ncortho
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -22,15 +22,15 @@
 NcOrtho is a tool for the targeted search of orthologous micro RNAs (miRNAs) throughout the tree of life. 
 Conceptually, it works similar to the program [fDOG](https://github.com/BIONF/fDOG) in that a probabilistic model of 
 a reference miRNA is created. For training the model, orthologs of the reference sequence are first identified in 
 a set of taxa that are more closely related to the reference species. In contrast to fDOG, ncOrtho does not train hidden 
 Markov Models but covariance models (CMs) (Eddy & Durbin, 1994) 
 which also model conservation of the miRNA's secondary structure.
 
-![workflow](https://github.com/felixlangschied/ncortho/blob/master/ncOrtho/docs/figure1_ncortho_worklfow.png)
+![workflow](https://github.com/BIONF/ncortho/blob/master/ncOrtho/docs/figure1_ncortho_worklfow.png)
 
 ## Getting Started
 NcOrtho depends on multiple third party applications, some of which are Linux specific.
 All dependencies can be installed with [Anaconda](https://www.anaconda.com/).
 It is recommended to create a new Anaconda environment for this. For example:
 ```
 conda create --name ncOrtho python=3.8
@@ -42,14 +42,15 @@
 * **Python:** version 3 or higher (tested with v3.8)
 
 Tool | Tested version | Anaconda installation
 ------------ | ------------- | -------------
 BLASTn | v2.7.1 | `conda install -c kantorlab blastn`
 Infernal | v1.1.4 | `conda install -c bioconda infernal`
 t_coffee | v13.45 | `conda install -c bioconda t-coffee`
+MUSCLE | v5.1 | `conda install -c bioconda muscle`
 
 ### Installing
 
 After installing all three dependencies, ncOrtho can be installed with `pip`:
 ```
  pip install ncOrtho
 ```
@@ -61,30 +62,37 @@
 
 For this reason, a few questions need to be answered, before we can start constructing covariance models:
 1. What is the reference species?
 2. How phylogenetically diverse will my set of target species be?
 3. From which species should the core set of miRNA orthologs be extracted, which will be used for training the CMs?
 4. Which miRNAs are going to be used for the ortholog search?
 
-You can (soon) find more information on how to answer these questions in the 
-[WIKI](https://github.com/felixlangschied/ncortho/wiki/Creating-miRNA-covariance-models#choosing-core-species).
+To identify suitable core species for a given reference species you can calculate an estimate of conserved synteny 
+given a set of pairwise ortholog predictions with:
+```
+ncCheck -p <parameters.yaml> -o <outdir>
+```
+You can find additional information about ncCheck in the
+[WIKI](https://github.com/BIONF/ncortho/wiki/Choosing-core-species).
+
+
 As soon as you know what your core species are going to be, you will need to collect the following data:
 
 * Genomic sequence in FASTA format (e.g "genomic.fna" from RefSeq)
 * Genome annotation in GFF3 format (e.g. "genomic.gff" from RefSeq)
 * Pairwise orthologs of all proteins between the reference and each core species (more information 
-[here](https://github.com/felixlangschied/ncortho/wiki/Input-Data#pairwise-orthologs)
+[here](https://github.com/BIONF/ncortho/wiki/Input-Data#pairwise-orthologs)
 
 Modify the [example parameters](ncOrtho/coreset/example_parameters.yaml) file to contain all 
 relevant paths to your input files. The "name" property of your reference and core species has to merely be a 
-unique identifier. It is however recommended to use the correct species names to increase readability.
+unique identifier. It is however recommended to use whitespace-free species names to increase readability.
 
 Additional to the parameters file, you will need a tab separated file containing the position and sequence of each 
 miRNA for which a model should be constructed (more information 
-[here](https://github.com/felixlangschied/ncortho/wiki/Input-Data#reference-mirnas)). 
+[here](https://github.com/BIONF/ncortho/wiki/Input-Data#reference-mirnas)). 
 
 You can then start CM construction with:
 ```
 ncCreate -p <parameters.yaml> -n <mirnas.tsv> -o <outdir>
 ```
 If you encounter errors, make sure that:
 * The identifiers in the pairwise orthologs files match the ones in the gff files (use the `-idtype=` flag to use other
@@ -98,19 +106,30 @@
 
 You can start the orthology search with:
 ```
 ncSearch -m <CMs/> -n <mirnas.tsv> -q <query_genome.fa> -r <reference_genome.fa> -o <outdir>
 ```
 
 Use `ncSearch -h` to see all available options for the orthology search or have a look at the 
-[WIKI](https://github.com/felixlangschied/ncortho/wiki/Running-the-orthology-search).
+[WIKI](https://github.com/BIONF/ncortho/wiki/Running-the-orthology-search).
+
+### Phylogenetic Analysis
+
+To facilitate the downstream analyses of miRNA orthologs, we also supply the `ncAnalyze` function:
+```
+ncAnalzye -r <result directory of ncOrtho> -o <output_dir> -m <mappingfile>
+```
+This will create a phylogenetic Profile ready for visualisation in [PhyloProfile](https://github.com/BIONF/PhyloProfile)
+as well as calculate a supermatrix species tree based on the miRNA orthologs.
+
+More information can be found with `ncAnalyze -h` or the [WIKI](https://github.com/BIONF/ncortho/wiki/Analysis)
 
 ## Support
 
-Please refer to our Wiki Page of [known issues](https://github.com/felixlangschied/ncortho/wiki/Known-Issues) first, 
+Please refer to our Wiki Page of [known issues](https://github.com/BIONF/ncortho/wiki/Known-Issues) first, 
 then consider opening an issue on GitHub or contacting me directly via [mail](langschied@bio.uni-frankfurt.de)
 
 ## Contributors
 
 * [Felix Langschied](https://github.com/felixlangschied)
 * [Andreas Blaumeiser](https://github.com/acblaumeiser)
 * Mirko Brüggemann
```

### Comparing `ncOrtho-0.3.9/README.md` & `ncOrtho-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 NcOrtho is a tool for the targeted search of orthologous micro RNAs (miRNAs) throughout the tree of life. 
 Conceptually, it works similar to the program [fDOG](https://github.com/BIONF/fDOG) in that a probabilistic model of 
 a reference miRNA is created. For training the model, orthologs of the reference sequence are first identified in 
 a set of taxa that are more closely related to the reference species. In contrast to fDOG, ncOrtho does not train hidden 
 Markov Models but covariance models (CMs) (Eddy & Durbin, 1994) 
 which also model conservation of the miRNA's secondary structure.
 
-![workflow](https://github.com/felixlangschied/ncortho/blob/master/ncOrtho/docs/figure1_ncortho_worklfow.png)
+![workflow](https://github.com/BIONF/ncortho/blob/master/ncOrtho/docs/figure1_ncortho_worklfow.png)
 
 ## Getting Started
 NcOrtho depends on multiple third party applications, some of which are Linux specific.
 All dependencies can be installed with [Anaconda](https://www.anaconda.com/).
 It is recommended to create a new Anaconda environment for this. For example:
 ```
 conda create --name ncOrtho python=3.8
@@ -25,14 +25,15 @@
 * **Python:** version 3 or higher (tested with v3.8)
 
 Tool | Tested version | Anaconda installation
 ------------ | ------------- | -------------
 BLASTn | v2.7.1 | `conda install -c kantorlab blastn`
 Infernal | v1.1.4 | `conda install -c bioconda infernal`
 t_coffee | v13.45 | `conda install -c bioconda t-coffee`
+MUSCLE | v5.1 | `conda install -c bioconda muscle`
 
 ### Installing
 
 After installing all three dependencies, ncOrtho can be installed with `pip`:
 ```
  pip install ncOrtho
 ```
@@ -44,30 +45,37 @@
 
 For this reason, a few questions need to be answered, before we can start constructing covariance models:
 1. What is the reference species?
 2. How phylogenetically diverse will my set of target species be?
 3. From which species should the core set of miRNA orthologs be extracted, which will be used for training the CMs?
 4. Which miRNAs are going to be used for the ortholog search?
 
-You can (soon) find more information on how to answer these questions in the 
-[WIKI](https://github.com/felixlangschied/ncortho/wiki/Creating-miRNA-covariance-models#choosing-core-species).
+To identify suitable core species for a given reference species you can calculate an estimate of conserved synteny 
+given a set of pairwise ortholog predictions with:
+```
+ncCheck -p <parameters.yaml> -o <outdir>
+```
+You can find additional information about ncCheck in the
+[WIKI](https://github.com/BIONF/ncortho/wiki/Choosing-core-species).
+
+
 As soon as you know what your core species are going to be, you will need to collect the following data:
 
 * Genomic sequence in FASTA format (e.g "genomic.fna" from RefSeq)
 * Genome annotation in GFF3 format (e.g. "genomic.gff" from RefSeq)
 * Pairwise orthologs of all proteins between the reference and each core species (more information 
-[here](https://github.com/felixlangschied/ncortho/wiki/Input-Data#pairwise-orthologs)
+[here](https://github.com/BIONF/ncortho/wiki/Input-Data#pairwise-orthologs)
 
 Modify the [example parameters](ncOrtho/coreset/example_parameters.yaml) file to contain all 
 relevant paths to your input files. The "name" property of your reference and core species has to merely be a 
-unique identifier. It is however recommended to use the correct species names to increase readability.
+unique identifier. It is however recommended to use whitespace-free species names to increase readability.
 
 Additional to the parameters file, you will need a tab separated file containing the position and sequence of each 
 miRNA for which a model should be constructed (more information 
-[here](https://github.com/felixlangschied/ncortho/wiki/Input-Data#reference-mirnas)). 
+[here](https://github.com/BIONF/ncortho/wiki/Input-Data#reference-mirnas)). 
 
 You can then start CM construction with:
 ```
 ncCreate -p <parameters.yaml> -n <mirnas.tsv> -o <outdir>
 ```
 If you encounter errors, make sure that:
 * The identifiers in the pairwise orthologs files match the ones in the gff files (use the `-idtype=` flag to use other
@@ -81,19 +89,30 @@
 
 You can start the orthology search with:
 ```
 ncSearch -m <CMs/> -n <mirnas.tsv> -q <query_genome.fa> -r <reference_genome.fa> -o <outdir>
 ```
 
 Use `ncSearch -h` to see all available options for the orthology search or have a look at the 
-[WIKI](https://github.com/felixlangschied/ncortho/wiki/Running-the-orthology-search).
+[WIKI](https://github.com/BIONF/ncortho/wiki/Running-the-orthology-search).
+
+### Phylogenetic Analysis
+
+To facilitate the downstream analyses of miRNA orthologs, we also supply the `ncAnalyze` function:
+```
+ncAnalzye -r <result directory of ncOrtho> -o <output_dir> -m <mappingfile>
+```
+This will create a phylogenetic Profile ready for visualisation in [PhyloProfile](https://github.com/BIONF/PhyloProfile)
+as well as calculate a supermatrix species tree based on the miRNA orthologs.
+
+More information can be found with `ncAnalyze -h` or the [WIKI](https://github.com/BIONF/ncortho/wiki/Analysis)
 
 ## Support
 
-Please refer to our Wiki Page of [known issues](https://github.com/felixlangschied/ncortho/wiki/Known-Issues) first, 
+Please refer to our Wiki Page of [known issues](https://github.com/BIONF/ncortho/wiki/Known-Issues) first, 
 then consider opening an issue on GitHub or contacting me directly via [mail](langschied@bio.uni-frankfurt.de)
 
 ## Contributors
 
 * [Felix Langschied](https://github.com/felixlangschied)
 * [Andreas Blaumeiser](https://github.com/acblaumeiser)
 * Mirko Brüggemann
```

### Comparing `ncOrtho-0.3.9/ncOrtho/analysis/concat_alignments_dmp.pl` & `ncOrtho-0.4.0/ncOrtho/analysis/concat_alignments_dmp.pl`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.9/ncOrtho/analysis/degapper.pl` & `ncOrtho-0.4.0/ncOrtho/analysis/degapper.pl`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.9/ncOrtho/analysis/ncAnalyze.py` & `ncOrtho-0.4.0/ncOrtho/analysis/ncAnalyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,21 +263,23 @@
     print('# Starting alignments')
     align_out = f'{outdir}/alignments'
     if not os.path.isdir(align_out):
         os.mkdir(align_out)
     for mirna in ortho_dict:
         with tempfile.NamedTemporaryFile(mode='w+') as fp:
             for spec, seq in ortho_dict[mirna].items():
-                if (
-                        spec not in spec_to_skip
-                        and spec in spec_include
-                ):
-                    fp.write(f'>{spec}\n{seq}\n')
+                if spec_to_skip:
+                    if (
+                            spec in spec_to_skip
+                            and spec not in spec_include
+                    ):
+                        continue
+                fp.write(f'>{spec}\n{seq}\n')
             fp.seek(0)
-            aln_cmd = f'muscle -in {fp.name} -out {align_out}/{mirna}.aln'
+            aln_cmd = f'muscle -align {fp.name} -output {align_out}/{mirna}.aln'
             res = sp.run(aln_cmd, shell=True, capture_output=True)
             if res.returncode != 0:
                 print(res.stderr.decode('utf8'))
                 sys.exit()
 
     sys.stdout.flush()
     superm_path = make_supermatrix(outdir)
```

### Comparing `ncOrtho-0.3.9/ncOrtho/blastparser.py` & `ncOrtho-0.4.0/ncOrtho/blastparser.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 along with ncOrtho.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import subprocess as sp
 from Bio import AlignIO
 from Bio.Phylo.TreeConstruction import DistanceCalculator
 import os
-import sys
-
+import logging
 
 def calculate_distance_matrix(aln_path):
     # align reBLAST hits
     aln_cmd = (
         't_coffee {0} -no_warning -quiet -type=dna '
         ' -output=fasta_aln -outfile={0}'.format(aln_path)
     )
@@ -48,26 +47,28 @@
     # blastpath: path to the output file of the reverse BLAST search
     # msl: ncOrtho minimum sequence length threshold
     def __init__(self, mirna, blasthits, msl):
         self.start = mirna.start
         self.end = mirna.end
         self.chromosome = mirna.chromosome
         self.strand = mirna.strand
-        self.refseq = mirna.pre
+        self.refseq = mirna.seq
         del mirna
         self.blasthits = blasthits
         self.msl = msl
 
     def evaluate_besthit(self,):
+        logger = logging.getLogger('ncortho')
+        logger.setLevel(level=logging.DEBUG)
         # with open(self.blastpath) as blastfile:
         #     blasthits = [line.strip().split() for line in blastfile]
         # If no BLAST hit was found, the search failed by default.
         outbool = False
         if not self.blasthits:
-            print('Rejecting: No reciprocal BLAST hit found')
+            logger.info('Rejecting: No reciprocal BLAST hit found')
             return False
         # Otherwise, check if the best hit and the reference miRNA overlap.
         else:
             topscore = float(self.blasthits[0][4])
             for tophit in self.blasthits:
                 if not tophit or float(tophit[4]) < topscore:
                     return False
@@ -81,37 +82,39 @@
                     send = int(tophit[1])
                 else:
                     raise ValueError('re-BLAST on neither plus nor minus strand')
 
                 # Sequences must be on the same contig, otherwise overlap can be
                 # ruled out instantaneously
                 if not sseqid == self.chromosome:
-                    print(f'Rejecting: Contig/Chromosome does not match. Expected {self.chromosome} but found {sseqid}')
+                    logger.info(f'Rejecting: Contig/Chromosome does not match. Expected {self.chromosome} but found {sseqid}')
                 # Contigs match, so overlap is possible.
                 else:
-                    print(f'Start miRNA: {self.start} End miRNA: {self.end}')
-                    print(f'Start BLAST hit: {sstart} End BLAST hit: {send}')
+                    logger.info(f'Start miRNA: {self.start} End miRNA: {self.end}')
+                    logger.info(f'Start BLAST hit: {sstart} End BLAST hit: {send}')
                     # first within second
                     if (
                         (sstart <= self.start <= send)
                         or (sstart <= self.end <= send)
                     ):
                         return True
                     # second within first
                     elif (
                         (self.start <= sstart <= self.end)
                         or (self.start <= send <= self.end)
                     ):
                         return True
                     # No overlap
                     else:
-                        print('Rejecting: No overlap between miRNA and best BLAST hit')
+                        logger.info('Rejecting: No overlap between miRNA and best BLAST hit')
         return outbool
 
     def check_coortholog_ref(self, candidate_seq, out):
+        logger = logging.getLogger('ncortho')
+        logger.setLevel(level=logging.DEBUG)
         # 1) get query sequence
         # 2) get reference sequence
         # 3) get sequence of best blast hit
         # 4) align sequences
         # 5) calculate difference
         # 6) if distance between best blast hit and reference smaller than
         # difference between best hit and candidate, accept candidate -> reBLAST hit co-ortholog instead of reference
@@ -129,34 +132,36 @@
             of.write(self.blasthits[0][12].replace('-', ''))
 
         dm = calculate_distance_matrix(tmp_out)
         distance_hit_query = dm['best_hit', 'candidate']
         distance_ref_hit = dm['best_hit', 'reference']
 
         if distance_ref_hit < distance_hit_query:
-            print(
+            logger.info(
                 "\t Distance query - BLAST hit: %6.4f, Distance blast hit - reference: %6.4f\tAccepting\n"
                 %(distance_hit_query, distance_ref_hit)
             )
             return True
         else:
-            print(
+            logger.info(
                 "\t Distance query - BLAST hit: %6.4f, Distance blast hit - reference: %6.4f\tRejecting\n"
                 %(distance_hit_query, distance_ref_hit)
             )
             return False
 
 
 class ReBlastParser(object):
     def __init__(self, mirna, reblast_dict):
-        self.refseq = mirna.pre
+        self.refseq = mirna.seq
         self.hits = reblast_dict
         self.best_candidate = list(reblast_dict.keys())[0]
 
     def verify_coorthologs(self, out):
+        logger = logging.getLogger('ncortho')
+        logger.setLevel(level=logging.DEBUG)
         out_dict = {}
         # get process id to ensure that the correct library is used when running ncOrtho in parallel
         pid = os.getpid()
         tmp_out = '{0}/{1}.fa'.format(out, pid)
         with open(tmp_out, 'w') as of:
             of.write('>reference\n')
             of.write(f'{self.refseq}\n')
@@ -168,13 +173,13 @@
         for candidate in self.hits:
             if candidate == self.best_candidate:
                 out_dict[candidate] = self.hits[candidate]
             else:
                 distance_candidates = dm[self.best_candidate, candidate]
                 distance_best_ref = dm[self.best_candidate, 'reference']
                 if distance_candidates < distance_best_ref:
-                    print(
+                    logger.info(
                         f'co-ortholog detected: distance of best candidate to {candidate} {distance_candidates} '
                         f'compared to distance of best candidate to reference of {distance_best_ref}'
                     )
                     out_dict[candidate] = self.hits[candidate]
         return out_dict
```

### Comparing `ncOrtho-0.3.9/ncOrtho/check/core_synteny.py` & `ncOrtho-0.4.0/ncOrtho/check/tmp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,17 @@
 import argparse
 import sys
 import os
+from collections import Counter
 import pandas as pd
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 import ncOrtho.coreset.coreset_utils as cu
 
-
-def neighbors(prot, anno, anchordist):
-    if prot not in anno:  # pseudogenes are not in parsed annotation file but can occur in ortholog file
-        return None
-    chrom, position = anno[prot]
-    anchors = []
-    for index in range(position - anchordist, position + anchordist + 1):
-        if index not in anno[chrom]:  # if gene positioned at end of contig, no more anchors can be considered
-            continue
-        anchor, a_start, a_end, a_strand = anno[chrom][index]
-        anchors.append(anchor)
-    anchors.remove(prot)
-    return anchors
-
-
-def synteny_distance(block, ref_prot, coreanno, orthodict, anchordist, corespecies):
-    """
-    returns: Number of conserved anchors per number of anchors
-    """
-    o = []
-
-    # find position of reference protein orthologs in core species
-    reforthos = orthodict[ref_prot]
-    for refortho in reforthos:
-        if refortho not in coreanno:  # pseudogenes are not in parsed annotation file but can occur in ortholog file
-            continue
-        conserved_anchors = 0
-        chrom, position = coreanno[refortho]
-
-        # find position of anchor protein orthologs in core species
-        for anchor in block:
-
-            # find orthologs of anchor proteins
-            if anchor not in orthodict:  # synteny not fulfilled if no ortholog in core species
-                # c.append(0)
-                continue
-            anchor_ortho_list = orthodict[anchor]
-            for anchor_ortho in anchor_ortho_list:
-                if anchor_ortho not in coreanno:  # e.g. for pseudogenes
-                    # c.append(0)
-                    continue
-
-                a_chrom, a_position = coreanno[anchor_ortho]
-                # if distance to reference protein is similar in core species than in reference species, accept
-                if a_chrom == chrom and abs(int(position) - int(a_position)) <= anchordist:
-                    conserved_anchors += 1
-                    break
-
-                # c.append(0)
-        # o.append(sum(c) / len(c))
-        o.append([corespecies, refortho, conserved_anchors])
-    return o
-
-
 def main():
     # Print header
     print('\n' + '#' * 38, flush=True)
     print('###' + ' ' * 32 + '###', flush=True)
     print('###   ncOrtho - core set synteny   ###', flush=True)
     print('###' + ' ' * 32 + '###', flush=True)
     print('#' * 38 + '\n', flush=True)
@@ -78,99 +25,130 @@
     )
     parser._action_groups.pop()
     required = parser.add_argument_group('Required Arguments')
     optional = parser.add_argument_group('Optional Arguments')
     # input file path
     required.add_argument('-p', '--parameters', metavar='<path>', type=str, required=True,
                           help='Path to the parameters file in yaml format')
-    # output folder
-    required.add_argument(
-        '-o', '--output', metavar='<path>', type=str, required=True,
-        help='Path for the output folder'
-    )
     optional.add_argument(
         '--max_anchor_dist', metavar='int', type=int,
         help='Number of additional genes to the left and right '
              'of the reference miRNA that are to be considered as syntenic anchors. (Default: 3)',
         nargs='?', const=3, default=3
     )
     optional.add_argument(
         '--idtype', metavar='str', type=str,
         help='Choose the ID in the reference gff file that is '
              'compared to the IDs in the pairwise orthologs file (default:GeneID) '
-             'Options: ID, Name, GeneID, gene_id, CDS',
+             'Options: ID, Name, GeneID, gene_id',
         nargs='?', const='ID=', default='ID'
     )
-    optional.add_argument(
-        '--outformat', metavar='str', type=str,
-        help='Choose format for output figures, as accepted by matplotlib package (Default: png)',
-        nargs='?', const='png', default='png'
-    )
     # Show help when no arguments are added.
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
     else:
         args = parser.parse_args()
 
     # parameters
     add_pos_orthos = args.max_anchor_dist
     idtype = args.idtype
 
     core_dict, ref_paths, all_paths = cu.parse_yaml(args.parameters)
     # check if files exist
-    # for cp in all_paths:
-    #    if not os.path.isfile(cp):
-    #        raise ValueError(f'{cp} does not exist')
+    for cp in all_paths:
+        if not os.path.isfile(cp):
+            raise ValueError(f'{cp} does not exist')
 
-    ref_anno_dict = cu.gff_parser(ref_paths['annotation'], 'ID')
     print('# Reading pairwise orthologs', flush=True)
-    if idtype == 'CDS':
-        ortho_dict = cu.pairwise_orthologs_from_cds(core_dict, ref_paths['annotation'])
-    else:
-        ortho_dict = cu.read_pairwise_orthologs(core_dict)
+    ortho_dict = cu.read_pairwise_orthologs(core_dict)
+
+
+    def neighbors(prot, anno, anchordist):
+        if prot not in anno:  # pseudogenes are not in parsed annotation file but can occur in ortholog file
+            return None
+        chrom, position = anno[prot]
+        anchors = []
+        for index in range(position - anchordist, position + anchordist + 1):
+            if index not in anno[chrom]:  # if gene positioned at end of contig, no more anchors can be considered
+                continue
+            anchor, a_start, a_end, a_strand = anno[chrom][index]
+            anchors.append(anchor)
+        anchors.remove(prot)
+        return anchors
+
+
+    def synteny_distance(block, ref_prot, coreanno, orthodict, anchordist, corespecies, mgi=3):
+        """
+        returns: Number of conserved anchors per number of anchors
+        """
+        o = []
+
+        # find position of reference protein orthologs in core species
+        reforthos = orthodict[ref_prot]
+        for refortho in reforthos:
+            conserved_anchors = 0
 
+            if refortho not in coreanno:  # pseudogenes are not in parsed annotation file but can occur in ortholog file
+                continue
+            chrom, position = coreanno[refortho]
+
+            # find position of anchor protein orthologs in core species
+            for anchor in block:
+
+                # find orthologs of anchor proteins
+                if anchor not in orthodict:  # synteny not fulfilled if no ortholog in core species
+                    # c.append(0)
+                    continue
+                anchor_ortho_list = orthodict[anchor]
+                for anchor_ortho in anchor_ortho_list:
+                    if anchor_ortho not in coreanno:  # e.g. for pseudogenes
+                        # c.append(0)
+                        continue
+
+                    a_chrom, a_position = coreanno[anchor_ortho]
+                    # if distance to reference protein is similar in core species than in reference species, accept
+                    if a_chrom == chrom and abs(int(position) - int(a_position)) <= anchordist + mgi:
+                        conserved_anchors += 1
+                        break
+
+                    # c.append(0)
+            # o.append(sum(c) / len(c))
+            o.append([corespecies, refortho, conserved_anchors])
+        return o
+
+
+    print('# Evaluating synteny')
+    ref_anno_dict = cu.parse_annotation(ref_paths['annotation'], idtype)
+    #syn_col = {}
     syn_col = []
-    ortho_col = []
-    print('# Checking synteny conservation', flush=True)
     for corespec, pairwiseorthos in ortho_dict.items():
-
-        core_col = []
+        #core_col = []
         print(corespec)
-        ortho_col.append([corespec, len(pairwiseorthos.keys())])
 
-        core_anno_dict = cu.gff_parser(core_dict[corespec]['annotation'], 'ID')
+        core_anno_dict = cu.parse_annotation(core_dict[corespec]['annotation'], idtype)
 
-        for refprot in pairwiseorthos.keys():
+        for refprot in pairwiseorthos:
             syn_block = neighbors(refprot, ref_anno_dict, add_pos_orthos)
             if not syn_block:  # in rare case that reference protein from orthology file is not found in annotation
                 continue
-            syn_fullfilled_list = synteny_distance(syn_block, refprot, core_anno_dict, pairwiseorthos, add_pos_orthos,
-                                                   corespec)
+            syn_fullfilled_list = synteny_distance(syn_block, refprot, core_anno_dict, pairwiseorthos, add_pos_orthos, corespec)
             syn_col.extend(syn_fullfilled_list)
 
-    orth = pd.DataFrame(ortho_col, columns=['species', 'Number orthologs'])
-    orth = orth.sort_values(by='Number orthologs', ascending=False)
-    o = orth.species.values
-    sns.set(rc={'figure.figsize': (6, 6), 'ytick.left': True, 'xtick.bottom': True}, font_scale=1.2, style='whitegrid')
-    sns.barplot(data=orth, x='species', y='Number orthologs')
-    plt.xticks(rotation=45, ha='right')
-    plt.xlabel('')
-    plt.tight_layout()
-    plt.savefig(f'{args.output}/ortholog_distribution.{args.outformat}')
+        #syn_col[corespec] = dict(Counter(core_col))
 
-
-    plt.clf()
-    plt.figure(figsize=(12, 4))
+    #print(syn_col)
     df = pd.DataFrame(syn_col, columns=['species', 'reference_protein', 'num_conserved_anchors'])
+    #display(df)
+
+    o = ['Gorilla_gorilla', 'Macaca_mulatta', 'Pongo_abelii', 'Nomascus_leucogenys', 'Saimiri_boliviensis',
+         'Mus_musculus', 'Cavia_porcellus', 'Canis_familiaris', 'Gallus_gallus']
     sns.set(rc={'figure.figsize': (12, 4), 'ytick.left': True, 'xtick.bottom': True}, font_scale=1.2, style='whitegrid')
     ax = sns.histplot(data=df, x='num_conserved_anchors', hue='species', discrete=True, multiple='dodge', hue_order=o,
                       shrink=0.8)
     sns.move_legend(ax, "upper left", bbox_to_anchor=(1, 1))
-    plt.xlabel(f'Number of conserved anchors in neighborhood k={add_pos_orthos}')
-    plt.tight_layout()
-    plt.savefig(f'{args.output}/anchor_conservation.{args.outformat}')
-    print(f'# Finished. Output created at: {args.output}')
+    plt.show()
+
 
 
 if __name__ == '__main__':
-    main()
+    main()
```

### Comparing `ncOrtho-0.3.9/ncOrtho/cmsearch.py` & `ncOrtho-0.4.0/ncOrtho/cmsearch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,301 +1,224 @@
-"""
-ncOrtho - Targeted ortholog search for miRNAs
-Copyright (C) 2021 Felix Langschied
-
-ncOrtho is a free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-ncOrtho is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with ncOrtho.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
 import pyfaidx
 import subprocess as sp
 import os
-import sys
-
-
-def candidate_blast(db, c, evalue, seq, task):
-    # extract candidate regions
-    print('# Identifying candidate regions for cmsearch heuristic')
-    blast_command = (
-        'blastn -task {0} -db {1} '
-        '-num_threads {2} -evalue {3} '
-        '-outfmt "6 sseqid sstart send sstrand length"'.format(task, db, c, evalue)
-    )
-    blast_call = sp.Popen(
-        blast_command, shell=True, stdin=sp.PIPE, stdout=sp.PIPE, stderr=sp.PIPE, encoding='utf8'
-    )
-    res, err = blast_call.communicate(seq)
-    return res, err
+import logging
 
 
+def heuristic_search(blastdb, rna, query, heuristic, cpu, out):
 
-def cmsearcher(mirna, cm_cutoff, cpu, msl, models, query, blastdb, out, cleanup, heuristic):
-    """
-    Parameters
-    ----------
-    mirna       :   Mirna object
-    cm_cutoff   :   Minimum bit score of the CMsearch hit relative to the
-                    bit score that results from searching in the reference genome with the same model
-    cpu         :   Number of cores to use
-    msl         :   Minimum length of CMsearch hit relative to the reference pre-miRNA length
-    models      :   Path to the directory that contains the CMs
-    query       :   Path to the query genome
-    blastdb     :   Optional Path to a BLASTdb of the query genome
-    out         :   Path to the output directory
-    cleanup     :   Delete intermediate files True/False
-    heuristic   :   Should heuristic mode be used and if yes, set parameters (True/False, evalue, minlength)
-
-    Returns
-    -------
-    cm_results : Dictionary containing hits of the cmsearch
-
-    """
-    mirna_id = mirna.name
-    cm_results = False
-    # Calculate the bit score cutoff.
-    cut_off = mirna.bit * cm_cutoff
-    # Calculate the length cutoff.
-    len_cut = len(mirna.pre) * msl
-    blast_len_cut = len(mirna.pre) * heuristic[2]
-    # if no model exists for mirna return False
-    if not os.path.isfile('{}/{}.cm'.format(models, mirna_id)):
-        print('# No model found for {}. Skipping..'.format(mirna_id))
-        exitstatus = 'No covariance model found'
-        return cm_results, exitstatus
-    # Perform covariance model search.
-    # Report and inclusion thresholds set according to cutoff.
-
-    if heuristic[0]:
+    def candidate_blast(db, c, evalue, seq, task):
         # extract candidate regions
-        #candidate_blast(db, c, evalue, seq, task):
-        res, err = candidate_blast(blastdb, cpu, heuristic[1], mirna.pre, 'blastn')
-        if not err and not res:
-            print('No BLASTn candidate regions with pre-miRNA. Trying mature sequence')
-            res, err = candidate_blast(blastdb, cpu, 10, mirna.mature, 'blastn-short')
-            # turn off length blast length cutoff
-            blast_len_cut = 0
+        blast_command = (
+            'blastn -task {0} -db {1} '
+            '-num_threads {2} -evalue {3} '
+            '-outfmt "6 sseqid sstart send sstrand length"'.format(task, db, c, evalue)
+        )
+        blast_call = sp.Popen(
+            blast_command, shell=True, stdin=sp.PIPE, stdout=sp.PIPE, stderr=sp.PIPE, encoding='utf8'
+        )
+        res, err = blast_call.communicate(seq)
         if err:
-            print(f'ERROR: {err}')
-            exitstatus = 'ERROR during candidate region BLAST search'
-            return cm_results, exitstatus
+            raise sp.SubprocessError(err)
 
-        # print('Blast step finished')
         result = list(filter(None, res.split('\n')))
         hit_list = [line.split() for line in result if line and float(line.split()[-1]) >= blast_len_cut]
-        if not hit_list:
-            exitstatus = 'No BLASTn candidate regions above length cutoff'
-            return cm_results, exitstatus
-        # hit_list = [line.split() for line in result if line]
-        print(f'# Found {len(hit_list)} BLAST hits of the reference '
-              f'pre-miRNA in the query')
-        genes = pyfaidx.Fasta(query)
-        # collect heuristic sequences
-        # print('collecting sequences')
-        # set border regions to include in analysis
-        extraregion = 1000
-        diff_dict = {}
+
+        return hit_list
+
+    def extract_candidate_regions(candidate_list, query, extraregion=1000):
         hit_at_start = False
         hit_at_end = False
-        heuristic_fa = '{0}/candidate_region_{1}.out'.format(out, mirna_id)
-        with open(heuristic_fa, 'w') as of:
-            for hit in hit_list:
-                chrom, start, end, strand, length = hit
-                strand = strand.replace('plus', '+')
-                strand = strand.replace('minus', '-')
-                if strand == '-':
-                    start, end = end, start
-                header = ">{}|{}|{}|{}\n".format(chrom, start, end, strand)
-                # print(header)
-                start = int(start)
-                end = int(end)
-                if start > extraregion:
-                    n_start = start - extraregion
-                else:
-                    # hit starts at the beginning of the chromosome
-                    n_start = 0
-                    hit_at_start = True
-                n_end = end + extraregion
-                if n_end > genes[chrom][-1].end:
-                    # hit is at the end of the chromosome
-                    n_end = genes[chrom][-1].end
-                    hit_at_end = True
-                if strand == '+':
-                    sequence = genes[chrom][n_start:n_end].seq
-                elif strand == '-':
-                    sequence = genes[chrom][n_start:n_end].reverse.complement.seq
-                header = ">{}|{}|{}|{}|{}|{}\n".format(chrom, start, end, strand, hit_at_start, hit_at_end)
-                of.write(header)
-                of.write(f'{sequence}\n')
+        genome = pyfaidx.Fasta(query)
+
+        regions = []
+        for hit in candidate_list:
+            chrom, start, end, strand, length = hit
+            strand = strand.replace('plus', '+').replace('minus', '-')
+            if strand == '-':
+                start, end = end, start
+            start = int(start)
+            end = int(end)
+
+            if start > extraregion:
+                n_start = start - extraregion
+            else:
+                # hit starts at the beginning of the chromosome
+                n_start = 0
+                hit_at_start = True
+            n_end = end + extraregion
+            if n_end > genome[chrom][-1].end:
+                # hit is at the end of the chromosome
+                n_end = genome[chrom][-1].end
+                hit_at_end = True
+            if strand == '+':
+                sequence = genome[chrom][n_start:n_end].seq
+            elif strand == '-':
+                sequence = genome[chrom][n_start:n_end].reverse.complement.seq
+            else:
+                raise ValueError(f'Unknown strand {strand}')
+            regions.append(f">{chrom}|{str(start)}|{str(end)}|{strand}|{hit_at_start}|{hit_at_end}\n{sequence}\n")
+
+        return regions
+
+
+    ################################################################################################
+    blast_len_cut = len(rna.seq) * heuristic[2]
+    candidate_list = candidate_blast(blastdb, cpu, heuristic[1], rna.seq, 'blastn')
+    if not candidate_list:
+        return ''
+
+    candidate_regions = extract_candidate_regions(candidate_list, query)
+    fasta = f'{out}/candidate_regions_{rna.name}.fa'
+    with open(fasta, 'w') as of:
+        for line in candidate_regions:
+            of.write(line)
+
+    return fasta
+
+
+#[
+# ['(1)', '!', '3.7e-23', '94.0', '0.0', 'NW_020173731.1|9158415|9158472|+|False|False', '1000', '1057', '+', 'cm', 'no', '0.41', '-'],
+# ['(2)', '!', '3.7e-23', '94.0', '0.0', 'NW_020173731.1|9274958|9275015|+|False|False', '1000', '1057', '+', 'cm', 'no', '0.41', '-'],
+# ['(3)', '!', '8.3e-15', '62.1', '0.0', 'NW_020172457.1|4920040|4920099|+|False|False', '1000', '1059', '+', 'cm', 'no', '0.33', '-']
+# ]
+
+def perform_model_search(models, rna, candidate_region_fasta, output, cm_cutoff, cpu, phmm):
+
+    def parse_phmm(tblout):
+        phmm_results = []
+        with open(tblout) as fh:
+            for line in fh:
+                if line.startswith('#'):
+                    continue
+                data = line.strip().split()
+                # print(data)
+                info = data[0]
+                start, end = data[6:8]
+                strand, evalue, score = data[11:14]
+                phmm_results.append(['a', 'b', evalue, score, 'c', info, start, end, strand, 'd', 'e', 'f', 'g'])
+        return phmm_results
 
+    def parse_cm(res):
         cm_results = []
-        return_data = []
-        cms_command = (
-            'cmsearch --cpu {0} --noali -T {3} --incT {3} {1}/{2}.cm {4}'
-            .format(cpu, models, mirna_id, cut_off, heuristic_fa)
-        )
-        cms_call = sp.Popen(
-            cms_command, shell=True, stdout=sp.PIPE, stderr=sp.PIPE, encoding='utf8'
-        )
-        res, err = cms_call.communicate(mirna.pre)
-        # delete temporary file
-        if cleanup:
-            os.remove(heuristic_fa)
-        # read results
-        if err:
-            print(f'ERROR: {err}')
-            sys.exit()
         for line in res.split('\n'):
+            # print(line)
             if line.startswith('  ('):
                 if 'No hits detected that satisfy reporting thresholds' in line:
-                    exitstatus = 'CMsearch found not hits'
-                    return cm_results, exitstatus
+                    return []
                 else:
                     data = line.strip().split()
                     cm_results.append(data)
-        if not cm_results:
-            exitstatus = 'CMsearch found no hits'
-            return cm_results, exitstatus
-
-        for data in cm_results:
-            # print(data)
-            # parse CMsearch output of candidate regions to acutal genomic regions
-            blast_chrom = data[5].split('|')[0]
-            blast_start, blast_end = map(int, data[5].split('|')[1:3])
-            hit_at_start, hit_at_end = data[5].split('|')[4:6]
-            blast_strand = data[5].split('|')[3]
-            cm_start, cm_end = map(int, data[6:8])
-            # cm_start, cm_end = map(int, data[5:7])
-            cm_strand = data[8]
-            if cm_strand == '-':
-                # reverse hits should not be possible since blasthits were extracted
-                # as reverse complement if they were on the minus strand
-                print('Unexpected hit of CMsearch')
-                continue
-            if hit_at_start == 'True':
-                print('# cmsearch hit for {} at the beginning of a chromosome in the query species'.format(mirna_id))
-                hit_start = cm_start
-                hit_end = cm_end
-            elif hit_at_end == 'True':
-                print('# cmsearch hit for {} at the end of a chromosome in the query species'.format(
-                    mirna_id))
-                hit_start = blast_start + (cm_start - extraregion) - 1
-                hit_end = hit_start + (cm_end - cm_start) - 1
-            else:
-                hit_start = blast_start + (cm_start - extraregion) - 1
-                hit_end = hit_start + (cm_end - extraregion) - 1
-            # fill output variable
-            return_data.append([blast_chrom, hit_start, hit_end, blast_strand, float(data[3])])
-        if not return_data:
-            exitstatus = 'No hits left after parsing of CMsearch results'
-            return False, exitstatus
-
-        cm_results, exitstatus = cmsearch_parser(return_data, cut_off, len_cut, mirna_id)
-
-        if not cleanup:
-            heur_results = '{0}/cmsearch_{1}.out'.format(out, mirna_id)
-            with open(heur_results, 'w') as of:
-                of.write('# CMsearch hits in query genome\n')
-                for hit in cm_results:
-                    out_d = [str(entry) for entry in cm_results[hit]]
-                    of.write('\t'.join(out_d))
-                    of.write('\n')
+        return cm_results
+
+    ################################################################################
+    cut_off = rna.bit * cm_cutoff
 
-    # non heuristic mode (searches whole query genome with CM)
+    if phmm:
+        tblout = f'{output}/{rna.name}_phmm.out'
+        call = sp.Popen(
+            f'nhmmer --cpu {cpu} --tblout {tblout} -T {cut_off} --incT {cut_off} {models}/{rna.name}.phmm {candidate_region_fasta}',
+            shell=True, stdin=sp.PIPE, stdout=sp.PIPE, stderr=sp.PIPE, encoding='utf8'
+        )
+        res, err = call.communicate(rna.seq)
+        if err:
+            raise sp.SubprocessError(err)
+        results = parse_phmm(tblout)
+        os.remove(tblout)
     else:
-        cm_res_list = []
-        cms_output = '{0}/cmsearch_{1}.out'.format(out, mirna_id)
-        if not os.path.isfile(cms_output):
-            # heuristic_cms = '{0}/cmsearch_heuristic_{1}.out'.format(out, mirna_id)
-            print('# Running covariance model search for {}'.format(mirna_id))
-            cms_command = (
-                'cmsearch -T {5} --incT {5} --cpu {0} --noali '
-                '-o {1} {2}/{3}.cm {4}'
-                .format(cpu, cms_output, models, mirna_id, query, cut_off)
-            )
-            sp.run(cms_command, shell=True)
+        call = sp.Popen(
+            f'cmsearch --cpu {cpu} --noali -T {cut_off} --incT {cut_off} {models}/{rna.name}.cm {candidate_region_fasta}',
+            shell=True, stdout=sp.PIPE, stderr=sp.PIPE, encoding='utf8'
+        )
+        res, err = call.communicate(rna.seq)
+        if err:
+            raise sp.SubprocessError(err)
+        results = parse_cm(res)
+
+    return results
 
+
+def parse_cmsearch_for_heuristic(cm_results, extraregion=1000):
+    logger = logging.getLogger('ncortho')
+    logger.setLevel(level=logging.DEBUG)
+    return_data = []
+    for data in cm_results:
+        # parse CMsearch output of candidate regions to acutal genomic regions
+        blast_chrom = data[5].split('|')[0]
+        blast_start, blast_end = map(int, data[5].split('|')[1:3])
+        hit_at_start, hit_at_end = data[5].split('|')[4:6]
+        blast_strand = data[5].split('|')[3]
+        cm_start, cm_end = map(int, data[6:8])
+        # cm_start, cm_end = map(int, data[5:7])
+        cm_strand = data[8]
+        if cm_strand == '-':
+            # reverse hits should not be possible since blasthits were extracted
+            # as reverse complement if they were on the minus strand
+            logger.info('Unexpected hit of CMsearch')
+            continue
+        if hit_at_start == 'True':
+            # print(f'# cmsearch hit for {rna_id} at the beginning of a chromosome in the query species')
+            hit_start = cm_start
+            hit_end = cm_end
+        elif hit_at_end == 'True':
+            # print(f'# cmsearch hit for {rna_id} at the end of a chromosome in the query species')
+            hit_start = blast_start + (cm_start - extraregion) - 1
+            hit_end = hit_start + (cm_end - cm_start) - 1
         else:
-            print('# Found cm_search results at: {}. Using those'.format(cms_output))
-        data = []
-        with open(cms_output, 'r') as inf:
-            for line in inf:
-                if line.startswith('  ('):
-                    if 'No hits detected that satisfy reporting thresholds' in line:
-                        exitstatus = 'CMsearch found not hits'
-                        return cm_results, exitstatus
-                    data = line.strip().split()
-                    h_chrom = data[5]
-                    h_start = int(data[6])
-                    h_end = int(data[7])
-                    h_score = float(data[3])
-                    h_strand = data[8]
-                    cm_res_list.append([h_chrom, h_start, h_end, h_strand, h_score])
-        if not data:
-            exitstatus = 'cmSearch did not find anything'
-            return cm_results, exitstatus
-
-        cm_results, exitstatus = cmsearch_parser(cm_res_list, cut_off, len_cut, mirna_id)
-    return cm_results, exitstatus
-
-
-# cmsearch_parser: Parse the output of cmsearch while eliminating
-#                  duplicates and filtering entries according to the
-#                  defined cutoff.
-def cmsearch_parser(cms, cmc, lc, mirid):
+            hit_start = blast_start + (cm_start - extraregion) - 1
+            hit_end = hit_start + (cm_end - extraregion) - 1
+        # fill output variable
+        return_data.append([blast_chrom, hit_start, hit_end, blast_strand, float(data[3])])
+    return return_data
+
+
+def cmsearch_parser(cms, cmc, lc, rna):
     """
     Parse the output of cmsearch while eliminating duplicates and filtering
     entries according to the defined cutoff.
 
     Parameters
     ----------
     cms     :   List with CMsearch hits [chrom, start, end, strand, score]
     cmc     :   Cutoff to decide which candidate hits should be included for the reverse BLAST search
     lc      :   Length cutoff
-    mirid   :   miRNA ID
+    rna     :   rna class
 
     Returns
     -------
     hits_dict : Dictionary containing hits of the cmsearch
 
     """
     # Output
     hits_dict = {}
     # Required for finding duplicates, stores hits per chromosome
     chromo_dict = {}
-    cut_off = cmc
 
     for candidate_nr, hit in enumerate(cms, 1):
         h_chrom, h_start, h_end, h_strand, h_score = hit
         # blastparser expects the start to be the smaller number, will extract reverse complement if on - strand
         if h_start > h_end:
-            start_tmp = h_start
-            h_start = h_end
-            h_end = start_tmp
-        data = (
-            '{0}_c{1}'.format(mirid, candidate_nr),
-            h_chrom, h_start, h_end, h_strand, h_score
-        )
-        hits_dict[data[0]] = data
+            h_start, h_end = h_end, h_start
+        length = h_end - h_start
+
+        if length <= length * lc:
+            continue
+        if h_score <= rna.bit * cmc:
+            continue
+
+        candidate = f'{rna.name}_c{candidate_nr}'
+        data = candidate, h_chrom, h_start, h_end, h_strand, h_score
+        hits_dict[candidate] = data
 
         # Store the hits that satisfy the bit score cutoff to filter
         # duplicates.
-        try:
-            chromo_dict[data[1]].append(data)
-        except:
-            chromo_dict[data[1]] = [data]
+        if h_chrom in chromo_dict:
+            chromo_dict[h_chrom] = []
+        chromo_dict[h_chrom] = [data]
+    # print(hits_dict)
 
     # Loop over the candidate hits to eliminate duplicates.
     for chromo in chromo_dict:
         nrhits = len(chromo_dict[chromo])
         if nrhits > 1:
             for hitnr in range(nrhits):
                 start = int(chromo_dict[chromo][hitnr][2])
@@ -315,20 +238,78 @@
                         if (
                                 start in range(cstart, cstop +1)
                                 or stop in range(cstart, cstop +1)
                                 or cstart in range(start, stop +1)
                                 or cstop in range(start, stop +1)
                         ):
                             if score > cscore:
-                                try:
-                                    del hits_dict[chromo_dict[chromo]
-                                    [chitnr][0]]
-                                except:
-                                    pass
+                                del hits_dict[chromo_dict[chromo][chitnr][0]]
+
                             else:
-                                try:
-                                    del hits_dict[chromo_dict[chromo]
-                                    [hitnr][0]]
-                                except:
-                                    pass
-    exitstatus = 'Sucess'
-    return hits_dict, exitstatus
+                                del hits_dict[chromo_dict[chromo][hitnr][0]]
+
+    return hits_dict
+
+
+def model_search(rna, cm_cutoff, cpu, msl, models, query, blastdb, out, cleanup, heuristic_col, phmm):
+    """
+    Parameters
+    ----------
+    rna       :   rna object
+    cm_cutoff   :   Minimum bit score of the CMsearch hit relative to the
+                    bit score that results from searching in the reference genome with the same model
+    cpu         :   Number of cores to use
+    msl         :   Minimum length of CMsearch hit relative to the reference pre-rna length
+    models      :   Path to the directory that contains the CMs
+    query       :   Path to the query genome
+    blastdb     :   Optional Path to a BLASTdb of the query genome
+    out         :   Path to the output directory
+    cleanup     :   Delete intermediate files True/False
+    heuristic   :   Should heuristic mode be used and if yes, set parameters (True/False, evalue, minlength)
+
+    Returns
+    -------
+    cm_results : Dictionary containing hits of the cmsearch
+
+    """
+    # print(os.path.isfile(f'{models}/{rna.name}.phmm'))
+    if (
+            not phmm and not os.path.isfile(f'{models}/{rna.name}.cm') or
+            phmm and not os.path.isfile(f'{models}/{rna.name}.phmm')
+    ):
+        return False, 'No model found'
+    heuristic, heuristic_evalue, heuristic_length, sensitive_heuristic = heuristic_col
+    if heuristic:
+        candidate_region_fasta = heuristic_search(blastdb, rna, query, heuristic_col, cpu, out)
+
+        if not candidate_region_fasta and sensitive_heuristic:
+            # No candidate regions above length cutoff found with BLASTn. Trying again without heuristic.
+            cm_results = perform_model_search(models, rna, query, out, cm_cutoff, cpu, phmm)
+        elif not candidate_region_fasta:
+            return False, 'No candidate region found with BLASTn'
+        else:
+            cm_results = perform_model_search(models, rna, candidate_region_fasta, out, cm_cutoff, cpu, phmm)
+            cm_results = parse_cmsearch_for_heuristic(cm_results)
+
+        if cleanup:
+            os.remove(candidate_region_fasta)
+    else:
+        cm_results = perform_model_search(models, rna, query, out, cm_cutoff, cpu, phmm)
+
+    if not cm_results:
+        return False, 'No CMsearch results in candidate regions or query genome'
+
+    parsed_cm_results = cmsearch_parser(cm_results, cm_cutoff, msl, rna)
+    if not parsed_cm_results:
+        return False, 'No CMsearch results above threshold'
+    else:
+        return parsed_cm_results, 'Sucess'
+
+
+
+
+
+
+
+
+
+
```

### Comparing `ncOrtho-0.3.9/ncOrtho/coreset/core_reblast.py` & `ncOrtho-0.4.0/ncOrtho/coreset/core_reblast.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,33 +7,42 @@
 
 
 def vprint(s, verbose):
     if verbose:
         print(s, flush=True)
 
 
-def make_alignment(out, mirna, cpu, core):
+def make_alignment(out, mirna, cpu, core, rcoffee):
     alignment = '{}/{}.aln'.format(out, mirna)
     stockholm = '{}/{}.sto'.format(out, mirna)
 
     # Call T-Coffee for the sequence alignment.
     # print('Building T-Coffee alignment.')
-    tc_cmd_1 = (
-        f't_coffee -quiet -multi_core={cpu} -special_mode=rcoffee -in {core} '
-        f'-output=clustalw_aln -outfile={alignment}'
-    )
-    sp.call(tc_cmd_1, shell=True)
+    if rcoffee == 'yes':
+        tc_cmd_1 = (
+            f't_coffee -quiet -multi_core={cpu} -mode=rcoffee -in {core} -output=clustalw_aln -outfile={alignment}'
+        )
+    else:
+        tc_cmd_1 = (
+            f't_coffee -quiet -multi_core={cpu} -in {core} -output=clustalw_aln -outfile={alignment}'
+        )
+    sp.run(tc_cmd_1, shell=True, capture_output=True)
 
     # Extend the sequence-based alignment by structural information.
     # Create Stockholm alignment.
     # print('Adding secondary structure to Stockholm format.')
-    tc_cmd_2 = (
-        f't_coffee -other_pg seq_reformat -in {alignment} -action +add_alifold -output stockholm_aln -out {stockholm}'
-    )
-    sp.call(tc_cmd_2, shell=True)
+    if rcoffee == 'yes':
+        tc_cmd_2 = (
+            f't_coffee -other_pg seq_reformat -in {alignment} -action +add_alifold -output stockholm_aln -out {stockholm}'
+        )
+    else:
+        tc_cmd_2 = (
+            f't_coffee -other_pg seq_reformat -in {alignment} -output stockholm_aln -out {stockholm}'
+        )
+    sp.run(tc_cmd_2, shell=True, capture_output=True)
     return stockholm
 
 
 def maximum_blast_bitscore(mirna, seq, blastdb, c, dust):
     # The miRNA precursors can show a low level of complexity, hence it might be
     # required to deactivate the dust filter for the BLAST search.
     bit_check = (
@@ -41,25 +50,26 @@
     )
     # print('# Determining reference bit score..')
     ref_bit_cmd = sp.Popen(
         bit_check, shell=True, stdin=sp.PIPE, stdout=sp.PIPE, stderr=sp.STDOUT, encoding='utf8'
     )
     ref_results, err = ref_bit_cmd.communicate(seq)
     if not ref_results:
-        raise ValueError(f'WARNING: Reference sequence of {mirna} not found in reference Genome. '
-              'Consider turning the dust filter off')
+        print(f'WARNING: Reference sequence of {mirna} not found in reference Genome. Setting maximum bitscore to 0', flush=True)
+        return 0.0
     try:
         ref_bit_score = float(ref_results.split('\n')[0].split('\t')[0])
     except ValueError:  # BLASTn errors are in output not in error
-        raise ValueError(ref_results)
+        print(f'WARNING: Reference sequence of {mirna} not found in reference Genome. Setting maximum bitscore to 0', flush=True)
+        return 0.0
     return ref_bit_score
 
 
 # Perform reciprocal BLAST search and construct Stockholm alignment
-def blastsearch(mirna, r_path, o_path, c, dust, v):
+def blastsearch(mirna, r_path, o_path, c, dust, v, coffee):
     """
 
     Parameters
     ----------
     m_path  :   Path to file with miRNA information
     r_path  :   Path to reference genome.
     o_path  :   Output Name
@@ -78,20 +88,20 @@
 
     miroutdir = f'{o_path}/{mirid}'
     if not os.path.isdir(miroutdir):
         os.mkdir(miroutdir)
     synteny_regs = f'{miroutdir}/synteny_regions_{mirid}.fa'  # this fasta file is created by the the main() script
     os.chdir(miroutdir)
 
-    print(f'# {mirid}')
+    print(f'# {mirid}', flush=True)
     if not os.path.isfile(synteny_regs):
         print(f'Warning: No synteny regions found for {mirid}. Training with reference miRNA only.', flush=True)
         with open(synteny_regs, 'w') as fastah:
             fastah.write(f'>{mirid}\n{preseq}\n')
-        stock = make_alignment(miroutdir, mirid, c, synteny_regs)
+        stock = make_alignment(miroutdir, mirid, c, synteny_regs, coffee)
         return stock
 
     # check if blastdb of reference genome exists
     fname = '.'.join(r_path.split("/")[-1].split('.')[0:-1])
     ref_blastdb = f'{o_path}/refBLASTdb/{fname}'
     if not check_blastdb(ref_blastdb):
         make_blastndb(r_path, ref_blastdb)
@@ -157,9 +167,9 @@
     with open(corefile, 'w') as outfile:
         outfile.write(f'>reference\n{preseq}\n')
         if outputcol:
             for synteny_region, sequence in outputcol.items():
                 outfile.write(f'>{synteny_region}\n{sequence}\n')
         else:
             print(f'Warning: No core orthologs found for {mirid}. Training with reference miRNA only.', flush=True)
-    stock = make_alignment(miroutdir, mirid, c, corefile)
+    stock = make_alignment(miroutdir, mirid, c, corefile, coffee)
     return stock
```

### Comparing `ncOrtho-0.3.9/ncOrtho/coreset/coreset.py` & `ncOrtho-0.4.0/ncOrtho/coreset/coreset.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,41 +26,33 @@
 # reference taxon: genome, blastdb, gtf file with gene coordinates
 # core set taxa: genome, gtf file, pairwise orthologs
 
 import argparse
 import multiprocessing as mp
 import os
 import sys
-import shutil
+from pyfiglet import Figlet
+from importlib.metadata import version
 
 try:
-    from createcm import CmConstructor
+    from createcm import create_cm, create_phmm
     from core_reblast import blastsearch
     from locate_position import categorize_mirna_position
     from synteny import analyze_synteny
     import coreset_utils as cu
 except ModuleNotFoundError:
     from ncOrtho.coreset.createcm import CmConstructor
     from ncOrtho.coreset.core_reblast import blastsearch
     from ncOrtho.coreset.synteny import analyze_synteny
     from ncOrtho.coreset.locate_position import categorize_mirna_position
     import ncOrtho.coreset.coreset_utils as cu
 
 
 ###############################################################################
 def main():
-    # Print header
-    print('\n' + '#' * 43, flush=True)
-    print('###' + ' ' * 37 + '###', flush=True)
-    print('###   ncOrtho - core set construction   ###', flush=True)
-    print('###' + ' ' * 37 + '###', flush=True)
-    print('#' * 43 + '\n', flush=True)
-
-    # Parse command-line arguments
-    # Define global variables
     parser = argparse.ArgumentParser(
         description=(
             'Build Covariance models of reference miRNAs from core set of orthologs.'
         )
     )
     parser._action_groups.pop()
     required = parser.add_argument_group('Required Arguments')
@@ -100,15 +92,29 @@
         const='no', default='no'
     )
     optional.add_argument(
         '--create_model', metavar='yes/no', type=str,
         help='set to "no" if you only want to create the alignment. (Default: yes)', nargs='?',
         const='yes', default='yes'
     )
-    #
+    optional.add_argument(
+        '--phmm', metavar='yes/no', type=str,
+        help='set to "yes" if you want to create a pHMM instead of a CM (Default: no)', nargs='?',
+        const='yes', default='yes'
+    )
+    optional.add_argument(
+        '--rcoffee', metavar='yes/no', type=str,
+        help='set to "no" to use default "t_coffee" instead of "r_coffee" (Default: yes)', nargs='?',
+        const='yes', default='yes'
+    )
+    optional.add_argument(
+        '--redo', metavar='yes/no', type=str,
+        help='set to "no" to reuse models found at output destination (Default: yes)', nargs='?',
+        const='yes', default='yes'
+    )
     optional.add_argument(
         '--idtype', metavar='str', type=str,
         help='Choose the ID in the reference gff file that is '
              'compared to the IDs in the pairwise orthologs file (default:GeneID) '
              'Options: ID, Name, GeneID, gene_id, CDS',
         nargs='?', const='ID=', default='ID'
     )
@@ -120,14 +126,19 @@
     )
     optional.add_argument(
         '--verbose', metavar='yes/no', type=str,
         help='Print additional information (Default: no)',
         nargs='?', const='no', default='no'
     )
 
+    # print header
+    custom_fig = Figlet(font='stop')
+    print(custom_fig.renderText('ncOrtho')[:-3], flush=True)
+    v = version('ncOrtho')
+    print(f'Version: {v}\n', flush=True)
     ###############################################################################
 
     # Show help when no arguments are added.
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
     else:
@@ -137,15 +148,17 @@
     available_cpu = mp.cpu_count()
     if args.threads > available_cpu:
         raise ValueError('The provided number of CPU cores is higher than the number available on this system')
     else:
         cpu = args.threads
 
     # parse mandatory arguments
-    output = args.output
+    output = os.path.realpath(args.output)
+    if not os.path.isdir(output):
+        os.mkdir(output)
 
     # parse optional arguments
     # mgi = args.mgi
     dust = args.dust
     create_model = args.create_model
     if args.verbose == 'yes':
         verbose = True
@@ -165,15 +178,15 @@
     ###############################################################################
     neighbor_dict = {}
     mirna_dict = {}
 
     # create directory for intermediate files
     tmpout = f'{output}/tmp'
     if not os.path.isdir(tmpout):
-        os.makedirs(tmpout)
+        os.mkdir(tmpout)
 
     print('# Reading pairwise orthologs', flush=True)
     if args.idtype == 'CDS':
         ortho_dict = cu.pairwise_orthologs_from_cds(core_dict, ref_paths['annotation'])
     else:
         ortho_dict = cu.read_pairwise_orthologs(core_dict)
 
@@ -187,51 +200,55 @@
     mirna_positions = {}
     for mirna in mirnas:
         mirid, chromo, start, end, strand = cu.mirna_position(mirna)
         syntype, core_orthos = categorize_mirna_position(
             mirid, chromo, start, end, strand, ref_dict, ortho_dict, add_pos_orthos, verbose
         )
         if not syntype:
-            print(f'Warning: Could not localize {mirid}')
+            print(f'Warning: Could not localize {mirid}', flush=True)
             continue
         mirna_positions[mirid] = (syntype, core_orthos)
 
-    print('### Identifying syntenic regions in core species', flush=True)
+    print('\n### Identifying syntenic regions in core species', flush=True)
     syntenyregion_per_mirna = analyze_synteny(core_dict, mirna_positions, tmpout, args.idtype, args.mgi, verbose)
 
     if not syntenyregion_per_mirna:
         raise ValueError('No regions of conserved synteny found in any core species')
 
     for mirid, fastalist in syntenyregion_per_mirna.items():
         if not fastalist:
             print(f'Warning: No syntenic region found in any core species for {mirid}. '
-                  f'Make sure that the IDs in the annotation file match the ones in the orthologs file')
+                  f'Make sure that the IDs in the annotation file match the ones in the orthologs file', flush=True)
             continue
         miroutdir = f'{tmpout}/{mirid}'
         if not os.path.isdir(miroutdir):
             os.mkdir(miroutdir)
         with open(f'{miroutdir}/synteny_regions_{mirid}.fa', 'w') as of:
             for line in fastalist:
                 of.write(line)
 
     #################################################################################################
-    print('\n### Starting Ortholog search')
+    print('\n### Starting Ortholog search', flush=True)
     for mirna in mirnas:
         mirid = mirna[0]
-        sto_path = blastsearch(mirna, ref_paths['genome'], tmpout, cpu, dust, verbose)
-        if create_model == 'yes' and sto_path is not None:
+        sto_path = blastsearch(mirna, ref_paths['genome'], tmpout, cpu, dust, verbose, args.rcoffee)
+        if create_model == 'no' or sto_path is None:
+            continue
+        if args.phmm == 'no':
             print(f'# Starting to construct covariance model for {mirid}', flush=True)
             model_out = f'{output}/{mirid}.cm'
-            if not os.path.isfile(model_out):
-                # Initiate covariance model construction and calibration.
-                cmc = CmConstructor(sto_path, output, mirid, cpu)
-                # Construct the model.
-                cmc.construct()
-                # Calibrate the model.
-                cmc.calibrate()
-            else:
+            if args.redo == 'no' and not os.path.isfile(model_out):
                 print(f'Model of {mirid} already found at {output}. Nothing done..', flush=True)
-    print('\n### Construction of core set finished')
+                continue
+            create_cm(sto_path, output, mirid, cpu)
+
+        elif args.phmm == 'yes':
+            print(f'# Starting to construct pHMM for {mirid}', flush=True)
+            create_phmm(sto_path, output, mirid, cpu)
+        else:
+            raise ValueError(f'Unknown value "{args.phmm}" for --phmm')
+
+    print('\n### Construction of core set finished', flush=True)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ncOrtho-0.3.9/ncOrtho/coreset/coreset_utils.py` & `ncOrtho-0.4.0/ncOrtho/coreset/coreset_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,23 +56,25 @@
 
     """
     chr_dict = {}
     chromo = ''
     # with open(inpath) as infile, open(outpath, 'wb') as outfile:
     with open(gff) as infile:
         for line in infile:
-            if line.startswith('#') or not 'gene_biotype=protein_coding' in line:
+            if line.startswith('#'):
+                continue
+            if 'gene_biotype=protein_coding' not in line:
                 continue
             linedata = line.strip().split('\t')
             if linedata[2] != 'gene':
                 continue
 
             if id_type == 'GeneID':
                 geneid = re.split('[;,]', linedata[-1].split(f'{id_type}:')[1])[0]
-            elif id_type in ['ID', 'Name', 'gene_id', 'CDS']:
+            elif id_type in ['ID', 'Name', 'CDS']:
                 geneid = linedata[-1].split(f'{id_type}=')[1].split(';')[0]
                 if id_type in ['ID', 'CDS']:
                     geneid = '-'.join(geneid.split('-')[1:])
             else:
                 raise ValueError('Unknown identifier type "{}"'.format(id_type))
 
             contig = linedata[0]
```

### Comparing `ncOrtho-0.3.9/ncOrtho/coreset/createcm.py` & `ncOrtho-0.4.0/ncOrtho/coreset/createcm.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,85 +17,101 @@
         self.alignment = alignment
         self.outpath = outpath
         self.name = name
         self.cpu = cpu
         self.model = '{0}/{1}.cm'.format(outpath, name)
     
     def construct(self):
-        print('# Constructing covariance model for {}.'.format(self.name))
+        # print('# Constructing covariance model for {}.'.format(self.name), '')
         construct_command = (
-            'cmbuild -n {0} {1}/{0}.cm {2}'
+            'cmbuild -F -n {0} {1}/{0}.cm {2}'
             .format(self.name, self.outpath, self.alignment)
         )
-        sp.call(construct_command, shell=True)
-        print('# Finished covariance model construction.')
+        sp.run(construct_command, shell=True, capture_output=True)
+        # print('# Finished covariance model construction.')
     
     def calibrate(self):
-        print('# Calibrating covariance model for {}.'.format(self.name))
+        # print('# Calibrating covariance model for {}.'.format(self.name))
         calibrate_command = (
             'cmcalibrate --cpu {0} {1}'.format(self.cpu, self.model)
         )
-        sp.call(calibrate_command, shell=True)
-        print('# Finished covariance model calibration.')
+        sp.run(calibrate_command, shell=True)
+        # print('# Finished covariance model calibration.')
 
 
-def main():
-
-    # Parse command-line arguments.
-    parser = argparse.ArgumentParser(
-        prog='python createcm.py', description='covariance model construction'
-    )
-    # "cpu", use maximum number of available CPUs unless specified otherwise.
-    parser.add_argument(
-        '-c', '--cpu', metavar='int', type=int,
-        help='number of CPU cores to use', nargs='?',
-        const=mp.cpu_count(), default=mp.cpu_count()
-    )
-    # Path to the desired output folder.
-    parser.add_argument(
-        '-o', '--output', metavar='<path>', type=str,
-        help='path to the output folder'
-    )
-    # Path to the input alignment
-    parser.add_argument(
-        '-a', '--alignment', metavar='<.sto>', type=str,
-        help='path to input alignment'
-    )
-
-    # Show help when no arguments are added.
-    if len(sys.argv) == 1:
-        parser.print_help()
-        sys.exit(1)
-    else:
-        args = parser.parse_args()
-    
-    # Check if computer provides the desired number of cores.
-    available_cpu = mp.cpu_count()
-    if args.cpu > available_cpu:
-        raise ValueError('The provided number of CPU cores is higher than the number available on this system')
-    else:
-        cpu = args.cpu
-
-    # Check if alignment file exists.
-    if not os.path.isfile(args.alignment):
-        raise ValueError('Invalid path to alignment file')
-    else:
-        alignment = args.alignment
-
-    output = args.output
-    name = alignment.split('/')[-1].split('.')[0]
-
-    # Check if the output folder exists.
-    if not os.path.isdir(output):
-        mkdir_cmd = 'mkdir -p {}'.format(output)
-        sp.call(mkdir_cmd, shell=True)
-
+def create_cm(alignment, outpath, name, cpu):
     # Initiate covariance model construction and calibration.
-    cmc = CmConstructor(alignment, output, name, cpu)
+    cmc = CmConstructor(alignment, outpath, name, cpu)
     # Construct the model.
     cmc.construct()
     # Calibrate the model.
     cmc.calibrate()
 
 
-if __name__ == '__main__':
-    main()
+def create_phmm(alignment, outpath, name, cpu):
+    model = f'{outpath}/{name}.phmm'
+    cmd = f'hmmbuild -n {name} --informat stockholm --dna {model} {alignment}'
+    res = sp.run(cmd, shell=True, capture_output=True)
+    res.check_returncode()
+
+
+# def main():
+#
+#     # Parse command-line arguments.
+#     parser = argparse.ArgumentParser(
+#         prog='python createcm.py', description='covariance model construction'
+#     )
+#     # "cpu", use maximum number of available CPUs unless specified otherwise.
+#     parser.add_argument(
+#         '-c', '--cpu', metavar='int', type=int,
+#         help='number of CPU cores to use', nargs='?',
+#         const=mp.cpu_count(), default=mp.cpu_count()
+#     )
+#     # Path to the desired output folder.
+#     parser.add_argument(
+#         '-o', '--output', metavar='<path>', type=str,
+#         help='path to the output folder'
+#     )
+#     # Path to the input alignment
+#     parser.add_argument(
+#         '-a', '--alignment', metavar='<.sto>', type=str,
+#         help='path to input alignment'
+#     )
+#
+#     # Show help when no arguments are added.
+#     if len(sys.argv) == 1:
+#         parser.print_help()
+#         sys.exit(1)
+#     else:
+#         args = parser.parse_args()
+#
+#     # Check if computer provides the desired number of cores.
+#     available_cpu = mp.cpu_count()
+#     if args.cpu > available_cpu:
+#         raise ValueError('The provided number of CPU cores is higher than the number available on this system')
+#     else:
+#         cpu = args.cpu
+#
+#     # Check if alignment file exists.
+#     if not os.path.isfile(args.alignment):
+#         raise ValueError('Invalid path to alignment file')
+#     else:
+#         alignment = args.alignment
+#
+#     output = args.output
+#     name = alignment.split('/')[-1].split('.')[0]
+#
+#     # Check if the output folder exists.
+#     if not os.path.isdir(output):
+#         mkdir_cmd = 'mkdir -p {}'.format(output)
+#         sp.call(mkdir_cmd, shell=True)
+#
+#     # Initiate covariance model construction and calibration.
+#     cmc = CmConstructor(alignment, output, name, cpu)
+#     # Construct the model.
+#     cmc.construct()
+#     # Calibrate the model.
+#     cmc.calibrate()
+#
+#
+# if __name__ == '__main__':
+#     main()
```

### Comparing `ncOrtho-0.3.9/ncOrtho/coreset/example_parameters.yaml` & `ncOrtho-0.4.0/ncOrtho/coreset/example_parameters.yaml`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.9/ncOrtho/coreset/locate_position.py` & `ncOrtho-0.4.0/ncOrtho/coreset/locate_position.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,69 +12,75 @@
     # case 1): there is no protein-coding gene on the same contig as the miRNA,
     # so there can be no neighbors (should only occur in highly fragmented
     # assemblies)
     if chrom not in reference.keys():
         print(
             f'WARNING: No protein-coding genes found on contig "{chrom}". '
             'Make sure that the contig identifiers of the miRNA input file '
-            'match the ones in the reference annotation file'
+            'match the ones in the reference annotation file', flush=True
         )
         return True
     # case 2): miRNA is located left of the first gene and hence has no left
     # neighbor, the first gene is therefore by default the right neighbor
 
     elif end < firstgene_start:
         print(
             f'There is no left neighbor of {mirna}, since it is located at the start of contig {chrom}\n'
-            f'{firstgene_info[0]} is the right neighbor of {mirna}'
+            f'{firstgene_info[0]} is the right neighbor of {mirna}', flush=True
         )
         return True
     # case 3): miRNA is located right to the last gene, so the last gene is the
     # left neighbor and there cannot be a right neighbor
     elif start > lastgene_end:
         print(
             f'There is no right neighbor of {mirna}, since it is located at the end of contig {chrom}\n'
-            f'{lastgene_info[0]} is the left neighbor of {mirna}')
+            f'{lastgene_info[0]} is the left neighbor of {mirna}', flush=True)
         return True
     else:
         return False
 
 
-def ortho_search(r_gene, core_dict, v):
-    """
-    Try to find the ortholog for a given reference gene in a core set species
-
-    Parameters
-    ----------
-    r_gene:     Gene of Reference Species
-    ortho_dict: {'corespecies': {r_gene: [ortho1], ...}, ...}
-
-    Returns:    {'corespecies': [coreortho1], ...}
-    -------
-
-    """
-    coreorthologs_per_species = {}
-    for core_taxon, orthodict in core_dict.items():
-        if r_gene in orthodict:
-            core_orthologs = orthodict[r_gene]
-            coreorthologs_per_species[core_taxon] = core_orthologs
-            vprint(f'{" ".join(core_orthologs)} identified as ortholog(s) to {r_gene} in {core_taxon}', v)
-        else:
-            vprint(f'No ortholog found for {r_gene} in {core_taxon}', v)
-    return coreorthologs_per_species
+# def ortho_search(r_gene, core_dict, v):
+#     """
+#     Try to find the ortholog for a given reference gene in a core set species
+#
+#     Parameters
+#     ----------
+#     r_gene:     Gene of Reference Species
+#     ortho_dict: {'corespecies': {r_gene: [ortho1], ...}, ...}
+#
+#     Returns:    {'corespecies': [coreortho1], ...}
+#     -------
+#
+#     """
+#     coreorthologs_per_species = {}
+#     for core_taxon, orthodict in core_dict.items():
+#         if r_gene in orthodict:
+#             core_orthologs = orthodict[r_gene]
+#             coreorthologs_per_species[core_taxon] = core_orthologs
+#             vprint(f'{" ".join(core_orthologs)} identified as ortholog(s) to {r_gene} in {core_taxon}', v)
+#         else:
+#             vprint(f'No ortholog found for {r_gene} in {core_taxon}', v)
+#     return coreorthologs_per_species
 
 
 def neighbor_search(leftgene, rightgene, core_dict, gene_position, chromdict, no_next_orthos, v):
+
     def find_ortho(genename, position, chromd, orthologs, next_orthos, typ, v):
         if genename in orthologs:
             core_orthologs = orthologs[genename]
             vprint(f'{" ".join(core_orthologs)} identified as ortholog(s) to {genename} in {core_taxon}', v)
             return core_orthologs
         else:
             for index in range(1, next_orthos):
+                if position - index < 1:
+                    continue
+                if position + index > len(chromd):
+                    continue
+
                 if typ == 'left':
                     nextgeneinfo = chromd[position - index]
                 else:
                     nextgeneinfo = chromd[position + index]
                 nextgene = nextgeneinfo[0]
                 if nextgene in orthologs:
                     core_orthologs = orthologs[nextgene]
@@ -109,15 +115,15 @@
     -------
 
     """
     syntenytype = None
     solved = False
     core_orthologs = []
     if no_synteny_possible(mirna, mirna_chrom, mirna_start, mirna_end, reference):
-        return solved
+        return solved, syntenytype
 
     # case 4): miRNA is located either between two genes or overlapping with (an
     # intron of) a gene, either on the same or the opposite strand
     ###############################################################################
     for position, geneinfo in reference[mirna_chrom].items():
         gene, gene_start, gene_end, gene_strand = geneinfo
         if mirna_start >= gene_start and mirna_end <= gene_end:
@@ -127,24 +133,30 @@
                 solved = True
                 vprint(f'{mirna} is located inside the gene {gene}', v)
             # case 4.2): miRNA opposite of gene
             else:
                 syntenytype = 'opposite'
                 solved = True
                 vprint(f'{mirna} is located opposite of the gene {gene}', v)
-            core_orthologs = ortho_search(gene, all_orthologs, v)
+            # core_orthologs = ortho_search(gene, all_orthologs, v)
+            core_orthologs = neighbor_search(
+                gene, gene, all_orthologs, position, reference[mirna_chrom], no_add_orthos, v
+            )
 
         # case 4.3): miRNA between genes
         else:
             if position == len(reference[mirna_chrom]):
                 continue
             rightneighborinfo = reference[mirna_chrom][position + 1]
             rightneighbor = rightneighborinfo[0]
             rn_start = rightneighborinfo[1]
-            if gene_end < mirna_start and rn_start > mirna_end:
+            rn_end = rightneighborinfo[2]
+
+            # if gene_end < mirna_start and rn_start > mirna_end:
+            if gene_start <= mirna_start and rn_end >= mirna_end:
                 syntenytype = 'in-between'
                 solved = True
                 vprint(f'{gene} is the left neighbor of {mirna}, {rightneighbor} is the right neighbor', v)
                 core_orthologs = neighbor_search(
                     gene, rightneighbor, all_orthologs, position, reference[mirna_chrom], no_add_orthos, v
                 )
     if solved:
```

### Comparing `ncOrtho-0.3.9/ncOrtho/coreset/synteny.py` & `ncOrtho-0.4.0/ncOrtho/coreset/synteny.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,28 @@
     except FileExistsError:
         pass
     g = pyfaidx.Fasta(slink)
     return g
 
 
 def synteny_check(left: list, right: list, orthodict: dict, mgi: int, v):
+    """
+    TODO: Will extract all syntenic regions using all available anchors. Should only return smallest region per co-ortholog
+    Parameters
+    ----------
+    left
+    right
+    orthodict
+    mgi
+    v
+
+    Returns
+    -------
+
+    """
     seqcol = []
     for left_ortho in left:
         if left_ortho not in orthodict:
             continue
         left_chromosome, left_position = orthodict[left_ortho]
         for right_ortho in right:
             if right_ortho not in orthodict:
@@ -79,16 +93,20 @@
             if mirid not in synteny_region_collector:
                 synteny_region_collector[mirid] = []
             style, core_ortholog_collection_all_taxa = positiontuple
             if taxon not in core_ortholog_collection_all_taxa:
                 vprint(f'No core orthologs found for {mirid} in {taxon}', v)
                 continue
             core_ortholog_collection = core_ortholog_collection_all_taxa[taxon]
-            if style in ['inside', 'opposite']:
-                for ortholog in core_ortholog_collection:
+
+            leftorthos, rightorthos = core_ortholog_collection
+            #print(style)
+            if leftorthos == rightorthos:  # for genes inside a gene for which an ortholog was found
+                #if style in ['inside', 'opposite']:
+                for ortholog in leftorthos:
                     if ortholog in core_anno_dict:
                         ortholog_chromosome, ortholog_position = core_anno_dict[ortholog]
                         orthostart, orthoend, orthostrand = core_anno_dict[ortholog_chromosome][ortholog_position][1:]
                         seq = genome[ortholog_chromosome][orthostart-1:orthoend].seq
 
                         synteny_fulfilled = True
                         synteny_region_collector[mirid].append(f'>{taxon}_0\n')
```

### Comparing `ncOrtho-0.3.9/ncOrtho/genparser.py` & `ncOrtho-0.4.0/ncOrtho/genparser.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.9/ncOrtho/ncortho.py` & `ncOrtho-0.4.0/ncOrtho/ncortho.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,158 +17,40 @@
 """
 
 
 # Modules import
 import argparse
 import multiprocessing as mp
 import os
-import subprocess as sp
 import sys
+from time import time
+from tqdm import tqdm
+import logging
+from pyfiglet import Figlet
+from importlib.metadata import version
 
 # Internal ncOrtho modules
 try:
-    from ncOrtho.blastparser import BlastParser
-    from ncOrtho.blastparser import ReBlastParser
-    from ncOrtho.genparser import GenomeParser
-    from ncOrtho.cmsearch import cmsearcher
-    from ncOrtho.utils import check_blastdb
-    from ncOrtho.utils import make_blastndb
-    from ncOrtho.utils import find_refbit
-except ModuleNotFoundError:
-    from blastparser import BlastParser
     from blastparser import ReBlastParser
     from genparser import GenomeParser
-    from cmsearch import cmsearcher
-    from utils import check_blastdb
-    from utils import make_blastndb
-    from utils import find_refbit
-
-###############################################################################
-
-
-# Central class of microRNA objects
-class Mirna(object):
-    def __init__(self, name, chromosome, start, end, strand, pre, mature, bit):
-        # miRNA identifier
-        self.name = name
-        # chromosome that the miRNA is located on
-        if chromosome.startswith('chr'):
-            self.chromosome = chromosome.split('chr')[1]
-        else:
-            self.chromosome = chromosome
-        # start position of the pre-miRNA
-        self.start = int(start)
-        # end position of the pre-miRNA
-        self.end = int(end)
-        # sense (+) or anti-sense (-) strand
-        self.strand = strand
-        # nucleotide sequence of the pre-miRNA
-        self.pre = pre.replace('U', 'T')
-        # nucleotide sequence of the mature miRNA
-        self.mature = mature.replace('U', 'T')
-        # reference bit score that miRNA receives by its own
-        # covariance model
-        self.bit = bit
-
-
-def mirna_maker(mirpath, cmpath, output, msl):
-    """
-    Parses the miRNA data input file and returns a dictionary of Mirna objects.
-
-    Parameters
-    ----------
-    mirpath : STR
-        Path to file with microRNA data.
-    cmpath : STR
-        Path to covariance models.
-    output : STR
-        Path for writing temporary files.
-    msl : FLOAT
-        Length filter.
-
-    Returns
-    -------
-    mmdict : DICT
-        Dictionary with Mirna objects.
-
-    """
-    
-    mmdict = {} # will be the return object
-    
-    with open(mirpath) as mirna_file:
-        mirna_data = [
-            line.strip().split() for line in mirna_file
-            if not line.startswith('#')
-        ]
-
-    print('# Calculating reference bit scores')
-    for mirna in mirna_data:
-        mirid = mirna[0]
-        seq = mirna[5]
-        query = '{0}/{1}.fa'.format(output, mirid)
-        model = '{0}/{1}.cm'.format(cmpath, mirid)
-        # Check if the covariance model even exists, otherwise skip to
-        # the next miRNA.
-        if not os.path.isfile(model):
-            print('WARNING: No covariance model found for {}'.format(mirid))
-            mmdict[mirna[0]] = ''
-            continue
-        # Check if the output folder exists, otherwise create it.
-        if not os.path.isdir('{}'.format(output)):
-            mkdir = 'mkdir -p {}'.format(output)
-            sp.call(mkdir, shell=True)
-
-        # Obtain the reference bit score for each miRNA by applying it
-        # to its own covariance model.
-        
-        # Create a temporary FASTA file with the miRNA sequence as
-        # query for external search tool cmsearch to calculate the
-        # reference bit score.
-        with open(query, 'w') as tmpfile:
-            tmpfile.write('>{0}\n{1}'.format(mirid, seq))
-        cms_command = (
-            'cmsearch -E 0.01 --noali {0} {1}'
-            .format(model, query)
-        )
-        res = sp.run(cms_command, shell=True, capture_output=True)
-        if res.returncode == 0:
-            top_score = find_refbit(res.stdout.decode('utf-8'))
-            mirna.append(top_score)
-        else:
-            print(f'ERROR: {res.stderr.decode("utf-8")}')
-            sys.exit()
-        # cleanup
-        os.remove(query)
-        # Create output.
-        mmdict[mirna[0]] = Mirna(*mirna)
-
-    return mmdict
-
-
-# Allow boolean argument parsing
-def str2bool(v):
-    if isinstance(v, bool):
-        return v
-    if v.lower() in ('yes', 'true', 't', 'y', '1'):
-        return True
-    elif v.lower() in ('no', 'false', 'f', 'n', '0'):
-        return False
-    else:
-        raise argparse.ArgumentTypeError('Boolean value expected.')
+    from cmsearch import model_search
+    from utils import check_blastdb, make_blastndb, write_output, str2bool
+    from reblast import perform_reblast
+    from rna_object import rna_maker
+except ModuleNotFoundError:
+    from ncOrtho.blastparser import ReBlastParser
+    from ncOrtho.genparser import GenomeParser
+    from ncOrtho.cmsearch import model_search
+    from ncOrtho.utils import check_blastdb, make_blastndb, write_output, str2bool
+    from ncOrtho.reblast import perform_reblast
+    from rna_object import rna_maker
 
 
 # Main function
 def main():
-    # Print header
-    print('\n'+'#'*57)
-    print('###'+' '*51+'###')
-    print('###   ncOrtho - ortholog search for non-coding RNAs   ###')
-    print('###'+' '*51+'###')
-    print('#'*57+'\n')
-
     ##########################################################################################
     # Command line arguments
     ##########################################################################################
     
     # Parse command-line arguments
     # Define global variables
     parser = argparse.ArgumentParser(
@@ -251,20 +133,32 @@
         help=(
             'Length cutoff for BLASTN search with which candidate regions for the CMsearch are identified.'
             'Cutoff is given as ratio of the reference pre-miRNA length '
             '(Default: 0.5) (Set to 0 to turn off)'
         )
     )
     optional.add_argument(
+        '--sensitive_heuristic', type=float, metavar='True/False', nargs='?', const=False, default=False,
+        help=(
+            'If no candidate region is found via BLASTn, search with CM in full query genome (Default: False)'
+        )
+    )
+    optional.add_argument(
         '--cleanup', type=str2bool, metavar='True/False', nargs='?', const=True, default=True,
         help=(
             'Cleanup temporary files (Default: True)'
         )
     )
     optional.add_argument(
+        '--phmm', type=str2bool, metavar='True/False', nargs='?', const=False, default=False,
+        help=(
+            'Use pHMM instead of CM for ortholog search (Default: False)'
+        )
+    )
+    optional.add_argument(
         '--refblast', type=str, metavar='<path>', nargs='?', const='', default='',
         help=(
             'Path to BLASTdb of the reference species'
         )
     )
     optional.add_argument(
         '--queryblast', type=str, metavar='<path>', nargs='?', const='', default='',
@@ -281,31 +175,33 @@
         )
     )
     # use dust filter?
     optional.add_argument(
         '--dust', metavar='yes/no', type=str,
         help='Use BLASTn dust filter during re-BLAST. Greatly decreases runtime if reference miRNA(s) '
              'are located in repeat regions. '
-             'However ncOrtho will also not identify orthologs for these miRNAs',
+             'However ncOrtho will also not identify orthologs for these miRNAs (Default: no)',
         nargs='?',
         const='no', default='no'
     )
     # check Co-ortholog-ref
     optional.add_argument(
         '--checkCoorthologsRef', type=str2bool, metavar='True/False', nargs='?', const=False, default=False,
         help=(
             'If the re-blast does not identify the original reference miRNA sequence as best hit,'
             'ncOrtho will check whether the best blast '
             'hit is likely a co-ortholog of the reference miRNA relative to the search taxon. '
-            'NOTE: Setting this flag will substantially increase'
-            'the sensitivity of HaMStR but most likely affect also the specificity, '
-            'especially when the search taxon is evolutionarily only very'
-            'distantly related to the reference taxon (Default: False)'
         )
     )
+
+    # print header
+    custom_fig = Figlet(font='stop')
+    print(custom_fig.renderText('ncOrtho')[:-3], flush=True)
+    v = version('ncOrtho')
+    print(f'Version: {v}\n', flush=True)
     ##########################################################################################
     # Parse arguments
     ##########################################################################################
 
     # Show help when no arguments are added.
     if len(sys.argv) == 1:
         parser.print_help()
@@ -319,27 +215,27 @@
         raise ValueError('The provided number of CPU cores is higher than the number available on this system')
     else:
         cpu = args.cpu
 
     # mandatory
     mirnas = args.ncrna
     models = args.models
-    output = args.output
+    output = os.path.realpath(args.output)
     query = args.query
     reference = args.reference
 
     # optional
     try:
         max_hits = int(args.maxcmhits)
     except TypeError:
         max_hits = None
     cm_cutoff = args.cm_cutoff
     checkCoorthref = args.checkCoorthologsRef
     cleanup = args.cleanup
-    heuristic = (args.heuristic, args.heur_blast_evalue, args.heur_blast_length)
+    heuristic = (args.heuristic, args.heur_blast_evalue, args.heur_blast_length, args.sensitive_heuristic)
     msl = args.minlength
     refblast = args.refblast
     qblast = args.queryblast
     dust = args.dust.strip()
 
     ##########################################################################################
     # Starting argument checks
@@ -347,14 +243,16 @@
 
     # Test if optional query name was given
     if args.queryname:
         qname = args.queryname
     else:
         qname = '.'.join(query.split('/')[-1].split('.')[:-1])
     # make folder for query in output dir
+    if not os.path.isdir(output):
+        os.mkdir(output)
     if not output.split('/')[-1] == qname:
         output = f'{output}/{qname}'
 
     # Test if input files exist
     all_files = [mirnas, reference, query]
     for pth in all_files:
         if not os.path.isfile(pth):
@@ -363,18 +261,16 @@
         raise ValueError(f'Directory with covariance models does not exist at: {models}')
 
     # create symbolic links to guarantee writing permissions for pyfaidx index
     q_data = '{}/data'.format(output)
     if not os.path.isdir(q_data):
         os.makedirs(q_data)
     qlink = f'{q_data}/{qname}.fa'
-    try:
+    if not os.path.islink(qlink):
         os.symlink(query, qlink)
-    except FileExistsError:
-        pass
 
     # check if reference BLASTdb was given as input
     if refblast:
         # check if BLASTdb exists
         if not check_blastdb(refblast):
             raise ValueError('# Reference BLASTdb not found at: {}'.format(refblast))
     else:
@@ -400,161 +296,133 @@
             make_blastndb(query, qlink)
 
     ###############################################################################################
     # Main
     ###############################################################################################
 
     # Print out query
-    print('### Starting ncOrtho run for {}\n'.format(qname))
+    print('# Starting ncOrtho run for {}\n'.format(qname), flush=True)
 
     # Create miRNA objects from the list of input miRNAs.
-    mirna_dict = mirna_maker(mirnas, models, output, msl)
+    mirna_dict = rna_maker(mirnas, models, args.phmm, cpu)
 
-    outpath = '{0}/{1}_orthologs.fa'.format(output, qname)
-    log_file = f'{output}/{qname}.log'
-    with open(log_file, 'w') as log, open(outpath, 'w') as of:
-        log.write(f'# miRNA\tStatus\n')
-        # Identify ortholog candidates.
-        for mirna in mirna_dict:
-            restricted = False
-            sys.stdout.flush()
-            mirna_data = mirna_dict[mirna]
-            # mirna objects for which no CM was found are empty
-            if not mirna_data:
-                log.write(f'{mirna}\tNo CM\n')
-                continue
-            print(f'\n### {mirna}')
+    # setup logging
+    shortlog = ['# miRNA\tSeconds\tStatus\n']
+    logout = f'{output}/{qname}_extended.log'
+    if os.path.isfile(logout):
+        os.remove(logout)
+    logger = logging.getLogger('ncortho')
+    logger.setLevel(logging.DEBUG)
+    fh = logging.FileHandler(logout)
+    fh.setLevel(logging.DEBUG)
+    logger.addHandler(fh)
+    sucess_count = 0
+
+    print('\n# Ortholog search', flush=True)
+    mirna_orthologs = []
+    for mirna in tqdm(mirna_dict, file=sys.stdout):
+        st = time()
+        restricted = False
+        sys.stdout.flush()
+        mirna_data = mirna_dict[mirna]
+        # mirna objects for which no CM was found are empty
+        if not mirna_data:
+            et = time()
+            elapsed_time = str(et - st)
+            shortlog.append(f'{mirna}\t{elapsed_time}\tNo CM\n')
+            continue
+        logger.info(f'\n### {mirna}')
 
-            # Create output folder, if not existent.
-            if not heuristic[0] or not cleanup:
-                outdir = '{}/{}'.format(output, mirna)
-            else:
-                outdir = '{}'.format(output)
-            if not os.path.isdir(outdir):
-                os.makedirs(outdir)
-
-            # start cmsearch
-            cm_results, exitstatus = cmsearcher(
-                mirna_data, cm_cutoff, cpu, msl, models, qlink, qblast, outdir, cleanup, heuristic
-            )
+        # Create output folder, if not existent.
+        if not heuristic[0] or not cleanup:
+            outdir = '{}/{}'.format(output, mirna)
+        else:
+            outdir = '{}'.format(output)
+        if not os.path.isdir(outdir):
+            os.makedirs(outdir)
+
+        # start cmsearch
+        cm_results, exitstatus = model_search(
+            mirna_data, cm_cutoff, cpu, msl, models, qlink, qblast, outdir, cleanup, heuristic, args.phmm
+        )
 
-            # Extract sequences for candidate hits (if any were found).
-            if not cm_results:
-                print('# {} for {}'.format(exitstatus, mirna))
-                log.write(f'{mirna}\t{exitstatus}\n')
+        # Extract sequences for candidate hits (if any were found).
+        if not cm_results:
+            logger.info('# {} for {}'.format(exitstatus, mirna))
+            et = time()
+            elapsed_time = str(et - st)
+            shortlog.append(f'{mirna}\t{elapsed_time}\t{exitstatus}\n')
+            continue
+        elif max_hits:
+            if len(cm_results) > max_hits:
+                logger.warning('# Maximum CMsearch hits reached. Restricting to best {} hits'.format(max_hits))
+                cm_results = {k: cm_results[k] for k in list(cm_results.keys())[:max_hits]}
+                restricted = True
+        # get sequences for each CM result
+        gp = GenomeParser(qlink, cm_results.values())
+        candidates = gp.extract_sequences()
+        logger.info('Covariance model search successful, found 1 ortholog candidate(s).')
+
+        # Perform reverse BLAST test to verify candidates, stored in
+        reblast_hits = {}
+        for candidate in candidates:
+            sequence = candidates[candidate]
+            if list(sequence).count('N') >= 0.9 * len(sequence):
                 continue
-            elif max_hits:
-                if len(cm_results) > max_hits:
-                    print('# Maximum CMsearch hits reached. Restricting to best {} hits'.format(max_hits))
-                    cm_results = {k: cm_results[k] for k in list(cm_results.keys())[:max_hits]}
-                    restricted = True
-            # get sequences for each CM result
-            gp = GenomeParser(qlink, cm_results.values())
-            candidates = gp.extract_sequences()
-            nr_candidates = len(candidates)
-            if nr_candidates == 1:
-                print(
-                    '# Covariance model search successful, found 1 '
-                    'ortholog candidate.'
-                )
+            # print('# Starting reverse blast for {}'.format(candidate))
+            reblasthit = perform_reblast(
+                sequence, refblast, cpu, outdir, candidate, mirna_data, dust, msl, cleanup, checkCoorthref
+            )
+            if reblasthit:
+                reblast_hits[candidate] = reblasthit
+
+        # Write output file if no candidate got accepted.
+        if not reblast_hits:
+            et = time()
+            elapsed_time = str(et - st)
+            logger.info(f'# None of the candidates for {mirna} could be verified.')
+            if restricted:
+                shortlog.append(f'{mirna}\t{elapsed_time}\tNo re-BLAST after restricting to {max_hits} CMsearch hits\n')
             else:
-                print(
-                    '# Covariance model search successful, found {} '
-                    'ortholog candidates.'
-                    .format(nr_candidates)
-                )
-            print('# Evaluating candidates.')
-
-            # Perform reverse BLAST test to verify candidates, stored in
-            # a list (accepted_hits).
-            reblast_hits = {}
-            for candidate in candidates:
-                sequence = candidates[candidate]
-                # print('# Starting reverse blast for {}'.format(candidate))
-                blast_command = (
-                    'blastn -task blastn -db {0} -num_threads {1} -dust {2} -outfmt "6 qseqid sseqid pident '
-                    'length mismatch gapopen qstart qend sstart send evalue bitscore sseq"'
-                        .format(refblast, cpu, dust)
-                )
-                blast_command = (
-                    'blastn -task blastn -db {0} -num_threads {1} -dust {2} -outfmt "6 sseqid '
-                    'sstart send sstrand bitscore"'
-                    .format(refblast, cpu, dust)
-                )
-                blast_call = sp.Popen(
-                    blast_command, shell=True, stdin=sp.PIPE,
-                    stdout=sp.PIPE, stderr=sp.PIPE, encoding='utf8'
-                )
-                # run BLAST
-                res, err = blast_call.communicate(sequence)
-                if err:
-                    print(f'ERROR: {err}')
-                    continue
-                if not cleanup:
-                    blast_output = '{0}/reBLAST_{1}.out'.format(outdir, candidate)
-                    with open(blast_output, 'w') as bh:
-                        for line in res:
-                            bh.write(line)
-                # parse BLASTn results
-                blast_output = [line.split() for line in res.split('\n')]
-                if not blast_output[0]:
-                    print('No re-BLAST hits')
-                    continue
-
-                # BlastParser will read the temp_fasta file
-                bp = BlastParser(mirna_data, blast_output, msl)
-                # the parse_blast_output function will return True if the candidate is accepted
-                if bp.evaluate_besthit():
-                    print('Found best hit')
-                    reblast_hits[candidate] = sequence
-                elif checkCoorthref:
-                    print('Best hit differs from reference sequence! Doing further checks\n')
-                    # coorth_out = '{0}/{1}_coorth'.format(outdir, candidate)
-                    if bp.check_coortholog_ref(sequence, outdir):
-                        reblast_hits[candidate] = sequence
-                else:
-                    print('Best hit does not overlap with miRNA location')
-
-            # Write output file if at least one candidate got accepted.
-            if reblast_hits:
-                nr_accepted = len(reblast_hits)
-                if nr_accepted == 1:
-                    print('# ncOrtho found 1 verified ortholog.')
-                    out_dict = reblast_hits
-                else:
-                    print(
-                        '# ncOrtho found {} potential co-orthologs.'
-                        .format(nr_accepted)
-                    )
-                    print('# Evaluating distance between candidates to verify co-orthologs')
-                    rbp = ReBlastParser(mirna_data, reblast_hits)
-                    out_dict = rbp.verify_coorthologs(outdir)
-                    if len(out_dict) == 1:
-                        print('ncOrtho found 1 verified ortholog')
-                    else:
-                        print(
-                            '# ncOrtho found {} verified co-orthologs.'
-                                .format(len(out_dict))
-                        )
-
-                for hit in out_dict:
-                    cmres = list(cm_results[hit])
-                    cmres.insert(0, qname)
-                    cmres = [str(entry) for entry in cmres]
-                    header = '|'.join(cmres)
-                    of.write('>{0}\n{1}\n'.format(header, out_dict[hit]))
+                shortlog.append(f'{mirna}\t{elapsed_time}\tNo re-BLAST\n')
+            continue
 
-                log.write(f'{mirna}\tSUCESS\n')
+        # Write output file if at least one candidate got accepted.
+        nr_accepted = len(reblast_hits)
+        if nr_accepted == 1:
+            logger.info('# ncOrtho found 1 verified ortholog.')
+            out_dict = reblast_hits
+        else:
+            logger.info(
+                '# ncOrtho found {} potential co-orthologs.'
+                .format(nr_accepted)
+            )
+            logger.info('# Evaluating distance between candidates to verify co-orthologs')
+            rbp = ReBlastParser(mirna_data, reblast_hits)
+            out_dict = rbp.verify_coorthologs(outdir)
+            if len(out_dict) == 1:
+                logger.info('ncOrtho found 1 verified ortholog')
             else:
-                print(
-                    '# None of the candidates for {} could be verified.'
-                    .format(mirna)
-                )
-                if restricted:
-                    log.write(f'{mirna}\tNo re-BLAST after restricting to {max_hits} CMsearch hits\n')
-                else:
-                    log.write(f'{mirna}\tNo re-BLAST\n')
-        print('\n### ncOrtho is finished!')
+                logger.info(f'# ncOrtho found {len(out_dict)} verified co-orthologs.')
+
+        for hit in out_dict:
+            cmres = list(cm_results[hit])
+            cmres.insert(0, qname)
+            cmres = [str(entry) for entry in cmres]
+            header = '|'.join(cmres)
+            mirna_orthologs.append('>{0}\n{1}\n'.format(header, out_dict[hit]))
+
+        et = time()
+        elapsed_time = str(round(et - st, 3))
+        shortlog.append(f'{mirna}\t{elapsed_time}\tSUCESS\n')
+        sucess_count += 1
+
+    write_output(mirna_orthologs, f'{output}/{qname}_orthologs.fa')
+    write_output(shortlog, f'{output}/{qname}_summary.log')
+    # logging.basicConfig(filename=f'{output}/{qname}_extended.log', level=logging.DEBUG)
+
+    print(f'\n### ncOrtho found orthologs for {sucess_count} out of {len(mirna_dict)} ncRNAs')
 
 
 if __name__ == "__main__":
     main()
+
```

### Comparing `ncOrtho-0.3.9/ncOrtho.egg-info/PKG-INFO` & `ncOrtho-0.4.0/ncOrtho.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncOrtho
-Version: 0.3.9
+Version: 0.4.0
 Summary:  Targeted ortholog search for miRNAs 
 Home-page: https://github.com/felixlangschied/ncortho
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -22,15 +22,15 @@
 NcOrtho is a tool for the targeted search of orthologous micro RNAs (miRNAs) throughout the tree of life. 
 Conceptually, it works similar to the program [fDOG](https://github.com/BIONF/fDOG) in that a probabilistic model of 
 a reference miRNA is created. For training the model, orthologs of the reference sequence are first identified in 
 a set of taxa that are more closely related to the reference species. In contrast to fDOG, ncOrtho does not train hidden 
 Markov Models but covariance models (CMs) (Eddy & Durbin, 1994) 
 which also model conservation of the miRNA's secondary structure.
 
-![workflow](https://github.com/felixlangschied/ncortho/blob/master/ncOrtho/docs/figure1_ncortho_worklfow.png)
+![workflow](https://github.com/BIONF/ncortho/blob/master/ncOrtho/docs/figure1_ncortho_worklfow.png)
 
 ## Getting Started
 NcOrtho depends on multiple third party applications, some of which are Linux specific.
 All dependencies can be installed with [Anaconda](https://www.anaconda.com/).
 It is recommended to create a new Anaconda environment for this. For example:
 ```
 conda create --name ncOrtho python=3.8
@@ -42,14 +42,15 @@
 * **Python:** version 3 or higher (tested with v3.8)
 
 Tool | Tested version | Anaconda installation
 ------------ | ------------- | -------------
 BLASTn | v2.7.1 | `conda install -c kantorlab blastn`
 Infernal | v1.1.4 | `conda install -c bioconda infernal`
 t_coffee | v13.45 | `conda install -c bioconda t-coffee`
+MUSCLE | v5.1 | `conda install -c bioconda muscle`
 
 ### Installing
 
 After installing all three dependencies, ncOrtho can be installed with `pip`:
 ```
  pip install ncOrtho
 ```
@@ -61,30 +62,37 @@
 
 For this reason, a few questions need to be answered, before we can start constructing covariance models:
 1. What is the reference species?
 2. How phylogenetically diverse will my set of target species be?
 3. From which species should the core set of miRNA orthologs be extracted, which will be used for training the CMs?
 4. Which miRNAs are going to be used for the ortholog search?
 
-You can (soon) find more information on how to answer these questions in the 
-[WIKI](https://github.com/felixlangschied/ncortho/wiki/Creating-miRNA-covariance-models#choosing-core-species).
+To identify suitable core species for a given reference species you can calculate an estimate of conserved synteny 
+given a set of pairwise ortholog predictions with:
+```
+ncCheck -p <parameters.yaml> -o <outdir>
+```
+You can find additional information about ncCheck in the
+[WIKI](https://github.com/BIONF/ncortho/wiki/Choosing-core-species).
+
+
 As soon as you know what your core species are going to be, you will need to collect the following data:
 
 * Genomic sequence in FASTA format (e.g "genomic.fna" from RefSeq)
 * Genome annotation in GFF3 format (e.g. "genomic.gff" from RefSeq)
 * Pairwise orthologs of all proteins between the reference and each core species (more information 
-[here](https://github.com/felixlangschied/ncortho/wiki/Input-Data#pairwise-orthologs)
+[here](https://github.com/BIONF/ncortho/wiki/Input-Data#pairwise-orthologs)
 
 Modify the [example parameters](ncOrtho/coreset/example_parameters.yaml) file to contain all 
 relevant paths to your input files. The "name" property of your reference and core species has to merely be a 
-unique identifier. It is however recommended to use the correct species names to increase readability.
+unique identifier. It is however recommended to use whitespace-free species names to increase readability.
 
 Additional to the parameters file, you will need a tab separated file containing the position and sequence of each 
 miRNA for which a model should be constructed (more information 
-[here](https://github.com/felixlangschied/ncortho/wiki/Input-Data#reference-mirnas)). 
+[here](https://github.com/BIONF/ncortho/wiki/Input-Data#reference-mirnas)). 
 
 You can then start CM construction with:
 ```
 ncCreate -p <parameters.yaml> -n <mirnas.tsv> -o <outdir>
 ```
 If you encounter errors, make sure that:
 * The identifiers in the pairwise orthologs files match the ones in the gff files (use the `-idtype=` flag to use other
@@ -98,19 +106,30 @@
 
 You can start the orthology search with:
 ```
 ncSearch -m <CMs/> -n <mirnas.tsv> -q <query_genome.fa> -r <reference_genome.fa> -o <outdir>
 ```
 
 Use `ncSearch -h` to see all available options for the orthology search or have a look at the 
-[WIKI](https://github.com/felixlangschied/ncortho/wiki/Running-the-orthology-search).
+[WIKI](https://github.com/BIONF/ncortho/wiki/Running-the-orthology-search).
+
+### Phylogenetic Analysis
+
+To facilitate the downstream analyses of miRNA orthologs, we also supply the `ncAnalyze` function:
+```
+ncAnalzye -r <result directory of ncOrtho> -o <output_dir> -m <mappingfile>
+```
+This will create a phylogenetic Profile ready for visualisation in [PhyloProfile](https://github.com/BIONF/PhyloProfile)
+as well as calculate a supermatrix species tree based on the miRNA orthologs.
+
+More information can be found with `ncAnalyze -h` or the [WIKI](https://github.com/BIONF/ncortho/wiki/Analysis)
 
 ## Support
 
-Please refer to our Wiki Page of [known issues](https://github.com/felixlangschied/ncortho/wiki/Known-Issues) first, 
+Please refer to our Wiki Page of [known issues](https://github.com/BIONF/ncortho/wiki/Known-Issues) first, 
 then consider opening an issue on GitHub or contacting me directly via [mail](langschied@bio.uni-frankfurt.de)
 
 ## Contributors
 
 * [Felix Langschied](https://github.com/felixlangschied)
 * [Andreas Blaumeiser](https://github.com/acblaumeiser)
 * Mirko Brüggemann
```

### Comparing `ncOrtho-0.3.9/ncOrtho.egg-info/SOURCES.txt` & `ncOrtho-0.4.0/ncOrtho.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 ncOrtho/__init__.py
 ncOrtho/blastparser.py
 ncOrtho/cmsearch.py
+ncOrtho/figletest.py
 ncOrtho/genparser.py
 ncOrtho/ncortho.py
+ncOrtho/reblast.py
+ncOrtho/rna_object.py
+ncOrtho/tmp_old_cmsearch.py
 ncOrtho/utils.py
 ncOrtho.egg-info/PKG-INFO
 ncOrtho.egg-info/SOURCES.txt
 ncOrtho.egg-info/dependency_links.txt
 ncOrtho.egg-info/entry_points.txt
 ncOrtho.egg-info/requires.txt
 ncOrtho.egg-info/top_level.txt
@@ -24,9 +28,8 @@
 ncOrtho/coreset/__init__.py
 ncOrtho/coreset/core_reblast.py
 ncOrtho/coreset/coreset.py
 ncOrtho/coreset/coreset_utils.py
 ncOrtho/coreset/createcm.py
 ncOrtho/coreset/example_parameters.yaml
 ncOrtho/coreset/locate_position.py
-ncOrtho/coreset/synteny.py
-ncOrtho/coreset/tmp.py
+ncOrtho/coreset/synteny.py
```

### Comparing `ncOrtho-0.3.9/setup.py` & `ncOrtho-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncOrtho",
-    version="0.3.9",
+    version="0.4.0",
     python_requires='>=3.7.0',
     description=" Targeted ortholog search for miRNAs ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     url="https://github.com/felixlangschied/ncortho",
     packages=find_packages(),
     package_data={'': ['*']},
     install_requires=[
         'PyYAML',
         'biopython',
-        'pyfaidx'
+        'pyfaidx',
+        'pyfiglet'
     ],
     entry_points={
         'console_scripts': ["ncCreate = ncOrtho.coreset.coreset:main",
                             "ncSearch = ncOrtho.ncortho:main",
                             "ncAnalyze = ncOrtho.analysis.ncAnalyze:main",
                             "ncCheck = ncOrtho.check.core_synteny:main"
                             ],
```

