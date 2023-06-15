# Comparing `tmp/inhandtest-0.0.55.tar.gz` & `tmp/inhandtest-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.55.tar", last modified: Mon Jun 12 09:13:43 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.56.tar", last modified: Thu Jun 15 06:17:55 2023, max compression
```

## Comparing `inhandtest-0.0.55.tar` & `inhandtest-0.0.56.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/
--rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.55/MANIFEST.in
--rw-rw-rw-   0        0        0      593 2023-06-12 09:13:42.000000 inhandtest-0.0.55/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.55/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/dm/
--rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.55/dm/mqtt.py
--rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.55/dm/register_v1.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.55/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/base_page/
--rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.55/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    40087 2023-06-07 07:00:46.000000 inhandtest-0.0.55/inhandtest/base_page/_ig_contents_locators.py
--rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.55/inhandtest/base_page/_ir3XX_contents_locators.py
--rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.55/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    59214 2023-06-12 05:21:09.000000 inhandtest-0.0.55/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    23673 2023-06-08 06:22:30.000000 inhandtest-0.0.55/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.55/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3895 2023-06-01 09:18:53.000000 inhandtest-0.0.55/inhandtest/file.py
--rw-rw-rw-   0        0        0    11861 2023-05-06 01:56:01.000000 inhandtest-0.0.55/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.55/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22057 2023-06-01 09:18:53.000000 inhandtest-0.0.55/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    52197 2023-06-07 03:52:54.000000 inhandtest-0.0.55/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0     7820 2023-06-07 06:08:07.000000 inhandtest-0.0.55/inhandtest/inserial.py
--rw-rw-rw-   0        0        0    14360 2023-06-01 09:15:20.000000 inhandtest-0.0.55/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6854 2023-06-01 09:15:20.000000 inhandtest-0.0.55/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.55/inhandtest/ip.py
--rw-rw-rw-   0        0        0    13416 2023-06-12 09:13:16.000000 inhandtest-0.0.55/inhandtest/mail.py
--rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.55/inhandtest/notice_email.html
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/
--rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.55/inhandtest/pages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/
--rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/
--rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/__init__.py
--rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
--rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
--rw-rw-rw-   0        0        0     3150 2023-06-12 08:58:41.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/ingateway.py
--rw-rw-rw-   0        0        0     8694 2023-06-08 08:54:15.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/locale.yml
--rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/locators.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/network/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/network/__init__.py
--rw-rw-rw-   0        0        0    67657 2023-06-12 05:25:10.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/network/network.py
--rw-rw-rw-   0        0        0    86112 2023-06-12 05:18:58.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/network/network_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/overview/
--rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/overview/__init__.py
--rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/overview/overview.py
--rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/overview/overview_locators.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/system/
--rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/system/__init__.py
--rw-rw-rw-   0        0        0    28496 2023-06-08 09:58:25.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/system/system.py
--rw-rw-rw-   0        0        0    30624 2023-06-08 09:03:50.000000 inhandtest-0.0.55/inhandtest/pages/ingateway/system/system_locators.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.55/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    33264 2023-06-12 08:58:41.000000 inhandtest-0.0.55/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    27509 2023-06-07 03:54:00.000000 inhandtest-0.0.55/inhandtest/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/
--rw-rw-rw-   0        0        0      593 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1667 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      123 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-12 09:13:42.000000 inhandtest-0.0.55/inhandtest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.55/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 09:13:42.000000 inhandtest-0.0.55/setup.cfg
--rw-rw-rw-   0        0        0     1615 2023-06-12 09:13:16.000000 inhandtest-0.0.55/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/
+-rw-rw-rw-   0        0        0       81 2023-04-13 01:59:22.000000 inhandtest-0.0.56/MANIFEST.in
+-rw-rw-rw-   0        0        0      593 2023-06-15 06:17:55.000000 inhandtest-0.0.56/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.56/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/dm/
+-rw-rw-rw-   0        0        0     1307 2023-04-26 07:13:22.000000 inhandtest-0.0.56/dm/mqtt.py
+-rw-rw-rw-   0        0        0     3565 2023-04-28 07:00:23.000000 inhandtest-0.0.56/dm/register_v1.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.56/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      330 2023-05-31 07:35:39.000000 inhandtest-0.0.56/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    40087 2023-06-07 07:00:46.000000 inhandtest-0.0.56/inhandtest/base_page/_ig_contents_locators.py
+-rw-rw-rw-   0        0        0    27868 2023-05-17 02:51:06.000000 inhandtest-0.0.56/inhandtest/base_page/_ir3XX_contents_locators.py
+-rw-rw-rw-   0        0        0    64964 2023-05-11 07:07:35.000000 inhandtest-0.0.56/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    57431 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    23845 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.56/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     4219 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/file.py
+-rw-rw-rw-   0        0        0    10907 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4451 2023-06-15 05:47:54.000000 inhandtest-0.0.56/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22019 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    52646 2023-06-15 06:06:07.000000 inhandtest-0.0.56/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0     7726 2023-06-15 06:12:16.000000 inhandtest-0.0.56/inhandtest/inserial.py
+-rw-rw-rw-   0        0        0    14792 2023-06-15 06:12:16.000000 inhandtest-0.0.56/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     8481 2023-06-15 06:12:16.000000 inhandtest-0.0.56/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1569 2023-05-24 09:45:24.000000 inhandtest-0.0.56/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     1390 2023-06-15 05:51:48.000000 inhandtest-0.0.56/inhandtest/log.py
+-rw-rw-rw-   0        0        0    13757 2023-06-15 05:47:54.000000 inhandtest-0.0.56/inhandtest/mail.py
+-rw-rw-rw-   0        0        0      387 2023-06-12 09:08:02.000000 inhandtest-0.0.56/inhandtest/notice_email.html
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/
+-rw-rw-rw-   0        0        0      230 2023-05-31 07:29:45.000000 inhandtest-0.0.56/inhandtest/pages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/
+-rw-rw-rw-   0        0        0      136 2023-05-31 07:30:00.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/
+-rw-rw-rw-   0        0        0      134 2023-05-25 07:33:25.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/__init__.py
+-rw-rw-rw-   0        0        0     8879 2023-06-02 05:53:59.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py
+-rw-rw-rw-   0        0        0     9486 2023-06-02 05:59:32.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py
+-rw-rw-rw-   0        0        0     3057 2023-06-14 06:26:03.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/ingateway.py
+-rw-rw-rw-   0        0        0     8694 2023-06-08 08:54:15.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/locale.yml
+-rw-rw-rw-   0        0        0      911 2023-06-02 06:30:38.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/locators.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/network/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/network/__init__.py
+-rw-rw-rw-   0        0        0    67657 2023-06-12 05:25:10.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/network/network.py
+-rw-rw-rw-   0        0        0    86112 2023-06-12 05:18:58.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/network/network_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/overview/
+-rw-rw-rw-   0        0        0      134 2023-05-15 07:33:50.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/overview/__init__.py
+-rw-rw-rw-   0        0        0     6953 2023-06-02 09:29:07.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/overview/overview.py
+-rw-rw-rw-   0        0        0     6260 2023-05-18 07:02:23.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/overview/overview_locators.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/system/
+-rw-rw-rw-   0        0        0      133 2023-06-02 06:29:57.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/system/__init__.py
+-rw-rw-rw-   0        0        0    28496 2023-06-08 09:58:25.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/system/system.py
+-rw-rw-rw-   0        0        0    30624 2023-06-08 09:03:50.000000 inhandtest-0.0.56/inhandtest/pages/ingateway/system/system_locators.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.56/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    33875 2023-06-15 06:12:16.000000 inhandtest-0.0.56/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    28008 2023-06-15 06:16:19.000000 inhandtest-0.0.56/inhandtest/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/
+-rw-rw-rw-   0        0        0      593 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1685 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      123 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 06:17:55.000000 inhandtest-0.0.56/inhandtest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-01 10:06:41.000000 inhandtest-0.0.56/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 06:17:55.000000 inhandtest-0.0.56/setup.cfg
+-rw-rw-rw-   0        0        0     1615 2023-06-15 06:16:19.000000 inhandtest-0.0.56/setup.py
```

### Comparing `inhandtest-0.0.55/PKG-INFO` & `inhandtest-0.0.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.55
+Version: 0.0.56
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.55/README.md` & `inhandtest-0.0.56/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/dm/mqtt.py` & `inhandtest-0.0.56/dm/mqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/dm/register_v1.py` & `inhandtest-0.0.56/dm/register_v1.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/base_page/_ig_contents_locators.py` & `inhandtest-0.0.56/inhandtest/base_page/_ig_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/base_page/_ir3XX_contents_locators.py` & `inhandtest-0.0.56/inhandtest/base_page/_ir3XX_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.56/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/base_page/base_page.py` & `inhandtest-0.0.56/inhandtest/base_page/base_page.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,28 @@
 # @Author  : Pane Li
 # @File    : base_page.py
 """
 base_page
 
 """
 import os.path
-import sys
 from os import path
-
 import playwright
-
 from inhandtest.base_page._ig_contents_locators import IGContentsLocators
 from typing import List
 from inhandtest.exception import ModelError
 from inhandtest.tools import loop_inspector, replace_str
 from playwright.sync_api import Page, Locator, expect, TimeoutError, sync_playwright
 from inhandtest.base_page._vg710_contents_locators import VGContentsLocators
 from inhandtest.base_page._ir3XX_contents_locators import Ir3XXContentsLocators
 from inhandtest.base_page.table_tr import Table, IgTable
 from collections import Counter
 import allure
-import logging
 import re
+import logging
 
 
 class BasePage:
 
     def __init__(self, host: str, username: str, password: str, protocol='https',
                  port=443, model='VG710', language='en', page: Page = None, **kwargs):
         """
@@ -58,14 +55,15 @@
         if self.model == 'VG710':
             self.content_locator = VGContentsLocators(self.page, language).tags_menu
         elif self.model in ('IG902', 'IG502'):
             self.content_locator = IGContentsLocators(self.page, language).tags_menu
         elif self.model in ('IR302', 'IR305', 'IR615'):
             self.content_locator = Ir3XXContentsLocators(self.page, language).tags_menu
         else:
+            logging.exception(f'not support this mode {model}')
             raise ModelError(f'not support this mode {model}')
         self.locale = kwargs.get('locale').get(language) if kwargs.get('locale') else None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
@@ -84,14 +82,15 @@
                     'submit': self.page.locator('//button[@type="submit"]'),
                     'wait_locator': self.page.locator('#logo')}
         elif self.model == 'IR302':
             return {'username': self.page.locator('#username'), 'password': self.page.locator('#passwd'),
                     'submit': self.page.locator('.login_button'),
                     'wait_locator': self.page.locator('#logo')}
         else:
+            logging.exception(f'not support this model {self.model}')
             raise Exception(f'not support this model {self.model}')
 
     def __new_page(self):
         def dialog_(dialog):
             logging.debug(f'dialog message is {dialog.message}, accepted')
             dialog.accept()
 
@@ -127,14 +126,15 @@
         password = self.password if not password else password
 
         def goto_router():
             device = "{}://{}:{}".format(self.protocol, self.host, self.port)
             try:
                 self.page.goto(device, timeout=120 * 1000)
             except Exception:
+                logging.exception(f'Open {self.host} device address {device} timeout')
                 raise
             self.page.bring_to_front()
             self.page.wait_for_timeout(500)
             if self.model in self.__http_credentials_model:
                 logging.info(f'Open {self.host} device address {device} and login')
             else:
                 logging.info(f'Open {self.host} device address {device}')
@@ -166,14 +166,15 @@
             else:
                 try:
                     logging.debug(f"Device %s refresh page {i + 1} times" % self.host)
                     self.page.reload()
                 except TimeoutError:
                     pass
         else:
+            logging.exception(f'Device {self.host} page error')
             raise Exception(f'Device {self.host} page error')
 
     @allure.step('页面抓取接口返回结果')
     def wait_for_response(self, url: str, timeout=30) -> dict:
         """
 
         :param url:  pattern 匹配的正则表达式,
