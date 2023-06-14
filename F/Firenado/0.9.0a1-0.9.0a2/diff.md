# Comparing `tmp/Firenado-0.9.0a1.tar.gz` & `tmp/Firenado-0.9.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Firenado-0.9.0a1.tar", last modified: Tue Jun  6 15:02:38 2023, max compression
+gzip compressed data, was "Firenado-0.9.0a2.tar", last modified: Wed Jun 14 15:03:16 2023, max compression
```

## Comparing `Firenado-0.9.0a1.tar` & `Firenado-0.9.0a2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.290004 Firenado-0.9.0a1/
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.280004 Firenado-0.9.0a1/Firenado.egg-info/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5202 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/PKG-INFO
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2539 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/SOURCES.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/dependency_links.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       71 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/entry_points.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      238 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/requires.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       15 2023-06-06 15:02:38.000000 Firenado-0.9.0a1/Firenado.egg-info/top_level.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    11361 2022-01-22 03:40:14.000000 Firenado-0.9.0a1/LICENSE
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      593 2021-03-14 16:46:20.000000 Firenado-0.9.0a1/MANIFEST.in
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5202 2023-06-06 15:02:38.290004 Firenado-0.9.0a1/PKG-INFO
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3789 2022-04-15 16:36:51.000000 Firenado-0.9.0a1/README.md
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3118 2019-01-26 05:48:04.000000 Firenado-0.9.0a1/README.rst
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.282004 Firenado-0.9.0a1/firenado/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1079 2023-06-06 14:40:55.000000 Firenado-0.9.0a1/firenado/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3895 2023-06-05 20:36:53.000000 Firenado-0.9.0a1/firenado/_pexpect_async_patch.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.283004 Firenado-0.9.0a1/firenado/bin/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2022-08-03 17:33:42.000000 Firenado-0.9.0a1/firenado/bin/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      752 2022-12-01 17:39:50.000000 Firenado-0.9.0a1/firenado/bin/firenado-cli.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      727 2022-08-30 19:14:45.000000 Firenado-0.9.0a1/firenado/bin/firenado-cli1.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.283004 Firenado-0.9.0a1/firenado/cli/
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       31 2022-08-30 19:14:45.000000 Firenado-0.9.0a1/firenado/cli/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      620 2022-03-19 18:33:11.000000 Firenado-0.9.0a1/firenado/cli/commands.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      194 2022-08-30 18:49:41.000000 Firenado-0.9.0a1/firenado/cli/root.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.283004 Firenado-0.9.0a1/firenado/components/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      759 2019-01-19 15:51:14.000000 Firenado-0.9.0a1/firenado/components/__init__.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.283004 Firenado-0.9.0a1/firenado/components/firenado/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/components/firenado/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      872 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/components/firenado/component.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1063 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/components/firenado/handlers.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.284004 Firenado-0.9.0a1/firenado/components/firenado/templates/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4008 2016-08-29 15:57:57.000000 Firenado-0.9.0a1/firenado/components/firenado/templates/info.html
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.284004 Firenado-0.9.0a1/firenado/components/static_maps/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/components/static_maps/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4137 2018-08-25 00:58:30.000000 Firenado-0.9.0a1/firenado/components/static_maps/component.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.284004 Firenado-0.9.0a1/firenado/components/toolbox/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-11-26 15:05:30.000000 Firenado-0.9.0a1/firenado/components/toolbox/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      831 2016-11-26 15:05:30.000000 Firenado-0.9.0a1/firenado/components/toolbox/component.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1961 2021-12-06 00:51:41.000000 Firenado-0.9.0a1/firenado/components/toolbox/uimodules.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.285004 Firenado-0.9.0a1/firenado/conf/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4774 2022-08-30 18:49:41.000000 Firenado-0.9.0a1/firenado/conf/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1092 2022-12-23 19:35:46.000000 Firenado-0.9.0a1/firenado/conf/firenado.yml
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    17831 2023-01-30 02:41:12.000000 Firenado-0.9.0a1/firenado/config.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    15458 2023-06-06 03:00:02.000000 Firenado-0.9.0a1/firenado/data.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    14990 2023-06-05 20:54:46.000000 Firenado-0.9.0a1/firenado/launcher.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.285004 Firenado-0.9.0a1/firenado/management/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      738 2019-05-18 04:12:04.000000 Firenado-0.9.0a1/firenado/management/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1993 2020-02-29 17:12:35.000000 Firenado-0.9.0a1/firenado/management/commands.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8627 2022-04-16 02:07:19.000000 Firenado-0.9.0a1/firenado/management/management.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6791 2022-04-13 19:58:05.000000 Firenado-0.9.0a1/firenado/management/tasks.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.278004 Firenado-0.9.0a1/firenado/management/templates/
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.286004 Firenado-0.9.0a1/firenado/management/templates/help/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      160 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/management/templates/help/app_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      119 2018-11-03 23:08:57.000000 Firenado-0.9.0a1/firenado/management/templates/help/header.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       46 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/management/templates/help/init_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      252 2018-11-03 23:09:50.000000 Firenado-0.9.0a1/firenado/management/templates/help/main_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      117 2017-06-19 04:13:32.000000 Firenado-0.9.0a1/firenado/management/templates/help/project_command_help.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      241 2020-02-29 17:12:35.000000 Firenado-0.9.0a1/firenado/management/templates/help/random_command_help.txt
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.286004 Firenado-0.9.0a1/firenado/management/templates/project/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      224 2018-11-21 07:38:12.000000 Firenado-0.9.0a1/firenado/management/templates/project/app.py.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      691 2016-09-10 17:22:04.000000 Firenado-0.9.0a1/firenado/management/templates/project/firenado.yml.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      212 2018-11-21 07:38:12.000000 Firenado-0.9.0a1/firenado/management/templates/project/handlers.py.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       54 2016-09-08 01:38:40.000000 Firenado-0.9.0a1/firenado/management/templates/project/init_command_help.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    15364 2022-04-16 01:20:31.000000 Firenado-0.9.0a1/firenado/schedule.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    10107 2022-12-18 22:48:38.000000 Firenado-0.9.0a1/firenado/security.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4906 2023-01-30 02:42:51.000000 Firenado-0.9.0a1/firenado/service.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    22717 2023-03-01 19:37:22.000000 Firenado-0.9.0a1/firenado/session.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     6160 2023-06-06 03:01:08.000000 Firenado-0.9.0a1/firenado/sqlalchemy.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4608 2022-11-12 06:31:24.000000 Firenado-0.9.0a1/firenado/testing.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    21715 2023-05-19 18:16:54.000000 Firenado-0.9.0a1/firenado/tornadoweb.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      847 2021-03-23 16:46:58.000000 Firenado-0.9.0a1/firenado/uimodules.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.287004 Firenado-0.9.0a1/firenado/util/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-02-29 17:12:35.000000 Firenado-0.9.0a1/firenado/util/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1084 2019-05-18 04:12:19.000000 Firenado-0.9.0a1/firenado/util/argparse_util.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      939 2023-06-06 01:39:44.000000 Firenado-0.9.0a1/firenado/util/sqlalchemy_util.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      920 2019-05-18 04:12:04.000000 Firenado-0.9.0a1/firenado/util/url_util.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.288004 Firenado-0.9.0a1/requirements/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       62 2020-07-28 14:20:19.000000 Firenado-0.9.0a1/requirements/all.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       29 2023-06-05 21:13:20.000000 Firenado-0.9.0a1/requirements/basic.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       15 2022-07-23 21:52:18.000000 Firenado-0.9.0a1/requirements/pexpect.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       28 2022-07-23 21:51:27.000000 Firenado-0.9.0a1/requirements/redis.txt
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       16 2022-12-23 19:45:17.000000 Firenado-0.9.0a1/requirements/schedule.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       19 2023-06-06 03:02:10.000000 Firenado-0.9.0a1/requirements/sqlalchemy.txt
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      103 2023-06-06 15:02:38.291004 Firenado-0.9.0a1/setup.cfg
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3716 2023-06-05 21:12:00.000000 Firenado-0.9.0a1/setup.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.289004 Firenado-0.9.0a1/tests/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2180 2022-08-30 18:19:09.000000 Firenado-0.9.0a1/tests/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2010 2022-12-18 22:09:16.000000 Firenado-0.9.0a1/tests/components_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     9962 2022-04-20 03:19:42.000000 Firenado-0.9.0a1/tests/conf_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1903 2021-03-23 17:03:37.000000 Firenado-0.9.0a1/tests/config_test.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5212 2022-12-18 22:07:05.000000 Firenado-0.9.0a1/tests/data_test.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.289004 Firenado-0.9.0a1/tests/features/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2019-05-18 04:12:19.000000 Firenado-0.9.0a1/tests/features/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1021 2020-03-17 14:16:49.000000 Firenado-0.9.0a1/tests/features/environment.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.290004 Firenado-0.9.0a1/tests/features/steps/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-03-17 14:16:49.000000 Firenado-0.9.0a1/tests/features/steps/__init__.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1037 2022-07-22 14:57:31.000000 Firenado-0.9.0a1/tests/features/steps/cli.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2403 2022-04-16 02:44:17.000000 Firenado-0.9.0a1/tests/features/steps/launcher.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1802 2022-12-18 22:01:58.000000 Firenado-0.9.0a1/tests/runtests.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3095 2023-06-05 20:59:34.000000 Firenado-0.9.0a1/tests/security_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8036 2023-06-06 02:55:20.000000 Firenado-0.9.0a1/tests/service_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     5182 2022-12-24 04:00:43.000000 Firenado-0.9.0a1/tests/session_test.py
--rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     8874 2023-06-06 02:56:41.000000 Firenado-0.9.0a1/tests/sqlalchemy_test.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6025 2021-03-23 17:08:06.000000 Firenado-0.9.0a1/tests/tornadoweb_test.py
-drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-06 15:02:38.290004 Firenado-0.9.0a1/tests/util/
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2018-07-08 04:28:25.000000 Firenado-0.9.0a1/tests/util/__init__.py
--rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1895 2021-03-23 17:10:31.000000 Firenado-0.9.0a1/tests/util/url_util_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.955233 Firenado-0.9.0a2/
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.941232 Firenado-0.9.0a2/Firenado.egg-info/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5202 2023-06-14 15:03:16.000000 Firenado-0.9.0a2/Firenado.egg-info/PKG-INFO
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2539 2023-06-14 15:03:16.000000 Firenado-0.9.0a2/Firenado.egg-info/SOURCES.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        1 2023-06-14 15:03:16.000000 Firenado-0.9.0a2/Firenado.egg-info/dependency_links.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       71 2023-06-14 15:03:16.000000 Firenado-0.9.0a2/Firenado.egg-info/entry_points.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      240 2023-06-14 15:03:16.000000 Firenado-0.9.0a2/Firenado.egg-info/requires.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       15 2023-06-14 15:03:16.000000 Firenado-0.9.0a2/Firenado.egg-info/top_level.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    11361 2022-01-22 03:40:14.000000 Firenado-0.9.0a2/LICENSE
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      593 2021-03-14 16:46:20.000000 Firenado-0.9.0a2/MANIFEST.in
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5202 2023-06-14 15:03:16.955233 Firenado-0.9.0a2/PKG-INFO
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3789 2022-04-15 16:36:51.000000 Firenado-0.9.0a2/README.md
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3118 2019-01-26 05:48:04.000000 Firenado-0.9.0a2/README.rst
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.943232 Firenado-0.9.0a2/firenado/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1067 2023-06-14 14:51:23.000000 Firenado-0.9.0a2/firenado/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3895 2023-06-05 20:36:53.000000 Firenado-0.9.0a2/firenado/_pexpect_async_patch.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.943232 Firenado-0.9.0a2/firenado/bin/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-10 05:12:04.000000 Firenado-0.9.0a2/firenado/bin/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      716 2023-06-10 05:14:23.000000 Firenado-0.9.0a2/firenado/bin/firenado-cli.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      727 2023-06-14 14:53:43.000000 Firenado-0.9.0a2/firenado/bin/firenado-cli1.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.943232 Firenado-0.9.0a2/firenado/cli/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       31 2023-06-14 14:53:43.000000 Firenado-0.9.0a2/firenado/cli/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      620 2023-06-14 14:53:43.000000 Firenado-0.9.0a2/firenado/cli/commands.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      194 2023-06-14 14:53:43.000000 Firenado-0.9.0a2/firenado/cli/root.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.943232 Firenado-0.9.0a2/firenado/components/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      759 2019-01-19 15:51:14.000000 Firenado-0.9.0a2/firenado/components/__init__.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.944232 Firenado-0.9.0a2/firenado/components/firenado/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.9.0a2/firenado/components/firenado/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      872 2016-09-08 01:38:40.000000 Firenado-0.9.0a2/firenado/components/firenado/component.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1063 2016-09-08 01:38:40.000000 Firenado-0.9.0a2/firenado/components/firenado/handlers.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.944232 Firenado-0.9.0a2/firenado/components/firenado/templates/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4008 2016-08-29 15:57:57.000000 Firenado-0.9.0a2/firenado/components/firenado/templates/info.html
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.946232 Firenado-0.9.0a2/firenado/components/static_maps/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-09-08 01:38:40.000000 Firenado-0.9.0a2/firenado/components/static_maps/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4137 2018-08-25 00:58:30.000000 Firenado-0.9.0a2/firenado/components/static_maps/component.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.946232 Firenado-0.9.0a2/firenado/components/toolbox/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2016-11-26 15:05:30.000000 Firenado-0.9.0a2/firenado/components/toolbox/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      831 2016-11-26 15:05:30.000000 Firenado-0.9.0a2/firenado/components/toolbox/component.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1937 2023-06-10 05:29:53.000000 Firenado-0.9.0a2/firenado/components/toolbox/uimodules.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.947232 Firenado-0.9.0a2/firenado/conf/
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4774 2023-06-14 14:53:43.000000 Firenado-0.9.0a2/firenado/conf/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1092 2022-12-23 19:35:46.000000 Firenado-0.9.0a2/firenado/conf/firenado.yml
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    17819 2023-06-10 05:19:53.000000 Firenado-0.9.0a2/firenado/config.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    15458 2023-06-06 03:00:02.000000 Firenado-0.9.0a2/firenado/data.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    13899 2023-06-14 14:51:23.000000 Firenado-0.9.0a2/firenado/launcher.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.947232 Firenado-0.9.0a2/firenado/management/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      738 2019-05-18 04:12:04.000000 Firenado-0.9.0a2/firenado/management/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1993 2020-02-29 17:12:35.000000 Firenado-0.9.0a2/firenado/management/commands.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8615 2023-06-10 05:24:28.000000 Firenado-0.9.0a2/firenado/management/management.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6784 2023-06-10 05:27:13.000000 Firenado-0.9.0a2/firenado/management/tasks.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.936232 Firenado-0.9.0a2/firenado/management/templates/
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.949232 Firenado-0.9.0a2/firenado/management/templates/help/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      160 2016-09-08 01:38:40.000000 Firenado-0.9.0a2/firenado/management/templates/help/app_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      119 2018-11-03 23:08:57.000000 Firenado-0.9.0a2/firenado/management/templates/help/header.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       46 2016-09-08 01:38:40.000000 Firenado-0.9.0a2/firenado/management/templates/help/init_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      252 2018-11-03 23:09:50.000000 Firenado-0.9.0a2/firenado/management/templates/help/main_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      117 2017-06-19 04:13:32.000000 Firenado-0.9.0a2/firenado/management/templates/help/project_command_help.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      241 2020-02-29 17:12:35.000000 Firenado-0.9.0a2/firenado/management/templates/help/random_command_help.txt
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.951233 Firenado-0.9.0a2/firenado/management/templates/project/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      224 2018-11-21 07:38:12.000000 Firenado-0.9.0a2/firenado/management/templates/project/app.py.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      691 2016-09-10 17:22:04.000000 Firenado-0.9.0a2/firenado/management/templates/project/firenado.yml.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      212 2018-11-21 07:38:12.000000 Firenado-0.9.0a2/firenado/management/templates/project/handlers.py.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       54 2016-09-08 01:38:40.000000 Firenado-0.9.0a2/firenado/management/templates/project/init_command_help.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    15352 2023-06-10 05:20:55.000000 Firenado-0.9.0a2/firenado/schedule.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    10095 2023-06-14 14:53:43.000000 Firenado-0.9.0a2/firenado/security.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     4894 2023-06-10 05:21:44.000000 Firenado-0.9.0a2/firenado/service.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)    22717 2023-03-01 19:37:22.000000 Firenado-0.9.0a2/firenado/session.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     6160 2023-06-06 03:01:08.000000 Firenado-0.9.0a2/firenado/sqlalchemy.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     4596 2023-06-14 14:53:43.000000 Firenado-0.9.0a2/firenado/testing.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)    21703 2023-06-10 05:22:53.000000 Firenado-0.9.0a2/firenado/tornadoweb.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      847 2023-06-10 05:23:10.000000 Firenado-0.9.0a2/firenado/uimodules.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.952232 Firenado-0.9.0a2/firenado/util/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-02-29 17:12:35.000000 Firenado-0.9.0a2/firenado/util/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1084 2023-06-10 05:28:19.000000 Firenado-0.9.0a2/firenado/util/argparse_util.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)      901 2023-06-10 05:28:55.000000 Firenado-0.9.0a2/firenado/util/sqlalchemy_util.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      896 2023-06-10 05:28:37.000000 Firenado-0.9.0a2/firenado/util/url_util.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.953233 Firenado-0.9.0a2/requirements/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       62 2020-07-28 14:20:19.000000 Firenado-0.9.0a2/requirements/all.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       29 2023-06-05 21:13:20.000000 Firenado-0.9.0a2/requirements/basic.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       15 2022-07-23 21:52:18.000000 Firenado-0.9.0a2/requirements/pexpect.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       28 2022-07-23 21:51:27.000000 Firenado-0.9.0a2/requirements/redis.txt
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)       17 2023-06-14 14:51:23.000000 Firenado-0.9.0a2/requirements/schedule.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)       19 2023-06-06 03:02:10.000000 Firenado-0.9.0a2/requirements/sqlalchemy.txt
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)      103 2023-06-14 15:03:16.955233 Firenado-0.9.0a2/setup.cfg
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     3704 2023-06-10 05:06:48.000000 Firenado-0.9.0a2/setup.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.954233 Firenado-0.9.0a2/tests/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2180 2022-08-30 18:19:09.000000 Firenado-0.9.0a2/tests/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     2010 2022-12-18 22:09:16.000000 Firenado-0.9.0a2/tests/components_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     9962 2023-06-10 05:31:08.000000 Firenado-0.9.0a2/tests/conf_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1903 2023-06-10 05:31:25.000000 Firenado-0.9.0a2/tests/config_test.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     5212 2023-06-10 05:31:35.000000 Firenado-0.9.0a2/tests/data_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.954233 Firenado-0.9.0a2/tests/features/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2019-05-18 04:12:19.000000 Firenado-0.9.0a2/tests/features/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1021 2023-06-10 05:33:47.000000 Firenado-0.9.0a2/tests/features/environment.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.955233 Firenado-0.9.0a2/tests/features/steps/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2020-03-17 14:16:49.000000 Firenado-0.9.0a2/tests/features/steps/__init__.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     1037 2023-06-14 14:53:43.000000 Firenado-0.9.0a2/tests/features/steps/cli.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     2227 2023-06-14 14:51:23.000000 Firenado-0.9.0a2/tests/features/steps/launcher.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1802 2023-06-10 05:30:37.000000 Firenado-0.9.0a2/tests/runtests.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     3083 2023-06-14 14:53:43.000000 Firenado-0.9.0a2/tests/security_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     8024 2023-06-10 05:32:16.000000 Firenado-0.9.0a2/tests/service_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     5170 2023-06-10 05:32:35.000000 Firenado-0.9.0a2/tests/session_test.py
+-rw-r--r--   0 fpiraz    (1000) fpiraz    (1000)     8862 2023-06-10 05:32:47.000000 Firenado-0.9.0a2/tests/sqlalchemy_test.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     6025 2023-06-10 05:32:56.000000 Firenado-0.9.0a2/tests/tornadoweb_test.py
+drwxr-xr-x   0 fpiraz    (1000) fpiraz    (1000)        0 2023-06-14 15:03:16.955233 Firenado-0.9.0a2/tests/util/
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)        0 2018-07-08 04:28:25.000000 Firenado-0.9.0a2/tests/util/__init__.py
+-rw-rw-r--   0 fpiraz    (1000) fpiraz    (1000)     1895 2021-03-23 17:10:31.000000 Firenado-0.9.0a2/tests/util/url_util_test.py
```

### Comparing `Firenado-0.9.0a1/Firenado.egg-info/PKG-INFO` & `Firenado-0.9.0a2/Firenado.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Firenado
-Version: 0.9.0a1
+Version: 0.9.0a2
 Summary: Firenado is a python web framework based on Tornado web framework/server.
 Home-page: https://github.com/candango/firenado
 Author: Flávio Gonçalves Garcia
 Author-email: piraz@candango.org
 Maintainer: Flávio Gonçalves Garcia
 Maintainer-email: piraz@candango.org
 License: Apache License V2.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: redis
 Provides-Extra: pexpect
 Provides-Extra: schedule
 Provides-Extra: sqlalchemy
 License-File: LICENSE
