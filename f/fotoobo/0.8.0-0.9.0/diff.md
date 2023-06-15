# Comparing `tmp/fotoobo-0.8.0.tar.gz` & `tmp/fotoobo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fotoobo-0.8.0.tar", max compression
+gzip compressed data, was "fotoobo-0.9.0.tar", max compression
```

## Comparing `fotoobo-0.8.0.tar` & `fotoobo-0.9.0.tar`

### file list

```diff
@@ -1,64 +1,63 @@
--rw-r--r--   0        0        0     7633 2023-04-13 12:43:19.567977 fotoobo-0.8.0/LICENSE
--rw-r--r--   0        0        0     2797 2023-04-13 12:43:19.567977 fotoobo-0.8.0/README.md
--rw-r--r--   0        0        0      256 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/__init__.py
--rw-r--r--   0        0        0      206 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/__init__.py
--rw-r--r--   0        0        0     1584 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/convert.py
--rw-r--r--   0        0        0       20 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/ems/__init__.py
--rw-r--r--   0        0        0     1488 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/ems/get_commands.py
--rw-r--r--   0        0        0      784 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/ems/main.py
--rw-r--r--   0        0        0     7418 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/ems/monitor_commands.py
--rw-r--r--   0        0        0       20 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/faz/__init__.py
--rw-r--r--   0        0        0      995 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/faz/get_commands.py
--rw-r--r--   0        0        0      639 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/faz/main.py
--rw-r--r--   0        0        0       20 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/__init__.py
--rw-r--r--   0        0        0     1537 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/config_commands.py
--rw-r--r--   0        0        0     1283 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/get_commands.py
--rw-r--r--   0        0        0     1951 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/main.py
--rw-r--r--   0        0        0     1711 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fgt/monitor_commands.py
--rw-r--r--   0        0        0       20 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fmg/__init__.py
--rw-r--r--   0        0        0     2582 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fmg/get_commands.py
--rw-r--r--   0        0        0     2199 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/fmg/main.py
--rw-r--r--   0        0        0     1033 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/get.py
--rw-r--r--   0        0        0     4743 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/cli/main.py
--rw-r--r--   0        0        0      196 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/exceptions/__init__.py
--rw-r--r--   0        0        0     1966 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/exceptions/exceptions.py
--rw-r--r--   0        0        0      190 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/__init__.py
--rw-r--r--   0        0        0    13955 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/convert.py
--rw-r--r--   0        0        0     1023 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortianalyzer.py
--rw-r--r--   0        0        0     5431 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/forticlientems.py
--rw-r--r--   0        0        0     2878 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortigate.py
--rw-r--r--   0        0        0    11342 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortigate_config.py
--rw-r--r--   0        0        0     8668 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortigate_config_check.py
--rw-r--r--   0        0        0      584 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortigate_info.py
--rw-r--r--   0        0        0    10421 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortimanager.py
--rw-r--r--   0        0        0     6468 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/fortinet/fortinet.py
--rw-r--r--   0        0        0      322 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/__init__.py
--rw-r--r--   0        0        0     1227 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/cli.py
--rw-r--r--   0        0        0     3435 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/config.py
--rw-r--r--   0        0        0     6414 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/files.py
--rw-r--r--   0        0        0    10407 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/log.py
--rw-r--r--   0        0        0     9300 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/helpers/output.py
--rw-r--r--   0        0        0      128 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/inventory/__init__.py
--rw-r--r--   0        0        0      568 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/inventory/generic.py
--rw-r--r--   0        0        0     4296 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/inventory/inventory.py
--rwxr-xr-x   0        0        0     1359 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/main.py
--rw-r--r--   0        0        0      440 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/utils/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/utils/convert.py
--rw-r--r--   0        0        0       92 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/utils/ems/__init__.py
--rw-r--r--   0        0        0     1518 2023-04-13 12:43:19.571977 fotoobo-0.8.0/fotoobo/utils/ems/get.py
--rw-r--r--   0        0        0     7725 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/ems/monitor.py
--rw-r--r--   0        0        0       56 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/faz/__init__.py
--rw-r--r--   0        0        0      779 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/faz/get.py
--rw-r--r--   0        0        0      129 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/__init__.py
--rw-r--r--   0        0        0     3468 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/config.py
--rw-r--r--   0        0        0     1114 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/get.py
--rw-r--r--   0        0        0     3286 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/main.py
--rw-r--r--   0        0        0     4583 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fgt/monitor.py
--rw-r--r--   0        0        0      105 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fmg/__init__.py
--rw-r--r--   0        0        0     4271 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fmg/get.py
--rw-r--r--   0        0        0     2534 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fmg/main.py
--rw-r--r--   0        0        0     1059 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/fmg/post_.py
--rw-r--r--   0        0        0     2152 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/get.py
--rw-r--r--   0        0        0     1306 2023-04-13 12:43:19.575977 fotoobo-0.8.0/fotoobo/utils/greet.py
--rw-r--r--   0        0        0     3730 2023-04-13 12:43:19.575977 fotoobo-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 fotoobo-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7633 2023-04-20 13:29:11.640759 fotoobo-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2797 2023-04-20 13:29:11.640759 fotoobo-0.9.0/README.md
+-rw-r--r--   0        0        0      256 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/__init__.py
+-rw-r--r--   0        0        0     1584 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/convert.py
+-rw-r--r--   0        0        0       20 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/ems/__init__.py
+-rw-r--r--   0        0        0     1488 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/ems/get_commands.py
+-rw-r--r--   0        0        0      784 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/ems/main.py
+-rw-r--r--   0        0        0     7418 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/ems/monitor_commands.py
+-rw-r--r--   0        0        0       20 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/faz/__init__.py
+-rw-r--r--   0        0        0      995 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/faz/get_commands.py
+-rw-r--r--   0        0        0      639 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/faz/main.py
+-rw-r--r--   0        0        0       20 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/__init__.py
+-rw-r--r--   0        0        0     1537 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/config_commands.py
+-rw-r--r--   0        0        0     1283 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/get_commands.py
+-rw-r--r--   0        0        0     1951 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/main.py
+-rw-r--r--   0        0        0     1711 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fgt/monitor_commands.py
+-rw-r--r--   0        0        0       20 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fmg/__init__.py
+-rw-r--r--   0        0        0     2582 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fmg/get_commands.py
+-rw-r--r--   0        0        0     2368 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/fmg/main.py
+-rw-r--r--   0        0        0     1033 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/get.py
+-rw-r--r--   0        0        0     4743 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/cli/main.py
+-rw-r--r--   0        0        0      196 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/exceptions/__init__.py
+-rw-r--r--   0        0        0     1966 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/exceptions/exceptions.py
+-rw-r--r--   0        0        0      190 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/__init__.py
+-rw-r--r--   0        0        0    13955 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/convert.py
+-rw-r--r--   0        0        0     1023 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/fortianalyzer.py
+-rw-r--r--   0        0        0     5431 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/forticlientems.py
+-rw-r--r--   0        0        0     2961 2023-04-20 13:29:11.644759 fotoobo-0.9.0/fotoobo/fortinet/fortigate.py
+-rw-r--r--   0        0        0    11342 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortigate_config.py
+-rw-r--r--   0        0        0     8668 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortigate_config_check.py
+-rw-r--r--   0        0        0      584 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortigate_info.py
+-rw-r--r--   0        0        0    10537 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortimanager.py
+-rw-r--r--   0        0        0     6523 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/fortinet/fortinet.py
+-rw-r--r--   0        0        0      322 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/__init__.py
+-rw-r--r--   0        0        0     1227 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/cli.py
+-rw-r--r--   0        0        0     3559 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/config.py
+-rw-r--r--   0        0        0     6414 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/files.py
+-rw-r--r--   0        0        0    11017 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/log.py
+-rw-r--r--   0        0        0     9300 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/helpers/output.py
+-rw-r--r--   0        0        0      128 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/inventory/__init__.py
+-rw-r--r--   0        0        0      568 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/inventory/generic.py
+-rw-r--r--   0        0        0     5050 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/inventory/inventory.py
+-rwxr-xr-x   0        0        0     1359 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/main.py
+-rw-r--r--   0        0        0      440 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/convert.py
+-rw-r--r--   0        0        0       92 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/ems/__init__.py
+-rw-r--r--   0        0        0     1518 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/ems/get.py
+-rw-r--r--   0        0        0     7725 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/ems/monitor.py
+-rw-r--r--   0        0        0       56 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/faz/__init__.py
+-rw-r--r--   0        0        0      779 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/faz/get.py
+-rw-r--r--   0        0        0      129 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/__init__.py
+-rw-r--r--   0        0        0     3468 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/config.py
+-rw-r--r--   0        0        0     1114 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/get.py
+-rw-r--r--   0        0        0     3286 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/main.py
+-rw-r--r--   0        0        0     4583 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fgt/monitor.py
+-rw-r--r--   0        0        0      105 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fmg/__init__.py
+-rw-r--r--   0        0        0     4271 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fmg/get.py
+-rw-r--r--   0        0        0     2707 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/fmg/main.py
+-rw-r--r--   0        0        0     2152 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/get.py
+-rw-r--r--   0        0        0     1306 2023-04-20 13:29:11.648759 fotoobo-0.9.0/fotoobo/utils/greet.py
+-rw-r--r--   0        0        0     3730 2023-04-20 13:29:11.648759 fotoobo-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 fotoobo-0.9.0/PKG-INFO
```

### Comparing `fotoobo-0.8.0/LICENSE` & `fotoobo-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/README.md` & `fotoobo-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/convert.py` & `fotoobo-0.9.0/fotoobo/cli/convert.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/ems/get_commands.py` & `fotoobo-0.9.0/fotoobo/cli/ems/get_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/ems/main.py` & `fotoobo-0.9.0/fotoobo/cli/ems/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/ems/monitor_commands.py` & `fotoobo-0.9.0/fotoobo/cli/ems/monitor_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/faz/get_commands.py` & `fotoobo-0.9.0/fotoobo/cli/faz/get_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/faz/main.py` & `fotoobo-0.9.0/fotoobo/cli/faz/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/fgt/config_commands.py` & `fotoobo-0.9.0/fotoobo/cli/fgt/config_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/fgt/get_commands.py` & `fotoobo-0.9.0/fotoobo/cli/fgt/get_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/fgt/main.py` & `fotoobo-0.9.0/fotoobo/cli/fgt/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/fgt/monitor_commands.py` & `fotoobo-0.9.0/fotoobo/cli/fgt/monitor_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/fmg/get_commands.py` & `fotoobo-0.9.0/fotoobo/cli/fmg/get_commands.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/fmg/main.py` & `fotoobo-0.9.0/fotoobo/cli/fmg/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,20 @@
         ...,
         help="The ADOMs to assign the global policy/objects to. Use "
         "'fotoobo fmg get adoms' to get a list of "
         "available ADOMs. Separate multiple ADOMs by comma (no spaces).",
         metavar="[adoms]",
         show_default=False,
     ),
