# Comparing `tmp/metaflow-2.9.4.tar.gz` & `tmp/metaflow-2.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-2.9.4.tar", last modified: Mon Jun 12 20:43:31 2023, max compression
+gzip compressed data, was "metaflow-2.9.5.tar", last modified: Thu Jun 15 19:26:54 2023, max compression
```

## Comparing `metaflow-2.9.4.tar` & `metaflow-2.9.5.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.947860 metaflow-2.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-12 20:43:20.000000 metaflow-2.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 20:43:20.000000 metaflow-2.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-12 20:43:31.947860 metaflow-2.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-12 20:43:20.000000 metaflow-2.9.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.915858 metaflow-2.9.4/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.915858 metaflow-2.9.4/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.919858 metaflow-2.9.4/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.919858 metaflow-2.9.4/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.919858 metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.919858 metaflow-2.9.4/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.919858 metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.919858 metaflow-2.9.4/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.919858 metaflow-2.9.4/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33396 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.923858 metaflow-2.9.4/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.923858 metaflow-2.9.4/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49461 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.923858 metaflow-2.9.4/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18785 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.923858 metaflow-2.9.4/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.927858 metaflow-2.9.4/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.927858 metaflow-2.9.4/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31438 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.927858 metaflow-2.9.4/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.927858 metaflow-2.9.4/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.927858 metaflow-2.9.4/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/argo/argo_events.py
--rw-r--r--   0 runner    (1001) docker     (123)   104779 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.927858 metaflow-2.9.4/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.931859 metaflow-2.9.4/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.931859 metaflow-2.9.4/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.931859 metaflow-2.9.4/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.931859 metaflow-2.9.4/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.931859 metaflow-2.9.4/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.935859 metaflow-2.9.4/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.935859 metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.935859 metaflow-2.9.4/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.935859 metaflow-2.9.4/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.935859 metaflow-2.9.4/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.939859 metaflow-2.9.4/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.939859 metaflow-2.9.4/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.939859 metaflow-2.9.4/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.939859 metaflow-2.9.4/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.939859 metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.939859 metaflow-2.9.4/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/environment_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/events_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.939859 metaflow-2.9.4/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.943859 metaflow-2.9.4/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.943859 metaflow-2.9.4/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19933 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.943859 metaflow-2.9.4/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.943859 metaflow-2.9.4/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.943859 metaflow-2.9.4/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.911857 metaflow-2.9.4/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.943859 metaflow-2.9.4/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.943859 metaflow-2.9.4/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.947860 metaflow-2.9.4/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.947860 metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.947860 metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.947860 metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.947860 metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.947860 metaflow-2.9.4/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.947860 metaflow-2.9.4/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-12 20:43:20.000000 metaflow-2.9.4/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 20:43:31.915858 metaflow-2.9.4/metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-12 20:43:31.000000 metaflow-2.9.4/metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-12 20:43:31.000000 metaflow-2.9.4/metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 20:43:31.000000 metaflow-2.9.4/metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-12 20:43:31.000000 metaflow-2.9.4/metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 20:43:31.000000 metaflow-2.9.4/metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 20:43:31.000000 metaflow-2.9.4/metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 20:43:31.947860 metaflow-2.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-12 20:43:20.000000 metaflow-2.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.635042 metaflow-2.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-15 19:26:44.000000 metaflow-2.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-15 19:26:44.000000 metaflow-2.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-15 19:26:54.635042 metaflow-2.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-06-15 19:26:44.000000 metaflow-2.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.611042 metaflow-2.9.5/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.611042 metaflow-2.9.5/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.611042 metaflow-2.9.5/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.611042 metaflow-2.9.5/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.611042 metaflow-2.9.5/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.611042 metaflow-2.9.5/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.615042 metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.615042 metaflow-2.9.5/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69283 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.615042 metaflow-2.9.5/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33396 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.615042 metaflow-2.9.5/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.615042 metaflow-2.9.5/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49461 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19721 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.615042 metaflow-2.9.5/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.615042 metaflow-2.9.5/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.619042 metaflow-2.9.5/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.619042 metaflow-2.9.5/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31438 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.619042 metaflow-2.9.5/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.619042 metaflow-2.9.5/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.619042 metaflow-2.9.5/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104799 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20298 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.619042 metaflow-2.9.5/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.619042 metaflow-2.9.5/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16677 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.619042 metaflow-2.9.5/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.623042 metaflow-2.9.5/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.623042 metaflow-2.9.5/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.623042 metaflow-2.9.5/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.623042 metaflow-2.9.5/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.623042 metaflow-2.9.5/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64398 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43163 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17724 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.627042 metaflow-2.9.5/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19933 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.607041 metaflow-2.9.5/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.631042 metaflow-2.9.5/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.635042 metaflow-2.9.5/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.635042 metaflow-2.9.5/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-15 19:26:44.000000 metaflow-2.9.5/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:26:54.611042 metaflow-2.9.5/metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-15 19:26:54.000000 metaflow-2.9.5/metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-06-15 19:26:54.000000 metaflow-2.9.5/metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:26:54.000000 metaflow-2.9.5/metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-15 19:26:54.000000 metaflow-2.9.5/metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 19:26:54.000000 metaflow-2.9.5/metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 19:26:54.000000 metaflow-2.9.5/metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 19:26:54.635042 metaflow-2.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-15 19:26:44.000000 metaflow-2.9.5/setup.py
```

### Comparing `metaflow-2.9.4/LICENSE` & `metaflow-2.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/PKG-INFO` & `metaflow-2.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.9.4
+Version: 2.9.5
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.9.4/README.md` & `metaflow-2.9.5/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/R.py` & `metaflow-2.9.5/metaflow/R.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/__init__.py` & `metaflow-2.9.5/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/__init__.py` & `metaflow-2.9.5/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/_bashcomplete.py` & `metaflow-2.9.5/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/_compat.py` & `metaflow-2.9.5/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/_termui_impl.py` & `metaflow-2.9.5/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/_textwrap.py` & `metaflow-2.9.5/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/_unicodefun.py` & `metaflow-2.9.5/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/_winconsole.py` & `metaflow-2.9.5/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/core.py` & `metaflow-2.9.5/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/decorators.py` & `metaflow-2.9.5/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/exceptions.py` & `metaflow-2.9.5/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/formatting.py` & `metaflow-2.9.5/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/globals.py` & `metaflow-2.9.5/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/parser.py` & `metaflow-2.9.5/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/termui.py` & `metaflow-2.9.5/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/testing.py` & `metaflow-2.9.5/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/types.py` & `metaflow-2.9.5/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/click/utils.py` & `metaflow-2.9.5/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `metaflow-2.9.5/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `metaflow-2.9.5/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_5/zipp.py` & `metaflow-2.9.5/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/typing_extensions.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/_vendor/v3_6/zipp.py` & `metaflow-2.9.5/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/cli.py` & `metaflow-2.9.5/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/cli_args.py` & `metaflow-2.9.5/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/client/core.py` & `metaflow-2.9.5/metaflow/client/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/client/filecache.py` & `metaflow-2.9.5/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/cmd/configure_cmd.py` & `metaflow-2.9.5/metaflow/cmd/configure_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/cmd/main_cli.py` & `metaflow-2.9.5/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/cmd/tutorials_cmd.py` & `metaflow-2.9.5/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/cmd_with_io.py` & `metaflow-2.9.5/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/current.py` & `metaflow-2.9.5/metaflow/current.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/datastore/content_addressed_store.py` & `metaflow-2.9.5/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/datastore/datastore_set.py` & `metaflow-2.9.5/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/datastore/datastore_storage.py` & `metaflow-2.9.5/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/datastore/flow_datastore.py` & `metaflow-2.9.5/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/datastore/task_datastore.py` & `metaflow-2.9.5/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/debug.py` & `metaflow-2.9.5/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/decorators.py` & `metaflow-2.9.5/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/event_logger.py` & `metaflow-2.9.5/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/events.py` & `metaflow-2.9.5/metaflow/events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/exception.py` & `metaflow-2.9.5/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/extension_support/__init__.py` & `metaflow-2.9.5/metaflow/extension_support/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/extension_support/cmd.py` & `metaflow-2.9.5/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/extension_support/integrations.py` & `metaflow-2.9.5/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/extension_support/plugins.py` & `metaflow-2.9.5/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/flowspec.py` & `metaflow-2.9.5/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/graph.py` & `metaflow-2.9.5/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/includefile.py` & `metaflow-2.9.5/metaflow/includefile.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/integrations.py` & `metaflow-2.9.5/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/lint.py` & `metaflow-2.9.5/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/metadata/heartbeat.py` & `metaflow-2.9.5/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/metadata/metadata.py` & `metaflow-2.9.5/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/metadata/util.py` & `metaflow-2.9.5/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/metaflow_config.py` & `metaflow-2.9.5/metaflow/metaflow_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,17 @@
 
 ###
 # Datatools (S3) configuration
 ###
 S3_ENDPOINT_URL = from_conf("S3_ENDPOINT_URL")
 S3_VERIFY_CERTIFICATE = from_conf("S3_VERIFY_CERTIFICATE")
 
