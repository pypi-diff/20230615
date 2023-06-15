# Comparing `tmp/embykeeper-2.1.1.tar.gz` & `tmp/embykeeper-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.1.1.tar", last modified: Tue Jun 13 09:11:16 2023, max compression
+gzip compressed data, was "embykeeper-2.2.0.tar", last modified: Thu Jun 15 08:38:45 2023, max compression
```

## Comparing `embykeeper-2.1.1.tar` & `embykeeper-2.2.0.tar`

### file list

```diff
@@ -1,64 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.731705 embykeeper-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 09:11:04.000000 embykeeper-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-06-13 09:11:16.731705 embykeeper-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19846 2023-06-13 09:11:04.000000 embykeeper-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.731705 embykeeper-2.1.1/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-13 09:11:04.000000 embykeeper-2.1.1/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.727705 embykeeper-2.1.1/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20689 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 09:11:16.000000 embykeeper-2.1.1/embykeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-13 09:11:04.000000 embykeeper-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:11:16.731705 embykeeper-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:11:16.731705 embykeeper-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-13 09:11:04.000000 embykeeper-2.1.1/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.106456 embykeeper-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 08:38:29.000000 embykeeper-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 08:38:29.000000 embykeeper-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21320 2023-06-15 08:38:45.106456 embykeeper-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20477 2023-06-15 08:38:29.000000 embykeeper-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.086456 embykeeper-2.2.0/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.090456 embykeeper-2.2.0/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.094456 embykeeper-2.2.0/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.098456 embykeeper-2.2.0/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.098456 embykeeper-2.2.0/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.098456 embykeeper-2.2.0/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.090456 embykeeper-2.2.0/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21320 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:38:44.000000 embykeeper-2.2.0/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.082456 embykeeper-2.2.0/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.082456 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/css/cascadia-code.css
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.082456 embykeeper-2.2.0/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 08:38:29.000000 embykeeper-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 08:38:45.106456 embykeeper-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.106456 embykeeper-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-15 08:38:29.000000 embykeeper-2.2.0/tests/test_cli.py
```

### Comparing `embykeeper-2.1.1/LICENSE` & `embykeeper-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/PKG-INFO` & `embykeeper-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.1.1
+Version: 2.2.0
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -44,26 +44,26 @@
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
+  - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
   - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
   - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
-    - ~~卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)~~ (机器人逻辑频繁变动, 暂时禁用)
     - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
     - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
 
 - Emby 保活
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
 
@@ -78,31 +78,32 @@
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Misty 开注自动注册: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
   - 默认禁用:
     - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
-### 从 PyPi 安装
+### Railway 在线部署
 
-Embykeeper 可以通过 `python` 运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
+Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)
 
-```bash
-pip install embykeeper
-```
+请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
-随后, 您需要执行:
+### 通过 Docker 部署
+
+Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
-embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
+(若您不需要连接本机代理, 可以去除 '--net=host' 参数)
 
-命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
 
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = 1080
 scheme = "socks5"
 
@@ -118,132 +119,142 @@
 ```
 
 对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
 
 随后, 您需要再次执行:
 
 ```bash
-embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+恭喜您！您已经成功部署了 Embykeeper.
+
+当您需要更新版本时, 您需要执行:
 
 ```bash
-tmux
+docker pull embykeeper/embykeeper
 ```
 
-这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
+### 通过 Docker Compose 部署
 
-您随时可以通过运行:
+您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
 
-```bash
-tmux a
+**注意**: 您需要先进行过 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
+
+您需要新建一个文件 `docker-compose.yml`:
+
+```yaml
+version: '3'
+services:
+  embykeeper:
+    container_name: embykeeper
+    image: embykeeper/embykeeper
+    restart: unless-stopped
+    volumes:
+      - ./embykeeper:/app
+    network_mode: host
+  watchtower:
+    container_name: watchtower
+    image: containrrr/watchtower
+    restart: unless-stopped
+    volumes:
+      - /var/run/docker.sock:/var/run/docker.sock:rw
 ```
 
-以重新连接到 `tmux` 终端.
+其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新版本.
 
-当版本更新时, 您需要执行:
+然后运行以下命令以启动:
 
-```
-pip install -U embykeeper
+```bash
+docker-compose up -d
 ```
 
-然后重新运行应用.
+即可在后台启动 embykeeper.
 
