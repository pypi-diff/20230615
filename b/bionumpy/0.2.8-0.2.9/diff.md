# Comparing `tmp/bionumpy-0.2.8.tar.gz` & `tmp/bionumpy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bionumpy-0.2.8.tar", last modified: Tue Dec  6 16:17:04 2022, max compression
+gzip compressed data, was "bionumpy-0.2.9.tar", last modified: Tue Dec 20 15:41:37 2022, max compression
```

## Comparing `bionumpy-0.2.8.tar` & `bionumpy-0.2.9.tar`

### file list

```diff
@@ -1,147 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.155853 bionumpy-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 16:16:24.000000 bionumpy-0.2.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-06 16:16:24.000000 bionumpy-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-06 16:16:24.000000 bionumpy-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2022-12-06 16:17:04.155853 bionumpy-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2022-12-06 16:16:24.000000 bionumpy-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.139854 bionumpy-0.2.8/bionumpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.139854 bionumpy-0.2.8/bionumpy/alignments/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/alignments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/alignments/cigar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.139854 bionumpy-0.2.8/bionumpy/arithmetics/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/arithmetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/arithmetics/bedgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/arithmetics/intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/arithmetics/similarity_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.143854 bionumpy-0.2.8/bionumpy/bnpdataclass/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/bnpdataclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/bnpdataclass/bnpdataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/bnpdataclass/bnpdataclassfunction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.143854 bionumpy-0.2.8/bionumpy/cupy_compatible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/cupy_compatible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/cupy_compatible/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.143854 bionumpy-0.2.8/bionumpy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/datatypes/gtf.py
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/encoded_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.143854 bionumpy-0.2.8/bionumpy/encodings/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/encodings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/encodings/_legacy_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/encodings/alphabet_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/encodings/base_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/encodings/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/encodings/kmer_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/encodings/vcf_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.147853 bionumpy-0.2.8/bionumpy/io/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/bam.py
--rw-r--r--   0 runner    (1001) docker     (123)    18977 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/delimited_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/dump_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10801 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/file_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/gfa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/indexed_fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/indexed_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/jaspar.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/matrix_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/motifs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/multiline_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/npdataclassreader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8505 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/io/strops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.147853 bionumpy-0.2.8/bionumpy/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/count_encoded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/genes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.147853 bionumpy-0.2.8/bionumpy/sequence/indexing/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/indexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/indexing/kmer_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/indexing/wildcard_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/kmers.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/minimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/position_weight_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/rollable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/string_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/sequence/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.147853 bionumpy-0.2.8/bionumpy/simulate/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/simulate/chipseq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/simulate/rnaseq.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/simulate/rng.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/simulate/sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.147853 bionumpy-0.2.8/bionumpy/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/streams/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/streams/groupby_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/streams/grouped.py
--rw-r--r--   0 runner    (1001) docker     (123)     9186 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/streams/multistream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/streams/reductions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/streams/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.151853 bionumpy-0.2.8/bionumpy/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/util/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/util/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.151853 bionumpy-0.2.8/bionumpy/variants/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/variants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2022-12-06 16:16:24.000000 bionumpy-0.2.8/bionumpy/variants/mutation_signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.139854 bionumpy-0.2.8/bionumpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2022-12-06 16:17:04.000000 bionumpy-0.2.8/bionumpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2022-12-06 16:17:04.000000 bionumpy-0.2.8/bionumpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 16:17:04.000000 bionumpy-0.2.8/bionumpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-06 16:17:04.000000 bionumpy-0.2.8/bionumpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 16:17:03.000000 bionumpy-0.2.8/bionumpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2022-12-06 16:17:04.000000 bionumpy-0.2.8/bionumpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-06 16:17:04.000000 bionumpy-0.2.8/bionumpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-06 16:17:04.155853 bionumpy-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2022-12-06 16:16:24.000000 bionumpy-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.155853 bionumpy-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/gfa_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 16:17:04.155853 bionumpy-0.2.8/tests/property_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/property_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/property_tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/property_tests/test_delimited_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/property_tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/property_tests/test_strops.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_bam.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_bionumpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_bnpdataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_chromosome_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_delimited_buffers.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_dna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_encoded_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_gtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_indexed_fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_io_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_kmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_kmer_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_kmer_nmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_minimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_multistream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_npdataclassstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_pileup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_position_weight_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_rollable.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_seqeunces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_similarity_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_streambroadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_string_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_strops.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_vcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_vcf_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2022-12-06 16:16:24.000000 bionumpy-0.2.8/tests/test_wildcard_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.965962 bionumpy-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:40:49.000000 bionumpy-0.2.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-20 15:40:49.000000 bionumpy-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-20 15:40:49.000000 bionumpy-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2022-12-20 15:41:37.965962 bionumpy-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2022-12-20 15:40:49.000000 bionumpy-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.949962 bionumpy-0.2.9/bionumpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.949962 bionumpy-0.2.9/bionumpy/alignments/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/alignments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/alignments/cigar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.949962 bionumpy-0.2.9/bionumpy/arithmetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/arithmetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/arithmetics/bedgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/arithmetics/global_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/arithmetics/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/arithmetics/similarity_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.949962 bionumpy-0.2.9/bionumpy/bnpdataclass/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/bnpdataclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/bnpdataclass/bnpdataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/bnpdataclass/bnpdataclassfunction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.949962 bionumpy-0.2.9/bionumpy/cupy_compatible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/cupy_compatible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/cupy_compatible/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.949962 bionumpy-0.2.9/bionumpy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/datatypes/gtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19166 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/encoded_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.953961 bionumpy-0.2.9/bionumpy/encodings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/encodings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/encodings/_legacy_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/encodings/alphabet_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/encodings/base_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/encodings/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/encodings/kmer_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/encodings/string_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/encodings/vcf_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.953961 bionumpy-0.2.9/bionumpy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/bam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/delimited_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/dump_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/file_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/gfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/indexed_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/indexed_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/jaspar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/matrix_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/motifs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/multiline_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/npdataclassreader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/io/strops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.953961 bionumpy-0.2.9/bionumpy/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/count_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/genes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.957961 bionumpy-0.2.9/bionumpy/sequence/indexing/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/indexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/indexing/kmer_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/indexing/wildcard_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/kmers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/minimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/position_weight_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/rollable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/string_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/sequence/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.957961 bionumpy-0.2.9/bionumpy/simulate/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/simulate/chipseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/simulate/rnaseq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/simulate/rng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/simulate/sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.957961 bionumpy-0.2.9/bionumpy/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/streams/chunk_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/streams/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/streams/groupby_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/streams/grouped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9186 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/streams/multistream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/streams/reductions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/streams/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.957961 bionumpy-0.2.9/bionumpy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/util/ascii_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/util/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/util/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.957961 bionumpy-0.2.9/bionumpy/variants/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/variants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2022-12-20 15:40:49.000000 bionumpy-0.2.9/bionumpy/variants/mutation_signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.949962 bionumpy-0.2.9/bionumpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2022-12-20 15:41:37.000000 bionumpy-0.2.9/bionumpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2022-12-20 15:41:37.000000 bionumpy-0.2.9/bionumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:41:37.000000 bionumpy-0.2.9/bionumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-20 15:41:37.000000 bionumpy-0.2.9/bionumpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:41:37.000000 bionumpy-0.2.9/bionumpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 15:41:37.000000 bionumpy-0.2.9/bionumpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-20 15:41:37.000000 bionumpy-0.2.9/bionumpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-20 15:41:37.965962 bionumpy-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2022-12-20 15:40:49.000000 bionumpy-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.961962 bionumpy-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/gfa_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.961962 bionumpy-0.2.9/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/performance/interval_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:41:37.965962 bionumpy-0.2.9/tests/property_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/property_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/property_tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/property_tests/test_delimited_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/property_tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/property_tests/test_strops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_asciihash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_bam.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_bionumpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_bnpdataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_chromosome_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_delimited_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_dna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_encoded_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_encodedarrayfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_entry_chunker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_global_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_gtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_indexed_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_io_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_kmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_kmer_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_kmer_nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_minimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_multistream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_npdataclassstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_pileup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_position_weight_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_rollable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_seqeunces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_similarity_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_streambroadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_string_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_string_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_strops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_vcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_vcf_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2022-12-20 15:40:49.000000 bionumpy-0.2.9/tests/test_wildcard_index.py
```

### Comparing `bionumpy-0.2.8/LICENSE` & `bionumpy-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/PKG-INFO` & `bionumpy-0.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bionumpy
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library for working with biological sequence data as numpy arrays.
 Home-page: https://github.com/knutdrand/bionumpy
 Author: Knut Rand
 Author-email: knutdrand@gmail.com
 License: MIT license
 Keywords: bionumpy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -29,33 +29,46 @@
         :target: https://github.com/bionumpy/bionumpy/actions/
         :alt: Build and test status
 
 .. image:: https://github.com/bionumpy/bionumpy-example-data/actions/workflows/run_checks.yml/badge.svg
         :target: https://github.com/bionumpy/bionumpy-example-data/actions/
         :alt: Testing on big data
 