@@ -273,14 +274,15 @@
             self.page.bring_to_front()
             self.login()
             try:
                 menu = menu.replace(' ', '_').replace('-', '_').lower()
                 menu = default_change(menu, self.content_locator).split('.')
                 access(menu)
             except Exception:
+                logging.exception(f'not support this menu {menu}')
                 raise f'not support this menu {menu}'
             if wait_time:
                 self.page.wait_for_timeout(wait_time)
 
     @allure.step('输入信息')
     def fill(self, locator: Locator, value: str or int, log_desc=None, force=False) -> None:
         """ 封装公共的输入操作
@@ -374,14 +376,15 @@
                         option_end = all_option_.last.inner_text()
                         all_option_.last.scroll_into_view_if_needed()
                         logging.debug(f'scroll down the scroll bar {find_time + 1} tims')
                     else:
                         logging.debug(f'scroll down the bottom')
                         break
                 else:
+                    logging.exception(f'found more option elements')
                     raise Exception('found more option elements')
             if not select:
                 for find_time in range(0, times):
                     if option_.count() == 1:
                         option_.click()
                         break
                     elif option_.count() == 0:
@@ -389,16 +392,18 @@
                             option_end = all_option_.first.inner_text()
                             all_option_.first.scroll_into_view_if_needed()
                             logging.debug(f'scroll up the scroll bar {find_time + 1}')
                         else:
                             logging.debug(f'scroll up the top')
                             break
                     else:
+                        logging.exception(f'found more option elements')
                         raise Exception('found more option elements')
                 else:
+                    logging.exception(f'scroll bar too lang, more 100 times')
                     raise Exception('scroll bar too lang, more 100 times')
 
         if value is not None:
             value = str(value)
             locator.wait_for(state='visible')
             if locator.get_attribute('aria-controls') or locator.locator('.ant-select-selection').get_attribute(
                     'aria-controls'):
@@ -470,28 +475,30 @@
                     option.click(force=True)
                     if log_desc:
                         logging.info(f"Device {self.host} {log_desc} radio select {value}")
                 else:
                     if log_desc:
                         logging.debug(f"Device {self.host} {log_desc} radio already select {value}")
             else:
+                logging.exception(f'found {value} option {option.count()} elements')
                 raise Exception(f'found {value} option {option.count()} elements')
 
     @allure.step('伸缩按钮')
     def expand(self, left_text: str, action: str = 'expand') -> None:
         """ 伸缩按钮
 
         :param left_text: 伸缩按钮 左边的文本，需要注意国际化
         :param action: expand|close|None
         :return:
         """
         text_locator = self.page.get_by_text(left_text, exact=True)
         if action is not None:
             text_locator.wait_for(state='visible')
             if text_locator.count() > 1:
+                logging.exception(f'found {left_text} {text_locator.count()} elements')
                 raise
             else:
                 if text_locator.locator('..').get_attribute('type') == 'button':  # IG 产品
                     if 'right' in text_locator.locator('..').locator('//span/i').get_attribute('aria-label'):
                         if action.lower() == 'expand':
                             self.click(text_locator.locator('..'), f'expand {left_text}')
                     else:
@@ -503,14 +510,15 @@
                     if action.lower() == 'expand':
                         if not locator.get_attribute('style'):
                             self.click(locator, f'expand {left_text}')
                     else:
                         if locator.get_attribute('style') == 'transform: rotate(90deg);':
                             self.click(locator, f'closed {left_text}')
                 else:
+                    logging.exception(f'not support this expand')
                     raise Exception("not support this expand")
 
     @allure.step('上传文件')
     def upload_file(self, locator: Locator, path_, dialog_massage=None) -> None:
         """
 
         :param locator:
@@ -698,14 +706,15 @@
                         if isinstance(value_[2], str):
                             file_path = value_[2]
                             file_name = None
                         elif isinstance(value_[2], dict):
                             file_path = value_[2].get('file_path')
                             file_name = value_[2].get('file_name')
                         else:
+                            logging.exception('download file_path type error')
                             raise TypeError('download file_path type error')
                         tr.download(self.download_file, value_[1], file_path, file_name)
                     elif value_[0] in ('upload', 'import_config'):
                         tr.upload(self.upload_file, value_[1], value_[2])
                     elif value_[0] == 'start':
                         tr.start(value_[1])
                     elif value_[0] == 'stop':
@@ -789,14 +798,15 @@
                             param_locator.get('locator')[1].click(timeout=1 * 1000)
                         except TimeoutError:
                             pass
                         self.tip_messages(tip_messages, tip_messages_timeout)
                         if wait_for_time:
                             self.page.wait_for_timeout(wait_for_time)
                     else:
+                        logging.exception(f'locator {param_locator.get("locator")} is not a Locator or list or tuple')
                         raise Exception(f'locator {param_locator.get("locator")} is not a Locator or list or tuple')
             elif param_locator.get('type') == 'check':
                 if value:
                     value_, tip_messages = value, None
                     if isinstance(value, dict):
                         value_ = value.get('value')
                         tip_messages = value.get('tip_messages')
@@ -857,14 +867,15 @@
                     if isinstance(value, dict):
                         timeout = value.get('timeout') if value.get('timeout') else 10
                         messages = value.get('messages')
                     self.title_messages(messages, timeout)
             elif param_locator.get('type') == 'fill_date':
                 self.fill_date(param_locator.get('locator'), value)
             else:
+                logging.exception(f"not support this param type {param_locator.get('type')}")
                 raise Exception(f"not support this param type {param_locator.get('type')}")
             if param_locator.get('wait_for'):
                 wait_for = [param_locator.get('wait_for')] if isinstance(param_locator.get('wait_for'),
                                                                          dict) else param_locator.get('wait_for')
                 for wait_for_ in wait_for:
                     if wait_for_.get('type') == 'timeout':
                         self.page.wait_for_timeout(wait_for_.get('timeout'))
@@ -977,14 +988,15 @@
                                 value = locator.first.inner_text()
                         else:
                             value = None
                     else:
                         value = str(locator)
                     result[key] = value
                 else:
+                    logging.exception(f'not support the key {key}')
                     raise KeyError(f'not support the key {key}')
         if result:
             if len(result.keys()) == 1:
                 return result.get(keys[0])
             else:
                 return result
         else:
@@ -1039,47 +1051,9 @@
             self.__context.close()
             self.__browser.close()
             self.__playwright.stop()
             logging.info('close browser and playwright')
 
 
 if __name__ == '__main__':
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.DEBUG,
-                        stream=sys.stdout)
-    with BasePage('10.5.24.96', 'adm', '123456', 'https', 443, model='ig902') as my_page:
-        # system = (
-        #     '3rd party notification', '3rd party notification', 'cloud edge computing.azure iot edge',
-        #     'cloud edge computing.aws iot greengrass',
-        #     'device supervisor',
-        #     'device supervisor.measure monitor.group', 'device supervisor.alarm', 'device supervisor.alarm.alarm rules',
-        #     'device supervisor.alarm.history alarms', 'device supervisor.alarm.alarm label', 'device supervisor.cloud',
-        #     'device supervisor.cloud.whitehawk energy manager',
-        #     'device supervisor.protocol', 'device supervisor.protocol.iec 104 server',
-        #     'device supervisor.protocol.opcua server',
-        #     'device supervisor.protocol.modbus rtu slave', 'device supervisor.parameter settings',
-        #     'device supervisor.custom quickfunctions',
-        #     'device supervisor.cloud.whitehawk energy manager',
-        #     'device supervisor.protocol.iec 104 server',)
-        for i in range(0, 1):
-            my_page.access_menu(f'system.inhand_cloud.inhand connect service')
-            my_page.page.wait_for_timeout(2 * 1000)
-            my_page.access_menu(f'system.inhand_cloud.inhand device manager')
-            my_page.access_menu(f'system.inhand_cloud.inhand device manager')
-            my_page.access_menu(f'system.inhand_cloud.inhand iscada cloud')
-            my_page.access_menu(f'system.inhand_cloud.inhand iscada cloud')
-        # a = my_page.get_text('language', [('language', {'locator': my_page.page.frame_locator('#window_content').locator('#_f_hostname'), 'type': 'fill'})])
-        # print(a)
-    # with BasePage('10.5.24.96', 'adm', '123456', model='IG902') as my_page:
-    #     my_page.access_menu('edge_computing.device_supervisor.measure_monitor')
-    #     my_page.page.wait_for_timeout(1000)
-    #     my_page.access_menu('edge_computing.device_supervisor.protocol')
-    #     my_page.page.wait_for_timeout(1000)
-    # user_table = Table(
-    #     [('mode', 'input'), ('status', 'input'), ('ssid', 'input'),  ('mac', 'input'),
-    #      ('auth', 'input'), ('encry', 'input'), ('network', 'input'), ('gateway', 'input'), ('dns', 'input'), ('time', 'input')],
-    #     my_base.page.frame_locator('#window_content').locator('#wifi-2g-grid'),
-    #     ['mode', 'status', 'ssid', 'mac', 'auth', 'encry', 'network', 'gateway', 'dns', 'time'], None)
-    # a = user_table.exists([{'mode': "'${value}'!='AP'", 'ssid': 'inhand-visitor-2g'}])
-    # print(a)
-    # print(user_table.exist(locale={'disable': 'Disabled'}, mode="'${value}'!='AP'", ssid='inhand-visitor-2g', status='disable'))
-    # user_table.delete(name='test2', value='222')
-    # my_base.page.wait_for_timeout(5 * 1000)
+    pass
+
```

### Comparing `inhandtest-0.0.55/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.56/inhandtest/base_page/table_tr.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # @Time    : 2023/3/21 10:13:10
 # @Author  : Pane Li
 # @File    : table_tr.py
 """
 table_tr
 
 """
-import logging
 import re
 from typing import List
 from inhandtest.tools import replace_str
 from playwright.sync_api import Locator, TimeoutError
+import logging
 
 
 class Table:
 
     def __init__(self, columns: list, table_locator: Locator, unique_columns: list, locale: dict = None, log_desc=None):
         """
 
@@ -60,14 +60,15 @@
                     self.tr.locator('//td').locator(f'.fi{column[0] + 1}').first.select_option(option)
                 elif column[2] == 'check':
                     if column[1] in ('check', 'Yes', '是', 'yes'):
                         self.tr.locator('//td').locator(f'.fi{column[0] + 1}').first.check()
                     else:
                         self.tr.locator('//td').locator(f'.fi{column[0] + 1}').first.uncheck()
                 else:
+                    logging.exception(f'not support this type {column[2]}')
                     raise Exception(f'not support this type {column[2]}')
 
     def exist(self, find_one=True, locale=None, **kwargs) -> int or None or List[int]:
         """ 传入的资源是否存在, 对于check 项是不计入重复选项的，因为勾选其实只是开启功能而已
 
 
         :param find_one: 是否只查询一个，当查询一个时返回的是int值，索引从0 开始， 当没查询到时返回的是None
@@ -155,14 +156,15 @@
                     action_attribute = self.tr.get_by_role('button').nth(i).get_attribute('onclick')
                     if action_attribute in (
                             "TGO(this).onDelete()", "TGO(this).footerDel()", 'footerDel()', 'delete_save(this)'):
                         if not self.tr.get_by_role('button').nth(i).is_disabled():
                             self.tr.get_by_role('button').nth(i).click()
                             break
                         else:
+                            logging.exception(f'the data in the row {nth} cannot be deleted')
                             raise TimeoutError  # 第一行的数据不能删除，走到第二行去
                 else:
                     break  # 所有行都走完了却没有删除按钮，也需要退出去
             except TimeoutError:
                 nth = nth + 1
         logging.info('table resource all delete')
```

### Comparing `inhandtest-0.0.55/inhandtest/exception.py` & `inhandtest-0.0.56/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/file.py` & `inhandtest-0.0.56/inhandtest/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # @Author  : Pane Li
 # @File    : file.py
 """
 file
 
 """
 import os
