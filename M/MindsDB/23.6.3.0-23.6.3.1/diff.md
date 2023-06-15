# Comparing `tmp/MindsDB-23.6.3.0.tar.gz` & `tmp/MindsDB-23.6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MindsDB-23.6.3.0.tar", last modified: Thu Jun 15 09:11:25 2023, max compression
+gzip compressed data, was "dist/MindsDB-23.6.3.1.tar", last modified: Thu Jun 15 10:28:35 2023, max compression
```

## Comparing `MindsDB-23.6.3.0.tar` & `MindsDB-23.6.3.1.tar`

### file list

```diff
@@ -1,1386 +1,1386 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/MindsDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25739 2023-06-15 09:11:24.000000 MindsDB-23.6.3.0/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66230 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:11:24.000000 MindsDB-23.6.3.0/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-06-15 09:11:24.000000 MindsDB-23.6.3.0/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 09:11:24.000000 MindsDB-23.6.3.0/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25739 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/namespaces/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    56903 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    67825 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/nlp/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autokeras_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autokeras_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cohere_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cohere_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cohere_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cohere_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/cohere_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/file_handler/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/flaml_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/flaml_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/flaml_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/flaml_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/flaml_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10399 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hackernews_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hackernews_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hackernews_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/jira_table.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/llama_index_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/llama_index_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/llama_index_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mlflow_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png
--rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monkeylearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29025 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/postgres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rockset_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rockset_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/solr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
--rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/error.png
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
--rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
--rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58244 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tpot_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/utilities/query_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/question_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/db_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/ml_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/ml_grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/ml_exec_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/ml_handler_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/libs/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/interfaces/chatbot/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/chatbot/chatbot_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/chatbot/chatbot_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/chatbot/chatbot_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/interfaces/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/interfaces/stream/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/stream/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/stream/base/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/interfaces/stream/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/requirements/requirements-grpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/requirements/requirements-telemetry.txt
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 09:11:25.000000 MindsDB-23.6.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 09:11:06.000000 MindsDB-23.6.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25739 2023-06-15 10:28:33.000000 MindsDB-23.6.3.1/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66230 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:28:33.000000 MindsDB-23.6.3.1/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-06-15 10:28:33.000000 MindsDB-23.6.3.1/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 10:28:33.000000 MindsDB-23.6.3.1/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25739 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12885 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/namespaces/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56903 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:34.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67825 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/nlp/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autokeras_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autokeras_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cohere_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cohere_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cohere_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cohere_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/cohere_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85600 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98275 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    98983 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/file_handler/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/flaml_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/flaml_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/flaml_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/flaml_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/flaml_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21392 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34337 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8618 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hackernews_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hackernews_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hackernews_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/tests/test_huggingface_api_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10766 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8801 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/llama_index_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/llama_index_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/llama_index_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/llama_index_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/llama_index_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mlflow_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544421 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png
+-rw-r--r--   0 runner    (1001) docker     (123)   423554 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   445044 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monkeylearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monkeylearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monkeylearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monkeylearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/monkeylearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29025 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97032 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)    98334 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63619 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112840 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/postgres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13384 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rockset_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13091 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/solr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+-rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58244 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tpot_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/utilities/query_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/utilities/query_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/question_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/writer_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/db_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/ml_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/ml_grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/handler_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/ml_exec_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/ml_handler_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/libs/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/interfaces/chatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/chatbot/chatbot_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/chatbot/chatbot_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/chatbot/chatbot_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22442 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/interfaces/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/interfaces/stream/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/stream/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/stream/base/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/interfaces/stream/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/requirements/requirements-grpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/requirements/requirements-telemetry.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 10:28:35.000000 MindsDB-23.6.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 10:28:00.000000 MindsDB-23.6.3.1/setup.py
```

### Comparing `MindsDB-23.6.3.0/MindsDB.egg-info/PKG-INFO` & `MindsDB-23.6.3.1/MindsDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.6.3.0
+Version: 23.6.3.1
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -206,126 +206,126 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: grpc
 Provides-Extra: telemetry
 Provides-Extra: all_extras
-Provides-Extra: edgelessdb
-Provides-Extra: mlflow
-Provides-Extra: derby
-Provides-Extra: d0lt
-Provides-Extra: vitess
-Provides-Extra: newsapi
-Provides-Extra: databend
-Provides-Extra: scylla
-Provides-Extra: huggingface
-Provides-Extra: flaml
-Provides-Extra: aurora
-Provides-Extra: orioledb
-Provides-Extra: vertica
-Provides-Extra: trino
-Provides-Extra: cloud_sql
-Provides-Extra: questdb
-Provides-Extra: mendeley
-Provides-Extra: dynamodb
-Provides-Extra: cohere
-Provides-Extra: crate
-Provides-Extra: sqreamdb
-Provides-Extra: oceanbase
-Provides-Extra: statsforecast
-Provides-Extra: shopify
-Provides-Extra: huggingface_api
-Provides-Extra: github
-Provides-Extra: datastax
-Provides-Extra: postgres
+Provides-Extra: empress
 Provides-Extra: solr
-Provides-Extra: lightwood
-Provides-Extra: stripe
-Provides-Extra: writer
-Provides-Extra: tidb
-Provides-Extra: redshift
-Provides-Extra: impala
-Provides-Extra: ingres
-Provides-Extra: google_fit
 Provides-Extra: access
-Provides-Extra: s3
-Provides-Extra: twitter
-Provides-Extra: neuralforecast
-Provides-Extra: gmail
-Provides-Extra: mysql
-Provides-Extra: plaid
-Provides-Extra: databricks
-Provides-Extra: supabase
-Provides-Extra: confluence
-Provides-Extra: sheets
-Provides-Extra: materialize
-Provides-Extra: firebird
-Provides-Extra: youtube
-Provides-Extra: mariadb
-Provides-Extra: monetdb
-Provides-Extra: pinot
-Provides-Extra: surrealdb
-Provides-Extra: informix
-Provides-Extra: influxdb
-Provides-Extra: merlion
-Provides-Extra: google_books
 Provides-Extra: binance
-Provides-Extra: db2
-Provides-Extra: paypal
-Provides-Extra: strava
+Provides-Extra: yugabyte
 Provides-Extra: bigquery
