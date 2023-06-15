# Comparing `tmp/pdm_utils-0.9.9.tar.gz` & `tmp/pdm_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdm_utils-0.9.9.tar", last modified: Tue Mar 23 14:47:05 2021, max compression
+gzip compressed data, was "dist/pdm_utils-1.0.0.tar", last modified: Thu Jun 15 00:24:09 2023, max compression
```

## Comparing `pdm_utils-0.9.9.tar` & `pdm_utils-1.0.0.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxr-xr-x   0 cgauthier   (502) staff       (20)        0 2021-03-23 14:47:05.161918 pdm_utils-0.9.9/
--rw-r--r--   0 cgauthier   (502) staff       (20)     1718 2021-03-23 14:47:05.161243 pdm_utils-0.9.9/PKG-INFO
--rw-r--r--   0 cgauthier   (502) staff       (20)      790 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/README.md
--rw-r--r--   0 cgauthier   (502) staff       (20)       38 2021-03-23 14:47:05.162224 pdm_utils-0.9.9/setup.cfg
--rw-r--r--   0 cgauthier   (502) staff       (20)     1287 2021-03-23 14:45:34.000000 pdm_utils-0.9.9/setup.py
-drwxr-xr-x   0 cgauthier   (502) staff       (20)        0 2021-03-23 14:47:05.103963 pdm_utils-0.9.9/src/
-drwxr-xr-x   0 cgauthier   (502) staff       (20)        0 2021-03-23 14:47:05.106229 pdm_utils-0.9.9/src/pdm_utils/
--rw-r--r--   0 cgauthier   (502) staff       (20)      146 2021-03-23 14:45:34.000000 pdm_utils-0.9.9/src/pdm_utils/__init__.py
--rw-r--r--   0 cgauthier   (502) staff       (20)      100 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/__main__.py
-drwxr-xr-x   0 cgauthier   (502) staff       (20)        0 2021-03-23 14:47:05.122253 pdm_utils-0.9.9/src/pdm_utils/classes/
--rw-r--r--   0 cgauthier   (502) staff       (20)        0 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/__init__.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    20060 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/alchemyhandler.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     8060 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/aragornhandler.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    10410 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/bundle.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    39957 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/cds.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     2461 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/cdspair.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     9923 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/dbcomparesummary.py
--rw-r--r--   0 cgauthier   (502) staff       (20)      696 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/evaluation.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     7966 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/fileio.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    23716 2021-03-23 13:58:17.000000 pdm_utils-0.9.9/src/pdm_utils/classes/filter.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    41594 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/genome.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     5574 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/genomepair.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    18395 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/genometriad.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     1007 2020-11-16 19:26:20.000000 pdm_utils-0.9.9/src/pdm_utils/classes/progressbar.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     7244 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/randomfieldupdatehandler.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     4243 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/source.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     8694 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/ticket.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    37793 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/tmrna.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    63963 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/trna.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     3694 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/classes/trnascansehandler.py
-drwxr-xr-x   0 cgauthier   (502) staff       (20)        0 2021-03-23 14:47:05.125519 pdm_utils-0.9.9/src/pdm_utils/constants/
--rw-r--r--   0 cgauthier   (502) staff       (20)        0 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/constants/__init__.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     6809 2020-12-09 14:41:56.000000 pdm_utils-0.9.9/src/pdm_utils/constants/constants.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    10763 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/constants/db_schema_0.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    12305 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/constants/eval_descriptions.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    35601 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/constants/schema_conversions.py
-drwxr-xr-x   0 cgauthier   (502) staff       (20)        0 2021-03-23 14:47:05.142148 pdm_utils-0.9.9/src/pdm_utils/functions/
--rw-r--r--   0 cgauthier   (502) staff       (20)        0 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/__init__.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     6113 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/annotation.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    45918 2021-01-04 13:42:59.000000 pdm_utils-0.9.9/src/pdm_utils/functions/basic.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     2962 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/cartography.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     2166 2020-12-08 21:13:40.000000 pdm_utils-0.9.9/src/pdm_utils/functions/configfile.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     4638 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/eval_modes.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    10526 2021-03-08 13:33:41.000000 pdm_utils-0.9.9/src/pdm_utils/functions/fileio.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    29939 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/flat_files.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     5302 2021-01-18 11:10:57.000000 pdm_utils-0.9.9/src/pdm_utils/functions/multithread.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    27400 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/mysqldb.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    13414 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/mysqldb_basic.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     6605 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/ncbi.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     3656 2020-11-30 22:55:14.000000 pdm_utils-0.9.9/src/pdm_utils/functions/parallelize.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    10972 2021-01-04 13:42:59.000000 pdm_utils-0.9.9/src/pdm_utils/functions/parsing.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    13264 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/phagesdb.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     8109 2021-01-18 11:10:57.000000 pdm_utils-0.9.9/src/pdm_utils/functions/pham_alignment.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    24951 2021-03-18 17:35:49.000000 pdm_utils-0.9.9/src/pdm_utils/functions/phameration.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     8473 2021-01-05 15:44:51.000000 pdm_utils-0.9.9/src/pdm_utils/functions/pipeline_shells.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     8828 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/pipelines_basic.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    30269 2021-03-23 13:58:17.000000 pdm_utils-0.9.9/src/pdm_utils/functions/querying.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     3475 2020-11-30 22:32:05.000000 pdm_utils-0.9.9/src/pdm_utils/functions/server.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    11826 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/functions/tickets.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    15996 2021-01-04 13:42:59.000000 pdm_utils-0.9.9/src/pdm_utils/functions/url_basic.py
-drwxr-xr-x   0 cgauthier   (502) staff       (20)        0 2021-03-23 14:47:05.159849 pdm_utils-0.9.9/src/pdm_utils/pipelines/
--rw-r--r--   0 cgauthier   (502) staff       (20)        0 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/__init__.py
--rwxr-xr-x   0 cgauthier   (502) staff       (20)    60772 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/compare_db.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     8327 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/convert_db.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    33534 2021-01-18 11:10:57.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/export_db.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    26787 2020-11-16 18:55:34.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/find_domains.py
--rwxr-xr-x   0 cgauthier   (502) staff       (20)     7930 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/freeze_db.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    37362 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/get_data.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    16273 2021-01-05 20:24:45.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/get_db.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    10665 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/get_gb_records.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    89397 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/import_genome.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    12880 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/pham_finder.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    25213 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/pham_review.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    14262 2021-03-22 17:07:03.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/phamerate.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     7937 2020-12-09 18:03:02.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/push_db.py
--rw-r--r--   0 cgauthier   (502) staff       (20)    36577 2021-01-05 20:24:45.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/revise.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     5578 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/pipelines/update_field.py
--rw-r--r--   0 cgauthier   (502) staff       (20)     3179 2020-11-03 19:45:24.000000 pdm_utils-0.9.9/src/pdm_utils/run.py
-drwxr-xr-x   0 cgauthier   (502) staff       (20)        0 2021-03-23 14:47:05.108492 pdm_utils-0.9.9/src/pdm_utils.egg-info/
--rw-r--r--   0 cgauthier   (502) staff       (20)     1718 2021-03-23 14:47:04.000000 pdm_utils-0.9.9/src/pdm_utils.egg-info/PKG-INFO
--rw-r--r--   0 cgauthier   (502) staff       (20)     2651 2021-03-23 14:47:04.000000 pdm_utils-0.9.9/src/pdm_utils.egg-info/SOURCES.txt
--rw-r--r--   0 cgauthier   (502) staff       (20)        1 2021-03-23 14:47:04.000000 pdm_utils-0.9.9/src/pdm_utils.egg-info/dependency_links.txt
--rw-r--r--   0 cgauthier   (502) staff       (20)      125 2021-03-23 14:47:04.000000 pdm_utils-0.9.9/src/pdm_utils.egg-info/requires.txt
--rw-r--r--   0 cgauthier   (502) staff       (20)       10 2021-03-23 14:47:04.000000 pdm_utils-0.9.9/src/pdm_utils.egg-info/top_level.txt
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.116989 pdm_utils-1.0.0/
+-rw-r--r--   0 labad      (502) staff       (20)     1718 2023-06-15 00:24:09.116735 pdm_utils-1.0.0/PKG-INFO
+-rw-r--r--   0 labad      (502) staff       (20)      790 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/README.md
+-rw-r--r--   0 labad      (502) staff       (20)       38 2023-06-15 00:24:09.117067 pdm_utils-1.0.0/setup.cfg
+-rw-r--r--   0 labad      (502) staff       (20)     1287 2023-06-15 00:21:24.000000 pdm_utils-1.0.0/setup.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.074887 pdm_utils-1.0.0/src/
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.077621 pdm_utils-1.0.0/src/pdm_utils/
+-rw-r--r--   0 labad      (502) staff       (20)      146 2023-06-15 00:23:21.000000 pdm_utils-1.0.0/src/pdm_utils/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)      100 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/__main__.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.089856 pdm_utils-1.0.0/src/pdm_utils/classes/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)    20060 2020-10-30 13:34:57.000000 pdm_utils-1.0.0/src/pdm_utils/classes/alchemyhandler.py
+-rw-r--r--   0 labad      (502) staff       (20)     8100 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/classes/aragornhandler.py
+-rw-r--r--   0 labad      (502) staff       (20)    10410 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/bundle.py
+-rw-r--r--   0 labad      (502) staff       (20)    39957 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/cds.py
+-rw-r--r--   0 labad      (502) staff       (20)     2461 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/cdspair.py
+-rw-r--r--   0 labad      (502) staff       (20)     9923 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/dbcomparesummary.py
+-rw-r--r--   0 labad      (502) staff       (20)      696 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/evaluation.py
+-rw-r--r--   0 labad      (502) staff       (20)     7966 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/fileio.py
+-rw-r--r--   0 labad      (502) staff       (20)    23716 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/classes/filter.py
+-rw-r--r--   0 labad      (502) staff       (20)    41595 2021-09-22 16:59:23.000000 pdm_utils-1.0.0/src/pdm_utils/classes/genome.py
+-rw-r--r--   0 labad      (502) staff       (20)     5574 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/genomepair.py
+-rw-r--r--   0 labad      (502) staff       (20)    18395 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/genometriad.py
+-rw-r--r--   0 labad      (502) staff       (20)     1007 2020-11-17 06:11:51.000000 pdm_utils-1.0.0/src/pdm_utils/classes/progressbar.py
+-rw-r--r--   0 labad      (502) staff       (20)     7244 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/randomfieldupdatehandler.py
+-rw-r--r--   0 labad      (502) staff       (20)     4243 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/source.py
+-rw-r--r--   0 labad      (502) staff       (20)     8694 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/ticket.py
+-rw-r--r--   0 labad      (502) staff       (20)    37793 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/tmrna.py
+-rw-r--r--   0 labad      (502) staff       (20)    64069 2021-09-22 15:49:23.000000 pdm_utils-1.0.0/src/pdm_utils/classes/trna.py
+-rw-r--r--   0 labad      (502) staff       (20)     3694 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/classes/trnascansehandler.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.091629 pdm_utils-1.0.0/src/pdm_utils/constants/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/constants/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)     6806 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/constants/constants.py
+-rw-r--r--   0 labad      (502) staff       (20)    10763 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/constants/db_schema_0.py
+-rw-r--r--   0 labad      (502) staff       (20)    12305 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/constants/eval_descriptions.py
+-rw-r--r--   0 labad      (502) staff       (20)    37071 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/constants/schema_conversions.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.105227 pdm_utils-1.0.0/src/pdm_utils/functions/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)     6113 2020-10-30 13:34:57.000000 pdm_utils-1.0.0/src/pdm_utils/functions/annotation.py
+-rw-r--r--   0 labad      (502) staff       (20)    45918 2021-01-04 16:11:55.000000 pdm_utils-1.0.0/src/pdm_utils/functions/basic.py
+-rw-r--r--   0 labad      (502) staff       (20)     2962 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/cartography.py
+-rw-r--r--   0 labad      (502) staff       (20)     2166 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/configfile.py
+-rw-r--r--   0 labad      (502) staff       (20)     2853 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/functions/deeptmhmm.py
+-rw-r--r--   0 labad      (502) staff       (20)     4638 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/eval_modes.py
+-rw-r--r--   0 labad      (502) staff       (20)    10526 2021-03-23 03:57:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/fileio.py
+-rw-r--r--   0 labad      (502) staff       (20)    30706 2021-09-22 16:59:23.000000 pdm_utils-1.0.0/src/pdm_utils/functions/flat_files.py
+-rw-r--r--   0 labad      (502) staff       (20)     5302 2021-01-17 17:23:11.000000 pdm_utils-1.0.0/src/pdm_utils/functions/multithread.py
+-rw-r--r--   0 labad      (502) staff       (20)    27400 2022-10-18 17:47:46.000000 pdm_utils-1.0.0/src/pdm_utils/functions/mysqldb.py
+-rw-r--r--   0 labad      (502) staff       (20)    13414 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/mysqldb_basic.py
+-rw-r--r--   0 labad      (502) staff       (20)     6605 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/ncbi.py
+-rw-r--r--   0 labad      (502) staff       (20)     3656 2020-12-08 05:42:09.000000 pdm_utils-1.0.0/src/pdm_utils/functions/parallelize.py
+-rw-r--r--   0 labad      (502) staff       (20)    10972 2020-12-29 20:15:44.000000 pdm_utils-1.0.0/src/pdm_utils/functions/parsing.py
+-rw-r--r--   0 labad      (502) staff       (20)    13257 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/functions/phagesdb.py
+-rw-r--r--   0 labad      (502) staff       (20)     8567 2021-09-22 16:59:23.000000 pdm_utils-1.0.0/src/pdm_utils/functions/pham_alignment.py
+-rw-r--r--   0 labad      (502) staff       (20)    24951 2021-03-23 03:57:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/phameration.py
+-rw-r--r--   0 labad      (502) staff       (20)     8473 2021-01-04 16:11:55.000000 pdm_utils-1.0.0/src/pdm_utils/functions/pipeline_shells.py
+-rw-r--r--   0 labad      (502) staff       (20)     8828 2020-12-28 19:11:26.000000 pdm_utils-1.0.0/src/pdm_utils/functions/pipelines_basic.py
+-rw-r--r--   0 labad      (502) staff       (20)    30269 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/functions/querying.py
+-rw-r--r--   0 labad      (502) staff       (20)     3475 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/server.py
+-rw-r--r--   0 labad      (502) staff       (20)    11826 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/functions/tickets.py
+-rw-r--r--   0 labad      (502) staff       (20)    15996 2021-01-04 16:11:55.000000 pdm_utils-1.0.0/src/pdm_utils/functions/url_basic.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.116294 pdm_utils-1.0.0/src/pdm_utils/pipelines/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/__init__.py
+-rwxr-xr-x   0 labad      (502) staff       (20)    60772 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/compare_db.py
+-rw-r--r--   0 labad      (502) staff       (20)     8327 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/convert_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    33685 2021-09-22 16:59:23.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/export_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    26787 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/find_domains.py
+-rw-r--r--   0 labad      (502) staff       (20)      972 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/find_membrane.py
+-rw-r--r--   0 labad      (502) staff       (20)    14635 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/find_transmembrane.py
+-rwxr-xr-x   0 labad      (502) staff       (20)     7930 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/freeze_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    37362 2020-10-23 17:14:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/get_data.py
+-rw-r--r--   0 labad      (502) staff       (20)    16273 2021-01-05 20:20:36.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/get_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    10665 2020-10-30 13:34:57.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/get_gb_records.py
+-rw-r--r--   0 labad      (502) staff       (20)    91298 2021-09-17 01:24:47.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/import_genome.py
+-rw-r--r--   0 labad      (502) staff       (20)    12771 2021-09-17 01:23:58.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/pham_finder.py
+-rw-r--r--   0 labad      (502) staff       (20)    25213 2020-10-30 13:34:57.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/pham_review.py
+-rw-r--r--   0 labad      (502) staff       (20)    14262 2021-03-23 03:57:54.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/phamerate.py
+-rw-r--r--   0 labad      (502) staff       (20)     7937 2020-12-13 18:52:56.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/push_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    36843 2023-03-09 18:26:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/revise.py
+-rw-r--r--   0 labad      (502) staff       (20)     5642 2023-03-09 18:26:12.000000 pdm_utils-1.0.0/src/pdm_utils/pipelines/update_field.py
+-rw-r--r--   0 labad      (502) staff       (20)     3347 2023-06-09 12:21:12.000000 pdm_utils-1.0.0/src/pdm_utils/run.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-15 00:24:09.079292 pdm_utils-1.0.0/src/pdm_utils.egg-info/
+-rw-r--r--   0 labad      (502) staff       (20)     1718 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/PKG-INFO
+-rw-r--r--   0 labad      (502) staff       (20)     2775 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 labad      (502) staff       (20)        1 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 labad      (502) staff       (20)      125 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/requires.txt
+-rw-r--r--   0 labad      (502) staff       (20)       10 2023-06-15 00:24:08.000000 pdm_utils-1.0.0/src/pdm_utils.egg-info/top_level.txt
```

### Comparing `pdm_utils-0.9.9/PKG-INFO` & `pdm_utils-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm_utils
-Version: 0.9.9
+Version: 1.0.0
 Summary: MySQL phage genomics database management utilities
 Home-page: https://github.com/SEA-PHAGES/pdm_utils
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
 License: UNKNOWN
 Project-URL: Documentation, https://pdm-utils.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/SEA-PHAGES/pdm_utils/