+.. image:: https://github.com/bionumpy/bionumpy/actions/workflows/benchmarking.yml/badge.svg
+        :target: https://github.com/bionumpy/bionumpy/blob/benchmarks/benchmarks/report_small.md
+        :alt: Benchmarks
+
+
 Documentation: `https://bionumpy.github.io/bionumpy/ <https://bionumpy.github.io/bionumpy/>`_
 
 
 What is BioNumPy?
 -----------------
-BioNumPy is a toolkit, built on top of NumPy, for enabling array programming on biological data in Python. BioNumPy aims to make it easy to read common bioinformatics file formats efficiently into NumPy-like data structures that enable efficient operations and analysis of the data. Working in BioNumPy should feel much like working in NumPy.
-
-
-Why BioNumPy?
--------------
-* There are no existing packages in Python for getting biological datasets efficiently into NumPy-like data structures.
-* Current packages for working with biological data do not use NumPy in an efficient way (e.g. individual sequences are stored as separate NumPy arrays, not together in shared arrays).
+BioNumPy is a Python library, built on top of NumPy, for enabling array programming on biological datasets in Python.
+BioNumPy aims to make it easy to read common bioinformatics file formats efficiently into NumPy-like data structures
+that enable efficient operations and analysis of the data. Working in BioNumPy should feel much like working in NumPy.
 
 
 Getting started
 ----------------
 
 1. Install with pip:
 
 	$ pip install bionumpy
 
-2. Check out the tutorials and getting started guide in the `documentation <https://bionumpy.github.io/bionumpy/>`_.
+2. Import BioNumPy and read your data, e.g.:
+
+    >>> import bionumpy as bnp
+    >>> import numpy as np
+    >>> f = bnp.open("example_data/big.fq.gz")
+    >>> # chunk contains the sequences of reads and NumPy-functions can be used
+    >>> for chunk in f:
+    ...      print(np.sum(chunk.sequence == "G"))
+    53686
+
+Check out the getting started guide and various tutorials in the `documentation <https://bionumpy.github.io/bionumpy/>`_.
+
+
```

### Comparing `bionumpy-0.2.8/README.rst` & `bionumpy-0.2.9/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -9,30 +9,43 @@
         :target: https://github.com/bionumpy/bionumpy/actions/
         :alt: Build and test status
 
 .. image:: https://github.com/bionumpy/bionumpy-example-data/actions/workflows/run_checks.yml/badge.svg
         :target: https://github.com/bionumpy/bionumpy-example-data/actions/
         :alt: Testing on big data
 
+.. image:: https://github.com/bionumpy/bionumpy/actions/workflows/benchmarking.yml/badge.svg
+        :target: https://github.com/bionumpy/bionumpy/blob/benchmarks/benchmarks/report_small.md
+        :alt: Benchmarks
+
+
 Documentation: `https://bionumpy.github.io/bionumpy/ <https://bionumpy.github.io/bionumpy/>`_
 
 
 What is BioNumPy?
 -----------------
-BioNumPy is a toolkit, built on top of NumPy, for enabling array programming on biological data in Python. BioNumPy aims to make it easy to read common bioinformatics file formats efficiently into NumPy-like data structures that enable efficient operations and analysis of the data. Working in BioNumPy should feel much like working in NumPy.
-
-
-Why BioNumPy?
--------------
-* There are no existing packages in Python for getting biological datasets efficiently into NumPy-like data structures.
-* Current packages for working with biological data do not use NumPy in an efficient way (e.g. individual sequences are stored as separate NumPy arrays, not together in shared arrays).
+BioNumPy is a Python library, built on top of NumPy, for enabling array programming on biological datasets in Python.
+BioNumPy aims to make it easy to read common bioinformatics file formats efficiently into NumPy-like data structures
+that enable efficient operations and analysis of the data. Working in BioNumPy should feel much like working in NumPy.
 
 
 Getting started
 ----------------
 
 1. Install with pip:
 
 	$ pip install bionumpy
 
-2. Check out the tutorials and getting started guide in the `documentation <https://bionumpy.github.io/bionumpy/>`_.
+2. Import BioNumPy and read your data, e.g.:
+
+    >>> import bionumpy as bnp
+    >>> import numpy as np
+    >>> f = bnp.open("example_data/big.fq.gz")
+    >>> # chunk contains the sequences of reads and NumPy-functions can be used
+    >>> for chunk in f:
+    ...      print(np.sum(chunk.sequence == "G"))
+    53686
+
+Check out the getting started guide and various tutorials in the `documentation <https://bionumpy.github.io/bionumpy/>`_.
+
+
```

### Comparing `bionumpy-0.2.8/bionumpy/__init__.py` & `bionumpy-0.2.9/bionumpy/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Top-level package for bionumpy."""
 
 __author__ = """Knut Rand"""
 __email__ = "knutdrand@gmail.com"
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 import npstructures as nps
 
 from .io import (count_entries, open_indexed, MultiLineFastaBuffer, bnp_open,
-                 TwoLineFastaBuffer, FastQBuffer,
+                 TwoLineFastaBuffer, FastQBuffer, Bed6Buffer,
                  BedBuffer, VCFBuffer, PhasedVCFMatrixBuffer, VCFMatrixBuffer,
                  GfaSequenceBuffer, get_bufferclass_for_datatype)
 from .encodings.alphabet_encoding import (DNAEncoding, RNAENcoding, AminoAcidEncoding)
 from .encoded_array import EncodedArray, EncodedRaggedArray, as_encoded_array, OneToOneEncoding, BaseEncoding, change_encoding
 from .sequence import (get_kmers, get_minimizers, get_motif_scores, count_encoded)
 from .streams import mean, bincount, histogram, streamable, quantile, MultiStream, groupby
 from .datatypes import SAMEntry, GFFEntry, Bed6
 from .io.strops import str_equal
+from .util.cli import run_as_commandline
 from . import simulate
 from . import arithmetics
 open = bnp_open
 
 
 SAMBuffer = get_bufferclass_for_datatype(SAMEntry)
 GFFBuffer = get_bufferclass_for_datatype(GFFEntry)
-Bed6Buffer = get_bufferclass_for_datatype(Bed6)
+# Bed6Buffer = get_bufferclass_for_datatype(Bed6)
 
 __all__ = ["EncodedArray", "EncodedRaggedArray",
            "KmerEncoder", "Minimizers", "PositionWeightMatrix", "mean",
            "bincount", "streamable", "histogram", "count_entries", "quantile",
            "BedBuffer", "VCFBuffer", "PhasedVCFMatrixBuffer", "VCFMatrixBuffer",
            "GfaSequenceBuffer",
            "TwoLineFastaBuffer", "FastQBuffer", "open_indexed", "groupby",
```

### Comparing `bionumpy-0.2.8/bionumpy/alignments/__init__.py` & `bionumpy-0.2.9/bionumpy/alignments/__init__.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/alignments/cigar.py` & `bionumpy-0.2.9/bionumpy/alignments/cigar.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/arithmetics/bedgraph.py` & `bionumpy-0.2.9/bionumpy/arithmetics/bedgraph.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/arithmetics/intervals.py` & `bionumpy-0.2.9/bionumpy/arithmetics/intervals.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,105 @@
 from typing import List
+from numbers import Number
+import numpy.typing as npt
 import dataclasses
 from operator import itemgetter
 import numpy as np
 from npstructures import RunLength2dArray, RunLengthArray
-
+from bionumpy.encodings.string_encodings import StringEncoding
 from .bedgraph import BedGraph
 from .. import streamable
 from ..streams.grouped import chromosome_map
 from ..datatypes import Interval
 from ..bnpdataclass import bnpdataclass
+from ..util import interleave
+
+
+class GenomicRunLengthArray(RunLengthArray):
+    def to_array(self) -> np.ndarray:
+        """Convert the runlength array to a normal numpy array
+
+        Returns
+        -------
+        np.ndarray
+        """
+        if len(self) == 0:
+            return np.empty_like(self._values, shape=(0,))
+        values = np.asarray(self._values)
+        if values.dtype == np.float64:
+            values = values.view(np.uint64)
+        elif values.dtype == np.float32:
+            values = values.view(np.uint32)
+        elif values.dtype == np.float16:
+            values = values.view(np.uint16)
+        array = np.zeros_like(values, shape=len(self))
+        op = np.logical_xor if array.dtype == bool else np.bitwise_xor
+        diffs = op(values[:-1], values[1:])
+        array[self._starts[1:]] = diffs
+        array[self._starts[0]] = values[0]
+        op.accumulate(array, out=array)
+        return array.view(self._values.dtype)
+
+    @classmethod
+    def from_intervals(cls, starts: npt.ArrayLike, ends: npt.ArrayLike, size: int, values: npt.ArrayLike = True, default_value=0) -> 'GenomicRunLengthArray':
+        """Constuct a runlength array from a set of intervals and values
+
+        Parameters
+        ----------
+        starts : ArrayLike
+        ends : ArrayLike
+        size : int
+        values : ArrayLike
+        default_value :
+
+        Returns
+        -------
+        'RunLengthArray'
+        """
+        
+        assert np.all(ends > starts)
+        assert np.all(starts[1:] > ends[:-1])
+        prefix = [0] if (len(starts) == 0 or starts[0] != 0) else []
+        postfix = [size] if (len(ends) == 0 or ends[-1] != size) else []
+
+        events = np.empty(len(prefix) + len(postfix) + starts.size + ends.size, dtype=int)
+        if len(prefix):
+            events[0] = prefix[0]
+        if len(postfix):
+            events[len(prefix):-1:2] = starts
+            events[len(prefix)+1:-1:2] = ends
+            events[-1] = postfix[0]
+        else:
+            events[len(prefix)::2] = starts
+            events[len(prefix)+1::2] = ends
+
+        tmp = values
+        if isinstance(values, Number):
+            values = np.empty(2*(events.size//2+1), dtype=np.array(values).dtype)
+            values[::2] = default_value
+            values[1::2] = tmp
+        else:
+            values = interleave([np.broadcast(default_value, values.shape), values])
+            if ends[-1] != size:
+                values = np.append(values, default_value)
+
+        if (len(starts) > 0) and (starts[0] == 0):
+            values = values[1:]
+
+        values = values[:(len(events)-1)]
+        return cls(events, values, do_clean=True)
 
 
 @bnpdataclass
 class RawInterval:
     start: int
     stop: int
 
 
-def get_pileup(intervals: Interval, chromosome_size: int) -> RunLengthArray:
+def get_pileup(intervals: Interval, chromosome_size: int) -> GenomicRunLengthArray:
     """Get the number of intervals that overlap each position of the chromosome/contig
 
     This uses run length encoded arrays to handle the sparse data that
     we get from intervals.
 
     Parameters
     ----------
