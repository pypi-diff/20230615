# Comparing `tmp/pdm_utils-1.0.0.tar.gz` & `tmp/pdm_utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdm_utils-1.0.0.tar", last modified: Thu Jun 15 00:24:09 2023, max compression
+gzip compressed data, was "/Users/labad/git_repos/pdm_utils/dist/.tmp-k0ze0vqk/pdm_utils-1.0.1.tar", last modified: Thu Jun 15 20:39:06 2023, max compression
```

## Comparing `pdm_utils-1.0.0.tar` & `pdm_utils-1.0.1.tar`

### file list

```diff
@@ -1,87 +1,96 @@
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.116989 pdm_utils-1.0.0/
--rw-r--r--   0 labad      (502) staff       (20)     1718 2023-06-15 00:24:09.116735 pdm_utils-1.0.0/PKG-INFO
--rw-r--r--   0 labad      (502) staff       (20)      790 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/README.md
--rw-r--r--   0 labad      (502) staff       (20)       38 2023-06-15 00:24:09.117067 pdm_utils-1.0.0/setup.cfg
--rw-r--r--   0 labad      (502) staff       (20)     1287 2023-06-15 00:21:24.000000 pdm_utils-1.0.0/setup.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.074887 pdm_utils-1.0.0/src/
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.077621 pdm_utils-1.0.0/src/pdm_utils/
--rw-r--r--   0 labad      (502) staff       (20)      146 2023-06-15 00:23:21.000000 pdm_utils-1.0.0/src/pdm_utils/__init__.py
--rw-r--r--   0 labad      (502) staff       (20)      100 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/__main__.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.089856 pdm_utils-1.0.0/src/pdm_utils/classes/
--rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/__init__.py
--rw-r--r--   0 labad      (502) staff       (20)    20060 2020-10-30 13:34:57.000000 pdm_utils-1.0.0/src/pdm_utils/classes/alchemyhandler.py
--rw-r--r--   0 labad      (502) staff       (20)     8100 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/classes/aragornhandler.py
--rw-r--r--   0 labad      (502) staff       (20)    10410 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/bundle.py
--rw-r--r--   0 labad      (502) staff       (20)    39957 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/cds.py
--rw-r--r--   0 labad      (502) staff       (20)     2461 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/cdspair.py
--rw-r--r--   0 labad      (502) staff       (20)     9923 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/dbcomparesummary.py
--rw-r--r--   0 labad      (502) staff       (20)      696 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/evaluation.py
--rw-r--r--   0 labad      (502) staff       (20)     7966 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/fileio.py
--rw-r--r--   0 labad      (502) staff       (20)    23716 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/classes/filter.py
--rw-r--r--   0 labad      (502) staff       (20)    41595 2021-09-22 16:59:23.000000 pdm_utils-1.0.0/src/pdm_utils/classes/genome.py
--rw-r--r--   0 labad      (502) staff       (20)     5574 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/genomepair.py
--rw-r--r--   0 labad      (502) staff       (20)    18395 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/genometriad.py
--rw-r--r--   0 labad      (502) staff       (20)     1007 2020-11-17 06:11:51.000000 pdm_utils-1.0.0/src/pdm_utils/classes/progressbar.py
--rw-r--r--   0 labad      (502) staff       (20)     7244 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/randomfieldupdatehandler.py
--rw-r--r--   0 labad      (502) staff       (20)     4243 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/source.py
--rw-r--r--   0 labad      (502) staff       (20)     8694 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/ticket.py
--rw-r--r--   0 labad      (502) staff       (20)    37793 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/tmrna.py
--rw-r--r--   0 labad      (502) staff       (20)    64069 2021-09-22 15:49:23.000000 pdm_utils-1.0.0/src/pdm_utils/classes/trna.py
--rw-r--r--   0 labad      (502) staff       (20)     3694 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/trnascansehandler.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.091629 pdm_utils-1.0.0/src/pdm_utils/constants/
--rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/constants/__init__.py
--rw-r--r--   0 labad      (502) staff       (20)     6806 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/constants/constants.py
--rw-r--r--   0 labad      (502) staff       (20)    10763 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/constants/db_schema_0.py
--rw-r--r--   0 labad      (502) staff       (20)    12305 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/constants/eval_descriptions.py
--rw-r--r--   0 labad      (502) staff       (20)    37071 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/constants/schema_conversions.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.105227 pdm_utils-1.0.0/src/pdm_utils/functions/
--rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/__init__.py
--rw-r--r--   0 labad      (502) staff       (20)     6113 2020-10-30 13:34:57.000000 pdm_utils-1.0.0/src/pdm_utils/functions/annotation.py
--rw-r--r--   0 labad      (502) staff       (20)    45918 2021-01-04 16:11:55.000000 pdm_utils-1.0.0/src/pdm_utils/functions/basic.py
--rw-r--r--   0 labad      (502) staff       (20)     2962 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/cartography.py
--rw-r--r--   0 labad      (502) staff       (20)     2166 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/configfile.py
--rw-r--r--   0 labad      (502) staff       (20)     2853 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/functions/deeptmhmm.py
--rw-r--r--   0 labad      (502) staff       (20)     4638 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/eval_modes.py
--rw-r--r--   0 labad      (502) staff       (20)    10526 2021-03-23 03:57:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/fileio.py
--rw-r--r--   0 labad      (502) staff       (20)    30706 2021-09-22 16:59:23.000000 pdm_utils-1.0.0/src/pdm_utils/functions/flat_files.py
--rw-r--r--   0 labad      (502) staff       (20)     5302 2021-01-17 17:23:11.000000 pdm_utils-1.0.0/src/pdm_utils/functions/multithread.py
--rw-r--r--   0 labad      (502) staff       (20)    27400 2022-10-18 17:47:46.000000 pdm_utils-1.0.0/src/pdm_utils/functions/mysqldb.py
--rw-r--r--   0 labad      (502) staff       (20)    13414 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/mysqldb_basic.py
--rw-r--r--   0 labad      (502) staff       (20)     6605 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/ncbi.py
--rw-r--r--   0 labad      (502) staff       (20)     3656 2020-12-08 05:42:09.000000 pdm_utils-1.0.0/src/pdm_utils/functions/parallelize.py
--rw-r--r--   0 labad      (502) staff       (20)    10972 2020-12-29 20:15:44.000000 pdm_utils-1.0.0/src/pdm_utils/functions/parsing.py
--rw-r--r--   0 labad      (502) staff       (20)    13257 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/functions/phagesdb.py
--rw-r--r--   0 labad      (502) staff       (20)     8567 2021-09-22 16:59:23.000000 pdm_utils-1.0.0/src/pdm_utils/functions/pham_alignment.py
--rw-r--r--   0 labad      (502) staff       (20)    24951 2021-03-23 03:57:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/phameration.py
--rw-r--r--   0 labad      (502) staff       (20)     8473 2021-01-04 16:11:55.000000 pdm_utils-1.0.0/src/pdm_utils/functions/pipeline_shells.py
--rw-r--r--   0 labad      (502) staff       (20)     8828 2020-12-28 19:11:26.000000 pdm_utils-1.0.0/src/pdm_utils/functions/pipelines_basic.py
--rw-r--r--   0 labad      (502) staff       (20)    30269 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/functions/querying.py
--rw-r--r--   0 labad      (502) staff       (20)     3475 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/server.py
--rw-r--r--   0 labad      (502) staff       (20)    11826 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/tickets.py
--rw-r--r--   0 labad      (502) staff       (20)    15996 2021-01-04 16:11:55.000000 pdm_utils-1.0.0/src/pdm_utils/functions/url_basic.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.116294 pdm_utils-1.0.0/src/pdm_utils/pipelines/
--rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/__init__.py
--rwxr-xr-x   0 labad      (502) staff       (20)    60772 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/compare_db.py
--rw-r--r--   0 labad      (502) staff       (20)     8327 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/convert_db.py
--rw-r--r--   0 labad      (502) staff       (20)    33685 2021-09-22 16:59:23.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/export_db.py
--rw-r--r--   0 labad      (502) staff       (20)    26787 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/find_domains.py
--rw-r--r--   0 labad      (502) staff       (20)      972 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/find_membrane.py
--rw-r--r--   0 labad      (502) staff       (20)    14635 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/find_transmembrane.py
--rwxr-xr-x   0 labad      (502) staff       (20)     7930 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/freeze_db.py
--rw-r--r--   0 labad      (502) staff       (20)    37362 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/get_data.py
--rw-r--r--   0 labad      (502) staff       (20)    16273 2021-01-05 20:20:36.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/get_db.py
--rw-r--r--   0 labad      (502) staff       (20)    10665 2020-10-30 13:34:57.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/get_gb_records.py
--rw-r--r--   0 labad      (502) staff       (20)    91298 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/import_genome.py
--rw-r--r--   0 labad      (502) staff       (20)    12771 2021-09-17 01:23:58.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/pham_finder.py
--rw-r--r--   0 labad      (502) staff       (20)    25213 2020-10-30 13:34:57.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/pham_review.py
--rw-r--r--   0 labad      (502) staff       (20)    14262 2021-03-23 03:57:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/phamerate.py
--rw-r--r--   0 labad      (502) staff       (20)     7937 2020-12-13 18:52:56.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/push_db.py
--rw-r--r--   0 labad      (502) staff       (20)    36843 2023-03-09 18:26:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/revise.py
--rw-r--r--   0 labad      (502) staff       (20)     5642 2023-03-09 18:26:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/update_field.py
--rw-r--r--   0 labad      (502) staff       (20)     3347 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/run.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.079292 pdm_utils-1.0.0/src/pdm_utils.egg-info/
--rw-r--r--   0 labad      (502) staff       (20)     1718 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/PKG-INFO
--rw-r--r--   0 labad      (502) staff       (20)     2775 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/SOURCES.txt
--rw-r--r--   0 labad      (502) staff       (20)        1 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/dependency_links.txt
--rw-r--r--   0 labad      (502) staff       (20)      125 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/requires.txt
--rw-r--r--   0 labad      (502) staff       (20)       10 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/top_level.txt
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 20:39:06.641003 pdm_utils-1.0.1/
+-rw-r--r--   0 labad      (502) staff       (20)    35186 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/LICENSE
+-rw-r--r--   0 labad      (502) staff       (20)     1720 2023-06-15 20:39:06.641282 pdm_utils-1.0.1/PKG-INFO
+-rw-r--r--   0 labad      (502) staff       (20)      790 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/README.md
+-rw-r--r--   0 labad      (502) staff       (20)       89 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/pyproject.toml
+-rw-r--r--   0 labad      (502) staff       (20)     1413 2023-06-15 20:39:06.642413 pdm_utils-1.0.1/setup.cfg
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 20:39:06.602948 pdm_utils-1.0.1/src/
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 20:39:06.606074 pdm_utils-1.0.1/src/pdm_utils/
+-rw-r--r--   0 labad      (502) staff       (20)      146 2023-06-15 20:37:17.000000 pdm_utils-1.0.1/src/pdm_utils/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)      114 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/__main__.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 20:39:06.619656 pdm_utils-1.0.1/src/pdm_utils/classes/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)    20060 2020-10-30 13:34:57.000000 pdm_utils-1.0.1/src/pdm_utils/classes/alchemyhandler.py
+-rw-r--r--   0 labad      (502) staff       (20)     8100 2021-09-17 01:24:47.000000 pdm_utils-1.0.1/src/pdm_utils/classes/aragornhandler.py
+-rw-r--r--   0 labad      (502) staff       (20)    10410 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/bundle.py
+-rw-r--r--   0 labad      (502) staff       (20)    39957 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/cds.py
+-rw-r--r--   0 labad      (502) staff       (20)     2461 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/cdspair.py
+-rw-r--r--   0 labad      (502) staff       (20)     9923 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/dbcomparesummary.py
+-rw-r--r--   0 labad      (502) staff       (20)      165 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/classes/error.py
+-rw-r--r--   0 labad      (502) staff       (20)      696 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/evaluation.py
+-rw-r--r--   0 labad      (502) staff       (20)     7966 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/fileio.py
+-rw-r--r--   0 labad      (502) staff       (20)    23716 2021-09-17 01:24:47.000000 pdm_utils-1.0.1/src/pdm_utils/classes/filter.py
+-rw-r--r--   0 labad      (502) staff       (20)    41595 2021-09-22 16:59:23.000000 pdm_utils-1.0.1/src/pdm_utils/classes/genome.py
+-rw-r--r--   0 labad      (502) staff       (20)     5574 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/genomepair.py
+-rw-r--r--   0 labad      (502) staff       (20)    18395 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/genometriad.py
+-rw-r--r--   0 labad      (502) staff       (20)     1124 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/classes/progress.py
+-rw-r--r--   0 labad      (502) staff       (20)     7244 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/randomfieldupdatehandler.py
+-rw-r--r--   0 labad      (502) staff       (20)     4243 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/source.py
+-rw-r--r--   0 labad      (502) staff       (20)     8694 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/ticket.py
+-rw-r--r--   0 labad      (502) staff       (20)    37793 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/tmrna.py
+-rw-r--r--   0 labad      (502) staff       (20)    64069 2021-09-22 15:49:23.000000 pdm_utils-1.0.1/src/pdm_utils/classes/trna.py
+-rw-r--r--   0 labad      (502) staff       (20)     3694 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/classes/trnascansehandler.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 20:39:06.622175 pdm_utils-1.0.1/src/pdm_utils/constants/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/constants/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)     6185 2023-06-15 19:41:31.000000 pdm_utils-1.0.1/src/pdm_utils/constants/constants.py
+-rw-r--r--   0 labad      (502) staff       (20)    10763 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/constants/db_schema_0.py
+-rw-r--r--   0 labad      (502) staff       (20)    12305 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/constants/eval_descriptions.py
+-rw-r--r--   0 labad      (502) staff       (20)    37071 2023-06-15 19:40:19.000000 pdm_utils-1.0.1/src/pdm_utils/constants/schema_conversions.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 20:39:06.631534 pdm_utils-1.0.1/src/pdm_utils/functions/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/functions/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)     6113 2020-10-30 13:34:57.000000 pdm_utils-1.0.1/src/pdm_utils/functions/annotation.py
+-rw-r--r--   0 labad      (502) staff       (20)    45918 2021-01-04 16:11:55.000000 pdm_utils-1.0.1/src/pdm_utils/functions/basic.py
+-rw-r--r--   0 labad      (502) staff       (20)     2962 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/functions/cartography.py
+-rw-r--r--   0 labad      (502) staff       (20)     2182 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/functions/configfile.py
+-rw-r--r--   0 labad      (502) staff       (20)     2853 2023-06-15 19:40:19.000000 pdm_utils-1.0.1/src/pdm_utils/functions/deeptmhmm.py
+-rw-r--r--   0 labad      (502) staff       (20)     4638 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/functions/eval_modes.py
+-rw-r--r--   0 labad      (502) staff       (20)     2301 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/functions/fasta.py
+-rw-r--r--   0 labad      (502) staff       (20)    10526 2021-03-23 03:57:54.000000 pdm_utils-1.0.1/src/pdm_utils/functions/fileio.py
+-rw-r--r--   0 labad      (502) staff       (20)    30706 2021-09-22 16:59:23.000000 pdm_utils-1.0.1/src/pdm_utils/functions/flat_files.py
+-rw-r--r--   0 labad      (502) staff       (20)     2858 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/functions/multiprocess.py
+-rw-r--r--   0 labad      (502) staff       (20)     5299 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/functions/multithread.py
+-rw-r--r--   0 labad      (502) staff       (20)    27400 2022-10-18 17:47:46.000000 pdm_utils-1.0.1/src/pdm_utils/functions/mysqldb.py
+-rw-r--r--   0 labad      (502) staff       (20)    13414 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/functions/mysqldb_basic.py
+-rw-r--r--   0 labad      (502) staff       (20)     6605 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/functions/ncbi.py
+-rw-r--r--   0 labad      (502) staff       (20)    10972 2020-12-29 20:15:44.000000 pdm_utils-1.0.1/src/pdm_utils/functions/parsing.py
+-rw-r--r--   0 labad      (502) staff       (20)    12611 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/functions/phagesdb.py
+-rw-r--r--   0 labad      (502) staff       (20)     8600 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/functions/pham_alignment.py
+-rw-r--r--   0 labad      (502) staff       (20)     9900 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/functions/phameration.py
+-rw-r--r--   0 labad      (502) staff       (20)     8473 2021-01-04 16:11:55.000000 pdm_utils-1.0.1/src/pdm_utils/functions/pipeline_shells.py
+-rw-r--r--   0 labad      (502) staff       (20)     8828 2020-12-28 19:11:26.000000 pdm_utils-1.0.1/src/pdm_utils/functions/pipelines_basic.py
+-rw-r--r--   0 labad      (502) staff       (20)    30269 2021-09-17 01:24:47.000000 pdm_utils-1.0.1/src/pdm_utils/functions/querying.py
+-rw-r--r--   0 labad      (502) staff       (20)     6325 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/functions/rpsblast.py
+-rw-r--r--   0 labad      (502) staff       (20)     3475 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/functions/server.py
+-rw-r--r--   0 labad      (502) staff       (20)      978 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/functions/subprocess.py
+-rw-r--r--   0 labad      (502) staff       (20)    11826 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/functions/tickets.py
+-rw-r--r--   0 labad      (502) staff       (20)    15996 2021-01-04 16:11:55.000000 pdm_utils-1.0.1/src/pdm_utils/functions/url_basic.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 20:39:06.639710 pdm_utils-1.0.1/src/pdm_utils/pipelines/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/__init__.py
+-rwxr-xr-x   0 labad      (502) staff       (20)    60772 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/compare_db.py
+-rw-r--r--   0 labad      (502) staff       (20)     8327 2023-06-15 19:40:19.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/convert_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    33685 2021-09-22 16:59:23.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/export_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    17323 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/find_domains.py
+-rw-r--r--   0 labad      (502) staff       (20)      972 2023-06-15 19:40:19.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/find_membrane.py
+-rw-r--r--   0 labad      (502) staff       (20)    14635 2023-06-15 19:40:19.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/find_transmembrane.py
+-rwxr-xr-x   0 labad      (502) staff       (20)     7930 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/freeze_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    37362 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/get_data.py
+-rw-r--r--   0 labad      (502) staff       (20)    16273 2021-01-05 20:20:36.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/get_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    10665 2020-10-30 13:34:57.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/get_gb_records.py
+-rw-r--r--   0 labad      (502) staff       (20)    91016 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/import_genome.py
+-rw-r--r--   0 labad      (502) staff       (20)    12771 2021-09-17 01:23:58.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/pham_finder.py
+-rw-r--r--   0 labad      (502) staff       (20)    25213 2020-10-30 13:34:57.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/pham_review.py
+-rw-r--r--   0 labad      (502) staff       (20)    10125 2023-06-15 19:38:37.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/phamerate.py
+-rw-r--r--   0 labad      (502) staff       (20)     7937 2020-12-13 18:52:56.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/push_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    36843 2023-06-15 19:40:19.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/revise.py
+-rw-r--r--   0 labad      (502) staff       (20)     5642 2023-06-15 19:40:19.000000 pdm_utils-1.0.1/src/pdm_utils/pipelines/update_field.py
+-rw-r--r--   0 labad      (502) staff       (20)     3494 2023-06-15 19:40:19.000000 pdm_utils-1.0.1/src/pdm_utils/run.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 20:39:06.608642 pdm_utils-1.0.1/src/pdm_utils.egg-info/
+-rw-r--r--   0 labad      (502) staff       (20)     1720 2023-06-15 20:39:06.000000 pdm_utils-1.0.1/src/pdm_utils.egg-info/PKG-INFO
+-rw-r--r--   0 labad      (502) staff       (20)     3023 2023-06-15 20:39:06.000000 pdm_utils-1.0.1/src/pdm_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 labad      (502) staff       (20)        1 2023-06-15 20:39:06.000000 pdm_utils-1.0.1/src/pdm_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 labad      (502) staff       (20)       54 2023-06-15 20:39:06.000000 pdm_utils-1.0.1/src/pdm_utils.egg-info/entry_points.txt
+-rw-r--r--   0 labad      (502) staff       (20)      160 2023-06-15 20:39:06.000000 pdm_utils-1.0.1/src/pdm_utils.egg-info/requires.txt
+-rw-r--r--   0 labad      (502) staff       (20)       10 2023-06-15 20:39:06.000000 pdm_utils-1.0.1/src/pdm_utils.egg-info/top_level.txt
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 20:39:06.640663 pdm_utils-1.0.1/tests/
+-rw-r--r--   0 labad      (502) staff       (20)    20144 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/tests/test_data_utils.py
+-rw-r--r--   0 labad      (502) staff       (20)    15441 2020-10-23 17:14:54.000000 pdm_utils-1.0.1/tests/test_db_utils.py
```

### Comparing `pdm_utils-1.0.0/PKG-INFO` & `pdm_utils-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: pdm_utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: MySQL phage genomics database management utilities
 Home-page: https://github.com/SEA-PHAGES/pdm_utils
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
-License: UNKNOWN
 Project-URL: Documentation, https://pdm-utils.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/SEA-PHAGES/pdm_utils/
