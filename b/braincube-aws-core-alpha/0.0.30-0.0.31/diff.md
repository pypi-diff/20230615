# Comparing `tmp/braincube-aws-core-alpha-0.0.30.tar.gz` & `tmp/braincube-aws-core-alpha-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-alpha-0.0.30.tar", last modified: Fri Jun  2 06:36:15 2023, max compression
+gzip compressed data, was "braincube-aws-core-alpha-0.0.31.tar", last modified: Thu Jun 15 08:06:48 2023, max compression
```

## Comparing `braincube-aws-core-alpha-0.0.30.tar` & `braincube-aws-core-alpha-0.0.31.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.654819 braincube-aws-core-alpha-0.0.30/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8820 2023-06-02 06:36:15.655113 braincube-aws-core-alpha-0.0.30/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8067 2023-06-01 08:04:11.000000 braincube-aws-core-alpha-0.0.30/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      953 2023-06-02 06:36:15.656479 braincube-aws-core-alpha-0.0.30/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.631394 braincube-aws-core-alpha-0.0.30/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.638180 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8820 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      871 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-02 06:36:15.000000 braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.638689 braincube-aws-core-alpha-0.0.30/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.641773 braincube-aws-core-alpha-0.0.30/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-05-15 18:52:22.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4110 2023-05-23 08:56:40.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-alpha-0.0.30/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.644462 braincube-aws-core-alpha-0.0.30/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.30/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.30/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.647762 braincube-aws-core-alpha-0.0.30/src/core/rest/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/rest/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.30/src/core/rest/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.30/src/core/rest/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.30/src/core/rest/data.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.651546 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/exceptions.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-alpha-0.0.30/src/core/rules_engine/rule_manager.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-02 06:36:15.654096 braincube-aws-core-alpha-0.0.30/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.30/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-alpha-0.0.30/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.30/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-15 08:06:48.384795 braincube-aws-core-alpha-0.0.31/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.31/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8856 2023-06-15 08:06:48.385046 braincube-aws-core-alpha-0.0.31/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8103 2023-06-15 05:48:44.000000 braincube-aws-core-alpha-0.0.31/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.31/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      953 2023-06-15 08:06:48.386766 braincube-aws-core-alpha-0.0.31/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.31/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-15 08:06:48.364537 braincube-aws-core-alpha-0.0.31/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-15 08:06:48.369466 braincube-aws-core-alpha-0.0.31/src/braincube_aws_core_alpha.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8856 2023-06-15 08:06:48.000000 braincube-aws-core-alpha-0.0.31/src/braincube_aws_core_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      871 2023-06-15 08:06:48.000000 braincube-aws-core-alpha-0.0.31/src/braincube_aws_core_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-15 08:06:48.000000 braincube-aws-core-alpha-0.0.31/src/braincube_aws_core_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-15 08:06:48.000000 braincube-aws-core-alpha-0.0.31/src/braincube_aws_core_alpha.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-15 08:06:48.000000 braincube-aws-core-alpha-0.0.31/src/braincube_aws_core_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-15 08:06:48.369984 braincube-aws-core-alpha-0.0.31/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.31/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-15 08:06:48.373201 braincube-aws-core-alpha-0.0.31/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.31/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-alpha-0.0.31/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-alpha-0.0.31/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-alpha-0.0.31/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-alpha-0.0.31/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-15 08:06:48.375900 braincube-aws-core-alpha-0.0.31/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.31/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-alpha-0.0.31/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-alpha-0.0.31/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-15 08:06:48.378768 braincube-aws-core-alpha-0.0.31/src/core/rest/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.31/src/core/rest/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-alpha-0.0.31/src/core/rest/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3722 2023-05-11 10:52:31.000000 braincube-aws-core-alpha-0.0.31/src/core/rest/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     3598 2023-05-11 17:50:46.000000 braincube-aws-core-alpha-0.0.31/src/core/rest/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-15 08:06:48.381531 braincube-aws-core-alpha-0.0.31/src/core/rules_engine/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.31/src/core/rules_engine/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-alpha-0.0.31/src/core/rules_engine/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-alpha-0.0.31/src/core/rules_engine/exceptions.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-alpha-0.0.31/src/core/rules_engine/rule_manager.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-15 08:06:48.383548 braincube-aws-core-alpha-0.0.31/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-alpha-0.0.31/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-alpha-0.0.31/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-alpha-0.0.31/src/core/utils/data.py
```

### Comparing `braincube-aws-core-alpha-0.0.30/LICENSE` & `braincube-aws-core-alpha-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/PKG-INFO` & `braincube-aws-core-alpha-0.0.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.30
+Version: 0.0.31
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -272,15 +272,15 @@
 sam-api$ sam local invoke ApiFunction --event events/event.json
 ```
 
 ### Deploy to AWS
 
 ```bash
 sam build --use-container