```

### Comparing `Firenado-0.9.0a1/Firenado.egg-info/SOURCES.txt` & `Firenado-0.9.0a2/Firenado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/LICENSE` & `Firenado-0.9.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/MANIFEST.in` & `Firenado-0.9.0a2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/PKG-INFO` & `Firenado-0.9.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Firenado
-Version: 0.9.0a1
+Version: 0.9.0a2
 Summary: Firenado is a python web framework based on Tornado web framework/server.
 Home-page: https://github.com/candango/firenado
 Author: Flávio Gonçalves Garcia
 Author-email: piraz@candango.org
 Maintainer: Flávio Gonçalves Garcia
 Maintainer-email: piraz@candango.org
 License: Apache License V2.0
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: redis
 Provides-Extra: pexpect
 Provides-Extra: schedule
 Provides-Extra: sqlalchemy
 License-File: LICENSE
```

### Comparing `Firenado-0.9.0a1/README.md` & `Firenado-0.9.0a2/README.md`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/README.rst` & `Firenado-0.9.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/__init__.py` & `Firenado-0.9.0a2/firenado/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """The Firenado Framework"""
 
 __author__ = "Flávio Gonçalves Garcia <piraz@candango.org>"
-__version__ = (0, 9, 0, "a1")
+__version__ = (0, 9, 0, "a2")
 __licence__ = "Apache License V2.0"
 
 
 def get_version():
     if isinstance(__version__[-1], str):
         return '.'.join(map(str, __version__[:-1])) + __version__[-1]
     return ".".join(map(str, __version__))
```

