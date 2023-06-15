# Comparing `tmp/vantage6-server-3.9.0rc2.tar.gz` & `tmp/vantage6-server-3.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-3.9.0rc2.tar", last modified: Tue May  9 13:37:06 2023, max compression
+gzip compressed data, was "vantage6-server-3.9.0rc4.tar", last modified: Wed May 24 09:34:10 2023, max compression
```

## Comparing `vantage6-server-3.9.0rc2.tar` & `vantage6-server-3.9.0rc4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 13:37:06.438941 vantage6-server-3.9.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.426940 vantage6-server-3.9.0rc2/tests_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)   100933 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.426940 vantage6-server-3.9.0rc2/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/node_config_skeleton.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/server_config_skeleton.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/testnodeconfiguration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.430940 vantage6-server-3.9.0rc2/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/collaboration.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/common/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    26260 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    27653 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    26410 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-09 13:36:37.000000 vantage6-server-3.9.0rc2/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:37:06.434940 vantage6-server-3.9.0rc2/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 13:37:06.000000 vantage6-server-3.9.0rc2/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.437729 vantage6-server-3.9.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-24 09:34:10.437729 vantage6-server-3.9.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:10.437729 vantage6-server-3.9.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11685 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100933 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)    25405 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/node_config_skeleton.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/server_config_skeleton.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/testnodeconfiguration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.429729 vantage6-server-3.9.0rc4/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.433729 vantage6-server-3.9.0rc4/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.433729 vantage6-server-3.9.0rc4/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.433729 vantage6-server-3.9.0rc4/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/common/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19180 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17265 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26260 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27653 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26410 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-24 09:33:56.000000 vantage6-server-3.9.0rc4/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:10.437729 vantage6-server-3.9.0rc4/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-24 09:34:10.000000 vantage6-server-3.9.0rc4/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-3.9.0rc2/PKG-INFO` & `vantage6-server-3.9.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 3.9.0rc2 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 3.9.0rc4 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-3.9.0rc2/setup.py` & `vantage6-server-3.9.0rc4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     long_description_content_type='text/markdown',
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'bcrypt==4.0.1',
         'flasgger==0.9.5',
-        'Flask==2.1.1',
+        'flask==2.2.5',
         'Flask-Cors==3.0.10',
         'Flask-JWT-Extended==4.4.4',
         'Flask-Mail==0.9.1',
         'Flask-Principal==0.4.0',
         'Flask-RESTful==0.3.9',
         'flask-marshmallow==0.14.0',
         'Flask-SocketIO==5.3.2',
@@ -47,19 +47,19 @@
         'ipython==8.10.0',
         'jinja2==3.1.2',
         'kombu==5.2.4',
         'marshmallow==2.16.3',
         'marshmallow-sqlalchemy==0.15.0',
         'pyotp==2.8.0',
         'questionary==1.10.0',
-        'requests==2.28.2',
+        'requests==2.31.0',
         'requests-oauthlib==1.3.1',
         'schema==0.7.5',
         'SQLAlchemy==1.4.46',
-        'Werkzeug==2.2.3',
+        'werkzeug==2.3.4',
         f'vantage6 == {version_ns["__version__"]}',
         f'vantage6-common == {version_ns["__version__"]}'
     ],
     extras_require={
         'dev': [
             'coverage==6.4.4'
         ]
```

### Comparing `vantage6-server-3.9.0rc2/tests_server/test_models.py` & `vantage6-server-3.9.0rc4/tests_server/test_models.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/tests_server/test_resources.py` & `vantage6-server-3.9.0rc4/tests_server/test_resources.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/__init__.py` & `vantage6-server-3.9.0rc4/vantage6/server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from flask_jwt_extended import JWTManager
 from flask_marshmallow import Marshmallow
 from flask_restful import Api
 from flask_mail import Mail
 from flask_principal import Principal, Identity, identity_changed
 from flask_socketio import SocketIO
 from threading import Thread
+from pathlib import Path
 
 from vantage6.common import logger_name
 from vantage6.common.globals import PING_INTERVAL_SECONDS
 from vantage6.server import db
 from vantage6.cli.context import ServerContext
 from vantage6.cli.globals import DEFAULT_SERVER_ENVIRONMENT
 from vantage6.server.model.base import DatabaseSessionManager, Database
@@ -51,14 +52,15 @@
     JWT_TEST_ACCESS_TOKEN_EXPIRES,
     RESOURCES,
     SUPER_USER_INFO,
     REFRESH_TOKENS_EXPIRE_HOURS,
     DEFAULT_SUPPORT_EMAIL_ADDRESS,
     MIN_TOKEN_VALIDITY_SECONDS,
     MIN_REFRESH_TOKEN_EXPIRY_DELTA,
+    SERVER_MODULE_NAME
 )
 from vantage6.server.resource.common.swagger_templates import swagger_template
 from vantage6.server._version import __version__
 from vantage6.server.mail_service import MailService
 from vantage6.server.websockets import DefaultSocketNamespace
 from vantage6.server.default_roles import get_default_roles, DefaultRole
 
