# Comparing `tmp/FastaTransformer-0.0.10.tar.gz` & `tmp/FastaTransformer-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastaTransformer-0.0.10.tar", last modified: Thu Jun 15 16:40:55 2023, max compression
+gzip compressed data, was "FastaTransformer-0.0.11.tar", last modified: Thu Jun 15 18:11:40 2023, max compression
```

## Comparing `FastaTransformer-0.0.10.tar` & `FastaTransformer-0.0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:40:55.489181 FastaTransformer-0.0.10/
--rw-rw-rw-   0        0        0     4137 2023-06-15 16:40:55.489181 FastaTransformer-0.0.10/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2023-06-14 21:00:48.000000 FastaTransformer-0.0.10/README.md
--rw-rw-rw-   0        0        0      150 2023-05-30 20:49:19.000000 FastaTransformer-0.0.10/pyproject.toml
--rw-rw-rw-   0        0        0      707 2023-06-15 16:40:55.497181 FastaTransformer-0.0.10/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 16:40:55.444201 FastaTransformer-0.0.10/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 16:40:55.455181 FastaTransformer-0.0.10/src/CigarBreaker/
--rw-rw-rw-   0        0        0     6947 2023-05-31 15:39:29.000000 FastaTransformer-0.0.10/src/CigarBreaker/CigarBreaker.py
--rw-rw-rw-   0        0        0       27 2023-06-15 16:35:28.000000 FastaTransformer-0.0.10/src/CigarBreaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:40:55.460182 FastaTransformer-0.0.10/src/FastaTransformer/
--rw-rw-rw-   0        0        0    49409 2023-06-14 19:52:04.000000 FastaTransformer-0.0.10/src/FastaTransformer/FastaTransformer.py
--rw-rw-rw-   0        0        0       83 2023-06-13 14:33:15.000000 FastaTransformer-0.0.10/src/FastaTransformer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:40:55.487184 FastaTransformer-0.0.10/src/FastaTransformer.egg-info/
--rw-rw-rw-   0        0        0     4137 2023-06-15 16:40:55.000000 FastaTransformer-0.0.10/src/FastaTransformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-06-15 16:40:55.000000 FastaTransformer-0.0.10/src/FastaTransformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:40:55.000000 FastaTransformer-0.0.10/src/FastaTransformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-15 16:40:55.000000 FastaTransformer-0.0.10/src/FastaTransformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.884285 FastaTransformer-0.0.11/
+-rw-rw-rw-   0        0        0     4241 2023-06-15 18:11:40.885290 FastaTransformer-0.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     3672 2023-06-15 18:00:21.000000 FastaTransformer-0.0.11/README.md
+-rw-rw-rw-   0        0        0      150 2023-05-30 20:49:19.000000 FastaTransformer-0.0.11/pyproject.toml
+-rw-rw-rw-   0        0        0      729 2023-06-15 18:11:40.893304 FastaTransformer-0.0.11/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.846190 FastaTransformer-0.0.11/src/
+drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.855214 FastaTransformer-0.0.11/src/CigarBreaker/
+-rw-rw-rw-   0        0        0     7061 2023-06-15 17:45:36.000000 FastaTransformer-0.0.11/src/CigarBreaker/CigarBreaker.py
+-rw-rw-rw-   0        0        0       39 2023-06-15 16:53:41.000000 FastaTransformer-0.0.11/src/CigarBreaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.860225 FastaTransformer-0.0.11/src/FastaTransformer/
+-rw-rw-rw-   0        0        0    49409 2023-06-14 19:52:04.000000 FastaTransformer-0.0.11/src/FastaTransformer/FastaTransformer.py
+-rw-rw-rw-   0        0        0       99 2023-06-15 16:54:04.000000 FastaTransformer-0.0.11/src/FastaTransformer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.883282 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/
+-rw-rw-rw-   0        0        0     4241 2023-06-15 18:11:40.000000 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-06-15 18:11:40.000000 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 18:11:40.000000 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-15 18:11:40.000000 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/top_level.txt
```

### Comparing `FastaTransformer-0.0.10/PKG-INFO` & `FastaTransformer-0.0.11/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: FastaTransformer
-Version: 0.0.10
+Version: 0.0.11
 Summary: This package helps resolve bioprogramming problems
-Home-page: https://github.com/MichaelKim0407/tutorial-pip-package
+Home-page: https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Author: MDinhobl
 Author-email: markdinhobl@gmail.com
-Project-URL: Bug Tracker, https://github.com/MichaelKim0407/tutorial-pip-package
+Project-URL: Bug Tracker, https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FastaTransformer
 FastaTransformer is a python toolset containing fucntions to simplify the usage of .fasta files in analysis as well as transform them into useful states for other tools.
 