-Description: # README #
-        
-        ### Purpose: ###
-        
-        * The pdm_utils repository provides the source code for pdm_utils Python package, developed in the SEA-PHAGES program to create, update, and maintain MySQL phage genomics databases.
-        
-        The source code is available on GitHub at https://github.com/SEA-PHAGES/pdm_utils/.
-        
-        The user guide for the package is available on ReadTheDocs at https://pdm-utils.readthedocs.io/en/latest/.
-        
-        The pdm_utils Python package is available on PyPI at https://pypi.org/project/pdm-utils/.
-        
-        ### Contribution guidelines: ###
-        
-        * Please contact us if you have any contributions or suggestions. Details about how to contribute can be found on the user guide.
-        
-        ### Developers: ###
-        
-        * Travis Mavrich (trm53@pitt.edu) and Christian Gauthier (christian.gauthier@pitt.edu).
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Database
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# README #
+
+### Purpose: ###
+
+* The pdm_utils repository provides the source code for pdm_utils Python package, developed in the SEA-PHAGES program to create, update, and maintain MySQL phage genomics databases.
+
+The source code is available on GitHub at https://github.com/SEA-PHAGES/pdm_utils/.
+
+The user guide for the package is available on ReadTheDocs at https://pdm-utils.readthedocs.io/en/latest/.
+
+The pdm_utils Python package is available on PyPI at https://pypi.org/project/pdm-utils/.
+
+### Contribution guidelines: ###
+
+* Please contact us if you have any contributions or suggestions. Details about how to contribute can be found on the user guide.
+
+### Developers: ###
+
+* Travis Mavrich (trm53@pitt.edu) and Christian Gauthier (christian.gauthier@pitt.edu).
```

### Comparing `pdm_utils-1.0.0/README.md` & `pdm_utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/alchemyhandler.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/alchemyhandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/aragornhandler.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/aragornhandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/bundle.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/bundle.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/cds.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/cds.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/cdspair.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/cdspair.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/dbcomparesummary.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/dbcomparesummary.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/evaluation.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/evaluation.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/fileio.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/fileio.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/filter.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/filter.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/genome.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/genome.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/genomepair.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/genomepair.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/genometriad.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/genometriad.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/progressbar.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/progress.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,37 @@
+"""Class for easy visualization of progress level for multiprocessing
+or multithreading."""
+
+
 class ProgressBar:
+    """Inline-updatable progress bar."""
     def __init__(self, current, end, width=50):
         self._percent = int(float(current) / end * 100)
         self._width = int(width)
-        self._width_ratio = int(100 / width)
-        self._multiplier = int(self._percent / self._width_ratio)
-        self._padding = self._width - self._multiplier
+        self._ratio = int(100 / width)
+        self._multi = int(self._percent / self._ratio)
+        self._pad = self._width - self._multi
+
+    def show(self):
+        """Print ProgressBar to the console."""
+        if self._percent < 100:
+            print("\r" + str(self), end="")
+        else:
+            print("\r" + str(self))
 
     def __str__(self):
-        s = f"[{'#' * self._multiplier}{' ' * self._padding}] {self._percent}%"
+        s = f"[{'#' * self._multi}{' ' * self._pad}] {self._percent}%"
         return s
 
 
 def show_progress(current, end, width=50):
-    """
-    Creates a ProgressBar instance and prints it in-line if
-    current < end. If current == end, prints with newline.
+    """Create an instance of ProgressBar and print it in-line.
+
     :param current: current step (1 through n)
     :type current: int
     :param end: number of steps (n)
     :type end: int
     :param width: character width for the progressbar
     :type width: int
     :return: progressbar
     """
-    progressbar = ProgressBar(current, end, width)
-    if current < end:
-        print(f"\r{progressbar}", end="")
-    else:
-        print(f"\r{progressbar}")
+    ProgressBar(current, end, width).show()
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/randomfieldupdatehandler.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/randomfieldupdatehandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/source.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/source.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/ticket.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/ticket.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/tmrna.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/tmrna.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/trna.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/trna.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/classes/trnascansehandler.py` & `pdm_utils-1.0.1/src/pdm_utils/classes/trnascansehandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/constants/constants.py` & `pdm_utils-1.0.1/src/pdm_utils/constants/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Collection of constants and dictionaries used for maintaining the phage
 database."""
 
 from Bio.Alphabet import IUPAC
 from Bio.Seq import Seq
 from datetime import datetime, date
-from pathlib import Path
 
-# pdm_utils is compatibile with this schema version.
 CODE_SCHEMA_VERSION = 11
 
 CURRENT_DATE = date.today().strftime("%Y%m%d")
 
 IMPORT_TABLE_STRUCTURE = {
     "order": [
                     "type",
@@ -67,16 +65,16 @@
                     "host_genus",
                     "accession"},
     "keywords": {"parse", "retrieve", "retain", "none"}
 }
 
 NAME_SUFFIX = "_Draft"
 ANNOTATION_STATUS_SET = {"draft", "final", "unknown"}
-ANNOTATION_AUTHOR_SET = {0,1}
-RETRIEVE_RECORD_SET = {0,1}
+ANNOTATION_AUTHOR_SET = {0, 1}
+RETRIEVE_RECORD_SET = {0, 1}
 EMPTY_DATE = datetime.strptime("1/1/0001 00:00:00", "%m/%d/%Y %H:%M:%S")
 
 # Some locus tags have "PHIRE", but this should not be the case.
 LOCUS_TAG_PREFIX_SET = {"SEA", "PBI"}
 EMPTY_GENOME_SEQ = Seq("", IUPAC.ambiguous_dna)
 EMPTY_PROTEIN_SEQ = Seq("", IUPAC.protein)
 
