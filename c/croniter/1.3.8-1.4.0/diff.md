# Comparing `tmp/croniter-1.3.8.tar.gz` & `tmp/croniter-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croniter-1.3.8.tar", last modified: Tue Nov 22 08:07:19 2022, max compression
+gzip compressed data, was "croniter-1.4.0.tar", last modified: Thu Jun 15 13:29:47 2023, max compression
```

## Comparing `croniter-1.3.8.tar` & `croniter-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2022-11-22 08:07:19.349861 croniter-1.3.8/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    10665 2022-11-22 08:07:19.000000 croniter-1.3.8/CHANGELOG.rst
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     1064 2022-11-22 08:07:19.000000 croniter-1.3.8/LICENSE
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      136 2022-11-22 08:07:19.000000 croniter-1.3.8/MANIFEST.in
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    23032 2022-11-22 08:07:19.349861 croniter-1.3.8/PKG-INFO
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    11054 2022-11-22 08:07:19.000000 croniter-1.3.8/README.rst
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2022-11-22 08:07:19.349861 croniter-1.3.8/requirements/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       21 2022-11-22 08:07:19.000000 croniter-1.3.8/requirements/base.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       44 2022-11-22 08:07:19.000000 croniter-1.3.8/requirements/release.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      109 2022-11-22 08:07:19.000000 croniter-1.3.8/requirements/test.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      324 2022-11-22 08:07:19.349861 croniter-1.3.8/setup.cfg
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     2071 2022-11-22 08:07:19.000000 croniter-1.3.8/setup.py
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2022-11-22 08:07:19.349861 croniter-1.3.8/src/
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2022-11-22 08:07:19.349861 croniter-1.3.8/src/croniter/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      380 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter/__init__.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    35173 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter/croniter.py
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2022-11-22 08:07:19.349861 croniter-1.3.8/src/croniter/tests/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        0 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter/tests/__init__.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      282 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter/tests/base.py
--rwxrwxr-x   0 kiorky    (1000) kiorky    (1000)    55865 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter/tests/test_croniter.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     6646 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter/tests/test_croniter_hash.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     1705 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter/tests/test_croniter_random.py
--rwxrwxr-x   0 kiorky    (1000) kiorky    (1000)     6786 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter/tests/test_croniter_range.py
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     5715 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter/tests/test_speed.py
-drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2022-11-22 08:07:19.349861 croniter-1.3.8/src/croniter.egg-info/
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    23032 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter.egg-info/PKG-INFO
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      622 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter.egg-info/SOURCES.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        1 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter.egg-info/dependency_links.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       16 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter.egg-info/requires.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        9 2022-11-22 08:07:19.000000 croniter-1.3.8/src/croniter.egg-info/top_level.txt
--rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      619 2022-11-22 08:07:19.000000 croniter-1.3.8/tox.ini
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2023-06-15 13:29:47.706512 croniter-1.4.0/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    11526 2023-06-15 13:29:47.000000 croniter-1.4.0/CHANGELOG.rst
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     1064 2023-06-15 13:29:47.000000 croniter-1.4.0/LICENSE
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      136 2023-06-15 13:29:47.000000 croniter-1.4.0/MANIFEST.in
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    23930 2023-06-15 13:29:47.706512 croniter-1.4.0/PKG-INFO
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    11091 2023-06-15 13:29:47.000000 croniter-1.4.0/README.rst
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2023-06-15 13:29:47.706512 croniter-1.4.0/requirements/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       21 2023-06-15 13:29:47.000000 croniter-1.4.0/requirements/base.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       44 2023-06-15 13:29:47.000000 croniter-1.4.0/requirements/release.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      109 2023-06-15 13:29:47.000000 croniter-1.4.0/requirements/test.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      324 2023-06-15 13:29:47.706512 croniter-1.4.0/setup.cfg
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     2071 2023-06-15 13:29:47.000000 croniter-1.4.0/setup.py
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2023-06-15 13:29:47.706512 croniter-1.4.0/src/
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2023-06-15 13:29:47.706512 croniter-1.4.0/src/croniter/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      380 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter/__init__.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    37090 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter/croniter.py
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2023-06-15 13:29:47.706512 croniter-1.4.0/src/croniter/tests/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        0 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter/tests/__init__.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      282 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter/tests/base.py
+-rwxrwxr-x   0 kiorky    (1000) kiorky    (1000)    60236 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter/tests/test_croniter.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    17186 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter/tests/test_croniter_hash.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     1705 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter/tests/test_croniter_random.py
+-rwxrwxr-x   0 kiorky    (1000) kiorky    (1000)     6786 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter/tests/test_croniter_range.py
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)     5715 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter/tests/test_speed.py
+drwxrwxr-x   0 kiorky    (1000) kiorky    (1000)        0 2023-06-15 13:29:47.706512 croniter-1.4.0/src/croniter.egg-info/
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)    23930 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter.egg-info/PKG-INFO
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      622 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        1 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)       16 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter.egg-info/requires.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)        9 2023-06-15 13:29:47.000000 croniter-1.4.0/src/croniter.egg-info/top_level.txt
+-rw-rw-r--   0 kiorky    (1000) kiorky    (1000)      619 2023-06-15 13:29:47.000000 croniter-1.4.0/tox.ini
```

### Comparing `croniter-1.3.8/CHANGELOG.rst` & `croniter-1.4.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,57 @@
 Changelog
 ==============
 
