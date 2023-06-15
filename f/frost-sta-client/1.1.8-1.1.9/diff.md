# Comparing `tmp/frost_sta_client-1.1.8.tar.gz` & `tmp/frost_sta_client-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frost_sta_client-1.1.8.tar", last modified: Fri Feb  4 08:37:14 2022, max compression
+gzip compressed data, was "frost_sta_client-1.1.9.tar", last modified: Thu Feb 17 11:34:03 2022, max compression
```

## Comparing `frost_sta_client-1.1.8.tar` & `frost_sta_client-1.1.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 08:37:14.902357 frost_sta_client-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     7814 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-02-04 08:37:14.902357 frost_sta_client-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 08:37:14.898357 frost_sta_client-1.1.8/frost_sta_client/
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      362 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 08:37:14.898357 frost_sta_client-1.1.8/frost_sta_client/dao/
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/actuator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6937 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/datastream.py
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/features_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/historical_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/location.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/multi_datastream.py
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/observedproperty.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/sensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/tasking_capability.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/dao/thing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 08:37:14.902357 frost_sta_client-1.1.8/frost_sta_client/model/
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6887 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/actuator.py
--rw-r--r--   0 runner    (1001) docker     (121)    12307 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/datastream.py
--rw-r--r--   0 runner    (1001) docker     (121)     3655 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/entity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 08:37:14.902357 frost_sta_client-1.1.8/frost_sta_client/model/ext/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4907 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/ext/entity_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/ext/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2137 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/ext/unitofmeasurement.py
--rw-r--r--   0 runner    (1001) docker     (121)     6945 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/feature_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/historical_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     8214 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/location.py
--rw-r--r--   0 runner    (1001) docker     (121)    14377 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/multi_datastream.py
--rw-r--r--   0 runner    (1001) docker     (121)     8888 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/observation.py
--rw-r--r--   0 runner    (1001) docker     (121)     7968 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/observedproperty.py
--rw-r--r--   0 runner    (1001) docker     (121)     8265 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/sensor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     7629 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/tasking_capability.py
--rw-r--r--   0 runner    (1001) docker     (121)    12136 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/model/thing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 08:37:14.902357 frost_sta_client-1.1.8/frost_sta_client/query/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/query/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 08:37:14.902357 frost_sta_client-1.1.8/frost_sta_client/service/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/service/auth_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/service/sensorthingsservice.py
--rw-r--r--   0 runner    (1001) docker     (121)     4321 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/frost_sta_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 08:37:14.898357 frost_sta_client-1.1.8/frost_sta_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-02-04 08:37:14.000000 frost_sta_client-1.1.8/frost_sta_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-02-04 08:37:14.000000 frost_sta_client-1.1.8/frost_sta_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 08:37:14.000000 frost_sta_client-1.1.8/frost_sta_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-04 08:37:14.000000 frost_sta_client-1.1.8/frost_sta_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-04 08:37:14.000000 frost_sta_client-1.1.8/frost_sta_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-02-04 08:37:14.902357 frost_sta_client-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-04 08:36:54.000000 frost_sta_client-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:34:03.205968 frost_sta_client-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     7814 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-02-17 11:34:03.205968 frost_sta_client-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2350 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:34:03.197968 frost_sta_client-1.1.9/frost_sta_client/
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      362 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:34:03.201969 frost_sta_client-1.1.9/frost_sta_client/dao/
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6949 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/features_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/historical_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/multi_datastream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/observation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/observedproperty.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/tasking_capability.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/dao/thing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:34:03.205968 frost_sta_client-1.1.9/frost_sta_client/model/
+-rw-r--r--   0 runner    (1001) docker     (121)      627 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6935 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12375 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/datastream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/entity.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:34:03.205968 frost_sta_client-1.1.9/frost_sta_client/model/ext/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4927 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/ext/entity_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/ext/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/ext/unitofmeasurement.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6989 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/feature_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4892 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/historical_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8262 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/location.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14493 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/multi_datastream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8916 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/observation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8024 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/observedproperty.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8313 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4435 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7689 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/tasking_capability.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12240 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/model/thing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:34:03.205968 frost_sta_client-1.1.9/frost_sta_client/query/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/query/query.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:34:03.205968 frost_sta_client-1.1.9/frost_sta_client/service/
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/service/auth_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3164 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/service/sensorthingsservice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4345 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/frost_sta_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 11:34:03.197968 frost_sta_client-1.1.9/frost_sta_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2710 2022-02-17 11:34:02.000000 frost_sta_client-1.1.9/frost_sta_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-02-17 11:34:03.000000 frost_sta_client-1.1.9/frost_sta_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 11:34:02.000000 frost_sta_client-1.1.9/frost_sta_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-02-17 11:34:03.000000 frost_sta_client-1.1.9/frost_sta_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-17 11:34:03.000000 frost_sta_client-1.1.9/frost_sta_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-02-17 11:34:03.205968 frost_sta_client-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-17 11:33:49.000000 frost_sta_client-1.1.9/setup.py
```

### Comparing `frost_sta_client-1.1.8/LICENSE` & `frost_sta_client-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/PKG-INFO` & `frost_sta_client-1.1.9/frost_sta_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: frost_sta_client
-Version: 1.1.8
+Name: frost-sta-client
+Version: 1.1.9
 Summary: a client library to facilitate interaction with a FROST SensorThingsAPI Server
 Home-page: https://github.com/FraunhoferIOSB/FROST-Python-Client
 Author: Katharina Emde
 Author-email: katharina.emde@iosb.fraunhofer.de
 License: LGPL3
 Keywords: sta,ogc,frost,sensorthingsapi,IoT
 Platform: UNKNOWN
```

### Comparing `frost_sta_client-1.1.8/README.md` & `frost_sta_client-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/__init__.py` & `frost_sta_client-1.1.9/frost_sta_client/__init__.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/actuator.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/actuator.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/base.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,37 +55,37 @@
 
     @property
     def entitytype(self):
         return self._entitytype
 
     @entitytype.setter
     def entitytype(self, value):
-        if value is None or type(value) == str:
+        if value is None or isinstance(value, str):
             self._entitytype = value
             return
         raise ValueError('entitytype should be of type String')
 
     @property
     def entitytype_plural(self):
         return self._entitytype_plural
 
     @entitytype_plural.setter
     def entitytype_plural(self, value):
-        if value is None or type(value) == str:
+        if value is None or isinstance(value, str):
             self._entitytype_plural = value
             return
         raise ValueError('entitytype_plural should be of type String')
 
     @property
     def entity_class(self):
         return self._entity_class
 
     @entity_class.setter
     def entity_class(self, value):
