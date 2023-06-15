# Comparing `tmp/authzed-0.8.0.tar.gz` & `tmp/authzed-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authzed-0.8.0.tar", max compression
+gzip compressed data, was "authzed-0.9.0.tar", max compression
```

## Comparing `authzed-0.8.0.tar` & `authzed-0.9.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2023-03-13 21:17:12.988382 authzed-0.8.0/LICENSE
--rw-r--r--   0        0        0     3973 2023-03-13 21:17:12.988382 authzed-0.8.0/README.md
--rw-r--r--   0        0        0     4245 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v0/core_pb2.py
--rw-r--r--   0        0        0     3854 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v0/core_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v0/core_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v0/core_pb2_grpc.pyi
--rw-r--r--   0        0        0     7771 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v0/developer_pb2.py
--rw-r--r--   0        0        0    17350 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v0/developer_pb2.pyi
--rw-r--r--   0        0        0    11293 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v0/developer_pb2_grpc.py
--rw-r--r--   0        0        0     2717 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v0/developer_pb2_grpc.pyi
--rw-r--r--   0        0        0     2720 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/__init__.py
--rw-r--r--   0        0        0     8107 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/core_pb2.py
--rw-r--r--   0        0        0    12510 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/core_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/core_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/core_pb2_grpc.pyi
--rw-r--r--   0        0        0     4070 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/debug_pb2.py
--rw-r--r--   0        0        0     7254 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/debug_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/debug_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/debug_pb2_grpc.pyi
--rw-r--r--   0        0        0     1960 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/error_reason_pb2.py
--rw-r--r--   0        0        0    12238 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/error_reason_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/error_reason_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/error_reason_pb2_grpc.pyi
--rw-r--r--   0        0        0     2091 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/openapi_pb2.py
--rw-r--r--   0        0        0      165 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/openapi_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/openapi_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/openapi_pb2_grpc.pyi
--rw-r--r--   0        0        0    24558 2023-03-13 21:17:12.988382 authzed-0.8.0/authzed/api/v1/permission_service_pb2.py
--rw-r--r--   0        0        0    35426 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/permission_service_pb2.pyi
--rw-r--r--   0        0        0    15215 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/permission_service_pb2_grpc.py
--rw-r--r--   0        0        0     6715 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/permission_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2850 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/schema_service_pb2.py
--rw-r--r--   0        0        0     2257 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/schema_service_pb2.pyi
--rw-r--r--   0        0        0     4769 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/schema_service_pb2_grpc.py
--rw-r--r--   0        0        0     2010 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/schema_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     2769 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/watch_service_pb2.py
--rw-r--r--   0        0        0     2879 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/watch_service_pb2.pyi
--rw-r--r--   0        0        0     2676 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/watch_service_pb2_grpc.py
--rw-r--r--   0        0        0      806 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1/watch_service_pb2_grpc.pyi
--rw-r--r--   0        0        0     3178 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1alpha1/schema_pb2.py
--rw-r--r--   0        0        0     4784 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1alpha1/schema_pb2.pyi
--rw-r--r--   0        0        0     4874 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1alpha1/schema_pb2_grpc.py
--rw-r--r--   0        0        0     2234 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1alpha1/schema_pb2_grpc.pyi
--rw-r--r--   0        0        0     4203 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1alpha1/watchresources_service_pb2.py
--rw-r--r--   0        0        0     6235 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1alpha1/watchresources_service_pb2.pyi
--rw-r--r--   0        0        0     3343 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1alpha1/watchresources_service_pb2_grpc.py
--rw-r--r--   0        0        0     1567 2023-03-13 21:17:12.992382 authzed-0.8.0/authzed/api/v1alpha1/watchresources_service_pb2_grpc.pyi
--rw-r--r--   0        0        0      739 2023-03-13 21:17:12.992382 authzed-0.8.0/grpcutil/__init__.py
--rw-r--r--   0        0        0     1173 2023-03-13 21:17:12.992382 authzed-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      264 2023-03-13 21:17:12.992382 authzed-0.8.0/validate/README.md
--rw-r--r--   0        0        0    15279 2023-03-13 21:17:12.992382 authzed-0.8.0/validate/validate_pb2.py
--rw-r--r--   0        0        0    64652 2023-03-13 21:17:12.992382 authzed-0.8.0/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-03-13 21:17:12.992382 authzed-0.8.0/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-03-13 21:17:12.992382 authzed-0.8.0/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0     4841 1970-01-01 00:00:00.000000 authzed-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-09 14:05:54.001886 authzed-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3973 2023-05-09 14:05:54.001886 authzed-0.9.0/README.md
+-rw-r--r--   0        0        0     4245 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v0/core_pb2.py
+-rw-r--r--   0        0        0     3854 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v0/core_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v0/core_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v0/core_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7771 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v0/developer_pb2.py
+-rw-r--r--   0        0        0    17350 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v0/developer_pb2.pyi
+-rw-r--r--   0        0        0    11293 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v0/developer_pb2_grpc.py
+-rw-r--r--   0        0        0     2717 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v0/developer_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2720 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v1/__init__.py
+-rw-r--r--   0        0        0     8107 2023-05-09 14:05:54.001886 authzed-0.9.0/authzed/api/v1/core_pb2.py
+-rw-r--r--   0        0        0    12510 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/core_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/core_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/core_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4070 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/debug_pb2.py
+-rw-r--r--   0        0        0     7254 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/debug_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/debug_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/debug_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1960 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/error_reason_pb2.py
+-rw-r--r--   0        0        0    12238 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/error_reason_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/error_reason_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/error_reason_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2091 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/openapi_pb2.py
+-rw-r--r--   0        0        0      165 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/openapi_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/openapi_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/openapi_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24558 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/permission_service_pb2.py
+-rw-r--r--   0        0        0    35426 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/permission_service_pb2.pyi
+-rw-r--r--   0        0        0    15215 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/permission_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6715 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/permission_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2850 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/schema_service_pb2.py
+-rw-r--r--   0        0        0     2257 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/schema_service_pb2.pyi
+-rw-r--r--   0        0        0     4769 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/schema_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2010 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/schema_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2769 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/watch_service_pb2.py
+-rw-r--r--   0        0        0     2879 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/watch_service_pb2.pyi
+-rw-r--r--   0        0        0     2676 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/watch_service_pb2_grpc.py
+-rw-r--r--   0        0        0      806 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1/watch_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3178 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1alpha1/schema_pb2.py
+-rw-r--r--   0        0        0     4784 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1alpha1/schema_pb2.pyi
+-rw-r--r--   0        0        0     4874 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1alpha1/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     2234 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1alpha1/schema_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4203 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1alpha1/watchresources_service_pb2.py
+-rw-r--r--   0        0        0     6235 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1alpha1/watchresources_service_pb2.pyi
+-rw-r--r--   0        0        0     3343 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1alpha1/watchresources_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1567 2023-05-09 14:05:54.005886 authzed-0.9.0/authzed/api/v1alpha1/watchresources_service_pb2_grpc.pyi
+-rw-r--r--   0        0        0      739 2023-05-09 14:05:54.005886 authzed-0.9.0/grpcutil/__init__.py
+-rw-r--r--   0        0        0     1170 2023-05-09 14:05:54.009886 authzed-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      264 2023-05-09 14:05:54.009886 authzed-0.9.0/validate/README.md
+-rw-r--r--   0        0        0    15279 2023-05-09 14:05:54.009886 authzed-0.9.0/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64652 2023-05-09 14:05:54.009886 authzed-0.9.0/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-09 14:05:54.009886 authzed-0.9.0/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-09 14:05:54.009886 authzed-0.9.0/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4829 1970-01-01 00:00:00.000000 authzed-0.9.0/PKG-INFO
```

### Comparing `authzed-0.8.0/LICENSE` & `authzed-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/README.md` & `authzed-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v0/core_pb2.py` & `authzed-0.9.0/authzed/api/v0/core_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v0/core_pb2.pyi` & `authzed-0.9.0/authzed/api/v0/core_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v0/developer_pb2.py` & `authzed-0.9.0/authzed/api/v0/developer_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v0/developer_pb2.pyi` & `authzed-0.9.0/authzed/api/v0/developer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v0/developer_pb2_grpc.py` & `authzed-0.9.0/authzed/api/v0/developer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v0/developer_pb2_grpc.pyi` & `authzed-0.9.0/authzed/api/v0/developer_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/__init__.py` & `authzed-0.9.0/authzed/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/core_pb2.py` & `authzed-0.9.0/authzed/api/v1/core_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/core_pb2.pyi` & `authzed-0.9.0/authzed/api/v1/core_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/debug_pb2.py` & `authzed-0.9.0/authzed/api/v1/debug_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/debug_pb2.pyi` & `authzed-0.9.0/authzed/api/v1/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/error_reason_pb2.py` & `authzed-0.9.0/authzed/api/v1/error_reason_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/error_reason_pb2.pyi` & `authzed-0.9.0/authzed/api/v1/error_reason_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/openapi_pb2.py` & `authzed-0.9.0/authzed/api/v1/openapi_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/permission_service_pb2.py` & `authzed-0.9.0/authzed/api/v1/permission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/permission_service_pb2.pyi` & `authzed-0.9.0/authzed/api/v1/permission_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/permission_service_pb2_grpc.py` & `authzed-0.9.0/authzed/api/v1/permission_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/permission_service_pb2_grpc.pyi` & `authzed-0.9.0/authzed/api/v1/permission_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/schema_service_pb2.py` & `authzed-0.9.0/authzed/api/v1/schema_service_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/schema_service_pb2.pyi` & `authzed-0.9.0/authzed/api/v1/schema_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/schema_service_pb2_grpc.py` & `authzed-0.9.0/authzed/api/v1/schema_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/schema_service_pb2_grpc.pyi` & `authzed-0.9.0/authzed/api/v1/schema_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/watch_service_pb2.py` & `authzed-0.9.0/authzed/api/v1/watch_service_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/watch_service_pb2.pyi` & `authzed-0.9.0/authzed/api/v1/watch_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/watch_service_pb2_grpc.py` & `authzed-0.9.0/authzed/api/v1/watch_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1/watch_service_pb2_grpc.pyi` & `authzed-0.9.0/authzed/api/v1/watch_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1alpha1/schema_pb2.py` & `authzed-0.9.0/authzed/api/v1alpha1/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1alpha1/schema_pb2.pyi` & `authzed-0.9.0/authzed/api/v1alpha1/schema_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1alpha1/schema_pb2_grpc.py` & `authzed-0.9.0/authzed/api/v1alpha1/schema_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1alpha1/schema_pb2_grpc.pyi` & `authzed-0.9.0/authzed/api/v1alpha1/schema_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1alpha1/watchresources_service_pb2.py` & `authzed-0.9.0/authzed/api/v1alpha1/watchresources_service_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1alpha1/watchresources_service_pb2.pyi` & `authzed-0.9.0/authzed/api/v1alpha1/watchresources_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1alpha1/watchresources_service_pb2_grpc.py` & `authzed-0.9.0/authzed/api/v1alpha1/watchresources_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/authzed/api/v1alpha1/watchresources_service_pb2_grpc.pyi` & `authzed-0.9.0/authzed/api/v1alpha1/watchresources_service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/grpcutil/__init__.py` & `authzed-0.9.0/grpcutil/__init__.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/pyproject.toml` & `authzed-0.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [tool.poetry]
 authors = ["Authzed <support@authzed.com>"]