@@ -90,18 +168,18 @@
     [0 0 0 1 1 1 1 1 0 1 1 1 1 1 1 0 0 0 0 0]
 
     Find wether some positions overlap the mask:
     >>> print(other_mask[intervals.start])
     [False False  True]
     """
     assert np.all(intervals.stop <= chromosome_size), (np.max(intervals.stop), chromosome_size)
-    rla = RunLength2dArray.from_intervals(intervals.start,
-                                          intervals.stop,
-                                          chromosome_size)
-    return rla.any(axis=0)
+    if len(intervals) == 0:
+        return GenomicRunLengthArray.from_intervals(np.array([], dtype=int), np.array([], dtype=int), int(chromosome_size), default_value=False)
+    merged = merge_intervals(intervals[np.argsort(intervals.start)])
+    return GenomicRunLengthArray.from_intervals(merged.start, merged.stop, size=chromosome_size, default_value=False)
 
 
 def human_key_func(chrom_name):
     assert chrom_name.startswith("chr"), chrom_name
     parts = chrom_name[3:].split("_", maxsplit=1)
     assert len(parts) <= 2, chrom_name
     is_numeric = 1-parts[0].isdigit()
@@ -120,14 +198,18 @@
 
     Returns
     -------
     Interval
         Sorted intervals
 
     """
+    if isinstance(intervals.chromosome.encoding, StringEncoding):
+        args = np.lexsort((intervals.start, intervals.chromosome))
+        return intervals[args]
+
     if sort_order is not None:
         chromosome_key_function = {name: i for i, name in enumerate(sort_order)}.__getitem__
     s = sorted((chromosome_key_function(interval.chromosome.to_string()), interval.start, interval.stop, i)
                for i, interval in enumerate(intervals))
     indices = list(map(itemgetter(-1), s))
     return intervals[indices]
 
@@ -153,15 +235,15 @@
 
     """
 
     assert np.all(intervals.start[:-1] <= intervals.start[1:]), "merge_intervals requires intervals sorted on start position"
     stops = np.maximum.accumulate(intervals.stop)
     if distance > 0:
         stops += distance
-    valid_start_mask = intervals.start[1:] > intervals[:-1].stop
+    valid_start_mask = intervals.start[1:] > stops[:-1] # intervals[:-1].stop
     start_mask = np.concatenate(([True], valid_start_mask))
     stop_mask = np.concatenate((valid_start_mask, [True]))
     new_interval = intervals[start_mask]
     new_interval.stop = stops[stop_mask]
     if distance > 0:
         new_interval.stop -= distance
     return new_interval
@@ -182,14 +264,32 @@
     all_intervals = all_intervals[np.argsort(all_intervals.start, kind="mergesort")]
     stops = np.sort(all_intervals.stop, kind="mergesort")
     mask = stops[:-1] > all_intervals.start[1:]
     result = all_intervals[1:][mask]
     result.stop = stops[:-1][mask]
     return result
 
+
+@streamable()
+def global_intersect(intervals_b, intervals_a):
+    all_intervals = np.concatenate([intervals_a, intervals_b])
+    all_intervals = all_intervals[np.lexsort((all_intervals.start, all_intervals.chromosome))]
+    stops = all_intervals.stop[np.lexsort((all_intervals.stop, all_intervals.chromosome))]
+    mask = stops[:-1] > all_intervals.start[1:]
+    result = all_intervals[1:][mask]
+    result.stop = stops[:-1][mask]
+    return result
+
+
+def unique_intersect(intervals_a, intervals_b, genome_size):
+    genome_mask = get_boolean_mask(intervals_b, genome_size)
+    entry_mask = genome_mask[intervals_a].any(axis=-1)
+    return intervals_a[entry_mask]
+
+
 @chromosome_map()
 def extend(intervals, both=None, forward=None, reverse=None, left=None, right=None):
     directed = (forward is not None) or (reverse is not None)
     undirected = (left is not None) or (right is not None)
     assert sum([both is not None, directed, undirected]) == 1
     if both is not None:
         return dataclasses.replace(intervals,
```

### Comparing `bionumpy-0.2.8/bionumpy/arithmetics/similarity_measures.py` & `bionumpy-0.2.9/bionumpy/arithmetics/similarity_measures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from .intervals import get_boolean_mask
-from ..streams import MultiStream, streamable
+from ..streams import MultiStream, streamable, BnpStream
 import numpy as np
 from ..datatypes import ChromosomeSize, Interval
 
+
 @streamable(sum)
 def get_contingency_table(intervals_a, intervals_b, sequence_length):
     boolean_a = get_boolean_mask(intervals_a, sequence_length)
+    not_a = ~boolean_a
     boolean_b = get_boolean_mask(intervals_b, sequence_length)
-    return np.array([[np.sum(boolean_a & boolean_b), np.sum(boolean_a & ~boolean_b)],
-                     [np.sum(~boolean_a & boolean_b), np.sum(~boolean_a & ~boolean_b)]])
+    not_b = ~boolean_b
+    return np.array([[np.sum(boolean_a & boolean_b), np.sum(boolean_a & not_b)],
+                     [np.sum(not_a & boolean_b), np.sum(not_a & not_b)]])
 
 
 def forbes(chromosome_sizes: ChromosomeSize, intervals_a: Interval, intervals_b: Interval) -> float:
     """Computes the Forbes similarity index for two sets of intervals.
 
     Parameters
     ----------
```

### Comparing `bionumpy-0.2.8/bionumpy/bnpdataclass/bnpdataclass.py` & `bionumpy-0.2.9/bionumpy/bnpdataclass/bnpdataclass.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/bnpdataclass/bnpdataclassfunction.py` & `bionumpy-0.2.9/bionumpy/bnpdataclass/bnpdataclassfunction.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/datatypes/__init__.py` & `bionumpy-0.2.9/bionumpy/datatypes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     start: int
     stop: int
 
 
 @bnpdataclass
 class Bed6(Interval):
     name: str
-    score: int
+    score: str
     strand: StrandEncoding
 
 
 @bnpdataclass
 class NarrowPeak(Bed6):
     signal_value: str
     p_value: float
@@ -160,8 +160,7 @@
 
 
 @bnpdataclass
 class GfaPath:
     name: str
     node_ids: List[int]
     directions: List[int]
-
```

### Comparing `bionumpy-0.2.8/bionumpy/datatypes/gtf.py` & `bionumpy-0.2.9/bionumpy/datatypes/gtf.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/encoded_array.py` & `bionumpy-0.2.9/bionumpy/encoded_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         data = self.encode(s.ravel())
         if isinstance(data, EncodedArray):
             return EncodedRaggedArray(data, s._shape)
 
         return RaggedArray(data, s._shape)
 
     def _encode_string(self, string: str):
-        s = EncodedArray([ord(c) for c in string], BaseEncoding)
+        s = EncodedArray(np.frombuffer(bytes(string, encoding="ascii"), dtype=np.uint8), BaseEncoding)
         s = self._encode_base_encoded_array(s)
         return s
 
     def _encode_base_encoded_array(self, encoded_array):
         assert encoded_array.encoding.is_base_encoding()
         encoded_array = self._encode(encoded_array.data)
         if self.is_numeric():
@@ -236,14 +236,16 @@
     def __len__(self) -> int:
         return len(self.data)
 
     def raw(self) -> np.ndarray:
         return self.data.view(np.ndarray)
 
     def to_string(self) -> str:
+        if not self.encoding.is_one_to_one_encoding():
+            return self.encoding.to_string(self.data)
         if hasattr(self.encoding, "_decode"):
             # new system, can be used in all cases after refactoring
             data = self
             return "".join([chr(c) for c in self.encoding.decode(data).raw()])
         else:
             data = self.data
             return "".join([chr(c) for c in self.encoding.decode(data)])