@@ -117,27 +115,17 @@
 # Settings to access data through the PhagesDB API.
 API_PREFIX = "https://phagesdb.org/api/phages/"
 API_SUFFIX = "/?format=json"
 API_HOST_GENERA = "https://phagesdb.org/api/host_genera/"
 API_CLUSTERS = "https://phagesdb.org/api/clusters/"
 
 # API at PhagesDB has you specify how many results to return.
-# 1 page at length 100000 will return everything.
-SEQUENCED_PAGE = 1
-SEQUENCED_SIZE = 100000
+# 1 page at length 7500 will return everything for a few years.
 API_SEQUENCED = ("https://phagesdb.org/api/sequenced_phages/"
-                 f"?page={SEQUENCED_PAGE}"
-                 f"&page_size={SEQUENCED_SIZE}")
-
-
-# TODO this may no longer be needed, now that get_data pipeline
-# determines which new genomes to retrieve based on the
-# MySQL database instance instead of PhagesDB.
-UNPHAMERATED_PHAGE_LIST = "https://phagesdb.org/data/unphameratedlist"
-
+                 f"?page=1&page_size=7500")
 
 # Auto-annotations from PECAAN
 PECAAN_PREFIX = "https://discover.kbrinsgd.org/phameratoroutput/phage/"
 
 
 # Phage name typo correction dictionary.
 # Key = Phage name as it is spelled in the GenBank-formatted record.
@@ -151,15 +139,15 @@
     "ATCC29399B_C": "ATCC29399BC",
     "ATCC29399B_T": "ATCC29399BT",
 
     # Names are spelled differently in GenBank record compared to
     # the original publication.
     "P100_1": "P100.1",
     "P100_A": "P100A",
-    "P14":"P14.4",
+    "P14": "P14.4",
     "phiELB20": "ELB20",
     "ZL12": "pZL12",
 
     # 'LeBron' was changed to 'Bron' by ICTV. They won't change it back.
     "Bron": "LeBron",
 
     # Inadvertent typos introduced at some point that GenBank won't
@@ -196,14 +184,9 @@
     "ReqiPoco6": "Poco6",
     "ReqiPine5": "Pine5",
     "vB_ArtM-ArV1": "ArV1",
     "vB_ArS-ArV2": "ArV2",
     "vB_MoxS-ISF9": "ISF9"
     }
 
-# TODO HOST_GENUS_DICT may no longer be needed.
-# List of host_genus synonyms.
-HOST_GENUS_SYNONYMS = [{"Mycobacterium", "Mycobacterio", "Mycolicibacterium"}]
-
 # Hatfull lab server info
-DB_WEBSITE = "http://phamerator.webfactional.com/databases_Hatfull/"
 DB_SERVER = "http://databases.hatfull.org/"
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils/constants/db_schema_0.py` & `pdm_utils-1.0.1/src/pdm_utils/constants/db_schema_0.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/constants/eval_descriptions.py` & `pdm_utils-1.0.1/src/pdm_utils/constants/eval_descriptions.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/constants/schema_conversions.py` & `pdm_utils-1.0.1/src/pdm_utils/constants/schema_conversions.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/annotation.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/annotation.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/basic.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/cartography.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/cartography.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/configfile.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/configfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 """Configuration file definition and parsing."""
 
 import configparser
-import pathlib
 import sys
 
 from pdm_utils.functions import basic
 
+
 def default_sections_keys():
-    dict = {"mysql": {"user", "password"},
-            "mysqldump": {"user", "password"},
-            "ncbi": {"api_key", "email", "tool"},
-            "upload_server": {"host", "dest", "user", "password"},
-            "download_server": {"url"},
-            "emailer": {"username", "password"}
-            }
-    return dict
+    sections = {"mysql": {"user", "password"},
+                "mysqldump": {"user", "password"},
+                "ncbi": {"api_key", "email", "tool"},
+                "upload_server": {"host", "dest", "user", "password"},
+                "download_server": {"url"},
+                "emailer": {"username", "password"}}
+    return sections
+
 
 def setup_section(keys, value):
-    dict = {}
+    section = {}
     for key in keys:
-        dict[key] = value
-    return dict
+        section[key] = value
+    return section
+
 
 def default_parser(null_value):
     """Constructs complete config with empty values."""
     # Need to allow no value if the null value is None.
     null_parser = configparser.ConfigParser(allow_no_value=True)
     all_configs = default_sections_keys()
     for key in all_configs.keys():
         null_parser[key] = setup_section(all_configs[key], null_value)
     return null_parser
 
+
 def parse_config(file, parser=None):
     """Get parameters from config file."""
     filepath = basic.set_path(file, kind="file", expect=True)
     if parser is None:
         parser = configparser.ConfigParser()
 
     try:
         parser.read(filepath)
     except:
         print("Unable to parse config file")
         sys.exit(1)
     else:
         return parser
 
+
 def build_complete_config(file):
     "Buid a complete config object by merging user-supplied and default config."
     parser = default_parser(None)
     if file is not None:
         parser = parse_config(file, parser)
     return parser
 
+
 def write_config(parser, filepath):
     """Write a ConfigParser to file."""
     with filepath.open("w") as fh:
         parser.write(fh)
 
+
 def create_empty_config_file(dir, file, null_value):
     """Create an empty config file with all available settings."""
     output_path = basic.set_path(dir, kind="dir", expect=True)
     config_path = basic.make_new_file(output_path, file, "txt", attempt=50)
     if config_path is None:
         print("Unable to create config file. File already exists.")
     else:
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/deeptmhmm.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/deeptmhmm.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/eval_modes.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/eval_modes.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/fileio.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/fileio.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/flat_files.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/flat_files.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/multithread.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/multithread.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Functions to multithread process a list of inputs.
 """
 
 from queue import Queue
 import time
 import threading
 
-from pdm_utils.classes.progressbar import ProgressBar, show_progress
+from pdm_utils.classes.progress import ProgressBar, show_progress
 
 
 class MixedThread(threading.Thread):
     def __init__(self, thread_id, work_queue, work_lock,
                  result_queue, result_lock, lock_timeout=-1,
                  kill_sig=None):
         threading.Thread.__init__(self)
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/mysqldb.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/mysqldb.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/mysqldb_basic.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/mysqldb_basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/ncbi.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/ncbi.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/parsing.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/parsing.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/phagesdb.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/phagesdb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Functions to interact with PhagesDB"""
 
 import json
 import pathlib
-import urllib.request
+from urllib import request, error
 
 from pdm_utils.classes import genome
 from pdm_utils.constants import constants
 
+
 def parse_phage_name(data_dict):
     """Retrieve Phage Name from PhagesDB.
 
     :param data_dict: Dictionary of data retrieved from PhagesDB.
     :type data_dict: dict
     :returns: Name of the phage.
     :rtype: str
     """
     try:
         phage_name = data_dict["phage_name"]
-    except:
+    except KeyError:
         phage_name = ""
     return phage_name
 
 
 def parse_cluster(data_dict):
     """Retrieve Cluster from PhagesDB.
 
@@ -40,15 +41,15 @@
     :rtype: str
     """
     try:
         if data_dict["pcluster"] is None:
             cluster = "UNK"
         else:
             cluster = data_dict["pcluster"]["cluster"]
-    except:
+    except KeyError:
         cluster = ""
     return cluster
 
 
 def parse_subcluster(data_dict):
     """Retrieve Subcluster from PhagesDB.
 
@@ -66,60 +67,60 @@
     :rtype: str
     """
     try:
         if data_dict["psubcluster"] is None:
             subcluster = "none"
         else:
             subcluster = data_dict["psubcluster"]["subcluster"]
-    except:
+    except KeyError:
         subcluster = ""
     return subcluster
 
 
 def parse_host_genus(data_dict):
     """Retrieve host_genus from PhagesDB.
 
     :param data_dict: Dictionary of data retrieved from PhagesDB.
     :type data_dict: dict
     :returns: Host genus of the phage.
     :rtype: str
     """
     try:
         host_genus = data_dict["isolation_host"]["genus"]
-    except:
+    except KeyError:
         host_genus = ""
     return host_genus
 
 
 def parse_accession(data_dict):
     """Retrieve Accession from PhagesDB.
 
     :param data_dict: Dictionary of data retrieved from PhagesDB.
     :type data_dict: dict
     :returns: Accession of the phage.
     :rtype: str
     """
     try:
         accession = data_dict["genbank_accession"]
-    except:
+    except KeyError:
         accession = ""
     return accession
 
 
 def parse_fasta_filename(data_dict):
     """Retrieve fasta filename from PhagesDB.
 
     :param data_dict: Dictionary of data retrieved from PhagesDB.
     :type data_dict: dict
     :returns: Name of the fasta file for the phage.
     :rtype: str
     """
     try:
         fastafile_url = data_dict["fasta_file"]
-    except:
+    except KeyError:
         fastafile_url = ""
     return fastafile_url
 
 
 def retrieve_url_data(url):
     """Retrieve fasta file from PhagesDB.
 
@@ -130,19 +131,19 @@
     """
     try:
         # gcontext = ssl.SSLContext(ssl.PROTOCOL_TLSv1) ==> required for
         # urllib2.URLError: <urlopen error [SSL: CERTIFICATE_VERIFY_FAILED]
         # certificate verify failed (_ssl.c:590)> ==> creating new TLS
         # context tells urllib2 to ignore certificate chain
         # NOTE this is BAD SECURITY, prone to man-in-the-middle attacks
-        request = urllib.request.Request(url)
-        with urllib.request.urlopen(request) as response:
+        rqst = request.Request(url)
+        with request.urlopen(rqst) as response:
             data = response.read()
             data = data.decode("utf-8")
-    except:
+    except error.HTTPError:
         print(f"Unable to retrieve data from {url}")
         data = ""
     return data
 
 
 def parse_fasta_data(fasta_data):
     """Parses data returned from a fasta-formatted file.
@@ -161,20 +162,20 @@
     # the header is retained in the first list element.
     split_fasta_data = fasta_data.split('\n')
     header = ""
     sequence = ""
     if len(split_fasta_data) > 1:
         header = split_fasta_data[0]
         if header[0] == ">":
-            header = header[1:] # Remove '>' symbol.
-        header = header.strip() # Remove any whitespace
+            header = header[1:]  # Remove '>' symbol.
+        header = header.strip()  # Remove any whitespace
         for index in range(1, len(split_fasta_data)):
             # Strip off potential whitespace before appending, such as '\r'.
             sequence = sequence + split_fasta_data[index].strip()
-    return (header, sequence)
+    return header, sequence
 
 
 def parse_genome_data(data_dict, gnm_type="", seq=False):
     """Parses a dictionary of PhagesDB genome data into a pdm_utils Genome object.
 
     :param data_dict: Dictionary of data retrieved from PhagesDB.
     :type data_dict: dict
@@ -201,53 +202,54 @@
     accession = parse_accession(data_dict)
     gnm.set_accession(accession, "empty_string")
 
     # Cluster
     cluster = parse_cluster(data_dict)
     gnm.set_cluster(cluster)
 
-    #Subcluster
+    # Subcluster
     subcluster = parse_subcluster(data_dict)
     gnm.set_subcluster(subcluster)
 
     # Fasta file URL
     fastafile_url = parse_fasta_filename(data_dict)
     fastafile_url_path = pathlib.Path(fastafile_url)
     gnm.set_filename(fastafile_url_path)
 
     # Fasta file record
     # if fastafile_url != "":
-    if (fastafile_url != "" and seq == True):
+    if fastafile_url != "" and seq is True:
         fasta_file = retrieve_url_data(fastafile_url)
 
         # TODO unit test - not sure how to test this, since this function
         # retrieves and parses files from PhagesDB.
         # Genome sequence and parsed record
         if fasta_file != "":
             header, seq = parse_fasta_data(fasta_file)
             gnm.set_sequence(seq)
             gnm.description = header
             gnm.parse_description()
 
     gnm.misc = data_dict
     return gnm
 
+
 def retrieve_genome_data(phage_url):
     """Retrieve all data from PhagesDB for a specific phage.
 
     :param phage_url: URL for data pertaining to a specific phage.
     :type phage_url: str
     :returns: Dictionary of data parsed from the URL.
     :rtype: dict
     """
     try:
-        data_json = urllib.request.urlopen(phage_url)
+        data_json = request.urlopen(phage_url)
         data_dict = json.loads(data_json.read())
         # TODO should data_dict.close() be called after retrieving data?
-    except:
+    except error.HTTPError:
         data_dict = {}
     return data_dict
 
 
 def construct_phage_url(phage_name):
     """Create URL to retrieve phage-specific data from PhagesDB.
 
@@ -291,15 +293,15 @@
     :type url: str
     :returns:
         List of dictionaries, where each dictionary contains
         data for each phage. If a problem is encountered during retrieval,
         an empty list is returned.
     :rtype: list
     """
-    data_json = urllib.request.urlopen(url)
+    data_json = request.urlopen(url)
     # Response is a bytes object that json.loads can't read without first
     # being decoded to a UTF-8 string.
     data_dict = json.loads(data_json.read().decode("utf-8"))
     data_json.close()
 
     # Returned dict:
     # Keys:
