# Comparing `tmp/routingfilter-1.6.0.tar.gz` & `tmp/routingfilter-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingfilter-1.6.0.tar", last modified: Wed Jun 14 08:00:23 2023, max compression
+gzip compressed data, was "routingfilter-1.6.1.tar", last modified: Thu Jun 15 15:57:41 2023, max compression
```

## Comparing `routingfilter-1.6.0.tar` & `routingfilter-1.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:00:23.675061 routingfilter-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-14 08:00:10.000000 routingfilter-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:00:10.000000 routingfilter-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-14 08:00:23.675061 routingfilter-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-14 08:00:10.000000 routingfilter-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-14 08:00:10.000000 routingfilter-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:00:23.675061 routingfilter-1.6.0/routingfilter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 08:00:10.000000 routingfilter-1.6.0/routingfilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-06-14 08:00:10.000000 routingfilter-1.6.0/routingfilter/configfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-14 08:00:10.000000 routingfilter-1.6.0/routingfilter/dictquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-06-14 08:00:10.000000 routingfilter-1.6.0/routingfilter/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    40397 2023-06-14 08:00:10.000000 routingfilter-1.6.0/routingfilter/routing_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    19796 2023-06-14 08:00:10.000000 routingfilter-1.6.0/routingfilter/routing_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 08:00:23.675061 routingfilter-1.6.0/routingfilter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-14 08:00:23.000000 routingfilter-1.6.0/routingfilter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-14 08:00:23.000000 routingfilter-1.6.0/routingfilter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 08:00:23.000000 routingfilter-1.6.0/routingfilter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-14 08:00:23.000000 routingfilter-1.6.0/routingfilter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 08:00:23.000000 routingfilter-1.6.0/routingfilter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 08:00:23.675061 routingfilter-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-14 08:00:10.000000 routingfilter-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:57:41.552708 routingfilter-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-15 15:57:27.000000 routingfilter-1.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:57:27.000000 routingfilter-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-15 15:57:41.552708 routingfilter-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-15 15:57:27.000000 routingfilter-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 15:57:27.000000 routingfilter-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:57:41.552708 routingfilter-1.6.1/routingfilter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9749 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/configfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/dictquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10157 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40397 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/routing_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21567 2023-06-15 15:57:27.000000 routingfilter-1.6.1/routingfilter/routing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:57:41.552708 routingfilter-1.6.1/routingfilter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 15:57:41.000000 routingfilter-1.6.1/routingfilter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:57:41.552708 routingfilter-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-15 15:57:27.000000 routingfilter-1.6.1/setup.py
```

### Comparing `routingfilter-1.6.0/LICENSE.txt` & `routingfilter-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.0/PKG-INFO` & `routingfilter-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.6.0
+Version: 1.6.1
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `routingfilter-1.6.0/README.md` & `routingfilter-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.0/routingfilter/configfilter.py` & `routingfilter-1.6.1/routingfilter/configfilter.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.0/routingfilter/dictquery.py` & `routingfilter-1.6.1/routingfilter/dictquery.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.0/routingfilter/routing.py` & `routingfilter-1.6.1/routingfilter/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,17 @@
         # Rename "filters" to "rules" and "type" to "output" to be more generic
         matching_rules = copy.deepcopy(matching_rules)
         for mr in matching_rules:
             if "filters" in mr:
                 mr["rules"] = mr.pop("filters")
             if type_ in mr:
                 mr["output"] = mr.pop(type_)
-                if len(mr["output"]) > 0:
-                    event["certego"]["routing_history"][list(mr["output"].keys())[0]] = datetime.now().isoformat()
+                if mr["output"]:
+                    for k in mr["output"].keys():
+                        event["certego"]["routing_history"][k] = datetime.now().isoformat()
         return matching_rules
 
     def load_from_dicts(self, rules_list: List[dict], validate_rules: bool = True, variables: Optional[dict] = None) -> None:
         """Load routing configuration from a dictionary. It merges the different rules in list into a single routing rule.
         It optionally performs some rules validation before accepting them (an exception is raised in case of errors).
 
         :param rules_list: The configuration
```

