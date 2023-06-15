# Comparing `tmp/dbt-oracle-1.5.0rc1.tar.gz` & `tmp/dbt-oracle-1.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-oracle-1.5.0rc1.tar", last modified: Wed May 10 21:49:02 2023, max compression
+gzip compressed data, was "dbt-oracle-1.5.1rc1.tar", last modified: Thu Jun 15 17:12:17 2023, max compression
```

## Comparing `dbt-oracle-1.5.0rc1.tar` & `dbt-oracle-1.5.1rc1.tar`

### file list

```diff
@@ -1,119 +1,121 @@
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.404169 dbt-oracle-1.5.0rc1/
--rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt-oracle-1.5.0rc1/HISTORY.md
--rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt-oracle-1.5.0rc1/LICENSE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      259 2021-11-24 19:19:59.000000 dbt-oracle-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt-oracle-1.5.0rc1/NOTICE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-05-10 21:49:02.404362 dbt-oracle-1.5.0rc1/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     2015 2023-03-24 16:45:44.000000 dbt-oracle-1.5.0rc1/README.md
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.150342 dbt-oracle-1.5.0rc1/bin/
--rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt-oracle-1.5.0rc1/bin/create-pem-from-p12
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.152805 dbt-oracle-1.5.0rc1/dbt/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:47.000000 dbt-oracle-1.5.0rc1/dbt/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.154669 dbt-oracle-1.5.0rc1/dbt/adapters/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt-oracle-1.5.0rc1/dbt/adapters/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.172775 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      654 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__version__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/column.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4707 2023-03-24 16:45:44.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connection_helper.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    10683 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connections.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    12691 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/impl.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/keyword_catalog.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1354 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0rc1/dbt/adapters/oracle/relation.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.174615 dbt-oracle-1.5.0rc1/dbt/include/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:43.000000 dbt-oracle-1.5.0rc1/dbt/include/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.180484 dbt-oracle-1.5.0rc1/dbt/include/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      138 2021-11-08 19:31:21.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/dbt_project.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.198140 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)    14448 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/adapters.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/apply_grants.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     5447 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/catalog.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/columns.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.135121 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.210903 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4087 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     6918 2023-03-24 16:45:44.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.214059 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2022-03-30 23:05:21.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.226700 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/
--rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.229583 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/table/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4403 2023-01-21 00:48:03.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/table/table.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.232665 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.238576 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/view/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-01-21 00:48:03.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/view/view.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/schema_tests.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.310552 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/data_types.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/dateadd.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datediff.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datetrunc.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/except.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/hash.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/last_day.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/position.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/right.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/timestamps.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt-oracle-1.5.0rc1/dbt/include/oracle/profile_template.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.341211 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     4110 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/not-zip-safe
--rw-r--r--   0 abhisoms   (501) staff       (20)       49 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/requires.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)       10 2023-05-10 21:49:02.000000 dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/top_level.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt-oracle-1.5.0rc1/pyproject.toml
--rw-r--r--   0 abhisoms   (501) staff       (20)     1446 2023-05-10 21:49:02.406084 dbt-oracle-1.5.0rc1/setup.cfg
--rw-r--r--   0 abhisoms   (501) staff       (20)     2973 2023-05-10 21:24:58.000000 dbt-oracle-1.5.0rc1/setup.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.349241 dbt-oracle-1.5.0rc1/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/README.md
--rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt-oracle-1.5.0rc1/tests/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt-oracle-1.5.0rc1/tests/conftest.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.136285 dbt-oracle-1.5.0rc1/tests/functional/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.371791 dbt-oracle-1.5.0rc1/tests/functional/adapter/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.376784 dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/
--rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5635 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/fixtures.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6658 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/test_constraints.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.384419 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.389141 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.390833 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/sync_schema/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.392581 dbt-oracle-1.5.0rc1/tests/functional/adapter/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/macros/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/macros/test_alter_column_type.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.398334 dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1103 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/test_simple_seed.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.400175 dbt-oracle-1.5.0rc1/tests/functional/adapter/snapshots/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/snapshots/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_basic.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3038 2023-05-10 21:07:55.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_caching.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_concurrency.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4307 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_config.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_data_types.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_genreferences.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_ephemeral.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_generictests_where.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_grants.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/test_quoted_relations.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-05-10 21:49:02.403370 dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)     5777 2023-02-10 17:55:45.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_common_utils.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_dateutils.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.731519 dbt-oracle-1.5.1rc1/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt-oracle-1.5.1rc1/HISTORY.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt-oracle-1.5.1rc1/LICENSE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)      259 2021-11-24 19:19:59.000000 dbt-oracle-1.5.1rc1/MANIFEST.in
+-rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt-oracle-1.5.1rc1/NOTICE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-06-15 17:12:17.731717 dbt-oracle-1.5.1rc1/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2015 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc1/README.md
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.274199 dbt-oracle-1.5.1rc1/bin/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt-oracle-1.5.1rc1/bin/create-pem-from-p12
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.278561 dbt-oracle-1.5.1rc1/dbt/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:47.000000 dbt-oracle-1.5.1rc1/dbt/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.281213 dbt-oracle-1.5.1rc1/dbt/adapters/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt-oracle-1.5.1rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.300392 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      654 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/__version__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/column.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4707 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/connection_helper.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    11633 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/connections.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    16010 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/impl.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/keyword_catalog.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1354 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc1/dbt/adapters/oracle/relation.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.303137 dbt-oracle-1.5.1rc1/dbt/include/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:08:43.000000 dbt-oracle-1.5.1rc1/dbt/include/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.328338 dbt-oracle-1.5.1rc1/dbt/include/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      138 2021-11-08 19:31:21.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/dbt_project.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.346517 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)    14870 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/adapters.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/apply_grants.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5447 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/catalog.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/columns.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.237899 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.371106 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4373 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6918 2023-03-24 16:45:44.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.374613 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/python_model/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3412 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/python_model/python.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.378757 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/seed/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2022-03-30 23:05:21.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.400526 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.425796 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/table/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5486 2023-06-14 23:03:43.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/table/table.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.430916 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.437725 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/view/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-06-13 04:33:00.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/view/view.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/schema_tests.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.539295 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/data_types.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/dateadd.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/datediff.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/datetrunc.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/except.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/hash.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/last_day.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/position.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/right.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/timestamps.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt-oracle-1.5.1rc1/dbt/include/oracle/profile_template.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.597033 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3236 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4177 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 abhisoms   (501) staff       (20)       49 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/requires.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)       10 2023-06-15 17:12:17.000000 dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/top_level.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt-oracle-1.5.1rc1/pyproject.toml
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1446 2023-06-15 17:12:17.733257 dbt-oracle-1.5.1rc1/setup.cfg
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2973 2023-06-15 17:11:44.000000 dbt-oracle-1.5.1rc1/setup.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.636261 dbt-oracle-1.5.1rc1/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/README.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt-oracle-1.5.1rc1/tests/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt-oracle-1.5.1rc1/tests/conftest.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.240158 dbt-oracle-1.5.1rc1/tests/functional/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.679712 dbt-oracle-1.5.1rc1/tests/functional/adapter/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.684892 dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5635 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/fixtures.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6658 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/test_constraints.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.692247 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.698927 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.701920 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/sync_schema/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.722119 dbt-oracle-1.5.1rc1/tests/functional/adapter/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/macros/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/macros/test_alter_column_type.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.724696 dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      601 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1103 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/test_simple_seed.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.726755 dbt-oracle-1.5.1rc1/tests/functional/adapter/snapshots/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/snapshots/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_basic.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3038 2023-05-10 21:07:55.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_caching.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_concurrency.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4307 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_config.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_data_types.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_docs_genreferences.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_ephemeral.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_generictests_where.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_grants.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/test_quoted_relations.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2023-06-15 17:12:17.730716 dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5777 2023-02-10 17:55:45.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/test_common_utils.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/test_dateutils.py
```

### Comparing `dbt-oracle-1.5.0rc1/LICENSE.txt` & `dbt-oracle-1.5.1rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/PKG-INFO` & `dbt-oracle-1.5.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.5.0rc1
+Version: 1.5.1rc1
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.5.0rc1/README.md` & `dbt-oracle-1.5.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/bin/create-pem-from-p12` & `dbt-oracle-1.5.1rc1/bin/create-pem-from-p12`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/__init__.py` & `dbt-oracle-1.5.1rc1/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/adapters/__init__.py` & `dbt-oracle-1.5.1rc1/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__init__.py` & `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/__version__.py` & `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
 """
-version = "1.5.0"
+version = "1.5.1"
```