@@ -336,49 +338,47 @@
     genome_dict = {}
     for key in data_dict.keys():
         gnm = parse_genome_data(data_dict[key], gnm_type=gnm_type, seq=seq)
         genome_dict[gnm.id] = gnm
     return genome_dict
 
 
-
-
 def retrieve_data_list(url):
     """Retrieve list of data from PhagesDB.
 
     :param url: A URL from which to retrieve data.
     :type url: str
     :returns: A list of data retrieved from the URL.
     :rtype: list
     """
     try:
-        data_json = urllib.request.urlopen(url)
+        data_json = request.urlopen(url)
         data_list = json.loads(data_json.read())
-    except:
+    except error.HTTPError:
         data_list = []
     return data_list
 
 
 def create_host_genus_set(url=constants.API_HOST_GENERA):
     """Create a set of host genera currently in PhagesDB.
 
     :param url: A URL from which to retrieve host genus data.
     :type url: str
     :returns: All unique host genera listed on PhagesDB.
     :rtype: set
     """
     try:
         output = retrieve_data_list(url)
-    except:
+    except error.HTTPError:
         output = []
     host_genera_set = set()
     for genus_dict in output:
         try:
             host_genera_set.add(genus_dict["genus_name"])
-        except:
+        except KeyError:
             pass
     return host_genera_set
 
 
 def create_cluster_subcluster_sets(url=constants.API_CLUSTERS):
     """Create sets of clusters and subclusters currently in PhagesDB.
 
@@ -389,45 +389,22 @@
         WHERE
         cluster_set(set) is a set of all unique clusters on PhagesDB.
         subcluster_set(set) is a set of all unique subclusters on PhagesDB.
     :rtype: tuple
     """
     try:
         output = retrieve_data_list(url)
-    except:
+    except error.HTTPError:
         output = []
     cluster_set = set()
     subcluster_set = set()
     for data in output:
         try:
-            cluster_set.add(data["cluster"]) # This set contains 'Singleton'.
+            cluster_set.add(data["cluster"])  # This set contains 'Singleton'.
             try:
                 subclusters_list = data["subclusters_set"]
                 subcluster_set = subcluster_set | set(subclusters_list)
-            except:
+            except KeyError:
                 pass
-        except:
+        except KeyError:
             pass
-    return (cluster_set, subcluster_set)
-
-
-# TODO unittest.
-def get_unphamerated_phage_list(url):
-    """Retreive list of unphamerated phages from PhagesDB.
-
-    :param url:
-        A URL from which to retrieve a list of PhagesDB genomes that are not
-        in the most up-to-date instance of the Actino_Draft
-        MySQL database.
-    :type url: str
-    :returns: List of PhageIDs.
-    :rtype: list
-    """
-    # Retrieved file is a tab-delimited text file.
-    # Each row is a newly-sequenced phage.
-    response = urllib.request.urlopen(url)
-    processed_list = []
-    for new_phage in response:
-        new_phage = new_phage.strip()  # Remove \t at end of each row
-        new_phage = new_phage.decode("utf-8")  # convert bytes object to str
-        processed_list.append(new_phage)
-    return processed_list
+    return cluster_set, subcluster_set
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/pham_alignment.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/pham_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import shlex
 from subprocess import (Popen, DEVNULL)
 
-from pdm_utils.functions import (fileio, multithread, parallelize)
+from pdm_utils.functions import (fileio, multithread, multiprocess)
 
 
 THREAD_LOCK_TIMEOUT = 10
 THREAD_JOIN_TIMEOUT = 30
 
 
 def run_clustalo(fasta_path, aln_path):
@@ -176,15 +176,16 @@
         aln_name = filepath.with_suffix(".aln").name
         aln_path = working_dir.joinpath(aln_name)
 
         pham_aln_map[pham] = aln_path
 
         work_items.append((filepath, aln_path))
 
-    parallelize.parallelize(work_items, threads, run_clustalo, verbose=verbose)
+    multiprocess.parallelize(work_items, threads, run_clustalo,
+                             verbose=verbose)
 
     return pham_aln_map
 
 
 def reintroduce_pham_fasta_duplicates(pham_path_map, pham_translations_dict,
                                       threads=1, verbose=False):
     """Uses multiple threads to read and re-write fasta-formatted sequence
@@ -216,16 +217,16 @@
 # of the above functions
 def write_phams(fasta_dir, aln_dir, phams_translations_dict, cores=1,
                 verbose=False):
     work_items = []
     for pham, pham_translations in phams_translations_dict.items():
         work_items.append((fasta_dir, aln_dir, pham, pham_translations))
 
-    parallelize.parallelize(work_items, cores, write_phams_process,
-                            verbose=verbose)
+    multiprocess.parallelize(work_items, cores, write_phams_process,
+                             verbose=verbose)
 
 
 def write_phams_process(fasta_dir, aln_dir, pham, pham_translations):
     fasta_path = fasta_dir.joinpath("".join([str(pham), "_genes.fasta"]))
     aln_path = aln_dir.joinpath("".join([str(pham), "_genes.aln"]))
 
     gs_to_ts = {}
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/pipeline_shells.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/pipeline_shells.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/pipelines_basic.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/pipelines_basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/querying.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/querying.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/server.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/server.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/tickets.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/tickets.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/functions/url_basic.py` & `pdm_utils-1.0.1/src/pdm_utils/functions/url_basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/compare_db.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/compare_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/convert_db.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/convert_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/export_db.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/export_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/find_domains.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/pham_review.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,712 +1,694 @@
+"""Pipeline to review discrepant or outdated cds product annotations. """
+
 import argparse
-import logging
-import os
-import pathlib
-import platform
-import shlex
 import sys
-from subprocess import Popen, PIPE # import warnings
+import textwrap
+import time
+from pathlib import Path
 
-from Bio.Blast import NCBIXML
-from Bio.Blast.Applications import NcbirpsblastCommandline
-import sqlalchemy
-
-import pdm_utils
-from pdm_utils.classes.alchemyhandler import AlchemyHandler
-from pdm_utils.constants import constants
+from pdm_utils.functions import annotation
 from pdm_utils.functions import basic
 from pdm_utils.functions import configfile
-from pdm_utils.functions import mysqldb
+from pdm_utils.functions import fileio
 from pdm_utils.functions import mysqldb_basic
-from pdm_utils.functions.basic import expand_path
-from pdm_utils.functions.parallelize import *
+from pdm_utils.functions import pipelines_basic
+from pdm_utils.functions import querying
+
+# -----------------------------------------------------------------------------
+# GLOBAL VARIABLES
+
+DEFAULT_FOLDER_NAME = f"{time.strftime('%Y%m%d')}_pham_review"
+
+REVIEW_HEADER = ["Pham", "Final Call", "#Members", "Clusters", "#Functions",
+                 "Functional Calls"]
+GR_HEADER = ["Gene",
+             "Phage",
+             "Gene#",
+             "Cluster",
+             "Subcluster",
+             "Functional Call",
+             "Translation"]
+
+REVIEW_DATA_COLUMNS = ["gene.GeneID", "phage.Cluster"]
+GR_DATA_COLUMNS = ["phage.PhageID", "gene.Name", "phage.Cluster",
+                   "phage.Subcluster", "gene.Notes", "gene.Translation"]
+
+BASE_CONDITIONALS = ("phage.Status = final AND "
+                     "phage.AnnotationAuthor = 1 AND "
+                     "phage.RetrieveRecord = 1")
+
+# -----------------------------------------------------------------------------
+# MAIN FUNCTIONS
+
+
+def main(unparsed_args_list):
+    """Uses parsed args to run the entirety of the pham_review pipeline.
 
