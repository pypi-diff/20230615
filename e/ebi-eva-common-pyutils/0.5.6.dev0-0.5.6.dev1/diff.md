# Comparing `tmp/ebi_eva_common_pyutils-0.5.6.dev0.tar.gz` & `tmp/ebi_eva_common_pyutils-0.5.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.5.6.dev0.tar", last modified: Tue Jun 13 13:32:54 2023, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.5.6.dev1.tar", last modified: Thu Jun 15 14:12:45 2023, max compression
```

## Comparing `ebi_eva_common_pyutils-0.5.6.dev0.tar` & `ebi_eva_common_pyutils-0.5.6.dev1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.360368 ebi_eva_common_pyutils-0.5.6.dev0/
--rw-rw-r--   0 april     (1000) april     (1000)     1812 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev0/CHANGELOG.md
--rw-rw-r--   0 april     (1000) april     (1000)    11357 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/LICENSE
--rw-rw-r--   0 april     (1000) april     (1000)       28 2022-10-21 09:58:13.000000 ebi_eva_common_pyutils-0.5.6.dev0/MANIFEST.in
--rw-rw-r--   0 april     (1000) april     (1000)      572 2023-06-13 13:32:54.360368 ebi_eva_common_pyutils-0.5.6.dev0/PKG-INFO
--rw-rw-r--   0 april     (1000) april     (1000)     1434 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/README.md
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.356368 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/
--rw-rw-r--   0 april     (1000) april     (1000)        0 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     4984 2022-12-14 10:24:31.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/archive_directory.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.356368 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/assembly/
--rw-rw-r--   0 april     (1000) april     (1000)       66 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/assembly/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     1570 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/assembly/assembly.py
--rw-rw-r--   0 april     (1000) april     (1000)     2151 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/command_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     1192 2022-11-15 14:54:19.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/common_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     2242 2022-10-21 09:58:09.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/config.py
--rw-rw-r--   0 april     (1000) april     (1000)     7952 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/config_utils.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.356368 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/contig_alias/
--rw-rw-r--   0 april     (1000) april     (1000)        0 2022-11-15 14:54:19.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     3056 2022-11-15 14:54:19.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-rw-r--   0 april     (1000) april     (1000)     1452 2022-10-21 09:58:13.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/ena_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     1375 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/file_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     4990 2022-10-21 09:58:13.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/logger.py
--rw-rw-r--   0 april     (1000) april     (1000)    14953 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/metadata_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     3573 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/mongo_utils.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.356368 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/mongodb/
--rw-rw-r--   0 april     (1000) april     (1000)       72 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/mongodb/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     9676 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/mongodb/mongo_database.py
--rw-rw-r--   0 april     (1000) april     (1000)     4859 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/ncbi_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     2285 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/network_utils.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.356368 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/nextflow/
--rw-rw-r--   0 april     (1000) april     (1000)      120 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/nextflow/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)    10114 2022-10-21 09:58:13.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
--rw-rw-r--   0 april     (1000) april     (1000)     4398 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/pg_utils.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.356368 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/reference/
--rw-rw-r--   0 april     (1000) april     (1000)      134 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/reference/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)    12162 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/reference/assembly.py
--rw-rw-r--   0 april     (1000) april     (1000)     3911 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/reference/sequence.py
--rw-rw-r--   0 april     (1000) april     (1000)    15054 2023-06-12 10:27:15.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/spring_properties.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.356368 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/taxonomy/
--rw-rw-r--   0 april     (1000) april     (1000)        0 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     2259 2022-11-15 14:54:19.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.356368 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/variation/
--rw-rw-r--   0 april     (1000) april     (1000)        0 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/variation/__init__.py
--rw-rw-r--   0 april     (1000) april     (1000)     3515 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/variation/assembly_utils.py
--rw-rw-r--   0 april     (1000) april     (1000)     5230 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-13 13:32:54.356368 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils.egg-info/
--rw-rw-r--   0 april     (1000) april     (1000)      572 2023-06-13 13:32:54.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-rw-r--   0 april     (1000) april     (1000)     1690 2023-06-13 13:32:54.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-rw-r--   0 april     (1000) april     (1000)        1 2023-06-13 13:32:54.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-rw-r--   0 april     (1000) april     (1000)       81 2023-06-13 13:32:54.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-rw-r--   0 april     (1000) april     (1000)       23 2023-06-13 13:32:54.000000 ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils.egg-info/top_level.txt
--rw-rw-r--   0 april     (1000) april     (1000)      225 2023-06-13 13:32:54.360368 ebi_eva_common_pyutils-0.5.6.dev0/setup.cfg
--rw-rw-r--   0 april     (1000) april     (1000)      912 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev0/setup.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/
+-rw-rw-r--   0 april     (1000) april     (1000)     1812 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev1/CHANGELOG.md
+-rw-rw-r--   0 april     (1000) april     (1000)    11357 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/LICENSE
+-rw-rw-r--   0 april     (1000) april     (1000)       28 2022-10-21 09:58:13.000000 ebi_eva_common_pyutils-0.5.6.dev1/MANIFEST.in
+-rw-rw-r--   0 april     (1000) april     (1000)      572 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/PKG-INFO
+-rw-rw-r--   0 april     (1000) april     (1000)     1434 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/README.md
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/
+-rw-rw-r--   0 april     (1000) april     (1000)        0 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     4984 2022-12-14 10:24:31.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/archive_directory.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/assembly/
+-rw-rw-r--   0 april     (1000) april     (1000)       66 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     1570 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-rw-r--   0 april     (1000) april     (1000)     2151 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/command_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     1192 2022-11-15 14:54:19.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/common_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     2242 2022-10-21 09:58:09.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/config.py
+-rw-rw-r--   0 april     (1000) april     (1000)     7952 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/config_utils.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/contig_alias/
+-rw-rw-r--   0 april     (1000) april     (1000)        0 2022-11-15 14:54:19.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     3056 2022-11-15 14:54:19.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-rw-r--   0 april     (1000) april     (1000)     1452 2022-10-21 09:58:13.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/ena_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     1375 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/file_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     4990 2022-10-21 09:58:13.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/logger.py
+-rw-rw-r--   0 april     (1000) april     (1000)    14953 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/metadata_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     3573 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/mongo_utils.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/mongodb/
+-rw-rw-r--   0 april     (1000) april     (1000)       72 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/mongodb/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     9676 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/mongodb/mongo_database.py
+-rw-rw-r--   0 april     (1000) april     (1000)     4859 2023-06-12 09:54:37.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     2285 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/network_utils.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/nextflow/
+-rw-rw-r--   0 april     (1000) april     (1000)      120 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/nextflow/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)    10114 2022-10-21 09:58:13.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
+-rw-rw-r--   0 april     (1000) april     (1000)     4398 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/pg_utils.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/reference/
+-rw-rw-r--   0 april     (1000) april     (1000)      134 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/reference/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)    12162 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/reference/assembly.py
+-rw-rw-r--   0 april     (1000) april     (1000)     3911 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/reference/sequence.py
+-rw-rw-r--   0 april     (1000) april     (1000)    15111 2023-06-15 14:10:52.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/spring_properties.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/taxonomy/
+-rw-rw-r--   0 april     (1000) april     (1000)        0 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     2259 2022-11-15 14:54:19.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/variation/
+-rw-rw-r--   0 april     (1000) april     (1000)        0 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/variation/__init__.py
+-rw-rw-r--   0 april     (1000) april     (1000)     3515 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/variation/assembly_utils.py
+-rw-rw-r--   0 april     (1000) april     (1000)     5230 2021-07-06 14:11:42.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxrwxr-x   0 april     (1000) april     (1000)        0 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils.egg-info/
+-rw-rw-r--   0 april     (1000) april     (1000)      572 2023-06-15 14:12:45.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-rw-r--   0 april     (1000) april     (1000)     1690 2023-06-15 14:12:45.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 april     (1000) april     (1000)        1 2023-06-15 14:12:45.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 april     (1000) april     (1000)       81 2023-06-15 14:12:45.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-rw-r--   0 april     (1000) april     (1000)       23 2023-06-15 14:12:45.000000 ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils.egg-info/top_level.txt
+-rw-rw-r--   0 april     (1000) april     (1000)      225 2023-06-15 14:12:45.988952 ebi_eva_common_pyutils-0.5.6.dev1/setup.cfg
+-rw-rw-r--   0 april     (1000) april     (1000)      912 2023-06-15 14:12:43.000000 ebi_eva_common_pyutils-0.5.6.dev1/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/CHANGELOG.md` & `ebi_eva_common_pyutils-0.5.6.dev1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/LICENSE` & `ebi_eva_common_pyutils-0.5.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/PKG-INFO` & `ebi_eva_common_pyutils-0.5.6.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ebi_eva_common_pyutils
-Version: 0.5.6.dev0
+Version: 0.5.6.dev1
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache
 Description: UNKNOWN
 Keywords: EBI,EVA,PYTHON,UTILITIES