+# Set ServerSideEncryption for S3 uploads
+S3_SERVER_SIDE_ENCRYPTION = from_conf("S3_SERVER_SIDE_ENCRYPTION")
+
 # S3 retry configuration
 # This is useful if you want to "fail fast" on S3 operations; use with caution
 # though as this may increase failures. Note that this is the number of *retries*
 # so setting it to 0 means each operation will be tried once.
 S3_RETRY_COUNT = from_conf("S3_RETRY_COUNT", 7)
 
 # Number of retries on *transient* failures (such as SlowDown errors). Note
```

### Comparing `metaflow-2.9.4/metaflow/metaflow_config_funcs.py` & `metaflow-2.9.5/metaflow/metaflow_config_funcs.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 
     Prior to a value being returned, we will validate using validate_fn (if provided).
     Only non-None values are validated.
 
     validate_fn should accept (name, value).
     If the value validates, return None, else raise an MetaflowException.
     """
-    env_name = "METAFLOW_%s" % name
     is_default = True
+    env_name = "METAFLOW_%s" % name
     value = os.environ.get(env_name, METAFLOW_CONFIG.get(env_name, default))
     if validate_fn and value is not None:
         validate_fn(env_name, value)
     if default is not None:
         # In this case, value is definitely not None because default is the ultimate
         # fallback and all other cases will return a string (even if an empty string)
         if isinstance(default, (list, dict)):
```

### Comparing `metaflow-2.9.4/metaflow/metaflow_environment.py` & `metaflow-2.9.5/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/metaflow_version.py` & `metaflow-2.9.5/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/mflog/__init__.py` & `metaflow-2.9.5/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/mflog/mflog.py` & `metaflow-2.9.5/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/mflog/save_logs.py` & `metaflow-2.9.5/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/mflog/save_logs_periodically.py` & `metaflow-2.9.5/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/mflog/tee.py` & `metaflow-2.9.5/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/monitor.py` & `metaflow-2.9.5/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/multicore_utils.py` & `metaflow-2.9.5/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/package.py` & `metaflow-2.9.5/metaflow/package.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/parameters.py` & `metaflow-2.9.5/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/__init__.py` & `metaflow-2.9.5/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/airflow/airflow.py` & `metaflow-2.9.5/metaflow/plugins/airflow/airflow.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/airflow/airflow_cli.py` & `metaflow-2.9.5/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/airflow/airflow_decorator.py` & `metaflow-2.9.5/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/airflow/airflow_utils.py` & `metaflow-2.9.5/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/airflow/plumbing/set_parameters.py` & `metaflow-2.9.5/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/airflow/sensors/base_sensor.py` & `metaflow-2.9.5/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `metaflow-2.9.5/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/airflow/sensors/s3_sensor.py` & `metaflow-2.9.5/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/argo/argo_client.py` & `metaflow-2.9.5/metaflow/plugins/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/argo/argo_events.py` & `metaflow-2.9.5/metaflow/plugins/argo/argo_events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/argo/argo_workflows.py` & `metaflow-2.9.5/metaflow/plugins/argo/argo_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
     KUBERNETES_SANDBOX_INIT_SCRIPT,
     KUBERNETES_SECRETS,
     S3_ENDPOINT_URL,
     SERVICE_HEADERS,
     SERVICE_INTERNAL_URL,
+    S3_SERVER_SIDE_ENCRYPTION,
 )
 from metaflow.mflog import BASH_SAVE_LOGS, bash_capture_logs, export_mflog_env_vars
 from metaflow.parameters import deploy_time_eval
 from metaflow.plugins.kubernetes.kubernetes import (
     parse_kube_keyvalue_list,
     validate_kube_labels,
 )
@@ -439,26 +440,24 @@
                 )
             options = self.flow._flow_decorators.get("trigger_on_finish")[0].options
 
         for event in triggers:
             # Assign a sanitized name since we need this at many places to please
             # Argo Events sensors. There is a slight possibility of name collision
             # but quite unlikely for us to worry about at this point.
-            event["sanitized_name"] = event["name"]
-            if any([x in event["name"] for x in [".", "-", "@", "+"]]):
-                event["sanitized_name"] = "%s_%s" % (
-                    event["name"]
-                    .replace(".", "")
-                    .replace("-", "")
-                    .replace("@", "")
-                    .replace("+", ""),
-                    to_unicode(
-                        base64.b32encode(sha1(to_bytes(event["name"])).digest())
-                    )[:4].lower(),
-                )
+            event["sanitized_name"] = "%s_%s" % (
+                event["name"]
+                .replace(".", "")
+                .replace("-", "")
+                .replace("@", "")
+                .replace("+", ""),
+                to_unicode(base64.b32encode(sha1(to_bytes(event["name"])).digest()))[
+                    :4
+                ].lower(),
+            )
         return triggers, options
 
     def _compile_workflow_template(self):
         # This method compiles a Metaflow FlowSpec into Argo WorkflowTemplate
         #
         # WorkflowTemplate
         #   |
@@ -933,18 +932,16 @@
                     + [
                         "init",
                         "--run-id %s" % run_id,
                         "--task-id %s" % task_id_params,
                     ]
                     + [
                         # Parameter names can be hyphenated, hence we use
-                        # {{foo.bar['param_name']}}. We quote the value to
-                        # make sure whitespaces are properly handled since
-                        # Argo Events wouldn't do that for us.
-                        "--%s='{{workflow.parameters.%s}}'"
+                        # {{foo.bar['param_name']}}.
+                        "--%s={{workflow.parameters.%s}}"
                         % (parameter["name"], parameter["name"])
                         for parameter in self.parameters.values()
                     ]
                 )
                 if self.tags:
                     init.extend("--tag %s" % tag for tag in self.tags)
                 # if the start step gets retried, we must be careful
@@ -1101,14 +1098,18 @@
             if self.triggers:
                 for event in self.triggers:
                     env[
                         "METAFLOW_ARGO_EVENT_PAYLOAD_%s_%s"
                         % (event["type"], event["sanitized_name"])
                     ] = ("{{workflow.parameters.%s}}" % event["sanitized_name"])
 
+            # Map S3 upload headers to environment variables
+            if S3_SERVER_SIDE_ENCRYPTION is not None:
+                env["METAFLOW_S3_SERVER_SIDE_ENCRYPTION"] = S3_SERVER_SIDE_ENCRYPTION
+
             metaflow_version = self.environment.get_environment_info()
             metaflow_version["flow_name"] = self.graph.name
             metaflow_version["production_token"] = self.production_token
             env["METAFLOW_VERSION"] = json.dumps(metaflow_version)
 
             # Set the template inputs and outputs for passing state. Very simply,
             # the container template takes in input-paths as input and outputs
@@ -1265,30 +1266,32 @@
                                     if isinstance(resources.get("secrets"), str)
                                     else resources.get("secrets")
                                 )
                                 + KUBERNETES_SECRETS.split(",")
                                 + ARGO_WORKFLOWS_KUBERNETES_SECRETS.split(",")
                                 if k
                             ],
-                            # Assign a volume point to pass state to the next task.
                             volume_mounts=[
+                                # Assign a volume mount to pass state to the next task.
                                 kubernetes_sdk.V1VolumeMount(
                                     name="out", mount_path="/mnt/out"
                                 )
                             ]
+                            # Support tmpfs.
                             + (
                                 [
                                     kubernetes_sdk.V1VolumeMount(
                                         name="tmpfs-ephemeral-volume",
                                         mount_path=tmpfs_path,
                                     )
                                 ]
                                 if tmpfs_enabled
                                 else []
                             )
+                            # Support persistent volume claims.
                             + (
                                 [
                                     kubernetes_sdk.V1VolumeMount(
                                         name=claim, mount_path=path
                                     )
                                     for claim, path in resources.get(
                                         "persistent_volume_claims"
```

### Comparing `metaflow-2.9.4/metaflow/plugins/argo/argo_workflows_cli.py` & `metaflow-2.9.5/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/argo/argo_workflows_decorator.py` & `metaflow-2.9.5/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/argo/process_input_paths.py` & `metaflow-2.9.5/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/aws_client.py` & `metaflow-2.9.5/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/aws_utils.py` & `metaflow-2.9.5/metaflow/plugins/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/batch/batch.py` & `metaflow-2.9.5/metaflow/plugins/aws/batch/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     DEFAULT_METADATA,
     SERVICE_HEADERS,
     BATCH_EMIT_TAGS,
     CARD_S3ROOT,
     S3_ENDPOINT_URL,
     DEFAULT_SECRETS_BACKEND_TYPE,
     AWS_SECRETS_MANAGER_DEFAULT_REGION,
+    S3_SERVER_SIDE_ENCRYPTION,
 )
 from metaflow.mflog import (
     export_mflog_env_vars,
     bash_capture_logs,
     tail_logs,
     BASH_SAVE_LOGS,
 )
@@ -259,14 +260,19 @@
             )
 
         tmpfs_enabled = use_tmpfs or (tmpfs_size and not use_tmpfs)
 
         if tmpfs_enabled and tmpfs_tempdir:
             job.environment_variable("METAFLOW_TEMPDIR", tmpfs_path)
 
+        if S3_SERVER_SIDE_ENCRYPTION is not None:
+            job.environment_variable(
+                "METAFLOW_S3_SERVER_SIDE_ENCRYPTION", S3_SERVER_SIDE_ENCRYPTION
+            )
+
         # Skip setting METAFLOW_DATASTORE_SYSROOT_LOCAL because metadata sync between the local user
         # instance and the remote AWS Batch instance assumes metadata is stored in DATASTORE_LOCAL_DIR
         # on the remote AWS Batch instance; this happens when METAFLOW_DATASTORE_SYSROOT_LOCAL
         # is NOT set (see get_datastore_root_from_config in datastore/local.py).
         # add METAFLOW_S3_ENDPOINT_URL
         if S3_ENDPOINT_URL is not None:
             job.environment_variable("METAFLOW_S3_ENDPOINT_URL", S3_ENDPOINT_URL)
```

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/batch/batch_cli.py` & `metaflow-2.9.5/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/batch/batch_client.py` & `metaflow-2.9.5/metaflow/plugins/aws/batch/batch_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/batch/batch_decorator.py` & `metaflow-2.9.5/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `metaflow-2.9.5/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `metaflow-2.9.5/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `metaflow-2.9.5/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/step_functions/production_token.py` & `metaflow-2.9.5/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `metaflow-2.9.5/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `metaflow-2.9.5/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions.py` & `metaflow-2.9.5/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `metaflow-2.9.5/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_client.py` & `metaflow-2.9.5/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `metaflow-2.9.5/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/azure/azure_tail.py` & `metaflow-2.9.5/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/azure/azure_utils.py` & `metaflow-2.9.5/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/azure/blob_service_client_factory.py` & `metaflow-2.9.5/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/azure/includefile_support.py` & `metaflow-2.9.5/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_cli.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_client.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_datastore.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_decorator.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/__init__.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/base.html` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/basic.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/bundle.css` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/card.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/main.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/components.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/main.js` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/renderer_tools.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_modules/test_cards.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/card_resolver.py` & `metaflow-2.9.5/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/component_serializer.py` & `metaflow-2.9.5/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/cards/exception.py` & `metaflow-2.9.5/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/catch_decorator.py` & `metaflow-2.9.5/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/conda/__init__.py` & `metaflow-2.9.5/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/conda/batch_bootstrap.py` & `metaflow-2.9.5/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/conda/conda.py` & `metaflow-2.9.5/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/conda/conda_environment.py` & `metaflow-2.9.5/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/conda/conda_flow_decorator.py` & `metaflow-2.9.5/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/conda/conda_step_decorator.py` & `metaflow-2.9.5/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/datastores/azure_storage.py` & `metaflow-2.9.5/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/datastores/gs_storage.py` & `metaflow-2.9.5/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/datastores/local_storage.py` & `metaflow-2.9.5/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/datastores/s3_storage.py` & `metaflow-2.9.5/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/datatools/__init__.py` & `metaflow-2.9.5/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/datatools/local.py` & `metaflow-2.9.5/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/datatools/s3/s3.py` & `metaflow-2.9.5/metaflow/plugins/datatools/s3/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from metaflow import FlowSpec
 from metaflow.current import current
 from metaflow.metaflow_config import (
     DATATOOLS_S3ROOT,
     S3_RETRY_COUNT,
     S3_TRANSIENT_RETRY_COUNT,
+    S3_SERVER_SIDE_ENCRYPTION,
     TEMPDIR,
 )
 from metaflow.util import (
     namedtuple_with_defaults,
     is_stringish,
     to_bytes,
     to_unicode,
@@ -79,17 +80,18 @@
 S3PutObject = namedtuple_with_defaults(
     "S3PutObject",
     [
         ("key", str),
         ("value", Optional[PutValue]),
         ("path", Optional[str]),
         ("content_type", Optional[str]),
+        ("encryption", Optional[str]),
         ("metadata", Optional[Dict[str, str]]),
     ],
-    defaults=(None, None, None, None),
+    defaults=(None, None, None, None, None),
 )
 S3PutObject.__module__ = __name__
 
 RangeInfo = namedtuple_with_defaults(
     "RangeInfo",
     [("total_size", int), ("request_offset", int), ("request_length", int)],
     defaults=(0, -1),
@@ -138,14 +140,15 @@
         url: str,
         path: str,
         size: Optional[int] = None,
         content_type: Optional[str] = None,
         metadata: Optional[Dict[str, str]] = None,
         range_info: Optional[RangeInfo] = None,
         last_modified: int = None,
+        encryption: Optional[str] = None,
     ):
         # all fields of S3Object should return a unicode object
         prefix, url, path = map(ensure_unicode, (prefix, url, path))
 
         self._size = size
         self._url = url
         self._path = path
@@ -172,14 +175,16 @@
         if prefix is None or prefix == url:
             self._key = url
             self._prefix = None
         else:
             self._key = url[len(prefix.rstrip("/")) + 1 :].rstrip("/")
             self._prefix = prefix
 
+        self._encryption = encryption
+
     @property
     def exists(self) -> bool:
         """
         Does this key correspond to an object in S3?
 
         Returns
         -------