-sam deploy --guided --profile analog_user --region eu-west-1
+sam deploy --capabilities CAPABILITY_NAMED_IAM --guided --profile analog_user --region eu-west-1
 ```
 
 ### Build and deploy new package version using twine
 
 ```bash
 python3 -m pip install --upgrade pip
 python3 -m pip install --upgrade build
```

### Comparing `braincube-aws-core-alpha-0.0.30/README.md` & `braincube-aws-core-alpha-0.0.31/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 sam-api$ sam local invoke ApiFunction --event events/event.json
 ```
 
 ### Deploy to AWS
 
 ```bash
 sam build --use-container
-sam deploy --guided --profile analog_user --region eu-west-1
+sam deploy --capabilities CAPABILITY_NAMED_IAM --guided --profile analog_user --region eu-west-1
 ```
 
 ### Build and deploy new package version using twine
 
 ```bash
 python3 -m pip install --upgrade pip
 python3 -m pip install --upgrade build
```

### Comparing `braincube-aws-core-alpha-0.0.30/setup.cfg` & `braincube-aws-core-alpha-0.0.31/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core-alpha
-version = 0.0.30
+version = 0.0.31
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/PKG-INFO` & `braincube-aws-core-alpha-0.0.31/src/braincube_aws_core_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core-alpha
-Version: 0.0.30
+Version: 0.0.31
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -272,15 +272,15 @@
 sam-api$ sam local invoke ApiFunction --event events/event.json
 ```
 
 ### Deploy to AWS
 
 ```bash
 sam build --use-container
-sam deploy --guided --profile analog_user --region eu-west-1
+sam deploy --capabilities CAPABILITY_NAMED_IAM --guided --profile analog_user --region eu-west-1
 ```
 
 ### Build and deploy new package version using twine
 
 ```bash
 python3 -m pip install --upgrade pip
 python3 -m pip install --upgrade build
```

### Comparing `braincube-aws-core-alpha-0.0.30/src/braincube_aws_core_alpha.egg-info/SOURCES.txt` & `braincube-aws-core-alpha-0.0.31/src/braincube_aws_core_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/dal/data.py` & `braincube-aws-core-alpha-0.0.31/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/dal/postgres_repository.py` & `braincube-aws-core-alpha-0.0.31/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/di/data.py` & `braincube-aws-core-alpha-0.0.31/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/di/injector.py` & `braincube-aws-core-alpha-0.0.31/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/rest/app_controller.py` & `braincube-aws-core-alpha-0.0.31/src/core/rest/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/rest/app_module.py` & `braincube-aws-core-alpha-0.0.31/src/core/rest/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/rest/data.py` & `braincube-aws-core-alpha-0.0.31/src/core/rest/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/rules_engine/data.py` & `braincube-aws-core-alpha-0.0.31/src/core/rules_engine/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/rules_engine/rule_manager.py` & `braincube-aws-core-alpha-0.0.31/src/core/rules_engine/rule_manager.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/utils/convert.py` & `braincube-aws-core-alpha-0.0.31/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-alpha-0.0.30/src/core/utils/data.py` & `braincube-aws-core-alpha-0.0.31/src/core/utils/data.py`

 * *Files identical despite different names*

