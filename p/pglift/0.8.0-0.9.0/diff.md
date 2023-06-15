# Comparing `tmp/pglift-0.8.0.tar.gz` & `tmp/pglift-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pglift-0.8.0.tar", last modified: Fri Nov 26 10:23:37 2021, max compression
+gzip compressed data, was "pglift-0.9.0.tar", last modified: Fri Dec 10 13:35:12 2021, max compression
```

## Comparing `pglift-0.8.0.tar` & `pglift-0.9.0.tar`

### file list

```diff
@@ -1,153 +1,154 @@
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.771483 pglift-0.8.0/
--rw-r--r--   0 denis     (1000) denis     (1000)       82 2021-08-05 12:45:15.000000 pglift-0.8.0/.bandit
--rw-r--r--   0 denis     (1000) denis     (1000)      175 2021-10-28 12:51:54.000000 pglift-0.8.0/.gitignore
--rw-r--r--   0 denis     (1000) denis     (1000)    35147 2021-02-23 10:40:56.000000 pglift-0.8.0/LICENSE
--rw-r--r--   0 denis     (1000) denis     (1000)      522 2021-09-24 12:19:11.000000 pglift-0.8.0/MANIFEST.in
--rw-r--r--   0 denis     (1000) denis     (1000)     2609 2021-11-26 10:23:37.771483 pglift-0.8.0/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1000)     1281 2021-08-06 12:29:55.000000 pglift-0.8.0/README.md
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.751483 pglift-0.8.0/docs/
--rw-r--r--   0 denis     (1000) denis     (1000)      651 2021-06-04 14:32:42.000000 pglift-0.8.0/docs/Makefile
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.751483 pglift-0.8.0/docs/_static/
--rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-03-16 14:48:49.000000 pglift-0.8.0/docs/_static/.gitignore
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.751483 pglift-0.8.0/docs/_templates/
--rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-03-16 14:48:49.000000 pglift-0.8.0/docs/_templates/.gitignore
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.751483 pglift-0.8.0/docs/ansible/
--rw-r--r--   0 denis     (1000) denis     (1000)     1475 2021-11-26 07:59:11.000000 pglift-0.8.0/docs/ansible/play1.yml
--rw-r--r--   0 denis     (1000) denis     (1000)     1111 2021-11-26 07:59:11.000000 pglift-0.8.0/docs/ansible/play2.yml
--rw-r--r--   0 denis     (1000) denis     (1000)      400 2021-10-22 08:30:38.000000 pglift-0.8.0/docs/ansible/play3.yml
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.755483 pglift-0.8.0/docs/api/
--rw-r--r--   0 denis     (1000) denis     (1000)      191 2021-10-22 08:30:38.000000 pglift-0.8.0/docs/api/cmd.rst
--rw-r--r--   0 denis     (1000) denis     (1000)      174 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/api/conf.rst
--rw-r--r--   0 denis     (1000) denis     (1000)      146 2021-09-09 11:54:02.000000 pglift-0.8.0/docs/api/ctx.rst
--rw-r--r--   0 denis     (1000) denis     (1000)      947 2021-11-15 13:19:24.000000 pglift-0.8.0/docs/api/datamodel.rst
--rw-r--r--   0 denis     (1000) denis     (1000)      931 2021-09-14 10:02:57.000000 pglift-0.8.0/docs/api/exceptions.rst
--rw-r--r--   0 denis     (1000) denis     (1000)      319 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/api/index.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     5757 2021-10-20 13:19:11.000000 pglift-0.8.0/docs/conf.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1855 2021-10-22 08:30:38.000000 pglift-0.8.0/docs/dev.rst
--rw-r--r--   0 denis     (1000) denis     (1000)      303 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/index.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     1630 2021-11-04 12:45:24.000000 pglift-0.8.0/docs/install.rst
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.755483 pglift-0.8.0/docs/ops/
--rw-r--r--   0 denis     (1000) denis     (1000)     3148 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/ops/backup.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     1551 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/ops/databases.rst
--rw-r--r--   0 denis     (1000) denis     (1000)      253 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/ops/index.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     2230 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/ops/instance.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     1790 2021-09-20 12:40:04.000000 pglift-0.8.0/docs/ops/monitoring.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     2170 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/ops/privileges.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     1514 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/ops/roles.rst
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.755483 pglift-0.8.0/docs/setup/
--rw-r--r--   0 denis     (1000) denis     (1000)      273 2021-11-26 07:59:11.000000 pglift-0.8.0/docs/setup/index.rst
--rw-r--r--   0 denis     (1000) denis     (1000)      990 2021-11-26 07:59:11.000000 pglift-0.8.0/docs/setup/postgresql_authentication.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     1578 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/setup/postgresql_configuration.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     2425 2021-09-20 08:37:39.000000 pglift-0.8.0/docs/setup/settings.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     3149 2021-11-08 08:27:08.000000 pglift-0.8.0/docs/setup/systemd.rst
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.759483 pglift-0.8.0/docs/tutorials/
--rw-r--r--   0 denis     (1000) denis     (1000)     7553 2021-10-22 13:51:44.000000 pglift-0.8.0/docs/tutorials/ansible.rst
--rw-r--r--   0 denis     (1000) denis     (1000)     4363 2021-11-08 08:27:08.000000 pglift-0.8.0/docs/tutorials/cli.rst
--rw-r--r--   0 denis     (1000) denis     (1000)       96 2021-09-09 11:54:02.000000 pglift-0.8.0/docs/tutorials/index.rst
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.759483 pglift-0.8.0/extras/
--rw-r--r--   0 denis     (1000) denis     (1000)      669 2021-08-05 12:45:15.000000 pglift-0.8.0/extras/.pglift-complete.bash
--rw-r--r--   0 denis     (1000) denis     (1000)      669 2021-08-05 12:45:15.000000 pglift-0.8.0/extras/.pglift-complete.fish
--rw-r--r--   0 denis     (1000) denis     (1000)      966 2021-08-05 12:45:15.000000 pglift-0.8.0/extras/.pglift-complete.zsh
--rw-r--r--   0 denis     (1000) denis     (1000)      282 2021-08-05 12:45:15.000000 pglift-0.8.0/extras/README.md
--rw-r--r--   0 denis     (1000) denis     (1000)      336 2021-07-16 11:34:26.000000 pglift-0.8.0/pyproject.toml
--rw-r--r--   0 denis     (1000) denis     (1000)     1265 2021-11-26 10:23:37.775483 pglift-0.8.0/setup.cfg
--rw-r--r--   0 denis     (1000) denis     (1000)     2770 2021-11-24 12:38:19.000000 pglift-0.8.0/setup.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.751483 pglift-0.8.0/src/
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.763483 pglift-0.8.0/src/pglift/
--rw-r--r--   0 denis     (1000) denis     (1000)      392 2021-10-22 08:30:38.000000 pglift-0.8.0/src/pglift/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1000)       59 2021-09-09 11:54:05.000000 pglift-0.8.0/src/pglift/__main__.py
--rw-r--r--   0 denis     (1000) denis     (1000)      599 2021-11-08 08:10:17.000000 pglift-0.8.0/src/pglift/_compat.py
--rw-r--r--   0 denis     (1000) denis     (1000)     5422 2021-11-04 07:45:48.000000 pglift-0.8.0/src/pglift/_install.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1708 2021-09-14 10:02:57.000000 pglift-0.8.0/src/pglift/ansible.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2579 2021-11-15 13:19:24.000000 pglift-0.8.0/src/pglift/backup.py
--rw-r--r--   0 denis     (1000) denis     (1000)    34074 2021-11-26 07:59:11.000000 pglift-0.8.0/src/pglift/cli.py
--rw-r--r--   0 denis     (1000) denis     (1000)    10470 2021-11-08 12:13:12.000000 pglift-0.8.0/src/pglift/cmd.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2756 2021-11-12 09:57:17.000000 pglift-0.8.0/src/pglift/conf.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3464 2021-09-14 10:02:57.000000 pglift-0.8.0/src/pglift/ctx.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.751483 pglift-0.8.0/src/pglift/data/
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.763483 pglift-0.8.0/src/pglift/data/postgresql/
--rw-r--r--   0 denis     (1000) denis     (1000)      535 2021-06-04 14:32:42.000000 pglift-0.8.0/src/pglift/data/postgresql/pg_hba.conf
--rw-r--r--   0 denis     (1000) denis     (1000)       52 2021-06-10 13:40:45.000000 pglift-0.8.0/src/pglift/data/postgresql/pg_ident.conf
--rw-r--r--   0 denis     (1000) denis     (1000)      102 2021-07-16 11:34:26.000000 pglift-0.8.0/src/pglift/data/postgresql/site.conf
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.763483 pglift-0.8.0/src/pglift/data/systemd/
--rw-r--r--   0 denis     (1000) denis     (1000)      183 2021-11-04 07:45:48.000000 pglift-0.8.0/src/pglift/data/systemd/pglift-backup@.service
--rw-r--r--   0 denis     (1000) denis     (1000)      212 2021-11-04 07:45:48.000000 pglift-0.8.0/src/pglift/data/systemd/pglift-backup@.timer
--rw-r--r--   0 denis     (1000) denis     (1000)      467 2021-11-04 07:45:48.000000 pglift-0.8.0/src/pglift/data/systemd/pglift-postgres_exporter@.service
--rw-r--r--   0 denis     (1000) denis     (1000)      427 2021-11-04 07:45:48.000000 pglift-0.8.0/src/pglift/data/systemd/pglift-postgresql@.service
--rw-r--r--   0 denis     (1000) denis     (1000)     5749 2021-11-26 07:59:11.000000 pglift-0.8.0/src/pglift/databases.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2767 2021-11-26 07:59:11.000000 pglift-0.8.0/src/pglift/db.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2163 2021-09-14 10:02:57.000000 pglift-0.8.0/src/pglift/exceptions.py
--rw-r--r--   0 denis     (1000) denis     (1000)      983 2021-11-15 13:19:24.000000 pglift-0.8.0/src/pglift/hookspecs.py
--rw-r--r--   0 denis     (1000) denis     (1000)    24344 2021-11-26 07:59:11.000000 pglift-0.8.0/src/pglift/instance.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.763483 pglift-0.8.0/src/pglift/models/
--rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-09-09 11:54:05.000000 pglift-0.8.0/src/pglift/models/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1000)     9858 2021-11-24 15:52:38.000000 pglift-0.8.0/src/pglift/models/helpers.py
--rw-r--r--   0 denis     (1000) denis     (1000)    10872 2021-11-26 07:59:11.000000 pglift-0.8.0/src/pglift/models/interface.py
--rw-r--r--   0 denis     (1000) denis     (1000)     7348 2021-11-24 07:51:28.000000 pglift-0.8.0/src/pglift/models/system.py
--rw-r--r--   0 denis     (1000) denis     (1000)    12450 2021-11-26 07:59:11.000000 pglift-0.8.0/src/pglift/pgbackrest.py
--rw-r--r--   0 denis     (1000) denis     (1000)      904 2021-09-23 12:38:16.000000 pglift-0.8.0/src/pglift/pm.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1353 2021-11-04 07:45:48.000000 pglift-0.8.0/src/pglift/postgres.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2256 2021-11-25 15:31:27.000000 pglift-0.8.0/src/pglift/privileges.py
--rw-r--r--   0 denis     (1000) denis     (1000)    10134 2021-11-26 07:59:11.000000 pglift-0.8.0/src/pglift/prometheus.py
--rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-06-04 14:32:42.000000 pglift-0.8.0/src/pglift/py.typed
--rw-r--r--   0 denis     (1000) denis     (1000)     3574 2021-09-14 10:02:57.000000 pglift-0.8.0/src/pglift/queries.sql
--rw-r--r--   0 denis     (1000) denis     (1000)    10423 2021-11-26 07:59:11.000000 pglift-0.8.0/src/pglift/roles.py
--rw-r--r--   0 denis     (1000) denis     (1000)    12968 2021-11-26 07:59:11.000000 pglift-0.8.0/src/pglift/settings.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3771 2021-11-04 07:45:48.000000 pglift-0.8.0/src/pglift/systemd.py
--rw-r--r--   0 denis     (1000) denis     (1000)     4439 2021-11-08 13:14:23.000000 pglift-0.8.0/src/pglift/task.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1675 2021-11-24 08:50:07.000000 pglift-0.8.0/src/pglift/types.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3958 2021-09-20 12:40:04.000000 pglift-0.8.0/src/pglift/util.py
--rw-r--r--   0 denis     (1000) denis     (1000)      148 2021-09-14 10:02:57.000000 pglift-0.8.0/src/pglift/validators.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.763483 pglift-0.8.0/src/pglift.egg-info/
--rw-r--r--   0 denis     (1000) denis     (1000)     2609 2021-11-26 10:23:37.000000 pglift-0.8.0/src/pglift.egg-info/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1000)     3305 2021-11-26 10:23:37.000000 pglift-0.8.0/src/pglift.egg-info/SOURCES.txt
--rw-r--r--   0 denis     (1000) denis     (1000)        1 2021-11-26 10:23:37.000000 pglift-0.8.0/src/pglift.egg-info/dependency_links.txt
--rw-r--r--   0 denis     (1000) denis     (1000)       61 2021-11-26 10:23:37.000000 pglift-0.8.0/src/pglift.egg-info/entry_points.txt
--rw-r--r--   0 denis     (1000) denis     (1000)      463 2021-11-26 10:23:37.000000 pglift-0.8.0/src/pglift.egg-info/requires.txt
--rw-r--r--   0 denis     (1000) denis     (1000)        7 2021-11-26 10:23:37.000000 pglift-0.8.0/src/pglift.egg-info/top_level.txt
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.763483 pglift-0.8.0/tests/
--rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-09-09 11:54:05.000000 pglift-0.8.0/tests/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1000)      129 2021-11-25 15:31:27.000000 pglift-0.8.0/tests/conftest.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.767483 pglift-0.8.0/tests/data/
--rw-r--r--   0 denis     (1000) denis     (1000)      286 2021-09-20 12:41:43.000000 pglift-0.8.0/tests/data/ansible-argspec-database.json
--rw-r--r--   0 denis     (1000) denis     (1000)     1184 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/data/ansible-argspec-instance.json
--rw-r--r--   0 denis     (1000) denis     (1000)      684 2021-09-20 12:41:43.000000 pglift-0.8.0/tests/data/ansible-argspec-postgresexporter.json
--rw-r--r--   0 denis     (1000) denis     (1000)     1095 2021-09-20 12:41:43.000000 pglift-0.8.0/tests/data/ansible-argspec-role.json
--rw-r--r--   0 denis     (1000) denis     (1000)     3648 2021-09-20 12:41:42.000000 pglift-0.8.0/tests/data/queries.json
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.767483 pglift-0.8.0/tests/func/
--rw-r--r--   0 denis     (1000) denis     (1000)      350 2021-06-04 14:32:42.000000 pglift-0.8.0/tests/func/README.md
--rw-r--r--   0 denis     (1000) denis     (1000)     2325 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/func/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1000)     8406 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/func/conftest.py
--rw-r--r--   0 denis     (1000) denis     (1000)    14079 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/func/test_10_instance.py
--rw-r--r--   0 denis     (1000) denis     (1000)     5879 2021-11-25 15:31:27.000000 pglift-0.8.0/tests/func/test_11_databases.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2120 2021-11-25 15:31:27.000000 pglift-0.8.0/tests/func/test_11_privileges.py
--rw-r--r--   0 denis     (1000) denis     (1000)     8622 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/func/test_11_roles.py
--rw-r--r--   0 denis     (1000) denis     (1000)      764 2021-11-25 15:31:27.000000 pglift-0.8.0/tests/func/test_20_backup.py
--rw-r--r--   0 denis     (1000) denis     (1000)     4106 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/func/test_20_pgbackrest.py
--rw-r--r--   0 denis     (1000) denis     (1000)     7463 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/func/test_20_prometheus.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2754 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/func/test_99_drop.py
--rw-r--r--   0 denis     (1000) denis     (1000)     5790 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/func/test_ansible.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-11-26 10:23:37.771483 pglift-0.8.0/tests/unit/
--rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-09-09 11:54:05.000000 pglift-0.8.0/tests/unit/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2796 2021-09-20 12:40:04.000000 pglift-0.8.0/tests/unit/conftest.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2455 2021-11-04 07:45:48.000000 pglift-0.8.0/tests/unit/test__install.py
--rw-r--r--   0 denis     (1000) denis     (1000)      160 2021-11-04 07:45:48.000000 pglift-0.8.0/tests/unit/test_backup.py
--rw-r--r--   0 denis     (1000) denis     (1000)    33734 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/unit/test_cli.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2570 2021-09-24 11:39:15.000000 pglift-0.8.0/tests/unit/test_cmd.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1476 2021-10-26 08:31:18.000000 pglift-0.8.0/tests/unit/test_conf.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1861 2021-11-25 15:31:27.000000 pglift-0.8.0/tests/unit/test_db.py
--rw-r--r--   0 denis     (1000) denis     (1000)      469 2021-09-14 10:02:57.000000 pglift-0.8.0/tests/unit/test_exceptions.py
--rw-r--r--   0 denis     (1000) denis     (1000)     7268 2021-11-23 08:53:12.000000 pglift-0.8.0/tests/unit/test_instance.py
--rw-r--r--   0 denis     (1000) denis     (1000)    10059 2021-11-15 12:58:36.000000 pglift-0.8.0/tests/unit/test_models_helpers.py
--rw-r--r--   0 denis     (1000) denis     (1000)      706 2021-11-15 13:19:24.000000 pglift-0.8.0/tests/unit/test_models_interface.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3633 2021-11-24 07:51:28.000000 pglift-0.8.0/tests/unit/test_models_system.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2281 2021-11-03 14:16:08.000000 pglift-0.8.0/tests/unit/test_pgbackrest.py
--rw-r--r--   0 denis     (1000) denis     (1000)      446 2021-09-09 11:54:05.000000 pglift-0.8.0/tests/unit/test_pm.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1115 2021-09-14 10:02:57.000000 pglift-0.8.0/tests/unit/test_postgres.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1131 2021-11-04 07:45:48.000000 pglift-0.8.0/tests/unit/test_prometheus.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2676 2021-11-25 15:31:27.000000 pglift-0.8.0/tests/unit/test_roles.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3955 2021-11-26 07:59:11.000000 pglift-0.8.0/tests/unit/test_settings.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1143 2021-11-04 07:45:48.000000 pglift-0.8.0/tests/unit/test_systemd.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3142 2021-11-08 13:14:23.000000 pglift-0.8.0/tests/unit/test_task.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1130 2021-09-09 11:54:05.000000 pglift-0.8.0/tests/unit/test_util.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1039 2021-11-25 15:31:27.000000 pglift-0.8.0/tox.ini
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.716364 pglift-0.9.0/
+-rw-r--r--   0 denis     (1000) denis     (1000)       82 2021-08-05 12:45:15.000000 pglift-0.9.0/.bandit
+-rw-r--r--   0 denis     (1000) denis     (1000)      175 2021-12-09 09:26:03.000000 pglift-0.9.0/.gitignore
+-rw-r--r--   0 denis     (1000) denis     (1000)    35147 2021-02-23 10:40:56.000000 pglift-0.9.0/LICENSE
+-rw-r--r--   0 denis     (1000) denis     (1000)      522 2021-12-03 08:03:48.000000 pglift-0.9.0/MANIFEST.in
+-rw-r--r--   0 denis     (1000) denis     (1000)     2609 2021-12-10 13:35:12.716364 pglift-0.9.0/PKG-INFO
+-rw-r--r--   0 denis     (1000) denis     (1000)     1281 2021-08-06 12:29:55.000000 pglift-0.9.0/README.md
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.684364 pglift-0.9.0/docs/
+-rw-r--r--   0 denis     (1000) denis     (1000)      651 2021-06-04 14:32:42.000000 pglift-0.9.0/docs/Makefile
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.684364 pglift-0.9.0/docs/_static/
+-rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-03-16 14:48:49.000000 pglift-0.9.0/docs/_static/.gitignore
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.688364 pglift-0.9.0/docs/_templates/
+-rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-03-16 14:48:49.000000 pglift-0.9.0/docs/_templates/.gitignore
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.688364 pglift-0.9.0/docs/ansible/
+-rw-r--r--   0 denis     (1000) denis     (1000)     1475 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ansible/play1.yml
+-rw-r--r--   0 denis     (1000) denis     (1000)     1111 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ansible/play2.yml
+-rw-r--r--   0 denis     (1000) denis     (1000)      400 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ansible/play3.yml
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.688364 pglift-0.9.0/docs/api/
+-rw-r--r--   0 denis     (1000) denis     (1000)      191 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/api/cmd.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)      174 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/api/conf.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)      146 2021-09-09 11:54:02.000000 pglift-0.9.0/docs/api/ctx.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)      947 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/api/datamodel.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)      931 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/api/exceptions.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)      319 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/api/index.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     5757 2021-10-20 13:19:11.000000 pglift-0.9.0/docs/conf.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1855 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/dev.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)      303 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/index.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     1630 2021-12-03 15:46:58.000000 pglift-0.9.0/docs/install.rst
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.688364 pglift-0.9.0/docs/ops/
+-rw-r--r--   0 denis     (1000) denis     (1000)     3148 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ops/backup.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     1551 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ops/databases.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)      253 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ops/index.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     2230 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ops/instance.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     1790 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ops/monitoring.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     2170 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ops/privileges.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     1514 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/ops/roles.rst
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.692364 pglift-0.9.0/docs/setup/
+-rw-r--r--   0 denis     (1000) denis     (1000)      273 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/setup/index.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     1203 2021-12-10 07:47:05.000000 pglift-0.9.0/docs/setup/postgresql_authentication.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     1578 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/setup/postgresql_configuration.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     2425 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/setup/settings.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     3149 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/setup/systemd.rst
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.692364 pglift-0.9.0/docs/tutorials/
+-rw-r--r--   0 denis     (1000) denis     (1000)     7553 2021-12-09 09:26:03.000000 pglift-0.9.0/docs/tutorials/ansible.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)     4467 2021-12-10 08:42:36.000000 pglift-0.9.0/docs/tutorials/cli.rst
+-rw-r--r--   0 denis     (1000) denis     (1000)       96 2021-09-09 11:54:02.000000 pglift-0.9.0/docs/tutorials/index.rst
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.692364 pglift-0.9.0/extras/
+-rw-r--r--   0 denis     (1000) denis     (1000)      669 2021-08-05 12:45:15.000000 pglift-0.9.0/extras/.pglift-complete.bash
+-rw-r--r--   0 denis     (1000) denis     (1000)      669 2021-08-05 12:45:15.000000 pglift-0.9.0/extras/.pglift-complete.fish
+-rw-r--r--   0 denis     (1000) denis     (1000)      966 2021-08-05 12:45:15.000000 pglift-0.9.0/extras/.pglift-complete.zsh
+-rw-r--r--   0 denis     (1000) denis     (1000)      282 2021-08-05 12:45:15.000000 pglift-0.9.0/extras/README.md
+-rw-r--r--   0 denis     (1000) denis     (1000)      336 2021-07-16 11:34:26.000000 pglift-0.9.0/pyproject.toml
+-rw-r--r--   0 denis     (1000) denis     (1000)     1214 2021-12-10 13:35:12.716364 pglift-0.9.0/setup.cfg
+-rw-r--r--   0 denis     (1000) denis     (1000)     2770 2021-12-09 09:26:03.000000 pglift-0.9.0/setup.py
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.680364 pglift-0.9.0/src/
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.700364 pglift-0.9.0/src/pglift/
+-rw-r--r--   0 denis     (1000) denis     (1000)      392 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/__init__.py
+-rw-r--r--   0 denis     (1000) denis     (1000)       59 2021-09-09 11:54:05.000000 pglift-0.9.0/src/pglift/__main__.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      599 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/_compat.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     5422 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/_install.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1708 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/ansible.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2579 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/backup.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    35584 2021-12-10 13:32:27.000000 pglift-0.9.0/src/pglift/cli.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    10470 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/cmd.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2780 2021-12-10 09:36:16.000000 pglift-0.9.0/src/pglift/conf.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     4093 2021-12-10 07:47:05.000000 pglift-0.9.0/src/pglift/ctx.py
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.684364 pglift-0.9.0/src/pglift/data/
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.704364 pglift-0.9.0/src/pglift/data/postgresql/
+-rw-r--r--   0 denis     (1000) denis     (1000)      535 2021-06-04 14:32:42.000000 pglift-0.9.0/src/pglift/data/postgresql/pg_hba.conf
+-rw-r--r--   0 denis     (1000) denis     (1000)       52 2021-06-10 13:40:45.000000 pglift-0.9.0/src/pglift/data/postgresql/pg_ident.conf
+-rw-r--r--   0 denis     (1000) denis     (1000)      102 2021-07-16 11:34:26.000000 pglift-0.9.0/src/pglift/data/postgresql/site.conf
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.704364 pglift-0.9.0/src/pglift/data/systemd/
+-rw-r--r--   0 denis     (1000) denis     (1000)      183 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/data/systemd/pglift-backup@.service
+-rw-r--r--   0 denis     (1000) denis     (1000)      212 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/data/systemd/pglift-backup@.timer
+-rw-r--r--   0 denis     (1000) denis     (1000)      467 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/data/systemd/pglift-postgres_exporter@.service
+-rw-r--r--   0 denis     (1000) denis     (1000)      427 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/data/systemd/pglift-postgresql@.service
+-rw-r--r--   0 denis     (1000) denis     (1000)     6747 2021-12-10 07:47:05.000000 pglift-0.9.0/src/pglift/databases.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2920 2021-12-10 07:47:05.000000 pglift-0.9.0/src/pglift/db.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2163 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/exceptions.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      983 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/hookspecs.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    24650 2021-12-10 09:36:16.000000 pglift-0.9.0/src/pglift/instance.py
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.704364 pglift-0.9.0/src/pglift/models/
+-rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-09-09 11:54:05.000000 pglift-0.9.0/src/pglift/models/__init__.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    10049 2021-12-10 09:36:16.000000 pglift-0.9.0/src/pglift/models/helpers.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    10872 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/models/interface.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     7348 2021-12-10 08:11:32.000000 pglift-0.9.0/src/pglift/models/system.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    12425 2021-12-10 07:47:05.000000 pglift-0.9.0/src/pglift/pgbackrest.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      904 2021-09-23 12:38:16.000000 pglift-0.9.0/src/pglift/pm.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1353 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/postgres.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2271 2021-12-10 07:47:05.000000 pglift-0.9.0/src/pglift/privileges.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    10134 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/prometheus.py
+-rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-06-04 14:32:42.000000 pglift-0.9.0/src/pglift/py.typed
+-rw-r--r--   0 denis     (1000) denis     (1000)     3574 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/queries.sql
+-rw-r--r--   0 denis     (1000) denis     (1000)    10458 2021-12-10 07:47:05.000000 pglift-0.9.0/src/pglift/roles.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    11962 2021-12-10 07:47:05.000000 pglift-0.9.0/src/pglift/settings.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     3771 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/systemd.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     4439 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/task.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1675 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/types.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     3958 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/util.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      148 2021-12-09 09:26:03.000000 pglift-0.9.0/src/pglift/validators.py
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.700364 pglift-0.9.0/src/pglift.egg-info/
+-rw-r--r--   0 denis     (1000) denis     (1000)     2609 2021-12-10 13:35:12.000000 pglift-0.9.0/src/pglift.egg-info/PKG-INFO
+-rw-r--r--   0 denis     (1000) denis     (1000)     3328 2021-12-10 13:35:12.000000 pglift-0.9.0/src/pglift.egg-info/SOURCES.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)        1 2021-12-10 13:35:12.000000 pglift-0.9.0/src/pglift.egg-info/dependency_links.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)       61 2021-12-10 13:35:12.000000 pglift-0.9.0/src/pglift.egg-info/entry_points.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)      463 2021-12-10 13:35:12.000000 pglift-0.9.0/src/pglift.egg-info/requires.txt
+-rw-r--r--   0 denis     (1000) denis     (1000)        7 2021-12-10 13:35:12.000000 pglift-0.9.0/src/pglift.egg-info/top_level.txt
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.704364 pglift-0.9.0/tests/
+-rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-09-09 11:54:05.000000 pglift-0.9.0/tests/__init__.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      129 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/conftest.py
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.708364 pglift-0.9.0/tests/data/
+-rw-r--r--   0 denis     (1000) denis     (1000)      286 2021-09-20 12:41:43.000000 pglift-0.9.0/tests/data/ansible-argspec-database.json
+-rw-r--r--   0 denis     (1000) denis     (1000)     1184 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/data/ansible-argspec-instance.json
+-rw-r--r--   0 denis     (1000) denis     (1000)      684 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/data/ansible-argspec-postgresexporter.json
+-rw-r--r--   0 denis     (1000) denis     (1000)     1095 2021-09-20 12:41:43.000000 pglift-0.9.0/tests/data/ansible-argspec-role.json
+-rw-r--r--   0 denis     (1000) denis     (1000)     3648 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/data/queries.json
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.712365 pglift-0.9.0/tests/func/
+-rw-r--r--   0 denis     (1000) denis     (1000)      350 2021-06-04 14:32:42.000000 pglift-0.9.0/tests/func/README.md
+-rw-r--r--   0 denis     (1000) denis     (1000)     2339 2021-12-10 07:47:05.000000 pglift-0.9.0/tests/func/__init__.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     8880 2021-12-10 07:47:05.000000 pglift-0.9.0/tests/func/conftest.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    14074 2021-12-10 07:47:05.000000 pglift-0.9.0/tests/func/test_10_instance.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     6548 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/func/test_11_databases.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2120 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/func/test_11_privileges.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     8622 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/func/test_11_roles.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      764 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/func/test_20_backup.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     4106 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/func/test_20_pgbackrest.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     7463 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/func/test_20_prometheus.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2754 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/func/test_99_drop.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     5790 2021-12-09 09:26:03.000000 pglift-0.9.0/tests/func/test_ansible.py
+drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2021-12-10 13:35:12.716364 pglift-0.9.0/tests/unit/
+-rw-r--r--   0 denis     (1000) denis     (1000)        0 2021-09-09 11:54:05.000000 pglift-0.9.0/tests/unit/__init__.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     3062 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/conftest.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2537 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test__install.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      225 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_backup.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    38053 2021-12-10 13:32:27.000000 pglift-0.9.0/tests/unit/test_cli.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2656 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_cmd.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1671 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_conf.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1129 2021-12-10 07:47:05.000000 pglift-0.9.0/tests/unit/test_ctx.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2118 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_db.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      493 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_exceptions.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     7937 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_instance.py
+-rw-r--r--   0 denis     (1000) denis     (1000)    10214 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_models_helpers.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      730 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_models_interface.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     4060 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_models_system.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2589 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_pgbackrest.py
+-rw-r--r--   0 denis     (1000) denis     (1000)      462 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_pm.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1321 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_postgres.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1281 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_prometheus.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     2934 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_roles.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     4093 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_settings.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1190 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_systemd.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     3224 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_task.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1200 2021-12-10 09:36:16.000000 pglift-0.9.0/tests/unit/test_util.py
+-rw-r--r--   0 denis     (1000) denis     (1000)     1039 2021-12-09 09:26:03.000000 pglift-0.9.0/tox.ini
```

### Comparing `pglift-0.8.0/LICENSE` & `pglift-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/MANIFEST.in` & `pglift-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/PKG-INFO` & `pglift-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglift
-Version: 0.8.0
+Version: 0.9.0
 Summary: Life-cycle management of production-ready PostgreSQL instances
 Home-page: https://gitlab.com/dalibo/pglift
 Author: Dalibo SCOP
 Author-email: contact@dalibo.com
 License: UNKNOWN
 Project-URL: Documentation, https://pglift.readthedocs.io/
 Project-URL: Source, https://gitlab.com/dalibo/pglift/