@@ -317,14 +322,15 @@
         bool
             True if additional metadata is available.
         """
         return (
             self._content_type is not None
             or self._metadata is not None
             or self._range_info is not None
+            or self._encryption is not None
         )
 
     @property
     def metadata(self) -> Optional[Dict[str, str]]:
         """
         Returns a dictionary of user-defined metadata, or None if no metadata
         is defined.
@@ -345,14 +351,26 @@
         -------
         str
             Content type or None if the content type is undefined.
         """
         return self._content_type
 
     @property
+    def encryption(self) -> Optional[str]:
+        """
+        Returns the encryption type of the S3 object or None if it is not defined.
+
+        Returns
+        -------
+        str
+            Server-side-encryption type or None if parameter is not set.
+        """
+        return self._encryption
+
+    @property
     def range_info(self) -> Optional[RangeInfo]:
         """
         If the object corresponds to a partially downloaded object, returns
         information of what was downloaded.
 
         The returned object has the following fields:
         - `total_size`: Size of the object in S3.
@@ -482,14 +500,15 @@
     def __init__(
         self,
         tmproot: str = TEMPDIR,
         bucket: Optional[str] = None,
         prefix: Optional[str] = None,
         run: Optional[Union[FlowSpec, "Run"]] = None,
         s3root: Optional[str] = None,
+        encryption: Optional[str] = S3_SERVER_SIDE_ENCRYPTION,
         **kwargs
     ):
         if not boto_found:
             raise MetaflowException("You need to install 'boto3' in order to use S3.")
 
         if run:
             # 1. use a (current) run ID with optional customizations