-        if value is None or type(value) == str:
+        if value is None or isinstance(value, str):
             self._entity_class = value
             return
         raise ValueError('entity_class should be of type string')
 
     def create(self, entity):
         url = furl(self.service.url)
         url.path.add(self.entitytype_plural)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/datastream.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/datastream.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/features_of_interest.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/features_of_interest.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/historical_location.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/historical_location.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/location.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/location.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/multi_datastream.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/multi_datastream.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/observation.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/observation.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/observedproperty.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/observedproperty.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/sensor.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/sensor.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/task.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/task.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/tasking_capability.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/tasking_capability.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/dao/thing.py` & `frost_sta_client-1.1.9/frost_sta_client/dao/thing.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/__init__.py` & `frost_sta_client-1.1.9/frost_sta_client/model/__init__.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/actuator.py` & `frost_sta_client-1.1.9/frost_sta_client/model/actuator.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,35 +55,35 @@
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._description = value
 
     @property
     def encoding_type(self):
         return self._encoding_type
 
     @encoding_type.setter
     def encoding_type(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('encodingtype should be of type str!')
         self._encoding_type = value
 
     @property
     def metadata(self):
         return self._metadata
 
@@ -99,32 +99,32 @@
 
     @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, value):
-        if type(value) != dict:
+        if not isinstance(value, dict):
             raise ValueError('properties should be of type dict!')
         self._properties = value
 
     @property
     def tasking_capabilities(self):
         return self._tasking_capabilities
 
     @tasking_capabilities.setter
     def tasking_capabilities(self, values):
         if values is None:
             self._tasking_capabilities = None
             return
-        if type(values) == list and all(isinstance(tc, tasking_capability.TaskingCapability) for tc in values):
+        if isinstance(values, list) and all(isinstance(tc, tasking_capability.TaskingCapability) for tc in values):
             entity_class = entity_type.EntityTypes['TaskingCapability']['class']
             self._tasking_capabilities = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or \
+        if not isinstance(values, entity_list.EntityList) or \
                 any((not isinstance(tc, tasking_capability.TaskingCapability)) for tc in values.entities):
             raise ValueError('Tasking capabilities should be a list of TaskingCapabilities')
         self._tasking_capabilities = values
 
     def ensure_service_on_children(self, service):
         if self.tasking_capabilities is not None:
             self.tasking_capabilities.set_service(service)
@@ -170,14 +170,14 @@
     def __setstate__(self, state):
         super().__setstate__(state)
         self.name = state.get("name", None)
         self.description = state.get("description", None)
         self.encoding_type = state.get("encodingType", "")
         self.metadata = state.get("metadata", "")
         self.properties = state.get("properties", None)
-        if state.get("TaskingCapabilities", None) is not None and type(state["TaskingCapabilities"] == list):
+        if state.get("TaskingCapabilities", None) is not None and isinstance(state["TaskingCapabilities"], list):
             entity_class = entity_type.EntityTypes['TaskingCapability']['class']
             self.tasking_capabilities = utils.transform_json_to_entity_list(state['TaskingCapabilities'], entity_class)
             self.tasking_capabilities.next_link = state.get("TaskingCapabilities@iot.nextLink", None)
 
     def get_dao(self, service):
         return ActuatorDao(service)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/datastream.py` & `frost_sta_client-1.1.9/frost_sta_client/model/datastream.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,81 +91,81 @@
         return self._name
 
     @name.setter
     def name(self, value):
         if value is None:
             self._name = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, value):
         if value is None:
             self._description = None
             return
-        if type(value) != str:
+        if isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._description = value
 
     @property
     def observation_type(self):
         return self._observation_type
 
     @observation_type.setter
     def observation_type(self, value):
         if value is None:
             self._observation_type = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('observation_type should be of type str!')
         self._observation_type = value
 
     @property
     def unit_of_measurement(self):
         return self._unit_of_measurement
 
     @unit_of_measurement.setter
     def unit_of_measurement(self, value):
-        if value is None or type(value) == unitofmeasurement.UnitOfMeasurement:
+        if value is None or isinstance(value, unitofmeasurement.UnitOfMeasurement):
             self._unit_of_measurement = value
             return
         raise ValueError('unitOfMeasurement should be of type UnitOfMeasurement!')
 
     @property
     def observed_area(self):
         return self._observed_area
 
     @observed_area.setter
     def observed_area(self, value):
         if value is None:
             self._observed_area = None
             return
-        if type(value) == geojson.geometry.Polygon or \
-           type(value) == geojson.geometry.Point or \
-           type(value) == geojson.geometry.Geometry:
+        if isinstance(value, geojson.geometry.Polygon) or \
+           isinstance(value, geojson.geometry.Point) or \
+           isinstance(value, geojson.geometry.Geometry):
             self._observed_area = geojson.dumps(value)
             return
         raise ValueError('observedArea should be a geojson object')
 
     @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, value):
         if value is None:
             self._properties = None
             return
-        if type(value) != dict:
+        if not isinstance(value, dict):
             raise ValueError('properties should be of type dict')
         self._properties = value
 
     @property
     def phenomenon_time(self):
         return self._phenomenon_time
 
@@ -183,55 +183,55 @@
 
     @property
     def thing(self):
         return self._thing
 
     @thing.setter
     def thing(self, value):
-        if value is None or type(value) == thing.Thing:
+        if value is None or isinstance(value, thing.Thing):
             self._thing = value
             return
         raise ValueError('thing should be of type Thing!')
 
     @property
     def sensor(self):
         return self._sensor
 
     @sensor.setter
     def sensor(self, value):
-        if value is None or type(value) == sensor.Sensor:
+        if value is None or isinstance(value, sensor.Sensor):
             self._sensor = value
             return
         raise ValueError('sensor should be of type Sensor!')
 
     @property
     def observed_property(self):
         return self._observed_property
 
     @observed_property.setter
     def observed_property(self, value):
-        if type(value) == observedproperty.ObservedProperty or value is None:
+        if isinstance(value, observedproperty.ObservedProperty) or value is None:
             self._observed_property = value
             return
         raise ValueError('observed property should by of type ObservedProperty!')
 
     @property
     def observations(self):
         return self._observations
 
     @observations.setter
     def observations(self, values):
         if values is None:
             self._observations = None
             return
-        if type(values) == list and all(isinstance(ob, observation.Observation) for ob in values):
+        if isinstance(values, list) and all(isinstance(ob, observation.Observation) for ob in values):
             entity_class = entity_type.EntityTypes['Observation']['class']
             self._observations = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) == entity_list.EntityList and \