### Comparing `Firenado-0.9.0a1/firenado/_pexpect_async_patch.py` & `Firenado-0.9.0a2/firenado/_pexpect_async_patch.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/bin/firenado-cli.py` & `Firenado-0.9.0a2/firenado/bin/firenado-cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
-# -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/bin/firenado-cli1.py` & `Firenado-0.9.0a2/firenado/bin/firenado-cli1.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/cli/commands.py` & `Firenado-0.9.0a2/firenado/cli/commands.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/components/__init__.py` & `Firenado-0.9.0a2/firenado/components/__init__.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/components/firenado/component.py` & `Firenado-0.9.0a2/firenado/components/firenado/component.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/components/firenado/handlers.py` & `Firenado-0.9.0a2/firenado/components/firenado/handlers.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/components/firenado/templates/info.html` & `Firenado-0.9.0a2/firenado/components/firenado/templates/info.html`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/components/static_maps/component.py` & `Firenado-0.9.0a2/firenado/components/static_maps/component.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/components/toolbox/component.py` & `Firenado-0.9.0a2/firenado/components/toolbox/component.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/components/toolbox/uimodules.py` & `Firenado-0.9.0a2/firenado/components/toolbox/uimodules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python
-#
-# Copyright 2015-2020 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/firenado/conf/__init__.py` & `Firenado-0.9.0a2/firenado/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/conf/firenado.yml` & `Firenado-0.9.0a2/firenado/conf/firenado.yml`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/config.py` & `Firenado-0.9.0a2/firenado/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/data.py` & `Firenado-0.9.0a2/firenado/data.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/launcher.py` & `Firenado-0.9.0a2/firenado/launcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: UTF-8 -*-
-#
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,20 +14,19 @@
 
 from cartola import sysexits
 import firenado.conf
 from importlib import reload
 import logging
 import os
 import sys