```

### Comparing `pdm_utils-0.9.9/README.md` & `pdm_utils-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/setup.py` & `pdm_utils-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pdm_utils",
-    version="0.9.9",
+    version="1.0.0",
     author="Christian Gauthier",
     author_email="chg60@pitt.edu",
     description="MySQL phage genomics database management utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SEA-PHAGES/pdm_utils",
     packages=setuptools.find_packages(where="src"),
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/alchemyhandler.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/alchemyhandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/aragornhandler.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/aragornhandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,17 +122,17 @@
         Searches `out_str` for matches to a regular expression for
         Aragorn tRNAs of determinate isotype.
         :return:
         """
         # values:       aa., orient, start, stop,          anticodon,
         # indices:       0      1      2     3                 4
         re_str = "tRNA-(\w+)\s+(c)?\[(-?\d+),(\d+)\]\s+\d+\s+\((\w+)\)\s+" \
-                 "([.]*?\w+)\s+([( )dAtv.]*)"
-        # values:   sequence,  structure
-        # indices:     5           6
+                 "([.]*?\w+[.]*?)\s+([( )dAtv.]*)"
+        # values:     sequence,      structure
+        # indices:       5               6
         regex = re.compile(re_str, re.MULTILINE | re.DOTALL)
 
         trnas = regex.findall(self.out_str)
 
         # Iterate through tRNAs and create dictionaries for each
         for trna in trnas:
             trna_data = dict()
@@ -185,17 +185,17 @@
         Searches `out_str` for matches to a regular expression for
         Aragorn tRNAs of indeterminate isotype.
         :return:
         """
         # values: possible amino acids., orient, start, stop,
         # indices:          0      1        2      3     4
         re_str = "tRNA-\?\((\w+)\|(\w+)\)\s+(c)?\[(-?\d+),(\d+)\]\s+\d+\s+" \
