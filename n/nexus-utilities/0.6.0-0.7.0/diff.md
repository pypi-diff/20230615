# Comparing `tmp/nexus-utilities-0.6.0.tar.gz` & `tmp/nexus-utilities-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.6.0.tar", last modified: Sat Jun  3 15:57:03 2023, max compression
+gzip compressed data, was "nexus-utilities-0.7.0.tar", last modified: Thu Jun 15 19:04:21 2023, max compression
```

## Comparing `nexus-utilities-0.6.0.tar` & `nexus-utilities-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:57:03.239004 nexus-utilities-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-03 15:57:03.239004 nexus-utilities-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:57:03.235004 nexus-utilities-0.6.0/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-03 15:57:02.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-03 15:57:03.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:57:02.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-03 15:57:02.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-03 15:57:02.000000 nexus-utilities-0.6.0/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:57:03.239004 nexus-utilities-0.6.0/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/nexus_utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 15:57:03.239004 nexus-utilities-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-03 15:56:49.000000 nexus-utilities-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:04:21.440708 nexus-utilities-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-15 19:04:21.440708 nexus-utilities-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:04:21.436708 nexus-utilities-0.7.0/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-15 19:04:21.000000 nexus-utilities-0.7.0/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 19:04:21.440708 nexus-utilities-0.7.0/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11429 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/nexus_utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 19:04:21.440708 nexus-utilities-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-15 19:04:08.000000 nexus-utilities-0.7.0/setup.py
```

### Comparing `nexus-utilities-0.6.0/LICENSE.txt` & `nexus-utilities-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.6.0/PKG-INFO` & `nexus-utilities-0.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.6.0
+Version: 0.7.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
```

### Comparing `nexus-utilities-0.6.0/README.md` & `nexus-utilities-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 - [datetime\_utils.py](#datetime_utilspy)
   - [**get\_current\_timestamp()**](#get_current_timestamp)
   - [**get\_duration(then, now=datetime.datetime.now())**](#get_durationthen-nowdatetimedatetimenow)
   - [**determine\_date\_format(date\_list)**](#determine_date_formatdate_list)
 - [flatfile\_utils.py](#flatfile_utilspy)
   - [**detect\_encoding(file\_path)**](#detect_encodingfile_path)
   - [**analyze\_dataframe(df)**](#analyze_dataframedf)
+  - [**check\_primary\_key\_fields(df, field\_list, print\_results=True)**](#check_primary_key_fieldsdf-field_list-print_resultstrue)
 - [package\_utils.py](#package_utilspy)
   - [**add\_package\_to\_path()**](#add_package_to_path)
   - [**import\_relative(package\_root\_name, module\_path, import\_name, alias=None)**](#import_relativepackage_root_name-module_path-import_name-aliasnone)
   - [**extract\_from\_error(full\_error\_message, error\_keyword)**](#extract_from_errorfull_error_message-error_keyword)
 - [password\_utils.py](#password_utilspy)
   - [**get\_password(password\_method, password\_key, account\_name=None, access\_key=None, secret\_key=None, endpoint\_url=None, region\_name=None, password\_path=None, encoding='utf-8')**](#get_passwordpassword_method-password_key-account_namenone-access_keynone-secret_keynone-endpoint_urlnone-region_namenone-password_pathnone-encodingutf-8)
 - [string\_utils.py](#string_utilspy)
@@ -201,14 +202,28 @@
 |More than 50 distinct values|Distinct Values: *{count}*|&nbsp;|&nbsp;|&nbsp;|&nbsp;|
 |||||||
 
 ***Notes:***
  * *{summary_metric}*: Will either be "Max Length: {value}" for strings, or "Max Value: {value}" for numeric values and dates.  Can be useful for estimating field size when designing tables
  * Will show up to 50 distinct values, sorted by number of occurrences descending.  If there are more than 50 distinct values, a note will be shown at the bottom of the list, along with the total number of distinct values
 
+### **check_primary_key_fields(df, field_list, print_results=True)**
+
+Arguments:
+ * ***df (pandas dataframe):*** Dataframe to check
+ * ***field_list (list):*** List of fields to check for duplicate values
+ * ***print_results (bool):*** Whether to print results to the terminal
+
+Returns:
+ * ***is_unique (bool):*** Indicator of whether the provided set of fields are unique in the data frame
+ * ***no_nulls (bool):*** Indicator of whether the provided set of fields have any NULL values
+ * ***sample_issue_rows (pandas dataframe):*** Sample rows from the data frame showing duplicates or NULLs
+
+Checks a data frame given a list of fields to see if they have duplicates or contain any NULL values.  Useful when trying to determine a Primary Key for a table to land data into.
+
 ---
 
 ## package_utils.py
 
 This module contains functions for working with Python packages.
 
 ### **add_package_to_path()**
```

### Comparing `nexus-utilities-0.6.0/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.7.0/nexus_utilities.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.6.0
+Version: 0.7.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
```

### Comparing `nexus-utilities-0.6.0/nexus_utils/config_utils.py` & `nexus-utilities-0.7.0/nexus_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.6.0/nexus_utils/database_utils.py` & `nexus-utilities-0.7.0/nexus_utils/database_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.6.0/nexus_utils/datetime_utils.py` & `nexus-utilities-0.7.0/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.6.0/nexus_utils/package_utils.py` & `nexus-utilities-0.7.0/nexus_utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.6.0/nexus_utils/password_utils.py` & `nexus-utilities-0.7.0/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.6.0/nexus_utils/string_utils.py` & `nexus-utilities-0.7.0/nexus_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.6.0/setup.py` & `nexus-utilities-0.7.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.6.0',
+    version='0.7.0',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
     install_requires=[
-        'boto3>=1.26.45',
-        'configparser >=5.3.0',
-        'sqlalchemy>=1.4.44',
-        'keyring>=23.13.1',
-        'chardet>=3.0.4',
-        'twine>=3.4.0'
+        'boto3>=1.26.45,<2.0.0',
+        'configparser>=5.3.0,<6.0.0',
+        'sqlalchemy>=1.4.44,<2.0.0',
+        'keyring>=23.13.1,<24.0.0',
+        'chardet>=3.0.4,<4.0.0',
+        'twine>=3.4.0,<4.0.0'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.8,<4.0',
 )
```

