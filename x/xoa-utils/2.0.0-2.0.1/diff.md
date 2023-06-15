# Comparing `tmp/xoa-utils-2.0.0.tar.gz` & `tmp/xoa-utils-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-utils-2.0.0.tar", last modified: Thu Jun 15 09:57:01 2023, max compression
+gzip compressed data, was "xoa-utils-2.0.1.tar", last modified: Thu Jun 15 14:11:14 2023, max compression
```

## Comparing `xoa-utils-2.0.0.tar` & `xoa-utils-2.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-15 09:56:49.000000 xoa-utils-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-15 09:56:49.000000 xoa-utils-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.529770 xoa-utils-2.0.0/xoa_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.533770 xoa-utils-2.0.0/xoa_utils/clicks/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.533770 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/an.py
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/anlt.py
--rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/lt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_commands/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clicks/click_help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/clis/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/clis/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/cmds/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/cmds/cmd_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/cmds/cmd_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/hub/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.537771 xoa-utils-2.0.0/xoa_utils/ssh_server/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/ssh_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 09:56:50.000000 xoa-utils-2.0.0/xoa_utils/ssh_server/xena_ssh_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 09:57:01.533770 xoa-utils-2.0.0/xoa_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 09:57:01.000000 xoa-utils-2.0.0/xoa_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.815502 xoa-utils-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-15 14:11:14.815502 xoa-utils-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 14:11:14.815502 xoa-utils-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.811502 xoa-utils-2.0.1/xoa_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.811502 xoa-utils-2.0.1/xoa_utils/clicks/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/click_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.811502 xoa-utils-2.0.1/xoa_utils/clicks/click_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/click_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/click_commands/an.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/click_commands/anlt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27448 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/click_commands/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/click_commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/click_commands/lt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/click_commands/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clicks/click_help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.815502 xoa-utils-2.0.1/xoa_utils/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/clis/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.815502 xoa-utils-2.0.1/xoa_utils/cmds/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/cmds/cmd_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/cmds/cmd_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.815502 xoa-utils-2.0.1/xoa_utils/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.815502 xoa-utils-2.0.1/xoa_utils/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/hub/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.815502 xoa-utils-2.0.1/xoa_utils/ssh_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/ssh_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 14:11:04.000000 xoa-utils-2.0.1/xoa_utils/ssh_server/xena_ssh_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:11:14.811502 xoa-utils-2.0.1/xoa_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-15 14:11:14.000000 xoa-utils-2.0.1/xoa_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-15 14:11:14.000000 xoa-utils-2.0.1/xoa_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:11:14.000000 xoa-utils-2.0.1/xoa_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 14:11:14.000000 xoa-utils-2.0.1/xoa_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-15 14:11:14.000000 xoa-utils-2.0.1/xoa_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 14:11:14.000000 xoa-utils-2.0.1/xoa_utils.egg-info/top_level.txt
```

### Comparing `xoa-utils-2.0.0/LICENSE` & `xoa-utils-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/PKG-INFO` & `xoa-utils-2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-utils
-Version: 2.0.0
+Version: 2.0.1
 Summary: Xena OpenAutomation Utilities provides a shell-like command-line interface for users to do explorative tests interactively, such as ANLT test.
 Home-page: https://github.com/xenanetworks/open-automation-utilities
 Author: Ron Ding, Leonard Yu
 Author-email: rdi@xenanetworks.com, hyu@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-utils-2.0.0/README.md` & `xoa-utils-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/setup.py` & `xoa-utils-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clicks/click_backend.py` & `xoa-utils-2.0.1/xoa_utils/clicks/click_backend.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/__init__.py` & `xoa-utils-2.0.1/xoa_utils/clicks/click_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/an.py` & `xoa-utils-2.0.1/xoa_utils/clicks/click_commands/an.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/anlt.py` & `xoa-utils-2.0.1/xoa_utils/clicks/click_commands/anlt.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/debug.py` & `xoa-utils-2.0.1/xoa_utils/clicks/click_commands/debug.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/lt.py` & `xoa-utils-2.0.1/xoa_utils/clicks/click_commands/lt.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clicks/click_commands/management.py` & `xoa-utils-2.0.1/xoa_utils/clicks/click_commands/management.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clicks/click_help.py` & `xoa-utils-2.0.1/xoa_utils/clicks/click_help.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clis/__init__.py` & `xoa-utils-2.0.1/xoa_utils/clis/__init__.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/clis/cli_utils.py` & `xoa-utils-2.0.1/xoa_utils/clis/cli_utils.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/cmds/cmd_context.py` & `xoa-utils-2.0.1/xoa_utils/cmds/cmd_context.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/cmds/cmd_worker.py` & `xoa-utils-2.0.1/xoa_utils/cmds/cmd_worker.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/entry.py` & `xoa-utils-2.0.1/xoa_utils/entry.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/exceptions/exceptions.py` & `xoa-utils-2.0.1/xoa_utils/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/hub/hub.py` & `xoa-utils-2.0.1/xoa_utils/hub/hub.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils/ssh_server/xena_ssh_server.py` & `xoa-utils-2.0.1/xoa_utils/ssh_server/xena_ssh_server.py`

 * *Files identical despite different names*

### Comparing `xoa-utils-2.0.0/xoa_utils.egg-info/PKG-INFO` & `xoa-utils-2.0.1/xoa_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-utils
-Version: 2.0.0
+Version: 2.0.1
 Summary: Xena OpenAutomation Utilities provides a shell-like command-line interface for users to do explorative tests interactively, such as ANLT test.
 Home-page: https://github.com/xenanetworks/open-automation-utilities
 Author: Ron Ding, Leonard Yu
 Author-email: rdi@xenanetworks.com, hyu@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-utils-2.0.0/xoa_utils.egg-info/SOURCES.txt` & `xoa-utils-2.0.1/xoa_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