-import logging
 import random
 import string
+import logging
 
 
 def del_file(file_path: str) -> None:
     """删除指定路径下的所有文件或单个文件
 
     :param file_path:
     :return:
@@ -42,17 +42,19 @@
         if os.path.exists(file_path_or_file_dir):
             logging.debug(f"check dir {file_path_or_file_dir} ok")
         else:
             if create_dir:
                 os.mkdir(file_path_or_file_dir)
                 logging.debug(f"create dir {file_path_or_file_dir} ok")
             else:
+                logging.exception(f"this dir {file_path_or_file_dir} not exist")
                 raise FileNotFoundError(f"this file {file_path_or_file_dir} not exist")
     else:
         if not os.path.isfile(file_path_or_file_dir):
+            logging.exception(f"this file {file_path_or_file_dir} not exist")
             raise FileNotFoundError(f"this file {file_path_or_file_dir} not exist")
         else:
             logging.debug(f"check file {file_path_or_file_dir} ok")
 
 
 def generate_str_or_file(size: int or str = '48KB', file_path=None) -> str:
     """生成指定大小字符串或文件 1024KB=1MB  1024MB=1GB  1024GB=1TB
@@ -69,14 +71,15 @@
         elif 'MB' in size:
             size = int(float(size.replace('MB', '')) * 1024 * 1024)
         elif 'GB' in size:
             size = int(float(size.replace('GB', '')) * 1024 * 1024 * 1024)
     elif isinstance(size, int):
         pass
     else:
+        logging.exception(f'param {size} type {type(size)} error, only can be str or int!')
         raise Exception(f'param {size} type {type(size)} error, only can be str or int!')
     if size:  # 都已经转换为byte
         str_ = ''.join(random.choice(string.ascii_letters + string.digits) for _ in range(size))
         if os.path.isfile(file_path):  # 生成文件
             with open(file_path, 'w') as file:
                 file.write(str_)
             logging.debug(
@@ -95,14 +98,15 @@
     if hash_type.lower() == 'md5':
         obj = md5()
     elif hash_type.lower() == 'sha1':
         obj = sha1()
     elif hash_type.lower() == 'sha256':
         obj = sha256()
     else:
+        logging.exception(f'Not support this hash_type {hash_type}')
         raise Exception(f'Not support this hash_type {hash_type}')
     if os.path.isfile(file_path_or_msg):
         with open(file_path_or_msg, 'rb') as f:
             obj.update(f.read())
     else:
         obj.update(file_path_or_msg.encode('utf-8'))
     return obj.hexdigest().upper()
```

### Comparing `inhandtest-0.0.55/inhandtest/inmodbus.py` & `inhandtest-0.0.56/inhandtest/inmodbus.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 
 import modbus_tk
 import modbus_tk.defines as cst
 import serial
 import math
 import struct
-import logging
 import ctypes
 import re
 from modbus_tk import modbus_rtu, modbus_tcp, utils
+import logging
 
 
 class ModbusMaster:
     __doc__ = "使用前需安装pyserial, modbus-tk"
 
     def __init__(self, protocol: str, host: str, port=502, slave_id=1, baud_rate=9600, bytesize=8, parity='N',
                  stop_bits=1):
@@ -29,25 +29,26 @@
         :param port: 端口号
         :param slave_id: 从站地址
         :param baud_rate: 串口波特率
         :param bytesize: 数据位
         :param parity: 校验位 N| O| E
         :param stop_bits: 停止位
         """
-        self.logger = utils.create_logger("console", level=logging.DEBUG)
+        self.logging = utils.create_logger("console", level=logging.DEBUG)
         try:
             if protocol.upper() == 'TCP':
                 self.master = modbus_tcp.TcpMaster(host=host, port=port)
             else:
                 self.uart = serial.Serial(host, baudrate=baud_rate, bytesize=bytesize, parity=parity, stopbits=stop_bits)
                 self.master = modbus_rtu.RtuMaster(self.uart)
             self.master.set_timeout(5.0)
             self.master.set_verbose(True)
-            self.logger.info("connected")
+            self.logging.info("connected")
         except modbus_tk.modbus_rtu.ModbusInvalidResponseError as err:
+            logging.exception("ModbusInvalidResponseError")
             raise err
         self.slave_id = slave_id
 
     def read_data(self, addr: str, datatype: str, length=0, decimal=0):
         """
         根据数据类型读指定寄存器地址
         :param addr: 寄存器地址
@@ -56,15 +57,15 @@
         :param decimal: datatype为float类型时，必填项
         :return:
         """
         function_code_dict = {'0': cst.READ_COILS, '1': cst.READ_DISCRETE_INPUTS, '3': cst.READ_INPUT_REGISTERS,
                               '4': cst.READ_HOLDING_REGISTERS}
         function_code = function_code_dict[addr[0]]
         # print('function code is %s' % function_code)
-        self.logger.info('PLC address function code is %s.' % function_code)
+        self.logging.info('PLC address function code is %s.' % function_code)
         type_ = datatype.upper()
         data = None
         if function_code in [1, 2] and type_ == 'BIT':
             return self.master.execute(self.slave_id, function_code, int(addr[1:]) - 1, 1)[0]
         elif function_code in [3, 4] and type_ in \
                 ['INT', 'WORD', 'DINT', 'DWORD', 'LONG', 'ULONG', 'BCD', 'FLOAT', 'DOUBLE', 'STRING']:
             if type_ == 'INT':
@@ -89,18 +90,18 @@
             elif type_ == 'STRING':
                 data_tuple = self.read_holding_registers(addr, function_code, (length + 1) // 2, symbol=False)
                 data = self.read_not_16int_data(data_tuple, datatype=type_)[:length]
             else:
                 pass
             if type_ in ['FLOAT', 'DOUBLE']:
                 data = round(data, decimal)
-            self.logger.info(f'PLC address {addr} read data is {data}')
+            self.logging.info(f'PLC address {addr} read data is {data}')
             return data
         else:
-            self.logger.error(f'Datatype Error')
+            self.logging.exception(f'Datatype Error')
             raise Exception('The current register address does not match the data type.')
 
     def write_data(self, addr: str, datatype: str, write_value):
         """
         都指定寄存器地址写入值
         :param addr: 寄存器地址
         :param datatype: datatype
@@ -109,14 +110,15 @@
         """
         type_ = datatype.upper()
         address = int(addr[1:]) - 1
         if isinstance(write_value, str) and type_ != 'STRING':
             write_value = int(write_value)
         if addr[0] == '0':
             if write_value not in [0, 1, True, False]:
+                logging.exception('This address type does not support writing such values.')
                 raise Exception('This address type does not support writing such values.')
             else:
                 self.master.execute(self.slave_id, cst.WRITE_MULTIPLE_COILS, address, output_value=[write_value])
         elif addr[0] == '4':
             if type_ == 'FLOAT':
                 self.write_float_data(addr, write_value)
             elif type_ == 'INT':
@@ -134,14 +136,15 @@
                 elif type_ == 'STRING':
                     value = write_value.ljust(math.ceil(len(write_value)/2) * 2)
                 else:
                     value = write_value
                 value_list = self.write_not_int16_data(value, type_)
                 self.master.execute(self.slave_id, cst.WRITE_MULTIPLE_REGISTERS, address, output_value=value_list)
         else:
+            logging.exception('This address type does not support write operations.')
             raise Exception('This address type does not support write operations.')
 
     def read_holding_registers(self, addr, function_code, number, symbol=True):
         """
         读取寄存器
         if start==42,读取x轴坐标，需要除以1000
         :param addr:
@@ -152,15 +155,15 @@
         """
         start = int(addr[1:]) - 1
         if symbol:
             data_format = ">" + (number * "h")
             data = self.master.execute(self.slave_id, function_code, start, number, data_format=data_format)
         else:
             data = self.master.execute(self.slave_id, function_code, start, number)
-        self.logger.info(f'PLC address {addr} read tuple is {data}')
+        self.logging.info(f'PLC address {addr} read tuple is {data}')
         return data
 
     def read_float_data(self, addr, function_code):
         """
         读取单精度类型浮点数
         :param addr: 地址
         :param function_code: 功能码
@@ -207,14 +210,15 @@
             elif datatype == 'LONG':
                 struct_format = '!q'
             elif datatype == 'DOUBLE':
                 struct_format = '!d'
             # elif datatype == 'STRING':
             #     struct_format = '!p'
             else:
+                logging.exception('NonsupportDataType')
                 raise Exception('NonsupportDataType')
             data = struct.unpack(struct_format, data_bytes)[0]
             return data
 
     @staticmethod
     def write_not_int16_data(value, datatype):
         """
@@ -231,38 +235,21 @@
             if datatype == 'DINT':
                 struct_format = '!i'
             elif datatype == 'LONG':
                 struct_format = '!q'
             elif datatype == 'DOUBLE':
                 struct_format = '!d'
             else:
+                logging.exception('NonsupportDataType')
                 raise Exception('NonsupportDataType')
             y_bytes = struct.pack(struct_format, value)
             # print(y_bytes)
             # y_hex = bytes.hex(y_bytes)
             y_hex = ''.join(['%02x' % i for i in y_bytes])
             eval_val = re.findall(r'.{4}', y_hex)
         value_list = []
         for val in eval_val:
             val = int(val, 16)
             # print(val)
             value_list.append(val)
         return value_list
 
-
-if __name__ == "__main__":
-    tcpMaster = ModbusMaster(protocol='TCP', host='10.5.23.84', port=502, slave_id=1)
-    print(tcpMaster.write_data("40001", datatype='STRING', write_value='A'))
-    print(tcpMaster.read_data("40001", datatype='STRING', length=1, decimal=2))
-    # print(tcpMaster.read_data("40001", datatype='INT', length=3, decimal=2))
-    # print(tcpMaster.read_data("40001", datatype='WORD', length=3, decimal=2))
-    # print(tcpMaster.read_data("40001", datatype='DINT', length=3, decimal=2))
-    # print(tcpMaster.read_data("40001", datatype='DWORD', length=3, decimal=2))
-    # print(tcpMaster.read_data("40001", datatype='DOUBLE', length=3, decimal=2))
-    # print(tcpMaster.read_data("40001", datatype='FLOAT', length=3, decimal=2))
-    # print(tcpMaster.read_data("40001", datatype='LONG', length=3, decimal=2))
-    # print(tcpMaster.read_data("40001", datatype='ULONG', length=3, decimal=2))
-    # tcpMaster.write_float_data(40001, value=3.156)
-    # print(tcpMaster.write_not_int16_data(value='ABCDEF', datatype='STRING'))
-    # rtuMaster = ModbusMaster(protocol='RTU', host='COM10', port=502, slave_id=1)
-    # rtuMaster.read_holding_registers('40001', cst.READ_HOLDING_REGISTERS, 1, symbol=False)
-    # print(rtuMaster.read_data("40001", datatype='INT', length=3, decimal=2))
```

### Comparing `inhandtest-0.0.55/inhandtest/inmongodb.py` & `inhandtest-0.0.56/inhandtest/inmongodb.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # @Time    : 2023/4/23 17:18:24
 # @Author  : Pane Li
 # @File    : inmongodb.py
 """
 inmongodb
 
 """
-import logging
 from pymongo import MongoClient
+import logging
 
 
 class Mongodb:
     """mongodb数据库操作类
 
     数据类型：
             ObjectId： from bson.objectid import ObjectId   ex: ObjectId("5f1f5b9d9c1b9b0b8c8b4567")
@@ -114,19 +114,7 @@
         :param db: 数据库
         :param collection: 集合
         :param data: 数据     [{'$match': {'name': 'liwei'}}]
         :return:
         """
         return list(self.client[db][collection].aggregate(data))
 
-
-if __name__ == '__main__':
-    mongodb = Mongodb('10.5.17.102', 27017, 'root', 'admin', )
-    from bson.objectid import ObjectId
-
-    # mongdodb 不等于条件查询
-
-    cursor = mongodb.find('nezha_iot', 'devices', {'serialNumber': 'RT805LIWEI82113'})[0]
-    print(cursor.get('_id'))
-    # for doc in cursor:
-    #     print(doc)
-    # print(mongodb.aggregate('test', 'test', [{'$match': {'name': 'liwei111'}}]))
```

### Comparing `inhandtest-0.0.55/inhandtest/inmqtt.py` & `inhandtest-0.0.56/inhandtest/inmqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # @Author  : HengYi Li
 # @File    : inmqtt.py
 """
 inmqtt
 
 """
 import json
-import logging
 import os
 import re
 import subprocess
 import uuid
 import time
 from paho.mqtt import client
 from inhandtest.tools import dict_flatten, check_windows_process
 from inhandtest.file import check_file
+import logging
 
 
 class MqttClient:
     __doc__ = "使用前需安装paho-mqtt  pip install paho-mqtt"
 
     def __init__(self, host: str, port: int = 1883, username=None, password=None, client_id=None, clean_session=True,
                  reconnect_on_failure=True, keepalive=120):
@@ -63,15 +63,16 @@
             logging.info(f"{client} Connection success, id: {self.client_id}")
             self.connect_time = int(time.time())
         else:
             logging.error(f'client {self.client_id} connect failed, code=%s' % rc)
 
     def __on_message(self, client, userdata, message):
         try:
-            logging.debug(f"client {self.client_id} recv topic '{message.topic}', payload {json.loads(message.payload)}")
+            logging.debug(
+                f"client {self.client_id} recv topic '{message.topic}', payload {json.loads(message.payload)}")
             self.recv_datas.append((message.topic, json.loads(message.payload), int(round(time.time() * 1000))))
         except Exception:
             logging.error(f'client {self.client_id} recv exception data: {message.payload}')
 
     def __on_subscribe(self, client, userdata, mid, granted_qos):
         logging.debug(f'On Subscribed: mid={mid}, qos={granted_qos}')
 
@@ -201,37 +202,41 @@
                                     if len(topic_payloads) >= 2:
                                         fist_time = topic_payloads[0][2]  # 取第一条的第3个元素
                                         for time_payload in topic_payloads[1:]:
                                             if assert_payload.get('time_interval')[0] <= time_payload[2] - fist_time <= \
                                                     assert_payload.get('time_interval')[1]:
                                                 fist_time = time_payload[2]
                                             else:
+                                                logging.exception(f"current data time is  {time_payload[2]},  last data time is {fist_time}")
                                                 raise AssertionError(
                                                     f"current data time is  {time_payload[2]},  last data time is {fist_time}")
                                 if assert_payload:
                                     def payload_verify(x):
                                         if x[0] == topic:
                                             expect_payload_ = dict_flatten(assert_payload)  # 平铺字典
                                             r_payload_ = dict_flatten(x[1])
                                             for expect_item_, expect_value_ in expect_payload_.items():
                                                 if expect_item_ not in ('number', 'exist', 'time_interval'):
                                                     value_ = r_payload_.get(expect_item_)
                                                     expect_value_ = str(expect_value_).replace('${value}', str(value_))
                                                     if not eval(expect_value_):
-                                                        logging.debug(expect_value_)
+                                                        logging.exception(expect_value_)
                                                         raise AssertionError(
                                                             f'payload error parm {expect_item_} value is {expect_value_} is False')
 
                                     [payload_verify(data_) for data_ in self.recv_datas]
                             else:
+                                logging.exception('param expect_recv_rules topic value must be boolean or dict')
                                 raise Exception('param expect_recv_rules topic value must be boolean or dict')
                 else:
+                    logging.exception('param expect_recv_rules must be dict')
                     raise Exception('param expect_recv_rules must be dict')
                 logging.info("analysis data is ok")
         except Exception:
+            logging.exception('analysis data is error')
             raise
         finally:
             self.recv_datas = []
 
 
 class MosquittoBrokerWindows:
     __doc__ = "使用mosquitto 搭建mqtt server, 使用前需要确保mosquitto 正确安装到windows上面"
@@ -388,30 +393,16 @@
                                 assert re.findall(key, logs), f"expect rule message {key} receive None"
                             else:
                                 assert not re.findall(key, logs), f"expect rule message {key} receive any"
                         elif (isinstance(value, tuple) or isinstance(value, list)) and len(value) == 2:
                             assert value[0] <= len(re.findall(key, logs)) <= value[
                                 1], f"expect rule message {key} number is error"
                         else:
+                            logging.exception(f"param rules error")
                             raise Exception('param rules error')
                 except Exception:
+                    logging.exception(f"analysis {log} log is error")
                     raise
                 finally:
                     if clear_log:
                         open(self.broker_log_file, 'w').close()
                 logging.info(f"analysis {log} log is ok")
-
-
-if __name__ == '__main__':
-    import sys
-
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
-                        stream=sys.stdout)
-    a = MosquittoBrokerWindows()
-    # a.close_server_and_expect_log(broker_log_rules={"New connection from 192.168.2.102:52621 on port 1883": (5, 5)},
-    #                               timeout=1)
-    a.start_mosquitto_broker()
-    # a.close()
-    # a.broker_user("liwei1", "123456")
-    # c = MqttClient('10.5.47.199', 1085)
-    # c.sub('v1/#')
-    # c.expect_data({"number": (1, 100000)}, 30)
```

### Comparing `inhandtest-0.0.55/inhandtest/inrequest.py` & `inhandtest-0.0.56/inhandtest/inrequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 # @Author  : Pane Li
 # @File    : inrequest.py
 """
 封装request， 使设备和平台都能来正常调用，统一入口，token过期时也能自动更新
 
 """
 import base64
-import logging
 import os
 import re
-import sys
 import time
 from typing import List
 import urllib3
 import requests
 from inhandtest.exception import ParameterValueError, UsernameOrPasswordError, TimeOutError, UpgradeFailedError, \
     ResourceNotFoundError
 from inhandtest.file import file_hash
 from inhandtest.tools import dict_in, dict_merge, replace_str, DotDict, loop_inspector
+import logging
 
 
 class DnInterface:
     def __init__(self, username, password, host='c.inhand.com.cn'):
         """
         :param username  平台用户名
         :param password  平台密码
@@ -44,14 +43,15 @@
         def get_model_id(model_name: str) -> str:
             models = self.api.send_request('api/models', method='get', param={'limit': 0, 'verbose': 1}).json().get(
                 'result')
             for model_ in models:
                 if model_.get('name').upper() == model_name.upper():
                     return model_.get('_id')
             else:
+                logging.exception(f"the model {model_name} not found")
                 raise ResourceNotFoundError(f"the model {model_name} not found")
 
         for i in range(3):
             response = self.api.send_request('api/devices', method='get',
                                              param={"verbose": 100, "limit": 10, "cursor": 0,
                                                     'serial_number': sn, 'plc_id': 0})
             if response.json().get('total') == 0:
@@ -120,14 +120,15 @@
                                                     'serial_number': sn})
             if response.json().get('total') == 1:
                 logging.debug(f'check {sn} device exist')
                 break
             logging.info(f'check {sn} device is not exist, please wait for {interval}s')
             time.sleep(interval)
         else:
+            logging.exception(f'{self.host} {self.username} account not found device {sn}')
             raise TimeOutError(f'{self.host} {self.username} account not found device {sn}')
 
     def device_state(self, sn: list) -> List[dict]:
         """根据sn 转换属性 属性值有：  online: 在线|离线   1|0
                                        iccid:
                                        imei:
                                        imsi:
@@ -230,14 +231,15 @@
                             break
                 else:
                     logging.info(f"check {sn} device all state success")
                     break
                 logging.info(f"check {sn} device state failed, please wait for {interval}s")
                 time.sleep(interval)
             else:
+                logging.exception(f"the {sn} state {state} check failed")
                 raise TimeOutError(f"the {sn} state {state} check failed")
 
     def send_config_online(self, sn: str or list, config: str) -> List[str]:
         """下发配置， 多台时仍然是一台一台下发的， 注意逻辑 设备必须是在线的才能下发
 
         :param config: 配置命令，多个配置用'\n'隔开
         :param sn: 一台设备或多台设备
@@ -280,20 +282,22 @@
                                                              'timeout': 30000,
                                                              'type': "4"}).json().get('result').get('state')
                     assert task_state == 3, "GET RUNNING CONFIG task status error!"
                     break
                 except Exception as e:
                     logging.error(f'get running config task status reason is {e}, try {i + 2} again')
             else:
+                logging.exception(f'device {sn} get running config task status failed')
                 raise Exception(f'device {sn} get running config task status failed')
             config_content = self.api.send_request(f'api/devices/{device_id}/config', 'get').json().get('result').get(
                 'content')
             if config:
                 assert set(config.split('\n')).issubset(set(config_content.split('\n'))), f'config {config} not exist'
         else:
+            logging.exception(f'the {sn} device not exist or offline')
             raise ResourceNotFoundError(f'the {sn} device not exist or offline')
 
     def upgrade_firmware_online(self, sn: str, firmware: str, timeout=10 * 60, interval=10) -> None:
         """ 升级固件， 保障升级成功不然就会报错
 
         :param sn: 设备序列号
         :param firmware: 升级的固件，本地全路径
@@ -327,14 +331,15 @@
                         body = {'fid': upload_file['_id'], 'jobTimeout': 30, 'model': model(file_name),
                                 'name': file_name,
                                 'version': version(file_name), 'desc': 'auto test upload firmware'}
                         firmware_id = self.api.send_request('api/firmware', 'post', body=body, ).json().get(
                             'result').get(
                             '_id')
                     else:
+                        logging.exception(f'{firmware} not exist')
                         raise FileNotFoundError(f'{firmware} not exist')
                 else:
                     logging.debug(f'This file {firmware} already exists on the cloud {self.host} {self.username}')
                     firmware_id = get_firmware.get('result')[0].get('_id')
                 # 已完成固件上传
                 job_id = self.api.send_request(f'api/device/{device_id}/upgrade', method='post',
                                                body={'deviceName': device_name, 'firmwareId': firmware_id,
@@ -347,23 +352,27 @@
                     job = [job for job in job_response if job.get('_id') == job_id]
                     if len(job) == 1:
                         if job[0].get('_id') == job_id:
                             if job[0].get('state') == 3:
                                 logging.info(f"upgrade to {file_name} success!")
                                 break
                             elif job[0].get('state') == -1:
+                                logging.exception(f'upgrade to {file_name} failed!')
                                 raise UpgradeFailedError(f'upgrade to {file_name} failed!')
                     else:
+                        logging.exception(f'upgrade to {file_name} failed!')
                         raise UpgradeFailedError('create upgrade task failed!')
                 else:
+                    logging.exception(f'upgrade to {file_name} timeout!')
                     raise TimeOutError('upgrade job check timeout')
                 self.assert_device_state(sn, state={'version': '"${value}" in ' + f'"{file_name}"'}, timeout=300)
             else:
                 logging.debug(f'{firmware} not is file or version of same ')
         else:
+            logging.exception(f'the device {sn} is offline or not exist')
             raise Exception(f'the device {sn} is offline or not exist')
 
     def upgrade_firmware(self, sn: str or list, firmware: str) -> None:
         """ 升级固件，只管下发升级任务，不监督是否升级成功
 
         :param sn: 设备序列号
         :param firmware: 升级的固件，本地全路径
@@ -393,14 +402,15 @@
                     body = {'fid': upload_file['_id'], 'jobTimeout': 30, 'model': model(file_name),
                             'name': file_name,
                             'version': version(file_name), 'desc': 'auto test upload firmware'}
                     firmware_id = self.api.send_request('api/firmware', 'post', body=body, ).json().get(
                         'result').get(
                         '_id')
                 else:
+                    logging.exception(f'{firmware} not exist')
                     raise FileNotFoundError(f'{firmware} not exist')
             else:
                 logging.debug(f'This file {firmware} already exists on the cloud {self.host} {self.username}')
                 firmware_id = get_firmware.get('result')[0].get('_id')
             self.api.send_request(f'api/firmware/{firmware_id}/devices', method='post',
                                   body={'deviceIds': [device.get('id') for device in devices], 'deviceGroupIds': [], })
         else:
@@ -432,16 +442,18 @@
                 try:
                     ngrok = self.api.send_request('api2/tasks/run', method='post', body=body).json()
                     if ngrok["result"]["data"]["response"]:
                         return ngrok["result"]["data"]["response"]
                 except Exception as e:
                     logging.error(f"ngrok request failed reason is {e}, try {i + 2} again")
             else:
+                logging.exception(f'Device {sn} get ngrok failed.')
                 raise Exception(f'Device {sn} get ngrok failed.')
         else:
+            logging.exception(f'the device {sn} is offline or not exist')
             raise ResourceNotFoundError(f'the {sn} is not exist or offline')
 
     def reboot_online(self, sn: str) -> None:
         """DM平台设备重启
         """
         response = self.api.send_request('api/devices', method='get',
                                          param={"verbose": 100, "limit": 10, "cursor": 0,
@@ -449,14 +461,15 @@
         if response.json().get('total') == 1 and response.json().get('result')[0].get('online') == 1:
             device_id = response.json().get('result')[0].get('_id')
             logging.debug(f'{self.host} send to {sn} reboot command')
             status = self.api.send_request(f'api/device/{device_id}/methods', 'post',
                                            body={'method': "reboot", 'timeout': 15000}).json().get('status')
             assert status == 'succeeded', 'reboot error!'
         else:
+            logging.exception(f'the device {sn} is offline or not exist')
             raise ResourceNotFoundError(f'the {sn} is not exist or offline')
 
     def remote_maintenance_online(self, sn: str, protocol='http', port=80, local_host='192.168.2.1',
                                   action='connect') -> str or None:
         """封装dm远程维护方法
 
         :param sn，必须在线
@@ -495,14 +508,15 @@
                     for i in range(0, 3):
                         connect = self.api.send_request(f'/api/touch/tunnels/{tunnel_id}/connect', 'put').json()
                         if connect.get('result').get('connected'):
                             pub_url = connect.get('result').get('publicUrl')
                             logging.info(f'tunnel {tunnel_des} connect success')
                             break
                     else:
+                        logging.exception(f'tunnel {tunnel_des} connect failed')
                         raise ConnectionError(f'tunnel {tunnel_des} connect failed')
                 else:
                     logging.debug(f'tunnel {tunnel_des} already connect')
                 return pub_url
             elif action == 'disconnect' and device[0].get('online'):
                 if tunnel_id and tunnel_status:
                     self.api.send_request(f'/api/touch/tunnels/{tunnel_id}/disconnect', 'put')
@@ -570,14 +584,15 @@
                                 body = {'serialNumber': sn, 'name': sn + str(int(time.time())),
                                         'lanInterface': lan_interface,
                                         'subnet': subnet}
                                 self.api.send_request('api/invpn/router', 'post', {'oid': self.oid}, body=body)
                                 logging.info(f'add device {sn} to cloud {self.host} successfully')
                             break
                     else:
+                        logging.exception(f'the Serial number {sn} and model do not match ')
                         raise Exception(f'the Serial number {sn} and model do not match ')
 
     def device_state(self, sn: list) -> List[dict]:
         """根据sn 转换属性 属性值有：  online: 在线|离线   1|0
                                        connected: true | None
                                        iccid:
                                        imei:
@@ -774,14 +789,15 @@
                             break
                 else:
                     logging.info(f"check {sn} device all state success")
                     break
                 logging.info(f"check {sn} device state failed, please wait for {interval}s")
                 time.sleep(interval)
             else:
+                logging.exception(f"the {sn} state {state} check failed")
                 raise TimeOutError(f"the {sn} state {state} check failed")
 
     def delete_device(self, sn: str or list) -> None:
         """
 
         :param sn: 设备序列号，一个或多个
         :return:
@@ -924,22 +940,25 @@
                 res = requests.delete(url, params=param, headers=header, verify=False)
         elif method == 'PUT':
             if params_type == 'JSON':
                 res = requests.put(url, json=body, params=param, headers=header, verify=False)
             else:
                 res = requests.put(url, data=param, headers=header, verify=False)
         else:
+            logging.exception(f"requests method {method} not support")
             raise ParameterValueError(f"requests method {method} not support")
         logging.debug(f'Requests Method:[{method}] Code: {res.status_code} URL: {url}, Param: {param}, Body: {body}')
         if res.status_code != 401:
             if self.type_ == 'device':
                 if res.status_code == 404:
+                    logging.exception(f"not support API login")
                     raise Exception('not support API login')
                 if res.status_code == 200 and 'login' in path:
                     if 'error' in res.json().keys():
+                        logging.exception(f"UsernameOrPasswordError")
                         raise UsernameOrPasswordError
             res.encoding = 'utf-8'  # 如返回内容有中文的需要编码正确
             try:
                 logging.debug(f'Requests Response json is {res.json()}')
             except Exception:
                 logging.warning(f'Requests Response json is None')
         else:
@@ -957,28 +976,14 @@
                         elif isinstance(i, dict):
                             dict_in(res.json(), i)
             elif isinstance(expect, dict):
                 dict_in(res.json(), expect)
             elif isinstance(expect, str) or isinstance(expect, int):
                 assert str(expect) in res.text, f"Response text {res.text} Does not contain {expect}"
             else:
+                logging.exception(f'expect param type error！')
                 raise ValueError('expect param type error！')
         return res
 
 
 if __name__ == "__main__":
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO, stream=sys.stdout)
-    # testApi = StarInterface('liwei@inhand.com.cn', '123456', 'star.nezha.inhand.dev')
-    api = DnInterface('smoke@inhand.com.cn', 'smoke@inhand', 'c.inhand.com.cn', )
-    api.add_device('RL6152315576161', '00:18:05:29:12:AB', 'IR6XX_EVDO')
-    api.delete_device('RL6152315576161')
-    # testApi.remote_maintenance_online('RF3052213006490', )
-    # testApi.add_device({'RF3052213006490': 'IR305'})
-    # print(testApi.web_remote_online('RF3052213006490'))
-    # testApi.device_exist('VG7512022009918')
-    # testApi.get_config_online('VG7512022009918', 'hello\r\nword')
-    # testApi.send_config_online('VG7512022009918', 'hello\nword')
-    # testApi.send_openvpn_config('RF3022206089272')
-    # print(testApi.remote_maintenance_online('RF3052213006490', action='delete'))
-    # print(re.findall('V(.*).bin', 'IR9-V1.0.0.r10190.bin')[0])
-    # # testApi.get_config_online('RF3052213006490', 'dhcpd_start=192.168.2.3')
-    # testApi.assert_device_state('RF3022206089272', state={'online': 1, 'connected': True})
+    pass
```

### Comparing `inhandtest-0.0.55/inhandtest/inserial.py` & `inhandtest-0.0.56/inhandtest/inserial.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 # @Time    : 2023/5/6 9:24:33
 # @Author  : Pane Li
 # @File    : inserial.py
 """
 inserial
 
 """
-import logging
 from threading import Thread
 from inhandtest.tools import check_windows_process
 from serial import *
 from serial.tools import list_ports
 from inhandtest.exception import *
+import logging
 
 
 class InSerial:
 
     def __init__(self, com='', baud_rate=115200, data_bits=8, parity='none', stop_bit=1, flow_control=False,
                  timeout=1, username='adm', password='123456'):
         """ 在使用串口做功能配置时需关闭日志服务器，避免影响功能，如果在接收日志时可不登录, 使用with 语句主动关闭串口
@@ -76,26 +76,28 @@
             if flag in (self.__config_flag, self.__super_flag, self.__normal_flag, self.__user_flag):
                 pass
             elif 'login:' in flag:
                 self.send_cli({username: ":"})
                 self.serial.write((password + '\n').encode('gbk'))
                 login_flag = self.serial.read_until('>'.encode("gbk")).decode("gbk")
                 if ' \r\n' == login_flag:
+                    logging.exception(f'Username Or Password Error')
                     raise UsernameOrPasswordError
                 else:
                     tag = login_flag.split('\r\n')[-1].strip().replace('>', '')
                     self.__user_flag = f'{tag}#'
                     self.__normal_flag = f'{tag}>'
                     logging.debug(login_flag)
                     pass
             else:
-                logging.error(f'Serial Connect {self.com} Failed')
+                logging.exception(f'Serial Connect {self.com} Failed')
                 raise ConnectionError
             logging.info(f'Serial Connect {self.com} Successful')
         except Exception:
+            logging.exception(f'Serial Connect {self.com} Failed')
             raise ConnectionError
 
     def __open(self):
         try:
             check_windows_process(['sscom', 'MobaXterm'], True)
         except:
             pass
@@ -109,14 +111,15 @@
         for i in range(0, 30, 3):
             if not self.serial.is_open:
                 self.serial.open()
                 logging.debug(f"open serial {self.com} success")
                 break
             time.sleep(3)
         else:
+            logging.exception(f"open serial {self.com} failed")
             raise SerialException(f'serial {self.com} already used')
 
     def receive_log(self, timeout=20, logs_number=1):
         """接收日志
 
         :param timeout: 接收超时时间
         :param logs_number
@@ -129,14 +132,15 @@
             if data:
                 self.logs_number.append(data.decode())
             if logs_number == len(self.logs_number):
                 break
             else:
                 time.sleep(1)
         else:
+            logging.exception(f'serial com {self.com} read log timeout')
             raise Exception('can not receive logs')
 
     def logout(self):
         self.send_cli({"exit": "[Y|N]", "y": "Press"})
 
     def send_cli(self, command: dict):
         """发送命令，支持多条，
@@ -185,24 +189,13 @@
                 command = "length == len(self.logs_number) and content in ','.join(self.logs_number)"
             if eval(command):
                 logging.info(f"assert data {self.logs_number} ok")
                 break
             else:
                 time.sleep(1)
         else:
+            logging.exception(f"assert data {self.logs_number} failed")
             raise Exception('serial not receive data')
 
 
 if __name__ == '__main__':
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO, stream=sys.stdout)
-    # ss.login(password='123456')
-    # ss.logout()
-    # ss.login()
-    # ss.read_all_and_write()
-    # for i in range(0, 50):
-    #     logging.info(ss.read_all_data)
-    #     time.sleep(1)
-    # ss.read_all_data
-    # ss.config_mode()
-    # result = ss.send_cli({"": "#"})
-    # logging.info(f'1111 {result[0]}')
-    # ss.close()
+    pass
```

### Comparing `inhandtest-0.0.55/inhandtest/insocket.py` & `inhandtest-0.0.56/inhandtest/insocket.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # @Author  : Pane Li
 # @File    : insocket.py
 """
 insocket
 
 """
 
-import logging
 import threading
 import time
 import socket
+import logging 
 
 
 def tcp_server_data(host, port, recv_content: dict = None, connect_time=10,
                     send_msg_to_server: str or list = None, function=None, timeout=5, **kwargs):
     """ 开启tcp_server, 并且接收数据，对数据做验证, 该连接为阻塞式，所以要确保客户端能正常连接过来，还要确保防火墙是关闭的
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
 
@@ -80,29 +80,33 @@
         if all_datas:
             for k, v in recv_content.items():
                 if k == 'content':
                     datas = b''.join([v_ for v_ in all_datas.values()])
                     contents = [v.encode('utf-8')] if isinstance(v, str) else [c_.encode('utf-8') for c_ in v]
                     # 校验数据内容
                     if list(filter(lambda x: x not in datas, contents)):
+                        logging.exception(f'tcp server {host}:{port} all clients not recv  content {v}')
                         raise AssertionError(f'tcp server {host}:{port} all clients not recv  content {v}')
                     else:
                         logging.info(f'tcp server {host}:{port} all clients recv content {v} success')
                 else:
                     datas = all_datas.get(k)
                     if datas is not None:
                         contents = [v.encode('utf-8')] if isinstance(v, str) else [c_.encode('utf-8') for c_ in v]
                         # 校验数据内容
                         if list(filter(lambda x: x not in datas, contents)):
+                            logging.exception(f'tcp server {host}:{port} client {k} not recv content {v}')
                             raise AssertionError(f'tcp server {host}:{port} client {k} not recv content {v}')
                         else:
                             logging.info(f'tcp server {host}:{port} client {k} recv content {v} success')
                     else:
+                        logging.exception(f'tcp server {host}:{port} client {k} not connected')
                         raise AssertionError(f'tcp server {host}:{port} client {k} not connected')
         else:
+            logging.exception(f'tcp server {host}:{port} client not connected')
             raise AssertionError(f'tcp server {host}:{port} client not connected')
 
 
 def tcp_client_data(server: tuple, client: tuple = None, recv_content: str or list = None, connect_time=10,
                     send_msg_to_server: str or list = None, function=None, timeout=5, **kwargs):
     """ 开启tcp_client, 并且接收数据，对数据做验证
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
@@ -146,18 +150,20 @@
 
     if recv_content is not None:
         if datas:
             contents = [recv_content.encode('utf-8')] if isinstance(recv_content, str) else [c_.encode('utf-8') for
                                                                                              c_ in recv_content]
             # 校验数据内容
             if list(filter(lambda x: x not in datas, contents)):
+                logging.exception(f'tcp client {client} not recv content {recv_content}')
                 raise AssertionError(f'tcp client {client} not recv content {recv_content}')
             else:
                 logging.info(f'tcp client {client} recv content {recv_content} success')
         else:
+            logging.exception(f'tcp client {client} not connected')
             raise AssertionError(f'tcp client {client} not connected')
 
 
 def udp_server_data(host, port, recv_content: str or list = None, connect_time=10, send_msg_to_client: dict = None):
     """ 开启udp_server, 并且接收数据，对数据做验证, udp 校验数据时未区分客户端，所以保证接入时只有一个客户端
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
 
@@ -197,15 +203,15 @@
                 contents = [recv_content.encode()] if isinstance(recv_content, str) else [c_.encode() for c_ in
                                                                                           recv_content]
                 # 校验数据内容
                 if not list(filter(lambda x: x not in datas, contents)):
                     break
         else:
             if recv_content is not None:
-                logging.error(f'recv all data is {datas}')
+                logging.exception(f'recv all data is {datas}')
                 raise AssertionError('recv data error')
 
 
 def udp_client_data(server: tuple, client: tuple = None, recv_content: str or list = None, connect_time=10,
                     send_msg_to_server: str or list = None):
     """ 开启udp_client, 并且接收数据，对数据做验证
         该连接使用with，所以不管是客户端还是服务端，还是在异常状态下都会正常关闭
@@ -240,16 +246,14 @@
                 contents = [recv_content.encode('utf-8')] if isinstance(recv_content, str) else [c_.encode('utf-8') for
                                                                                                  c_ in recv_content]
                 # 校验数据内容
                 if not list(filter(lambda x: x not in datas, contents)):
                     break
         else:
             if recv_content is not None:
-                logging.error(f'recv all data is {datas}')
+                logging.exception(f'recv all data is {datas}')
                 raise AssertionError('recv data error')
 
 
 if __name__ == '__main__':
     import sys
-
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
-                        stream=sys.stdout)
+    pass
```

### Comparing `inhandtest-0.0.55/inhandtest/inssh.py` & `inhandtest-0.0.56/inhandtest/inssh.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # @Author  : Pane Li
 # @File    : inssh.py
 """
 inssh
 
 """
 import functools