-Provides-Extra: cockroach
-Provides-Extra: starrocks
-Provides-Extra: clickhouse
-Provides-Extra: maxdb
-Provides-Extra: hsqldb
-Provides-Extra: cloud_spanner
-Provides-Extra: phoenix
-Provides-Extra: ludwig
-Provides-Extra: slack
-Provides-Extra: duckdb
-Provides-Extra: mongodb
+Provides-Extra: timescaledb
+Provides-Extra: github
+Provides-Extra: cohere
+Provides-Extra: snowflake
 Provides-Extra: quickbooks
+Provides-Extra: clickhouse
 Provides-Extra: sendinblue
-Provides-Extra: yugabyte
-Provides-Extra: matrixone
-Provides-Extra: openai
-Provides-Extra: reddit
-Provides-Extra: elasticsearch
-Provides-Extra: singlestore
-Provides-Extra: google_content_shopping
-Provides-Extra: langchain
+Provides-Extra: youtube
+Provides-Extra: monetdb
+Provides-Extra: aurora
+Provides-Extra: s3
+Provides-Extra: autosklearn
+Provides-Extra: dremio
+Provides-Extra: paypal
 Provides-Extra: rocket_chat
-Provides-Extra: frappe
+Provides-Extra: edgelessdb
+Provides-Extra: cockroach
+Provides-Extra: planetscale
+Provides-Extra: google_books
 Provides-Extra: ray_serve
+Provides-Extra: starrocks
+Provides-Extra: huggingface_api
+Provides-Extra: hive
+Provides-Extra: altibase
+Provides-Extra: mariadb
+Provides-Extra: ignite
+Provides-Extra: strava
+Provides-Extra: firebird
+Provides-Extra: tidb
+Provides-Extra: crate
+Provides-Extra: influxdb
+Provides-Extra: neuralforecast
+Provides-Extra: merlion
+Provides-Extra: vertica
+Provides-Extra: sheets
+Provides-Extra: hana
+Provides-Extra: pinot
+Provides-Extra: confluence
+Provides-Extra: opengauss
+Provides-Extra: redshift
+Provides-Extra: trino
+Provides-Extra: slack
+Provides-Extra: datastax
+Provides-Extra: questdb
 Provides-Extra: nuo_jdbc
-Provides-Extra: dremio
-Provides-Extra: timescaledb
-Provides-Extra: rockset
-Provides-Extra: druid
-Provides-Extra: ckan
-Provides-Extra: tdengine
-Provides-Extra: mssql
+Provides-Extra: orioledb
+Provides-Extra: teradata
+Provides-Extra: gmail
 Provides-Extra: oracle
+Provides-Extra: flaml
+Provides-Extra: langchain
+Provides-Extra: impala
+Provides-Extra: cloud_spanner
+Provides-Extra: ingres
+Provides-Extra: tdengine
+Provides-Extra: google_fit
+Provides-Extra: google_search
+Provides-Extra: db2
+Provides-Extra: tpot
+Provides-Extra: shopify
+Provides-Extra: google_content_shopping
 Provides-Extra: google_calendar
+Provides-Extra: ckan
+Provides-Extra: cassandra
+Provides-Extra: rockset
+Provides-Extra: monkeylearn
 Provides-Extra: sqlany
+Provides-Extra: mssql
+Provides-Extra: huggingface
+Provides-Extra: postgres
+Provides-Extra: ludwig
+Provides-Extra: airtable
+Provides-Extra: mysql
+Provides-Extra: phoenix
+Provides-Extra: singlestore
+Provides-Extra: oceanbase
+Provides-Extra: vitess
+Provides-Extra: newsapi
+Provides-Extra: druid
+Provides-Extra: hsqldb
+Provides-Extra: statsforecast
+Provides-Extra: materialize
+Provides-Extra: openai
+Provides-Extra: databricks
 Provides-Extra: jira
-Provides-Extra: planetscale
-Provides-Extra: autosklearn
-Provides-Extra: hive
-Provides-Extra: opengauss
-Provides-Extra: hana
-Provides-Extra: empress
-Provides-Extra: google_search
+Provides-Extra: scylla
+Provides-Extra: twitter
 Provides-Extra: gitlab
-Provides-Extra: airtable
-Provides-Extra: llama_index
+Provides-Extra: surrealdb
+Provides-Extra: plaid
+Provides-Extra: duckdb
+Provides-Extra: d0lt
+Provides-Extra: databend
+Provides-Extra: stripe
+Provides-Extra: mendeley
+Provides-Extra: maxdb
+Provides-Extra: derby
+Provides-Extra: mlflow
+Provides-Extra: writer
 Provides-Extra: couchbase
-Provides-Extra: ignite
-Provides-Extra: cassandra
-Provides-Extra: monkeylearn
-Provides-Extra: tpot
-Provides-Extra: altibase
-Provides-Extra: snowflake
-Provides-Extra: teradata
+Provides-Extra: dynamodb
+Provides-Extra: sqreamdb
+Provides-Extra: mongodb
+Provides-Extra: cloud_sql
+Provides-Extra: llama_index
+Provides-Extra: supabase
+Provides-Extra: matrixone
+Provides-Extra: informix
+Provides-Extra: elasticsearch
+Provides-Extra: reddit
+Provides-Extra: frappe
+Provides-Extra: lightwood
 Provides-Extra: all_handlers_extras
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.6.3.0 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.6.3.1 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -143,47 +143,47 @@
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
 product updates, information about MindsDB events and contests, and useful
 content, like tutorials. ## License MindsDB is licensed under [GNU General
 Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown Provides-Extra: grpc Provides-Extra: telemetry Provides-
