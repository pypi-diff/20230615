# Comparing `tmp/globus-cli-3.8.0.tar.gz` & `tmp/globus-cli-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-cli-3.8.0.tar", last modified: Wed Aug 31 19:57:41 2022, max compression
+gzip compressed data, was "globus-cli-3.9.0.tar", last modified: Thu Oct 13 19:54:04 2022, max compression
```

## Comparing `globus-cli-3.8.0.tar` & `globus-cli-3.9.0.tar`

### file list

```diff
@@ -1,220 +1,231 @@
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.357107 globus-cli-3.8.0/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11357 2018-06-22 20:40:13.000000 globus-cli-3.8.0/LICENSE
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2362 2022-08-31 19:57:41.357107 globus-cli-3.8.0/PKG-INFO
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1632 2022-02-18 18:39:30.000000 globus-cli-3.8.0/README.rst
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      611 2022-08-31 19:57:41.357107 globus-cli-3.8.0/setup.cfg
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2198 2022-08-30 16:41:57.000000 globus-cli-3.8.0/setup.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.329107 globus-cli-3.8.0/src/
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.333107 globus-cli-3.8.0/src/globus_cli/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      115 2022-05-11 22:34:48.000000 globus-cli-3.8.0/src/globus_cli/__init__.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.337107 globus-cli-3.8.0/src/globus_cli/commands/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1491 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2777 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10017 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/api.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.337107 globus-cli-3.8.0/src/globus_cli/commands/bookmark/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      401 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/bookmark/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1473 2022-08-08 18:20:27.000000 globus-cli-3.8.0/src/globus_cli/commands/bookmark/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2161 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/bookmark/create.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1058 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/bookmark/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1742 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/bookmark/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1068 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/bookmark/rename.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1863 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/bookmark/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3559 2022-08-31 15:54:18.000000 globus-cli-3.8.0/src/globus_cli/commands/cli_profile_list.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.337107 globus-cli-3.8.0/src/globus_cli/commands/collection/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      361 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/collection/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      693 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/collection/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3088 2022-05-12 18:05:07.000000 globus-cli-3.8.0/src/globus_cli/commands/collection/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3206 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/collection/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8989 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/collection/update.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5750 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/delete.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.341107 globus-cli-3.8.0/src/globus_cli/commands/endpoint/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1018 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10050 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10636 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/activate.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3563 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/create.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      901 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/deactivate.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1017 2022-05-11 21:57:50.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4137 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/is_activated.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1694 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/local_id.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1008 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/my_shared_endpoint_list.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.341107 globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      425 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3309 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/create.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1099 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1547 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1529 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1413 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/update.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.341107 globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      323 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2621 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/create.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1127 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1957 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1731 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3695 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/search.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.341107 globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      629 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3146 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1844 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/add.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3441 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1548 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2377 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1884 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/update.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1703 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/set_subscription_id.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1956 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1448 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/endpoint/update.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3647 2022-06-24 13:34:44.000000 globus-cli-3.8.0/src/globus_cli/commands/get_identities.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.345107 globus-cli-3.8.0/src/globus_cli/commands/group/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      619 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/group/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1870 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/group/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      645 2022-02-18 18:39:30.000000 globus-cli-3.8.0/src/globus_cli/commands/group/create.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      543 2022-02-18 18:39:30.000000 globus-cli-3.8.0/src/globus_cli/commands/group/delete.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.345107 globus-cli-3.8.0/src/globus_cli/commands/group/invite/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      267 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/group/invite/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1867 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/group/invite/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1555 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/group/invite/accept.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1566 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/group/invite/decline.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2150 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/group/join.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2909 2022-08-08 18:27:06.000000 globus-cli-3.8.0/src/globus_cli/commands/group/leave.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1072 2022-02-18 18:39:30.000000 globus-cli-3.8.0/src/globus_cli/commands/group/list.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.345107 globus-cli-3.8.0/src/globus_cli/commands/group/member/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      440 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/group/member/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1902 2022-05-12 18:05:07.000000 globus-cli-3.8.0/src/globus_cli/commands/group/member/add.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1741 2022-05-12 18:05:07.000000 globus-cli-3.8.0/src/globus_cli/commands/group/member/approve.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2095 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/group/member/invite.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1399 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/group/member/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1686 2022-05-12 18:05:07.000000 globus-cli-3.8.0/src/globus_cli/commands/group/member/reject.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1657 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/group/member/remove.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3088 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/group/set_policies.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1220 2022-05-12 18:05:07.000000 globus-cli-3.8.0/src/globus_cli/commands/group/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1144 2022-02-18 18:39:30.000000 globus-cli-3.8.0/src/globus_cli/commands/group/update.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3015 2022-05-11 22:04:07.000000 globus-cli-3.8.0/src/globus_cli/commands/list_commands.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3703 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/login.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5304 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/logout.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6723 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/ls.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1094 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/mkdir.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1368 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/rename.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3712 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/rm.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.345107 globus-cli-3.8.0/src/globus_cli/commands/search/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      483 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/search/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1446 2022-08-08 18:23:06.000000 globus-cli-3.8.0/src/globus_cli/commands/search/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2072 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/search/delete_by_query.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.345107 globus-cli-3.8.0/src/globus_cli/commands/search/index/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      374 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/search/index/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      751 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/search/index/create.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      631 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/search/index/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      700 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/search/index/list.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.349107 globus-cli-3.8.0/src/globus_cli/commands/search/index/role/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      290 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/search/index/role/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2871 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/search/index/role/create.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      687 2022-02-18 21:34:38.000000 globus-cli-3.8.0/src/globus_cli/commands/search/index/role/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      885 2022-02-18 21:34:38.000000 globus-cli-3.8.0/src/globus_cli/commands/search/index/role/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      613 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/search/index/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1840 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/search/ingest.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3625 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/search/query.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.349107 globus-cli-3.8.0/src/globus_cli/commands/search/subject/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      328 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/search/subject/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1170 2022-05-27 23:00:42.000000 globus-cli-3.8.0/src/globus_cli/commands/search/subject/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1255 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/search/subject/show.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.349107 globus-cli-3.8.0/src/globus_cli/commands/search/task/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      227 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/search/task/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      840 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/search/task/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      883 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/search/task/show.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.349107 globus-cli-3.8.0/src/globus_cli/commands/session/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      308 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/session/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1272 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/session/consent.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3051 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/session/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4883 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/session/update.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.349107 globus-cli-3.8.0/src/globus_cli/commands/task/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      572 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/commands/task/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      437 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/task/_common.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3317 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/task/cancel.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3319 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/task/event_list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1305 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/task/generate_submission_id.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6542 2022-08-29 17:53:20.000000 globus-cli-3.8.0/src/globus_cli/commands/task/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3519 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/task/pause_info.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4874 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/task/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1273 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/task/update.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1675 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/task/wait.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.349107 globus-cli-3.8.0/src/globus_cli/commands/timer/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      348 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/commands/timer/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2613 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/commands/timer/_common.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.349107 globus-cli-3.8.0/src/globus_cli/commands/timer/create/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      218 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/commands/timer/create/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6800 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/commands/timer/create/transfer.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      783 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/timer/delete.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      655 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/timer/list.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      648 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/commands/timer/show.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12035 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/commands/transfer.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6835 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/update.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3241 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/commands/version.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3334 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/commands/whoami.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      612 2022-05-12 18:05:07.000000 globus-cli-3.8.0/src/globus_cli/constants.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.353107 globus-cli-3.8.0/src/globus_cli/endpointish/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      850 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/endpointish/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2426 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/endpointish/endpoint_type.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2354 2022-08-08 18:24:04.000000 globus-cli-3.8.0/src/globus_cli/endpointish/endpointish.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2472 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/endpointish/errors.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.353107 globus-cli-3.8.0/src/globus_cli/exception_handling/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2142 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/exception_handling/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9781 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/exception_handling/hooks.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2191 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/exception_handling/registry.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1240 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/globus_cli_flake8.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.353107 globus-cli-3.8.0/src/globus_cli/login_manager/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      557 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/login_manager/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2027 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/login_manager/_old_config.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4244 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/login_manager/auth_flows.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1364 2022-08-08 18:27:05.000000 globus-cli-3.8.0/src/globus_cli/login_manager/client_login.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      839 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/login_manager/errors.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9279 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/login_manager/local_server.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12258 2022-08-31 18:46:23.000000 globus-cli-3.8.0/src/globus_cli/login_manager/manager.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5869 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/login_manager/tokenstore.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      108 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/login_manager/utils.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.353107 globus-cli-3.8.0/src/globus_cli/parsing/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1928 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6536 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/parsing/command_state.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8887 2022-08-31 18:38:56.000000 globus-cli-3.8.0/src/globus_cli/parsing/commands.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2515 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/parsing/mutex_group.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2753 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/one_use_option.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.353107 globus-cli-3.8.0/src/globus_cli/parsing/param_types/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      749 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/param_types/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1692 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/parsing/param_types/comma_delimited.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2013 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/param_types/endpoint_plus_path.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2590 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/param_types/identity_type.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      581 2022-08-16 18:28:32.000000 globus-cli-3.8.0/src/globus_cli/parsing/param_types/location.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1988 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/param_types/nullable.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2814 2022-08-08 18:16:56.000000 globus-cli-3.8.0/src/globus_cli/parsing/param_types/prefix_mapper.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4157 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/param_types/task_path.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1004 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/param_types/timedelta.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.353107 globus-cli-3.8.0/src/globus_cli/parsing/shared_options/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    14013 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/shared_options/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3869 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/shared_options/transfer_task_options.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3067 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/parsing/shell_completion.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4192 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/principal_resolver.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.357107 globus-cli-3.8.0/src/globus_cli/services/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/services/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1220 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/services/auth.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2020 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/services/gcs.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.357107 globus-cli-3.8.0/src/globus_cli/services/transfer/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      909 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/services/transfer/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3174 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/services/transfer/activation.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3958 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/services/transfer/client.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1970 2022-08-31 19:55:17.000000 globus-cli-3.8.0/src/globus_cli/services/transfer/data.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9467 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/services/transfer/delegate_proxy.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5913 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/services/transfer/recursive_ls.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.357107 globus-cli-3.8.0/src/globus_cli/termio/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1325 2022-06-13 18:43:55.000000 globus-cli-3.8.0/src/globus_cli/termio/__init__.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4457 2022-06-01 15:15:58.000000 globus-cli-3.8.0/src/globus_cli/termio/awscli_text.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2057 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/termio/context.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1903 2022-02-07 21:41:17.000000 globus-cli-3.8.0/src/globus_cli/termio/errors.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11298 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/termio/output_formatter.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      911 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/types.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5675 2022-08-18 18:07:31.000000 globus-cli-3.8.0/src/globus_cli/utils.py
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1332 2022-08-31 19:55:45.000000 globus-cli-3.8.0/src/globus_cli/version.py
-drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-08-31 19:57:41.333107 globus-cli-3.8.0/src/globus_cli.egg-info/
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2362 2022-08-31 19:57:41.000000 globus-cli-3.8.0/src/globus_cli.egg-info/PKG-INFO
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     7910 2022-08-31 19:57:41.000000 globus-cli-3.8.0/src/globus_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2022-08-31 19:57:41.000000 globus-cli-3.8.0/src/globus_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       43 2022-08-31 19:57:41.000000 globus-cli-3.8.0/src/globus_cli.egg-info/entry_points.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      208 2022-08-31 19:57:41.000000 globus-cli-3.8.0/src/globus_cli.egg-info/requires.txt
--rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       11 2022-08-31 19:57:41.000000 globus-cli-3.8.0/src/globus_cli.egg-info/top_level.txt
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.614527 globus-cli-3.9.0/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11357 2018-06-22 20:40:13.000000 globus-cli-3.9.0/LICENSE
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2362 2022-10-13 19:54:04.614527 globus-cli-3.9.0/PKG-INFO
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1632 2022-02-18 18:39:30.000000 globus-cli-3.9.0/README.rst
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      611 2022-10-13 19:54:04.614527 globus-cli-3.9.0/setup.cfg
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2395 2022-10-13 17:19:29.000000 globus-cli-3.9.0/setup.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.570527 globus-cli-3.9.0/src/
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.574527 globus-cli-3.9.0/src/globus_cli/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      115 2022-05-11 22:34:48.000000 globus-cli-3.9.0/src/globus_cli/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.582527 globus-cli-3.9.0/src/globus_cli/commands/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1575 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3205 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10017 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/api.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.582527 globus-cli-3.9.0/src/globus_cli/commands/bookmark/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      401 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/bookmark/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1473 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/bookmark/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2161 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/bookmark/create.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1058 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/bookmark/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1742 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/bookmark/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1068 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/bookmark/rename.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1863 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/bookmark/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3559 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/cli_profile_list.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.582527 globus-cli-3.9.0/src/globus_cli/commands/collection/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      361 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/collection/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      693 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/collection/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3088 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/collection/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3206 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/collection/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8989 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/collection/update.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5750 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/delete.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.586527 globus-cli-3.9.0/src/globus_cli/commands/endpoint/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1018 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8027 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    10636 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/activate.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3754 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/create.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      901 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/deactivate.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1017 2022-05-11 21:57:50.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4137 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/is_activated.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1694 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/local_id.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1008 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/my_shared_endpoint_list.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.586527 globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      425 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3309 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/create.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1099 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1547 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1529 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1413 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/update.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.586527 globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      323 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       75 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2621 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/create.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1127 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1957 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1731 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3695 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/search.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.590527 globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      629 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3146 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1844 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/add.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3441 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1548 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2377 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1884 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/update.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1703 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/set_subscription_id.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1956 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1502 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/endpoint/update.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.590527 globus-cli-3.9.0/src/globus_cli/commands/flows/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      205 2022-10-13 19:14:43.000000 globus-cli-3.9.0/src/globus_cli/commands/flows/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      400 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/flows/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1654 2022-10-13 19:14:43.000000 globus-cli-3.9.0/src/globus_cli/commands/flows/list.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.590527 globus-cli-3.9.0/src/globus_cli/commands/gcp/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      209 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/gcp/__init__.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.590527 globus-cli-3.9.0/src/globus_cli/commands/gcp/create/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      263 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/gcp/create/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2178 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/gcp/create/guest.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2409 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/gcp/create/mapped.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3647 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/get_identities.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.594527 globus-cli-3.9.0/src/globus_cli/commands/group/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      619 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1870 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      645 2022-02-18 18:39:30.000000 globus-cli-3.9.0/src/globus_cli/commands/group/create.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      543 2022-02-18 18:39:30.000000 globus-cli-3.9.0/src/globus_cli/commands/group/delete.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.594527 globus-cli-3.9.0/src/globus_cli/commands/group/invite/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      267 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/invite/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1867 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/invite/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1555 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/invite/accept.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1566 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/invite/decline.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2150 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/join.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2909 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/leave.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1072 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/group/list.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.594527 globus-cli-3.9.0/src/globus_cli/commands/group/member/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      440 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/member/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1902 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/member/add.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1741 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/member/approve.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2095 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/member/invite.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1399 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/member/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1686 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/member/reject.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1657 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/group/member/remove.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3088 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/set_policies.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1220 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/group/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1144 2022-02-18 18:39:30.000000 globus-cli-3.9.0/src/globus_cli/commands/group/update.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3015 2022-05-11 22:04:07.000000 globus-cli-3.9.0/src/globus_cli/commands/list_commands.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3703 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/login.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5304 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/logout.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6723 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/ls.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1094 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/mkdir.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1368 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/rename.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3712 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/rm.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.594527 globus-cli-3.9.0/src/globus_cli/commands/search/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      483 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1446 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2072 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/delete_by_query.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.598527 globus-cli-3.9.0/src/globus_cli/commands/search/index/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      374 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/index/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      751 2022-10-06 22:54:10.000000 globus-cli-3.9.0/src/globus_cli/commands/search/index/create.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      631 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/index/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      700 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/search/index/list.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.598527 globus-cli-3.9.0/src/globus_cli/commands/search/index/role/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      290 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/index/role/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2871 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/index/role/create.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      687 2022-02-18 21:34:38.000000 globus-cli-3.9.0/src/globus_cli/commands/search/index/role/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      885 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/search/index/role/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      613 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/search/index/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1840 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/search/ingest.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3625 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/query.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.598527 globus-cli-3.9.0/src/globus_cli/commands/search/subject/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      328 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/subject/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1170 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/subject/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1255 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/subject/show.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.598527 globus-cli-3.9.0/src/globus_cli/commands/search/task/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      227 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/search/task/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      840 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/search/task/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      883 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/search/task/show.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.598527 globus-cli-3.9.0/src/globus_cli/commands/session/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      308 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/session/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1272 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/session/consent.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3051 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/session/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4883 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/session/update.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.602527 globus-cli-3.9.0/src/globus_cli/commands/task/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      572 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/task/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      437 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/task/_common.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3317 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/task/cancel.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3319 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/task/event_list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1305 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/task/generate_submission_id.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6542 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/task/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3519 2022-10-10 20:40:58.000000 globus-cli-3.9.0/src/globus_cli/commands/task/pause_info.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4874 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/task/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1273 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/task/update.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1675 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/task/wait.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.602527 globus-cli-3.9.0/src/globus_cli/commands/timer/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      348 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/timer/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2295 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/timer/_common.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.602527 globus-cli-3.9.0/src/globus_cli/commands/timer/create/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      218 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/timer/create/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6800 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/timer/create/transfer.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      783 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/timer/delete.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      655 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/timer/list.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      648 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/timer/show.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12052 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/transfer.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6835 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/update.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3241 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/commands/version.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3334 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/commands/whoami.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      612 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/constants.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.602527 globus-cli-3.9.0/src/globus_cli/endpointish/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      850 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/endpointish/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2426 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/endpointish/endpoint_type.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2354 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/endpointish/endpointish.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2472 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/endpointish/errors.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.602527 globus-cli-3.9.0/src/globus_cli/exception_handling/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2142 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/exception_handling/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9781 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/exception_handling/hooks.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2191 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/exception_handling/registry.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1240 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/globus_cli_flake8.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.606527 globus-cli-3.9.0/src/globus_cli/login_manager/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      557 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/login_manager/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2027 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/login_manager/_old_config.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4244 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/login_manager/auth_flows.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1364 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/login_manager/client_login.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      839 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/login_manager/errors.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9279 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/login_manager/local_server.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    12750 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/login_manager/manager.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5869 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/login_manager/tokenstore.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      108 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/login_manager/utils.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.606527 globus-cli-3.9.0/src/globus_cli/parsing/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2073 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6536 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/command_state.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8887 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/commands.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2488 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/mutex_group.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2753 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/parsing/one_use_option.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.610527 globus-cli-3.9.0/src/globus_cli/parsing/param_types/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      749 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/param_types/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1692 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/param_types/comma_delimited.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2013 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/parsing/param_types/endpoint_plus_path.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2590 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/parsing/param_types/identity_type.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      581 2022-08-16 18:28:32.000000 globus-cli-3.9.0/src/globus_cli/parsing/param_types/location.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1988 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/parsing/param_types/nullable.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2814 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/param_types/prefix_mapper.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4157 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/parsing/param_types/task_path.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1004 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/param_types/timedelta.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.610527 globus-cli-3.9.0/src/globus_cli/parsing/shared_options/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    14013 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/shared_options/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2343 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/shared_options/endpoint_create_and_update.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3869 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/parsing/shared_options/transfer_task_options.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3067 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/parsing/shell_completion.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4192 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/principal_resolver.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.610527 globus-cli-3.9.0/src/globus_cli/services/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        0 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/services/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1220 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/services/auth.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2020 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/services/gcs.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.610527 globus-cli-3.9.0/src/globus_cli/services/transfer/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      909 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/services/transfer/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3174 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/services/transfer/activation.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     3958 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/services/transfer/client.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1970 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/services/transfer/data.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     9467 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/services/transfer/delegate_proxy.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     5913 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/services/transfer/recursive_ls.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.614527 globus-cli-3.9.0/src/globus_cli/termio/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1325 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/termio/__init__.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     4457 2022-06-01 15:15:58.000000 globus-cli-3.9.0/src/globus_cli/termio/awscli_text.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2057 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/termio/context.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1903 2022-02-07 21:41:17.000000 globus-cli-3.9.0/src/globus_cli/termio/errors.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)    11298 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/termio/output_formatter.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      911 2022-10-13 15:48:21.000000 globus-cli-3.9.0/src/globus_cli/types.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     6195 2022-10-13 19:14:43.000000 globus-cli-3.9.0/src/globus_cli/utils.py
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     1332 2022-10-13 19:53:17.000000 globus-cli-3.9.0/src/globus_cli/version.py
+drwxrwxr-x   0 sirosen  (10000) sirosen  (10000)        0 2022-10-13 19:54:04.578527 globus-cli-3.9.0/src/globus_cli.egg-info/
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     2362 2022-10-13 19:54:04.000000 globus-cli-3.9.0/src/globus_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)     8275 2022-10-13 19:54:04.000000 globus-cli-3.9.0/src/globus_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)        1 2022-10-13 19:54:04.000000 globus-cli-3.9.0/src/globus_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       43 2022-10-13 19:54:04.000000 globus-cli-3.9.0/src/globus_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)      259 2022-10-13 19:54:04.000000 globus-cli-3.9.0/src/globus_cli.egg-info/requires.txt
+-rw-rw-r--   0 sirosen  (10000) sirosen  (10000)       11 2022-10-13 19:54:04.000000 globus-cli-3.9.0/src/globus_cli.egg-info/top_level.txt
```

### Comparing `globus-cli-3.8.0/LICENSE` & `globus-cli-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/PKG-INFO` & `globus-cli-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-cli
-Version: 3.8.0
+Version: 3.9.0
 Summary: Globus CLI
 Home-page: https://github.com/globus/globus-cli
 Author: Stephen Rosen
 Author-email: sirosen@globus.org
 Keywords: globus,cli,command line
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `globus-cli-3.8.0/README.rst` & `globus-cli-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/setup.cfg` & `globus-cli-3.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/setup.py` & `globus-cli-3.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,21 +38,24 @@
 setup(
     name="globus-cli",
     version=parse_version(),
     packages=find_packages("src"),
     package_dir={"": "src"},
     python_requires=">=3.7",
     install_requires=[
-        "globus-sdk==3.11.0",
+        "globus-sdk==3.13.0",
         "click>=8.0.0,<9",
         "jmespath==0.10.0",
         # these are dependencies of the SDK, but they are used directly in the CLI
         # declare them here in case the underlying lib ever changes
         "requests>=2.19.1,<3.0.0",
         "cryptography>=3.3.1,<37",
+        # depend on the latest version of typing-extensions on python versions which do
+        # not have all of the typing features we use
+        'typing_extensions>=4.0;python_version<"3.11"',
     ],
     extras_require={"development": DEV_REQUIREMENTS},
     entry_points={"console_scripts": ["globus = globus_cli:main"]},
     # descriptive info, non-critical
     description="Globus CLI",
     long_description=read_readme(),
     author="Stephen Rosen",
```

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/__init__.py` & `globus-cli-3.9.0/src/globus_cli/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     lazy_subcommands={
         "api": ("api", "api_command"),
         "bookmark": ("bookmark", "bookmark_command"),
         "cli-profile-list": ("cli_profile_list", "cli_profile_list"),
         "collection": ("collection", "collection_command"),
         "delete": ("delete", "delete_command"),
         "endpoint": ("endpoint", "endpoint_command"),
+        "flows": ("flows", "flows_command"),
+        "gcp": ("gcp", "gcp_command"),
         "get-identities": ("get_identities", "get_identities_command"),
         "group": ("group", "group_command"),
         "list-commands": ("list_commands", "list_commands"),
         "login": ("login", "login_command"),
         "logout": ("logout", "logout_command"),
         "ls": ("ls", "ls_command"),
         "mkdir": ("mkdir", "mkdir_command"),
```

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/_common.py` & `globus-cli-3.9.0/src/globus_cli/commands/_common.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+from __future__ import annotations
+
+import datetime
 import sys
 from typing import TYPE_CHECKING
 
 import click
 
 from globus_cli.termio import FORMAT_SILENT, formatted_print
 
 if TYPE_CHECKING:
     from ..services.transfer import CustomTransferClient
 
 
 def transfer_task_wait_with_io(
-    transfer_client: "CustomTransferClient",
+    transfer_client: CustomTransferClient,
     meow,
     heartbeat,
     polling_interval,
     timeout,
     task_id,
     timeout_exit_code,
 ) -> None:
@@ -95,7 +98,19 @@
         exit_code = timeout_exit_code
 
     # output json if requested, but nothing for text mode
     res = transfer_client.get_task(task_id)
     formatted_print(res, text_format=FORMAT_SILENT)
 
     click.get_current_context().exit(exit_code)
+
+
+def isoformat_to_local(
+    utc_str: str | None, localtz: datetime.tzinfo | None = None
+) -> str | None:
+    if not utc_str:
+        return None
+    # let this raise ValueError
+    date = datetime.datetime.fromisoformat(utc_str)
+    if date.tzinfo is None:
+        return date.strftime("%Y-%m-%d %H:%M:%S")
+    return date.astimezone(tz=localtz).strftime("%Y-%m-%d %H:%M:%S")
```

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/api.py` & `globus-cli-3.9.0/src/globus_cli/commands/api.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/bookmark/_common.py` & `globus-cli-3.9.0/src/globus_cli/commands/bookmark/_common.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/bookmark/create.py` & `globus-cli-3.9.0/src/globus_cli/commands/bookmark/create.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/bookmark/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/bookmark/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/bookmark/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/bookmark/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/bookmark/rename.py` & `globus-cli-3.9.0/src/globus_cli/commands/bookmark/rename.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/bookmark/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/bookmark/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/cli_profile_list.py` & `globus-cli-3.9.0/src/globus_cli/commands/cli_profile_list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/collection/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/collection/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/collection/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/collection/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/collection/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/collection/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/collection/update.py` & `globus-cli-3.9.0/src/globus_cli/commands/collection/update.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/__init__.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/_common.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/activate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,285 +1,303 @@
 from __future__ import annotations
 
-import functools
-from typing import Callable
-
 import click
+import globus_sdk
 
-from globus_cli.constants import EXPLICIT_NULL
-from globus_cli.parsing import LocationType, MutexInfo, mutex_option_group
-
-
-def endpoint_create_and_update_params(
-    f: Callable | None = None, *, create: bool = False
-) -> Callable:
+from globus_cli.login_manager import LoginManager, is_remote_session
+from globus_cli.parsing import command, endpoint_id_arg, mutex_option_group
+from globus_cli.termio import FORMAT_TEXT_RAW, formatted_print
+
+
+@command(
+    "activate",
+    short_help="Activate an endpoint",
+    adoc_examples="""Activate an endpoint using just Automatic activation:
+
+[source,bash]
+----
+$ ep_id=ddb59aef-6d04-11e5-ba46-22000b92c6ec
+$ globus endpoint activate $ep_id
+----
+
+Activate an endpoint using Web activation
+
+[source,bash]
+----
+$ ep_id=ddb59aef-6d04-11e5-ba46-22000b92c6ec
+$ globus endpoint activate $ep_id --web
+----
+
+Activate an endpoint using Myproxy activation, skipping the username prompt.
+
+[source,bash]
+----
+$ ep_id=ddb59aef-6d04-11e5-ba46-22000b92c6ec
+$ globus endpoint activate $ep_id --myproxy -U username
+----
+""",
+)
+@endpoint_id_arg
+@click.option(
+    "--web",
+    is_flag=True,
+    default=False,
+    help="Use web activation. Mutually exclusive with --myproxy  and --delegate-proxy.",
+)
+@click.option(
+    "--no-browser",
+    is_flag=True,
+    default=False,
+    help=(
+        "If using --web, Give a url to manually follow instead of "
+        "opening your default web browser. Implied if the CLI "
+        "detects this is a remote session."
+    ),
+)
+@click.option(
+    "--myproxy",
+    is_flag=True,
+    default=False,
+    help="Use myproxy activation. Mutually exclusive with --web and --delegate-proxy.",
+)
+@click.option(
+    "--myproxy-username",
+    "-U",
+    help=("Give a username to use with --myproxy"),
+)
+@click.option("--myproxy-password", "-P", hidden=True)
+@click.option(
+    "--myproxy-lifetime",
+    type=int,
+    help=(
+        "The lifetime for the credential to request from the "
+        "server under --myproxy activation, in hours. "
+        "The myproxy server may be configured with a maximum "
+        "lifetime which it will use if this value is too high"
+    ),
+)
+@click.option(
+    "--delegate-proxy",
+    metavar="X.509_PEM_FILE",
+    help=(
+        "Use delegate proxy activation, takes an X.509 "
+        "certificate in pem format as an argument. Mutually "
+        "exclusive with --web and --myproxy."
+    ),
+)
+@click.option(
+    "--proxy-lifetime",
+    type=int,
+    default=None,
+    help=(
+        "Set a lifetime in hours for the proxy generated with "
+        "--delegate-proxy. [default: 12]"
+    ),
+)
+@click.option(
+    "--no-autoactivate",
+    is_flag=True,
+    default=False,
+    help=(
+        "Don't attempt to autoactivate endpoint before using "
+        "another activation method."
+    ),
+)
+@click.option(
+    "--force",
+    is_flag=True,
+    default=False,
+    help="Force activation even if endpoint is already activated.",
+)
+@mutex_option_group("--web", "--myproxy", "--delegate-proxy")
+@LoginManager.requires_login(LoginManager.TRANSFER_RS)
+def endpoint_activate(
+    *,
+    login_manager: LoginManager,
+    endpoint_id: str,
+    myproxy: bool,
+    myproxy_username: str | None,
+    myproxy_password: str | None,
+    myproxy_lifetime: int | None,
+    web: bool,
+    no_browser: bool,
+    delegate_proxy: bool,
+    proxy_lifetime: int | None,
+    no_autoactivate: bool,
+    force: bool,
+) -> None:
     """
-    Collection of options consumed by Transfer endpoint create and update
-    operations -- accepts toggle regarding create vs. update that makes
-    display_name required vs. optional.
-
-    Usage:
-
-    >>> @endpoint_create_and_update_params(create=True)
-    >>> def command_func(display_name, description, info_link, contact_info,
-    >>>                  contact_email, organization, department, keywords,
-    >>>                  public, location, disable_verify, myproxy_dn,
-    >>>                  myproxy_server, oauth_server, force_encryption,
-    >>>                  default_directory, subscription_id, network_use,
-    >>>                  max_concurrency, preferred_concurrency,
-    >>>                  max_parallelism, preferred_parallelism):
-    >>>     ...
+    Activate an endpoint using Autoactivation, Myproxy, Delegate Proxy,
+    or Web activation.
+    Note that --web, --delegate-proxy, and --myproxy activation are mutually
+    exclusive options.
+
+    \b
+    Autoactivation will always be attempted unless the --no-autoactivate
+    option is given. If autoactivation succeeds any other activation options
+    will be ignored as the endpoint has already been successfully activated.
+
+    \b
+    To use Web activation use the --web option.
+    The CLI will try to open your default browser to the endpoint's activation
+    page, but if a remote CLI session is detected, or the --no-browser option
+    is given, a url will be printed for you to manually follow and activate
+    the endpoint.
+
+    \b
+    To use Myproxy activation give the --myproxy option.
+    Myproxy activation requires your username and password for the myproxy
+    server the endpoint is using for authentication. e.g. for default
+    Globus Connect Server endpoints this will be your login credentials for the
+    server the endpoint is hosted on.
+    You can enter your username when prompted or give your username with the
+    --myproxy-username option.
+    For security it is recommended that you only enter your password when
+    prompted to hide your inputs and keep your password out of your
+    command history, but you may pass your password with the hidden
+    --myproxy-password or -P options.
+
+    \b
+    To use Delegate Proxy activation use the --delegate-proxy option with a
+    file containing an X.509 certificate as an argument (e.g. an X.509
+    gotten from the myproxy-logon command). This certificate must
+    be a valid credential or proxy credential for the user from an identity
+    provider accepted by the endpoint being activated, and the endpoint must be
+    configured with a gridmap that will match the globus user using this
+    command with the local user the certificate was made to. Note if the X.509
+    is valid, but the endpoint does not recognize the identity provider or the
+    user the error will not be detected until the user attempts to perform an
+    operation on the endpoint.
     """
-    if f is None:
-        return functools.partial(endpoint_create_and_update_params, create=create)
+    from globus_cli.services.transfer import (
+        activation_requirements_help_text,
+        fill_delegate_proxy_activation_requirements,
+    )
 
-    update_help_prefix = (not create and "New ") or ""
+    transfer_client = login_manager.get_transfer_client()
 
-    # display name is required for create, not update
-    if create:
-        f = click.argument("display_name")(f)
-    else:
-        f = click.option(
-            "--display-name", help=f"{update_help_prefix}Name for the endpoint"
-        )(f)
-
-    # Options available to any endpoint
-    f = click.option(
-        "--description", help=f"{update_help_prefix}Description for the endpoint"
-    )(f)
-    f = click.option(
-        "--info-link", help=f"{update_help_prefix}Link for Info about the endpoint"
-    )(f)
-    f = click.option(
-        "--contact-info", help=f"{update_help_prefix}Contact Info for the endpoint"
-    )(f)
-    f = click.option(
-        "--contact-email", help=f"{update_help_prefix}Contact Email for the endpoint"
-    )(f)
-    f = click.option(
-        "--organization", help=f"{update_help_prefix}Organization for the endpoint"
-    )(f)
-    f = click.option(
-        "--department",
-        help=f"{update_help_prefix}Department which operates the endpoint",
-    )(f)
-    f = click.option(
-        "--keywords",
-        help=f"{update_help_prefix}Comma separated list of keywords to help searches "
-        "for the endpoint",
-    )(f)
-
-    f = click.option("--default-directory", help="Set the default directory")(f)
-    f = click.option(
-        "--no-default-directory",
-        is_flag=True,
-        flag_value=True,
-        default=None,
-        help="Unset any default directory on the endpoint",
-    )(f)
-    f = mutex_option_group("--default-directory", "--no-default-directory")(f)
-
-    f = click.option(
-        "--force-encryption/--no-force-encryption",
-        default=None,
-        help="(Un)Force the endpoint to encrypt transfers",
-    )(f)
-    f = click.option(
-        "--disable-verify/--no-disable-verify",
-        default=None,
-        is_flag=True,
-        help="(Un)Set the endpoint to ignore checksum verification",
-    )(f)
-
-    # GCS only options
-    gcsonly = "(Globus Connect Server only)"
-    f = click.option(
-        "--public/--private",
-        "public",
-        default=None,
-        help=f"Set the endpoint to be public or private {gcsonly}",
-    )(f)
-    f = click.option("--myproxy-dn", help=f"Set the MyProxy Server DN {gcsonly}")(f)
-    f = click.option("--myproxy-server", help=f"Set the MyProxy Server URI {gcsonly}")(
-        f
-    )
-    f = click.option("--oauth-server", help=f"Set the OAuth Server URI {gcsonly}")(f)
-    f = click.option(
-        "--location",
-        type=LocationType(),
-        default=None,
-        help=f"Manually set the endpoint's latitude and longitude {gcsonly}",
-    )(f)
-
-    # Managed Endpoint options
-    f = click.option(
-        "--managed",
-        "managed",
-        is_flag=True,
-        flag_value=True,
-        default=None,
-        help=(
-            "Set the endpoint as a managed endpoint. Requires the "
-            "user to be a subscription manager. If the user has "
-            "multiple subscription IDs, --subscription-id must be used "
-            "instead"
-        ),
-    )(f)
-    f = click.option(
-        "--no-managed",
-        "managed",
-        is_flag=True,
-        flag_value=False,
-        default=None,
-        help=(
-            "Unset the endpoint as a managed endpoint. "
-            "Does not require the user to be a subscription manager. "
-            "Mutually exclusive with --subscription-id"
-        ),
-    )(f)
-    f = click.option(
-        "--subscription-id",
-        type=click.UUID,
-        default=None,
-        help="Set the endpoint as a managed endpoint with the given "
-        "subscription ID. Mutually exclusive with --no-managed",
-    )(f)
-    f = mutex_option_group(
-        "--subscription-id",
-        MutexInfo(
-            "--no-managed", param="managed", present=lambda d: d.get("managed") is False
-        ),
-    )(f)
-
-    managedonly = "(Managed endpoints only)"
-    f = click.option(
-        "--network-use",
-        default=None,
-        type=click.Choice(["normal", "minimal", "aggressive", "custom"]),
-        help=(
-            "Set the endpoint's network use level. If using custom, "
-            "the endpoint's max and preferred concurrency and "
-            f"parallelism must be set {managedonly} {gcsonly}"
-        ),
-    )(f)
-    f = click.option(
-        "--max-concurrency",
-        type=int,
-        default=None,
-        help="Set the endpoint's max concurrency; requires --network-use=custom "
-        f"{managedonly} {gcsonly}",
-    )(f)
-    f = click.option(
-        "--preferred-concurrency",
-        type=int,
-        default=None,
-        help="Set the endpoint's preferred concurrency; requires --network-use=custom "
-        f"{managedonly} {gcsonly}",
-    )(f)
-    f = click.option(
-        "--max-parallelism",
-        type=int,
-        default=None,
-        help="Set the endpoint's max parallelism; requires --network-use=custom "
-        f"{managedonly} {gcsonly}",
-    )(f)
-    f = click.option(
-        "--preferred-parallelism",
-        type=int,
-        default=None,
-        help="Set the endpoint's preferred parallelism; requires --network-use=custom "
-        f"{managedonly} {gcsonly}",
-    )(f)
+    # validate options
+    if no_autoactivate and not (myproxy or web or delegate_proxy):
+        raise click.UsageError(
+            "--no-autoactivate requires another activation method be given."
+        )
+    if myproxy_username and not myproxy:
+        raise click.UsageError("--myproxy-username requires --myproxy.")
+    if myproxy_password and not myproxy:
+        raise click.UsageError("--myproxy-password requires --myproxy.")
+    # NOTE: "0" is a legitimate, though weird, value
+    # In the case where someone is setting this value programatically,
+    # respecting it behaves more consistently/predictably
+    if myproxy_lifetime is not None and not myproxy:
+        raise click.UsageError("--myproxy-lifetime requires --myproxy.")
+    if no_browser and not web:
+        raise click.UsageError("--no-browser requires --web.")
+    if proxy_lifetime and not delegate_proxy:
+        raise click.UsageError("--proxy-lifetime requires --delegate-proxy.")
+
+    # check if endpoint is already activated unless --force
+    if not force:
+        res: (
+            dict[str, str] | globus_sdk.GlobusHTTPResponse
+        ) = transfer_client.endpoint_autoactivate(endpoint_id, if_expires_in=60)
+
+        if "AlreadyActivated" == res["code"]:
+            formatted_print(
+                res,
+                simple_text=(
+                    "Endpoint is already activated. Activation "
+                    "expires at {}".format(res["expire_time"])
+                ),
+            )
+            return
 
-    return f
+    # attempt autoactivation unless --no-autoactivate
+    if not no_autoactivate:
 
+        res = transfer_client.endpoint_autoactivate(endpoint_id)
 
-def validate_endpoint_create_and_update_params(
-    endpoint_type: str, managed: bool, params: dict
-) -> None:
-    """
-    Given an endpoint type of "shared" "server" or "personal" and option values
-    Confirms the option values are valid for the given endpoint
-    """
-    # options only allowed for GCS endpoints
-    if endpoint_type != "server":
-        # catch params with two option flags
-        if params["public"] is False:
-            raise click.UsageError(
-                "Option --private only allowed for Globus Connect Server endpoints"
+        if "AutoActivated" in res["code"]:
+            formatted_print(
+                res,
+                simple_text=(
+                    "Autoactivation succeeded with message: {}".format(res["message"])
+                ),
             )
-        # catch any params only usable with GCS
-        for option in [
-            "public",
-            "myproxy_dn",
-            "myproxy_server",
-            "oauth_server",
-            "location",
-            "network_use",
-            "max_concurrency",
-            "preferred_concurrency",
-            "max_parallelism",
-            "preferred_parallelism",
-        ]:
-            if params[option] is not None:
-                raise click.UsageError(
-                    f"Option --{option.replace('_', '-')} can only be used with "
-                    "Globus Connect Server endpoints"
-                )
+            return
 
-    # if the endpoint was not previously managed, and is not being passed
-    # a subscription id, it cannot use managed endpoint only fields
-    if (not managed) and not (params["subscription_id"] or params["managed"]):
-        for option in [
-            "network_use",
-            "max_concurrency",
-            "preferred_concurrency",
-            "max_parallelism",
-            "preferred_parallelism",
-        ]:
-            if params[option] is not None:
-                raise click.UsageError(
-                    f"Option --{option.replace('_', '-')} can only be used with "
-                    "managed endpoints"
-                )
+        # override potentially confusing autoactivation failure response
+        else:
+            message = (
+                "The endpoint could not be auto-activated.\n\n"
+                + activation_requirements_help_text(res, endpoint_id)
+            )
+            res = {"message": message}
 
-    # because the Transfer service doesn't do network use level updates in a
-    # patchy way, *both* endpoint `POST`s *and* `PUT`s must either use
-    # - `network_use='custom'` with *every* other parameter specified (which
-    #   is validated by the service), or
-    # - a preset/absent `network_use` with *no* other parameter specified
-    #   (which is *not* validated by the service; in this case, Transfer will
-    #   accept but ignore the others parameters if given, leading to user
-    #   confusion if we don't do this validation check)
-    custom_network_use_params = (
-        "max_concurrency",
-        "preferred_concurrency",
-        "max_parallelism",
-        "preferred_parallelism",
-    )
-    if params["network_use"] != "custom":
-        for option in custom_network_use_params:
-            if params[option] is not None:
-                raise click.UsageError(
-                    "The {} options require you use --network-use=custom.".format(
-                        "/".join(
-                            "--" + option.replace("_", "-")
-                            for option in custom_network_use_params
-                        )
-                    )
-                )
+    # myproxy activation
+    if myproxy:
+        # fetch activation requirements
+        requirements_data = transfer_client.endpoint_get_activation_requirements(
+            endpoint_id
+        ).data
+        # filter to the myproxy requirements; ensure that there are values
+        myproxy_requirements_data = [
+            x for x in requirements_data["DATA"] if x["type"] == "myproxy"
+        ]
+        if not len(myproxy_requirements_data):
+            raise click.ClickException(
+                "This endpoint does not support myproxy activation"
+            )
 
-    # resolve the subscription_id value if "managed" was set
-    # if --managed given pass --subscription-id or DEFAULT
-    # if --no-managed given, pass explicit null
-    managed_flag = params.get("managed")
-    if managed_flag is not None:
-        params.pop("managed")
-        if managed_flag:
-            params["subscription_id"] = params.get("subscription_id") or "DEFAULT"
+        # get username and password
+        if not myproxy_username:
+            myproxy_username = click.prompt("Myproxy username")
+        if not myproxy_password:
+            myproxy_password = click.prompt("Myproxy password", hide_input=True)
+
+        # fill out the requirements data -- note that because everything has been done
+        # by reference, `requirements_data` still refers to the document containing
+        # these values
+        for data in myproxy_requirements_data:
+            if data["name"] == "passphrase":
+                data["value"] = myproxy_password
+            if data["name"] == "username":
+                data["value"] = myproxy_username
+            if data["name"] == "hostname" and data["value"] is None:
+                raise click.ClickException(
+                    "This endpoint has no myproxy server "
+                    "and so cannot be activated through myproxy"
+                )
+            # NOTE: remember that "0" is a possible value
+            if data["name"] == "lifetime_in_hours" and myproxy_lifetime is not None:
+                data["value"] = str(myproxy_lifetime)
+
+        res = transfer_client.endpoint_activate(
+            endpoint_id, requirements_data=requirements_data
+        )
+
+    # web activation
+    elif web:
+        import webbrowser
+
+        from globus_sdk.config import get_webapp_url
+
+        url = f"{get_webapp_url()}file-manager?origin_id={endpoint_id}"
+        if no_browser or is_remote_session():
+            res = {"message": f"Web activation url: {url}", "url": url}
         else:
-            params["subscription_id"] = EXPLICIT_NULL
+            webbrowser.open(url, new=1)
+            res = {"message": "Browser opened to web activation page", "url": url}
+
+    # delegate proxy activation
+    elif delegate_proxy:
+        requirements_data = transfer_client.endpoint_get_activation_requirements(
+            endpoint_id
+        ).data
+        filled_requirements_data = fill_delegate_proxy_activation_requirements(
+            requirements_data, delegate_proxy, lifetime_hours=proxy_lifetime or 12
+        )
+        res = transfer_client.endpoint_activate(
+            endpoint_id, requirements_data=filled_requirements_data
+        )
 
-    # if --no-default-directory given, pass an EXPLICIT_NULL
-    if params.get("no_default_directory"):
-        params["default_directory"] = EXPLICIT_NULL
-        params.pop("no_default_directory")
+    # output
+    formatted_print(res, text_format=FORMAT_TEXT_RAW, response_key="message")
```

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/create.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/create.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 from typing import Any
 
 from globus_cli.login_manager import LoginManager
 from globus_cli.parsing import (
     ENDPOINT_PLUS_REQPATH,
     command,
+    endpointish_create_and_update_params,
     mutex_option_group,
     one_use_option,
 )
 from globus_cli.termio import FORMAT_TEXT_RECORD, formatted_print
 
-from ._common import (
-    endpoint_create_and_update_params,
-    validate_endpoint_create_and_update_params,
-)
+from ._common import endpoint_create_params, validate_endpoint_create_and_update_params
 
 COMMON_FIELDS = [("Message", "message"), ("Endpoint ID", "id")]
 
 GCP_FIELDS = [("Setup Key", "globus_connect_setup_key")]
 
 
 @command(
@@ -43,15 +41,16 @@
 [source,bash]
 ----
 $ host_ep=ddb59aef-6d04-11e5-ba46-22000b92c6ec
 $ globus endpoint create --shared host_ep:~/ my_shared_endpoint
 ----
 """,
 )
-@endpoint_create_and_update_params(create=True)
+@endpointish_create_and_update_params("create")
+@endpoint_create_params
 @one_use_option(
     "--personal",
     is_flag=True,
     help=(
         "Create a Globus Connect Personal endpoint. "
         "Mutually exclusive with --server and --shared."
     ),
@@ -80,15 +79,18 @@
     login_manager: LoginManager,
     personal: bool,
     server: bool,
     shared: tuple[str, str] | None,
     **kwargs: Any,
 ) -> None:
     """
-    Create a new endpoint.
+    Create a new endpoint. (deprecated)
+
+    This command is deprecated. Either `globus gcp create` or the Globus Connect Server
+    CLI should be used instead for most cases.
 
     Requires a display name and exactly one of --personal, --server, or --shared to make
     a Globus Connect Personal, Globus Connect Server, or Shared endpoint respectively.
 
     Note that `--personal` does not perform local setup steps. When this command is run
     with the `--personal` flag, it returns a setup key which can be passed to
     Globus Connect Personal during setup.
```

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/deactivate.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/deactivate.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/is_activated.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/is_activated.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/local_id.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/local_id.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/my_shared_endpoint_list.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/my_shared_endpoint_list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/create.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/create.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/permission/update.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/permission/update.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/create.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/create.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/role/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/role/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/search.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/search.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/__init__.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/_common.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/_common.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/add.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/add.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/server/update.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/server/update.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/set_subscription_id.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/set_subscription_id.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/endpoint/update.py` & `globus-cli-3.9.0/src/globus_cli/commands/endpoint/update.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from globus_cli.endpointish import Endpointish
 from globus_cli.login_manager import LoginManager
-from globus_cli.parsing import command, endpoint_id_arg
+from globus_cli.parsing import (
+    command,
+    endpoint_id_arg,
+    endpointish_create_and_update_params,
+)
 from globus_cli.termio import FORMAT_TEXT_RAW, formatted_print
 
-from ._common import (
-    endpoint_create_and_update_params,
-    validate_endpoint_create_and_update_params,
-)
+from ._common import endpoint_update_params, validate_endpoint_create_and_update_params
 
 
 @command("update")
 @endpoint_id_arg
-@endpoint_create_and_update_params(create=False)
+@endpoint_update_params
+@endpointish_create_and_update_params("update")
 @LoginManager.requires_login(LoginManager.TRANSFER_RS)
 def endpoint_update(*, login_manager: LoginManager, **kwargs):
     """Update attributes of an endpoint"""
     from globus_cli.services.transfer import assemble_generic_doc
 
     transfer_client = login_manager.get_transfer_client()
     endpoint_id = kwargs.pop("endpoint_id")
```

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/get_identities.py` & `globus-cli-3.9.0/src/globus_cli/commands/get_identities.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/__init__.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/_common.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/_common.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/create.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/create.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/invite/_common.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/invite/_common.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/invite/accept.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/invite/accept.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/invite/decline.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/invite/decline.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/join.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/join.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/leave.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/leave.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/member/add.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/member/add.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/member/approve.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/member/approve.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/member/invite.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/member/invite.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/member/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/member/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/member/reject.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/member/reject.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/member/remove.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/member/remove.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/set_policies.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/set_policies.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/group/update.py` & `globus-cli-3.9.0/src/globus_cli/commands/group/update.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/list_commands.py` & `globus-cli-3.9.0/src/globus_cli/commands/list_commands.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/login.py` & `globus-cli-3.9.0/src/globus_cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/logout.py` & `globus-cli-3.9.0/src/globus_cli/commands/logout.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/ls.py` & `globus-cli-3.9.0/src/globus_cli/commands/ls.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/mkdir.py` & `globus-cli-3.9.0/src/globus_cli/commands/mkdir.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/rename.py` & `globus-cli-3.9.0/src/globus_cli/commands/rename.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/rm.py` & `globus-cli-3.9.0/src/globus_cli/commands/rm.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/_common.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/_common.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/delete_by_query.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/delete_by_query.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/index/create.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/index/create.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/index/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/index/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/index/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/index/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/index/role/create.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/index/role/create.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/index/role/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/index/role/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/index/role/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/index/role/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/index/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/index/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/ingest.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/ingest.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/query.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/query.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/subject/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/subject/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/subject/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/subject/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/task/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/task/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/search/task/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/search/task/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/session/consent.py` & `globus-cli-3.9.0/src/globus_cli/commands/session/consent.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/session/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/session/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/session/update.py` & `globus-cli-3.9.0/src/globus_cli/commands/session/update.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/task/__init__.py` & `globus-cli-3.9.0/src/globus_cli/commands/task/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/task/cancel.py` & `globus-cli-3.9.0/src/globus_cli/commands/task/cancel.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/task/event_list.py` & `globus-cli-3.9.0/src/globus_cli/commands/task/event_list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/task/generate_submission_id.py` & `globus-cli-3.9.0/src/globus_cli/commands/task/generate_submission_id.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/task/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/task/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/task/pause_info.py` & `globus-cli-3.9.0/src/globus_cli/commands/task/pause_info.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/task/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/task/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/task/update.py` & `globus-cli-3.9.0/src/globus_cli/commands/task/update.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/task/wait.py` & `globus-cli-3.9.0/src/globus_cli/commands/task/wait.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/timer/_common.py` & `globus-cli-3.9.0/src/globus_cli/commands/timer/_common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import datetime
 from typing import Any
 from urllib.parse import urlparse
 
+from globus_cli.commands._common import isoformat_to_local
+
 # List of datetime formats accepted as input. (`%z` means timezone.)
 DATETIME_FORMATS = [
     "%Y-%m-%d",
     "%Y-%m-%d %H:%M:%S",
     "%Y-%m-%d %H:%M:%S%z",
     "%Y-%m-%dT%H:%M:%S",
     "%Y-%m-%dT%H:%M:%S%z",
@@ -42,26 +44,14 @@
 
 def _get_interval(data: dict[str, Any]) -> str | None:
     if not data["interval"]:
         return None
     return str(datetime.timedelta(seconds=data["interval"]))
 
 
-def isoformat_to_local(
-    utc_str: str | None, localtz: datetime.tzinfo | None = None
-) -> str | None:
-    if not utc_str:
-        return None
-    # let this raise ValueError
-    date = datetime.datetime.fromisoformat(utc_str)
-    if date.tzinfo is None:
-        return date.strftime("%Y-%m-%d %H:%M:%S")
-    return date.astimezone(tz=localtz).strftime("%Y-%m-%d %H:%M:%S")
-
-
 JOB_FORMAT_FIELDS = [
     ("Job ID", "job_id"),
     ("Name", "name"),
     ("Type", _get_action_type),
     ("Submitted At", lambda data: isoformat_to_local(data["submitted_at"])),
     ("Start", lambda data: isoformat_to_local(data["start"])),
     ("Interval", _get_interval),
```

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/timer/create/transfer.py` & `globus-cli-3.9.0/src/globus_cli/commands/timer/create/transfer.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/timer/delete.py` & `globus-cli-3.9.0/src/globus_cli/commands/timer/delete.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/timer/list.py` & `globus-cli-3.9.0/src/globus_cli/commands/timer/list.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/timer/show.py` & `globus-cli-3.9.0/src/globus_cli/commands/timer/show.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/transfer.py` & `globus-cli-3.9.0/src/globus_cli/commands/transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,15 @@
         formatted_print(
             transfer_data.data,
             response_key="DATA",
             fields=(
                 ("Source Path", "source_path"),
                 ("Dest Path", "destination_path"),
                 ("Recursive", "recursive"),
-                ("External Checksum", "external_checksum"),
+                ("External Checksum", lambda x: x.get("external_checksum")),
             ),
         )
         # exit safely
         return
 
     # autoactivate after parsing all args and putting things together
     # skip this if skip-activation-check is given
```

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/update.py` & `globus-cli-3.9.0/src/globus_cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/version.py` & `globus-cli-3.9.0/src/globus_cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/commands/whoami.py` & `globus-cli-3.9.0/src/globus_cli/commands/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/constants.py` & `globus-cli-3.9.0/src/globus_cli/constants.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/endpointish/__init__.py` & `globus-cli-3.9.0/src/globus_cli/endpointish/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/endpointish/endpoint_type.py` & `globus-cli-3.9.0/src/globus_cli/endpointish/endpoint_type.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/endpointish/endpointish.py` & `globus-cli-3.9.0/src/globus_cli/endpointish/endpointish.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/endpointish/errors.py` & `globus-cli-3.9.0/src/globus_cli/endpointish/errors.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/exception_handling/__init__.py` & `globus-cli-3.9.0/src/globus_cli/exception_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/exception_handling/hooks.py` & `globus-cli-3.9.0/src/globus_cli/exception_handling/hooks.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/exception_handling/registry.py` & `globus-cli-3.9.0/src/globus_cli/exception_handling/registry.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/globus_cli_flake8.py` & `globus-cli-3.9.0/src/globus_cli/globus_cli_flake8.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/login_manager/__init__.py` & `globus-cli-3.9.0/src/globus_cli/login_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/login_manager/_old_config.py` & `globus-cli-3.9.0/src/globus_cli/login_manager/_old_config.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/login_manager/auth_flows.py` & `globus-cli-3.9.0/src/globus_cli/login_manager/auth_flows.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/login_manager/client_login.py` & `globus-cli-3.9.0/src/globus_cli/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/login_manager/errors.py` & `globus-cli-3.9.0/src/globus_cli/login_manager/errors.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/login_manager/local_server.py` & `globus-cli-3.9.0/src/globus_cli/login_manager/local_server.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/login_manager/manager.py` & `globus-cli-3.9.0/src/globus_cli/login_manager/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import uuid
 from typing import TYPE_CHECKING, Iterator
 
 import click
 import globus_sdk
 from globus_sdk.scopes import (
     AuthScopes,
+    FlowsScopes,
     GCSEndpointScopeBuilder,
     GroupsScopes,
     SearchScopes,
     TimerScopes,
     TransferScopes,
 )
 
@@ -31,18 +32,19 @@
 
 
 class LoginManager:
     # TEST_MODE skips token validation
     _TEST_MODE: bool = False
 
     AUTH_RS = AuthScopes.resource_server
-    TRANSFER_RS = TransferScopes.resource_server
+    FLOWS_RS = FlowsScopes.resource_server
     GROUPS_RS = GroupsScopes.resource_server
     SEARCH_RS = SearchScopes.resource_server
     TIMER_RS = TimerScopes.resource_server
+    TRANSFER_RS = TransferScopes.resource_server
 
     STATIC_SCOPES: dict[str, list[str]] = {
         AUTH_RS: [
             AuthScopes.openid,
             AuthScopes.profile,
             AuthScopes.email,
             AuthScopes.view_identity_set,
@@ -55,14 +57,21 @@
         ],
         SEARCH_RS: [
             SearchScopes.all,
         ],
         TIMER_RS: [
             TimerScopes.timer,
         ],
+        FLOWS_RS: [
+            FlowsScopes.manage_flows,
+            FlowsScopes.view_flows,
+            FlowsScopes.run,
+            FlowsScopes.run_status,
+            FlowsScopes.run_manage,
+        ],
     }
 
     def __init__(self) -> None:
         self._token_storage = token_storage_adapter()
         self._nonstatic_requirements: dict[str, list[str]] = {}
 
     def add_requirement(self, rs_name: str, scopes: list[str]) -> None:
@@ -171,26 +180,26 @@
         """
         Command decorator for specifying a resource server that the user must have
         tokens for in order to run the command.
 
         Simple usage for commands that have static resource needs: simply list all
         needed resource servers as args:
 
-        @LoginManager.requries_login("auth.globus.org")
+        @LoginManager.requires_login("auth.globus.org")
 
-        @LoginManager.requries_login(LoginManager.AUTH_RS)
+        @LoginManager.requires_login(LoginManager.AUTH_RS)
 
         @LoginManager.requires_login("auth.globus.org", "transfer.api.globus.org")
 
-        @LoginManager.requries_login(LoginManager.AUTH_RS, LoginManager.TRANSFER_RS)
+        @LoginManager.requires_login(LoginManager.AUTH_RS, LoginManager.TRANSFER_RS)
 
         Usage for commands which have dynamic resource servers depending
         on the arguments passed to the command (e.g. commands for the GCS API)
 
-        @LoginManager.requies_login()
+        @LoginManager.requires_login()
         def command(login_manager, endpoint_id)
 
             login_manager.<do the thing>(endpoint_id)
 
         """
 
         def inner(func):
@@ -266,14 +275,18 @@
         authorizer = self._get_client_authorizer(AuthScopes.resource_server)
         return CustomAuthClient(authorizer=authorizer, app_name=version.app_name)
 
     def get_groups_client(self) -> globus_sdk.GroupsClient:
         authorizer = self._get_client_authorizer(GroupsScopes.resource_server)
         return globus_sdk.GroupsClient(authorizer=authorizer, app_name=version.app_name)
 
+    def get_flows_client(self) -> globus_sdk.FlowsClient:
+        authorizer = self._get_client_authorizer(FlowsScopes.resource_server)
+        return globus_sdk.FlowsClient(authorizer=authorizer, app_name=version.app_name)
+
     def get_search_client(self) -> globus_sdk.SearchClient:
         authorizer = self._get_client_authorizer(SearchScopes.resource_server)
         return globus_sdk.SearchClient(authorizer=authorizer, app_name=version.app_name)
 
     def get_timer_client(self) -> globus_sdk.TimerClient:
         authorizer = self._get_client_authorizer(TimerScopes.resource_server)
         return globus_sdk.TimerClient(authorizer=authorizer, app_name=version.app_name)
```

### Comparing `globus-cli-3.8.0/src/globus_cli/login_manager/tokenstore.py` & `globus-cli-3.9.0/src/globus_cli/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/__init__.py` & `globus-cli-3.9.0/src/globus_cli/parsing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     endpoint_id_arg,
     no_local_server_option,
     security_principal_opts,
     synchronous_task_wait_options,
     task_notify_option,
     task_submission_options,
 )
+from .shared_options.endpoint_create_and_update import (
+    endpointish_create_and_update_params,
+)
 from .shared_options.transfer_task_options import (
     encrypt_data_option,
     fail_on_quota_errors_option,
     preserve_timestamp_option,
     skip_source_errors_option,
     sync_level_option,
     transfer_batch_option,
@@ -71,8 +74,9 @@
     "sync_level_option",
     "task_notify_option",
     "fail_on_quota_errors_option",
     "encrypt_data_option",
     "preserve_timestamp_option",
     "skip_source_errors_option",
     "verify_checksum_option",
+    "endpointish_create_and_update_params",
 ]
```

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/command_state.py` & `globus-cli-3.9.0/src/globus_cli/parsing/command_state.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/commands.py` & `globus-cli-3.9.0/src/globus_cli/parsing/commands.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/mutex_group.py` & `globus-cli-3.9.0/src/globus_cli/parsing/mutex_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import functools
 from typing import Any, Callable, TypeVar, cast
 
 import click
 
 from ..utils import format_list_of_words
 
-RT = TypeVar("RT")
-C = TypeVar("C", bound=Callable[..., RT])
+C = TypeVar("C", bound=Callable)
 
 
 class MutexInfo:
     def __init__(self, opt, param=None, present=None):
         self.option_name = opt
         if param:
             self.param_name = param
@@ -58,15 +57,15 @@
         if isinstance(opt, str):
             opt_infos.append(MutexInfo(opt))
         else:
             opt_infos.append(opt)
 
     def decorator(func: C) -> C:
         @functools.wraps(func)
-        def wrapped(*args: Any, **kwargs: Any) -> RT:
+        def wrapped(*args: Any, **kwargs: Any) -> Any:
             found_opts = []
             for opt in opt_infos:
                 if opt.is_present(kwargs):
                     found_opts.append(opt)
             if len(found_opts) > 1:
                 option_str = format_list_of_words(*(str(o) for o in opt_infos))
                 raise click.UsageError(f"{option_str} are mutually exclusive")
```

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/one_use_option.py` & `globus-cli-3.9.0/src/globus_cli/parsing/one_use_option.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/param_types/__init__.py` & `globus-cli-3.9.0/src/globus_cli/parsing/param_types/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/param_types/comma_delimited.py` & `globus-cli-3.9.0/src/globus_cli/parsing/param_types/comma_delimited.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/param_types/endpoint_plus_path.py` & `globus-cli-3.9.0/src/globus_cli/parsing/param_types/endpoint_plus_path.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/param_types/identity_type.py` & `globus-cli-3.9.0/src/globus_cli/parsing/param_types/identity_type.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/param_types/location.py` & `globus-cli-3.9.0/src/globus_cli/parsing/param_types/location.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/param_types/nullable.py` & `globus-cli-3.9.0/src/globus_cli/parsing/param_types/nullable.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/param_types/prefix_mapper.py` & `globus-cli-3.9.0/src/globus_cli/parsing/param_types/prefix_mapper.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/param_types/task_path.py` & `globus-cli-3.9.0/src/globus_cli/parsing/param_types/task_path.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/param_types/timedelta.py` & `globus-cli-3.9.0/src/globus_cli/parsing/param_types/timedelta.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/shared_options/__init__.py` & `globus-cli-3.9.0/src/globus_cli/parsing/shared_options/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/shared_options/transfer_task_options.py` & `globus-cli-3.9.0/src/globus_cli/parsing/shared_options/transfer_task_options.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/parsing/shell_completion.py` & `globus-cli-3.9.0/src/globus_cli/parsing/shell_completion.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/principal_resolver.py` & `globus-cli-3.9.0/src/globus_cli/principal_resolver.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/services/auth.py` & `globus-cli-3.9.0/src/globus_cli/services/auth.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/services/gcs.py` & `globus-cli-3.9.0/src/globus_cli/services/gcs.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/services/transfer/__init__.py` & `globus-cli-3.9.0/src/globus_cli/services/transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/services/transfer/activation.py` & `globus-cli-3.9.0/src/globus_cli/services/transfer/activation.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/services/transfer/client.py` & `globus-cli-3.9.0/src/globus_cli/services/transfer/client.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/services/transfer/data.py` & `globus-cli-3.9.0/src/globus_cli/services/transfer/data.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/services/transfer/delegate_proxy.py` & `globus-cli-3.9.0/src/globus_cli/services/transfer/delegate_proxy.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/services/transfer/recursive_ls.py` & `globus-cli-3.9.0/src/globus_cli/services/transfer/recursive_ls.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/termio/__init__.py` & `globus-cli-3.9.0/src/globus_cli/termio/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/termio/awscli_text.py` & `globus-cli-3.9.0/src/globus_cli/termio/awscli_text.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/termio/context.py` & `globus-cli-3.9.0/src/globus_cli/termio/context.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/termio/errors.py` & `globus-cli-3.9.0/src/globus_cli/termio/errors.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/termio/output_formatter.py` & `globus-cli-3.9.0/src/globus_cli/termio/output_formatter.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/types.py` & `globus-cli-3.9.0/src/globus_cli/types.py`

 * *Files identical despite different names*

### Comparing `globus-cli-3.8.0/src/globus_cli/utils.py` & `globus-cli-3.9.0/src/globus_cli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -133,18 +133,24 @@
 
     def __getitem__(self, key: str) -> Any:
         return self.data[key]
 
 
 # wrap to add a `has_next()` method and `limit` param to a naive iterator
 class PagingWrapper:
-    def __init__(self, iterator: Iterator[Any], limit: int | None = None) -> None:
+    def __init__(
+        self,
+        iterator: Iterator[Any],
+        limit: int | None = None,
+        json_conversion_key: str | None = None,
+    ) -> None:
         self.iterator = iterator
         self.next = None
         self.limit = limit
+        self.json_conversion_key = json_conversion_key
         self._step()
 
     def _step(self) -> None:
         try:
             self.next = next(self.iterator)
         except StopIteration:
             self.next = None
@@ -156,14 +162,25 @@
         yielded = 0
         while self.has_next() and (self.limit is None or yielded < self.limit):
             cur = self.next
             self._step()
             yield cur
             yielded += 1
 
+    @property
+    def json_converter(self) -> Callable[[Iterator[Any]], dict[str, list[Any]]]:
+        if self.json_conversion_key is None:
+            raise NotImplementedError("does not support json_converter")
+        key: str = self.json_conversion_key
+
+        def converter(it: Iterator[Any]) -> dict[str, list[Any]]:
+            return {key: list(it)}
+
+        return converter
+
 
 def shlex_process_stream(process_command: click.Command, stream: TextIO) -> None:
     """
     Use shlex to process stdin line-by-line.
     Also prints help text.
 
     Requires that @process_command be a Click command object, used for
```

### Comparing `globus-cli-3.8.0/src/globus_cli/version.py` & `globus-cli-3.9.0/src/globus_cli/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from distutils.version import LooseVersion
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "3.8.0"
+__version__ = "3.9.0"
 
 # app name to send as part of SDK requests
 app_name = f"Globus CLI v{__version__}"
 
 
 # pull down version data from PyPi
 def get_versions() -> tuple[LooseVersion | None, LooseVersion]:
```

### Comparing `globus-cli-3.8.0/src/globus_cli.egg-info/PKG-INFO` & `globus-cli-3.9.0/src/globus_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-cli
-Version: 3.8.0
+Version: 3.9.0
 Summary: Globus CLI
 Home-page: https://github.com/globus/globus-cli
 Author: Stephen Rosen
 Author-email: sirosen@globus.org
 Keywords: globus,cli,command line
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `globus-cli-3.8.0/src/globus_cli.egg-info/SOURCES.txt` & `globus-cli-3.9.0/src/globus_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,21 @@
 src/globus_cli/commands/endpoint/server/__init__.py
 src/globus_cli/commands/endpoint/server/_common.py
 src/globus_cli/commands/endpoint/server/add.py
 src/globus_cli/commands/endpoint/server/delete.py
 src/globus_cli/commands/endpoint/server/list.py
 src/globus_cli/commands/endpoint/server/show.py
 src/globus_cli/commands/endpoint/server/update.py
+src/globus_cli/commands/flows/__init__.py
+src/globus_cli/commands/flows/_common.py
+src/globus_cli/commands/flows/list.py
+src/globus_cli/commands/gcp/__init__.py
+src/globus_cli/commands/gcp/create/__init__.py
+src/globus_cli/commands/gcp/create/guest.py
+src/globus_cli/commands/gcp/create/mapped.py
 src/globus_cli/commands/group/__init__.py
 src/globus_cli/commands/group/_common.py
 src/globus_cli/commands/group/create.py
 src/globus_cli/commands/group/delete.py
 src/globus_cli/commands/group/join.py
 src/globus_cli/commands/group/leave.py
 src/globus_cli/commands/group/list.py
@@ -166,14 +173,15 @@
 src/globus_cli/parsing/param_types/identity_type.py
 src/globus_cli/parsing/param_types/location.py
 src/globus_cli/parsing/param_types/nullable.py
 src/globus_cli/parsing/param_types/prefix_mapper.py
 src/globus_cli/parsing/param_types/task_path.py
 src/globus_cli/parsing/param_types/timedelta.py
 src/globus_cli/parsing/shared_options/__init__.py
+src/globus_cli/parsing/shared_options/endpoint_create_and_update.py
 src/globus_cli/parsing/shared_options/transfer_task_options.py
 src/globus_cli/services/__init__.py
 src/globus_cli/services/auth.py
 src/globus_cli/services/gcs.py
 src/globus_cli/services/transfer/__init__.py
 src/globus_cli/services/transfer/activation.py
 src/globus_cli/services/transfer/client.py
```