+        if isinstance(values, entity_list.EntityList) and \
                 all(isinstance(ob, observation.Observation) for ob in values.entities):
             self._observations = values
             return
         raise ValueError('Observations should be a list of Observations')
 
     def ensure_service_on_children(self, service):
         if self.thing is not None:
@@ -312,14 +312,14 @@
             self.result_time = state["resultTime"]
         if state.get("Thing", None) is not None:
             self.thing = frost_sta_client.model.thing.Thing()
             self.thing.__setstate__(state["Thing"])
         if state.get("ObservedProperty", None) is not None:
             self.observed_property = frost_sta_client.model.observedproperty.ObservedProperty()
             self.observed_property.__setstate__(state["ObservedProperty"])
-        if state.get("Observations", None) is not None and type(state["Observations"] == list):
+        if state.get("Observations", None) is not None and isinstance(state["Observations"], list):
             entity_class = entity_type.EntityTypes['Observation']['class']
             self.observations = utils.transform_json_to_entity_list(state['Observations'], entity_class)
             self.observations.next_link = state.get("Observations@iot.nextLink", None)
 
     def get_dao(self, service):
         return DatastreamDao(service)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/entity.py` & `frost_sta_client-1.1.9/frost_sta_client/model/entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         return self._id
 
     @id.setter
     def id(self, value):
         if value is None:
             self._id = None
             return
-        if type(value) == int or type(value) == str:
+        if isinstance(value, int) or isinstance(value, str):
             self._id = value
             return
         raise ValueError('id of entity should be of type int!')
 
     @property
     def self_link(self):
         return self._self_link
 
     @self_link.setter
     def self_link(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('self_link should be of type str!')
         self._self_link = value
 
     @property
     def service(self):
         return self._service
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/ext/entity_list.py` & `frost_sta_client-1.1.9/frost_sta_client/model/ext/entity_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,51 +63,51 @@
             self.next_link = json_response.get("@iot.nextLink", None)
             self.iterable_entities = iter(self.entities[-len(result_list.entities):])
             return next(self)
         else:
             raise StopIteration
 
     def get(self, index):
-        if type(index) != int:
+        if not isinstance(index, int):
             raise IndexError('index must be an integer')
         if index >= len(self.entities):
             raise IndexError('index exceeds total number of entities')
         if index < 0:
             raise IndexError('negative indices cannot be accessed')
         return self.entities[index]
 
     @property
     def entity_class(self):
         return self._entity_class
 
     @entity_class.setter
     def entity_class(self, value):
-        if type(value) == str:
+        if isinstance(value, str):
             self._entity_class = value
             return
         raise ValueError('entity_class should be of type str')
 
     @property
     def entities(self):
         return self._entities
 
     @entities.setter
     def entities(self, values):
-        if type(values) == list and all(isinstance(v, frost_sta_client.model.entity.Entity) for v in values):
+        if isinstance(values, list) and all(isinstance(v, frost_sta_client.model.entity.Entity) for v in values):
             self._entities = values
             return
         raise ValueError('entities should be a list of entities')
 
     @property
     def next_link(self):
         return self._next_link
 
     @next_link.setter
     def next_link(self, value):
-        if value is None or type(value) == str:
+        if value is None or isinstance(value, str):
             self._next_link = value
             return
         raise ValueError('next_link should be of type string')
 
     @property
     def service(self):
         return self._service
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/ext/entity_type.py` & `frost_sta_client-1.1.9/frost_sta_client/model/ext/entity_type.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/ext/unitofmeasurement.py` & `frost_sta_client-1.1.9/frost_sta_client/model/ext/unitofmeasurement.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,35 +25,35 @@
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def symbol(self):
         return self._symbol
 
     @symbol.setter
     def symbol(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('symbol should be of type str!')
         self._symbol = value
 
     @property
     def definition(self):
         return self._definition
 
     @definition.setter
     def definition(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('definition should be of type str!')
         self._definition = value
 
     def __getstate__(self):
         data = {
             'symbol': self._symbol,
             'definition': self._definition,
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/feature_of_interest.py` & `frost_sta_client-1.1.9/frost_sta_client/model/feature_of_interest.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,72 +55,72 @@
         return self._name
 
     @name.setter
     def name(self, value):
         if value is None:
             self._name = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, value):
         if value is None:
             self._description = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._description = value
 
     @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, value):
         if value is None:
             self._properties = None
             return
-        if type(value) != dict:
+        if not isinstance(value, dict):
             raise ValueError('properties should be of type dict!')
         self._properties = value
 
     @property
     def encoding_type(self):
         return self._encoding_type
 
     @encoding_type.setter
     def encoding_type(self, value):
         if value is None:
             self._encoding_type = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('encodingType should be of type str!')
         self._encoding_type = value
 
     @property
     def observations(self):
         return self._observations
 
     @observations.setter
     def observations(self, values):
         if values is None:
             self._observations = None
             return
-        if type(values) == list and \
+        if isinstance(values, list) and \
                 all(isinstance(ob, frost_sta_client.model.observation.Observation) for ob in values):
             entity_class = entity_type.EntityTypes['Observation']['class']
             self._observations = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) == entity_list.EntityList and \
+        if isinstance(values, entity_list.EntityList) and \
                 all((isinstance(ob, frost_sta_client.model.observation.Observation)) for ob in values.entities):
             self._observations = values
             return
         raise ValueError('Observations should be a list of Observations')
 
     @property
     def feature(self):
@@ -181,15 +181,15 @@
 
     def __setstate__(self, state):
         super().__setstate__(state)
         self.name = state.get("name", None)
         self.description = state.get("description", None)
         self.properties = state.get("properties", None)
         self.encoding_type = state.get("encodingType", None)
-        if state.get("Observations", None) is not None and type(state["Observations"]) == list:
+        if state.get("Observations", None) is not None and isinstance(state["Observations"], list):
             self.observation = []
             for value in state["Observation"]:
                 obs = frost_sta_client.model.observation.Observation()
                 obs.__setstate__(value)
                 self.observation.append(obs)
 
     def get_dao(self, service):
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/historical_location.py` & `frost_sta_client-1.1.9/frost_sta_client/model/historical_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,31 +64,31 @@
         return self._locations
 
     @locations.setter
     def locations(self, values):
         if values is None:
             self._locations = None
             return
-        if type(values) == list and all(isinstance(loc, location.Location) for loc in values):
+        if isinstance(values, list) and all(isinstance(loc, location.Location) for loc in values):
             entity_class = entity_type.EntityTypes['Location']['class']
             self._locations = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) == entity_list.EntityList and\
