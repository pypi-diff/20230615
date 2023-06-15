# Comparing `tmp/fenjing-0.3.8.tar.gz` & `tmp/fenjing-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenjing-0.3.8.tar", last modified: Sat Jun  3 01:27:23 2023, max compression
+gzip compressed data, was "fenjing-0.3.9.tar", last modified: Thu Jun 15 06:22:16 2023, max compression
```

## Comparing `fenjing-0.3.8.tar` & `fenjing-0.3.9.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:27:23.940680 fenjing-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-03 01:27:14.000000 fenjing-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-03 01:27:14.000000 fenjing-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-03 01:27:23.936680 fenjing-0.3.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6115 2023-06-03 01:27:14.000000 fenjing-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 01:27:14.000000 fenjing-0.3.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:27:23.936680 fenjing-0.3.8/fenjing/
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/config_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/form_cracker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5080 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/full_payload_gen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/int_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    30746 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/payload_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/scan_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/shell_payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:27:23.936680 fenjing-0.3.8/fenjing/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/waf_func_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-03 01:27:14.000000 fenjing-0.3.8/fenjing/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 01:27:23.936680 fenjing-0.3.8/fenjing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-03 01:27:23.000000 fenjing-0.3.8/fenjing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-03 01:27:14.000000 fenjing-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 01:27:23.940680 fenjing-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-03 01:27:14.000000 fenjing-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.934390 fenjing-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-15 06:22:04.000000 fenjing-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-15 06:22:04.000000 fenjing-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-15 06:22:16.934390 fenjing-0.3.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6115 2023-06-15 06:22:04.000000 fenjing-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 06:22:04.000000 fenjing-0.3.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.930390 fenjing-0.3.9/fenjing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/config_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/form_cracker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5080 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/full_payload_gen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/int_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30746 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/scan_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/shell_payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.934390 fenjing-0.3.9/fenjing/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/waf_func_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-15 06:22:04.000000 fenjing-0.3.9/fenjing/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.934390 fenjing-0.3.9/fenjing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 06:22:16.000000 fenjing-0.3.9/fenjing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 06:22:04.000000 fenjing-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 06:22:16.934390 fenjing-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-15 06:22:04.000000 fenjing-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 06:22:16.934390 fenjing-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-15 06:22:04.000000 fenjing-0.3.9/tests/test_full_payload_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-15 06:22:04.000000 fenjing-0.3.9/tests/test_payload_gen.py
```

### Comparing `fenjing-0.3.8/LICENSE` & `fenjing-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/PKG-INFO` & `fenjing-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.8/README.md` & `fenjing-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/cli.py` & `fenjing-0.3.9/fenjing/cli.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/colorize.py` & `fenjing-0.3.9/fenjing/colorize.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/config_payload.py` & `fenjing-0.3.9/fenjing/config_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/const.py` & `fenjing-0.3.9/fenjing/const.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/form.py` & `fenjing-0.3.9/fenjing/form.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/form_cracker.py` & `fenjing-0.3.9/fenjing/form_cracker.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/full_payload_gen.py` & `fenjing-0.3.9/fenjing/full_payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/int_vars.py` & `fenjing-0.3.9/fenjing/int_vars.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/payload_gen.py` & `fenjing-0.3.9/fenjing/payload_gen.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/requester.py` & `fenjing-0.3.9/fenjing/requester.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/scan_url.py` & `fenjing-0.3.9/fenjing/scan_url.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/shell_payload.py` & `fenjing-0.3.9/fenjing/shell_payload.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/templates/index.html` & `fenjing-0.3.9/fenjing/templates/index.html`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing/waf_func_gen.py` & `fenjing-0.3.9/fenjing/waf_func_gen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from collections import Counter, namedtuple
 from functools import lru_cache
 import logging
 from typing import List, Dict, Tuple, Callable, Any, Union
+import random
+import string
 
 from .const import *
 from .form import fill_form
 from .requester import Requester
 from .colorize import colored
 
 
@@ -14,18 +16,21 @@
 
 
 class WafFuncGen:
     """
     根据指定的表单生成对应的WAF函数
     """
     dangerous_keywords = [
-        "config", "self", "os", "class", "mro", "base", "request",
-        "attr", "open", "system",
-        "[", '"', "'", "_", ".", "+", "{{", "|",
-        "0", "1", "2",
+        '"', "'", "+", ".", "0", "1", "2", "=", "[", "_", "%",
+        "attr", "builtins", "chr", "class", "config", 
+        "eval", "global", "include", 
+        "lipsum", "mro", "namespace", "open",
+        "pop", "popen", "read", "request", "self", 
+        "subprocess", "system", "url_for", "value", 
+        "{{", "|", "}}", "~"
     ]
 
     def __init__(
             self,
             url: str,
             form: Dict[str, Any],
             requester: Requester,
@@ -83,18 +88,23 @@
             logger.info(
                 f"Testing dangerous keyword {colored('yellow', repr(keyword * 3))}")
             resps[keyword] = self.submit({input_field: keyword * 3})
         hashes = [
             hash(r.text) for keyword, r in resps.items()
             if r is not None and r.status_code != 500 and keyword not in r.text
         ]
-        return [pair[0] for pair in Counter(hashes).most_common(2)]
+        return [k for k, v in Counter(hashes).items() if v >= 3]
 
     def generate(self, input_field):
         waf_hashes = self.waf_page_hash(input_field)
 
         @lru_cache(1000)
         def waf_func(value):
-            r = self.submit({input_field: value})
+            extra_content = "".join(random.choices(string.ascii_lowercase, k=6))
+            r = self.submit({input_field: extra_content + value})
             assert r is not None
-            return hash(r.text) not in waf_hashes
+            if hash(r.text) in waf_hashes: # 页面的hash和waf页面的hash相同
+                return False
+            if r.status_code == 500: # Jinja渲染错误
+                return True
+            return extra_content in r.text # 产生回显
         return waf_func
```

### Comparing `fenjing-0.3.8/fenjing/webui.py` & `fenjing-0.3.9/fenjing/webui.py`

 * *Files identical despite different names*

### Comparing `fenjing-0.3.8/fenjing.egg-info/PKG-INFO` & `fenjing-0.3.9/fenjing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fenjing
-Version: 0.3.8
+Version: 0.3.9
 Summary: A Jinja SSTI cracker for CTF competitions
 Home-page: https://github.com/Marven11/Fenjing
 Author: Marven11
 Author-email: marven11@example.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
```

### Comparing `fenjing-0.3.8/fenjing.egg-info/SOURCES.txt` & `fenjing-0.3.9/fenjing.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -21,8 +21,10 @@
 fenjing/waf_func_gen.py
 fenjing/webui.py
 fenjing.egg-info/PKG-INFO
 fenjing.egg-info/SOURCES.txt
 fenjing.egg-info/dependency_links.txt
 fenjing.egg-info/requires.txt
 fenjing.egg-info/top_level.txt
-fenjing/templates/index.html
+fenjing/templates/index.html
+tests/test_full_payload_gen.py
+tests/test_payload_gen.py
```

### Comparing `fenjing-0.3.8/setup.py` & `fenjing-0.3.9/setup.py`

 * *Files identical despite different names*