@@ -79,15 +81,20 @@
 
     def __init__(self, ctx: ServerContext) -> None:
         """Create a vantage6-server application."""
 
         self.ctx = ctx
 
         # initialize, configure Flask
-        self.app = Flask(APPNAME, root_path=os.path.dirname(__file__))
+        self.app = Flask(
+            SERVER_MODULE_NAME, root_path=Path(__file__),
+            template_folder=Path(__file__).parent / 'templates',
+            static_folder=Path(__file__).parent / 'static'
+        )
+        self.debug: dict = self.ctx.config.get('debug', {})
         self.configure_flask()
 
         # Setup SQLAlchemy and Marshmallow for marshalling/serializing
         self.ma = Marshmallow(self.app)
 
         # Setup the Flask-JWT-Extended extension (JWT: JSON Web Token)
         self.jwt = JWTManager(self.app)
@@ -112,17 +119,14 @@
         self.permissions = PermissionManager()
 
         # Api - REST JSON-rpc
         self.api = Api(self.app)
         self.configure_api()
         self.load_resources()
 
-        # make specific log settings (muting etc)
-        self.configure_logging()
-
         # set the server version
         self.__version__ = __version__
 
         # set up socket ping/pong
         log.debug("Starting thread to set node status")
         t = Thread(target=self.__node_status_worker, daemon=True)
         t.start()
@@ -141,54 +145,48 @@
             SocketIO object
         """
 
         msg_queue = self.ctx.config.get('rabbitmq_uri')
         if msg_queue:
             log.debug(f'Connecting to msg queue: {msg_queue}')
 
+        debug_mode = self.debug.get('socketio', False)
+        if debug_mode:
+            log.debug("SocketIO debug mode enabled")
         try:
             socketio = SocketIO(
                 self.app,
                 async_mode='gevent_uwsgi',
                 message_queue=msg_queue,
                 ping_timeout=60,
-                cors_allowed_origins='*'
+                cors_allowed_origins='*',
+                logger=debug_mode,
+                engineio_logger=debug_mode
             )
         except Exception as e:
             log.warning('Default socketio settings failed, attempt to run '
                         'without gevent_uwsgi packages! This leads to '
                         'performance issues and possible issues concerning '
                         'the websocket channels!')
             log.debug(e)
             socketio = SocketIO(
                 self.app,
                 message_queue=msg_queue,
                 ping_timeout=60,
-                cors_allowed_origins='*'
+                cors_allowed_origins='*',
+                logger=debug_mode,
+                engineio_logger=debug_mode
             )
 
         # FIXME: temporary fix to get socket object into the namespace class
         DefaultSocketNamespace.socketio = socketio
         socketio.on_namespace(DefaultSocketNamespace("/tasks"))
 
         return socketio
 
-    @staticmethod
-    def configure_logging() -> None:
-        """Set third party loggers to a warning level"""
-
-        # Prevent logging from urllib3
-        logging.getLogger("urllib3").setLevel(logging.WARNING)
-        logging.getLogger("socketIO-client").setLevel(logging.WARNING)
-        logging.getLogger("engineio.server").setLevel(logging.WARNING)
-        logging.getLogger("socketio.server").setLevel(logging.WARNING)
-        logging.getLogger('sqlalchemy.engine').setLevel(logging.WARNING)
-        logging.getLogger('requests_oauthlib.oauth2_session')\
-            .setLevel(logging.WARNING)
-
     def configure_flask(self) -> None:
         """Configure the Flask settings of the vantage6 server."""
 
         # let us handle exceptions
         self.app.config['PROPAGATE_EXCEPTIONS'] = True
 
         # patch where to obtain token
@@ -243,14 +241,18 @@
             DEFAULT_SUPPORT_EMAIL_ADDRESS
         )
         self.app.config["MAIL_PASSWORD"] = mail_config.get("password", "")
         self.app.config["MAIL_USE_TLS"] = mail_config.get("MAIL_USE_TLS",
                                                           True)
         self.app.config["MAIL_USE_SSL"] = mail_config.get("MAIL_USE_SSL",
                                                           False)
+        debug_mode = self.debug.get('flask', False)
+        if debug_mode:
+            log.debug("Flask debug mode enabled")
+        self.app.debug = debug_mode
 
         def _get_request_path(request: Request) -> str:
             """
             Return request extension of request URL, e.g.
             http://localhost:5000/api/task/1 -> api/task/1
 
             Parameters