-import logging
 import os.path
 
 import paramiko
 from paramiko.ssh_exception import *
+import logging
 
 
 class InSsh:
     def __init__(self, host: str, username: str, password: str, port=22, sftp=True):
         """
 
         :param host: ssh 连接主机地址
@@ -27,57 +27,105 @@
         self.__host = host
         self.__username = username
         self.__password = password
         self.__port = port
         self.ssh = paramiko.SSHClient()
         self.ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
         self.transport = paramiko.Transport((host, port))
-        try:
-            logging.info(f"ssh connect {self.__host} by {self.__username}:{self.__password}")
-            self.ssh.connect(self.__host, self.__port, self.__username, self.__password, timeout=5)
-        except AuthenticationException:
-            raise AuthenticationException(f"ssh connect {self.__host} Username or Password error")
-        except Exception:
-            raise ConnectionError(f"ssh connect {self.__host} connect error")
+        self.__connect()
         self.transport.connect(username=username, password=password)
         if sftp:
             self.sftp = paramiko.SFTPClient.from_transport(self.transport)
         else:
             self.sftp = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
+    def __connect(self):
+        try:
+            logging.info(f"ssh connect {self.__host} by {self.__username}:{self.__password}")
+            self.ssh.connect(self.__host, self.__port, self.__username, self.__password, timeout=5)
+        except AuthenticationException:
+            logging.exception(f"ssh connect {self.__host} Username or Password error")
+            raise AuthenticationException(f"ssh connect {self.__host} Username or Password error")
+        except Exception:
+            logging.exception(f"ssh connect {self.__host} connect error")
+            raise ConnectionError(f"ssh connect {self.__host} connect error")
+
+    def __auto_connect(function):
+        """自动重连, 只能当装饰器使用， 不对外使用
+
+        :param function:
+        :return:
+        """
+
+        def auto_connect(self, *args, **kwargs):
+            try:
+                res = function(self, *args, **kwargs)
+            except (ConnectionResetError, ConnectionAbortedError):
+                logging.debug(f"ssh connect {self.__host} error, reconnect")
+                self.__connect()
+                res = function(self, *args, **kwargs)
+            return res
+
+        return auto_connect
+
     def enable_sftp(func):
         @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
             if self.sftp is None:
+                logging.exception("please set sftp=True when init InSsh")
                 raise Exception("please set sftp=True when init InSsh")
             result = func(self, *args, **kwargs)
             return result
 
         return wrapper
 
+    @__auto_connect
     def exec_command(self, command: str) -> str:
         """执行命令并返回结果
 
         :param command: 执行命令, 多条时使用分号隔开
         :return: 返回所有命令执行后的结果
         """
         result = None
         if command:
             stdin, stdout, stderr = self.ssh.exec_command(command)
             logging.info(f'exec command 【{command}】')
             result = stdout.read().decode("utf-8")
             logging.debug(f'command result 【{result}】')
         return result
 
+    def ping(self, host, package=4, assert_lost_package=True, max_delay=100):
+        """
+
+        :param host: ip or host
+        :param package:  默认ping4个包
+        :param assert_lost_package: 判断是否存在丢包
+        :param max_delay:  最大延迟，单位ms
+        :return:
+        """
+        result = self.exec_command(f'ping -c {package} {host}')
+        if not result:
+            logging.exception('未建立openvpn连接')
+            raise AssertionError('未建立openvpn连接')
+        else:
+            if len(result) >= 2:
+                if assert_lost_package:
+                    assert package == int(result[-2].split(' ')[3]), '存在丢包'
+                if max_delay:
+                    assert float(max_delay) >= float(result[-1].split('/')[-2]), '延迟过大'
+            else:
+                logging.exception('ping 包失败')
+                raise AssertionError('ping 包失败')
+
     @enable_sftp
     def download_file(self, remote_file, local_file) -> None:
         """
         从服务器上下载文件
         :param remote_file: 远端文件路径
         :param local_file: 本地文件路径
         :return:
@@ -202,9 +250,8 @@
             self.sftp.close()
         self.transport.close()
 
 
 if __name__ == '__main__':
     import sys
 
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO, stream=sys.stdout)
-    InSsh('10.5.17.45', 'inhand', '64391099@inhand', sftp=False).download_file('/home/inhand/1.txt', 'D:\ecoer\1.txt')
+    pass
```

### Comparing `inhandtest-0.0.55/inhandtest/ip.py` & `inhandtest-0.0.56/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/mail.py` & `inhandtest-0.0.56/inhandtest/mail.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # @Author  : Pane Li
 # @File    : mail.py
 """
 mail
 
 """
 import datetime
-import logging
 import subprocess
 import re
 import emails
 import os
 import json
 import imaplib
 import email
 from email.header import decode_header
 from lxml import etree
 from inhandtest.tools import kill_windows_port, loop_inspector
+import logging
 
 
 def pytest_send_report_mail(mail_to: str or list, mail_from: tuple or list, render: dict):
     """使用已配置好的邮件模板，发送邮件内容, 且使用node.js anywhere启动一个本地服务，用于分享报告,
 
     :param mail_to:  发送给谁
     :param mail_from: 元组($email, $password)
@@ -32,14 +32,25 @@
                              host: 必填 测试主机， 10.5.24.107
                              port： 必填 分享报告端口， 63330
                              allure_results_path: 必填 报告中的/allure-results 路径
 
     :return:
     """
     port = render.get('port') if render.get('port') else 63330