-Extra: all_extras Provides-Extra: edgelessdb Provides-Extra: mlflow Provides-
-Extra: derby Provides-Extra: d0lt Provides-Extra: vitess Provides-Extra:
-newsapi Provides-Extra: databend Provides-Extra: scylla Provides-Extra:
-huggingface Provides-Extra: flaml Provides-Extra: aurora Provides-Extra:
-orioledb Provides-Extra: vertica Provides-Extra: trino Provides-Extra:
-cloud_sql Provides-Extra: questdb Provides-Extra: mendeley Provides-Extra:
-dynamodb Provides-Extra: cohere Provides-Extra: crate Provides-Extra: sqreamdb
-Provides-Extra: oceanbase Provides-Extra: statsforecast Provides-Extra: shopify
-Provides-Extra: huggingface_api Provides-Extra: github Provides-Extra: datastax
-Provides-Extra: postgres Provides-Extra: solr Provides-Extra: lightwood
-Provides-Extra: stripe Provides-Extra: writer Provides-Extra: tidb Provides-
-Extra: redshift Provides-Extra: impala Provides-Extra: ingres Provides-Extra:
-google_fit Provides-Extra: access Provides-Extra: s3 Provides-Extra: twitter
-Provides-Extra: neuralforecast Provides-Extra: gmail Provides-Extra: mysql
-Provides-Extra: plaid Provides-Extra: databricks Provides-Extra: supabase
-Provides-Extra: confluence Provides-Extra: sheets Provides-Extra: materialize
-Provides-Extra: firebird Provides-Extra: youtube Provides-Extra: mariadb
-Provides-Extra: monetdb Provides-Extra: pinot Provides-Extra: surrealdb
-Provides-Extra: informix Provides-Extra: influxdb Provides-Extra: merlion
-Provides-Extra: google_books Provides-Extra: binance Provides-Extra: db2
-Provides-Extra: paypal Provides-Extra: strava Provides-Extra: bigquery
-Provides-Extra: cockroach Provides-Extra: starrocks Provides-Extra: clickhouse
-Provides-Extra: maxdb Provides-Extra: hsqldb Provides-Extra: cloud_spanner
-Provides-Extra: phoenix Provides-Extra: ludwig Provides-Extra: slack Provides-
-Extra: duckdb Provides-Extra: mongodb Provides-Extra: quickbooks Provides-
-Extra: sendinblue Provides-Extra: yugabyte Provides-Extra: matrixone Provides-
-Extra: openai Provides-Extra: reddit Provides-Extra: elasticsearch Provides-
-Extra: singlestore Provides-Extra: google_content_shopping Provides-Extra:
-langchain Provides-Extra: rocket_chat Provides-Extra: frappe Provides-Extra:
-ray_serve Provides-Extra: nuo_jdbc Provides-Extra: dremio Provides-Extra:
-timescaledb Provides-Extra: rockset Provides-Extra: druid Provides-Extra: ckan
-Provides-Extra: tdengine Provides-Extra: mssql Provides-Extra: oracle Provides-
-Extra: google_calendar Provides-Extra: sqlany Provides-Extra: jira Provides-
-Extra: planetscale Provides-Extra: autosklearn Provides-Extra: hive Provides-
-Extra: opengauss Provides-Extra: hana Provides-Extra: empress Provides-Extra:
-google_search Provides-Extra: gitlab Provides-Extra: airtable Provides-Extra:
-llama_index Provides-Extra: couchbase Provides-Extra: ignite Provides-Extra:
-cassandra Provides-Extra: monkeylearn Provides-Extra: tpot Provides-Extra:
-altibase Provides-Extra: snowflake Provides-Extra: teradata Provides-Extra:
+Extra: all_extras Provides-Extra: empress Provides-Extra: solr Provides-Extra:
+access Provides-Extra: binance Provides-Extra: yugabyte Provides-Extra:
+bigquery Provides-Extra: timescaledb Provides-Extra: github Provides-Extra:
+cohere Provides-Extra: snowflake Provides-Extra: quickbooks Provides-Extra:
+clickhouse Provides-Extra: sendinblue Provides-Extra: youtube Provides-Extra:
+monetdb Provides-Extra: aurora Provides-Extra: s3 Provides-Extra: autosklearn
+Provides-Extra: dremio Provides-Extra: paypal Provides-Extra: rocket_chat
+Provides-Extra: edgelessdb Provides-Extra: cockroach Provides-Extra:
+planetscale Provides-Extra: google_books Provides-Extra: ray_serve Provides-
+Extra: starrocks Provides-Extra: huggingface_api Provides-Extra: hive Provides-
+Extra: altibase Provides-Extra: mariadb Provides-Extra: ignite Provides-Extra:
+strava Provides-Extra: firebird Provides-Extra: tidb Provides-Extra: crate
+Provides-Extra: influxdb Provides-Extra: neuralforecast Provides-Extra: merlion
+Provides-Extra: vertica Provides-Extra: sheets Provides-Extra: hana Provides-
+Extra: pinot Provides-Extra: confluence Provides-Extra: opengauss Provides-
+Extra: redshift Provides-Extra: trino Provides-Extra: slack Provides-Extra:
+datastax Provides-Extra: questdb Provides-Extra: nuo_jdbc Provides-Extra:
+orioledb Provides-Extra: teradata Provides-Extra: gmail Provides-Extra: oracle
+Provides-Extra: flaml Provides-Extra: langchain Provides-Extra: impala
+Provides-Extra: cloud_spanner Provides-Extra: ingres Provides-Extra: tdengine
+Provides-Extra: google_fit Provides-Extra: google_search Provides-Extra: db2
+Provides-Extra: tpot Provides-Extra: shopify Provides-Extra:
+google_content_shopping Provides-Extra: google_calendar Provides-Extra: ckan
+Provides-Extra: cassandra Provides-Extra: rockset Provides-Extra: monkeylearn
+Provides-Extra: sqlany Provides-Extra: mssql Provides-Extra: huggingface
+Provides-Extra: postgres Provides-Extra: ludwig Provides-Extra: airtable
+Provides-Extra: mysql Provides-Extra: phoenix Provides-Extra: singlestore
+Provides-Extra: oceanbase Provides-Extra: vitess Provides-Extra: newsapi
+Provides-Extra: druid Provides-Extra: hsqldb Provides-Extra: statsforecast
+Provides-Extra: materialize Provides-Extra: openai Provides-Extra: databricks
+Provides-Extra: jira Provides-Extra: scylla Provides-Extra: twitter Provides-
+Extra: gitlab Provides-Extra: surrealdb Provides-Extra: plaid Provides-Extra:
+duckdb Provides-Extra: d0lt Provides-Extra: databend Provides-Extra: stripe
+Provides-Extra: mendeley Provides-Extra: maxdb Provides-Extra: derby Provides-
+Extra: mlflow Provides-Extra: writer Provides-Extra: couchbase Provides-Extra:
+dynamodb Provides-Extra: sqreamdb Provides-Extra: mongodb Provides-Extra:
+cloud_sql Provides-Extra: llama_index Provides-Extra: supabase Provides-Extra:
+matrixone Provides-Extra: informix Provides-Extra: elasticsearch Provides-
+Extra: reddit Provides-Extra: frappe Provides-Extra: lightwood Provides-Extra:
 all_handlers_extras