-import warnings
 
 logger = logging.getLogger(__name__)
 
 
-class FirenadoLauncher(object):
+class FirenadoLauncher:
 
     def __init__(self, **settings):
         self.app = settings.get("app", None)
         self.path = settings.get("path", None)
         if self.path is not None:
             sys.path.append(self.path)
         if self.app:
@@ -44,21 +41,19 @@
         # Fixing and cleaning PYTHONPATH and sys.path
         # This is useful so we can run a process launcher with the same
         # PYTHONPATH from the parent process
         real_pythonpaths = sys.path[:]
         if "PYTHONPATH" in os.environ and os.environ['PYTHONPATH'] is not None:
             current_pythonpaths = os.environ['PYTHONPATH'].split(":")
             for path in current_pythonpaths:
-                if path.strip() != "":
-                    if path.strip() not in real_pythonpaths:
-                        real_pythonpaths.append(path.strip())
+                if path.strip() != "" and path.strip() not in real_pythonpaths:
+                    real_pythonpaths.append(path.strip())
             for path in sys.path:
-                if path.strip() != "":
-                    if path.strip() not in real_pythonpaths:
-                        real_pythonpaths.append(path.strip())
+                if path.strip() != "" and path.strip() not in real_pythonpaths:
+                    real_pythonpaths.append(path.strip())
         sys.path = real_pythonpaths
         os.environ['PYTHONPATH'] = ":".join(real_pythonpaths)
         if self.dir is not None:
             os.chdir(self.dir)
         if self.app is not None or self.dir is not None:
             reload(firenado.conf)
 