```

### Comparing `pglift-0.8.0/README.md` & `pglift-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/Makefile` & `pglift-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/ansible/play1.yml` & `pglift-0.9.0/docs/ansible/play1.yml`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/ansible/play2.yml` & `pglift-0.9.0/docs/ansible/play2.yml`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/api/datamodel.rst` & `pglift-0.9.0/docs/api/datamodel.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/api/exceptions.rst` & `pglift-0.9.0/docs/api/exceptions.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/conf.py` & `pglift-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/dev.rst` & `pglift-0.9.0/docs/dev.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/install.rst` & `pglift-0.9.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/ops/backup.rst` & `pglift-0.9.0/docs/ops/backup.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/ops/databases.rst` & `pglift-0.9.0/docs/ops/databases.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/ops/instance.rst` & `pglift-0.9.0/docs/ops/instance.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/ops/monitoring.rst` & `pglift-0.9.0/docs/ops/monitoring.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/ops/privileges.rst` & `pglift-0.9.0/docs/ops/privileges.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/ops/roles.rst` & `pglift-0.9.0/docs/ops/roles.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/setup/postgresql_authentication.rst` & `pglift-0.9.0/docs/setup/postgresql_authentication.rst`

 * *Files 16% similar despite different names*

```diff
@@ -21,8 +21,12 @@
 
 When the password file is used, nothing special is required for authentication
 as all libpq operations would use it.
 
 Otherwise, the password is read from ``PGPASSWORD`` environment variable so
 this should be set in the environment running interactive commands.
 
+Alternatively, you can configure a ``postgresql.auth.password_command`` option
+in site settings, it can be any user-managed executable command and `pglift`
+and must return the super-user role password as stdout.
+
 .. _`password file`: https://www.postgresql.org/docs/current/libpq-pgpass.html
```

### Comparing `pglift-0.8.0/docs/setup/postgresql_configuration.rst` & `pglift-0.9.0/docs/setup/postgresql_configuration.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/setup/settings.rst` & `pglift-0.9.0/docs/setup/settings.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/setup/systemd.rst` & `pglift-0.9.0/docs/setup/systemd.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/tutorials/ansible.rst` & `pglift-0.9.0/docs/tutorials/ansible.rst`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/docs/tutorials/cli.rst` & `pglift-0.9.0/docs/tutorials/cli.rst`

 * *Files 2% similar despite different names*

```diff
@@ -123,7 +123,13 @@
     name       owner     encoding    collation    ctype    acls                                         size  description                                 tablespace    tablespace      tablespace
                                                                                                                                                           name          location              size
     ---------  --------  ----------  -----------  -------  ----------------------------------------  -------  ------------------------------------------  ------------  ------------  ------------
     myapp      postgres  UTF8        C            C                                                  8167939                                              pg_default                      41011771
     postgres   postgres  UTF8        C            C                                                  8319535  default administrative connection database  pg_default                      41011771
     template1  postgres  UTF8        C            C        ['=c/postgres', 'postgres=CTc/postgres']  8167939  default template for new databases          pg_default                      41011771
     $ pglift database drop 13/main myapp
+
+Dumping a database of an instance:
+
+::
+
+    $ pglift database backup 13/main myapp my/path/mydump.dump
```

### Comparing `pglift-0.8.0/extras/.pglift-complete.bash` & `pglift-0.9.0/extras/.pglift-complete.bash`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/extras/.pglift-complete.fish` & `pglift-0.9.0/extras/.pglift-complete.fish`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/extras/.pglift-complete.zsh` & `pglift-0.9.0/extras/.pglift-complete.zsh`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/setup.cfg` & `pglift-0.9.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 show_error_codes = true
 strict = true
 warn_unused_ignores = true
 
 [mypy-pglift._compat]
 warn_unused_ignores = false
 
-[mypy-tests.unit.*]
-disallow_untyped_defs = false
-
 [mypy-ansible.module_utils.*]
 ignore_missing_imports = true
 
 [mypy-contextlib2]
 ignore_missing_imports = true
 
 [mypy-importlib_metadata]
```

### Comparing `pglift-0.8.0/setup.py` & `pglift-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/_compat.py` & `pglift-0.9.0/src/pglift/_compat.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/_install.py` & `pglift-0.9.0/src/pglift/_install.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/ansible.py` & `pglift-0.9.0/src/pglift/ansible.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/backup.py` & `pglift-0.9.0/src/pglift/backup.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/cli.py` & `pglift-0.9.0/src/pglift/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,19 @@
         keep_logfile = False
         try:
             try:
                 return super().invoke(context)
             except exceptions.Error as e:
                 logger.debug("an internal error occurred", exc_info=True)
                 msg = str(e)
-                if isinstance(e, exceptions.CommandError) and e.stderr:
-                    msg += f"\n{e.stderr}"
+                if isinstance(e, exceptions.CommandError):
+                    if e.stderr:
+                        msg += f"\n{e.stderr}"
+                    if e.stdout:
+                        msg += f"\n{e.stdout}"
                 raise click.ClickException(msg)
             except (click.ClickException, click.Abort, click.exceptions.Exit):
                 raise
             except pydantic.ValidationError as e:
                 logger.debug("a validation error occurred", exc_info=True)
                 raise click.ClickException(str(e))
             except Exception:
@@ -148,14 +151,36 @@
 require_pgbackrest = partial(require_component, pgbackrest, "pgbackrest")
 require_prometheus = partial(
     require_component, prometheus, "Prometheus postgres_exporter"
 )
 
 
 def get_instance(ctx: Context, name: str, version: Optional[str]) -> Instance:
+    """Return an Instance from name/version, possibly guessing version if unspecified."""
+    if version is None:
+        found = None
+        for version in POSTGRESQL_SUPPORTED_VERSIONS:
+            try:
+                instance = Instance.system_lookup(ctx, (name, version))
+            except exceptions.InstanceNotFound:
+                ctx.debug("instance '%s' not found in version %s", name, version)
+            else:
+                ctx.info("instance '%s' found in version %s", name, version)
+                if found:
+                    raise click.BadParameter(
+                        f"instance '{name}' exists in several PostgreSQL version;"
+                        " please select version explicitly"
+                    )
+                found = instance
+
+        if found:
+            return found
+
+        raise click.BadParameter(f"instance '{name}' not found")
+
     try:
         return Instance.system_lookup(ctx, (name, version))
     except Exception as e:
         raise click.BadParameter(str(e))
 
 
 def nameversion_from_id(instance_id: str) -> Tuple[str, Optional[str]]:
@@ -449,27 +474,29 @@
     """Apply manifest as a PostgreSQL instance"""
     instance = interface.Instance.parse_yaml(file)
     with runner:
         instance_mod.apply(ctx, instance)
 
 
 @instance.command("alter")
-@helpers.parameters_from_model(interface.Instance, parse_model=False)
+@instance_identifier
+@helpers.parameters_from_model(
+    interface.Instance, exclude=["name", "version"], parse_model=False
+)
 @pass_runner
 @pass_ctx
 def instance_alter(
     ctx: Context,
     runner: Runner,
-    name: str,
-    version: Optional[str] = None,
+    instance: Instance,
     **changes: Any,
 ) -> None:
     """Alter a PostgreSQL instance"""
     changes = helpers.unnest(interface.Instance, changes)