-description = "Client library for the Authzed service."
+description = "Client library for SpiceDB."
 name = "authzed"
 packages = [
   {include = "authzed"},
   {include = "validate"},
   {include = "grpcutil"},
 ]
 readme = "README.md"
-version = "0.8.0"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
 async_generator = "^1.10"
 google-api-core = "^2.4.0"
 google_api = "^0.1.12"
-grpcio = "~1.51"
+grpcio = "^1.54"
 mock = "^4.0.3"
 protobuf = "~4.21"
-protoc-gen-validate = "^0.4.1"
+protoc-gen-validate = ">=0.4.1,<0.11.0"
 python = "^3.7"
 typing-extensions = ">=3.7.4,<5"
 
 [tool.poetry.dev-dependencies]
-black = "^22.8.0"
+black = "^23.3.0"
 grpcio-tools = "~1.51"
 isort = "^5.6.4"
 jedi = "0.17.2"
 mypy = "1.0.1"
 mypy-protobuf = "3.3.0"
 parso = "0.7.1"
-pyflakes = "^2.2.0"
+pyflakes = "^3.0.1"
 pytest = "^7.1.3"
-pytest-asyncio = "^0.19.0"
+pytest-asyncio = "^0.21.0"
 python-language-server = "^0.36.2"
 
 [tool.black]
 exclude = '(^\.(.*)|^(.*)_pb2(_grpc)?\.py)'
 line-length = 100
 
 [tool.pytest.ini_options]