```

### Comparing `MindsDB-23.6.3.0/MindsDB.egg-info/SOURCES.txt` & `MindsDB-23.6.3.1/MindsDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/MindsDB.egg-info/requires.txt` & `MindsDB-23.6.3.1/MindsDB.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -41,159 +41,159 @@
 pyodbc
 sqlalchemy-access
 
 [airtable]
 duckdb
 
 [all_extras]
-grpcio-tools
 sentry-sdk
+grpcio-tools
 
 [all_handlers_extras]
-rocketchat_API
-hdbcli
-dill
-redshift_connector
-pysqream_sqlalchemy>=0.8
-sqlalchemy-hana
-pinotdb
-boto3
-impyla
-websocket
-mindsdb-evaluator>=0.0.6
-sqlalchemy-databricks
-teradatasqlalchemy
-ray[serve]
-pymongo[srv]>=4.1.1
-mlflow
-flaml<=1.2.3
-tpot<=0.11.7
+pandas
 paypalrestsdk
-stripe
-sib_api_v3_sdk
-ckanapi
-snowflake-sqlalchemy>=1.4.3
-binance-connector
-python-gitlab
-sqlalchemy-monetdb
-google-api-python-client
-openai>=0.27.0
-scylla-driver
-pyodbc==4.0.34
-pymonetdb
-sqlalchemy-redshift
 tiktoken>=0.3.0
+sqlalchemy_dremio
+databricks-sql-connector
+stripe
+mindsdb_sql<0.5.0,>=0.4.9
 google-cloud-spanner
-sqlalchemy-sqlany
-psycopg
-tensorflow
-thrift-sasl
-vertica-python
-elasticsearch-dbapi
-pysqream>=3.2.5
-pyphoenix
-teradatasql
-mindsdb_sql<0.5.0,>=0.4.6
-oracledb==1.0.2
+ludwig[distributed]>=0.5.2
+ingres_sa_dialect==0.3
+sqlalchemy-informix
+pymssql>=2.1.4
+qbosdk
+mysql-connector-python
+sentencepiece==0.1.97
+mindsdb_sql>=0.4.0
+pyhive
+ray[serve]
+pymonetdb
+google-auth-httplib2
+mindsdb>=22.6.2.1
 mindsdb_sql<0.5.0,>=0.4.4
-mindsdb_sql<0.5.0,>=0.4.9
+hdbcli
+sqlalchemy
+thrift-sasl
+mindsdb>=23.3.5.0
+mendeley
+rockset
+tqdm
+sqlalchemy<2.0.0
+sqlanydb
 sasl
-pyodbc
-monkeylearn==3.6.0
-mindsdb>=22.10.2.1
-ludwig[distributed]>=0.5.2
+dask
+openai==0.27.0
+oracledb==1.0.2
+sqlalchemy-access
+ibm-db-sa
+pysurrealdb
+psycopg
 wikipedia==1.4.0
+pandas<=1.4.3
+google-cloud-bigquery
 certifi
-sentence_transformers
-newsapi-python
+salesforce-merlion<=1.3.1,>=1.2.0
+hugging_py_face
+sqlalchemy-monetdb
+mindsdb>=23.3.2.0
+mlflow
+snowflake-sqlalchemy>=1.4.3
+teradatasql
+scylla-driver
+mindsdb>=22.10.2.1
 google-auth-oauthlib
-duckdb==0.7.1.dev187
-sentencepiece==0.1.97
-mindsdb>=23.3.5.0
-slack_sdk
-psycopg2
-trino~=0.313.0
+jaydebeapi
+sqlalchemy-redshift
+elasticsearch
+neuralforecast<1.5.0,>=1.4.0
 transformers==4.21.0
-pyhive
-thrift
-langchain==0.0.186
-tweepy
-databricks-sql-connector
-pytz
+tensorflow
 tzlocal
-duckdb
-plaid-python
-dask
-mindsdb_sql>=0.4.0
-sqlalchemy-informix
-hyperopt<1.0
-openai==0.27.0
-crate[sqlalchemy]
-sqlalchemy<2.0.0
-mindsdb>=22.7.5.0
-statsforecast<2.0,>=1.4.0
-fdb
-sqlalchemy
-mendeley
-mindsdb>=22.6.2.1
-cohere==4.5.1
-sqlalchemy-vertica-python
-google-cloud-bigquery
+thrift
+pyodbc==4.0.34
+torch
+google
+pyodbc
 sqlalchemy-bigquery
-praw
-pandas
-IfxPy
-snowflake-connector-python>=2.7.12
+psycopg[binary]
+cohere==4.5.1
+duckdb
+mindsdb>=22.12.4.3
+pinotdb
 ibm-db
+praw
+mindsdb_sql<0.5.0,>=0.4.6
+pydantic==1.10.8
+teradatasqlalchemy
+flaml<=1.2.3
+llama-index==0.6.11
+psycopg2
+mindsdb-evaluator>=0.0.6
+sqlalchemy-sqlany
+openai>=0.27.0
 atlassian-python-api
-phoenixdb
-mindsdb>=23.3.2.0
-sqlalchemy-access
-pygithub
-sqlanydb
-google-auth-httplib2
-ShopifyAPI
-pymssql>=2.1.4
-neuralforecast<1.5.0,>=1.4.0
+redshift_connector
+dill
+plaid-python
+pymongo[srv]>=4.1.1
+sentence_transformers
+ckanapi
+sib_api_v3_sdk
+taospy
 pyignite
-pysurrealdb
-hierarchicalforecast<1.0
-ingres_sa_dialect==0.3
-qbosdk
+boto3
+lightwood[all_extras]>=22.8.1.0
+pysqream_sqlalchemy>=0.8
+ray<=1.13.0
+binance-connector
+phoenixdb
+google-api-python-client
 requests-kerberos==0.12.0
+sqlalchemy-solr
+pydruid
+langchain==0.0.186
+mindsdb>=22.7.5.0
+stravalib
 pymysql