-    values = instance_mod.describe(ctx, name, version).dict()
+    values = instance_mod.describe(ctx, instance.name, instance.version).dict()
     values = deep_update(values, changes)
     altered = interface.Instance.parse_obj(values)
     with runner:
         instance_mod.apply(ctx, altered)
 
 
 @instance.command("schema")
@@ -1002,14 +1029,32 @@
 @pass_ctx
 def database_drop(ctx: Context, runner: Runner, instance: Instance, name: str) -> None:
     """Drop a database"""
     with instance_mod.running(ctx, instance), runner:
         databases.drop(ctx, instance, name)
 
 
+@database.command("backup")
+@instance_identifier
+@click.argument("name")
+@click.argument("output_file", type=click.Path(path_type=pathlib.Path))
+@pass_runner
+@pass_ctx
+def database_backup(
+    ctx: Context,
+    runner: Runner,
+    instance: Instance,
+    name: str,
+    output_file: pathlib.Path,
+) -> None:
+    """Dump a database in a PostgreSQL instance"""
+    with runner, instance_mod.running(ctx, instance):
+        databases.backup(ctx, instance, name, output_file)
+
+
 @database.command("privileges")
 @instance_identifier
 @click.argument("name")
 @click.option("-r", "--role", "roles", multiple=True, help="Role to inspect")
 @as_json_option
 @pass_ctx
 def database_privileges(
```

### Comparing `pglift-0.8.0/src/pglift/cmd.py` & `pglift-0.9.0/src/pglift/cmd.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/conf.py` & `pglift-0.9.0/src/pglift/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import shutil
 from functools import wraps
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Tuple, cast
+from typing import TYPE_CHECKING, Callable, Optional, Tuple, cast
 
 from pgtoolkit import conf as pgconf
 
 from . import __name__ as pkgname
 from . import exceptions
 
 if TYPE_CHECKING:
     from .models.system import BaseInstance
 
 
-def make(instance: str, **confitems: Any) -> pgconf.Configuration:
+def make(instance: str, **confitems: Optional[pgconf.Value]) -> pgconf.Configuration:
     """Return a :class:`pgtoolkit.conf.Configuration` for named `instance`
     filled with given items.
     """
     conf = pgconf.Configuration()
     for key, value in confitems.items():
         if value is not None:
             conf[key] = value
```

### Comparing `pglift-0.8.0/src/pglift/ctx.py` & `pglift-0.9.0/src/pglift/ctx.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import functools
 import logging
+import os
 from abc import ABC, abstractmethod
-from typing import Any, Optional, Sequence
+from typing import Any, Dict, Optional, Sequence
 
 from pgtoolkit import ctl
 from pluggy import PluginManager
 
 from . import __name__ as pkgname
 from . import cmd, exceptions, util
 from ._compat import shlex_join
@@ -42,14 +43,28 @@
             if installed_version != version:
                 raise exceptions.SystemError(
                     f"PostgreSQL version from {pg_bindir} mismatches with declared value: "
                     f"{installed_version} != {version}"
                 )
         return pg_ctl
 
+    def libpq_environ(self, *, base: Optional[Dict[str, str]] = None) -> Dict[str, str]:
+        """Return a dict with libpq environment variables for authentication."""
+        auth = self.settings.postgresql.auth
+        if base is None:
+            env = os.environ.copy()
+        else:
+            env = base.copy()
+        env.setdefault("PGPASSFILE", str(auth.passfile))
+        if auth.password_command and "PGPASSWORD" not in env:
+            password = self.run([auth.password_command], check=True).stdout.strip()
+            if password:
+                env["PGPASSWORD"] = password
+        return env
+
     @abstractmethod
     def debug(self, msg: str, *args: Any, **kwargs: Any) -> None:
         ...
 
     @abstractmethod
     def info(self, msg: str, *args: Any, **kwargs: Any) -> None:
         ...
```

### Comparing `pglift-0.8.0/src/pglift/data/postgresql/pg_hba.conf` & `pglift-0.9.0/src/pglift/data/postgresql/pg_hba.conf`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/databases.py` & `pglift-0.9.0/src/pglift/databases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pathlib
 from typing import Any, Dict, List, Sequence, Tuple
 
 import psycopg2
 import psycopg2.extensions
 from psycopg2 import sql
 
 from . import db, exceptions, types
@@ -32,25 +33,25 @@
 def describe(ctx: BaseContext, instance: Instance, name: str) -> interface.Database:
     """Return a database described as a manifest.
 
     :raises ~pglift.exceptions.DatabaseNotFound: if no role with specified 'name' exists.
     """
     if not exists(ctx, instance, name):
         raise exceptions.DatabaseNotFound(name)
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         with cnx.cursor() as cur:
             cur.execute(db.query("database_inspect"), {"datname": name})
             values = dict(cur.fetchone())
     return interface.Database(name=name, **values)
 
 
 def list(ctx: BaseContext, instance: Instance) -> List[interface.DetailedDatabase]:
     """List all databases in instance."""
 
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         psycopg2.extensions.register_type(
             # select typarray from pg_type where typname = 'aclitem'; -> 1034
             psycopg2.extensions.new_array_type((1034,), "ACLITEM[]", psycopg2.STRING)
         )
         with cnx.cursor() as cur:
             cur.execute(db.query("database_list"))
             values = cur.fetchall()
@@ -61,25 +62,25 @@
 def drop(ctx: BaseContext, instance: Instance, name: str) -> None:
     """Drop a database from instance.
 
     :raises ~pglift.exceptions.DatabaseNotFound: if no role with specified 'name' exists.
     """
     if not exists(ctx, instance, name):
         raise exceptions.DatabaseNotFound(name)
-    with db.superuser_connect(instance, autocommit=True) as cnx:
+    with db.superuser_connect(ctx, instance, autocommit=True) as cnx:
         with cnx.cursor() as cur:
             cur.execute(db.query("database_drop", database=sql.Identifier(name)))
 
 
 def exists(ctx: BaseContext, instance: Instance, name: str) -> bool:
     """Return True if named database exists in 'instance'.
 
     The instance should be running.
     """
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         with cnx.cursor() as cur:
             cur.execute(db.query("database_exists"), {"database": name})
             return cur.rowcount == 1  # type: ignore[no-any-return]
 
 
 def options_and_args(
     database: interface.Database,
@@ -99,15 +100,15 @@
 @task("create '{database.name}' database on instance {instance}")
 def create(ctx: BaseContext, instance: Instance, database: interface.Database) -> None:
     """Create 'database' in 'instance'.
 
     The instance should be running and the database should not exist already.
     """
     options, args = options_and_args(database)
-    with db.superuser_connect(instance, autocommit=True) as cnx:
+    with db.superuser_connect(ctx, instance, autocommit=True) as cnx:
         with cnx.cursor() as cur:
             cur.execute(
                 db.query(
                     "database_create",
                     database=sql.Identifier(database.name),
                     options=options,
                 ),
@@ -125,26 +126,62 @@
         raise exceptions.DatabaseNotFound(database.name)
 
     if database.owner is None:
         owner = sql.SQL("CURRENT_USER")
     else:
         owner = sql.Identifier(database.owner)
     options = sql.SQL(" ").join([sql.SQL("OWNER TO"), owner])
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         with cnx.cursor() as cur:
             cur.execute(
                 db.query(
                     "database_alter_owner",
                     database=sql.Identifier(database.name),
                     options=options,
                 ),
             )
         cnx.commit()
 
 
+@task("backup '{name}' database on instance {instance}")
+def backup(
+    ctx: BaseContext, instance: Instance, name: str, output_file: pathlib.Path
+) -> None:
+    """Dump a database.
+
+    The instance should be running and the database should exist already.
+    """
+    if not exists(ctx, instance, name):
+        raise exceptions.DatabaseNotFound(name)
+
+    bindir = ctx.pg_ctl(instance.version).bindir
+    config = instance.config()
+    try:
+        host = config.unix_socket_directories.split(",")[0]  # type: ignore[union-attr]
+    except (AttributeError, IndexError):
+        host = "localhost"
+    user = ctx.settings.postgresql.surole.name
+    cmd = [
+        str(bindir / "pg_dump"),
+        "--port",
+        str(instance.port),
+        "--host",
+        host,
+        "--user",
+        user,
+        "-Fc",
+        "-f",
+        str(output_file),
+        name,
+    ]
+
+    env = ctx.libpq_environ()
+    ctx.run(cmd, check=True, env=env)
+
+
 def run(
     ctx: BaseContext,
     instance: Instance,
     sql_command: str,
     *,
     dbnames: Sequence[str] = (),
     exclude_dbnames: Sequence[str] = (),
@@ -152,13 +189,13 @@
 ) -> None:
     for database in list(ctx, instance):
         if (
             dbnames and database.name not in dbnames
         ) or database.name in exclude_dbnames:
             continue
         with db.superuser_connect(
-            instance, dbname=database.name, autocommit=True
+            ctx, instance, dbname=database.name, autocommit=True
         ) as cnx:
             cnx.notices = notice_handler
             with cnx.cursor() as cur:
                 ctx.info("run %s on database %s of %s", sql_command, database, instance)
                 cur.execute(sql_command)
```

### Comparing `pglift-0.8.0/src/pglift/db.py` & `pglift-0.9.0/src/pglift/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import psycopg2
 import psycopg2.extensions
 import psycopg2.extras
 from psycopg2 import sql
 
 if TYPE_CHECKING:  # pragma: nocover
+    from .ctx import BaseContext
     from .models.system import PostgreSQLInstance
 
 QUERIES = pathlib.Path(__file__).parent / "queries.sql"
 
 
 def query(name: str, **kwargs: sql.Composable) -> sql.Composed:
     for qname, qstr in queries():
@@ -75,19 +76,21 @@
 ) -> ContextManager[psycopg2.extensions.connection]:
     """Connect to specified database of `instance` with `role`."""
     conninfo = dsn(instance, dbname=dbname, **kwargs)
     return connect_dsn(conninfo, autocommit=autocommit)
 
 
 def superuser_connect(
-    instance: "PostgreSQLInstance", **kwargs: Any
+    ctx: "BaseContext", instance: "PostgreSQLInstance", **kwargs: Any
 ) -> ContextManager[psycopg2.extensions.connection]:
     if "user" in kwargs:
         raise TypeError("unexpected 'user' argument")
     kwargs["user"] = instance.settings.postgresql.surole.name
+    if "password" not in kwargs:
+        kwargs["password"] = ctx.libpq_environ().get("PGPASSWORD")
     return connect(instance, **kwargs)
 
 
 class NoticeHandlerStderr:
     @staticmethod
     def append(notice: str) -> None:
         sys.stderr.write(notice)
```

### Comparing `pglift-0.8.0/src/pglift/exceptions.py` & `pglift-0.9.0/src/pglift/exceptions.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/hookspecs.py` & `pglift-0.9.0/src/pglift/hookspecs.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/instance.py` & `pglift-0.9.0/src/pglift/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import builtins
 import contextlib
-import os
 import shutil
 import tempfile
 import time
 from pathlib import Path
 from typing import Any, Dict, Iterator, Optional, Tuple, Union
 
 from pgtoolkit import conf as pgconf
+from pgtoolkit import pgpass
 from pgtoolkit.ctl import Status as Status
+from pydantic import SecretStr
 from typing_extensions import Literal
 
 from . import (
     cmd,
     conf,
     datapath,
     db,
@@ -38,22 +39,14 @@
 def systemd_unit(instance: BaseInstance) -> str:
     return f"pglift-postgresql@{instance.version}-{instance.name}.service"
 
 
 def init_replication(
     ctx: BaseContext, instance: BaseInstance, standby_for: str, slot: Optional[str]
 ) -> None:
-
-    # use existing PGPASSFILE env or use passfile from settings
-    passfile = (
-        None
-        if "PGPASSFILE" in os.environ
-        else str(instance.settings.postgresql.auth.passfile)
-    )
-
     with tempfile.TemporaryDirectory() as _tmpdir:
         tmpdir = Path(_tmpdir)
         # pg_basebackup will also copy config files from primary datadir.
         # So to have expected configuration at this stage we have to backup
         # postgresql.conf & pg_hba.conf (created by prior pg_ctl init) and
         # restore after pg_basebackup finishes.
         keep = {"postgresql.conf", "pg_hba.conf"}
@@ -73,29 +66,31 @@
             "--verbose",
             "--dbname",
             standby_for,
             "--waldir",
             str(instance.waldir),
         ]
 
+        env = ctx.libpq_environ()
         if slot:
             cmd += ["--slot", slot]
-            with db.connect_dsn(standby_for, passfile=passfile) as cnx:
+            with db.connect_dsn(
+                standby_for,
+                passfile=env.get("PGPASSFILE"),
+                password=env.get("PGPASSWORD"),
+            ) as cnx:
                 # ensure the replication slot does not exists
                 # otherwise --create-slot will raise an error
                 with cnx.cursor() as cur:
                     cur.execute(db.query("drop_replication_slot"), {"slot": slot})
                     if int(instance.version) <= 10:
                         cur.execute(db.query("create_replication_slot"), {"slot": slot})
                     else:
                         cmd += ["--create-slot"]
 
-        env = os.environ.copy()
-        if passfile:
-            env["PGPASSFILE"] = passfile
         ctx.run(cmd, env=env, check=True)
         for name in keep:
             shutil.copyfile(tmpdir / name, instance.datadir / name)
         # When primary is also managed by pglift, pg_basebackup will also copy
         # conf.pglift.d. So we must drop it to not interfer with site/user
         # config generated by instance_configure
         shutil.rmtree(instance.datadir / "conf.pglift.d", ignore_errors=True)
@@ -167,15 +162,15 @@
 
 
 def configure(
     ctx: BaseContext,
     manifest: interface.Instance,
     *,
     ssl: Union[bool, Tuple[Path, Path]] = False,
-    **confitems: Any,
+    **confitems: Optional[pgconf.Value],
 ) -> ConfigChanges:
     """Write instance's configuration and include it in its postgresql.conf.
 
     `ssl` parameter controls SSL configuration. If False, SSL is not enabled.
     If True, a self-signed certificate is generated. A tuple of two
     `~pathlib.Path` corresponding to the location of SSL cert file and key
     file to use may also be passed.
@@ -198,23 +193,23 @@
     if not pgconfig.get("ssl", False) and ssl is True:
         util.generate_certificate(configdir, run_command=ctx.run)
     elif isinstance(ssl, tuple):
         try:
             certfile, keyfile = ssl
         except ValueError:
             raise ValueError("expecting a 2-tuple for 'ssl' parameter") from None
-        confitems["ssl_cert_file"] = certfile
-        confitems["ssl_key_file"] = keyfile
+        confitems["ssl_cert_file"] = str(certfile)
+        confitems["ssl_key_file"] = str(keyfile)
     original_content = postgresql_conf.read_text()
     if not any(line.startswith(include) for line in original_content.splitlines()):
         with postgresql_conf.open("w") as f:
             f.write(f"{include}\n\n")
             f.write(original_content)
 
-    site_confitems: Dict[str, pgconf.Value] = {"cluster_name": instance.name}
+    site_confitems: Dict[str, Optional[pgconf.Value]] = {"cluster_name": instance.name}
     site_config_template = datapath / "postgresql" / "site.conf"
     if site_config_template.exists():
         site_confitems.update(pgconf.parse(site_config_template).as_dict())
 
     def format_values(
         confitems: Dict[str, Any], memtotal: float = util.total_memory()
     ) -> None:
@@ -232,15 +227,17 @@
         for k, v in confitems.items():
             if isinstance(v, str):
                 confitems[k] = v.format(settings=ctx.settings.postgresql)
 
     format_values(confitems)
     format_values(site_confitems)
 
-    def make_config(fpath: Path, items: Dict[str, Any]) -> ConfigChanges:
+    def make_config(
+        fpath: Path, items: Dict[str, Optional[pgconf.Value]]
+    ) -> ConfigChanges:
         config = conf.make(instance.name, **items)
 
         config_before = {}
         if fpath.exists():
             config_before = {e.name: e.value for e in pgconf.parse(fpath)}
         config_after = {e.name: e.value for e in config}
         changes: ConfigChanges = {}
@@ -533,20 +530,28 @@
     name: Optional[str] = None,
     port: Optional[int] = None,
     jobs: Optional[int] = None,
 ) -> Instance:
     """Upgrade an instance using pg_upgrade"""
     if version is None:
         version = default_postgresql_version(ctx)
+    surole = ctx.settings.postgresql.surole
+    surole_password = ctx.libpq_environ().get("PGPASSWORD")
+    if not surole_password and ctx.settings.postgresql.auth.passfile:
+        with pgpass.edit(ctx.settings.postgresql.auth.passfile) as passfile:
+            for entry in passfile:
+                if entry.matches(port=instance.port, username=surole.name):
+                    surole_password = entry.password
     new_manifest = interface.Instance(
         name=name or instance.name,
         version=version,
         port=port or instance.port,
         state=interface.InstanceState.stopped,
         prometheus={"port": instance.prometheus.port},
+        surole_password=SecretStr(surole_password) if surole_password else None,
     )
     result = apply(ctx, new_manifest)
     assert result is not None, new_manifest
     (newinstance, _) = result
     bindir = ctx.pg_ctl(version).bindir
     pg_upgrade = str(bindir / "pg_upgrade")
     cmd = [
@@ -555,27 +560,23 @@
         f"--new-bindir={bindir}",
         f"--old-datadir={instance.datadir}",
         f"--new-datadir={newinstance.datadir}",
         f"--username={ctx.settings.postgresql.surole.name}",
     ]
     if jobs is not None:
         cmd.extend(["--jobs", str(jobs)])
-    surole = ctx.settings.postgresql.surole
-    env = ctx.settings.postgresql.auth.libpq_environ()
-    hba_path = newinstance.datadir / "pg_hba.conf"
-    hba_content = hba_path.read_bytes()
+    env = ctx.libpq_environ()
+    if surole_password:
+        env.setdefault("PGPASSWORD", surole_password)
     try:
-        hba_path.write_text(f"local all {surole.name} trust\n")
         with tempfile.TemporaryDirectory() as tmpdir:
             ctx.run(cmd, check=True, cwd=tmpdir, env=env)
     except exceptions.CommandError:
         drop(ctx, newinstance)
         raise
-    else:
-        hba_path.write_bytes(hba_content)
     return newinstance
 
 
 def apply(
     ctx: BaseContext, manifest: interface.Instance
 ) -> Optional[Tuple[Instance, ConfigChanges]]:
     """Apply state described by specified manifest as a PostgreSQL instance.
@@ -727,15 +728,16 @@
         "--host",
         host,
         "--user",
         user,
     ]
     if dbname is not None:
         args.extend(["--dbname", dbname])
-    cmd.execute_program(args, logger=ctx)
+    env = ctx.libpq_environ()
+    cmd.execute_program(args, logger=ctx, env=env)
 
 
 def exists(ctx: BaseContext, name: str, version: Optional[str]) -> bool:
     """Return true when instance exists"""
     try:
         PostgreSQLInstance.system_lookup(ctx, (name, version))
     except exceptions.InstanceNotFound:
```

### Comparing `pglift-0.8.0/src/pglift/models/helpers.py` & `pglift-0.9.0/src/pglift/models/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import (
     Any,
     Callable,
     Dict,
     Iterator,
     List,
     Mapping,
+    Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import pydantic
@@ -55,15 +56,15 @@
     return model_type.parse_obj(obj)
 
 
 DEFAULT = object()
 
 
 def _decorators_from_model(
-    model_type: ModelType, *, _prefix: str = ""
+    model_type: ModelType, *, exclude: Sequence[str] = (), _prefix: str = ""
 ) -> Iterator[Tuple[Tuple[str, str], Callable[[Callback], Callback]]]:
     """Yield click.{argument,option} decorators corresponding to fields of
     a pydantic model type along with respective callback argument name and
     model name.
     """
     import click
 
@@ -73,14 +74,16 @@
         return value
 
     for field in model_type.__fields__.values():
         cli_config = field.field_info.extra.get("cli", {})
         if cli_config.get("hide", False):
             continue
         argname = cli_config.get("name", field.alias)
+        if argname in exclude:
+            continue
         modelname = field.alias
         ftype = field.outer_type_
         if not _prefix and field.required:
             yield (modelname, argname.replace("-", "_")), click.argument(
                 argname, type=ftype
             )
         else:
@@ -128,26 +131,27 @@
                 if description[-1] not in ".?":
                     description += "."
                 attrs["help"] = description
             yield (modelname, argname), click.option(fname, callback=default, **attrs)
 
 
 def parameters_from_model(
-    model_type: ModelType, *, parse_model: bool = True
+    model_type: ModelType, *, exclude: Sequence[str] = (), parse_model: bool = True
 ) -> Callable[[Callback], Callback]:
     """Attach click parameters (arguments or options) built from a pydantic
     model to the command.
 
     >>> class Obj(pydantic.BaseModel):
     ...     message: str
+    ...     ignored: int = 0
 
     >>> import click
 
     >>> @click.command("echo")
-    ... @parameters_from_model(Obj)
+    ... @parameters_from_model(Obj, exclude=['ignored'])
     ... @click.option("--caps", is_flag=True, default=False)
     ... @click.pass_context
     ... def cmd(ctx, obj, caps):
     ...     output = obj.message
     ...     if caps:
     ...         output = output.upper()
     ...     click.echo(output)
@@ -165,15 +169,15 @@
     >>> print(r.stdout.strip())
     HELLO, WORLD
     """
 
     def decorator(f: Callback) -> Callback:
 
         modelnames_and_argnames, param_decorators = zip(
-            *reversed(list(_decorators_from_model(model_type)))
+            *reversed(list(_decorators_from_model(model_type, exclude=exclude)))
         )
 
         def params_to_modelargs(kwargs: Dict[str, Any]) -> Dict[str, Any]:
             args = {}
             for modelname, argname in modelnames_and_argnames:
                 value = kwargs.pop(argname)
                 if value is DEFAULT:
```

### Comparing `pglift-0.8.0/src/pglift/models/interface.py` & `pglift-0.9.0/src/pglift/models/interface.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/models/system.py` & `pglift-0.9.0/src/pglift/models/system.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/pgbackrest.py` & `pglift-0.9.0/src/pglift/pgbackrest.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,15 @@
 ) -> None:
     """Perform a backup of ``instance``.
 
     :param type: backup type (one of 'full', 'incr', 'diff').
 
     Ref.: https://pgbackrest.org/command.html#command-backup
     """
-    env = ctx.settings.postgresql.auth.libpq_environ()
+    env = ctx.libpq_environ()
     ctx.run(backup_command(instance, type=type), check=True, env=env)
 
 
 def expire_command(instance: BaseInstance) -> List[str]:
     """Return the full pgbackrest command to expire backups for ``instance``.
 
     Ref.: https://pgbackrest.org/command.html#command-expire
```

### Comparing `pglift-0.8.0/src/pglift/pm.py` & `pglift-0.9.0/src/pglift/pm.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/postgres.py` & `pglift-0.9.0/src/pglift/postgres.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/privileges.py` & `pglift-0.9.0/src/pglift/privileges.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     ctx: BaseContext, instance: Instance, database: str, roles: Sequence[str] = ()
 ) -> List[interface.Privilege]:
     args = {}
     where_clause = sql.SQL("")
     if roles:
         where_clause = sql.SQL("WHERE pg_roles.rolname IN %(roles)s")
         args["roles"] = tuple(roles)
-    with db.superuser_connect(instance, dbname=database) as cnx:
+    with db.superuser_connect(ctx, instance, dbname=database) as cnx:
         with cnx.cursor() as cur:
             cur.execute(
                 db.query("database_default_acl", where_clause=where_clause), args
             )
             results = cur.fetchall()
     return [interface.Privilege(**r) for r in results]
 
@@ -38,27 +38,27 @@
         unspecified).
     :param roles: list of roles to restrict inspection on.
 
     :raises ValueError: if an element of `databases` or `roles` does not
         exist.
     """
 
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         with cnx.cursor() as cur:
             cur.execute(db.query("database_list"))
             existing_databases = [db["name"] for db in cur.fetchall()]
     if not databases:
         databases = existing_databases
     else:
         unknown_dbs = set(databases) - set(existing_databases)
         if unknown_dbs:
             raise ValueError(f"database(s) not found: {', '.join(unknown_dbs)}")
 
     if roles:
-        with db.superuser_connect(instance) as cnx:
+        with db.superuser_connect(ctx, instance) as cnx:
             with cnx.cursor() as cur:
                 cur.execute(db.query("role_list_names"))
                 existing_roles = [n for n, in cur.fetchall()]
         unknown_roles = set(roles) - set(existing_roles)
         if unknown_roles:
             raise ValueError(f"role(s) not found: {', '.join(unknown_roles)}")
```

### Comparing `pglift-0.8.0/src/pglift/prometheus.py` & `pglift-0.9.0/src/pglift/prometheus.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/queries.sql` & `pglift-0.9.0/src/pglift/queries.sql`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/roles.py` & `pglift-0.9.0/src/pglift/roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     :raises ~pglift.exceptions.RoleNotFound: if no role with specified 'name' exists.
     """
     if not exists(ctx, instance, name):
         raise exceptions.RoleNotFound(name)
     role = interface.Role(name=name)
     values = role.dict()
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         cnx.autocommit = True
         with cnx.cursor() as cur:
             cur.execute(db.query("role_inspect"), {"username": name})
             values.update(dict(cur.fetchone()))
     if in_pgpass(ctx, instance, name):
         values["pgpass"] = True
     return interface.Role(**values)
@@ -103,36 +103,36 @@
 def drop(ctx: BaseContext, instance: Instance, name: str) -> None:
     """Drop a role from instance.
 
     :raises ~pglift.exceptions.RoleNotFound: if no role with specified 'name' exists.
     """
     if not exists(ctx, instance, name):
         raise exceptions.RoleNotFound(name)
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         with cnx.cursor() as cur:
             cur.execute(db.query("role_drop", username=sql.Identifier(name)))
         cnx.commit()
     role = interface.Role(name=name, pgpass=False)
     set_pgpass_entry_for(ctx, instance, role)
 
 
 def exists(ctx: BaseContext, instance: Instance, name: str) -> bool:
     """Return True if named role exists in 'instance'.
 
     The instance should be running.
     """
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         with cnx.cursor() as cur:
             cur.execute(db.query("role_exists"), {"username": name})
             return cur.rowcount == 1  # type: ignore[no-any-return]
 
 
 def has_password(ctx: BaseContext, instance: Instance, name: str) -> bool:
     """Return True if the role has a password set."""
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         with cnx.cursor() as cur:
             cur.execute(db.query("role_has_password"), {"username": name})
             (haspassword,) = cur.fetchone()
             return haspassword  # type: ignore[no-any-return]
 
 
 def options_and_args(
@@ -181,15 +181,15 @@
 @task("create role '{role.name}' on instance {instance}")
 def create(ctx: BaseContext, instance: Instance, role: interface.Role) -> None:
     """Create 'role' in 'instance'.
 
     The instance should be running and the role should not exist already.
     """
     options, args = options_and_args(role)
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         with cnx.cursor() as cur:
             cur.execute(
                 db.query(
                     "role_create",
                     username=sql.Identifier(role.name),
                     options=options,
                 ),
@@ -208,15 +208,15 @@
     options, args = options_and_args(
         role, with_password=not has_password(ctx, instance, role.name), in_roles=False
     )
     in_roles = {
         "grant": set(role.in_roles) - set(actual_role.in_roles),
         "revoke": set(actual_role.in_roles) - set(role.in_roles),
     }
-    with db.superuser_connect(instance) as cnx:
+    with db.superuser_connect(ctx, instance) as cnx:
         with cnx.cursor() as cur:
             cur.execute(
                 db.query(
                     "role_alter",
                     username=sql.Identifier(role.name),
                     options=options,
                 ),
@@ -241,15 +241,15 @@
 def set_password_for(
     ctx: BaseContext, instance: PostgreSQLInstance, role: Role
 ) -> None:
     """Set password for a PostgreSQL role on instance."""
     if role.password is None:
         return
 
-    with db.superuser_connect(instance) as conn:
+    with db.superuser_connect(ctx, instance) as conn:
         conn.autocommit = True
         with conn.cursor() as cur:
             cur.execute(
                 db.query("role_alter_password", username=sql.Identifier(role.name)),
                 {"password": role.password.get_secret_value()},
             )
```

### Comparing `pglift-0.8.0/src/pglift/settings.py` & `pglift-0.9.0/src/pglift/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,20 @@
 import json
 import os
 import shutil
 from pathlib import Path, PosixPath
 from typing import Any, Callable, Dict, Iterator, Optional, Tuple, Type, TypeVar
 
 import yaml
-from pydantic import BaseSettings, Field, SecretStr, root_validator, validator
+from pydantic import BaseSettings, Field, root_validator, validator
 from pydantic.fields import ModelField
 from typing_extensions import Literal
 
 from . import __name__ as pkgname
 from . import datapath
-from .types import Role
 from .util import xdg_data_home
 
 try:
     from pydantic.env_settings import SettingsSourceCallable
 except ImportError:
     SettingsSourceCallable = Callable[[BaseSettings], Dict[str, Any]]  # type: ignore[misc]
 
@@ -139,39 +138,16 @@
     """Default authentication method for local TCP/IP connections"""
     host: AuthMethod = "trust"
     """Default authentication method for local-socket connections."""
 
     passfile: Path = Path.home() / ".pgpass"
     """Path to .pgpass file."""
 
-    def libpq_environ(
-        self,
-        role: Optional[Role] = None,
-        *,
-        base: Dict[str, str] = os.environ,  # type: ignore[assignment]
-    ) -> Dict[str, str]:
-        """Return a dict with libpq environment variables for `role`
-        authentication.
-
-        >>> class MyRole(BaseSettings):
-        ...     name: str
-        ...     password: Optional[SecretStr] = None
-
-        >>> s = AuthSettings.parse_obj({"passfile": "/srv/pg/.pgpass"})
-        >>> s.libpq_environ(MyRole(name="bob"), base={"PGPASSWORD": "secret"})
-        {'PGPASSWORD': 'secret', 'PGPASSFILE': '/srv/pg/.pgpass'}
-        >>> s.libpq_environ(MyRole(name="bob", password=SecretStr("secret")),
-        ...                 base={'PGPASSFILE': '/var/lib/pgsql/pgpass'})
-        {'PGPASSFILE': '/var/lib/pgsql/pgpass', 'PGPASSWORD': 'secret'}
-        """
-        env = base.copy()
-        env.setdefault("PGPASSFILE", str(self.passfile))
-        if role is not None and role.password:
-            env.setdefault("PGPASSWORD", role.password.get_secret_value())
-        return env
+    password_command: Optional[str] = None
+    """An optional command to retrieve PGPASSWORD from"""
 
 
 @frozen
 class InitdbSettings(BaseSettings):
     """Settings for initdb step of a PostgreSQL instance."""
 
     class Config:
```

### Comparing `pglift-0.8.0/src/pglift/systemd.py` & `pglift-0.9.0/src/pglift/systemd.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/task.py` & `pglift-0.9.0/src/pglift/task.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/types.py` & `pglift-0.9.0/src/pglift/types.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift/util.py` & `pglift-0.9.0/src/pglift/util.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/src/pglift.egg-info/PKG-INFO` & `pglift-0.9.0/src/pglift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglift
-Version: 0.8.0
+Version: 0.9.0
 Summary: Life-cycle management of production-ready PostgreSQL instances
 Home-page: https://gitlab.com/dalibo/pglift
 Author: Dalibo SCOP
 Author-email: contact@dalibo.com
 License: UNKNOWN
 Project-URL: Documentation, https://pglift.readthedocs.io/
 Project-URL: Source, https://gitlab.com/dalibo/pglift/
```

### Comparing `pglift-0.8.0/src/pglift.egg-info/SOURCES.txt` & `pglift-0.9.0/src/pglift.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/test__install.py
 tests/unit/test_backup.py
 tests/unit/test_cli.py
 tests/unit/test_cmd.py
 tests/unit/test_conf.py
+tests/unit/test_ctx.py
 tests/unit/test_db.py
 tests/unit/test_exceptions.py
 tests/unit/test_instance.py
 tests/unit/test_models_helpers.py
 tests/unit/test_models_interface.py
 tests/unit/test_models_system.py
 tests/unit/test_pgbackrest.py
```

### Comparing `pglift-0.8.0/tests/data/ansible-argspec-instance.json` & `pglift-0.9.0/tests/data/ansible-argspec-instance.json`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/data/ansible-argspec-postgresexporter.json` & `pglift-0.9.0/tests/data/ansible-argspec-postgresexporter.json`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/data/ansible-argspec-role.json` & `pglift-0.9.0/tests/data/ansible-argspec-role.json`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/data/queries.json` & `pglift-0.9.0/tests/data/queries.json`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/func/__init__.py` & `pglift-0.9.0/tests/func/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     query: str,
     fetch: bool = True,
     autocommit: bool = False,
     role: Optional[Role] = None,
     **kwargs: Any,
 ) -> Optional[List[Any]]:
     if role is None:
-        connect = db.superuser_connect
+        connect = partial(db.superuser_connect, ctx)
     elif role.password:
         connect = partial(
             db.connect, user=role.name, password=role.password.get_secret_value()
         )
     else:
         connect = partial(db.connect, user=role.name)
     with instance_mod.running(ctx, instance):
```

### Comparing `pglift-0.8.0/tests/func/conftest.py` & `pglift-0.9.0/tests/func/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import logging
 import pathlib
 import platform
 import shutil
 import subprocess
 from datetime import datetime
 from typing import Any, Iterator, Optional, Set
-from unittest.mock import patch
 
 import pgtoolkit.conf
 import port_for
 import pydantic
 import pytest
 from pgtoolkit.ctl import Status
 from typing_extensions import Protocol
@@ -68,15 +67,15 @@
                 "host": "reject",
             },
             "surole": {
                 "pgpass": True,
             },
         },
     },