@@ -292,17 +294,17 @@
             if n_dims == 0:
                 return self.encoding.to_string(self.data)
             elif n_dims == 1:
                 data_to_show = data_to_show[0:20]
             elif n_dims == 2:
                 # show first columns and rows
                 #raise NotImplemented("Str for n_dims=2 not implemented")
-                return self.encoding.to_string(self.data)[0:40] + "..."
+                return self.encoding.to_string(self.data[0:10, 0:10]) + "...."
                 # data_to_show = None
-            text = "[" + ", ".join(self.encoding.to_string(e) for e in data_to_show) + "]"
+            text = "[" + ", ".join(self.encoding.to_string(e).strip() for e in data_to_show) + "]"
             return text
 
         else:
             data = self.data
             if hasattr(self.encoding, "_decode"):
                 data = self  # todo: Default after encoding refactoring
                 text = self.encoding.decode(data).raw()
@@ -387,14 +389,21 @@
             return self.__class__(func([e.data for e in args[0]]), self.encoding)
         if func == np.where:
             return self.__class__(func(args[0], args[1].data, args[2].data), encoding = self.encoding)
         if func == np.zeros_like:
             return self.__class__(func(args[0].data, *args[1:], **kwargs), encoding=self.encoding)
         if func == np.append:
             return self.__class__(func(args[0].data, args[1].data, *args[2:], **kwargs), encoding=self.encoding)
+        if func == np.lexsort:
+            if not all(issubclass(t, (EncodedArray, np.ndarray)) for t in types):
+                return NotImplemented
+
+            args = [a.raw() if isinstance(a, EncodedArray) else np.asarray(a) for a in args[0]]
+            return func(args, *kwargs)
+
         if func == np.insert:
             return self.__class__(func(args[0].data, args[1], args[2].data, *args[3:], **kwargs), encoding = self.encoding)
         elif func in (np.lib.stride_tricks.sliding_window_view, np.lib.stride_tricks.as_strided):
             return self.__class__(func(args[0].data, *args[1:], **kwargs), self.encoding)
         
         return NotImplemented
         return super().__array_function__(func, types, args, kwargs)
@@ -412,15 +421,15 @@
         """
         assert isinstance(self.data, np.ndarray) and not np.issubdtype(self.data.dtype, np.object_)
         return self.__class__(np.lib.stride_tricks.as_strided(self.data, *args, **kwargs), self.encoding)
 
 
 def _parse_ufunc_inputs(inputs, target_encoding):
     for a in inputs:
-        assert isinstance(a, (str, list, EncodedArray, EncodedRaggedArray)), repr(a)
+        assert isinstance(a, (str, list, EncodedArray, EncodedRaggedArray)), "%s is not str, list, EncodedArray or EncodedRaggedArray" % type(a)
         if isinstance(a, str):
             a = target_encoding.encode(a)
         elif isinstance(a, list):
             a = target_encoding.encode(a)
         else:
             # already encoded
             pass
```

### Comparing `bionumpy-0.2.8/bionumpy/encodings/__init__.py` & `bionumpy-0.2.9/bionumpy/encodings/__init__.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/encodings/_legacy_encodings.py` & `bionumpy-0.2.9/bionumpy/encodings/_legacy_encodings.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/encodings/alphabet_encoding.py` & `bionumpy-0.2.9/bionumpy/encodings/alphabet_encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,19 @@
         self._mask[lower_alphabet] = True
         self._is_initialized = True
 
     def _encode(self, byte_array):
         self._initialize()
         ret = self._lookup[byte_array]
         if np.any(ret == 255):
-            offset = np.flatnonzero(ret==255)[0]
-            raise EncodingError(f"Error when encoding {''.join(chr(c) for c in byte_array[0:100])} "
+            offset = np.flatnonzero(ret.ravel()==255)[0]
+            tmp = [chr(c) for c in byte_array.ravel()[ret.ravel()==255]]
+            raise EncodingError(f"Error when encoding {''.join(chr(c) for c in byte_array.ravel()[0:100])} "
                                 f"to {self.__class__.__name__}. Invalid character(s): "
-                                f"{[chr(c) for c in byte_array[ret==255]]}", offset)
+                                f"{tmp}", offset)
         return ret
 
     def _decode(self, encoded):
         self._initialize()
         return self._alphabet[np.asarray(encoded)]
 
     @property
```

### Comparing `bionumpy-0.2.8/bionumpy/encodings/kmer_encodings.py` & `bionumpy-0.2.9/bionumpy/encodings/kmer_encodings.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/encodings/vcf_encoding.py` & `bionumpy-0.2.9/bionumpy/encodings/vcf_encoding.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 
 import numpy as np
 from bionumpy.encodings import Encoding
 
 
-class GenotypeRowEncoding(Encoding):
+class _GenotypeRowEncoding(Encoding):
     """
     Encoding for a row of genotype data in VCF-format.
     Supports phased and unphased genotypes and missing genotypes on the format ./.
 
     Does only support biallelic and triallelic variants.
     """
 
@@ -22,88 +22,93 @@
     _alphabet_lookup[_reverse_alphabet_lookup] = np.arange(len(_reverse_alphabet_lookup))
     _genotypes = list(itertools.product(_alleles, _seperators, _alleles))
     _alphabet_size = len(_alphabet)
 
     def get_labels(self):
         pass
 
-    @classmethod
-    def decode_lookup(cls):
+    def decode_lookup(self):
         _genotype_lookup = [
-            sum([len(cls._alphabet) ** (2 - i) * cls._alphabet_lookup[ord(g)] for i, g in enumerate(genotype)])
-            for genotype in cls._genotypes
+            sum([len(self._alphabet) ** (2 - i) * self._alphabet_lookup[ord(g)] for i, g in enumerate(genotype)])
+            for genotype in self._genotypes
         ]
         _reverse_genotype_lookup = np.zeros((256, 4), dtype=np.uint8)
         _reverse_genotype_lookup[_genotype_lookup] = np.array([
-            [ord(g) for g in genotype] + [ord("\t")] for genotype in cls._genotypes
+            [ord(g) for g in genotype] + [ord("\t")] for genotype in self._genotypes
         ])
 
         return _reverse_genotype_lookup
 
-    @classmethod
-    def encode(cls, genotype_rows):
-        data = cls._preprocess_data_for_encoding(genotype_rows)
+    def encode(self, genotype_rows):
+        data = self._preprocess_data_for_encoding(genotype_rows)
         n_rows = len(genotype_rows)
         encoded = \
-            cls._alphabet_size**2 * cls._alphabet_lookup[data[:, 0].raw()] + \
-            cls._alphabet_size ** 1 * cls._alphabet_lookup[data[:, 1].raw()] + \
-            cls._alphabet_size ** 0 * cls._alphabet_lookup[data[:, 2].raw()]
+            self._alphabet_size**2 * self._alphabet_lookup[data[:, 0].raw()] + \
+            self._alphabet_size ** 1 * self._alphabet_lookup[data[:, 1].raw()] + \
+            self._alphabet_size ** 0 * self._alphabet_lookup[data[:, 2].raw()]
 
         encoded = encoded.reshape(n_rows, len(encoded)//n_rows).astype(np.int8)
         return encoded
 
-    @classmethod
-    def _preprocess_data_for_encoding(cls, genotype_rows):
+    def _preprocess_data_for_encoding(self, genotype_rows):
         # split the row of genotype data
         from ..io.strops import split, replace_inplace
-        data = genotype_rows
+        data = genotype_rows.ravel()
         # hack because the row sometime ends with \n and sometimes with \t
         replace_inplace(data, "\n", "\t")
-        data = split(data.ravel(), "\t")[:-1, 0:3]  # don't include last element which is empty
-        return data
+        indices = np.flatnonzero(data == "\t")
+        indices = np.insert(indices, 0, -1)
+        return data[indices[:-1, np.newaxis] + np.array([1, 2, 3])]
+        #data = split(data.ravel(), "\t")[:-1, 0:3]  # don't include last element which is empty
+        #return data
 
-    @classmethod
-    def decode(cls, genotype):
+    def decode(self, genotype):
         if len(genotype.shape) == 0:
-            return cls.decode_lookup()[genotype]
+            return self.decode_lookup()[genotype]
 
         new_shape = genotype.shape[:-1] + (4*genotype.shape[-1],)
         if not isinstance(genotype, np.ndarray):
             genotype = genotype.raw()
-        decoded = cls.decode_lookup()[genotype].reshape(new_shape)# genotype.shape[0], genotype.shape[1]*4)
+        decoded = self.decode_lookup()[genotype].reshape(new_shape)# genotype.shape[0], genotype.shape[1]*4)
         # remove last tab
         return decoded[..., :-1]
 
-    @classmethod
-    def to_string(cls, e):
+    def to_string(self, e):
         if isinstance(e, np.ndarray):
             e = np.atleast_1d(e)
 
         if len(e.shape) == 2:
-            return '\n'.join(cls.to_string(c) for c in e)
+            return '\n'.join(self.to_string(c) for c in e)
 
-        return ''.join(chr(c) for c in cls.decode(e))
+        return ''.join(chr(c) for c in self.decode(e))
 
+    def __repr__(self):
+        return "GenotypeRowEncoding"
 
-class PhasedGenotypeRowEncoding(GenotypeRowEncoding):
+class _PhasedGenotypeRowEncoding(_GenotypeRowEncoding):
     """Encoding that can be used when all records are phased
      and there is no missing data, i.e. every genotype is
      either 0|0, 0|1, 1|0 or 1|1.
 
      Does only support biallelic variants.
     """
 
     genotypes = ["0|0", "0|1", "1|0", "1|1"]
 
-    @classmethod
-    def decode_lookup(cls):
+    def decode_lookup(self):
         return np.array([
             [ord(c) for c in genotype] + [ord("\t")]
-            for genotype in cls.genotypes], dtype=np.uint8)
+            for genotype in self.genotypes], dtype=np.uint8)
 
-    @classmethod
-    def encode(cls, genotype_rows):
-        data = cls._preprocess_data_for_encoding(genotype_rows)
+    def encode(self, genotype_rows):
+        data = self._preprocess_data_for_encoding(genotype_rows)
         n_rows = len(genotype_rows)
         encoded = (data[:, 0] == "1") * 2 + (data[:, 2] == "1")
         encoded = encoded.reshape(n_rows, len(encoded)//n_rows).astype(np.int8)
         return encoded
+
+    def __repr__(self):
+        return "PhasedGenotypeRowEncoding"
+
+
+PhasedGenotypeRowEncoding = _PhasedGenotypeRowEncoding()
+GenotypeRowEncoding = _GenotypeRowEncoding()
```

### Comparing `bionumpy-0.2.8/bionumpy/io/bam.py` & `bionumpy-0.2.9/bionumpy/io/bam.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/io/delimited_buffers.py` & `bionumpy-0.2.9/bionumpy/io/delimited_buffers.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from ..bnpdataclass import bnpdataclass, BNPDataClass
 from ..datatypes import (Interval, VCFGenotypeEntry,
                          SequenceEntry, VCFEntry, Bed12, Bed6,
                          GFFEntry, SAMEntry, ChromosomeSize, NarrowPeak, PhasedVCFGenotypeEntry,
                          GfaPath)
 from ..encoded_array import EncodedArray, EncodedRaggedArray
 from ..encoded_array import as_encoded_array
-from ..encodings import (Encoding, DigitEncoding)
+from ..encodings import Encoding
 from ..encodings.exceptions import EncodingError
 from ..encodings.vcf_encoding import GenotypeRowEncoding, PhasedGenotypeRowEncoding
-from ..encodings.alphabet_encoding import get_alphabet_encodings
+from ..encodings.alphabet_encoding import get_alphabet_encodings, DigitEncoding
 from ..encoded_array import get_base_encodings, BaseEncoding
 from ..util import is_subclass_or_instance
 from .file_buffers import FileBuffer, NEWLINE
 from .strops import (
     ints_to_strings, split, str_to_int, str_to_float,
     int_lists_to_strings, float_to_strings)
 from .dump_csv import dump_csv
@@ -448,23 +448,50 @@
     DatatypeBuffer.__qualname__ = _dataclass.__qualname__ + "Buffer"
     return DatatypeBuffer
 
 
 class BedBuffer(DelimitedBuffer):
     dataclass = Interval
 
+    def get_integers(self, cols: list) -> np.ndarray:
+        """Get integers from integer string
 