-sqlalchemy_dremio
-salesforce-merlion<=1.3.1,>=1.2.0
-couchbase==4.0.2
-taospy
-tqdm
+trino~=0.313.0
+fdb
+sqlalchemy-vertica-python
+hyperopt
+vertica-python
+db-dtypes
+impyla
+hierarchicalforecast<1.0
+sqlalchemy-hana
 auto-sklearn
-pydantic==1.10.8
-pandas<=1.4.3
+ShopifyAPI
+tpot<=0.11.7
+websocket
+couchbase==4.0.2
 clickhouse-sqlalchemy
-jaydebeapi
-psycopg[binary]
-lightwood[all_extras]>=22.8.1.0
-sqlalchemy-solr
-ray<=1.13.0
-elasticsearch
-rockset
+slack_sdk
+duckdb==0.7.1.dev187
+python-gitlab
+pyphoenix
+tweepy
+pytz
+pygithub
+monkeylearn==3.6.0
+snowflake-connector-python>=2.7.12
+elasticsearch-dbapi
+sqlalchemy-databricks
+hyperopt<1.0
+IfxPy
+crate[sqlalchemy]
+pysqream>=3.2.5
+rocketchat_API
 pyHive
-hugging_py_face
-hyperopt
-mysql-connector-python
-stravalib
-db-dtypes
-llama-index==0.6.11
-torch
-google
-ibm-db-sa
-pydruid
+newsapi-python
 protobuf==3.20.*
-mindsdb>=22.12.4.3
+statsforecast<2.0,>=1.4.0
 
 [altibase]
 jaydebeapi
 
 [aurora]
 psycopg[binary]
 mysql-connector-python
```

### Comparing `MindsDB-23.6.3.0/PKG-INFO` & `MindsDB-23.6.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.6.3.0
+Version: 23.6.3.1
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -206,126 +206,126 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: grpc
 Provides-Extra: telemetry
 Provides-Extra: all_extras
-Provides-Extra: edgelessdb
-Provides-Extra: mlflow
-Provides-Extra: derby
-Provides-Extra: d0lt
-Provides-Extra: vitess
-Provides-Extra: newsapi
-Provides-Extra: databend
-Provides-Extra: scylla
-Provides-Extra: huggingface
-Provides-Extra: flaml
-Provides-Extra: aurora
-Provides-Extra: orioledb
-Provides-Extra: vertica
-Provides-Extra: trino
-Provides-Extra: cloud_sql
-Provides-Extra: questdb
-Provides-Extra: mendeley
-Provides-Extra: dynamodb
-Provides-Extra: cohere
-Provides-Extra: crate
-Provides-Extra: sqreamdb
-Provides-Extra: oceanbase
-Provides-Extra: statsforecast
-Provides-Extra: shopify
-Provides-Extra: huggingface_api
-Provides-Extra: github
-Provides-Extra: datastax
-Provides-Extra: postgres
+Provides-Extra: empress
 Provides-Extra: solr
-Provides-Extra: lightwood
-Provides-Extra: stripe
-Provides-Extra: writer
-Provides-Extra: tidb
-Provides-Extra: redshift
-Provides-Extra: impala
-Provides-Extra: ingres
-Provides-Extra: google_fit
 Provides-Extra: access
-Provides-Extra: s3
-Provides-Extra: twitter
-Provides-Extra: neuralforecast
-Provides-Extra: gmail
-Provides-Extra: mysql
-Provides-Extra: plaid
-Provides-Extra: databricks
-Provides-Extra: supabase
-Provides-Extra: confluence
-Provides-Extra: sheets
-Provides-Extra: materialize
-Provides-Extra: firebird
-Provides-Extra: youtube
-Provides-Extra: mariadb
-Provides-Extra: monetdb
-Provides-Extra: pinot
-Provides-Extra: surrealdb
-Provides-Extra: informix
-Provides-Extra: influxdb
-Provides-Extra: merlion
-Provides-Extra: google_books
 Provides-Extra: binance
-Provides-Extra: db2
-Provides-Extra: paypal
-Provides-Extra: strava
+Provides-Extra: yugabyte
 Provides-Extra: bigquery
-Provides-Extra: cockroach
-Provides-Extra: starrocks
-Provides-Extra: clickhouse
-Provides-Extra: maxdb
-Provides-Extra: hsqldb
-Provides-Extra: cloud_spanner
-Provides-Extra: phoenix
-Provides-Extra: ludwig
-Provides-Extra: slack
-Provides-Extra: duckdb
-Provides-Extra: mongodb
+Provides-Extra: timescaledb
+Provides-Extra: github
+Provides-Extra: cohere
+Provides-Extra: snowflake
 Provides-Extra: quickbooks
+Provides-Extra: clickhouse
 Provides-Extra: sendinblue
-Provides-Extra: yugabyte
-Provides-Extra: matrixone
-Provides-Extra: openai
-Provides-Extra: reddit
-Provides-Extra: elasticsearch
-Provides-Extra: singlestore
-Provides-Extra: google_content_shopping
-Provides-Extra: langchain
+Provides-Extra: youtube
+Provides-Extra: monetdb
+Provides-Extra: aurora
+Provides-Extra: s3
+Provides-Extra: autosklearn
+Provides-Extra: dremio
+Provides-Extra: paypal
 Provides-Extra: rocket_chat
-Provides-Extra: frappe
+Provides-Extra: edgelessdb
+Provides-Extra: cockroach
+Provides-Extra: planetscale
+Provides-Extra: google_books
 Provides-Extra: ray_serve
+Provides-Extra: starrocks
+Provides-Extra: huggingface_api
+Provides-Extra: hive
+Provides-Extra: altibase
+Provides-Extra: mariadb
+Provides-Extra: ignite
+Provides-Extra: strava
+Provides-Extra: firebird
+Provides-Extra: tidb
+Provides-Extra: crate
+Provides-Extra: influxdb
+Provides-Extra: neuralforecast
+Provides-Extra: merlion
+Provides-Extra: vertica
+Provides-Extra: sheets
+Provides-Extra: hana
+Provides-Extra: pinot
+Provides-Extra: confluence
+Provides-Extra: opengauss
+Provides-Extra: redshift
+Provides-Extra: trino
+Provides-Extra: slack
+Provides-Extra: datastax
+Provides-Extra: questdb
 Provides-Extra: nuo_jdbc