-# SQL QUERIES
-GET_GENES_FOR_CDD = (
-    "SELECT GeneID, CONVERT(Translation USING utf8) as Translation "
-    "FROM gene WHERE DomainStatus = 0")
-GET_UNIQUE_HIT_IDS = "SELECT HitID FROM domain"
-
-# SQL COMMANDS
-INSERT_INTO_DOMAIN = (
-    """INSERT INTO domain (HitID, DomainID, Name, Description) """
-    """VALUES ("{}", "{}", "{}", "{}")""")
-
-INSERT_INTO_GENE_DOMAIN = (
-    """INSERT INTO gene_domain """
-    """(GeneID, HitID, Expect, QueryStart, QueryEnd) """
-    """VALUES ("{}", "{}", {}, {}, {})""")
-
-UPDATE_GENE = "UPDATE gene SET DomainStatus = 1 WHERE GeneID = '{}'"
-
-CLEAR_GENE_DOMAIN = "TRUNCATE gene_domain"
-CLEAR_DOMAIN = "DELETE FROM domain"
-CLEAR_GENE_DOMAINSTATUS = "UPDATE gene SET DomainStatus = 0"
-
-
-
-# MISC
-VERSION = pdm_utils.__version__
-
-# TODO tmp dir stores rpsblast output, while output folder stores logged info
-# about the find_domains pipeline. These two directories could possibly be
-# combined, so that all tmp dir automatically gets created within output folder
-# beside the results folder, or something like that.
-DEFAULT_TMP_DIR = "/tmp/find_domains"
-DEFAULT_OUTPUT_FOLDER = os.getcwd()
-RESULTS_FOLDER = f"{constants.CURRENT_DATE}_find_domains"
-MAIN_LOG_FILE = "find_domains.log"
-DEFAULT_CDD = "~/Databases/Cdd_LE"
-
-# LOGGING
-# Add a logger named after this module. Then add a null handler, which
-# suppresses any output statements. This allows other modules that call this
-# module to define the handler and output formats. If this module is the
-# main module being called, the top level main function configures
-# the root logger and primary file handle.
-logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
-
-
-def setup_argparser():
-    """
-    Builds argparse.ArgumentParser for this script
-    :return:
-    """
-    # Pipeline description
-    description = (
-        "Uses rpsblast to search the NCBI conserved domain database "
-        "for significant domain hits in all new proteins of a "
-        "MySQL database.")
-    output_folder_help = (
-        "Directory where log data can be generated.")
-    reset_help = (
-        "Clear all domain data in the database before finding domains.")
-    cdd_help = (
-        "Path to local NCBI Conserved Domain Database. "
-        f"Default is {DEFAULT_CDD}.")
-    config_file_help = (
-        "Path to the file containing user-specific login data.")
-
-    # Initialize parser and add arguments
-    parser = argparse.ArgumentParser(description=description)
-    parser.add_argument("database", type=str,
-                        help="name of database to find conserved domains for")
-    parser.add_argument("-d", "--cdd", type=str, default=DEFAULT_CDD,
-                        help=cdd_help)
-    parser.add_argument("-t", "--threads", default=mp.cpu_count(), type=int,
-                        help="number of concurrent CDD searches to run")
-    parser.add_argument("-e", "--evalue", default=0.001, type=float,
-                        help="evalue cutoff for rpsblast(+) hits")
-    parser.add_argument("-td", "--tmp_dir", default=DEFAULT_TMP_DIR, type=str,
-                        help="path to temporary directory for file I/O")
-    parser.add_argument("-r", "--rpsblast", default="", type=str,
-                        help="path to rpsblast(+) binary")
-    parser.add_argument("-o", "--output_folder", type=pathlib.Path,
-                        default=pathlib.Path(DEFAULT_OUTPUT_FOLDER),
-                        help=output_folder_help)
-    parser.add_argument("-b", "--batch_size", default=10000, type=int,
-                        help="number of translations to search at a time")
-    parser.add_argument("-x", "--reset", action="store_true",
-                        default=False, help=reset_help)
-    parser.add_argument("-c", "--config_file", type=pathlib.Path,
-                        help=config_file_help, default=None)
-
-    return parser
-
-
-def make_tempdir(tmp_dir):
-    """
-    Uses pdm_utils.functions.basic.expand_path to expand TMP_DIR; then
-    checks whether tmpdir exists - if it doesn't, uses os.makedirs to
-    make it recursively.
-    :param tmp_dir: location where I/O should take place
-    :return:
-    """
-    try:
-        path = expand_path(tmp_dir)
-        # If the path doesn't exist yet
-        if not os.path.exists(path):
-            # Make it recursively
-            os.makedirs(path)
-    except OSError as err:
-        print(f"Error {err.args[0]}: {err.args[1]}")
-
-
-def search_and_process(rpsblast, cdd_name, tmp_dir, evalue,
-                       translation_id, translation):
-    """
-    Uses rpsblast to search indicated gene against the indicated CDD
-    :param rpsblast: path to rpsblast binary
-    :param cdd_name: CDD database path/name
-    :param tmp_dir: path to directory where I/O will take place
-    :param evalue: evalue cutoff for rpsblast
-    :param translation_id: unique identifier for the translation sequence
-    :param translation: protein sequence for gene to query
-    :return: results
-    """
-    # Currently translation_id is used only for file formatting.
-    # Setup I/O variables
-    i = "{}/{}.txt".format(tmp_dir, translation_id)
-    o = "{}/{}.xml".format(tmp_dir, translation_id)
-
-    # Write the input file
-    with open(i, "w") as fh:
-        fh.write(">{}\n{}".format(translation_id, translation))
-
-    # Setup, run the rpsblast command, and process results
-    rps_command = NcbirpsblastCommandline(cmd=rpsblast, db=cdd_name,
-                                          query=i, out=o, outfmt=5,
-                                          evalue=evalue)
-    rps_command()
-    data = process_rps_output(o, evalue)
-
-    # Currently need to return as a list due to a
-    # filter in parallelize.start_processes()
-    results = [{"Translation": translation, "Data": data}]
-    return results
-
-
-def process_rps_output(filepath, evalue):
-    """Process rpsblast output and return list of dictionaries."""
-    results = []
-    with open(filepath, "r") as fh:
-        for record in NCBIXML.parse(fh):
-            for align in record.alignments:
-                des, d_id, name = process_align(align)
-                for hsp in align.hsps:
-                    if hsp.expect <= evalue:
-                        dict = {"HitID": align.hit_id,
-                                "DomainID": d_id,
-                                "Name": name,
-                                "Description": des,
-                                "Expect": float(hsp.expect),
-                                "QueryStart": int(hsp.query_start),
-                                "QueryEnd": int(hsp.query_end)}
-                        results.append(dict)
-    return results
-
-
-def process_align(align):
-    """Process alignment data.
-
-    Returns description, domain_id, and name.
-    """
-    align.hit_def = align.hit_def.replace("\"", "\'")
-    des_list = align.hit_def.split(",")
-    if len(des_list) == 1:
-        description = des_list[0].strip()
-        domain_id = None
-        name = None
-    elif len(des_list) == 2:
-        domain_id = des_list[0].strip()
-        description = des_list[1].strip()
-        name = None
+    :param unparsed_args_list: Input a list of command line args.
+    :type unparsed_args_list: list[str]
+    """
+    args = parse_pham_review(unparsed_args_list)
+
+    config = configfile.build_complete_config(args.config_file)
+
+    alchemist = pipelines_basic.build_alchemist(args.database, config=config)
+
+    values = pipelines_basic.parse_value_input(args.input)
+
+    if not args.all_reports:
+        gr_reports = args.gene_reports
+        s_report = args.summary_report
+        psr_reports = args.pham_summary_reports
     else:
-        domain_id = des_list[0].strip()
-        name = des_list[1].strip()
-        # Name is occassionally longer than permitted
-        # in the database. Truncating avoids a
-        # MySQL error.
-        # TODO perhaps the database schema should be
-        # changed to account for this.
-        name = basic.truncate_value(name, 25, "...")
-        description = ",".join(des_list[2:]).strip()
-
-    return description, domain_id, name
-
-
-def learn_cdd_name(cdd_dir):
-    cdd_files = os.listdir(cdd_dir)
-    cdd_files = [os.path.join(cdd_dir, x.split(".")[0]) for x in cdd_files]
-    file_set = set(cdd_files)
-    if len(file_set) == 1:
-        cdd_name = cdd_files[0]
+        gr_reports = True
+        s_report = True
+        psr_reports = True
+
+    execute_pham_review(
+                   alchemist,
+                   folder_path=args.folder_path, folder_name=args.folder_name,
+                   no_review=args.no_review, values=values, force=args.force,
+                   filters=args.filters, groups=args.groups, sort=args.sort,
+                   s_report=s_report, gr_reports=gr_reports,
+                   production=args.production, psr_reports=psr_reports,
+                   verbose=args.verbose)
+
+
+def parse_pham_review(unparsed_args_list):
+    """Parses review arguments and stores them with an argparse object.
+
+    :param unparsed_args_list: Input a list of command line args.
+    :type unparsed_args_list: list[str]
+    :returns: ArgParse module parsed args.
+    """
+    DATABASE_HELP = """
+        Name of the MySQL database to export from.
+        """
+
+    FORCE_HELP = """
+        Review option that aggresively creates and overwrites directories.
+        """
+    CONFIG_FILE_HELP = """
+        Review option that enables use of a config file for sourcing
+        credentials
+            Follow selection argument with the path to the config file
+            specifying MySQL and NCBI credentials.
+        """
+    VERBOSE_HELP = """
+        Review option that enables progress print statements.
+        """
+    FOLDER_PATH_HELP = """
+        Review option to change the path
+        of the directory where the exported files are stored.
+            Follow selection argument with the path to the
+            desired directory.
+        """
+    FOLDER_NAME_HELP = """
+        Review option to change the name
+        of the directory where the exported files are stored.
+            Follow selection argument with the desired name.
+        """
+
+    ALL_REPORTS_HELP = """
+        Review option to toggle export of all report options.
+        """
+    GENE_REPORTS_HELP = """
+        Review option to toggle export of supplemental information about
+        the genes in the phams selected.
+        """
+    SUMMARY_REPORT_HELP = """
+        Review option to toggle export of supplemental information about
+        the profile of the phages selected.
+        """
+    PHAM_SUMMARY_REPORT_HELP = """
+        Review option to toggle export of supplemental information about
+        the profile of a pham selected for review.
+        """
+    PRODUCTION_HELP = """
+        Review option to toggle additional filters to support production-level
+        review.
+        """
+
+    REVIEW_HELP = """
+        Review option to toggle review of phams.  If enabled,
+        phams inputted or auto-generated will not be reviewed
+        for inconsistencies.
+        """
+    IMPORT_FILE_HELP = """
+        Selection input option that imports values from a csv file.
+            Follow selection argument with path to the
+            csv file containing the names of each genome in the first column.
+        """
+    IMPORT_NAMES_HELP = """
+        Selection input option that imports values from cmd line input.
+            Follow selection argument with space separated
+            names of genomes in the database.
+        """
+
+    WHERE_HELP = """
+        Data filtering option that filters data by the inputted expressions.
+            Follow selection argument with formatted filter expression:
+                {Table}.{Column}={Value}
+        """
+    GROUP_BY_HELP = """
+        Data selection option that groups data by the inputted columns.
+            Follow selection argument with formatted column expressions:
+                {Table}.{Column}={Value}
+        """
+    ORDER_BY_HELP = """
+        Data selection option that sorts data by the inputted columns.
+            Follow selection argument with formatted column expressions:
+                {Table}.{Column}={Value}
+        """
+
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument("database", type=str,  help=DATABASE_HELP)
+
+    parser.add_argument("-f", "--force", action="store_true",
+                        help=FORCE_HELP)
+    parser.add_argument("-c", "--config_file",
+                        type=pipelines_basic.convert_file_path,
+                        help=CONFIG_FILE_HELP)
+    parser.add_argument("-m", "--folder_name",
+                        type=str,  help=FOLDER_NAME_HELP)
+    parser.add_argument("-o", "--folder_path", type=Path,
+                        help=FOLDER_PATH_HELP)
+    parser.add_argument("-v", "--verbose", action="store_true",
+                        help=VERBOSE_HELP)
+
+    parser.add_argument("-a", "--all_reports", action="store_true",
+                        help=ALL_REPORTS_HELP)
+    parser.add_argument("-gr", "--gene_reports", action="store_true",
+                        help=GENE_REPORTS_HELP)
+    parser.add_argument("-sr", "--summary_report", action="store_true",
+                        help=SUMMARY_REPORT_HELP)
+    parser.add_argument("-psr", "--pham_summary_reports", action="store_true",
+                        help=PHAM_SUMMARY_REPORT_HELP)
+    parser.add_argument("-p", "--production", action="store_true",
+                        help=PRODUCTION_HELP)
+
+    parser.add_argument("-nr", "--no_review", action="store_true",
+                        help=REVIEW_HELP)
+    parser.add_argument("-if", "--import_files", dest="input",
+                        type=pipelines_basic.convert_file_path,
+                        help=IMPORT_FILE_HELP)
+    parser.add_argument("-in", "--import_names", nargs="*", dest="input",
+                        help=IMPORT_NAMES_HELP)
+
+    parser.add_argument("-w", "--where", nargs="?", dest="filters",
+                        help=WHERE_HELP)
+    parser.add_argument("-g", "--group_by", nargs="*", dest="groups",
+                        help=GROUP_BY_HELP)
+    parser.add_argument("-s", "--order_by", nargs="*", dest="sort",
+                        help=ORDER_BY_HELP)
+
+    default_folder_name = DEFAULT_FOLDER_NAME
+
+    parser.set_defaults(folder_name=default_folder_name,
+                        folder_path=None,
+                        input=[], filters="", groups=[], sort=[],
+                        config_file=None,
+                        no_review=False, gene_report=False,
+                        summary_report=False, verbose=False)
+
+    parsed_args = parser.parse_args(unparsed_args_list[2:])
+    return parsed_args
+
+
+def execute_pham_review(
+                   alchemist, folder_path=None,
+                   folder_name=DEFAULT_FOLDER_NAME, no_review=False, values=[],
+                   filters="", groups=[], sort=[], s_report=False,
+                   gr_reports=False, psr_reports=False, production=False,
+                   verbose=False, force=False):
+    """Executes the entirety of the pham review pipeline.
+
+    :param alchemist: A connected and fully built AlchemyHandler object.
+    :type alchemist: AlchemyHandler
+    :param folder_path: Path to a valid dir for new dir creation.
+    :type folder_path: Path
+    :param folder_name: A name for the export folder.
+    :type folder_name: str
+    :param csv_title: Title for an appended csv file prefix.
+    :type csv_title: str
+    :param review: A boolean to toggle filtering of phams by pham discrepancies
+    :type review: bool
+    :param values: List of values to filter database results.
+    :type values: list[str]
+    :param force: A boolean to toggle aggresive building of directories.
+    :type force: bool
+    :param filters: A list of lists with filter values, grouped by ORs.
+    :type filters: list[list[str]]
+    :param groups: A list of supported MySQL column names to group by.
+    :type groups: list[str]
+    :param sort: A list of supported MySQL column names to sort by.
+    :param gr_reports: A boolean to toggle export of additional pham info
+    :type gr_reports: bool
+    :param production: Toggles additional filters for production-level review
+    :type production: bool
+    :param verbose: A boolean value to toggle progress print statements.
+    :type verbose: bool
+    """
+    db_filter = pipelines_basic.build_filter(alchemist, "gene.PhamID", filters,
+                                                        values=values,
+                                                        verbose=verbose)
+    if production:
+        db_filter.add(BASE_CONDITIONALS)
+        db_filter.update()
     else:
-        cdd_name = ""
-    return cdd_name
+        conditionals = db_filter.build_where_clauses()
+        db_filter.values = db_filter.build_values(where=conditionals)
 
+    if not db_filter.values:
+        print("Current settings produced no database hits.")
+        sys.exit(1)
+    else:
+        if verbose:
+            print(f"Identified {db_filter.hits()} phams to review...")
 
-def main(argument_list):
+    if not no_review:
+        review_phams(db_filter, verbose=verbose)
+
+    if sort:
+        db_filter.sort(sort)
+
+    if verbose:
+        print("Creating export folder...")
+    export_path = pipelines_basic.create_working_path(folder_path, folder_name,
+                                                      force=force)
+
+    conditionals_map = pipelines_basic.build_groups_map(db_filter, export_path,
+                                                        groups=groups,
+                                                        verbose=verbose,
+                                                        force=force)
+
+    if verbose:
+        print("Prepared query and path structure, beginning review export...")
+    original_phams = db_filter.values
+    gr_data_cache = {}
+    psr_data_cache = {}
+    for mapped_path in conditionals_map.keys():
+        conditionals = conditionals_map[mapped_path]
+        db_filter.values = original_phams
+        db_filter.values = db_filter.build_values(where=conditionals)
+
+        pipelines_basic.create_working_dir(mapped_path, force=force)
+
+        review_data = get_review_data(alchemist, db_filter, verbose=verbose)
+        write_report(review_data, mapped_path, REVIEW_HEADER,
+                     csv_name="FunctionReport", verbose=verbose)
+
+        if s_report:
+            summary_data = get_summary_data(alchemist, db_filter)
+            write_summary_report(alchemist, summary_data, mapped_path,
+                                 verbose=verbose)
+
+        if gr_reports or psr_reports:
+            execute_pham_report_export(alchemist, db_filter, mapped_path,
+                                       gr_reports=gr_reports,
+                                       psr_reports=psr_reports,
+                                       gr_data_cache=gr_data_cache,
+                                       psr_data_cache=psr_data_cache,
+                                       verbose=verbose)
+
+
+def execute_pham_report_export(alchemist, db_filter, export_path,
+                               gr_reports=False, gr_data_cache={},
+                               psr_reports=False, psr_data_cache={},
+                               verbose=False):
+    """Executes export of gene data for a reviewed pham.
+
+    :param alchemist: A connected and fully built AlchemyHandler object.
+    :type alchemist: AlchemyHandler
+    :param export_path: Path to a valid dir for new file creation.
+    :type export_path: Path
+    :param gr_data_cache: Total data extracted for gene reports.
+    :type gr_data_cache: dict
+    :param verbose: A boolean value to toggle progress print statements.
+    :type verbose: bool
     """
-    :param argument_list:
-    :return:
+    phams = db_filter.values
+
+    pham_report_path = export_path.joinpath("PhamReports")
+    pham_report_path.mkdir()
+
+    for pham in phams:
+        pham_path = pham_report_path.joinpath(str(pham))
+        pham_path.mkdir()
+
+        db_filter.values = [pham]
+
+        if gr_reports:
+            gr_data = gr_data_cache.get(pham)
+            if gr_data is None:
+                gr_data = get_gr_data(alchemist, db_filter, verbose=verbose)
+                gr_data_cache[pham] = gr_data
+
+            write_report(gr_data, pham_path, GR_HEADER,
+                         csv_name=f"{pham}_GeneReport",
+                         verbose=verbose)
+        if psr_reports:
+            psr_data = psr_data_cache.get(pham)
+            if psr_data is None:
+                psr_data = get_psr_data(alchemist, db_filter, verbose=verbose)
+                psr_data_cache[pham] = psr_data
+
+            write_pham_summary_report(psr_data, pham_path, verbose=verbose)
+
+
+def review_phams(db_filter, verbose=False):
+    """Finds and stores phams with discrepant function calls in a Filter.
+
     """
-    # Setup argument parser
-    cdd_parser = setup_argparser()
-
-    # Use argument parser to parse argument_list
-    args = cdd_parser.parse_args(argument_list[2:])
-
-    # Store arguments in more easily accessible variables
-    database = args.database
-    cdd_dir = expand_path(args.cdd)
-    cdd_name = learn_cdd_name(cdd_dir)
-    threads = args.threads
-    evalue = args.evalue
-    rpsblast = args.rpsblast
-    tmp_dir = args.tmp_dir
-    output_folder = args.output_folder
-    reset = args.reset
-    batch_size = args.batch_size
+    notes = db_filter.get_column("gene.Notes")
 
-    # Create config object with data obtained from file and/or defaults.
-    config = configfile.build_complete_config(args.config_file)
-    mysql_creds = config["mysql"]
+    if verbose:
+        print("Reviewing phams...")
 
-    # Set up directory.
-    output_folder = basic.set_path(output_folder, kind="dir", expect=True)
-    results_folder = pathlib.Path(RESULTS_FOLDER)
-    results_path = basic.make_new_dir(output_folder, results_folder,
-                                      attempt=50)
-    if results_path is None:
-        print("Unable to create output_folder.")
-        sys.exit(1)
+    reviewed_phams = []
+    for index in range(len(db_filter.values)):
+        pham = db_filter.values[index]
+        if verbose:
+            print(f"...Analyzing Pham {pham}...")
 
-    log_file = pathlib.Path(results_path, MAIN_LOG_FILE)
+        query = querying.build_count(db_filter.graph, notes.distinct(),
+                                     where=(db_filter.key == pham))
+        func_count = mysqldb_basic.scalar(db_filter.engine, query)
 
-    # Set up root logger.
-    logging.basicConfig(filename=log_file, filemode="w", level=logging.DEBUG,
-                        format="pdm_utils find_domains: %(levelname)s: %(message)s")
-    logger.info(f"pdm_utils version: {VERSION}")
-    logger.info(f"CDD run date: {constants.CURRENT_DATE}")
-    logger.info(f"Command line arguments: {' '.join(argument_list)}")
-    logger.info(f"Results directory: {results_path}")
-
-    # Early exit if either 1) cdd_name == "" or 2) no rpsblast given and we are
-    # unable to find one
-    if cdd_name == "":
-        msg = (f"Unable to learn CDD database name. Make sure the files in "
-              f"{cdd_dir} all have the same basename.")
-        logger.error(msg)
-        print(msg)
-        return
-
-    # Get the rpsblast command and path.
-    if rpsblast == "":
-        command = get_rpsblast_command()
-        rpsblast = get_rpsblast_path(command)
-
-    # Verify database connection and schema compatibility.
-    alchemist = AlchemyHandler(database=database,
-                               username=mysql_creds["user"],
-                               password=mysql_creds["password"])
-    alchemist.connect(pipeline=True)
-    engine = alchemist.engine
-    logger.info(f"Connected to database: {database}.")
-    mysqldb.check_schema_compatibility(engine, "the find_domains pipeline")
-    logger.info(f"Schema version is compatible.")
-    logger.info("Command line arguments verified.")
-
-    if reset:
-        logger.info("Clearing all domain data currently in the database.")
-        clear_domain_data(engine)
-
-    # Get gene data that needs to be processed
-    # in dict format where key = column name, value = stored value.
-    cdd_genes = mysqldb_basic.query_dict_list(engine, GET_GENES_FOR_CDD)
-    msg = f"{len(cdd_genes)} genes to search for conserved domains..."
-    logger.info(msg)
-    print(msg)
-
-    # Only run the pipeline if there are genes returned that need it
-    if len(cdd_genes) > 0:
-
-        log_gene_ids(cdd_genes)
-        make_tempdir(tmp_dir)
-
-        # Identify unique translations to process mapped to GeneIDs.
-        cds_trans_dict = create_cds_translation_dict(cdd_genes)
-
-        unique_trans = list(cds_trans_dict.keys())
-        msg = (f"{len(unique_trans)} unique translations "
-               "to search for conserved domains...")
-        logger.info(msg)
-        print(msg)
-
-        # Process translations in batches. Otherwise, searching could take
-        # so long that MySQL connection closes resulting in 1 or more
-        # transaction errors.
-        batch_indices = basic.create_indices(unique_trans, batch_size)
-        total_rolled_back = 0
-        for indices in batch_indices:
-            start = indices[0]
-            stop = indices[1]
-            msg = f"Processing translations {start + 1} to {stop}..."
-            logger.info(msg)
-            print(msg)
-            sublist = unique_trans[start:stop]
-            batch_rolled_back = search_translations(
-                                    rpsblast, cdd_name, tmp_dir, evalue,
-                                    threads, engine, sublist, cds_trans_dict)
-            total_rolled_back += batch_rolled_back
-
-        search_summary(total_rolled_back)
-        engine.dispose()
-
-    return
-
-
-def search_summary(rolled_back):
-    """Print search results."""
-    if rolled_back > 0:
-        msg = (f"Error executing {rolled_back} transaction(s). "
-               "Some genes may still contain unidentified domains.")
-        logger.error(msg)
-    else:
-        msg = "All genes successfully searched for conserved domains."
-        logger.info(msg)
-    print("\n\n\n" + msg)
-
-
-def search_translations(rpsblast, cdd_name, tmp_dir, evalue, threads,
-                        engine, unique_trans, cds_trans_dict):
-    """Search for conserved domains in a list of unique translations.
-    """
-    # Build jobs list
-    jobs = []
-    for id, translation in enumerate(unique_trans):
-        jobs.append((rpsblast, cdd_name, tmp_dir, evalue, id, translation))
-    results_temp = parallelize(jobs, threads, search_and_process)
-    # Get rid of unneeded list type which was only needed due to
-    # filter restriction in parallelize.start_processes()
-    results = [i[0] for i in results_temp]
-
-    # List of dictionaries. Each dictionary:
-    # keys: "Translation": translation, "Data": list of results
-    # In each list of results, each element is a dictionary:
-    # data_dict = {
-    #     "HitID": align.hit_id,
-    #     "DomainID": domain_id,
-    #     "Name": name,
-    #     "Description": description,
-    #     "Expect": float(hsp.expect),
-    #     "QueryStart": int(hsp.query_start),
-    #     "QueryEnd": int(hsp.query_end)
-    #     }
-
-    results_dict = create_results_dict(results)
-    # Returns a dictionary, where:
-    # key = unique translation,
-    # value = list of dictionaries, each dictionary a unique rpsblast result
-
-    transactions = construct_sql_txns(cds_trans_dict, results_dict)
-    rolled_back = insert_domain_data(engine, transactions)
-    return rolled_back
-
-
-def create_cds_translation_dict(cdd_genes):
-    """Create a dictionary of genes and translations.
-
-    Returns a dictionary, where:
-    key = unique translation
-    value = set of GeneIDs with that translation."""
-    trans_dict = {}
-    for cds in cdd_genes:
-        trans = cds["Translation"]
-        gene_id = cds["GeneID"]
-        if trans in trans_dict.keys():
-            trans_dict[trans].add(gene_id)
-        else:
-            trans_dict[trans] = {gene_id}
-    return trans_dict
+        if func_count <= 1:
+            continue
 
+        if verbose:
+            print(f"......Detected discrepencies in Pham {pham}")
+        reviewed_phams.append(pham)
 
-def construct_sql_txns(cds_trans_dict, rpsblast_results):
-    """Construct the list of SQL transactions."""
-    # Since identical domain data may be used for > 1 genes, it is simply
-    # duplicated for each gene. This could probably be simplified so that it
-    # only tries to insert domain data once, and if that fails, then
-    # all gene_domain and gene statements that depend on that domain data
-    # will also fail.
-    transactions = []
-    for translation in rpsblast_results.keys():
-        # Each translation has a list of rps_data
-        rps_data_list = rpsblast_results[translation]
-        # Each translation has a set of GeneIDs
-        gene_ids = cds_trans_dict[translation]
-        for gene_id in gene_ids:
-            txn = construct_sql_txn(gene_id, rps_data_list)
-            transactions.append(txn)
-    return transactions
-
-
-def construct_sql_txn(gene_id, rps_data_list):
-    """Map domain data back to gene_id and create SQL statements for one transaction.
-
-    rps_data_list is a list of dictionaries, where each dictionary reflects
-    a significat rpsblast domain hit.
-    """
-    txn = []
-    for rps_hit in rps_data_list:
-        domain_stmt = construct_domain_stmt(rps_hit)
-        gene_domain_stmt = construct_gene_domain_stmt(rps_hit, gene_id)
-        txn.append(domain_stmt)
-        txn.append(gene_domain_stmt)
-    update_stmt = construct_gene_update_stmt(gene_id)
-    txn.append(update_stmt)
-    return txn
-
-
-def construct_domain_stmt(data_dict):
-    """Construct the SQL statement to insert data into the domain table."""
-    stmt = INSERT_INTO_DOMAIN.format(data_dict["HitID"],
-                                    data_dict["DomainID"],
-                                    data_dict["Name"],
-                                    data_dict["Description"])
-    return stmt
-
-
-def construct_gene_domain_stmt(data_dict, gene_id):
-    """Construct the SQL statement to insert data into the gene_domain table."""
-    stmt = INSERT_INTO_GENE_DOMAIN.format(gene_id,
-                                          data_dict["HitID"],
-                                          data_dict["Expect"],
-                                          data_dict["QueryStart"],
-                                          data_dict["QueryEnd"])
-    return stmt
-
-
-def construct_gene_update_stmt(gene_id):
-    """Construct the SQL statement to update data in the gene table."""
-    stmt = UPDATE_GENE.format(gene_id)
-    return stmt
-
-
-def create_results_dict(search_results):
-    """Create a dictionary of search results
-
-    Input is a list of dictionaries, one dict per translation, where:
-    keys = "Translation" and "Data", where
-    key = "Translation" has value = translation,
-    key = "Data"" has value = list of rpsblast results, where
-    Each result element is a dictionary containing domain and gene_domain data.
-
-    Returns a dictionary, where:
-    key = unique translation,
-    value = list of dictionaries, each dictionary a unique rpsblast result
-    """
-    dict = {}
-    for result in search_results:
-        dict[result["Translation"]] = result["Data"]
-    return dict
-
-
-def get_rpsblast_command():
-    """Determine rpsblast+ command based on operating system."""
-    # See if we're running on a Mac
-    if platform.system() == "Darwin":
-        msg = "Detected MacOS operating system..."
-        logger.info(msg)
-        print(msg)
-        command = shlex.split("which rpsblast")
-    # Otherwise see if we're on a Linux machine
-    elif platform.system() == "Linux":
-        msg = "Detected Linux operating system..."
-        logger.info(msg)
-        print(msg)
-        command = shlex.split("which rpsblast+")
-    # Windows or others - unsupported, leave early
-    else:
-        msg = (f"Unsupported system '{platform.system()}'; cannot run "
-              f"find_domains pipeline.")
-        logger.error(msg)
-        print(msg)
-        sys.exit(1)
-    return command
+    if verbose:
+        print(f"Detected {len(reviewed_phams)} disrepent phams...")
 
+    db_filter.values = reviewed_phams
 
-def get_rpsblast_path(command):
-    """Determine rpsblast+ binary path."""
 
-    # If we didn't exit, we have a command.
-    # Run it, and PIPE stdout into rpsblast_path
-    with Popen(args=command, stdout=PIPE) as proc:
-        rpsblast = proc.stdout.read().decode("utf-8").rstrip("\n")
-
-    # If empty string, rpsblast not found in globally
-    # available executables, otherwise proceed with value.
-    if rpsblast == "":
-        msg = ("No rpsblast binary found. "
-              "If you have rpsblast on your machine, please try "
-              "again with the '--rpsblast' flag and provide the "
-              "full path to your rpsblast binary.")
-        logger.error(msg)
-        print(msg)
+def write_report(data, export_path, header, csv_name="Report", verbose=False):
+    """Outputs a csv file
+    """
+    if not export_path.is_dir():
+        print("Passed in path is not a directory.")
         sys.exit(1)
-    else:
-        msg = f"Found rpsblast binary at '{rpsblast}'..."
-        logger.info(msg)
-        print(msg)
-        return rpsblast
-
-
-def log_gene_ids(cdd_genes):
-    """Record names of the genes processed for reference."""
-    batch_indices = basic.create_indices(cdd_genes, 20)
-    for indices in batch_indices:
-        genes_subset = cdd_genes[indices[0]: indices[1]]
-        gene_ids = []
-        for gene in genes_subset:
-            gene_ids.append(gene["GeneID"])
-        logger.info("; ".join(gene_ids))
-
-
-def insert_domain_data(engine, results):
-    """Attempt to insert domain data into the database."""
-    msg = "Inserting data..."
-    logger.info(msg)
-    print(msg)
-
-    rolled_back = 0
-    connection = engine.connect()
-    for result in results:
-        exe_result = execute_transaction(connection, result)
-        rolled_back += exe_result
-
-    if rolled_back > 0:
-        msg = (f"Error executing {rolled_back} transaction(s).")
-        logger.error(msg)
-        print(msg)
-    return rolled_back
-
-
-def execute_transaction(connection, statement_list=[]):
-    trans = connection.begin()
-    failed = 0
-    index = 0
-    # Even though the execution of individual statements are handled within
-    # a try/exept block, this try/except block encapsulates all code
-    # that is executed while uncommitted changes have been made to the database.
-    # Without this encapsulation, even if all MySQL execution errors are caught,
-    # other types of errors generated while processing the results would
-    # crash the code and possibly result in changes made to the database
-    # that shouldn't be persisted.
-    try:
-        # Try to execute statements as long as none of them failed.
-        # Once one statement fails, don't try to execute any other statements.
-        while (failed == 0 and index < len(statement_list)):
-            statement = statement_list[index]
-            result_tup = execute_statement(connection, statement)
-            stmt_result = result_tup[0]
-            type_error = result_tup[1]
-            value_error = result_tup[2]
-            msg = result_tup[3]
-
-            msg = msg + "Statement: " + statement
-            if stmt_result == 0:
-                logger.info(msg)
-            else:
-                if (type_error == False and value_error == False):
-                    logger.error(msg)
-                else:
-                    # If the insertion failed due to a TypeError, it could be
-                    # due to the fact that the string contains '%'.
-                    # Some CDD descriptions contain '%', which throws an error
-                    # when SQLAlchemy's engine.Connection.execute() is used.
-                    # The string gets passed to a pymysql.cursor function which
-                    # interprets the % as a string formatting operator,
-                    # and since there is no value to insert and format,
-                    # the MySQL statement fails and the
-                    # entire transactions is rolled back.
-                    # For these edge cases, one way around this is to
-                    # attempt to replace all '%' with '%%'.
-                    # SQLAlchemy provides several different ways to
-                    # implement changes to the database, and another strategy
-                    # is likely to get around this problem.
-                    if "%" not in statement:
-                        logger.error(msg)
-                    else:
-                        logger.warning(msg)
-                        logger.info("Attempting to resolve '%' error(s).")
-                        statement = statement.replace("%", "%%")
-                        result_tup = execute_statement(connection, statement)
-                        stmt_result = result_tup[0]
-                        type_error = result_tup[1]
-                        value_error = result_tup[2]
-                        msg = result_tup[3]
-
-                        if stmt_result == 0:
-                            logger.info(("The '%' replacement resolved the "
-                                         "error(s)."))
-                            logger.info(msg + statement)
-                        else:
-                            logger.info(("The '%' replacement failed to "
-                                         "resolve the error(s)."))
-                            logger.error(msg + statement)
-            failed += stmt_result
-            index += 1
-
-        msg = (f"There are {failed} statements that failed execution.")
-        if failed == 0:
-            logger.info(msg)
-            logger.info("Committing all changes.")
-            trans.commit()
-            txn_result = 0
-        else:
-            logger.error(msg)
-            logger.info("Rolling back transaction.")
-            trans.rollback()
-            txn_result = 1
-    except:
-        print("Error executing MySQL statements.")
-        print("Rolling back transaction...")
-        logger.error("Unable to execute MySQL statements.")
-        logger.info("Rolling back transaction.")
-        trans.rollback()
-        txn_result = 1
-
-    return txn_result
-
-
-def execute_statement(connection, statement):
-    type_error = False
-    value_error = False
-    try:
-        connection.execute(statement)
-    except sqlalchemy.exc.DBAPIError as err:
-        err_stmt = err.statement
-        sqla_err_type = str(type(err))
-        pymysql_err_type = str(type(err.orig))
-        pymysql_err_code = err.orig.args[0]
-        pymysql_err_msg = err.orig.args[1]
-        msg = (f"SQLAlchemy Error type: {sqla_err_type}. "
-               f"PyMySQL Error type: {pymysql_err_type}. "
-               f"PyMYSQL Error code: {pymysql_err_code}. "
-               f"PyMySQL Error message: {pymysql_err_msg}.")
-        if pymysql_err_code == 1062:
-            msg = "Duplicate entry error ignored. " + msg
-            result = 0
+
+    file_path = export_path.joinpath(f"{csv_name}.csv")
+    if verbose:
+        print(f"Writing {file_path.name} in {export_path.name}...")
+
+    fileio.export_data_dict(data, file_path, header, include_headers=True)
+
+
+def write_summary_report(alchemist, summary_data, export_path, verbose=False):
+    if verbose:
+        print(f"Writing SummaryReport.txt in {export_path.name}")
+
+    s_path = export_path.joinpath("SummaryReport.txt")
+    s_file = open(s_path, "w")
+
+    version_data = summary_data["version_data"]
+    recurring_phages = summary_data["recurring_phages"]
+    recent_phages = summary_data["recent_phages"]
+
+    s_file.write(f"Phams reviewed on: {time.strftime('%d-%m-%Y')}\n")
+    s_file.write(f"Database reviewed: {alchemist.database}\n")
+    s_file.write(f"Schema version: {version_data['SchemaVersion']} "
+                 f"Database version: {version_data['Version']}\n\n")
+    s_file.write("Phams reviewed using the following base conditionals:\n")
+    s_file.write(f"    {BASE_CONDITIONALS}\n")
+
+    s_file.write("\n\n")
+    s_file.write(f"Most occuring phages: {', '.join(recurring_phages)}\n")
+    s_file.write(f"Phages recently submitted: {', '.join(recent_phages)}\n")
+    s_file.close()
+
+
+def write_pham_summary_report(psr_data, export_path, verbose=False):
+    if verbose:
+        print(f"Writing SummaryReport.txt in {export_path.name}")
+
+    s_path = export_path.joinpath("SummaryReport.txt")
+    s_file = open(s_path, "w")
+
+    s_file.write(f"Pham: {export_path.name}\n\n")
+
+    s_file.write("Annotations of genes to the left:\n")
+    s_file.write(f"{psr_data['left_annotations']}\n")
+
+    s_file.write("\n")
+    s_file.write("Annotations of genes to the right:\n")
+    s_file.write(f"{psr_data['right_annotations']}\n")
+
+    s_file.write("\n\n")
+    s_file.write("Conserved Database Domains in pham:\n\n")
+    for domain in psr_data["cdd_domains"]:
+        s_file.write(f"{domain}\n\n")
+
+    s_file.close()
+# -----------------------------------------------------------------------------
+# REVIEW-SPECIFIC HELPER FUNCTIONS
+
+
+# TODO Documentation
+def get_review_data(alchemist, db_filter, verbose=False):
+    """
+    """
+    if verbose:
+        print("Retrieving data for phams...")
+
+    review_columns = get_review_data_columns(alchemist)
+    row_dicts = db_filter.retrieve(review_columns)
+
+    review_data = []
+    for pham in row_dicts.keys():
+        if verbose:
+            print(f"...Processing data for pham {pham}...")
+        row_dict = row_dicts[pham]
+        row_dict["Notes"] = annotation.get_count_annotations_in_pham(
+                                                            alchemist, pham)
+
+        format_review_data(row_dict, pham)
+        review_data.append(row_dict)
+
+    return review_data
+
+
+def get_summary_data(alchemist, db_filter, verbose=False):
+    phams = db_filter.values
+
+    phages_data = db_filter.retrieve("phage.PhageID", filter=True)
+
+    db_filter.values = phams
+    db_filter.transpose("phage.PhageID", set_values=True)
+    db_filter.sort("phage.DateLastModified")
+
+    version_data = mysqldb_basic.get_first_row_data(alchemist.engine,
+                                                    "version")
+
+    summary_data = {}
+    summary_data["recent_phages"] = db_filter.values
+    summary_data["recurring_phages"] = phages_data
+    summary_data["version_data"] = version_data
+
+    format_summary_data(summary_data)
+
+    db_filter.values = phams
+    db_filter.key = "gene.PhamID"
+    return summary_data
+
+
+def get_gr_data(alchemist, db_filter, verbose=False):
+    pham = db_filter.values[0]
+    if verbose:
+        print(f"Retrieving genes in pham {pham}...")
+    db_filter.transpose("gene.GeneID", set_values=True)
+
+    pg_columns = get_gr_data_columns(alchemist)
+    row_dicts = db_filter.retrieve(pg_columns)
+
+    gr_data = []
+    for gene in row_dicts.keys():
+        if verbose:
+            print(f"...Processing data for gene {gene}...")
+
+        row_dict = row_dicts[gene]
+
+        format_gr_data(row_dict, gene)
+        gr_data.append(row_dict)
+
+    db_filter.values = [pham]
+    db_filter.key = "gene.PhamID"
+    return gr_data
+
+
+def get_psr_data(alchemist, db_filter, verbose=False):
+    pham = db_filter.values[0]
+    adjacent_genes = annotation.get_genes_adjacent_to_pham(alchemist, pham)
+    psr_data = {}
+
+    psr_data["left_annotations"] = annotation.get_count_annotations_in_genes(
+                                                alchemist, adjacent_genes[0])
+    psr_data["right_annotations"] = annotation.get_count_annotations_in_genes(
+                                                alchemist, adjacent_genes[1])
+
+    db_filter.values = [pham]
+    db_filter.transpose("domain.Name", set_values=True)
+    cdd_domains = db_filter.retrieve("domain.Description")
+    psr_data["cdd_domains"] = cdd_domains
+
+    format_psr_data(psr_data)
+
+    db_filter.values = [pham]
+    db_filter.key = "gene.PhamID"
+    return psr_data
+
+
+def format_review_data(row_dict, pham):
+    """Function to format function report dictionary keys.
+
+    :param row_dict: Data dictionary for a function report.
+    :type row_dict: dict
+    :param pham: PhamID to append to the function report data dictionary.
+    :type pham: int
+    """
+    row_dict["Pham"] = pham
+    row_dict["Final Call"] = ""
+    row_dict["#Members"] = len(row_dict.pop("GeneID"))
+    row_dict["#Functions"] = len(row_dict["Notes"])
+
+    row_dict["Clusters"] = ";".join([str(cluster)
+                                    for cluster in row_dict.pop("Cluster")])
+
+    count_functional_calls = []
+    notes = row_dict.pop("Notes")
+    notes = basic.sort_histogram(notes)
+    for key in notes.keys():
+        if key is None or key == "":
+            function = "hypothetical protein"
         else:
-            msg = "Unable to execute MySQL statement. " + msg
-            result = 1
-    except TypeError as err:
-        type_error = True
-        msg = "Unable to execute statement due to a TypeError. "
-        result = 1
-    except ValueError as err:
-        value_error = True
-        msg = "Unable to execute statement due to a ValueError. "
-        result = 1
-    except:
-        # TODO not sure how to test this block. Would need to construct a
-        # statement that causes a Python built-in exception other
-        # than TypeError or ValueError.
-        msg = "Unable to execute statement. "
-        result = 1
-    else:
-        msg = "Successful statement execution. "
-        result = 0
+            function = key
 
-    return result, type_error, value_error, msg
+        count_functional_calls.append(
+            "".join([function, f"({str(notes[key])})"]))
 
+    row_dict["Functional Calls"] = ";".join(count_functional_calls)
 
-def clear_domain_data(engine):
-    """Delete all domain data stored in the database."""
-    connection = engine.connect()
-    stmts = [CLEAR_GENE_DOMAIN, CLEAR_DOMAIN, CLEAR_GENE_DOMAINSTATUS]
-    exe_result = execute_transaction(connection, stmts)
-    if exe_result == 1:
-        logger.error("Unable to clear all domain data.")
-    else:
-        logger.info("All domain data cleared.")
+
+def format_summary_data(summary_data):
+    recent_phages = summary_data["recent_phages"]
+    recent_phages.reverse()
+    recent_phages = basic.partition_list(recent_phages, 5)[0]
+    summary_data["recent_phages"] = recent_phages
+
+    phages_data = summary_data["recurring_phages"]
+    phages_histogram = {}
+    for pham in phages_data.keys():
+        basic.increment_histogram(phages_data[pham]["PhageID"],
+                                  phages_histogram)
+
+    recurring_phages = basic.sort_histogram_keys(phages_histogram)
+    recurring_phages = basic.partition_list(recurring_phages, 5)[0]
+    for i in range(len(recurring_phages)):
+        recurring_phages[i] = "".join(
+                           [recurring_phages[i],
+                            f"({str(phages_histogram[recurring_phages[i]])})"])
+    summary_data["recurring_phages"] = recurring_phages
+
+
+def format_gr_data(row_dict, gene):
+    """Function to format gene report dictionary keys.
+
+    :param row_dict: Data dictionary for a gene report.
+    :type row_dict: dict
+    :param gene: GeneID to append to the gene report data dictionary.
+    :type gene: str
+    """
+    row_dict["Gene"] = gene
+    row_dict["Phage"] = row_dict.pop("PhageID")[0]
+    row_dict["Gene#"] = row_dict.pop("Name")[0]
+    row_dict["Cluster"] = row_dict["Cluster"][0]
+    row_dict["Subcluster"] = row_dict["Subcluster"][0]
+    row_dict["Translation"] = row_dict["Translation"][0]
+
+    note = row_dict.pop("Notes")[0]
+    if note is None or note == "":
+        note = "hypothetical protein"
+
+    row_dict["Functional Call"] = note
+
+
+def format_psr_data(psr_data):
+    left_annotations = format_adjacent_annotations(
+                                                psr_data["left_annotations"])
+    psr_data["left_annotations"] = left_annotations
+
+    right_annotations = format_adjacent_annotations(
+                                                psr_data["right_annotations"])
+    psr_data["right_annotations"] = right_annotations
+
+    cdd_domains_data = psr_data["cdd_domains"]
+    cdd_domains = []
+    for domain in cdd_domains_data.keys():
+        description = cdd_domains_data[domain]["Description"][0]
+        description = textwrap.wrap(description, 72)
+        description = "\n".join(description)
+        description = textwrap.indent(description, "    ")
+        cdd_domain = "".join([domain, "\n", description])
+        cdd_domains.append(cdd_domain)
+    psr_data["cdd_domains"] = cdd_domains
+
+
+def format_adjacent_annotations(annotation_histogram):
+    annotation_histogram = basic.sort_histogram(annotation_histogram)
+
+    annotation_list = []
+    for note in annotation_histogram.keys():
+        count = annotation_histogram[note]
+        if (note == "") or (note is None):
+            note = "hypothetical protein"
+        annotation_list.append("".join([note, "(", str(count), ")"]))
+
+    annotations = ", ".join(annotation_list)
+    wrapped_annotations = textwrap.wrap(annotations, 72)
+    annotations = "\n".join(wrapped_annotations)
+    annotations = textwrap.indent(annotations, "    ")
+    return annotations
+
+
+def get_review_data_columns(alchemist):
+    """Gets labelled columns for pham function data retrieval.
+
+    :returns: List of labelled columns for function data retrieval.
+    :rtype: list[Column]
+    """
+    review_columns = []
+
+    for column_name in REVIEW_DATA_COLUMNS:
+        review_columns.append(querying.get_column(alchemist.metadata,
+                                                  column_name))
+
+    return review_columns
+
+
+def get_gr_data_columns(alchemist):
+    """Gets labelled columns for pham gene data retrieval.
+
+    :returns: List of labelled columns for gene data retrieval.
+    :rtype: list[Column]
+    """
+    pg_columns = []
+
+    for column_name in GR_DATA_COLUMNS:
+        pg_columns.append(querying.get_column(alchemist.metadata, column_name))
+
+    return pg_columns
+
+
+if __name__ == "__main__":
+    args = sys.argv
+    args.insert(0, "")
+    main(args)
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/find_membrane.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/find_membrane.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/find_transmembrane.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/find_transmembrane.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/freeze_db.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/freeze_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/get_data.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/get_data.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/get_db.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/get_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/get_gb_records.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/get_gb_records.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/import_genome.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/import_genome.py`

 * *Files 1% similar despite different names*

```diff
@@ -1650,18 +1650,14 @@
     if eval_flags["check_id_typo"]:
         src_ftr.check_attribute("_organism_name", {src_ftr.genome_id},
                                 expect=True, eval_id="SRC-EVAL-001",
                                 fail="warning", eval_def=EDD["SRC-EVAL-001"])
 
     if eval_flags["check_host_typo"]:
 
-        # TODO not sure if host genus synonyms is needed anymore.
-        # Strategy to utilize host genus synonyms, such as 'Mycolicibacterium'.
-        # host_genus_synonyms = basic.get_synonyms(host_genus,
-        #                                 constants.HOST_GENUS_SYNONYMS)
         # Alternatively, a host_genus_set could be passed into the function,
         # instead of a string, and the decision to pass in a set of synonyms
         # could be pushed up a level.
 
         # Only evaluate attributes if the field is not empty, since they
         # are not required to be present.
         if src_ftr.organism != "":
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/pham_finder.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/pham_finder.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/push_db.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/push_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/revise.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/revise.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/pipelines/update_field.py` & `pdm_utils-1.0.1/src/pdm_utils/pipelines/update_field.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.0.0/src/pdm_utils/run.py` & `pdm_utils-1.0.1/src/pdm_utils/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Use this script to run all pipelines within the pipelines folder.
 It verifies a valid pipeline is selected,
 then passes all command line arguments to the main pipeline module.
 """