-                 "\((\w+)\)\s+([.]*?\w+)\s+([( )dAtv.]*)"
-        # values: anticodon,   sequence, structure
-        # indices:    5           6          7
+                 "\((\w+)\)\s+([.]*?\w+[.]*?)\s+([( )dAtv.]*)"
+        # values: anticodon,      sequence,       structure
+        # indices:    5              6                7
         regex = re.compile(re_str, re.MULTILINE | re.DOTALL)
 
         trnas = regex.findall(self.out_str)
 
         # Iterate through tRNAs and create dictionaries for each
         for trna in trnas:
             trna_data = dict()
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/bundle.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/bundle.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/cds.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/cds.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/cdspair.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/cdspair.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/dbcomparesummary.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/dbcomparesummary.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/evaluation.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/evaluation.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/fileio.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/fileio.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/filter.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/filter.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/genome.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/genome.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from Bio.Seq import Seq
 from Bio.SeqUtils import GC
 
 from pdm_utils.classes import evaluation, cds, trna, tmrna, source
 from pdm_utils.constants import constants
 from pdm_utils.functions import basic
 
+
 class Genome:
     """Class to hold data about a phage genome."""
 
     def __init__(self):
 
         # The following attributes are common to any genome.
         self.nucleic_acid_type = "" # dsDNA, ssDNA, etc.
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/genomepair.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/genomepair.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/genometriad.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/genometriad.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/progressbar.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/progressbar.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/randomfieldupdatehandler.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/randomfieldupdatehandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/source.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/source.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/ticket.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/ticket.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/tmrna.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/tmrna.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/trna.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/trna.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 # Amino acids that Genbank allows in the product field
 GENBANK_AMINO_ACIDS = {"Ala", "Arg", "Asn", "Asp", "Cys", "Gln", "Glu", "Gly",
                        "His", "Ile", "Leu", "Lys", "Met", "Phe", "Pro", "Ser",
                        "Thr", "Trp", "Tyr", "Val", "OTHER"}
 
 # Additional amino acids that SEA-PHAGES may annotate in the note field
 SPECIAL_AMINO_ACIDS = {"fMet": "fMet", "Ile2": "Ile2", "Pyl": "Pyl",
-                       "SeC": "SeC", "Stop": "Stop", "Sup": "Stop",
-                       "Undet": "OTHER"}
+                       "SeC": "SeC", "Sec": "SeC", "Term": "Stop",
+                       "Stop": "Stop", "Sup": "Stop", "Undet": "OTHER"}
 
 # Extracts amino acid from product field
 PRODUCT_REGEX = re.compile("tRNA-(\w+)")
 
 # Extracts amino acid and anticodon from note field for Aragorn-determinate
 # or tRNAscan-SE- determinate or indeterminate tRNAs
 NOTE_STANDARD_REGEX = re.compile("tRNA-(\w+)\s?\((\w+)\)")
@@ -550,17 +550,17 @@
             amino_acid = results[0]
             # If amino acid we got is "OTHER", we need to check the note
             # field for a more specific amino acid
             if amino_acid == "OTHER":
                 results = NOTE_STANDARD_REGEX.findall(self.note)
                 # If we got two items (e.g. the amino acid and anticodon)
                 # and the amino acid is in our allowed special amino acids
-                if len(results) == 2 and results[0] in SPECIAL_AMINO_ACIDS:
+                if len(results) != 0 and results[0][0] in SPECIAL_AMINO_ACIDS:
                     # Use the re-formatted special amino acid
-                    amino_acid = SPECIAL_AMINO_ACIDS[results[0]]
+                    amino_acid = SPECIAL_AMINO_ACIDS[results[0][0]]
                 # Else, we will leave amino acid as "OTHER"
             # Else, there is nothing else to do but set the attribute
             self.amino_acid = amino_acid
         # Else, the product is not formatted properly and will fail checks
 
     def set_anticodon(self, value):
         """
@@ -576,21 +576,21 @@
         Attempts to parse the `anticodon` attribute from the `note`
         attribute.
         :return:
         """
         results = NOTE_STANDARD_REGEX.findall(self.note)
         # If we got two items (e.g. the amino acid and anticodon)
         if len(results) == 1:
-            self.anticodon = results[0][-1].lower()
+            self.anticodon = results[0][-1].lower().replace('u', 't')
         else:
             results = NOTE_SPECIAL_REGEX.findall(self.note)
             # If we got three items (e.g. the two amino acid choices and
             # part of anticodon)
             if len(results) == 1:
-                self.anticodon = results[0][-1].lower()
+                self.anticodon = results[0][-1].lower().replace('u', 't')
         # If the regex fails to parse an anticodon using either regex, it
         # will be left as "nnn"
 
     def set_structure(self, value):
         """
         Set the secondary structure string so downstream users can
         easily display the predicted fold of this tRNA.
@@ -1374,43 +1374,44 @@
                 # tRNA is annotated longer than Aragorn thinks it should be
                 structure = structure + ("." * stop_offset)
                 result += f"should be moved left by {stop_offset} base(s)."
 
         self.structure = structure
 
         definition = f"Check if the tRNA coordinates appear to match the " \
-                     f"Aragorn or tRNAscan-SE prediction(s) for {self.locus_tag} ({self.id})."
+                     f"Aragorn or tRNAscan-SE prediction(s) for " \
+                     f"{self.locus_tag} ({self.id})."
         definition = basic.join_strings([definition, eval_def])
         self.set_eval(eval_id, definition, result, status)
 
     def check_terminal_nucleotides(self, eval_id=None, success="correct",
-                                   fail="error", eval_def=None):
+                                   fail="warning", eval_def=None):
         """
         Checks that the tRNA ends with "CCA" or "CC" or "C".
         :param eval_id: unique identifier for the evaluation
         :type eval_id: str
         :param success: status if the outcome is successful
         :type success: str
         :param fail: status if the outcome is unsuccessful
         :type fail: str
         :param eval_def: description of the evaluation
         :type eval_def: str
         :return:
         """
         if len(self.seq) > 4:
             result = f"The tRNA ends with '...{self.seq[-4:]}'. "
-            # tRNAs must end in "NCCA" to function - some are this way naturally.
+            # tRNAs must end in "NCCA" to function - some are this way naturally
             # The others must end in "NCC" or "NC" or N
-            if self.seq[-3:] == "CCA":
+            if self.seq.endswith("CCA"):
                 result += "This is expected."
                 status = success
-            elif self.seq[-2:] == "CC":
+            elif self.seq.endswith("CC"):
                 result += "This is expected."
                 status = success
-            elif self.seq[-1:] == "C":
+            elif self.seq.endswith("C"):
                 result += "This is expected."
                 status = success
             else:
                 result += " This is not expected."
                 status = fail
         else:
             result = f"Cannot check terminal nucleotides on a sequence of " \
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/classes/trnascansehandler.py` & `pdm_utils-1.0.0/src/pdm_utils/classes/trnascansehandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/constants/constants.py` & `pdm_utils-1.0.0/src/pdm_utils/constants/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from Bio.Alphabet import IUPAC
 from Bio.Seq import Seq
 from datetime import datetime, date
 from pathlib import Path
 
 # pdm_utils is compatibile with this schema version.
-CODE_SCHEMA_VERSION = 10
+CODE_SCHEMA_VERSION = 11
 
 CURRENT_DATE = date.today().strftime("%Y%m%d")
 
 IMPORT_TABLE_STRUCTURE = {
     "order": [
                     "type",
                     "phage_id",
@@ -132,15 +132,15 @@
 # TODO this may no longer be needed, now that get_data pipeline
 # determines which new genomes to retrieve based on the
 # MySQL database instance instead of PhagesDB.
 UNPHAMERATED_PHAGE_LIST = "https://phagesdb.org/data/unphameratedlist"
 
 
 # Auto-annotations from PECAAN
-PECAAN_PREFIX = "https://discoverdev.kbrinsgd.org/phameratoroutput/phage/"
+PECAAN_PREFIX = "https://discover.kbrinsgd.org/phameratoroutput/phage/"
 
 
 # Phage name typo correction dictionary.
 # Key = Phage name as it is spelled in the GenBank-formatted record.
 # Value = Phage name as it is spelled in PhagesDB and/or the MySQL database, and thus
 # how it should be spelled in the import ticket.
 # The phage name parsed from the GenBank-formatted record gets
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/constants/db_schema_0.py` & `pdm_utils-1.0.0/src/pdm_utils/constants/db_schema_0.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/constants/eval_descriptions.py` & `pdm_utils-1.0.0/src/pdm_utils/constants/eval_descriptions.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/constants/schema_conversions.py` & `pdm_utils-1.0.0/src/pdm_utils/constants/schema_conversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,37 @@
         statements: [
             """ALTER TABLE `gene` MODIFY COLUMN `Translation` blob DEFAULT NULL;""",
             """UPDATE `version` SET `SchemaVersion` = 10;"""
             ],
         step_summary_dict: {}
         },
 
+    "upgrade_10_to_11": {
+        statements: [
+            """CREATE TABLE `gene_transmembrane` (
+                  `ID` int(10) unsigned NOT NULL AUTO_INCREMENT,
+                  `GeneID` varchar(35) DEFAULT NULL,
+                  `QueryStart` int(10) unsigned NOT NULL,
+                  `QueryEnd` int(10) unsigned NOT NULL,
+                  `Type` enum('signal', 'transmembrane') DEFAULT NULL,
+                  `Source`  enum('deeptmhmm', 'sosui') DEFAULT NULL,
+                  PRIMARY KEY (`ID`),
+                  KEY `GeneID` (`GeneID`),
+                  FOREIGN KEY (`GeneID`) REFERENCES `gene` (`GeneID`)
+                ) ENGINE=InnoDB DEFAULT CHARSET=latin1;""",
+            """ALTER TABLE `gene` ADD COLUMN `MembraneStatus` tinyint(1) NOT NULL AFTER `PhamID`;""",
+            """UPDATE `version` SET `SchemaVersion` = 11;"""
+            ],
+        step_summary_dict: {
+            inaccurate_column: [
+                "gene.MembraneStatus"
+                ]
+            }
+        },
+
     # Downgrade steps
     "downgrade_1_to_0": {
         statements: [
             """ALTER TABLE `gene` DROP COLUMN `cdd_status`;""",
             """ALTER TABLE `scores_summary` DROP FOREIGN KEY `scores_summary_ibfk_1`;""",
             """ALTER TABLE `scores_summary` DROP FOREIGN KEY `scores_summary_ibfk_2`;""",
             """ALTER TABLE `scores_summary`