### Comparing `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/column.py` & `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/column.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connection_helper.py` & `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/connection_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/connections.py` & `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/connections.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 import time
 import uuid
 
 import dbt.exceptions
 from dbt.adapters.base import Credentials
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterResponse
+from dbt.events.functions import fire_event
+from dbt.events.types import ConnectionUsed, SQLQuery, SQLCommit, SQLQueryStatus
 from dbt.events import AdapterLogger
+from dbt.events.contextvars import get_node_info
+from dbt.utils import cast_to_str
 
 from dbt.version import __version__ as dbt_version
 from dbt.adapters.oracle.connection_helper import oracledb, SQLNET_ORA_CONFIG
 
 logger = AdapterLogger("oracle")
 
 
@@ -101,14 +105,17 @@
     cclass: Optional[str] = None
     purity: Optional[str] = None
 
     # Connection retry params
     retry_count: Optional[int] = 1
     retry_delay: Optional[int] = 3
 
+    # Fetch an auth token to run Python UDF
+    oml_auth_token_uri: Optional[str] = None
+
 
     _ALIASES = {
         'dbname': 'database',
         'pass': 'password',
     }
 
     @property
@@ -125,15 +132,15 @@
         """
         return (
             'user', 'database', 'schema',
             'protocol', 'host', 'port', 'tns_name',
             'service', 'connection_string',
             'shardingkey', 'supershardingkey',
             'cclass', 'purity', 'retry_count',
-            'retry_delay'
+            'retry_delay', 'oml_auth_token_uri'
         )
 
     @classmethod
     def __pre_deserialize__(cls, data: Dict[Any, Any]) -> Dict[Any, Any]:
         # If database is not defined as adapter credentials
         data = super().__pre_deserialize__(data)
         if "database" not in data:
@@ -289,31 +296,54 @@
         bindings: Optional[Any] = {},
         abridge_sql_log: bool = False
     ) -> Tuple[oracledb.Connection, Any]:
         connection = self.get_thread_connection()
         if auto_begin and connection.transaction_open is False:
             self.begin()
 
-        logger.debug('Using {} connection "{}".'
-                     .format(self.TYPE, connection.name))
+        fire_event(
+            ConnectionUsed(
+                conn_type=self.TYPE,
+                conn_name=cast_to_str(connection.name),
+                node_info=get_node_info(),
+            )
+        )
 
         with self.exception_handler(sql):
             if abridge_sql_log:
                 log_sql = '{}...'.format(sql[:512])
             else:
                 log_sql = sql
 
-            logger.debug(f'On {connection.name}: f{log_sql}')
+            fire_event(
+                SQLQuery(
+                    conn_name=cast_to_str(connection.name), sql=log_sql, node_info=get_node_info()
+                )
+            )
+
             pre = time.time()
             cursor = connection.handle.cursor()
             cursor.execute(sql, bindings)
-            logger.debug(f"SQL status: {self.get_status(cursor)} in {(time.time() - pre)} seconds")
+            fire_event(
+                SQLQueryStatus(
+                    status=str(self.get_response(cursor)),
+                    elapsed=round((time.time() - pre)),
+                    node_info=get_node_info(),
+                )
+            )
             return connection, cursor
 
     def add_begin_query(self):
         connection = self.get_thread_connection()
         cursor = connection.handle.cursor
         return connection, cursor
 
     @classmethod
     def data_type_code_to_name(cls, type_code) -> str:
         return DATATYPES[type_code.name]
+
+    def commit(self):
+        connection = self.get_thread_connection()
+        fire_event(SQLCommit(conn_name=connection.name, node_info=get_node_info()))
+        self.add_commit_query()
+        connection.transaction_open = False
+        return connection
```

### Comparing `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/impl.py` & `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/impl.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,24 +10,26 @@
 
   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
 """