+1.4.0 (2023-06-15)
+------------------
+
+- Added "implement_cron_bug" flag to make the cron parser compatible with a bug in Vixie/ISC Cron
+  [kiorky, David White <dwhite2@cisco.com>]
+  *WARNING*: EXPAND METHOD CHANGES RETURN VALUE
+
+
+1.3.15 (2023-05-25)
+-------------------
+
+- Fix hashed expressions omitting some entries
+  [@waltervos/Walter Vos <walter.vos@ns.nl>]
+- Enhance .match() precision for 6 position expressions
+  [@szpol/szymon <szymon.polinkiewicz@gmail.com>]
+
+1.3.14 (2023-04-12)
+-------------------
+
+- Lint
+
+
+1.3.13 (2023-04-12)
+-------------------
+
+- Add check for range begin/end
+
+
+
+1.3.12 (2023-04-12)
+-------------------
+
+- restore py2 compat
+
+
+1.3.11 (2023-04-12)
+-------------------
+
+-  Do not expose `i` into global namespace
+
+
+1.3.10 (2023-04-07)
+-------------------
+
+- Fix DOW hash parsing [kiorky]
+- better error handling on py3 [kiorky]
+
 1.3.8 (2022-11-22)
 ------------------
 
 - Add Python 3.11 support and move docs files to main folder [rafsaf]
 
 
 1.3.7 (2022-09-06)
```

### Comparing `croniter-1.3.8/LICENSE` & `croniter-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `croniter-1.3.8/PKG-INFO` & `croniter-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croniter
-Version: 1.3.8
+Version: 1.4.0
 Summary: croniter provides iteration for datetime object with cron like format
 Home-page: http://github.com/kiorky/croniter
 Author: Matsumoto Taichi, kiorky
 Author-email: taichino@gmail.com, kiorky@cryptelium.net
 License: MIT License
 Keywords: datetime,iterator,cron
 Platform: UNKNOWN
@@ -44,18 +44,18 @@
      / __| '__/ _ \| '_ \| | __/ _ \ '__|
     | (__| | | (_) | | | | | ||  __/ |
      \___|_|  \___/|_| |_|_|\__\___|_|
 
 
 Website: https://github.com/kiorky/croniter
 
-Travis badge
-=============
-.. image:: https://travis-ci.org/kiorky/croniter.svg?branch=master
-    :target: https://travis-ci.org/kiorky/croniter
+Build Badge
+===========
+.. image:: https://github.com/kiorky/croniter/actions/workflows/cicd.yml/badge.svg
+    :target: https://github.com/kiorky/croniter/actions/workflows/cicd.yml
 
 
 Usage
 ============
 
 A simple example::
 
@@ -319,14 +319,61 @@
     - Ryan Finnie (rfinnie)
 
 
 
 Changelog
 ==============
 
+1.4.0 (2023-06-15)
+------------------
+
+- Added "implement_cron_bug" flag to make the cron parser compatible with a bug in Vixie/ISC Cron
+  [kiorky, David White <dwhite2@cisco.com>]
+  *WARNING*: EXPAND METHOD CHANGES RETURN VALUE
+
+
+1.3.15 (2023-05-25)
+-------------------
+
+- Fix hashed expressions omitting some entries
+  [@waltervos/Walter Vos <walter.vos@ns.nl>]
+- Enhance .match() precision for 6 position expressions
+  [@szpol/szymon <szymon.polinkiewicz@gmail.com>]
+
+1.3.14 (2023-04-12)
+-------------------
+
+- Lint
+
+
+1.3.13 (2023-04-12)
+-------------------
+
+- Add check for range begin/end
+
+
+
+1.3.12 (2023-04-12)
+-------------------
+
+- restore py2 compat
+
+
+1.3.11 (2023-04-12)
+-------------------
+
+-  Do not expose `i` into global namespace
+
+
+1.3.10 (2023-04-07)
+-------------------
+
+- Fix DOW hash parsing [kiorky]
+- better error handling on py3 [kiorky]
+
 1.3.8 (2022-11-22)
 ------------------
 
 - Add Python 3.11 support and move docs files to main folder [rafsaf]
 
 
 1.3.7 (2022-09-06)
```