+        if isinstance(values, entity_list.EntityList) and\
                 all((isinstance(loc, location.Location)) for loc in values.entities):
             self._locations = values
             return
         raise ValueError('locations should be a list of locations!')
 
     @property
     def thing(self):
         return self._thing
 
     @thing.setter
     def thing(self, value):
-        if value is None or type(value) == thing.Thing:
+        if value is None or isinstance(value, thing.Thing):
             self._thing = value
             return
         raise ValueError('thing should be of type Thing!')
 
     def ensure_service_on_children(self, service):
         if self.locations is not None:
             self.locations.set_service(service)
@@ -121,14 +121,14 @@
 
     def __setstate__(self, state):
         super().__setstate__(state)
         self.time = state.get("Time", None)
         if state.get("Thing", None) is not None:
             self.thing = frost_sta_client.model.thing.Thing()
             self.thing.__setstate__(state["Thing"])
-        if state.get("Locations", None) is not None and type(state["Locations"] == list):
+        if state.get("Locations", None) is not None and isinstance(state["Locations"], list):
             entity_class = entity_type.EntityTypes['Location']['class']
             self.locations = utils.transform_json_to_entity_list(state['Locations'], entity_class)
             self.locations.next_link = state.get('Locations@iot.nextLink', None)
 
     def get_dao(self, service):
         return HistoricalLocationDao(service)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/location.py` & `frost_sta_client-1.1.9/frost_sta_client/model/location.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,54 +66,54 @@
         return self._name
 
     @name.setter
     def name(self, value):
         if value is None:
             self._name = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, value):
         if value is None:
             self._description = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._description = value
 
     @property
     def encoding_type(self):
         return self._encoding_type
 
     @encoding_type.setter
     def encoding_type(self, value):
         if value is None:
             self._encoding_type = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('encodingType should be of type str!')
         self._encoding_type = value
 
     @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, values):
         if values is None:
             self._properties = None
             return
-        if type(values) != dict:
+        if not isinstance(values, dict):
             raise ValueError('properties should be of type dict!')
         self._properties = values
 
     @property
     def location(self):
         return self._location
 
@@ -139,32 +139,32 @@
         return self._thing
 
     @thing.setter
     def thing(self, value):
         if value is None:
             self._thing = None
             return
-        if type(value) != thing.Thing:
+        if not isinstance(value, thing.Thing):
             raise ValueError('thing should be of type Thing!')
         self._thing = value
 
     @property
     def historical_locations(self):
         return self._historical_locations
 
     @historical_locations.setter
     def historical_locations(self, values):
         if values is None:
             self._historical_locations = None
             return
-        if type(values) == list and all(isinstance(hl, historical_location.HistoricalLocation) for hl in values):
+        if isinstance(values, list) and all(isinstance(hl, historical_location.HistoricalLocation) for hl in values):
             entity_class = entity_type.EntityTypes['HistoricalLocation']['class']
             self._historical_locations = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) == entity_list.EntityList and \
+        if isinstance(values, entity_list.EntityList) and \
                 all(isinstance(hl, historical_location.HistoricalLocation) for hl in values.entities):
             self._historical_locations = values
         raise ValueError('historical_location should be of type HistoricalLocation!')
 
     def ensure_service_on_children(self, service):
         if self.thing is not None:
             self.thing.set_service(service)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/multi_datastream.py` & `frost_sta_client-1.1.9/frost_sta_client/model/multi_datastream.py`

 * *Files 13% similar despite different names*

```diff
@@ -81,92 +81,92 @@
         return self._name
 
     @name.setter
     def name(self, value):
         if value is None:
             self._name = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, value):
         if value is None:
             self._description = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._description = value
 
     @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, values):
         if values is None:
             self._properties = {}
             return
-        if type(values) != dict:
+        if not isinstance(values, dict):
             raise ValueError('properties should be of type dict!')
         self._properties = values
 
     @property
     def unit_of_measurements(self):
         return self._unit_of_measurements
 
     @unit_of_measurements.setter
     def unit_of_measurements(self, values):
         if values is None:
             self._unit_of_measurements = None
             return
-        if type(values) == list and all(isinstance(uom, unitofmeasurement.UnitOfMeasurement) for uom in values):
+        if isinstance(values, list) and all(isinstance(uom, unitofmeasurement.UnitOfMeasurement) for uom in values):
             entity_class = entity_type.EntityTypes['UnitOfMeasurement']['class']
             self._unit_of_measurements = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or \