@@ -535,14 +554,15 @@
                 s3_client_params=self._s3_client_params,
             ),
         )
         self._s3_inject_failures = kwargs.get(
             "inject_failure_rate", TEST_INJECT_RETRYABLE_FAILURES
         )
         self._tmpdir = mkdtemp(dir=tmproot, prefix="metaflow.s3.")
+        self._encryption = encryption
 
     def __enter__(self) -> "S3":
         return self
 
     def __exit__(self, *args):
         self.close()
 
@@ -735,14 +755,15 @@
         def _info(s3, tmp):
             resp = s3.head_object(Bucket=src.netloc, Key=src.path.lstrip('/"'))
             return {
                 "content_type": resp["ContentType"],
                 "metadata": resp["Metadata"],
                 "size": resp["ContentLength"],
                 "last_modified": get_timestamp(resp["LastModified"]),
+                "encryption": resp["ServerSideEncryption"],
             }
 
         info_results = None
         try:
             _, info_results = self._one_boto_op(_info, url, create_tmp_file=False)
         except MetaflowS3NotFound:
             if return_missing:
@@ -754,14 +775,15 @@
                 self._s3root,
                 url,
                 path=None,
                 size=info_results["size"],
                 content_type=info_results["content_type"],
                 metadata=info_results["metadata"],
                 last_modified=info_results["last_modified"],