```

### Comparing `authzed-0.8.0/validate/validate_pb2.py` & `authzed-0.9.0/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/validate/validate_pb2.pyi` & `authzed-0.9.0/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `authzed-0.8.0/PKG-INFO` & `authzed-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: authzed
-Version: 0.8.0
-Summary: Client library for the Authzed service.
+Version: 0.9.0
+Summary: Client library for SpiceDB.
 Author: Authzed
 Author-email: support@authzed.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: async_generator (>=1.10,<2.0)
 Requires-Dist: google-api-core (>=2.4.0,<3.0.0)
 Requires-Dist: google_api (>=0.1.12,<0.2.0)
-Requires-Dist: grpcio (>=1.51,<1.52)
+Requires-Dist: grpcio (>=1.54,<2.0)
 Requires-Dist: mock (>=4.0.3,<5.0.0)
 Requires-Dist: protobuf (>=4.21,<4.22)
-Requires-Dist: protoc-gen-validate (>=0.4.1,<0.5.0)
+Requires-Dist: protoc-gen-validate (>=0.4.1,<0.11.0)
 Requires-Dist: typing-extensions (>=3.7.4,<5)
 Description-Content-Type: text/markdown
 
 # Authzed Python Client
 
 [![PyPI](https://img.shields.io/pypi/v/authzed?color=%23006dad)](https://pypi.org/project/authzed)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)
```

