# Comparing `tmp/data_diff-0.7.7.tar.gz` & `tmp/data_diff-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.7.7.tar", max compression
+gzip compressed data, was "data_diff-0.7.8.tar", max compression
```

## Comparing `data_diff-0.7.7.tar` & `data_diff-0.7.8.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.7/LICENSE
--rw-r--r--   0        0        0     2696 2023-05-11 19:39:43.703801 data_diff-0.7.7/README.md
--rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.7/data_diff/__init__.py
--rw-r--r--   0        0        0    16024 2023-05-05 21:08:17.222127 data_diff-0.7.7/data_diff/__main__.py
--rw-r--r--   0        0        0      126 2023-05-15 21:10:13.082463 data_diff-0.7.7/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.7/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0    10067 2023-05-15 21:10:13.082649 data_diff-0.7.7/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.7/data_diff/config.py
--rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.7/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.7/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.7/data_diff/databases/base.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.7/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.7/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.7/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.7/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.7/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.7/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.7/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.7/data_diff/databases/presto.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.7/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.7/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.7/data_diff/databases/trino.py
--rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.7/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    14233 2023-05-15 21:10:13.082842 data_diff-0.7.7/data_diff/dbt.py
--rw-r--r--   0        0        0    18122 2023-05-15 21:10:13.083057 data_diff-0.7.7/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.7/data_diff/diff_tables.py
--rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.7/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.7/data_diff/info_tree.py
--rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.7/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.7/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.7/data_diff/parse_time.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.7/data_diff/query_utils.py
--rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.7/data_diff/sqeleton/__init__.py
--rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.7/data_diff/sqeleton/__main__.py
--rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.7/data_diff/sqeleton/abcs/__init__.py
--rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.7/data_diff/sqeleton/abcs/compiler.py
--rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.7/data_diff/sqeleton/abcs/database_types.py
--rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.7/data_diff/sqeleton/abcs/mixins.py
--rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.7/data_diff/sqeleton/bound_exprs.py
--rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.7/data_diff/sqeleton/databases/__init__.py
--rw-r--r--   0        0        0     9245 2023-05-15 21:10:13.083663 data_diff-0.7.7/data_diff/sqeleton/databases/_connect.py
--rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.7.7/data_diff/sqeleton/databases/base.py
--rw-r--r--   0        0        0    10135 2023-05-05 21:08:17.223531 data_diff-0.7.7/data_diff/sqeleton/databases/bigquery.py
--rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.7/data_diff/sqeleton/databases/clickhouse.py
--rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.7/data_diff/sqeleton/databases/databricks.py
--rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.7/data_diff/sqeleton/databases/duckdb.py
--rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.7/data_diff/sqeleton/databases/mssql.py
--rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.7/data_diff/sqeleton/databases/mysql.py
--rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.7/data_diff/sqeleton/databases/oracle.py
--rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.7/data_diff/sqeleton/databases/postgresql.py
--rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.7/data_diff/sqeleton/databases/presto.py
--rw-r--r--   0        0        0     6312 2023-05-05 21:08:17.223928 data_diff-0.7.7/data_diff/sqeleton/databases/redshift.py
--rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.7/data_diff/sqeleton/databases/snowflake.py
--rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.7/data_diff/sqeleton/databases/trino.py
--rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.7/data_diff/sqeleton/databases/vertica.py
--rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.7/data_diff/sqeleton/queries/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.7/data_diff/sqeleton/queries/api.py
--rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.7/data_diff/sqeleton/queries/ast_classes.py
--rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.7/data_diff/sqeleton/queries/base.py
--rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.7/data_diff/sqeleton/queries/compiler.py
--rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.7/data_diff/sqeleton/queries/extras.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.7/data_diff/sqeleton/query_utils.py
--rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.7/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.7/data_diff/sqeleton/schema.py
--rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.7/data_diff/sqeleton/utils.py
--rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.7/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.7/data_diff/thread_utils.py
--rw-r--r--   0        0        0     4322 2023-05-15 21:10:13.084169 data_diff-0.7.7/data_diff/tracking.py
--rw-r--r--   0        0        0     5646 2023-05-15 21:10:13.084338 data_diff-0.7.7/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-05-15 22:24:21.626159 data_diff-0.7.7/data_diff/version.py
--rwxr-xr-x   0        0        0     2831 2023-05-15 22:24:21.626341 data_diff-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     5332 1970-01-01 00:00:00.000000 data_diff-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.8/LICENSE
+-rw-r--r--   0        0        0     2696 2023-05-11 19:39:43.703801 data_diff-0.7.8/README.md
+-rw-r--r--   0        0        0     8710 2023-05-24 18:36:17.565800 data_diff-0.7.8/data_diff/__init__.py
+-rw-r--r--   0        0        0    16024 2023-05-05 21:08:17.222127 data_diff-0.7.8/data_diff/__main__.py
+-rw-r--r--   0        0        0      126 2023-05-15 21:10:13.082463 data_diff-0.7.8/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.8/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0    10067 2023-05-15 21:10:13.082649 data_diff-0.7.8/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.8/data_diff/config.py
+-rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.8/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.8/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.8/data_diff/databases/base.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.8/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.8/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.8/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.8/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.8/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.8/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.8/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.8/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.8/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.8/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.8/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.8/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    14911 2023-05-24 18:36:17.566053 data_diff-0.7.8/data_diff/dbt.py
+-rw-r--r--   0        0        0    18022 2023-05-24 18:36:17.566418 data_diff-0.7.8/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.8/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.8/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.8/data_diff/info_tree.py
+-rw-r--r--   0        0        0    15337 2023-05-24 18:36:17.566783 data_diff-0.7.8/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.8/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.8/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.8/data_diff/query_utils.py
+-rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.8/data_diff/sqeleton/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.8/data_diff/sqeleton/__main__.py
+-rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.8/data_diff/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.8/data_diff/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.8/data_diff/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.8/data_diff/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.8/data_diff/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.8/data_diff/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9245 2023-05-15 21:10:13.083663 data_diff-0.7.8/data_diff/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    20140 2023-05-11 19:39:43.705453 data_diff-0.7.8/data_diff/sqeleton/databases/base.py
+-rw-r--r--   0        0        0    10135 2023-05-05 21:08:17.223531 data_diff-0.7.8/data_diff/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.8/data_diff/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.8/data_diff/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.8/data_diff/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.8/data_diff/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.8/data_diff/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.8/data_diff/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.8/data_diff/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.8/data_diff/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     6297 2023-05-24 18:36:17.567499 data_diff-0.7.8/data_diff/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.8/data_diff/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.8/data_diff/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.8/data_diff/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.8/data_diff/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.8/data_diff/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.8/data_diff/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.8/data_diff/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.8/data_diff/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.8/data_diff/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.8/data_diff/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.8/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.8/data_diff/sqeleton/schema.py
+-rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.8/data_diff/sqeleton/utils.py
+-rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.8/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.8/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     4322 2023-05-15 21:10:13.084169 data_diff-0.7.8/data_diff/tracking.py
+-rw-r--r--   0        0        0     6600 2023-05-24 18:36:17.567734 data_diff-0.7.8/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-05-24 18:36:17.567903 data_diff-0.7.8/data_diff/version.py
+-rwxr-xr-x   0        0        0     2849 2023-05-24 18:36:17.569021 data_diff-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     5332 1970-01-01 00:00:00.000000 data_diff-0.7.8/PKG-INFO
```

### Comparing `data_diff-0.7.7/LICENSE` & `data_diff-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/README.md` & `data_diff-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/__init__.py` & `data_diff-0.7.8/data_diff/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,16 @@
     sample_exclusive_rows: bool = False,
     # Path of new table to write diff results to. Disabled if not provided. (joindiff only)
     materialize_to_table: Union[str, DbPath] = None,
     # Materialize every row, not just those that are different. (joindiff only)
     materialize_all_rows: bool = False,
     # Maximum number of rows to write when materializing, per thread. (joindiff only)
     table_write_limit: int = TABLE_WRITE_LIMIT,