+    policy: str = typer.Argument(
+        ...,
+        help="The global policy to assign",
+        metavar="[policy]",
+        show_default=False,
+    ),
     host: str = typer.Argument(
         "fmg",
         help="The FortiManager to access (must be defined in the inventory).",
         metavar="[host]",
     ),
     timeout: int = typer.Option(
         60,
@@ -47,34 +53,33 @@
         help="The timeout to wait for the FortiManager task to finish.",
         metavar="[timeout]",
     ),
 ) -> None:
     """
     Assign a global policy to a specified ADOM or to a list of ADOMs.
     """
-    fmg.assign(host, adoms, timeout=timeout)
+    fmg.assign(adoms=adoms, policy=policy, host=host, timeout=timeout)
 
 
 @app.command(no_args_is_help=True)
 def post(
-    host: str = typer.Argument(
-        ...,
-        help="The FortiManager to access (must be defined in the inventory).",
-        metavar="[host]",
-        show_default=False,
-    ),
     file: str = typer.Argument(
         ..., help="JSON file with payload(s).", show_default=False, metavar="[file]"
     ),
     adom: str = typer.Argument(
         ..., help="The ADOM to issue the set command(s).", metavar="[adom]", show_default=False
     ),
+    host: str = typer.Argument(
+        "fmg",
+        help="The FortiManager to access (must be defined in the inventory).",
+        metavar="[host]",
+    ),
 ) -> None:
     """
     POST any valid JSON request to the FortiManager.
 
     Configure the FortiManager with any valid API call(s) given within the JSON file.
     """
