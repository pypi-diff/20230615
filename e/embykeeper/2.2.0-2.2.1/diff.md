# Comparing `tmp/embykeeper-2.2.0.tar.gz` & `tmp/embykeeper-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embykeeper-2.2.0.tar", last modified: Thu Jun 15 08:38:45 2023, max compression
+gzip compressed data, was "embykeeper-2.2.1.tar", last modified: Thu Jun 15 16:44:48 2023, max compression
```

## Comparing `embykeeper-2.2.0.tar` & `embykeeper-2.2.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.106456 embykeeper-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 08:38:29.000000 embykeeper-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 08:38:29.000000 embykeeper-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21320 2023-06-15 08:38:45.106456 embykeeper-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20477 2023-06-15 08:38:29.000000 embykeeper-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.086456 embykeeper-2.2.0/embykeeper/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.090456 embykeeper-2.2.0/embykeeper/embywatcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/embywatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/embywatcher/emby.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/embywatcher/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.094456 embykeeper-2.2.0/embykeeper/telechecker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.098456 embykeeper-2.2.0/embykeeper/telechecker/bots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/bluesea.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/charon.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/jms.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/jms_iptv.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/ljyy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/nebula.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/peach.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/singularity.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/sssq.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/bots/terminus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.098456 embykeeper-2.2.0/embykeeper/telechecker/messager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/nakonako.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/messager/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.098456 embykeeper-2.2.0/embykeeper/telechecker/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/bgk.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/embyhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/misty.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/polo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/pornemby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/monitor/viper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/telechecker/tele.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.090456 embykeeper-2.2.0/embykeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21320 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 08:38:44.000000 embykeeper-2.2.0/embykeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 08:38:45.000000 embykeeper-2.2.0/embykeeper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.082456 embykeeper-2.2.0/embykeeperweb/templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.082456 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/css/
--rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/js/
--rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/css/cascadia-code.css
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/css/icons.css
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/css/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.082456 embykeeper-2.2.0/embykeeperweb/templates/assets/img/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/404.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/login.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.102456 embykeeper-2.2.0/embykeeperweb/templates/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/js/console.js
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/assets/js/script.js
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/console.html
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-15 08:38:29.000000 embykeeper-2.2.0/embykeeperweb/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 08:38:29.000000 embykeeper-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 08:38:45.106456 embykeeper-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 08:38:45.106456 embykeeper-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-15 08:38:29.000000 embykeeper-2.2.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.196441 embykeeper-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 16:44:35.000000 embykeeper-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-15 16:44:35.000000 embykeeper-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-06-15 16:44:48.196441 embykeeper-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20575 2023-06-15 16:44:35.000000 embykeeper-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.180441 embykeeper-2.2.1/embykeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.184441 embykeeper-2.2.1/embykeeper/embywatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/embywatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/embywatcher/emby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/embywatcher/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.184441 embykeeper-2.2.1/embykeeper/telechecker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.188441 embykeeper-2.2.1/embykeeper/telechecker/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17239 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/bluesea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/charon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/jms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/jms_iptv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/ljyy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/nebula.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/peach.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/sssq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/bots/terminus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeper/telechecker/messager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/nakonako.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/messager/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeper/telechecker/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/bgk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/embyhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/misty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/polo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/pornemby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/monitor/viper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13968 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/telechecker/tele.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.184441 embykeeper-2.2.1/embykeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:44:47.000000 embykeeper-2.2.1/embykeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 16:44:48.000000 embykeeper-2.2.1/embykeeper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.176441 embykeeper-2.2.1/embykeeperweb/templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.176441 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   202097 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    80372 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/css/cascadia-code.css
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/css/icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/css/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.176441 embykeeper-2.2.1/embykeeperweb/templates/assets/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/404.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/login.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/logo-only.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/embykeeperweb/templates/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/js/console.js
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/assets/js/script.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/console.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-15 16:44:35.000000 embykeeper-2.2.1/embykeeperweb/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-15 16:44:35.000000 embykeeper-2.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:44:48.196441 embykeeper-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:44:48.192441 embykeeper-2.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-15 16:44:35.000000 embykeeper-2.2.1/tests/test_cli.py
```

### Comparing `embykeeper-2.2.0/LICENSE` & `embykeeper-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/PKG-INFO` & `embykeeper-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.0
+Version: 2.2.1
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -104,26 +104,22 @@
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = 1080
 scheme = "socks5"
 
 [[telegram]]
-api_id = "27894236"
-api_hash = "622159182fdd4b15b627eeb3ac695271"
 phone = "+8612109347899"
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
-
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
@@ -172,15 +168,15 @@
 
 即可在后台启动 embykeeper.
 
 您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
 ### 从 PyPi 安装
 