@@ -384,22 +386,23 @@
         # helper to create HATEOAS schemas
         HATEOASModelSchema.api = self.api
 
         # whatever you get try to json it
         @self.api.representation('application/json')
         # pylint: disable=unused-argument
         def output_json(
-            data: Any, code: HTTPStatus, headers: dict = None
+            data: db.Base | list[db.Base], code: HTTPStatus,
+            headers: dict = None
         ) -> Response:
             """
             Return jsonified data for request responses.
 
             Parameters
             ----------
-            data: Any
+            data: db.Base | list[db.Base]
                 The data to be jsonified
             code: HTTPStatus
                 The HTTP status code of the response
             headers: dict
                 Additional headers to be added to the response
             """
 
@@ -455,15 +458,15 @@
             return claims
 
         @self.jwt.user_identity_loader
         # pylint: disable=unused-argument
         def user_identity_loader(
                 identity: db.Authenticatable | dict) -> str | dict:
             """"
-            JSON serializing identity to be used by create_access_token.
+            JSON serializing identity to be used by ``create_access_token``.
 
             Parameters
             ----------
             identity: db.Authenticatable | dict
                 The identity to be serialized
 
             Returns
```

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-3.9.0rc4/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-3.9.0rc4/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-3.9.0rc4/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_data/dev/server.yaml` & `vantage6-server-3.9.0rc4/vantage6/server/_data/dev/server.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-3.9.0rc4/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_data/node_config_skeleton.yaml` & `vantage6-server-3.9.0rc4/vantage6/server/_data/node_config_skeleton.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_data/server_config_skeleton.yaml` & `vantage6-server-3.9.0rc4/vantage6/server/_data/server_config_skeleton.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-3.9.0rc4/vantage6/server/_data/unittest_config.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-3.9.0rc4/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/_version.py` & `vantage6-server-3.9.0rc4/vantage6/server/_version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/cli/server.py` & `vantage6-server-3.9.0rc4/vantage6/server/cli/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,18 +327,24 @@
 
     # Suppress logging (e.g. on tab-completion)
     import logging
     logging.getLogger('parso.cache').setLevel(logging.WARNING)
     logging.getLogger('parso.python.diff').setLevel(logging.WARNING)
     logging.getLogger('urllib3.connectionpool').setLevel(logging.WARNING)
     logging.getLogger('asyncio').setLevel(logging.WARNING)
+
+    logging.warning(
+        "Using the shell is not recommended! There are no checks on "
+        "the validity of the data you are entering.")
+    logging.warning("Please use the User interface, Python client, or API.")
     del logging
 
     import vantage6.server.db as db
 
+
     IPython.embed(config=c)
 
 
 #
 #   version
 #
 @cli_server.command(name='version')
```

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/context.py` & `vantage6-server-3.9.0rc4/vantage6/server/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import vantage6.server.globals as constants
 
 from vantage6.common.context import AppContext
 from vantage6.cli.configuration_manager import (
     TestingConfigurationManager
 )
 
@@ -14,15 +15,15 @@
     separate test context.
     """
 
     INST_CONFIG_MANAGER = TestingConfigurationManager
     LOGGING_ENABLED = False
 
     @classmethod