-Provides-Extra: dremio
-Provides-Extra: timescaledb
-Provides-Extra: rockset
-Provides-Extra: druid
-Provides-Extra: ckan
-Provides-Extra: tdengine
-Provides-Extra: mssql
+Provides-Extra: orioledb
+Provides-Extra: teradata
+Provides-Extra: gmail
 Provides-Extra: oracle
+Provides-Extra: flaml
+Provides-Extra: langchain
+Provides-Extra: impala
+Provides-Extra: cloud_spanner
+Provides-Extra: ingres
+Provides-Extra: tdengine
+Provides-Extra: google_fit
+Provides-Extra: google_search
+Provides-Extra: db2
+Provides-Extra: tpot
+Provides-Extra: shopify
+Provides-Extra: google_content_shopping
 Provides-Extra: google_calendar
+Provides-Extra: ckan
+Provides-Extra: cassandra
+Provides-Extra: rockset
+Provides-Extra: monkeylearn
 Provides-Extra: sqlany
+Provides-Extra: mssql
+Provides-Extra: huggingface
+Provides-Extra: postgres
+Provides-Extra: ludwig
+Provides-Extra: airtable
+Provides-Extra: mysql
+Provides-Extra: phoenix
+Provides-Extra: singlestore
+Provides-Extra: oceanbase
+Provides-Extra: vitess
+Provides-Extra: newsapi
+Provides-Extra: druid
+Provides-Extra: hsqldb
+Provides-Extra: statsforecast
+Provides-Extra: materialize
+Provides-Extra: openai
+Provides-Extra: databricks
 Provides-Extra: jira
-Provides-Extra: planetscale
-Provides-Extra: autosklearn
-Provides-Extra: hive
-Provides-Extra: opengauss
-Provides-Extra: hana
-Provides-Extra: empress
-Provides-Extra: google_search
+Provides-Extra: scylla
+Provides-Extra: twitter
 Provides-Extra: gitlab
-Provides-Extra: airtable
-Provides-Extra: llama_index
+Provides-Extra: surrealdb
+Provides-Extra: plaid
+Provides-Extra: duckdb
+Provides-Extra: d0lt
+Provides-Extra: databend
+Provides-Extra: stripe
+Provides-Extra: mendeley
+Provides-Extra: maxdb
+Provides-Extra: derby
+Provides-Extra: mlflow
+Provides-Extra: writer
 Provides-Extra: couchbase