@@ -687,9 +710,25 @@
             """UPDATE `gene` SET `Translation` = NULL WHERE LENGTH(`Translation`) > 5000;""",
             """ALTER TABLE `gene` MODIFY COLUMN `Translation` varchar(5000) DEFAULT NULL;""",
             """UPDATE `version` SET `SchemaVersion` = 9;"""
             ],
         step_summary_dict: {
             lost_data: ["gene.Translation"]
             }
+        },
+
+    "downgrade_11_to_10": {
+        statements: [
+            """DROP TABLE `gene_transmembrane`;""",
+            """ALTER TABLE `gene` DROP COLUMN `MembraneStatus`;""",
+            """UPDATE `version` SET `SchemaVersion` = 10;"""
+            ],
+        step_summary_dict: {
+            lost_table: [
+                "gene_transmembrane"
+                ],
+            lost_column: [
+                "gene.MembraneStatus"
+                ]
+            }
         }
     }
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/annotation.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/annotation.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/basic.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/cartography.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/cartography.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/configfile.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/configfile.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/eval_modes.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/eval_modes.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/fileio.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/fileio.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/flat_files.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/flat_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -616,32 +616,31 @@
     record.features = get_genome_seqrecord_features(phage_genome)
     record.description = get_genome_seqrecord_description(phage_genome)
     record.annotations = get_genome_seqrecord_annotations(phage_genome)
 
     return record
 
 
-def cds_to_seqrecord(cds, parent_genome, gene_domains=[]):
+def cds_to_seqrecord(cds, parent_genome, gene_domains=[], desc_type="gb"):
     """Creates a SeqRecord object from a Cds and its parent Genome.
 
     :param cds: A populated Cds object.
     :type cds: Cds
     :param phage_genome: Populated parent Genome object of the Cds object.
     :param domains: List of domain objects populated with column attributes
     :type domains: list
+    :param desc_type: Inteneded format of the CDS SeqRecord description.
+    :type desc_type: str
     :returns: Filled Biopython SeqRecord object.
     :rtype: SeqRecord
     """
     record = SeqRecord(cds.translation)
     record.seq.alphabet = IUPAC.IUPACProtein()
     record.name = cds.id
-    if cds.locus_tag == "" or cds.locus_tag is None:
-        record.id = "".join(["DRAFT ", cds.id])
-    else:
-        record.id = cds.locus_tag
+    record.id = cds.id
 
     cds.set_seqfeature()
 
     source = f"{parent_genome.host_genus} phage {cds.genome_id}"
     source_feature = cds.create_seqfeature("source", 0,
                                            cds.translation_length, 1)
     source_feature.qualifiers["organism"] = [source]
@@ -654,16 +653,37 @@
     format_cds_seqrecord_CDS_feature(cds_feature, cds, parent_genome)
     record.features.append(cds_feature)
 
     region_features = get_cds_seqrecord_regions(gene_domains, cds)
     for region_feature in region_features:
         record.features.append(region_feature)
 
-    record.description = (f"{cds.seqfeature.qualifiers['product'][0]} "
-                          f"[{source}]")
+    if desc_type == "fasta":
+        description = ""
+
+        product = cds.seqfeature.qualifiers["product"][0]
+        if product > "":
+            description = "".join([description, f"[product={product}]"])
+
+        cluster = parent_genome.cluster
+        if cluster > "":
+            description = " ".join([description, f"[cluster={cluster}]"])
+
+        host_genus = parent_genome.host_genus
+        if host_genus > "":
+            description = " ".join([description, f"[host_genus={host_genus}]"])
+
+        if cds.locus_tag > "":
+            description = " ".join([description, f"[locus={cds.locus_tag}]"])
+
+        record.description = description
+    elif desc_type == "gb":
+        description = f"{source} gp {cds.name}"
+        record.description = description
+
     record.annotations = get_cds_seqrecord_annotations(cds, parent_genome)
 
     return record
 
 
 def get_genome_seqrecord_features(phage_genome):
     """Helper function that uses Genome data to populate
@@ -789,16 +809,22 @@
 def get_cds_seqrecord_regions(gene_domains, cds):
     region_features = []
     for gene_domain in gene_domains:
         region_feature = cds.create_seqfeature("Region",
                                                gene_domain["QueryStart"],
                                                gene_domain["QueryEnd"], 1)
         region_feature.qualifiers["region_name"] = [gene_domain["Name"]]
-        region_feature.qualifiers["note"] = [
-                                    gene_domain["Description"].decode("utf-8")]
+
+        description = gene_domain["Description"]
+        if description is None:
+            description = ""
+        else:
+            description = description.decode("utf-8")
+        region_feature.qualifiers["note"] = [description]
+
         region_feature.qualifiers["db_xref"] = ["CDD:"
                                                 f"{gene_domain['DomainID']}"]
         region_features.append(region_feature)
 
     return region_features
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/multithread.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/multithread.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/mysqldb.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/mysqldb.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/mysqldb_basic.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/mysqldb_basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/ncbi.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/ncbi.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/parallelize.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/parallelize.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/parsing.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/parsing.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/phagesdb.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/phagesdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -412,15 +412,15 @@
 
 # TODO unittest.
 def get_unphamerated_phage_list(url):
     """Retreive list of unphamerated phages from PhagesDB.
 
     :param url:
         A URL from which to retrieve a list of PhagesDB genomes that are not
-        in the most up-to-date instance of the Actinobacteriophage
+        in the most up-to-date instance of the Actino_Draft
         MySQL database.
     :type url: str
     :returns: List of PhageIDs.
     :rtype: list
     """
     # Retrieved file is a tab-delimited text file.
     # Each row is a newly-sequenced phage.
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/pham_alignment.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/pham_alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import shlex
-import shutil
 from subprocess import (Popen, DEVNULL)
 
 from pdm_utils.functions import (fileio, multithread, parallelize)
 
 
 THREAD_LOCK_TIMEOUT = 10
 THREAD_JOIN_TIMEOUT = 30
@@ -43,27 +42,31 @@
     :return: Returns a dictionary mapping phams to translations to geneids
     :rtype: dict{dict}
     """
     engine = alchemist.engine
 
     # Build phage>>cluster lookup table
     cluster_lookup = dict()
-    query = "SELECT PhageID, Cluster, Subcluster FROM phage"
+    host_lookup = dict()
+    query = "SELECT PhageID, Cluster, Subcluster, HostGenus FROM phage"
     results = engine.execute(query)
     for result in results:
         phageid = result["PhageID"]
         cluster = result["Cluster"]
         subcluster = result["Subcluster"]
+        host = result["HostGenus"]
         if cluster is None:
             cluster_lookup[phageid] = "Singleton"
         elif subcluster is None:
             cluster_lookup[phageid] = cluster
         else:
             cluster_lookup[phageid] = subcluster
 
+        host_lookup[phageid] = host
+
     # Build pham>>translation>>gene lookup table
     phams = dict()
     query = ("SELECT PhamID, LocusTag, Name, Translation, Notes, PhageID "
              "FROM gene")
     results = engine.execute(query)
     for result in results:
         phageid = result["PhageID"]
@@ -71,20 +74,30 @@
         translation = result["Translation"].decode('utf-8')
         product = result["Notes"].decode('utf-8')
         phamid = result["PhamID"]
         if locus is not None:
             name = locus.split('_')[-1]
         else:
             name = result["Name"]
+
         geneid = f"{phageid}_{name}"
+
         if product is not None and product > "":
-            geneid += f" ({product})"
+            geneid = "".join([geneid, " [product=", str(product), "]"])
+
         cluster = cluster_lookup[phageid]