@@ -108,15 +103,15 @@
     else:
         return exp.expect_loop(timeout)
 
 
 class ProcessLauncher(FirenadoLauncher):
     try:
         import pexpect
-        process = None  # type: pexpect.spawn
+        process: pexpect.spawn = None
     except ImportError:
         logger.debug("The pexpect module ins't isn't installed. Consider "
                      "installing it in order to launch applications using "
                      "ProcessLauncher.")
 
     def __init__(self, **settings):
         super().__init__(**settings)
@@ -126,65 +121,57 @@
         self.logfile = settings.get("logfile", None)
         self.command = None
         self.response = None
 
     def load(self):
         firenado_script = os.path.join(firenado.conf.ROOT, "bin",
                                        "firenado-cli.py")
-        self.command = "%s %s app run" % (sys.executable, firenado_script)
+        self.command = f"{sys.executable} {firenado_script} app run"
         if self.dir is not None:
-            dir_parameter = "--dir=%s" % self.dir
-            self.command = "%s %s" % (self.command, dir_parameter)
-
-        if self.socket is None:
-            if self.addresses is not None:
-                addresses_parameter = "--port=%s" % self.addresses
-                self.command = "%s %s" % (self.command, addresses_parameter)
-            if self.port is not None:
-                port_parameter = "--port=%s" % self.port
-                self.command = "%s %s" % (self.command, port_parameter)
-        else:
-            socket_parameter = "--port=%s" % self.socket
-            self.command = "%s %s" % (self.command, socket_parameter)
+            self.command = f"{self.command} --dir={self.dir}"
+        if self.socket is None and self.addresses is not None:
+            self.command = f"{self.command} --addresses={self.addresses}"
+        if self.socket is None and self.port is not None:
+            self.command = f"{self.command} --port={self.port}"
+        if self.socket is not None:
+            self.command = f"{self.command} --socke={self.socket}"
 
     async def read_process(self):
         import pexpect
         self.process_callback.stop()
         try:
             # Simple way to catch everything is wait for a new line:
             #
             await self.process.expect("\n", async_=True)
         except pexpect.TIMEOUT:
             logger.debug("Reached timeout, getting back in the loop.")
         self.process_callback.start()
 
     async def launch(self):
