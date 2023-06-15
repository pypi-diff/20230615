# Comparing `tmp/automation-common-test-2.0.2.tar.gz` & `tmp/automation-common-test-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation-common-test-2.0.2.tar", last modified: Wed Jun 14 14:46:45 2023, max compression
+gzip compressed data, was "automation-common-test-2.0.3.tar", last modified: Thu Jun 15 12:04:08 2023, max compression
```

## Comparing `automation-common-test-2.0.2.tar` & `automation-common-test-2.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-14 14:46:45.816468 automation-common-test-2.0.2/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-06-14 14:46:45.816263 automation-common-test-2.0.2/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-2.0.2/README.md
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-14 14:46:45.811779 automation-common-test-2.0.2/automation_common_test.egg-info/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-06-14 14:46:45.000000 automation-common-test-2.0.2/automation_common_test.egg-info/PKG-INFO
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      487 2023-06-14 14:46:45.000000 automation-common-test-2.0.2/automation_common_test.egg-info/SOURCES.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-06-14 14:46:45.000000 automation-common-test-2.0.2/automation_common_test.egg-info/dependency_links.txt
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-06-14 14:46:45.000000 automation-common-test-2.0.2/automation_common_test.egg-info/top_level.txt
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-14 14:46:45.813944 automation-common-test-2.0.2/helpers/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-2.0.2/helpers/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     2715 2023-06-08 05:41:40.000000 automation-common-test-2.0.2/helpers/api_operations.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-2.0.2/helpers/base_locator.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1876 2023-06-08 03:42:00.000000 automation-common-test-2.0.2/helpers/decorator.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     5164 2023-05-31 08:38:28.000000 automation-common-test-2.0.2/helpers/driver_manager.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-2.0.2/helpers/soft_check.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)    65913 2023-05-17 05:05:21.000000 automation-common-test-2.0.2/helpers/web_operations.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-06-14 14:46:45.816523 automation-common-test-2.0.2/setup.cfg
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-06-14 14:46:43.000000 automation-common-test-2.0.2/setup.py
-drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-14 14:46:45.815865 automation-common-test-2.0.2/utils/
--rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-2.0.2/utils/__init__.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-2.0.2/utils/config_parser.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-2.0.2/utils/encryption_decryption.py
--rw-r--r--   0 chitranjankumar   (501) staff       (20)     4112 2023-05-17 05:11:54.000000 automation-common-test-2.0.2/utils/json_utils.py
--rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4660 2023-05-09 03:29:52.000000 automation-common-test-2.0.2/utils/post_results_teams.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-15 12:04:08.663905 automation-common-test-2.0.3/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-06-15 12:04:08.663719 automation-common-test-2.0.3/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1847 2023-03-29 14:50:23.000000 automation-common-test-2.0.3/README.md
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-15 12:04:08.660076 automation-common-test-2.0.3/automation_common_test.egg-info/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      200 2023-06-15 12:04:08.000000 automation-common-test-2.0.3/automation_common_test.egg-info/PKG-INFO
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      487 2023-06-15 12:04:08.000000 automation-common-test-2.0.3/automation_common_test.egg-info/SOURCES.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        1 2023-06-15 12:04:08.000000 automation-common-test-2.0.3/automation_common_test.egg-info/dependency_links.txt
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       14 2023-06-15 12:04:08.000000 automation-common-test-2.0.3/automation_common_test.egg-info/top_level.txt
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-15 12:04:08.662135 automation-common-test-2.0.3/helpers/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:00.000000 automation-common-test-2.0.3/helpers/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     2715 2023-06-08 05:41:40.000000 automation-common-test-2.0.3/helpers/api_operations.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      209 2022-09-02 04:55:52.000000 automation-common-test-2.0.3/helpers/base_locator.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1876 2023-06-08 03:42:00.000000 automation-common-test-2.0.3/helpers/decorator.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     5164 2023-05-31 08:38:28.000000 automation-common-test-2.0.3/helpers/driver_manager.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     6797 2023-04-14 07:36:34.000000 automation-common-test-2.0.3/helpers/soft_check.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)    65913 2023-05-17 05:05:21.000000 automation-common-test-2.0.3/helpers/web_operations.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)       38 2023-06-15 12:04:08.663955 automation-common-test-2.0.3/setup.cfg
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      366 2023-06-15 12:03:57.000000 automation-common-test-2.0.3/setup.py
+drwxr-xr-x   0 chitranjankumar   (501) staff       (20)        0 2023-06-15 12:04:08.663259 automation-common-test-2.0.3/utils/
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)        0 2023-04-12 09:43:11.000000 automation-common-test-2.0.3/utils/__init__.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)      376 2023-04-14 09:22:06.000000 automation-common-test-2.0.3/utils/config_parser.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     1568 2023-04-14 09:34:24.000000 automation-common-test-2.0.3/utils/encryption_decryption.py
+-rw-r--r--   0 chitranjankumar   (501) staff       (20)     3993 2023-06-15 12:03:37.000000 automation-common-test-2.0.3/utils/json_utils.py
+-rwxr-xr-x   0 chitranjankumar   (501) staff       (20)     4660 2023-05-09 03:29:52.000000 automation-common-test-2.0.3/utils/post_results_teams.py
```

### Comparing `automation-common-test-2.0.2/README.md` & `automation-common-test-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.2/helpers/api_operations.py` & `automation-common-test-2.0.3/helpers/api_operations.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.2/helpers/decorator.py` & `automation-common-test-2.0.3/helpers/decorator.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.2/helpers/driver_manager.py` & `automation-common-test-2.0.3/helpers/driver_manager.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.2/helpers/soft_check.py` & `automation-common-test-2.0.3/helpers/soft_check.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.2/helpers/web_operations.py` & `automation-common-test-2.0.3/helpers/web_operations.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.2/utils/encryption_decryption.py` & `automation-common-test-2.0.3/utils/encryption_decryption.py`

 * *Files identical despite different names*

### Comparing `automation-common-test-2.0.2/utils/json_utils.py` & `automation-common-test-2.0.3/utils/json_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,20 @@
 
 # set the path of test data and update the dictionary
 def set_data_path(file_path):
     global data_path
     data_path = file_path
     global dic_data
     dic_data = get_json_object(data_path)
-    logging.info(f"Dic DFata{dic_data}")
     if type(modify_data) == dict and len(modify_data.items()):
         modify_main_dict_value_param()
 def modify_parameter(param):
     global modify_data
     modify_data = param
 
-        
-# def get_json_object(file_path):
-#     return open(file_path, 'rb')
 def get_json_object(file_path):
     with open(file_path, 'r') as f:
         distros_dict = json.load(f)
     return distros_dict
 
 def get_json_dict(file_path):
     logging.info(file_path)
```

### Comparing `automation-common-test-2.0.2/utils/post_results_teams.py` & `automation-common-test-2.0.3/utils/post_results_teams.py`

 * *Files identical despite different names*