+import datetime
 from typing import (
     Optional, List, Set
 )
 from itertools import chain
 from typing import (
     Any,
     Callable,
     Dict)
 
 import agate
+import requests
 
 import dbt.exceptions
 from dbt.adapters.base.relation import BaseRelation, InformationSchema
 from dbt.adapters.base.impl import GET_CATALOG_MACRO_NAME, ConstraintSupport
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.base.meta import available
 from dbt.adapters.oracle import OracleAdapterConnectionManager
@@ -341,7 +343,73 @@
                 constraint = cls._parse_column_constraint(con)
                 c = cls.process_parsed_constraint(constraint, cls.render_column_constraint)
                 if c is not None:
                     rendered_column_constraint.append(c)
             rendered_column_constraints.append(" ".join(rendered_column_constraint))
 
         return rendered_column_constraints
+
+    def get_oml_auth_token(self) -> str:
+        if self.config.credentials.oml_auth_token_uri is None:
+            raise dbt.exceptions.DbtRuntimeError("oml_auth_token_uri should be set to run dbt-py models")
+        data = {
+            "grant_type": "password",
+            "username": self.config.credentials.user,
+            "password": self.config.credentials.password
+        }
+        try:
+            r = requests.post(url=self.config.credentials.oml_auth_token_uri,
+                              json=data)
+            r.raise_for_status()
+        except requests.exceptions.RequestException:
+            raise dbt.exceptions.DbtRuntimeError("Error getting OML OAuth2.0 token")
+        else:
+            return r.json()["accessToken"]
+
+    def submit_python_job(self, parsed_model: dict, compiled_code: str):
+        """Submit user defined Python function
+
+        The function pyqEval when used in Oracle Autonomous Database,
+        calls a user-defined Python function.
+
+        pyqEval(PAR_LST, OUT_FMT, SRC_NAME, SRC_OWNER, ENV_NAME)
+
+        - PAR_LST -> Parameter List
+        - OUT_FMT -> JSON clob of the columns
+        - ENV_NAME -> Name of conda environment
+
+
+        """
+        identifier = parsed_model["alias"]
+        oml_oauth_access_token = self.get_oml_auth_token()
+        py_q_script_name = f"{identifier}_dbt_py_script"
+        py_q_eval_output_fmt = '{"result":"number"}'
+        py_q_eval_result_table = f"o$pt_dbt_pyqeval_{identifier}_tmp_{datetime.datetime.utcnow().strftime('%H%M%S')}"
+
+        conda_env_name = parsed_model["config"].get("conda_env_name")
+        if conda_env_name:
+            logger.info("Custom python environment is %s", conda_env_name)
+            py_q_eval_sql = f"""CREATE GLOBAL TEMPORARY TABLE {py_q_eval_result_table} 
+                                AS SELECT * FROM TABLE(pyqEval(par_lst => NULL, 
+                                                               out_fmt => ''{py_q_eval_output_fmt}'',
+                                                               scr_name => ''{py_q_script_name}'', 
+                                                               scr_owner => NULL, 
+                                                               env_name => ''{conda_env_name}''))"""
+        else:
+            py_q_eval_sql = f"""CREATE GLOBAL TEMPORARY TABLE {py_q_eval_result_table} 
+                                AS SELECT * FROM TABLE(pyqEval(par_lst => NULL, 
+                                                               out_fmt => ''{py_q_eval_output_fmt}'',
+                                                               scr_name => ''{py_q_script_name}'', 
+                                                               scr_owner => NULL))"""
+
+        py_exec_main_sql = f""" 
+                BEGIN
+                   sys.pyqSetAuthToken('{oml_oauth_access_token}');
+                   sys.pyqScriptCreate('{py_q_script_name}', '{compiled_code.strip()}', FALSE, TRUE);
+                   EXECUTE IMMEDIATE '{py_q_eval_sql}';
+                   EXECUTE IMMEDIATE 'DROP TABLE {py_q_eval_result_table}';
+                   sys.pyqScriptDrop('{py_q_script_name}');
+                END;
+        """
+        response, _ = self.execute(sql=py_exec_main_sql)
+        logger.info(response)
+        return response
```

### Comparing `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/keyword_catalog.py` & `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/keyword_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/adapters/oracle/relation.py` & `dbt-oracle-1.5.1rc1/dbt/adapters/oracle/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/__init__.py` & `dbt-oracle-1.5.1rc1/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/__init__.py` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/adapters.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/adapters.sql`

 * *Files 2% similar despite different names*

