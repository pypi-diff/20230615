# Comparing `tmp/nci_cidc_cli-0.10.4.tar.gz` & `tmp/nci_cidc_cli-0.10.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-90vh0odb/nci_cidc_cli-0.10.4.tar", last modified: Fri May 26 17:28:55 2023, max compression
+gzip compressed data, was "/home/runner/work/cidc-cli/cidc-cli/dist/.tmp-71i106wl/nci_cidc_cli-0.10.5.tar", last modified: Thu Jun 15 15:27:02 2023, max compression
```

## Comparing `nci_cidc_cli-0.10.4.tar` & `nci_cidc_cli-0.10.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/consent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/nci_cidc_cli/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:55.000000 nci_cidc_cli-0.10.4/tests/dbedit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/dbedit/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-26 17:28:43.000000 nci_cidc_cli-0.10.4/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/consent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13941 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17247 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/nci_cidc_cli/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/nci_cidc_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/nci_cidc_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/nci_cidc_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/nci_cidc_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/nci_cidc_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/nci_cidc_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/nci_cidc_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 15:27:02.000000 nci_cidc_cli-0.10.5/tests/dbedit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/dbedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/dbedit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/dbedit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/dbedit/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57256 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/dbedit/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-15 15:26:54.000000 nci_cidc_cli-0.10.5/tests/util.py
```

### Comparing `nci_cidc_cli-0.10.4/LICENSE` & `nci_cidc_cli-0.10.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/PKG-INFO` & `nci_cidc_cli-0.10.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_cli
-Version: 0.10.4
+Version: 0.10.5
 Summary: A command-line interface for interacting with the NCI CIDC.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NCI-CIDC-CLI
```

### Comparing `nci_cidc_cli-0.10.4/README.md` & `nci_cidc_cli-0.10.5/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/api.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/auth.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/cache.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/cache.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/cli.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/config.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,14 @@
 
 
 # Environment-specific config
 _current_env = get_env()
 if _current_env == "prod":
     API_V2_URL = "PROD_PLACEHOLDER"
 elif _current_env == "staging":
-    API_V2_URL = "STAGE_PLACEHOLDER"
+    API_V2_URL = "https://nih-nci-cimac-cidc-dpline-stg.uk.r.appspot.com"
 elif _current_env == "dev-int":
     API_V2_URL = "https://nih-nci-cimac-cidc-dpline-dev.uk.r.appspot.com"
 elif _current_env == "dev":
     API_V2_URL = "http://localhost:8000"
 else:
     raise ValueError(f"Unsupported environment: {_current_env}")
```

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/consent.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/consent.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/cli.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/core.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,27 @@
     if not username:
         username = input("Username: ")
         set_username(username)
 
     password = getpass.getpass()
     connections = {
         "prod": "PROD_PLACEHOLDER",
-        "staging": "STAGE_PLACEHOLDER",
+        "staging": "nih-nci-cimac-cidc-dpline-stg:us-east4:cidc-postgresql-cidc-stage2",
         "dev-int": "nih-nci-cimac-cidc-dpline-dev:us-east4:cidc-postgresql-cidc-dev2",
     }
     connection_name = connections[ENV]
 
     # initialize Connector object
     connector = Connector()
 
     # function to return the database connection
     def getconn():
         databases = {
             "prod": "cidc-prod",
-            "staging": "cidc-staging",
+            "staging": "cidc-cidc-stage2",
             "dev-int": "cidc-cidc-dev2",
         }
         conn = connector.connect(
             connection_name,
             "pg8000",
             user=username,
             password=password,
```

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/list.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/list.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/dbedit/remove.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/dbedit/remove.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/gcloud.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/gcloud.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli/upload.py` & `nci_cidc_cli-0.10.5/nci_cidc_cli/upload.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/PKG-INFO` & `nci_cidc_cli-0.10.5/nci_cidc_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci-cidc-cli
-Version: 0.10.4
+Version: 0.10.5
 Summary: A command-line interface for interacting with the NCI CIDC.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## NCI-CIDC-CLI
```

### Comparing `nci_cidc_cli-0.10.4/nci_cidc_cli.egg-info/SOURCES.txt` & `nci_cidc_cli-0.10.5/nci_cidc_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/setup.py` & `nci_cidc_cli-0.10.5/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/dbedit/constants.py` & `nci_cidc_cli-0.10.5/tests/dbedit/constants.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/dbedit/test_core.py` & `nci_cidc_cli-0.10.5/tests/dbedit/test_core.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/dbedit/test_list.py` & `nci_cidc_cli-0.10.5/tests/dbedit/test_list.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/dbedit/test_remove.py` & `nci_cidc_cli-0.10.5/tests/dbedit/test_remove.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/test_api.py` & `nci_cidc_cli-0.10.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/test_auth.py` & `nci_cidc_cli-0.10.5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/test_cache.py` & `nci_cidc_cli-0.10.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/test_cli.py` & `nci_cidc_cli-0.10.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/test_upload.py` & `nci_cidc_cli-0.10.5/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_cli-0.10.4/tests/util.py` & `nci_cidc_cli-0.10.5/tests/util.py`

 * *Files identical despite different names*