+        if not isinstance(values, entity_list.EntityList) or \
                 any((not isinstance(uom, unitofmeasurement.UnitOfMeasurement)) for uom in values.entities):
             raise ValueError('unit_of_measurements should be an entity_list of type UnitOfMeasurement')
         self._unit_of_measurements = values
 
     @property
     def observation_type(self):
         return self._observation_type
 
     @observation_type.setter
     def observation_type(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('observation_type should be of type str!')
         self._observation_type = value
 
     @property
     def multi_observation_data_types(self):
         return self._multi_observation_data_types
 
     @multi_observation_data_types.setter
     def multi_observation_data_types(self, values):
-        if values is not None and (type(values) != list or any((not isinstance(dtype, str)) for dtype in values)):
+        if values is not None and (not isinstance(values, list) or any((not isinstance(dtype, str)) for dtype in values)):
             raise ValueError('multi_observations_data_types should be list of type str!')
         self._multi_observation_data_types = values
 
     @property
     def observed_area(self):
         return self._observed_area
 
     @observed_area.setter
     def observed_area(self, value):
         if value is None:
             self._observed_area = None
             return
-        if type(value) != geojson.geometry.Polygon:
+        if not isinstance(value, geojson.geometry.Polygon):
             raise ValueError('observedArea should be geojson object')
         self._observed_area = value
 
     @property
     def phenomenon_time(self):
         return self._phenomenon_time
 
@@ -184,60 +184,60 @@
 
     @property
     def thing(self):
         return self._thing
 
     @thing.setter
     def thing(self, value):
-        if value is not None and type(value) != thing.Thing:
+        if value is not None and not isinstance(value, thing.Thing):
             raise ValueError('thing should be of type Thing!')
         self._thing = value
 
     @property
     def sensor(self):
         return self._sensor
 
     @sensor.setter
     def sensor(self, value):
-        if value is not None and type(value) != sensor.Sensor:
+        if value is not None and not isinstance(value, sensor.Sensor):
             raise ValueError('sensor should be of type Sensor!')
         self._sensor = value
 
     @property
     def observed_properties(self):
         return self._observed_properties
 
     @observed_properties.setter
     def observed_properties(self, values):
         if values is None:
             self._observed_properties = None
             return
-        if type(values) == list and all(isinstance(op, observedproperty.ObservedProperty) for op in values):
+        if isinstance(values, list) and all(isinstance(op, observedproperty.ObservedProperty) for op in values):
             entity_class = entity_type.EntityTypes['ObservedProperty']['class']
             self._observed_properties = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or \
+        if not isinstance(values, entity_list.EntityList) or \
                 any(not isinstance(op, observedproperty.ObservedProperty) for op in values.entities):
             raise ValueError('observed_properties should be an entity list of ObservedProperty!')
         self._observed_properties = values
 
     @property
     def observations(self):
         return self._observations
 
     @observations.setter
     def observations(self, values):
         if values is None:
             self._observations = None
             return
-        if type(values) == list and all(isinstance(ob, observation.Observation) for ob in values):
+        if isinstance(values, list) and all(isinstance(ob, observation.Observation) for ob in values):
             entity_class = entity_type.EntityTypes['Observation']['class']
             self._observations = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or \
+        if not isinstance(values, entity_list.EntityList) or \
                 any(not isinstance(ob, observation.Observation) for ob in values.entities):
             raise ValueError('Observations should be an entity list of Observations')
         self._observations = values
 
     def ensure_service_on_children(self, service):
         if self.thing is not None:
             self.thing.set_service(service)
@@ -317,27 +317,27 @@
         self.properties = state.get('properties', None)
         if state.get('Thing', None) is not None:
             self.thing = frost_sta_client.model.thing.Thing()
             self.thing.__setstate__(state['Thing'])
         if state.get('Sensor', None) is not None:
             self.sensor = frost_sta_client.model.sensor.Sensor()
             self.sensor.__setstate__(state['Sensor'])
-        if state.get('unitOfMeasurements', None) is not None and type(state['unitOfMeasurements']) == list:
+        if state.get('unitOfMeasurements', None) is not None and isinstance(state['unitOfMeasurements'], list):
             entity_class = entity_type.EntityTypes['UnitOfMeasurement']['class']
             self.unit_of_measurements = utils.transform_json_to_entity_list(state['unitOfMeasurements'], entity_class)
             self.unit_of_measurements.next_link = state.get('unitOfMeasurements', None)
         if state.get('multiObservationDataTypes', None) is not None \
-                and type(state['multiObservationDataTypes']) == list:
+                and isinstance(state['multiObservationDataTypes'], list):
             self.multi_observation_data_types = []
             for value in state['multiObservationDataTypes']:
                 self.multi_observation_data_types.append(value)
-        if state.get('ObservedProperties', None) is not None and type(state['ObservedProperties']) == list:
+        if state.get('ObservedProperties', None) is not None and isinstance(state['ObservedProperties'], list):
             entity_class = entity_type.EntityTypes['ObservedProperty']['class']
             self.observed_properties = utils.transform_json_to_entity_list(state['ObservedProperty'], entity_class)
             self.observed_properties.next_link = state.get('ObservedProperties@iot.nextLink')
-        if state.get('Observations', None) is not None and type(state['Observations']) == list:
+        if state.get('Observations', None) is not None and isinstance(state['Observations'], list):
             entity_class = entity_type.EntityTypes['Observation']['class']
             self.observations = utils.transform_json_to_entity_list(state['Observations'], entity_class)
             self.observed_properties.next_link = state.get('Observations@iot.nextLink')
 
     def get_dao(self):
         return MultiDatastreamDao(self)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/observation.py` & `frost_sta_client-1.1.9/frost_sta_client/model/observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,54 +121,54 @@
         return self._parameters
 
     @parameters.setter
     def parameters(self, values):
         if values is None:
             self._parameters = None
             return
-        if type(values) != dict:
+        if not isinstance(values, dict):
             raise ValueError('parameters should be of type dict!')
         self._parameters = values
 
     @property
     def feature_of_interest(self):
         return self._feature_of_interest
 
     @feature_of_interest.setter
     def feature_of_interest(self, value):
         if value is None:
             self._feature_of_interest = None
             return
-        if type(value) != feature_of_interest.FeatureOfInterest:
+        if not isinstance(value, feature_of_interest.FeatureOfInterest):
             raise ValueError('feature_of_interest should be of type FeatureOfInterest!')
         self._feature_of_interest = value
 
     @property
     def datastream(self):
         return self._datastream
 
     @datastream.setter
     def datastream(self, value):
         if value is None:
             self._datastream = None
             return
-        if type(value) != datastream.Datastream:
+        if not isinstance(value, datastream.Datastream):
             raise ValueError('datastream should be of type Datastream!')
         self._datastream = value
 
     @property
     def multi_datastream(self):
         return self._multi_datastream
 
     @multi_datastream.setter
     def multi_datastream(self, value):
         if value is None:
             self._multi_datastream = None
             return
-        if type(value) == multi_datastream.MultiDatastream:
+        if isinstance(value, multi_datastream.MultiDatastream):
             self._multi_datastream = value
             return
         raise ValueError('multi_datastream should be of type MultiDatastream!')
 
     def ensure_service_on_children(self, service):
         if self.datastream is not None:
             self.datastream.set_service(service)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/observedproperty.py` & `frost_sta_client-1.1.9/frost_sta_client/model/observedproperty.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,89 +58,89 @@
         return self._name
 
     @name.setter
     def name(self, value):
         if value is None:
             self._name = None
             return
-        if isinstance(value, str):
+        if not isinstance(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, value):
         if value is None:
             self._description = None
             return
-        if isinstance(value, str):
+        if not isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._description = value
 
     @property
     def definition(self):
         return self._definition
 
     @definition.setter
     def definition(self, value):
         if value is None:
             self._definition = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._definition = value
 
     @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, value):
         if value is None:
             self._properties = {}
             return
-        if type(value) != dict:
+        if not isinstance(value, dict):
             raise ValueError('properties should be of type dict!')
         self._properties = value
 
     @property
     def datastreams(self):
         return self._datastreams
 
     @datastreams.setter
     def datastreams(self, value):
         if value is None:
             self._datastreams = None
             return
-        if type(value) == list and all(isinstance(ds, datastream.Datastream) for ds in value):
+        if isinstance(value, list) and all(isinstance(ds, datastream.Datastream) for ds in value):
             entity_class = entity_type.EntityTypes['Datastream']['class']
             self._datastreams = entity_list.EntityList(entity_class=entity_class, entities=value)
             return
-        if type(value) != entity_list.EntityList \
+        if not isinstance(value, entity_list.EntityList) \
                 or any((not isinstance(ds, datastream.Datastream)) for ds in value.entities):
             raise ValueError('datastreams should be of list of type Datastream!')
         self._datastreams = value
 
     @property
     def multi_datastreams(self):
         return self._multi_datastreams
 
     @multi_datastreams.setter
     def multi_datastreams(self, values):
         if values is None:
             self._multi_datastreams = None
             return