+    # Skips diffing any rows with null keys. (joindiff only)
+    skip_null_keys: bool = False,
 ) -> Iterator:
     """Finds the diff between table1 and table2.
 
     Parameters:
         key_columns (Tuple[str, ...]): Name of the key column, which uniquely identifies each row (usually id)
         update_column (str, optional): Name of updated column, which signals that rows changed.
                                        Usually updated_at or last_update.  Used by `min_update` and `max_update`.
@@ -103,14 +105,15 @@
         validate_unique_key (bool): Enable/disable validating that the key columns are unique. (used for `JOINDIFF`. default: True)
                                     Single query, and can't be threaded, so it's very slow on non-cloud dbs.
                                     Future versions will detect UNIQUE constraints in the schema.
         sample_exclusive_rows (bool): Enable/disable sampling of exclusive rows. Creates a temporary table. (used for `JOINDIFF`. default: False)
         materialize_to_table (Union[str, DbPath], optional): Path of new table to write diff results to. Disabled if not provided. Used for `JOINDIFF`.
         materialize_all_rows (bool): Materialize every row, not just those that are different. (used for `JOINDIFF`. default: False)
         table_write_limit (int): Maximum number of rows to write when materializing, per thread.
+        skip_null_keys (bool): Skips diffing any rows with null PKs (displays a warning if any are null) (used for `JOINDIFF`. default: False)
 
     Note:
         The following parameters are used to override the corresponding attributes of the given :class:`TableSegment` instances:
         `key_columns`, `update_column`, `extra_columns`, `min_key`, `max_key`, `where`.
         If different values are needed per table, it's possible to omit them here, and instead set
         them directly when creating each :class:`TableSegment`.
 
@@ -164,12 +167,13 @@
             threaded=threaded,
             max_threadpool_size=max_threadpool_size,
             validate_unique_key=validate_unique_key,
             sample_exclusive_rows=sample_exclusive_rows,
             materialize_to_table=materialize_to_table,
             materialize_all_rows=materialize_all_rows,
             table_write_limit=table_write_limit,
+            skip_null_keys=skip_null_keys,
         )
     else:
         raise ValueError(f"Unknown algorithm: {algorithm}")
 
     return differ.diff_tables(*segments)
```

### Comparing `data_diff-0.7.7/data_diff/__main__.py` & `data_diff-0.7.8/data_diff/__main__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/cloud/data_source.py` & `data_diff-0.7.8/data_diff/cloud/data_source.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/cloud/datafold_api.py` & `data_diff-0.7.8/data_diff/cloud/datafold_api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/config.py` & `data_diff-0.7.8/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/databases/_connect.py` & `data_diff-0.7.8/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/dbt.py` & `data_diff-0.7.8/data_diff/dbt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 import os
 import time
 import webbrowser
+from typing import List, Optional, Dict
+import keyring
+
 import pydantic
 import rich
 from rich.prompt import Confirm
 
-from typing import List, Optional, Dict
-from .utils import (
-    dbt_diff_string_template,
-    getLogger,
-    columns_added_template,
-    columns_removed_template,
-    no_differences_template,
-)
-from pathlib import Path
-
-import keyring
-
+from . import connect_to_table, diff_tables, Algorithm
 from .cloud import DatafoldAPI, TCloudApiDataDiff, TCloudApiOrgMeta, get_or_create_data_source
 from .dbt_parser import DbtParser, PROJECT_FILE
-
-
-logger = getLogger(__name__)
-
-
 from .tracking import (
     set_entrypoint_name,
     set_dbt_user_id,
     set_dbt_version,
     set_dbt_project_id,
     create_end_event_json,
     create_start_event_json,
     send_event_json,
     is_tracking_enabled,
 )
-from .utils import run_as_daemon, truncate_error
-from . import connect_to_table, diff_tables, Algorithm
+from .utils import (
+    dbt_diff_string_template,
+    getLogger,
+    columns_added_template,
+    columns_removed_template,
+    no_differences_template,
+    columns_type_changed_template,
+    run_as_daemon,
+    truncate_error,
+    print_version_info,
+)
+
+logger = getLogger(__name__)
 
 
 class TDiffVars(pydantic.BaseModel):
     dev_path: List[str]
     prod_path: List[str]
     primary_keys: List[str]
     connection: Dict[str, Optional[str]]
@@ -51,14 +49,15 @@
 
 def dbt_diff(
     profiles_dir_override: Optional[str] = None,
     project_dir_override: Optional[str] = None,
     is_cloud: bool = False,
     dbt_selection: Optional[str] = None,
 ) -> None:
+    print_version_info()
     diff_threads = []
     set_entrypoint_name("CLI-dbt")
     dbt_parser = DbtParser(profiles_dir_override, project_dir_override)
     models = dbt_parser.get_models(dbt_selection)
     datadiff_variables = dbt_parser.get_datadiff_variables()
     config_prod_database = datadiff_variables.get("prod_database")
     config_prod_schema = datadiff_variables.get("prod_schema")
@@ -135,15 +134,21 @@
     model,
 ) -> TDiffVars:
     dev_database = model.database
     dev_schema = model.schema_
 
     primary_keys = dbt_parser.get_pk_from_model(model, dbt_parser.unique_columns, "primary-key")
 
-    prod_database = config_prod_database if config_prod_database else dev_database
+    # "custom" dbt config database
+    if model.config.database:
+        prod_database = model.config.database
+    elif config_prod_database:
+        prod_database = config_prod_database
+    else:
+        prod_database = dev_database
 
     # prod schema name differs from dev schema name
     if config_prod_schema:
         custom_schema = model.config.schema_
 
         # the model has a custom schema config(schema='some_schema')
         if custom_schema:
@@ -187,34 +192,44 @@
     diff_output_str = _diff_output_base(dev_qualified_str, prod_qualified_str)
 
     table1 = connect_to_table(diff_vars.connection, dev_qualified_str, tuple(diff_vars.primary_keys), diff_vars.threads)
     table2 = connect_to_table(
         diff_vars.connection, prod_qualified_str, tuple(diff_vars.primary_keys), diff_vars.threads
     )
 
-    table1_columns = list(table1.get_schema())
+    table1_columns = table1.get_schema()
     try:
-        table2_columns = list(table2.get_schema())
+        table2_columns = table2.get_schema()
     # Not ideal, but we don't have more specific exceptions yet
     except Exception as ex:
         logger.debug(ex)
         diff_output_str += "[red]New model or no access to prod table.[/] \n"
         rich.print(diff_output_str)
         return
 
-    column_set = set(table1_columns).intersection(table2_columns)
-    columns_added = set(table1_columns).difference(table2_columns)
-    columns_removed = set(table2_columns).difference(table1_columns)
+    table1_column_names = set(table1_columns.keys())
+    table2_column_names = set(table2_columns.keys())
+    column_set = table1_column_names.intersection(table2_column_names)
+    columns_added = table1_column_names.difference(table2_column_names)
+    columns_removed = table2_column_names.difference(table1_column_names)
+    # col type is i = 1 in tuple
+    columns_type_changed = {
+        k for k, v in table1_columns.items() if k in table2_columns and v[1] != table2_columns[k][1]
+    }
 
     if columns_added:
         diff_output_str += columns_added_template(columns_added)
 
     if columns_removed:
         diff_output_str += columns_removed_template(columns_removed)
 
+    if columns_type_changed:
+        diff_output_str += columns_type_changed_template(columns_type_changed)
+        column_set = column_set.difference(columns_type_changed)
+
     column_set = column_set - set(diff_vars.primary_keys)
 
     if diff_vars.include_columns:
         column_set = {x for x in column_set if x.upper() in [y.upper() for y in diff_vars.include_columns]}
 
     if diff_vars.exclude_columns:
         column_set = {x for x in column_set if x.upper() not in [y.upper() for y in diff_vars.exclude_columns]}
@@ -224,14 +239,15 @@
     diff = diff_tables(
         table1,
         table2,
         threaded=True,
         algorithm=Algorithm.JOINDIFF,
         extra_columns=extra_columns,
         where=diff_vars.where_filter,
+        skip_null_keys=True,
     )
 
     if list(diff):
         diff_output_str += f"{diff.get_stats_string(is_dbt=True)} \n"
         rich.print(diff_output_str)
     else:
         diff_output_str += no_differences_template()
@@ -317,15 +333,15 @@
         if columns_added:
             diff_output_str += columns_added_template(columns_added)
 
         if columns_removed:
             diff_output_str += columns_removed_template(columns_removed)
 
         if column_type_changes:
-            diff_output_str += "Type change: " + str(column_type_changes) + "\n"
+            diff_output_str += columns_type_changed_template(column_type_changes)
 
         if any([rows_added_count, rows_removed_count, rows_updated]):
             diff_output = dbt_diff_string_template(
                 rows_added_count,
                 rows_removed_count,
                 rows_updated,
                 str(rows_unchanged),
```

### Comparing `data_diff-0.7.7/data_diff/dbt_parser.py` & `data_diff-0.7.8/data_diff/dbt_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from argparse import Namespace
 from collections import defaultdict
 import json
-import os
 from pathlib import Path
 from typing import List, Dict, Tuple, Set, Optional
 import yaml
 
 from packaging.version import parse as parse_version
 import pydantic
 from dbt_artifacts_parser.parser import parse_run_results, parse_manifest
 from dbt.config.renderer import ProfileRenderer
 
 from .utils import getLogger, get_from_dict_with_raise
-from .version import __version__
 
 
 logger = getLogger(__name__)
 
 
 # getting this dbt_runner will only succeed in dbt-core>=1.5
 # it's needed for `--select` functionality
@@ -183,15 +181,14 @@
             )
 
         success_models = [x.unique_id for x in run_results_obj.results if x.status.name == "success"]
         models = [self.manifest_obj.nodes.get(x) for x in success_models]
         if not models:
             raise ValueError("Expected > 0 successful models runs from the last dbt command.")
 
-        print(f"Running with data-diff={__version__}\n")
         return models
 
     def get_manifest_obj(self):
         with open(self.project_dir / MANIFEST_PATH) as manifest:
             logger.info(f"Parsing file {MANIFEST_PATH}")
             manifest_dict = json.load(manifest)
             manifest_obj = parse_manifest(manifest=manifest_dict)
```

### Comparing `data_diff-0.7.7/data_diff/diff_tables.py` & `data_diff-0.7.8/data_diff/diff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/hashdiff_tables.py` & `data_diff-0.7.8/data_diff/hashdiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/info_tree.py` & `data_diff-0.7.8/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/joindiff_tables.py` & `data_diff-0.7.8/data_diff/joindiff_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,21 +127,23 @@
                                     If there are no UNIQUE constraints in the schema, it is done in a single query,
                                     and can't be threaded, so it's very slow on non-cloud dbs.
         sample_exclusive_rows (bool): Enable/disable sampling of exclusive rows. (default: False)
                                       Creates a temporary table.
         materialize_to_table (DbPath, optional): Path of new table to write diff results to. Disabled if not provided.
         materialize_all_rows (bool): Materialize every row, not just those that are different. (default: False)
         table_write_limit (int): Maximum number of rows to write when materializing, per thread.
+        skip_null_keys (bool): Skips diffing any rows with null PKs (displays a warning if any are null) (default: False)
     """
 
     validate_unique_key: bool = True
     sample_exclusive_rows: bool = False
     materialize_to_table: DbPath = None
     materialize_all_rows: bool = False
     table_write_limit: int = TABLE_WRITE_LIMIT
