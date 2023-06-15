# Comparing `tmp/kmerator-0.7.7b0.tar.gz` & `tmp/kmerator-0.8.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerator-0.7.7b0.tar", last modified: Tue May 16 08:28:58 2023, max compression
+gzip compressed data, was "kmerator-0.8.1b0.tar", last modified: Thu Jun 15 13:05:40 2023, max compression
```

## Comparing `kmerator-0.7.7b0.tar` & `kmerator-0.8.1b0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-16 08:28:58.832640 kmerator-0.7.7b0/
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.7.7b0/MANIFEST.in
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13261 2023-05-16 08:28:58.828371 kmerator-0.7.7b0/PKG-INFO
--rw-r--r--   0 benoit    (1017) bio2m     (1010)    11434 2023-05-10 16:09:57.000000 kmerator-0.7.7b0/README.md
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-16 08:28:58.724654 kmerator-0.7.7b0/kmerator/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.7.7b0/kmerator/__init__.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.7.7b0/kmerator/color.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.7.7b0/kmerator/config.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19683 2023-05-16 08:28:01.000000 kmerator-0.7.7b0/kmerator/dataset.py
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.7.7b0/kmerator/exit.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-05-15 12:09:40.000000 kmerator-0.7.7b0/kmerator/info.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    11941 2023-05-16 08:27:00.000000 kmerator-0.7.7b0/kmerator/kmerator.py
--rw-r--r--   0 benoit    (1017) bio2m     (1010)    16939 2023-05-11 10:39:13.000000 kmerator-0.7.7b0/kmerator/kmerize.py
--rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.7.7b0/kmerator/longest_transcript.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.7.7b0/kmerator/mk_geneinfo.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.7.7b0/kmerator/mk_transcriptome.py
--rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    12152 2023-05-16 08:26:02.000000 kmerator-0.7.7b0/kmerator/options.py
-drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-05-16 08:28:58.812392 kmerator-0.7.7b0/kmerator.egg-info/
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13261 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/PKG-INFO
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/SOURCES.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/dependency_links.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/entry_points.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/requires.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-05-16 08:28:58.000000 kmerator-0.7.7b0/kmerator.egg-info/top_level.txt
--rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-05-16 08:28:58.835056 kmerator-0.7.7b0/setup.cfg
--rw-r--r--   0 benoit    (1017) bio2m     (1010)     1008 2023-02-28 16:14:06.000000 kmerator-0.7.7b0/setup.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-15 13:05:40.573857 kmerator-0.8.1b0/
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      182 2023-04-17 07:20:43.000000 kmerator-0.8.1b0/MANIFEST.in
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-15 13:05:40.569773 kmerator-0.8.1b0/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    11626 2023-06-15 12:20:25.000000 kmerator-0.8.1b0/README.md
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-15 13:05:40.452747 kmerator-0.8.1b0/kmerator/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      115 2023-04-17 07:49:13.000000 kmerator-0.8.1b0/kmerator/__init__.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)      249 2023-02-16 14:55:54.000000 kmerator-0.8.1b0/kmerator/color.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     2715 2023-02-17 12:04:30.000000 kmerator-0.8.1b0/kmerator/config.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    19683 2023-05-16 08:28:01.000000 kmerator-0.8.1b0/kmerator/dataset.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      289 2023-02-13 12:52:30.000000 kmerator-0.8.1b0/kmerator/exit.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)     1554 2023-06-15 12:58:43.000000 kmerator-0.8.1b0/kmerator/info.py
+-rwxrwxr-x   0 benoit    (1017) bio2m     (1010)    11984 2023-06-15 12:31:45.000000 kmerator-0.8.1b0/kmerator/kmerator.py
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    18618 2023-06-15 12:55:37.000000 kmerator-0.8.1b0/kmerator/kmerize.py
+-rw-r--r--   0 benoit    (1017) bio2m     (1010)      757 2023-02-16 14:24:06.000000 kmerator-0.8.1b0/kmerator/longest_transcript.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    10602 2023-02-28 11:49:15.000000 kmerator-0.8.1b0/kmerator/mk_geneinfo.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)     8671 2023-02-20 09:09:59.000000 kmerator-0.8.1b0/kmerator/mk_transcriptome.py
+-rwxr-xr-x   0 benoit    (1017) bio2m     (1010)    12152 2023-05-16 08:26:02.000000 kmerator-0.8.1b0/kmerator/options.py
+drwxrwxr-x   0 benoit    (1017) bio2m     (1010)        0 2023-06-15 13:05:40.553502 kmerator-0.8.1b0/kmerator.egg-info/
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)    13556 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/PKG-INFO
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)      481 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/SOURCES.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        1 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/dependency_links.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       53 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/entry_points.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       18 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/requires.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)        9 2023-06-15 13:05:40.000000 kmerator-0.8.1b0/kmerator.egg-info/top_level.txt
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)       38 2023-06-15 13:05:40.576299 kmerator-0.8.1b0/setup.cfg
+-rw-rw-r--   0 benoit    (1017) bio2m     (1010)     1109 2023-06-15 12:34:30.000000 kmerator-0.8.1b0/setup.py
```

### Comparing `kmerator-0.7.7b0/PKG-INFO` & `kmerator-0.8.1b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.7.7b0
+Version: 0.8.1b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
         
         ## Prototype for decomposition of transcript or gene sequences and extraction of their specific k-mers
         
         ref: <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8221386/>
         