+### Authors
+
+The primary author of the FastaTransformer package is MDinhobl.
+
 ## Major Functions
 The following list contains the most useful functions of FastaTransformer.
 
 ### Creating Data Folders
 
 1. **MakeGeneBank** - Take a CSV or pandas Dataframe with columns representing Genomes, Gene (or other category), and Sequence and create a folder of .fasta files for each Gene (or chosen category).
 1. **GeneBankToAlignmentBank** - Uses [Muscle](https://www.drive5.com/muscle/) (must be installed locally) to transform a folder of .fasta files into a folder of matching alignment files.
```

### Comparing `FastaTransformer-0.0.10/README.md` & `FastaTransformer-0.0.11/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # FastaTransformer
 FastaTransformer is a python toolset containing fucntions to simplify the usage of .fasta files in analysis as well as transform them into useful states for other tools.
 
+### Authors
+
+The primary author of the FastaTransformer package is MDinhobl.
+
 ## Major Functions
 The following list contains the most useful functions of FastaTransformer.
 
 ### Creating Data Folders
 
 1. **MakeGeneBank** - Take a CSV or pandas Dataframe with columns representing Genomes, Gene (or other category), and Sequence and create a folder of .fasta files for each Gene (or chosen category).
 1. **GeneBankToAlignmentBank** - Uses [Muscle](https://www.drive5.com/muscle/) (must be installed locally) to transform a folder of .fasta files into a folder of matching alignment files.
```

### Comparing `FastaTransformer-0.0.10/setup.cfg` & `FastaTransformer-0.0.11/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2046 6173 7461 5472 616e 7366 6f72   = FastaTransfor
 00000020: 6d65 720d 0a76 6572 7369 6f6e 203d 2030  mer..version = 0
-00000030: 2e30 2e31 300d 0a61 7574 686f 7220 3d20  .0.10..author = 
+00000030: 2e30 2e31 310d 0a61 7574 686f 7220 3d20  .0.11..author = 
 00000040: 4d44 696e 686f 626c 0d0a 6175 7468 6f72  MDinhobl..author
 00000050: 5f65 6d61 696c 203d 206d 6172 6b64 696e  _email = markdin
 00000060: 686f 626c 4067 6d61 696c 2e63 6f6d 0d0a  hobl@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 00000080: 6973 2070 6163 6b61 6765 2068 656c 7073  is package helps
 00000090: 2072 6573 6f6c 7665 2062 696f 7072 6f67   resolve bioprog
 000000a0: 7261 6d6d 696e 6720 7072 6f62 6c65 6d73  ramming problems
 000000b0: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
 000000c0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
 000000d0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
 000000e0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
 000000f0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
 00000100: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
-00000110: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d69  ://github.com/Mi
-00000120: 6368 6165 6c4b 696d 3034 3037 2f74 7574  chaelKim0407/tut
-00000130: 6f72 6961 6c2d 7069 702d 7061 636b 6167  orial-pip-packag
-00000140: 650d 0a70 726f 6a65 6374 5f75 726c 7320  e..project_urls 
-00000150: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
-00000160: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000170: 622e 636f 6d2f 4d69 6368 6165 6c4b 696d  b.com/MichaelKim
-00000180: 3034 3037 2f74 7574 6f72 6961 6c2d 7069  0407/tutorial-pi
-00000190: 702d 7061 636b 6167 650d 0a63 6c61 7373  p-package..class
-000001a0: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
-000001b0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-000001c0: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
-000001d0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-000001e0: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-000001f0: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-00000200: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000210: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
-00000220: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000230: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-00000240: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-00000250: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000260: 7569 7265 7320 3d20 3e3d 332e 360d 0a0d  uires = >=3.6...
-00000270: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000280: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-00000290: 3d20 7372 630d 0a0d 0a5b 6567 675f 696e  = src....[egg_in
-000002a0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000002b0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000002c0: 0a0d 0a                                  ...
+00000110: 3a2f 2f67 6974 6875 622e 636f 6d2f 476c  ://github.com/Gl
+00000120: 6f62 616c 2d41 5346 562d 5265 7365 6172  obal-ASFV-Resear
+00000130: 6368 2d41 6c6c 6961 6e63 652f 4661 7374  ch-Alliance/Fast
+00000140: 6154 7261 6e73 666f 726d 6572 0d0a 7072  aTransformer..pr
+00000150: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
+00000160: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
+00000170: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000180: 2f47 6c6f 6261 6c2d 4153 4656 2d52 6573  /Global-ASFV-Res
+00000190: 6561 7263 682d 416c 6c69 616e 6365 2f46  earch-Alliance/F
+000001a0: 6173 7461 5472 616e 7366 6f72 6d65 720d  astaTransformer.
+000001b0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
+000001c0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000001d0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+000001e0: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
+000001f0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000200: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+00000210: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000220: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000230: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
+00000240: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+00000250: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
+00000260: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+00000270: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+00000280: 332e 360d 0a0d 0a5b 6f70 7469 6f6e 732e  3.6....[options.
+00000290: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+000002a0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+000002b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000002c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000002d0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `FastaTransformer-0.0.10/src/CigarBreaker/CigarBreaker.py` & `FastaTransformer-0.0.11/src/CigarBreaker/CigarBreaker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,58 @@
 #Imported TSV file
 def ImportTsv(tsv, nosubpositions = False):
     """
-    For understanding a tsv file see https://resources.qiagenbioinformatics.com/manuals/clcgenomicsworkbench/current/User_Manual.pdf, page 1119.
+    A program for importing tsv files into an understandable and usable format. For understanding a tsv file see https://resources.qiagenbioinformatics.com/manuals/clcgenomicsworkbench/current/User_Manual.pdf, page 1119.
+    
+    Parameters
+    ---
+    tsv : a string that is the path to a .tsv file.
+    
+    nosubpositions : Boolean, default False. If True will on select items without subpositions.
+    
+    Returns
+    ---
+    A pd.DataFrame
+    
     """
     import pandas as pd
     df = pd.read_csv(str(tsv), sep = '\t', names = ["RefName", "RefPosition", "RefSubPosition", "RefSymbol", "Num_A", "Num_C", "Num_G", "Num_T", "Num_N", "Num_Gap", "Total_Reads"])
     if nosubpositions == True:
         df[df['RefSubPosition'] == '-']
     return df
-    #in_file_tsv["AbsolutePosition"] = in_file_tsv.index
-    #in_file_tsv["AbsolutePosition"] += 1
     
 def CigarQualityConverter(string):
     """
-    Take a quality string, such as those featured in a .sam for .fastq file, and turns them into a numerical representation of quality.
+    Take a quality string, such as those featured in a .sam or .fastq file, and turn them into a numerical representation of quality.
+    
+    Parameters
+    ---
+    A quality string.
+    
+    Returns
+    ---
+    A list of quality scores.
+    
     """
     listOrd = []
     if string != "N/A":
         for character in string:
             listOrd.append(ord(character))
     else:
         listOrd == ["N/A"]
     return listOrd
 
 def CigarConverter(SamLine, consumes_read = "MIS=X", consumes_consensus = "MDN=X"):
+    
+    """
+    
+    """
+    
     import pandas as pd
     RefPositionList = []
-    #CigarList = []
     Sequence = ""
     Quality = ""
     ReadEaten = 0
     RefPositionStart = SamLine.pos
 
     CigarSequence = []
     CigarPosiiton = []
@@ -60,22 +82,15 @@
         else:
             RefPositionList.extend(cigar_length*[RefPositionStart])
             if len(CigarPosiiton) == 0:
                 CigarPosiiton.append(RefPositionStart)
             else:
                 CigarPosiiton.append(RefPositionStart-1)
 
-
-        #CigarList.extend(cigar_length*cigar_type)
-
-
         CigarType.append(cigar_type)
-        #CigarSequence.append(Sequence[-cigar_length:])
-        #CigarQuality.append(Quality[-cigar_length:])
-        #CigarPosiiton.append(RefPositionList[-cigar_length:])
         CigarLength.append(cigar_length)
 
     #CigarList
     df_cigar = pd.DataFrame()
     df_cigar['Type'] = CigarType
     df_cigar['Length'] = CigarLength
     df_cigar['Sequence'] = CigarSequence
```

### Comparing `FastaTransformer-0.0.10/src/FastaTransformer/FastaTransformer.py` & `FastaTransformer-0.0.11/src/FastaTransformer/FastaTransformer.py`

 * *Files identical despite different names*

### Comparing `FastaTransformer-0.0.10/src/FastaTransformer.egg-info/PKG-INFO` & `FastaTransformer-0.0.11/src/FastaTransformer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: FastaTransformer
-Version: 0.0.10
+Version: 0.0.11
 Summary: This package helps resolve bioprogramming problems
-Home-page: https://github.com/MichaelKim0407/tutorial-pip-package
+Home-page: https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Author: MDinhobl
 Author-email: markdinhobl@gmail.com
-Project-URL: Bug Tracker, https://github.com/MichaelKim0407/tutorial-pip-package
+Project-URL: Bug Tracker, https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # FastaTransformer
 FastaTransformer is a python toolset containing fucntions to simplify the usage of .fasta files in analysis as well as transform them into useful states for other tools.
 
+### Authors
+
+The primary author of the FastaTransformer package is MDinhobl.
+
 ## Major Functions
 The following list contains the most useful functions of FastaTransformer.
 
 ### Creating Data Folders
 
 1. **MakeGeneBank** - Take a CSV or pandas Dataframe with columns representing Genomes, Gene (or other category), and Sequence and create a folder of .fasta files for each Gene (or chosen category).
 1. **GeneBankToAlignmentBank** - Uses [Muscle](https://www.drive5.com/muscle/) (must be installed locally) to transform a folder of .fasta files into a folder of matching alignment files.
```