-        if type(values) == list and all(isinstance(mds, multi_datastream.MultiDatastream) for mds in values):
+        if isinstance(values, list) and all(isinstance(mds, multi_datastream.MultiDatastream) for mds in values):
             entity_class = entity_type.EntityTypes['MultiDatastream']['class']
             self._multi_datastreams = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or\
+        if not isinstance(values, entity_list.EntityList) or\
                 any((not isinstance(mds, multi_datastream.MultiDatastream)) for mds in values.entities):
             raise ValueError('multi_datastreams should be a list of multi_datastreams!')
         self._multi_datastreams = values
 
     def ensure_service_on_children(self, service):
         if self.datastreams is not None:
             self.datastreams.set_service(service)
@@ -185,18 +185,18 @@
 
     def __setstate__(self, state):
         super().__setstate__(state)
         self.name = state.get("name", None)
         self.description = state.get("description", None)
         self.definition = state.get("definition", None)
         self.properties = state.get("properties", None)
-        if state.get("Datastreams", None) is not None and type(state["Datastreams"]) == list:
+        if state.get("Datastreams", None) is not None and isinstance(state["Datastreams"], list):
             entity_class = entity_type.EntityTypes['Datastream']['class']
             self.datastreams = utils.transform_json_to_entity_list(state['Datastreams'], entity_class)
             self.datastreams.next_link = state.get('Datastreams@iot.nextLink', None)
-        if state.get("MultiDatastreams", None) is not None and type(state["MultiDatastreams"]) == list:
+        if state.get("MultiDatastreams", None) is not None and isinstance(state["MultiDatastreams"], list):
             entity_class = entity_type.EntityTypes['MultiDatastream']['class']
             self.multi_datastreams = utils.transform_json_to_entity_list(state['MultiDatatstreams'], entity_class)
             self.multi_datastreams.next_link = state.get('MultiDatastreams@iot.nextLink', None)
 
     def get_dao(self, service):
         return ObservedPropertyDao(service)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/sensor.py` & `frost_sta_client-1.1.9/frost_sta_client/model/sensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,45 +59,45 @@
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
-        if type(value) != str:
+        if not id(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._description = value
 
     @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, value):
-        if type(value) != dict:
+        if not isinstance(value, dict):
             raise ValueError('properties should be of type dict!')
         self._properties = value
 
     @property
     def encoding_type(self):
         return self._encoding_type
 
     @encoding_type.setter
     def encoding_type(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('encoding_type should be of type str!')
         self._encoding_type = value
 
     @property
     def metadata(self):
         return self._metadata
 
@@ -117,37 +117,37 @@
         return self._datastreams
 
     @datastreams.setter
     def datastreams(self, values):
         if values is None:
             self._datastreams = None
             return
-        if type(values) == list and all(isinstance(ds, datastream.Datastream) for ds in values):
+        if isinstance(values, list) and all(isinstance(ds, datastream.Datastream) for ds in values):
             entity_class = entity_type.EntityTypes['Datastream']['class']
             self._datastreams = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or\
+        if not isinstance(values, entity_list.EntityList) or\
                 any((not isinstance(ds, datastream.Datastream)) for ds in values.entities):
             raise ValueError('datastreams should be an entity list of datastreams!')
         self._datastreams = values
 
     @property
     def multi_datastreams(self):
         return self._multi_datastreams
 
     @multi_datastreams.setter
     def multi_datastreams(self, values):
         if values is None:
             self._multi_datastreams = None
             return
-        if type(values) == list and all(isinstance(mds, multi_datastream.MultiDatastream) for mds in values):
+        if isinstance(values, list) and all(isinstance(mds, multi_datastream.MultiDatastream) for mds in values):
             entity_class = entity_type.EntityTypes['MultiDatastream']['class']
             self._multi_datastreams = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or\
+        if not isinstance(values, entity_list.EntityList) or\
                 any((not isinstance(mds, multi_datastream.MultiDatastream)) for mds in values.entities):
             raise ValueError('multi_datastreams should be a list of multi_datastreams!')
         self._multi_datastreams = values
 
     def ensure_service_on_children(self, service):
         if self.datastreams is not None:
             self.datastreams.set_service(service)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/task.py` & `frost_sta_client-1.1.9/frost_sta_client/model/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     @property
     def tasking_parameters(self):
         return self._tasking_parameters
 
     @tasking_parameters.setter
     def tasking_parameters(self, value):
-        if value is None or type(value) != dict:
+        if value is None or not isinstance(value, dict):
             raise ValueError('tasking parameter should be of type dict!')
         self._tasking_parameters = value
 
     @property
     def creation_time(self):
         return self._creation_time
 
@@ -67,15 +67,15 @@
         return self._tasking_capability
 
     @tasking_capability.setter
     def tasking_capability(self, value):
         if value is None:
             self._tasking_capability = None
             return
-        if type(value) != tasking_capability.TaskingCapability:
+        if not isinstance(value, tasking_capability.TaskingCapability):
             raise ValueError('tasking capability should be of type TaskingCapability!')
         self._tasking_capability = value
 
     def ensure_service_on_children(self, service):
         if self.tasking_capability is not None:
             self.tasking_capability.set_service(service)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/tasking_capability.py` & `frost_sta_client-1.1.9/frost_sta_client/model/tasking_capability.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,93 +60,93 @@
 
     @property
     def name(self):
         return self._name
 
     @name.setter
     def name(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, value):
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._description = value
 
     @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, value):
-        if type(value) != dict:
+        if not isinstance(value, dict):
             raise ValueError('properties should be of type dict!')
         self._properties = value
 
     @property
     def tasking_parameters(self):
         return self._tasking_parameters
 
     @tasking_parameters.setter
     def tasking_parameters(self, value):
         if value is None:
             self._tasking_parameters = {}
             return
-        if type(value) != dict:
+        if not isinstance(value, dict):
             raise ValueError('Tasking parameters should be of type dict!')
         self._tasking_parameters = value
 
     @property
     def tasks(self):
         return self._tasks
 
     @tasks.setter
     def tasks(self, value):
         if value is None:
             self._tasks = None
             return
-        if type(value) == list and all(isinstance(t, frost_sta_client.model.task.Task) for t in value):
+        if not isinstance(value, list) and all(isinstance(t, frost_sta_client.model.task.Task) for t in value):
             entity_class = entity_type.EntityTypes['Task']['class']
             self._tasks = entity_list.EntityList(entity_class=entity_class, entities=value)
             return