### Comparing `croniter-1.3.8/README.rst` & `croniter-1.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
      / __| '__/ _ \| '_ \| | __/ _ \ '__|
     | (__| | | (_) | | | | | ||  __/ |
      \___|_|  \___/|_| |_|_|\__\___|_|
 
 
 Website: https://github.com/kiorky/croniter
 
-Travis badge
-=============
-.. image:: https://travis-ci.org/kiorky/croniter.svg?branch=master
-    :target: https://travis-ci.org/kiorky/croniter
+Build Badge
+===========
+.. image:: https://github.com/kiorky/croniter/actions/workflows/cicd.yml/badge.svg
+    :target: https://github.com/kiorky/croniter/actions/workflows/cicd.yml
 
 
 Usage
 ============
 
 A simple example::
```

### Comparing `croniter-1.3.8/setup.py` & `croniter-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         read('README.rst'),
         read('CHANGELOG.rst'),
     ]
 )
 
 setup(
     name='croniter',
-    version='1.3.8',
+    version='1.4.0',
     py_modules=['croniter', ],
     description=(
         'croniter provides iteration for datetime '
         'object with cron like format'
     ),
     long_description=long_description,
     author="Matsumoto Taichi, kiorky",
```

### Comparing `croniter-1.3.8/src/croniter/croniter.py` & `croniter-1.4.0/src/croniter/croniter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from __future__ import absolute_import, print_function, division
 
+import traceback as _traceback
+import copy
 import math
 import re
 import sys
 import inspect
 from time import time
 import datetime
 from dateutil.relativedelta import relativedelta
@@ -17,18 +19,32 @@
 
 try:
     from collections import OrderedDict
 except ImportError:
     OrderedDict = dict  # py26 degraded mode, expanders order will not be immutable
 
 
+M_ALPHAS = {'jan': 1, 'feb': 2, 'mar': 3, 'apr': 4, 'may': 5, 'jun': 6,
+            'jul': 7, 'aug': 8, 'sep': 9, 'oct': 10, 'nov': 11, 'dec': 12}
+DOW_ALPHAS = {'sun': 0, 'mon': 1, 'tue': 2, 'wed': 3, 'thu': 4, 'fri': 5, 'sat': 6}
+ALPHAS = {}
+for i in M_ALPHAS, DOW_ALPHAS:
+    ALPHAS.update(i)
+del i
 step_search_re = re.compile(r'^([^-]+)-([^-/]+)(/(\d+))?$')
 only_int_re = re.compile(r'^\d+$')
+
+WEEKDAYS = '|'.join(DOW_ALPHAS.keys())
+MONTHS = '|'.join(M_ALPHAS.keys())
 star_or_int_re = re.compile(r'^(\d+|\*)$')
-special_weekday_re = re.compile(r'^(\w+)#(\d+)|l(\d+)$')
+special_dow_re = re.compile(
+    (r'^(?P<pre>((?P<he>(({WEEKDAYS})(-({WEEKDAYS}))?)').format(WEEKDAYS=WEEKDAYS) +
+    (r'|(({MONTHS})(-({MONTHS}))?)|\w+)#)|l)(?P<last>\d+)$').format(MONTHS=MONTHS)
+)
+re_star = re.compile('[*]')
 hash_expression_re = re.compile(
     r'^(?P<hash_type>h|r)(\((?P<range_begin>\d+)-(?P<range_end>\d+)\))?(\/(?P<divisor>\d+))?$'
 )
 VALID_LEN_EXPRESSION = [5, 6]
 
 
 def timedelta_to_seconds(td):
@@ -102,18 +118,17 @@
     )
 
     ALPHACONV = (
         {},  # 0: min
         {},  # 1: hour
         {"l": "l"},  # 2: dom
         # 3: mon
-        {'jan': 1, 'feb': 2, 'mar': 3, 'apr': 4, 'may': 5, 'jun': 6,
-         'jul': 7, 'aug': 8, 'sep': 9, 'oct': 10, 'nov': 11, 'dec': 12},
+        copy.deepcopy(M_ALPHAS),
         # 4: dow
-        {'sun': 0, 'mon': 1, 'tue': 2, 'wed': 3, 'thu': 4, 'fri': 5, 'sat': 6},
+        copy.deepcopy(DOW_ALPHAS),
         # command/user
         {}
     )
 
     LOWMAP = (
         {},
         {},
@@ -133,17 +148,18 @@
     )
 
     bad_length = 'Exactly 5 or 6 columns has to be specified for iterator ' \
                  'expression.'
 
     def __init__(self, expr_format, start_time=None, ret_type=float,
                  day_or=True, max_years_between_matches=None, is_prev=False,
-                 hash_id=None):
+                 hash_id=None, implement_cron_bug=False):
         self._ret_type = ret_type
         self._day_or = day_or