+                encryption=info_results["encryption"],
             )
         return S3Object(self._s3root, url, None)
 
     def info_many(
         self, keys: Iterable[str], return_missing: bool = False
     ) -> List[S3Object]:
         """
@@ -807,15 +829,17 @@
                         elif info["error"] == s3op.ERROR_URL_ACCESS_DENIED:
                             raise MetaflowS3AccessDenied()
                         else:
                             raise MetaflowS3Exception("Got error: %d" % info["error"])
                     else:
                         yield self._s3root, s3url, None, info["size"], info[
                             "content_type"
-                        ], info["metadata"], None, info["last_modified"]
+                        ], info["metadata"], None, info["last_modified"], info[
+                            "encryption"
+                        ]
                 else:
                     # This should not happen; we should always get a response
                     # even if it contains an error inside it
                     raise MetaflowS3Exception("Did not get a response to HEAD")
 
         return list(starmap(S3Object, _head()))
 
@@ -882,14 +906,15 @@
                 s3.download_file(src.netloc, src.path.lstrip("/"), tmp)
             else:
                 with open(tmp, mode="wb") as t:
                     read_in_chunks(t, resp["Body"], sz, DOWNLOAD_MAX_CHUNK)
             if return_info:
                 return {
                     "content_type": resp["ContentType"],
+                    "encryption": resp["ServerSideEncryption"],
                     "metadata": resp["Metadata"],
                     "range_result": range_result,
                     "last_modified": get_timestamp(resp["LastModified"]),
                 }
             return None
 
         addl_info = None
@@ -902,14 +927,15 @@
                 raise
         if addl_info:
             return S3Object(
                 self._s3root,
                 url,
                 path,
                 content_type=addl_info["content_type"],
+                encryption=addl_info["encryption"],
                 metadata=addl_info["metadata"],
                 range_info=addl_info["range_result"],
                 last_modified=addl_info["last_modified"],
             )
         return S3Object(self._s3root, url, path)
 
     def get_many(
@@ -963,21 +989,23 @@
                             range_info = RangeInfo(
                                 range_info["total"],
                                 request_offset=range_info["start"],
                                 request_length=range_info["end"]
                                 - range_info["start"]
                                 + 1,
                             )
-                        yield self._s3root, s3url, os.path.join(
-                            self._tmpdir, fname
-                        ), None, info["content_type"], info[
-                            "metadata"
-                        ], range_info, info[
-                            "last_modified"
-                        ]
+                            yield self._s3root, s3url, os.path.join(
+                                self._tmpdir, fname
+                            ), None, info["content_type"], info[
+                                "metadata"
+                            ], range_info, info[
+                                "last_modified"
+                            ], info[
+                                "encryption"
+                            ]
                     else:
                         yield self._s3root, s3prefix, None
                 else:
                     if fname:
                         yield self._s3root, s3url, os.path.join(self._tmpdir, fname)
                     else:
                         # missing entries per return_missing=True
@@ -1029,14 +1057,16 @@
                             request_offset=range_info["start"],
                             request_length=range_info["end"] - range_info["start"] + 1,
                         )
                     yield self._s3root, s3url, os.path.join(
                         self._tmpdir, fname
                     ), None, info["content_type"], info["metadata"], range_info, info[
                         "last_modified"
+                    ], info[
+                        "encryption"
                     ]
                 else:
                     yield s3prefix, s3url, os.path.join(self._tmpdir, fname)
 
         return list(starmap(S3Object, _get()))
 
     def get_all(self, return_info: bool = False) -> List[S3Object]:
@@ -1116,22 +1146,24 @@
         # will/may close it on failure)
         real_close = blob.close
         blob.close = lambda: None
 
         url = self._url(key)
         src = urlparse(url)
         extra_args = None
-        if content_type or metadata:
+        if content_type or metadata or self._encryption:
             extra_args = {}
             if content_type:
                 extra_args["ContentType"] = content_type
             if metadata:
                 extra_args["Metadata"] = {
                     "metaflow-user-attributes": json.dumps(metadata)
                 }
+            if self._encryption:
+                extra_args["ServerSideEncryption"] = self._encryption
 
         def _upload(s3, _):
             # We make sure we are at the beginning in case we are retrying
             blob.seek(0)
             s3.upload_fileobj(
                 blob, src.netloc, src.path.lstrip("/"), ExtraArgs=extra_args
             )
@@ -1196,14 +1228,16 @@
                     "content_type": getattr(key_obj, "content_type", None),
                 }
                 metadata = getattr(key_obj, "metadata", None)
                 if metadata:
                     store_info["metadata"] = {
                         "metaflow-user-attributes": json.dumps(metadata)
                     }
+                if self._encryption:
+                    store_info["encryption"] = self._encryption
                 if isinstance(obj, (RawIOBase, BufferedIOBase)):
                     if not obj.readable() or not obj.seekable():
                         raise MetaflowS3InvalidObject(
                             "Object corresponding to the key '%s' is not readable or seekable"
                             % key
                         )
                 else:
@@ -1268,14 +1302,16 @@
                     "content_type": getattr(key_path, "content_type", None),
                 }
                 metadata = getattr(key_path, "metadata", None)
                 if metadata:
                     store_info["metadata"] = {
                         "metaflow-user-attributes": json.dumps(metadata)
                     }
+                if self._encryption:
+                    store_info["encryption"] = self._encryption
                 if not os.path.exists(path):
                     raise MetaflowS3NotFound("Local file not found: %s" % path)
                 yield path, self._url(key), store_info
 
         return self._put_many_files(_check(), overwrite)
 
     def _one_boto_op(self, op, url, create_tmp_file=True):
```

### Comparing `metaflow-2.9.4/metaflow/plugins/datatools/s3/s3op.py` & `metaflow-2.9.5/metaflow/plugins/datatools/s3/s3op.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,28 +59,30 @@
         self,
         bucket,
         path,
         url,
         local,
         prefix,
         content_type=None,
+        encryption=None,
         metadata=None,
         range=None,
         idx=None,
     ):
 
         self.bucket = bucket
         self.path = path
         self.url = url
         self.local = local
         self.prefix = prefix
         self.content_type = content_type
         self.metadata = metadata
         self.range = range
         self.idx = idx
+        self.encryption = encryption
 
     def __str__(self):
         return self.url
 
 
 # We use error codes instead of Exceptions, which are trickier to
 # handle reliably in a multiprocess world
@@ -167,14 +169,15 @@
     def op_info(url):
         try:
             head = s3.head_object(Bucket=url.bucket, Key=url.path)
             to_return = {
                 "error": None,
                 "size": head["ContentLength"],
                 "content_type": head["ContentType"],
+                "encryption": head["ServerSideEncryption"],
                 "metadata": head["Metadata"],
                 "last_modified": get_timestamp(head["LastModified"]),
             }
         except client_error as err:
             error_code = normalize_client_error(err)
             if error_code == 404:
                 to_return = {"error": ERROR_URL_NOT_FOUND, "raise_error": err}
@@ -272,14 +275,16 @@
                                 "size": resp["ContentLength"],
                                 "range_result": range_result,
                             }
                             if resp["ContentType"]:
                                 args["content_type"] = resp["ContentType"]
                             if resp["Metadata"] is not None:
                                 args["metadata"] = resp["Metadata"]
+                            if resp["ServerSideEncryption"] is not None:
+                                args["encryption"] = resp["ServerSideEncryption"]
                             if resp["LastModified"]:
                                 args["last_modified"] = get_timestamp(
                                     resp["LastModified"]
                                 )
                             json.dump(args, f)
                     # Finally, we push out the size to the result_pipe since
                     # the size is used for verification and other purposes, and
@@ -295,20 +300,22 @@
                             # We only upload if the file is not found
                             do_upload = True
                     else:
                         # No pre-op so we upload
                         do_upload = True
                     if do_upload:
                         extra = None
-                        if url.content_type or url.metadata:
+                        if url.content_type or url.metadata or url.encryption:
                             extra = {}
                             if url.content_type:
                                 extra["ContentType"] = url.content_type
                             if url.metadata is not None:
                                 extra["Metadata"] = url.metadata
+                            if url.encryption is not None:
+                                extra["ServerSideEncryption"] = url.encryption
                         try:
                             s3.upload_file(
                                 url.local, url.bucket, url.path, ExtraArgs=extra
                             )
                             # We indicate that the file was uploaded
                             result_file.write("%d %d\n" % (idx, 0))
                         except client_error as err:
@@ -457,14 +464,15 @@
                             bucket=url.bucket,
                             path=url.path,
                             url=url.url,
                             local=url.local,
                             prefix=url.prefix,
                             content_type=head["ContentType"],
                             metadata=head["Metadata"],
+                            encryption=head["ServerSideEncryption"],
                             range=url.range,
                         ),
                         head["ContentLength"],
                     )
                 ],
             )
         except self.client_error as err:
@@ -574,15 +582,15 @@
             print("verifying %s, expected %s" % (url, expected), file=sys.stderr)
         try:
             got = os.stat(url.local).st_size
         except OSError:
             raise
         if expected != got:
             exit(ERROR_VERIFY_FAILED, url)
-        if url.content_type or url.metadata:
+        if url.content_type or url.metadata or url.encryption:
             # Verify that we also have a metadata file present
             try:
                 os.stat("%s_meta" % url.local)
             except OSError:
                 exit(ERROR_VERIFY_FAILED, url)
 
 
@@ -834,29 +842,31 @@
                 else:
                     input_line_idx = line_idx
                 line_idx += 1
                 local = r["local"]
                 url = r["url"]
                 content_type = r.get("content_type", None)
                 metadata = r.get("metadata", None)
+                encryption = r.get("encryption", None)
                 if not os.path.exists(local):
                     exit(ERROR_LOCAL_FILE_NOT_FOUND, local)
-                yield input_line_idx, local, url, content_type, metadata
+                yield input_line_idx, local, url, content_type, metadata, encryption
 
-    def _make_url(idx, local, user_url, content_type, metadata):
+    def _make_url(idx, local, user_url, content_type, metadata, encryption):
         src = urlparse(user_url)
         url = S3Url(
             url=user_url,
             bucket=src.netloc,
             path=src.path.lstrip("/"),
             local=local,
             prefix=None,
             content_type=content_type,
             metadata=metadata,
             idx=idx,
+            encryption=encryption,
         )
         if src.scheme != "s3":
             exit(ERROR_INVALID_URL, url)
         if not src.path:
             exit(ERROR_NOT_FULL_PATH, url)
         return url
 
@@ -892,14 +902,15 @@
                 json.dumps(
                     {
                         "idx": url.idx,
                         "url": url.url,
                         "local": url.local,
                         "content_type": url.content_type,
                         "metadata": url.metadata,
+                        "encryption": url.encryption,
                     }
                 )
                 + "\n"
             )
             # Output something to get a total count the first time around
             if not is_transient_retry:
                 out_lines.append("%d %s\n" % (url.idx, TRANSIENT_RETRY_LINE_CONTENT))
```

### Comparing `metaflow-2.9.4/metaflow/plugins/datatools/s3/s3tail.py` & `metaflow-2.9.5/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/datatools/s3/s3util.py` & `metaflow-2.9.5/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/debug_logger.py` & `metaflow-2.9.5/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/debug_monitor.py` & `metaflow-2.9.5/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/__init__.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/client.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/client_modules.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/communication/bytestream.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/communication/channel.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/communication/utils.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/consts.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/data_transferer.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/exception_transferer.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/override_decorators.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/server.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/stub.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/env_escape/utils.py` & `metaflow-2.9.5/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/environment_decorator.py` & `metaflow-2.9.5/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/events_decorator.py` & `metaflow-2.9.5/metaflow/plugins/events_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/frameworks/pytorch.py` & `metaflow-2.9.5/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/gcp/gs_storage_client_factory.py` & `metaflow-2.9.5/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/gcp/gs_tail.py` & `metaflow-2.9.5/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/gcp/gs_utils.py` & `metaflow-2.9.5/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/gcp/includefile_support.py` & `metaflow-2.9.5/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes.py` & `metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     DEFAULT_SECRETS_BACKEND_TYPE,
     KUBERNETES_FETCH_EC2_METADATA,
     KUBERNETES_LABELS,
     KUBERNETES_SANDBOX_INIT_SCRIPT,
     S3_ENDPOINT_URL,
     SERVICE_HEADERS,
     SERVICE_INTERNAL_URL,
+    S3_SERVER_SIDE_ENCRYPTION,
 )
 from metaflow.mflog import (
     BASH_SAVE_LOGS,
     bash_capture_logs,
     export_mflog_env_vars,
     get_log_tailer,
     tail_logs,
@@ -254,14 +255,19 @@
             # Skip setting METAFLOW_DATASTORE_SYSROOT_LOCAL because metadata sync
             # between the local user instance and the remote Kubernetes pod
             # assumes metadata is stored in DATASTORE_LOCAL_DIR on the Kubernetes
             # pod; this happens when METAFLOW_DATASTORE_SYSROOT_LOCAL is NOT set (
             # see get_datastore_root_from_config in datastore/local.py).
         )
 
+        if S3_SERVER_SIDE_ENCRYPTION is not None:
+            job.environment_variable(
+                "METAFLOW_S3_SERVER_SIDE_ENCRYPTION", S3_SERVER_SIDE_ENCRYPTION
+            )
+
         # Set environment variables to support metaflow.integrations.ArgoEvent
         job.environment_variable(
             "METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ARGO_EVENTS_INTERNAL_WEBHOOK_URL
         )
         job.environment_variable("METAFLOW_ARGO_EVENTS_EVENT", ARGO_EVENTS_EVENT)
         job.environment_variable(
             "METAFLOW_ARGO_EVENTS_EVENT_BUS", ARGO_EVENTS_EVENT_BUS
```

### Comparing `metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_cli.py` & `metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_client.py` & `metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/kubernetes/kubernetes_job.py` & `metaflow-2.9.5/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/metadata/local.py` & `metaflow-2.9.5/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/metadata/service.py` & `metaflow-2.9.5/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/package_cli.py` & `metaflow-2.9.5/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/parallel_decorator.py` & `metaflow-2.9.5/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/project_decorator.py` & `metaflow-2.9.5/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/resources_decorator.py` & `metaflow-2.9.5/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/retry_decorator.py` & `metaflow-2.9.5/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/secrets/secrets_decorator.py` & `metaflow-2.9.5/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/storage_executor.py` & `metaflow-2.9.5/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/tag_cli.py` & `metaflow-2.9.5/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/test_unbounded_foreach_decorator.py` & `metaflow-2.9.5/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/plugins/timeout_decorator.py` & `metaflow-2.9.5/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/procpoll.py` & `metaflow-2.9.5/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/pylint_wrapper.py` & `metaflow-2.9.5/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/runtime.py` & `metaflow-2.9.5/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/sidecar/sidecar.py` & `metaflow-2.9.5/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/sidecar/sidecar_messages.py` & `metaflow-2.9.5/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/sidecar/sidecar_subprocess.py` & `metaflow-2.9.5/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/sidecar/sidecar_worker.py` & `metaflow-2.9.5/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tagging_util.py` & `metaflow-2.9.5/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/task.py` & `metaflow-2.9.5/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/00-helloworld/helloworld.py` & `metaflow-2.9.5/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/01-playlist/README.md` & `metaflow-2.9.5/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/01-playlist/movies.csv` & `metaflow-2.9.5/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/01-playlist/playlist.ipynb` & `metaflow-2.9.5/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/01-playlist/playlist.py` & `metaflow-2.9.5/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/02-statistics/README.md` & `metaflow-2.9.5/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/02-statistics/movies.csv` & `metaflow-2.9.5/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/02-statistics/stats.ipynb` & `metaflow-2.9.5/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/02-statistics/stats.py` & `metaflow-2.9.5/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/README.md` & `metaflow-2.9.5/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/03-playlist-redux/playlist.py` & `metaflow-2.9.5/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/README.md` & `metaflow-2.9.5/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/04-playlist-plus/playlist.py` & `metaflow-2.9.5/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/README.md` & `metaflow-2.9.5/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `metaflow-2.9.5/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `metaflow-2.9.5/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/README.md` & `metaflow-2.9.5/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `metaflow-2.9.5/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/07-worldview/worldview.ipynb` & `metaflow-2.9.5/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/08-autopilot/README.md` & `metaflow-2.9.5/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `metaflow-2.9.5/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/util.py` & `metaflow-2.9.5/metaflow/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow/vendor.py` & `metaflow-2.9.5/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/metaflow.egg-info/PKG-INFO` & `metaflow-2.9.5/metaflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.9.4
+Version: 2.9.5
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.9.4/metaflow.egg-info/SOURCES.txt` & `metaflow-2.9.5/metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-2.9.4/setup.py` & `metaflow-2.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.9.4"
+version = "2.9.5"
 
 setup(
     include_package_data=True,
     name="metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```