-    fmg.post(host, file, adom)
+    fmg.post(file=file, adom=adom, host=host)
 
 
 app.add_typer(get.app, name="get", help="FortiManager get commands.")
```

### Comparing `fotoobo-0.8.0/fotoobo/cli/get.py` & `fotoobo-0.9.0/fotoobo/cli/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/cli/main.py` & `fotoobo-0.9.0/fotoobo/cli/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/exceptions/exceptions.py` & `fotoobo-0.9.0/fotoobo/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/fortinet/convert.py` & `fotoobo-0.9.0/fotoobo/fortinet/convert.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/fortinet/fortianalyzer.py` & `fotoobo-0.9.0/fotoobo/fortinet/fortianalyzer.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/fortinet/forticlientems.py` & `fotoobo-0.9.0/fotoobo/fortinet/forticlientems.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/fortinet/fortigate.py` & `fotoobo-0.9.0/fotoobo/fortinet/fortigate.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,18 +66,21 @@
         self.session.headers.update({"Authorization": f"Bearer {self.token}"})
         return super().api(
             method, url, payload=payload, params=params, timeout=timeout, headers=headers
         )
 
     def backup(self, timeout: int = 10) -> str:
         """
-        Get the configuration backup from a FortiGate
+        Get the configuration backup from a FortiGate.
+
+        Args:
+            timeout (int): Timeout in sec to wait for the response
 
         Returns:
-            str: configuration backup as text
+            str: Configuration backup as text
         """
         data = self.api(
             "get", "monitor/system/config/backup", params={"scope": "global"}, timeout=timeout
         )
         return data.text
 
     def get_version(self) -> str:
```

### Comparing `fotoobo-0.8.0/fotoobo/fortinet/fortigate_config.py` & `fotoobo-0.9.0/fotoobo/fortinet/fortigate_config.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/fortinet/fortigate_config_check.py` & `fotoobo-0.9.0/fotoobo/fortinet/fortigate_config_check.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/fortinet/fortigate_info.py` & `fotoobo-0.9.0/fotoobo/fortinet/fortigate_info.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/fortinet/fortimanager.py` & `fotoobo-0.9.0/fotoobo/fortinet/fortimanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,38 +87,40 @@
         if method.lower() == "post":
             payload["session"] = self.sessionkey
 
         return super().api(
             method, url, headers=headers, payload=payload, params=params, timeout=timeout
         )
 
-    def assign_all_objects(self, adoms: str) -> int:
+    def assign_all_objects(self, adoms: str, policy: str) -> int:
         """
         Copies all objects from the global ADOM database to a given ADOM.
 
         Args:
             adoms (str): The ADOM to assign the global policy/objects to. If you specify an invalid
-            ADOM name you'll get a permission error. You can specify multiple ADOMs by separating
-            them with a comma (no spaces)
+                ADOM name you'll get a permission error. You can specify multiple ADOMs by
+                separating them with a comma (no spaces)
+
+            policy (str): Specify the global policy to assign [Default: 'default'].
 
         Returns:
-            int: The id of the created task or 0 (zero) if unsuccessful
+            int: The id of the FortiManager task created or 0 (zero) if unsuccessful
 
         """
         task_id = 0
         adom_payload = []
         for adom in adoms.split(","):
             adom_payload.append({"adom": adom, "excluded": "disable"})
         payload = {
             "method": "exec",
             "params": [
                 {
                     "data": {
                         "flags": ["cp_all_objs"],
-                        "pkg": "default",
+                        "pkg": policy,
                         "target": adom_payload,
                     },
                     "url": "/securityconsole/assign/package",
                 }
             ],
         }
         response = self.api("post", payload=payload)
```

### Comparing `fotoobo-0.8.0/fotoobo/fortinet/fortinet.py` & `fotoobo-0.9.0/fotoobo/fortinet/fortinet.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from time import time
 from typing import Any, Dict, Optional
 
 import requests
 import urllib3
 
 from fotoobo.exceptions import APIError, GeneralError