-        with warnings.catch_warnings():
-            import pexpect
-            import tornado.ioloop
-            logger.info("Launching %s", self.command)
-            parameters = {
-                'command': self.command,
-                'encoding': "utf-8"
-            }
-            if self.dir:
-                parameters['cwd'] = self.dir
-            if self.logfile is not None:
-                parameters['logfile'] = self.logfile
-            self.process = pexpect.spawn(**parameters)
-            self.process.expect_list = expect_list_mp.__get__(self.process,
-                                                              pexpect.spawn)
-            warnings.simplefilter("ignore")
-            await self.process.expect(
-                [r"[Firenado server started successfully].*"], async_=True)
-            self.process_callback = tornado.ioloop.PeriodicCallback(
-                self.read_process,
-                self.process_callback_time
-            )
-            self.process_callback.start()
+        import pexpect
+        import tornado.ioloop
+        logger.info("Launching %s", self.command)
+        parameters = {
+            'command': self.command,
+            'encoding': "utf-8"
+        }
+        if self.dir:
+            parameters['cwd'] = self.dir
+        if self.logfile is not None:
+            parameters['logfile'] = self.logfile
+        self.process = pexpect.spawn(**parameters)
+        self.process.expect_list = expect_list_mp.__get__(self.process,
+                                                          pexpect.spawn)
+        await self.process.expect(
+            [r"[Firenado server started successfully].*"], async_=True)
+        self.process_callback = tornado.ioloop.PeriodicCallback(
+            self.read_process,
+            self.process_callback_time
+        )
+        self.process_callback.start()
 
     def send(self, line):
         logger.info("Sending line %s", line)
         self.process.sendline(line)
 
     def shutdown(self):
         logger.warning("Shutting down process launcher.")
@@ -215,14 +202,15 @@
         # TODO: Resolve module if doesn't exists
         if firenado.conf.app['pythonpath']:
             sys.path.append(firenado.conf.app['pythonpath'])
         self.application = TornadoApplication(**firenado.conf.app['settings'])
 
     def launch(self):
         import signal
+        from tornado.ioloop import IOLoop
         import tornado.httpserver
         signal.signal(signal.SIGTERM, self.sig_handler)
         signal.signal(signal.SIGINT, self.sig_handler)
         if os.name == "posix":
             signal.signal(signal.SIGTSTP, self.sig_handler)
         self.http_server = tornado.httpserver.HTTPServer(self.application)
         if firenado.conf.app['xheaders'] is not None and type(
@@ -255,110 +243,102 @@
                     if self.add_sockets(self.port, address):
                         listening_count += 1
             else:
                 if self.add_sockets(self.port):
                     listening_count += 1
         if listening_count:
             if listening_count > 1:
-                listening_what = "%ss" % listening_what
+                listening_what = f"{listening_what}s"
             logger.info("Firenado server started successfully. Listening at %s"
                         " %s.", listening_count, listening_what)
             if firenado.conf.app['process']['num_processes'] is not None:
-                import tornado.process
+                from tornado.process import fork_processes
                 num_processes = firenado.conf.app['process']['num_processes']
                 max_restarts = firenado.conf.app['process']['max_restarts']
                 num_processes_alert = num_processes
                 if num_processes == 0:
-                    num_processes_alert = ("0 (assuming %s as cpu count)" %
-                                           tornado.process.cpu_count())
+                    num_processes_alert = (
+                        f"0 (assuming {tornado.process.cpu_count()} as cpu "
+                        "count)")
                 logger.info("Tornado set to start %s processes with %s max "
                             "restarts.", num_processes_alert, max_restarts)
-                tornado.process.fork_processes(num_processes, max_restarts)
-            tornado.ioloop.IOLoop.current().start()
+                fork_processes(num_processes, max_restarts)
+            IOLoop.current().start()
         else:
             logger.critical("Firenado unable to start.")
             sysexits.exit_fatal(sysexits.EX_SOFTWARE)
 
     def sig_handler(self, sig, _):
         """ Handle the signal sent to the process
         :param sig:  Signal set to the process
         :param _: Frame is not being used
         """
-        import tornado.ioloop
+        from tornado.ioloop import IOLoop
         from tornado.process import task_id
         tid = task_id()
         pid = os.getpid()
         if tid is None:
             logger.warning("main process (pid %s) caught signal: %s", pid, sig)
         else:
             logger.warning("child %s (pid %s) caught signal: %s", tid, pid,
                            sig)
-        tornado.ioloop.IOLoop.current().add_callback_from_signal(self.shutdown)
+        IOLoop.current().add_callback_from_signal(self.shutdown)
 
-    def add_sockets(self, port, address=None):
+    def add_sockets(self, port: int, address: str = None):
         from socket import gaierror
+        from tornado.netutil import bind_sockets
         try:
-            from tornado.netutil import bind_sockets
-            if address:
-                sockets = bind_sockets(port, address.strip())
-            else:
-                sockets = bind_sockets(port)
+            if address is None:
                 address = "127.0.0.1"
+            sockets = bind_sockets(port, address.strip())
             self.http_server.add_sockets(sockets)
             logger.info("Firenado listening at http://%s:%s.", address.strip(),
                         port)
             return True
-        except gaierror as error:
+        except gaierror:
             logger.error("Firenado failed to listen at http://%s:%s.",
                          address.strip(), port)
-        except OSError as error:
+        except OSError:
             logger.error("Firenado failed to listen at http://%s:%s. Check if "
                          "another process is listening at this port or if you "
                          "provided a dns name and the correspondent ip in the "
                          "addresses configuration or if the machine owns the "
-                         "ip Fireando will start to listen.", address, port)
+                         "ip Firenado will start to listen.", address, port)
         return False
 
     def shutdown(self):
