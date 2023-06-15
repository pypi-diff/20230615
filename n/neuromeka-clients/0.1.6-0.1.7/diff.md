# Comparing `tmp/neuromeka-clients-0.1.6.tar.gz` & `tmp/neuromeka-clients-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuromeka-clients-0.1.6.tar", last modified: Fri May 12 07:50:19 2023, max compression
+gzip compressed data, was "neuromeka-clients-0.1.7.tar", last modified: Thu Jun 15 09:23:55 2023, max compression
```

## Comparing `neuromeka-clients-0.1.6.tar` & `neuromeka-clients-0.1.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 07:50:19.512108 neuromeka-clients-0.1.6/
--rw-rw-rw-   0        0        0     1076 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     2316 2023-05-12 07:50:19.508124 neuromeka-clients-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-12 07:50:19.361225 neuromeka-clients-0.1.6/neuromeka/
--rw-rw-rw-   0        0        0      246 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/__init__.py
--rw-rw-rw-   0        0        0     7442 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/ecat.py
--rw-rw-rw-   0        0        0    14598 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/eye.py
--rw-rw-rw-   0        0        0    10651 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/indy.py
--rw-rw-rw-   0        0        0    40863 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/indy_client3.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:50:19.367210 neuromeka-clients-0.1.6/neuromeka/indy_dcp/
--rw-rw-rw-   0        0        0        0 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/indy_dcp/__init__.py
--rw-rw-rw-   0        0        0    21703 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/indy_dcp/indy_program_maker.py
--rw-rw-rw-   0        0        0    61482 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/indy_dcp/indydcp_client.py
--rw-rw-rw-   0        0        0     7436 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/moby.py
--rw-rw-rw-   0        0        0     3379 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/motor.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:50:19.473196 neuromeka-clients-0.1.6/neuromeka/proto/
--rw-rw-rw-   0        0        0    65863 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/EtherCATCommgRPCServer_pb2.py
--rw-rw-rw-   0        0        0    61370 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py
--rw-rw-rw-   0        0        0     5567 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/EyeTask_pb2.py
--rw-rw-rw-   0        0        0     6780 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/EyeTask_pb2_grpc.py
--rw-rw-rw-   0        0        0    61466 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/IndygRPCTask_pb2.py
--rw-rw-rw-   0        0        0   128168 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/IndygRPCTask_pb2_grpc.py
--rw-rw-rw-   0        0        0    74574 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/MobygRPCServer_pb2.py
--rw-rw-rw-   0        0        0    52785 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/MobygRPCServer_pb2_grpc.py
--rw-rw-rw-   0        0        0    41733 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/MotorControlgRPCServer_pb2.py
--rw-rw-rw-   0        0        0    39460 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py
--rw-rw-rw-   0        0        0        0 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/__init__.py
--rw-rw-rw-   0        0        0   333650 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/control_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/control_msgs_pb2_grpc.py
--rw-rw-rw-   0        0        0    12892 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/control_pb2.py
--rw-rw-rw-   0        0        0   139890 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/control_pb2_grpc.py
--rw-rw-rw-   0        0        0      519 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/grpc_wrapper.py
--rw-rw-rw-   0        0        0    73456 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/shared_msgs_pb2.py
--rw-rw-rw-   0        0        0      159 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.6/neuromeka/proto/shared_msgs_pb2_grpc.py
-drwxrwxrwx   0        0        0        0 2023-05-12 07:50:19.506123 neuromeka-clients-0.1.6/neuromeka_clients.egg-info/
--rw-rw-rw-   0        0        0     2316 2023-05-12 07:50:19.000000 neuromeka-clients-0.1.6/neuromeka_clients.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1175 2023-05-12 07:50:19.000000 neuromeka-clients-0.1.6/neuromeka_clients.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 07:50:19.000000 neuromeka-clients-0.1.6/neuromeka_clients.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-12 07:50:19.000000 neuromeka-clients-0.1.6/neuromeka_clients.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-12 07:50:19.000000 neuromeka-clients-0.1.6/neuromeka_clients.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-12 07:50:19.512108 neuromeka-clients-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1186 2023-05-12 07:49:27.000000 neuromeka-clients-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:23:55.018514 neuromeka-clients-0.1.7/
+-rw-rw-rw-   0        0        0     1076 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2316 2023-06-15 09:23:55.017252 neuromeka-clients-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 09:23:54.955853 neuromeka-clients-0.1.7/neuromeka/
+-rw-rw-rw-   0        0        0      246 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/__init__.py
+-rw-rw-rw-   0        0        0     7490 2023-06-15 09:21:44.000000 neuromeka-clients-0.1.7/neuromeka/ecat.py
+-rw-rw-rw-   0        0        0    14598 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/eye.py
+-rw-rw-rw-   0        0        0    10651 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/indy.py
+-rw-rw-rw-   0        0        0    40863 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/indy_client3.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:23:54.961890 neuromeka-clients-0.1.7/neuromeka/indy_dcp/
+-rw-rw-rw-   0        0        0        0 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/indy_dcp/__init__.py
+-rw-rw-rw-   0        0        0    21703 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/indy_dcp/indy_program_maker.py
+-rw-rw-rw-   0        0        0    61482 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/indy_dcp/indydcp_client.py
+-rw-rw-rw-   0        0        0     7436 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/moby.py
+-rw-rw-rw-   0        0        0     3379 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/motor.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:23:55.004256 neuromeka-clients-0.1.7/neuromeka/proto/
+-rw-rw-rw-   0        0        0    65863 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/EtherCATCommgRPCServer_pb2.py
+-rw-rw-rw-   0        0        0    61370 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py
+-rw-rw-rw-   0        0        0     5567 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/EyeTask_pb2.py
+-rw-rw-rw-   0        0        0     6780 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/EyeTask_pb2_grpc.py
+-rw-rw-rw-   0        0        0    61466 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/IndygRPCTask_pb2.py
+-rw-rw-rw-   0        0        0   128168 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/IndygRPCTask_pb2_grpc.py
+-rw-rw-rw-   0        0        0    74574 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/MobygRPCServer_pb2.py
+-rw-rw-rw-   0        0        0    52785 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/MobygRPCServer_pb2_grpc.py
+-rw-rw-rw-   0        0        0    41733 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/MotorControlgRPCServer_pb2.py
+-rw-rw-rw-   0        0        0    39460 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py
+-rw-rw-rw-   0        0        0        0 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/__init__.py
+-rw-rw-rw-   0        0        0   333650 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/control_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/control_msgs_pb2_grpc.py
+-rw-rw-rw-   0        0        0    12892 2023-06-15 09:17:54.000000 neuromeka-clients-0.1.7/neuromeka/proto/control_pb2.py
+-rw-rw-rw-   0        0        0   139890 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/control_pb2_grpc.py
+-rw-rw-rw-   0        0        0      519 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/grpc_wrapper.py
+-rw-rw-rw-   0        0        0    73456 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/shared_msgs_pb2.py
+-rw-rw-rw-   0        0        0      159 2023-05-12 07:36:00.000000 neuromeka-clients-0.1.7/neuromeka/proto/shared_msgs_pb2_grpc.py
+drwxrwxrwx   0        0        0        0 2023-06-15 09:23:55.015228 neuromeka-clients-0.1.7/neuromeka_clients.egg-info/
+-rw-rw-rw-   0        0        0     2316 2023-06-15 09:23:54.000000 neuromeka-clients-0.1.7/neuromeka_clients.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1175 2023-06-15 09:23:54.000000 neuromeka-clients-0.1.7/neuromeka_clients.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 09:23:54.000000 neuromeka-clients-0.1.7/neuromeka_clients.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-15 09:23:54.000000 neuromeka-clients-0.1.7/neuromeka_clients.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-15 09:23:54.000000 neuromeka-clients-0.1.7/neuromeka_clients.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 09:23:55.018514 neuromeka-clients-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1186 2023-06-15 09:23:49.000000 neuromeka-clients-0.1.7/setup.py
```

### Comparing `neuromeka-clients-0.1.6/LICENSE` & `neuromeka-clients-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/PKG-INFO` & `neuromeka-clients-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromeka-clients
-Version: 0.1.6
+Version: 0.1.7
 Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients
 Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuromeka-clients-0.1.6/README.md` & `neuromeka-clients-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/ecat.py` & `neuromeka-clients-0.1.7/neuromeka/ecat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 import json
 import grpc
 import math
 
 from .proto.grpc_wrapper import GRPCECatTaskStub
 from .proto.grpc_wrapper import *