```diff
@@ -132,37 +132,41 @@
   {%- endif %} table {{ relation.include(schema=(not temporary)) }}
   {% if temporary -%} on commit preserve rows {%- endif %}
   as
     {{ sql }}
 {%- endmacro %}
 
 
-{% macro oracle__create_table_as(temporary, relation, sql) -%}
-  {%- set sql_header = config.get('sql_header', none) -%}
-  {%- set parallel = config.get('parallel', none) -%}
-  {%- set compression_clause = config.get('table_compression_clause', none) -%}
-  {%- set contract_config = config.get('contract') -%}
-
-  {{ sql_header if sql_header is not none }}
-
-  create {% if temporary -%}
-    global temporary
-  {%- endif %} table {{ relation.include(schema=(not temporary)) }}
-  {%- if contract_config.enforced -%}
-      {{ get_assert_columns_equivalent(sql) }}
-      {{ get_table_columns_and_constraints() }}
-      {%- set sql = get_select_subquery(sql) %}
-  {% endif %}
-  {% if temporary -%} on commit preserve rows {%- endif %}
-  {% if not temporary -%}
-    {% if parallel %} parallel {{ parallel }}{% endif %}
-    {% if compression_clause %} {{ compression_clause }} {% endif %}
-  {%- endif %}
-  as
-    {{ sql }}
+{% macro oracle__create_table_as(temporary, relation, sql, language='sql') -%}
+ {%- if language == 'sql' -%}
+      {%- set sql_header = config.get('sql_header', none) -%}
+      {%- set parallel = config.get('parallel', none) -%}
+      {%- set compression_clause = config.get('table_compression_clause', none) -%}
+      {%- set contract_config = config.get('contract') -%}
+      {{ sql_header if sql_header is not none }}
+      create {% if temporary -%}
+        global temporary
+      {%- endif %} table {{ relation.include(schema=(not temporary)) }}
+      {%- if contract_config.enforced -%}
+          {{ get_assert_columns_equivalent(sql) }}
+          {{ get_table_columns_and_constraints() }}
+          {%- set sql = get_select_subquery(sql) %}
+      {% endif %}
+      {% if temporary -%} on commit preserve rows {%- endif %}
+      {% if not temporary -%}
+        {% if parallel %} parallel {{ parallel }}{% endif %}
+        {% if compression_clause %} {{ compression_clause }} {% endif %}
+      {%- endif %}
+      as
+        {{ sql }}
+{%- elif language == 'python' -%}
+    {{ py_write_table(compiled_code=compiled_code, target_relation=relation, temporary=temporary) }}
+  {%- else -%}
+      {% do exceptions.raise_compiler_error("oracle__create_table_as macro didn't get supported language, it got %s" % language) %}
+  {%- endif -%}
 
 {%- endmacro %}
 {% macro oracle__create_view_as(relation, sql) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
    {%- set contract_config = config.get('contract') -%}
    {%- if contract_config.enforced -%}
       {{ get_assert_columns_equivalent(sql) }}
```

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/apply_grants.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/catalog.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/columns.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql`

 * *Files 13% similar despite different names*

```diff
@@ -10,49 +10,53 @@
 
   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
 #}