-        Kmerator is a prototype tool designed for the prediction of specific k-mers (also called tags) from input sequences, considering a reference genome and an ENSEMBL-like transcriptome. From these specific k-mers, it also outputs their corresponding specific contigs which are sequences of consecutive k-mers (overlapping length between k-mers must be k-1, otherwise, it's a new contig). Kmerator first uses Jellyfish [1] to create 2 requestable indexes from the reference genome and transcriptome, and second, decomposes your input transcript or gene sequences to count the occurences of each k-mer in the genome and transcriptome. Number of occurrences are then interpreted, in different manners, to select specific k-mer from your input. 
+        Kmerator is a prototype tool designed for the prediction of specific k-mers (also called tags) from input sequences, considering a reference genome and an ENSEMBL-like transcriptome. From these specific k-mers, it also outputs their corresponding specific contigs which are sequences of consecutive k-mers (overlapping length between k-mers must be k-1, otherwise, it's a new contig). You need to provide kmerator with a jellifsh index of the reference genome. Kmerator itself builds a jellyfish index of the reference transcriptome (by default the latest available version of Ensembl). It then  decomposes your input transcript or gene sequences to count the occurences of each k-mer in the genome and transcriptome. Number of occurrences are then interpreted, in different manners, to select specific k-mer from your input. 
         
         Before using kmerator, a jellyfish index of the reference genome must be created. kmerator automatically creates a dataset according to the species and the desired release number (by default, homo_sapiens and the latest version). The dataset is composed of 4 files per species/version: a jellyfish index of the modified transcriptome (cDNA + ncRNA - alternative chormosomes) from Ensembl, a binary file representing the same transcriptome, another binary file containing general information on the genes of the transcriptome and a report file.
         
         
         #### Specific kmers
         
         ![](https://github.com/Transipedia/kmerator/raw/main/img/specific-kmers.png)
@@ -49,15 +49,15 @@
         git clone https://github.com/Transipedia/kmerator3.git
         ln -s $PWD/kmerator3/kmerator/kmerator.py /usr/local/bin/kmerator  # or somewhere in your $PATH
         ```
         
         
         ## How to use kmerator
         
-        Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying. You can store and name the index file whatever you want.
+        Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying. You can store and name the index file whatever you want. Please note that you must **not use the jellyfish -C option** when building the reference genome index.
         
         ### Configuration file
         
         The arguments to run kmerator are numerous, so to reduce the number of arguments to enter, it is advisable to edit the configuration file with the command :
         
         ```
         kmerator -e
@@ -151,14 +151,16 @@
         ## References
         
         [1] Guillaume Marçais, Carl Kingsford, A fast, lock-free approach for efficient parallel counting of occurrences of k-mers, Bioinformatics, Volume 27, Issue 6, 15 March 2011, Pages 764–770, https://doi.org/10.1093/bioinformatics/btr011
         [2] Rodriguez JM, et al. Nucleic Acids Res. Database issue; 2017 Oct 23
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
-Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `kmerator-0.7.7b0/README.md` & `kmerator-0.8.1b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Kmerator
 
 ## Prototype for decomposition of transcript or gene sequences and extraction of their specific k-mers
 
 ref: <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8221386/>
 
-Kmerator is a prototype tool designed for the prediction of specific k-mers (also called tags) from input sequences, considering a reference genome and an ENSEMBL-like transcriptome. From these specific k-mers, it also outputs their corresponding specific contigs which are sequences of consecutive k-mers (overlapping length between k-mers must be k-1, otherwise, it's a new contig). Kmerator first uses Jellyfish [1] to create 2 requestable indexes from the reference genome and transcriptome, and second, decomposes your input transcript or gene sequences to count the occurences of each k-mer in the genome and transcriptome. Number of occurrences are then interpreted, in different manners, to select specific k-mer from your input. 
+Kmerator is a prototype tool designed for the prediction of specific k-mers (also called tags) from input sequences, considering a reference genome and an ENSEMBL-like transcriptome. From these specific k-mers, it also outputs their corresponding specific contigs which are sequences of consecutive k-mers (overlapping length between k-mers must be k-1, otherwise, it's a new contig). You need to provide kmerator with a jellifsh index of the reference genome. Kmerator itself builds a jellyfish index of the reference transcriptome (by default the latest available version of Ensembl). It then  decomposes your input transcript or gene sequences to count the occurences of each k-mer in the genome and transcriptome. Number of occurrences are then interpreted, in different manners, to select specific k-mer from your input. 
 
 Before using kmerator, a jellyfish index of the reference genome must be created. kmerator automatically creates a dataset according to the species and the desired release number (by default, homo_sapiens and the latest version). The dataset is composed of 4 files per species/version: a jellyfish index of the modified transcriptome (cDNA + ncRNA - alternative chormosomes) from Ensembl, a binary file representing the same transcriptome, another binary file containing general information on the genes of the transcriptome and a report file.
 
 
 #### Specific kmers
 
 ![](https://github.com/Transipedia/kmerator/raw/main/img/specific-kmers.png)
@@ -41,15 +41,15 @@
 git clone https://github.com/Transipedia/kmerator3.git
 ln -s $PWD/kmerator3/kmerator/kmerator.py /usr/local/bin/kmerator  # or somewhere in your $PATH
 ```
 
 
 ## How to use kmerator
 
-Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying. You can store and name the index file whatever you want.
+Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying. You can store and name the index file whatever you want. Please note that you must **not use the jellyfish -C option** when building the reference genome index.
 
 ### Configuration file
 
 The arguments to run kmerator are numerous, so to reduce the number of arguments to enter, it is advisable to edit the configuration file with the command :
 
 ```
 kmerator -e
```

### Comparing `kmerator-0.7.7b0/kmerator/config.py` & `kmerator-0.8.1b0/kmerator/config.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.7b0/kmerator/dataset.py` & `kmerator-0.8.1b0/kmerator/dataset.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.7b0/kmerator/info.py` & `kmerator-0.8.1b0/kmerator/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 Genral informations on to the program.
 """
 
 APPNAME = "kmerator"
 SHORTDESC = "Find specific gene or transcript kmers. And more."
 LICENCE = "GPL3"
-VERSION = "0.7.7-beta"
+VERSION = "0.8.1-beta"
 AUTHOR = 'Sébastien RIQUIER, IRMB, Montpellier'
 AUTHOR_EMAIL = "sebastien.riquier@ucd.ie"
 CONTIBUTORS = [
     'Chloe BESSIERE chloe.bessiere@inserm.fr>'
     'Benoit GUIBERT <benoit.guibert@inserm.fr>',
 ]
 DOC = f"""
```

### Comparing `kmerator-0.7.7b0/kmerator/kmerator.py` & `kmerator-0.8.1b0/kmerator/kmerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,30 +147,31 @@
 
             if found_count > 1:
                 report['multiple'].append(f"{given}: {found_count} ({', '.join([i for i in found_transcripts])})")
 
 
     ### With '--fasta-file' option
     if args.fasta_file:
+        type = 'chimera' if args.chimera else 'transcript'
         with open(args.fasta_file) as fh:
             seq = ""
             f_id = fh.readline()[1:].split(' ')[0].rstrip()
             for raw in fh:
                 if raw.startswith('>'):
                     if len(seq) >= args.kmer_length:
-                        items.append({'f_id': f_id, 'seq': seq, 'type': 'transcript'})
+                        items.append({'f_id': f_id, 'seq': seq, 'type': type})
                     else:
                         report['failed'].append(f"{f_id}: sequence to short ({len(seq)} < {args.kmer_length})")
                     f_id = raw[1:].split(' ')[0].rstrip()
                     seq = ""
                 else:
                     seq += raw.rstrip()
             ### last f_id/sequence
             if len(seq) >= args.kmer_length:
-                items.append({'f_id': f_id, 'seq': seq, 'type': 'transcript'})
+                items.append({'f_id': f_id, 'seq': seq, 'type': type})
             else:
                 report['failed'].append(f"{f_id}: sequence to short ({len(seq)} < {args.kmer_length})")
 
 
 
 def longest_transcript(args, ENSG):
     print(args)
```

### Comparing `kmerator-0.7.7b0/kmerator/kmerize.py` & `kmerator-0.8.1b0/kmerator/kmerize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ### kmerize.py
 
+"""
+https://stackoverflow.com/questions/44587669/python-multiprocessing-how-to-close-the-multiprocessing-pool-on-exception
+https://stackoverflow.com/questions/47903791/how-to-terminate-a-multiprocess-in-python-when-a-given-condition-is-met
+"""
+
 import os
 import sys
+import shutil
 import subprocess
 import multiprocessing
 import copy
 
 from color import *
 
 
@@ -27,21 +33,27 @@
         self.args = manager.dict(args.__dict__)
         if args.selection:
             self.transcriptome_dict = manager.dict(transcriptome_dict)
             self.geneinfo_dict = manager.dict(geneinfo_dict)
 
         ### launch workers
         self.transcriptome_file = os.path.join(args.datadir, f"{args.specie}.{args.assembly}.{args.release}.transcriptome.jf")
-        with multiprocessing.Pool(processes=args.thread) as pool:
-            if args.selection:
-                messages = pool.map(self.worker_selection, items)
-            elif args.fasta_file:
-                messages = pool.map(self.worker_fasta_file, items)
-        for type,mesg in messages:
-            report[type].append(mesg)
+        try:
+            with multiprocessing.Pool(processes=args.thread) as pool:
+                if args.selection:
+                    messages = pool.map(self.worker_selection, items)
+                elif args.fasta_file:
+                    messages = pool.map(self.worker_fasta_file, items)
+            for type,mesg in messages:
+                report[type].append(mesg)
+        except KeyError as e:
+            pool.close()
+            shutil.rmtree(args.tmpdir)
+            sys.exit(f"{RED}{e.args[0]}")
+
 
 
     def worker_selection(self, item):
         """ Function doc """
         ### unpack item
         globals().update(item)
         global level
@@ -70,15 +82,14 @@
 
         return mesg
 
 
     def worker_fasta_file(self, item):
         ### unpack item
         globals().update(item)
-        # ~ print(f"{f_id}: start worker")
         ### 1. write separate file for each item
         seq_file = self.dump_seq(item['f_id'], item['seq'])
 
         ### 2. From sequence, compute jellyfish against the genome/transcriptome and convert results as dict ()
         kmercounts_transcriptome_dict = self.jellyfish(seq_file, self.transcriptome_file)
         kmercounts_genome_dict = self.jellyfish(seq_file, self.args['genome'])
 
@@ -99,54 +110,58 @@
         with open(seq_file, 'w') as fh:
             fh.write(f">{f_id}\n{seq}\n")
         return seq_file
 
 
     def jellyfish(self, seq_file, jf_file):
         """
-        From sequence, compute jellyfish againt the genome/transcriptome and convert results as dict ()
+        From sequence, compute jellyfish againt the genome/transcriptome and convert results
+        as dict ()
         """
-        if self.args['debug']: print(f"{YELLOW}start jellyfish on {os.path.basename(seq_file)} against {os.path.basename(jf_file)}{ENDCOL}")
+        if self.args['debug']: print(f"{YELLOW}start jellyfish on {os.path.basename(seq_file)} "
+                                     f"against {os.path.basename(jf_file)}{ENDCOL}")
         cmd = f"jellyfish query -s '{seq_file}' {jf_file}"
         try:
-            # ~ result = subprocess.run(cmd, shell=True, check=True, capture_output=True).stdout.decode().rstrip().split('\n')
-            result = subprocess.check_output(cmd, shell=True, text=True, stderr=subprocess.STDOUT).rstrip('\n').split('\n')
+            result = subprocess.check_output(cmd, shell=True, text=True, stderr=subprocess.STDOUT) \
+                                             .rstrip('\n').split('\n')
         except subprocess.CalledProcessError as err:
             sys.exit(f"{ERROR}Error: executing jellyfish:\n"
                      f"  {ERROR}command: {ENDCOL}{cmd}\n"
                      f"  {ERROR}returned: {ENDCOL}{err.output}")
-        result_dict = dict([ (b[0], int(b[1])) for b in [a.split() for a in result]])
+        if not result[0]:
+            return {}
+        result_dict = dict([(b[0], int(b[1])) for b in [a.split() for a in result]])
         return result_dict
 
 
     def get_specific_kmers(self, item, kmercounts_transcriptome_dict, kmercounts_genome_dict):
         '''
         Keep only specific kmers, according to the arguments
         '''
         args = copy.deepcopy(self.args)
         ### Define some variables: gene_name, transcript_name, variants_dic and output file names
         '''
         d = {
-            'specific_kmers': [],             # specific kmers list
+            'specific_kmers': [],              # specific kmers list
             'specific_contigs': [],            # specific contigs list
-            'contig': "",                     # initialize contig sequence
-            'knb': 0,                         # kmer number (selected kmer)
+            'contig': "",                      # initialize contig sequence
+            'knb': 0,                          # kmer number (selected kmer)
             'c_nb': 1,                         # contig number
-            'kmer_pos_prev': 0,               # position of retained kmer
-            'contig_pos': 0,                  # position of retained contig
+            'kmer_pos_prev': 0,                # position of retained kmer
+            'contig_pos': 0,                   # position of retained contig
         }
         '''
-        level = 'transcript' if item['type'] == 'transcript' else 'gene'
-        specific_kmers = []             # specific kmers list
+        level = 'gene' if item['type'] not in ['transcript', 'chimera'] else item['type']
+        specific_kmers = []              # specific kmers list
         specific_contigs = []            # specific contigs list
-        contig = ""                     # initialize contig sequence
-        knb = 0                         # kmer number (selected kmer)
+        contig = ""                      # initialize contig sequence
+        knb = 0                          # kmer number (selected kmer)
         c_nb = 1                         # contig number
-        kmer_pos_prev = 0               # position of retained kmer
-        contig_pos = 0                  # position of retained contig
+        kmer_pos_prev = 0                # position of retained kmer
+        contig_pos = 0                   # position of retained contig
 
         ### initialization of count variables
         total_kmers = len(kmercounts_transcriptome_dict)
         if args['selection']:
             given_up = given.upper()
             isoforms = self.geneinfo_dict['gene'][ENSG]['transcript']
             isoforms_nb = len(isoforms)
@@ -166,15 +181,26 @@
             contig_outfile = f"{f_id}-transcript-specific_contigs.fa"
 
 
         i = 1
         for mer, abund_in_tr in kmercounts_transcriptome_dict.items():
 
             kmer_pos = i
-            abund_in_ge = int(kmercounts_genome_dict[mer])    # abundance in genome for this kmer
+            try:
+                abund_in_ge = int(kmercounts_genome_dict[mer])    # abundance in genome for this kmer
+            except KeyError:
+                if len(mer) != len(next(iter(kmercounts_genome_dict))):
+                    raise KeyError(f"ErrorIndexLength: length of kmer expected: {self.args['kmer_length']}\n"
+                                   f"  Genome kmer index length: {len(next(iter(kmercounts_genome_dict)))}\n"
+                                   f"  Transcriptome kmer index length (dataset): {len(mer)}")
+                revcomp = self.__revcomp(mer)
+                if revcomp in kmercounts_genome_dict:
+                    raise KeyError("ErrorGenomeIndex: The jellyfish indexes of the genome and "
+                                   "transcriptome do not match.\nA possible error is that the "
+                                   "genome index was built with the jellyfish '-C' option.")
 
             if level == 'gene':
                 ### if the kmer is present/unique or does not exist (splicing?) on the genome
                 if abund_in_ge <= 1:
 
                     isoforms_with_mer = [enst for enst, seq in isoforms_dict.items() if mer in seq]
                     isoforms_with_mer_nb = len(isoforms_with_mer)
@@ -217,22 +243,24 @@
                         ## kmers case
                         knb += 1
                         specific_kmers.append(f">{given_up}:{transcript}.kmer{kmer_pos} ({isoforms_with_mer_nb}/{isoforms_nb})\n{mer}")
                         ## contigs case
                         if knb == 1:                                    # first kmer in contig
                             contig = mer
                             kmer_pos_prev = kmer_pos
+                            contig_pos = kmer_pos
                         elif knb>1 and kmer_pos == kmer_pos_prev+1:     # add last bp to existing contig
                             contig += mer[-1]
                             kmer_pos_prev = kmer_pos
                         else:                                           # store contig and create new
                             specific_contigs.append(f">{given_up}:{transcript}.contig{c_nb} (at position {kmer_pos})\n{contig}")
                             c_nb += 1
                             contig = mer
                             kmer_pos_prev = kmer_pos
+                            contig_pos = kmer_pos
 
             ### Cases of transcripts 1) unannotated, 2) annotated.
             elif level == 'transcript':
                 ### Case of annotated transcripts
                 if args['selection'] and abund_in_tr == 1 and abund_in_ge <= 1:
                     ## kmers case
                     knb += 1
@@ -255,14 +283,15 @@
                 ### Case of unannotated transcripts
                 elif args['fasta_file'] and abund_in_tr <= self.args['max_on_transcriptome'] and abund_in_ge <= 1:     # max_on_transcriptome = 0 by default
                     ### kmers case
                     knb += 1
                     specific_kmers.append(f">{f_id}.kmer{kmer_pos}\n{mer}")
                     ### contigs case
                     if knb == 1:                                    # first kmer in contig
+                        contig = mer
                         kmer_pos_prev = kmer_pos
                         contig_pos = kmer_pos
                     elif knb>1 and kmer_pos == kmer_pos_prev+1:     # add last bp to existing contig
                         contig += mer[-1]
                         kmer_pos_prev = kmer_pos
                     else:
                         specific_contigs.append(f">{f_id}.contig{c_nb} (at position {contig_pos})\n{contig}")
@@ -271,32 +300,33 @@
                         kmer_pos_prev = kmer_pos
                         contig_pos = kmer_pos
 
             ### Case of chimera
             elif level == 'chimera':
                 if abund_in_tr == abund_in_ge == 0:
                     ### kmers case
-                    i += 1
+                    knb += 1
                     specific_kmers.append(f">{f_id}.kmer{kmer_pos}\n{mer}")
                     ### contig case
                     if knb == 1:
                         contig = mer
+                        kmer_pos_prev = kmer_pos
                         contig_pos = kmer_pos
                     elif knb>1 and kmer_pos == kmer_pos_prev+1:
                         contig += mer[-1]
                         kmer_pos_prev = kmer_pos
                     else:
                         specific_contigs.append(f">{f_id}.contig{c_nb} (at position {contig_pos})\n{contig}")
                         c_nb += 1
                         contig = mer
                         kmer_pos_prev = kmer_pos
                         contig_pos = kmer_pos
             ### not a gene, transcript, or chimera
             else:
-                sys.exit(f"{RED}Error: level {level} unknown.{ENDCOL}")
+                raise KeyError(f"{RED}Error: level {level!r} unknown.{ENDCOL}")
 
             i += 1
 
 
         ### append last contig in list
         if args['fasta_file'] and contig:
             specific_contigs.append(f">{f_id}.contig{c_nb} (at position {contig_pos})\n{contig}")
@@ -323,27 +353,32 @@
                 mesg = f"{f_id}: no specific kmers found"
             return 'failed', mesg
 
         ### report
         if args['selection']:
             mesg = f"{given}: {item['symbol']}:{ENST} - kmers/contigs: {len(specific_kmers)}/{len(specific_contigs)} (level: {level})"
         else:
-            mesg = f"{f_id} (level: {level})"
+            mesg = f"{f_id} - kmers/contigs: {len(specific_kmers)}/{len(specific_contigs)} (level: {level})"
 
         return 'done', mesg
 
 
     def write(self, args, outfile, specific_seq, type):
         """ Write results as fasta file"""
         outdir = os.path.join(args['tmpdir'], type)
         os.makedirs(outdir, exist_ok=True)
         with open(os.path.join(outdir, outfile), 'w') as fh:
             fh.write("\n".join(specific_seq) + '\n')
 
 
+    def __revcomp(self, mer):
+        revcomp = lambda mer: ''.join([{'A':'T', 'C':'G', 'G':'C', 'T':'A'}[B] for B in mer][::-1])
+        return revcomp(mer)
+
+
 '''
 def handle_kmers(**kwargs):
     print("LOCALS():", locals())
     ## kmers case
     knb += 1
     specific_kmers.append(f">{given_up}:{given_up}.kmer{kmer_pos} ({isoforms_with_mer_nb}/{isoforms_nb})\n{mer}")
     ## contigs case
```

### Comparing `kmerator-0.7.7b0/kmerator/longest_transcript.py` & `kmerator-0.8.1b0/kmerator/longest_transcript.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.7b0/kmerator/mk_geneinfo.py` & `kmerator-0.8.1b0/kmerator/mk_geneinfo.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.7b0/kmerator/mk_transcriptome.py` & `kmerator-0.8.1b0/kmerator/mk_transcriptome.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.7b0/kmerator/options.py` & `kmerator-0.8.1b0/kmerator/options.py`

 * *Files identical despite different names*

### Comparing `kmerator-0.7.7b0/kmerator.egg-info/PKG-INFO` & `kmerator-0.8.1b0/kmerator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: kmerator
-Version: 0.7.7b0
+Version: 0.8.1b0
 Summary: Find specific gene or transcript kmers. And more.
 Home-page: https://github.com/Transipedia/kmerator
 Author: Sébastien RIQUIER, IRMB, Montpellier
 Author-email: sebastien.riquier@ucd.ie
 License: GPLv3
 Description: # Kmerator
         
         ## Prototype for decomposition of transcript or gene sequences and extraction of their specific k-mers
         
         ref: <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8221386/>
         
-        Kmerator is a prototype tool designed for the prediction of specific k-mers (also called tags) from input sequences, considering a reference genome and an ENSEMBL-like transcriptome. From these specific k-mers, it also outputs their corresponding specific contigs which are sequences of consecutive k-mers (overlapping length between k-mers must be k-1, otherwise, it's a new contig). Kmerator first uses Jellyfish [1] to create 2 requestable indexes from the reference genome and transcriptome, and second, decomposes your input transcript or gene sequences to count the occurences of each k-mer in the genome and transcriptome. Number of occurrences are then interpreted, in different manners, to select specific k-mer from your input. 
+        Kmerator is a prototype tool designed for the prediction of specific k-mers (also called tags) from input sequences, considering a reference genome and an ENSEMBL-like transcriptome. From these specific k-mers, it also outputs their corresponding specific contigs which are sequences of consecutive k-mers (overlapping length between k-mers must be k-1, otherwise, it's a new contig). You need to provide kmerator with a jellifsh index of the reference genome. Kmerator itself builds a jellyfish index of the reference transcriptome (by default the latest available version of Ensembl). It then  decomposes your input transcript or gene sequences to count the occurences of each k-mer in the genome and transcriptome. Number of occurrences are then interpreted, in different manners, to select specific k-mer from your input. 
         
         Before using kmerator, a jellyfish index of the reference genome must be created. kmerator automatically creates a dataset according to the species and the desired release number (by default, homo_sapiens and the latest version). The dataset is composed of 4 files per species/version: a jellyfish index of the modified transcriptome (cDNA + ncRNA - alternative chormosomes) from Ensembl, a binary file representing the same transcriptome, another binary file containing general information on the genes of the transcriptome and a report file.
         
         
         #### Specific kmers
         
         ![](https://github.com/Transipedia/kmerator/raw/main/img/specific-kmers.png)
@@ -49,15 +49,15 @@
         git clone https://github.com/Transipedia/kmerator3.git
         ln -s $PWD/kmerator3/kmerator/kmerator.py /usr/local/bin/kmerator  # or somewhere in your $PATH
         ```
         
         
         ## How to use kmerator
         
-        Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying. You can store and name the index file whatever you want.
+        Before all, remember that kmerator needs a jellyfish index of the genome. You must build it according to the species you are studying. You can store and name the index file whatever you want. Please note that you must **not use the jellyfish -C option** when building the reference genome index.
         
         ### Configuration file
         
         The arguments to run kmerator are numerous, so to reduce the number of arguments to enter, it is advisable to edit the configuration file with the command :
         
         ```
         kmerator -e
@@ -151,14 +151,16 @@
         ## References
         
         [1] Guillaume Marçais, Carl Kingsford, A fast, lock-free approach for efficient parallel counting of occurrences of k-mers, Bioinformatics, Volume 27, Issue 6, 15 March 2011, Pages 764–770, https://doi.org/10.1093/bioinformatics/btr011
         [2] Rodriguez JM, et al. Nucleic Acids Res. Database issue; 2017 Oct 23
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
-Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `kmerator-0.7.7b0/setup.py` & `kmerator-0.8.1b0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,21 @@
     description = info.SHORTDESC,
     long_description = open('README.md').read(),
     long_description_content_type = "text/markdown",
     url="https://github.com/Transipedia/kmerator",
     packages = setuptools.find_packages(),
     classifiers = [
         'Development Status :: 4 - Beta',
+        'Environment :: Console',
+        'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: POSIX :: Linux',
-        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
         'Natural Language :: English',
-        'Intended Audience :: Science/Research',
+        'Topic :: Scientific/Engineering :: Bio-Informatics',
     ],
     entry_points = {
         'console_scripts': [
             'kmerator = kmerator.kmerator:main',
         ],
     },
     include_package_data = True,
```