-        import time
-        import tornado.ioloop
+        from tornado.ioloop import IOLoop
         from tornado.process import task_id
+        import time
+
+        def log_message(message: str, pid: int, tid: int = None):
+            if tid is None:
+                logger.info("main process (pid %s): %s", pid, message)
+                return
+            logger.info("child %s (pid %s): %s", tid, pid, message)
+
         tid = task_id()
         pid = os.getpid()
-        if tid is None:
-            logger.info("main process (pid %s): stopping http server.", pid)
-        else:
-            logger.info("child %s (pid %s): stopping http server.", tid, pid)
+        log_message("stopping http server", pid, tid)
         for key, component in self.application.components.items():
             component.shutdown()
         self.http_server.stop()
 
-        io_loop = tornado.ioloop.IOLoop.current()
+        io_loop: IOLoop = IOLoop.current()
 
         if self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN == 0:
             io_loop.stop()
-            if tid is None:
-                logger.info("main process (pid %s): application is down", pid)
-            else:
-                logger.info("child %s (pid %s): application is down", tid, pid)
-        else:
-            if tid is None:
-                logger.info("main process (pid %s): shutdown in %s seconds "
-                            "...", pid, self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN)
-            else:
-                logger.info("child %s (pid %s): shutdown in %s seconds ...",
-                            tid, pid, self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN)
-            deadline = time.time() + self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN
-
-            def stop_loop():
-                now = time.time()
-                if now < deadline:
-                    io_loop.add_timeout(now + 1, stop_loop)
-                else:
-                    io_loop.stop()
-                    if tid is None:
-                        logger.info("main process (pid %s): application is "
-                                    "down", pid)
-                    else:
-                        logger.info("child %s (pid %s): application is down",
-                                    tid, pid)
-            stop_loop()
+            log_message("application is down", pid, tid)
+            return
+
+        log_message(f"shutdown in {self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN}s"
+                    " seconds", pid, tid)
+        deadline = time.time() + self.MAX_WAIT_SECONDS_BEFORE_SHUTDOWN
+
+        def stop_loop():
+            now = time.time()
+            if now < deadline:
+                io_loop.add_timeout(now + 1, stop_loop)
+                return
+            io_loop.stop()
+            log_message("application is down", pid, tid)
+        stop_loop()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/management/__init__.py` & `Firenado-0.9.0a2/firenado/management/__init__.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/management/commands.py` & `Firenado-0.9.0a2/firenado/management/commands.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/management/management.py` & `Firenado-0.9.0a2/firenado/management/management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/management/tasks.py` & `Firenado-0.9.0a2/firenado/management/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,27 +13,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from cartola import fs
 import firenado.conf
 from firenado.management import ManagementTask
-from firenado.util import argparse_util
 import logging
 import os
 import sys
 
 logger = logging.getLogger(__name__)
 
 
 class CreateProjectTask(ManagementTask):
-    """
-    Creates a new project from scratch
-    """
     def run(self, namespace):
+        """
+        Creates a new project from scratch
+        """
         from tornado import template
         if len(sys.argv) > 2:
             module = namespace.module
             component = module.replace(".", " ").title().replace(" ", "")
             project_name = module.replace(".", "_").lower()
             project_directory = fs.create_module(module, os.getcwd())
             # TODO: Check if project exists
@@ -90,14 +89,15 @@
         return str(exception)
 
 
 class InstallProjectTask(ManagementTask):
     """ Triggers the install method of all components registered in the
     application.
     """
+
     def run(self, namespace):
         # TODO: Resolve module if doesn't exists
         if firenado.conf.app['pythonpath']:
             sys.path.append(firenado.conf.app['pythonpath'])
         # TODO This should consider the type of application being handled by
         # Firenado.
         from firenado.tornadoweb import TornadoApplication
@@ -112,18 +112,18 @@
         parser.add_argument("-a", "--addresses", default=None)
         parser.add_argument("-A", "--app", default=None)
         parser.add_argument("-d", "--dir", default=None)
         parser.add_argument("-p", "--path", default=None)
         parser.add_argument("-P", "--port", type=int)
         parser.add_argument("-s", "--socket", default=None)
 
-    """ Runs a Firenado Tornado Application based
-    on the it's project configuration
-    """
     def run(self, namespace):
+        """ Runs a Firenado Tornado Application based
+        on the it's project configuration
+        """
         # TODO throw a custom error when type is not found
         from firenado.config import get_class_from_config
         parameters = {}
         if namespace.app is not None:
             parameters['app'] = namespace.app
         if namespace.dir is not None:
             parameters['dir'] = namespace.dir
@@ -159,14 +159,14 @@
             sys.exit(1)
         logger.debug("Displaying a random string with size {}".format(size))
         print(security.random_string(size))
         sys.exit(0)
 
 
 class GenerateUuidTask(ManagementTask):