+from fotoobo.helpers.config import config
 
 log = logging.getLogger("fotoobo")
 
 
 class Fortinet(ABC):
     """
     This is the Fortinet abstract base class. All other Fortinet product classes should inherit
@@ -50,15 +51,15 @@
         self.https_port: int = kwargs.get("https_port", 443)
         self.session = requests.Session()
         self.session.trust_env = False
         self.session.proxies: Dict[str, Any] = {"http": None, "https": None}  # type: ignore
         if proxy := kwargs.get("proxy", ""):
             self.session.proxies = {"http": f"{proxy}", "https": f"{proxy}"}
 
-        self.ssl_verify: bool = kwargs.get("ssl_verify", True)
+        self.ssl_verify: bool = kwargs.get("ssl_verify", config.ssl_verify)
         if not self.ssl_verify:
             urllib3.disable_warnings()
 
         self.timeout = kwargs.get("timeout", 3)
         self.type: str = ""
 
     def api(  # pylint: disable=too-many-arguments
```

### Comparing `fotoobo-0.8.0/fotoobo/helpers/cli.py` & `fotoobo-0.9.0/fotoobo/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/helpers/config.py` & `fotoobo-0.9.0/fotoobo/helpers/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     # set default values
     inventory_file: str = "inventory.yaml"
     logging: Union[Dict[str, Any], None] = None
     audit_logging: Union[Dict[str, Any], None] = None
     no_logo: bool = False
     snmp_community: str = ""
     cli_info: Dict[str, Any] = field(default_factory=dict)
+    ssl_verify: Union[str, bool] = True
 
     def load_configuration(self, config_file: Union[str, None]) -> None:
         """
         Load the global fotoobo configuration file. If the configuration file is not present it just
         will be ignored and all the options remain as they are.
         If a file is present it looks for configuration options to set. Keep in mind that it is not
         mandatory to define every option in the configuration file. For that case make sure that an
@@ -73,9 +74,11 @@
 
                 if loaded_config.get("audit_logging"):
                     self.audit_logging = loaded_config["audit_logging"]
 
                 self.no_logo = loaded_config.get("no_logo", self.no_logo)
                 self.snmp_community = loaded_config.get("snmp_community", self.snmp_community)
 
+                self.ssl_verify = loaded_config.get("ssl_verify", self.ssl_verify)
+
 
 config = Config()
```

### Comparing `fotoobo-0.8.0/fotoobo/helpers/files.py` & `fotoobo-0.9.0/fotoobo/helpers/files.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/helpers/log.py` & `fotoobo-0.9.0/fotoobo/helpers/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import logging.config
 import os
 import pwd
 import socket
 from datetime import datetime
 from logging.handlers import RotatingFileHandler, SysLogHandler
 from typing import Optional, Union
-
 from syslog import LOG_AUTH, LOG_CRIT, LOG_DEBUG, LOG_ERR, LOG_INFO, LOG_USER, LOG_WARNING
+
 from rich.logging import RichHandler
 
 from fotoobo.exceptions import GeneralError, GeneralWarning
 from fotoobo.helpers.config import config
 from fotoobo.helpers.files import load_yaml_file
 
 logger = logging.getLogger("fotoobo")
@@ -206,23 +206,28 @@
                                 "%(message)s"
                             )
                         )
 
                         logger.addHandler(file_handler)
 
                     if "log_syslog" in config.logging:
-                        syslog_handler = SysLogHandler(
-                            address=(
-                                config.logging["log_syslog"]["host"],
-                                int(config.logging["log_syslog"]["port"]),
-                            ),
-                            socktype=socket.SOCK_STREAM
-                            if config.logging["log_syslog"]["protocol"] == "TCP"
-                            else socket.SOCK_DGRAM,
-                        )
+                        try:
+                            syslog_handler = SysLogHandler(
+                                address=(
+                                    config.logging["log_syslog"]["host"],
+                                    int(config.logging["log_syslog"]["port"]),
+                                ),
+                                socktype=socket.SOCK_STREAM
+                                if config.logging["log_syslog"]["protocol"] == "TCP"
+                                else socket.SOCK_DGRAM,
+                            )
+                        except (OSError, socket.gaierror) as error:
+                            raise GeneralError(
+                                f"Cannot configure SysLog logging: {str(error)}"
+                            ) from error
 
                         syslog_handler.setFormatter(SysLogFormatter(LOG_USER))
 
                         logger.addHandler(syslog_handler)
 
                 else:
                     logger.disabled = True
@@ -243,24 +248,29 @@
                                 fmt="%(asctime)s - AUDIT - %(filename)s:%(lineno)d: %(message)s"
                             )
                         )
 
                         audit_logger.addHandler(audit_file_handler)
 
                     if "log_syslog" in config.audit_logging:
-                        audit_syslog_handler = SysLogHandler(
-                            address=(
-                                config.audit_logging["log_syslog"]["host"],
-                                int(config.audit_logging["log_syslog"]["port"]),
-                            ),
-                            facility=LOG_AUTH,
-                            socktype=socket.SOCK_STREAM
-                            if config.audit_logging["log_syslog"]["protocol"] == "TCP"
-                            else socket.SOCK_DGRAM,
-                        )
+                        try:
+                            audit_syslog_handler = SysLogHandler(
+                                address=(
+                                    config.audit_logging["log_syslog"]["host"],
+                                    int(config.audit_logging["log_syslog"]["port"]),
+                                ),
+                                facility=LOG_AUTH,
+                                socktype=socket.SOCK_STREAM
+                                if config.audit_logging["log_syslog"]["protocol"] == "TCP"
+                                else socket.SOCK_DGRAM,
+                            )
+                        except (OSError, socket.gaierror) as error:
+                            raise GeneralError(
+                                f"Cannot configure SysLog logging: {str(error)}"
+                            ) from error
 
                         audit_syslog_handler.setFormatter(SysLogFormatter(LOG_AUTH))
 
                         audit_logger.addHandler(audit_syslog_handler)
 
                 else:
                     audit_logger.disabled = True
```

### Comparing `fotoobo-0.8.0/fotoobo/helpers/output.py` & `fotoobo-0.9.0/fotoobo/helpers/output.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/inventory/generic.py` & `fotoobo-0.9.0/fotoobo/inventory/generic.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/inventory/inventory.py` & `fotoobo-0.9.0/fotoobo/inventory/inventory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Devices class for storing device information
 """
 
 import logging
 from typing import Any, Dict, Optional
+import os
 
 from fotoobo.exceptions import GeneralWarning
 from fotoobo.fortinet.fortianalyzer import FortiAnalyzer
 from fotoobo.fortinet.forticlientems import FortiClientEMS
 from fotoobo.fortinet.fortigate import FortiGate
 from fotoobo.fortinet.fortimanager import FortiManager
 from fotoobo.helpers.files import load_yaml_file
@@ -76,16 +77,18 @@
 
         return assets
 
     def _load_inventory(self) -> None:
         """
         Load the inventory from a file given
         """
-        log.debug("loading assets from '%s'", self._inventory_file)
-        inventory_raw: Dict[str, Any] = dict(load_yaml_file(self._inventory_file) or {})
+        # Expand user home shortcuts in the inventory file path
+        expanded_inventory_file = os.path.expanduser(self._inventory_file)
+        log.debug("loading assets from '%s'", expanded_inventory_file)
+        inventory_raw: Dict[str, Any] = dict(load_yaml_file(expanded_inventory_file) or {})
 
         # set the globals
         # this has to be done before the looping over all inventory items so that the globals are
         # already set during looping
         if "globals" in inventory_raw:
             self._set_globals(inventory_raw["globals"])
 
@@ -110,14 +113,30 @@
 
             elif asset.get("type", "") == "fortimanager":
                 self.assets[name] = FortiManager(**asset)
 
             else:
                 self.assets[name] = GenericDevice(**asset)
 
+    # pylint: disable=pointless-string-statement
+    """
+        # create asset object using the match and case keywords
+        match asset_type:
+            case "fortigate":
+                self.assets[name] = FortiGate(**asset)
+            case "forticlientems":
+                self.assets[name] = FortiClientEMS(**asset)
+            case "fortianalyzer":
+                self.assets[name] = FortiAnalyzer(**asset)
+            case "fortimanager":
+                self.assets[name] = FortiManager(**asset)
+            case _:
+                self.assets[name] = GenericDevice(**asset)
+    """
+
     def _set_globals(self, data: Dict[str, Any]) -> None:
         """
         Set some defaults for device types
 
         Args:
             data (Dict[str, Any]): defaults by device where key is the device type and value defines
             its defaults
```

### Comparing `fotoobo-0.8.0/fotoobo/main.py` & `fotoobo-0.9.0/fotoobo/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/convert.py` & `fotoobo-0.9.0/fotoobo/utils/convert.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/ems/get.py` & `fotoobo-0.9.0/fotoobo/utils/ems/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/ems/monitor.py` & `fotoobo-0.9.0/fotoobo/utils/ems/monitor.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/faz/get.py` & `fotoobo-0.9.0/fotoobo/utils/faz/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/fgt/config.py` & `fotoobo-0.9.0/fotoobo/utils/fgt/config.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/fgt/get.py` & `fotoobo-0.9.0/fotoobo/utils/fgt/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/fgt/main.py` & `fotoobo-0.9.0/fotoobo/utils/fgt/main.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/fgt/monitor.py` & `fotoobo-0.9.0/fotoobo/utils/fgt/monitor.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/fmg/get.py` & `fotoobo-0.9.0/fotoobo/utils/fmg/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/fmg/main.py` & `fotoobo-0.9.0/fotoobo/utils/fmg/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,33 +8,31 @@
 from fotoobo.helpers.config import config
 from fotoobo.helpers.files import load_json_file
 from fotoobo.inventory import Inventory
 
 log = logging.getLogger("fotoobo")
 
 