+import sys
 import argparse
 
 from pdm_utils.pipelines import compare_db
 from pdm_utils.pipelines import convert_db
 from pdm_utils.pipelines import export_db
 from pdm_utils.pipelines import find_domains
 from pdm_utils.pipelines import find_transmembrane
@@ -23,16 +24,42 @@
 
 VALID_PIPELINES = {"compare", "convert", "export", "find_domains",
                    "find_transmembrane", "find_phams", "freeze", "get_data",
                    "get_db", "get_gb_records", "import", "phamerate", "push",
                    "revise", "pham_review", "update"}
 
 
-def main(unparsed_args):
-    """Run a pdm_utils pipeline."""
+def parse_args(unparsed_args):
+    """
+    Use argparse to verify pipeline argument only.
+
+    :param unparsed_args: raw command line args
+    :type unparsed_args: list
+    """
+    run_help = "Commandline script to call a pdm_utils pipeline."
+    usage = "python3 -m pdm_utils [pipeline]"
+    pipeline_help = "name of the pdm_utils pipeline to run"
+
+    parser = argparse.ArgumentParser(description=run_help, usage=usage)
+    parser.add_argument("pipeline", type=str, choices=list(VALID_PIPELINES),
+                        help=pipeline_help)
+
+    # Assumed command line arg structure:
+    # python3 -m pdm_utils.run <pipeline> <additional args...>
+    # sys.argv:      [0]            [1]         [2...]
+    return parser.parse_args(unparsed_args[1:2])
+
+
+def main(unparsed_args=None):
+    """Commandline entry point for the pdm_utils package."""
+    if not unparsed_args:
+        if len(sys.argv) == 1:
+            sys.argv.append("-h")
+        unparsed_args = sys.argv
+
     args = parse_args(unparsed_args)
 
     if args.pipeline == "compare":
         compare_db.main(unparsed_args)
     elif args.pipeline == "convert":
         convert_db.main(unparsed_args)
     elif args.pipeline == "find_transmembrane":