-    """ Generates an uuid4 string
-    """
     def run(self, namespace):
+        """ Generates an uuid4 string
+        """
         from uuid import uuid4
         logger.debug("Displaying a random uuid4 string.")
         print(uuid4())
         sys.exit(0)
```

### Comparing `Firenado-0.9.0a1/firenado/management/templates/project/firenado.yml.txt` & `Firenado-0.9.0a2/firenado/management/templates/project/firenado.yml.txt`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/schedule.py` & `Firenado-0.9.0a2/firenado/schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/security.py` & `Firenado-0.9.0a2/firenado/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2023 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/service.py` & `Firenado-0.9.0a2/firenado/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2023 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/session.py` & `Firenado-0.9.0a2/firenado/session.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/sqlalchemy.py` & `Firenado-0.9.0a2/firenado/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/firenado/testing.py` & `Firenado-0.9.0a2/firenado/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/tornadoweb.py` & `Firenado-0.9.0a2/firenado/tornadoweb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/uimodules.py` & `Firenado-0.9.0a2/firenado/uimodules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/firenado/util/argparse_util.py` & `Firenado-0.9.0a2/firenado/util/argparse_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2015-2019 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/firenado/util/sqlalchemy_util.py` & `Firenado-0.9.0a2/firenado/util/sqlalchemy_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: UTF-8 -*-
-#
-# Copyright 2015-2023 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/firenado/util/url_util.py` & `Firenado-0.9.0a2/firenado/util/url_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python
-#
-# Copyright 2015-2017 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/setup.py` & `Firenado-0.9.0a2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -55,15 +55,15 @@
     long_description_content_type="text/markdown",
     license=firenado.__licence__,
     author=firenado.get_author(),
     author_email=firenado.get_author_email(),
     maintainer=firenado.get_author(),
     maintainer_email=firenado.get_author_email(),
     install_requires=resolve_requires("requirements/basic.txt"),
-    python_requires=">= 3.7",
+    python_requires=">= 3.8",
     extras_require={
         'all': resolve_requires("requirements/all.txt"),
         'redis': resolve_requires("requirements/redis.txt"),
         'pexpect': resolve_requires("requirements/pexpect.txt"),
         'schedule': resolve_requires("requirements/schedule.txt"),
         'sqlalchemy': resolve_requires("requirements/sqlalchemy.txt"),
     },
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/tests/__init__.py` & `Firenado-0.9.0a2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/tests/components_test.py` & `Firenado-0.9.0a2/tests/components_test.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/tests/conf_test.py` & `Firenado-0.9.0a2/tests/conf_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/tests/config_test.py` & `Firenado-0.9.0a2/tests/config_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/tests/data_test.py` & `Firenado-0.9.0a2/tests/data_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/tests/features/environment.py` & `Firenado-0.9.0a2/tests/features/environment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2020 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/tests/features/steps/cli.py` & `Firenado-0.9.0a2/tests/features/steps/cli.py`

 * *Files identical despite different names*

### Comparing `Firenado-0.9.0a1/tests/features/steps/launcher.py` & `Firenado-0.9.0a2/tests/features/steps/launcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: UTF-8 -*-
-#
-# Copyright 2015-2020 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,35 +17,32 @@
 from tests import PROJECT_ROOT, chdir_fixture_app
 from firenado.launcher import ProcessLauncher
 from tornado import gen
 from tornado.httpclient import AsyncHTTPClient
 import sys
 
 
-@given("We launch {application} application using process launcher at {port} "
-       "port")
+@given("{application} application is launched at {port} port")
 @async_run_until_complete
-async def step_we_launch_application_using_process_launcher(context,
-                                                            application, port):
+async def step_application_launched_at_port(context, application, port):
     application_dir = chdir_fixture_app(application, suppress_log=True)
     context.launcher = ProcessLauncher(
         dir=application_dir, path=PROJECT_ROOT, port=port, logfile=sys.stderr)
     context.launcher.load()
     await context.launcher.launch()
     await gen.sleep(1)
     context.tester.assertTrue(context.launcher.is_alive())
 
 
 @when("The application is running correctly at {port} port")
 @async_run_until_complete
 async def step_application_running_correctly_at_port(context, port):
     http_client = AsyncHTTPClient()
     try:
-        response = await http_client.fetch("http://localhost:%s" %
-                                           port)
+        response = await http_client.fetch("http://localhost:%s" % port)
     except Exception as e:
         print("Error: %s" % e)
         context.tester.assertTrue(False)
     else:
         context.tester.assertEquals(b"IndexHandler output", response.body)
         context.tester.assertTrue(context.launcher.is_alive())
```

### Comparing `Firenado-0.9.0a1/tests/runtests.py` & `Firenado-0.9.0a2/tests/runtests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/tests/security_test.py` & `Firenado-0.9.0a2/tests/security_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/tests/service_test.py` & `Firenado-0.9.0a2/tests/service_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015-2023 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/tests/session_test.py` & `Firenado-0.9.0a2/tests/session_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: UTF-8 -*-
 #
-# Copyright 2015-2022 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/tests/sqlalchemy_test.py` & `Firenado-0.9.0a2/tests/sqlalchemy_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2015-2023 Flávio Gonçalves Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Firenado-0.9.0a1/tests/tornadoweb_test.py` & `Firenado-0.9.0a2/tests/tornadoweb_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 #
-# Copyright 2015-2021 Flavio Garcia
+# Copyright 2015-2023 Flavio Garcia
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `Firenado-0.9.0a1/tests/util/url_util_test.py` & `Firenado-0.9.0a2/tests/util/url_util_test.py`

 * *Files identical despite different names*