-{% materialization incremental, adapter='oracle' %}
+{% materialization incremental, adapter='oracle', supported_languages=['sql', 'python'] %}
 
   {% set unique_key = config.get('unique_key') %}
   {% set full_refresh_mode = flags.FULL_REFRESH %}
-
+  {%- set language = model['language'] -%}
   {% set target_relation = this.incorporate(type='table') %}
   {% set existing_relation = load_relation(this) %}
   {% set tmp_relation = make_temp_relation(this) %}
   {% set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') %}
   {% set  grant_config = config.get('grants') %}
 
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
   -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% set to_drop = [] %}
   {% if existing_relation is none %}
-      {% set build_sql = create_table_as(False, target_relation, sql) %}
+      {% set build_sql = create_table_as(False, target_relation, sql, language) %}
   {% elif existing_relation.is_view or full_refresh_mode %}
       {#-- Make sure the backup doesn't exist so we don't encounter issues with the rename below #}
       {% set backup_identifier = existing_relation.identifier ~ "__dbt_backup" %}
       {% set backup_relation = existing_relation.incorporate(path={"identifier": backup_identifier}) %}
       {% do adapter.drop_relation(backup_relation) %}
       {% if existing_relation.is_view %}
             {% do adapter.drop_relation(existing_relation) %}
       {% else %}
             {% do adapter.rename_relation(existing_relation, backup_relation) %}
       {% endif %}
-      {% set build_sql = create_table_as(False, target_relation, sql) %}
+      {% set build_sql = create_table_as(False, target_relation, sql, language) %}
       {% do to_drop.append(backup_relation) %}
   {% else %}
       {% set tmp_relation = make_temp_relation(target_relation) %}
       {% do to_drop.append(tmp_relation) %}
-      {% do run_query(create_table_as(True, tmp_relation, sql)) %}
+      {% call statement("make_tmp_relation", language=language) %}
+        {{create_table_as(True, tmp_relation, sql, language)}}
+      {% endcall %}
+      {#-- After this language should be SQL --#}
+      {% set language = 'sql' %}
       {% do adapter.expand_target_column_types(
              from_relation=tmp_relation,
              to_relation=target_relation) %}
       {% set dest_columns = process_schema_changes(on_schema_change, tmp_relation, existing_relation) %}
       {% if not dest_columns %}
         {% set dest_columns = adapter.get_columns_in_relation(existing_relation) %}
       {% endif %}
@@ -62,15 +66,15 @@
       {% set incremental_predicates = config.get('predicates', none) or config.get('incremental_predicates', none) %}
       {% set strategy_sql_macro_func = adapter.get_incremental_strategy_macro(context, incremental_strategy) %}
       {% set strategy_arg_dict = ({'target_relation': target_relation, 'temp_relation': tmp_relation, 'unique_key': unique_key, 'dest_columns': dest_columns, 'incremental_predicates': incremental_predicates }) %}
       {% set build_sql = strategy_sql_macro_func(strategy_arg_dict) %}
 
   {% endif %}
 
-  {% call statement("main") %}
+  {% call statement("main", language=language) %}
       {{ build_sql }}
   {% endcall %}
 
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=True) }}
```

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/seed/seed.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/table/table.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/view/view.sql`

 * *Files 26% similar despite different names*