@@ -62,30 +89,7 @@
     elif args.pipeline == "pham_review":
         pham_review.main(unparsed_args)
     elif args.pipeline == "update":
         update_field.main(unparsed_args)
     else:
         pass
     print("\n\nPipeline completed")
-
-
-def parse_args(unparsed_args):
-    """
-    Use argparse to verify pipeline argument only.
-
-    :param unparsed_args: raw command line args
-    :type unparsed_args: list
-    """
-    run_help = "Command line script to call a pdm_utils pipeline."
-    usage = "python3 -m pdm_utils [pipeline]"
-    pipeline_help = "Name of the pdm_utils pipeline to run."
-
-    parser = argparse.ArgumentParser(description=run_help, usage=usage)
-    parser.add_argument("pipeline", type=str, choices=list(VALID_PIPELINES),
-                        help=pipeline_help)
-
-    # Assumed command line arg structure:
-    # python3 -m pdm_utils.run <pipeline> <additional args...>
-    # sys.argv:      [0]            [1]         [2...]
-    args = parser.parse_args(unparsed_args[1:2])
-
-    return args
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils.egg-info/PKG-INFO` & `pdm_utils-1.0.1/src/pdm_utils.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: pdm-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: MySQL phage genomics database management utilities
 Home-page: https://github.com/SEA-PHAGES/pdm_utils
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
-License: UNKNOWN
 Project-URL: Documentation, https://pdm-utils.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/SEA-PHAGES/pdm_utils/