+        if cluster is not None and cluster > "":
+            geneid = "".join([geneid, " [cluster=", str(cluster), "]"])
+
+        host = host_lookup[phageid]
+        if host is not None and host > "":
+            geneid = "".join([geneid, " [host_genus=", str(host), "]"])
 
-        geneid = "".join(["[", cluster, "]", " ", geneid])
+        if locus is not None and locus > "":
+            geneid = "".join([geneid, " [locus=", str(locus), "]"])
 
         pham_translations = phams.get(phamid, dict())
         gene_ids = pham_translations.get(translation, [])
         gene_ids.append(geneid)
         pham_translations[translation] = gene_ids
         phams[phamid] = pham_translations
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/phameration.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/phameration.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/pipeline_shells.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/pipeline_shells.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/pipelines_basic.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/pipelines_basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/querying.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/querying.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/server.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/server.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/tickets.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/tickets.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/functions/url_basic.py` & `pdm_utils-1.0.0/src/pdm_utils/functions/url_basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/compare_db.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/compare_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/convert_db.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/convert_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import sys
 
 from pdm_utils.classes.alchemyhandler import AlchemyHandler
 from pdm_utils.functions import configfile
 from pdm_utils.functions import mysqldb, mysqldb_basic
 from pdm_utils.constants import schema_conversions
 
-MAX_VERSION = 10
-CURRENT_VERSION = 10
+MAX_VERSION = 11
+CURRENT_VERSION = 11
 VERSIONS = list(range(0, MAX_VERSION + 1))
 CHOICES = set(VERSIONS)
 
 
 # TODO unittest.
 def get_step_name(dir, step):
     """Generates the name of the script conversion filename."""
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/export_db.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/export_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,16 @@
 
     if table == "phage":
         seqrecords = get_genome_seqrecords(alchemist, values,
                                            data_cache=data_cache,
                                            verbose=verbose)
     elif table == "gene":
         seqrecords = get_cds_seqrecords(alchemist, values,
-                                        data_cache=data_cache, verbose=verbose)
+                                        data_cache=data_cache, verbose=verbose,
+                                        file_format=file_format)
     else:
         print(f"Unknown error occured, table '{table}' is not recognized "
               "for SeqRecord export pipelines.")
         sys.exit(1)
 
     if file_format == "tbl":
         fileio.write_feature_table(seqrecords, export_path, verbose=verbose)
@@ -611,15 +612,15 @@
         seqrecords.append(seqrecord)
 
     return seqrecords
 
 
 # TODO Document and Unittest
 def get_cds_seqrecords(alchemist, values, data_cache=None, nucleotide=False,
-                       verbose=False):
+                       verbose=False, file_format=None):
     if data_cache is None:
         data_cache = {}
 
     cds_list = parse_feature_data(alchemist, values=values)
 
     db_filter = Filter(alchemist)
     db_filter.key = 'gene.GeneID'
@@ -638,15 +639,16 @@
         cds.genome_length = parent_genome.length
         cds.set_seqfeature()
 
         db_filter.values = [cds.id]
         gene_domains = db_filter.select(CDD_DATA_COLUMNS)
 
         record = flat_files.cds_to_seqrecord(cds, parent_genome,
-                                             gene_domains=gene_domains)
+                                             gene_domains=gene_domains,
+                                             desc_type=file_format)
         seqrecords.append(record)
 
     return seqrecords
 
 
 def get_sort_columns(alchemist, sort_inputs):
     """Function that converts input for sorting to SQLAlchemy Columns.
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/find_domains.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/find_domains.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/freeze_db.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/freeze_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/get_data.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/get_data.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/get_db.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/get_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/get_gb_records.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/get_gb_records.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/import_genome.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/import_genome.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Primary pipeline to process and evaluate data to be imported
 into the MySQL database."""
 
 import argparse
-import csv
 from datetime import datetime, date
 import logging
 import os
 import pathlib
 import shutil
 import sys
 
@@ -33,25 +32,27 @@
 # main module being called, the top level main function configures
 # the root logger and primary file handle.
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 DEFAULT_OUTPUT_FOLDER = os.getcwd()
-IMPORT_DATE = datetime.today().replace(hour=0, minute=0, second=0, microsecond=0)
+IMPORT_DATE = datetime.today().replace(hour=0, minute=0, second=0,
+                                       microsecond=0)
 CURRENT_DATE = date.today().strftime("%Y%m%d")
 RESULTS_FOLDER = f"{CURRENT_DATE}_import"
 SUCCESS_FOLDER = "success"
 FAIL_FOLDER = "fail"
 GENOMES_FOLDER = "genomes"
 LOGS_FOLDER = "logs"
 VERSION = pdm_utils.__version__
 EDD = eval_descriptions.EVAL_DESCRIPTIONS
 MAIN_LOG_FILE = "import.log"
 
+
 def main(unparsed_args_list):
     """Runs the complete import pipeline.
 
     This is the only function of the pipeline that requires user input.
     All other functions can be implemented from other scripts.
 
     :param unparsed_args_list:
@@ -111,15 +112,15 @@
             import_table_file=args.import_table,
             genome_id_field=args.genome_id_field,
             host_genus_field=args.host_genus_field,
             prod_run=args.prod_run,
             description_field=args.description_field,
             eval_mode=args.eval_mode,
             output_folder=results_path,
-            interactive=args.interactive)
+            interactive=args.interactive, accept_warning=args.accept_warning)
 
     logger.info("Import complete.")
 
 
 def parse_args(unparsed_args_list):
     """Verify the correct arguments are selected for import new genomes.
 
@@ -157,14 +158,16 @@
     eval_mode_help = (
         "Indicates the evaluation configuration for importing genomes.")
     description_field_help = (
         "Indicates the field in CDS features that is expected "
         "to store the gene description.")
     interactive_help = (
         "Indicates whether interactive evaluation of data is permitted.")
+    accept_warning_help = (
+        "Indicates whether warnings are accepted without interactivity.")
     config_file_help = "Path to the file containing user-specific login data."
 
     parser = argparse.ArgumentParser(description=import_help)
     parser.add_argument("database", type=str, help=database_help)
     parser.add_argument("input_folder", type=pathlib.Path,
         help=input_folder_help)
     parser.add_argument("import_table", type=pathlib.Path,
@@ -187,35 +190,37 @@
     parser.add_argument("-d", "--description_field", type=str.lower,
         default="product", choices=list(constants.DESCRIPTION_FIELD_SET),
         help=description_field_help)
     parser.add_argument("-o", "--output_folder", type=pathlib.Path,
         default=pathlib.Path(DEFAULT_OUTPUT_FOLDER), help=output_folder_help)
     parser.add_argument("-i", "--interactive", action="store_true",
         default=False, help=interactive_help)
+    parser.add_argument("-Y", "--accept_warning", action="store_true",
+                        default=False, help=accept_warning_help)
     parser.add_argument("-c", "--config_file", type=pathlib.Path,
                         help=config_file_help, default=None)
 
 
     # Assumed command line arg structure:
     # python3 -m pdm_utils.run <pipeline> <additional args...>
     # sys.argv:      [0]            [1]         [2...]
     args = parser.parse_args(unparsed_args_list[2:])
 
     return args
 
 
-
-
 def data_io(engine=None, genome_folder=pathlib.Path(),
-    import_table_file=pathlib.Path(), genome_id_field="", host_genus_field="",
-    prod_run=False, description_field="", eval_mode="",
-    output_folder=pathlib.Path(), interactive=False):
+            import_table_file=pathlib.Path(), genome_id_field="",
+            host_genus_field="", prod_run=False, description_field="",
+            eval_mode="", output_folder=pathlib.Path(), interactive=False,
+            accept_warning=False):
     """Set up output directories, log files, etc. for import.
 
-    :param engine: SQLAlchemy Engine object able to connect to a MySQL database.
+    :param engine:
+        SQLAlchemy Engine object able to connect to a MySQL database.
     :type engine: Engine
     :param genome_folder: Path to the folder of flat files.
     :type genome_folder: Path
     :param import_table_file: Path to the import table file.
     :type import_table_file: Path
     :param genome_id_field:
         The SeqRecord attribute that stores the genome identifier/name.
@@ -231,16 +236,20 @@
     :param eval_mode:
         Name of the evaluation mode to evaluation genomes.
     :type eval_mode: str
     :param output_folder: Path to the folder to store results.
     :type output_folder: Path
     :param interactive:
         Indicates whether user is able to interact with genome evaluations
-        at run time.
+        at run time
     :type interactive: bool
+    :param accept_warning:
+        Toggles whether the import pipeline will accept warnings without
+        interactivity.
+    :type accept_warning: bool
     """
 
     logger.info("Setting up environment.")
     # Get the files to process.
     files_to_process = basic.identify_contents(genome_folder, kind="file",
                                                ignore_set=set([".DS_Store"]))
     file_msg = f"There are {len(files_to_process)} flat files to evaluate."
@@ -288,15 +297,15 @@
     # Evaluate files and tickets.
     results_tuple = process_files_and_tickets(
                         ticket_dict, files_to_process,
                         engine=engine,
                         prod_run=prod_run,
                         genome_id_field=genome_id_field,
                         host_genus_field=host_genus_field,
-                        interactive=interactive,
+                        interactive=interactive, accept_warning=accept_warning,
                         log_folder_paths_dict=log_folder_paths_dict)
     success_ticket_list = results_tuple[0]
     failed_ticket_list = results_tuple[1]
     success_filepath_list = results_tuple[2]
     failed_filepath_list = results_tuple[3]
     evaluation_dict = results_tuple[4]
 