+    skip_null_keys: bool = False
 
     stats: dict = {}
 
     def _diff_tables_root(self, table1: TableSegment, table2: TableSegment, info_tree: InfoTree) -> DiffResult:
         db = table1.database
 
         if table1.database is not table2.database:
@@ -205,15 +207,19 @@
             logger.debug("Querying for different rows")
             diff = db.query(diff_rows, list)
             info_tree.info.set_diff(diff)
             for is_xa, is_xb, *x in diff:
                 if is_xa and is_xb:
                     # Can't both be exclusive, meaning a pk is NULL
                     # This can happen if the explicit null test didn't finish running yet
-                    raise ValueError("NULL values in one or more primary keys")
+                    if self.skip_null_keys:
+                        # warning is thrown in explicit null test
+                        continue
+                    else:
+                        raise ValueError("NULL values in one or more primary keys")
                 # _is_diff, a_row, b_row = _slice_tuple(x, len(is_diff_cols), len(a_cols), len(b_cols))
                 _is_diff, ab_row = _slice_tuple(x, len(is_diff_cols), len(a_cols) + len(b_cols))
                 a_row, b_row = ab_row[::2], ab_row[1::2]
                 assert len(a_row) == len(b_row)
                 if not is_xb:
                     yield "-", tuple(a_row)
                 if not is_xa:
@@ -248,15 +254,20 @@
         for ts in [table1, table2]:
             t = ts.make_select()
             key_columns = ts.key_columns
 
             q = t.select(*this[key_columns]).where(or_(this[k] == None for k in key_columns))
             nulls = ts.database.query(q, list)
             if nulls:
-                raise ValueError(f"NULL values in one or more primary keys of {ts.table_path}")
+                if self.skip_null_keys:
+                    logger.warning(
+                        f"NULL values in one or more primary keys of {ts.table_path}. Skipping rows with NULL keys."
+                    )
+                else:
+                    raise ValueError(f"NULL values in one or more primary keys of {ts.table_path}")
 
     def _collect_stats(self, i, table_seg: TableSegment, info_tree: InfoTree):
         logger.debug(f"Collecting stats for table #{i}")
         db = table_seg.database
 
         # Metrics
         col_exprs = merge_dicts(
```

### Comparing `data_diff-0.7.7/data_diff/lexicographic_space.py` & `data_diff-0.7.8/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/parse_time.py` & `data_diff-0.7.8/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/query_utils.py` & `data_diff-0.7.8/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/abcs/database_types.py` & `data_diff-0.7.8/data_diff/sqeleton/abcs/database_types.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/abcs/mixins.py` & `data_diff-0.7.8/data_diff/sqeleton/abcs/mixins.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/bound_exprs.py` & `data_diff-0.7.8/data_diff/sqeleton/bound_exprs.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/__init__.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/_connect.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/base.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/base.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/bigquery.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/bigquery.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/clickhouse.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/clickhouse.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/databricks.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/databricks.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/duckdb.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/mssql.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/mysql.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/oracle.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/oracle.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/postgresql.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/presto.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/presto.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/redshift.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/redshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,28 +144,28 @@
             scale = None
 
             if len(type_info) > 1:
                 if base_type == 'numeric':
                     precision, scale = type_info[1][:-1].split(',')
                     precision = int(precision)
                     scale = int(scale)
-                
+
             out = [col_name, base_type, None, precision, scale]
             output[col_name] = tuple(out)
 
         return output
 
     def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
         try:
             return super().query_table_schema(path)
         except RuntimeError:
             try:
-                return self.query_external_table_schema(path)	
-            except RuntimeError:	
-                return self.query_pg_get_cols() 
+                return self.query_external_table_schema(path)
+            except RuntimeError:
+                return self.query_pg_get_cols(path)
 
     def _normalize_table_path(self, path: DbPath) -> DbPath:
         if len(path) == 1:
             return None, self.default_schema, path[0]
         elif len(path) == 2:
             return None, path[0], path[1]
         elif len(path) == 3:
```

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/snowflake.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/trino.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/trino.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/databases/vertica.py` & `data_diff-0.7.8/data_diff/sqeleton/databases/vertica.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/queries/api.py` & `data_diff-0.7.8/data_diff/sqeleton/queries/api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/queries/ast_classes.py` & `data_diff-0.7.8/data_diff/sqeleton/queries/ast_classes.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/queries/compiler.py` & `data_diff-0.7.8/data_diff/sqeleton/queries/compiler.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/queries/extras.py` & `data_diff-0.7.8/data_diff/sqeleton/queries/extras.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/query_utils.py` & `data_diff-0.7.8/data_diff/sqeleton/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/repl.py` & `data_diff-0.7.8/data_diff/sqeleton/repl.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/schema.py` & `data_diff-0.7.8/data_diff/sqeleton/schema.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/sqeleton/utils.py` & `data_diff-0.7.8/data_diff/sqeleton/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/table_segment.py` & `data_diff-0.7.8/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/thread_utils.py` & `data_diff-0.7.8/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/tracking.py` & `data_diff-0.7.8/data_diff/tracking.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.7/data_diff/utils.py` & `data_diff-0.7.8/data_diff/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 import logging
 import re
 from typing import Dict, Iterable, Sequence
 from urllib.parse import urlparse
 import operator
 import threading
 from datetime import datetime
+from packaging.version import parse as parse_version
+import requests
 from tabulate import tabulate
+from .version import __version__
 
 
 def safezip(*args):
     "zip but makes sure all sequences are the same length"
     lens = list(map(len, args))
     if len(set(lens)) != 1:
         raise ValueError(f"Mismatching lengths in arguments to safezip: {lens}")
@@ -167,19 +170,42 @@
                 overriden_diff_cols.add(json_cols[i])
                 match = True
         if not match:
             break
     return match, overriden_diff_cols
 
 
-def columns_removed_template(table2_set_diff) -> str:
-    columns_removed = "Column(s) removed: " + str(table2_set_diff) + "\n"
-    return columns_removed
+def columns_removed_template(columns_removed) -> str:
+    columns_removed_str = f"Column(s) removed: {columns_removed}\n"
+    return columns_removed_str
 
 
-def columns_added_template(table1_set_diff) -> str:
-    columns_added = "Column(s) added: " + str(table1_set_diff) + "\n"
-    return columns_added
+def columns_added_template(columns_added) -> str:
+    columns_added_str = f"Column(s) added: {columns_added}\n"
+    return columns_added_str
+
+
+def columns_type_changed_template(columns_type_changed) -> str:
+    columns_type_changed_str = f"Type change: {columns_type_changed}\n"
+    return columns_type_changed_str
 
 
 def no_differences_template() -> str:
     return "[bold][green]No row differences[/][/]\n"
+
+
+def print_version_info() -> None:
+    base_version_string = f"Running with data-diff={__version__}"
+    logger = getLogger(__name__)
+    latest_version = None
+    try:
+        response = requests.get(url="https://pypi.org/pypi/data-diff/json", timeout=3)
+        response.raise_for_status()
+        response_json = response.json()
+        latest_version = response_json["info"]["version"]
+    except Exception as ex:
+        logger.debug(f"Failed checking version: {ex}")
+
+    if latest_version and parse_version(__version__) < parse_version(latest_version):
+        print(f"{base_version_string} (Update {latest_version} is available!)")
+    else:
+        print(base_version_string)
```

### Comparing `data_diff-0.7.7/pyproject.toml` & `data_diff-0.7.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.7.7"
+version = "0.7.8"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
@@ -30,15 +30,15 @@
     { version = "*", markers = "python_version >= '3.8.0'" }
 ]
 click = "^8.1"
 rich = "*"
 toml = "^0.10.2"
 mysql-connector-python = {version="8.0.29", optional=true}
 psycopg2 = {version="*", optional=true}