```diff
@@ -10,89 +10,71 @@
 
   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
 #}
-{% materialization table, adapter='oracle' %}
-  {% set identifier = model['alias'] %}
-  {% set grant_config = config.get('grants') %}
-  {% set tmp_identifier = model['alias'] + '__dbt_tmp' %}
-  {% set backup_identifier = model['alias'] + '__dbt_backup' %}
-  {% set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) %}
-  {% set target_relation = api.Relation.create(identifier=identifier,
-                                                schema=schema,
-                                                database=database,
-                                                type='table') %}
-  {% set intermediate_relation = api.Relation.create(identifier=tmp_identifier,
-                                                      schema=schema,
-                                                      database=database,
-                                                      type='table') %}
-  -- the intermediate_relation should not already exist in the database; get_relation
-  -- will return None in that case. Otherwise, we get a relation that we can drop
-  -- later, before we try to use this name for the current operation
-  {% set preexisting_intermediate_relation = adapter.get_relation(identifier=tmp_identifier,
-                                                                   schema=schema,
-                                                                   database=database) %}
+{%- materialization view, adapter='oracle' -%}
+
+  {%- set identifier = model['alias'] -%}
+  {%- set grant_config = config.get('grants') -%}
+  {%- set backup_identifier = model['alias'] + '__dbt_backup' -%}
+
+  {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
+  {%- set target_relation = api.Relation.create(identifier=identifier, schema=schema, database=database,
+                                                type='view') -%}
   /*
-      See ../view/view.sql for more information about this relation.
+     This relation (probably) doesn't exist yet. If it does exist, it's a leftover from
+     a previous run, and we're going to try to drop it immediately. At the end of this
+     materialization, we're going to rename the "old_relation" to this identifier,
+     and then we're going to drop it. In order to make sure we run the correct one of:
+       - drop view ...
+       - drop table ...
+
+     We need to set the type of this relation to be the type of the old_relation, if it exists,
+     or else "view" as a sane default if it does not. Note that if the old_relation does not
+     exist, then there is nothing to move out of the way and subsequentally drop. In that case,
+     this relation will be effectively unused.
   */
-  {% set backup_relation_type = 'table' if old_relation is none else old_relation.type %}
-  {% set backup_relation = api.Relation.create(identifier=backup_identifier,
-                                                schema=schema,
-                                                database=database,
-                                                type=backup_relation_type) %}
+  {%- set backup_relation_type = 'view' if old_relation is none else old_relation.type -%}
+  {%- set backup_relation = api.Relation.create(identifier=backup_identifier,
+                                                schema=schema, database=database,
+                                                type=backup_relation_type) -%}
   -- as above, the backup_relation should not already exist
-  {% set preexisting_backup_relation = adapter.get_relation(identifier=backup_identifier,
+  {%- set preexisting_backup_relation = adapter.get_relation(identifier=backup_identifier,
                                                              schema=schema,
-                                                             database=database) %}
-
-
-    {% do log("Preexisting intermediate relation=" ~ preexisting_intermediate_relation) %}
-    {% do log("Preexisting backup relation=" ~ preexisting_backup_relation) %}
+                                                             database=database) -%}
 
+  {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
-  -- drop the temp relations if they exist already in the database
-  {{ drop_relation_if_exists(preexisting_intermediate_relation) }}
   {{ drop_relation_if_exists(preexisting_backup_relation) }}
 
-  {{ run_hooks(pre_hooks, inside_transaction=False) }}
-
   -- `BEGIN` happens here:
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
-  -- build model
-  {% call statement('main') %}
-    {{ create_table_as(False, intermediate_relation, sql) }}
-  {%- endcall %}
-
-  -- cleanup
-  {% if old_relation is not none %}
-      {% if old_relation.is_view %}
-            {% do adapter.drop_relation(old_relation) %}
-      {% else %}
-            {% do adapter.rename_relation(old_relation, backup_relation) %}
-      {% endif %}
+  -- if old_relation was a table
+  {% if old_relation is not none and old_relation.type == 'table' %}
+    {{ adapter.rename_relation(old_relation, backup_relation) }}
   {% endif %}
 
-  {{ adapter.rename_relation(intermediate_relation, target_relation) }}
+  -- build model
+  {% call statement('main') -%}
+    {{ create_view_as(target_relation, sql) }}
+  {%- endcall %}
 
-  {% do create_indexes(target_relation) %}
+  {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks, inside_transaction=True) }}
 
-  {% do persist_docs(target_relation, model) %}
-
-  -- `COMMIT` happens here
   {{ adapter.commit() }}
 
-  -- finally, drop the existing/backup relation after the commit
   {{ drop_relation_if_exists(backup_relation) }}
 
   {{ run_hooks(post_hooks, inside_transaction=False) }}
 
   {% set should_revoke = should_revoke(old_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
 
   {{ return({'relations': [target_relation]}) }}
-{% endmaterialization %}
+
+{%- endmaterialization -%}
```

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/schema_tests.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/schema_tests.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/data_types.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/dateadd.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datediff.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/datetrunc.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/datetrunc.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/except.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/except.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/hash.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/last_day.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/position.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/right.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/right.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/macros/utils/timestamps.sql` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt/include/oracle/profile_template.yml` & `dbt-oracle-1.5.1rc1/dbt/include/oracle/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/PKG-INFO` & `dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.5.0rc1
+Version: 1.5.1rc1
 Summary: dbt (data build tool) adapter for the Oracle database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
```