@@ -407,15 +416,14 @@
                     logger.info(msg3)
 
     if logfile_path is not None:
         flatfile_logger.close()
         logger.removeHandler(flatfile_logger)
 
 
-
 def prepare_tickets(import_table_file=pathlib.Path(), eval_data_dict=None,
         description_field="", table_structure_dict={}):
     """Prepare dictionary of pdm_utils ImportTickets.
 
     :param import_table_file: same as for data_io().
     :param description_field: same as for data_io().
     :param eval_data_dict:
@@ -503,18 +511,20 @@
         logger.error("Error generating tickets from import table.")
         return None
     else:
         logger.info("Tickets were successfully generated from import table.")
 
         return ticket_dict
 
+
 def process_files_and_tickets(ticket_dict, files_in_folder, engine=None,
                               prod_run=False, genome_id_field="",
                               host_genus_field="", interactive=False,
-                              log_folder_paths_dict=None):
+                              log_folder_paths_dict=None,
+                              accept_warning=False):
     """Process GenBank-formatted flat files and import tickets.
 
     :param ticket_dict:
         A dictionary
         WHERE
         key (str) = The ticket's phage_id
         value (Ticket) = The ticket
@@ -522,14 +532,15 @@
     :param files_in_folder: A list of filepaths to be parsed.
     :type files_in_folder: list
     :param engine: same as for data_io().
     :param prod_run: same as for data_io().
     :param genome_id_field: same as for data_io().
     :param host_genus_field: same as for data_io().
     :param interactive: same as for data_io().
+    :param accept_warning: same as for data_io().
     :param log_folder_paths_dict:
         Dictionary indicating paths to success and fail folders.
     :type log_folder_paths_dict: dict
     :returns:
         tuple of five objects
         WHERE
         [0] success_ticket_list (list) is a list of successful ImportTickets.
@@ -600,15 +611,16 @@
                    seq_set=ref_data["seq_set"],
                    host_genus_set=ref_data["host_genera_set"],
                    cluster_set=ref_data["cluster_set"],
                    subcluster_set=ref_data["subcluster_set"],
                    file_ref=file_ref, ticket_ref=ticket_ref,
                    retrieve_ref=retrieve_ref, retain_ref=retain_ref)
 
-        review_bundled_objects(bndl, interactive=interactive)
+        review_bundled_objects(bndl, interactive=interactive,
+                               accept_warning=accept_warning)
 
         # TODO this section below could probably be improved.
         # import_into_db may not need to return result, since it now
         # records in an Evaluation object whether import succeeded or not.
         # It also checks_for_errors twice (before and after attempting to add
         # data to MySQL), which can probably be simplified.
         bndl.check_for_errors()
@@ -948,142 +960,160 @@
                              host_genus=gnm.host_genus)
 
         if retain_ref in bndl.genome_dict.keys():
             gnm2 = bndl.genome_dict[retain_ref]
             check_retain_genome(gnm2, tkt.type, eval_flags)
 
 
-def review_bundled_objects(bndl, interactive=False):
+def review_bundled_objects(bndl, interactive=False, accept_warning=False):
     """Review all evaluations of all bundled objects.
 
     Iterate through all objects stored in the bundle.
     If there are warnings, review whether status should be changed.
 
     :param bndl: same as for run_checks().
     :param interactive: same as for data_io().
+    :param accept_warnring: same as for data_io().
     """
 
     # Bundle-level evaluations.
-    review_object_list([bndl], "Bundle", ["id"], interactive=interactive)
+    review_object_list([bndl], "Bundle", ["id"], interactive=interactive,
+                       accept_warning=accept_warning)
 
     # Ticket-level evaluations.
     review_object_list([bndl.ticket], "Ticket", ["id", "type", "phage_id"],
-                       interactive=interactive)
+                       interactive=interactive, accept_warning=accept_warning)
 
     # Genome check.
     if len(bndl.genome_dict.keys()) > 0:
         for key in bndl.genome_dict.keys():
             gnm = bndl.genome_dict[key]
 
             # Genome-level evaluations.
             # Instead of passing all genomes from the genome_dict at one time,
             # it makes more sense to evaluate only one genome.evaluations list
             # at the same time as the evaluations for its cds, tRNA, tmRNA,
             # and source features.
             review_object_list([gnm], "Genome", ["id", "type"],
-                               interactive=interactive)
+                               interactive=interactive,
+                               accept_warning=accept_warning)
 
             review_object_list(gnm.cds_features, "CDS feature",
                                ["id", "start", "stop", "orientation"],
-                               interactive=interactive)
+                               interactive=interactive,
+                               accept_warning=accept_warning)
 
             review_object_list(gnm.source_features, "Source feature",
-                               ["id"], interactive=interactive)
+                               ["id"], interactive=interactive,
+                               accept_warning=accept_warning)
 
             review_object_list(gnm.trna_features, "tRNA feature",
                                ["id", "start", "stop", "orientation"],
-                               interactive=interactive)
+                               interactive=interactive,
+                               accept_warning=accept_warning)
 
             review_object_list(gnm.tmrna_features, "tmRNA feature",
                                ["id", "start", "stop", "orientation"],
-                               interactive=interactive)
+                               interactive=interactive,
+                               accept_warning=accept_warning)
 
     else:
         log_and_print("No genomes to review.", False)
 
     # Genome-pair check.
     genome_pair_list = list(bndl.genome_pair_dict.values())
     review_object_list(genome_pair_list, "Genome pair",
-                       ["genome1","genome2"], interactive=interactive)
+                       ["genome1","genome2"], interactive=interactive,
+                       accept_warning=accept_warning)
 
 
-def review_object_list(object_list, object_type, attr_list, interactive=False):
+def review_object_list(object_list, object_type, attr_list, interactive=False,
+                       accept_warning=False):
     """Determine if evaluations are present and record results.
 
     :param object_list: List of pdm_utils objects containing evaluations.
     :type object_list: list
     :param object_type: Name of the pdm_utils object.
     :type object_type: str
     :param attr_list:
         List of attributes used to log data about the object instance.
     :type attr_list: list
     :param interactive: same as for data_io().
+    :param accept_warning: same as for data_io().
     """
     # Test for None, since tkt data can be missing and be None.
     if (len(object_list) > 0 and object_list[0] is not None):
         # Capture the exit status for each CDS feature. If user exits
         # the review at any point, skip all of the other CDS features.
         exit = False
         for x in range(len(object_list)):
             object = object_list[x]
             # Compile description of the object being reviewed.
             string = get_result_string(object, attr_list)
             partial_msg = f"evaluations for {object_type}: {string}."
             if len(object.evaluations) > 0:
                 log_and_print("Reviewing " + partial_msg, interactive)
                 if exit == False:
-                    exit = review_evaluation_list(object.evaluations,
-                                interactive=interactive)
+                    exit = review_evaluation_list(
+                                                object.evaluations,
+                                                interactive=interactive,
+                                                accept_warning=accept_warning)
                 else:
                     # If exit=True, all 'warning' evaluations are automatically
                     # changed to 'error'. The exit response is not captured.
-                    review_evaluation_list(object.evaluations, interactive=False)
+                    review_evaluation_list(object.evaluations,
+                                           interactive=False,
+                                           accept_warning=False)
             else:
                 log_and_print("No " + partial_msg, False)
         if exit:
             msg = ("Not all evaluations were reviewed, "
                    "since the review was exited.")
             log_and_print(msg, False)
     else:
         log_and_print(f"No evaluations for {object_type}(s)", False)
 
 
-def review_evaluation_list(evaluation_list, interactive=False):
+def review_evaluation_list(evaluation_list, interactive=False,
+                           accept_warning=False):
     """Iterate through all evaluations and review 'warning' results.
 
     :param evaluation_list: List of pdm_utils Evaluation objects.
     :type evaluation_list: list
     :param interactive: same as for data_io().
+    :param accept_warning: same as for data_io().
     :returns: Indicates whether user selected to exit the review process.
     :rtype: bool
     """
     exit = False
     y = 0
     for x in range(len(evaluation_list)):
         evl = evaluation_list[x]
         if exit == False:
-            exit, correct = review_evaluation(evl, interactive=interactive)
+            exit, correct = review_evaluation(evl, interactive=interactive,
+                                              accept_warning=accept_warning)
         else:
             # If exit=True, then all 'warning' evaluations are automatically
             # changed to 'error'. The exit2 response is unused and thrown away.
             exit2, correct = review_evaluation(evl, interactive=False)
         if not correct:
             y += 1
 
     if y == 0:
         log_and_print(f"No warnings or errors encountered.", interactive)
     return exit
 
 
-def review_evaluation(evl, interactive=False):
+def review_evaluation(evl, interactive=False, accept_warning=False):
     """Review an evaluation object.
 
     :param evl: A pdm_utils Evaluation object.
     :type evl: Evaluation
     :param interactive: same as for data_io().
+    :param accept_warning: same as for data_io().
     :returns:
         tuple (exit, message)
         WHERE
         exit (bool) indicates whether user selected to exit the review process.
         correct(bool) indicates whether the evalution status is accurate.
     :rtype: tuple
     """
@@ -1109,14 +1139,16 @@
                 evl.status = "error"
                 if result == False:
                     evl.result = evl.result + msg.format("manually")
                 else:
                     exit = True
                     evl.result = evl.result + msg.format(
                                     "automatically due to review exit")