-snowflake-connector-python = {version="^2.7.2", optional=true}
+snowflake-connector-python = {version = ">=2.7.2,<4.0.0", optional=true}
 cryptography = {version="*", optional=true}
 trino = {version="^0.314.0", optional=true}
 presto-python-client = {version="*", optional=true}
 clickhouse-driver = {version="*", optional=true}
 duckdb = {version="^0.7.0", optional=true}
 dbt-artifacts-parser = {version="^0.3.0"}
 dbt-core = {version="^1.0.0"}
@@ -51,15 +51,15 @@
 
 [tool.poetry.dev-dependencies]
 parameterized = "*"
 unittest-parallel = "*"
 preql = "^0.2.19"
 mysql-connector-python = "*"
 psycopg2 = "*"
-snowflake-connector-python = "^2.7.2"
+snowflake-connector-python = ">=2.7.2,<4.0.0"
 cryptography = "*"
 trino = "^0.314.0"
 presto-python-client = "*"
 clickhouse-driver = "*"
 vertica-python = "*"
 duckdb = "^0.7.0"
 dbt-artifacts-parser = "^0.3.0"
```

### Comparing `data_diff-0.7.7/PKG-INFO` & `data_diff-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-diff
-Version: 0.7.7
+Version: 0.7.8
 Summary: Command-line tool and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff
 License: MIT
 Author: Datafold
 Author-email: data-diff@datafold.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -48,15 +48,15 @@
 Requires-Dist: keyring
 Requires-Dist: mysql-connector-python (==8.0.29) ; extra == "mysql"
 Requires-Dist: preql (>=0.2.19,<0.3.0) ; extra == "preql"
 Requires-Dist: presto-python-client ; extra == "presto"
 Requires-Dist: psycopg2 ; extra == "postgresql" or extra == "redshift"
 Requires-Dist: rich
 Requires-Dist: runtype (>=0.2.6,<0.3.0)
-Requires-Dist: snowflake-connector-python (>=2.7.2,<3.0.0) ; extra == "snowflake"
+Requires-Dist: snowflake-connector-python (>=2.7.2,<4.0.0) ; extra == "snowflake"
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: trino (>=0.314.0,<0.315.0) ; extra == "trino"
 Requires-Dist: urllib3 (<2)
 Requires-Dist: vertica-python ; extra == "vertica"
 Project-URL: Repository, https://github.com/datafold/data-diff
 Description-Content-Type: text/markdown
```