+        self._implement_cron_bug = implement_cron_bug
 
         if hash_id:
             if not isinstance(hash_id, (bytes, str)):
                 raise TypeError('hash_id must be bytes or UTF-8 string')
             if not isinstance(hash_id, bytes):
                 hash_id = hash_id.encode('UTF-8')
 
@@ -159,15 +175,15 @@
         self.tzinfo = None
 
         self.start_time = None
         self.dst_start_time = None
         self.cur = None
         self.set_current(start_time, force=False)
 
-        self.expanded, self.nth_weekday_of_month = self.expand(expr_format, hash_id=hash_id)
+        self.expanded, self.nth_weekday_of_month, self.expressions = self.expand(expr_format, hash_id=hash_id)
         self._is_prev = is_prev
 
     @classmethod
     def _alphaconv(cls, index, key, expressions):
         try:
             return cls.ALPHACONV[index][key]
         except KeyError:
@@ -236,27 +252,38 @@
         ret_type = ret_type or self._ret_type
 
         if not issubclass(ret_type, (float, datetime.datetime)):
             raise TypeError("Invalid ret_type, only 'float' or 'datetime' "
                             "is acceptable.")
 
         # exception to support day of month and day of week as defined in cron
+        dom_dow_exception_processed = False
         if (expanded[2][0] != '*' and expanded[4][0] != '*') and self._day_or:
-            bak = expanded[4]
-            expanded[4] = ['*']
-            t1 = self._calc(self.cur, expanded, nth_weekday_of_month, is_prev)
-            expanded[4] = bak
-            expanded[2] = ['*']
-
-            t2 = self._calc(self.cur, expanded, nth_weekday_of_month, is_prev)
-            if not is_prev:
-                result = t1 if t1 < t2 else t2
+            # If requested, handle a bug in vixie cron/ISC cron where day_of_month and day_of_week form
+            # an intersection (AND) instead of a union (OR) if either field is an asterisk or starts with an asterisk
+            # (https://crontab.guru/cron-bug.html)
+            if self._implement_cron_bug and (re_star.match(self.expressions[2]) or re_star.match(self.expressions[4])):
+                # To produce a schedule identical to the cron bug, we'll bypass the code that
+                # makes a union of DOM and DOW, and instead skip to the code that does an intersect instead
+                pass
             else:
-                result = t1 if t1 > t2 else t2
-        else:
+                bak = expanded[4]
+                expanded[4] = ['*']
+                t1 = self._calc(self.cur, expanded, nth_weekday_of_month, is_prev)
+                expanded[4] = bak
+                expanded[2] = ['*']
+
+                t2 = self._calc(self.cur, expanded, nth_weekday_of_month, is_prev)
+                if not is_prev:
+                    result = t1 if t1 < t2 else t2
+                else:
+                    result = t1 if t1 > t2 else t2
+                dom_dow_exception_processed = True
+
+        if not dom_dow_exception_processed:
             result = self._calc(self.cur, expanded,
                                 nth_weekday_of_month, is_prev)
 
         # DST Handling for cron job spanning across days
         dtstarttime = self._timestamp_to_datetime(self.dst_start_time)
         dtstarttime_utcoffset = (
             dtstarttime.utcoffset() or datetime.timedelta(0))