+        elif accept_warning:
+            pass
         else:
             # If interactive is set to False,
             # change all 'warnings' to 'errors'.
             evl.status = "error"
             evl.result = evl.result + msg.format(
                             "automatically due to no interactivity")
     elif evl.status == "error":
@@ -1254,16 +1286,16 @@
     print(msg)
     logger.info(msg)
 
     # Return either the original or the new description field.
     return new_field
 
 
-
-def check_bundle(bndl, ticket_ref="", file_ref="", retrieve_ref="", retain_ref=""):
+def check_bundle(bndl, ticket_ref="", file_ref="", retrieve_ref="",
+                 retain_ref=""):
     """Check a Bundle for errors.
 
     Evaluate whether all genomes have been successfully grouped,
     and whether all genomes have been paired, as expected.
     Based on the ticket type, there are expected to be certain
     types of genomes and pairs of genomes in the bundle.
 
@@ -1709,14 +1741,15 @@
         # TODO not implemented yet:
         #    cds_ftr.check_valid_description(eval_id="CDS-EVAL-013")
     if eval_flags["check_description_field"]:
         cds_ftr.check_description_field(attribute=description_field,
                                         eval_id="CDS-EVAL-012", fail="warning",
                                         eval_def=EDD["CDS-EVAL-012"])
 
+
 def compare_genomes(genome_pair, eval_flags):
     """Compare two genomes to identify discrepancies.
 
     :param genome_pair: A pdm_utils GenomePair object.
     :type genome_pair: GenomePair
     :param eval_flags: Dictionary of boolean evaluation flags.
     :type eval_flags: dicts
@@ -1867,17 +1900,17 @@
             eval_id="TRNA-EVAL-018", fail="warning",
             eval_def=EDD["TRNA-EVAL-018"])
         # 6. check_orientation_correct
         trna_ftr.check_orientation_correct(
             eval_id="TRNA-EVAL-016", fail="warning",
             eval_def=EDD["TRNA-EVAL-016"])
         # 7. check_terminal_nucleotides
-        trna_ftr.check_terminal_nucleotides(
-            eval_id="TRNA-EVAL-015", fail="warning",
-            eval_def=EDD["TRNA-EVAL-015"])
+        # trna_ftr.check_terminal_nucleotides(
+        #     eval_id="TRNA-EVAL-015", fail="warning",
+        #     eval_def=EDD["TRNA-EVAL-015"])
 
 
 def check_tmrna(tmrna_ftr, eval_flags):
     """Check a Tmrna object for errors.
 
     :param tmrna_ftr: A pdm_utils Cds object.
     :type tmrna_ftr: Tmrna
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/pham_finder.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/pham_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 from pathlib import Path
 
 from pdm_utils.functions import basic
 from pdm_utils.functions import configfile
 from pdm_utils.functions import fileio
 from pdm_utils.functions import pipelines_basic
 
-#GLOBAL VARIABLES
-#-----------------------------------------------------------------------------
+# GLOBAL VARIABLES
+# -----------------------------------------------------------------------------
 DEFAULT_FOLDER_NAME = f"{time.strftime('%Y%m%d')}_pham_finder"
 DEFAULT_FOLDER_PATH = Path.cwd()
 
 PHAM_FINDER_HEADER = ["Reference Pham", "Corresponding Phams"]
 
+
 def main(unparsed_args_list):
     """Uses parsed args to run the entirety of the pham_finder pipeline.
 
     :param unparsed_args_list: Input a list of command line args.
     :type unparsed_args_list: list[str]
     """
     args = parse_pham_finder(unparsed_args_list)
@@ -36,14 +37,15 @@
 
     execute_pham_finder(alchemist, args.folder_path, args.folder_name,
                         args.adatabase, args.bdatabase, values=values,
                         filters=args.filters, groups=args.groups, 
                         sort=args.sort, show_per=args.show_percentages,
                         use_locus=args.use_locus, verbose=args.verbose)
 
+
 def parse_pham_finder(unparsed_args_list):
     """Parses pham_finder arguments and stores them with an argparse object.
 
     :param unparsed_args_list: Input a list of command line args.
     :type unparsed_args_list: list[str]
     :returns: ArgParse module parsed args.
     """
@@ -147,16 +149,17 @@
                         config_file=None, verbose=False, input=[],
                         filters="", groups=[], sort=[],
                         show_percentages=False)
 
     parsed_args = parser.parse_args(unparsed_args_list[2:])
     return parsed_args
 
-#TODO Owen Needs unittests
-def execute_pham_finder(alchemist, folder_path, folder_name, 
+
+# TODO Owen Needs unittests
+def execute_pham_finder(alchemist, folder_path, folder_name,
                         adatabase, bdatabase, values=None,
                         filters="", groups=[], sort=[],
                         show_per=False, use_locus=False, verbose=False):
     """Executes the entirety of the file export pipeline.
 
     :param alchemist: A connected and fully build AlchemyHandler object.
     :type alchemist: AlchemyHandler
@@ -182,18 +185,18 @@
     :param sort: A list of supported MySQL column names to sort by.
     :type sort: list[str]
     :param show_per: Enables display gene coverage of the corresponding phams.
     :type show_per: bool
     :param use_locus: Toggles conversion between phams using LocusTag instead
     :type use_locus: bool
     """
-    if not (adatabase in alchemist.databases and \
+    if not (adatabase in alchemist.databases and
             bdatabase in alchemist.databases):
         print("User credentials does not have access to both "
-             f"databases {adatabase} and {bdatabase}.\n"
+              f"databases {adatabase} and {bdatabase}.\n"
               "Please check your database access and try again.")
         sys.exit(1)
 
     alchemist.database = adatabase
     alchemist.connect()
     a_filter = pipelines_basic.build_filter(alchemist, "gene.PhamID", filters,
                                             values=values, verbose=verbose)
@@ -206,68 +209,66 @@
         b_filter = pipelines_basic.build_filter(alchemist, "gene", "")
 
     if sort:
         try:
             a_filter.sort(sort)
         except:
             print("Please check your syntax for sorting columns:\n"
-                 f"{', '.join(sort)}")
+                  f"{', '.join(sort)}")
             sys.exit(1)
 
     if verbose:
         print("Creating pham_finder folder...")
     export_path = folder_path.joinpath(folder_name)
     export_path = basic.make_new_dir(folder_path, export_path, attempt=50)
 
-    conditionals_map = {}
-    pipelines_basic.build_groups_map(a_filter, export_path,
-                                        conditionals_map,
-                                        groups=groups,
-                                        verbose=verbose)
+    conditionals_map = pipelines_basic.build_groups_map(a_filter, export_path,
+                                                        groups=groups,
+                                                        verbose=verbose)
 
     if verbose:
         print("Prepared query and path structure, beginning export...")
 
     values = a_filter.values
     for mapped_path in conditionals_map.keys():
         a_filter.reset()
         a_filter.values = values
 
         conditionals = conditionals_map[mapped_path]
         a_filter.values = a_filter.build_values(where=conditionals)
-        
+
         if a_filter.hits() == 0:
             print("No database entries received from gene.PhamID "
-                 f"for '{mapped_path}'.")
+                  f"for '{mapped_path}'.")
             shutil.rmtree(mapped_path)
             continue
 
         if sort:
-            sort_columns = get_sort_columns(alchemist, sort)
-            a_filter.sort(sort_columns)
+            a_filter.sort(sort)
 
         mapped_phams = find_phams(a_filter, b_filter, show_per=show_per)
         if not mapped_phams:
             print("Phams are consistent between the two databases "
-                 f"for '{mapped_path}'.")
+                  f"for '{mapped_path}'.")
             shutil.rmtree(mapped_path)
             continue
 
         out_data_dicts = []
         for ref_pham, corr_phams in mapped_phams.items():
             data_dict = {}
             data_dict[PHAM_FINDER_HEADER[0]] = ref_pham
             data_dict[PHAM_FINDER_HEADER[1]] = corr_phams
             out_data_dicts.append(data_dict)
 
         file_path = mapped_path.joinpath("PhamMap.csv")
         fileio.export_data_dict(out_data_dicts, file_path, PHAM_FINDER_HEADER,
                                 include_headers=True)
 
-#TODO Owen Needs unittests
+
+# TODO Owen Needs unittests
 def find_phams(a_filter, b_filter, show_per=False, use_locus=False):
     """Find phams helper function that finds phams via GeneID intermediates.
 
     :param a_filter: Fully built Filter connected to the reference database.
     :type a_filter: Filter
     :param b_filter: Fully build Filter connected to a database.
     :type b_filter: Filter
@@ -319,14 +320,10 @@
                                         "(", str(percent), "%)"])
             corr_phams = ";".join([str(join_pham) for join_pham in phams_list])
 
         mapped_phams[pham] = corr_phams
         
     return mapped_phams
 
+
 if __name__ == "__main__":
     main(sys.argv)
-    
-
-
-
-
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/pham_review.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/pham_review.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/phamerate.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/phamerate.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/push_db.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/push_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/revise.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/revise.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         execute_local_revise(alchemist, args.revisions_file,
                              folder_path=args.folder_path,
                              folder_name=args.folder_name,
                              config=config, input_type=args.input_type,
                              output_type=args.output_type,
                              filters=args.filters, groups=args.groups,
                              verbose=args.verbose, force=args.force,
-                             production=args.production)
+                             production=args.production, draft=args.draft)
     elif args.pipeline == "remote":
         values = pipelines_basic.parse_value_input(args.input)
         execute_remote_revise(alchemist, folder_path=args.folder_path,
                               folder_name=args.folder_name, config=config,
                               values=values, filters=args.filters,
                               groups=args.groups, verbose=args.verbose,
                               output_type=args.output_type, force=args.force)
