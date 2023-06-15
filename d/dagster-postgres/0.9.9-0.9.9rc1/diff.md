# Comparing `tmp/dagster-postgres-0.9.9.tar.gz` & `tmp/dagster-postgres-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-postgres-0.9.9.tar", last modified: Thu Sep 17 21:27:49 2020, max compression
+gzip compressed data, was "dist/dagster-postgres-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:07 2020, max compression
```

## Comparing `dagster-postgres-0.9.9.tar` & `dagster-postgres-0.9.9rc1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)      148 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      576 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      134 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/
--rw-r--r--   0 bobchen    (501) staff       (20)      391 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/
--rw-r--r--   0 bobchen    (501) staff       (20)       47 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/
--rw-r--r--   0 bobchen    (501) staff       (20)      195 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/README
--rw-r--r--   0 bobchen    (501) staff       (20)     1034 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/alembic.ini
--rw-r--r--   0 bobchen    (501) staff       (20)     1984 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/env.py
--rw-r--r--   0 bobchen    (501) staff       (20)      494 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/script.py.mako
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/
--rw-r--r--   0 bobchen    (501) staff       (20)     1088 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/07f83cc13695_create_run_id_idx.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1108 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2759 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/567bc23fd1ac_.py
--rw-r--r--   0 bobchen    (501) staff       (20)      871 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/5c18fd3c2957_scheduler_update.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1541 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/727ffe943a9f_add_asset_key.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1486 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8688 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/event_log/event_log.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4953 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/pynotify.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/
--rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/
--rw-r--r--   0 bobchen    (501) staff       (20)      195 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/README
--rw-r--r--   0 bobchen    (501) staff       (20)     1034 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/alembic.ini
--rw-r--r--   0 bobchen    (501) staff       (20)     1969 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/env.py
--rw-r--r--   0 bobchen    (501) staff       (20)      494 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/script.py.mako
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/
--rw-r--r--   0 bobchen    (501) staff       (20)     1088 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/07f83cc13695_create_run_id_idx.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1108 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2759 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/567bc23fd1ac_.py
--rw-r--r--   0 bobchen    (501) staff       (20)      871 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/5c18fd3c2957_scheduler_update.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1541 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/727ffe943a9f_add_asset_key.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1486 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2898 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/run_storage/run_storage.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/
--rw-r--r--   0 bobchen    (501) staff       (20)       54 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/
--rw-r--r--   0 bobchen    (501) staff       (20)      195 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/README
--rw-r--r--   0 bobchen    (501) staff       (20)     1034 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/alembic.ini
--rw-r--r--   0 bobchen    (501) staff       (20)     1969 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/env.py
--rw-r--r--   0 bobchen    (501) staff       (20)      494 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/script.py.mako
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/
--rw-r--r--   0 bobchen    (501) staff       (20)     1088 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/07f83cc13695_create_run_id_idx.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1108 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2759 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/567bc23fd1ac_.py
--rw-r--r--   0 bobchen    (501) staff       (20)      871 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/5c18fd3c2957_scheduler_update.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1541 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/727ffe943a9f_add_asset_key.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1486 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2891 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/schedule_storage/schedule_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1576 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/utils.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      576 2020-09-17 21:27:48.000000 dagster-postgres-0.9.9/dagster_postgres.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)     3392 2020-09-17 21:27:48.000000 dagster-postgres-0.9.9/dagster_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:48.000000 dagster-postgres-0.9.9/dagster_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:48.000000 dagster-postgres-0.9.9/dagster_postgres.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       24 2020-09-17 21:27:48.000000 dagster-postgres-0.9.9/dagster_postgres.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       40 2020-09-17 21:27:48.000000 dagster-postgres-0.9.9/dagster_postgres.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/__init__.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/dagster_postgres_tests/compat_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/compat_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     8220 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/compat_tests/test_back_compat.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1234 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/compat_tests/test_migration_scripts.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2118 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/conftest.py
--rw-r--r--   0 bobchen    (501) staff       (20)    17189 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/test_event_log.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2102 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/test_instance.py
--rw-r--r--   0 bobchen    (501) staff       (20)     4840 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/test_run_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)      384 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/test_schedule_storage.py
--rw-r--r--   0 bobchen    (501) staff       (20)       94 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/dagster_postgres_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:27:49.000000 dagster-postgres-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:24:45.000000 dagster-postgres-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)      148 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      579 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      134 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/
+-rw-r--r--   0 bobchen    (501) staff       (20)      391 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/
+-rw-r--r--   0 bobchen    (501) staff       (20)       47 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/
+-rw-r--r--   0 bobchen    (501) staff       (20)      195 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/README
+-rw-r--r--   0 bobchen    (501) staff       (20)     1034 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/alembic.ini
+-rw-r--r--   0 bobchen    (501) staff       (20)     1984 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/env.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      494 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/script.py.mako
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/
+-rw-r--r--   0 bobchen    (501) staff       (20)     1088 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/07f83cc13695_create_run_id_idx.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1108 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2759 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/567bc23fd1ac_.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      871 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/5c18fd3c2957_scheduler_update.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1541 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/727ffe943a9f_add_asset_key.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1486 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     8688 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/event_log/event_log.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4953 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/pynotify.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/
+-rw-r--r--   0 bobchen    (501) staff       (20)       44 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/
+-rw-r--r--   0 bobchen    (501) staff       (20)      195 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/README
+-rw-r--r--   0 bobchen    (501) staff       (20)     1034 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/alembic.ini
+-rw-r--r--   0 bobchen    (501) staff       (20)     1969 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/env.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      494 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/script.py.mako
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/
+-rw-r--r--   0 bobchen    (501) staff       (20)     1088 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/07f83cc13695_create_run_id_idx.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1108 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2759 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/567bc23fd1ac_.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      871 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/5c18fd3c2957_scheduler_update.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1541 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/727ffe943a9f_add_asset_key.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1486 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2898 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/run_storage.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/
+-rw-r--r--   0 bobchen    (501) staff       (20)       54 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/
+-rw-r--r--   0 bobchen    (501) staff       (20)      195 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/README
+-rw-r--r--   0 bobchen    (501) staff       (20)     1034 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/alembic.ini
+-rw-r--r--   0 bobchen    (501) staff       (20)     1969 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/env.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      494 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/script.py.mako
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/
+-rw-r--r--   0 bobchen    (501) staff       (20)     1088 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/07f83cc13695_create_run_id_idx.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1108 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2759 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/567bc23fd1ac_.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      871 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/5c18fd3c2957_scheduler_update.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1541 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/727ffe943a9f_add_asset_key.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1486 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2891 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/schedule_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1576 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/utils.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      579 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)     3392 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       24 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       40 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/__init__.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     8220 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/test_back_compat.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1234 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/test_migration_scripts.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2118 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/conftest.py
+-rw-r--r--   0 bobchen    (501) staff       (20)    17189 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_event_log.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2102 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_instance.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     4840 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_run_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)      384 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_schedule_storage.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       94 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:07.000000 dagster-postgres-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1335 2020-09-17 21:04:59.000000 dagster-postgres-0.9.9rc1/setup.py
```

### Comparing `dagster-postgres-0.9.9/LICENSE` & `dagster-postgres-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/PKG-INFO` & `dagster-postgres-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-postgres
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for postgres
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-postgres
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/alembic.ini` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/env.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/07f83cc13695_create_run_id_idx.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/07f83cc13695_create_run_id_idx.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/567bc23fd1ac_.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/567bc23fd1ac_.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/5c18fd3c2957_scheduler_update.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/5c18fd3c2957_scheduler_update.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/727ffe943a9f_add_asset_key.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/727ffe943a9f_add_asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/event_log/event_log.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/event_log/event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/pynotify.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/pynotify.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/alembic.ini` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/env.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/07f83cc13695_create_run_id_idx.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/07f83cc13695_create_run_id_idx.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/567bc23fd1ac_.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/567bc23fd1ac_.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/5c18fd3c2957_scheduler_update.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/5c18fd3c2957_scheduler_update.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/727ffe943a9f_add_asset_key.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/727ffe943a9f_add_asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/run_storage/run_storage.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/run_storage/run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/alembic.ini` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/env.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/07f83cc13695_create_run_id_idx.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/07f83cc13695_create_run_id_idx.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/1ebdd7a9686f_add_step_key_pipeline_name.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/567bc23fd1ac_.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/567bc23fd1ac_.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/5c18fd3c2957_scheduler_update.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/5c18fd3c2957_scheduler_update.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/727ffe943a9f_add_asset_key.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/727ffe943a9f_add_asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/8f8dba68fd3b_cascade_run_deletion.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/alembic/versions/c63a27054f08_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/schedule_storage/schedule_storage.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/schedule_storage/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres/utils.py` & `dagster-postgres-0.9.9rc1/dagster_postgres/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres.egg-info/PKG-INFO` & `dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-postgres
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Dagster integration for postgres
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-postgres
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-postgres-0.9.9/dagster_postgres.egg-info/SOURCES.txt` & `dagster-postgres-0.9.9rc1/dagster_postgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres_tests/compat_tests/test_back_compat.py` & `dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/test_back_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres_tests/compat_tests/test_migration_scripts.py` & `dagster-postgres-0.9.9rc1/dagster_postgres_tests/compat_tests/test_migration_scripts.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres_tests/conftest.py` & `dagster-postgres-0.9.9rc1/dagster_postgres_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres_tests/test_event_log.py` & `dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres_tests/test_instance.py` & `dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/dagster_postgres_tests/test_run_storage.py` & `dagster-postgres-0.9.9rc1/dagster_postgres_tests/test_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-postgres-0.9.9/setup.py` & `dagster-postgres-0.9.9rc1/setup.py`

 * *Files identical despite different names*