### Comparing `dbt-oracle-1.5.0rc1/dbt_oracle.egg-info/SOURCES.txt` & `dbt-oracle-1.5.1rc1/dbt_oracle.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 dbt/include/oracle/macros/adapters.sql
 dbt/include/oracle/macros/apply_grants.sql
 dbt/include/oracle/macros/catalog.sql
 dbt/include/oracle/macros/columns.sql
 dbt/include/oracle/macros/schema_tests.sql
 dbt/include/oracle/macros/materializations/incremental/incremental.sql
 dbt/include/oracle/macros/materializations/incremental/strategies.sql
+dbt/include/oracle/macros/materializations/python_model/python.sql
 dbt/include/oracle/macros/materializations/seed/seed.sql
 dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
 dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
 dbt/include/oracle/macros/materializations/snapshot/strategies.sql
 dbt/include/oracle/macros/materializations/table/table.sql
 dbt/include/oracle/macros/materializations/tests/helpers.sql
 dbt/include/oracle/macros/materializations/view/view.sql
```

### Comparing `dbt-oracle-1.5.0rc1/setup.cfg` & `dbt-oracle-1.5.1rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dbt-oracle
-version = 1.5.0
+version = 1.5.1
 description = dbt (data build tool) adapter for the Oracle database
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Oracle dbt
 author = Oracle
 license = Apache Software License 2.0
 classifiers = 