+    # 杀掉端口, 防止端口占用
+    kill_windows_port(render.get('host'), [port, port + 1])  # port+1 是https端口
+    # 启动本地服务，分享报告
+    p = subprocess.Popen(f'npx anywhere -h {render.get("host")} -p {port}', cwd=render.get('allure_results_path'),
+                         shell=True,
+                         stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
+    while True:
+        output = p.stdout.readline()
+        logging.debug(output)
+        if len(re.findall(r'Running at (.*)/', output)) < 1:  # 无论是否启动成功，都会退出循环
+            break
     # 读取报告中的summary.json文件，获取测试结果
     summary = json.load(
         open(os.path.join(render.get('allure_results_path'), 'widgets', 'summary.json'), 'r', encoding='utf-8'))
     html_file_path = os.path.join(os.path.dirname(__file__), 'pytest_email.html')
     from emails.template import JinjaTemplate as Te
 
     message = emails.html(html=Te(open(html_file_path, encoding='utf-8').read()),
@@ -261,12 +272,8 @@
     logging.info('delete all emails')
     imap_server.close()
     imap_server.logout()
 
 
 if __name__ == '__main__':
     # 设置日志
-    import sys
-
-    logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s', stream=sys.stdout)
-    start_test_notice('liwei@inhand.com.cn', ('test@inhand.com.cn', 'ABc124'),
-                      {'model': 'IR302', 'version': '123', 'host': '10.5.24.224'})
+    pass
```

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/edge_computing_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/edge_computing/python_edge_computing.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/ingateway.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/ingateway.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 # @Time    : 2023/5/15 16:09:27
 # @Author  : Pane Li
 # @File    : ingateway.py
 """
 ingateway
 
 """
-import logging
-
 from playwright.sync_api import Page
 from inhandtest.base_page.base_page import BasePage
 from inhandtest.pages.ingateway.edge_computing.python_edge_computing import EdgeComputing
 from inhandtest.pages.ingateway.network.network import Network
 from inhandtest.pages.ingateway.overview.overview import Overview
 from inhandtest.pages.ingateway.system.system import System
 from inhandtest.telnet import Telnet
@@ -60,15 +58,12 @@
         self.network: Network = Network(host, username, password, protocol, port, model, language, self.page,
                                         self.locale)
         self.edge = EdgeComputing(host, username, password, protocol, port, model, language, self.page, self.locale)
         self.system = System(host, username, password, protocol, port, model, language, self.page, self.locale)
 
 
 if __name__ == '__main__':
-    from inhandtest.tools import enable_log
-
-    enable_log('./log.log', console_level=logging.INFO)
-    with InGateway('10.5.24.96') as device:
+    with InGateway('10.5.24.96', 'inhand', '64391099@inhand') as device:
         device.network.cellular.config(cellular_enable=False,
                                        submit={'tip_messages': 'cellular_configuration_changed_successful'})
 
         # device.page.wait_for_timeout(3 * 1000)
```

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/locale.yml` & `inhandtest-0.0.56/inhandtest/pages/ingateway/locale.yml`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/locators.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/network/network.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/network/network.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/network/network_locators.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/network/network_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/overview/overview.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/overview/overview.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/overview/overview_locators.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/overview/overview_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/system/system.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/system/system.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pages/ingateway/system/system_locators.py` & `inhandtest-0.0.56/inhandtest/pages/ingateway/system/system_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/pytest_email.html` & `inhandtest-0.0.56/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.55/inhandtest/telnet.py` & `inhandtest-0.0.56/inhandtest/telnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # @Time    : 2023/2/7 15:56:30
 # @Author  : Pane Li
 # @File    : telnet.py
 """
 telnet
 
 """
-import logging
+
 import re
 import telnetlib
 import time
 from typing import List
-
 from inhandtest.tools import loop_inspector, replace_str
+import logging
 
 
 class Telnet:
     __doc__ = '使用telnet连接设备，封装下面命令'
 
     def __init__(self, model: str, host: str, super_user: str, super_password: str, user='adm', password='123456',
                  port=23, **kwargs):
@@ -41,21 +41,23 @@
         self.super_password = super_password
         self.user = user
         self.password = password
         self.port = port
         self.host_name = ''
         self.super_tag = '/www #'
         self.config_tag = '(config)#'
-        self.user_tag = '#'    # 特权模式
+        self.user_tag = '#'  # 特权模式
         self.normal_tag = '>'
         self.factory_tag = '(factory)#'  # 仅部分设备支持工厂模式
         self.factory_username = kwargs.get('factory_username')
         self.factory_password = kwargs.get('factory_password')
         self.interface_replace: dict = kwargs.get('interface_replace')
-        if self.model not in ['VG710', 'IR302', 'IR305', 'IR615', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915', 'ODU2002']:
+        if self.model not in ['VG710', 'IR302', 'IR305', 'IR615', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915',
+                              'ODU2002']:
+            logging.exception(f'Not support this device model {self.model}')
             raise Exception(f'Not support this device model {self.model}')
         self.tn: telnetlib.Telnet
         self.__login()
 
     def update_hostname(self, hostname: str) -> None:
         """更新hostname 后对应的telnet也需要更新
 
@@ -75,25 +77,27 @@
         login_spe = {"VG710": '#', 'IR302': '>', 'ER805': '#', 'ER605': '#', 'IG902': '#', 'IG502': '#', 'IR915': '#',
                      'ODU2002': '>', 'IR305': '>', 'IR615': '>'}
         try:
             # 连接telnet服务器
             logging.debug("Start telnet 【%s:%s】" % (self.host, self.port))
             self.tn = telnetlib.Telnet(self.host, self.port, timeout=10)
         except:
+            logging.exception(f'ConnectionError Device【{self.host}:{self.port} connect failed】')
             raise ConnectionError(f'Device【{self.host}:{self.port} connect failed】')
         logging.debug("Telnet 【%s:%s】 connected" % (self.host, self.port))
         self.tn.write("\n".encode("cp936"))
         logging.debug(self.tn.read_until('login:'.encode("cp936")).decode("cp936").strip())
         # 登录路由器
         self.tn.write("{}\n".format(self.user).encode("cp936"))
         logging.debug(self.tn.read_until('Password:'.encode("cp936")).decode("cp936").strip())
         self.tn.write("{}\n".format(self.password).encode("cp936"))
         login_result = self.tn.read_until(login_spe.get(self.model).encode("cp936"), timeout=20).decode("cp936").strip()
         logging.debug(login_result)
         if 'Login incorrect' in login_result:
+            logging.exception('UsernameOrPasswordError')
             raise Exception('UsernameOrPasswordError')
         self.update_hostname(login_result.split('\r\n')[-1].split(' ')[-1][:-1])
         logging.info(f"Device {self.host} login success. user_tag: {self.user_tag}")
         return self
 
     def __enter__(self):
         return self
@@ -266,14 +270,15 @@
     @__auto_login
     def factory_mode(self) -> None:
         """工厂模式， 仅部分机型支持该模式，使用时需注意
 
         :return:
         """
         if not self.factory_username or not self.factory_password:
+            logging.exception(f"sure this device support factory mode, and init factory_username、factory_password")
             raise Exception("sure this device support factory mode, and init factory_username、factory_password")
         self.tn.write(("\003" + "\r").encode("cp936"))
         time.sleep(1)
         read_contents = self.tn.read_very_eager().decode('cp936').strip()
         logging.debug(read_contents)
         if self.config_tag in read_contents:
             if self.model in ['VG710', 'IR302', 'IR305', 'IR615', 'ER805', 'ER605', 'IG902', 'IG502', 'IR915']:
@@ -339,23 +344,25 @@
             self.factory_mode()
         logging.info(f"Device {self.host} send cli {command}")
         if command:
             command = [command] if isinstance(command, str) else command
             if read_until:
                 read_until = [read_until] if isinstance(read_until, str) else read_until
                 if len(read_until) != len(command):
+                    logging.exception('The read_until params is error')
                     raise Exception('The read_until params is error')
             else:
                 read_until = [None for i in range(0, len(command))]
+            self.tn.read_very_eager()
             for com, read_until_ in zip(command, read_until):
                 self.tn.write((com + "\n").encode("cp936"))
                 until_result = []
                 for i in range(0, timeout, 1):  # 30秒没有找到期望的就主动断开
                     time.sleep(1)
-                    result = self.tn.read_very_eager().decode('cp936', "ignore").strip()
+                    result = self.tn.read_very_eager().decode('cp936', "ignore").strip().replace('\x08', '')
                     if result:
                         logging.debug(result)
                         result = result.split(com + "\r\n")[-1]
                     if read_until_:
                         until_result.append(result)
                         if isinstance(read_until_, str):
                             if read_until_ in ''.join(until_result):
@@ -368,14 +375,15 @@
                                 break
                     else:
                         # 如果没有readuntil 直接返回
                         break
                 else:
                     self.tn.write(("\003" + "\r").encode("cp936"))
                     time.sleep(1)
+                    logging.exception(f"Device {self.host} send cli {command} ReadUntilTimeOutError")
                     raise Exception('ReadUntilTimeOutError')
         if kwargs.get('key_replace') and 'last_read' in key_replace_type:
             result = replace_str(result, kwargs.get('key_replace'))
         if self.interface_replace and 'last_read' in interface_replace_type:  # 替换接口的关键字
             result = replace_str(result, self.interface_replace)
         return result
 
@@ -441,21 +449,23 @@
                                     check_ = False
                                     break
                             else:
                                 if k in result:
                                     check_ = False
                                     break
                     else:
+                        logging.exception(f'parameter expect type error, expect {expect}')
                         raise Exception('parameter expect is error')
                 if check_:
                     break
                 else:
                     time.sleep(interval)
                     logging.info(f"{expect} assert failure, wait for {interval}s inspection")
             else:
+                logging.exception(f'{expect} not found timeout')
                 raise Exception(f'{expect} not found timeout')
             logging.info(f'assert cli success')
 
     @__auto_login
     @loop_inspector('Telnet ping')
     def ping(self, address='www.baidu.com', packets_number=4, params='', key_replace=None, lost_packets=False,
              timeout=30, interval=5) -> bool:
@@ -534,14 +544,15 @@
                                   key_replace_type='cli')
                     self.tn.write(("\003" + "\r").encode("cp936"))
                     time.sleep(interval)
                     continue
                 except:
                     break
         else:
+            logging.exception('TcpdumpTimeOutError')
             raise Exception('TcpdumpTimeOutError')
 
     @__auto_login
     @loop_inspector('Telnet regular match content')
     def re_match(self, command: str or list, regular: str or list, type_='super',
                  key_replace=None, key_replace_type='last_read', timeout=20, interval=5) -> str or List[str]:
         """根据表达式获取最后一次执行命令的匹配值
@@ -628,33 +639,32 @@
     def reboot(self) -> None:
         """直接重启设备
 
         @return:
         """
         self.user_mode()
         self.send_cli(['reboot', 'y'])
-        logging.info("【%s】Device is rebooting, wait for 120s" % self.host)
-        time.sleep(120)
+        logging.info("【%s】Device is rebooting, wait for moment" % self.host)
+        time.sleep(10)
+        for i in range(0, 150, 5):
+            try:
+                telnetlib.Telnet(self.host, self.port, timeout=5)
+                break
+            except:
+                pass
 
     @__auto_login
     def close(self) -> None:
         """关闭连接
 
         @return:
         """
         self.tn.close()
         logging.info("Telnet 【%s:%s】 close connect session" % (self.host, self.port))
 
 
 if __name__ == '__main__':
-    from inhandtest.tools import enable_log
-
-    enable_log('./log.log')
-    device = Telnet('IG902', '10.5.24.96')
-    # device.tcpdump(expect='10.5.24.224.62227', interface='eth0.4094',)
-
-    # device = Telnet('IG902', '
-    # device = Telnet('VG710', '10.5.24.206', 'inhand', '64391099@inhand')
-    # a = device.send_cli('ping www.baidu.com -c 4', '/www #', 'super')
-    # print(eval('1==2'))
-    # device.assert_cli('ifconfig |grep wifi', expect='Local', interface_replace_type='cli_expect_last_read')
-    # print(device.re_match('ifconfig eth0', r'HWaddr(.*)inet6', key_replace={'\r\n':'', ' ': ''}))
+    from inhandtest.log import enable_log
+    enable_log('./log.log', 'DEBUG')
+    a = Telnet('IG902', '10.5.24.96', 'inhand', '64391099@inhand')
+    a.reboot()
+    a.send_cli('ifconfig', type_='super')
```

### Comparing `inhandtest-0.0.55/inhandtest/tools.py` & `inhandtest-0.0.56/inhandtest/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # @Time    : 2023/1/31 16:42:40
 # @Author  : Pane Li
 # @File    : tools.py
 """
 tools
 
 """
-import logging
 import os.path
 import random
 import re
 import string
 import subprocess
 import time
 import datetime
 from functools import wraps
 from typing import List
 import pytz
 import winreg
 import requests
 from inhandtest.file import file_hash
 from inhandtest.exception import ResourceNotFoundError
+import logging
 
 
 def loop_inspector(flag='status', timeout=90, interval=5, assertion=True):
     """装饰器，期望接收函数返回的值为True，如果为False时进行轮询，直至超时失败，如果正确就退出
 
     :param flag:  功能名称，用以输出日志，如果不填  默认为’状态’二字
     :param timeout:  循环检测超时时间
@@ -46,14 +46,15 @@
                     time.sleep(interval)
                     continue
                 else:
                     logging.info(f'{flag} assert success')
                     return result
             else:
                 if assertion:
+                    logging.exception(f'{flag} assert timeout failure')
                     raise AssertionError(f'{flag} assert timeout failure')
 
         return inspector
 
     return timeout_
 
 
@@ -69,23 +70,25 @@
     def wrapper(obj):
         if isinstance(obj, type):
             @wraps(obj, updated=())
             class Inner(obj):
                 def __init__(self, *args, **kwargs):
                     super().__init__(*args, **kwargs)
                     if self.product.lower() not in support_product:
+                        logging.exception(f"This class not support this device that product is {self.product}")
                         raise Exception(f"This class not support this device that product is {self.product}")
 
             return Inner
         else:
             @wraps(obj)
             def inner(self, *args, **kwargs):
                 if self.product.lower() in support_product:
                     return obj(self, *args, **kwargs)
                 else:
+                    logging.exception(f"This method not support this device that product is {self.product}")
                     raise Exception(f"This method not support this device that product is {self.product}")
 
             return inner
 
     return wrapper
 
 
@@ -165,14 +168,15 @@
     """
 
     def _search(process_):
         if process_:
             if isinstance(process_, str) or isinstance(process_, int):
                 command = f'tasklist |findstr {process_}'
             else:
+                logging.exception("not support process type")
                 raise Exception("not support process type")
             logging.info(command)
             p = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
             task_result = p.communicate()[0].strip()
             logging.debug(f'find {process_} process is: {task_result}')
             try:
                 task_result = re.sub('\s+', ' ', task_result).split(' ')
@@ -208,14 +212,15 @@
             elif isinstance(name_, int):
                 logging.debug(f'taskkill /pid {name_} /F')
                 p = subprocess.Popen(f'taskkill /pid {name_} /F', shell=True, stdout=subprocess.PIPE,
                                      stderr=subprocess.STDOUT, encoding='gbk')
                 logging.debug(p.communicate()[0])
                 time.sleep(3)  # 删除服务应等待几秒，服务完全退出
             else:
+                logging.exception("not support process type")
                 raise Exception("not support process type")
 
 
 def kill_windows_port(ip_, port: int or list) -> None:
     """ 杀死windows 相关端口服务
 
     :param ip_: 本机IP地址
@@ -244,14 +249,15 @@
                     s.bind((ip_, one_port))
                     s.close()
                     time.sleep(1)
                     break
                 except socket.error:
                     continue
         else:
+            logging.exception(f"kill process {one_port} failed")
             raise Exception(f"kill process {one_port} failed")
 
     [kill_one_port(port_) for port_ in port] if isinstance(port, list) else kill_one_port(port)
     [port_is_close(port_) for port_ in port] if isinstance(port, list) else port_is_close(port)
 
 
 def windows_cmd(command: str or list, expect: str or list or dict = None, last_read_replace: dict = None):
@@ -275,27 +281,32 @@
             last_read_content = p.communicate()[0].strip()
             logging.debug(last_read_content)
     if last_read_replace and last_read_content is not None:
         last_read_content = replace_str(last_read_content, last_read_replace)
     if expect is not None:
         if isinstance(expect, str):
             if expect not in last_read_content:
+                logging.exception(f'{expect} not in last read content')
                 raise AssertionError(f'{expect} not in last read content')
         elif isinstance(expect, list):
             if [expect_ for expect_ in expect if expect_ not in last_read_content]:
+                logging.exception(f'{expect} not in last read content')
                 raise AssertionError(f'{expect} not in last read content')
         elif isinstance(expect, dict):
             for k, v in expect.items():
                 if v:
                     if k not in last_read_content:
+                        logging.exception(f'{k} not in last read content')
                         raise AssertionError(f'{k} not in last read content')
                 else:
                     if k in last_read_content:
+                        logging.exception(f'{k} in last read content')
                         raise AssertionError(f'{k} in last read content')
         else:
+            logging.exception('parameter expect is error')
             raise Exception('parameter expect is error')
 
 
 def download_svn_package(svn: dict, file_path, check_package=True) -> None:
     """
 
     :param svn: dict {'url': $url, 'username': $username, 'password': $password} 固件全路径
@@ -315,36 +326,40 @@
         if (not os.path.isfile(local_firmware_path)) and (not os.path.exists(local_firmware_path)):
             logging.info(f"download {local_firmware_path} from svn and wait for a moment!")
             s = requests.Session()
             s.mount('http://', HTTPAdapter(max_retries=3))  # 本身请求失败会重试3次
             for i in range(3):  # 文件下载错误再继续下载
                 r = s.get(url_path, auth=auth)
                 if r.status_code == 401:
+                    logging.exception("svn username or password error")
                     raise Exception("svn username or password error")
                 elif r.status_code == 200:
                     with open(local_firmware_path, 'wb') as fi_:  # 覆盖写入
                         fi_.write(r.content)
                     r_hash_file = s.get(svn_hash_file_path, auth=auth)
                     if check_package:
                         for co_ in r_hash_file.content.split(b'\n'):
                             if co_.decode('utf-8').endswith(firmware_name):
                                 hash_sha256_value = co_.decode('utf-8').split(' ')[0].upper()
                                 break
                         else:
+                            logging.exception(f'{svn_hash_file_path} not contain {firmware_name} hash_sha256 value')
                             raise Exception(f'{svn_hash_file_path} not contain {firmware_name} hash_sha256 value')
                         if file_hash(local_firmware_path, 'sha256') == hash_sha256_value:
                             logging.debug(f'{local_firmware_path} download success')
                             break
                         else:
                             logging.warning(f'download package failed, try {i + 1} time')
                     else:
                         break
                 else:
+                    logging.exception("svn server down error")
                     raise Exception("svn server down error")
             else:
+                logging.exception("download package failed")
                 raise Exception('download package failed')
 
 
 def get_time_stamp(time_='', delta=0, delta_type='h', time_format='%Y-%m-%dT%H:%M:%SZ') -> str:
     """获取时间戳
 
     :param time_: 默认获取当前时间
@@ -383,14 +398,15 @@
         contain_flatten = dict_flatten(contain)  # 平铺字典
         expect_dict_flatten = dict_flatten(expect_dict)  # 平铺字典
         for contain_item, contain_value in contain_flatten.items():
             value = expect_dict_flatten.get(contain_item)
             if isinstance(contain_value, str) and '${value}' in contain_value:
                 expect_value = contain_value.replace('${value}', str(value))
                 if not eval(expect_value):
+                    logging.exception(f'expect_item {contain_item} value is {expect_value} is False')
                     raise AssertionError(f'expect_item {contain_item} value is {expect_value} is False')
             else:
                 assert value == contain_value, f'expect_item {contain_item} value is {contain_value} is False'
 
         else:
             logging.info(f'{contain} in {expect_dict} assert ok')
 
@@ -419,14 +435,15 @@
             elif isinstance(old, list):
                 new_old = [replace_(str(old_)) for old_ in old]
             elif isinstance(old, dict):
                 new_old = {}
                 for k, v in old.items():
                     new_old.update({replace_(str(k)): v})
             else:
+                logging.exception('Not support this type')
                 raise Exception('Not support this type')
     return new_old
 
 
 def generate_string(length, digits=True, lowercase=True, uppercase=True, special_chars=True, chinese_chars=False,
                     peer_chinese_chars_len=1):
     """生成指定长度的密码，可以选择包含类型，如（数字、大小写字母、特殊字符、中文）
@@ -488,18 +505,20 @@
                         one = random.randrange(2, num - i, 2)
                         contain_even_ = False
                     else:
                         one = random.randint(1, num - i)
                     num = num - one
                 elif num - i == 0:
                     if contain_even_:
+                        logging.exception('The minimum generated string does not support the inclusion of Chinese char')
                         raise Exception('The minimum generated string does not support the inclusion of Chinese char')
                     one = 1
                     num = num - one
                 else:
+                    logging.exception('the length of the generated string does not meet the kind requirement')
                     raise Exception('the length of the generated string does not meet the kind requirement')
             else:
                 one = num
             value.append(one)
         return value
 
     contain_char = [type_ for type_, exist_ in all_type.items() if exist_]
@@ -557,27 +576,29 @@
     def _async_raise(tid, exctype):
         """raises the exception, performs cleanup if needed"""
         tid = ctypes.c_long(tid)
         if not inspect.isclass(exctype):
             exctype = type(exctype)
         res = ctypes.pythonapi.PyThreadState_SetAsyncExc(tid, ctypes.py_object(exctype))
         if res == 0:
+            logging.exception('PyThreadState_SetAsyncExc failed')
             raise ValueError("invalid thread id or thread already stop")
         elif res != 1:
             # """if it returns a number greater than one, you're in trouble,
             # and you should call it again with exc=NULL to revert the effect"""
             ctypes.pythonapi.PyThreadState_SetAsyncExc(tid, None)
+            logging.exception('PyThreadState_SetAsyncExc failed')
             raise SystemError("PyThreadState_SetAsyncExc failed")
         else:
             logging.debug(f'threading {thread} stop success')
 
     try:
         _async_raise(thread.ident, SystemExit)
     except Exception as e:
-        logging.warning(e)
+        logging.exception(e)
 
 
 def is_installed(name):
     """
     判断windows系统是否安装了某个软件
     :param name:
     :return: ResourceNotFoundError
@@ -592,65 +613,33 @@
             all_installed.append(value)
             if name in value:
                 logging.debug(f'Found the software {name}')
                 break
         except:
             pass
     else:
-        logging.debug(f'all installed software is {all_installed}')
+        logging.exception(f'all installed software is {all_installed}')
         raise ResourceNotFoundError(f'Not found the software {name}')
 
 
-def enable_log(filename: str = None, console_level=logging.INFO):
-    """
-
-    :param filename:  日志文件名称 ex: './test.log'
-    :param console_level: logging.INFO, logging.DEBUG
-    :return:
-    """
-    import colorlog
-    console_handler = logging.StreamHandler()
-    formatter = colorlog.ColoredFormatter(
-        '%(log_color)s%(asctime)s %(levelname)s [%(module)s]:%(message)s',
-        log_colors={
-            'DEBUG': 'blue',
-            'INFO': 'green',
-            'WARNING': 'yellow',
-            'ERROR': 'red',
-            'CRITICAL': 'red,bg_white',
-        }
-    )
-    console_handler.setFormatter(formatter)
-    if filename is not None:
-        file_handler = logging.FileHandler(filename)  # 日志文件及名称
-        file_handler.setFormatter(logging.Formatter('%(asctime)s %(levelname)s [%(module)s]:%(message)s'))
-        logging.basicConfig(level=logging.DEBUG, handlers=[file_handler, console_handler])
-        file_handler.setLevel(logging.DEBUG)
-    else:
-        logging.basicConfig(level=logging.DEBUG, handlers=[console_handler])
-    console_handler.setLevel(console_level)
-
-
 class DotDict(dict):
     """使用点号深度获取字典key的值
 
     """
 
     def __getattr__(self, key):
         try:
             return self[key]
         except KeyError:
+            logging.exception(f'Not found the key {key}')
             raise AttributeError(key)
 
     def __setattr__(self, key, value):
         self[key] = value
 
 
 if __name__ == '__main__':
-    import sys
-
-    logging.basicConfig(format='%(asctime)s %(levelname)s %(message)s', level=logging.INFO,
-                        stream=sys.stdout)
+    kill_windows_port('10.5.24.224', 1111)
     # is_installed('Google Chrome123')
     # print(windows_cmd('route delete 192.168.2.102 mask 255.255.255.255 192.168.4.2', '操作完成', {' ': '', '\n': ''}))
     # print(generate_password(length=2, lowercase=True, uppercase=True, special_chars=True, chinese_chars=True))
     # print(get_time_stamp('2022-02-18T13:39:32Z', -2))
```

### Comparing `inhandtest-0.0.55/inhandtest.egg-info/PKG-INFO` & `inhandtest-0.0.56/inhandtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: inhandtest
-Version: 0.0.55
+Version: 0.0.56
 Summary: inhand test tools, so easy
 Home-page: https://inhandnetworks.yuque.com/irhb08/mrpu1r/qgu0imvigkm2xry9?singleDoc# 《inhandtest docs》
 Author: liwei
 Author-email: liwei@inhand.com.cn
 Maintainer: liwei
 Maintainer-email: liwei@inhand.com.cn
 License: UNKNOWN
```

### Comparing `inhandtest-0.0.55/inhandtest.egg-info/SOURCES.txt` & `inhandtest-0.0.56/inhandtest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 inhandtest/inmongodb.py
 inhandtest/inmqtt.py
 inhandtest/inrequest.py
 inhandtest/inserial.py
 inhandtest/insocket.py
 inhandtest/inssh.py
 inhandtest/ip.py
+inhandtest/log.py
 inhandtest/mail.py
 inhandtest/notice_email.html
 inhandtest/pytest_email.html
 inhandtest/telnet.py
 inhandtest/tools.py
 inhandtest.egg-info/PKG-INFO
 inhandtest.egg-info/SOURCES.txt
```

### Comparing `inhandtest-0.0.55/setup.py` & `inhandtest-0.0.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 """
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='inhandtest',
-    version='0.0.55',
+    version='0.0.56',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