-        if type(value) == entity_list.EntityList \
+        if isinstance(value, entity_list.EntityList) \
                 and all(isinstance(t, frost_sta_client.model.task.Task) for t in value.entities):
             self._tasks = value
             return
         raise ValueError('tasks should be of type Task!')
 
     @property
     def thing(self):
         return self._thing
 
     @thing.setter
     def thing(self, value):
         if value is None:
             self._thing = None
             return
-        if type(value) != thing.Thing:
+        if not isinstance(value, thing.Thing):
             raise ValueError('thing should be of type Thing!')
         self._thing = value
 
     @property
     def actuator(self):
         return self._actuator
 
     @actuator.setter
     def actuator(self, value):
         if value is None:
             self._actuator = None
             return
-        if type(value) != actuator.Actuator:
+        if not isinstance(value, actuator.Actuator):
             raise ValueError('actuator should be of type Actuator!')
         self._actuator = value
 
     def ensure_service_on_children(self, service):
         if self.actuator is not None:
             self.actuator.set_service(service)
         if self.thing is not None:
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/model/thing.py` & `frost_sta_client-1.1.9/frost_sta_client/model/thing.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,130 +65,130 @@
         return self._name
 
     @name.setter
     def name(self, value):
         if value is None:
             self._name = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('name should be of type str!')
         self._name = value
 
     @property
     def description(self):
         return self._description
 
     @description.setter
     def description(self, value):
         if value is None:
             self._description = None
             return
-        if type(value) != str:
+        if not isinstance(value, str):
             raise ValueError('description should be of type str!')
         self._description = value
 
     @property
     def properties(self):
         return self._properties
 
     @properties.setter
     def properties(self, value):
         if value is None:
             self._properties = None
             return
-        if type(value) != dict:
+        if not isinstance(value, dict):
             raise ValueError('properties should be of type dict!')
         self._properties = value
 
     @property
     def locations(self):
         return self._locations
 
     @locations.setter
     def locations(self, values):
         if values is None:
             self._locations = None
             return
-        if type(values) == list and all(isinstance(loc, location.Location) for loc in values):
+        if isinstance(values, list) and all(isinstance(loc, location.Location) for loc in values):
             entity_class = entity_type.EntityTypes['Location']['class']
             self._locations = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or \
+        if not isinstance(values, entity_list.EntityList) or \
                 any((not isinstance(loc, location.Location)) for loc in values.entities):
             raise ValueError('locations should be a list of locations')
         self._locations = values
 
     @property
     def historical_locations(self):
         return self._historical_locations
 
     @historical_locations.setter
     def historical_locations(self, values):
         if values is None:
             self._historical_locations = None
             return
-        if type(values) == list and all(isinstance(loc, historical_location.HistoricalLocation) for loc in values):
+        if isinstance(values, list) and all(isinstance(loc, historical_location.HistoricalLocation) for loc in values):
             entity_class = entity_type.EntityTypes['HistoricalLocation']['class']
             self._historical_locations = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or \
+        if not isinstance(values, entity_list.EntityList) or \
                 any((not isinstance(loc, historical_location.HistoricalLocation)) for loc in values.entities):
             raise ValueError('historical_locations should be a list of historical locations')
         self._historical_locations = values
 
     @property
     def datastreams(self):
         return self._datastreams
 
     @datastreams.setter
     def datastreams(self, values):
         if values is None:
             self._datastreams = None
             return
-        if type(values) == list and all(isinstance(ds, datastream.Datastream) for ds in values):
+        if isinstance(values, list) and all(isinstance(ds, datastream.Datastream) for ds in values):
             entity_class = entity_type.EntityTypes['Datastream']['class']
             self._datastreams = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or \
+        if not isinstance(values, entity_list.EntityList) or \
                 any((not isinstance(ds, datastream.Datastream)) for ds in values.entities):
             raise ValueError('datastreams should be a list of datastreams')
         self._datastreams = values
 
     @property
     def multi_datastreams(self):
         return self._multi_datastreams
 
     @multi_datastreams.setter
     def multi_datastreams(self, values):
         if values is None:
             self._multi_datastreams = None
             return
-        if type(values) == list and all(isinstance(ds, multi_datastream.MultiDatastream) for ds in values):
+        if isinstance(values, list) and all(isinstance(ds, multi_datastream.MultiDatastream) for ds in values):
             entity_class = entity_type.EntityTypes['MultiDatastream']['class']
             self._multi_datastreams = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or \
+        if not isinstance(values, entity_list.EntityList) or \
                 any((not isinstance(ds, multi_datastream.MultiDatastream)) for ds in values.entities):
             raise ValueError('Multidatastreams should be a list of MultiDatastreams')
         self._multi_datastreams = values
 
     @property
     def tasking_capabilities(self):
         return self._tasking_capabilities
 
     @tasking_capabilities.setter
     def tasking_capabilities(self, values):
         if values is None:
             self._tasking_capabilities = None
             return
-        if type(values) == list and all(isinstance(tc, tasking_capability.TaskingCapability) for tc in values):
+        if isinstance(values, list) and all(isinstance(tc, tasking_capability.TaskingCapability) for tc in values):
             entity_class = entity_type.EntityTypes['TaskingCapability']['class']
             self._tasking_capabilities = entity_list.EntityList(entity_class=entity_class, entities=values)
             return
-        if type(values) != entity_list.EntityList or \
+        if not isinstance(values, entity_list.EntityList) or \
                 any((not isinstance(tc, tasking_capability.TaskingCapability)) for tc in values.entities):
             raise ValueError('Tasking capabilities should be a list of TaskingCapabilities')
         self._tasking_capabilities = values
 
     def ensure_service_on_children(self, service):
         if self.locations is not None:
             self.locations.set_service(service)
@@ -239,30 +239,30 @@
 
     def __setstate__(self, state):
         super().__setstate__(state)
         self.name = state.get("name", None)
         self.description = state.get("description", None)
         self.properties = state.get("properties", None)
 
-        if state.get("Locations", None) is not None and type(state["Locations"] == list):
+        if state.get("Locations", None) is not None and isinstance(state["Locations"], list):
             entity_class = entity_type.EntityTypes['Location']['class']
             self.locations = utils.transform_json_to_entity_list(state['Locations'], entity_class)
             self.locations.next_link = state.get("Locations@iot.nextLink", None)