-class Bed12Buffer(DelimitedBuffer):
-    dataclass = Bed12
+        Extract integers from the specified columns
 
+        Parameters
+        ----------
+        cols : list
+            list of columns containing integers
 
-class Bed6Buffer(DelimitedBuffer):
+        """
+        assert np.all(cols < self._n_cols), (str(self._data), cols, self._n_cols)
+        cols = np.asanyarray(cols)
+        integer_starts = self._delimiters[:-1].reshape(-1, self._n_cols)[:, cols] + 1
+        integer_ends = self._delimiters[1:].reshape(-1, self._n_cols)[:, cols]
+        array = self._move_intervals_to_2d_array(integer_starts, integer_ends, fill_value='0')
+        try:
+            digits = as_encoded_array(array, DigitEncoding).raw()
+        except EncodingError as e:
+            row_number = e.offset//array.shape[-1]#  rows._shape.starts, e.offset, side="right")-1
+            raise FormatException(e.args[0], line_number=row_number)
+        powers = 10**np.arange(digits.shape[-1])[::-1]
+        return digits.dot(powers).reshape(-1, cols.size)
+        #integers = self._extract_integers(integer_starts.ravel(), integer_ends.ravel())
+        #return integers.reshape(-1, cols.size)
+
+
+class Bed6Buffer(BedBuffer):
     dataclass = Bed6
 
 
+class Bed12Buffer(Bed6Buffer):
+    dataclass = Bed12
+
+
+
 class VCFBuffer(DelimitedBuffer):
     dataclass = VCFEntry
 
     def get_data(self):
         data = super().get_data()
         data.position -= 1
         return data
@@ -492,15 +519,15 @@
         if prev_line is None:
             return []
 
         sample_names = prev_line.split("\t")[9:]
         return sample_names
 
     def get_data(self):
-        data = VCFBuffer.get_data(self)
+        data = super().get_data()
         genotypes = self.get_column_range_as_text(9, self._n_cols, keep_sep=True)
         genotypes = EncodedArray(self.genotype_encoding.encode(genotypes), self.genotype_encoding)
         return self.genotype_dataclass(*data.shallow_tuple(), genotypes)
 
 
 class PhasedVCFMatrixBuffer(VCFMatrixBuffer):
     dataclass = VCFEntry
```

### Comparing `bionumpy-0.2.8/bionumpy/io/dump_csv.py` & `bionumpy-0.2.9/bionumpy/io/dump_csv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,63 @@
 import numpy as np
 from numpy.typing import ArrayLike
 from typing import List, Dict, Tuple
 from .strops import ints_to_strings, int_lists_to_strings, float_to_strings
 from ..encoded_array import EncodedArray, Encoding, EncodedRaggedArray, BaseEncoding
+from ..encodings.string_encodings import StringEncoding
 from npstructures import RaggedArray
 from ..util import is_subclass_or_instance
 
 
+def str_func(column):
+    if column.encoding == BaseEncoding:
+        return column
+    elif isinstance(column.encoding, StringEncoding):
+        return column.encoding.decode(column)
+    assert False
+
 def dump_csv(data_dict: List[Tuple], sep: str = "\t") -> EncodedArray:
     """Put each field of the dataclass into a column in a buffer.
 
     Parameters
     data : bnpdataclass
         Data
     """
 
     funcs = {int: ints_to_strings,
-             str: lambda x: x,
+             str: str_func,  #lambda x: x,
              List[int]: int_lists_to_strings,
              float: float_to_strings,
              List[bool]: lambda x: int_lists_to_strings(x.astype(int), sep="")
              }
 
     def get_func_for_datatype(datatype):
         if is_subclass_or_instance(datatype, Encoding):
             encoding = datatype
 
             def dynamic(x):
                 if isinstance(x, EncodedRaggedArray):
-                    # print(repr(x.ravel()))
                     return EncodedRaggedArray(EncodedArray(encoding.decode(x.ravel()), BaseEncoding), x.shape)
                 return EncodedArray(encoding.decode(x), BaseEncoding)
             return dynamic
         else:
             return funcs[datatype]
 
     columns = [get_func_for_datatype(key)(value) for key, value in data_dict]
-    # columns = [get_func_for_datatype(field.type)(getattr(data, field.name))
-    # for field in dataclasses.fields(data)]
-
     lengths = np.concatenate([((column.lengths if
                                 isinstance(column, RaggedArray)
                                 else np.array([
                                             column.shape[-1] if len(column.shape) == 2 else 1
                                               ]*len(column))) + 1
                                )[:, np.newaxis]
                               
                               for column in columns], axis=-1).ravel()
     lines = EncodedRaggedArray(EncodedArray(np.empty(lengths.sum(), dtype=np.uint8), BaseEncoding),
                                lengths)
     n_columns = len(columns)
     for i, column in enumerate(columns):
-        if (not isinstance(column, RaggedArray)) and len(column.shape)==1:
-            column = EncodedRaggedArray.from_numpy_array(column[:, np.newaxis]) # AND HERE
+        if (not isinstance(column, RaggedArray)) and len(column.shape) == 1:
+            column = EncodedRaggedArray.from_numpy_array(column[:, np.newaxis])
         lines[i::n_columns, :-1] = column
     lines[:, -1] = sep
     lines[(n_columns - 1)::n_columns, -1] = "\n"
     return lines.ravel()
```

### Comparing `bionumpy-0.2.8/bionumpy/io/file_buffers.py` & `bionumpy-0.2.9/bionumpy/io/file_buffers.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
             FileBuffer containing the data
         """
         return NotImplemented
 
     def validate_if_not(self):
         if not self._is_validated:
             self._validate()