```

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/README.md` & `ebi_eva_common_pyutils-0.5.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/spring_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,15 @@
                                temp_mongo_db=None):
         common_props = self._common_accessioning_properties(assembly_accession=assembly_accession,
                                                             read_preference='secondaryPreferred', chunk_size=1000)
         # For release in Embassy only
         if temp_mongo_db:
             common_props['spring.data.mongodb.database'] = temp_mongo_db
             common_props['mongodb.read-preference'] = 'primaryPreferred'
+            common_props.pop('spring.data.mongodb.host')
             common_props.pop('spring.data.mongodb.username')
             common_props.pop('spring.data.mongodb.password')
         return self._format(
             common_props,
             {
                 'spring.batch.job.names': job_name,
                 'parameters.taxonomyAccession': taxonomy_accession,
```

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/variation/assembly_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/variation/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils.egg-info/PKG-INFO` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ebi-eva-common-pyutils
-Version: 0.5.6.dev0
+Version: 0.5.6.dev1
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: Apache
 Description: UNKNOWN
 Keywords: EBI,EVA,PYTHON,UTILITIES
```

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.5.6.dev1/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.6.dev0/setup.py` & `ebi_eva_common_pyutils-0.5.6.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_common_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.5.6.dev0',
+    version='0.5.6.dev1',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['psycopg2-binary', 'requests', 'pymongo', 'lxml', 'pyyaml', 'cached-property', 'retry',
                       'networkx<=2.5'],
     classifiers=[
```