@@ -195,14 +195,15 @@
 
     local_parser.add_argument("-it", "--input_type", help=INPUT_TYPE_HELP,
                               choices=LOCAL_INPUT_FILE_TYPES)
     local_parser.add_argument("-ft", "--output_type", help=OUTPUT_TYPE_HELP,
                               choices=LOCAL_OUTPUT_FILE_TYPES)
     local_parser.add_argument("-p", "--production", help=PRODUCTION_HELP,
                               action="store_true")
+    local_parser.add_argument("-d", "--draft", action="store_true")
 
     remote_parser.add_argument("-if", "--import_file", dest="input",
                                type=pipelines_basic.convert_file_path,
                                help=IMPORT_FILE_HELP)
     remote_parser.add_argument("-in", "--import_names", nargs="*",
                                dest="input", help=SINGLE_GENOMES_HELP)
 
@@ -236,14 +237,15 @@
     return parsed_args
 
 
 def execute_local_revise(alchemist, revisions_file_path, folder_path=None,
                          folder_name=DEFAULT_FOLDER_NAME, config=None,
                          input_type="function_report",
                          output_type="p_curation", production=False,
+                         draft=False,
                          filters="", groups=[],
                          force=False, verbose=False):
     """Executes the entirety of the genbank local revise pipeline.
 
     :param alchemist: A connected and fully built AlchemyHandler object.
     :type alchemist: AlchemyHandler
     :param revisions_data_dicts: Data dictionaries containing pham/notes data.
@@ -298,15 +300,15 @@
     for mapped_path in conditionals_map.keys():
         conditionals = conditionals_map[mapped_path]
 
         if input_type == "function_report":
             export_dicts = use_function_report_data(
                                         db_filter, revisions_data_dicts,
                                         revise_columns, conditionals,
-                                        verbose=verbose)
+                                        verbose=verbose, draft=draft)
         elif input_type == "csv":
             export_dicts = use_csv_data(db_filter, revisions_data_dicts,
                                         revise_columns, conditionals,
                                         verbose=verbose)
 
         if not export_dicts:
             if verbose:
@@ -403,15 +405,15 @@
                                     CURATION_HEADER, include_headers=True)
 
 # LOCAL REVISE HELPER FUNCTIONS
 # -----------------------------------------------------------------------------
 
 
 def use_function_report_data(db_filter, data_dicts, columns, conditionals,
-                             verbose=False):
+                             verbose=False, draft=False):
     """Reads in FunctionReport data and pairs it with existing data.
 
     :param db_filter: A connected and fully built Filter object.
     :type db_filter: Filter
     :param data_dicts: List of data dictionaries from a FunctionReport file.
     :type data_dicts: list[dict]
     :param columns: List of SQLAlchemy Columns to retrieve data for.
@@ -425,27 +427,31 @@
         print("Retreiving feature data using pham function report...")
 
     export_dicts = []
     for data_dict in data_dicts:
         final_call = data_dict["Final Call"]
         if final_call.lower() == "hypothetical protein":
             final_call = ""
-        conditionals.append(querying.build_where_clause(
+
+        pham_conditionals = [condition for condition in conditionals]
+        pham_conditionals.append(querying.build_where_clause(
                             db_filter.graph, f"gene.Notes!='{final_call}'"))
 
         query = querying.build_select(db_filter.graph, columns,
-                                      where=conditionals)
+                                      where=pham_conditionals)
 
         results = querying.execute(db_filter.engine, query,
                                    in_column=db_filter.key,
                                    values=[data_dict["Pham"]])
 
         for result in results:
-            if (not result["Accession"]) or (not result["LocusTag"]):
-                continue
+            if not draft:
+                if (not result["Accession"]) or (not result["LocusTag"]):
+                    continue
+
             result["Notes"] = data_dict["Final Call"]
             result["Start"] = result["Start"] + 1
             export_dicts.append(result)
 
     return export_dicts
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/pipelines/update_field.py` & `pdm_utils-1.0.0/src/pdm_utils/pipelines/update_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,19 +111,22 @@
     key_value_count = mysqldb_basic.scalar(alchemist.engine, key_value_query)
 
     if key_value_count != 1:
         print(f"\nInvalid selection value '{update_ticket['key_value']}' "
               f"for key '{key_field.name}' in table '{table_obj.name}'")
         return 0
 
-    if update_ticket["value"] == "NULL":
-        update_ticket["value"] = None
+    value = update_ticket["value"]
+    if value == "NULL":
+        value = None
+    elif field.type.python_type == bytes:
+        value = value.encode("utf-8")
 
     statement = update(table_obj).where(key_value_clause).values(
-                                    {field.name : update_ticket["value"]})
+                                    {field.name : value})
     alchemist.engine.execute(statement)
     return 1
 
 
 # TODO unittest.
 def parse_args(unparsed_args_list):
     """Verify the correct arguments are selected for getting updates."""
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils/run.py` & `pdm_utils-1.0.0/src/pdm_utils/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,40 +4,43 @@
 """
 import argparse
 
 from pdm_utils.pipelines import compare_db
 from pdm_utils.pipelines import convert_db
 from pdm_utils.pipelines import export_db
 from pdm_utils.pipelines import find_domains
+from pdm_utils.pipelines import find_transmembrane
 from pdm_utils.pipelines import freeze_db
 from pdm_utils.pipelines import get_data
 from pdm_utils.pipelines import get_db
 from pdm_utils.pipelines import get_gb_records
 from pdm_utils.pipelines import import_genome
 from pdm_utils.pipelines import phamerate
 from pdm_utils.pipelines import pham_finder
 from pdm_utils.pipelines import push_db
 from pdm_utils.pipelines import revise
 from pdm_utils.pipelines import pham_review
 from pdm_utils.pipelines import update_field
 
 VALID_PIPELINES = {"compare", "convert", "export", "find_domains",
-                   "find_phams", "freeze", "get_data", "get_db",
-                   "get_gb_records", "import", "phamerate", "push",
+                   "find_transmembrane", "find_phams", "freeze", "get_data",
+                   "get_db", "get_gb_records", "import", "phamerate", "push",
                    "revise", "pham_review", "update"}
 
 
 def main(unparsed_args):
     """Run a pdm_utils pipeline."""
     args = parse_args(unparsed_args)
 
     if args.pipeline == "compare":
         compare_db.main(unparsed_args)
     elif args.pipeline == "convert":
         convert_db.main(unparsed_args)
+    elif args.pipeline == "find_transmembrane":
+        find_transmembrane.main(unparsed_args)
     elif args.pipeline == "export":
         export_db.main(unparsed_args)
     elif args.pipeline == "find_domains":
         find_domains.main(unparsed_args)
     elif args.pipeline == "find_phams":
         pham_finder.main(unparsed_args)
     elif args.pipeline == "freeze":
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils.egg-info/PKG-INFO` & `pdm_utils-1.0.0/src/pdm_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-utils
-Version: 0.9.9
+Version: 1.0.0
 Summary: MySQL phage genomics database management utilities
 Home-page: https://github.com/SEA-PHAGES/pdm_utils
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
 License: UNKNOWN
 Project-URL: Documentation, https://pdm-utils.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/SEA-PHAGES/pdm_utils/
```

### Comparing `pdm_utils-0.9.9/src/pdm_utils.egg-info/SOURCES.txt` & `pdm_utils-1.0.0/src/pdm_utils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 src/pdm_utils/constants/eval_descriptions.py
 src/pdm_utils/constants/schema_conversions.py
 src/pdm_utils/functions/__init__.py
 src/pdm_utils/functions/annotation.py
 src/pdm_utils/functions/basic.py
 src/pdm_utils/functions/cartography.py
 src/pdm_utils/functions/configfile.py
+src/pdm_utils/functions/deeptmhmm.py
 src/pdm_utils/functions/eval_modes.py
 src/pdm_utils/functions/fileio.py
 src/pdm_utils/functions/flat_files.py
 src/pdm_utils/functions/multithread.py
 src/pdm_utils/functions/mysqldb.py
 src/pdm_utils/functions/mysqldb_basic.py
 src/pdm_utils/functions/ncbi.py
@@ -57,14 +58,16 @@
 src/pdm_utils/functions/tickets.py
 src/pdm_utils/functions/url_basic.py
 src/pdm_utils/pipelines/__init__.py
 src/pdm_utils/pipelines/compare_db.py
 src/pdm_utils/pipelines/convert_db.py
 src/pdm_utils/pipelines/export_db.py
 src/pdm_utils/pipelines/find_domains.py
+src/pdm_utils/pipelines/find_membrane.py
+src/pdm_utils/pipelines/find_transmembrane.py
 src/pdm_utils/pipelines/freeze_db.py
 src/pdm_utils/pipelines/get_data.py
 src/pdm_utils/pipelines/get_db.py
 src/pdm_utils/pipelines/get_gb_records.py
 src/pdm_utils/pipelines/import_genome.py
 src/pdm_utils/pipelines/pham_finder.py
 src/pdm_utils/pipelines/pham_review.py
```