@@ -26,20 +26,20 @@
 
 [options]
 python_requires = >=3.7.2
 zip_safe = False
 packages = find:
 include_package_data = True
 install_requires = 
-	dbt-core==1.5.0
+	dbt-core==1.5.1
 	cx_Oracle==8.3.0
 	oracledb==1.3.1
 test_suite = tests
 test_requires = 
-	dbt-tests-adapter==1.5.0
+	dbt-tests-adapter==1.5.1
 	pytest
 scripts = 
 	bin/create-pem-from-p12
 
 [options.package_data]
 dbt = include/oracle/dbt_project.yml, include/oracle/macros/*.sql, include/oracle/macros/**/**/*.sql, include/oracle/profile_template.yml
```

### Comparing `dbt-oracle-1.5.0rc1/setup.py` & `dbt-oracle-1.5.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,35 +28,35 @@
 
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 
 requirements = [
-        "dbt-core==1.5.0",
+        "dbt-core==1.5.1",
         "cx_Oracle==8.3.0",
         "oracledb==1.3.1"
 ]
 
 test_requirements = [
-    "dbt-tests-adapter==1.5.0",
+    "dbt-tests-adapter==1.5.1",
     "pytest"
 ]
 
 project_urls = {
     'Documentation': 'https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile',
     'Source': 'https://github.com/oracle/dbt-oracle',
     'Bug Tracker': 'https://github.com/oracle/dbt-oracle/issues',
     'CI': 'https://github.com/oracle/dbt-oracle/actions',
     "Release Notes": "https://github.com/oracle/dbt-oracle/releases"
 }
 
 url = 'https://github.com/oracle/dbt-oracle'
 
-VERSION = '1.5.0rc1'
+VERSION = '1.5.1rc1'
 setup(
     author="Oracle",
     python_requires='>=3.7.2',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `dbt-oracle-1.5.0rc1/tests/README.md` & `dbt-oracle-1.5.1rc1/tests/README.md`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/__init__.py` & `dbt-oracle-1.5.1rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/conftest.py` & `dbt-oracle-1.5.1rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/__init__.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/fixtures.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/constraints/test_constraints.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/constraints/test_constraints.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/macros/test_alter_column_type.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/macros/test_alter_column_type.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/__init__.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/simple_seed/test_simple_seed.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/simple_seed/test_simple_seed.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_basic.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_caching.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_caching.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_concurrency.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_config.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_config.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_data_types.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_generate.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_docs_genreferences.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_docs_genreferences.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_ephemeral.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_generictests_where.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_generictests_where.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_grants.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/test_quoted_relations.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/test_quoted_relations.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_common_utils.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/test_common_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-oracle-1.5.0rc1/tests/functional/adapter/utils/test_dateutils.py` & `dbt-oracle-1.5.1rc1/tests/functional/adapter/utils/test_dateutils.py`

 * *Files identical despite different names*