-    "postgresql_password_auth__surole_no_pgpass": {
+    "postgresql_password_auth__surole_password_command": {
         "postgresql": {
             "auth": {
                 "local": "password",
                 "host": "reject",
             },
             "surole": {
                 "pgpass": False,
@@ -105,14 +104,22 @@
     obj["prefix"] = str(prefix)
     pg_obj = obj.setdefault("postgresql", {})
     assert "root" not in pg_obj
     pg_obj["root"] = str(tmp_path_factory.mktemp("postgres"))
     pgauth_obj = pg_obj.setdefault("auth", {})
     assert "passfile" not in pgauth_obj
     pgauth_obj["passfile"] = str(passfile)
+
+    if pgauth_obj.get("local", "trust") != "trust" and not pg_obj.get("surole", {}).get(
+        "pgpass", True
+    ):
+        assert "password_command" not in pgauth_obj
+        pgauth_obj["password_command"] = str(
+            tmp_path_factory.mktemp("home") / "passcmd"
+        )
     if obj.get("service_manager") == "systemd" and not systemd_available:
         pytest.skip("systemd not functional")
     try:
         return Settings.parse_obj(obj)
     except pydantic.ValidationError as exc:
         pytest.skip(
             "; ".join(
@@ -180,17 +187,25 @@
 
 @pytest.fixture(scope="session")
 def surole_password(settings: Settings) -> Iterator[Optional[str]]:
     if settings.postgresql.auth.local == "trust":
         yield None
         return
 
-    password = "s3kret"
-    with patch.dict("os.environ", {"PGPASSWORD": password}):
-        yield password
+    passcmdfile = (
+        pathlib.Path(settings.postgresql.auth.password_command)
+        if settings.postgresql.auth.password_command
+        else None
+    )
+    if passcmdfile:
+        with passcmdfile.open("w") as f:
+            f.write("#!/bin/sh\necho s3kret\n")
+        passcmdfile.chmod(0o700)
+
+    yield "s3kret"
 
 
 @pytest.fixture(scope="session")
 def instance_manifest(
     pg_version: str,
     settings: Settings,
     surole_password: Optional[str],
```

### Comparing `pglift-0.8.0/tests/func/test_10_instance.py` & `pglift-0.9.0/tests/func/test_10_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import contextlib
 import logging
 from pathlib import Path
-from typing import Iterator, List, NoReturn, Optional
+from typing import Iterator, List, NoReturn
 from unittest.mock import patch
 
 import psycopg2
 import pytest
 from pgtoolkit.ctl import Status
 from tenacity import retry
 from tenacity.retry import retry_if_exception_type
@@ -299,14 +299,15 @@
         standby_for += f" password={surole.password.get_secret_value()}"
     else:
         standby_for += f" passfile={settings.postgresql.auth.passfile}"
     standby_manifest = interface.Instance(
         name="standby",
         version=pg_version,
         standby=interface.Instance.Standby(**{"for": standby_for, "slot": slot}),
+        surole_password=surole.password,
     )
 
     @contextlib.contextmanager
     def instance_running_with_table() -> Iterator[None]:
         with instance_mod.running(ctx, instance):
             execute(ctx, instance, "CREATE TABLE t AS (SELECT 1 AS i)", fetch=False)
             try:
@@ -367,15 +368,14 @@
             assert not pg_replication_slots()
             instance_mod.drop(ctx, standby_instance)
 
 
 def test_instance_upgrade(
     ctx: Context,
     instance: system.Instance,
-    surole_password: Optional[str],
     tmp_port_factory: Iterator[int],
     database_factory: DatabaseFactory,
 ) -> None:
     database_factory("present")
     port = next(tmp_port_factory)
     newinstance = instance_mod.upgrade(
         ctx,
```

### Comparing `pglift-0.8.0/tests/func/test_11_databases.py` & `pglift-0.9.0/tests/func/test_11_databases.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import pathlib
 import time
 from typing import Iterator
 
 import pytest
 
 from pglift import databases, exceptions
 from pglift import instance as instance_mod
@@ -142,14 +143,34 @@
         databases.drop(ctx, instance, "absent")
 
     database_factory("dropme")
     databases.drop(ctx, instance, "dropme")
     assert not databases.exists(ctx, instance, "dropme")
 
 
+def test_backup(
+    ctx: Context,
+    instance: system.Instance,
+    database_factory: DatabaseFactory,
+    tmp_path: pathlib.Path,
+) -> None:
+    output_file = tmp_path / "db.dump"
+    with pytest.raises(exceptions.DatabaseNotFound, match="absent"):
+        databases.backup(ctx, instance, "absent", output_file)
+    assert not output_file.exists()
+
+    database_factory("backupme")
+    databases.run(
+        ctx, instance, "CREATE TABLE test(x int, y text);", dbnames=["backupme"]
+    )
+    databases.backup(ctx, instance, "backupme", output_file)
+    assert output_file.exists()
+    assert b"CREATE TABLE public.test " in output_file.read_bytes()
+
+
 def test_run_analyze(
     ctx: Context, instance: system.Instance, database_factory: DatabaseFactory
 ) -> None:
     database_factory("test")
 
     def last_analyze() -> datetime.datetime:
         result = execute(
```

### Comparing `pglift-0.8.0/tests/func/test_11_privileges.py` & `pglift-0.9.0/tests/func/test_11_privileges.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/func/test_11_roles.py` & `pglift-0.9.0/tests/func/test_11_roles.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/func/test_20_backup.py` & `pglift-0.9.0/tests/func/test_20_backup.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/func/test_20_pgbackrest.py` & `pglift-0.9.0/tests/func/test_20_pgbackrest.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/func/test_20_prometheus.py` & `pglift-0.9.0/tests/func/test_20_prometheus.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/func/test_99_drop.py` & `pglift-0.9.0/tests/func/test_99_drop.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/func/test_ansible.py` & `pglift-0.9.0/tests/func/test_ansible.py`

 * *Files identical despite different names*

### Comparing `pglift-0.8.0/tests/unit/conftest.py` & `pglift-0.9.0/tests/unit/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import logging
 from pathlib import Path
+from typing import Any
 
 import pytest
 from pgtoolkit.ctl import PGCtl
 
 from pglift import pm, prometheus
 from pglift.ctx import Context
+from pglift.models import interface
 from pglift.models.system import Instance, PrometheusService
 from pglift.settings import Settings
 from pglift.util import short_version
 
 
-def pytest_addoption(parser, pluginmanager):
+def pytest_addoption(parser: Any) -> None:
     parser.addoption(
         "--regen-test-data",
         action="store_true",
         default=False,
         help="Re-generate test data from actual results",
     )
 
 
 @pytest.fixture
-def regen_test_data(request):
-    return request.config.getoption("--regen-test-data")
+def regen_test_data(request: Any) -> bool:
+    value = request.config.getoption("--regen-test-data")
+    assert isinstance(value, bool)
+    return value
 
 
 @pytest.fixture
 def settings(tmp_path: Path) -> Settings:
     passfile = tmp_path / "pgass"
     passfile.touch()
     return Settings.parse_obj(
@@ -57,14 +61,19 @@
 @pytest.fixture
 def ctx(settings: Settings) -> Context:
     p = pm.PluginManager.get()
     return Context(plugin_manager=p, settings=settings)
 
 
 @pytest.fixture
+def instance_manifest(pg_version: str) -> interface.Instance:
+    return interface.Instance(name="test", version=pg_version)
+
+
+@pytest.fixture
 def instance(pg_version: str, settings: Settings) -> Instance:
     prometheus_port = 9817
     instance = Instance(
         name="test",
         version=pg_version,
         settings=settings,
         prometheus=PrometheusService(port=prometheus_port),
```

### Comparing `pglift-0.8.0/tests/unit/test__install.py` & `pglift-0.9.0/tests/unit/test__install.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 
 from pglift import _install
+from pglift.ctx import Context
 
 
-def test_postgresql_systemd_unit_template(ctx):
+def test_postgresql_systemd_unit_template(ctx: Context) -> None:
     _install.postgresql_systemd_unit_template(
         ctx, env="SETTINGS=@settings.json", header="# Postgres managed by pglift"
     )
     unit = ctx.settings.systemd.unit_path / "pglift-postgresql@.service"
     assert unit.exists()
     lines = unit.read_text().splitlines()
     assert lines[0] == "# Postgres managed by pglift"
@@ -20,15 +21,15 @@
             break
     else:
         raise AssertionError("ExecStart line not found")
     _install.revert_postgresql_systemd_unit_template(ctx)
     assert not unit.exists()
 
 
-def test_postgres_exporter_systemd_unit_template(ctx):
+def test_postgres_exporter_systemd_unit_template(ctx: Context) -> None:
     _install.postgres_exporter_systemd_unit_template(ctx)
     unit = ctx.settings.systemd.unit_path / "pglift-postgres_exporter@.service"
     assert unit.exists()
     lines = unit.read_text().splitlines()
     assert (
         f"EnvironmentFile=-{ctx.settings.prefix}/etc/prometheus/postgres_exporter-%i.conf"
         in lines
@@ -37,15 +38,15 @@
         "ExecStart=/usr/bin/prometheus-postgres-exporter $POSTGRES_EXPORTER_OPTS"
         in lines
     )
     _install.revert_postgres_exporter_systemd_unit_template(ctx)
     assert not unit.exists()
 
 
-def test_postgresql_backup_systemd_templates(ctx):
+def test_postgresql_backup_systemd_templates(ctx: Context) -> None:
     _install.postgresql_backup_systemd_templates(ctx, env="X-DEBUG=no")
     service_unit = ctx.settings.systemd.unit_path / "pglift-backup@.service"
     assert service_unit.exists()
     service_lines = service_unit.read_text().splitlines()
     for line in service_lines:
         if line.startswith("ExecStart"):
             execstart = line.split("=", 1)[-1]
```

### Comparing `pglift-0.8.0/tests/unit/test_cli.py` & `pglift-0.9.0/tests/unit/test_cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,158 @@
 import datetime
 import functools
 import json
 import re
-from typing import Iterator
+from pathlib import Path
+from typing import Any, Dict, Iterator
 from unittest.mock import MagicMock, patch
 
 import click
 import pytest
 import yaml
 from click.testing import CliRunner
 from pgtoolkit.ctl import Status
 
 from pglift import _install, databases, exceptions
 from pglift import instance as instance_mod
 from pglift import pgbackrest, prometheus, roles
-from pglift.cli import Command, Obj, cli, instance_init, require_component
+from pglift.cli import Command, Obj, cli, get_instance, instance_init, require_component
 from pglift.ctx import Context
 from pglift.models import interface
 from pglift.models.system import Instance
 
 
 @pytest.fixture
-def runner():
+def runner() -> CliRunner:
     return CliRunner(mix_stderr=False)
 
 
 @pytest.fixture
-def obj(ctx):
+def obj(ctx: Context) -> Obj:
     return Obj(ctx, None)
 
 
 @pytest.fixture
 def running(ctx: Context, instance: Instance) -> Iterator[MagicMock]:
     with patch("pglift.instance.running") as m:
         yield m
     m.assert_called_once_with(ctx, instance)
 
 
 @click.command(cls=Command)
 @click.argument("error")
 @click.pass_context
-def cmd(ctx, error):
+def cmd(ctx: click.Context, error: str) -> None:
     if error == "error":
         raise exceptions.CommandError(1, ["bad", "cmd"], "output", "errs")
     if error == "runtimeerror":
         raise RuntimeError("oups")
     if error == "exit":
         ctx.exit(1)
 
 
-def test_command_error(runner, obj):
+def test_command_error(runner: CliRunner, obj: Obj) -> None:
     result = runner.invoke(cmd, ["error"], obj=obj)
     assert result.exit_code == 1
     assert (
         result.stderr
-        == "Error: Command '['bad', 'cmd']' returned non-zero exit status 1.\nerrs\n"
+        == "Error: Command '['bad', 'cmd']' returned non-zero exit status 1.\nerrs\noutput\n"
     )
     logpath = obj.ctx.settings.logpath
     assert not list(logpath.glob("*.log"))
 
 
-def test_command_exit(runner, obj):
+def test_command_exit(runner: CliRunner, obj: Obj) -> None:
     result = runner.invoke(cmd, ["exit"], obj=obj)
     assert result.exit_code == 1
     assert not result.stdout
     logpath = obj.ctx.settings.logpath
     assert not list(logpath.glob("*.log"))
 
 
-def test_command_internal_error(runner, obj):
+def test_command_internal_error(runner: CliRunner, obj: Obj) -> None:
     result = runner.invoke(cmd, ["runtimeerror"], obj=obj)
     assert result.exit_code == 1
     logpath = obj.ctx.settings.logpath
     logfile = next(logpath.glob("*.log"))
     logcontent = logfile.read_text()
     assert "an unexpected error occurred" in logcontent
     assert "Traceback (most recent call last):" in logcontent
     assert "RuntimeError: oups" in logcontent
 
 
-def test_require_component(runner, ctx):
+def test_require_component(runner: CliRunner, ctx: Context) -> None:
     mod = MagicMock()
 
     @click.command("command")
     @click.pass_obj
     @functools.partial(require_component, mod, "mymod")
-    def command(ctx, *args):
+    def command(ctx: click.Context, *args: Any) -> None:
         click.echo(f"ctx is {type(ctx)}")
 
     mod.enabled.return_value = False
     r = runner.invoke(command, obj=ctx)
     assert r.exit_code == 1
     assert r.stderr == "mymod not available\n"
 
     mod.enabled.return_value = True
     r = runner.invoke(command, obj=ctx)
     assert r.exit_code == 0
     assert r.stdout == "ctx is <class 'pglift.ctx.Context'>\n"
 
 
-def test_cli(runner, obj):
+def test_get_instance(ctx: Context, instance: Instance) -> None:
+    assert get_instance(ctx, instance.name, instance.version) == instance
+
+    assert get_instance(ctx, instance.name, None) == instance
+
+    with pytest.raises(click.BadParameter):
+        get_instance(ctx, "notfound", None)
+
+    with pytest.raises(click.BadParameter):
+        get_instance(ctx, "notfound", instance.version)
+
+    with patch.object(Instance, "system_lookup") as system_lookup:
+        with pytest.raises(
+            click.BadParameter,
+            match="instance 'foo' exists in several PostgreSQL version",
+        ):
+            get_instance(ctx, "foo", None)
+    assert system_lookup.call_count == 2
+
+
+def test_cli(runner: CliRunner, obj: Obj) -> None:
     result = runner.invoke(cli, obj=obj)
     assert result.exit_code == 0
 
 
-def test_version(runner, obj):
+def test_version(runner: CliRunner, obj: Obj) -> None:
     result = runner.invoke(cli, ["--version"], obj=obj)
     assert re.match(r"pglift version (\d\.).*", result.stdout)
 
 
-def test_site_configure(runner, ctx, obj, tmp_path):
+def test_site_configure(
+    runner: CliRunner, ctx: Context, obj: Obj, tmp_path: Path
+) -> None:
     with patch.object(_install, "do") as do_install:
         result = runner.invoke(
             cli, ["site-configure", "install", f"--settings={tmp_path}"], obj=obj
         )
     assert result.exit_code == 0, result
     do_install.assert_called_once_with(ctx, env=f"SETTINGS=@{tmp_path}")
 
     with patch.object(_install, "undo") as undo_install:
         result = runner.invoke(cli, ["site-configure", "uninstall"], obj=obj)
     assert result.exit_code == 0, result
     undo_install.assert_called_once_with(ctx)
 
 
-def test_instance_init(runner, ctx, obj, instance):
+def test_instance_init(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance
+) -> None:
     assert [p.name for p in instance_init.params] == [
         "name",
         "version",
         "port",
         "state",
         "surole_password",
         "standby_for",
@@ -151,15 +176,17 @@
             ["instance", "init", "new", "--port=1234"],
             obj=obj,
         )
     apply.assert_called_once_with(ctx, interface.Instance(name="new", port=1234))
     assert result.exit_code == 0, result
 
 
-def test_instance_apply(tmp_path, runner, ctx, obj):
+def test_instance_apply(
+    tmp_path: Path, runner: CliRunner, ctx: Context, obj: Obj
+) -> None:
     result = runner.invoke(cli, ["--log-level=debug", "instance", "apply"], obj=obj)
     assert result.exit_code == 2
     assert "Missing option '-f'" in result.stderr
 
     manifest = tmp_path / "manifest.yml"
     content = yaml.dump({"name": "test"})
     manifest.write_text(content)
@@ -167,71 +194,77 @@
         result = runner.invoke(cli, ["instance", "apply", "-f", str(manifest)], obj=obj)
     assert result.exit_code == 0, (result, result.output)
     mock_method.assert_called_once()
     assert mock_method.call_args[0][0] == ctx
     assert isinstance(mock_method.call_args[0][1], interface.Instance)
 
 
-def test_instance_alter(runner, ctx, obj):
+def test_instance_alter(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance
+) -> None:
     result = runner.invoke(
-        cli, ["instance", "alter", "notfound", "--version=11"], obj=obj
+        cli, ["instance", "alter", "11/notfound", "--port=1"], obj=obj
     )
-    assert result.exit_code == 1
-    assert "Error: instance '11/notfound' not found" in result.stderr
+    assert result.exit_code == 2, result.stderr
+    assert "instance '11/notfound' not found" in result.stderr
 
     actual = interface.Instance.parse_obj(
-        {"name": "alterme", "prometheus": {"port": 1212}}
+        {"name": instance.name, "prometheus": {"port": 1212}}
     )
     altered = interface.Instance.parse_obj(
         {
-            "name": "alterme",
+            "name": instance.name,
             "state": "stopped",
             "prometheus": {"port": 2121},
         }
     )
     with patch.object(instance_mod, "apply") as apply, patch.object(
         instance_mod, "describe", return_value=actual
     ) as describe:
         result = runner.invoke(
             cli,
             [
                 "instance",
                 "alter",
-                "alterme",
+                str(instance),
                 "--state=stopped",
                 "--prometheus-port=2121",
             ],
             obj=obj,
         )
-    describe.assert_called_once_with(ctx, "alterme", None)
+    describe.assert_called_once_with(ctx, instance.name, instance.version)
     apply.assert_called_once_with(ctx, altered)
     assert result.exit_code == 0, result.output
 
 
-def test_instance_schema(runner, obj):
+def test_instance_schema(runner: CliRunner, obj: Obj) -> None:
     result = runner.invoke(cli, ["instance", "schema"], obj=obj)
     schema = json.loads(result.output)
     assert schema["title"] == "Instance"
     assert schema["description"] == "PostgreSQL instance"
 
 
-def test_instance_describe(runner, ctx, obj, instance, pg_version):
+def test_instance_describe(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance, pg_version: str
+) -> None:
     result = runner.invoke(cli, ["instance", "describe"], obj=obj)
     assert result.exit_code == 2
     assert "Missing argument '<version>/<name>'" in result.stderr
 
-    instance = interface.Instance(name="test")
-    with patch.object(instance_mod, "describe", return_value=instance) as describe:
+    manifest = interface.Instance(name="test")
+    with patch.object(instance_mod, "describe", return_value=manifest) as describe:
         result = runner.invoke(cli, ["instance", "describe", "test"], obj=obj)
     assert result.exit_code == 0, (result, result.output)
     describe.assert_called_once_with(ctx, "test", pg_version)
     assert "name: test" in result.output
 
 
-def test_instance_list(runner, instance, ctx, obj, tmp_path):
+def test_instance_list(
+    runner: CliRunner, instance: Instance, ctx: Context, obj: Obj, tmp_path: Path
+) -> None:
     name, version = instance.name, instance.version
     port = instance.config().port
     path = instance.path
     expected_list_as_json = [
         {
             "name": name,
             "path": str(path),
@@ -268,33 +301,37 @@
     result = runner.invoke(
         cli, ["instance", "list", f"--version={other_version}"], obj=obj
     )
     assert result.exit_code == 0
     assert not result.output
 
 
-def test_instance_config_show(runner, obj, instance):
+def test_instance_config_show(runner: CliRunner, obj: Obj, instance: Instance) -> None:
     result = runner.invoke(cli, ["instance", "config", "show", str(instance)], obj=obj)
     assert result.exit_code == 0, result.stderr
     assert result.stdout.strip() == "\n".join(
         ["port = 999", "unix_socket_directories = '/socks'"]
     )
 
 
-def test_instance_config_set_validate(runner, obj, instance):
+def test_instance_config_set_validate(
+    runner: CliRunner, obj: Obj, instance: Instance
+) -> None:
     result = runner.invoke(
         cli,
         ["instance", "config", "set", str(instance), "invalid"],
         obj=obj,
     )
     assert result.exit_code == 2
     assert "Error: Invalid value for '<PARAMETER>=<VALUE>': invalid" in result.stderr
 
 
-def test_instance_config_set(runner, ctx, obj, instance):
+def test_instance_config_set(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance
+) -> None:
     with patch.object(
         instance_mod, "configure", return_value={"foo": ("baz", "bar")}
     ) as configure:
         result = runner.invoke(
             cli,
             [
                 "instance",
@@ -329,15 +366,17 @@
     manifest = interface.Instance(name=instance.name, version=instance.version)
     configure.assert_called_once_with(ctx, manifest, foo="bar")
     assert "foo: baz -> bar" not in result.stderr
     assert "changes in 'foo' not applied" in result.stderr
     assert "\n hint:" in result.stderr
 
 
-def test_instance_config_remove(runner, ctx, obj, instance):
+def test_instance_config_remove(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance
+) -> None:
     with patch.object(
         instance_mod, "configure", return_value={"cluster_name": ("blah", None)}
     ) as configure:
         result = runner.invoke(
             cli,
             [
                 "instance",
@@ -350,60 +389,75 @@
         )
     manifest = interface.Instance(name=instance.name, version=instance.version)
     configure.assert_called_once_with(ctx, manifest, cluster_name=None)
     assert result.exit_code == 0, result.stderr
     assert "cluster_name: blah -> None" in result.stderr
 
 
-def test_instance_config_edit(runner, ctx, obj, instance):
+def test_instance_config_edit(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance
+) -> None:
     with patch("click.edit") as edit:
         result = runner.invoke(
             cli,
             ["instance", "config", "edit", str(instance)],
             obj=obj,
         )
     assert result.exit_code == 0, result.stderr
     edit.assert_called_once_with(
         filename=str(instance.datadir / "conf.pglift.d" / "user.conf")
     )
 
 
-def test_instance_drop(runner, ctx, obj, instance):
+def test_instance_drop(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance
+) -> None:
     result = runner.invoke(cli, ["instance", "drop"], obj=obj)
     assert result.exit_code == 2
     assert "Missing argument '<version>/<name>'" in result.stderr
 
     with patch.object(instance_mod, "drop") as patched:
         result = runner.invoke(cli, ["instance", "drop", "test"], obj=obj)
     assert result.exit_code == 0, (result, result.output)
     patched.assert_called_once_with(ctx, instance)
 
 
-def test_instance_status(runner, instance, ctx, obj):
+def test_instance_status(
+    runner: CliRunner, instance: Instance, ctx: Context, obj: Obj
+) -> None:
     with patch.object(
         instance_mod, "status", return_value=Status.not_running
     ) as patched:
         result = runner.invoke(cli, ["instance", "status", instance.name], obj=obj)
     assert result.exit_code == 3, (result, result.output)
     assert result.stdout == "not running\n"
     patched.assert_called_once_with(ctx, instance)
 
 
 @pytest.mark.parametrize(
     ["action", "kwargs"],
     [("start", {"foreground": False}), ("stop", {}), ("reload", {}), ("restart", {})],
 )
-def test_instance_operations(runner, instance, ctx, obj, action, kwargs):
+def test_instance_operations(
+    runner: CliRunner,
+    instance: Instance,
+    ctx: Context,
+    obj: Obj,
+    action: str,
+    kwargs: Dict[str, bool],
+) -> None:
     with patch.object(instance_mod, action) as patched:
         result = runner.invoke(cli, ["instance", action, str(instance)], obj=obj)
     assert result.exit_code == 0, result
     patched.assert_called_once_with(ctx, instance, **kwargs)
 
 
-def test_instance_shell(runner, instance, ctx, obj):
+def test_instance_shell(
+    runner: CliRunner, instance: Instance, ctx: Context, obj: Obj
+) -> None:
     with patch.object(
         instance_mod, "status", return_value=instance_mod.Status.not_running
     ) as status, patch.object(instance_mod, "shell") as shell:
         r = runner.invoke(cli, ["instance", "shell", instance.name], obj=obj)
     status.assert_called_once_with(ctx, instance)
     assert not shell.called
     assert r.exit_code == 1
@@ -413,27 +467,27 @@
         instance_mod, "status", return_value=instance_mod.Status.running
     ) as status, patch.object(instance_mod, "shell") as shell:
         runner.invoke(cli, ["instance", "shell", instance.name, "-U", "bob"], obj=obj)
     status.assert_called_once_with(ctx, instance)
     shell.assert_called_once_with(ctx, instance, user="bob", dbname=None)
 
 
-def test_instance_backup(runner, instance, obj):
+def test_instance_backup(runner: CliRunner, instance: Instance, obj: Obj) -> None:
     with patch.object(pgbackrest, "backup") as backup:
         result = runner.invoke(
             cli,
             ["instance", "backup", str(instance), "--type=diff"],
             obj=obj,
         )
     assert result.exit_code == 0, result
     assert backup.call_count == 1
     assert backup.call_args[1] == {"type": pgbackrest.BackupType("diff")}
 
 
-def test_instance_restore_list(runner, instance, obj):
+def test_instance_restore_list(runner: CliRunner, instance: Instance, obj: Obj) -> None:
     bck = interface.InstanceBackup(
         label="foo",
         size=12,
         repo_size=13,
         datetime=datetime.datetime(2012, 1, 1),
         type="incr",
         databases="postgres, prod",
@@ -455,15 +509,17 @@
         "13.0",
         "2012-01-01 00:00:00",
         "incr",
         "postgres, prod",
     ]
 
 
-def test_instance_restore(runner, instance, ctx, obj):
+def test_instance_restore(
+    runner: CliRunner, instance: Instance, ctx: Context, obj: Obj
+) -> None:
     with patch("pglift.instance.status", return_value=Status.running) as status:
         result = runner.invoke(
             cli,
             ["instance", "restore", str(instance)],
             obj=obj,
         )
     assert result.exit_code == 1, result
@@ -476,15 +532,17 @@
             ["instance", "restore", str(instance), "--label=xyz"],
             obj=obj,
         )
     assert result.exit_code == 0, result
     assert restore.called_once_with(ctx, instance, label="xyz")
 
 
-def test_instance_privileges(ctx, obj, instance, runner, running):
+def test_instance_privileges(
+    ctx: Context, obj: Obj, instance: Instance, runner: CliRunner, running: MagicMock
+) -> None:
     with patch(
         "pglift.privileges.get",
         return_value=[
             interface.Privilege(
                 database="db2",
                 schema="public",
                 role="rol2",
@@ -518,15 +576,17 @@
             "role": "rol2",
             "object_type": "FUNCTION",
             "privileges": ["EXECUTE"],
         }
     ]
 
 
-def test_role_create(ctx, obj, instance, runner, running):
+def test_role_create(
+    ctx: Context, obj: Obj, instance: Instance, runner: CliRunner, running: MagicMock
+) -> None:
     with patch.object(roles, "exists", return_value=False) as exists, patch.object(
         roles, "apply"
     ) as apply:
         result = runner.invoke(
             cli,
             [
                 "role",
@@ -570,15 +630,17 @@
         )
     assert result.exit_code == 1
     assert "role already exists" in result.stderr
     exists.assert_called_once_with(ctx, instance, "bob")
     running.assert_called_once_with(ctx, instance)
 
 
-def test_role_alter(runner, ctx, obj, instance, running):
+def test_role_alter(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance, running: MagicMock
+) -> None:
     actual = interface.Role(name="alterme", connection_limit=3)
     altered = interface.Role(
         name="alterme",
         connection_limit=30,
         pgpass=True,
         password="blah",
         login=True,
@@ -604,22 +666,29 @@
             obj=obj,
         )
     describe.assert_called_once_with(ctx, instance, "alterme")
     apply.assert_called_once_with(ctx, instance, altered)
     assert result.exit_code == 0, result.output
 
 
-def test_role_schema(runner):
+def test_role_schema(runner: CliRunner) -> None:
     result = runner.invoke(cli, ["role", "schema"])
     schema = json.loads(result.output)
     assert schema["title"] == "Role"
     assert schema["description"] == "PostgreSQL role"
 
 
-def test_role_apply(runner, tmp_path, ctx, obj, instance, running):
+def test_role_apply(
+    runner: CliRunner,
+    tmp_path: Path,
+    ctx: Context,
+    obj: Obj,
+    instance: Instance,
+    running: MagicMock,
+) -> None:
     manifest = tmp_path / "manifest.yml"
     content = yaml.dump({"name": "roltest", "pgpass": True})
     manifest.write_text(content)
     with patch.object(roles, "apply") as apply:
         result = runner.invoke(
             cli,
             ["role", "apply", str(instance), "-f", str(manifest)],
@@ -631,15 +700,17 @@
     (call_ctx, call_instance, call_role), kwargs = apply.call_args
     assert call_ctx == ctx
     assert call_instance == instance
     assert call_role.name == "roltest"
     assert kwargs == {}
 
 
-def test_role_describe(runner, ctx, obj, instance, running):
+def test_role_describe(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance, running: MagicMock
+) -> None:
     with patch.object(
         roles, "describe", side_effect=exceptions.RoleNotFound("absent")
     ) as describe:
         result = runner.invoke(
             cli,
             ["role", "describe", str(instance), "absent"],
             obj=obj,
@@ -683,15 +754,17 @@
         "login": False,
         "connection_limit": 5,
         "validity": "2022-01-01T00:00:00",
         "in_roles": ["observers", "monitoring"],
     }
 
 
-def test_role_drop(runner, ctx, obj, instance, running):
+def test_role_drop(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance, running: MagicMock
+) -> None:
     with patch.object(
         roles, "drop", side_effect=exceptions.RoleNotFound("bar")
     ) as drop:
         result = runner.invoke(
             cli,
             ["role", "drop", str(instance), "foo"],
             obj=obj,
@@ -710,15 +783,17 @@
             obj=obj,
         )
     drop.assert_called_once_with(ctx, instance, "foo")
     running.assert_called_once_with(ctx, instance)
     assert result.exit_code == 0
 
 
-def test_role_privileges(ctx, obj, instance, runner, running):
+def test_role_privileges(
+    ctx: Context, obj: Obj, instance: Instance, runner: CliRunner, running: MagicMock
+) -> None:
     with patch(
         "pglift.privileges.get",
         return_value=[
             interface.Privilege(
                 database="db2",
                 schema="public",
                 role="rol2",
@@ -752,15 +827,17 @@
             "role": "rol2",
             "object_type": "FUNCTION",
             "privileges": ["EXECUTE"],
         }
     ]
 
 
-def test_database_create(ctx, obj, instance, runner, running):
+def test_database_create(
+    ctx: Context, obj: Obj, instance: Instance, runner: CliRunner, running: MagicMock
+) -> None:
     with patch.object(databases, "exists", return_value=False) as exists, patch.object(
         databases, "apply"
     ) as apply:
         result = runner.invoke(
             cli,
             [
                 "database",
@@ -791,15 +868,17 @@
         )
     assert result.exit_code == 1
     assert "database already exists" in result.stderr
     exists.assert_called_once_with(ctx, instance, "db_test2")
     running.assert_called_once_with(ctx, instance)
 
 
-def test_database_alter(runner, ctx, obj, instance, running):
+def test_database_alter(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance, running: MagicMock
+) -> None:
     actual = interface.Database(name="alterme")
     altered = interface.Database(name="alterme", owner="dba")
 
     with patch.object(
         databases, "describe", return_value=actual
     ) as describe, patch.object(databases, "apply") as apply:
         result = runner.invoke(
@@ -814,22 +893,29 @@
             obj=obj,
         )
     describe.assert_called_once_with(ctx, instance, "alterme")
     apply.assert_called_once_with(ctx, instance, altered)
     assert result.exit_code == 0, result.output
 
 
-def test_database_schema(runner):
+def test_database_schema(runner: CliRunner) -> None:
     result = runner.invoke(cli, ["database", "schema"])
     schema = json.loads(result.output)
     assert schema["title"] == "Database"
     assert schema["description"] == "PostgreSQL database"
 
 
-def test_database_apply(runner, tmp_path, ctx, obj, instance, running):
+def test_database_apply(
+    runner: CliRunner,
+    tmp_path: Path,
+    ctx: Context,
+    obj: Obj,
+    instance: Instance,
+    running: MagicMock,
+) -> None:
     manifest = tmp_path / "manifest.yml"
     content = yaml.dump({"name": "dbtest"})
     manifest.write_text(content)
     with patch.object(databases, "apply") as apply:
         result = runner.invoke(
             cli,
             ["database", "apply", str(instance), "-f", str(manifest)],
@@ -841,15 +927,17 @@
     (call_ctx, call_instance, call_database), kwargs = apply.call_args
     assert call_ctx == ctx
     assert call_instance == instance
     assert call_database.name == "dbtest"
     assert kwargs == {}
 
 
-def test_database_describe(runner, ctx, obj, instance, running):
+def test_database_describe(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance, running: MagicMock
+) -> None:
     with patch.object(
         databases, "describe", side_effect=exceptions.DatabaseNotFound("absent")
     ) as describe:
         result = runner.invoke(
             cli,
             ["database", "describe", str(instance), "absent"],
             obj=obj,
@@ -874,15 +962,17 @@
     describe.assert_called_once_with(ctx, instance, "present")
     running.assert_called_once_with(ctx, instance)
     assert result.exit_code == 0
     described = yaml.safe_load(result.stdout)
     assert described == {"name": "present", "owner": "dba"}
 
 
-def test_database_list(runner, ctx, obj, instance, running):
+def test_database_list(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance, running: MagicMock
+) -> None:
     with patch.object(
         databases,
         "list",
         return_value=[
             interface.DetailedDatabase(
                 name="template1",
                 owner="postgres",
@@ -918,15 +1008,17 @@
             "owner": "postgres",
             "size": 8167939,
             "tablespace": {"location": "", "name": "pg_default", "size": 41011771},
         }
     ]
 
 
-def test_database_drop(runner, ctx, obj, instance, running):
+def test_database_drop(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance, running: MagicMock
+) -> None:
     with patch.object(
         databases, "drop", side_effect=exceptions.DatabaseNotFound("bar")
     ) as drop:
         result = runner.invoke(
             cli,
             ["database", "drop", str(instance), "foo"],
             obj=obj,
@@ -945,15 +1037,59 @@
             obj=obj,
         )
     drop.assert_called_once_with(ctx, instance, "foo")
     running.assert_called_once_with(ctx, instance)
     assert result.exit_code == 0
 
 
-def test_database_privileges(ctx, obj, instance, runner, running):
+def test_database_backup(
+    runner: CliRunner, ctx: Context, obj: Obj, instance: Instance, running: MagicMock
+) -> None:
+    output_file = "my/root/foo.dump"
+    with patch.object(
+        databases, "backup", side_effect=exceptions.DatabaseNotFound("bar")
+    ) as backup:
+        result = runner.invoke(
+            cli,
+            [
+                "database",
+                "backup",
+                str(instance),
+                "foo",
+                output_file,
+            ],
+            obj=obj,
+        )
+    backup.assert_called_once_with(ctx, instance, "foo", Path(output_file))
+    running.assert_called_once_with(ctx, instance)
+    assert result.exit_code == 1
+    assert "Error: database 'bar' not found" in result.stderr.strip()
+
+    running.reset_mock()
+
+    with patch.object(databases, "backup") as backup:
+        result = runner.invoke(
+            cli,
+            [
+                "database",
+                "backup",
+                str(instance),
+                "foo",
+                output_file,
+            ],
+            obj=obj,
+        )
+    backup.assert_called_once_with(ctx, instance, "foo", Path(output_file))
+    running.assert_called_once_with(ctx, instance)
+    assert result.exit_code == 0
+
+
+def test_database_privileges(
+    ctx: Context, obj: Obj, instance: Instance, runner: CliRunner, running: MagicMock
+) -> None:
     with patch(
         "pglift.privileges.get",
         return_value=[
             interface.Privilege(
                 database="db2",
                 schema="public",
                 role="rol2",
@@ -991,33 +1127,42 @@
     ]
 
 
 @pytest.mark.parametrize(
     ("action", "kwargs"),
     [("start", {"foreground": False}), ("stop", {})],
 )
-def test_postgres_exporter_start_stop(runner, ctx, obj, instance, action, kwargs):
+def test_postgres_exporter_start_stop(
+    runner: CliRunner,
+    ctx: Context,
+    obj: Obj,
+    instance: Instance,
+    action: str,
+    kwargs: Dict[str, bool],
+) -> None:
     with patch.object(prometheus, action) as patched:
         result = runner.invoke(
             cli,
             ["postgres_exporter", action, instance.qualname],
             obj=obj,
         )
     patched.assert_called_once_with(ctx, instance.qualname, **kwargs)
     assert result.exit_code == 0, result
 
 
-def test_postgres_exporter_schema(runner):
+def test_postgres_exporter_schema(runner: CliRunner) -> None:
     result = runner.invoke(cli, ["postgres_exporter", "schema"])
     schema = json.loads(result.output)
     assert schema["title"] == "PostgresExporter"
     assert schema["description"] == "Prometheus postgres_exporter service."
 
 
-def test_postgres_exporter_apply(runner, tmp_path, ctx, obj):
+def test_postgres_exporter_apply(
+    runner: CliRunner, tmp_path: Path, ctx: Context, obj: Obj
+) -> None:
     manifest = tmp_path / "manifest.yml"
     content = yaml.dump({"name": "123-exp", "dsn": "dbname=monitoring", "port": 123})
     manifest.write_text(content)
     with patch.object(prometheus, "apply") as apply:
         result = runner.invoke(
             cli,
             ["postgres_exporter", "apply", "-f", str(manifest)],
@@ -1026,29 +1171,29 @@
     assert result.exit_code == 0
     apply.assert_called_once_with(
         ctx,
         interface.PostgresExporter(name="123-exp", dsn="dbname=monitoring", port=123),
     )
 
 
-def test_postgres_exporter_install(runner, ctx, obj):
+def test_postgres_exporter_install(runner: CliRunner, ctx: Context, obj: Obj) -> None:
     with patch.object(prometheus, "apply") as apply:
         result = runner.invoke(
             cli,
             ["postgres_exporter", "install", "123-exp", "dbname=monitoring", "123"],
             obj=obj,
         )
     assert result.exit_code == 0
     apply.assert_called_once_with(
         ctx,
         interface.PostgresExporter(name="123-exp", dsn="dbname=monitoring", port=123),
     )
 
 
-def test_postgres_exporter_uninstall(runner, ctx, obj):
+def test_postgres_exporter_uninstall(runner: CliRunner, ctx: Context, obj: Obj) -> None:
     with patch.object(prometheus, "drop") as drop:
         result = runner.invoke(
             cli,
             ["postgres_exporter", "uninstall", "123-exp"],
             obj=obj,
         )
     assert result.exit_code == 0
```

### Comparing `pglift-0.8.0/tests/unit/test_cmd.py` & `pglift-0.9.0/tests/unit/test_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pytest
 
 from pglift import cmd
 from pglift.exceptions import CommandError, SystemError
 
 
-def test_execute_program(caplog, tmp_path):
+def test_execute_program(caplog: pytest.LogCaptureFixture, tmp_path: Path) -> None:
     command = ["/c", "m", "d"]
     with patch("os.execve") as execve, patch("os.execv") as execv:
         cmd.execute_program(command, env={"X": "Y"})
         execve.assert_called_once_with("/c", command, {"X": "Y"})
         assert not execv.called
     logger = logging.getLogger(__name__)
     with patch("os.execve") as execve, patch("os.execv") as execv, caplog.at_level(
@@ -21,15 +21,17 @@
     ):
         cmd.execute_program(command, logger=logger)
         execv.assert_called_once_with("/c", command)
         assert not execve.called
     assert "executing program /c m d" in caplog.records[0].message
 
 
-def test_start_program_terminate_program_status_program(caplog, tmp_path):
+def test_start_program_terminate_program_status_program(
+    caplog: pytest.LogCaptureFixture, tmp_path: Path
+) -> None:
     logger = logging.getLogger(__name__)
 
     pidfile = tmp_path / "sleep" / "pid"
     cmd.start_program(
         ["sleep", "10"], pidfile, timeout=0.01, env={"X_DEBUG": "1"}, logger=logger
     )
     with pidfile.open() as f:
```

### Comparing `pglift-0.8.0/tests/unit/test_conf.py` & `pglift-0.9.0/tests/unit/test_conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from pathlib import Path
+from typing import Any, Tuple
 
 import pytest
 
 from pglift import conf
+from pglift.models.system import Instance
+from pglift.settings import Settings
 
 
-def test_read(pg_version, settings, tmp_path):
+def test_read(pg_version: str, settings: Settings, tmp_path: Path) -> None:
     datadir = tmp_path
     (datadir / "postgresql.auto.conf").touch()
     postgresql_conf = datadir / "postgresql.conf"
     postgresql_conf.touch()
     postgresql_conf.write_text("\n".join(["bonjour = hello", "port=1234"]))
 
     config = conf.read(tmp_path)
@@ -23,24 +26,26 @@
     user_conf.write_text("\n".join(["port=5555"]))
     mconf = conf.read(datadir, True)
     assert mconf is not None
     assert mconf.port == 5555
 
 
 @pytest.fixture(params=["relative", "absolute"])
-def log_directory(instance, request, tmp_path):
+def log_directory(
+    instance: Instance, request: Any, tmp_path: Path
+) -> Tuple[Path, Path]:
     if request.param == "relative":
         path = Path("loghere")
         return path, instance.datadir / path
-    elif request.param == "absolute":
+    else:
         path = tmp_path / "log" / "here"
         return path, path
 
 
-def test_log_directory(instance, log_directory):
+def test_log_directory(instance: Instance, log_directory: Tuple[Path, Path]) -> None:
     log_dir, abs_log_dir = log_directory
     assert not abs_log_dir.exists()
     conf.create_log_directory(instance, log_dir)
     assert abs_log_dir.exists()
     conf.remove_log_directory(instance, log_dir)
     assert not abs_log_dir.exists()
     assert abs_log_dir.parent.exists()
```

### Comparing `pglift-0.8.0/tests/unit/test_db.py` & `pglift-0.9.0/tests/unit/test_db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import json
+from pathlib import Path
+from typing import Dict
 from unittest.mock import patch
 
 import psycopg2.extras
 import pytest
 from psycopg2 import sql
 
 from pglift import db
+from pglift.models.system import Instance
+from pglift.settings import Settings
 
 
-def test_queries(datadir, regen_test_data):
+def test_queries(datadir: Path, regen_test_data: bool) -> None:
     actual = dict(db.queries())
     fpath = datadir / "queries.json"
     if regen_test_data:
         with fpath.open("w") as f:
             json.dump(actual, f, indent=2, sort_keys=True)
     expected = json.loads(fpath.read_text())
     assert actual == expected
 
 
-def test_query():
+def test_query() -> None:
     query = db.query("role_alter_password", username=sql.Identifier("bob"))
     qs = "".join(q.string for q in query.seq)
     assert qs == "ALTER ROLE bob PASSWORD %(password)s;"
 
 
 @pytest.mark.parametrize(
     "connargs, expected",
@@ -33,26 +37,28 @@
         ),
         (
             {"user": "alice", "password": "s3kret"},
             "dbname=mydb sslmode=off user=alice password=s3kret port=999 host=/socks passfile={passfile}",
         ),
     ],
 )
-def test_dsn(settings, instance, connargs, expected):
+def test_dsn(
+    settings: Settings, instance: Instance, connargs: Dict[str, str], expected: str
+) -> None:
     passfile = settings.postgresql.auth.passfile
     conninfo = db.dsn(instance, dbname="mydb", sslmode="off", **connargs)
     assert conninfo == expected.format(passfile=passfile)
 
 
-def test_dsn_badarg(instance):
+def test_dsn_badarg(instance: Instance) -> None:
     with pytest.raises(TypeError, match="unexpected 'port' argument"):
         db.dsn(instance, port=123)
 
 
-def test_connect(instance, settings):
+def test_connect(instance: Instance, settings: Settings) -> None:
     with patch("psycopg2.connect") as connect:
         cnx = db.connect(instance, user="dba")
         assert not connect.called
         with cnx:
             pass
     passfile = settings.postgresql.auth.passfile
     assert passfile.exists()
```

### Comparing `pglift-0.8.0/tests/unit/test_instance.py` & `pglift-0.9.0/tests/unit/test_instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,47 @@
+import os
 import pathlib
 import re
 from unittest.mock import patch
 
 import pytest
 from pgtoolkit.conf import parse as parse_pgconf
 
 from pglift import instance as instance_mod
 from pglift import task
+from pglift.ctx import Context
 from pglift.exceptions import CommandError, InstanceStateError
 from pglift.models import interface
-from pglift.models.system import BaseInstance
+from pglift.models.system import BaseInstance, Instance
+from pglift.settings import Settings
 
 
-def test_systemd_unit(pg_version, instance):
+def test_systemd_unit(pg_version: str, instance: Instance) -> None:
     assert (
         instance_mod.systemd_unit(instance)
         == f"pglift-postgresql@{pg_version}-test.service"
     )
 
 
-def test_init_lookup_failed(pg_version, settings, ctx):
+def test_init_lookup_failed(pg_version: str, settings: Settings, ctx: Context) -> None:
     manifest = interface.Instance(name="dirty", version=pg_version)
     i = BaseInstance("dirty", pg_version, settings)
     i.datadir.mkdir(parents=True)
     (i.datadir / "postgresql.conf").touch()
-    pg_version = i.datadir / "PG_VERSION"
-    pg_version.write_text("7.1")
+    pg_version_file = i.datadir / "PG_VERSION"
+    pg_version_file.write_text("7.1")
     with pytest.raises(Exception, match="version mismatch"):
         with task.Runner(ctx):
             instance_mod.init(ctx, manifest)
-    assert not pg_version.exists()  # per revert
+    assert not pg_version_file.exists()  # per revert
 
 
-def test_init_dirty(pg_version, settings, ctx, monkeypatch):
+def test_init_dirty(
+    pg_version: str, settings: Settings, ctx: Context, monkeypatch: pytest.MonkeyPatch
+) -> None:
     manifest = interface.Instance(name="dirty", version=pg_version)
     i = BaseInstance("dirty", pg_version, settings)
     i.datadir.mkdir(parents=True)
     (i.datadir / "dirty").touch()
     calls = []
     with pytest.raises(CommandError):
         with task.Runner(ctx):
@@ -45,45 +50,47 @@
                 instance_mod.init(ctx, manifest)
     assert not i.datadir.exists()  # XXX: not sure this is a sane thing to do?
     assert not i.waldir.exists()
     if ctx.settings.service_manager == "systemd":
         assert not calls
 
 
-def test_init_version_not_available(ctx):
+def test_init_version_not_available(ctx: Context) -> None:
     settings = ctx.settings
     version = "11"
     if pathlib.Path(settings.postgresql.bindir.format(version=version)).exists():
         pytest.skip(f"PostgreSQL {version} seems available")
     manifest = interface.Instance(name=f"pg{version}", version=version)
     with pytest.raises(EnvironmentError, match="pg_ctl executable not found"):
         instance_mod.init(ctx, manifest)
 
 
-def test_list_no_pgroot(ctx):
+def test_list_no_pgroot(ctx: Context) -> None:
     assert not ctx.settings.postgresql.root.exists()
     assert list(instance_mod.list(ctx)) == []
 
 
 @pytest.fixture
-def ctx_nohook(ctx):
+def ctx_nohook(ctx: Context) -> Context:
     ctx.pm.unregister_all()
     return ctx
 
 
-def test_configure(ctx_nohook, instance):
+def test_configure(
+    ctx_nohook: Context, instance: Instance, instance_manifest: interface.Instance
+) -> None:
     ctx = ctx_nohook
     configdir = instance.datadir
     postgresql_conf = configdir / "postgresql.conf"
     with postgresql_conf.open("w") as f:
         f.write("bonjour_name = 'test'\n")
 
     changes = instance_mod.configure(
         ctx,
-        instance,
+        instance_manifest,
         port=5433,
         max_connections=100,
         shared_buffers="10 %",
         effective_cache_size="5MB",
     )
     old_shared_buffers, new_shared_buffers = changes.pop("shared_buffers")
     assert old_shared_buffers is None
@@ -113,15 +120,15 @@
     with postgresql_conf.open() as f:
         config = parse_pgconf(f)
     assert config.port == 5433
     assert config.bonjour_name == "test"
     assert config.cluster_name == "test"
 
     changes = instance_mod.configure(
-        ctx, instance, listen_address="*", ssl=True, port=None
+        ctx, instance_manifest, listen_address="*", ssl=True, port=None
     )
     assert changes == {
         "effective_cache_size": ("5MB", None),
         "listen_address": (None, "*"),
         "max_connections": (100, None),
         "port": (5433, None),
         "shared_buffers": (new_shared_buffers, None),
@@ -129,90 +136,94 @@
     }
     # Same configuration, no change.
     mtime_before = (
         postgresql_conf.stat().st_mtime,
         site_configfpath.stat().st_mtime,
         user_configfpath.stat().st_mtime,
     )
-    changes = instance_mod.configure(ctx, instance, listen_address="*", ssl=True)
+    changes = instance_mod.configure(
+        ctx, instance_manifest, listen_address="*", ssl=True
+    )
     assert changes == {}
     mtime_after = (
         postgresql_conf.stat().st_mtime,
         site_configfpath.stat().st_mtime,
         user_configfpath.stat().st_mtime,
     )
     assert mtime_before == mtime_after
 
-    changes = instance_mod.configure(ctx, instance, ssl=True)
+    changes = instance_mod.configure(ctx, instance_manifest, ssl=True)
     lines = user_configfpath.read_text().splitlines()
     assert "ssl = on" in lines
     assert (configdir / "server.crt").exists()
     assert (configdir / "server.key").exists()
 
     ssl = (cert_file, key_file) = (
         instance.datadir / "c.crt",
         instance.datadir / "k.key",
     )
     for fpath in ssl:
         fpath.touch()
-    changes = instance_mod.configure(ctx, instance, ssl=ssl)
+    changes = instance_mod.configure(ctx, instance_manifest, ssl=ssl)
     assert changes == {
-        "ssl_cert_file": (None, cert_file),
-        "ssl_key_file": (None, key_file),
+        "ssl_cert_file": (None, str(cert_file)),
+        "ssl_key_file": (None, str(key_file)),
     }
     lines = user_configfpath.read_text().splitlines()
     assert "ssl = on" in lines
-    assert f"ssl_cert_file = {instance.datadir / 'c.crt'}" in lines
-    assert f"ssl_key_file = {instance.datadir / 'k.key'}" in lines
+    assert f"ssl_cert_file = '{instance.datadir / 'c.crt'}'" in lines
+    assert f"ssl_key_file = '{instance.datadir / 'k.key'}'" in lines
     for fpath in ssl:
         assert fpath.exists()
 
     # reconfigure default ssl certs
-    changes = instance_mod.configure(ctx, instance, ssl=True)
+    changes = instance_mod.configure(ctx, instance_manifest, ssl=True)
     assert changes == {
         "ssl_cert_file": (str(cert_file), None),
         "ssl_key_file": (str(key_file), None),
     }
 
     # disable ssl
-    changes = instance_mod.configure(ctx, instance, ssl=False)
+    changes = instance_mod.configure(ctx, instance_manifest, ssl=False)
     assert changes == {
         "ssl": (True, None),
     }
 
 
-def test_check_status(ctx, instance):
+def test_check_status(ctx: Context, instance: Instance) -> None:
     with pytest.raises(InstanceStateError, match="instance is not_running"):
         instance_mod.check_status(ctx, instance, instance_mod.Status.running)
     instance_mod.check_status(ctx, instance, instance_mod.Status.not_running)
 
 
-def test_start_foreground(ctx, instance):
+def test_start_foreground(ctx: Context, instance: Instance) -> None:
     with patch("os.execv") as execv:
         instance_mod.start(ctx, instance, foreground=True)
     postgres = ctx.pg_ctl(instance.version).bindir / "postgres"
     execv.assert_called_once_with(
         str(postgres), f"{postgres} -D {instance.datadir}".split()
     )
 
 
-def test_shell(ctx, instance):
-    with patch("os.execv") as patched:
+def test_shell(ctx: Context, instance: Instance) -> None:
+    with patch("os.execve") as patched:
         instance_mod.shell(ctx, instance, user="test", dbname="test")
     psql = str(ctx.pg_ctl(instance.version).bindir / "psql")
     cmd = [
         psql,
         "--port",
         str(instance.port),
         "--host",
         "/socks",
         "--user",
         "test",
         "--dbname",
         "test",
     ]
-    patched.assert_called_once_with(psql, cmd)
+    expected_env = os.environ.copy()
+    expected_env["PGPASSFILE"] = str(ctx.settings.postgresql.auth.passfile)
+    patched.assert_called_once_with(psql, cmd, expected_env)
 
 
-def test_exists(ctx, instance):
+def test_exists(ctx: Context, instance: Instance) -> None:
     assert instance_mod.exists(ctx, instance.name, instance.version)
     assert not instance_mod.exists(ctx, "doesnotexists", instance.version)
```

### Comparing `pglift-0.8.0/tests/unit/test_models_helpers.py` & `pglift-0.9.0/tests/unit/test_models_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import enum
 import json
 from datetime import datetime
-from typing import Any, List, Optional
+from pathlib import Path
+from typing import Any, List, Optional, Type
 
 import click
 import pytest
 from click.testing import CliRunner
 from pydantic import BaseModel, Field, SecretStr
 
 from pglift.models import helpers, interface
@@ -57,15 +58,15 @@
     address: Optional[Address]
     dob: Optional[datetime] = Field(alias="birthdate", description="date of birth")
 
     class Config:
         extra = "forbid"
 
 
-def test_parameters_from_model_typeerror():
+def test_parameters_from_model_typeerror() -> None:
     with pytest.raises(TypeError, match="expecting a 'person: Person' parameter"):
 
         @click.command("add-person")
         @helpers.parameters_from_model(Person)
         @click.pass_context
         def cb1(ctx: click.core.Context, x: Person) -> None:
             pass
@@ -75,15 +76,15 @@
         @click.command("add-person")
         @helpers.parameters_from_model(Person)
         @click.pass_context
         def cb2(ctx: click.core.Context, person: str) -> None:
             pass
 
 
-def test_parameters_from_model():
+def test_parameters_from_model() -> None:
     @click.command("add-person")
     @click.option("--sort-keys", is_flag=True, default=False)
     @helpers.parameters_from_model(Person)
     @click.option("--indent", type=int)
     @click.pass_context
     def add_person(
         ctx: click.core.Context, sort_keys: bool, person: Person, indent: int
@@ -149,15 +150,15 @@
         "dob": "1981-02-18T01:02:00",
         "gender": "F",
         "name": "alice",
         "nickname": "**********",
     }
 
 
-def test_parameters_from_model_no_parse():
+def test_parameters_from_model_no_parse() -> None:
     @click.command("add-person")
     @helpers.parameters_from_model(Person, parse_model=False)
     @click.pass_context
     def add_person(ctx: click.core.Context, **values: Any) -> None:
         click.echo(json.dumps(values))
 
     runner = CliRunner()
@@ -183,15 +184,15 @@
         "age": "42",
         "birthdate": "1981-02-18T01:02",
         "gender": "F",
         "name": "alice",
     }
 
 
-def test_unnest():
+def test_unnest() -> None:
     params = {
         "name": "alice",
         "age": 42,
         "gender": "F",
         "address_city": "paris",
         "address_country": "fr",
         "address_street": ["bd montparnasse"],
@@ -213,15 +214,15 @@
 
     with pytest.raises(ValueError, match="invalid"):
         helpers.unnest(Person, {"age": None, "invalid": "value"})
     with pytest.raises(ValueError, match="in_va_lid"):
         helpers.unnest(Person, {"age": None, "in_va_lid": "value"})
 
 
-def test_parse_params_as():
+def test_parse_params_as() -> None:
     address_params = {
         "city": "paris",
         "country": "fr",
         "street": ["bd montparnasse"],
         "zip_code": 0,
         "shared": True,
     }
@@ -253,15 +254,15 @@
         "age": 42,
         "gender": "F",
     }
     params_nested.update({f"address_{k}": v for k, v in address_params.items()})
     assert helpers.parse_params_as(Person, params_nested) == person
 
 
-def test_argspec_from_model():
+def test_argspec_from_model() -> None:
     argspec = helpers.argspec_from_model(Person)
     assert argspec == {
         "name": {"required": True, "type": "str"},
         "nickname": {"no_log": True, "type": "str"},
         "gender": {"choices": ["M", "F"]},
         "age": {"type": "int", "description": ["age"]},
         "birthdate": {"description": ["date of birth"]},
@@ -278,15 +279,15 @@
         "address_primary": {
             "type": "bool",
             "description": ["is this person's primary address?"],
         },
     }
 
 
-def test_argspec_from_model_nested_optional():
+def test_argspec_from_model_nested_optional() -> None:
     """An optional nested model should propagate non-required on all nested models."""
 
     class Sub(BaseModel):
         f: int
 
     class Nested(BaseModel):
         s: Sub
@@ -299,15 +300,15 @@
         n: Optional[Nested]
 
     assert helpers.argspec_from_model(Model) == {
         "n_s_f": {"type": "int"},
     }
 
 
-def test_argspec_from_model_nested_default():
+def test_argspec_from_model_nested_default() -> None:
     """A default value on a optional nested model should not be set as "default" in ansible"""
 
     class Nested(BaseModel):
         r: int
         d: int = 42
 
     class Model(BaseModel):
@@ -315,15 +316,15 @@
 
     assert helpers.argspec_from_model(Model) == {
         "n_r": {"type": "int"},
         "n_d": {"type": "int"},
     }
 
 
-def test_argspec_from_model_keep_default():
+def test_argspec_from_model_keep_default() -> None:
     """A non-required field with a default value should keep the "default" in ansible"""
 
     class Nested(BaseModel):
         f: int = 42
 
     class Model(BaseModel):
         n: Nested = Nested()
@@ -338,14 +339,16 @@
     [
         interface.Instance,
         interface.PostgresExporter,
         interface.Role,
         interface.Database,
     ],
 )
-def test_argspec_from_model_manifest(datadir, regen_test_data, manifest_type):
+def test_argspec_from_model_manifest(
+    datadir: Path, regen_test_data: bool, manifest_type: Type[interface.Manifest]
+) -> None:
     actual = helpers.argspec_from_model(manifest_type)
     fpath = datadir / f"ansible-argspec-{manifest_type.__name__.lower()}.json"
     if regen_test_data:
         fpath.write_text(json.dumps(actual, indent=2, sort_keys=True))
     expected = json.loads(fpath.read_text())
     assert actual == expected
```

### Comparing `pglift-0.8.0/tests/unit/test_models_interface.py` & `pglift-0.9.0/tests/unit/test_models_interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 
 class Point(interface.Manifest):
     x: float
     y: float
 
 
-def test_parse_yaml():
+def test_parse_yaml() -> None:
     stream = io.StringIO()
     yaml.dump({"x": 1.2, "y": 3.4}, stream)
     stream.seek(0)
     point = Point.parse_yaml(stream)
     assert point == Point(x=1.2, y=3.4)
 
 
-def test_yaml():
+def test_yaml() -> None:
     point = Point(x=0, y=1.2)
     s = point.yaml()
     assert s == "x: 0.0\ny: 1.2\n"
 
 
-def test_postgresexporter():
+def test_postgresexporter() -> None:
     m = interface.PostgresExporter(name="12-x", dsn="dbname=postgres", port=9876)
     assert m.dsn == "dbname=postgres"
     with pytest.raises(pydantic.ValidationError):
         interface.PostgresExporter(dsn="x=y", port=9876)
```

### Comparing `pglift-0.8.0/tests/unit/test_models_system.py` & `pglift-0.9.0/tests/unit/test_models_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,116 @@
 import pytest
 
 from pglift import exceptions
+from pglift.ctx import Context
 from pglift.models import system
+from pglift.models.system import Instance
+from pglift.settings import Settings
 
 
-def test_default_postgresql_version(pg_version, ctx, monkeypatch):
+def test_default_postgresql_version(
+    pg_version: str, ctx: Context, monkeypatch: pytest.MonkeyPatch
+) -> None:
     major_version = pg_version[:2]
     assert system.default_postgresql_version(ctx) == major_version
 
     new_settings = ctx.settings.copy(
         update={
             "postgresql": ctx.settings.postgresql.copy(update={"default_version": "42"})
         }
     )
     with monkeypatch.context() as m:
         m.setattr(ctx, "settings", new_settings)
         assert system.default_postgresql_version(ctx) == "42"
 
 
-def test_baseinstance_str(pg_version, instance):
+def test_baseinstance_str(pg_version: str, instance: Instance) -> None:
     assert str(instance) == f"{pg_version}/test"
 
 
-def test_baseinstance_qualname(pg_version, instance):
+def test_baseinstance_qualname(pg_version: str, instance: Instance) -> None:
     assert instance.qualname == f"{pg_version}-test"
 
 
 @pytest.mark.parametrize(
     ["attrname", "expected_suffix"],
     [
         ("path", "srv/pgsql/{version}/test"),
         ("datadir", "srv/pgsql/{version}/test/data"),
         ("waldir", "srv/pgsql/{version}/test/wal"),
     ],
 )
-def test_baseinstance_paths(pg_version, instance, attrname, expected_suffix):
+def test_baseinstance_paths(
+    pg_version: str, instance: Instance, attrname: str, expected_suffix: str
+) -> None:
     path = getattr(instance, attrname)
     assert path.match(expected_suffix.format(version=pg_version))
 
 
-def test_baseinstance_get(ctx):
+def test_baseinstance_get(ctx: Context) -> None:
     i = system.BaseInstance.get("test", None, ctx=ctx)
     major_version = str(ctx.pg_ctl(None).version)[:2]
     assert i.version == major_version
 
 
-def test_postgresqlinstance_system_lookup(ctx, instance):
+def test_postgresqlinstance_system_lookup(ctx: Context, instance: Instance) -> None:
     i = system.PostgreSQLInstance.system_lookup(ctx, instance)
     expected = system.PostgreSQLInstance(
         instance.name, instance.version, instance.settings
     )
     assert i == expected
 
     i = system.PostgreSQLInstance.system_lookup(ctx, (instance.name, instance.version))
     assert i == expected
 
     with pytest.raises(TypeError, match="expecting either a BaseInstance or"):
         system.PostgreSQLInstance.system_lookup(ctx, ("nameonly",))  # type: ignore[arg-type]
 
 
-def test_instance_system_lookup(ctx, instance):
+def test_instance_system_lookup(ctx: Context, instance: Instance) -> None:
     i = system.Instance.system_lookup(ctx, instance)
     assert i == instance
 
     i = system.Instance.system_lookup(ctx, (instance.name, instance.version))
     assert i == instance
 
 
-def test_instance_system_lookup_misconfigured(ctx, instance):
+def test_instance_system_lookup_misconfigured(ctx: Context, instance: Instance) -> None:
     (instance.datadir / "postgresql.conf").unlink()
     with pytest.raises(exceptions.InstanceNotFound, match=str(instance)):
         system.Instance.system_lookup(ctx, instance)
 
 
-def test_postgresqlinstance_exists(pg_version, settings):
+def test_postgresqlinstance_exists(pg_version: str, settings: Settings) -> None:
     instance = system.PostgreSQLInstance(
         name="exists", version=pg_version, settings=settings
     )
     with pytest.raises(exceptions.InstanceNotFound):
         instance.exists()
     instance.datadir.mkdir(parents=True)
     (instance.datadir / "PG_VERSION").write_text(pg_version)
     with pytest.raises(exceptions.InstanceNotFound):
         instance.exists()
     (instance.datadir / "postgresql.conf").touch()
     assert instance.exists()
 
 
-def test_postgresqlinstance_port(instance):
+def test_postgresqlinstance_port(instance: Instance) -> None:
     assert instance.port == 999
 
 
-def test_postgresqlinstance_config(instance):
+def test_postgresqlinstance_config(instance: Instance) -> None:
     config = instance.config()
     assert config.port == 999
     assert config.unix_socket_directories == "/socks"
 
     assert not instance.config(managed_only=True).as_dict()
 
 
-def test_postgresqlinstance_standby_for(ctx, instance):
+def test_postgresqlinstance_standby_for(ctx: Context, instance: Instance) -> None:
     (instance.datadir / "postgresql.auto.conf").write_text(
         "primary_conninfo = host=/tmp port=4242 user=pg\n"
     )
     assert not instance.standby
     standbyfile = "standby.signal" if int(instance.version) >= 12 else "recovery.conf"
     (instance.datadir / standbyfile).touch()
     assert instance.standby
```

### Comparing `pglift-0.8.0/tests/unit/test_pgbackrest.py` & `pglift-0.9.0/tests/unit/test_pgbackrest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from datetime import datetime, timezone
 from unittest.mock import patch
 
 from pglift import pgbackrest
+from pglift.ctx import Context
+from pglift.models.system import Instance
+from pglift.settings import Settings
 
 
-def test_make_cmd(pg_version, settings, instance):
+def test_make_cmd(pg_version: str, settings: Settings, instance: Instance) -> None:
     assert pgbackrest.make_cmd(instance, settings.pgbackrest, "stanza-upgrade") == [
         "/usr/bin/pgbackrest",
         f"--config={settings.prefix}/etc/pgbackrest/pgbackrest-{pg_version}-test.conf",
         f"--stanza={pg_version}-test",
         "stanza-upgrade",
     ]
 
 
-def test_backup_info(ctx, settings, pg_version, instance):
+def test_backup_info(
+    ctx: Context, settings: Settings, pg_version: str, instance: Instance
+) -> None:
     with patch.object(ctx, "run") as run:
         run.return_value.stdout = "[]"
         assert pgbackrest.backup_info(ctx, instance, backup_set="foo") == []
     run.assert_called_once_with(
         [
             "/usr/bin/pgbackrest",
             f"--config={settings.prefix}/etc/pgbackrest/pgbackrest-{pg_version}-test.conf",
@@ -26,37 +31,43 @@
             "--output=json",
             "info",
         ],
         check=True,
     )
 
 
-def test_backup_command(pg_version, settings, instance):
+def test_backup_command(
+    pg_version: str, settings: Settings, instance: Instance
+) -> None:
     assert pgbackrest.backup_command(instance, type=pgbackrest.BackupType.full) == [
         "/usr/bin/pgbackrest",
         f"--config={settings.prefix}/etc/pgbackrest/pgbackrest-{pg_version}-test.conf",
         f"--stanza={pg_version}-test",
         "--type=full",
         "--log-level-console=info",
         "--start-fast",
         "backup",
     ]
 
 
-def test_expire_command(pg_version, settings, instance):
+def test_expire_command(
+    pg_version: str, settings: Settings, instance: Instance
+) -> None:
     assert pgbackrest.expire_command(instance) == [
         "/usr/bin/pgbackrest",
         f"--config={settings.prefix}/etc/pgbackrest/pgbackrest-{pg_version}-test.conf",
         f"--stanza={pg_version}-test",
         "--log-level-console=info",
         "expire",
     ]
 
 
-def test_restore_command(pg_version, settings, instance):
+def test_restore_command(
+    pg_version: str, settings: Settings, instance: Instance
+) -> None:
     assert pgbackrest.restore_command(
         instance, date=datetime(2003, 1, 1).replace(tzinfo=timezone.utc), backup_set="x"
     ) == [
         "/usr/bin/pgbackrest",
         f"--config={settings.prefix}/etc/pgbackrest/pgbackrest-{pg_version}-test.conf",
         f"--stanza={pg_version}-test",
         "--log-level-console=info",
```

### Comparing `pglift-0.8.0/tests/unit/test_postgres.py` & `pglift-0.9.0/tests/unit/test_postgres.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import subprocess
+from typing import Any, List, NoReturn
 
 import pytest
 
 from pglift import postgres
+from pglift.ctx import Context
+from pglift.models.system import Instance
 
 
-def test_main_errors():
+def test_main_errors() -> None:
     with pytest.raises(SystemExit, match="2"):
         postgres.main(["aa"])
     with pytest.raises(SystemExit, match="2"):
         postgres.main(["12-"])
     with pytest.raises(SystemExit, match="2"):
         postgres.main(["12-test"])
 
 
-def test_main(monkeypatch, ctx, instance):
+def test_main(
+    monkeypatch: pytest.MonkeyPatch, ctx: Context, instance: Instance
+) -> None:
     calls = []
 
     class Popen:
-        def __init__(self, cmd, **kwargs):
+        def __init__(self, cmd: List[str], **kwargs: Any):
             calls.append(cmd)
             self.cmd = cmd
             self.pid = 123
             self.returncode = 0
 
-        def communicate(self, **kwargs):
+        def communicate(self, **kwargs: Any) -> NoReturn:
             raise subprocess.TimeoutExpired(self.cmd, 12)
 
     with monkeypatch.context() as m:
         m.setattr("subprocess.Popen", Popen)
         postgres.main([f"{instance.version}-{instance.name}"], ctx=ctx)
     bindir = ctx.settings.postgresql.versions[instance.version].bindir
     assert calls == [[str(bindir / "postgres"), "-D", str(instance.datadir)]]
```

### Comparing `pglift-0.8.0/tests/unit/test_prometheus.py` & `pglift-0.9.0/tests/unit/test_prometheus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import pathlib
 
 import pytest
 
 from pglift import exceptions, prometheus
+from pglift.ctx import Context
 from pglift.models import interface
+from pglift.models.system import Instance
 
 
-def test_systemd_unit(pg_version, instance):
+def test_systemd_unit(pg_version: str, instance: Instance) -> None:
     assert (
         prometheus.systemd_unit(instance.qualname)
         == f"pglift-postgres_exporter@{pg_version}-test.service"
     )
 
 
-def test_port(ctx, instance):
+def test_port(ctx: Context, instance: Instance) -> None:
     port = prometheus.port(ctx, instance.qualname)
     assert port == 9817
 
     configpath = pathlib.Path(
         str(ctx.settings.prometheus.configpath).format(name=instance.qualname)
     )
     configpath.write_text("\nempty\n")
@@ -27,11 +29,11 @@
     configpath.write_text("\nPG_EXPORTER_WEB_LISTEN_ADDRESS=42\n")
     with pytest.raises(
         LookupError, match="malformatted PG_EXPORTER_WEB_LISTEN_ADDRESS"
     ):
         prometheus.port(ctx, instance.qualname)
 
 
-def test_apply(ctx, instance):
+def test_apply(ctx: Context, instance: Instance) -> None:
     m = interface.PostgresExporter(name=instance.qualname, dsn="", port=123)
     with pytest.raises(exceptions.InstanceStateError, match="exists locally"):
         prometheus.apply(ctx, m)
```

### Comparing `pglift-0.8.0/tests/unit/test_roles.py` & `pglift-0.9.0/tests/unit/test_roles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import datetime
+from pathlib import Path
 from typing import Optional
 
 import pytest
 from psycopg2 import sql
 from pydantic import SecretStr
 
 from pglift import roles
+from pglift.ctx import Context
 from pglift.models import interface
+from pglift.models.system import Instance
 
 
 @pytest.mark.parametrize("with_password", [True, False])
-def test_options_and_args(with_password):
+def test_options_and_args(with_password: bool) -> None:
     role = interface.Role(
         name="r",
         password="skret",
         inherit=False,
         login=True,
         connection_limit=2,
         validity=datetime.datetime(2024, 1, 1),
@@ -51,31 +54,33 @@
         "validity": "2024-01-01T00:00:00",
     }
     if with_password:
         expected_args["password"] = "skret"
     assert args == expected_args
 
 
-class Role:
+class Role(interface.Role):
     def __init__(
         self, name: str, password: Optional[str] = None, pgpass: bool = False
     ) -> None:
-        self.name = name
-        self.password = SecretStr(password) if password is not None else None
-        self.pgpass = pgpass
+        super().__init__(
+            name=name,
+            password=SecretStr(password) if password is not None else None,
+            pgpass=pgpass,
+        )
 
 
 @pytest.fixture
-def passfile(ctx):
+def passfile(ctx: Context) -> Path:
     fpath = ctx.settings.postgresql.auth.passfile
     fpath.write_text("*:999:*:edgar:fbi\n")
     return fpath
 
 
-def test_in_pgpass(ctx, instance, passfile):
+def test_in_pgpass(ctx: Context, instance: Instance, passfile: Path) -> None:
     assert roles.in_pgpass(ctx, instance, "edgar")
     assert not roles.in_pgpass(ctx, instance, "alice")
 
 
 @pytest.mark.parametrize(
     "role, pgpass",
     [
@@ -83,10 +88,12 @@
         (Role("bob", "secret"), "*:999:*:edgar:fbi\n"),
         (Role("charles", pgpass=True), "*:999:*:edgar:fbi\n"),
         (Role("danny", "sss", True), "*:999:*:danny:sss\n*:999:*:edgar:fbi\n"),
         (Role("edgar", "fbi", True), "*:999:*:edgar:fbi\n"),
         (Role("edgar", None, False), ""),
     ],
 )
-def test_set_pgpass_entry_for(ctx, instance, passfile, role, pgpass):
+def test_set_pgpass_entry_for(
+    ctx: Context, instance: Instance, passfile: Path, role: Role, pgpass: str
+) -> None:
     roles.set_pgpass_entry_for(ctx, instance, role)
     assert passfile.read_text() == pgpass
```

### Comparing `pglift-0.8.0/tests/unit/test_settings.py` & `pglift-0.9.0/tests/unit/test_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 import pytest
 from pydantic import ValidationError
 
 from pglift.settings import DataPath, Settings
 
 
-def test_json_config_settings_source(monkeypatch, tmp_path):
+def test_json_config_settings_source(
+    monkeypatch: pytest.MonkeyPatch, tmp_path: Path
+) -> None:
     settings = tmp_path / "settings.json"
     settings.write_text('{"postgresql": {"root": "/mnt/postgresql"}}')
     with monkeypatch.context() as m:
         m.setenv("SETTINGS", f"@{settings}")
         s = Settings()
     assert s.postgresql.root == Path("/mnt/postgresql")
     with monkeypatch.context() as m:
@@ -21,29 +23,29 @@
     assert s.postgresql.root == Path("/data/postgres")
     with monkeypatch.context() as m:
         m.setenv("SETTINGS", f"@{tmp_path / 'notfound'}")
         with pytest.raises(FileNotFoundError):
             Settings()
 
 
-def test_yaml_settings(tmp_path, monkeypatch):
+def test_yaml_settings(tmp_path: Path, monkeypatch: pytest.MonkeyPatch) -> None:
     (tmp_path / "settings.yaml").write_text("prefix: /tmp")
     with monkeypatch.context() as m:
         m.setattr("pglift.settings.datapath", tmp_path)
         s = Settings()
     assert str(s.prefix) == "/tmp"
 
     (tmp_path / "settings.yaml").write_text("hello")
     with monkeypatch.context() as m:
         m.setattr("pglift.settings.datapath", tmp_path)
         with pytest.raises(TypeError, match="expecting an object"):
             Settings()
 
 
-def test_settings(tmp_path):
+def test_settings(tmp_path: Path) -> None:
     s = Settings(prefix="/")
     assert hasattr(s, "postgresql")
     assert hasattr(s.postgresql, "root")
     assert s.postgresql.root == Path("/srv/pgsql")
     assert s.logpath == Path("/log")
 
     with pytest.raises(Exception) as e:
@@ -56,15 +58,15 @@
             "postgresql": {"root": str(tmp_path), "pid_directory": "pgsql"},
         }
     )
     assert s.postgresql.root == tmp_path
     assert str(s.postgresql.pid_directory) == "/prefix/run/pgsql"
 
 
-def test_postgresql_versions(monkeypatch, tmp_path):
+def test_postgresql_versions(monkeypatch: pytest.MonkeyPatch, tmp_path: Path) -> None:
     config = {
         "postgresql": {
             "bindir": "/usr/lib/pgsql/{version}/bin",
             "versions": {
                 "10": {
                     "bindir": "/opt/pgsql-10/bin",
                 },
@@ -92,22 +94,22 @@
     config_path.write_text(json.dumps(config))
     with monkeypatch.context() as m:
         m.setenv("SETTINGS", f"@{config_path}")
         s = Settings()
     assert s.postgresql.default_version == "13"
 
 
-def test_systemd_systemctl():
+def test_systemd_systemctl() -> None:
     with patch("shutil.which", return_value=None) as which:
         with pytest.raises(ValidationError, match="systemctl command not found"):
             Settings(service_manager="systemd")
     which.assert_called_once_with("systemctl")
 
 
-def test_systemd_sudo_user():
+def test_systemd_sudo_user() -> None:
     with patch("shutil.which", return_value=True) as which:
         with pytest.raises(
             ValidationError, match="'user' mode cannot be used with 'sudo'"
         ):
             Settings.parse_obj(
                 {"service_manager": "systemd", "systemd": {"user": True, "sudo": True}}
             )
```

### Comparing `pglift-0.8.0/tests/unit/test_systemd.py` & `pglift-0.9.0/tests/unit/test_systemd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import logging
+from pathlib import Path
 
 import pytest
 
 from pglift import systemd
 from pglift.settings import SystemdSettings
 
 
-def test_systemctl():
+def test_systemctl() -> None:
     settings = SystemdSettings()
     systemd.systemctl(settings, "user") == ["systemctl", "--user", "user"]
 
     settings = SystemdSettings(user=False)
     systemd.systemctl(settings, "root") == ["systemctl", "--system", "root"]
 
     settings = SystemdSettings(user=False, sudo=True)
     systemd.systemctl(settings, "sudoer") == ["sudo", "systemctl", "--system", "sudoer"]
 
 
-def test_install_uninstall(tmp_path):
+def test_install_uninstall(tmp_path: Path) -> None:
     logger = logging.getLogger(__name__)
     systemd.install("foo", "ahah", tmp_path, logger=logger)
     unit_path = tmp_path / "foo"
     mtime = unit_path.stat().st_mtime
     assert unit_path.read_text() == "ahah"
     systemd.install("foo", "ahah", tmp_path, logger=logger)
     assert unit_path.stat().st_mtime == mtime
```

### Comparing `pglift-0.8.0/tests/unit/test_task.py` & `pglift-0.9.0/tests/unit/test_task.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         except Exception:
             self.records.append((msg, False))
             raise
         else:
             self.records.append((msg, True))
 
 
-def test_task():
+def test_task() -> None:
     @task.task("negate")
     def neg(x: int) -> int:
         return -x
 
     assert re.match(r"<Task 'neg' at 0x(\d+)>" "", repr(neg))
 
     assert neg(1) == -1
@@ -41,28 +41,28 @@
     def revert_neg(x: int) -> int:
         return -x
 
     assert neg.revert_action
     assert neg.revert_action(-1) == 1
 
 
-def test_runner_state(logger):
+def test_runner_state(logger: logging.Logger) -> None:
     with pytest.raises(RuntimeError, match="inconsistent task state"):
         with task.Runner(logger):
             with task.Runner(logger):
                 pass
 
     with pytest.raises(ValueError, match="expected"):
         with task.Runner(logger):
             assert task.Task._calls is not None
             raise ValueError("expected")
     assert task.Task._calls is None
 
 
-def test_runner(logger, caplog):
+def test_runner(logger: logging.Logger, caplog: pytest.LogCaptureFixture) -> None:
     values = set()
 
     @task.task("add {x} to values")
     def add(x: int, fail: bool = False) -> None:
         values.add(x)
         if fail:
             raise RuntimeError("oups")
```

### Comparing `pglift-0.8.0/tests/unit/test_util.py` & `pglift-0.9.0/tests/unit/test_util.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 from pathlib import Path
 
 import pytest
 
 from pglift import util
 
 
-def test_xdg_data_home(monkeypatch):
+def test_xdg_data_home(monkeypatch: pytest.MonkeyPatch) -> None:
     with monkeypatch.context() as m:
         m.setenv("XDG_DATA_HOME", "/x/y")
         assert util.xdg_data_home() == Path("/x/y")
     with monkeypatch.context() as m:
         try:
             m.delenv("XDG_DATA_HOME")
         except KeyError:
             pass
         m.setattr("pathlib.Path.home", lambda: Path("/ho/me"))
         assert util.xdg_data_home() == Path("/ho/me/.local/share")
 
 
-def test_gen_certificate(tmp_path):
+def test_gen_certificate(tmp_path: Path) -> None:
 
     util.generate_certificate(tmp_path)
     crt = tmp_path / "server.crt"
     key = tmp_path / "server.key"
     assert crt.exists()
     assert key.exists()
     assert stat.filemode(crt.stat().st_mode) == "-rw-------"
     assert stat.filemode(key.stat().st_mode) == "-rw-------"
 
 
-def test_total_memory(meminfo):
+def test_total_memory(meminfo: Path) -> None:
     assert util.total_memory(meminfo) == 6166585344.0
 
 
-def test_total_memory_error(tmp_path):
+def test_total_memory_error(tmp_path: Path) -> None:
     meminfo = tmp_path / "meminfo"
     meminfo.touch()
     with pytest.raises(Exception, match="could not retrieve memory information from"):
         util.total_memory(meminfo)
```

### Comparing `pglift-0.8.0/tox.ini` & `pglift-0.9.0/tox.ini`

 * *Files identical despite different names*