+            self._is_validated = True
 
     def get_data(self) -> bnpdataclass:
         """Extract the data from the buffer
 
         The default way to extract data from the the buffer
 
         Returns
@@ -140,16 +141,19 @@
         zeroed, _ = RaggedView(np.arange(starts.size)*max_chars, max_chars-(ends-starts)).get_flat_indices()
         array[zeroed] = fill_value
         return array.reshape((-1, max_chars))
 
     def _move_intervals_to_ragged_array(self, starts, ends=None, lens=None, as_sequence=True):
         if lens is None:
             lens = ends - starts
-        indices, shape = RaggedView(starts, lens).get_flat_indices()
-        return EncodedRaggedArray(self._data[indices], shape)
+            # indices, shape = RaggedView(starts, lens).get_flat_indices()
+        e = EncodedRaggedArray(self._data, RaggedView(starts, lens))
+        e.is_contigous = False
+        return e
+        # return EncodedRaggedArray(self._data[indices], shape)
 
     def _move_2d_array_to_intervals(self, array, starts, ends):
         max_chars = array.shape[-1]
         to_indices = ends[::-1, None]-max_chars+np.arange(max_chars)
         self._data[to_indices] = array[::-1]
 
     @classmethod
```

### Comparing `bionumpy-0.2.8/bionumpy/io/files.py` & `bionumpy-0.2.9/bionumpy/io/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,7 +194,14 @@
         buffer_type = _get_buffer_type(suffix)
 
     file_reader = NumpyFileReader(open_func(filename, "rb"), buffer_type)
     if is_gzip:
         file_reader.set_prepend_mode()
     chunk_counts = (chunk.count_entries() for chunk in file_reader.read_chunks())
     return sum(chunk_counts)
+
+
+def read(filename: str, mode: str = None, buffer_type=None) -> NpDataclassReader:
+    'openes a file, reads it and closes it '
+    with bnp_open(filename, mode, buffer_type) as f:
+        content = f.read()
+    return content
```

### Comparing `bionumpy-0.2.8/bionumpy/io/gfa.py` & `bionumpy-0.2.9/bionumpy/io/gfa.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/io/indexed_fasta.py` & `bionumpy-0.2.9/bionumpy/io/indexed_fasta.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/io/indexed_files.py` & `bionumpy-0.2.9/bionumpy/io/indexed_files.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/io/matrix_dump.py` & `bionumpy-0.2.9/bionumpy/io/matrix_dump.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/io/multiline_buffer.py` & `bionumpy-0.2.9/bionumpy/io/multiline_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         return False
 
     def get_data(self):
         self.validate_if_not()
         line_starts = np.insert(self._new_lines + 1, 0, 0)
         line_ends = np.append(self._new_lines, self._data.size-1)
         data = self._move_intervals_to_ragged_array(line_starts, line_ends)
+        data.ravel()
         new_entries = np.insert(self._new_entries+1, 0, 0)
         n_lines_per_entry = np.diff(np.append(new_entries, self._new_lines.size+1))-1
         line_offsets = np.insert(np.cumsum(n_lines_per_entry),0, 0)
         headers = data[new_entries, 1:]
         mask  = np.ones(len(data), dtype=bool)
         mask[new_entries] = False
         sequence_lines = data[mask]
```

### Comparing `bionumpy-0.2.8/bionumpy/io/npdataclassreader.py` & `bionumpy-0.2.9/bionumpy/io/npdataclassreader.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/io/parser.py` & `bionumpy-0.2.9/bionumpy/io/parser.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/io/strops.py` & `bionumpy-0.2.9/bionumpy/io/strops.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,17 @@
 
     Examples
     --------
     FIXME: Add docs.
 
     """
     number_text = as_encoded_array(number_text)
+    assert number_text.encoding == BaseEncoding
+    return np.array([float(row.to_string()) for row in number_text])
+
     scientific = np.any(number_text == "e", axis=-1)
     numbers = np.empty(len(number_text))
     if np.sum(scientific):
         numbers[scientific] = _scientific_str_to_float(number_text[scientific])
     if np.sum(~scientific):
         numbers[~scientific] = _decimal_str_to_float(number_text[~scientific])
     return numbers
@@ -197,14 +200,15 @@
 
     Returns
     -------
     EncodedRaggedArray
         strings in EncodedRaggedArray
 
     """
+    return as_encoded_array([str(f) for f in floats])
     s = np.array2string(floats, max_line_width=10**15, threshold=10**15, separator=",").replace(" ", "")
     assert " " not in s, s
     b = np.frombuffer(bytes(s, encoding="ascii"), dtype=np.uint8)
     return split(EncodedArray(b[1:-1]), sep=",")
 
 
 def int_lists_to_strings(int_lists: RaggedArray, sep: str = ",", keep_last: bool = False) -> EncodedRaggedArray:
```

### Comparing `bionumpy-0.2.8/bionumpy/sequence/__init__.py` & `bionumpy-0.2.9/bionumpy/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/count_encoded.py` & `bionumpy-0.2.9/bionumpy/sequence/count_encoded.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/dna.py` & `bionumpy-0.2.9/bionumpy/sequence/dna.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/genes.py` & `bionumpy-0.2.9/bionumpy/sequence/genes.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/indexing/kmer_indexing.py` & `bionumpy-0.2.9/bionumpy/sequence/indexing/kmer_indexing.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/indexing/wildcard_index.py` & `bionumpy-0.2.9/bionumpy/sequence/indexing/wildcard_index.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/kmers.py` & `bionumpy-0.2.9/bionumpy/sequence/kmers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/lookup.py` & `bionumpy-0.2.9/bionumpy/sequence/lookup.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/minimizers.py` & `bionumpy-0.2.9/bionumpy/sequence/minimizers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/position_weight_matrix.py` & `bionumpy-0.2.9/bionumpy/sequence/position_weight_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,15 +168,21 @@
     -------
     RaggedArray
         A numeric RaggedArray. Contains one row for every read
         with the scores for every position of that read.
 
     Examples
     --------
-
+    >>> import bionumpy as bnp
+    >>> pwm = bnp.sequence.position_weight_matrix.PWM.from_dict({"A": [5, 1], "C": [1, 5], "G": [0, 0], "T": [0, 0]})
+    >>> sequences = bnp.as_encoded_array(["ACTGAC", "CA", "GG"])
+    >>> bnp.get_motif_scores(sequences, pwm)
+    ragged_array([5.99146455       -inf       -inf       -inf 5.99146455]
+    [2.77258872]
+    [-inf])
     """
     sequence = as_encoded_array(sequence)
     flat_sequence, shape = (sequence.ravel(), sequence.shape)
     scores = pwm.calculate_scores(flat_sequence)
     if isinstance(sequence, EncodedRaggedArray):
         scores = RaggedArray(scores, shape[-1])
     return scores[..., :(-pwm.window_size+1)]
```

### Comparing `bionumpy-0.2.8/bionumpy/sequence/rollable.py` & `bionumpy-0.2.9/bionumpy/sequence/rollable.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/string_matcher.py` & `bionumpy-0.2.9/bionumpy/sequence/string_matcher.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/sequence/translate.py` & `bionumpy-0.2.9/bionumpy/sequence/translate.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/simulate/chipseq.py` & `bionumpy-0.2.9/bionumpy/simulate/chipseq.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         fragments.stop)
     starts = np.maximum(starts, fragments.start)
     stops = np.minimum(stops, fragments.stop)
     return Bed6(fragments.chromosome,
                 starts,
                 stops,
                 ["."]*len(stops),
-                [0]*len(stops),
+                ["0"]*len(stops),
                 strands)
 
 
 @streamable()
 def simulate_chip_seq_reads(reference_sequence, settings):
     n_fragments = settings.coverage*len(reference_sequence)//settings.read_length
     fragments = simulate_chip_seq_fragments(reference_sequence, settings.motif, n_fragments, settings.fragment_length)
```

### Comparing `bionumpy-0.2.8/bionumpy/simulate/rnaseq.py` & `bionumpy-0.2.9/bionumpy/simulate/rnaseq.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/simulate/sequences.py` & `bionumpy-0.2.9/bionumpy/simulate/sequences.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/streams/decorators.py` & `bionumpy-0.2.9/bionumpy/streams/decorators.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/streams/groupby_func.py` & `bionumpy-0.2.9/bionumpy/streams/groupby_func.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from npstructures import RaggedView, RaggedArray
 import dataclasses
 import itertools
 import numpy as np
 from . import streamable, grouped_stream
 from ..bnpdataclass import bnpdataclass
-
+from ..encoded_array import EncodedArray
 
 def get_changes(array):
     if isinstance(array, RaggedArray):
         return get_ragged_changes(array)
     array = array.reshape(len(array), -1)
     return np.flatnonzero(np.all(array[1:]!=array[-1], axis=-1))+1
 