### Comparing `routingfilter-1.6.0/routingfilter/routing_benchmark.py` & `routingfilter-1.6.1/routingfilter/routing_benchmark.py`

 * *Files identical despite different names*

### Comparing `routingfilter-1.6.0/routingfilter/routing_test.py` & `routingfilter-1.6.1/routingfilter/routing_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         self.test_event_11 = load_test_data("test_event_11")
         self.test_event_12 = load_test_data("test_event_12")
         self.test_event_13 = load_test_data("test_event_13")
         self.test_event_14 = load_test_data("test_event_14")
         self.test_event_15 = load_test_data("test_event_15")
         self.test_event_16 = load_test_data("test_event_16")
         self.test_event_17 = load_test_data("test_event_17")
+        self.test_event_18 = load_test_data("test_event_18")
         self.test_event_with_list_1 = load_test_data("test_event_with_list_1")
         self.test_event_with_list_2 = load_test_data("test_event_with_list_2")
 
     def test_wrong_inputs(self):
         self.assertIsNone(self.routing.get_rules())
         with self.assertRaises(ValueError):
             self.routing.match({})
@@ -68,14 +69,28 @@
         rule_all = load_test_data("test_rule_2_all_equals")
         filter_2 = copy.deepcopy(rule_all["streams"]["rules"]["all"][0])
         filter_2["streams"] = {"Other": None}
         rule_all["streams"]["rules"]["all"].append(filter_2)
         self.routing.load_from_dicts([rule_all])
         self.assertDictEqual(self.routing.match(self.test_event_1)[0]["output"], {'Workshop': {'workers_needed': 1}})
 
+    def test_match_streams_none(self):
+        self.routing.load_from_dicts([load_test_data("test_rule_25_routing_history_streams_none")])
+        self.routing.match(self.test_event_1)
+        self.assertTrue("rules" in self.routing.match(self.test_event_1)[0])
+        self.assertTrue("output" in self.routing.match(self.test_event_1)[0])
+        self.assertEqual(None, self.routing.match(self.test_event_1)[0]["output"])
+
+    def test_no_match_streams_none(self):
+        self.routing.load_from_dicts([load_test_data("test_rule_25_routing_history_streams_none")])
+        self.routing.match(self.test_event_4)
+        self.assertFalse("rules" in self.routing.match(self.test_event_4))
+        self.assertEqual([], self.routing.match(self.test_event_4))
+        self.assertFalse("output" in self.routing.match(self.test_event_4))
+
     def test_routing_history(self):
         self.routing.load_from_dicts([load_test_data("test_rule_24_routing_history")])
         self.routing.match(self.test_event_1)
         self.assertTrue(self.test_event_1["certego"]["routing_history"]["Workshop"])
         # Check if the rule is processed twice
         self.assertTrue("Workshop" in self.test_event_1["certego"]["routing_history"])
         self.assertFalse("TyreFit" in self.test_event_1["certego"]["routing_history"])
@@ -83,30 +98,47 @@
         self.routing.match(self.test_event_1)
         self.assertTrue("Workshop" in self.test_event_1["certego"]["routing_history"])
         self.assertTrue("TyreFit" in self.test_event_1["certego"]["routing_history"])
         
     def test_routing_history_stream_none(self):
         self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
         self.routing.match(self.test_event_1)
+        # Match rules
         self.assertTrue(self.test_event_1["certego"]["routing_history"]["Workshop"])
         self.routing.load_from_dicts([load_test_data("test_rule_25_routing_history_streams_none")])
         self.routing.match(self.test_event_1)
+        # Checking no match, the message should be filtered
         self.assertEqual(len(self.test_event_1["certego"]["routing_history"].keys()), 1)
+        self.assertEqual(None, self.routing.match(self.test_event_1)[0]["output"])
 
     def test_routing_history_same_rule_twice(self):