-Embykeeper 可以通过 `python >= 3.7, < 3.11` 运行, 您可以通过 [virtualvenv](https://virtualenv.pypa.io/) 进行环境的管理:
+Embykeeper 可以通过 `python >= 3.8, < 3.11` 运行, 您可以通过 [virtualvenv](https://virtualenv.pypa.io/) 进行环境的管理:
 
 ```bash
 python -m venv embykeeper-venv
 . ./embykeeper-venv/bin/activate
 pip install embykeeper
 ```
 
@@ -326,14 +322,15 @@
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
 若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
 若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
 当前支持的名称包括:
+
 | 站点        | 名称       |     | 站点        | 名称          |
 | ----------- | ---------- | --- | ----------- | ------------- |
 | 垃圾影音    | `ljyy`     |     | 搜书神器    | `sosdbot`     |
 | 卷毛鼠 IPTV | `jms_iptv` |     | 终点站      | `terminus`    |
 | Pornemby    | `pornemby` |     | Singularity | `singularity` |
 | Peach       | `peach`    |     | Nebula      | `nebula`      |
 | Bluesea     | `bluesea`  |     | Embyhub     | `embyhub`     |
@@ -347,19 +344,21 @@
 | `port`     | `int`  | 代理端口号                              | `1080`      |
 | `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
 
 `telegram` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                                               | 默认值  |
 | ---------- | ------ | ------------------------------------------------------------------ | ------- |
-| `api_id`   | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
-| `api_hash` | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
 | `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
 | `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
 | `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
+| `api_id`   | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
+| `api_hash` | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
+
+如果您在使用过程中遇到 'API_ID_PUBLISHED_FLOOD' 错误, 您可能需要申请自己的 API, 可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试. 申请后请将 api_id 和 api_hash 填入 telegram 配置中即可.
 
 `emby` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                                      | 默认值 |
 | ---------- | ------ | --------------------------------------------------------- | ------ |
 | `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
 | `username` | `str`  | Emby 服务器用户名                                         |        |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.0 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.1 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
 :: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
@@ -98,26 +98,19 @@
 æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
 ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
 embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
 net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
 `config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
 æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
 ```toml [proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [
-[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
-phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
-"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
-[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
-ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
-è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
-"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
-æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
-éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --
-rm -it --net=host embykeeper/embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+[telegram]] phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/
+" username = "carrie19" password = "s*D7MMCpS$" ``` éå,
+æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
+net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
+ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
 compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
 é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
 %E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
@@ -129,15 +122,15 @@
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
 docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
 watchtower) è¢«ç¨äºèªå¨æ´æ°çæ¬. ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨:
 ```bash docker-compose up -d ``` å³å¯å¨åå°å¯å¨ embykeeper.
 æ¨å¯ä»¥éè¿ `docker logs -f embykeeper` æ `docker-compose logs -
 f embykeeper` ä»¥æ¥çææ°æ¥å¿. ### ä» PyPi å®è£ Embykeeper
-å¯ä»¥éè¿ `python >= 3.7, < 3.11` è¿è¡, æ¨å¯ä»¥éè¿ [virtualvenv]
+å¯ä»¥éè¿ `python >= 3.8, < 3.11` è¿è¡, æ¨å¯ä»¥éè¿ [virtualvenv]
 (https://virtualenv.pypa.io/) è¿è¡ç¯å¢çç®¡ç: ```bash python -m venv
 embykeeper-venv . ./embykeeper-venv/bin/activate pip install embykeeper ```
 éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
 å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
 æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, åè§ [éè¿ Docker é¨ç½²](https://
 github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
@@ -207,22 +200,30 @@
 | | å¡æ | `charon` | `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å |
 ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------------------
 ----- | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
 `localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` | `str`
 | ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
 è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
 ------ | ------------------------------------------------------------------ | -
------- | | `api_id` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/
-)ç³è¯·ç Application ID | | | `api_hash` | `str` | ä»[Telegram å®ç½]
-(https://my.telegram.org/)ç³è¯·ç Application Hash | | | `phone` | `str` |
-è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | | `monitor` | `bool` |
-å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` | `bool` |
-å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹
-| å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | --------------------
-------------------------------------- | ------ | | `url` | `str` | Emby
+------ | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | |
+`monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` |
+`bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | | `api_id` | `str` |
+(å¯é) ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID
+| | | `api_hash` | `str` | (å¯é) ä»[Telegram å®ç½](https://
+my.telegram.org/)ç³è¯·ç Application Hash | |
+å¦ææ¨å¨ä½¿ç¨è¿ç¨ä¸­éå° 'API_ID_PUBLISHED_FLOOD' éè¯¯,
+æ¨å¯è½éè¦ç³è¯·èªå·±ç API, å¯ä»¥éè¿ [Telegram å®ç½](https://
+my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
+development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
+æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
+æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
+æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. ç³è¯·åè¯·å° api_id å
+api_hash å¡«å¥ telegram éç½®ä¸­å³å¯. `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
+å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
+----------------------------------- | ------ | | `url` | `str` | Emby
 æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
 | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
 æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
 bgk, embyhub, polo unique_name = "your_username_for_registeration" #
 èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
```

### Comparing `embykeeper-2.2.0/README.md` & `embykeeper-2.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -84,26 +84,22 @@
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = 1080
 scheme = "socks5"
 
 [[telegram]]
-api_id = "27894236"
-api_hash = "622159182fdd4b15b627eeb3ac695271"
 phone = "+8612109347899"
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
-
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
@@ -152,15 +148,15 @@
 
 即可在后台启动 embykeeper.
 
 您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
 ### 从 PyPi 安装
 
-Embykeeper 可以通过 `python >= 3.7, < 3.11` 运行, 您可以通过 [virtualvenv](https://virtualenv.pypa.io/) 进行环境的管理:
+Embykeeper 可以通过 `python >= 3.8, < 3.11` 运行, 您可以通过 [virtualvenv](https://virtualenv.pypa.io/) 进行环境的管理:
 
 ```bash
 python -m venv embykeeper-venv
 . ./embykeeper-venv/bin/activate
 pip install embykeeper
 ```
 
@@ -306,14 +302,15 @@
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
 若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
 若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
 当前支持的名称包括:
+
 | 站点        | 名称       |     | 站点        | 名称          |
 | ----------- | ---------- | --- | ----------- | ------------- |
 | 垃圾影音    | `ljyy`     |     | 搜书神器    | `sosdbot`     |
 | 卷毛鼠 IPTV | `jms_iptv` |     | 终点站      | `terminus`    |
 | Pornemby    | `pornemby` |     | Singularity | `singularity` |
 | Peach       | `peach`    |     | Nebula      | `nebula`      |
 | Bluesea     | `bluesea`  |     | Embyhub     | `embyhub`     |
@@ -327,19 +324,21 @@
 | `port`     | `int`  | 代理端口号                              | `1080`      |
 | `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
 
 `telegram` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                                               | 默认值  |
 | ---------- | ------ | ------------------------------------------------------------------ | ------- |
-| `api_id`   | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
-| `api_hash` | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
 | `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
 | `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
 | `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
+| `api_id`   | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
+| `api_hash` | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
+
+如果您在使用过程中遇到 'API_ID_PUBLISHED_FLOOD' 错误, 您可能需要申请自己的 API, 可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试. 申请后请将 api_id 和 api_hash 填入 telegram 配置中即可.
 
 `emby` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                                      | 默认值 |
 | ---------- | ------ | --------------------------------------------------------- | ------ |
 | `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
 | `username` | `str`  | Emby 服务器用户名                                         |        |
```

#### html2text {}

```diff
@@ -87,26 +87,19 @@
 æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
 ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
 embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
 net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
 `config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
 æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
 ```toml [proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [
-[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
-phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
-"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
-[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
-ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
-è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
-"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
-æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
-éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --
-rm -it --net=host embykeeper/embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+[telegram]] phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/
+" username = "carrie19" password = "s*D7MMCpS$" ``` éå,
+æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
+net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
+ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
 compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
 é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
 %E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
@@ -118,15 +111,15 @@
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
 docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
 watchtower) è¢«ç¨äºèªå¨æ´æ°çæ¬. ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨:
 ```bash docker-compose up -d ``` å³å¯å¨åå°å¯å¨ embykeeper.
 æ¨å¯ä»¥éè¿ `docker logs -f embykeeper` æ `docker-compose logs -
 f embykeeper` ä»¥æ¥çææ°æ¥å¿. ### ä» PyPi å®è£ Embykeeper
-å¯ä»¥éè¿ `python >= 3.7, < 3.11` è¿è¡, æ¨å¯ä»¥éè¿ [virtualvenv]
+å¯ä»¥éè¿ `python >= 3.8, < 3.11` è¿è¡, æ¨å¯ä»¥éè¿ [virtualvenv]
 (https://virtualenv.pypa.io/) è¿è¡ç¯å¢çç®¡ç: ```bash python -m venv
 embykeeper-venv . ./embykeeper-venv/bin/activate pip install embykeeper ```
 éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
 å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
 æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, åè§ [éè¿ Docker é¨ç½²](https://
 github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
@@ -196,22 +189,30 @@
 | | å¡æ | `charon` | `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å |
 ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------------------
 ----- | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
 `localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` | `str`
 | ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
 è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
 ------ | ------------------------------------------------------------------ | -
------- | | `api_id` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/
-)ç³è¯·ç Application ID | | | `api_hash` | `str` | ä»[Telegram å®ç½]
-(https://my.telegram.org/)ç³è¯·ç Application Hash | | | `phone` | `str` |
-è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | | `monitor` | `bool` |
-å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` | `bool` |
-å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹
-| å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | --------------------
-------------------------------------- | ------ | | `url` | `str` | Emby
+------ | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | |
+`monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` |
+`bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | | `api_id` | `str` |
+(å¯é) ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID
+| | | `api_hash` | `str` | (å¯é) ä»[Telegram å®ç½](https://
+my.telegram.org/)ç³è¯·ç Application Hash | |
+å¦ææ¨å¨ä½¿ç¨è¿ç¨ä¸­éå° 'API_ID_PUBLISHED_FLOOD' éè¯¯,
+æ¨å¯è½éè¦ç³è¯·èªå·±ç API, å¯ä»¥éè¿ [Telegram å®ç½](https://
+my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
+development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
+æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
+æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
+æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. ç³è¯·åè¯·å° api_id å
+api_hash å¡«å¥ telegram éç½®ä¸­å³å¯. `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
+å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
+----------------------------------- | ------ | | `url` | `str` | Emby
 æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
 | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
 æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
 bgk, embyhub, polo unique_name = "your_username_for_registeration" #
 èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
```

### Comparing `embykeeper-2.2.0/embykeeper/cli.py` & `embykeeper-2.2.1/embykeeper/cli.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/data.py` & `embykeeper-2.2.1/embykeeper/data.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/embywatcher/emby.py` & `embykeeper-2.2.1/embykeeper/embywatcher/emby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/embywatcher/main.py` & `embykeeper-2.2.1/embykeeper/embywatcher/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,18 @@
                             return False
                         else:
                             logger.info(f"连接失败, 正在重试.")
                     except PlayError as e:
                         logger.info(f"发生错误: {e}, 正在重试其他视频.")
                         break
                     finally:
-                        if not await hide_from_resume(obj):
+                        try:
+                            if not await asyncio.shield(asyncio.wait_for(hide_from_resume(obj), 0.5)):
+                                logger.debug(f"未能成功从最近播放中隐藏视频.")
+                        except asyncio.TimeoutError:
                             logger.debug(f"未能成功从最近播放中隐藏视频.")
             else:
                 logger.warning(f"由于没有成功播放视频, 保活失败, 请重新检查配置.")
                 return False
         except (ClientError, OSError):
             retry += 1
             if retry > retries:
```

### Comparing `embykeeper-2.2.0/embykeeper/log.py` & `embykeeper-2.2.1/embykeeper/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/settings.py` & `embykeeper-2.2.1/embykeeper/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 import base64
 import hashlib
 
 from loguru import logger
 import tomli as tomllib
 from schema import And, Optional, Or, Regex, Schema, SchemaError
 
+PUBLISHED_API = {
+    "nicegram": {"api_id": "94575", "api_hash": "a3406de8d171bb422bb6ddf3bbd800e2"},
+    "android": {"api_id": "6", "api_hash": "eb06d4abfb49dc3eeb1aeb98ae0f581e"},
+    "ios": {"api_id": "94575", "api_hash": "a3406de8d171bb422bb6ddf3bbd800e2"},
+}
+
 
 def check_config(config):
     PositiveInt = lambda: And(int, lambda n: n > 0)
     schema = Schema(
         {
             Optional("timeout"): PositiveInt(),
             Optional("retries"): PositiveInt(),
@@ -34,19 +40,19 @@
                     Optional("monitor"): [str],
                     Optional("messager"): [str],
                 }
             ),
             Optional("telegram"): [
                 Schema(
                     {
-                        "api_id": Regex(r"^\d+$"),
-                        "api_hash": Regex(r"^[a-z0-9]+$"),
                         "phone": str,
                         Optional("monitor"): bool,
                         Optional("send"): bool,
+                        Optional("api_id"): Regex(r"^\d+$"),
+                        Optional("api_hash"): Regex(r"^[a-z0-9]+$"),
                     }
                 )
             ],
             Optional("emby"): [
                 Schema(
                     {
                         "url": Regex(
@@ -134,23 +140,19 @@
         doc.add(comment(line))
     doc.add(nl())
     doc.add(comment("Telegram 账号设置, 您可以重复该片段多次以增加多个账号."))
     telegram = []
     for _ in range(2):
         t = item(
             {
-                "api_id": fake.numerify(text="########"),
-                "api_hash": uuid.uuid4().hex,
                 "phone": f'+861{fake.numerify(text="##########")}',
                 "send": False,
                 "monitor": False,
             }
         )
-        t["api_id"].comment("通过 Telegram 官网申请 API: https://my.telegram.org/")
-        t["api_hash"].comment("通过 Telegram 官网申请 API: https://my.telegram.org/")
         telegram.append(t)
     doc["telegram"] = telegram
     for t in doc["telegram"]:
         t.value.item("send").comment("启用该账号的自动水群功能 (谨慎使用)")
         t.value.item("monitor").comment("启用该账号的自动监控功能 (需要高级账号)")
     doc.add(nl())
     doc.add(comment("Emby 账号设置, 您可以重复该片段多次以增加多个账号."))
@@ -226,20 +228,16 @@
                 )
                 logger.info(
                     "(登陆后选择 API development tools, 随后应用信息可以随意填写, 若提示Error您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试)"
                 )
         if not more:
             break
         phone = Prompt.ask(pad + "请输入您的 Telegram 账号 (带国家区号) [dark_green](+861xxxxxxxxxx)[/]")
-        api_id = Prompt.ask(pad + "请输入您的 Telegram api_id")
-        api_hash = Prompt.ask(pad + "请输入您的 Telegram api_hash")
         monitor = Confirm.ask(pad + "是否开启该账号的自动监控功能? (需要高级账号)", default=False)
-        telegrams.append(
-            {"phone": phone, "api_id": api_id, "api_hash": api_hash, "send": False, "monitor": monitor}
-        )
+        telegrams.append({"phone": phone, "send": False, "monitor": monitor})
     embies = config.get("emby", [])
     while True:
         if len(embies) > 0:
             logger.info(f"您当前填写了 {len(embies)} 个 Emby 账号信息.")
             more = Confirm.ask(pad + "是否继续添加?", default=False)
         else:
             more = Confirm.ask(pad + "是否添加 Emby 账号?", default=True)
@@ -287,14 +285,15 @@
         content = content.encode()
     content = base64.b64encode(content)
     logger.info(f"您的配置[green]已生成完毕[/]! 您需要将以下内容写入 SECRETS 变量配置 (名称: EK_CONFIG), 否则配置将在重启后丢失.")
     print()
     get_console().rule("EK_CONFIG")
     print(content.decode())
     get_console().rule()
+    print()
     start_now = Confirm.ask(pad + "是否立即启动?", default=True)
     if start_now:
         return config
 
 
 def load_env_config(data: str):
     from rich.prompt import Prompt
@@ -367,8 +366,11 @@
         logger.error(f"配置文件错误, 请检查配置文件:\n{error}.")
         sys.exit(253)
     proxy: dict = config.get("proxy", None)
     if proxy:
         proxy.setdefault("scheme", "socks5")
         proxy.setdefault("hostname", "127.0.0.1")
         proxy.setdefault("port", 1080)
+    for tg in config.get("telegram", []):
+        if tg.get("api_id", None) is None and tg.get("api_hash", None) is None:
+            tg.update(PUBLISHED_API["nicegram"])
     return config
```

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/bots/base.py` & `embykeeper-2.2.1/embykeeper/telechecker/bots/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,25 +178,29 @@
                     await self.send_checkin()
                 try:
                     await asyncio.wait_for(self.finished.wait(), self.timeout)
                 except asyncio.TimeoutError:
                     pass
                 finally:
                     if self._is_archived:
-                        self.log.debug(f"[gray50]将会话重新归档: {bot.username}[/]")
+                        self.log.debug(f"[gray50]将会话重新归档: {ident}[/]")
                         try:
-                            await asyncio.shield(asyncio.wait_for(chat.archive(), 0.5))
+                            await asyncio.shield(asyncio.wait_for(chat.archive(), 3))
                         except asyncio.TimeoutError:
-                            pass
+                            self.log.debug(f"[gray50]归档失败: {ident}[/]")
         except OSError as e:
             self.log.warning(f'初始化错误: "{e}".')
             return False
         finally:
             if not self.chat_name:
-                await self.client.read_chat_history(ident)
+                self.log.debug(f"[gray50]将会话设为已读: {ident}[/]")
+                try:
+                    await asyncio.shield(asyncio.wait_for(self.client.read_chat_history(ident), 3))
+                except asyncio.TimeoutError:
+                    self.log.debug(f"[gray50]设为已读失败: {ident}[/]")
         if not self.finished.is_set():
             self.log.warning("无法在时限内完成签到.")
             return False
         else:
             return self._retries <= self.retries
 
     async def walk_history(self, limit=0):
```

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/bots/charon.py` & `embykeeper-2.2.1/embykeeper/telechecker/bots/charon.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/bots/jms.py` & `embykeeper-2.2.1/embykeeper/telechecker/bots/jms.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/bots/nebula.py` & `embykeeper-2.2.1/embykeeper/telechecker/bots/nebula.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/bots/peach.py` & `embykeeper-2.2.1/embykeeper/telechecker/bots/peach.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/bots/pornemby.py` & `embykeeper-2.2.1/embykeeper/telechecker/bots/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/bots/singularity.py` & `embykeeper-2.2.1/embykeeper/telechecker/bots/singularity.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/link.py` & `embykeeper-2.2.1/embykeeper/telechecker/link.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/log.py` & `embykeeper-2.2.1/embykeeper/telechecker/log.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/main.py` & `embykeeper-2.2.1/embykeeper/telechecker/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,21 +167,24 @@
             tasks = []
             names = []
             for c in checkiners:
                 names.append(c.name)
                 wait = 0 if instant else random.randint(0, 60 * config.get("random", 15))
                 task = asyncio.create_task(checkin_task(c, sem, wait))
                 tasks.append(task)
-            coros.append(gather_task(tasks, username=tg.me.name))
+            coros.append(asyncio.ensure_future(gather_task(tasks, username=tg.me.name)))
             if names:
                 log.debug(f'已启用签到器: {", ".join(names)}')
         while coros:
             done, coros = await asyncio.wait(coros, return_when=asyncio.FIRST_COMPLETED)
             for t in done:
-                username, results = await t
+                try:
+                    username, results = await t
+                except asyncio.CancelledError:
+                    continue
                 log = logger.bind(scheme="telechecker", username=username)
                 failed = []
                 ignored = []
                 successful = []
                 for i, c in enumerate(checkiners):
                     if results[i] == False:
                         failed.append(c)
```

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/messager/base.py` & `embykeeper-2.2.1/embykeeper/telechecker/messager/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/messager/common.py` & `embykeeper-2.2.1/embykeeper/telechecker/messager/common.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/monitor/base.py` & `embykeeper-2.2.1/embykeeper/telechecker/monitor/base.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/monitor/bgk.py` & `embykeeper-2.2.1/embykeeper/telechecker/monitor/bgk.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/monitor/embyhub.py` & `embykeeper-2.2.1/embykeeper/telechecker/monitor/embyhub.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/monitor/misty.py` & `embykeeper-2.2.1/embykeeper/telechecker/monitor/misty.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/monitor/polo.py` & `embykeeper-2.2.1/embykeeper/telechecker/monitor/polo.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/monitor/pornemby.py` & `embykeeper-2.2.1/embykeeper/telechecker/monitor/pornemby.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/monitor/test.py` & `embykeeper-2.2.1/embykeeper/telechecker/monitor/test.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/monitor/viper.py` & `embykeeper-2.2.1/embykeeper/telechecker/monitor/viper.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/telechecker/tele.py` & `embykeeper-2.2.1/embykeeper/telechecker/tele.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper/utils.py` & `embykeeper-2.2.1/embykeeper/utils.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeper.egg-info/PKG-INFO` & `embykeeper-2.2.1/embykeeper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embykeeper
-Version: 2.2.0
+Version: 2.2.1
 Summary: Daily checkin automator for emby bots in telegram.
 Author-email: jackzzs <jackzzs@outlook.com>
 Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -104,26 +104,22 @@
 ```toml
 [proxy]
 hostname = "127.0.0.1"
 port = 1080
 scheme = "socks5"
 
 [[telegram]]
-api_id = "27894236"
-api_hash = "622159182fdd4b15b627eeb3ac695271"
 phone = "+8612109347899"
 
 [[emby]]
 url = "https://weiss-griffin.com/"
 username = "carrie19"
 password = "s*D7MMCpS$"
 ```
 
-对于 Telegram 而言, 您可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试.
-
 随后, 您需要再次执行:
 
 ```bash
 docker run -v $(pwd)/embykeeper:/app --rm -it --net=host embykeeper/embykeeper
 ```
 
 您将被询问设备验证码以登录, 登录成功后, Embykeeper 将首先执行一次签到和保活, 然后启动群组监控和水群计划任务 (若启用).
@@ -172,15 +168,15 @@
 
 即可在后台启动 embykeeper.
 
 您可以通过 `docker logs -f embykeeper` 或 `docker-compose logs -f embykeeper` 以查看最新日志.
 
 ### 从 PyPi 安装
 
-Embykeeper 可以通过 `python >= 3.7, < 3.11` 运行, 您可以通过 [virtualvenv](https://virtualenv.pypa.io/) 进行环境的管理:
+Embykeeper 可以通过 `python >= 3.8, < 3.11` 运行, 您可以通过 [virtualvenv](https://virtualenv.pypa.io/) 进行环境的管理:
 
 ```bash
 python -m venv embykeeper-venv
 . ./embykeeper-venv/bin/activate
 pip install embykeeper
 ```
 
@@ -326,14 +322,15 @@
 | `monitor`   | `list` | 启用的监视会话 | (当前所有支持的会话) |
 | `messager`  | `list` | 启用的水群会话 | (当前所有支持的会话) |
 
 注意, 当您未曾与站点机器人对话, 该站点签到将不会运行.
 若您需要禁用部分签到站点, 您可以在列表中删除对应的名称.
 若您需要使用默认禁用的签到站点, 您可以在列表中增加对应的名称.
 当前支持的名称包括:
+
 | 站点        | 名称       |     | 站点        | 名称          |
 | ----------- | ---------- | --- | ----------- | ------------- |
 | 垃圾影音    | `ljyy`     |     | 搜书神器    | `sosdbot`     |
 | 卷毛鼠 IPTV | `jms_iptv` |     | 终点站      | `terminus`    |
 | Pornemby    | `pornemby` |     | Singularity | `singularity` |
 | Peach       | `peach`    |     | Nebula      | `nebula`      |
 | Bluesea     | `bluesea`  |     | Embyhub     | `embyhub`     |
@@ -347,19 +344,21 @@
 | `port`     | `int`  | 代理端口号                              | `1080`      |
 | `scheme`   | `str`  | 代理协议, 可以为 "`socks5`" 或 "`http`" | `socks5`    |
 
 `telegram` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                                               | 默认值  |
 | ---------- | ------ | ------------------------------------------------------------------ | ------- |
-| `api_id`   | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
-| `api_hash` | `str`  | 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
 | `phone`    | `str`  | 账户手机号, 一般为 "`+86...`"                                      |         |
 | `monitor`  | `bool` | 启用群组监控系列功能                                               | `false` |
 | `send`     | `bool` | 启用自动水群系列功能                                               | `false` |
+| `api_id`   | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application ID   |         |
+| `api_hash` | `str`  | (可选) 从[Telegram 官网](https://my.telegram.org/)申请的 Application Hash |         |
+
+如果您在使用过程中遇到 'API_ID_PUBLISHED_FLOOD' 错误, 您可能需要申请自己的 API, 可以通过 [Telegram 官网](https://my.telegram.org/) 申请 `api_id` 和 `api_hash`. 登陆后选择 `API development tools`, 随后应用信息可以随意填写, 请注意 `URL` 是必填项, 可以填写 `localhost`. 提交时若显示 "Error", 您可能需要再次多次点击提交, 或等待新账户脱离风控期/更换代理/清除浏览器记录并重试. 申请后请将 api_id 和 api_hash 填入 telegram 配置中即可.
 
 `emby` 设置可以为:
 
 | 设置项     | 值类型 | 简介                                                      | 默认值 |
 | ---------- | ------ | --------------------------------------------------------- | ------ |
 | `url`      | `str`  | Emby 服务器地址, 一般为 "`https://...`" 或 "`http://...`" |        |
 | `username` | `str`  | Emby 服务器用户名                                         |        |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: embykeeper Version: 2.2.0 Summary: Daily checkin
+Metadata-Version: 2.1 Name: embykeeper Version: 2.2.1 Summary: Daily checkin
 automator for emby bots in telegram. Author-email: jackzzs
 outlook.com> Project-URL: Homepage, https://github.com/embykeeper/embykeeper
 Keywords: emby,telegram,checkin,automator,bot,telegram bot,keep active
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop Classifier: Natural Language
 :: Chinese (Simplified) Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Programming Language :: Python :: 3
@@ -98,26 +98,19 @@
 æ¨é [å®è£ docker](https://yeasy.gitbook.io/docker_practice/install),
 ç¶åæ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --net=host
 embykeeper/embykeeper ``` (è¥æ¨ä¸éè¦è¿æ¥æ¬æºä»£ç, å¯ä»¥å»é¤ '--
 net=host' åæ°) å½ä»¤å°ä¼å¨ `embykeeper` ç®å½ä¸çææ¨¡æ¿
 `config.toml` æä»¶, æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯,
 æ¨ä¹å¯ä»¥ä½¿ç¨æå°éç½® (ä»¥ä¸ææä¿¡æ¯ä¸ºçæ, ä»ååè):
 ```toml [proxy] hostname = "127.0.0.1" port = 1080 scheme = "socks5" [
-[telegram]] api_id = "27894236" api_hash = "622159182fdd4b15b627eeb3ac695271"
-phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/" username =
-"carrie19" password = "s*D7MMCpS$" ``` å¯¹äº Telegram èè¨, æ¨å¯ä»¥éè¿
-[Telegram å®ç½](https://my.telegram.org/) ç³è¯· `api_id` å `api_hash`.
-ç»éåéæ© `API development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å,
-è¯·æ³¨æ `URL` æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º
-"Error", æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤,
-æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯.
-éå, æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --
-rm -it --net=host embykeeper/embykeeper ```
-æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½, ç»å½æåå, Embykeeper
-å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
+[telegram]] phone = "+8612109347899" [[emby]] url = "https://weiss-griffin.com/
+" username = "carrie19" password = "s*D7MMCpS$" ``` éå,
+æ¨éè¦åæ¬¡æ§è¡: ```bash docker run -v $(pwd)/embykeeper:/app --rm -it --
+net=host embykeeper/embykeeper ``` æ¨å°è¢«è¯¢é®è®¾å¤éªè¯ç ä»¥ç»å½,
+ç»å½æåå, Embykeeper å°é¦åæ§è¡ä¸æ¬¡ç­¾å°åä¿æ´»,
 ç¶åå¯å¨ç¾¤ç»çæ§åæ°´ç¾¤è®¡åä»»å¡ (è¥å¯ç¨).
 æ­åæ¨ï¼æ¨å·²ç»æåé¨ç½²äº Embykeeper. å½æ¨éè¦æ´æ°çæ¬æ¶,
 æ¨éè¦æ§è¡: ```bash docker pull embykeeper/embykeeper ``` ### éè¿
 Docker Compose é¨ç½² æ¨å¯ä»¥ä½¿ç¨ [docker-compose](https://docs.docker.com/
 compose/) é¨ç½² Embykeeper. **æ³¨æ**: æ¨éè¦åè¿è¡è¿ [éè¿ Docker
 é¨ç½²](https://github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-
 %E9%83%A8%E7%BD%B2) æè½éè¿ `docker-compose` é¨ç½²,
@@ -129,15 +122,15 @@
 network_mode: host watchtower: container_name: watchtower image: containrrr/
 watchtower restart: unless-stopped volumes: - /var/run/docker.sock:/var/run/
 docker.sock:rw ``` å¶ä¸­, [watchtower](https://github.com/containrrr/
 watchtower) è¢«ç¨äºèªå¨æ´æ°çæ¬. ç¶åè¿è¡ä»¥ä¸å½ä»¤ä»¥å¯å¨:
 ```bash docker-compose up -d ``` å³å¯å¨åå°å¯å¨ embykeeper.
 æ¨å¯ä»¥éè¿ `docker logs -f embykeeper` æ `docker-compose logs -
 f embykeeper` ä»¥æ¥çææ°æ¥å¿. ### ä» PyPi å®è£ Embykeeper
-å¯ä»¥éè¿ `python >= 3.7, < 3.11` è¿è¡, æ¨å¯ä»¥éè¿ [virtualvenv]
+å¯ä»¥éè¿ `python >= 3.8, < 3.11` è¿è¡, æ¨å¯ä»¥éè¿ [virtualvenv]
 (https://virtualenv.pypa.io/) è¿è¡ç¯å¢çç®¡ç: ```bash python -m venv
 embykeeper-venv . ./embykeeper-venv/bin/activate pip install embykeeper ```
 éå, æ¨éè¦æ§è¡: ```bash embykeeper ```
 å½ä»¤å°ä¼å¨å½åç®å½çææ¨¡æ¿ `config.toml` æä»¶,
 æ¨éè¦éç½®æ¨çè´¦æ·ä¿¡æ¯, åè§ [éè¿ Docker é¨ç½²](https://
 github.com/embykeeper/embykeeper#%E9%80%9A%E8%BF%87-docker-%E9%83%A8%E7%BD%B2).
 éå, æ¨éè¦åæ¬¡æ§è¡: ```bash embykeeper ```
@@ -207,22 +200,30 @@
 | | å¡æ | `charon` | `proxy` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å |
 ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------------------
 ----- | ----------- | | `hostname` | `str` | ä»£çæå¡å¨å°å |
 `localhost` | | `port` | `int` | ä»£çç«¯å£å· | `1080` | | `scheme` | `str`
 | ä»£çåè®®, å¯ä»¥ä¸º "`socks5`" æ "`http`" | `socks5` | `telegram`
 è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ | å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- |
 ------ | ------------------------------------------------------------------ | -
------- | | `api_id` | `str` | ä»[Telegram å®ç½](https://my.telegram.org/
-)ç³è¯·ç Application ID | | | `api_hash` | `str` | ä»[Telegram å®ç½]
-(https://my.telegram.org/)ç³è¯·ç Application Hash | | | `phone` | `str` |
-è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | | `monitor` | `bool` |
-å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` | `bool` |
-å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹
-| å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | --------------------
-------------------------------------- | ------ | | `url` | `str` | Emby
+------ | | `phone` | `str` | è´¦æ·ææºå·, ä¸è¬ä¸º "`+86...`" | | |
+`monitor` | `bool` | å¯ç¨ç¾¤ç»çæ§ç³»ååè½ | `false` | | `send` |
+`bool` | å¯ç¨èªå¨æ°´ç¾¤ç³»ååè½ | `false` | | `api_id` | `str` |
+(å¯é) ä»[Telegram å®ç½](https://my.telegram.org/)ç³è¯·ç Application ID
+| | | `api_hash` | `str` | (å¯é) ä»[Telegram å®ç½](https://
+my.telegram.org/)ç³è¯·ç Application Hash | |
+å¦ææ¨å¨ä½¿ç¨è¿ç¨ä¸­éå° 'API_ID_PUBLISHED_FLOOD' éè¯¯,
+æ¨å¯è½éè¦ç³è¯·èªå·±ç API, å¯ä»¥éè¿ [Telegram å®ç½](https://
+my.telegram.org/) ç³è¯· `api_id` å `api_hash`. ç»éåéæ© `API
+development tools`, éååºç¨ä¿¡æ¯å¯ä»¥éæå¡«å, è¯·æ³¨æ `URL`
+æ¯å¿å¡«é¡¹, å¯ä»¥å¡«å `localhost`. æäº¤æ¶è¥æ¾ç¤º "Error",
+æ¨å¯è½éè¦åæ¬¡å¤æ¬¡ç¹å»æäº¤, æç­å¾æ°è´¦æ·è±ç¦»é£æ§æ/
+æ´æ¢ä»£ç/æ¸é¤æµè§å¨è®°å½å¹¶éè¯. ç³è¯·åè¯·å° api_id å
+api_hash å¡«å¥ telegram éç½®ä¸­å³å¯. `emby` è®¾ç½®å¯ä»¥ä¸º: | è®¾ç½®é¡¹ |
+å¼ç±»å | ç®ä» | é»è®¤å¼ | | ---------- | ------ | ----------------------
+----------------------------------- | ------ | | `url` | `str` | Emby
 æå¡å¨å°å, ä¸è¬ä¸º "`https://...`" æ "`http://...`" | | | `username`
 | `str` | Emby æå¡å¨ç¨æ·å | | | `password` | `str` | Emby
 æå¡å¨å¯ç  | | | `time` | `int` | æ¨¡æè§ççæ¶é´ (ç§) | `800` | |
 `progress` | `int` | è§çåæ¨¡æè¿åº¦æ¡ä¿å­çæ¶é´ (ç§) | `1000` |
 æå¡å¯ä»¥è¿è¡ç¹å®éç½®, å¦ä¸æç¤º: ```toml [monitor.bgk] # æ¯æ
 bgk, embyhub, polo unique_name = "your_username_for_registeration" #
 èªå¨æ¢æ³¨æ¶ä½¿ç¨çç¨æ·å [monitor.pornemby] only_history = true #
```

### Comparing `embykeeper-2.2.0/embykeeper.egg-info/SOURCES.txt` & `embykeeper-2.2.1/embykeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/app.py` & `embykeeper-2.2.1/embykeeperweb/app.py`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/404.html` & `embykeeper-2.2.1/embykeeperweb/templates/404.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css` & `embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js` & `embykeeper-2.2.1/embykeeperweb/templates/assets/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/assets/css/icons.css` & `embykeeper-2.2.1/embykeeperweb/templates/assets/css/icons.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/assets/css/styles.css` & `embykeeper-2.2.1/embykeeperweb/templates/assets/css/styles.css`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/404.svg` & `embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/404.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/login.svg` & `embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/login.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/assets/img/illustrations/logo-only.svg` & `embykeeper-2.2.1/embykeeperweb/templates/assets/img/illustrations/logo-only.svg`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/assets/js/console.js` & `embykeeper-2.2.1/embykeeperweb/templates/assets/js/console.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/assets/js/script.js` & `embykeeper-2.2.1/embykeeperweb/templates/assets/js/script.js`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/console.html` & `embykeeper-2.2.1/embykeeperweb/templates/console.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/embykeeperweb/templates/login.html` & `embykeeper-2.2.1/embykeeperweb/templates/login.html`

 * *Files identical despite different names*

### Comparing `embykeeper-2.2.0/pyproject.toml` & `embykeeper-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "embykeeper"
-version = "2.2.0"
+version = "2.2.1"
 authors = [
     {name = "jackzzs", email = "jackzzs@outlook.com"},
 ]
 description = "Daily checkin automator for emby bots in telegram."
 keywords = [
     "emby",
     "telegram",
```

### Comparing `embykeeper-2.2.0/tests/test_cli.py` & `embykeeper-2.2.1/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,12 +67,12 @@
 
 def test_check_config(in_temp_dir: Path):
     with open("config.toml", "w+") as f:
         f.write("notifier: true")
     result = runner.invoke(app)
     assert result.exit_code == 252
 
-    config = {"telegram": {k: "Test" for k in ("api_id", "api_hash", "phone")}}
+    config = {"telegram": {"phone": "Test"}}
     with open("config.toml", "w+") as f:
         tomlkit.dump(config, f)
     result = runner.invoke(app)
     assert result.exit_code == 253
```