-    def from_external_config_file(cls) -> 'TestContext':
+    def from_external_config_file(cls) -> TestContext:
         """
         Create a context the unittest configuration file.
 
         Returns
         -------
         TestContext
             Context object
```

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/controller/fixture.py` & `vantage6-server-3.9.0rc4/vantage6/server/controller/fixture.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/db.py` & `vantage6-server-3.9.0rc4/vantage6/server/db.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/default_roles.py` & `vantage6-server-3.9.0rc4/vantage6/server/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/globals.py` & `vantage6-server-3.9.0rc4/vantage6/server/globals.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #
 #   INSTALLATION SETTINGS
 #
 PACKAGE_FOLDER = Path(__file__).parent.parent.parent
 
 DATA_FOLDER = PACKAGE_FOLDER / APPNAME / "server" / "_data"
 
+SERVER_MODULE_NAME = APPNAME + "-server"
+
 #
 #   RUNTIME SETTINGS
 #
 
 # Expiretime of JWT tokens
 ACCESS_TOKEN_EXPIRES_HOURS = 6
```

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/mail_service.py` & `vantage6-server-3.9.0rc4/vantage6/server/mail_service.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/__init__.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/algorithm_port.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/algorithm_port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/authenticatable.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/base.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/collaboration.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/member.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/node.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/node_config.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/organization.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/permission.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/result.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/result.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/role.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/rule.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/task.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/model/user.py` & `vantage6-server-3.9.0rc4/vantage6/server/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/permission.py` & `vantage6-server-3.9.0rc4/vantage6/server/permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
         Parameters
         ----------
         rules: List[Rule]
             List of rules that user is checked to have
 
         Returns
         -------
-        Union[dict, bool]
+        dict | bool
             Dict with a message which rule is missing, else None
         """
         for rule in rules:
             requires = RuleNeed(rule.name, rule.scope, rule.operation)
             try:
                 Permission(requires).test()
             except PermissionDenied:
```

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/__init__.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/collaboration.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/common/_schema.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/common/_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/common/auth_helper.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/common/swagger_templates.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/event.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/event.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/health.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/health.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/node.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/organization.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/pagination.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import math
 import logging
 import flask
 import sqlalchemy
 
 from urllib.parse import urlencode
 
@@ -148,15 +150,15 @@
                 args['page'] = nav['page']
                 links[nav['rel']] = f'{url}?{urlencode(args)}'
 
         return links
 
     @classmethod
     def from_query(cls, query: sqlalchemy.orm.query,
-                   request: flask.Request) -> 'Pagination':
+                   request: flask.Request) -> Pagination:
         """
         Create a Pagination object from a query.
 
         Parameters
         ----------
         query : sqlalchemy.orm.query
             Query to paginate
@@ -191,15 +193,15 @@
         items = query.distinct().limit(per_page).offset((page_id-1)*per_page)\
             .all()
 
         return cls(items, page_id, per_page, total, request)
 
     @classmethod
     def from_list(cls, items: list[db.Base],
-                  request: flask.Request) -> 'Pagination':
+                  request: flask.Request) -> Pagination:
         """
         Create a Pagination object from a list of database objects.
 
         Parameters
         ----------
         items : list[db.Base]
             List of database objects to paginate
```

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/port.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/recover.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/recover.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/result.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/result.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/role.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/rule.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/stats.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/stats.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/task.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/token.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/token.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/user.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/version.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/vpn.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/vpn.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/resource/websocket_test.py` & `vantage6-server-3.9.0rc4/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6/server/websockets.py` & `vantage6-server-3.9.0rc4/vantage6/server/websockets.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-3.9.0rc2/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-3.9.0rc4/vantage6_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 3.9.0rc2
+Version: 3.9.0rc4
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 3.9.0rc2 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 3.9.0rc4 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-server-3.9.0rc2/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-3.9.0rc4/vantage6_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