-        if state.get("HistoricalLocations", None) is not None and type(state["HistoricalLocations"] == list):
+        if state.get("HistoricalLocations", None) is not None and isinstance(state["HistoricalLocations"], list):
             entity_class = entity_type.EntityTypes['HistoricalLocation']['class']
             self.historical_locations = utils.transform_json_to_entity_list(state['HistoricalLocations'], entity_class)
             self.historical_locations.next_link = state.get("HistoricalLocations@iot.nextLink", None)
-        if state.get("Datastreams", None) is not None and type(state["Datastreams"] == list):
+        if state.get("Datastreams", None) is not None and isinstance(state["Datastreams"], list):
             entity_class = entity_type.EntityTypes['Datastream']['class']
             self.datastreams = utils.transform_json_to_entity_list(state['Datastreams'], entity_class)
             self.datastreams.next_link = state.get("Datastreams@iot.nextLink", None)
-        if state.get("MultiDatastreams", None) is not None and type(state["MultiDatastreams"] == list):
+        if state.get("MultiDatastreams", None) is not None and isinstance(state["MultiDatastreams"], list):
             entity_class = entity_type.EntityTypes['MultiDatastream']['class']
             self.multi_datastreams = utils.transform_json_to_entity_list(state['MultiDatastreams'], entity_class)
             self.multi_datastreams.next_link = state.get("MultiDatastreams@iot.nextLink", None)
-        if state.get("TaskingCapabilities", None) is not None and type(state["TaskingCapabilities"] == list):
+        if state.get("TaskingCapabilities", None) is not None and isinstance(state["TaskingCapabilities"], list):
             entity_class = entity_type.EntityTypes['TaskingCapability']['class']
             self.tasking_capabilities = utils.transform_json_to_entity_list(state['TaskingCapabilities'], entity_class)
             self.tasking_capabilities.next_link = state.get("TaskingCapabilities@iot.nextLink", None)
 
     def get_dao(self, service):
         return ThingDao(service)
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/query/query.py` & `frost_sta_client-1.1.9/frost_sta_client/query/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,37 +45,37 @@
 
     @property
     def entity(self):
         return self._entity
 
     @entity.setter
     def entity(self, value):
-        if value is None or type(value) == str:
+        if value is None or isinstance(value, str):
             self._entity = value
             return
         raise ValueError('entity should be of type String')
 
     @property
     def entitytype_plural(self):
         return self._entitytype_plural
 
     @entitytype_plural.setter
     def entitytype_plural(self, value):
-        if value is None or type(value) == str:
+        if value is None or isinstance(value, str):
             self._entitytype_plural = value
             return
         raise ValueError('entitytype_plural should be of type String')
 
     @property
     def entity_class(self):
         return self._entity_class
 
     @entity_class.setter
     def entity_class(self, value):
-        if value is None or type(value) == str:
+        if value is None or isinstance(value, str):
             self._entity_class = value
             return
         raise ValueError('entity_class should be of type string')
 
     def remove_all_params(self, key):
         self.params.pop(key, None)
 
@@ -96,15 +96,15 @@
 
     def select(self, *args):
         self.remove_all_params('$select')
         if args is None:
             return self
         values = ''
         for item in args:
-            if type(item) != str:
+            if not isinstance(item, str):
                 return self
             values = values + item + ','
         values = values[:-1]
         self.params['$select'] = values
         return self
 
     def filter(self, statement=None):
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client/service/auth_handler.py` & `frost_sta_client-1.1.9/frost_sta_client/service/auth_handler.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/service/sensorthingsservice.py` & `frost_sta_client-1.1.9/frost_sta_client/service/sensorthingsservice.py`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/frost_sta_client/utils.py` & `frost_sta_client-1.1.9/frost_sta_client/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     + jsonpickle.encode(json_response, unpicklable=False) + '}'
     return jsonpickle.decode(decodable_str, backend=demjson3)
 
 
 def transform_json_to_entity_list(json_response, entity_class):
     entity_list = frost_sta_client.model.ext.entity_list.EntityList(entity_class)
     result_list = []
-    if type(json_response) == dict:
+    if isinstance(json_response, dict):
         try:
             response_list = json_response['value']
             entity_list.next_link = json_response.get("@iot.nextLink", None)
         except AttributeError as e:
             raise e
     else:
         response_list = json_response
@@ -52,15 +52,15 @@
     entity_list.entities = result_list
     return entity_list
 
 
 def process_datetime(value):
     if value is None:
         return value
-    if type(value) == str:
+    if isinstance(value, str):
         value = value.replace('Z', '')
         if '/' in value:
             try:
                 times = value.split('/')
                 if len(times) != 2:
                     raise ValueError("If the phenomenon time interval is provided as a string,"
                                      " it should be in isoformat")
@@ -76,24 +76,24 @@
                 result = datetime.datetime.fromisoformat(value)
             except ValueError:
                 raise ValueError("If the phenomenon time is provided as string, it should be in isoformat")
             result = result.isoformat() + 'Z'
             return result
     if value is None:
         return None
-    if type(value) == datetime.datetime:
+    if isinstance(value, datetime.datetime):
         return value.isoformat() + 'Z'
-    if type(value) == list and all(isinstance(v, datetime.datetime) for v in value):
+    if isinstance(value, list) and all(isinstance(v, datetime.datetime) for v in value):
         return value[0].isoformat() + 'Z/' + value[1].isoformat() + 'Z'
     else:
         raise ValueError('phenomenon_time should consist of one or two datetimes')
 
 
 def process_area(value):
-    if type(value) != dict:
+    if not isinstance(value, dict):
         raise ValueError("geojsons can only be handled as dictionaries!")
     if value.get("type", None) is None or value.get("coordinates", None) is None:
         raise ValueError("Both type and coordinates need to be specified in the dictionary")
     if value["type"] == "Point":
         return geojson.geometry.Point(value["coordinates"])
     if value["type"] == "Polygon":
         return geojson.geometry.Polygon(value["coordinates"])
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client.egg-info/PKG-INFO` & `frost_sta_client-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: frost-sta-client
-Version: 1.1.8
+Name: frost_sta_client
+Version: 1.1.9
 Summary: a client library to facilitate interaction with a FROST SensorThingsAPI Server
 Home-page: https://github.com/FraunhoferIOSB/FROST-Python-Client
 Author: Katharina Emde
 Author-email: katharina.emde@iosb.fraunhofer.de
 License: LGPL3
 Keywords: sta,ogc,frost,sensorthingsapi,IoT
 Platform: UNKNOWN
```

### Comparing `frost_sta_client-1.1.8/frost_sta_client.egg-info/SOURCES.txt` & `frost_sta_client-1.1.9/frost_sta_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frost_sta_client-1.1.8/setup.py` & `frost_sta_client-1.1.9/setup.py`

 * *Files identical despite different names*