@@ -94,15 +94,15 @@
 
     """
     if column is not None:
         assert hasattr(data, column), (data.__class__, dataclasses.fields(data), column)
         keys = getattr(data, column)
     else:
         keys = data
-    if (keys.lengths[-1] == keys.lengths[0]) and np.all(keys[-1] == keys[0]):
+    if (isinstance(keys, EncodedArray) or (keys.lengths[-1] == keys.lengths[0])) and np.all(keys[-1] == keys[0]):
         return grouped_stream(((key(keys[start]), data[start:]) for start in [0]), column)
                                        
 
     changes = get_changes(keys)
     changes = np.append(np.insert(changes, 0, 0), len(data))
     assert np.all(np.diff(changes)>0), changes
     return grouped_stream(((key(keys[start]), data[start:end])
```

### Comparing `bionumpy-0.2.8/bionumpy/streams/grouped.py` & `bionumpy-0.2.9/bionumpy/streams/grouped.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/streams/multistream.py` & `bionumpy-0.2.9/bionumpy/streams/multistream.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/streams/reductions.py` & `bionumpy-0.2.9/bionumpy/streams/reductions.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/streams/stream.py` & `bionumpy-0.2.9/bionumpy/streams/stream.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/util/__init__.py` & `bionumpy-0.2.9/bionumpy/util/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+import numpy.typing as npt
 import logging
 from npstructures import RaggedArray
 import dataclasses
 import sys
 from . import testing
 from . import typing
 logger = logging.getLogger(__name__)
@@ -58,7 +59,12 @@
     if not hasattr(obj, "__plot__"):
         logger.warning(f"{obj} has no __plot__ method")
 
 
 def is_subclass_or_instance(obj, c):
     return (isinstance(obj, type) and issubclass(obj, c)) or isinstance(obj, c)
 
+def interleave(array_a: npt.ArrayLike, array_b: npt.ArrayLike) -> npt.ArrayLike:
+    c = np.empty((array_a.size + array_b.size,), dtype=array_a.dtype)
+    c[0::2] = array_a
+    c[1::2] = array_b
+    return c
```

### Comparing `bionumpy-0.2.8/bionumpy/util/testing.py` & `bionumpy-0.2.9/bionumpy/util/testing.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy/variants/mutation_signature.py` & `bionumpy-0.2.9/bionumpy/variants/mutation_signature.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/bionumpy.egg-info/PKG-INFO` & `bionumpy-0.2.9/bionumpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bionumpy
-Version: 0.2.8
+Version: 0.2.9
 Summary: Library for working with biological sequence data as numpy arrays.
 Home-page: https://github.com/knutdrand/bionumpy
 Author: Knut Rand
 Author-email: knutdrand@gmail.com
 License: MIT license
 Keywords: bionumpy
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -29,33 +29,46 @@
         :target: https://github.com/bionumpy/bionumpy/actions/
         :alt: Build and test status
 
 .. image:: https://github.com/bionumpy/bionumpy-example-data/actions/workflows/run_checks.yml/badge.svg
         :target: https://github.com/bionumpy/bionumpy-example-data/actions/
         :alt: Testing on big data
 
+.. image:: https://github.com/bionumpy/bionumpy/actions/workflows/benchmarking.yml/badge.svg
+        :target: https://github.com/bionumpy/bionumpy/blob/benchmarks/benchmarks/report_small.md
+        :alt: Benchmarks
+
+
 Documentation: `https://bionumpy.github.io/bionumpy/ <https://bionumpy.github.io/bionumpy/>`_
 
 
 What is BioNumPy?
 -----------------
-BioNumPy is a toolkit, built on top of NumPy, for enabling array programming on biological data in Python. BioNumPy aims to make it easy to read common bioinformatics file formats efficiently into NumPy-like data structures that enable efficient operations and analysis of the data. Working in BioNumPy should feel much like working in NumPy.
-
-
-Why BioNumPy?
--------------
-* There are no existing packages in Python for getting biological datasets efficiently into NumPy-like data structures.
-* Current packages for working with biological data do not use NumPy in an efficient way (e.g. individual sequences are stored as separate NumPy arrays, not together in shared arrays).
+BioNumPy is a Python library, built on top of NumPy, for enabling array programming on biological datasets in Python.
+BioNumPy aims to make it easy to read common bioinformatics file formats efficiently into NumPy-like data structures
+that enable efficient operations and analysis of the data. Working in BioNumPy should feel much like working in NumPy.
 
 
 Getting started
 ----------------
 
 1. Install with pip:
 
 	$ pip install bionumpy
 
-2. Check out the tutorials and getting started guide in the `documentation <https://bionumpy.github.io/bionumpy/>`_.
+2. Import BioNumPy and read your data, e.g.:
+
+    >>> import bionumpy as bnp
+    >>> import numpy as np
+    >>> f = bnp.open("example_data/big.fq.gz")
+    >>> # chunk contains the sequences of reads and NumPy-functions can be used
+    >>> for chunk in f:
+    ...      print(np.sum(chunk.sequence == "G"))
+    53686
+
+Check out the getting started guide and various tutorials in the `documentation <https://bionumpy.github.io/bionumpy/>`_.
+
+
```

### Comparing `bionumpy-0.2.8/bionumpy.egg-info/SOURCES.txt` & `bionumpy-0.2.9/bionumpy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 bionumpy.egg-info/not-zip-safe
 bionumpy.egg-info/requires.txt
 bionumpy.egg-info/top_level.txt
 bionumpy/alignments/__init__.py
 bionumpy/alignments/cigar.py
 bionumpy/arithmetics/__init__.py
 bionumpy/arithmetics/bedgraph.py
+bionumpy/arithmetics/global_offset.py
 bionumpy/arithmetics/intervals.py
 bionumpy/arithmetics/similarity_measures.py
 bionumpy/bnpdataclass/__init__.py
 bionumpy/bnpdataclass/bnpdataclass.py
 bionumpy/bnpdataclass/bnpdataclassfunction.py
 bionumpy/cupy_compatible/__init__.py
 bionumpy/cupy_compatible/parser.py
@@ -28,14 +29,15 @@
 bionumpy/datatypes/gtf.py
 bionumpy/encodings/__init__.py
 bionumpy/encodings/_legacy_encodings.py
 bionumpy/encodings/alphabet_encoding.py
 bionumpy/encodings/base_encoding.py
 bionumpy/encodings/exceptions.py
 bionumpy/encodings/kmer_encodings.py
+bionumpy/encodings/string_encodings.py
 bionumpy/encodings/vcf_encoding.py
 bionumpy/io/__init__.py
 bionumpy/io/bam.py
 bionumpy/io/delimited_buffers.py
 bionumpy/io/dump_csv.py
 bionumpy/io/exceptions.py
 bionumpy/io/file_buffers.py
@@ -66,37 +68,43 @@
 bionumpy/sequence/indexing/wildcard_index.py
 bionumpy/simulate/__init__.py
 bionumpy/simulate/chipseq.py
 bionumpy/simulate/rnaseq.py
 bionumpy/simulate/rng.py
 bionumpy/simulate/sequences.py
 bionumpy/streams/__init__.py
+bionumpy/streams/chunk_entries.py
 bionumpy/streams/decorators.py
 bionumpy/streams/groupby_func.py
 bionumpy/streams/grouped.py
 bionumpy/streams/multistream.py
 bionumpy/streams/reductions.py
 bionumpy/streams/stream.py
 bionumpy/util/__init__.py
+bionumpy/util/ascii_hash.py
 bionumpy/util/cli.py
 bionumpy/util/testing.py
 bionumpy/util/typing.py
 bionumpy/variants/__init__.py
 bionumpy/variants/mutation_signature.py
 tests/__init__.py
 tests/buffers.py
 tests/gfa_test.py
+tests/test_asciihash.py
 tests/test_bam.py
 tests/test_bionumpy.py
 tests/test_bnpdataclass.py
 tests/test_chromosome_provider.py
 tests/test_delimited_buffers.py
 tests/test_dna.py
 tests/test_encoded_array.py
+tests/test_encodedarrayfunctions.py
 tests/test_encodings.py
+tests/test_entry_chunker.py
+tests/test_global_offset.py
 tests/test_groupby.py
 tests/test_gtf.py
 tests/test_indexed_fasta.py
 tests/test_integration.py
 tests/test_intervals.py
 tests/test_io.py
 tests/test_io_exceptions.py
@@ -110,19 +118,21 @@
 tests/test_pileup.py
 tests/test_position_weight_matrix.py
 tests/test_rollable.py
 tests/test_seqeunces.py
 tests/test_similarity_measures.py
 tests/test_simulate.py
 tests/test_streambroadcast.py
+tests/test_string_encodings.py
 tests/test_string_matcher.py
 tests/test_strops.py
 tests/test_translate.py
 tests/test_util.py
 tests/test_vcf.py
 tests/test_vcf_encoding.py
 tests/test_wildcard_index.py
+tests/performance/interval_sort.py
 tests/property_tests/__init__.py
 tests/property_tests/strategies.py
 tests/property_tests/test_delimited_buffers.py
 tests/property_tests/test_encodings.py
 tests/property_tests/test_strops.py
```

### Comparing `bionumpy-0.2.8/setup.py` & `bionumpy-0.2.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['numpy>=1.20',
-                'npstructures>=0.2.3']
+    requirements = ['numpy>=1.20,<1.24',
+                    'npstructures>=0.2.8']
 # 'npstructures @ git+https://github.com/knutdrand/npstructures.git']
 
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Knut Rand",
     author_email='knutdrand@gmail.com',
@@ -42,13 +42,13 @@
     include_package_data=True,
     keywords='bionumpy',
     name='bionumpy',
     packages=find_packages(include=['bionumpy', 'bionumpy.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/knutdrand/bionumpy',
-    version='0.2.8',
+    version='0.2.9',
     zip_safe=False,
 )
 
 # python -m build
 # twine upload dist/*
```

### Comparing `bionumpy-0.2.8/tests/buffers.py` & `bionumpy-0.2.9/tests/buffers.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,17 +78,17 @@
 """
 }
 
 buffers = {key: chunk_from_text(val) for key, val in buffer_texts.items()}
 
 data = {
     "bed": [
-        Bed6.single_entry("chr1", 1, 3, ".", 0, "-"),
-        Bed6.single_entry("chr1", 40, 60, ".", 1, "+"),
-        Bed6.single_entry("chr20",  400, 600, ".", 2, "+")],
+        Bed6.single_entry("chr1", 1, 3, ".", "0", "-"),
+        Bed6.single_entry("chr1", 40, 60, ".", "1", "+"),
+        Bed6.single_entry("chr20",  400, 600, ".", "2", "+")],
     "vcf2": [
         VCFEntry.single_entry("chr1",	88361, "rs4970378",	"A",	"G", ".", ".", "."),
         VCFEntry.single_entry("chr1",	887559, "rs3748595",	"A",	"CAA", ".", ".", "."),
         VCFEntry.single_entry("chr2",	8877, "rs3828047",	"AGG",	"C", ".", ".", ".")],
     "vcf": [
         VCFEntry.single_entry("chr1",	88361, "rs4970378",	"A",	"G", ".", ".", "."),
         VCFEntry.single_entry("chr1",	887559, "rs3748595",	"A",	"C", ".", ".", "."),
@@ -105,16 +105,16 @@
     "gfa_sequence": [
         SequenceEntry.single_entry("id1", "AACCTTGG"),
         SequenceEntry.single_entry("id4", "ACTG")],
     "sam": [
         SAMEntry.single_entry("SRR1524970.144283", 16, "test_ref", 1705, 255, "25M",	"*", 0, 0, "TGCTGATGAAGCAGAACAACTTTAA", "]YG[^baaaa^W`ab]]````aaba"),
         SAMEntry.single_entry("SRR1524970.316478", 16, "test_ref", 1705, 255, "24M", "*", 0, 0, "TGCTGATGAAGCAGAACAACTTTA", 	"`\X_`aaaaaY]``b_aa_aaaaa")],
     "bed12": [
-        Bed12.single_entry("chr21", 10079666,  10120808,   "uc002yiv.1", 0, "-", 10081686, 10120608,  "0",     4,   [[528,91,101,215]], [[0,1930,39750,40927]]),
-        Bed12.single_entry("chr21", 10080031,  10081687,   "uc002yiw.1",  0,  "-",  10080031,  10080031,  "0",     2,   [[200,91]],    [[0,1565]])]
+        Bed12.single_entry("chr21", 10079666,  10120808,   "uc002yiv.1", "0", "-", 10081686, 10120608,  "0",     4,   [[528,91,101,215]], [[0,1930,39750,40927]]),
+        Bed12.single_entry("chr21", 10080031,  10081687,   "uc002yiw.1",  "0",  "-",  10080031,  10080031,  "0",     2,   [[200,91]],    [[0,1565]])]
 }
 
 
 buffer_type = {"bed": Bed6Buffer,
                "vcf2": VCFBuffer,
                "vcf": VCFBuffer,
                "fastq": FastQBuffer,
```

### Comparing `bionumpy-0.2.8/tests/property_tests/strategies.py` & `bionumpy-0.2.9/tests/property_tests/strategies.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/property_tests/test_delimited_buffers.py` & `bionumpy-0.2.9/tests/property_tests/test_delimited_buffers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/property_tests/test_encodings.py` & `bionumpy-0.2.9/tests/property_tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/property_tests/test_strops.py` & `bionumpy-0.2.9/tests/property_tests/test_strops.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_bnpdataclass.py` & `bionumpy-0.2.9/tests/test_bnpdataclass.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_chromosome_provider.py` & `bionumpy-0.2.9/tests/test_chromosome_provider.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_delimited_buffers.py` & `bionumpy-0.2.9/tests/test_delimited_buffers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_dna.py` & `bionumpy-0.2.9/tests/test_dna.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_encoded_array.py` & `bionumpy-0.2.9/tests/test_encoded_array.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_encodings.py` & `bionumpy-0.2.9/tests/test_encodings.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,25 +90,24 @@
     assert np.all(encoded2 == encoded)
 
 
 TestDigitEncoding = DigitEncodingFactory("1")
 
 
 @bnpdataclass
-class TestEntry:
+class Entry:
     a: TestDigitEncoding
 
 
 def test_numeric_entry():
     encoding = TestDigitEncoding
-    a = TestEntry.single_entry("1234")
+    a = Entry.single_entry("1234")
     assert np.all(encoding.decode(a.a) == 48 + np.array([1, 2, 3, 4]))
 
 
-
 @pytest.mark.parametrize("data", ["!#", ["!#"]])
 def test_quality_encoding(data):
     data = as_encoded_array(data, BaseEncoding)
     encoded_data = as_encoded_array(data, QualityEncoding)
     assert np.all(encoded_data.ravel() == [0, 2])
```

### Comparing `bionumpy-0.2.8/tests/test_groupby.py` & `bionumpy-0.2.9/tests/test_groupby.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_gtf.py` & `bionumpy-0.2.9/tests/test_gtf.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_indexed_fasta.py` & `bionumpy-0.2.9/tests/test_indexed_fasta.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_integration.py` & `bionumpy-0.2.9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_io.py` & `bionumpy-0.2.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_io_exceptions.py` & `bionumpy-0.2.9/tests/test_io_exceptions.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_kmer.py` & `bionumpy-0.2.9/tests/test_kmer.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_kmer_index.py` & `bionumpy-0.2.9/tests/test_kmer_index.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_kmer_nmf.py` & `bionumpy-0.2.9/tests/test_kmer_nmf.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_minimizers.py` & `bionumpy-0.2.9/tests/test_minimizers.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_multistream.py` & `bionumpy-0.2.9/tests/test_multistream.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_npdataclassstream.py` & `bionumpy-0.2.9/tests/test_npdataclassstream.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_parsers.py` & `bionumpy-0.2.9/tests/test_parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,30 +156,37 @@
 
 def test_read_gtf():
     file = bnp.open("example_data/small.gtf")
     chunk = file.read_chunk()
     assert True
 
 
+@pytest.mark.skip("makingtrouble")
 @pytest.mark.parametrize("file_name", glob.glob("example_data/*"))
 def test_read_example_data(file_name):
     if "broken" in file_name:
         # broken data should not pass tests
         return
 
+    if file_name.endswith(".txt"):
+        return
+
     if file_name.endswith(".sam"):
         return
 
     if file_name.endswith(".fa.fai"):
         return
 
     if file_name.endswith(".jaspar"):
         return
 
     if file_name.endswith(".tsv"):
         return
 
+    if file_name.startswith("demultiplex"):
+        return
+
     file = bnp.open(file_name)
     for chunk in file.read_chunks():
         continue
 
     assert True
```

### Comparing `bionumpy-0.2.8/tests/test_pileup.py` & `bionumpy-0.2.9/tests/test_pileup.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_position_weight_matrix.py` & `bionumpy-0.2.9/tests/test_position_weight_matrix.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_rollable.py` & `bionumpy-0.2.9/tests/test_rollable.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_seqeunces.py` & `bionumpy-0.2.9/tests/test_seqeunces.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_similarity_measures.py` & `bionumpy-0.2.9/tests/test_similarity_measures.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_simulate.py` & `bionumpy-0.2.9/tests/test_simulate.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_streambroadcast.py` & `bionumpy-0.2.9/tests/test_streambroadcast.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_string_matcher.py` & `bionumpy-0.2.9/tests/test_string_matcher.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_strops.py` & `bionumpy-0.2.9/tests/test_strops.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         assert i == s
 
 
 def test_str_to_float(floats):
     np.testing.assert_array_almost_equal([float(c) for c in floats], str_to_float(floats))
 
 
-@pytest.mark.skip("Inaccurate float")
+#@pytest.mark.skip("Inaccurate float")
 def test_float_to_str(floats):
     _floats = np.array([float(c) for c in floats])
     ra = float_to_strings(_floats)
     np.testing.assert_array_almost_equal([float(row.to_string()) for row in ra],
                                          _floats)
```

### Comparing `bionumpy-0.2.8/tests/test_util.py` & `bionumpy-0.2.9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_vcf.py` & `bionumpy-0.2.9/tests/test_vcf.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_vcf_encoding.py` & `bionumpy-0.2.9/tests/test_vcf_encoding.py`

 * *Files identical despite different names*

### Comparing `bionumpy-0.2.8/tests/test_wildcard_index.py` & `bionumpy-0.2.9/tests/test_wildcard_index.py`

 * *Files identical despite different names*