@@ -631,35 +658,34 @@
                 expr = expander(cls).expand(efl, i, expr, hash_id=hash_id)
 
             e_list = expr.split(',')
             res = []
 
             while len(e_list) > 0:
                 e = e_list.pop()
+                nth = None
 
                 if i == 4:
-                    # Handle special case in the day-of-week expression
-                    m = special_weekday_re.match(str(e))
-                    if m:
-                        orig_e = e
-                        e, nth, last = m.groups()
-                        if nth:
+                    # Handle special case in the dow expression: 2#3, l3
+                    special_dow_rem = special_dow_re.match(str(e))
+                    if special_dow_rem:
+                        g = special_dow_rem.groupdict()
+                        he, last = g.get('he', ''), g.get('last', '')
+                        if he:
+                            e = he
                             try:
-                                nth = int(nth)
+                                nth = int(last)
                                 assert (nth >= 1 and nth <= 5)
-                            except (ValueError, AssertionError):
+                            except (KeyError, ValueError, AssertionError):
                                 raise CroniterBadCronError(
                                     "[{0}] is not acceptable.  Invalid day_of_week "
-                                    "value: '{1}'".format(expr_format, orig_e))
+                                    "value: '{1}'".format(expr_format, nth))
                         elif last:
-                            nth = "l"
                             e = last
-                        del last, orig_e
-                    else:
-                        nth = None
+                            nth = g['pre']  # 'l'
 
                 # Before matching step_search_re, normalize "*" to "{min}-{max}".
                 # Example: in the minute field, "*/5" normalizes to "0-59/5"
                 t = re.sub(r'^\*(\/.+)$', r'%d-%d\1' % (
                     cls.RANGES[i][0],
                     cls.RANGES[i][1]),
                     str(e))
@@ -765,28 +791,29 @@
             dow_expanded_set = dow_expanded_set.difference(nth_weekday_of_month.keys())
             dow_expanded_set.discard("*")
             if dow_expanded_set:
                 raise CroniterUnsupportedSyntaxError(
                     "day-of-week field does not support mixing literal values and nth day of week syntax.  "
                     "Cron: '{}'    dow={} vs nth={}".format(expr_format, dow_expanded_set, nth_weekday_of_month))
 
-        return expanded, nth_weekday_of_month
+        return expanded, nth_weekday_of_month, expressions
 
     @classmethod
     def expand(cls, expr_format, hash_id=None):
         """Shallow non Croniter ValueError inside a nice CroniterBadCronError"""
         try:
             return cls._expand(expr_format, hash_id=hash_id)
-        except ValueError as exc:
+        except (ValueError,) as exc:
             error_type, error_instance, traceback = sys.exc_info()
             if isinstance(exc, CroniterError):
                 raise
             if int(sys.version[0]) >= 3:
+                trace = _traceback.format_exc()
                 globs, locs = _get_caller_globals_and_locals()
-                exec("raise CroniterBadCronError from  exc", globs, locs)
+                raise CroniterBadCronError(trace)
             else:
                 raise CroniterBadCronError("{0}".format(exc))
 
     @classmethod
     def is_valid(cls, expression, hash_id=None):
         try:
             cls.expand(expression, hash_id=hash_id)
@@ -799,15 +826,16 @@
     def match(cls, cron_expression, testdate, day_or=True):
         cron = cls(cron_expression, testdate, ret_type=datetime.datetime, day_or=day_or)
         td, ms1 = cron.get_current(datetime.datetime), relativedelta(microseconds=1)
         if not td.microsecond:
             td = td + ms1
         cron.set_current(td, force=True)
         tdp, tdt = cron.get_current(), cron.get_prev()
