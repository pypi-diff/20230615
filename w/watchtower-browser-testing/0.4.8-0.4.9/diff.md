# Comparing `tmp/watchtower_browser_testing-0.4.8.tar.gz` & `tmp/watchtower_browser_testing-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.4.8.tar", last modified: Fri May 19 18:18:40 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.4.9.tar", last modified: Sat May 20 11:47:49 2023, max compression
```

## Comparing `watchtower_browser_testing-0.4.8.tar` & `watchtower_browser_testing-0.4.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 18:18:40.144399 watchtower_browser_testing-0.4.8/
--rw-rw-rw-   0        0        0      310 2023-05-19 18:18:40.144399 watchtower_browser_testing-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 18:18:40.144399 watchtower_browser_testing-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:18:40.144399 watchtower_browser_testing-0.4.8/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:18:40.144399 watchtower_browser_testing-0.4.8/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    17926 2023-05-19 12:18:04.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7887 2023-05-19 18:18:32.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-05-19 18:18:32.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:18:40.144399 watchtower_browser_testing-0.4.8/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-05-19 18:18:39.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-05-19 18:18:40.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 18:18:39.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-19 18:18:39.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-05-19 18:18:39.000000 watchtower_browser_testing-0.4.8/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-20 11:47:49.987478 watchtower_browser_testing-0.4.9/
+-rw-rw-rw-   0        0        0      310 2023-05-20 11:47:49.987478 watchtower_browser_testing-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-20 11:47:49.987478 watchtower_browser_testing-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:47:49.970668 watchtower_browser_testing-0.4.9/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1834 2023-05-20 11:47:19.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:47:49.970668 watchtower_browser_testing-0.4.9/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6195 2023-04-25 13:45:16.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    18276 2023-05-20 11:47:19.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7887 2023-05-19 18:18:32.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-05-20 11:47:19.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-05-20 11:47:49.970668 watchtower_browser_testing-0.4.9/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-05-20 11:47:49.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-05-20 11:47:49.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-20 11:47:49.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-20 11:47:49.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-05-20 11:47:49.000000 watchtower_browser_testing-0.4.9/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.4.8/setup.py` & `watchtower_browser_testing-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.8/watchtower_browser_testing/config.py` & `watchtower_browser_testing-0.4.9/watchtower_browser_testing/config.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.8/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.4.9/watchtower_browser_testing/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import json
 from marko.ext.gfm import gfm as markdown
+import collections
 
 
 def trim(docstring):
     if not docstring:
         return ''
     # Convert tabs to spaces (following the normal Python rules)
     # and split into a list of lines:
@@ -41,8 +42,23 @@
 
 
 class ExtendedEncoder(json.JSONEncoder):
 
     def default(self, obj):
         if callable(obj):
             return obj.__name__
-        return super().default(obj)
+        return super().default(obj)
+
+class Storage(collections.UserDict):
+
+    def get(self, key, default=None):
+
+        value = super().get(key, default)
+
+        if value is None:
+            value = self.key_name_string(key)
+
+        return value
+
+    @staticmethod
+    def key_name_string(key):
+        return f'<{key}>'
```

### Comparing `watchtower_browser_testing-0.4.8/watchtower_browser_testing/templates/measurement_plan.html` & `watchtower_browser_testing-0.4.9/watchtower_browser_testing/templates/measurement_plan.html`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.8/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.4.9/watchtower_browser_testing/testsuite.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,18 @@
 
 class TrackingTest(object):
 
     browsers = config.DEFAULT_BROWSERS
 
     pipeline_patterns = [config.DEFAULT_PIPELINE_PATTERN]
 
+    def __init__(self):
+
+        self.storage = helpers.Storage()
+
     def setUpInstance(self,
                       playwright,
                       browser,
                       gtm_web_preview_link=None,
                       tag_assistant_path=None,
                       headless=False):
 
@@ -209,15 +213,20 @@
                 for test in tests:
 
                     scenario = test[len(config.SCENARIO_METHOD_PREFIX):]
 
                     self.beforeEach()
 
                     getattr(self, test)()
-                    validation_setup = getattr(self, config.VALIDATION_METHOD_PREFIX + scenario)()
+                    validation_func = getattr(self, config.VALIDATION_METHOD_PREFIX + scenario)
+                    sig = inspect.signature(validation_func)
+                    if len(sig.parameters) > 0:
+                        validation_setup = validation_func(storage=self.storage)
+                    else:
+                        validation_setup = validation_func()
 
                     for event, setup in validation_setup.items():
 
                         validator = RequestValidator(**setup)
                         validator.select(self.event_queue.requests)
 
                         if validator.is_valid():
```

### Comparing `watchtower_browser_testing-0.4.8/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.4.9/watchtower_browser_testing/tracking_validation.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.4.8/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.4.9/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

