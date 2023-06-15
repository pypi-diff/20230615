# Comparing `tmp/taranis_ng_shared-0.1.8.tar.gz` & `tmp/taranis_ng_shared-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taranis_ng_shared-0.1.8.tar", last modified: Wed Jun 14 11:34:52 2023, max compression
+gzip compressed data, was "taranis_ng_shared-0.1.9.tar", last modified: Thu Jun 15 11:58:49 2023, max compression
```

## Comparing `taranis_ng_shared-0.1.8.tar` & `taranis_ng_shared-0.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:34:52.917303 taranis_ng_shared-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-14 11:34:52.917303 taranis_ng_shared-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-14 11:34:52.917303 taranis_ng_shared-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:34:52.913303 taranis_ng_shared-0.1.8/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:34:52.917303 taranis_ng_shared-0.1.8/shared/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/acl_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/bots_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/collectors_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/news_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/notification_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/osint_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/parameter_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/presentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/presenters_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/product_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/publisher_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/publishers_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/report_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/report_item_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/role.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/tag_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-14 11:34:37.000000 taranis_ng_shared-0.1.8/shared/schema/word_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 11:34:52.917303 taranis_ng_shared-0.1.8/taranis_ng_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-14 11:34:52.000000 taranis_ng_shared-0.1.8/taranis_ng_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-14 11:34:52.000000 taranis_ng_shared-0.1.8/taranis_ng_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:34:52.000000 taranis_ng_shared-0.1.8/taranis_ng_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 11:34:52.000000 taranis_ng_shared-0.1.8/taranis_ng_shared.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-14 11:34:52.000000 taranis_ng_shared-0.1.8/taranis_ng_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 11:34:52.000000 taranis_ng_shared-0.1.8/taranis_ng_shared.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:58:49.609712 taranis_ng_shared-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-15 11:58:49.609712 taranis_ng_shared-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-15 11:58:49.609712 taranis_ng_shared-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:58:49.601712 taranis_ng_shared-0.1.9/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:58:49.609712 taranis_ng_shared-0.1.9/shared/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/acl_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/bots_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/collectors_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/news_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/notification_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/osint_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/parameter_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/presentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/presenters_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/product_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/publisher_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/publishers_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/report_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/report_item_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/tag_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-15 11:58:40.000000 taranis_ng_shared-0.1.9/shared/schema/word_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:58:49.609712 taranis_ng_shared-0.1.9/taranis_ng_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-15 11:58:49.000000 taranis_ng_shared-0.1.9/taranis_ng_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-15 11:58:49.000000 taranis_ng_shared-0.1.9/taranis_ng_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:58:49.000000 taranis_ng_shared-0.1.9/taranis_ng_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:58:49.000000 taranis_ng_shared-0.1.9/taranis_ng_shared.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 11:58:49.000000 taranis_ng_shared-0.1.9/taranis_ng_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 11:58:49.000000 taranis_ng_shared-0.1.9/taranis_ng_shared.egg-info/top_level.txt
```

### Comparing `taranis_ng_shared-0.1.8/PKG-INFO` & `taranis_ng_shared-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taranis_ng_shared
-Version: 0.1.8
+Version: 0.1.9
 Summary: Taranis-NG Shared Classes
 Home-page: https://github.com/SK-CERT/Taranis-NG
 Author: SK-CERT, AIT
 License: EUPL
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `taranis_ng_shared-0.1.8/setup.cfg` & `taranis_ng_shared-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = taranis-ng_shared
-version = 0.1.8
+version = 0.1.9
 description = Taranis-NG Shared Classes
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = EUPL
 platforms = any
 author = SK-CERT, AIT
 url = https://github.com/SK-CERT/Taranis-NG
```

### Comparing `taranis_ng_shared-0.1.8/shared/log.py` & `taranis_ng_shared-0.1.9/shared/log.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/__init__.py` & `taranis_ng_shared-0.1.9/shared/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/acl_entry.py` & `taranis_ng_shared-0.1.9/shared/schema/acl_entry.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/asset.py` & `taranis_ng_shared-0.1.9/shared/schema/asset.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/attribute.py` & `taranis_ng_shared-0.1.9/shared/schema/attribute.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/bot.py` & `taranis_ng_shared-0.1.9/shared/schema/bot.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/bots_node.py` & `taranis_ng_shared-0.1.9/shared/schema/bots_node.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/collector.py` & `taranis_ng_shared-0.1.9/shared/schema/collector.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/collectors_node.py` & `taranis_ng_shared-0.1.9/shared/schema/collectors_node.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/news_item.py` & `taranis_ng_shared-0.1.9/shared/schema/news_item.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/notification_template.py` & `taranis_ng_shared-0.1.9/shared/schema/notification_template.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/osint_source.py` & `taranis_ng_shared-0.1.9/shared/schema/osint_source.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/parameter.py` & `taranis_ng_shared-0.1.9/shared/schema/parameter.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/parameter_value.py` & `taranis_ng_shared-0.1.9/shared/schema/parameter_value.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/presenter.py` & `taranis_ng_shared-0.1.9/shared/schema/presenter.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/presenters_node.py` & `taranis_ng_shared-0.1.9/shared/schema/presenters_node.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/product.py` & `taranis_ng_shared-0.1.9/shared/schema/product.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/product_type.py` & `taranis_ng_shared-0.1.9/shared/schema/product_type.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/publisher.py` & `taranis_ng_shared-0.1.9/shared/schema/publisher.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/publisher_preset.py` & `taranis_ng_shared-0.1.9/shared/schema/publisher_preset.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/publishers_node.py` & `taranis_ng_shared-0.1.9/shared/schema/publishers_node.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/remote.py` & `taranis_ng_shared-0.1.9/shared/schema/remote.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/report_item.py` & `taranis_ng_shared-0.1.9/shared/schema/report_item.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/report_item_type.py` & `taranis_ng_shared-0.1.9/shared/schema/report_item_type.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/role.py` & `taranis_ng_shared-0.1.9/shared/schema/role.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/tag_cloud.py` & `taranis_ng_shared-0.1.9/shared/schema/tag_cloud.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/shared/schema/user.py` & `taranis_ng_shared-0.1.9/shared/schema/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,8 +64,8 @@
     alias = fields.Str()
 
 
 class UserProfileSchema(Schema):
     spellcheck = fields.Bool()
     dark_theme = fields.Bool()
     hotkeys = fields.Nested(HotkeySchema, many=True)
-    language = fields.Str(default="en")
+    language = fields.Str(load_default="en", dump_default="en")
```

### Comparing `taranis_ng_shared-0.1.8/shared/schema/word_list.py` & `taranis_ng_shared-0.1.9/shared/schema/word_list.py`

 * *Files identical despite different names*

### Comparing `taranis_ng_shared-0.1.8/taranis_ng_shared.egg-info/PKG-INFO` & `taranis_ng_shared-0.1.9/taranis_ng_shared.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taranis-ng-shared
-Version: 0.1.8
+Version: 0.1.9
 Summary: Taranis-NG Shared Classes
 Home-page: https://github.com/SK-CERT/Taranis-NG
 Author: SK-CERT, AIT
 License: EUPL
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `taranis_ng_shared-0.1.8/taranis_ng_shared.egg-info/SOURCES.txt` & `taranis_ng_shared-0.1.9/taranis_ng_shared.egg-info/SOURCES.txt`

 * *Files identical despite different names*