-        return (max(tdp, tdt) - min(tdp, tdt)).total_seconds() < 60
+        precision_in_seconds = 1 if len(cron.expanded) == 6 else 60
+        return (max(tdp, tdt) - min(tdp, tdt)).total_seconds() < precision_in_seconds
 
 
 def croniter_range(start, stop, expr_format, ret_type=None, day_or=True, exclude_ends=False,
                    _croniter=None):
     """
     Generator that provides all times from start to stop matching the given cron expression.
     If the cron expression matches either 'start' and/or 'stop', those times will be returned as
@@ -868,23 +896,28 @@
 class HashExpander:
 
     def __init__(self, cronit):
         self.cron = cronit
 
     def do(self, idx, hash_type="h", hash_id=None, range_end=None, range_begin=None):
         """Return a hashed/random integer given range/hash information"""
+        hours_or_minutes = idx in {0, 1}
         if range_end is None:
             range_end = self.cron.RANGES[idx][1]
+            if hours_or_minutes:
+                range_end += 1
         if range_begin is None:
             range_begin = self.cron.RANGES[idx][0]
         if hash_type == 'r':
             crc = random.randint(0, 0xFFFFFFFF)
         else:
             crc = binascii.crc32(hash_id) & 0xFFFFFFFF
-        return ((crc >> idx) % (range_end - range_begin + 1)) + range_begin
+        if not hours_or_minutes:
+            return ((crc >> idx) % (range_end - range_begin + 1)) + range_begin
+        return ((crc >> idx) % (range_end - range_begin)) + range_begin
 
     def match(self, efl, idx, expr, hash_id=None, **kw):
         return hash_expression_re.match(expr)
 
     def expand(self, efl, idx, expr, hash_id=None, match='', **kw):
         """Expand a hashed/random expression to its normal representation"""
         if match == '':
@@ -892,14 +925,18 @@
         if not match:
             return expr
         m = match.groupdict()
 
         if m['hash_type'] == 'h' and hash_id is None:
             raise CroniterBadCronError('Hashed definitions must include hash_id')
 
+        if m['range_begin'] and m['range_end']:
+            if int(m['range_begin']) >= int(m['range_end']):
+                raise CroniterBadCronError('Range end must be greater than range begin')
+
         if m['range_begin'] and m['range_end'] and m['divisor']:
             # Example: H(30-59)/10 -> 34-59/10 (i.e. 34,44,54)
             if int(m["divisor"]) == 0:
                 raise CroniterBadCronError("Bad expression: {0}".format(expr))
 
             return '{0}-{1}/{2}'.format(
                 self.do(
```

### Comparing `croniter-1.3.8/src/croniter/tests/test_croniter.py` & `croniter-1.4.0/src/croniter/tests/test_croniter.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,31 @@
         self.assertEqual(n2.day, 1)
         self.assertEqual(n2.year, 2010)
         n3 = itr.get_next(datetime)
         self.assertEqual(n3.month, 11)
         self.assertEqual(n3.day, 1)
         self.assertEqual(n3.year, 2010)
 
+    def testDomDowVixieCronBug(self):
+        expr = '0 16 */2 * sat'
+
+        # UNION OF "every odd-numbered day" and "every Saturday"
+        itr = croniter(expr, start_time=datetime(2023, 5, 2), ret_type=datetime)
+        self.assertEqual(itr.get_next(), datetime(2023, 5, 3, 16, 0, 0))    # Wed May 3 2023
+        self.assertEqual(itr.get_next(), datetime(2023, 5, 5, 16, 0, 0))    # Fri May 5 2023
+        self.assertEqual(itr.get_next(), datetime(2023, 5, 6, 16, 0, 0))    # Sat May 6 2023
+        self.assertEqual(itr.get_next(), datetime(2023, 5, 7, 16, 0, 0))    # Sun May 7 2023
+
+        # INTERSECTION OF "every odd-numbered day" and "every Saturday"
+        itr = croniter(expr, start_time=datetime(2023, 5, 2), ret_type=datetime, implement_cron_bug=True)
+        self.assertEqual(itr.get_next(), datetime(2023, 5, 13, 16, 0, 0))    # Sat May  13 2023
+        self.assertEqual(itr.get_next(), datetime(2023, 5, 27, 16, 0, 0))    # Sat May  27 2023
+        self.assertEqual(itr.get_next(), datetime(2023, 6, 3, 16, 0, 0))     # Sat June  3 2023
+        self.assertEqual(itr.get_next(), datetime(2023, 6, 17, 16, 0, 0))    # Sun June 17 2023
+
     def testMonth(self):
         base = datetime(2010, 1, 25)
         itr = croniter('0 0 1 * *', base)
         n1 = itr.get_next(datetime)
         self.assertEqual(n1.month, 2)
         self.assertEqual(n1.day, 1)
         n2 = itr.get_next(datetime)
@@ -1011,14 +1028,22 @@
             datetime(2019, 1, 14, 0, 0, 0, 0)
         ))
         self.assertFalse(croniter.match(
             "0 0 * * *",
             datetime(2019, 1, 14, 0, 1, 0, 0)
         ))
         self.assertTrue(croniter.match(
+            "0 0 * * * 1",
+            datetime(2023, 5, 25, 0, 0, 1, 0)
+        ))
+        self.assertFalse(croniter.match(
+            "0 0 * * * 1",
+            datetime(2023, 5, 25, 0, 0, 2, 0)
+        ))
+        self.assertTrue(croniter.match(
             "31 * * * *",
             datetime(2019, 1, 14, 1, 31, 0, 0)
         ))
         self.assertTrue(croniter.match(
             "0 0 10 * wed",
             datetime(2020, 6, 10, 0, 0, 0, 0),
             day_or=True
@@ -1469,10 +1494,76 @@
         base = datetime(2010, 1, 23, 12, 18, tzinfo=tz)
         itr = croniter('* * * * *')
         itr.set_current(start_time=base)
         n1 = itr.get_next()   # 19
 
         self.assertEqual(n1, datetime_to_timestamp(base) + 60)
 
+    def test_issue_k34(self):
+        # invalid cron, but should throw appropriate exception
+        self.assertRaises(CroniterBadCronError, croniter, "4 0 L/2 2 0")
+
+    def test_issue_k33(self):
+        y = 2018
+        # At 11:30 PM, between day 1 and 7 of the month, Monday through Friday, only in January
+        ret = []
+        for i in range(10):
+            cron = croniter("30 23 1-7 JAN MON-FRI#1", datetime(y+i, 1, 1), ret_type=datetime)
+            for j in range(7):
+                d = cron.get_next()
+                if d.year == y + i:
+                    ret.append(d)
+        rets = [datetime(2018, 1, 1, 23, 30),
+                datetime(2018, 1, 2, 23, 30),
+                datetime(2018, 1, 3, 23, 30),
+                datetime(2018, 1, 4, 23, 30),
+                datetime(2018, 1, 5, 23, 30),
+                datetime(2019, 1, 1, 23, 30),
+                datetime(2019, 1, 2, 23, 30),
+                datetime(2019, 1, 3, 23, 30),
+                datetime(2019, 1, 4, 23, 30),
+                datetime(2019, 1, 7, 23, 30),
+                datetime(2020, 1, 1, 23, 30),
+                datetime(2020, 1, 2, 23, 30),
+                datetime(2020, 1, 3, 23, 30),
+                datetime(2020, 1, 6, 23, 30),
+                datetime(2020, 1, 7, 23, 30),
+                datetime(2021, 1, 1, 23, 30),
+                datetime(2021, 1, 4, 23, 30),
+                datetime(2021, 1, 5, 23, 30),
+                datetime(2021, 1, 6, 23, 30),
+                datetime(2021, 1, 7, 23, 30),
+                datetime(2022, 1, 3, 23, 30),
+                datetime(2022, 1, 4, 23, 30),
+                datetime(2022, 1, 5, 23, 30),
+                datetime(2022, 1, 6, 23, 30),
+                datetime(2022, 1, 7, 23, 30),
+                datetime(2023, 1, 2, 23, 30),
+                datetime(2023, 1, 3, 23, 30),
+                datetime(2023, 1, 4, 23, 30),
+                datetime(2023, 1, 5, 23, 30),
+                datetime(2023, 1, 6, 23, 30),
+                datetime(2024, 1, 1, 23, 30),
+                datetime(2024, 1, 2, 23, 30),
+                datetime(2024, 1, 3, 23, 30),
+                datetime(2024, 1, 4, 23, 30),
+                datetime(2024, 1, 5, 23, 30),
+                datetime(2025, 1, 1, 23, 30),
+                datetime(2025, 1, 2, 23, 30),
+                datetime(2025, 1, 3, 23, 30),
+                datetime(2025, 1, 6, 23, 30),
+                datetime(2025, 1, 7, 23, 30),
+                datetime(2026, 1, 1, 23, 30),
+                datetime(2026, 1, 2, 23, 30),
+                datetime(2026, 1, 5, 23, 30),
+                datetime(2026, 1, 6, 23, 30),
+                datetime(2026, 1, 7, 23, 30),
+                datetime(2027, 1, 1, 23, 30),
+                datetime(2027, 1, 4, 23, 30),
+                datetime(2027, 1, 5, 23, 30),
+                datetime(2027, 1, 6, 23, 30),
+                datetime(2027, 1, 7, 23, 30)]
+        self.assertEqual(ret, rets)
+        croniter.expand("30 6 1-7 MAY MON#1")
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `croniter-1.3.8/src/croniter/tests/test_croniter_random.py` & `croniter-1.4.0/src/croniter/tests/test_croniter_random.py`

 * *Files identical despite different names*

### Comparing `croniter-1.3.8/src/croniter/tests/test_croniter_range.py` & `croniter-1.4.0/src/croniter/tests/test_croniter_range.py`

 * *Files identical despite different names*

### Comparing `croniter-1.3.8/src/croniter/tests/test_speed.py` & `croniter-1.4.0/src/croniter/tests/test_speed.py`

 * *Files identical despite different names*

### Comparing `croniter-1.3.8/src/croniter.egg-info/PKG-INFO` & `croniter-1.4.0/src/croniter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croniter
-Version: 1.3.8
+Version: 1.4.0
 Summary: croniter provides iteration for datetime object with cron like format
 Home-page: http://github.com/kiorky/croniter
 Author: Matsumoto Taichi, kiorky
 Author-email: taichino@gmail.com, kiorky@cryptelium.net
 License: MIT License
 Keywords: datetime,iterator,cron
 Platform: UNKNOWN
@@ -44,18 +44,18 @@
      / __| '__/ _ \| '_ \| | __/ _ \ '__|
     | (__| | | (_) | | | | | ||  __/ |
      \___|_|  \___/|_| |_|_|\__\___|_|
 
 
 Website: https://github.com/kiorky/croniter
 
-Travis badge
-=============
-.. image:: https://travis-ci.org/kiorky/croniter.svg?branch=master
-    :target: https://travis-ci.org/kiorky/croniter
+Build Badge
+===========
+.. image:: https://github.com/kiorky/croniter/actions/workflows/cicd.yml/badge.svg
+    :target: https://github.com/kiorky/croniter/actions/workflows/cicd.yml
 
 
 Usage
 ============
 
 A simple example::
 
@@ -319,14 +319,61 @@
     - Ryan Finnie (rfinnie)
 
 
 
 Changelog
 ==============
 
+1.4.0 (2023-06-15)
+------------------
+
+- Added "implement_cron_bug" flag to make the cron parser compatible with a bug in Vixie/ISC Cron
+  [kiorky, David White <dwhite2@cisco.com>]
+  *WARNING*: EXPAND METHOD CHANGES RETURN VALUE
+
+
+1.3.15 (2023-05-25)
+-------------------
+
+- Fix hashed expressions omitting some entries
+  [@waltervos/Walter Vos <walter.vos@ns.nl>]
+- Enhance .match() precision for 6 position expressions
+  [@szpol/szymon <szymon.polinkiewicz@gmail.com>]
+
+1.3.14 (2023-04-12)
+-------------------
+
+- Lint
+
+
+1.3.13 (2023-04-12)
+-------------------
+
+- Add check for range begin/end
+
+
+
+1.3.12 (2023-04-12)
+-------------------
+
+- restore py2 compat
+
+
+1.3.11 (2023-04-12)
+-------------------
+
+-  Do not expose `i` into global namespace
+
+
+1.3.10 (2023-04-07)
+-------------------
+
+- Fix DOW hash parsing [kiorky]
+- better error handling on py3 [kiorky]
+
 1.3.8 (2022-11-22)
 ------------------
 
 - Add Python 3.11 support and move docs files to main folder [rafsaf]
 
 
 1.3.7 (2022-09-06)
```

### Comparing `croniter-1.3.8/src/croniter.egg-info/SOURCES.txt` & `croniter-1.4.0/src/croniter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `croniter-1.3.8/tox.ini` & `croniter-1.4.0/tox.ini`

 * *Files identical despite different names*

