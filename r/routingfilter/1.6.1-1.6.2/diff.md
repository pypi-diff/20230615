# Comparing `tmp/routingfilter-1.6.1.tar.gz` & `tmp/routingfilter-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingfilter-1.6.1.tar", last modified: Thu Jun 15 15:57:41 2023, max compression
+gzip compressed data, was "routingfilter-1.6.2.tar", last modified: Thu Jun 15 16:58:53 2023, max compression
```

## Comparing `routingfilter-1.6.1.tar` & `routingfilter-1.6.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:57:41.552708 routingfilter-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 15:57:27.000000 routingfilter-1.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:57:27.000000 routingfilter-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-15 15:57:41.552708 routingfilter-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 15:57:27.000000 routingfilter-1.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 15:57:27.000000 routingfilter-1.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:57:41.552708 routingfilter-1.6.1/routingfilter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/configfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/dictquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    40397 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/routing_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/routing_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:57:41.552708 routingfilter-1.6.1/routingfilter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:57:41.552708 routingfilter-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 15:57:27.000000 routingfilter-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:58:53.319733 routingfilter-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 16:58:40.000000 routingfilter-1.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:58:40.000000 routingfilter-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-15 16:58:53.319733 routingfilter-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 16:58:40.000000 routingfilter-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 16:58:40.000000 routingfilter-1.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:58:53.319733 routingfilter-1.6.2/routingfilter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/configfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/dictquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40397 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/routing_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-06-15 16:58:40.000000 routingfilter-1.6.2/routingfilter/routing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:58:53.319733 routingfilter-1.6.2/routingfilter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 16:58:53.000000 routingfilter-1.6.2/routingfilter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 16:58:53.319733 routingfilter-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 16:58:40.000000 routingfilter-1.6.2/setup.py
```

### Comparing `routingfilter-1.6.1/LICENSE.txt` & `routingfilter-1.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.1/PKG-INFO` & `routingfilter-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.6.1
+Version: 1.6.2
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `routingfilter-1.6.1/README.md` & `routingfilter-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.1/routingfilter/configfilter.py` & `routingfilter-1.6.2/routingfilter/configfilter.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.1/routingfilter/dictquery.py` & `routingfilter-1.6.2/routingfilter/dictquery.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.1/routingfilter/routing.py` & `routingfilter-1.6.2/routingfilter/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,33 +60,34 @@
         if "all" in streams_tags:
             # the first matching rule wins
             rules = self.rules[type_]["rules"]["all"]
             rules = rules if rules else []
             for rule in rules:
                 # check if ALL the filters are matching
                 filters = [ConfigFilter(f) for f in rule.get("filters", [])]
-                if all(f.is_matching(event) for f in filters) and not self.rule_in_routing_history(event, rule):
+                if all(f.is_matching(event) for f in filters) and not self.rule_in_routing_history(type_, event, rule):
                     matching_rules.append(rule)
                     break
         if not matching_rules:
             for tag_field_name in msg_tags:
                 for rule in self.rules[type_]["rules"].get(tag_field_name, []):
                     # check if ALL the filters are matching
                     config_filters = [ConfigFilter(f) for f in rule.get("filters", [])]
-                    if config_filters and all(f.is_matching(event) for f in config_filters) and not self.rule_in_routing_history(event, rule):
+                    if config_filters and all(f.is_matching(event) for f in config_filters) and not self.rule_in_routing_history(type_, event, rule):
                         matching_rules.append(rule)
                         break  # the first matching rule wins if it doesn't exist in the output field
         # Rename "filters" to "rules" and "type" to "output" to be more generic
         matching_rules = copy.deepcopy(matching_rules)
         for mr in matching_rules:
             if "filters" in mr:
                 mr["rules"] = mr.pop("filters")
             if type_ in mr:
                 mr["output"] = mr.pop(type_)
-                if mr["output"]:
+                # We are only interested in dict type
+                if mr["output"] and isinstance(mr["output"], dict):
                     for k in mr["output"].keys():
                         event["certego"]["routing_history"][k] = datetime.now().isoformat()
         return matching_rules
 
     def load_from_dicts(self, rules_list: List[dict], validate_rules: bool = True, variables: Optional[dict] = None) -> None:
         """Load routing configuration from a dictionary. It merges the different rules in list into a single routing rule.
         It optionally performs some rules validation before accepting them (an exception is raised in case of errors).
@@ -189,21 +190,26 @@
         for type_ in rules.keys():
             for tag_ in rules[type_]["rules"].keys():
                 for filter_output in rules[type_]["rules"][tag_]:
                     for filter_ in filter_output["filters"]:
                         config_filter_obj = ConfigFilter(filter_)
                         config_filter_obj.is_matching({})
 
-    def rule_in_routing_history(self, event, rule):
+    def rule_in_routing_history(self, type_, event, rule):
         """Checking if the given rule has already been processed
 
+        :param type_: The type_ of the event
+        :type type_: dict
         :param event: The entire event to process
         :type event: dict
         :param rule: The rule to check
         :type rule: dict
         """
-        if rule["streams"] is None:
+        if rule[type_] is None:
             return False
-        for key in rule["streams"].keys():
+        # we are only interested in rule[type_] containing dict
+        if not isinstance(rule[type_], dict):
+            return False
+        for key in rule[type_].keys():
             if key in event["certego"]["routing_history"]:
                 return True
         return False
```

### Comparing `routingfilter-1.6.1/routingfilter/routing_benchmark.py` & `routingfilter-1.6.2/routingfilter/routing_benchmark.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.1/routingfilter/routing_test.py` & `routingfilter-1.6.2/routingfilter/routing_test.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.1/routingfilter.egg-info/PKG-INFO` & `routingfilter-1.6.2/routingfilter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.6.1
+Version: 1.6.2
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `routingfilter-1.6.1/setup.py` & `routingfilter-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='routingfilter',
-    version='1.6.1',
+    version='1.6.2',
     packages=['routingfilter'],
     include_package_data=True,
     install_requires=["IPy~=1.1", "macaddress~=2.0.2"],
     url='https://github.com/certego/RoutingFilter',
     license='GNU LGPLv3',
     author='Certego S.r.l.',
     author_email='support@certego.net',
```