-### 从源码构建
+您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
-和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
+### 从 PyPi 安装
+
+Embykeeper 可以通过 `python >= 3.7, < 3.11` 运行, 您可以通过 [virtualvenv](https://virtualenv.pypa.io/) 进行环境的管理:
 
 ```bash
-git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-pip install -e .
+python -m venv embykeeper-venv
+. ./embykeeper-venv/bin/activate
+pip install embykeeper
 ```
 
-然后即可执行 Embykeeper:
+随后, 您需要执行:
 
 ```bash
 embykeeper
 ```
 
-详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
+命令将会在当前目录生成模板 `config.toml` 文件, 您需要配置您的账户信息, 参见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 
-当版本更新时, 您需要执行:
+随后, 您需要再次执行:
 
-```
-git pull
+```bash
+embykeeper
 ```
 
-然后重新运行应用.
-
-### 从 Docker 部署
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
 
 ```bash
-docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
+tmux
 ```
 
-命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息 (详见[从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)).
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
 
-随后, 您需要再次执行:
+您随时可以通过运行:
 
 ```bash
-docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
+tmux a
 ```
 
-您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
-
-恭喜您！您已经成功部署了 Embykeeper.
+以重新连接到 `tmux` 终端.
 
-当您需要更新版本时, 您需要执行:
+当版本更新时, 您需要执行:
 
-```bash
-docker pull embykeeper/embykeeper
+```
+pip install -U embykeeper
 ```
 
-### 通过 Docker Compose 部署
-
-您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
+然后重新运行应用.
 
-**注意**: 您需要先进行过 [从 Docker 部署](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
+### 从源码构建
 
-您需要新建一个文件 `docker-compose.yml`:
+首先拉取并设置环境:
 
-```yaml
-version: '3'
-services:
-  embykeeper:
-    container_name: embykeeper
-    image: embykeeper/embykeeper
-    restart: unless-stopped
-    volumes:
-      - ./embykeeper:/app
-    network_mode: host
-  watchtower:
-    container_name: watchtower
-    image: containrrr/watchtower
-    restart: unless-stopped
-    volumes:
-      - /var/run/docker.sock:/var/run/docker.sock:rw
+```bash
+git clone https://github.com/embykeeper/embykeeper.git
+cd embykeeper
+python -m venv venv
+. ./venv/bin/activate
+pip install -e .
 ```
 
-其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新版本.
-
-然后运行以下命令以启动:
+然后即可执行 Embykeeper:
 
 ```bash
-docker-compose up -d
+embykeeper
 ```
 
-即可在后台启动 embykeeper.
+详细配置方法详见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 
-您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
+当版本更新时, 您需要执行:
+
+```
+git pull
+```
+
+然后重新运行应用.
 
 ## 命令行帮助
 
 您可以通过运行 `embykeeper -h` 以获取帮助:
 
 ```bash
 $ embykeeper -h
@@ -261,14 +272,15 @@
     --no-instant  -I   不立刻执行一次计划任务
     --once        -o   仅执行一次任务而不计划执行
     --debug       -d   开启调试输出, 错误将会导致程序停止运行
     --version     -v   打印 Embykeeper 版本
     --follow      -f   仅启动消息调试
     --analyze     -a   仅启动历史信息分析
     --basedir          设定输出文件默认位置
+    --public           启用在线部署模式
 ```
 
 例如:
 
 ```bash
 # 启动所有功能 (在各账号配置中进一步设置功能开启/关闭)
 $ embykeeper config.toml
@@ -288,62 +300,20 @@
 # 启动所有功能, 只运行一次
 $ embykeeper config.toml --once
 
 # 启动所有功能, 不立即执行一次签到/保活
 $ embykeeper config.toml -I
 ```
 
-您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
-
-```bash
-# 启动历史信息分析
-$ embykeeper config.toml -a
-
-请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
-请输入关键词 (以空格分隔):
-输入时间范围 (以"-"分割): 8:00AM-10:00AM
-请输入各群组最大获取数量 [1000]:
-```
-
-该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
-
-另一个工具是即时信息分析:
-
-![follow screenshot](images/follow.svg)
-
-该工具可以实时输出消息的 ID 等信息, 以方便调试.
-
-## 消息推送与高级用户
-
-您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
-
-本项目涉及的需要 Cloudflare 验证码付费跳过的操作 (例如 Nebula 签到)、可能会引起竞争的操作 (例如自动抢邀请码)将需要高级用户, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
-
-目前有三种方式成为高级用户:
-
-1. 分享 1 个邀请制 Emby 的邀请码;
-2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
-3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
-
-## 支持 Embykeeper
-
-##### 开发者团队
-
-- [jackzzs](https://github.com/jackzzs)
-
-##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
-
-![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
-
 ## 配置项
 
 | 设置项       | 值类型             | 简介                                         | 默认值  |
 | ------------ | ------------------ | -------------------------------------------- | ------- |
 | `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`    |
+| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`     |
 | `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
 | `random`     | `int`              | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
 | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
 | `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
 | `proxy`      | `dict`             | 代理设置                                     | `{}`    |
 | `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
 | `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
@@ -356,22 +326,22 @@
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
 若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
 若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
 当前支持的名称包括:
-| 站点 | 名称 | | 站点 | 名称 |
-| --- | --- | --- |--- | --- |
-| 垃圾影音 | `ljyy` | | 搜书神器 | `sosdbot` |
-| 卷毛鼠 IPTV | `jms_iptv` | | 终点站 | `terminus` |
-| Pornemby | `pornemby` | | Singularity | `singularity` |
-| Peach | `peach` | | Nebula | `nebula` |
-| Bluesea | `bluesea` | | Embyhub | `embyhub` |
-| 卷毛鼠 | `jms` | | 卡戎 | `charon` |
+| 站点        | 名称       |     | 站点        | 名称          |
+| ----------- | ---------- | --- | ----------- | ------------- |
+| 垃圾影音    | `ljyy`     |     | 搜书神器    | `sosdbot`     |
+| 卷毛鼠 IPTV | `jms_iptv` |     | 终点站      | `terminus`    |
+| Pornemby    | `pornemby` |     | Singularity | `singularity` |
+| Peach       | `peach`    |     | Nebula      | `nebula`      |
+| Bluesea     | `bluesea`  |     | Embyhub     | `embyhub`     |
+| 卷毛鼠      | `jms`      |     | 卡戎        | `charon`      |
 
 `proxy` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                    | 默认值      |
 | ---------- | ------ | --------------------------------------- | ----------- |
 | `hostname` | `str`  | 代理服务器地址                          | `localhost` |
 | `port`     | `int`  | 代理端口号                              | `1080`      |
@@ -404,14 +374,36 @@
 [monitor.bgk] # 支持 bgk, embyhub, polo
 unique_name = "your_username_for_registeration" # 自动抢注时使用的用户名
 
 [monitor.pornemby]
 only_history = true # 仅当问题历史中找到答案时自动回答
 ```
 
+## 消息推送与高级用户
+
+您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
+
+本项目涉及的需要 Cloudflare 验证码付费跳过的操作 (例如 Nebula 签到)、可能会引起竞争的操作 (例如自动抢邀请码)将需要高级用户, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
+
+目前有三种方式成为高级用户:
+
+1. 分享 1 个邀请制 Emby 的邀请码;
+2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
+3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
+
+## 支持 Embykeeper
+
+##### 开发者团队
+
+- [jackzzs](https://github.com/jackzzs)
+
+##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
+
+![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
+
 ## 代码重用与开发
 
 代码架构如下:
 
 ```mermaid
 flowchart TD
     A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
@@ -459,10 +451,32 @@
                 break
 ```
 
 上述代码实现每次按对应一个字符按键的功能.
 
 当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
 
+## 开发工具
+
+您可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
+
+```bash
+# 启动历史信息分析
+$ embykeeper config.toml -a
+
+请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
+请输入关键词 (以空格分隔):
+输入时间范围 (以"-"分割): 8:00AM-10:00AM
+请输入各群组最大获取数量 [1000]:
+```
+
+该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
+
+另一个工具是即时信息分析:
+
+![follow screenshot](images/follow.svg)
+
+该工具可以实时输出消息的 ID 等信息, 以方便调试.
+
 ## 趋势
 
 [![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.1.1 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.0 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
 :: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
@@ -45,39 +45,38 @@
 å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
 Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
 å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
 åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
-æºå¨äººç­¾å° - ç»ç¹ç«: [é¢é](https://t.me/embypub) [ç¾¤ç»](https://
-t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) - Nebula: [é¢é]
-(https://t.me/Nebula_Emby) [ç¾¤ç»](https://t.me/NebulaEmbyUser) [æºå¨äºº]
-(https://t.me/Nebula_Account_bot) (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare
-éªè¯ç , éè¦[é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) -
-Singularity: [é¢é](https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://
-t.me/Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) -
-Peach: [é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
-peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
-(https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
-t.me/EdHubot) - Pornemby: [é¢é](https://t.me/pornembyservice) [ç¾¤ç»]
-(https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
-åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
-t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
-t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
-ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
-pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
-~~å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https://t.me/
-Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot)~~
-(æºå¨äººé»è¾é¢ç¹åå¨, ææ¶ç¦ç¨) - ~~BlueSea: [ç¾¤ç»](https://t.me/
-blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~ (æ ååº) -
-~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/
-Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) - Emby
-ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
-Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+æºå¨äººç­¾å° - å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https:/
+/t.me/Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot) - ç»ç¹ç«: [é¢é]
+(https://t.me/embypub) [ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://
+t.me/EmbyPublicBot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
+(https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
+(ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
+t.me/embykeeper_bot?start=__prime)) - Singularity: [é¢é](https://t.me/
+Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/Singularity_Emby_Group)
+[æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach: [é¢é](https://t.me/
+peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
+t.me/peach_emby_bot) - EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https:/
+/t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Pornemby: [é¢é](https://
+t.me/pornembyservice) [ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/
+PronembyTGBot2_bot) - åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1)
+[æºå¨äºº](https://t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV)
+[ç¾¤ç»](https://t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) -
+å¶ä»é Emby ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/
+embykeeper/pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
+~~BlueSea: [ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/
+blueseamusic_bot)~~ (æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/
+CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://
+t.me/JMSIPTV_bot)~~ (æ ååº) - Emby ä¿æ´» -
+å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
+èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
 t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
 Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
 embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
 t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
 [é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime),
 åç­åç¡®çä¸è¬è¯·è°¨æä½¿ç¨) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»](https:
@@ -85,166 +84,168 @@
 æ¢éè¯·ç : [é¢é](https://t.me/viper_emby_channel) [ç¾¤ç»](https://t.me/
 Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
 å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
-(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### ä»
-PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡, æ¨å¯ä»¥éè¿ [conda]
-(https://github.com/conda/conda) æ [virtualvenv](https://virtualenv.pypa.io/
-) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip` å®è£ `embykeeper`
-(éè¦ `python >= 3.7, < 3.11`): ```bash pip install embykeeper ``` éå,
-æ¨éè¦æ§è¡: ```bash embykeeper ``` å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿
-`config.toml` æä»¶, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
-(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [proxy] hostname =
-"127.0.0.1" port = 1080 scheme = "socks5" [[telegram]] api_id = "27894236"
-api_hash = "622159182fdd4b15b627eeb3ac695271" phone = "+8612109347899" [[emby]]
-url = "https://weiss-griffin.com/" username = "carrie19" password =
-"s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿ [Telegram å®ç½]
-(https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
-development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
-æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
-æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
-æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡:
-```bash embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
-ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
-ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
-``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
-æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
-Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
-æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º åä» PyPi
-å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python ç¯å¢, ç¶åæå Github
-å¹¶å®è£: ```bash git clone https://github.com/embykeeper/embykeeper.git cd
-embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash
-embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/
-embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
-æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ### ä» Docker
-é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://
-yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡: ```bash docker run -
-v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
-å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯ (è¯¦è§[ä» Pypi å®è£](https://github.com/
-embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)). éå,
-æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
-net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
-ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### Railway
+å¨çº¿é¨ç½² Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
+(https://railway.app/button.svg)](https://railway.app/template/
+WFYaj9?referralCode=Fj6Yvy) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
+ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
+é¨ç½². ### éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½²,
+æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
+ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
+embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
+net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
+`config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
+æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
+```toml [proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [
+[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
+[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
+ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
+è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
+"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
+æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --
+rm -it --net=host embykeeper/embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
-compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker
-é¨ç½²](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-
+compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
+é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
 %E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
 è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
 ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
 compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
 version: '3' services: embykeeper: container_name: embykeeper image:
 embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
 docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
 watchtower) è¢«ç¨äºèªå¨æ´æ°çæ¬. ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨:
 ```bash docker-compose up -d ``` å³å¯å¨åå°å¯å¨ embykeeper.
 æ¨å¯ä»¥éè¿ `docker logs -f embykeeper` æ `docker-compose logs -
-f embykeeper` ä»¥æ¥çææ°æ¥å¿. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡
-`embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨
-Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
-(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
-(ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
-e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+f embykeeper` ä»¥æ¥çææ°æ¥å¿. ### ä» PyPi å®è£ Embykeeper
+å¯ä»¥éè¿ `python >= 3.7, < 3.11` è¿è¡, æ¨å¯ä»¥éè¿ [virtualvenv]
+(https://virtualenv.pypa.io/) è¿è¡ç¯å¢çç®¡ç: ```bash python -m venv
+embykeeper-venv . ./embykeeper-venv/bin/activate pip install embykeeper ```
+éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, åè§ [éè¿ Docker é¨ç½²](https://
+github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
+Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
+æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
+ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæåå¹¶è®¾ç½®ç¯å¢:
+```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
+python -m venv venv . ./venv/bin/activate pip install -e . ```
+ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§
+[éè¿ Docker é¨ç½²](https://github.com/embykeeper/
+embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2). å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
+æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
+h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
+config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
+c å¯ç¨æ¯æ¥ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --
+emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ --
-basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® ``` ä¾å¦: ```bash # å¯å¨ææåè½
+basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® --public å¯ç¨å¨çº¿é¨ç½²æ¨¡å¼ ```
+ä¾å¦: ```bash # å¯å¨ææåè½
 (å¨åè´¦å·éç½®ä¸­è¿ä¸æ­¥è®¾ç½®åè½å¼å¯/å³é­) $ embykeeper
 config.toml # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 ä»å¯å¨æ¯æ¥ 8:00 PM - 9:00 PM éæºæ¶é´ç­¾å° $ embykeeper config.toml -
 c <8:00PM,9:00PM> # å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -s #
 å¯å¨ææåè½, åªè¿è¡ä¸æ¬¡ $ embykeeper config.toml --once #
 å¯å¨ææåè½, ä¸ç«å³æ§è¡ä¸æ¬¡ç­¾å°/ä¿æ´» $ embykeeper config.toml
--I ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
-ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
-config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
-10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
-"åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
-è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
-ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
-å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
-è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ##
+-I ``` ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------
+-- | ------------------ | -------------------------------------------- | ------
+- | | `timeout` | `int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | |
+`retries` | `int` | Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | |
+`concurrent` | `int` | Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random`
+| `int` | Telegram æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` |
+| `notifier` | `int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/
+ææºå·) | `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/
+çè§åè½å¼å¯ç«ç¹è®¾ç½® | `{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `
+{}` | | `telegram` | `list` | Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
+| `emby` | `list` | Emby è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
+`service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----
+------- | ------ | -------------- | -------------------- | | `checkiner` |
+`list` | å¯ç¨çç­¾å°ç«ç¹ | (å½åæææ¯æçç«ç¹) | | `monitor` |
+`list` | å¯ç¨ççè§ä¼è¯ | (å½åæææ¯æçä¼è¯) | | `messager` |
+`list` | å¯ç¨çæ°´ç¾¤ä¼è¯ | (å½åæææ¯æçä¼è¯) | æ³¨æ,
+å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯, è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡.
+è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
+è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
+ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | ----------- | ---------- | --- | ------
+----- | ------------- | | åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` |
+| å·æ¯é¼  IPTV | `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby |
+`pornemby` | | Singularity | `singularity` | | Peach | `peach` | | Nebula |
+`nebula` | | Bluesea | `bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms`
+| | å¡æ | `charon` | `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å |
+ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------------------
+----- | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
+`localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` | `str`
+| ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
+è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
+------ | ------------------------------------------------------------------ | -
+------ | | `api_id` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/
+)ç³è¯·ç Application ID | | | `api_hash` | `str` | ä»[Telegram å®ç½]
+(https://my.telegram.org/)ç³è¯·ç Application Hash | | | `phone` | `str` |
+è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | | `monitor` | `bool` |
+å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` | `bool` |
+å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹
+| å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | --------------------
+------------------------------------- | ------ | | `url` | `str` | Emby
+æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
+| `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
+æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
+`progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
+æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
+bgk, embyhub, polo unique_name = "your_username_for_registeration" #
+èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
+ä»å½é®é¢åå²ä¸­æ¾å°ç­æ¡æ¶èªå¨åç­ ``` ##
 æ¶æ¯æ¨éä¸é«çº§ç¨æ· æ¨å¯ä»¥éè¿è®¾ç½®é¡¹ "`notifier`" è®¾ç½®
 æå/å¤±è´¥ éç¥å°è¢«åéç Telegram è´¦å·, æ¨å¯ä»¥éè¿
 [Embykeeper Bot](https://t.me/embykeeper_bot)
 è®¾ç½®æ¶æ¯æ¯æ¥åéçæ¶é´. æ¬é¡¹ç®æ¶åçéè¦ Cloudflare
 éªè¯ç ä»è´¹è·³è¿çæä½ (ä¾å¦ Nebula
 ç­¾å°)ãå¯è½ä¼å¼èµ·ç«äºçæä½
 (ä¾å¦èªå¨æ¢éè¯·ç )å°éè¦é«çº§ç¨æ·, æ¨å¯ä»¥éè¿ [Embykeeper
 Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
 (https://afdian.net/a/jackzzs)èµå© ![Kitty](https://github.com/embykeeper/
-embykeeper/raw/main/images/kitty.gif) ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å |
-ç®ä» | é»è®¤å¼ | | ------------ | ------------------ | --------------------
------------------------- | ------- | | `timeout` | `int` | Telegram
-æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | | `retries` | `int` | Telegram
-æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | | `concurrent` | `int` | Telegram
-æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random` | `int` | Telegram
-æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` | | `notifier` |
-`int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/ææºå·) |
-`False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/çè§åè½å¼å¯ç«ç¹è®¾ç½® |
-`{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `{}` | | `telegram` | `list` |
-Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | | `emby` | `list` | Emby
-è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------- | ------ | -------------- | ----
----------------- | | `checkiner` | `list` | å¯ç¨çç­¾å°ç«ç¹ |
-(å½åæææ¯æçç«ç¹) | | `monitor` | `list` | å¯ç¨ççè§ä¼è¯ |
-(å½åæææ¯æçä¼è¯) | | `messager` | `list` | å¯ç¨çæ°´ç¾¤ä¼è¯ |
-(å½åæææ¯æçä¼è¯) | æ³¨æ, å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯,
-è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡. è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
-æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
-è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
-æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
-ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | --- | --- | --- |--- | --- | |
-åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` | | å·æ¯é¼  IPTV |
-`jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby | `pornemby` | | Singularity
-| `singularity` | | Peach | `peach` | | Nebula | `nebula` | | Bluesea |
-`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | å¡æ | `charon` |
-`proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | -----
------ | ------ | --------------------------------------- | ----------- | |
-`hostname` | `str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
-ä»£çç«¯å£å· | `1080` | | `scheme` | `str` | ä»£çåè®®, å¯ä»¥ä¸º
-"`socks5`" æ "`http`" | `socks5` | `telegram` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
--------------------------------------------- | ------- | | `api_id` | `str` |
-ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID | | |
-`api_hash` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç
-Application Hash | | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
-| | | `monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send`
-| `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: |
-è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------
------------------------------------------------ | ------ | | `url` | `str` |
-Emby æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | |
-`username` | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
-æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
-`progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
-æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
-bgk, embyhub, polo unique_name = "your_username_for_registeration" #
-èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
-ä»å½é®é¢åå²ä¸­æ¾å°ç­æ¡æ¶èªå¨åç­ ``` ## ä»£ç éç¨ä¸å¼å
+embykeeper/raw/main/images/kitty.gif) ## ä»£ç éç¨ä¸å¼å
 ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-
 telegram telechecker) A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-
 robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message
 Messager] C --watcher--> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A
 ``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
 `embykeeper.telechecker.monitor` - `embykeeper.telechecker.messager`
 éå¸¸æ¥è¯´, å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
@@ -257,10 +258,19 @@
 å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from .base import AnswerBotCheckin
 class DummyCheckin(AnswerBotCheckin): .... async def on_captcha(self, message:
 Message, captcha: str): for l in captcha: try: await self.message.click(l)
 except ValueError: self.log.info(f'æªè½æ¾å°å¯¹åº "{l}" çæé®,
 æ­£å¨éè¯.') await self.retry() break ```
 ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
 å½æ¨å®ç°ä¸ä¸ªæ°çç­¾å°å¨æ¶, æ¬¢è¿æ¨æåº [Pull Requests](https://
-github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! ## è¶å¿ [!
-[Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
+github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! ##
+å¼åå·¥å· æ¨å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
+ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
+config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
+10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
+"åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
+è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
+ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
+å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
+è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ## è¶å¿
+[![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
 embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

### Comparing `embykeeper-2.1.1/README.md` & `embykeeper-2.2.0/embykeeper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: embykeeper
+Version: 2.2.0
+Summary: Daily checkin automator for emby bots in telegram.
+Author-email: jackzzs <jackzzs@outlook.com>
+Project-URL: Homepage, https://github.com/embykeeper/embykeeper
+Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: <3.11,>=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![build status](https://img.shields.io/github/actions/workflow/status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
 
 <p align="center">
   <a href='https://github.com/embykeeper/embykeeper'>
     <img src="https://github.com/embykeeper/embykeeper/raw/main/images/logo.svg" alt="Embykeeper" />
   </a>
 </p>
@@ -24,26 +44,26 @@
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
+  - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
   - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
   - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
-    - ~~卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)~~ (机器人逻辑频繁变动, 暂时禁用)
     - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
     - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
 
 - Emby 保活
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
 
@@ -58,31 +78,32 @@
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Misty 开注自动注册: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
   - 默认禁用:
     - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
-### 从 PyPi 安装
+### Railway 在线部署
 
-Embykeeper 可以通过 `python` 运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
+Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)
 
-```bash
-pip install embykeeper
-```
+请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
-随后, 您需要执行:
+### 通过 Docker 部署
+
+Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
-embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
+(若您不需要连接本机代理, 可以去除 '--net=host' 参数)
 
-命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
 
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = 1080
 scheme = "socks5"
 
@@ -98,132 +119,142 @@
 ```
 
 对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
 
 随后, 您需要再次执行:
 
 ```bash
-embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+恭喜您！您已经成功部署了 Embykeeper.
+
+当您需要更新版本时, 您需要执行:
 
 ```bash
-tmux
+docker pull embykeeper/embykeeper
 ```
 
-这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
+### 通过 Docker Compose 部署
 
-您随时可以通过运行:
+您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
 
-```bash
-tmux a
+**注意**: 您需要先进行过 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
+
+您需要新建一个文件 `docker-compose.yml`:
+
+```yaml
+version: '3'
+services:
+  embykeeper:
+    container_name: embykeeper
+    image: embykeeper/embykeeper
+    restart: unless-stopped
+    volumes:
+      - ./embykeeper:/app
+    network_mode: host
+  watchtower:
+    container_name: watchtower
+    image: containrrr/watchtower
+    restart: unless-stopped
+    volumes:
+      - /var/run/docker.sock:/var/run/docker.sock:rw
 ```
 
-以重新连接到 `tmux` 终端.
+其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新版本.
 
-当版本更新时, 您需要执行:
+然后运行以下命令以启动:
 
-```
-pip install -U embykeeper
+```bash
+docker-compose up -d
 ```
 
-然后重新运行应用.
+即可在后台启动 embykeeper.
 
-### 从源码构建
+您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
+
+### 从 PyPi 安装
 
-和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
+Embykeeper 可以通过 `python >= 3.7, < 3.11` 运行, 您可以通过 [virtualvenv](https://virtualenv.pypa.io/) 进行环境的管理:
 
 ```bash
-git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-pip install -e .
+python -m venv embykeeper-venv
+. ./embykeeper-venv/bin/activate
+pip install embykeeper
 ```
 
-然后即可执行 Embykeeper:
+随后, 您需要执行:
 
 ```bash
 embykeeper
 ```
 
-详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
+命令将会在当前目录生成模板 `config.toml` 文件, 您需要配置您的账户信息, 参见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 
-当版本更新时, 您需要执行:
+随后, 您需要再次执行:
 
+```bash
+embykeeper
 ```
-git pull
-```
-
-然后重新运行应用.
 
-### 从 Docker 部署
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
 
 ```bash
-docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
+tmux
 ```
 
-命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息 (详见[从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)).
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
 
-随后, 您需要再次执行:
+您随时可以通过运行:
 
 ```bash
-docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
+tmux a
 ```
 
-您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
-
-恭喜您！您已经成功部署了 Embykeeper.
+以重新连接到 `tmux` 终端.
 
-当您需要更新版本时, 您需要执行:
+当版本更新时, 您需要执行:
 
-```bash
-docker pull embykeeper/embykeeper
+```
+pip install -U embykeeper
 ```
 
-### 通过 Docker Compose 部署
-
-您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
+然后重新运行应用.
 
-**注意**: 您需要先进行过 [从 Docker 部署](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
+### 从源码构建
 
-您需要新建一个文件 `docker-compose.yml`:
+首先拉取并设置环境:
 
-```yaml
-version: '3'
-services:
-  embykeeper:
-    container_name: embykeeper
-    image: embykeeper/embykeeper
-    restart: unless-stopped
-    volumes:
-      - ./embykeeper:/app
-    network_mode: host
-  watchtower:
-    container_name: watchtower
-    image: containrrr/watchtower
-    restart: unless-stopped
-    volumes:
-      - /var/run/docker.sock:/var/run/docker.sock:rw
+```bash
+git clone https://github.com/embykeeper/embykeeper.git
+cd embykeeper
+python -m venv venv
+. ./venv/bin/activate
+pip install -e .
 ```
 
-其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新版本.
-
-然后运行以下命令以启动:
+然后即可执行 Embykeeper:
 
 ```bash
-docker-compose up -d
+embykeeper
 ```
 
-即可在后台启动 embykeeper.
+详细配置方法详见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 
-您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
+当版本更新时, 您需要执行:
+
+```
+git pull
+```
+
+然后重新运行应用.
 
 ## 命令行帮助
 
 您可以通过运行 `embykeeper -h` 以获取帮助:
 
 ```bash
 $ embykeeper -h
@@ -241,14 +272,15 @@
     --no-instant  -I   不立刻执行一次计划任务
     --once        -o   仅执行一次任务而不计划执行
     --debug       -d   开启调试输出, 错误将会导致程序停止运行
     --version     -v   打印 Embykeeper 版本
     --follow      -f   仅启动消息调试
     --analyze     -a   仅启动历史信息分析
     --basedir          设定输出文件默认位置
+    --public           启用在线部署模式
 ```
 
 例如:
 
 ```bash
 # 启动所有功能 (在各账号配置中进一步设置功能开启/关闭)
 $ embykeeper config.toml
@@ -268,62 +300,20 @@
 # 启动所有功能, 只运行一次
 $ embykeeper config.toml --once
 
 # 启动所有功能, 不立即执行一次签到/保活
 $ embykeeper config.toml -I
 ```
 
-您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
-
-```bash
-# 启动历史信息分析
-$ embykeeper config.toml -a
-
-请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
-请输入关键词 (以空格分隔):
-输入时间范围 (以"-"分割): 8:00AM-10:00AM
-请输入各群组最大获取数量 [1000]:
-```
-
-该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
-
-另一个工具是即时信息分析:
-
-![follow screenshot](images/follow.svg)
-
-该工具可以实时输出消息的 ID 等信息, 以方便调试.
-
-## 消息推送与高级用户
-
-您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
-
-本项目涉及的需要 Cloudflare 验证码付费跳过的操作 (例如 Nebula 签到)、可能会引起竞争的操作 (例如自动抢邀请码)将需要高级用户, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
-
-目前有三种方式成为高级用户:
-
-1. 分享 1 个邀请制 Emby 的邀请码;
-2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
-3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
-
-## 支持 Embykeeper
-
-##### 开发者团队
-
-- [jackzzs](https://github.com/jackzzs)
-
-##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
-
-![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
-
 ## 配置项
 
 | 设置项       | 值类型             | 简介                                         | 默认值  |
 | ------------ | ------------------ | -------------------------------------------- | ------- |
 | `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`    |
+| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`     |
 | `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
 | `random`     | `int`              | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
 | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
 | `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
 | `proxy`      | `dict`             | 代理设置                                     | `{}`    |
 | `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
 | `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
@@ -336,22 +326,22 @@
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
 若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
 若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
 当前支持的名称包括:
-| 站点 | 名称 | | 站点 | 名称 |
-| --- | --- | --- |--- | --- |
-| 垃圾影音 | `ljyy` | | 搜书神器 | `sosdbot` |
-| 卷毛鼠 IPTV | `jms_iptv` | | 终点站 | `terminus` |
-| Pornemby | `pornemby` | | Singularity | `singularity` |
-| Peach | `peach` | | Nebula | `nebula` |
-| Bluesea | `bluesea` | | Embyhub | `embyhub` |
-| 卷毛鼠 | `jms` | | 卡戎 | `charon` |
+| 站点        | 名称       |     | 站点        | 名称          |
+| ----------- | ---------- | --- | ----------- | ------------- |
+| 垃圾影音    | `ljyy`     |     | 搜书神器    | `sosdbot`     |
+| 卷毛鼠 IPTV | `jms_iptv` |     | 终点站      | `terminus`    |
+| Pornemby    | `pornemby` |     | Singularity | `singularity` |
+| Peach       | `peach`    |     | Nebula      | `nebula`      |
+| Bluesea     | `bluesea`  |     | Embyhub     | `embyhub`     |
+| 卷毛鼠      | `jms`      |     | 卡戎        | `charon`      |
 
 `proxy` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                    | 默认值      |
 | ---------- | ------ | --------------------------------------- | ----------- |
 | `hostname` | `str`  | 代理服务器地址                          | `localhost` |
 | `port`     | `int`  | 代理端口号                              | `1080`      |
@@ -384,14 +374,36 @@
 [monitor.bgk] # 支持 bgk, embyhub, polo
 unique_name = "your_username_for_registeration" # 自动抢注时使用的用户名
 
 [monitor.pornemby]
 only_history = true # 仅当问题历史中找到答案时自动回答
 ```
 
+## 消息推送与高级用户
+
+您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
+
+本项目涉及的需要 Cloudflare 验证码付费跳过的操作 (例如 Nebula 签到)、可能会引起竞争的操作 (例如自动抢邀请码)将需要高级用户, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
+
+目前有三种方式成为高级用户:
+
+1. 分享 1 个邀请制 Emby 的邀请码;
+2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
+3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
+
+## 支持 Embykeeper
+
+##### 开发者团队
+
+- [jackzzs](https://github.com/jackzzs)
+
+##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
+
+![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
+
 ## 代码重用与开发
 
 代码架构如下:
 
 ```mermaid
 flowchart TD
     A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
@@ -439,10 +451,32 @@
                 break
 ```
 
 上述代码实现每次按对应一个字符按键的功能.
 
 当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
 
+## 开发工具
+
+您可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
+
+```bash
+# 启动历史信息分析
+$ embykeeper config.toml -a
+
+请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
+请输入关键词 (以空格分隔):
+输入时间范围 (以"-"分割): 8:00AM-10:00AM
+请输入各群组最大获取数量 [1000]:
+```
+
+该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
+
+另一个工具是即时信息分析:
+
+![follow screenshot](images/follow.svg)
+
+该工具可以实时输出消息的 ID 等信息, 以方便调试.
+
 ## 趋势
 
 [![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

#### html2text {}

```diff
@@ -1,12 +1,23 @@
-[![build status](https://img.shields.io/github/actions/workflow/status/
-embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/
-embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/
-embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://
-img.shields.io/pypi/dm/
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.0 Summary: Daily checkin
+automator for emby bots in telegram. Author-email: jackzzs
+outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
+Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
+Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
+:: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
+Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-
+File: LICENSE [![build status](https://img.shields.io/github/actions/workflow/
+status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/
+embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/
+v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https:
+//img.shields.io/pypi/dm/
 embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
 embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
 embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
 embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
 [telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
 embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
@@ -34,39 +45,38 @@
 å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
 Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
 å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
 åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
-æºå¨äººç­¾å° - ç»ç¹ç«: [é¢é](https://t.me/embypub) [ç¾¤ç»](https://
-t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) - Nebula: [é¢é]
-(https://t.me/Nebula_Emby) [ç¾¤ç»](https://t.me/NebulaEmbyUser) [æºå¨äºº]
-(https://t.me/Nebula_Account_bot) (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare
-éªè¯ç , éè¦[é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) -
-Singularity: [é¢é](https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://
-t.me/Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) -
-Peach: [é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
-peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
-(https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
-t.me/EdHubot) - Pornemby: [é¢é](https://t.me/pornembyservice) [ç¾¤ç»]
-(https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
-åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
-t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
-t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
-ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
-pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
-~~å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https://t.me/
-Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot)~~
-(æºå¨äººé»è¾é¢ç¹åå¨, ææ¶ç¦ç¨) - ~~BlueSea: [ç¾¤ç»](https://t.me/
-blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~ (æ ååº) -
-~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/
-Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) - Emby
-ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
-Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+æºå¨äººç­¾å° - å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https:/
+/t.me/Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot) - ç»ç¹ç«: [é¢é]
+(https://t.me/embypub) [ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://
+t.me/EmbyPublicBot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
+(https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
+(ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
+t.me/embykeeper_bot?start=__prime)) - Singularity: [é¢é](https://t.me/
+Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/Singularity_Emby_Group)
+[æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach: [é¢é](https://t.me/
+peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
+t.me/peach_emby_bot) - EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https:/
+/t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Pornemby: [é¢é](https://
+t.me/pornembyservice) [ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/
+PronembyTGBot2_bot) - åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1)
+[æºå¨äºº](https://t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV)
+[ç¾¤ç»](https://t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) -
+å¶ä»é Emby ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/
+embykeeper/pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
+~~BlueSea: [ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/
+blueseamusic_bot)~~ (æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/
+CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://
+t.me/JMSIPTV_bot)~~ (æ ååº) - Emby ä¿æ´» -
+å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
+èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
 t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
 Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
 embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
 t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
 [é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime),
 åç­åç¡®çä¸è¬è¯·è°¨æä½¿ç¨) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»](https:
@@ -74,166 +84,168 @@
 æ¢éè¯·ç : [é¢é](https://t.me/viper_emby_channel) [ç¾¤ç»](https://t.me/
 Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
 å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
-(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### ä»
-PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡, æ¨å¯ä»¥éè¿ [conda]
-(https://github.com/conda/conda) æ [virtualvenv](https://virtualenv.pypa.io/
-) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip` å®è£ `embykeeper`
-(éè¦ `python >= 3.7, < 3.11`): ```bash pip install embykeeper ``` éå,
-æ¨éè¦æ§è¡: ```bash embykeeper ``` å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿
-`config.toml` æä»¶, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
-(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [proxy] hostname =
-"127.0.0.1" port = 1080 scheme = "socks5" [[telegram]] api_id = "27894236"
-api_hash = "622159182fdd4b15b627eeb3ac695271" phone = "+8612109347899" [[emby]]
-url = "https://weiss-griffin.com/" username = "carrie19" password =
-"s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿ [Telegram å®ç½]
-(https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
-development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
-æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
-æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
-æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡:
-```bash embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
-ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
-ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
-``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
-æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
-Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
-æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º åä» PyPi
-å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python ç¯å¢, ç¶åæå Github
-å¹¶å®è£: ```bash git clone https://github.com/embykeeper/embykeeper.git cd
-embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash
-embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/
-embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
-æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ### ä» Docker
-é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://
-yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡: ```bash docker run -
-v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
-å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯ (è¯¦è§[ä» Pypi å®è£](https://github.com/
-embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)). éå,
-æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
-net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
-ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### Railway
+å¨çº¿é¨ç½² Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
+(https://railway.app/button.svg)](https://railway.app/template/
+WFYaj9?referralCode=Fj6Yvy) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
+ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
+é¨ç½². ### éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½²,
+æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
+ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
+embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
+net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
+`config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
+æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
+```toml [proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [
+[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
+[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
+ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
+è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
+"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
+æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --
+rm -it --net=host embykeeper/embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
-compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker
-é¨ç½²](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-
+compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
+é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
 %E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
 è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
 ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
 compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
 version: '3' services: embykeeper: container_name: embykeeper image:
 embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
 docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
 watchtower) è¢«ç¨äºèªå¨æ´æ°çæ¬. ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨:
 ```bash docker-compose up -d ``` å³å¯å¨åå°å¯å¨ embykeeper.
 æ¨å¯ä»¥éè¿ `docker logs -f embykeeper` æ `docker-compose logs -
-f embykeeper` ä»¥æ¥çææ°æ¥å¿. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡
-`embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨
-Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
-(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
-(ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
-e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+f embykeeper` ä»¥æ¥çææ°æ¥å¿. ### ä» PyPi å®è£ Embykeeper
+å¯ä»¥éè¿ `python >= 3.7, < 3.11` è¿è¡, æ¨å¯ä»¥éè¿ [virtualvenv]
+(https://virtualenv.pypa.io/) è¿è¡ç¯å¢çç®¡ç: ```bash python -m venv
+embykeeper-venv . ./embykeeper-venv/bin/activate pip install embykeeper ```
+éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, åè§ [éè¿ Docker é¨ç½²](https://
+github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
+Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
+æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
+ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæåå¹¶è®¾ç½®ç¯å¢:
+```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
+python -m venv venv . ./venv/bin/activate pip install -e . ```
+ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§
+[éè¿ Docker é¨ç½²](https://github.com/embykeeper/
+embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2). å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
+æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
+h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
+config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
+c å¯ç¨æ¯æ¥ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --
+emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ --
-basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® ``` ä¾å¦: ```bash # å¯å¨ææåè½
+basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® --public å¯ç¨å¨çº¿é¨ç½²æ¨¡å¼ ```
+ä¾å¦: ```bash # å¯å¨ææåè½
 (å¨åè´¦å·éç½®ä¸­è¿ä¸æ­¥è®¾ç½®åè½å¼å¯/å³é­) $ embykeeper
 config.toml # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 ä»å¯å¨æ¯æ¥ 8:00 PM - 9:00 PM éæºæ¶é´ç­¾å° $ embykeeper config.toml -
 c <8:00PM,9:00PM> # å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -s #
 å¯å¨ææåè½, åªè¿è¡ä¸æ¬¡ $ embykeeper config.toml --once #
 å¯å¨ææåè½, ä¸ç«å³æ§è¡ä¸æ¬¡ç­¾å°/ä¿æ´» $ embykeeper config.toml
--I ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
-ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
-config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
-10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
-"åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
-è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
-ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
-å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
-è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ##
+-I ``` ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------
+-- | ------------------ | -------------------------------------------- | ------
+- | | `timeout` | `int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | |
+`retries` | `int` | Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | |
+`concurrent` | `int` | Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random`
+| `int` | Telegram æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` |
+| `notifier` | `int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/
+ææºå·) | `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/
+çè§åè½å¼å¯ç«ç¹è®¾ç½® | `{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `
+{}` | | `telegram` | `list` | Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
+| `emby` | `list` | Emby è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
+`service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----
+------- | ------ | -------------- | -------------------- | | `checkiner` |
+`list` | å¯ç¨çç­¾å°ç«ç¹ | (å½åæææ¯æçç«ç¹) | | `monitor` |
+`list` | å¯ç¨ççè§ä¼è¯ | (å½åæææ¯æçä¼è¯) | | `messager` |
+`list` | å¯ç¨çæ°´ç¾¤ä¼è¯ | (å½åæææ¯æçä¼è¯) | æ³¨æ,
+å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯, è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡.
+è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
+è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
+ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | ----------- | ---------- | --- | ------
+----- | ------------- | | åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` |
+| å·æ¯é¼  IPTV | `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby |
+`pornemby` | | Singularity | `singularity` | | Peach | `peach` | | Nebula |
+`nebula` | | Bluesea | `bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms`
+| | å¡æ | `charon` | `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å |
+ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------------------
+----- | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
+`localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` | `str`
+| ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
+è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
+------ | ------------------------------------------------------------------ | -
+------ | | `api_id` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/
+)ç³è¯·ç Application ID | | | `api_hash` | `str` | ä»[Telegram å®ç½]
+(https://my.telegram.org/)ç³è¯·ç Application Hash | | | `phone` | `str` |
+è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | | `monitor` | `bool` |
+å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` | `bool` |
+å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹
+| å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | --------------------
+------------------------------------- | ------ | | `url` | `str` | Emby
+æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
+| `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
+æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
+`progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
+æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
+bgk, embyhub, polo unique_name = "your_username_for_registeration" #
+èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
+ä»å½é®é¢åå²ä¸­æ¾å°ç­æ¡æ¶èªå¨åç­ ``` ##
 æ¶æ¯æ¨éä¸é«çº§ç¨æ· æ¨å¯ä»¥éè¿è®¾ç½®é¡¹ "`notifier`" è®¾ç½®
 æå/å¤±è´¥ éç¥å°è¢«åéç Telegram è´¦å·, æ¨å¯ä»¥éè¿
 [Embykeeper Bot](https://t.me/embykeeper_bot)
 è®¾ç½®æ¶æ¯æ¯æ¥åéçæ¶é´. æ¬é¡¹ç®æ¶åçéè¦ Cloudflare
 éªè¯ç ä»è´¹è·³è¿çæä½ (ä¾å¦ Nebula
 ç­¾å°)ãå¯è½ä¼å¼èµ·ç«äºçæä½
 (ä¾å¦èªå¨æ¢éè¯·ç )å°éè¦é«çº§ç¨æ·, æ¨å¯ä»¥éè¿ [Embykeeper
 Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
 (https://afdian.net/a/jackzzs)èµå© ![Kitty](https://github.com/embykeeper/
-embykeeper/raw/main/images/kitty.gif) ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å |
-ç®ä» | é»è®¤å¼ | | ------------ | ------------------ | --------------------
------------------------- | ------- | | `timeout` | `int` | Telegram
-æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | | `retries` | `int` | Telegram
-æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | | `concurrent` | `int` | Telegram
-æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random` | `int` | Telegram
-æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` | | `notifier` |
-`int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/ææºå·) |
-`False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/çè§åè½å¼å¯ç«ç¹è®¾ç½® |
-`{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `{}` | | `telegram` | `list` |
-Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | | `emby` | `list` | Emby
-è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------- | ------ | -------------- | ----
----------------- | | `checkiner` | `list` | å¯ç¨çç­¾å°ç«ç¹ |
-(å½åæææ¯æçç«ç¹) | | `monitor` | `list` | å¯ç¨ççè§ä¼è¯ |
-(å½åæææ¯æçä¼è¯) | | `messager` | `list` | å¯ç¨çæ°´ç¾¤ä¼è¯ |
-(å½åæææ¯æçä¼è¯) | æ³¨æ, å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯,
-è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡. è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
-æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
-è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
-æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
-ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | --- | --- | --- |--- | --- | |
-åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` | | å·æ¯é¼  IPTV |
-`jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby | `pornemby` | | Singularity
-| `singularity` | | Peach | `peach` | | Nebula | `nebula` | | Bluesea |
-`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | å¡æ | `charon` |
-`proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | -----
------ | ------ | --------------------------------------- | ----------- | |
-`hostname` | `str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
-ä»£çç«¯å£å· | `1080` | | `scheme` | `str` | ä»£çåè®®, å¯ä»¥ä¸º
-"`socks5`" æ "`http`" | `socks5` | `telegram` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
--------------------------------------------- | ------- | | `api_id` | `str` |
-ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID | | |
-`api_hash` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç
-Application Hash | | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
-| | | `monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send`
-| `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: |
-è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------
------------------------------------------------ | ------ | | `url` | `str` |
-Emby æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | |
-`username` | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
-æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
-`progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
-æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
-bgk, embyhub, polo unique_name = "your_username_for_registeration" #
-èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
-ä»å½é®é¢åå²ä¸­æ¾å°ç­æ¡æ¶èªå¨åç­ ``` ## ä»£ç éç¨ä¸å¼å
+embykeeper/raw/main/images/kitty.gif) ## ä»£ç éç¨ä¸å¼å
 ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-
 telegram telechecker) A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-
 robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message
 Messager] C --watcher--> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A
 ``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
 `embykeeper.telechecker.monitor` - `embykeeper.telechecker.messager`
 éå¸¸æ¥è¯´, å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
@@ -246,10 +258,19 @@
 å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from .base import AnswerBotCheckin
 class DummyCheckin(AnswerBotCheckin): .... async def on_captcha(self, message:
 Message, captcha: str): for l in captcha: try: await self.message.click(l)
 except ValueError: self.log.info(f'æªè½æ¾å°å¯¹åº "{l}" çæé®,
 æ­£å¨éè¯.') await self.retry() break ```
 ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
 å½æ¨å®ç°ä¸ä¸ªæ°çç­¾å°å¨æ¶, æ¬¢è¿æ¨æåº [Pull Requests](https://
-github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! ## è¶å¿ [!
-[Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
+github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! ##
+å¼åå·¥å· æ¨å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
+ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
+config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
+10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
+"åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
+è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
+ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
+å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
+è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ## è¶å¿
+[![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
 embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

### Comparing `embykeeper-2.1.1/embykeeper/cli.py` & `embykeeper-2.2.0/embykeeper/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 @app.async_command(
     cls=FlagValueCommand, help=f"欢迎使用 [orange3]{__name__.capitalize()}[/] {__version__} :cinema: 无参数默认开启全部功能."
 )
 async def main(
     config: Path = typer.Argument(
         None,
-        envvar=f"{__name__.upper()}_CONFIG",
         dir_okay=False,
         allow_dash=True,
         rich_help_panel="参数",
         help="配置文件 (置空以生成)",
     ),
     checkin: str = typer.Option(
         Flagged("", "<10:00AM,9:00PM>"),
@@ -93,15 +92,16 @@
 
     if not checkin and not monitor and not emby and not send:
         checkin = "<5:00PM,8:00PM>"
         emby = 7
         monitor = True
         send = True
 
-    logger.info(f"欢迎使用 [orange3]{__name__.capitalize()}[/]! 正在启动, 请稍等. 您可以通过 Ctrl+C 以结束运行.")
+    msg = " 您可以通过 Ctrl+C 以结束运行." if not public else ""
+    logger.info(f"欢迎使用 [orange3]{__name__.capitalize()}[/]! 正在启动, 请稍等.{msg}")
     logger.info(f'当前版本 ({__version__}) 活跃贡献者: {", ".join(__author__)}.')
     logger.debug(f'命令行参数: "{" ".join(sys.argv[1:])}".')
 
     basedir = Path(basedir or user_data_dir(__name__))
     basedir.mkdir(parents=True, exist_ok=True)
     config["basedir"] = basedir
     try:
```

### Comparing `embykeeper-2.1.1/embykeeper/data.py` & `embykeeper-2.2.0/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/embywatcher/emby.py` & `embykeeper-2.2.0/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/embywatcher/main.py` & `embykeeper-2.2.0/embykeeper/embywatcher/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/log.py` & `embykeeper-2.2.0/embykeeper/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 
 def initialize(level="INFO"):
     logger.remove()
     handler = RichHandler(
         console=Console(stderr=True), markup=True, rich_tracebacks=True, tracebacks_suppress=[asyncio]
     )
     handler.setFormatter(Formatter(None, "[%m/%d %H:%M]"))
-    logger.add(handler, format=formatter, level=level, colorize=False, enqueue=True)
+    logger.add(handler, format=formatter, level=level, colorize=False)
```

### Comparing `embykeeper-2.1.1/embykeeper/settings.py` & `embykeeper-2.2.0/embykeeper/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     from tomlkit import item
     from rich import get_console
     from rich.prompt import Prompt, IntPrompt, Confirm
 
     from . import __name__, __url__
 
     pad = " " * 23
-    logger.info("我们将为您生成配置, 需要您根据提示填入信息, 并按回车确认, 您可以随时通过 Ctrl+C 结束运行.")
+    logger.info("我们将为您生成配置, 需要您根据提示填入信息, 并按回车确认.")
     logger.info(f"配置帮助详见: {__url__}.")
     telegrams = config.get("telegram", [])
     while True:
         if len(telegrams) > 0:
             logger.info(
                 f'您当前填写了 {len(telegrams)} 个 Telegram 账号信息: {", ".join([t["phone"] for t in telegrams])}'
             )
@@ -275,26 +275,29 @@
         config["concurrent"] = IntPrompt.ask(
             pad + "设置最大可同时进行的 Telegram Bot 签到", default=config["concurrent"], show_default=True
         )
         config["random"] = IntPrompt.ask(
             pad + "设置计划任务时, 各站点之间签到的随机时间差异 (分钟)", default=config["random"], show_default=True
         )
     content = item(config).as_string()
-    enc = Confirm.ask(pad + "是否生成加密配置 ([red]为了您的密钥安全, 强烈建议生成[/])", default=True)
+    enc = Confirm.ask(pad + "是否生成加密配置", default=False)
     if enc:
         enc_password = Prompt.ask(pad + "请输入加密密码, 程序启动时将要求输入 (不显示, 按回车确认)", password=True)
         content = encrypt(content, enc_password)
     else:
         content = content.encode()
     content = base64.b64encode(content)
-    logger.info(f"您的配置[green]已生成完毕[/]! 您需要将以下内容写入 SECRETS 变量配置 (名称: {__name__.upper()}_CONFIG)")
+    logger.info(f"您的配置[green]已生成完毕[/]! 您需要将以下内容写入 SECRETS 变量配置 (名称: EK_CONFIG), 否则配置将在重启后丢失.")
     print()
-    get_console().rule("EMBYKEEPER_CONFIG")
+    get_console().rule("EK_CONFIG")
     print(content.decode())
-    print("\n\n")
+    get_console().rule()
+    start_now = Confirm.ask(pad + "是否立即启动?", default=True)
+    if start_now:
+        return config
 
 
 def load_env_config(data: str):
     from rich.prompt import Prompt
 
     data = base64.b64decode(data.strip().encode())
     try:
@@ -312,57 +315,57 @@
             sys.exit(252)
     else:
         logger.debug("您正在使用 SECRETS 变量配置.")
     return config
 
 
 def prepare_config(config_file=None, public=False):
-    from . import __name__
-
-    env_config = os.environ.get(f"{__name__.upper()}_CONFIG", None)
+    env_config = os.environ.get(f"EK_CONFIG", None)
     if env_config:
         config = load_env_config(env_config)
     else:
         if public:
-            logger.warning("您正在使用公共仓库, 因此[red]请勿[/]将密钥存储于[red]任何配置文件[/].")
+            # logger.warning("您正在使用公共仓库, 因此[red]请勿[/]将密钥存储于[red]任何配置文件[/].")
             config = {}
             if config_file:
                 try:
                     with open(config_file, "rb") as f:
                         config = tomllib.load(f)
                 except tomllib.TOMLDecodeError as e:
                     logger.error(f"TOML 配置文件错误: {e}.")
                     sys.exit(252)
                 else:
                     logger.info(f"将以 {Path(config_file).name} 为基础生成配置.")
-            interactive_config(config)
-            sys.exit(0)
-        default_config_file = Path("config.toml")
-        if not config_file:
-            if not default_config_file.exists():
-                write_faked_config(default_config_file)
+            config = interactive_config(config)
+            if not config:
                 sys.exit(250)
-            else:
-                config_file = default_config_file
-        try:
-            if not Path(config_file).exists():
-                logger.error(f'配置文件 "{config_file}" 不存在.')
-                sys.exit(251)
-            elif config_file == default_config_file:
-                with open(config_file, "rb") as f:
-                    config = tomllib.load(f)
-                if not config:
-                    write_faked_config(config_file)
+        else:
+            default_config_file = Path("config.toml")
+            if not config_file:
+                if not default_config_file.exists():
+                    write_faked_config(default_config_file)
                     sys.exit(250)
-            else:
-                with open(config_file, "rb") as f:
-                    config = tomllib.load(f)
-        except tomllib.TOMLDecodeError as e:
-            logger.error(f"TOML 配置文件错误: {e}.")
-            sys.exit(252)
+                else:
+                    config_file = default_config_file
+            try:
+                if not Path(config_file).exists():
+                    logger.error(f'配置文件 "{config_file}" 不存在.')
+                    sys.exit(251)
+                elif config_file == default_config_file:
+                    with open(config_file, "rb") as f:
+                        config = tomllib.load(f)
+                    if not config:
+                        write_faked_config(config_file)
+                        sys.exit(250)
+                else:
+                    with open(config_file, "rb") as f:
+                        config = tomllib.load(f)
+            except tomllib.TOMLDecodeError as e:
+                logger.error(f"TOML 配置文件错误: {e}.")
+                sys.exit(252)
     error = check_config(config)
     if error:
         logger.error(f"配置文件错误, 请检查配置文件:\n{error}.")
         sys.exit(253)
     proxy: dict = config.get("proxy", None)
     if proxy:
         proxy.setdefault("scheme", "socks5")
```

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/bots/base.py` & `embykeeper-2.2.0/embykeeper/telechecker/bots/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.2.0/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.2.0/embykeeper/telechecker/bots/jms.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 import random
 from pyrogram.types import Message
 from thefuzz import process, fuzz
 
 from ...data import get_data
 from .base import AnswerBotCheckin
 
-__ignore__ = True
-
 
 class JMSCheckin(AnswerBotCheckin):
-    ocr = "idioms@v1"
+    ocr = "idioms@v2"
     idioms = None
 
     name = "卷毛鼠"
     bot_username = "jmsembybot"
 
     async def start(self):
         self.retries = 2
@@ -36,14 +34,15 @@
         return result
 
     async def on_captcha(self, message: Message, captcha: str):
         captcha = self.to_idiom(captcha)
         async with self.operable:
             if not self.message:
                 await self.operable.wait()
+            await asyncio.sleep(random.randint(300, 500) / 100)
             for l in captcha:
                 try:
                     await self.message.click(l)
                     await asyncio.sleep(random.randint(50, 300) / 100)
                 except ValueError:
                     self.log.info(f'未能找到对应 "{l}" 的按键, 正在重试.')
                     await self.retry()
```

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.2.0/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.2.0/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.2.0/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.2.0/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/link.py` & `embykeeper-2.2.0/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/log.py` & `embykeeper-2.2.0/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/main.py` & `embykeeper-2.2.0/embykeeper/telechecker/main.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/messager/base.py` & `embykeeper-2.2.0/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/messager/common.py` & `embykeeper-2.2.0/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.2.0/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.2.0/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.2.0/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.2.0/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.2.0/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.2.0/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.2.0/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.2.0/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/telechecker/tele.py` & `embykeeper-2.2.0/embykeeper/telechecker/tele.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper/utils.py` & `embykeeper-2.2.0/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.1.1/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: embykeeper
-Version: 2.1.1
-Summary: Daily checkin automator for emby bots in telegram.
-Author-email: jackzzs <jackzzs@outlook.com>
-Project-URL: Homepage, https://github.com/embykeeper/embykeeper
-Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: <3.11,>=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![build status](https://img.shields.io/github/actions/workflow/status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://img.shields.io/pypi/dm/embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [![telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-channel-green)](https://t.me/embykeeper)
 
 <p align="center">
   <a href='https://github.com/embykeeper/embykeeper'>
     <img src="https://github.com/embykeeper/embykeeper/raw/main/images/logo.svg" alt="Embykeeper" />
   </a>
 </p>
@@ -44,26 +24,26 @@
 当您使用 "消息提示" 功能, 该工具时候将自动向 "[Embykeeper Auth Bot](https://t.me/embykeeper_auth_bot)" 发送关键的成功/失败日志以供从 "[Embykeeper Bot](https://t.me/embykeeper_bot)" 向您推送, 日志内容不含任何密码或密钥信息, 您认可该命令不会给您带来隐私与安全问题.
 
 当您安装并使用该工具, 默认您已经阅读并同意上述声明, 并确认自己并非出于"集邮"目的而安装.
 
 ## 功能
 
 - Telegram 机器人签到
+  - 卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)
   - 终点站: [频道](https://t.me/embypub) [群组](https://t.me/EmbyPublic) [机器人](https://t.me/EmbyPublicBot)
   - Nebula: [频道](https://t.me/Nebula_Emby) [群组](https://t.me/NebulaEmbyUser) [机器人](https://t.me/Nebula_Account_bot) (由于需要付费跳过 Cloudflare 验证码, 需要[高级用户](https://t.me/embykeeper_bot?start=__prime))
   - Singularity: [频道](https://t.me/Singularity_Emby_Channel) [群组](https://t.me/Singularity_Emby_Group) [机器人](https://t.me/Singularity_Emby_Bot)
   - Peach: [频道](https://t.me/peach_emby_channel) [群组](https://t.me/peach_emby_chat) [机器人](https://t.me/peach_emby_bot)
   - EmbyHub: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Pornemby: [频道](https://t.me/pornembyservice) [群组](https://t.me/Pornemby) [机器人](https://t.me/PronembyTGBot2_bot)
   - 垃圾影音: [群组](https://t.me/+3sP2A-fgeXg0ZmY1) [机器人](https://t.me/zckllflbot)
   - 卡戎: [频道](https://t.me/CharonTV) [群组](https://t.me/CharonTV_Talk) [机器人](https://t.me/CharonTV_Bot)
   - 其他非 Emby 相关:
     - 搜书神器 ([@chneez](https://github.com/embykeeper/embykeeper/pull/8) 增加): [机器人](https://t.me/sosdbot)
   - 默认禁用:
-    - ~~卷毛鼠: [频道](https://t.me/CurlyMouse) [群组](https://t.me/Curly_Mouse) [机器人](https://t.me/jmsembybot)~~ (机器人逻辑频繁变动, 暂时禁用)
     - ~~BlueSea: [群组](https://t.me/blueseachat) [机器人](https://t.me/blueseamusic_bot)~~ (无响应)
     - ~~卷毛鼠 IPTV: [频道](https://t.me/CurlyMouseIPTV) [群组](https://t.me/Curly_MouseIPTV) [机器人](https://t.me/JMSIPTV_bot)~~ (无响应)
 
 - Emby 保活
   - 定时模拟账号登录视频播放
   - 播放时间与进度模拟
 
@@ -78,31 +58,32 @@
   - Embyhub 开注自动注册: [频道](https://t.me/embyhub) [群组](https://t.me/emby_hub) [机器人](https://t.me/EdHubot)
   - Misty 开注自动注册: [频道](https://t.me/FreeEmbyChannel) [群组](https://t.me/FreeEmby) [机器人](https://t.me/EmbyMistyBot)
   - 默认禁用:
     - ~~Polo 抢邀请码: [频道](https://t.me/poloembyc) [群组](https://t.me/poloemby) [机器人](https://t.me/polo_emby_bot)~~ (公益服关闭)
 
 ## 安装与使用
 
-### 从 PyPi 安装
+### Railway 在线部署
 
-Embykeeper 可以通过 `python` 运行, 您可以通过 [conda](https://github.com/conda/conda) 或 [virtualvenv](https://virtualenv.pypa.io/) 等工具进行环境的管理.
+Embykeeper 可以通过免费的 Railway Docker 托管平台进行部署, 点击下方按钮开始部署:
 
-您可以通过 `pip` 安装 `embykeeper` (需要 `python >= 3.7, < 3.11`):
+[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/WFYaj9?referralCode=Fj6Yvy)
 
-```bash
-pip install embykeeper
-```
+请注意 Railway 的免费用量有每月 5 美元, 500 小时 (21 天) 的限制. 如有额外需要请通过 Docker 部署.
 
-随后, 您需要执行:
+### 通过 Docker 部署
+
+Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
 
 ```bash
-embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
+(若您不需要连接本机代理, 可以去除 '--net=host' 参数)
 
-命令将会在当前目录生成模板 `config.toml` 文件, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
+命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息, 您也可以使用最小配置 (以下敏感信息为生成, 仅做参考):
 
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = 1080
 scheme = "socks5"
 
@@ -118,132 +99,142 @@
 ```
 
 对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
 
 随后, 您需要再次执行:
 
 ```bash
-embykeeper
+docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
+恭喜您！您已经成功部署了 Embykeeper.
+
+当您需要更新版本时, 您需要执行:
 
 ```bash
-tmux
+docker pull embykeeper/embykeeper
 ```
 
-这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
+### 通过 Docker Compose 部署
 
-您随时可以通过运行:
+您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
 
-```bash
-tmux a
+**注意**: 您需要先进行过 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
+
+您需要新建一个文件 `docker-compose.yml`:
+
+```yaml
+version: '3'
+services:
+  embykeeper:
+    container_name: embykeeper
+    image: embykeeper/embykeeper
+    restart: unless-stopped
+    volumes:
+      - ./embykeeper:/app
+    network_mode: host
+  watchtower:
+    container_name: watchtower
+    image: containrrr/watchtower
+    restart: unless-stopped
+    volumes:
+      - /var/run/docker.sock:/var/run/docker.sock:rw
 ```
 
-以重新连接到 `tmux` 终端.
+其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新版本.
 
-当版本更新时, 您需要执行:
+然后运行以下命令以启动:
 
-```
-pip install -U embykeeper
+```bash
+docker-compose up -d
 ```
 
-然后重新运行应用.
+即可在后台启动 embykeeper.
 
-### 从源码构建
+您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
+
+### 从 PyPi 安装
 
-和从 PyPi 安装类似，您需要一个先设置 Python 环境, 然后拉取 Github 并安装:
+Embykeeper 可以通过 `python >= 3.7, < 3.11` 运行, 您可以通过 [virtualvenv](https://virtualenv.pypa.io/) 进行环境的管理:
 
 ```bash
-git clone https://github.com/embykeeper/embykeeper.git
-cd embykeeper
-pip install -e .
+python -m venv embykeeper-venv
+. ./embykeeper-venv/bin/activate
+pip install embykeeper
 ```
 
-然后即可执行 Embykeeper:
+随后, 您需要执行:
 
 ```bash
 embykeeper
 ```
 
-详细配置方法详见 [从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85).
+命令将会在当前目录生成模板 `config.toml` 文件, 您需要配置您的账户信息, 参见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 
-当版本更新时, 您需要执行:
+随后, 您需要再次执行:
 
+```bash
+embykeeper
 ```
-git pull
-```
-
-然后重新运行应用.
 
-### 从 Docker 部署
+您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
 
-Embykeeper 可以通过 `docker` 部署, 您需 [安装 docker](https://yeasy.gitbook.io/docker_practice/install), 然后执行:
+恭喜您！您已经成功部署了 Embykeeper, 为了让 Embykeeper 长期后台运行, 您可以通过`Ctrl+C`停止, 然后运行:
 
 ```bash
-docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
+tmux
 ```
 
-命令将会在 `embykeeper` 目录下生成模板 `config.toml` 文件, 您需要配置您的账户信息 (详见[从 Pypi 安装](https://github.com/embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)).
+这将启动一个 `tmux` 终端, 您可以在该终端中运行上述命令 (`embykeeper config.toml`), 并按 Ctrl + B, 松开 B 再按 D, 以脱离 `tmux` 终端.
 
-随后, 您需要再次执行:
+您随时可以通过运行:
 
 ```bash
-docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
+tmux a
 ```
 
-您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
-
-恭喜您！您已经成功部署了 Embykeeper.
+以重新连接到 `tmux` 终端.
 
-当您需要更新版本时, 您需要执行:
+当版本更新时, 您需要执行:
 
-```bash
-docker pull embykeeper/embykeeper
+```
+pip install -U embykeeper
 ```
 
-### 通过 Docker Compose 部署
-
-您可以使用 [docker-compose](https://docs.docker.com/compose/) 部署 Embykeeper.
+然后重新运行应用.
 
-**注意**: 您需要先进行过 [从 Docker 部署](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-%E9%83%A8%E7%BD%B2) 才能通过 `docker-compose` 部署, 这是由于首次登录会命令行请求两步验证码, 登录成功后会生成 `.session` 文件, 随后才能部署为 `docker-compose` 服务.
+### 从源码构建
 
-您需要新建一个文件 `docker-compose.yml`:
+首先拉取并设置环境:
 
-```yaml
-version: '3'
-services:
-  embykeeper:
-    container_name: embykeeper
-    image: embykeeper/embykeeper
-    restart: unless-stopped
-    volumes:
-      - ./embykeeper:/app
-    network_mode: host
-  watchtower:
-    container_name: watchtower
-    image: containrrr/watchtower
-    restart: unless-stopped
-    volumes:
-      - /var/run/docker.sock:/var/run/docker.sock:rw
+```bash
+git clone https://github.com/embykeeper/embykeeper.git
+cd embykeeper
+python -m venv venv
+. ./venv/bin/activate
+pip install -e .
 ```
 
-其中, [watchtower](https://github.com/containrrr/watchtower) 被用于自动更新版本.
-
-然后运行以下命令以启动:
+然后即可执行 Embykeeper:
 
 ```bash
-docker-compose up -d
+embykeeper
 ```
 
-即可在后台启动 embykeeper.
+详细配置方法详见 [通过 Docker 部署](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 
-您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
+当版本更新时, 您需要执行:
+
+```
+git pull
+```
+
+然后重新运行应用.
 
 ## 命令行帮助
 
 您可以通过运行 `embykeeper -h` 以获取帮助:
 
 ```bash
 $ embykeeper -h
@@ -261,14 +252,15 @@
     --no-instant  -I   不立刻执行一次计划任务
     --once        -o   仅执行一次任务而不计划执行
     --debug       -d   开启调试输出, 错误将会导致程序停止运行
     --version     -v   打印 Embykeeper 版本
     --follow      -f   仅启动消息调试
     --analyze     -a   仅启动历史信息分析
     --basedir          设定输出文件默认位置
+    --public           启用在线部署模式
 ```
 
 例如:
 
 ```bash
 # 启动所有功能 (在各账号配置中进一步设置功能开启/关闭)
 $ embykeeper config.toml
@@ -288,62 +280,20 @@
 # 启动所有功能, 只运行一次
 $ embykeeper config.toml --once
 
 # 启动所有功能, 不立即执行一次签到/保活
 $ embykeeper config.toml -I
 ```
 
-您也可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
-
-```bash
-# 启动历史信息分析
-$ embykeeper config.toml -a
-
-请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
-请输入关键词 (以空格分隔):
-输入时间范围 (以"-"分割): 8:00AM-10:00AM
-请输入各群组最大获取数量 [1000]:
-```
-
-该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
-
-另一个工具是即时信息分析:
-
-![follow screenshot](images/follow.svg)
-
-该工具可以实时输出消息的 ID 等信息, 以方便调试.
-
-## 消息推送与高级用户
-
-您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
-
-本项目涉及的需要 Cloudflare 验证码付费跳过的操作 (例如 Nebula 签到)、可能会引起竞争的操作 (例如自动抢邀请码)将需要高级用户, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
-
-目前有三种方式成为高级用户:
-
-1. 分享 1 个邀请制 Emby 的邀请码;
-2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
-3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
-
-## 支持 Embykeeper
-
-##### 开发者团队
-
-- [jackzzs](https://github.com/jackzzs)
-
-##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
-
-![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
-
 ## 配置项
 
 | 设置项       | 值类型             | 简介                                         | 默认值  |
 | ------------ | ------------------ | -------------------------------------------- | ------- |
 | `timeout`    | `int`              | Telegram 机器人签到超时 (秒)                 | `120`   |
-| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`    |
+| `retries`    | `int`              | Telegram 机器人签到错误重试次数              | `4`     |
 | `concurrent` | `int`              | Telegram 机器人签到最大并发                  | `1`     |
 | `random`     | `int`              | Telegram 机器人签到各站点间时间随机量 (分钟) | `15`    |
 | `notifier`   | `int`/`bool`/`str` | 发送通知到 Telegram 账号 (序号/手机号)       | `False` |
 | `service`    | `dict`             | 签到/水群/监视功能开启站点设置               | `{}`    |
 | `proxy`      | `dict`             | 代理设置                                     | `{}`    |
 | `telegram`   | `list`             | Telegram 账号设置 (支持多账号)               | `[]`    |
 | `emby`       | `list`             | Emby 账号设置 (支持多账号)                   | `[]`    |
@@ -356,22 +306,22 @@
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
 若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
 若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
 当前支持的名称包括:
-| 站点 | 名称 | | 站点 | 名称 |
-| --- | --- | --- |--- | --- |
-| 垃圾影音 | `ljyy` | | 搜书神器 | `sosdbot` |
-| 卷毛鼠 IPTV | `jms_iptv` | | 终点站 | `terminus` |
-| Pornemby | `pornemby` | | Singularity | `singularity` |
-| Peach | `peach` | | Nebula | `nebula` |
-| Bluesea | `bluesea` | | Embyhub | `embyhub` |
-| 卷毛鼠 | `jms` | | 卡戎 | `charon` |
+| 站点        | 名称       |     | 站点        | 名称          |
+| ----------- | ---------- | --- | ----------- | ------------- |
+| 垃圾影音    | `ljyy`     |     | 搜书神器    | `sosdbot`     |
+| 卷毛鼠 IPTV | `jms_iptv` |     | 终点站      | `terminus`    |
+| Pornemby    | `pornemby` |     | Singularity | `singularity` |
+| Peach       | `peach`    |     | Nebula      | `nebula`      |
+| Bluesea     | `bluesea`  |     | Embyhub     | `embyhub`     |
+| 卷毛鼠      | `jms`      |     | 卡戎        | `charon`      |
 
 `proxy` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                    | 默认值      |
 | ---------- | ------ | --------------------------------------- | ----------- |
 | `hostname` | `str`  | 代理服务器地址                          | `localhost` |
 | `port`     | `int`  | 代理端口号                              | `1080`      |
@@ -404,14 +354,36 @@
 [monitor.bgk] # 支持 bgk, embyhub, polo
 unique_name = "your_username_for_registeration" # 自动抢注时使用的用户名
 
 [monitor.pornemby]
 only_history = true # 仅当问题历史中找到答案时自动回答
 ```
 
+## 消息推送与高级用户
+
+您可以通过设置项 "`notifier`" 设置 成功/失败 通知将被发送的 Telegram 账号, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot) 设置消息每日发送的时间.
+
+本项目涉及的需要 Cloudflare 验证码付费跳过的操作 (例如 Nebula 签到)、可能会引起竞争的操作 (例如自动抢邀请码)将需要高级用户, 您可以通过 [Embykeeper Bot](https://t.me/embykeeper_bot?start=__prime) 成为高级用户.
+
+目前有三种方式成为高级用户:
+
+1. 分享 1 个邀请制 Emby 的邀请码;
+2. 为本项目提供 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 并被合并;
+3. 通过爱发电赞助一个[小包子](https://afdian.net/a/jackzzs);
+
+## 支持 Embykeeper
+
+##### 开发者团队
+
+- [jackzzs](https://github.com/jackzzs)
+
+##### 通过[爱发电](https://afdian.net/a/jackzzs)赞助
+
+![Kitty](https://github.com/embykeeper/embykeeper/raw/main/images/kitty.gif)
+
 ## 代码重用与开发
 
 代码架构如下:
 
 ```mermaid
 flowchart TD
     A(fa:fa-terminal cli) --> B(fa:fa-telegram telechecker)
@@ -459,10 +431,32 @@
                 break
 ```
 
 上述代码实现每次按对应一个字符按键的功能.
 
 当您实现一个新的签到器时, 欢迎您提出 [Pull Requests](https://github.com/embykeeper/embykeeper/pulls) 以帮助更多人使用!
 
+## 开发工具
+
+您可以使用附带的调试工具帮助本项目的开发, 例如历史记录分析器:
+
+```bash
+# 启动历史信息分析
+$ embykeeper config.toml -a
+
+请输入群组用户名 (以空格分隔): https://t.me/XXX YYY 10253512
+请输入关键词 (以空格分隔):
+输入时间范围 (以"-"分割): 8:00AM-10:00AM
+请输入各群组最大获取数量 [1000]:
+```
+
+该命令会分析特定群组的历史记录, 以帮助您撰写自动水群工具的话术列表.
+
+另一个工具是即时信息分析:
+
+![follow screenshot](images/follow.svg)
+
+该工具可以实时输出消息的 ID 等信息, 以方便调试.
+
 ## 趋势
 
 [![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

#### html2text {}

```diff
@@ -1,23 +1,12 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.1.1 Summary: Daily checkin
-automator for emby bots in telegram. Author-email: jackzzs
-outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
-Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
-Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
-:: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
-Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: <3.11,>=3.8 Description-Content-Type: text/markdown License-
-File: LICENSE [![build status](https://img.shields.io/github/actions/workflow/
-status/embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/
-embykeeper/embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/
-v/embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https:
-//img.shields.io/pypi/dm/
+[![build status](https://img.shields.io/github/actions/workflow/status/
+embykeeper/embykeeper/ci.yml?branch=main)](https://github.com/embykeeper/
+embykeeper/commits/main) [![pypi badge](https://img.shields.io/pypi/v/
+embykeeper)](https://pypi.org/project/embykeeper/) [![downloads badge](https://
+img.shields.io/pypi/dm/
 embykeeper?color=%234287f5&label=downloads&logoColor=%234287f5)](https://
 pypi.org/project/embykeeper/) [![docker](https://img.shields.io/docker/v/
 embykeeper/embykeeper?label=docker)](https://hub.docker.com/r/embykeeper/
 embykeeper) [![license badge](https://img.shields.io/github/license/embykeeper/
 embykeeper)](https://github.com/embykeeper/embykeeper/blob/main/LICENSE) [!
 [telegram badge](https://img.shields.io/badge/telegram-bot-blue)](https://t.me/
 embykeeper_bot) [![telegram badge](https://img.shields.io/badge/telegram-
@@ -45,39 +34,38 @@
 å½æ¨ä½¿ç¨ "æ¶æ¯æç¤º" åè½, è¯¥å·¥å·æ¶åå°èªå¨å "[Embykeeper
 Auth Bot](https://t.me/embykeeper_auth_bot)" åéå³é®çæå/
 å¤±è´¥æ¥å¿ä»¥ä¾ä» "[Embykeeper Bot](https://t.me/embykeeper_bot)"
 åæ¨æ¨é, æ¥å¿åå®¹ä¸å«ä»»ä½å¯ç æå¯é¥ä¿¡æ¯,
 æ¨è®¤å¯è¯¥å½ä»¤ä¸ä¼ç»æ¨å¸¦æ¥éç§ä¸å®å¨é®é¢.
 å½æ¨å®è£å¹¶ä½¿ç¨è¯¥å·¥å·, é»è®¤æ¨å·²ç»éè¯»å¹¶åæä¸è¿°å£°æ,
 å¹¶ç¡®è®¤èªå·±å¹¶éåºäº"éé®"ç®çèå®è£. ## åè½ - Telegram
-æºå¨äººç­¾å° - ç»ç¹ç«: [é¢é](https://t.me/embypub) [ç¾¤ç»](https://
-t.me/EmbyPublic) [æºå¨äºº](https://t.me/EmbyPublicBot) - Nebula: [é¢é]
-(https://t.me/Nebula_Emby) [ç¾¤ç»](https://t.me/NebulaEmbyUser) [æºå¨äºº]
-(https://t.me/Nebula_Account_bot) (ç±äºéè¦ä»è´¹è·³è¿ Cloudflare
-éªè¯ç , éè¦[é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime)) -
-Singularity: [é¢é](https://t.me/Singularity_Emby_Channel) [ç¾¤ç»](https://
-t.me/Singularity_Emby_Group) [æºå¨äºº](https://t.me/Singularity_Emby_Bot) -
-Peach: [é¢é](https://t.me/peach_emby_channel) [ç¾¤ç»](https://t.me/
-peach_emby_chat) [æºå¨äºº](https://t.me/peach_emby_bot) - EmbyHub: [é¢é]
-(https://t.me/embyhub) [ç¾¤ç»](https://t.me/emby_hub) [æºå¨äºº](https://
-t.me/EdHubot) - Pornemby: [é¢é](https://t.me/pornembyservice) [ç¾¤ç»]
-(https://t.me/Pornemby) [æºå¨äºº](https://t.me/PronembyTGBot2_bot) -
-åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1) [æºå¨äºº](https://
-t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV) [ç¾¤ç»](https://
-t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) - å¶ä»é Emby
-ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/embykeeper/
-pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
-~~å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https://t.me/
-Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot)~~
-(æºå¨äººé»è¾é¢ç¹åå¨, ææ¶ç¦ç¨) - ~~BlueSea: [ç¾¤ç»](https://t.me/
-blueseachat) [æºå¨äºº](https://t.me/blueseamusic_bot)~~ (æ ååº) -
-~~å·æ¯é¼  IPTV: [é¢é](https://t.me/CurlyMouseIPTV) [ç¾¤ç»](https://t.me/
-Curly_MouseIPTV) [æºå¨äºº](https://t.me/JMSIPTV_bot)~~ (æ ååº) - Emby
-ä¿æ´» - å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ -
-Telegram èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
+æºå¨äººç­¾å° - å·æ¯é¼ : [é¢é](https://t.me/CurlyMouse) [ç¾¤ç»](https:/
+/t.me/Curly_Mouse) [æºå¨äºº](https://t.me/jmsembybot) - ç»ç¹ç«: [é¢é]
+(https://t.me/embypub) [ç¾¤ç»](https://t.me/EmbyPublic) [æºå¨äºº](https://
+t.me/EmbyPublicBot) - Nebula: [é¢é](https://t.me/Nebula_Emby) [ç¾¤ç»]
+(https://t.me/NebulaEmbyUser) [æºå¨äºº](https://t.me/Nebula_Account_bot)
+(ç±äºéè¦ä»è´¹è·³è¿ Cloudflare éªè¯ç , éè¦[é«çº§ç¨æ·](https://
+t.me/embykeeper_bot?start=__prime)) - Singularity: [é¢é](https://t.me/
+Singularity_Emby_Channel) [ç¾¤ç»](https://t.me/Singularity_Emby_Group)
+[æºå¨äºº](https://t.me/Singularity_Emby_Bot) - Peach: [é¢é](https://t.me/
+peach_emby_channel) [ç¾¤ç»](https://t.me/peach_emby_chat) [æºå¨äºº](https://
+t.me/peach_emby_bot) - EmbyHub: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https:/
+/t.me/emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Pornemby: [é¢é](https://
+t.me/pornembyservice) [ç¾¤ç»](https://t.me/Pornemby) [æºå¨äºº](https://t.me/
+PronembyTGBot2_bot) - åå¾å½±é³: [ç¾¤ç»](https://t.me/+3sP2A-fgeXg0ZmY1)
+[æºå¨äºº](https://t.me/zckllflbot) - å¡æ: [é¢é](https://t.me/CharonTV)
+[ç¾¤ç»](https://t.me/CharonTV_Talk) [æºå¨äºº](https://t.me/CharonTV_Bot) -
+å¶ä»é Emby ç¸å³: - æä¹¦ç¥å¨ ([@chneez](https://github.com/embykeeper/
+embykeeper/pull/8) å¢å ): [æºå¨äºº](https://t.me/sosdbot) - é»è®¤ç¦ç¨: -
+~~BlueSea: [ç¾¤ç»](https://t.me/blueseachat) [æºå¨äºº](https://t.me/
+blueseamusic_bot)~~ (æ ååº) - ~~å·æ¯é¼  IPTV: [é¢é](https://t.me/
+CurlyMouseIPTV) [ç¾¤ç»](https://t.me/Curly_MouseIPTV) [æºå¨äºº](https://
+t.me/JMSIPTV_bot)~~ (æ ååº) - Emby ä¿æ´» -
+å®æ¶æ¨¡æè´¦å·ç»å½è§é¢æ­æ¾ - æ­æ¾æ¶é´ä¸è¿åº¦æ¨¡æ - Telegram
+èªå¨æ°´ç¾¤ (é»è®¤ä½¿ç¨åå»ºè¯æ¯åè¡¨, æè¢«è¾¨å«åå°ç¦,
 è¯·è°¨æä½¿ç¨) - é»è®¤ç¦ç¨: - ~~NakoNako èªå¨æ°´ç¾¤: [ç¾¤ç»](https://
 t.me/NakoNetwork) [æºå¨äºº](https://t.me/nakonetwork_bot)~~ (åæ) -
 Telegram èªå¨çæ§ä¿¡æ¯ (éè¦[è¶çº§ç¨æ·](https://t.me/
 embykeeper_bot?start=__prime)) - Pornemby ç§ä¸¾èè¯: [æ´»å¨é¢é](https://
 t.me/PornembyFun) (ç±äºéè¦ä½¿ç¨ OpenAI API è¿è¡åç­, éè¦
 [é«çº§ç¨æ·](https://t.me/embykeeper_bot?start=__prime),
 åç­åç¡®çä¸è¬è¯·è°¨æä½¿ç¨) - ä¸ç»ç æ¢éè¯·ç : [ç¾¤ç»](https:
@@ -85,166 +73,168 @@
 æ¢éè¯·ç : [é¢é](https://t.me/viper_emby_channel) [ç¾¤ç»](https://t.me/
 Viper_Emby_Chat) [æºå¨äºº](https://t.me/viper_emby_bot) - Embyhub
 å¼æ³¨èªå¨æ³¨å: [é¢é](https://t.me/embyhub) [ç¾¤ç»](https://t.me/
 emby_hub) [æºå¨äºº](https://t.me/EdHubot) - Misty å¼æ³¨èªå¨æ³¨å:
 [é¢é](https://t.me/FreeEmbyChannel) [ç¾¤ç»](https://t.me/FreeEmby)
 [æºå¨äºº](https://t.me/EmbyMistyBot) - é»è®¤ç¦ç¨: - ~~Polo æ¢éè¯·ç :
 [é¢é](https://t.me/poloembyc) [ç¾¤ç»](https://t.me/poloemby) [æºå¨äºº]
-(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### ä»
-PyPi å®è£ Embykeeper å¯ä»¥éè¿ `python` è¿è¡, æ¨å¯ä»¥éè¿ [conda]
-(https://github.com/conda/conda) æ [virtualvenv](https://virtualenv.pypa.io/
-) ç­å·¥å·è¿è¡ç¯å¢çç®¡ç. æ¨å¯ä»¥éè¿ `pip` å®è£ `embykeeper`
-(éè¦ `python >= 3.7, < 3.11`): ```bash pip install embykeeper ``` éå,
-æ¨éè¦æ§è¡: ```bash embykeeper ``` å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿
-`config.toml` æä»¶, æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½®
-(ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè): ```toml [proxy] hostname =
-"127.0.0.1" port = 1080 scheme = "socks5" [[telegram]] api_id = "27894236"
-api_hash = "622159182fdd4b15b627eeb3ac695271" phone = "+8612109347899" [[emby]]
-url = "https://weiss-griffin.com/" username = "carrie19" password =
-"s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿ [Telegram å®ç½]
-(https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
-development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
-æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
-æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
-æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. éå, æ¨éè¦åæ¬¡æ§è¡:
-```bash embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
-ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
-ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
-æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
-é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
-``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
-æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
-Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
-æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
-ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
-ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º åä» PyPi
-å®è£ç±»ä¼¼ï¼æ¨éè¦ä¸ä¸ªåè®¾ç½® Python ç¯å¢, ç¶åæå Github
-å¹¶å®è£: ```bash git clone https://github.com/embykeeper/embykeeper.git cd
-embykeeper pip install -e . ``` ç¶åå³å¯æ§è¡ Embykeeper: ```bash
-embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§ [ä» Pypi å®è£](https://github.com/
-embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85). å½çæ¬æ´æ°æ¶,
-æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ### ä» Docker
-é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½², æ¨é [å®è£ docker](https://
-yeasy.gitbook.io/docker_practice/install), ç¶åæ§è¡: ```bash docker run -
-v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper ```
-å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿ `config.toml` æä»¶,
-æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯ (è¯¦è§[ä» Pypi å®è£](https://github.com/
-embykeeper/embykeeper#%E4%BB%8E-pypi-%E5%AE%89%E8%A3%85)). éå,
-æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
-net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
-ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+(https://t.me/polo_emby_bot)~~ (å¬çæå³é­) ## å®è£ä¸ä½¿ç¨ ### Railway
+å¨çº¿é¨ç½² Embykeeper å¯ä»¥éè¿åè´¹ç Railway Docker
+æç®¡å¹³å°è¿è¡é¨ç½², ç¹å»ä¸æ¹æé®å¼å§é¨ç½²: [![Deploy on Railway]
+(https://railway.app/button.svg)](https://railway.app/template/
+WFYaj9?referralCode=Fj6Yvy) è¯·æ³¨æ Railway çåè´¹ç¨éææ¯æ 5
+ç¾å, 500 å°æ¶ (21 å¤©) çéå¶. å¦æé¢å¤éè¦è¯·éè¿ Docker
+é¨ç½². ### éè¿ Docker é¨ç½² Embykeeper å¯ä»¥éè¿ `docker` é¨ç½²,
+æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
+ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
+embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
+net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
+`config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
+æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
+```toml [proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [
+[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
+phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
+"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
+[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
+ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
+è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
+"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
+æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --
+rm -it --net=host embykeeper/embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
-compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [ä» Docker
-é¨ç½²](https://github.com/embykeeper/embykeeper#%E4%BB%8E-Docker-
+compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
+é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
 %E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
 è¿æ¯ç±äºé¦æ¬¡ç»å½ä¼å½ä»¤è¡è¯·æ±ä¸¤æ­¥éªè¯ç ,
 ç»å½æååä¼çæ `.session` æä»¶, éåæè½é¨ç½²ä¸º `docker-
 compose` æå¡. æ¨éè¦æ°å»ºä¸ä¸ªæä»¶ `docker-compose.yml`: ```yaml
 version: '3' services: embykeeper: container_name: embykeeper image:
 embykeeper/embykeeper restart: unless-stopped volumes: - ./embykeeper:/app
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
 docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
 watchtower) è¢«ç¨äºèªå¨æ´æ°çæ¬. ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨:
 ```bash docker-compose up -d ``` å³å¯å¨åå°å¯å¨ embykeeper.
 æ¨å¯ä»¥éè¿ `docker logs -f embykeeper` æ `docker-compose logs -
-f embykeeper` ä»¥æ¥çææ°æ¥å¿. ## å½ä»¤è¡å¸®å© æ¨å¯ä»¥éè¿è¿è¡
-`embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -h æ¬¢è¿ä½¿ç¨
-Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°: config éç½®æä»¶
-(ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -c å¯ç¨æ¯æ¥ç­¾å°
-(ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --emby -
-e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
+f embykeeper` ä»¥æ¥çææ°æ¥å¿. ### ä» PyPi å®è£ Embykeeper
+å¯ä»¥éè¿ `python >= 3.7, < 3.11` è¿è¡, æ¨å¯ä»¥éè¿ [virtualvenv]
+(https://virtualenv.pypa.io/) è¿è¡ç¯å¢çç®¡ç: ```bash python -m venv
+embykeeper-venv . ./embykeeper-venv/bin/activate pip install embykeeper ```
+éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
+å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
+æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, åè§ [éè¿ Docker é¨ç½²](https://
+github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
+éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
+æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
+å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
+æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper, ä¸ºäºè®© Embykeeper
+é¿æåå°è¿è¡, æ¨å¯ä»¥éè¿`Ctrl+C`åæ­¢, ç¶åè¿è¡: ```bash tmux
+``` è¿å°å¯å¨ä¸ä¸ª `tmux` ç»ç«¯,
+æ¨å¯ä»¥å¨è¯¥ç»ç«¯ä¸­è¿è¡ä¸è¿°å½ä»¤ (`embykeeper config.toml`), å¹¶æ
+Ctrl + B, æ¾å¼ B åæ D, ä»¥è±ç¦» `tmux` ç»ç«¯.
+æ¨éæ¶å¯ä»¥éè¿è¿è¡: ```bash tmux a ``` ä»¥éæ°è¿æ¥å° `tmux`
+ç»ç«¯. å½çæ¬æ´æ°æ¶, æ¨éè¦æ§è¡: ``` pip install -U embykeeper ```
+ç¶åéæ°è¿è¡åºç¨. ### ä»æºç æå»º é¦åæåå¹¶è®¾ç½®ç¯å¢:
+```bash git clone https://github.com/embykeeper/embykeeper.git cd embykeeper
+python -m venv venv . ./venv/bin/activate pip install -e . ```
+ç¶åå³å¯æ§è¡ Embykeeper: ```bash embykeeper ``` è¯¦ç»éç½®æ¹æ³è¯¦è§
+[éè¿ Docker é¨ç½²](https://github.com/embykeeper/
+embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2). å½çæ¬æ´æ°æ¶,
+æ¨éè¦æ§è¡: ``` git pull ``` ç¶åéæ°è¿è¡åºç¨. ## å½ä»¤è¡å¸®å©
+æ¨å¯ä»¥éè¿è¿è¡ `embykeeper -h` ä»¥è·åå¸®å©: ```bash $ embykeeper -
+h æ¬¢è¿ä½¿ç¨ Embykeeper. ð¦ æ åæ°é»è®¤å¼å¯å¨é¨åè½. åæ°:
+config éç½®æä»¶ (ç½®ç©ºä»¥çæ) æ¨¡åå¼å³: --checkin -
+c å¯ç¨æ¯æ¥ç­¾å° (ä¸æå®å¼æ¶é»è®¤ä¸º<8:00PM,9:00PM>éæºæ¶é´) --
+emby -e å¯ç¨æ¯éå¤©æ°Embyèªå¨ä¿æ´» (ä¸æå®å¼æ¶é»è®¤ä¸ºæ¯7å¤©) --
 monitor -m å¯ç¨ç¾¤èçè§ --send -s å¯ç¨èªå¨æ°´ç¾¤ è°è¯åæ°: --no-
 instant -I ä¸ç«å»æ§è¡ä¸æ¬¡è®¡åä»»å¡ --once -
 o ä»æ§è¡ä¸æ¬¡ä»»å¡èä¸è®¡åæ§è¡ --debug -d å¼å¯è°è¯è¾åº,
 éè¯¯å°ä¼å¯¼è´ç¨åºåæ­¢è¿è¡ --version -v æå° Embykeeper çæ¬ --
 follow -f ä»å¯å¨æ¶æ¯è°è¯ --analyze -a ä»å¯å¨åå²ä¿¡æ¯åæ --
-basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® ``` ä¾å¦: ```bash # å¯å¨ææåè½
+basedir è®¾å®è¾åºæä»¶é»è®¤ä½ç½® --public å¯ç¨å¨çº¿é¨ç½²æ¨¡å¼ ```
+ä¾å¦: ```bash # å¯å¨ææåè½
 (å¨åè´¦å·éç½®ä¸­è¿ä¸æ­¥è®¾ç½®åè½å¼å¯/å³é­) $ embykeeper
 config.toml # ä»å¯å¨æ¯æ¥ç­¾å° $ embykeeper config.toml -c #
 ä»å¯å¨æ¯æ¥ 8:00 PM ç­¾å° $ embykeeper config.toml -c 8:00PM #
 ä»å¯å¨æ¯æ¥ 8:00 PM - 9:00 PM éæºæ¶é´ç­¾å° $ embykeeper config.toml -
 c <8:00PM,9:00PM> # å¯å¨ææåè½, åæ¶è°æ´ç­¾å°æ¶é´ä¸º 8:00 AM,
 è°æ´ä¿æ´»é´éå¤©æ°ä¸º 14 $ embykeeper config.toml -c 8:00PM -e 14 -m -s #
 å¯å¨ææåè½, åªè¿è¡ä¸æ¬¡ $ embykeeper config.toml --once #
 å¯å¨ææåè½, ä¸ç«å³æ§è¡ä¸æ¬¡ç­¾å°/ä¿æ´» $ embykeeper config.toml
--I ``` æ¨ä¹å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
-ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
-config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
-10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
-"åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
-è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
-ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
-å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
-è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ##
+-I ``` ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------
+-- | ------------------ | -------------------------------------------- | ------
+- | | `timeout` | `int` | Telegram æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | |
+`retries` | `int` | Telegram æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | |
+`concurrent` | `int` | Telegram æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random`
+| `int` | Telegram æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` |
+| `notifier` | `int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/
+ææºå·) | `False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/
+çè§åè½å¼å¯ç«ç¹è®¾ç½® | `{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `
+{}` | | `telegram` | `list` | Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
+| `emby` | `list` | Emby è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` |
+`service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----
+------- | ------ | -------------- | -------------------- | | `checkiner` |
+`list` | å¯ç¨çç­¾å°ç«ç¹ | (å½åæææ¯æçç«ç¹) | | `monitor` |
+`list` | å¯ç¨ççè§ä¼è¯ | (å½åæææ¯æçä¼è¯) | | `messager` |
+`list` | å¯ç¨çæ°´ç¾¤ä¼è¯ | (å½åæææ¯æçä¼è¯) | æ³¨æ,
+å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯, è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡.
+è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
+è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
+æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
+ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | ----------- | ---------- | --- | ------
+----- | ------------- | | åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` |
+| å·æ¯é¼  IPTV | `jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby |
+`pornemby` | | Singularity | `singularity` | | Peach | `peach` | | Nebula |
+`nebula` | | Bluesea | `bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms`
+| | å¡æ | `charon` | `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å |
+ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------------------
+----- | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
+`localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` | `str`
+| ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
+è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
+------ | ------------------------------------------------------------------ | -
+------ | | `api_id` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/
+)ç³è¯·ç Application ID | | | `api_hash` | `str` | ä»[Telegram å®ç½]
+(https://my.telegram.org/)ç³è¯·ç Application Hash | | | `phone` | `str` |
+è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | | `monitor` | `bool` |
+å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` | `bool` |
+å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹
+| å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | --------------------
+------------------------------------- | ------ | | `url` | `str` | Emby
+æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
+| `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
+æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
+`progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
+æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
+bgk, embyhub, polo unique_name = "your_username_for_registeration" #
+èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
+ä»å½é®é¢åå²ä¸­æ¾å°ç­æ¡æ¶èªå¨åç­ ``` ##
 æ¶æ¯æ¨éä¸é«çº§ç¨æ· æ¨å¯ä»¥éè¿è®¾ç½®é¡¹ "`notifier`" è®¾ç½®
 æå/å¤±è´¥ éç¥å°è¢«åéç Telegram è´¦å·, æ¨å¯ä»¥éè¿
 [Embykeeper Bot](https://t.me/embykeeper_bot)
 è®¾ç½®æ¶æ¯æ¯æ¥åéçæ¶é´. æ¬é¡¹ç®æ¶åçéè¦ Cloudflare
 éªè¯ç ä»è´¹è·³è¿çæä½ (ä¾å¦ Nebula
 ç­¾å°)ãå¯è½ä¼å¼èµ·ç«äºçæä½
 (ä¾å¦èªå¨æ¢éè¯·ç )å°éè¦é«çº§ç¨æ·, æ¨å¯ä»¥éè¿ [Embykeeper
 Bot](https://t.me/embykeeper_bot?start=__prime) æä¸ºé«çº§ç¨æ·.
 ç®åæä¸ç§æ¹å¼æä¸ºé«çº§ç¨æ·: 1. åäº« 1 ä¸ªéè¯·å¶ Emby
 çéè¯·ç ; 2. ä¸ºæ¬é¡¹ç®æä¾ [Pull Requests](https://github.com/
 embykeeper/embykeeper/pulls) å¹¶è¢«åå¹¶; 3. éè¿ç±åçµèµå©ä¸ä¸ª
 [å°åå­](https://afdian.net/a/jackzzs); ## æ¯æ Embykeeper #####
 å¼åèå¢é - [jackzzs](https://github.com/jackzzs) ##### éè¿[ç±åçµ]
 (https://afdian.net/a/jackzzs)èµå© ![Kitty](https://github.com/embykeeper/
-embykeeper/raw/main/images/kitty.gif) ## éç½®é¡¹ | è®¾ç½®é¡¹ | å¼ç±»å |
-ç®ä» | é»è®¤å¼ | | ------------ | ------------------ | --------------------
------------------------- | ------- | | `timeout` | `int` | Telegram
-æºå¨äººç­¾å°è¶æ¶ (ç§) | `120` | | `retries` | `int` | Telegram
-æºå¨äººç­¾å°éè¯¯éè¯æ¬¡æ° | `4` | | `concurrent` | `int` | Telegram
-æºå¨äººç­¾å°æå¤§å¹¶å | `1` | | `random` | `int` | Telegram
-æºå¨äººç­¾å°åç«ç¹é´æ¶é´éæºé (åé) | `15` | | `notifier` |
-`int`/`bool`/`str` | åééç¥å° Telegram è´¦å· (åºå·/ææºå·) |
-`False` | | `service` | `dict` | ç­¾å°/æ°´ç¾¤/çè§åè½å¼å¯ç«ç¹è®¾ç½® |
-`{}` | | `proxy` | `dict` | ä»£çè®¾ç½® | `{}` | | `telegram` | `list` |
-Telegram è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | | `emby` | `list` | Emby
-è´¦å·è®¾ç½® (æ¯æå¤è´¦å·) | `[]` | `service`è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ----------- | ------ | -------------- | ----
----------------- | | `checkiner` | `list` | å¯ç¨çç­¾å°ç«ç¹ |
-(å½åæææ¯æçç«ç¹) | | `monitor` | `list` | å¯ç¨ççè§ä¼è¯ |
-(å½åæææ¯æçä¼è¯) | | `messager` | `list` | å¯ç¨çæ°´ç¾¤ä¼è¯ |
-(å½åæææ¯æçä¼è¯) | æ³¨æ, å½æ¨æªæ¾ä¸ç«ç¹æºå¨äººå¯¹è¯,
-è¯¥ç«ç¹ç­¾å°å°ä¸ä¼è¿è¡. è¥æ¨éè¦ç¦ç¨é¨åç­¾å°ç«ç¹,
-æ¨å¯ä»¥å¨åè¡¨ä¸­å é¤å¯¹åºçåç§°.
-è¥æ¨éè¦ä½¿ç¨é»è®¤ç¦ç¨çç­¾å°ç«ç¹,
-æ¨å¯ä»¥å¨åè¡¨ä¸­å¢å å¯¹åºçåç§°. å½åæ¯æçåç§°åæ¬: |
-ç«ç¹ | åç§° | | ç«ç¹ | åç§° | | --- | --- | --- |--- | --- | |
-åå¾å½±é³ | `ljyy` | | æä¹¦ç¥å¨ | `sosdbot` | | å·æ¯é¼  IPTV |
-`jms_iptv` | | ç»ç¹ç« | `terminus` | | Pornemby | `pornemby` | | Singularity
-| `singularity` | | Peach | `peach` | | Nebula | `nebula` | | Bluesea |
-`bluesea` | | Embyhub | `embyhub` | | å·æ¯é¼  | `jms` | | å¡æ | `charon` |
-`proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | -----
------ | ------ | --------------------------------------- | ----------- | |
-`hostname` | `str` | ä»£çæå¡å¨å°å | `localhost` | | `port` | `int` |
-ä»£çç«¯å£å· | `1080` | | `scheme` | `str` | ä»£çåè®®, å¯ä»¥ä¸º
-"`socks5`" æ "`http`" | `socks5` | `telegram` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
-å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
--------------------------------------------- | ------- | | `api_id` | `str` |
-ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID | | |
-`api_hash` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç
-Application Hash | | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`"
-| | | `monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send`
-| `bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: |
-è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------
------------------------------------------------ | ------ | | `url` | `str` |
-Emby æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | |
-`username` | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
-æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
-`progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
-æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
-bgk, embyhub, polo unique_name = "your_username_for_registeration" #
-èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
-ä»å½é®é¢åå²ä¸­æ¾å°ç­æ¡æ¶èªå¨åç­ ``` ## ä»£ç éç¨ä¸å¼å
+embykeeper/raw/main/images/kitty.gif) ## ä»£ç éç¨ä¸å¼å
 ä»£ç æ¶æå¦ä¸: ```mermaid flowchart TD A(fa:fa-terminal cli) --> B(fa:fa-
 telegram telechecker) A --> C(fa:fa-play embywatcher) B --checker--> E[fa:fa-
 robot Bot] B --monitor--> G[fa:fa-eye Monitor] B --messager--> F[fa:fa-message
 Messager] C --watcher--> H[fa:fa-circle-play EmbyWatcher] F ---- |schedule| A
 ``` ä¸»è¦å¯ä»¥æ©å±çç±»ä½äº: - `embykeeper.telechecker.bots` -
 `embykeeper.telechecker.monitor` - `embykeeper.telechecker.messager`
 éå¸¸æ¥è¯´, å¢å ä¸ä¸ªæºå¨äººçç­¾å°éå¸¸ç®å, æ¨éè¦å¨ `bots`
@@ -257,10 +247,19 @@
 å½æ°æ¥å®ç°èªå®ä¹åè½: ```python from .base import AnswerBotCheckin
 class DummyCheckin(AnswerBotCheckin): .... async def on_captcha(self, message:
 Message, captcha: str): for l in captcha: try: await self.message.click(l)
 except ValueError: self.log.info(f'æªè½æ¾å°å¯¹åº "{l}" çæé®,
 æ­£å¨éè¯.') await self.retry() break ```
 ä¸è¿°ä»£ç å®ç°æ¯æ¬¡æå¯¹åºä¸ä¸ªå­ç¬¦æé®çåè½.
 å½æ¨å®ç°ä¸ä¸ªæ°çç­¾å°å¨æ¶, æ¬¢è¿æ¨æåº [Pull Requests](https://
-github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! ## è¶å¿ [!
-[Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
+github.com/embykeeper/embykeeper/pulls) ä»¥å¸®å©æ´å¤äººä½¿ç¨! ##
+å¼åå·¥å· æ¨å¯ä»¥ä½¿ç¨éå¸¦çè°è¯å·¥å·å¸®å©æ¬é¡¹ç®çå¼å,
+ä¾å¦åå²è®°å½åæå¨: ```bash # å¯å¨åå²ä¿¡æ¯åæ $ embykeeper
+config.toml -a è¯·è¾å¥ç¾¤ç»ç¨æ·å (ä»¥ç©ºæ ¼åé): https://t.me/XXX YYY
+10253512 è¯·è¾å¥å³é®è¯ (ä»¥ç©ºæ ¼åé): è¾å¥æ¶é´èå´ (ä»¥"-
+"åå²): 8:00AM-10:00AM è¯·è¾å¥åç¾¤ç»æå¤§è·åæ°é [1000]: ```
+è¯¥å½ä»¤ä¼åæç¹å®ç¾¤ç»çåå²è®°å½,
+ä»¥å¸®å©æ¨æ°åèªå¨æ°´ç¾¤å·¥å·çè¯æ¯åè¡¨.
+å¦ä¸ä¸ªå·¥å·æ¯å³æ¶ä¿¡æ¯åæ: ![follow screenshot](images/follow.svg)
+è¯¥å·¥å·å¯ä»¥å®æ¶è¾åºæ¶æ¯ç ID ç­ä¿¡æ¯, ä»¥æ¹ä¾¿è°è¯. ## è¶å¿
+[![Star History Chart](https://api.star-history.com/svg?repos=embykeeper/
 embykeeper&type=Date)](https://star-history.com/#embykeeper/embykeeper&Date)
```

### Comparing `embykeeper-2.1.1/pyproject.toml` & `embykeeper-2.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.1.1"
+version = "2.2.0"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
@@ -47,26 +47,32 @@
     "pyrogram",
     "tgcrypto",
     "pillow",
     "thefuzz[speedup]",
     "schema",
     "aiocache",
     "fake_useragent",
-    "pycryptodome"
+    "pycryptodome",
+    "flask",
+    "flask_socketio",
+    "flask_login",
+    "simple-websocket",
+    "eventlet",
 ]
 
 [project.urls]
 Homepage = "https://github.com/embykeeper/embykeeper"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.scripts]
 embykeeper = "embykeeper.cli:app"
+embykeeperweb = "embykeeperweb.app:cli"
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.packages]
 find = {namespaces = false}
```

### Comparing `embykeeper-2.1.1/tests/test_cli.py` & `embykeeper-2.2.0/tests/test_cli.py`

 * *Files identical despite different names*

