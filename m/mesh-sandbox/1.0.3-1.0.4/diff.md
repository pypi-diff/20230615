# Comparing `tmp/mesh_sandbox-1.0.3-py3-none-any.whl.zip` & `tmp/mesh_sandbox-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -67,12 +67,12 @@
 -rw-r--r--  2.0 unx     1237 b- defN 80-Jan-01 00:00 mesh_sandbox/views/__init__.py
 -rw-r--r--  2.0 unx     1315 b- defN 80-Jan-01 00:00 mesh_sandbox/views/admin.py
 -rw-r--r--  2.0 unx     3885 b- defN 80-Jan-01 00:00 mesh_sandbox/views/error.py
 -rw-r--r--  2.0 unx     5662 b- defN 80-Jan-01 00:00 mesh_sandbox/views/inbox.py
 -rw-r--r--  2.0 unx     2775 b- defN 80-Jan-01 00:00 mesh_sandbox/views/lookup.py
 -rw-r--r--  2.0 unx     4932 b- defN 80-Jan-01 00:00 mesh_sandbox/views/outbox.py
 -rw-r--r--  2.0 unx     8918 b- defN 80-Jan-01 00:00 mesh_sandbox/views/tracking.py
--rw-r--r--  2.0 unx     2428 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx     1051 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     6901 b- defN 16-Jan-01 00:00 mesh_sandbox-1.0.3.dist-info/RECORD
+-rw-r--r--  2.0 unx     2428 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx     1051 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     6901 b- defN 16-Jan-01 00:00 mesh_sandbox-1.0.4.dist-info/RECORD
 76 files, 259441 bytes uncompressed, 67191 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -210,20 +210,20 @@
 
 Filename: mesh_sandbox/views/outbox.py
 Comment: 
 
 Filename: mesh_sandbox/views/tracking.py
 Comment: 
 
-Filename: mesh_sandbox-1.0.3.dist-info/METADATA
+Filename: mesh_sandbox-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: mesh_sandbox-1.0.3.dist-info/LICENSE
+Filename: mesh_sandbox-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: mesh_sandbox-1.0.3.dist-info/WHEEL
+Filename: mesh_sandbox-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: mesh_sandbox-1.0.3.dist-info/RECORD
+Filename: mesh_sandbox-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mesh_sandbox/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.3"
+__version__ = "1.0.4"
```

## Comparing `mesh_sandbox-1.0.3.dist-info/METADATA` & `mesh_sandbox-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesh-sandbox
-Version: 1.0.3
+Version: 1.0.4
 Summary: NHSDigital mesh sandbox, a locally testable version of the MESH api
 License: MIT
 Author: spinecore
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

## Comparing `mesh_sandbox-1.0.3.dist-info/LICENSE` & `mesh_sandbox-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mesh_sandbox-1.0.3.dist-info/RECORD` & `mesh_sandbox-1.0.4.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-mesh_sandbox/__init__.py,sha256=2plzdEEb24FLjE2I2XyBBcJEPYWHccNL4SgtLC_6erg,22
+mesh_sandbox/__init__.py,sha256=acuR_XSJzp4OrQ5T8-Ac5gYe48mUwObuwjRmisFmZ7k,22
 mesh_sandbox/api.py,sha256=F2KUKENAsSe6NAGG0wzHA2jebGF6mWFgta1q55oqacU,3925
 mesh_sandbox/common/__init__.py,sha256=MwKS4FixADUGgN49MQJI7vW0Wx6mnf9SBOPbgE4RddM,3403
 mesh_sandbox/common/constants.py,sha256=_hnaHDkAQGHWLF7n_WfC5ZHIY5D-fUbOdpSqLusUMNY,6504
 mesh_sandbox/common/exceptions.py,sha256=YQII8w6DQQoKuW0cukEr6PIE9j0rwrqDpCn5lapgmkQ,1481
 mesh_sandbox/common/fernet.py,sha256=f8yygkVnK1cmQLBgcPifoB4PwGpgiOrG8Yk-6OMDy8o,551
 mesh_sandbox/common/handler_helpers.py,sha256=Eg00Tide2mL87EoMFw83fDuxiTL5DgIwxHs2RaJasgE,392
 mesh_sandbox/common/messaging.py,sha256=xZbNpWQLhfjI4wiBG3PpIkEy2WbvwxqaWSR90sSb4hk,14664
@@ -66,11 +66,11 @@
 mesh_sandbox/views/__init__.py,sha256=nZkb6_1S8jz8Xl_AayfwjgEZG0JD2dfulfGxjJ5W9Ec,1237
 mesh_sandbox/views/admin.py,sha256=2YGslfDyC0QKoq3WTGXBicqrOMR9UmQYocP3R0qTbAY,1315
 mesh_sandbox/views/error.py,sha256=9lnUr3P93Vm-nOrBTEuAD6nrSBUvpI6-XqXzILWjgGk,3885
 mesh_sandbox/views/inbox.py,sha256=gnaD9Csx5BqilVRefQQ_tXmeq80lwcLJfepW005GrkU,5662
 mesh_sandbox/views/lookup.py,sha256=HHUqZ-Iy22ysC3qaO8Bl5GBQqf_7IiBbe5acyxqS78M,2775
 mesh_sandbox/views/outbox.py,sha256=jxYiHylEdpljZ6Wl45Ke3aaH5rEKb-kzUuCNEKDS3So,4932
 mesh_sandbox/views/tracking.py,sha256=1H7Ghcvqkmx__KS1Y-lm105EVx_Z1eJo3oMDh8pzRMQ,8918
-mesh_sandbox-1.0.3.dist-info/METADATA,sha256=0RJSlRuPU88gf77vJIj1NoqnqZBmg1aHGwR7V59pisA,2428
-mesh_sandbox-1.0.3.dist-info/LICENSE,sha256=usgzIvDUpVX5pYZepJTRXQJqIaz0mdd32GuS5a3PFlY,1051
-mesh_sandbox-1.0.3.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-mesh_sandbox-1.0.3.dist-info/RECORD,,
+mesh_sandbox-1.0.4.dist-info/METADATA,sha256=Wh9gYotOc1wzMnqO-Kf-WUzTFko6JEQyM1sXnttQ72g,2428
+mesh_sandbox-1.0.4.dist-info/LICENSE,sha256=usgzIvDUpVX5pYZepJTRXQJqIaz0mdd32GuS5a3PFlY,1051
+mesh_sandbox-1.0.4.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+mesh_sandbox-1.0.4.dist-info/RECORD,,
```