-def assign(host: str, adoms: str, timeout: int = 60) -> None:
+def assign(adoms: str, policy: str, host: str, timeout: int = 60) -> None:
     """
     Assign the global policy to the given ADOM
 
     Args:
-        host (str):  The FortiManager defined in inventory
-
-        adoms (str): The ADOMs to assign the global policy to. Specify multiple ADOMs as a comma
-        separated list (no spaces)
-
-    Raises:
-        GeneralWarning: _description_
+        adoms (str):   The ADOMs to assign the global policy to. Specify multiple ADOMs as a comma
+            separated list (no spaces).
+        policy (str):  Specify the global policy to assign [Default: 'default'].
+        host (str):    The FortiManager defined in inventory.
+        timeout (int): Timeout in sec. to wait for the FortiManager task to finish [Default: 60].
     """
     inventory = Inventory(config.inventory_file)
     fmg = inventory.get(host, "fortimanager")[host]
     fmg.login()
 
     log.debug("Assigning global policy/objects to ADOM %s", adoms)
-    task_id = fmg.assign_all_objects(adoms)
+    task_id = fmg.assign_all_objects(adoms=adoms, policy=policy)
     if task_id > 0:
         log.info("created FortiManager task id %s", task_id)
         messages = fmg.wait_for_task(task_id, timeout=timeout)
         for message in messages:
             level = "debug" if message["state"] == 4 else "error"
             elapsed = (
                 str(message["end_tm"] - message["start_tm"]) + " sec"
@@ -51,31 +49,31 @@
             if message["history"]:
                 for line in message["history"]:
                     getattr(log, level)("- %s", line["detail"])
 
     fmg.logout()
 
 
-def post(host: str, file: str, adom: str) -> None:
+def post(file: str, adom: str, host: str) -> None:
     """
-    Set the given configuration from a JSON file to the FortiManager
+    POST the given configuration from a JSON file to the FortiManager
 
     Args:
-        host (str): The FortiManager defined in inventory
         file (str): The configuration file to oad the configuration from
         adom (str): The ADOM to assign the global policy to
+        host (str): The FortiManager defined in inventory
 
     Raises:
         GeneralWarning: GeneralWarning
     """
     if not (payloads := load_json_file(file)):
         raise GeneralWarning(f"there is no data in the given file ({file})")
 
     inventory = Inventory(config.inventory_file)
     fmg = inventory.get(host, "fortimanager")[host]
     fmg.login()
 
-    log.debug("FortiManager set command ...")
-    log.info("start setting assets to '%s'", host + "/" + adom)
+    log.debug("FortiManager post command ...")
+    log.info("start POSTing assets to '%s'", host + "/" + adom)
 
     fmg.post(adom, payloads)
     fmg.logout()
```

### Comparing `fotoobo-0.8.0/fotoobo/utils/get.py` & `fotoobo-0.9.0/fotoobo/utils/get.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/fotoobo/utils/greet.py` & `fotoobo-0.9.0/fotoobo/utils/greet.py`

 * *Files identical despite different names*

### Comparing `fotoobo-0.8.0/pyproject.toml` & `fotoobo-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fotoobo"
-version = "0.8.0"
+version = "0.9.0"
 description = "The awesome Fortinet Toolbox"
 authors = ["Patrik Spiess <patrik.spiess@mgb.ch>", "Lukas Murer-Jäckle <lukas.murer@mgb.ch>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.0, <3.12"
 typer = "~0.6.0"
```

### Comparing `fotoobo-0.8.0/PKG-INFO` & `fotoobo-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fotoobo
-Version: 0.8.0
+Version: 0.9.0
 Summary: The awesome Fortinet Toolbox
 Author: Patrik Spiess
 Author-email: patrik.spiess@mgb.ch
 Requires-Python: >=3.8.0,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