-            workshop_count = 0
-            self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
-            self.routing.match(self.test_event_1)
-            self.assertTrue(self.test_event_1["certego"]["routing_history"]["Workshop"])
-            self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
-            self.routing.match(self.test_event_1)
-            for key in self.test_event_1["certego"]["routing_history"].keys():
-                if key == "Workshop":
-                    workshop_count = workshop_count + 1
-            self.assertEqual(workshop_count, 1)
+        workshop_count = 0
+        self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
+        self.routing.match(self.test_event_1)
+        self.assertTrue(self.test_event_1["certego"]["routing_history"]["Workshop"])
+        self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
+        res = self.routing.match(self.test_event_1)
+        for key in self.test_event_1["certego"]["routing_history"].keys():
+            if key == "Workshop":
+                workshop_count = workshop_count + 1
+        self.assertEqual(workshop_count, 1)
+        self.assertEqual([], res)
+
+    def test_double_stream(self):
+        self.routing.load_from_dicts([load_test_data("test_rule_28_double_stream")])
+        res = self.routing.match(self.test_event_1)
+        self.assertDictEqual({'Workshop': {'workers_needed': 1}, 'Lab': {'workers_needed': 2}}, res[0]["output"])
+        self.assertTrue("Workshop" in self.test_event_1["certego"]["routing_history"])
+        self.assertTrue("Lab" in self.test_event_1["certego"]["routing_history"])
+        self.assertEqual(2, len(res[0]["output"]))
+
+    def test_double_tag(self):
+        self.routing.load_from_dicts([load_test_data("test_rule_29_double_tag")])
+        res = self.routing.match(self.test_event_18)
+        self.assertEqual(2, len(res))
 
     def test_rule_1(self):
         # Test rule loading and applying with full output
         self.routing.load_from_dicts([load_test_data("test_rule_1_equals")])
         self.assertDictEqual(self.routing.match(self.test_event_1)[0], load_test_data("test_event_1_rule_1_response"))
         self.assertEqual(self.routing.match(self.test_event_2), [])
         self.assertEqual(self.routing.match(self.test_event_3), [])
@@ -140,15 +172,14 @@
         test_rule_1_equals = load_test_data("test_rule_1_equals")
         test_rule_2_all_equals = load_test_data("test_rule_2_all_equals")
         self.routing.load_from_dicts([test_rule_1_equals, test_rule_2_all_equals])
         self.assertDictEqual(self.routing.match(self.test_event_1)[0], load_test_data("test_event_1_rule_1_response"))
         self.assertDictEqual(self.routing.match(self.test_event_2)[0], load_test_data("test_event_1_rule_1_response"))
         self.assertEqual(self.routing.match(self.test_event_3), [])
         
-
     def test_special_tag_all2(self):
         test_rule_1_equals = load_test_data("test_rule_1_equals")
         test_rule_2_all_equals = load_test_data("test_rule_2_all_equals")
         test_rule_2_all_equals["streams"]["rules"]["all"][0]["filters"][0]["key"] = "wheel_model_wrong"
         self.routing.load_from_dicts([test_rule_1_equals, test_rule_2_all_equals])
         self.assertDictEqual(self.routing.match(self.test_event_1)[0], load_test_data("test_event_1_rule_1_response"))
         self.assertEqual(self.routing.match(load_test_data("test_event_2")), [])
@@ -359,8 +390,10 @@
             ],
             "streams": {
                 "Workshop": {
                     "workers_needed": 1
                 }
             }
           }
-        self.assertTrue(self.routing.rule_in_routing_history(event, rule))
+        self.assertTrue(self.routing.rule_in_routing_history(event, rule))
+
+
```

### Comparing `routingfilter-1.6.0/routingfilter.egg-info/PKG-INFO` & `routingfilter-1.6.1/routingfilter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingfilter
-Version: 1.6.0
+Version: 1.6.1
 Summary: Generic Business Logic Implementation for Routing objects as python dictionaries
 Home-page: https://github.com/certego/RoutingFilter
 Author: Certego S.r.l.
 Author-email: support@certego.net
 License: GNU LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `routingfilter-1.6.0/setup.py` & `routingfilter-1.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name='routingfilter',
-    version='1.6.0',
+    version='1.6.1',
     packages=['routingfilter'],
     include_package_data=True,
     install_requires=["IPy~=1.1", "macaddress~=2.0.2"],
     url='https://github.com/certego/RoutingFilter',
     license='GNU LGPLv3',
     author='Certego S.r.l.',
     author_email='support@certego.net',
```