-Description: # README #
-        
-        ### Purpose: ###
-        
-        * The pdm_utils repository provides the source code for pdm_utils Python package, developed in the SEA-PHAGES program to create, update, and maintain MySQL phage genomics databases.
-        
-        The source code is available on GitHub at https://github.com/SEA-PHAGES/pdm_utils/.
-        
-        The user guide for the package is available on ReadTheDocs at https://pdm-utils.readthedocs.io/en/latest/.
-        
-        The pdm_utils Python package is available on PyPI at https://pypi.org/project/pdm-utils/.
-        
-        ### Contribution guidelines: ###
-        
-        * Please contact us if you have any contributions or suggestions. Details about how to contribute can be found on the user guide.
-        
-        ### Developers: ###
-        
-        * Travis Mavrich (trm53@pitt.edu) and Christian Gauthier (christian.gauthier@pitt.edu).
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Database
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# README #
+
+### Purpose: ###
+
+* The pdm_utils repository provides the source code for pdm_utils Python package, developed in the SEA-PHAGES program to create, update, and maintain MySQL phage genomics databases.
+
+The source code is available on GitHub at https://github.com/SEA-PHAGES/pdm_utils/.
+
+The user guide for the package is available on ReadTheDocs at https://pdm-utils.readthedocs.io/en/latest/.
+
+The pdm_utils Python package is available on PyPI at https://pypi.org/project/pdm-utils/.
+
+### Contribution guidelines: ###
+
+* Please contact us if you have any contributions or suggestions. Details about how to contribute can be found on the user guide.
+
+### Developers: ###
+
+* Travis Mavrich (trm53@pitt.edu) and Christian Gauthier (christian.gauthier@pitt.edu).
```

### Comparing `pdm_utils-1.0.0/src/pdm_utils.egg-info/SOURCES.txt` & `pdm_utils-1.0.1/src/pdm_utils.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+LICENSE
 README.md
-setup.py
+pyproject.toml
+setup.cfg
 src/pdm_utils/__init__.py
 src/pdm_utils/__main__.py
 src/pdm_utils/run.py
 src/pdm_utils.egg-info/PKG-INFO
 src/pdm_utils.egg-info/SOURCES.txt
 src/pdm_utils.egg-info/dependency_links.txt
+src/pdm_utils.egg-info/entry_points.txt
 src/pdm_utils.egg-info/requires.txt
 src/pdm_utils.egg-info/top_level.txt
 src/pdm_utils/classes/__init__.py
 src/pdm_utils/classes/alchemyhandler.py
 src/pdm_utils/classes/aragornhandler.py
 src/pdm_utils/classes/bundle.py
 src/pdm_utils/classes/cds.py
 src/pdm_utils/classes/cdspair.py
 src/pdm_utils/classes/dbcomparesummary.py
+src/pdm_utils/classes/error.py
 src/pdm_utils/classes/evaluation.py
 src/pdm_utils/classes/fileio.py
 src/pdm_utils/classes/filter.py
 src/pdm_utils/classes/genome.py
 src/pdm_utils/classes/genomepair.py
 src/pdm_utils/classes/genometriad.py
-src/pdm_utils/classes/progressbar.py
+src/pdm_utils/classes/progress.py
 src/pdm_utils/classes/randomfieldupdatehandler.py
 src/pdm_utils/classes/source.py
 src/pdm_utils/classes/ticket.py
 src/pdm_utils/classes/tmrna.py
 src/pdm_utils/classes/trna.py
 src/pdm_utils/classes/trnascansehandler.py
 src/pdm_utils/constants/__init__.py
@@ -36,29 +40,32 @@
 src/pdm_utils/functions/__init__.py
 src/pdm_utils/functions/annotation.py
 src/pdm_utils/functions/basic.py
 src/pdm_utils/functions/cartography.py
 src/pdm_utils/functions/configfile.py
 src/pdm_utils/functions/deeptmhmm.py
 src/pdm_utils/functions/eval_modes.py
+src/pdm_utils/functions/fasta.py
 src/pdm_utils/functions/fileio.py
 src/pdm_utils/functions/flat_files.py
+src/pdm_utils/functions/multiprocess.py
 src/pdm_utils/functions/multithread.py
 src/pdm_utils/functions/mysqldb.py
 src/pdm_utils/functions/mysqldb_basic.py
 src/pdm_utils/functions/ncbi.py
-src/pdm_utils/functions/parallelize.py
 src/pdm_utils/functions/parsing.py
 src/pdm_utils/functions/phagesdb.py
 src/pdm_utils/functions/pham_alignment.py
 src/pdm_utils/functions/phameration.py
 src/pdm_utils/functions/pipeline_shells.py
 src/pdm_utils/functions/pipelines_basic.py
 src/pdm_utils/functions/querying.py
+src/pdm_utils/functions/rpsblast.py
 src/pdm_utils/functions/server.py
+src/pdm_utils/functions/subprocess.py
 src/pdm_utils/functions/tickets.py
 src/pdm_utils/functions/url_basic.py
 src/pdm_utils/pipelines/__init__.py
 src/pdm_utils/pipelines/compare_db.py
 src/pdm_utils/pipelines/convert_db.py
 src/pdm_utils/pipelines/export_db.py
 src/pdm_utils/pipelines/find_domains.py
@@ -70,8 +77,10 @@
 src/pdm_utils/pipelines/get_gb_records.py
 src/pdm_utils/pipelines/import_genome.py
 src/pdm_utils/pipelines/pham_finder.py
 src/pdm_utils/pipelines/pham_review.py
 src/pdm_utils/pipelines/phamerate.py
 src/pdm_utils/pipelines/push_db.py
 src/pdm_utils/pipelines/revise.py
-src/pdm_utils/pipelines/update_field.py
+src/pdm_utils/pipelines/update_field.py
+tests/test_data_utils.py
+tests/test_db_utils.py
```