+from .proto.EtherCATCommgRPCServer_pb2 import *
 
 
 class EcatClient:
     def __init__(self, step_ip='127.0.0.1'):
         # initialize RPC
         
         self.channel = grpc.insecure_channel('%s:50050'%step_ip)
```

### Comparing `neuromeka-clients-0.1.6/neuromeka/eye.py` & `neuromeka-clients-0.1.7/neuromeka/eye.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/indy.py` & `neuromeka-clients-0.1.7/neuromeka/indy.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/indy_client3.py` & `neuromeka-clients-0.1.7/neuromeka/indy_client3.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/indy_dcp/indy_program_maker.py` & `neuromeka-clients-0.1.7/neuromeka/indy_dcp/indy_program_maker.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/indy_dcp/indydcp_client.py` & `neuromeka-clients-0.1.7/neuromeka/indy_dcp/indydcp_client.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/moby.py` & `neuromeka-clients-0.1.7/neuromeka/moby.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/motor.py` & `neuromeka-clients-0.1.7/neuromeka/motor.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/EtherCATCommgRPCServer_pb2.py` & `neuromeka-clients-0.1.7/neuromeka/proto/EtherCATCommgRPCServer_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py` & `neuromeka-clients-0.1.7/neuromeka/proto/EtherCATCommgRPCServer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/EyeTask_pb2.py` & `neuromeka-clients-0.1.7/neuromeka/proto/EyeTask_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/EyeTask_pb2_grpc.py` & `neuromeka-clients-0.1.7/neuromeka/proto/EyeTask_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/IndygRPCTask_pb2.py` & `neuromeka-clients-0.1.7/neuromeka/proto/IndygRPCTask_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/IndygRPCTask_pb2_grpc.py` & `neuromeka-clients-0.1.7/neuromeka/proto/IndygRPCTask_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/MobygRPCServer_pb2.py` & `neuromeka-clients-0.1.7/neuromeka/proto/MobygRPCServer_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/MobygRPCServer_pb2_grpc.py` & `neuromeka-clients-0.1.7/neuromeka/proto/MobygRPCServer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/MotorControlgRPCServer_pb2.py` & `neuromeka-clients-0.1.7/neuromeka/proto/MotorControlgRPCServer_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py` & `neuromeka-clients-0.1.7/neuromeka/proto/MotorControlgRPCServer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/control_msgs_pb2.py` & `neuromeka-clients-0.1.7/neuromeka/proto/control_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/control_pb2.py` & `neuromeka-clients-0.1.7/neuromeka/proto/control_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/control_pb2_grpc.py` & `neuromeka-clients-0.1.7/neuromeka/proto/control_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/grpc_wrapper.py` & `neuromeka-clients-0.1.7/neuromeka/proto/grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka/proto/shared_msgs_pb2.py` & `neuromeka-clients-0.1.7/neuromeka/proto/shared_msgs_pb2.py`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/neuromeka_clients.egg-info/PKG-INFO` & `neuromeka-clients-0.1.7/neuromeka_clients.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuromeka-clients
-Version: 0.1.6
+Version: 0.1.7
 Summary: Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor
 Home-page: https://github.com/neuromeka-robotics/neuromeka-clients
 Author: Neuromeka
 Author-email: youngjin.heo@neuromeka.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuromeka-clients-0.1.6/neuromeka_clients.egg-info/SOURCES.txt` & `neuromeka-clients-0.1.7/neuromeka_clients.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuromeka-clients-0.1.6/setup.py` & `neuromeka-clients-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="neuromeka-clients",
-    version="0.1.6",
+    version="0.1.7",
     author="Neuromeka",
     author_email="youngjin.heo@neuromeka.com",
     description="Neuromeka client protocols for Indy, IndyEye, Moby, Ecat, and Motor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/neuromeka-robotics/neuromeka-clients",
     packages=find_packages(),
```