-Provides-Extra: ignite
-Provides-Extra: cassandra
-Provides-Extra: monkeylearn
-Provides-Extra: tpot
-Provides-Extra: altibase
-Provides-Extra: snowflake
-Provides-Extra: teradata
+Provides-Extra: dynamodb
+Provides-Extra: sqreamdb
+Provides-Extra: mongodb
+Provides-Extra: cloud_sql
+Provides-Extra: llama_index
+Provides-Extra: supabase
+Provides-Extra: matrixone
+Provides-Extra: informix
+Provides-Extra: elasticsearch
+Provides-Extra: reddit
+Provides-Extra: frappe
+Provides-Extra: lightwood
 Provides-Extra: all_handlers_extras
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.6.3.0 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.6.3.1 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
@@ -143,47 +143,47 @@
 ?utm_medium=community&utm_source=github&utm_campaign=mindsdb%20repo) to get
 product updates, information about MindsDB events and contests, and useful
 content, like tutorials. ## License MindsDB is licensed under [GNU General
 Public License v3.0](https://github.com/mindsdb/mindsdb/blob/master/LICENSE)
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.8 Description-Content-
 Type: text/markdown Provides-Extra: grpc Provides-Extra: telemetry Provides-
-Extra: all_extras Provides-Extra: edgelessdb Provides-Extra: mlflow Provides-
-Extra: derby Provides-Extra: d0lt Provides-Extra: vitess Provides-Extra:
-newsapi Provides-Extra: databend Provides-Extra: scylla Provides-Extra:
-huggingface Provides-Extra: flaml Provides-Extra: aurora Provides-Extra:
-orioledb Provides-Extra: vertica Provides-Extra: trino Provides-Extra:
-cloud_sql Provides-Extra: questdb Provides-Extra: mendeley Provides-Extra:
-dynamodb Provides-Extra: cohere Provides-Extra: crate Provides-Extra: sqreamdb
-Provides-Extra: oceanbase Provides-Extra: statsforecast Provides-Extra: shopify
-Provides-Extra: huggingface_api Provides-Extra: github Provides-Extra: datastax
-Provides-Extra: postgres Provides-Extra: solr Provides-Extra: lightwood
-Provides-Extra: stripe Provides-Extra: writer Provides-Extra: tidb Provides-
-Extra: redshift Provides-Extra: impala Provides-Extra: ingres Provides-Extra:
-google_fit Provides-Extra: access Provides-Extra: s3 Provides-Extra: twitter
-Provides-Extra: neuralforecast Provides-Extra: gmail Provides-Extra: mysql
-Provides-Extra: plaid Provides-Extra: databricks Provides-Extra: supabase
-Provides-Extra: confluence Provides-Extra: sheets Provides-Extra: materialize
-Provides-Extra: firebird Provides-Extra: youtube Provides-Extra: mariadb
-Provides-Extra: monetdb Provides-Extra: pinot Provides-Extra: surrealdb
-Provides-Extra: informix Provides-Extra: influxdb Provides-Extra: merlion
-Provides-Extra: google_books Provides-Extra: binance Provides-Extra: db2
-Provides-Extra: paypal Provides-Extra: strava Provides-Extra: bigquery
-Provides-Extra: cockroach Provides-Extra: starrocks Provides-Extra: clickhouse
-Provides-Extra: maxdb Provides-Extra: hsqldb Provides-Extra: cloud_spanner
-Provides-Extra: phoenix Provides-Extra: ludwig Provides-Extra: slack Provides-
-Extra: duckdb Provides-Extra: mongodb Provides-Extra: quickbooks Provides-
-Extra: sendinblue Provides-Extra: yugabyte Provides-Extra: matrixone Provides-
-Extra: openai Provides-Extra: reddit Provides-Extra: elasticsearch Provides-
-Extra: singlestore Provides-Extra: google_content_shopping Provides-Extra:
-langchain Provides-Extra: rocket_chat Provides-Extra: frappe Provides-Extra:
-ray_serve Provides-Extra: nuo_jdbc Provides-Extra: dremio Provides-Extra:
-timescaledb Provides-Extra: rockset Provides-Extra: druid Provides-Extra: ckan
-Provides-Extra: tdengine Provides-Extra: mssql Provides-Extra: oracle Provides-
-Extra: google_calendar Provides-Extra: sqlany Provides-Extra: jira Provides-
-Extra: planetscale Provides-Extra: autosklearn Provides-Extra: hive Provides-
-Extra: opengauss Provides-Extra: hana Provides-Extra: empress Provides-Extra:
-google_search Provides-Extra: gitlab Provides-Extra: airtable Provides-Extra:
-llama_index Provides-Extra: couchbase Provides-Extra: ignite Provides-Extra:
-cassandra Provides-Extra: monkeylearn Provides-Extra: tpot Provides-Extra:
-altibase Provides-Extra: snowflake Provides-Extra: teradata Provides-Extra:
+Extra: all_extras Provides-Extra: empress Provides-Extra: solr Provides-Extra:
+access Provides-Extra: binance Provides-Extra: yugabyte Provides-Extra:
+bigquery Provides-Extra: timescaledb Provides-Extra: github Provides-Extra:
+cohere Provides-Extra: snowflake Provides-Extra: quickbooks Provides-Extra:
+clickhouse Provides-Extra: sendinblue Provides-Extra: youtube Provides-Extra:
+monetdb Provides-Extra: aurora Provides-Extra: s3 Provides-Extra: autosklearn
+Provides-Extra: dremio Provides-Extra: paypal Provides-Extra: rocket_chat
+Provides-Extra: edgelessdb Provides-Extra: cockroach Provides-Extra:
+planetscale Provides-Extra: google_books Provides-Extra: ray_serve Provides-
+Extra: starrocks Provides-Extra: huggingface_api Provides-Extra: hive Provides-
+Extra: altibase Provides-Extra: mariadb Provides-Extra: ignite Provides-Extra:
+strava Provides-Extra: firebird Provides-Extra: tidb Provides-Extra: crate
+Provides-Extra: influxdb Provides-Extra: neuralforecast Provides-Extra: merlion
+Provides-Extra: vertica Provides-Extra: sheets Provides-Extra: hana Provides-
+Extra: pinot Provides-Extra: confluence Provides-Extra: opengauss Provides-
+Extra: redshift Provides-Extra: trino Provides-Extra: slack Provides-Extra:
+datastax Provides-Extra: questdb Provides-Extra: nuo_jdbc Provides-Extra:
+orioledb Provides-Extra: teradata Provides-Extra: gmail Provides-Extra: oracle
+Provides-Extra: flaml Provides-Extra: langchain Provides-Extra: impala
+Provides-Extra: cloud_spanner Provides-Extra: ingres Provides-Extra: tdengine
+Provides-Extra: google_fit Provides-Extra: google_search Provides-Extra: db2
+Provides-Extra: tpot Provides-Extra: shopify Provides-Extra:
+google_content_shopping Provides-Extra: google_calendar Provides-Extra: ckan
+Provides-Extra: cassandra Provides-Extra: rockset Provides-Extra: monkeylearn
+Provides-Extra: sqlany Provides-Extra: mssql Provides-Extra: huggingface
+Provides-Extra: postgres Provides-Extra: ludwig Provides-Extra: airtable
+Provides-Extra: mysql Provides-Extra: phoenix Provides-Extra: singlestore
+Provides-Extra: oceanbase Provides-Extra: vitess Provides-Extra: newsapi
+Provides-Extra: druid Provides-Extra: hsqldb Provides-Extra: statsforecast
+Provides-Extra: materialize Provides-Extra: openai Provides-Extra: databricks
+Provides-Extra: jira Provides-Extra: scylla Provides-Extra: twitter Provides-
+Extra: gitlab Provides-Extra: surrealdb Provides-Extra: plaid Provides-Extra:
+duckdb Provides-Extra: d0lt Provides-Extra: databend Provides-Extra: stripe
+Provides-Extra: mendeley Provides-Extra: maxdb Provides-Extra: derby Provides-
+Extra: mlflow Provides-Extra: writer Provides-Extra: couchbase Provides-Extra:
+dynamodb Provides-Extra: sqreamdb Provides-Extra: mongodb Provides-Extra:
+cloud_sql Provides-Extra: llama_index Provides-Extra: supabase Provides-Extra:
+matrixone Provides-Extra: informix Provides-Extra: elasticsearch Provides-
+Extra: reddit Provides-Extra: frappe Provides-Extra: lightwood Provides-Extra:
 all_handlers_extras
```

### Comparing `MindsDB-23.6.3.0/README.md` & `MindsDB-23.6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/__main__.py` & `MindsDB-23.6.3.1/mindsdb/__main__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/common/check_auth.py` & `MindsDB-23.6.3.1/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/gui.py` & `MindsDB-23.6.3.1/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-23.6.3.1/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/initialize.py` & `MindsDB-23.6.3.1/mindsdb/api/http/initialize.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/auth.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/config.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/databases.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/default.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/file.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/models.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/models.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/projects.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/sql.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/tab.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/tree.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/util.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/namespaces/views.py` & `MindsDB-23.6.3.1/mindsdb/api/http/namespaces/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/start.py` & `MindsDB-23.6.3.1/mindsdb/api/http/start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/http/utils.py` & `MindsDB-23.6.3.1/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/classes/responder.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/classes/scram.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/classes/session.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/delete.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/find.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/insert.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/server.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-23.6.3.1/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/data_types.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/data_types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/functions.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/mysql/mysql_proxy/utilities/sql.py` & `MindsDB-23.6.3.1/mindsdb/api/mysql/mysql_proxy/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/nlp/nlp.py` & `MindsDB-23.6.3.1/mindsdb/api/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-23.6.3.1/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/autokeras_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/autokeras_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/autosklearn_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/autosklearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/logo.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/logo.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/logo.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/logo.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cohere_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cohere_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cohere_handler/cohere_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/cohere_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/cohere_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/confluence_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/confluence_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/create-db.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/predict-target.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/logo.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/flaml_handler/flaml_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/flaml_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/flaml_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_client.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/frappe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/frappe_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/frappe_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/github_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/github_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/gitlab_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/gitlab_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/gitlab_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/gmail_handler/tests/test_gmail_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/google_books_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_books_handler/tests/test_google_books_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
                 start_id = int(params['start_id'])
                 end_id = int(params['end_id'])
             for i in range(start_id, end_id):
                 service.events().delete(calendarId='primary', eventId=str(i)).execute()
                 df = pd.concat([df, pd.DataFrame([{'eventId': str(i), 'status': 'deleted'}])], ignore_index=True)
             return df
 
-    def call_application_api(self, method_name: str = None, params: dict = None) -> DataFrame:
+    def call_application_api(self, method_name: str = None, params: dict = None) -> pd.DataFrame:
         """
         Call Google Calendar API and map the data to pandas DataFrame
         Args:
             method_name (str): method name
             params (dict): query parameters
         Returns:
             DataFrame
```

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/google_content_shopping_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_content_shopping_handler/tests/test_google_content_shopping_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/google_fit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_fit_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_fit_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/google_search_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/google_search_handler/tests/test_google_search_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hackernews_handler/hn_table.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hackernews_handler/hn_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hackernews_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hackernews_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/huggingface_api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_api_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_api_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/huggingface_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/huggingface_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/jira_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/jira_handler/jira_table.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/jira_handler/jira_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/mindsdb_database_agent.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/langchain_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/langchain_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/llama_index_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/llama_index_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/llama_index_handler/llama_index_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/llama_index_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/llama_index_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ludwig_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ludwig_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/maxdb_handler/tests/test_maxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/mendeley_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mendeley_handler/tests/test_mendeley_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/merlion_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/merlion_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mlflow_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mlflow_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/create-database.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/create-database.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/select-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monkeylearn_handler/monkeylearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/monkeylearn_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/monkeylearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/neuralforecast_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/neuralforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/newsapi_handler/tests/test_newsapi_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/openai_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/openai_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/paypal_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/paypal_handler/paypal_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/create-db.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/create-predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/drop-db.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/drop-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/planetscale_handler/predict-target.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/planetscale_handler/predict-target.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/quickbooks_handler/quickbooks_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/ray_serve_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/ray_serve_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/rocket_chat_handler/rocket_chat_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/rockset_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/rockset_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/logo.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sendinblue_handler/sendinblue_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/shopify_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/shopify_handler/shopify_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/slack_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/slack_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/slack_handler/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/solr.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/solr.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/db_connection.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/db_connection.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/error.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/error.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/model_drop.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/model_drop.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/statsforecast_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/statsforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/strava_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/strava_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/strava_handler/strava_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/strava_handler/strava_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/stripe_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/stripe_handler/stripe_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/teradata_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/teradata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/tpot_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/tpot_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/twitter_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/twitter_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/utilities/query_utilities/select_query_utilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/ingest.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/ingest.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/question_answer.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/question_answer.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/settings.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/settings.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/setup.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/writer_handler/writer_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/writer_handler/writer_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/__init__.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/icon.png` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/youtube_handler/youtube_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/ml_client_factory.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/ml_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers_client/ml_grpc_client.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers_client/ml_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-23.6.3.1/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/libs/api_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/libs/api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/libs/base.py` & `MindsDB-23.6.3.1/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-23.6.3.1/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-23.6.3.1/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/libs/ml_handler_proc.py` & `MindsDB-23.6.3.1/mindsdb/integrations/libs/ml_handler_proc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-23.6.3.1/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/libs/response.py` & `MindsDB-23.6.3.1/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-23.6.3.1/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-23.6.3.1/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/utilities/install.py` & `MindsDB-23.6.3.1/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-23.6.3.1/mindsdb/integrations/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-23.6.3.1/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-23.6.3.1/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/chatbot/chatbot_controller.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/chatbot/chatbot_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/chatbot/chatbot_monitor.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/chatbot/chatbot_monitor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/chatbot/chatbot_task.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/chatbot/chatbot_task.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/database/database.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/database/integrations.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/database/integrations.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/database/projects.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/database/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/database/views.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/file/file_controller.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/model/functions.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/model/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/model/model_controller.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/model/model_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/storage/db.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/storage/db.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/storage/fs.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/storage/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/storage/json.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/stream/base/integration.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/stream/base/integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/interfaces/stream/stream.py` & `MindsDB-23.6.3.1/mindsdb/interfaces/stream/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-23.6.3.1/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-23.6.3.1/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-23.6.3.1/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-23.6.3.1/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-23.6.3.1/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-23.6.3.1/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-23.6.3.1/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-23.6.3.1/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/alembic.ini` & `MindsDB-23.6.3.1/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/env.py` & `MindsDB-23.6.3.1/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/migrate.py` & `MindsDB-23.6.3.1/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-05-24_6d748f2c7b0b_remove_streams.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py` & `MindsDB-23.6.3.1/mindsdb/migrations/versions/2023-05-31_aaecd7012a78_chatbot.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/auth.py` & `MindsDB-23.6.3.1/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/cache.py` & `MindsDB-23.6.3.1/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/config.py` & `MindsDB-23.6.3.1/mindsdb/utilities/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/context.py` & `MindsDB-23.6.3.1/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/fs.py` & `MindsDB-23.6.3.1/mindsdb/utilities/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/functions.py` & `MindsDB-23.6.3.1/mindsdb/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/hooks/profiling.py` & `MindsDB-23.6.3.1/mindsdb/utilities/hooks/profiling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/json_encoder.py` & `MindsDB-23.6.3.1/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/log.py` & `MindsDB-23.6.3.1/mindsdb/utilities/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/log_controller.py` & `MindsDB-23.6.3.1/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/profiler/profiler.py` & `MindsDB-23.6.3.1/mindsdb/utilities/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/ps.py` & `MindsDB-23.6.3.1/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/telemetry.py` & `MindsDB-23.6.3.1/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/mindsdb/utilities/wizards.py` & `MindsDB-23.6.3.1/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/requirements/requirements.txt` & `MindsDB-23.6.3.1/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `MindsDB-23.6.3.0/setup.py` & `MindsDB-23.6.3.1/setup.py`

 * *Files identical despite different names*

