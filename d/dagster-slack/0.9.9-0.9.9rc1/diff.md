# Comparing `tmp/dagster-slack-0.9.9.tar.gz` & `tmp/dagster-slack-0.9.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dagster-slack-0.9.9.tar", last modified: Thu Sep 17 21:27:24 2020, max compression
+gzip compressed data, was "dist/dagster-slack-0.9.9rc1.tar", last modified: Thu Sep 17 21:08:49 2020, max compression
```

## Comparing `dagster-slack-0.9.9.tar` & `dagster-slack-0.9.9rc1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/
--rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/LICENSE
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/MANIFEST.in
--rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/README.md
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/dagster_slack/
--rw-r--r--   0 bobchen    (501) staff       (20)      224 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/dagster_slack/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     2865 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/dagster_slack/resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       22 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/dagster_slack/version.py
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/dagster_slack.egg-info/
--rw-r--r--   0 bobchen    (501) staff       (20)      580 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/dagster_slack.egg-info/PKG-INFO
--rw-r--r--   0 bobchen    (501) staff       (20)      452 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/dagster_slack.egg-info/SOURCES.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/dagster_slack.egg-info/dependency_links.txt
--rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/dagster_slack.egg-info/not-zip-safe
--rw-r--r--   0 bobchen    (501) staff       (20)       26 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/dagster_slack.egg-info/requires.txt
--rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/dagster_slack.egg-info/top_level.txt
-drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/dagster_slack_tests/
--rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/dagster_slack_tests/__init__.py
--rw-r--r--   0 bobchen    (501) staff       (20)     1068 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/dagster_slack_tests/test_resources.py
--rw-r--r--   0 bobchen    (501) staff       (20)       91 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/dagster_slack_tests/test_version.py
--rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:27:24.000000 dagster-slack-0.9.9/setup.cfg
--rw-r--r--   0 bobchen    (501) staff       (20)     1236 2020-09-17 21:24:45.000000 dagster-slack-0.9.9/setup.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/
+-rw-r--r--   0 bobchen    (501) staff       (20)    11357 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/LICENSE
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/MANIFEST.in
+-rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      125 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/README.md
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack/
+-rw-r--r--   0 bobchen    (501) staff       (20)      224 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     2865 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack/resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       27 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack/version.py
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/
+-rw-r--r--   0 bobchen    (501) staff       (20)      583 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/PKG-INFO
+-rw-r--r--   0 bobchen    (501) staff       (20)      452 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)        1 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/not-zip-safe
+-rw-r--r--   0 bobchen    (501) staff       (20)       26 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/requires.txt
+-rw-r--r--   0 bobchen    (501) staff       (20)       34 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack.egg-info/top_level.txt
+drwxr-xr-x   0 bobchen    (501) staff       (20)        0 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/dagster_slack_tests/
+-rw-r--r--   0 bobchen    (501) staff       (20)        0 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack_tests/__init__.py
+-rw-r--r--   0 bobchen    (501) staff       (20)     1068 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack_tests/test_resources.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       91 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/dagster_slack_tests/test_version.py
+-rw-r--r--   0 bobchen    (501) staff       (20)       74 2020-09-17 21:08:49.000000 dagster-slack-0.9.9rc1/setup.cfg
+-rw-r--r--   0 bobchen    (501) staff       (20)     1236 2020-09-17 21:04:59.000000 dagster-slack-0.9.9rc1/setup.py
```

### Comparing `dagster-slack-0.9.9/LICENSE` & `dagster-slack-0.9.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-slack-0.9.9/PKG-INFO` & `dagster-slack-0.9.9rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-slack
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Slack client resource for posting to Slack
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-slack
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-slack-0.9.9/dagster_slack/resources.py` & `dagster-slack-0.9.9rc1/dagster_slack/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-slack-0.9.9/dagster_slack.egg-info/PKG-INFO` & `dagster-slack-0.9.9rc1/dagster_slack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: dagster-slack
-Version: 0.9.9
+Version: 0.9.9rc1
 Summary: A Slack client resource for posting to Slack
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-slack
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `dagster-slack-0.9.9/dagster_slack_tests/test_resources.py` & `dagster-slack-0.9.9rc1/dagster_slack_tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-slack-0.9.9/setup.py` & `dagster-slack-0.9.9rc1/setup.py`

 * *Files identical despite different names*

